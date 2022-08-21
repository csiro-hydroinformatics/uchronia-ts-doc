---
title: datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy

---

# datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy



 [More...](#detailed-description)


`#include <time_series_store.hpp>`

Inherits from [datatypes::timeseries::EnsembleStoragePolicy< TsType >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)

## Public Types

|                | Name           |
| -------------- | -------------- |
| using double | **[T](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#using-t)**  |
| typedef std::remove_pointer< TsType >::type | **[Type](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-type)**  |
| typedef std::add_pointer< [Type](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-type) >::type | **[PtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-ptrtype)**  |
| typedef Type::ElementType | **[ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-elementtype)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[TimeSeriesEnsembleTimeSeriesStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-timeseriesensembletimeseriesstoragepolicy)**([WritableTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/)< [T](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#using-t) > * store, size_t index) |
| virtual void | **[Reset](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-reset)**(const vector< [PtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-ptrtype) > & values, const ptime & startDate, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| | **[TimeSeriesEnsembleTimeSeriesStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-timeseriesensembletimeseriesstoragepolicy)**(const [TimeSeriesEnsembleTimeSeriesStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/)< TsType > & src) |
| virtual [EnsembleStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)< TsType > * | **[Clone](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-clone)**() const |
| | **[~TimeSeriesEnsembleTimeSeriesStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-~timeseriesensembletimeseriesstoragepolicy)**() |
| [TimeSeriesEnsembleTimeSeriesStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/) & | **[operator=](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-operator=)**([TimeSeriesEnsembleTimeSeriesStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/) && src) |
| virtual void | **[ResetSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-resetseries)**(const size_t & numSeries, const size_t & lengthSeries, const ptime & startDate, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| [PtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-ptrtype) | **[GetReplicate](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-getreplicate)**(size_t i) |
| virtual TsType | **[Get](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-get)**(size_t i) |
| virtual [ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-elementtype) | **[Get](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-get)**(size_t i, size_t tsIndex) |
| virtual void | **[Set](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-set)**(size_t i, size_t tsIndex, [ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-elementtype) val) |
| virtual void | **[Set](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-set)**(size_t i, const [Type](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-type) & val) |
| virtual vector< [ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-elementtype) * > * | **[GetValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-getvalues)**() const |
| virtual void | **[CopyTo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-copyto)**([ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-elementtype) ** dest) const |
| virtual size_t | **[Size](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-size)**() const |
| virtual size_t | **[GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-getlength)**(size_t i) const |
| virtual void | **[Clear](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-clear)**() |
| virtual const vector< [PtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#typedef-ptrtype) > & | **[AsReadonlyVector](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-asreadonlyvector)**() const |

## Protected Functions

|                | Name           |
| -------------- | -------------- |
| virtual void | **[OperatorEqualImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-operatorequalimpl)**(const [EnsembleStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)< TsType > & src) |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::EnsembleStoragePolicy< TsType >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)**

|                | Name           |
| -------------- | -------------- |
| | **[EnsembleStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-ensemblestoragepolicy)**() |
| virtual | **[~EnsembleStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-~ensemblestoragepolicy)**() |


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


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::Reset](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-reset)


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


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::Clone](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-clone)


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


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::ResetSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-resetseries)


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


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::Get](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-get)


### function Get

```cpp
inline virtual ElementType Get(
    size_t i,
    size_t tsIndex
)
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::Get](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-get)


### function Set

```cpp
inline virtual void Set(
    size_t i,
    size_t tsIndex,
    ElementType val
)
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::Set](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-set)


### function Set

```cpp
inline virtual void Set(
    size_t i,
    const Type & val
)
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::Set](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-set)


### function GetValues

```cpp
inline virtual vector< ElementType * > * GetValues() const
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::GetValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-getvalues)


### function CopyTo

```cpp
inline virtual void CopyTo(
    ElementType ** dest
) const
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::CopyTo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-copyto)


### function Size

```cpp
inline virtual size_t Size() const
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::Size](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-size)


### function GetLength

```cpp
inline virtual size_t GetLength(
    size_t i
) const
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-getlength)


### function Clear

```cpp
inline virtual void Clear()
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::Clear](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-clear)


### function AsReadonlyVector

```cpp
inline virtual const vector< PtrType > & AsReadonlyVector() const
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::AsReadonlyVector](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-asreadonlyvector)


## Protected Functions Documentation

### function OperatorEqualImpl

```cpp
inline virtual void OperatorEqualImpl(
    const EnsembleStoragePolicy< TsType > & src
)
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::OperatorEqualImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-operatorequalimpl)


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000