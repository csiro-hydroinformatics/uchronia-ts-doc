---
title: datatypes/datatypes_test_helpers.h

---

# datatypes/datatypes_test_helpers.h



## Namespaces

| Name           |
| -------------- |
| **[datatypes](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes/)**  |
| **[datatypes::tests](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1tests/)**  |

## Classes

|                | Name           |
| -------------- | -------------- |
| class | **[datatypes::tests::FileSystemHelper](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1FileSystemHelper/)**  |
| class | **[datatypes::tests::TempFileCleaner](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TempFileCleaner/)**  |
| class | **[datatypes::tests::TestDataLocationHelper](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/)**  |
| class | **[datatypes::tests::TestSingleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/)**  |
| class | **[datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/)** <br>A time series store for unit tests.  |
| class | **[datatypes::tests::TestEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestEnsembleTimeSeriesStore/)**  |
| class | **[datatypes::tests::TestTimeSeriesStoreFactory](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesStoreFactory/)**  |




## Source code

```cpp
#pragma once

#include "datatypes/common.h"
#include "datatypes/time_series_store.hpp"

using namespace datatypes::timeseries;

namespace datatypes {
    namespace tests {

        template<typename T>
        bool AreEqual(const vector<T>& a, const vector<T>& b, bool strict = false, double tolerance = 1e-12)
        {
            size_t lengthA = a.size();
            size_t lengthB = b.size();

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

        class DATATYPES_DLL_LIB FileSystemHelper {
        public:
            static boost::filesystem::path GetTempFile(const string& format = "%%%%%%%%%%%%.tmp");
            static boost::filesystem::path GetTempDir(const string& format = "%%%%%%%%%%%%");
            static void Remove(const boost::filesystem::path& p);
            static void Remove(const string& p);
            static bool Exists(const string& p);
            static bool Exists(const boost::filesystem::path& p);
        };

        class DATATYPES_DLL_LIB TempFileCleaner
        {
        public:
            string uri;
            TempFileCleaner(const string uri);
            ~TempFileCleaner();
        };

        class DATATYPES_DLL_LIB TestDataLocationHelper
        {
        public:
            static string ReadEnvironmentVariable(const string& envVar);
            static string BuildPath(const vector<string>& folders);
            static TimeSeriesLibrary CreateEnsembleTimeSeriesLibrary(string& rainObsId, string& petObsId, string& rainFcastId, string& petFcastId);
            static TimeSeriesLibrary GetTestTimeSeriesLibrary();
            static vector<string> TestTsLibraryIdentifiers();
            static TimeSeriesLibrary* CreateTestTimeSeriesLibrary();
            static void MakeTestTimeSeriesLibrary(TimeSeriesLibrary& dataLibrary);

            const static string kVarSingleStation;
            const static string kVarMultiStations;
            const static string kFileSingleStation;
            const static string kFileMultiStations;


            const static string kFileAllDataCases;
            const static string kVar1FcastEns;
            const static string kVar2FcastEns;
            const static string kVar1Obs;
            const static string kVar2Obs;
            const static string kVar1Ens;
            const static string kVar2Ens;

            const static string kIdentifier1FcastEns;
            const static string kIdentifier2FcastEns;
            const static string kIdentifier1Obs;
            const static string kIdentifier2Obs;
            const static string kIdentifier1Ens;
            const static string kIdentifier2Ens;


            const static string kSingleStationId;
            const static string kStationIdOne;
            const static string kStationIdTwo;
            const static size_t kTimeSeriesLength;

            static vector<string> TestStationIds();
        };

        class DATATYPES_DLL_LIB TestSingleTimeSeriesStore :
            public SingleTimeSeriesStore<double>
        {
        public:

            TestSingleTimeSeriesStore(const vector<double>& values, const ptime& startDate, const TimeStep& timeStep = TimeStep::GetHourly());
            TestSingleTimeSeriesStore(const TimeSeries& series);
            string GetDataSummary() const;
            vector<DataDimensionDescriptor> GetDataDimensionsDescription() const;
            TTimeSeries<double>* Read();
            TTimeSeries<double>* Read(const string& blah);
            MultiTimeSeries<TTimeSeries<double>*>* ReadAllCollection();
            std::vector<std::string> GetIdentifiers() const;
        private:
            TTimeSeries<double> innerTs;

        };

        class DATATYPES_DLL_LIB TestTimeSeriesEnsembleTimeSeriesStore : public WritableTimeSeriesEnsembleTimeSeriesStore<double>
        {
        public:

            using T = double;
            using SeriesType = CommonTypes<T>::SeriesType;
            using PtrSeriesType = CommonTypes<T>::PtrSeriesType;
            using EnsemblePtrType = CommonTypes<T>::EnsemblePtrType;
            using PtrEnsemblePtrType = CommonTypes<T>::PtrEnsemblePtrType;
            using TSeriesEnsemblePtrType = CommonTypes<T>::TSeriesEnsemblePtrType;
            using PtrTSeriesEnsemblePtrType = CommonTypes<T>::PtrTSeriesEnsemblePtrType;

            ~TestTimeSeriesEnsembleTimeSeriesStore();
            TestTimeSeriesEnsembleTimeSeriesStore(const string& id = "");
            TestTimeSeriesEnsembleTimeSeriesStore(const TSeriesEnsemblePtrType& ensFts, const string& id = "");
            PtrTSeriesEnsemblePtrType GetSeries(const string& dataId);
            PtrTSeriesEnsemblePtrType GetSeriesTestBackend(const string& dataId);

            PtrEnsemblePtrType Read(const std::string& ensembleIdentifier);
            size_t GetLength() const;
            ptime GetStart() const;
            //vector<string> GetItemIdentifiers() const;
            string GetDataSummary() const;
            vector<DataDimensionDescriptor> GetDataDimensionsDescription() const;
            TimeStep GetTimeStep() const;

            bool IsActive();
            void Allocate(size_t length, PtrEnsemblePtrType value);
            void AllocateValues(const vector<PtrEnsemblePtrType>& values);
            void SetSeries(const string& dataId, PtrTSeriesEnsemblePtrType value);
            void SetItem(const string& dataId, size_t index, PtrEnsemblePtrType value);
            void SetItem(const string& dataId, size_t index, const EnsemblePtrType& value);
            //EnsemblePtrType Read(const string& ensembleIdentifier) = 0;
            void SetLength(size_t);

            void SetStart(ptime);

            //vector<string> GetItemIdentifiers() const = 0;
            void SetTimeStep(const TimeStep&);

            PtrEnsemblePtrType GetItem(const string& dataId, size_t fcastIndex) override;
            PtrSeriesType GetItem(const string& dataId, size_t fcastIndex, size_t ensIndex) override;
            size_t GetEnsembleSize(const string& dataId, size_t fcastIndex) const override;

        private:
            PtrTSeriesEnsemblePtrType GetFirstTsEnsTs() const;
            PtrTSeriesEnsemblePtrType CreateNewSeries();
            std::map<string, PtrTSeriesEnsemblePtrType> ensFcastsSeries;
            bool allowDynamicCreation = false;
            //PtrTSeriesEnsemblePtrType ensFts;
            //string id;
        };

        class DATATYPES_DLL_LIB TestEnsembleTimeSeriesStore : public EnsembleTimeSeriesStore<double>
        {
        public:
            TestEnsembleTimeSeriesStore(const MultiTimeSeries<>& data);
            MultiTimeSeries<TTimeSeries<double>*>* Read();
            string GetDataSummary() const;
            vector<DataDimensionDescriptor> GetDataDimensionsDescription() const;
        private:
            MultiTimeSeries<> data;
        };

        class DATATYPES_DLL_LIB TestTimeSeriesStoreFactory :
            public TimeSeriesStoreFactory
        {
        public:
            TestTimeSeriesStoreFactory();
            ~TestTimeSeriesStoreFactory();
            TimeSeriesEnsembleTimeSeriesStore<double>* CreateTimeSeriesEnsembleTimeSeriesStore(const string& dataId);
            bool CanCreateTimeSeriesEnsembleTimeSeriesStore(const string& dataId);
        };

    }
}
```


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000
