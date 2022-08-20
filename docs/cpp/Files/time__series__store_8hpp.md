---
title: datatypes/time_series_store.hpp

---

# datatypes/time_series_store.hpp



## Namespaces

| Name           |
| -------------- |
| **[datatypes](/cpp/Namespaces/namespacedatatypes/)**  |
| **[datatypes::timeseries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/)**  |

## Classes

|                | Name           |
| -------------- | -------------- |
| class | **[datatypes::timeseries::IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/)** <br>An interface definition for objects that can provide hierarchical identification.  |
| class | **[datatypes::timeseries::TimeSeriesProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesProvider/)** <br>Library of time series, for high level access to sources of univariate, single instance time series that may have varying on-disk representations.  |
| class | **[datatypes::timeseries::DataDimensionDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/)**  |
| class | **[datatypes::timeseries::DataDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/)**  |
| class | **[datatypes::timeseries::SingleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/)** <br>Interface definition for storages of single, univariate time series.  |
| class | **[datatypes::timeseries::EnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/)** <br>Interface definition for storages of ensembles of univariate time series.  |
| class | **[datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)** <br>Interface definition for storages of time series of ensembles of time series.  |
| class | **[datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/)**  |
| class | **[datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/)**  |
| class | **[datatypes::timeseries::TTimeSeriesLibrary](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/)**  |
| class | **[datatypes::timeseries::TimeSeriesSourceInfoImpl](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/)**  |
| class | **[datatypes::timeseries::TimeSeriesSourceInfo](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/)**  |
| class | **[datatypes::timeseries::NetCdfSourceInfo](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/)**  |
| class | **[datatypes::timeseries::TimeSeriesLibraryDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/)**  |
| class | **[datatypes::timeseries::TimeSeriesSourceInfoBuilder](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoBuilder/)** <br>An abstract class to allow callers to inject custom time series data sources into a time series library.  |
| class | **[datatypes::timeseries::TimeSeriesStoreFactory](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/)**  |
| class | **[datatypes::timeseries::TimeSeriesLibrary](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/)** <br>Library of time series, for high level access to sources of time series that nmay have varying on-disk representations.  |

## Defines

