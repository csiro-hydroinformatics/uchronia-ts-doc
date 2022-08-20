---
title: datatypes::timeseries::StoragePolicy
summary: An interface for classes that can handle the storage of data for time series. 

---

# datatypes::timeseries::StoragePolicy



An interface for classes that can handle the storage of data for time series.  [More...](#detailed-description)


`#include <time_series_strategies.hpp>`

Inherits from [datatypes::timeseries::TimeSeriesInfoProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/)

Inherited by [datatypes::timeseries::MultiFileTsStorage< T >](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual | **[~StoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-~storagepolicy)**() |
| virtual void | **[CopyTo](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-copyto)**(vector< T > & dest, size_t from =0, size_t to =-1) const =0 |
| virtual size_t | **[Size](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-size)**() const =0 |
| virtual void | **[Allocate](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-allocate)**(size_t length, T value) =0 |
| virtual void | **[AllocateValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-allocatevalues)**(size_t length, const T * values) =0 |
| virtual void | **[AllocateValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-allocatevalues)**(const vector< T > & values) =0 |
| virtual const T & | **[operator[]](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-operator[])**(const size_t i) const =0 |
| virtual T & | **[operator[]](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-operator[])**(const size_t i) =0 |
| virtual [StoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/) * | **[Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-clone)**() const =0 |
| virtual void | **[CopyTo](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-copyto)**([StoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)< T > & dest) |
| virtual bool | **[ReadOnly](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-readonly)**() |
| virtual [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-gettimestep)**() const =0 |
| virtual ptime | **[GetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-getstart)**() const =0 |
| virtual void | **[SetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-settimestep)**(const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & tStep) =0 |
| virtual void | **[SetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-setstart)**(const ptime & start) =0 |

## Protected Functions

|                | Name           |
| -------------- | -------------- |
| | **[StoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-storagepolicy)**(const [StoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/) & src) |
| | **[StoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-storagepolicy)**() |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::TimeSeriesInfoProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeSeriesInfoProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/#function-~timeseriesinfoprovider)**() |
| virtual size_t | **[GetLength](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/#function-getlength)**() const =0 |


## Detailed Description

```cpp
template <typename T >
class datatypes::timeseries::StoragePolicy;
```

An interface for classes that can handle the storage of data for time series. 

**Template Parameters**: 

  * **T** The type of each data item this can handle, e.g. a double, float, or even pointers. 




```
     The storage of time series data is using a software pattern usually named Strategy,
     or Policy. The word "policy" is more of a legacy (time series storage used to be 
     template-arguments for time series). The purpose is to delegate the details of the 
     data handling (memory, file, and data caching between different types of storages.) 
     out of TTimeSeries objects.
```

## Public Functions Documentation

### function ~StoragePolicy

```cpp
inline virtual ~StoragePolicy()
```


### function CopyTo

```cpp
virtual void CopyTo(
    vector< T > & dest,
    size_t from =0,
    size_t to =-1
) const =0
```


**Reimplemented by**: [datatypes::timeseries::EagerWriter::CopyTo](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-copyto), [datatypes::timeseries::MultiFileTsStorage::CopyTo](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-copyto)


### function Size

```cpp
virtual size_t Size() const =0
```


**Reimplemented by**: [datatypes::timeseries::EagerWriter::Size](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-size), [datatypes::timeseries::MultiFileTsStorage::Size](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-size), [datatypes::timeseries::StlVectorStorage::Size](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-size), [datatypes::timeseries::SharedVectorStorage::Size](/cpp/Classes/classdatatypes_1_1timeseries_1_1SharedVectorStorage/#function-size), [datatypes::timeseries::MemoryCachingStorageWriter::Size](/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-size)


### function Allocate

```cpp
virtual void Allocate(
    size_t length,
    T value
) =0
```


**Reimplemented by**: [datatypes::timeseries::EagerWriter::Allocate](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-allocate), [datatypes::timeseries::MultiFileTsStorage::Allocate](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-allocate)


### function AllocateValues

```cpp
virtual void AllocateValues(
    size_t length,
    const T * values
) =0
```


**Reimplemented by**: [datatypes::timeseries::EagerWriter::AllocateValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-allocatevalues), [datatypes::timeseries::MultiFileTsStorage::AllocateValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-allocatevalues)


### function AllocateValues

```cpp
virtual void AllocateValues(
    const vector< T > & values
) =0
```


**Reimplemented by**: [datatypes::timeseries::EagerWriter::AllocateValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-allocatevalues), [datatypes::timeseries::MultiFileTsStorage::AllocateValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-allocatevalues)


### function operator[]

```cpp
virtual const T & operator[](
    const size_t i
) const =0
```


**Reimplemented by**: [datatypes::timeseries::EagerWriter::operator[]](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-operator[]), [datatypes::timeseries::MultiFileTsStorage::operator[]](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-operator[]), [datatypes::timeseries::StlVectorStorage::operator[]](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-operator[]), [datatypes::timeseries::SharedVectorStorage::operator[]](/cpp/Classes/classdatatypes_1_1timeseries_1_1SharedVectorStorage/#function-operator[]), [datatypes::timeseries::MemoryCachingStorageWriter::operator[]](/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-operator[])


### function operator[]

```cpp
virtual T & operator[](
    const size_t i
) =0
```


**Reimplemented by**: [datatypes::timeseries::EagerWriter::operator[]](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-operator[]), [datatypes::timeseries::MultiFileTsStorage::operator[]](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-operator[]), [datatypes::timeseries::StlVectorStorage::operator[]](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-operator[]), [datatypes::timeseries::SharedVectorStorage::operator[]](/cpp/Classes/classdatatypes_1_1timeseries_1_1SharedVectorStorage/#function-operator[]), [datatypes::timeseries::MemoryCachingStorageWriter::operator[]](/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-operator[])


### function Clone

```cpp
virtual StoragePolicy * Clone() const =0
```


**Reimplemented by**: [datatypes::timeseries::EagerWriter::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-clone), [datatypes::timeseries::MultiFileTsStorage::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-clone), [datatypes::timeseries::StlVectorStorage::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-clone), [datatypes::timeseries::SharedVectorStorage::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1SharedVectorStorage/#function-clone), [datatypes::timeseries::MemoryCachingStorageWriter::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-clone)


### function CopyTo

```cpp
inline virtual void CopyTo(
    StoragePolicy< T > & dest
)
```


### function ReadOnly

```cpp
inline virtual bool ReadOnly()
```


**Reimplemented by**: [datatypes::timeseries::EagerWriter::ReadOnly](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-readonly), [datatypes::timeseries::MultiFileTsStorage::ReadOnly](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-readonly)


### function GetTimeStep

```cpp
virtual TimeStep GetTimeStep() const =0
```


**Reimplements**: [datatypes::timeseries::TimeSeriesInfoProvider::GetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/#function-gettimestep)


**Reimplemented by**: [datatypes::timeseries::EagerWriter::GetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-gettimestep), [datatypes::timeseries::MultiFileTsStorage::GetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-gettimestep), [datatypes::timeseries::StlVectorStorage::GetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-gettimestep), [datatypes::timeseries::SharedVectorStorage::GetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1SharedVectorStorage/#function-gettimestep), [datatypes::timeseries::MemoryCachingStorageWriter::GetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-gettimestep)


### function GetStart

```cpp
virtual ptime GetStart() const =0
```


**Reimplements**: [datatypes::timeseries::TimeSeriesInfoProvider::GetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/#function-getstart)


**Reimplemented by**: [datatypes::timeseries::EagerWriter::GetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-getstart), [datatypes::timeseries::MultiFileTsStorage::GetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-getstart), [datatypes::timeseries::StlVectorStorage::GetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-getstart), [datatypes::timeseries::SharedVectorStorage::GetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1SharedVectorStorage/#function-getstart), [datatypes::timeseries::MemoryCachingStorageWriter::GetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-getstart)


### function SetTimeStep

```cpp
virtual void SetTimeStep(
    const TimeStep & tStep
) =0
```


**Reimplemented by**: [datatypes::timeseries::EagerWriter::SetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-settimestep), [datatypes::timeseries::MultiFileTsStorage::SetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-settimestep), [datatypes::timeseries::StlVectorStorage::SetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-settimestep), [datatypes::timeseries::SharedVectorStorage::SetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1SharedVectorStorage/#function-settimestep), [datatypes::timeseries::MemoryCachingStorageWriter::SetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-settimestep)


### function SetStart

```cpp
virtual void SetStart(
    const ptime & start
) =0
```


**Reimplemented by**: [datatypes::timeseries::EagerWriter::SetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-setstart), [datatypes::timeseries::MultiFileTsStorage::SetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-setstart), [datatypes::timeseries::StlVectorStorage::SetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-setstart), [datatypes::timeseries::SharedVectorStorage::SetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1SharedVectorStorage/#function-setstart), [datatypes::timeseries::MemoryCachingStorageWriter::SetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-setstart)


## Protected Functions Documentation

### function StoragePolicy

```cpp
inline StoragePolicy(
    const StoragePolicy & src
)
```


### function StoragePolicy

```cpp
inline StoragePolicy()
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000