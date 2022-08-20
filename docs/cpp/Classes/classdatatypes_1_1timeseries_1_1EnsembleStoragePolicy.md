---
title: datatypes::timeseries::EnsembleStoragePolicy

---

# datatypes::timeseries::EnsembleStoragePolicy



 [More...](#detailed-description)


`#include <time_series_strategies.hpp>`

Inherited by [datatypes::timeseries::StdVectorEnsembleStoragePolicy< TsType >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/), [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy< TsType >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/)

## Public Types

|                | Name           |
| -------------- | -------------- |
| typedef std::remove_pointer< TsType >::type | **[Type](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-type)**  |
| typedef std::add_pointer< [Type](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-type) >::type | **[PtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-ptrtype)**  |
| typedef Type::ElementType | **[ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-elementtype)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[EnsembleStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-ensemblestoragepolicy)**() |
| virtual | **[~EnsembleStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-~ensemblestoragepolicy)**() |
| virtual void | **[Reset](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-reset)**(const vector< [PtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-ptrtype) > & values, const ptime & startDate, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) =0 |
| [EnsembleStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/) & | **[operator=](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-operator=)**(const [EnsembleStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/) & src) |
| virtual void | **[ResetSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-resetseries)**(const size_t & numSeries, const size_t & lengthSeries, const ptime & startDate, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) =0 |
| virtual TsType | **[Get](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-get)**(size_t i) =0 |
| virtual [ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-elementtype) | **[Get](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-get)**(size_t i, size_t tsIndex) =0 |
| virtual void | **[Set](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-set)**(size_t i, size_t tsIndex, [ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-elementtype) val) =0 |
| virtual void | **[Set](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-set)**(size_t i, const [Type](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-type) & val) =0 |
| virtual vector< [ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-elementtype) * > * | **[GetValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-getvalues)**() const =0 |
| virtual void | **[CopyTo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-copyto)**([ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-elementtype) ** dest) const =0 |
| virtual size_t | **[Size](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-size)**() const =0 |
| virtual size_t | **[GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-getlength)**(size_t i) const =0 |
| virtual void | **[Clear](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-clear)**() =0 |
| virtual const vector< [PtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-ptrtype) > & | **[AsReadonlyVector](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-asreadonlyvector)**() const =0 |
| virtual [EnsembleStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)< TsType > * | **[Clone](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-clone)**() const =0 |

## Protected Functions

|                | Name           |
| -------------- | -------------- |
| virtual void | **[OperatorEqualImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-operatorequalimpl)**(const [EnsembleStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)< TsType > & src) =0 |

## Detailed Description

```cpp
template <typename TsType >
class datatypes::timeseries::EnsembleStoragePolicy;
```

## Public Types Documentation

### typedef Type

```cpp
typedef std::remove_pointer<TsType>::type datatypes::timeseries::EnsembleStoragePolicy< TsType >::Type;
```


### typedef PtrType

```cpp
typedef std::add_pointer<Type>::type datatypes::timeseries::EnsembleStoragePolicy< TsType >::PtrType;
```


### typedef ElementType

```cpp
typedef Type::ElementType datatypes::timeseries::EnsembleStoragePolicy< TsType >::ElementType;
```


## Public Functions Documentation

### function EnsembleStoragePolicy

```cpp
inline EnsembleStoragePolicy()
```


### function ~EnsembleStoragePolicy

```cpp
inline virtual ~EnsembleStoragePolicy()
```


### function Reset

```cpp
virtual void Reset(
    const vector< PtrType > & values,
    const ptime & startDate,
    const TimeStep & timeStep
) =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::Reset](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-reset), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::Reset](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-reset)


### function operator=

```cpp
inline EnsembleStoragePolicy & operator=(
    const EnsembleStoragePolicy & src
)
```


### function ResetSeries

```cpp
virtual void ResetSeries(
    const size_t & numSeries,
    const size_t & lengthSeries,
    const ptime & startDate,
    const TimeStep & timeStep
) =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::ResetSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-resetseries), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::ResetSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-resetseries)


### function Get

```cpp
virtual TsType Get(
    size_t i
) =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::Get](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-get), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::Get](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-get)


### function Get

```cpp
virtual ElementType Get(
    size_t i,
    size_t tsIndex
) =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::Get](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-get), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::Get](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-get)


### function Set

```cpp
virtual void Set(
    size_t i,
    size_t tsIndex,
    ElementType val
) =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::Set](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-set), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::Set](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-set)


### function Set

```cpp
virtual void Set(
    size_t i,
    const Type & val
) =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::Set](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-set), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::Set](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-set)


### function GetValues

```cpp
virtual vector< ElementType * > * GetValues() const =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::GetValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-getvalues), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::GetValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-getvalues)


### function CopyTo

```cpp
virtual void CopyTo(
    ElementType ** dest
) const =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::CopyTo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-copyto), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::CopyTo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-copyto)


### function Size

```cpp
virtual size_t Size() const =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::Size](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-size), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::Size](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-size)


### function GetLength

```cpp
virtual size_t GetLength(
    size_t i
) const =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-getlength), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-getlength)


### function Clear

```cpp
virtual void Clear() =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::Clear](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-clear), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::Clear](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-clear)


### function AsReadonlyVector

```cpp
virtual const vector< PtrType > & AsReadonlyVector() const =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::AsReadonlyVector](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-asreadonlyvector), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::AsReadonlyVector](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-asreadonlyvector)


### function Clone

```cpp
virtual EnsembleStoragePolicy< TsType > * Clone() const =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::Clone](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-clone), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::Clone](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-clone)


## Protected Functions Documentation

### function OperatorEqualImpl

```cpp
virtual void OperatorEqualImpl(
    const EnsembleStoragePolicy< TsType > & src
) =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::OperatorEqualImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-operatorequalimpl), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::OperatorEqualImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-operatorequalimpl)


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000