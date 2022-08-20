---
title: datatypes::timeseries::MultiTimeSeries
summary: Template for time series with multiple values at time point; e.g. to hold multiple realizations of time series in an ensemble. 

---

# datatypes::timeseries::MultiTimeSeries



Template for time series with multiple values at time point; e.g. to hold multiple realizations of time series in an ensemble.  [More...](#detailed-description)


`#include <time_series.hpp>`

## Public Types

|                | Name           |
| -------------- | -------------- |
| typedef std::remove_pointer< TsType >::type | **[Type](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-type)**  |
| typedef std::add_pointer< [Type](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-type) >::type | **[PtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-ptrtype)**  |
| typedef TsType | **[ItemType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-itemtype)**  |
| typedef Type::ElementType | **[ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-elementtype)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-multitimeseries)**(const vector< [ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-elementtype) * > & values, size_t length, const ptime & startDate, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| | **[MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-multitimeseries)**(const vector< vector< [ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-elementtype) >> & values, const ptime & startDate, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| | **[MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-multitimeseries)**([ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-elementtype) **const values, size_t ensSize, size_t length, const ptime & startDate, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| | **[MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-multitimeseries)**(const vector< [PtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-ptrtype) > & values, const ptime & startDate, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| | **[MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-multitimeseries)**(const [Type](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-type) & series) |
| | **[MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-multitimeseries)**(const vector< [Type](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-type) > & values, const ptime & startDate, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| | **[MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-multitimeseries)**(std::function< [Type](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-type)(size_t)> & valueGen, size_t ensSize, const ptime & startDate, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| | **[MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-multitimeseries)**(const [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< TsType > & src) |
| | **[MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-multitimeseries)**([EnsembleStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)< TsType > * store) |
| | **[MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-multitimeseries)**() |
| [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [PtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-ptrtype) > * | **[AsPointerSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-aspointerseries)**() |
| [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [Type](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-type) > | **[AsValueSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-asvalueseries)**() |
| | **[~MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-~multitimeseries)**() |
| [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/) & | **[operator=](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-operator=)**(const [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/) & src) |
| [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/) & | **[operator=](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-operator=)**([MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/) && src) |
| void | **[ResetSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-resetseries)**(const size_t & numSeries, const size_t & lengthSeries, const ptime & startDate, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| TsType | **[Get](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-get)**(size_t i) |
| [Type](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-type) | **[Get](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-get)**(size_t i) const |
| [ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-elementtype) | **[Get](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-get)**(size_t i, size_t tsIndex) |
| void | **[Set](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-set)**(size_t i, size_t tsIndex, [ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-elementtype) val) |
| void | **[Set](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-set)**(size_t i, const [Type](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-type) & val) |
| vector< [ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-elementtype) * > * | **[GetValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-getvalues)**() const |
| void | **[CopyTo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-copyto)**([ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-elementtype) ** dest) const |
| size_t | **[Size](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-size)**() const |
| size_t | **[GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-getlength)**(size_t i) const |
| ptime | **[GetStartDate](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-getstartdate)**() const |
| void | **[SetStartDate](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-setstartdate)**(const ptime & start) |
| [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-gettimestep)**() const |
| void | **[Clear](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-clear)**() |

## Protected Functions

|                | Name           |
| -------------- | -------------- |
| virtual void | **[InitializeStorage](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-initializestorage)**() |
| virtual void | **[OperatorEqualImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-operatorequalimpl)**(const [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< TsType > & src) |

## Detailed Description

```cpp
template <typename TsType  =TimeSeries>
class datatypes::timeseries::MultiTimeSeries;
```

Template for time series with multiple values at time point; e.g. to hold multiple realizations of time series in an ensemble. 

**Template Parameters**: 

  * **TsType** type of time series, typically a time series of double or float. 

## Public Types Documentation

### typedef Type

```cpp
typedef std::remove_pointer<TsType>::type datatypes::timeseries::MultiTimeSeries< TsType >::Type;
```


### typedef PtrType

```cpp
typedef std::add_pointer<Type>::type datatypes::timeseries::MultiTimeSeries< TsType >::PtrType;
```


### typedef ItemType

```cpp
typedef TsType datatypes::timeseries::MultiTimeSeries< TsType >::ItemType;
```


### typedef ElementType

```cpp
typedef Type::ElementType datatypes::timeseries::MultiTimeSeries< TsType >::ElementType;
```


## Public Functions Documentation

### function MultiTimeSeries

```cpp
inline MultiTimeSeries(
    const vector< ElementType * > & values,
    size_t length,
    const ptime & startDate,
    const TimeStep & timeStep
)
```


### function MultiTimeSeries

```cpp
inline MultiTimeSeries(
    const vector< vector< ElementType >> & values,
    const ptime & startDate,
    const TimeStep & timeStep
)
```


### function MultiTimeSeries

```cpp
inline MultiTimeSeries(
    ElementType **const values,
    size_t ensSize,
    size_t length,
    const ptime & startDate,
    const TimeStep & timeStep
)
```


### function MultiTimeSeries

```cpp
inline MultiTimeSeries(
    const vector< PtrType > & values,
    const ptime & startDate,
    const TimeStep & timeStep
)
```


### function MultiTimeSeries

```cpp
inline MultiTimeSeries(
    const Type & series
)
```


### function MultiTimeSeries

```cpp
inline MultiTimeSeries(
    const vector< Type > & values,
    const ptime & startDate,
    const TimeStep & timeStep
)
```


### function MultiTimeSeries

```cpp
inline MultiTimeSeries(
    std::function< Type(size_t)> & valueGen,
    size_t ensSize,
    const ptime & startDate,
    const TimeStep & timeStep
)
```


### function MultiTimeSeries

```cpp
inline MultiTimeSeries(
    const MultiTimeSeries< TsType > & src
)
```


### function MultiTimeSeries

```cpp
inline MultiTimeSeries(
    EnsembleStoragePolicy< TsType > * store
)
```


### function MultiTimeSeries

```cpp
inline MultiTimeSeries()
```


### function AsPointerSeries

```cpp
inline MultiTimeSeries< PtrType > * AsPointerSeries()
```


### function AsValueSeries

```cpp
inline MultiTimeSeries< Type > AsValueSeries()
```


### function ~MultiTimeSeries

```cpp
inline ~MultiTimeSeries()
```


### function operator=

```cpp
inline MultiTimeSeries & operator=(
    const MultiTimeSeries & src
)
```


### function operator=

```cpp
inline MultiTimeSeries & operator=(
    MultiTimeSeries && src
)
```


### function ResetSeries

```cpp
inline void ResetSeries(
    const size_t & numSeries,
    const size_t & lengthSeries,
    const ptime & startDate,
    const TimeStep & timeStep
)
```


### function Get

```cpp
inline TsType Get(
    size_t i
)
```


### function Get

```cpp
inline Type Get(
    size_t i
) const
```


### function Get

```cpp
inline ElementType Get(
    size_t i,
    size_t tsIndex
)
```


### function Set

```cpp
inline void Set(
    size_t i,
    size_t tsIndex,
    ElementType val
)
```


### function Set

```cpp
inline void Set(
    size_t i,
    const Type & val
)
```


### function GetValues

```cpp
inline vector< ElementType * > * GetValues() const
```


### function CopyTo

```cpp
inline void CopyTo(
    ElementType ** dest
) const
```


### function Size

```cpp
inline size_t Size() const
```


### function GetLength

```cpp
inline size_t GetLength(
    size_t i
) const
```


### function GetStartDate

```cpp
inline ptime GetStartDate() const
```


### function SetStartDate

```cpp
inline void SetStartDate(
    const ptime & start
)
```


### function GetTimeStep

```cpp
inline TimeStep GetTimeStep() const
```


### function Clear

```cpp
inline void Clear()
```


## Protected Functions Documentation

### function InitializeStorage

```cpp
inline virtual void InitializeStorage()
```


### function OperatorEqualImpl

```cpp
inline virtual void OperatorEqualImpl(
    const MultiTimeSeries< TsType > & src
)
```


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000