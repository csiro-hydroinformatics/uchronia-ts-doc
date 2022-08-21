---
title: datatypes::timeseries::TimeSeriesInfoProvider
summary: An interface definition for classes that can provide essential time series temporal characteristics. 

---

# datatypes::timeseries::TimeSeriesInfoProvider



An interface definition for classes that can provide essential time series temporal characteristics. 


`#include <time_step.h>`

Inherited by [datatypes::timeseries::StoragePolicy< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/), [datatypes::timeseries::StoragePolicy< StorageType >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/), [datatypes::timeseries::StoragePolicy< T >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/), [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore< T >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeSeriesInfoProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/#function-~timeseriesinfoprovider)**() |
| virtual size_t | **[GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/#function-getlength)**() const =0 |
| virtual [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/#function-gettimestep)**() const =0 |
| virtual ptime | **[GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/#function-getstart)**() const =0 |

## Public Functions Documentation

### function ~TimeSeriesInfoProvider

```cpp
virtual ~TimeSeriesInfoProvider()
```


### function GetLength

```cpp
virtual size_t GetLength() const =0
```


**Reimplemented by**: [datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getlength), [datatypes::timeseries::EagerWriter::GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-getlength), [datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore::GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-getlength), [datatypes::timeseries::MultiFileTsStorage::GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-getlength), [datatypes::timeseries::MultiFileTimeSeriesEnsembleTimeSeriesStore::GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-getlength), [datatypes::timeseries::MultiFileTimeSeriesEnsembleTimeSeriesStore::GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-getlength), [datatypes::timeseries::StlVectorStorage::GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-getlength), [datatypes::timeseries::SharedVectorStorage::GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SharedVectorStorage/#function-getlength), [datatypes::timeseries::MemoryCachingStorageWriter::GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-getlength), [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getlength)


### function GetTimeStep

```cpp
virtual TimeStep GetTimeStep() const =0
```


**Reimplemented by**: [datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-gettimestep), [datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore::GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-gettimestep), [datatypes::timeseries::MultiFileTimeSeriesEnsembleTimeSeriesStore::GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-gettimestep), [datatypes::timeseries::MultiFileTimeSeriesEnsembleTimeSeriesStore::GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-gettimestep), [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-gettimestep), [datatypes::timeseries::StoragePolicy::GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-gettimestep), [datatypes::timeseries::EagerWriter::GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-gettimestep), [datatypes::timeseries::MultiFileTsStorage::GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-gettimestep), [datatypes::timeseries::StlVectorStorage::GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-gettimestep), [datatypes::timeseries::SharedVectorStorage::GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SharedVectorStorage/#function-gettimestep), [datatypes::timeseries::MemoryCachingStorageWriter::GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-gettimestep), [datatypes::timeseries::StoragePolicy::GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-gettimestep), [datatypes::timeseries::StoragePolicy::GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-gettimestep)


### function GetStart

```cpp
virtual ptime GetStart() const =0
```


**Reimplemented by**: [datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getstart), [datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore::GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-getstart), [datatypes::timeseries::MultiFileTimeSeriesEnsembleTimeSeriesStore::GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-getstart), [datatypes::timeseries::MultiFileTimeSeriesEnsembleTimeSeriesStore::GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-getstart), [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getstart), [datatypes::timeseries::StoragePolicy::GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-getstart), [datatypes::timeseries::EagerWriter::GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-getstart), [datatypes::timeseries::MultiFileTsStorage::GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-getstart), [datatypes::timeseries::StlVectorStorage::GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-getstart), [datatypes::timeseries::SharedVectorStorage::GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SharedVectorStorage/#function-getstart), [datatypes::timeseries::MemoryCachingStorageWriter::GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-getstart), [datatypes::timeseries::StoragePolicy::GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-getstart), [datatypes::timeseries::StoragePolicy::GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-getstart)


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000