|                | Name           |
| -------------- | -------------- |
|  | **[TIME_DIM_TYPE_DATA_DIMENSION](/cpp/Files/time__series__store_8hpp/#define-time-dim-type-data-dimension)**  |
|  | **[COLLECTION_DIM_TYPE_DATA_DIMENSION](/cpp/Files/time__series__store_8hpp/#define-collection-dim-type-data-dimension)**  |
|  | **[ENSEMBLE_DIM_TYPE_DATA_DIMENSION](/cpp/Files/time__series__store_8hpp/#define-ensemble-dim-type-data-dimension)**  |




## Macros Documentation

### define TIME_DIM_TYPE_DATA_DIMENSION

```cpp
#define TIME_DIM_TYPE_DATA_DIMENSION "time"
```


### define COLLECTION_DIM_TYPE_DATA_DIMENSION

```cpp
#define COLLECTION_DIM_TYPE_DATA_DIMENSION "collection"
```


### define ENSEMBLE_DIM_TYPE_DATA_DIMENSION

```cpp
#define ENSEMBLE_DIM_TYPE_DATA_DIMENSION "ensemble"
```


## Source code

```cpp
#pragma once

#include <stdexcept> 
#include <netcdf.h>
#include <map>
#ifdef __GNUC__
// https ://jira.csiro.au/browse/WIRADA-350  GNU gcc regex bug; use boost instead
#if (__GNUC__ <= 4 && __GNUC_MINOR__ < 9)
#include <boost/regex.hpp>
#else
#include <regex>
#endif
#else
#include <regex>
#endif // __GNUC__
#include <boost/function.hpp>
#include <boost/filesystem.hpp>
#include <boost/range/iterator_range.hpp>

#include <boost/algorithm/string/predicate.hpp>
#include <boost/algorithm/string/split.hpp>
#include <boost/algorithm/string/classification.hpp>
#include <boost/algorithm/string.hpp>    

#include "datatypes/time_series.hpp"
#include "datatypes/exception_utilities.h"
#include "yaml-cpp/yaml.h"

namespace datatypes
{
    namespace timeseries
    {
        class DATATYPES_DLL_LIB IdentifiersProvider
        {
        public:
            virtual ~IdentifiersProvider() {}
            virtual vector<string> GetIdentifiers() const = 0;
            static vector<string> SplitHierarchicalIdentifier(const string& longId);
            static string GetTopmostIdentifier(const string& longId);
            static void CheckNotEmpty(const string& longId);
        };

        template <typename T>
        class DATATYPES_DLL_LIB TimeSeriesProvider :
            public IdentifiersProvider
        {
        public:
            virtual ~TimeSeriesProvider() {}

            virtual TTimeSeries<T>* GetSingle(const string& dataId) = 0;
        };

#define TIME_DIM_TYPE_DATA_DIMENSION "time"

        // Collection may not be a necessary distinction compared to ensemble. Reconsider.
#define COLLECTION_DIM_TYPE_DATA_DIMENSION "collection"
#define ENSEMBLE_DIM_TYPE_DATA_DIMENSION "ensemble"

        class DATATYPES_DLL_LIB DataDimensionDescriptor
        {
        public:
            DataDimensionDescriptor(const string& type, const string& dimname = "", size_t size = 0);
            DataDimensionDescriptor(const DataDimensionDescriptor& src);
            DataDimensionDescriptor(DataDimensionDescriptor&& src);
            DataDimensionDescriptor& operator=(const DataDimensionDescriptor& src);
            DataDimensionDescriptor& operator=(DataDimensionDescriptor&& src);
            string DimensionType; // "collection", "ensemble", "time"
            string DimensionName;
            size_t Size = 0;
        };


        class DATATYPES_DLL_LIB DataDescriptor
        {
        public:
            virtual string GetDataSummary() const = 0;
            virtual vector<DataDimensionDescriptor> GetDataDimensionsDescription() const = 0;
        };


        template <typename T>
        class DATATYPES_DLL_LIB SingleTimeSeriesStore :
            public IdentifiersProvider, 
            public DataDescriptor
        {
        public:
            virtual ~SingleTimeSeriesStore() {};
            virtual TTimeSeries<T>* Read() = 0;
            virtual TTimeSeries<T>* Read(const string& collectionIdentifier) = 0;
            virtual MultiTimeSeries<TTimeSeries<T>*>* ReadAllCollection() = 0;
            //virtual string GetDataSummary() const = 0;
            //virtual vector<DataDimensionDescriptor> GetDataDimensionsDescription() const = 0;
        };

        template <typename T>
        class DATATYPES_DLL_LIB EnsembleTimeSeriesStore :
            public IdentifiersProvider,
            public DataDescriptor
        {
        public:
            virtual ~EnsembleTimeSeriesStore() {};
            virtual MultiTimeSeries<TTimeSeries<T>*>* Read() = 0;
            //virtual string GetDataSummary() const = 0;
            virtual vector<string> GetIdentifiers() const { datatypes::exceptions::ExceptionUtilities::ThrowNotImplemented();  vector<string> x; return x; }
        };

        template <typename T>
        class DATATYPES_DLL_LIB TimeSeriesEnsembleTimeSeriesStore :
            public IdentifiersProvider,
            public TimeSeriesInfoProvider,
            public DataDescriptor
        {
        public:

            using SeriesType = typename CommonTypes<T>::SeriesType;
            using PtrSeriesType = typename CommonTypes<T>::PtrSeriesType;
            using EnsemblePtrType = typename CommonTypes<T>::EnsemblePtrType;
            using PtrEnsemblePtrType = typename CommonTypes<T>::PtrEnsemblePtrType;
            using TSeriesEnsemblePtrType = typename CommonTypes<T>::TSeriesEnsemblePtrType;
            using PtrTSeriesEnsemblePtrType = typename CommonTypes<T>::PtrTSeriesEnsemblePtrType;

            virtual ~TimeSeriesEnsembleTimeSeriesStore() {};
            virtual PtrTSeriesEnsemblePtrType GetSeries(const string& dataId) = 0;
            virtual PtrEnsemblePtrType GetItem(const string& dataId, size_t fcastIndex)
            {
                datatypes::exceptions::ExceptionUtilities::ThrowNotImplemented();
                return nullptr;
            }

            virtual PtrSeriesType GetItem(const string& dataId, size_t fcastIndex, size_t ensIndex)
            {
                datatypes::exceptions::ExceptionUtilities::ThrowNotImplemented();
                return nullptr;
            }

            virtual size_t GetEnsembleSize(const string& dataId, size_t fcastIndex) const
            {
                datatypes::exceptions::ExceptionUtilities::ThrowNotImplemented();
                return 0;
            }

            //virtual string GetDataSummary() const = 0;
            // TODO: revise these. Now that the store has a GetSeries method, these should be hidden further. 
            //protected:
            virtual PtrEnsemblePtrType Read(const string& ensembleIdentifier) = 0;
            virtual size_t GetLength() const = 0;
            virtual ptime GetStart() const = 0;
            virtual TimeStep GetTimeStep() const = 0;
            virtual vector<string> GetIdentifiers() const { datatypes::exceptions::ExceptionUtilities::ThrowNotImplemented();  vector<string> x; return x; }
        };

        template <typename T>
        class DATATYPES_DLL_LIB WritableTimeSeriesEnsembleTimeSeriesStore :
            public TimeSeriesEnsembleTimeSeriesStore<T>
        {
        public:
            using SeriesType = typename CommonTypes<T>::SeriesType;
            using PtrSeriesType = typename CommonTypes<T>::PtrSeriesType;
            using EnsemblePtrType = typename CommonTypes<T>::EnsemblePtrType;
            using PtrEnsemblePtrType = typename CommonTypes<T>::PtrEnsemblePtrType;
            using TSeriesEnsemblePtrType = typename CommonTypes<T>::TSeriesEnsemblePtrType;
            using PtrTSeriesEnsemblePtrType = typename CommonTypes<T>::PtrTSeriesEnsemblePtrType;

            virtual ~WritableTimeSeriesEnsembleTimeSeriesStore() {};

            virtual bool IsActive() = 0;
            virtual void Allocate(size_t length, PtrEnsemblePtrType value) = 0;
            void AllocateValues(size_t length, const PtrEnsemblePtrType* values)
            {
                vector<PtrEnsemblePtrType> v(length);
                v.assign(values, values + length);
                AllocateValues(v);
            }
            virtual void AllocateValues(const vector<PtrEnsemblePtrType>& values)
            {
                datatypes::exceptions::ExceptionUtilities::ThrowNotImplemented();
            }
            virtual void SetSeries(const string& dataId, PtrTSeriesEnsemblePtrType value) = 0;
            virtual void SetItem(const string& dataId, size_t index, PtrEnsemblePtrType value) = 0;
            virtual void SetItem(const string& dataId, size_t index, const EnsemblePtrType& value) = 0;
            //virtual PtrEnsemblePtrType Read(const string& ensembleIdentifier) = 0;
            virtual void SetLength(size_t) = 0;
            virtual void SetStart(ptime) = 0;
            //virtual vector<string> GetItemIdentifiers() const = 0;
            virtual void SetTimeStep(const TimeStep&) = 0;
            //virtual vector<string> GetIdentifiers() const { datatypes::exceptions::ExceptionUtilities::ThrowNotImplemented();  vector<string> x; return x; }
        };

        template <typename TsType>
        class TimeSeriesEnsembleTimeSeriesStoragePolicy : public EnsembleStoragePolicy<TsType>
        {

        public:

            // TODO T should be derived from StorageType, but this is 
            // more work with datatypes' type traits than 
            // I have time and know how, for now. 
            using T = double;
            typedef typename std::remove_pointer<TsType>::type Type;
            typedef typename std::add_pointer<Type>::type PtrType;
            typedef typename Type::ElementType ElementType;

        private:

            WritableTimeSeriesEnsembleTimeSeriesStore<T> * store = nullptr;
            size_t index;

            TimeSeriesEnsembleTimeSeriesStoragePolicy()
            {
            }

        public:

            TimeSeriesEnsembleTimeSeriesStoragePolicy(WritableTimeSeriesEnsembleTimeSeriesStore<T> * store, size_t index) :
                store(store), index(index)
            {
                if (store == nullptr) datatypes::exceptions::ExceptionUtilities::ThrowInvalidArgument("store must not be nullptr for an TimeSeriesEnsembleTimeSeriesStoragePolicy");
            }

            void Reset(const vector<PtrType>& values, const ptime& startDate, const TimeStep& timeStep)
            {
                datatypes::exceptions::ExceptionUtilities::ThrowNotImplemented();
            }

            TimeSeriesEnsembleTimeSeriesStoragePolicy(const TimeSeriesEnsembleTimeSeriesStoragePolicy<TsType>& src)
            {
                DeepCopyFrom(src);
            }

            EnsembleStoragePolicy<TsType>* Clone() const
            {
                return new TimeSeriesEnsembleTimeSeriesStoragePolicy<TsType>(*this);
            }

            ~TimeSeriesEnsembleTimeSeriesStoragePolicy()
            {
                Clear();
            }

            TimeSeriesEnsembleTimeSeriesStoragePolicy& operator=(TimeSeriesEnsembleTimeSeriesStoragePolicy&& src) {
                if (&src == this) {
                    return *this;
                }
                std::swap(store, src.store);
                return *this;
            }

            void ResetSeries(const size_t& numSeries, const size_t& lengthSeries, const ptime& startDate, const TimeStep& timeStep)
            {
                datatypes::exceptions::ExceptionUtilities::ThrowNotImplemented();
            }

            PtrType GetReplicate(size_t i)
            {
                return store->GetItem("", index, i);
            }

            TsType Get(size_t i)
            {
                return TsType(GetReplicate(i));
            }

            ElementType Get(size_t i, size_t tsIndex)
            {
                return GetReplicate(i)->GetValue(tsIndex);
            }

            void Set(size_t i, size_t tsIndex, ElementType val)
            {
                PtrType ts = GetReplicate(i);
                (*ts)[tsIndex] = val;
            }

            void Set(size_t i, const Type& val)
            {
                PtrType ts = GetReplicate(i);
                *ts = val; // overloaded operator= should do this as expected - tbc
            }

            vector<ElementType*>* GetValues() const
            {
                vector<ElementType*>* result = new vector<ElementType*>();
                datatypes::exceptions::ExceptionUtilities::ThrowNotImplemented();
                return nullptr;
                //for (auto& d : series)
                //{
                //  result->push_back(d->GetValues());
                //}
                //return result;
            }

            void CopyTo(ElementType ** dest) const
            {
                datatypes::exceptions::ExceptionUtilities::ThrowNotImplemented();
                //size_t n = this->Size();
                //for (size_t i = 0; i < n; i++)
                //{
                //  dest[i] = GetReplicate(i)->GetValues();
                //}
            }

            size_t Size() const
            {
                return store->GetEnsembleSize("", index);
            }

            size_t GetLength(size_t i) const
            {
                datatypes::exceptions::ExceptionUtilities::ThrowNotImplemented();
                return 0;
                //return GetReplicate(i)->GetLength();
            }

            void Clear()
            {
                //for (auto& d : series)
                //{
                //  if (d != nullptr) delete d;
                //}
                //series.clear();
            }

            const vector<PtrType>& AsReadonlyVector() const
            {
                datatypes::exceptions::ExceptionUtilities::ThrowNotImplemented();
                return dummy; // required for compilation.
            }

        private:
            vector<PtrType> dummy;

            void DeepCopyFrom(const EnsembleStoragePolicy<TsType>& src)
            {
                datatypes::exceptions::ExceptionUtilities::ThrowNotImplemented();
                Clear();
                auto v = src.AsReadonlyVector();
                //for (size_t i = 0; i < v.size(); i++)
                //{
                //  Type* copy = new Type(*(v.at(i)));
                //  this->series.push_back(copy);
                //}
            }

        protected:
            void OperatorEqualImpl(const EnsembleStoragePolicy<TsType>& src)
            {
                DeepCopyFrom(src);
            }

        };


        using namespace datatypes::exceptions;

        template<typename T>
        class TTimeSeriesLibrary
        {
        public:
            typedef TTimeSeries<T> TS;
            typedef MultiTimeSeries<TS*> MTS;
            virtual ~TTimeSeriesLibrary() {}

            virtual TS* GetSingle(const string& dataId)
            {
                ExceptionUtilities::ThrowNotImplemented();
                return nullptr;
            }

            virtual TS* GetSingle(const string& dataId, const string& collectionIdentifier)
            {
                ExceptionUtilities::ThrowNotImplemented();
                return nullptr;
            }

            virtual MTS* GetCollection(const string& dataId)
            {
                ExceptionUtilities::ThrowNotImplemented();
                return nullptr;
            }

            virtual TimeSeriesProvider<T>* GetProvider(const string& dataId)
            {
                ExceptionUtilities::ThrowNotImplemented();
                return nullptr;
            }

            virtual MultiTimeSeries<TS*>* GetEnsembleTimeSeries(const string& dataId)
            {
                ExceptionUtilities::ThrowNotImplemented();
                return nullptr;
            }

            virtual MultiTimeSeries<TS*>* GetAllTimeSeries(const string& dataId)
            {
                ExceptionUtilities::ThrowNotImplemented();
                return nullptr;
            }

            virtual EnsembleForecastTimeSeries<TS>* GetTimeSeriesEnsembleTimeSeries(const string& dataId)
            {
                ExceptionUtilities::ThrowNotImplemented();
                return nullptr;
            }

            virtual vector<string> GetIdentifiers() const
            {
                ExceptionUtilities::ThrowNotImplemented();
                vector<string> res;
                return res;
            }
        };

        class TimeSeriesLibrary;

        class DATATYPES_DLL_LIB TimeSeriesSourceInfoImpl
        {
        protected:
            TimeSeriesSourceInfoImpl();
            TimeSeriesSourceInfoImpl(const TimeSeriesSourceInfoImpl& src);
        public:
            virtual ~TimeSeriesSourceInfoImpl();
            virtual TimeSeriesSourceInfoImpl* Clone() const = 0;
            virtual bool ApplyRootDir(const string& rootDir);

            virtual SingleTimeSeriesStore<double>* CreateSingleTimeSeriesStore() const;
            virtual EnsembleTimeSeriesStore<double>* CreateEnsembleTimeSeriesStore() const;
            virtual TimeSeriesEnsembleTimeSeriesStore<double>* CreateTimeSeriesEnsembleTimeSeriesStore() const;
            virtual std::map<string, string> GetSerializableConfiguration() const;

            static string OptionalApplyRootDir(const std::string& rootDir, const std::string& filename, bool checkDirExists = true);
        };

        class DATATYPES_DLL_LIB TimeSeriesSourceInfo
        {
        private:
            TimeSeriesSourceInfoImpl * impl = nullptr;
        public:
            TimeSeriesSourceInfo(const TimeSeriesSourceInfoImpl& t);
            TimeSeriesSourceInfo(const TimeSeriesSourceInfo& src);
            TimeSeriesSourceInfo();
            virtual ~TimeSeriesSourceInfo();
            TimeSeriesSourceInfo(TimeSeriesSourceInfo&& src);
            TimeSeriesSourceInfo& operator= (const TimeSeriesSourceInfo& src);
            TimeSeriesSourceInfo& operator= (TimeSeriesSourceInfo&& src);

            SingleTimeSeriesStore<double>* CreateSingleTimeSeriesStore() const;
            EnsembleTimeSeriesStore<double>* CreateEnsembleTimeSeriesStore() const;
            TimeSeriesEnsembleTimeSeriesStore<double>* CreateTimeSeriesEnsembleTimeSeriesStore() const;
            bool ApplyRootDir(const string& rootDir);
            std::map<string, string> GetSerializableConfiguration() const;

            static const string IdDataKey;

            static const string SingleSeriesTypeId;
            static const string EnsembleSeriesTypeId;
            static const string TimeSeriesEnsemblesTypeId;
            static const string SingleSeriesCollectionTypeId;

        private:
            //string DataId() const;
            //string Identifier() const;
            //string StorageType() const;
            //int Index() const;

            //string TimeStep() const;
            //string Start() const;
            //int Length() const;
            //int EnsembleSize() const;
            //int EnsembleLength() const;
            //string EnsembleTimeStep() const;
            //string FileName() const;
            //string NcVarName() const;
        };

        class DATATYPES_DLL_LIB NetCdfSourceInfo :
            public TimeSeriesSourceInfoImpl
        {
        private:
            bool IsFileNamePattern(const string& s) const;
        public:
            NetCdfSourceInfo() {}
            NetCdfSourceInfo(const string& dataId, const string& fileName, const string& ncVarName, const string& identifier = "",
                int index = -1, const string& storageType = "", const string& timeStep = "", const string& start = "", int length = -1,
                int ensembleSize = -1, int ensembleLength = -1, const string& ensembleTimeStep = "", const string& containingDirectory="");

            NetCdfSourceInfo(const string& dataId, const string& fileName, const string& ncVarName, const string& identifier,
                int index, const string& storageType, const TimeStep& timeStep, const ptime& start, int length,
                int ensembleSize, int ensembleLength, const TimeStep& ensembleTimeStep/*, const string& collectionDimensionId*/);

            TimeSeriesSourceInfoImpl * Clone() const;
            bool ApplyRootDir(const string& rootDir);

            SingleTimeSeriesStore<double>* CreateSingleTimeSeriesStore() const;
            EnsembleTimeSeriesStore<double>* CreateEnsembleTimeSeriesStore() const;
            TimeSeriesEnsembleTimeSeriesStore<double>* CreateTimeSeriesEnsembleTimeSeriesStore() const;
            std::map<string, string> GetSerializableConfiguration() const;


            static const string FileKey;
            static const string VarKey;
            static const string IdentifierKey;
            static const string IndexKey;
            static const string TypeKey;
            //static const string TimeStepKey;
            //static const string StartKey;
            //static const string LengthKey;
            //static const string EnsembleSizeKey;
            //static const string EnsembleLengthKey;
            //static const string EnsembleTimeStepKey;
            //static const string FilePatternKey;
            //static const string MappingKey;
            //static const string StorageKey;

            static const string StorageTypeSingleNetcdfFile;
            static const string StorageTypeMultipleNetcdfFiles;


        private:
            string dataId;
            string fileName;
            string ncVarName;
            string identifier;
            //string collectionDimensionId;
            string storageType;
            int index = -1;

            TimeStep timeStep;
            ptime start;
            int length = -1;
            int ensembleSize = -1;
            int ensembleLength = -1;
            TimeStep ensembleTimeStep;
        };

        class DATATYPES_DLL_LIB TimeSeriesLibraryDescription
        {
            friend class TimeSeriesLibrary;
        private:
            std::map < string, TimeSeriesSourceInfo > tsEnsProviders;
            std::map < string, TimeSeriesSourceInfo > singleProviders;
            std::map < string, TimeSeriesSourceInfo > ensProviders;
            TimeSeriesSourceInfo GetInfo(const string& dataId, bool applyRootDir=false) const;
            boost::filesystem::path GetRootDirPath() const;
            string filenameLoadedFrom;
            string dataPath;

        public:

            void AddSingle(const string& dataId, const TimeSeriesSourceInfo& t);
            void AddEnsembleTs(const string& dataId, const TimeSeriesSourceInfo& t);
            void AddTsEnsembleTs(const string& dataId, const TimeSeriesSourceInfo& t);

            boost::filesystem::path GetFullPath(const string& relativePath) const;
            string GetRootDirectory() const;

            vector<string> GetDataIdSingle() const;
            vector<string> GetDataIdEnsembleTs() const;
            vector<string> GetDataIdTsEnsembleTs() const;

            std::map<string, string> GetSerializableConfiguration(const string& dataId, const vector<string>& mandatoryKeys = vector<string>({}) ) const;

            void SetLoadedFileName(const string& fileName);
            void SetDataPath(const string& dataPath);
            string GetDataPath() const;

            SingleTimeSeriesStore<double>* CreateSingleTimeSeriesStore(const string& dataId) const;
            EnsembleTimeSeriesStore<double>* CreateEnsembleTimeSeriesStore(const string& dataId) const;
            TimeSeriesEnsembleTimeSeriesStore<double>* CreateTimeSeriesEnsembleTimeSeriesStore(const string& dataId) const;

        };

        class DATATYPES_DLL_LIB TimeSeriesSourceInfoBuilder
        {
        public:
            virtual bool HandlesStorageType(const string storageType) const = 0;
            virtual void BuildTimeSeriesSource(const string& storageType, const string& dataId, const YAML::Node& storage, TimeSeriesLibraryDescription& targetContainer) const = 0;
        };

        class DATATYPES_DLL_LIB TimeSeriesStoreFactory
        {
        protected:
            TimeSeriesStoreFactory();
        public:
            virtual ~TimeSeriesStoreFactory();
            virtual TimeSeriesEnsembleTimeSeriesStore<double>* CreateTimeSeriesEnsembleTimeSeriesStore(const string& dataId) = 0;
            virtual bool CanCreateTimeSeriesEnsembleTimeSeriesStore(const string& dataId) = 0;
        };

        class DATATYPES_DLL_LIB TimeSeriesLibrary :
            public TimeSeriesProvider<double>,
            public TTimeSeriesLibrary<double>
        {
            
        public:
            TimeSeriesLibrary(TimeSeriesStoreFactory* storeCreator = nullptr);

            TimeSeriesLibrary(const TimeSeriesLibraryDescription& description);

            virtual ~TimeSeriesLibrary();
            void Close();

            TimeSeriesLibrary& operator=(TimeSeriesLibrary&& src);

            TimeSeriesLibrary(TimeSeriesLibrary&& src);

            // Maybe the following,m but may introduce too much coupling with on disk representation with SwiftNetCDFAccess.
            // TTimeSeries<double>* GetSingle(const string& dataId, boost::function<TTimeSeries<double>*(SwiftNetCDFAccess * dataAccess)> tsTransform);

            TTimeSeries<double>* GetSingle(const string& dataId, boost::function<TTimeSeries<double>*(TTimeSeries<double>*)>& tsTransform);

            vector<string> GetIdentifiers() const;

            vector<string> GetIdentifiers(const string& dataId) const;

            string GetDataSummary(const string& dataId);

            vector<DataDimensionDescriptor> GetDataDimensionsDescription(const string& dataId);

            TTimeSeries<double>* GetSingle(const string& dataId);

            MultiTimeSeries<TTimeSeries<double>*>* GetCollection(const string& dataId);

            // * \brief Gets a provider, a facade to a collection of time series.
            // *
            // * \param dataId  Identifier for the data.
            // *
            // * \return    the time series provider.
            // */
            //TimeSeriesProvider<double>* GetProvider(const string& dataId);

            TTimeSeries<double>* GetSingle(const string& dataId, const string& collectionIdentifier);

            MultiTimeSeries<TTimeSeries<double>*>* GetEnsemble(const string& dataId, const string& dataItemIdentifier);

            MultiTimeSeries<TTimeSeries<double>*>* GetEnsembleTimeSeries(const string& dataId);

            MultiTimeSeries<TTimeSeries<double>*>* GetAllTimeSeries(const string& dataId);

            EnsembleForecastTimeSeries<TTimeSeries<double>>* GetTimeSeriesEnsembleTimeSeries(const string& dataId);

            void AddSource(const string& dataId, SingleTimeSeriesStore<double>* store);

            void AddSource(const string& dataId, EnsembleTimeSeriesStore<double>* store);

            void AddSource(const string& dataId, TimeSeriesEnsembleTimeSeriesStore<double>* dataAccess);

            bool CanCreateTimeSeriesEnsembleSeriesStore(const string& dataId);

            void CreateTimeSeriesEnsembleSeriesStore(const string& dataId);

        private:
            template<typename U>
            static bool hasKey(const std::map<string, U>& m, const string& dataId)
            {
                return m.find(dataId) != m.end();
            }

            std::map < string, TimeSeriesEnsembleTimeSeriesStore<double>* > tsEnsTimeSeriesProviders;
            std::map < string, EnsembleTimeSeriesStore<double>* > ensTimeSeriesProviders;
            std::map < string, SingleTimeSeriesStore<double>* > timeSeriesProviders;

            SingleTimeSeriesStore<double> * GetSeriesInformation(const string& dataId);

            EnsembleTimeSeriesStore<double> * GetEnsembleSeriesInformation(const string& dataId);

            bool IsDataIdTsEnsemble(const string& dataId);
            bool IsDataIdEnsemble(const string& dataId);
            bool IsDataIdSingle(const string& dataId);

            TimeSeriesEnsembleTimeSeriesStore<double> * GetTimeSeriesEnsembleSeriesInformation(const string& dataId);

            SingleTimeSeriesStore<double>* CreateTsSource(const TimeSeriesSourceInfo& desc);
            EnsembleTimeSeriesStore<double>* CreateEnsTsSource(const TimeSeriesSourceInfo& desc);
            TimeSeriesEnsembleTimeSeriesStore<double>* CreateTsEnsTsSource(const TimeSeriesSourceInfo& desc);

            TimeSeriesStoreFactory* storeCreator = nullptr;
        };
    }
}
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000
