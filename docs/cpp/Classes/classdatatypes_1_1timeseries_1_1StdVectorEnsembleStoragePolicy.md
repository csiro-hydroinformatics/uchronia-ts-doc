---
title: datatypes::timeseries::StdVectorEnsembleStoragePolicy

---

# datatypes::timeseries::StdVectorEnsembleStoragePolicy



 [More...](#detailed-description)


`#include <time_series_strategies.hpp>`

Inherits from [datatypes::timeseries::EnsembleStoragePolicy< TsType >](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)

## Public Types

|                | Name           |
| -------------- | -------------- |
| typedef std::remove_pointer< TsType >::type | **[Type](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#typedef-type)**  |
| typedef std::add_pointer< [Type](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-type) >::type | **[PtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#typedef-ptrtype)**  |
| typedef Type::ElementType | **[ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#typedef-elementtype)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual void | **[Reset](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-reset)**(const vector< [PtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-ptrtype) > & values, const ptime & startDate, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| | **[StdVectorEnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-stdvectorensemblestoragepolicy)**(const [StdVectorEnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/)< TsType > & src) |
| | **[StdVectorEnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-stdvectorensemblestoragepolicy)**() |
| | **[~StdVectorEnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-~stdvectorensemblestoragepolicy)**() |
| [StdVectorEnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/) & | **[operator=](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-operator=)**([StdVectorEnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/) && src) |
| virtual void | **[ResetSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-resetseries)**(const size_t & numSeries, const size_t & lengthSeries, const ptime & startDate, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| virtual TsType | **[Get](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-get)**(size_t i) |
| [Type](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-type) | **[Get](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-get)**(size_t i) const |
| virtual [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-elementtype) | **[Get](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-get)**(size_t i, size_t tsIndex) |
| virtual void | **[Set](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-set)**(size_t i, size_t tsIndex, [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-elementtype) val) |
| virtual void | **[Set](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-set)**(size_t i, const [Type](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-type) & val) |
| virtual vector< [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-elementtype) * > * | **[GetValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-getvalues)**() const |
| virtual void | **[CopyTo](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-copyto)**([ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-elementtype) ** dest) const |
| virtual size_t | **[Size](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-size)**() const |
| virtual size_t | **[GetLength](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-getlength)**(size_t i) const |
| virtual void | **[Clear](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-clear)**() |
| virtual const vector< [PtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#typedef-ptrtype) > & | **[AsReadonlyVector](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-asreadonlyvector)**() const |
| virtual [EnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)< TsType > * | **[Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-clone)**() const |

## Protected Functions

|                | Name           |
| -------------- | -------------- |
| virtual void | **[OperatorEqualImpl](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/#function-operatorequalimpl)**(const [EnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)< TsType > & src) |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::EnsembleStoragePolicy< TsType >](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)**

|                | Name           |
| -------------- | -------------- |
| | **[EnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-ensemblestoragepolicy)**() |
| virtual | **[~EnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-~ensemblestoragepolicy)**() |


## Detailed Description

```cpp
template <typename TsType >
class datatypes::timeseries::StdVectorEnsembleStoragePolicy;
```

## Public Types Documentation

### typedef Type

```cpp
typedef std::remove_pointer<TsType>::type datatypes::timeseries::StdVectorEnsembleStoragePolicy< TsType >::Type;
```


### typedef PtrType

```cpp
typedef std::add_pointer<Type>::type datatypes::timeseries::StdVectorEnsembleStoragePolicy< TsType >::PtrType;
```


### typedef ElementType

```cpp
typedef Type::ElementType datatypes::timeseries::StdVectorEnsembleStoragePolicy< TsType >::ElementType;
```


## Public Functions Documentation

### function Reset

```cpp
inline virtual void Reset(
    const vector< PtrType > & values,
    const ptime & startDate,
    const TimeStep & timeStep
)
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::Reset](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-reset)


### function StdVectorEnsembleStoragePolicy

```cpp
inline StdVectorEnsembleStoragePolicy(
    const StdVectorEnsembleStoragePolicy< TsType > & src
)
```


### function StdVectorEnsembleStoragePolicy

```cpp
inline StdVectorEnsembleStoragePolicy()
```


### function ~StdVectorEnsembleStoragePolicy

```cpp
inline ~StdVectorEnsembleStoragePolicy()
```


### function operator=

```cpp
inline StdVectorEnsembleStoragePolicy & operator=(
    StdVectorEnsembleStoragePolicy && src
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


### function Get

```cpp
inline virtual TsType Get(
    size_t i
)
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::Get](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-get)


### function Get

```cpp
inline Type Get(
    size_t i
) const
```


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


### function Clone

```cpp
inline virtual EnsembleStoragePolicy< TsType > * Clone() const
```


**Reimplements**: [datatypes::timeseries::EnsembleStoragePolicy::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/#function-clone)


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