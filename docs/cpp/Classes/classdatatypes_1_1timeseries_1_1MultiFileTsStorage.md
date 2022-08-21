---
title: datatypes::timeseries::MultiFileTsStorage
summary: An implementation of StoragePolicy such that the content of a time series is spread amongst several files. 

---

# datatypes::timeseries::MultiFileTsStorage



An implementation of [StoragePolicy]() such that the content of a time series is spread amongst several files.  [More...](#detailed-description)


`#include <time_series_io.hpp>`

Inherits from [datatypes::timeseries::StoragePolicy< T >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/), [datatypes::timeseries::TimeSeriesInfoProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/)

## Public Types

|                | Name           |
| -------------- | -------------- |
| typedef std::remove_pointer< T >::type::ElementType | **[ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#typedef-elementtype)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[MultiFileTsStorage](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-multifiletsstorage)**(const [MultiFileTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/)< [ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#typedef-elementtype) > & storage, const string & dataIdentifier, bool readOnly =true) |
| virtual bool | **[ReadOnly](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-readonly)**() override |
| virtual size_t | **[Size](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-size)**() const |
| void | **[ReserveVectorData](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-reservevectordata)**(size_t length) |
| virtual void | **[Allocate](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-allocate)**(size_t length, T value) |
| virtual void | **[AllocateValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-allocatevalues)**(size_t length, const T * values) |
| virtual void | **[AllocateValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-allocatevalues)**(const vector< T > & values) |
| virtual void | **[CopyTo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-copyto)**(vector< T > & dest, size_t from =0, size_t to =-1) const |
| virtual T & | **[operator[]](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-operator[])**(const size_t i) |
| virtual const T & | **[operator[]](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-operator[])**(const size_t i) const |
| virtual [StoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)< T > * | **[Clone](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-clone)**() const |
| virtual size_t | **[GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-getlength)**() const |
| virtual [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-gettimestep)**() const override |
| virtual ptime | **[GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-getstart)**() const override |
| virtual void | **[SetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-settimestep)**(const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & tStep) override |
| virtual void | **[SetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#function-setstart)**(const ptime & start) override |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| vector< T > | **[data](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#variable-data)**  |
| bool | **[readOnly](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/#variable-readonly)**  |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::StoragePolicy< T >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~StoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-~storagepolicy)**() |

**Protected Functions inherited from [datatypes::timeseries::StoragePolicy< T >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)**

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
template <typename T >
class datatypes::timeseries::MultiFileTsStorage;
```

An implementation of [StoragePolicy]() such that the content of a time series is spread amongst several files. 

**Template Parameters**: 

  * **T** The type of each data item this can handle. 

## Public Types Documentation

### typedef ElementType

```cpp
typedef std::remove_pointer<T>::type::ElementType datatypes::timeseries::MultiFileTsStorage< T >::ElementType;
```


## Public Functions Documentation

### function MultiFileTsStorage

```cpp
inline MultiFileTsStorage(
    const MultiFileTimeSeriesEnsembleTimeSeriesStore< ElementType > & storage,
    const string & dataIdentifier,
    bool readOnly =true
)
```


### function ReadOnly

```cpp
inline virtual bool ReadOnly() override
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::ReadOnly](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-readonly)


### function Size

```cpp
inline virtual size_t Size() const
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::Size](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-size)


### function ReserveVectorData

```cpp
inline void ReserveVectorData(
    size_t length
)
```


### function Allocate

```cpp
inline virtual void Allocate(
    size_t length,
    T value
)
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::Allocate](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-allocate)


### function AllocateValues

```cpp
inline virtual void AllocateValues(
    size_t length,
    const T * values
)
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::AllocateValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-allocatevalues)


### function AllocateValues

```cpp
inline virtual void AllocateValues(
    const vector< T > & values
)
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::AllocateValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-allocatevalues)


### function CopyTo

```cpp
inline virtual void CopyTo(
    vector< T > & dest,
    size_t from =0,
    size_t to =-1
) const
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::CopyTo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-copyto)


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


## Public Attributes Documentation

### variable data

```cpp
vector< T > data;
```


### variable readOnly

```cpp
bool readOnly = true;
```


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000