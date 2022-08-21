---
title: datatypes::exceptions::RangeCheck< size_t >

---

# datatypes::exceptions::RangeCheck< size_t >






`#include <exception_utilities.h>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| size_t | **[MaxIndexing](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1exceptions_1_1RangeCheck_3_01size__t_01_4/#function-maxindexing)**() |
| void | **[Check](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1exceptions_1_1RangeCheck_3_01size__t_01_4/#function-check)**(size_t value, size_t min, size_t max, const string & variableName) |
| void | **[CheckTimeSeriesInterval](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1exceptions_1_1RangeCheck_3_01size__t_01_4/#function-checktimeseriesinterval)**(const size_t & from, size_t & to, const size_t & tsLength) |
| void | **[CheckTimeSeriesIndex](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1exceptions_1_1RangeCheck_3_01size__t_01_4/#function-checktimeseriesindex)**(const size_t & index, const size_t & tsLength, const string & variableName ="index") |

## Public Functions Documentation

### function MaxIndexing

```cpp
static inline size_t MaxIndexing()
```


### function Check

```cpp
static inline void Check(
    size_t value,
    size_t min,
    size_t max,
    const string & variableName
)
```


### function CheckTimeSeriesInterval

```cpp
static inline void CheckTimeSeriesInterval(
    const size_t & from,
    size_t & to,
    const size_t & tsLength
)
```


### function CheckTimeSeriesIndex

```cpp
static inline void CheckTimeSeriesIndex(
    const size_t & index,
    const size_t & tsLength,
    const string & variableName ="index"
)
```


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000