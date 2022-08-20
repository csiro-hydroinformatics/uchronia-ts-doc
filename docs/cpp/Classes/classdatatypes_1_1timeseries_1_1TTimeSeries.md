---
title: datatypes::timeseries::TTimeSeries
summary: A template for univariate, single realisasion time series. 

---

# datatypes::timeseries::TTimeSeries



A template for univariate, single realisasion time series.  [More...](#detailed-description)


`#include <time_series.hpp>`

## Public Types

|                | Name           |
| -------------- | -------------- |
| using T | **[ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#using-elementtype)** <br>The type of each element in this time series.  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| bool | **[IsMissingValue](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-ismissingvalue)**(const T & value) const |
| T | **[GetMissingValue](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-getmissingvalue)**() const |
| | **[TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-ttimeseries)**([StoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)< T > * storage =nullptr, [MissingValuePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/)< T > * mvp =nullptr) |
| | **[TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-ttimeseries)**(T default_value, size_t length, const ptime & startDate, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =[TimeStep::GetHourly](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-gethourly)(), [StoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)< T > * storage =nullptr, [MissingValuePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/)< T > * mvp =nullptr) |
| | **[TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-ttimeseries)**(size_t length, const ptime & startDate, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =[TimeStep::GetHourly](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-gethourly)(), [StoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)< T > * storage =nullptr, [MissingValuePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/)< T > * mvp =nullptr) |
| | **[TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-ttimeseries)**(const vector< T > & values, const ptime & startDate, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =[TimeStep::GetHourly](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-gethourly)(), [StoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)< T > * storage =nullptr, [MissingValuePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/)< T > * mvp =nullptr) |
| | **[TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-ttimeseries)**(const T * values, size_t length, const ptime & startDate, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =[TimeStep::GetHourly](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-gethourly)(), [StoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)< T > * storage =nullptr, [MissingValuePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/)< T > * mvp =nullptr) |
| | **[TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-ttimeseries)**(std::function< T(size_t)> & valueGen, size_t length, const ptime & startDate, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =[TimeStep::GetHourly](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-gethourly)(), [StoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)< T > * storage =nullptr, [MissingValuePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/)< T > * mvp =nullptr) |
| | **[TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-ttimeseries)**(const [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > & src) |
| | **[TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-ttimeseries)**(const [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > & src, [StoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)< T > * storage) |
| | **[TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-ttimeseries)**(const [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > * src) |
| | **[TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-ttimeseries)**([TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > && src)<br>Constructor using the move semantics.  |
| [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > & | **[operator=](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-operator=)**([TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > && src) |
| [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > & | **[operator=](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-operator=)**(const [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > & src) |
| virtual | **[~TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-~ttimeseries)**() |
| T | **[GetValueNoConst](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-getvaluenoconst)**(const size_t & index) |
| const T & | **[GetValueConst](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-getvalueconst)**(const size_t & index) const |
| T | **[GetValue](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-getvalue)**(const size_t & index) |
| const T & | **[GetValue](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-getvalue)**(const size_t & index) const |
| T | **[GetValueNoConst](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-getvaluenoconst)**(const ptime & instant) |
| T | **[GetValue](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-getvalue)**(const ptime & instant) |
| const T & | **[GetValue](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-getvalue)**(const ptime & instant) const |
| T | **[GetLastValue](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-getlastvalue)**() |
| void | **[CopyTo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-copyto)**(T * dest, size_t from =0, size_t to =-1) const |
| void | **[CopyWithMissingValueTo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-copywithmissingvalueto)**(T * dest, const T & missingValueValue, size_t from =0, size_t to =-1) const |
| void | **[CopyValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-copyvalues)**(const [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > & src) |
| void | **[CopyTo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-copyto)**(vector< T > & dest, size_t from =0, size_t to =-1) const |
| T * | **[GetValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-getvalues)**(size_t from =0, size_t to =std::numeric_limits< size_t >::max()) const |
| vector< T > | **[GetValuesVector](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-getvaluesvector)**(size_t from =0, size_t to =std::numeric_limits< size_t >::max()) const |
| [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > | **[Subset](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-subset)**(size_t from =0, size_t to =std::numeric_limits< size_t >::max()) const |
| void | **[SetValue](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-setvalue)**(size_t index, T value) |
| void | **[SetValue](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-setvalue)**(const ptime & instant, T value) |
| void | **[Reset](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-reset)**(size_t length, const ptime & startDate, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| void | **[Reset](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-reset)**(size_t length, const ptime & startDate, const T * values =nullptr) |
| void | **[Reset](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-reset)**(size_t length, const ptime & startDate, T value) |
| void | **[Reset](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-reset)**(const vector< T > & values, const ptime & startDate) |
| void | **[Reset](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-reset)**(const vector< T > & values, const ptime & startDate, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| size_t | **[GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-getlength)**() const |
| ptime | **[GetStartDate](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-getstartdate)**() const |
| ptime | **[GetEndDate](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-getenddate)**() const |
| [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-gettimestep)**() const |
| void | **[SetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-settimestep)**(const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| void | **[SetStartDate](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-setstartdate)**(const ptime & start) |
| ptime | **[TimeForIndex](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-timeforindex)**(size_t timeIndex) const |
| vector< ptime > | **[TimeIndices](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-timeindices)**() const |
| size_t | **[IndexForTime](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-indexfortime)**(const ptime & instant) const |
| size_t | **[UpperIndexForTime](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-upperindexfortime)**(const ptime & instant) const |
| size_t | **[LowerIndexForTime](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-lowerindexfortime)**(const ptime & instant) const |
| string | **[GetSummary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-getsummary)**() const |
| T & | **[operator[]](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-operator[])**(const ptime & instant) |
| T & | **[operator[]](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-operator[])**(const size_t i) |
| const T & | **[operator[]](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-operator[])**(const ptime & instant) const |
| const T & | **[operator[]](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-operator[])**(const size_t i) const |
| [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > | **[operator+](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-operator+)**(const [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > & rhs) const |
| [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > | **[operator+](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-operator+)**(T value) const |
| template <typename M \> <br>[TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > | **[operator*](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-operator*)**(M multiplicator) const |
| int | **[NumInstances](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-numinstances)**() |

## Protected Functions

|                | Name           |
| -------------- | -------------- |
| T | **[GetNACode](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#function-getnacode)**() const |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| string | **[Tag](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/#variable-tag)**  |

## Detailed Description

```cpp
template <typename T  =double>
class datatypes::timeseries::TTimeSeries;
```

A template for univariate, single realisasion time series. 

**Template Parameters**: 

  * **T** Element type, typically double or float, but possibly a more complicated type such as another [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/). 

## Public Types Documentation

### using ElementType

```cpp
using datatypes::timeseries::TTimeSeries< T >::ElementType =  T;
```

The type of each element in this time series. 

## Public Functions Documentation

### function IsMissingValue

```cpp
inline bool IsMissingValue(
    const T & value
) const
```


### function GetMissingValue

```cpp
inline T GetMissingValue() const
```


### function TTimeSeries

```cpp
inline TTimeSeries(
    StoragePolicy< T > * storage =nullptr,
    MissingValuePolicy< T > * mvp =nullptr
)
```


### function TTimeSeries

```cpp
inline TTimeSeries(
    T default_value,
    size_t length,
    const ptime & startDate,
    const TimeStep & timeStep =TimeStep::GetHourly(),
    StoragePolicy< T > * storage =nullptr,
    MissingValuePolicy< T > * mvp =nullptr
)
```


### function TTimeSeries

```cpp
inline TTimeSeries(
    size_t length,
    const ptime & startDate,
    const TimeStep & timeStep =TimeStep::GetHourly(),
    StoragePolicy< T > * storage =nullptr,
    MissingValuePolicy< T > * mvp =nullptr
)
```


### function TTimeSeries

```cpp
inline TTimeSeries(
    const vector< T > & values,
    const ptime & startDate,
    const TimeStep & timeStep =TimeStep::GetHourly(),
    StoragePolicy< T > * storage =nullptr,
    MissingValuePolicy< T > * mvp =nullptr
)
```


### function TTimeSeries

```cpp
inline TTimeSeries(
    const T * values,
    size_t length,
    const ptime & startDate,
    const TimeStep & timeStep =TimeStep::GetHourly(),
    StoragePolicy< T > * storage =nullptr,
    MissingValuePolicy< T > * mvp =nullptr
)
```


### function TTimeSeries

```cpp
inline TTimeSeries(
    std::function< T(size_t)> & valueGen,
    size_t length,
    const ptime & startDate,
    const TimeStep & timeStep =TimeStep::GetHourly(),
    StoragePolicy< T > * storage =nullptr,
    MissingValuePolicy< T > * mvp =nullptr
)
```


### function TTimeSeries

```cpp
inline TTimeSeries(
    const TTimeSeries< T > & src
)
```


### function TTimeSeries

```cpp
inline TTimeSeries(
    const TTimeSeries< T > & src,
    StoragePolicy< T > * storage
)
```


### function TTimeSeries

```cpp
inline TTimeSeries(
    const TTimeSeries< T > * src
)
```


### function TTimeSeries

```cpp
inline TTimeSeries(
    TTimeSeries< T > && src
)
```

Constructor using the move semantics. 

**Parameters**: 

  * **src** time series from which to move data. 


**Remark**: C++ for the Impatient Appendix A. A Painless Introduction to Rvalue References (C++11) See also [http://stackoverflow.com/a/3109981/2752565](http://stackoverflow.com/a/3109981/2752565) for information on move semantic 

### function operator=

```cpp
inline TTimeSeries< T > & operator=(
    TTimeSeries< T > && src
)
```


### function operator=

```cpp
inline TTimeSeries< T > & operator=(
    const TTimeSeries< T > & src
)
```


### function ~TTimeSeries

```cpp
inline virtual ~TTimeSeries()
```


### function GetValueNoConst

```cpp
inline T GetValueNoConst(
    const size_t & index
)
```


### function GetValueConst

```cpp
inline const T & GetValueConst(
    const size_t & index
) const
```


### function GetValue

```cpp
inline T GetValue(
    const size_t & index
)
```


### function GetValue

```cpp
inline const T & GetValue(
    const size_t & index
) const
```


### function GetValueNoConst

```cpp
inline T GetValueNoConst(
    const ptime & instant
)
```


### function GetValue

```cpp
inline T GetValue(
    const ptime & instant
)
```


### function GetValue

```cpp
inline const T & GetValue(
    const ptime & instant
) const
```


### function GetLastValue

```cpp
inline T GetLastValue()
```


### function CopyTo

```cpp
inline void CopyTo(
    T * dest,
    size_t from =0,
    size_t to =-1
) const
```


### function CopyWithMissingValueTo

```cpp
inline void CopyWithMissingValueTo(
    T * dest,
    const T & missingValueValue,
    size_t from =0,
    size_t to =-1
) const
```


### function CopyValues

```cpp
inline void CopyValues(
    const TTimeSeries< T > & src
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


### function GetValues

```cpp
inline T * GetValues(
    size_t from =0,
    size_t to =std::numeric_limits< size_t >::max()
) const
```


### function GetValuesVector

```cpp
inline vector< T > GetValuesVector(
    size_t from =0,
    size_t to =std::numeric_limits< size_t >::max()
) const
```


### function Subset

```cpp
inline TTimeSeries< T > Subset(
    size_t from =0,
    size_t to =std::numeric_limits< size_t >::max()
) const
```


### function SetValue

```cpp
inline void SetValue(
    size_t index,
    T value
)
```


### function SetValue

```cpp
inline void SetValue(
    const ptime & instant,
    T value
)
```


### function Reset

```cpp
inline void Reset(
    size_t length,
    const ptime & startDate,
    const TimeStep & timeStep
)
```


### function Reset

```cpp
inline void Reset(
    size_t length,
    const ptime & startDate,
    const T * values =nullptr
)
```


### function Reset

```cpp
inline void Reset(
    size_t length,
    const ptime & startDate,
    T value
)
```


### function Reset

```cpp
inline void Reset(
    const vector< T > & values,
    const ptime & startDate
)
```


### function Reset

```cpp
inline void Reset(
    const vector< T > & values,
    const ptime & startDate,
    const TimeStep & timeStep
)
```


### function GetLength

```cpp
inline size_t GetLength() const
```


### function GetStartDate

```cpp
inline ptime GetStartDate() const
```


### function GetEndDate

```cpp
inline ptime GetEndDate() const
```


### function GetTimeStep

```cpp
inline TimeStep GetTimeStep() const
```


### function SetTimeStep

```cpp
inline void SetTimeStep(
    const TimeStep & timeStep
)
```


### function SetStartDate

```cpp
inline void SetStartDate(
    const ptime & start
)
```


### function TimeForIndex

```cpp
inline ptime TimeForIndex(
    size_t timeIndex
) const
```


### function TimeIndices

```cpp
inline vector< ptime > TimeIndices() const
```


### function IndexForTime

```cpp
inline size_t IndexForTime(
    const ptime & instant
) const
```


### function UpperIndexForTime

```cpp
inline size_t UpperIndexForTime(
    const ptime & instant
) const
```


### function LowerIndexForTime

```cpp
inline size_t LowerIndexForTime(
    const ptime & instant
) const
```


### function GetSummary

```cpp
inline string GetSummary() const
```


### function operator[]

```cpp
inline T & operator[](
    const ptime & instant
)
```


### function operator[]

```cpp
inline T & operator[](
    const size_t i
)
```


### function operator[]

```cpp
inline const T & operator[](
    const ptime & instant
) const
```


### function operator[]

```cpp
inline const T & operator[](
    const size_t i
) const
```


### function operator+

```cpp
inline TTimeSeries< T > operator+(
    const TTimeSeries< T > & rhs
) const
```


### function operator+

```cpp
inline TTimeSeries< T > operator+(
    T value
) const
```


### function operator*

```cpp
template <typename M >
inline TTimeSeries< T > operator*(
    M multiplicator
) const
```


### function NumInstances

```cpp
static inline int NumInstances()
```


## Protected Functions Documentation

### function GetNACode

```cpp
inline T GetNACode() const
```


## Public Attributes Documentation

### variable Tag

```cpp
string Tag;
```


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000