---
title: datatypes::timeseries::MemoryCachingStorageWriter

---

# datatypes::timeseries::MemoryCachingStorageWriter



 [More...](#detailed-description)


`#include <time_series_strategies.hpp>`

Inherits from [datatypes::timeseries::StoragePolicy< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/), [datatypes::timeseries::TimeSeriesInfoProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[MemoryCachingStorageWriter](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-memorycachingstoragewriter)**(size_t bufferSize, [StoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)< T > * wrappedStorage) |
| T & | **[GetWindowItem](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-getwindowitem)**(size_t i) |
| T & | **[GetBackendItem](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-getbackenditem)**(size_t i) |
| virtual size_t | **[Size](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-size)**() const |
| virtual size_t | **[GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-getlength)**() const |
| virtual [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-gettimestep)**() const override |
| virtual ptime | **[GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-getstart)**() const override |
| virtual void | **[SetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-settimestep)**(const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & tStep) override |
| virtual void | **[SetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-setstart)**(const ptime & start) override |
| void | **[ResetBuffer](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-resetbuffer)**() |
| void | **[Allocate](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-allocate)**(size_t length, T value) |
| void | **[AllocateValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-allocatevalues)**(size_t length, const T * values) |
| void | **[AllocateValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-allocatevalues)**(const vector< T > & values) |
| void | **[CopyTo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-copyto)**(vector< T > & dest, size_t from =0, size_t to =-1) const |
| virtual T & | **[operator[]](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-operator[])**(const size_t i) |
| virtual const T & | **[operator[]](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-operator[])**(const size_t i) const |
| virtual [StoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)< T > * | **[Clone](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-clone)**() const |

## Protected Functions

|                | Name           |
| -------------- | -------------- |
| | **[MemoryCachingStorageWriter](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/#function-memorycachingstoragewriter)**(const [MemoryCachingStorageWriter](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/) & src) |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::StoragePolicy< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~StoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-~storagepolicy)**() |
| virtual bool | **[ReadOnly](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-readonly)**() |

**Protected Functions inherited from [datatypes::timeseries::StoragePolicy< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)**

|                | Name           |
| -------------- | -------------- |
| | **[StoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-storagepolicy)**(const [StoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/) & src) |
| | **[StoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-storagepolicy)**() |

**Public Functions inherited from [datatypes::timeseries::TimeSeriesInfoProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeSeriesInfoProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/#function-~timeseriesinfoprovider)**() |


## Detailed Description

```cpp
template <typename T  =double>
class datatypes::timeseries::MemoryCachingStorageWriter;
```

## Public Functions Documentation

### function MemoryCachingStorageWriter

```cpp
inline MemoryCachingStorageWriter(
    size_t bufferSize,
    StoragePolicy< T > * wrappedStorage
)
```


### function GetWindowItem

```cpp
inline T & GetWindowItem(
    size_t i
)
```


### function GetBackendItem

```cpp
inline T & GetBackendItem(
    size_t i
)
```


### function Size

```cpp
inline virtual size_t Size() const
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::Size](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-size)


### function GetLength

```cpp
inline virtual size_t GetLength() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesInfoProvider::GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/#function-getlength)


### function GetTimeStep

```cpp
inline virtual TimeStep GetTimeStep() const override
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-gettimestep)


### function GetStart

```cpp
inline virtual ptime GetStart() const override
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-getstart)


### function SetTimeStep

```cpp
inline virtual void SetTimeStep(
    const TimeStep & tStep
) override
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::SetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-settimestep)


### function SetStart

```cpp
inline virtual void SetStart(
    const ptime & start
) override
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::SetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-setstart)


### function ResetBuffer

```cpp
inline void ResetBuffer()
```


### function Allocate

```cpp
inline void Allocate(
    size_t length,
    T value
)
```


### function AllocateValues

```cpp
inline void AllocateValues(
    size_t length,
    const T * values
)
```


### function AllocateValues

```cpp
inline void AllocateValues(
    const vector< T > & values
)
```


### function CopyTo

```cpp
inline void CopyTo(
    vector< T > & dest,
    size_t from =0,
    size_t to =-1
) const
```


### function operator[]

```cpp
inline virtual T & operator[](
    const size_t i
)
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::operator[]](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-operator[])


### function operator[]

```cpp
inline virtual const T & operator[](
    const size_t i
) const
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::operator[]](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-operator[])


### function Clone

```cpp
inline virtual StoragePolicy< T > * Clone() const
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::Clone](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-clone)


## Protected Functions Documentation

### function MemoryCachingStorageWriter

```cpp
inline MemoryCachingStorageWriter(
    const MemoryCachingStorageWriter & src
)
```


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000