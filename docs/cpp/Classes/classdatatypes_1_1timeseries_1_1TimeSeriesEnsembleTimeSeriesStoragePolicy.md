---
title: datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy

---

# datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy



 [More...](#detailed-description)


`#include <time_series_store.hpp>`

Inherits from [datatypes::timeseries::EnsembleStoragePolicy< TsType >](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)

## Public Types

|                | Name           |
| -------------- | -------------- |
| using double | **[T](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#using-t)**  |
| typedef std::remove_pointer< TsType >::type | **[Type](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-type)**  |
| typedef std::add_pointer< [Type](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-type) >::type | **[PtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-ptrtype)**  |
| typedef Type::ElementType | **[ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-elementtype)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[TimeSeriesEnsembleTimeSeriesStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-timeseriesensembletimeseriesstoragepolicy)**([WritableTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/)< [T](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#using-t) > * store, size_t index) |
| virtual void | **[Reset](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-reset)**(const vector< [PtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-ptrtype) > & values, const ptime & startDate, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| | **[TimeSeriesEnsembleTimeSeriesStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-timeseriesensembletimeseriesstoragepolicy)**(const [TimeSeriesEnsembleTimeSeriesStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/)< TsType > & src) |
| virtual [EnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)< TsType > * | **[Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-clone)**() const |
| | **[~TimeSeriesEnsembleTimeSeriesStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-~timeseriesensembletimeseriesstoragepolicy)**() |
| [TimeSeriesEnsembleTimeSeriesStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/) & | **[operator=](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-operator=)**([TimeSeriesEnsembleTimeSeriesStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/) && src) |
| virtual void | **[ResetSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-resetseries)**(const size_t & numSeries, const size_t & lengthSeries, const ptime & startDate, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| [PtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-ptrtype) | **[GetReplicate](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-getreplicate)**(size_t i) |
| virtual TsType | **[Get](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-get)**(size_t i) |
| virtual [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-elementtype) | **[Get](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-get)**(size_t i, size_t tsIndex) |
| virtual void | **[Set](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-set)**(size_t i, size_t tsIndex, [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-elementtype) val) |
| virtual void | **[Set](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-set)**(size_t i, const [Type](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-type) & val) |
| virtual vector< [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-elementtype) * > * | **[GetValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-getvalues)**() const |
| virtual void | **[CopyTo](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-copyto)**([ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-elementtype) ** dest) const |
| virtual size_t | **[Size](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-size)**() const |
| virtual size_t | **[GetLength](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-getlength)**(size_t i) const |
| virtual void | **[Clear](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-clear)**() |
| virtual const vector< [PtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-ptrtype) > & | **[AsReadonlyVector](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-asreadonlyvector)**() const |

## Protected Functions

|                | Name           |
| -------------- | -------------- |
| virtual void | **[OperatorEqualImpl](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-operatorequalimpl)**(const [EnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)< TsType > & src) |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::EnsembleStoragePolicy< TsType >](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)**

|                | Name           |
| -------------- | -------------- |
| | **[EnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-ensemblestoragepolicy)**() |
| virtual | **[~EnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-~ensemblestoragepolicy)**() |


## Detailed Description

```cpp
template <typename TsType >
class datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy;
```

## Public Types Documentation

### using T

```cpp
using datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy< TsType >::T =  double;
```


### typedef Type

```cpp
typedef std::remove_pointer<TsType>::type datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy< TsType >::Type;
```


### typedef PtrType

```cpp
typedef std::add_pointer<Type>::type datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy< TsType >::PtrType;
```


### typedef ElementType

```cpp
typedef Type::ElementType datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy< TsType >::ElementType;
```


## Public Functions Documentation

### function TimeSeriesEnsembleTimeSeriesStoragePolicy

```cpp
inline TimeSeriesEnsembleTimeSeriesStoragePolicy(
    WritableTimeSeriesEnsembleTimeSeriesStore< T > * store,
    size_t index
)
```


### function Reset

```cpp
inline virtual void Reset(
    const vector< PtrType > & values,
    const ptime & startDate,
    const TimeStep & timeStep
)
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::Reset](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-reset)


### function TimeSeriesEnsembleTimeSeriesStoragePolicy

```cpp
inline TimeSeriesEnsembleTimeSeriesStoragePolicy(
    const TimeSeriesEnsembleTimeSeriesStoragePolicy< TsType > & src
)
```


### function Clone

```cpp
inline virtual EnsembleStoragePolicy< TsType > * Clone() const
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-clone)


### function ~TimeSeriesEnsembleTimeSeriesStoragePolicy

```cpp
inline ~TimeSeriesEnsembleTimeSeriesStoragePolicy()
```


### function operator=

```cpp
inline TimeSeriesEnsembleTimeSeriesStoragePolicy & operator=(
    TimeSeriesEnsembleTimeSeriesStoragePolicy && src
)
```


### function ResetSeries

```cpp
inline virtual void ResetSeries(
    const size_t & numSeries,
    const size_t & lengthSeries,
    const ptime & startDate,
    const TimeStep & timeStep
)
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::ResetSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-resetseries)


### function GetReplicate

```cpp
inline PtrType GetReplicate(
    size_t i
)
```


### function Get

```cpp
inline virtual TsType Get(
    size_t i
)
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::Get](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-get)


### function Get

```cpp
inline virtual ElementType Get(
    size_t i,
    size_t tsIndex
)
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::Get](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-get)


### function Set

```cpp
inline virtual void Set(
    size_t i,
    size_t tsIndex,
    ElementType val
)
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::Set](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-set)


### function Set

```cpp
inline virtual void Set(
    size_t i,
    const Type & val
)
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::Set](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-set)


### function GetValues

```cpp
inline virtual vector< ElementType * > * GetValues() const
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::GetValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-getvalues)


### function CopyTo

```cpp
inline virtual void CopyTo(
    ElementType ** dest
) const
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::CopyTo](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-copyto)


### function Size

```cpp
inline virtual size_t Size() const
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::Size](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-size)


### function GetLength

```cpp
inline virtual size_t GetLength(
    size_t i
) const
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::GetLength](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-getlength)


### function Clear

```cpp
inline virtual void Clear()
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::Clear](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-clear)


### function AsReadonlyVector

```cpp
inline virtual const vector< PtrType > & AsReadonlyVector() const
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::AsReadonlyVector](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-asreadonlyvector)


## Protected Functions Documentation

### function OperatorEqualImpl

```cpp
inline virtual void OperatorEqualImpl(
    const EnsembleStoragePolicy< TsType > & src
)
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::OperatorEqualImpl](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-operatorequalimpl)


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000