---
title: datatypes/time_series.hpp

---

# datatypes/time_series.hpp



## Namespaces

| Name           |
| -------------- |
| **[datatypes](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes/)**  |
| **[datatypes::timeseries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/)**  |
| **[datatypes::exceptions](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1exceptions/)**  |

## Classes

|                | Name           |
| -------------- | -------------- |
| struct | **[datatypes::timeseries::DefaultMissingValuePolicyTypeFactory](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1DefaultMissingValuePolicyTypeFactory/)**  |
| class | **[datatypes::timeseries::TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)** <br>A template for univariate, single realisasion time series.  |
| class | **[datatypes::timeseries::MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)** <br>Template for time series with multiple values at time point; e.g. to hold multiple realizations of time series in an ensemble.  |
| struct | **[datatypes::timeseries::time_series_of](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1time__series__of/)**  |
| struct | **[datatypes::timeseries::ensemble_of](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1ensemble__of/)**  |
| struct | **[datatypes::timeseries::item_type_of](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1item__type__of/)**  |
| struct | **[datatypes::timeseries::CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)** <br>Typical ensemble and time series data types derived from a fundamental data type for each data item.  |
| class | **[datatypes::timeseries::TimeSeriesOperations](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/)**  |
| class | **[datatypes::timeseries::TimeWindow](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeWindow/)** <br>An object that represents a time window, defining subset/trim operations on time series.  |
| class | **[datatypes::exceptions::TimeSeriesChecks](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1exceptions_1_1TimeSeriesChecks/)**  |




## Source code

