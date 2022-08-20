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
| typedef std::remove_pointer< TsType >::type | **[Type](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-type)**  |
| typedef std::add_pointer< [Type](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-type) >::type | **[PtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-ptrtype)**  |
| typedef TsType | **[ItemType](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-itemtype)**  |
| typedef Type::ElementType | **[ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-elementtype)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-multitimeseries)**(const vector< [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-elementtype) * > & values, size_t length, const ptime & startDate, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| | **[MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-multitimeseries)**(const vector< vector< [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-elementtype) >> & values, const ptime & startDate, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| | **[MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-multitimeseries)**([ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-elementtype) **const values, size_t ensSize, size_t length, const ptime & startDate, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| | **[MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-multitimeseries)**(const vector< [PtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-ptrtype) > & values, const ptime & startDate, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| | **[MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-multitimeseries)**(const [Type](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-type) & series) |
| | **[MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-multitimeseries)**(const vector< [Type](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-type) > & values, const ptime & startDate, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| | **[MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-multitimeseries)**(std::function< [Type](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-type)(size_t)> & valueGen, size_t ensSize, const ptime & startDate, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| | **[MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-multitimeseries)**(const [MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< TsType > & src) |
| | **[MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-multitimeseries)**([EnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)< TsType > * store) |
| | **[MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-multitimeseries)**() |
| [MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [PtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-ptrtype) > * | **[AsPointerSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-aspointerseries)**() |
| [MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [Type](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-type) > | **[AsValueSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-asvalueseries)**() |
| | **[~MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-~multitimeseries)**() |
| [MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/) & | **[operator=](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-operator=)**(const [MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/) & src) |
| [MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/) & | **[operator=](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-operator=)**([MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/) && src) |
| void | **[ResetSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-resetseries)**(const size_t & numSeries, const size_t & lengthSeries, const ptime & startDate, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| TsType | **[Get](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-get)**(size_t i) |
| [Type](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-type) | **[Get](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-get)**(size_t i) const |
| [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-elementtype) | **[Get](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-get)**(size_t i, size_t tsIndex) |
| void | **[Set](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-set)**(size_t i, size_t tsIndex, [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-elementtype) val) |
| void | **[Set](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-set)**(size_t i, const [Type](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-type) & val) |
| vector< [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-elementtype) * > * | **[GetValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-getvalues)**() const |
| void | **[CopyTo](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-copyto)**([ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#typedef-elementtype) ** dest) const |
| size_t | **[Size](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-size)**() const |
| size_t | **[GetLength](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-getlength)**(size_t i) const |
| ptime | **[GetStartDate](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-getstartdate)**() const |
| void | **[SetStartDate](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-setstartdate)**(const ptime & start) |
| [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-gettimestep)**() const |
| void | **[Clear](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-clear)**() |

## Protected Functions

|                | Name           |
| -------------- | -------------- |
| virtual void | **[InitializeStorage](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-initializestorage)**() |
| virtual void | **[OperatorEqualImpl](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/#function-operatorequalimpl)**(const [MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< TsType > & src) |

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

Updated on 2022-08-20 at 18:35:57 +1000