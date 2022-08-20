---
title: datatypes::timeseries::EnsembleStoragePolicy

---

# datatypes::timeseries::EnsembleStoragePolicy



 [More...](#detailed-description)


`#include <time_series_strategies.hpp>`

Inherited by [datatypes::timeseries::StdVectorEnsembleStoragePolicy< TsType >](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/), [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy< TsType >](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/)

## Public Types

|                | Name           |
| -------------- | -------------- |
| typedef std::remove_pointer< TsType >::type | **[Type](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-type)**  |
| typedef std::add_pointer< [Type](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-type) >::type | **[PtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-ptrtype)**  |
| typedef Type::ElementType | **[ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-elementtype)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[EnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-ensemblestoragepolicy)**() |
| virtual | **[~EnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-~ensemblestoragepolicy)**() |
| virtual void | **[Reset](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-reset)**(const vector< [PtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-ptrtype) > & values, const ptime & startDate, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) =0 |
| [EnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/) & | **[operator=](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-operator=)**(const [EnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/) & src) |
| virtual void | **[ResetSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-resetseries)**(const size_t & numSeries, const size_t & lengthSeries, const ptime & startDate, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) =0 |
| virtual TsType | **[Get](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-get)**(size_t i) =0 |
| virtual [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-elementtype) | **[Get](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-get)**(size_t i, size_t tsIndex) =0 |
| virtual void | **[Set](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-set)**(size_t i, size_t tsIndex, [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-elementtype) val) =0 |
| virtual void | **[Set](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-set)**(size_t i, const [Type](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-type) & val) =0 |
| virtual vector< [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-elementtype) * > * | **[GetValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-getvalues)**() const =0 |
| virtual void | **[CopyTo](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-copyto)**([ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-elementtype) ** dest) const =0 |
| virtual size_t | **[Size](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-size)**() const =0 |
| virtual size_t | **[GetLength](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-getlength)**(size_t i) const =0 |
| virtual void | **[Clear](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-clear)**() =0 |
| virtual const vector< [PtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-ptrtype) > & | **[AsReadonlyVector](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-asreadonlyvector)**() const =0 |
| virtual [EnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)< TsType > * | **[Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-clone)**() const =0 |

## Protected Functions

|                | Name           |
| -------------- | -------------- |
| virtual void | **[OperatorEqualImpl](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-operatorequalimpl)**(const [EnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)< TsType > & src) =0 |

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


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::Reset](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-reset), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::Reset](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-reset)


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


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::ResetSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-resetseries), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::ResetSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-resetseries)


### function Get

```cpp
virtual TsType Get(
    size_t i
) =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::Get](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-get), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::Get](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-get)


### function Get

```cpp
virtual ElementType Get(
    size_t i,
    size_t tsIndex
) =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::Get](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-get), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::Get](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-get)


### function Set

```cpp
virtual void Set(
    size_t i,
    size_t tsIndex,
    ElementType val
) =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::Set](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-set), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::Set](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-set)


### function Set

```cpp
virtual void Set(
    size_t i,
    const Type & val
) =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::Set](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-set), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::Set](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-set)


### function GetValues

```cpp
virtual vector< ElementType * > * GetValues() const =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::GetValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-getvalues), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::GetValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-getvalues)


### function CopyTo

```cpp
virtual void CopyTo(
    ElementType ** dest
) const =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::CopyTo](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-copyto), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::CopyTo](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-copyto)


### function Size

```cpp
virtual size_t Size() const =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::Size](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-size), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::Size](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-size)


### function GetLength

```cpp
virtual size_t GetLength(
    size_t i
) const =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::GetLength](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-getlength), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::GetLength](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-getlength)


### function Clear

```cpp
virtual void Clear() =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::Clear](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-clear), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::Clear](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-clear)


### function AsReadonlyVector

```cpp
virtual const vector< PtrType > & AsReadonlyVector() const =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::AsReadonlyVector](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-asreadonlyvector), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::AsReadonlyVector](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-asreadonlyvector)


### function Clone

```cpp
virtual EnsembleStoragePolicy< TsType > * Clone() const =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-clone), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-clone)


## Protected Functions Documentation

### function OperatorEqualImpl

```cpp
virtual void OperatorEqualImpl(
    const EnsembleStoragePolicy< TsType > & src
) =0
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy::OperatorEqualImpl](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/#function-operatorequalimpl), [datatypes::timeseries::StdVectorEnsembleStoragePolicy::OperatorEqualImpl](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-operatorequalimpl)


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000