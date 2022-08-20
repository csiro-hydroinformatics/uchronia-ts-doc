---
title: datatypes::timeseries::EagerWriter

---

# datatypes::timeseries::EagerWriter



 [More...](#detailed-description)


`#include <time_series_io.hpp>`

Inherits from [datatypes::timeseries::StoragePolicy< StorageType >](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/), [datatypes::timeseries::TimeSeriesInfoProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/)

## Public Types

|                | Name           |
| -------------- | -------------- |
| using typename [TimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)< double >::[EnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#using-ensembleptrtype) | **[EnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#using-ensembleptrtype)**  |
| using StorageType | **[PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#using-ptrensembleptrtype)**  |
| using typename EnsemblePtrType::ElementType | **[ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#using-elementtype)**  |
| using EnsemblePtrType::ItemType | **[TsType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#using-tstype)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[EagerWriter](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-eagerwriter)**([WritableTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/)< [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#using-elementtype) > * store) |
| | **[EagerWriter](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-eagerwriter)**(const [EagerWriter](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/) & src) |
| virtual bool | **[ReadOnly](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-readonly)**() override |
| virtual size_t | **[Size](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-size)**() const |
| virtual void | **[Allocate](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-allocate)**(size_t length, [PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#using-ptrensembleptrtype) value) |
| virtual void | **[AllocateValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-allocatevalues)**(size_t length, const [PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#using-ptrensembleptrtype) * values) |
| virtual void | **[AllocateValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-allocatevalues)**(const vector< [PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#using-ptrensembleptrtype) > & values) |
| virtual void | **[CopyTo](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-copyto)**(vector< [PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#using-ptrensembleptrtype) > & dest, size_t from =0, size_t to =-1) const |
| [PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#using-ptrensembleptrtype) & | **[GetProxy](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-getproxy)**(const size_t i) |
| virtual [PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#using-ptrensembleptrtype) & | **[operator[]](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-operator[])**(const size_t i) |
| virtual const [PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#using-ptrensembleptrtype) & | **[operator[]](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-operator[])**(const size_t i) const |
| virtual [StoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)< [PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#using-ptrensembleptrtype) > * | **[Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-clone)**() const |
| virtual size_t | **[GetLength](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-getlength)**() const |
| virtual [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-gettimestep)**() const override |
| virtual ptime | **[GetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-getstart)**() const override |
| virtual void | **[SetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-settimestep)**(const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & tStep) override |
| virtual void | **[SetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/#function-setstart)**(const ptime & start) override |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::StoragePolicy< StorageType >](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~StoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-~storagepolicy)**() |

**Protected Functions inherited from [datatypes::timeseries::StoragePolicy< StorageType >](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)**

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
template <typename StorageType >
class datatypes::timeseries::EagerWriter;
```

## Public Types Documentation

### using EnsemblePtrType

```cpp
using datatypes::timeseries::EagerWriter< StorageType >::EnsemblePtrType =  typename TimeSeriesEnsembleTimeSeriesStore<double>::EnsemblePtrType;
```


### using PtrEnsemblePtrType

```cpp
using datatypes::timeseries::EagerWriter< StorageType >::PtrEnsemblePtrType =  StorageType;
```


### using ElementType

```cpp
using datatypes::timeseries::EagerWriter< StorageType >::ElementType =  typename EnsemblePtrType::ElementType;
```


### using TsType

```cpp
using datatypes::timeseries::EagerWriter< StorageType >::TsType =  EnsemblePtrType::ItemType;
```


## Public Functions Documentation

### function EagerWriter

```cpp
inline EagerWriter(
    WritableTimeSeriesEnsembleTimeSeriesStore< ElementType > * store
)
```


### function EagerWriter

```cpp
inline EagerWriter(
    const EagerWriter & src
)
```


### function ReadOnly

```cpp
inline virtual bool ReadOnly() override
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::ReadOnly](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-readonly)


### function Size

```cpp
inline virtual size_t Size() const
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::Size](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-size)


### function Allocate

```cpp
inline virtual void Allocate(
    size_t length,
    PtrEnsemblePtrType value
)
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::Allocate](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-allocate)


### function AllocateValues

```cpp
inline virtual void AllocateValues(
    size_t length,
    const PtrEnsemblePtrType * values
)
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::AllocateValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-allocatevalues)


### function AllocateValues

```cpp
inline virtual void AllocateValues(
    const vector< PtrEnsemblePtrType > & values
)
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::AllocateValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-allocatevalues)


### function CopyTo

```cpp
inline virtual void CopyTo(
    vector< PtrEnsemblePtrType > & dest,
    size_t from =0,
    size_t to =-1
) const
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::CopyTo](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-copyto)


### function GetProxy

```cpp
inline PtrEnsemblePtrType & GetProxy(
    const size_t i
)
```


### function operator[]

```cpp
inline virtual PtrEnsemblePtrType & operator[](
    const size_t i
)
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::operator[]](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-operator[])


### function operator[]

```cpp
inline virtual const PtrEnsemblePtrType & operator[](
    const size_t i
) const
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::operator[]](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-operator[])


### function Clone

```cpp
inline virtual StoragePolicy< PtrEnsemblePtrType > * Clone() const
```


**Reimplements**: [datatypes::timeseries::StoragePolicy::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/#function-clone)


### function GetLength

```cpp
inline virtual size_t GetLength() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesInfoProvider::GetLength](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/#function-getlength)


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