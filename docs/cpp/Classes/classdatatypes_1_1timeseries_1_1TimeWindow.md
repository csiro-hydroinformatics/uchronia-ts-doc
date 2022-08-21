---
title: datatypes::timeseries::TimeWindow
summary: An object that represents a time window, defining subset/trim operations on time series. 

---

# datatypes::timeseries::TimeWindow



An object that represents a time window, defining subset/trim operations on time series.  [More...](#detailed-description)


`#include <time_series.hpp>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[TimeWindow](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeWindow/#function-timewindow)**(const ptime & startDate, const ptime & endDate) |
| Tts * | **[Trim](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeWindow/#function-trim)**(const Tts & timeSeries) const |

## Detailed Description

```cpp
template <typename Tts  =TimeSeries>
class datatypes::timeseries::TimeWindow;
```

An object that represents a time window, defining subset/trim operations on time series. 

**Template Parameters**: 

  * **T** Generic type parameter, element type of the time series 

## Public Functions Documentation

### function TimeWindow

```cpp
inline TimeWindow(
    const ptime & startDate,
    const ptime & endDate
)
```


### function Trim

```cpp
inline Tts * Trim(
    const Tts & timeSeries
) const
```


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000