```cpp
#pragma once


#include <iterator>
#include "boost/date_time/posix_time/posix_time.hpp"
#include <boost/function.hpp>
#include "datatypes/common.h"
#include "datatypes/time_step.h"
#include "datatypes/time_series_strategies.hpp"
#include "datatypes/exception_utilities.h"
#include "cinterop/common_c_interop.h"


using namespace boost::posix_time;
using namespace boost::gregorian;

using namespace datatypes::utils;

namespace datatypes
{
    namespace timeseries
    {

        template <typename T>
        struct DefaultMissingValuePolicyTypeFactory {
            typedef typename IfThenElse<
                std::is_pointer<T>::value, 
                NullPointerIsMissingPolicy<T>, 
                DefaultMissingFloatingPointPolicy<T>>::ResultT type;
        };
        
        template <typename T>
        MissingValuePolicy<T>* DefaultMissingValuePolicy() 
        {
            using U = typename DefaultMissingValuePolicyTypeFactory<T>::type;
            return new U();
        }
/*
        template <typename T>
        std::enable_if_t<std::is_pointer<T>::value, MissingValuePolicy<T>*>
            DefaultMissingValuePolicy() { return new NullPointerIsMissingPolicy<T>(); }
        template <typename T>
        std::enable_if_t<!std::is_pointer<T>::value, MissingValuePolicy<T>*>
            DefaultMissingValuePolicy() { return new DefaultMissingFloatingPointPolicy<T>(); }
*/

        template <typename T>
        StoragePolicy<T>* DefaultStoragePolicy() { return new StlVectorStorage<T>(); }

        template <typename T = double>
        class TTimeSeries
        {
        public:
            using ElementType = T;
        private:
            StoragePolicy<T>* storage = nullptr;
            MissingValuePolicy<T>* mvp = nullptr;

            void CheckConstructorReadonly()
            {
                if (this->storage->ReadOnly())
                    datatypes::exceptions::ExceptionUtilities::ThrowInvalidOperation("The storage for this time series is marked as read-only; there may be inconsistencies");
            }

        protected:

            inline T GetNACode() const { return this->mvp->GetMissingValue(); }

        public:

            inline bool IsMissingValue(const T& value) const { return this->mvp->IsMissingValue(value); }

            inline T GetMissingValue() const { return this->mvp->GetMissingValue(); }

            TTimeSeries(StoragePolicy<T>* storage = nullptr, MissingValuePolicy<T>* mvp = nullptr)
            {
                SetDefaults(storage, mvp);
                if (!this->storage->ReadOnly())
                    Reset(0, not_a_date_time);
                instances++;
            }

            TTimeSeries(T default_value, size_t length, const ptime& startDate, const TimeStep& timeStep = TimeStep::GetHourly(), StoragePolicy<T>* storage = nullptr, MissingValuePolicy<T>* mvp = nullptr)
            {
                SetDefaults(storage, mvp);
                CheckConstructorReadonly();
                this->storage->SetTimeStep(timeStep);
                Reset(length, startDate, default_value);
                instances++;
            }

            TTimeSeries(size_t length, const ptime& startDate, const TimeStep& timeStep = TimeStep::GetHourly(), StoragePolicy<T>* storage = nullptr, MissingValuePolicy<T>* mvp = nullptr)
            {
                SetDefaults(storage, mvp);
                CheckConstructorReadonly();
                this->storage->SetTimeStep(timeStep);
                Reset(length, startDate, this->mvp->GetMissingValue());
                instances++;
            }

            TTimeSeries(const vector<T>& values, const ptime& startDate, const TimeStep& timeStep = TimeStep::GetHourly(), StoragePolicy<T>* storage = nullptr, MissingValuePolicy<T>* mvp = nullptr)
            {
                SetDefaults(storage, mvp);
                CheckConstructorReadonly();
                this->storage->SetTimeStep(timeStep);
                Reset(values, startDate);
                instances++;
            }

            TTimeSeries(const T * values, size_t length, const ptime& startDate, const TimeStep& timeStep = TimeStep::GetHourly(), StoragePolicy<T>* storage = nullptr, MissingValuePolicy<T>* mvp = nullptr)
            {
                SetDefaults(storage, mvp);
                CheckConstructorReadonly();
                this->storage->SetTimeStep(timeStep);
                Reset(length, startDate, values);
                instances++;
            }

            // This constructor is initially intended only as a convenience for testing purposes.
            TTimeSeries(std::function<T(size_t)>& valueGen, size_t length, const ptime& startDate, const TimeStep& timeStep = TimeStep::GetHourly(), StoragePolicy<T>* storage = nullptr, MissingValuePolicy<T>* mvp = nullptr)
            {
                SetDefaults(storage, mvp);
                CheckConstructorReadonly();
                this->storage->SetTimeStep(timeStep);
                vector<T> values(length);
                for (size_t i = 0; i < length; i++)
                    values[i] = valueGen(i);
                Reset(values, startDate);
                instances++;
            }

            TTimeSeries(const TTimeSeries<T>& src) {   // (Deep) Copy constructor.
                *this = src;
                instances++;
            }

            TTimeSeries(const TTimeSeries<T>& src, StoragePolicy<T>* storage) {   // (Deep) Copy constructor.
                Tag = src.Tag;
                mvp = src.mvp->Clone();
                this->storage = (storage == nullptr) ? DefaultStoragePolicy<T>() : storage;
                src.storage->CopyTo(*(this->storage));
                instances++;
            }

            TTimeSeries(const TTimeSeries<T>* src) {   // (Deep) Copy constructor.
                *this = *src;
                instances++;
            }

            TTimeSeries(TTimeSeries<T>&& src) {   // Move constructor.
                *this = std::move(src);
                instances++;
            }

            TTimeSeries<T>& operator=(TTimeSeries<T>&& src){
                // Avoid self assignment
                if (&src == this){
                    return *this;
                }
                std::swap(Tag, src.Tag);
                std::swap(storage, src.storage);
                std::swap(mvp, src.mvp);
                return *this;
            }

            TTimeSeries<T>& operator=(const TTimeSeries<T>& src)
            {
                if (&src == this){
                    return *this;
                }
                DeepCopyFrom(src);
                return *this;
            }

            virtual ~TTimeSeries()
            {
                if (storage != nullptr)
                    delete storage;
                if (mvp != nullptr)
                    delete mvp;
                instances--;
            }

            T GetValueNoConst(const size_t& index)
            {
                if (index < 0 || index >= GetLength())
                    datatypes::exceptions::ExceptionUtilities::ThrowOutOfRange("Trying to access a time series value with an index outside of its bounds");
                return storage->operator[](index);
            }

            const T& GetValueConst(const size_t& index) const {
                if (index < 0 || index >= GetLength())
                    datatypes::exceptions::ExceptionUtilities::ThrowOutOfRange("Trying to access a time series value with an index outside of its bounds");
                return storage->operator[](index);
            }

            T GetValue(const size_t& index)
            {
                return GetValueNoConst(index);
            }

            const T& GetValue(const size_t& index) const {
                return GetValueConst(index);
            }

            T GetValueNoConst(const ptime& instant)
            {
                return GetValueNoConst(IndexForTime(instant));
            }

            T GetValue(const ptime& instant)
            {
                return GetValueNoConst(IndexForTime(instant));
            }

            const T& GetValue(const ptime& instant) const
            {
                const size_t index = IndexForTime(instant);
                return GetValue(index);
            }

            T GetLastValue()
            {
                size_t length = GetLength();
                if (length == 0)
                    datatypes::exceptions::ExceptionUtilities::ThrowOutOfRange("TimeSeries::GetLastValue cannot be called on an empty time series");
                size_t index = length - 1;
                return GetValue(index);
            }

            void CopyTo(T * dest, size_t from = 0, size_t to = -1) const
            {
                CheckIntervalBounds(from, to);
                UncheckedCopyTo(dest, from, to);
            }

            void CopyWithMissingValueTo(T * dest, const T& missingValueValue, size_t from = 0, size_t to = -1) const
            {
                CheckIntervalBounds(from, to);
                UncheckedCopyTo(dest, from, to, missingValueValue);
            }

            void CopyValues(const TTimeSeries<T>& src)
            {
                if (GetTimeStep() != src.GetTimeStep())
                    datatypes::exceptions::ExceptionUtilities::ThrowInvalidOperation("time series copy values is only for identical time steps");
                size_t from = IndexForTime(src.GetStartDate());
                size_t to = IndexForTime(src.GetEndDate());
                CheckIntervalBounds(from, to);
                for (size_t i = from; i <= to; i++)
                {
                    T val = src.GetValue(i - from);
                    this->SetValue(i, (src.IsMissingValue(val) ? GetMissingValue() : val));
                }
            }

            void CopyTo(vector<T>& dest, size_t from = 0, size_t to = -1) const
            {
                CheckIntervalBounds(from, to);
                storage->CopyTo(dest, from, to);
            }

            T * GetValues(size_t from = 0, size_t to = std::numeric_limits<size_t>::max()) const
            {
                CheckIntervalBounds(from, to);
                size_t len = (to - from) + 1;
                T * values = new T[len];
                this->UncheckedCopyTo(values, from, to);
                return values;
            }

            vector<T> GetValuesVector(size_t from = 0, size_t to = std::numeric_limits<size_t>::max()) const
            {
                CheckIntervalBounds(from, to);
                vector<T> values;
                this->CopyTo(values, from, to);
                return values;
            }

            TTimeSeries<T> Subset(size_t from = 0, size_t to = std::numeric_limits<size_t>::max()) const
            {
                CheckIntervalBounds(from, to);
                size_t len = (to - from) + 1;
                T * values = GetValues(from, to);
                // TODO: consider what to do with storage policy. MVP makes sense to keep the same.
                auto res = TTimeSeries<T>(values, len, TimeForIndex(from), GetTimeStep(), nullptr, mvp->Clone());
                delete[] values;
                return res;
            }

            void SetValue(size_t index, T value)
            {
                storage->operator[](index) = value;
            }

            void SetValue(const ptime& instant, T value)
            {
                SetValue(IndexForTime(instant), value);
            }

            void Reset(size_t length, const ptime& startDate, const TimeStep& timeStep)
            {
                this->storage->SetStart(startDate);
                this->storage->SetTimeStep(timeStep);
                this->storage->Allocate(length, mvp->GetMissingValue());
            }

            void Reset(size_t length, const ptime& startDate, const T * values = nullptr)
            {
                if (values == nullptr)
                    this->storage->Allocate(length, mvp->GetMissingValue());
                else
                    this->storage->AllocateValues(length, values);
                this->storage->SetStart(startDate);
            }

            void Reset(size_t length, const ptime& startDate, T value)
            {
                this->storage->Allocate(length, value);
                this->storage->SetStart(startDate);
            }

            void Reset(const vector<T>& values, const ptime& startDate)
            {
                this->storage->AllocateValues(values);
                this->storage->SetStart(startDate);
            }

            void Reset(const vector<T>& values, const ptime& startDate, const TimeStep& timeStep)
            {
                this->storage->AllocateValues(values);
                this->storage->SetStart(startDate);
                this->storage->SetTimeStep(timeStep);
            }

            size_t GetLength() const
            {
                return storage->Size();
            }

            ptime GetStartDate() const
            {
                return storage->GetStart();
            }

            ptime GetEndDate() const
            {
                size_t n = GetLength();
                if (n == 0) return GetStartDate(); // what else?
                else
                    return GetTimeStep().AddSteps(GetStartDate(), n-1);
            }

            TimeStep GetTimeStep() const
            {
                return storage->GetTimeStep();
            }

            void SetTimeStep(const TimeStep& timeStep)
            {
                this->storage->SetTimeStep(timeStep);
            }

            void SetStartDate(const ptime& start)
            {
                this->storage->SetStart(start);
            }

            ptime TimeForIndex(size_t timeIndex) const
            {
                return GetTimeStep().AddSteps(this->GetStartDate(), timeIndex);
            }

            vector<ptime> TimeIndices() const
            {
                auto tstep = GetTimeStep();
                return tstep.AddSteps(this->GetStartDate(), SeqVec<double>(0, 1, GetLength()));
            }

            size_t IndexForTime(const ptime& instant) const {
                return LowerIndexForTime(instant);
            }

            size_t UpperIndexForTime(const ptime& instant) const
            {
                auto uIndex = GetTimeStep().GetUpperNumSteps(GetStartDate(), instant) - 1;
                datatypes::exceptions::ExceptionUtilities::CheckInRange<ptrdiff_t>(uIndex, 0, GetLength() - 1, "UpperIndexForTime");
                return (size_t)uIndex;
            }

            size_t LowerIndexForTime(const ptime& instant) const
            {
                auto uIndex = GetTimeStep().GetNumSteps(GetStartDate(), instant) - 1;
                datatypes::exceptions::ExceptionUtilities::CheckInRange<ptrdiff_t>(uIndex, 0, GetLength() - 1, "LowerIndexForTime");
                return (size_t)uIndex;
            }

            string GetSummary() const
            {
                string result = "[" + to_iso_extended_string(GetStartDate()) + "/" + to_iso_extended_string(GetEndDate()) + "];length=" +
                    std::to_string(GetLength()) + ";time step=" + GetTimeStep().GetName();
                return result;
            }

            T& operator[](const ptime& instant) {
                return storage->operator[](IndexForTime(instant));
            }

            T& operator[](const size_t i) {
                return storage->operator[](i);
            }

            const T& operator[](const ptime& instant) const {
                return this->operator[](IndexForTime(instant));
            }

            const T& operator[](const size_t i) const {
                return storage->operator[](i);
            }

            TTimeSeries<T> operator+(const TTimeSeries<T>& rhs) const
            {
                // TODO check geometry compatibility
                T a, b;
                T na = this->mvp->GetMissingValue();
                size_t length = rhs.GetLength();
                TTimeSeries<T> ts(na, length, GetStartDate(), GetTimeStep(), nullptr, mvp->Clone());
                //ts.naCode = this->naCode;
                for (size_t i = 0; i < length; i++)
                {
                    a = this->operator[](i);
                    b = rhs.operator[](i);
                    if (IsMissingValue(a) || rhs.IsMissingValue(b))
                        ts.operator[](i) = ts.GetNACode();
                    else
                        ts.operator[](i) = a + b;
                }
                return ts;
            }

            TTimeSeries<T> operator+(T value) const
            {
                T a;
                T na = this->mvp->GetMissingValue();
                size_t length = this->GetLength();
                TTimeSeries<T> ts(na, length, GetStartDate(), GetTimeStep(), nullptr, mvp->Clone());
                for (size_t i = 0; i < length; i++)
                {
                    a = this->operator[](i);
                    if (IsMissingValue(a))
                        ts.operator[](i) = ts.GetNACode();
                    else
                        ts.operator[](i) = a + value;
                }
                return ts;
            }

            template<typename M>
            TTimeSeries<T> operator*(M multiplicator) const
            {
                T a;
                TTimeSeries<T> ts(*this);
                auto length = GetLength();
                for (size_t i = 0; i < length; i++)
                {
                    a = this->operator[](i);
                    if (IsMissingValue(a))
                        ts.operator[](i) = ts.GetNACode();
                    else
                        ts.operator[](i) = a * multiplicator;
                }
                return ts;
            }

            string Tag;

        private:

            void CheckIntervalBounds(const size_t& from, size_t& to) const
            {
                size_t tsLen = this->GetLength();
                datatypes::exceptions::RangeCheck<size_t>::CheckTimeSeriesInterval(from, to, tsLen);
            }

            void UncheckedCopyTo(T * dest, const size_t& from, const size_t& to) const
            {
                // The following is neat and safe but not portable...
                //std::copy(data.begin() + from, data.begin() + to + 1, stdext::checked_array_iterator<T*>(dest, to - from + 1));
                // so, looking potentially unsafe:
                for (size_t i = from; i <= to; i++)
                {
                    dest[i - from] = storage->operator[](i);
                }
            }

            void UncheckedCopyTo(T * dest, const size_t& from, const size_t& to, const T& missingValue) const
            {
                for (size_t i = from; i <= to; i++)
                {
                    T value = storage->operator[](i);
                    dest[i - from] = IsMissingValue(value) ? missingValue : value;
                }
            }

            void DeepCopyFrom(const TTimeSeries<T>& src) {
                Tag = src.Tag;
                mvp = src.mvp->Clone();
                if (storage == nullptr)
                    storage = src.storage->Clone();
                else
                    src.storage->CopyTo(*(this->storage));
            }

            //ptime startDate;
            //TimeStep timeStep;
            static std::atomic<int> instances;

            void SetDefaults(StoragePolicy<T>* storage, MissingValuePolicy<T>* mvp)
            {
                this->mvp = (mvp != nullptr) ? mvp : DefaultMissingValuePolicy<T>();
                this->storage = (storage != nullptr) ? storage : DefaultStoragePolicy<T>();
                if(!this->storage->ReadOnly())
                    this->SetTimeStep(TimeStep::GetHourly());
            }

        public:
            static int NumInstances() { return instances; };
        };

        //template <typename T, template <typename> class StP, template <typename> class MvP>
        template <typename T>
        std::atomic<int> TTimeSeries<T>::instances(0);

        typedef TTimeSeries < double > TimeSeries;

        template <typename TsType = TimeSeries>
        class MultiTimeSeries // This may become an abstract class with specializations for lazy loading time series from the data store.
        {
        private:
            EnsembleStoragePolicy<TsType>* store = nullptr;
        protected:
            virtual void InitializeStorage()
            {
                if (store == nullptr)
                    store = new StdVectorEnsembleStoragePolicy<TsType>();
            }
        public:

            typedef typename std::remove_pointer<TsType>::type Type;
            typedef typename std::add_pointer<Type>::type PtrType;
            typedef TsType ItemType;
            typedef typename Type::ElementType ElementType;

            MultiTimeSeries(const vector<ElementType*>& values, size_t length, const ptime& startDate, const TimeStep& timeStep)
            {
                Clear();
                this->startDate = startDate;
                this->timeStep = timeStep;
                vector<PtrType> series;
                for (auto& d : values)
                    series.push_back(new Type(d, length, startDate, timeStep));
                store->Reset(series, startDate, timeStep);
            }

            MultiTimeSeries(const vector<vector<ElementType>>& values, const ptime& startDate, const TimeStep& timeStep)
            {
                Clear();
                this->startDate = startDate;
                this->timeStep = timeStep;
                vector<PtrType> series;
                for (auto& d : values)
                    series.push_back(new Type(d, startDate, timeStep));
                store->Reset(series, startDate, timeStep);
            }

            MultiTimeSeries(ElementType** const values, size_t ensSize, size_t length, const ptime& startDate, const TimeStep& timeStep)
            {
                Clear(); 
                this->startDate = startDate;
                this->timeStep = timeStep;
                vector<PtrType> series;
                for (int i = 0; i < ensSize; i++)
                    series.push_back(new Type(values[i], length, startDate, timeStep));
                store->Reset(series, startDate, timeStep);
            }

            MultiTimeSeries(const vector<PtrType>& values, const ptime& startDate, const TimeStep& timeStep)
            {
                Clear();
                this->startDate = startDate;
                this->timeStep = timeStep;
                store->Reset(values, startDate, timeStep);
            }

            MultiTimeSeries(const Type& series)
            {
                Clear();
                this->startDate = series.GetStartDate();
                this->timeStep = series.GetTimeStep();
                vector<PtrType> s;
                s.push_back(new Type(series));
                store->Reset(s, startDate, timeStep);
            }

            MultiTimeSeries(const vector<Type>& values, const ptime& startDate, const TimeStep& timeStep)
            {
                Clear();
                this->startDate = startDate;
                this->timeStep = timeStep;
                vector<PtrType> series;
                for (const Type& d : values)
                    series.push_back(new Type(d));
                store->Reset(series, startDate, timeStep);
            }

            // This constructor is initially intended only as a convenience for testing purposes.
            MultiTimeSeries(std::function<Type(size_t)>& valueGen, size_t ensSize, const ptime& startDate, const TimeStep& timeStep)
            {
                Clear();
                this->startDate = startDate;
                this->timeStep = timeStep;
                vector<PtrType> series;
                for (size_t i = 0; i < ensSize; i++)
                    series.push_back(new Type(valueGen(i)));
                store->Reset(series, startDate, timeStep);
            }

            MultiTimeSeries(const MultiTimeSeries<TsType>& src)
            {
                *this = src;
            }

            MultiTimeSeries(EnsembleStoragePolicy<TsType>* store)
            {
                if (store == nullptr) datatypes::exceptions::ExceptionUtilities::ThrowInvalidArgument("store must not be nullptr");
                this->store = store;
            }

            MultiTimeSeries()
            {
                this->startDate = ptime(not_a_date_time);
                this->timeStep = TimeStep::GetHourly();
            }

            MultiTimeSeries<PtrType>* AsPointerSeries()
            {
                return new MultiTimeSeries<PtrType>(store->AsReadonlyVector(), startDate, timeStep);
            }

            MultiTimeSeries<Type> AsValueSeries()
            {
                return MultiTimeSeries<Type>(store->AsReadonlyVector(), startDate, timeStep);
            }

            ~MultiTimeSeries()
            {
                Clear();
            }

            MultiTimeSeries& operator=(const MultiTimeSeries& src) {
                if (&src == this) {
                    return *this;
                }
                OperatorEqualImpl(src);
                return *this;
            }

            MultiTimeSeries& operator=(MultiTimeSeries&& src) {
                if (&src == this) {
                    return *this;
                }
                std::swap(timeStep, src.timeStep);
                std::swap(startDate, src.startDate);
                std::swap(store, src.store);
                return *this;
            }

            void ResetSeries(const size_t& numSeries, const size_t& lengthSeries, const ptime& startDate, const TimeStep& timeStep)
            {
                Clear();
                store->ResetSeries(numSeries, lengthSeries, startDate, timeStep);
                this->startDate = startDate;
                this->timeStep = timeStep;
            }

            TsType Get(size_t i)
            {
                return store->Get(i);
            }

            Type Get(size_t i) const
            {
                return store->Get(i);
            }

            ElementType Get(size_t i, size_t tsIndex)
            {
                return store->Get(i, tsIndex);
            }

            void Set(size_t i, size_t tsIndex, ElementType val)
            {
                store->Set(i, tsIndex, val);
            }

            void Set(size_t i, const Type& val)
            {
                store->Set(i, val);
            }

            vector<ElementType*>* GetValues() const
            {
                return store->GetValues();
            }

            void CopyTo(ElementType ** dest) const
            {
                store->CopyTo(dest);
            }

            size_t Size() const
            {
                return store->Size();
            }

            size_t GetLength(size_t i) const
            {
                return store->GetLength(i);
            }

            ptime GetStartDate() const
            {
                return startDate;
            }

            void SetStartDate(const ptime& start)
            {
                startDate = start;
            }

            TimeStep GetTimeStep() const
            {
                return timeStep;
            }

            void Clear()
            {
                if (store == nullptr)
                    InitializeStorage();
                else
                    store->Clear();
            }

        private:

            ptime startDate;
            TimeStep timeStep;

            void DeepCopyFrom(const MultiTimeSeries<TsType>& src)
            {
                this->startDate = src.startDate;
                this->timeStep = src.timeStep;
                if (store == nullptr)
                    store = src.store->Clone();
                else
                    *(src.store) = (*(this->store));
            }

        protected:
            virtual void OperatorEqualImpl(const MultiTimeSeries<TsType>& src)
            {
                DeepCopyFrom(src);
            }
        };


        template<typename T>
        struct time_series_of
        {
            typedef TTimeSeries<T> type;
        };

        template<typename T>
        struct ensemble_of
        {
            typedef MultiTimeSeries<T> type;
        };

        template<typename T>
        struct item_type_of
        {
            typedef typename T::ElementType type;
        };

        template<typename ElementType=double>
        struct CommonTypes
        {
            using SeriesType = typename time_series_of<ElementType>::type;
            using PtrSeriesType = typename std::add_pointer<SeriesType>::type;

            using EnsembleType = typename ensemble_of<SeriesType>::type;
            using EnsemblePtrType = typename ensemble_of<PtrSeriesType>::type;
            using PtrEnsemblePtrType = typename std::add_pointer<EnsemblePtrType>::type;

            using TSeriesEnsemblePtrType = typename time_series_of<PtrEnsemblePtrType>::type;
            using PtrTSeriesEnsemblePtrType = typename std::add_pointer<TSeriesEnsemblePtrType>::type;
        };

        template <typename ItemType>
        using PointerTypeTimeSeries = TTimeSeries < ItemType* > ;

        template <typename Tts = TimeSeries>
        using MultiTimeSeriesPtr = MultiTimeSeries < Tts* > ;

        template <typename Tts = TimeSeries>
        using ForecastTimeSeries = PointerTypeTimeSeries < Tts >;

        template <typename Tts = TimeSeries>
        using TimeSeriesEnsemble = MultiTimeSeriesPtr < Tts >;

        template <typename Tts = TimeSeries>
        using EnsembleForecastTimeSeries = PointerTypeTimeSeries < MultiTimeSeriesPtr<Tts> > ;

        template <typename Tts = TimeSeries>
        class TimeSeriesOperations
        {
        public:

            using ElementType = typename Tts::ElementType;
            using SeriesType = typename CommonTypes<ElementType>::SeriesType;
            using PtrSeriesType = typename CommonTypes<ElementType>::PtrSeriesType;
            using EnsembleType = typename CommonTypes<ElementType>::EnsembleType;
            using EnsemblePtrType = typename CommonTypes<ElementType>::EnsemblePtrType;
            using PtrEnsemblePtrType = typename CommonTypes<ElementType>::PtrEnsemblePtrType;
            using TSeriesEnsemblePtrType = typename CommonTypes<ElementType>::TSeriesEnsemblePtrType;
            using PtrTSeriesEnsemblePtrType = typename CommonTypes<ElementType>::PtrTSeriesEnsemblePtrType;

            static PtrSeriesType TrimTimeSeries(const SeriesType& timeSeries, const ptime& startDate, const ptime& endDate)
            {
                ptime sd = timeSeries.GetStartDate();
                ptime ed = timeSeries.GetEndDate();

                size_t sIndex = timeSeries.UpperIndexForTime(startDate);
                size_t eIndex = timeSeries.LowerIndexForTime(endDate);

                return new SeriesType(timeSeries.Subset(sIndex, eIndex));
            }

            static PtrSeriesType Resample(const SeriesType& timeSeries, const string& method)
            {
                using namespace boost::algorithm;
                string m = method;
                to_lower(m);
                if (m == "")
                    return new TimeSeries(timeSeries);
                else if (m == "daily_to_hourly")
                    return DailyToHourly(timeSeries);
                else
                {
                    datatypes::exceptions::ExceptionUtilities::ThrowInvalidArgument("Time series resampling method not known: " + method);
                    return nullptr;
                }
            }

            static PtrSeriesType DailyToHourly(const SeriesType& dailyTimeSeries)
            {
                using T = typename SeriesType::ElementType;
                size_t length = dailyTimeSeries.GetLength();

                T * data = new T[length * 24];

                for (size_t i = 0; i < length; i++)
                    for (size_t j = 0; j < 24; j++)
                        data[(i * 24) + j] = (dailyTimeSeries[i] / 24);

                PtrSeriesType result = new SeriesType(data, length * 24, dailyTimeSeries.GetStartDate());

                delete[] data;

                return result;
            }

            static PtrSeriesType JoinTimeSeries(const SeriesType& head, const SeriesType& tail)
            {
                using T = typename SeriesType::ElementType;
                ptime startDate = head.GetStartDate();

                size_t headLength = head.GetLength();
                size_t tailLength = tail.GetLength();

                size_t length = headLength + tailLength;

                T * data = new T[length];

                for (size_t i = 0; i < length; i++)
                {
                    if (i < headLength)
                        data[i] = head[i];
                    else
                        data[i] = tail[i - headLength];
                }

                PtrSeriesType result = new SeriesType(data, length, startDate);

                delete[] data;

                return result;
            }

            static SeriesType AggregateTimeStep(const SeriesType& series, const string& argument) {

                using sec_type = boost::posix_time::time_duration::sec_type;
                auto newTimeStep = TimeStep::Parse(argument);
                sec_type deltaNew = newTimeStep.GetRegularStepDuration().total_seconds();
                sec_type delta = series.GetTimeStep().GetRegularStepDuration().total_seconds();
                if (deltaNew < delta)
                    throw std::logic_error("Cannot aggregate to a target time step finer than data source");
                sec_type remainder = deltaNew %delta;
                if (remainder != 0)
                    throw std::logic_error("Aggregate: target time step must be a multiple of the starting time step");
                sec_type multiple = deltaNew / delta;

                size_t targetSize = series.GetLength() / multiple;
                if (targetSize < 1)
                    throw std::logic_error("Aggregate: source lenght too short to aggregate");
                SeriesType newTs(0.0, targetSize, series.TimeForIndex(multiple-1), newTimeStep);

                for (size_t i = 0; i < targetSize; i++)
                {
                    double accumulated = 0;
                    for (size_t j = 0; j < multiple; j++)
                    {
                        auto val = series.GetValue(i * multiple + j);
                        if (series.IsMissingValue(val))
                        {
                            newTs.SetValue(i, newTs.GetMissingValue());
                            accumulated = .0;
                            break;
                        }
                        else
                            accumulated += val;
                    }
                    newTs.SetValue(i, accumulated);
                    accumulated = .0;
                }
                return newTs;
            }

            static SeriesType DisaggregateTimeStep(const SeriesType& series, const string& argument) {

                using sec_type = boost::posix_time::time_duration::sec_type;
                TimeStep newTimeStep = TimeStep::Parse(argument);
                sec_type deltaNew = newTimeStep.GetRegularStepDuration().total_seconds();
                sec_type delta = series.GetTimeStep().GetRegularStepDuration().total_seconds();
                if (deltaNew > delta)
                    throw std::logic_error("Cannot disaggregate to a target time step coarser than data source");
                sec_type remainder = delta % deltaNew;
                if (remainder != 0)
                    throw std::logic_error("Disaggregate: the starting time step must be a multiple of the target time step");

                sec_type multiple_sc = delta / deltaNew;
                // NOTE: I had changed from sec_type to size_t because of a compilation issue with gcc 8.3.0 (??), but this breaks the UT on calling AddSteps
                size_t multiple = (size_t)multiple_sc;

                size_t srcSize = series.GetLength();
                size_t targetSize = series.GetLength() * multiple;
                if (targetSize < 1)
                    throw std::logic_error("Disaggregate: source lengh is too short to aggregate");
                ptime newStartDate = newTimeStep.AddSteps(series.GetStartDate(), -( ((double)multiple) - 1));
                SeriesType newTs(0.0, targetSize, newStartDate, newTimeStep);

                for (size_t i = 0; i < srcSize; i++)
                {
                    auto val = series.GetValue(i);
                    for (size_t j = 0; j < multiple; j++)
                    {
                        if (series.IsMissingValue(val))
                            newTs.SetValue(i * multiple + j, newTs.GetMissingValue());
                        else
                            newTs.SetValue(i * multiple + j, val / multiple);
                    }
                }
                return newTs;
            }

            static void AggregateTimeStep(SeriesType& series, const string& argument) {
                series = AggregateTimeStep((const SeriesType&)series, argument);
            }

            static void DisaggregateTimeStep(SeriesType& series, const string& argument) {
                series = DisaggregateTimeStep((const SeriesType&)series, argument);
            }

            static void TransformEachItem(TSeriesEnsemblePtrType& efts, const string& method, const string& methodArgument)
            {
                if (method == string("accumulate"))
                {
                    auto n = efts.GetLength();
                    for (size_t i = 0; i < n; i++)
                    {
                        PtrEnsemblePtrType item = efts.GetValue(i);
                        EnsemblePtrType& y = *item;
                        for (size_t j = 0; j < y.Size(); j++)
                        {
                            PtrSeriesType t = y.Get(j);
                            AggregateTimeStep(*t, methodArgument);
                            if (j == 0) y.SetStartDate(t->GetStartDate());
                        }
                    }
                }
                else if (method == string("disaggregate"))
                {
                    auto n = efts.GetLength();
                    for (size_t i = 0; i < n; i++)
                    {
                        PtrEnsemblePtrType item = efts.GetValue(i);
                        EnsemblePtrType& y = *item;
                        for (size_t j = 0; j < y.Size(); j++)
                        {
                            PtrSeriesType t = y.Get(j);
                            DisaggregateTimeStep(*t, methodArgument);
                            if (j == 0) y.SetStartDate(t->GetStartDate());
                        }
                    }
                }
                else
                    throw std::logic_error("TransformEachItem is limited to 'accumulate' or 'disaggregate'");
            }

        private:
            static const PtrEnsemblePtrType& GetEnsemble(const TSeriesEnsemblePtrType& ensTs, size_t index = 0)
            {
                using datatypes::exceptions::ExceptionUtilities;
                if (ensTs.GetLength() == 0) ExceptionUtilities::ThrowInvalidArgument("ensemble time series is of length zero");
                ExceptionUtilities::CheckInRange<size_t>(index, 0, ensTs.GetLength(), "index");
                const PtrEnsemblePtrType& ens = ensTs.GetValue(index);
                //if (ens->Size() == 0) ExceptionUtilities::ThrowInvalidArgument("ensemble is of size zero");
                return ens;
            }
        public:

            static ptime GetStart(const TSeriesEnsemblePtrType& ensTs, size_t index = 0)
            {
                auto ens = GetEnsemble(ensTs, index);
                return ens->GetStartDate();
            }

            static ptime GetEnd(const TSeriesEnsemblePtrType& ensTs, size_t index = 0)
            {
                auto ens = GetEnsemble(ensTs, index);
                return ens->Get(0)->GetEndDate();
            }

            static void CreateForecast(TSeriesEnsemblePtrType& forecast, const SeriesType& observations, const ptime& start, size_t length, const TimeStep& issueTimeStep, size_t leadTime, size_t offsetForecasts)
            {
                forecast.Reset(length, start, issueTimeStep);
                TimeStep obsTstep = observations.GetTimeStep();
                for (size_t i = 0; i < length; i++)
                {
                    // Index in the observation time series corresponding to the forecast issue time 'i'
                    size_t obsIndex = observations.IndexForTime(issueTimeStep.AddSteps(start, i));
                    size_t from = obsIndex + offsetForecasts;
                    size_t to = from + (leadTime-1);
                    SeriesType fcast = observations.Subset(from, to);
                    EnsemblePtrType* mts = new EnsemblePtrType(fcast);
                    forecast.SetValue(i, mts);
                }
            }

            static TSeriesEnsemblePtrType* CreateForecastPtr(const SeriesType& observations, const ptime& start, size_t length, const TimeStep& issueTimeStep, size_t leadTime, size_t offsetForecasts)
            {
                TSeriesEnsemblePtrType* forecast = new TSeriesEnsemblePtrType(length, start, issueTimeStep);
                CreateForecast(*forecast, observations, start, length, issueTimeStep, leadTime, offsetForecasts);
                return forecast;
            }

            static TSeriesEnsemblePtrType CreateForecast(const SeriesType& observations, const ptime& start, size_t length, const TimeStep& issueTimeStep, size_t leadTime, size_t offsetForecasts)
            {
                TSeriesEnsemblePtrType forecast;
                CreateForecast(forecast, observations, start, length, issueTimeStep, leadTime, offsetForecasts);
                return forecast;
            }

            template<typename U>
            static bool AreEqual(const SeriesType& a, const U& b, bool strict = false, double tolerance = 1e-12)
            {
                size_t lengthA = a.GetLength();
                for (size_t i = 0; i < lengthA; i++)
                {
                    auto valA = a[i];

                    if (strict && (valA != b))
                        return false;
                    else if (std::abs(valA - b) > tolerance)
                        return false;
                }
                return true;
            }

            static bool AreTimeSeriesEqual(const SeriesType& a, const SeriesType& b, bool strict = false, double tolerance = 1e-12)
            {
                ptime startA = a.GetStartDate();
                ptime startB = b.GetStartDate();

                if (startA != startB)
                    return false;

                ptime endA = a.GetEndDate();
                ptime endB = b.GetEndDate();

                if (endA != endB)
                    return false;

                size_t lengthA = a.GetLength();
                size_t lengthB = b.GetLength();

                if (lengthA != lengthB)
                    return false;

                for (size_t i = 0; i < lengthA; i++)
                {
                    auto valA = a[i];
                    auto valB = b[i];

                    if (strict && (valA != valB))
                        return false;
                    else if (std::abs(valA - valB) > tolerance)
                        return false;
                }

                return true;
            }

            static bool AreTimeSeriesEqual(const SeriesType& a, const SeriesType& b, const ptime& from, const ptime& to, bool strict = false, double tolerance = 1e-12)
            {
                TimeStep ta = a.GetTimeStep();
                TimeStep tb = b.GetTimeStep();
                if (ta != tb)
                    return false;

                auto n = ta.GetNumSteps(from, to);
                if (n < 0)
                    return false;
                size_t s = (size_t)n;
                auto offsetA = a.IndexForTime(from);
                auto offsetB = b.IndexForTime(from);
                for (size_t i = 0; i < s; i++)
                {
                    auto valA = a[i + offsetA];
                    auto valB = b[i + offsetB];
                    if (strict && (valA != valB))
                        return false;
                    else if (std::abs(valA - valB) > tolerance)
                        return false;
                }

                return true;
            }

            static bool AreValueEqual(const SeriesType& a, const vector<ElementType>& b, size_t from = 0, size_t to = std::numeric_limits<size_t>::max(), bool strict = false, double tolerance = 1e-12)
            {
                vector<ElementType> v = a.GetValuesVector(from, to);
                if (v.size() != b.size())
                    return false;
                for (size_t i = 0; i < v.size(); i++)
                {
                    auto valA = v[i];
                    auto valB = b[i];
                    if (strict && (valA != valB))
                        return false;
                    else if (std::abs(valA - valB) > tolerance)
                        return false;
                }
                return true;
            }


            static bool AreEnsembleTimeSeriesEqual(EnsemblePtrType& a, EnsemblePtrType& b)
            {
                size_t lengthA = a.Size();
                size_t lengthB = b.Size();

                if (lengthA != lengthB)
                    return false;

                for (size_t i = 0; i < lengthA; i++)
                {
                    auto valA = a.Get(i);
                    auto valB = b.Get(i);

                    if (!AreTimeSeriesEqual(*valA, *valB))
                        return false;
                }
                return true;
            }

            static bool AreEnsembleTimeSeriesEqual(EnsembleType& a, EnsembleType& b)
            {
                size_t lengthA = a.Size();
                size_t lengthB = b.Size();

                if (lengthA != lengthB)
                    return false;

                for (size_t i = 0; i < lengthA; i++)
                {
                    auto valA = a.Get(i);
                    auto valB = b.Get(i);

                    if (!AreTimeSeriesEqual(valA, valB))
                        return false;
                }
                return true;
            }

            static bool AreTimeSeriesEnsembleTimeSeriesEqual(TSeriesEnsemblePtrType& a, TSeriesEnsemblePtrType& b)
            {
                size_t lengthA = a.GetLength();
                size_t lengthB = b.GetLength();

                if (lengthA != lengthB)
                    return false;

                ptime startA = a.GetStartDate();
                ptime startB = b.GetStartDate();

                if (startA != startB)
                    return false;

                for (size_t i = 0; i < lengthA; i++)
                {
                    auto valA = a.GetValue(i);
                    auto valB = b.GetValue(i);

                    if (!AreEnsembleTimeSeriesEqual(*valA, *valB))
                        return false;
                }
                return true;
            }

            template <typename T = typename Tts::ElementType>
            static PtrSeriesType MaskTimeSeries(const SeriesType& timeSeries, const ptime& start, const ptime& end, T maskValue)
            {
                if (start < timeSeries.GetStartDate())
                    datatypes::exceptions::ExceptionUtilities::ThrowInvalidArgument("start needs to be greater than time series start");

                if (end > timeSeries.GetEndDate())
                    datatypes::exceptions::ExceptionUtilities::ThrowInvalidArgument("end needs to be less than time series end");

                size_t sIndex = timeSeries.UpperIndexForTime(start);
                size_t eIndex = timeSeries.LowerIndexForTime(end);

                size_t len = timeSeries.GetLength();
                double* d = new double[len];
                timeSeries.CopyTo(d, 0, len - 1);

                for (size_t i = sIndex; i <= eIndex; i++)
                    d[i] = maskValue;

                PtrSeriesType result = new SeriesType(d, len, timeSeries.GetStartDate(), timeSeries.GetTimeStep());

                delete[] d;

                return result;
            }
        };

        template <typename T>
        TTimeSeries<T> operator<<(const TTimeSeries<T>& a, const TTimeSeries<T>& b) {
            using TsOps = TimeSeriesOperations<TTimeSeries<T>>;
            if (a.GetTimeStep() != b.GetTimeStep()) // TODO: this is a minimum requirement
                datatypes::exceptions::ExceptionUtilities::ThrowNotSupported("operator<< requires identical time steps");
            auto s = std::min(a.GetStartDate(), b.GetStartDate());
            auto e = std::max(a.GetEndDate(), b.GetEndDate());
            auto tstep = a.GetTimeStep();
            auto length = tstep.GetNumSteps(s, e);
            TTimeSeries<T> result(length, s, tstep);
            result.CopyValues(a);
            result.CopyValues(b);
            return result;
        }

        template <typename Tts = TimeSeries>
        class TimeWindow
        {
        public:
            TimeWindow(const ptime& startDate, const ptime& endDate)
            {
                this->startDate = startDate;
                this->endDate = endDate;
            }

            Tts* Trim(const Tts& timeSeries) const
            {
                return TimeSeriesOperations<Tts>::TrimTimeSeries(timeSeries, startDate, endDate);
            }

        private:
            ptime startDate;
            ptime endDate;

        };

        /*******************
        Below are implementations of the template code; they would normally be found in a .cpp file, but as
        templates putting them here makes it more reusable from other programs.
        ******************/
    }
    namespace exceptions
    {
        class DATATYPES_DLL_LIB TimeSeriesChecks
        {
        public:
            static void CheckOutOfRange(const string& msg, const datatypes::timeseries::TimeSeries& ts, const ptime& d);
        };
    }
}
```


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000
