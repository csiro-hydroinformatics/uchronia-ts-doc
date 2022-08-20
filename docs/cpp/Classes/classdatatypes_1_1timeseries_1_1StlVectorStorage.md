---
title: datatypes::timeseries::StlVectorStorage

---

# datatypes::timeseries::StlVectorStorage



 [More...](#detailed-description)


`#include <time_series_strategies.hpp>`

Inherits from [datatypes::timeseries::StoragePolicy< double >](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/), [datatypes::timeseries::TimeSeriesInfoProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[StlVectorStorage](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-stlvectorstorage)**() |
| virtual size_t | **[Size](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-size)**() const |
| virtual size_t | **[GetLength](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-getlength)**() const |
| void | **[Allocate](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-allocate)**(size_t length, T value) |
| void | **[AllocateValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-allocatevalues)**(size_t length, const T * values) |
| void | **[AllocateValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-allocatevalues)**(const vector< T > & values) |
| void | **[CopyTo](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-copyto)**(vector< T > & dest, size_t from =0, size_t to =-1) const |
| virtual T & | **[operator[]](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-operator[])**(const size_t i) |
| virtual const T & | **[operator[]](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-operator[])**(const size_t i) const |
| virtual [StoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)< T > * | **[Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-clone)**() const |
| virtual [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-gettimestep)**() const override |
| virtual ptime | **[GetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-getstart)**() const override |
| virtual void | **[SetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-settimestep)**(const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & tStep) override |
| virtual void | **[SetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/#function-setstart)**(const ptime & start) override |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::StoragePolicy< double >](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~StoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-~storagepolicy)**() |
| virtual bool | **[ReadOnly](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-readonly)**() |

**Protected Functions inherited from [datatypes::timeseries::StoragePolicy< double >](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)**

|                | Name           |
| -------------- | -------------- |
| | **[StoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-storagepolicy)**(const [StoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/) & src) |
| | **[StoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-storagepolicy)**() |

**Public Functions inherited from [datatypes::timeseries::TimeSeriesInfoProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeSeriesInfoProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/#function-~timeseriesinfoprovider)**() |


## Detailed Description

```cpp
template <typename T  =double>
class datatypes::timeseries::StlVectorStorage;
```

## Public Functions Documentation

### function StlVectorStorage

```cpp
inline StlVectorStorage()
```


### function Size

```cpp
inline virtual size_t Size() const
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::Size](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-size)


### function GetLength

```cpp
inline virtual size_t GetLength() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesInfoProvider::GetLength](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/#function-getlength)


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


**Reimplements**: [datatypes::timeseries::StoragePolicy::operator[]](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-operator[])


### function operator[]

```cpp
inline virtual const T & operator[](
    const size_t i
) const
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::operator[]](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-operator[])


### function Clone

```cpp
inline virtual StoragePolicy< T > * Clone() const
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-clone)


### function GetTimeStep

```cpp
inline virtual TimeStep GetTimeStep() const override
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::GetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-gettimestep)


### function GetStart

```cpp
inline virtual ptime GetStart() const override
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::GetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-getstart)


### function SetTimeStep

```cpp
inline virtual void SetTimeStep(
    const TimeStep & tStep
) override
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::SetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-settimestep)


### function SetStart

```cpp
inline virtual void SetStart(
    const ptime & start
) override
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::SetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-setstart)


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000