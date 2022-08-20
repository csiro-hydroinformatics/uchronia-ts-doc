---
title: datatypes::timeseries::TimeSeriesOperations

---

# datatypes::timeseries::TimeSeriesOperations



 [More...](#detailed-description)


`#include <time_series.hpp>`

## Public Types

|                | Name           |
| -------------- | -------------- |
| using typename Tts::ElementType | **[ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-elementtype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-elementtype) >::[SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) | **[SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-elementtype) >::[PtrSeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-ptrseriestype) | **[PtrSeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-ptrseriestype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-elementtype) >::[EnsembleType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-ensembletype) | **[EnsembleType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-ensembletype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-elementtype) >::[EnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-ensembleptrtype) | **[EnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-ensembleptrtype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-elementtype) >::[PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-ptrensembleptrtype) | **[PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-ptrensembleptrtype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-elementtype) >::[TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-tseriesensembleptrtype) | **[TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-tseriesensembleptrtype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-elementtype) >::[PtrTSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-ptrtseriesensembleptrtype) | **[PtrTSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-ptrtseriesensembleptrtype)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| [PtrSeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-ptrseriestype) | **[TrimTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-trimtimeseries)**(const [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) & timeSeries, const ptime & startDate, const ptime & endDate) |
| [PtrSeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-ptrseriestype) | **[Resample](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-resample)**(const [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) & timeSeries, const string & method) |
| [PtrSeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-ptrseriestype) | **[DailyToHourly](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-dailytohourly)**(const [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) & dailyTimeSeries) |
| [PtrSeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-ptrseriestype) | **[JoinTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-jointimeseries)**(const [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) & head, const [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) & tail) |
| [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) | **[AggregateTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-aggregatetimestep)**(const [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) & series, const string & argument) |
| [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) | **[DisaggregateTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-disaggregatetimestep)**(const [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) & series, const string & argument) |
| void | **[AggregateTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-aggregatetimestep)**([SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) & series, const string & argument) |
| void | **[DisaggregateTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-disaggregatetimestep)**([SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) & series, const string & argument) |
| void | **[TransformEachItem](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-transformeachitem)**([TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-tseriesensembleptrtype) & efts, const string & method, const string & methodArgument) |
| ptime | **[GetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-getstart)**(const [TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-tseriesensembleptrtype) & ensTs, size_t index =0) |
| ptime | **[GetEnd](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-getend)**(const [TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-tseriesensembleptrtype) & ensTs, size_t index =0) |
| void | **[CreateForecast](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-createforecast)**([TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-tseriesensembleptrtype) & forecast, const [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) & observations, const ptime & start, size_t length, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & issueTimeStep, size_t leadTime, size_t offsetForecasts) |
| [TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-tseriesensembleptrtype) * | **[CreateForecastPtr](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-createforecastptr)**(const [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) & observations, const ptime & start, size_t length, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & issueTimeStep, size_t leadTime, size_t offsetForecasts) |
| [TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-tseriesensembleptrtype) | **[CreateForecast](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-createforecast)**(const [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) & observations, const ptime & start, size_t length, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & issueTimeStep, size_t leadTime, size_t offsetForecasts) |
| template <typename U \> <br>bool | **[AreEqual](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-areequal)**(const [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) & a, const U & b, bool strict =false, double tolerance =1e-12) |
| bool | **[AreTimeSeriesEqual](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-aretimeseriesequal)**(const [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) & a, const [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) & b, bool strict =false, double tolerance =1e-12) |
| bool | **[AreTimeSeriesEqual](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-aretimeseriesequal)**(const [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) & a, const [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) & b, const ptime & from, const ptime & to, bool strict =false, double tolerance =1e-12) |
| bool | **[AreValueEqual](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-arevalueequal)**(const [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) & a, const vector< [ElementType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-elementtype) > & b, size_t from =0, size_t to =std::numeric_limits< size_t >::max(), bool strict =false, double tolerance =1e-12) |
| bool | **[AreEnsembleTimeSeriesEqual](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-areensembletimeseriesequal)**([EnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-ensembleptrtype) & a, [EnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-ensembleptrtype) & b) |
| bool | **[AreEnsembleTimeSeriesEqual](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-areensembletimeseriesequal)**([EnsembleType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-ensembletype) & a, [EnsembleType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-ensembletype) & b) |
| bool | **[AreTimeSeriesEnsembleTimeSeriesEqual](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-aretimeseriesensembletimeseriesequal)**([TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-tseriesensembleptrtype) & a, [TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-tseriesensembleptrtype) & b) |
| template <typename T  =typename Tts::ElementType\> <br>[PtrSeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-ptrseriestype) | **[MaskTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#function-masktimeseries)**(const [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/#using-seriestype) & timeSeries, const ptime & start, const ptime & end, T maskValue) |

## Detailed Description

```cpp
template <typename Tts  =TimeSeries>
class datatypes::timeseries::TimeSeriesOperations;
```

## Public Types Documentation

### using ElementType

```cpp
using datatypes::timeseries::TimeSeriesOperations< Tts >::ElementType =  typename Tts::ElementType;
```


### using SeriesType

```cpp
using datatypes::timeseries::TimeSeriesOperations< Tts >::SeriesType =  typename CommonTypes<ElementType>::SeriesType;
```


### using PtrSeriesType

```cpp
using datatypes::timeseries::TimeSeriesOperations< Tts >::PtrSeriesType =  typename CommonTypes<ElementType>::PtrSeriesType;
```


### using EnsembleType

```cpp
using datatypes::timeseries::TimeSeriesOperations< Tts >::EnsembleType =  typename CommonTypes<ElementType>::EnsembleType;
```


### using EnsemblePtrType

```cpp
using datatypes::timeseries::TimeSeriesOperations< Tts >::EnsemblePtrType =  typename CommonTypes<ElementType>::EnsemblePtrType;
```


### using PtrEnsemblePtrType

```cpp
using datatypes::timeseries::TimeSeriesOperations< Tts >::PtrEnsemblePtrType =  typename CommonTypes<ElementType>::PtrEnsemblePtrType;
```


### using TSeriesEnsemblePtrType

```cpp
using datatypes::timeseries::TimeSeriesOperations< Tts >::TSeriesEnsemblePtrType =  typename CommonTypes<ElementType>::TSeriesEnsemblePtrType;
```


### using PtrTSeriesEnsemblePtrType

```cpp
using datatypes::timeseries::TimeSeriesOperations< Tts >::PtrTSeriesEnsemblePtrType =  typename CommonTypes<ElementType>::PtrTSeriesEnsemblePtrType;
```


## Public Functions Documentation

### function TrimTimeSeries

```cpp
static inline PtrSeriesType TrimTimeSeries(
    const SeriesType & timeSeries,
    const ptime & startDate,
    const ptime & endDate
)
```


### function Resample

```cpp
static inline PtrSeriesType Resample(
    const SeriesType & timeSeries,
    const string & method
)
```


### function DailyToHourly

```cpp
static inline PtrSeriesType DailyToHourly(
    const SeriesType & dailyTimeSeries
)
```


### function JoinTimeSeries

```cpp
static inline PtrSeriesType JoinTimeSeries(
    const SeriesType & head,
    const SeriesType & tail
)
```


### function AggregateTimeStep

```cpp
static inline SeriesType AggregateTimeStep(
    const SeriesType & series,
    const string & argument
)
```


### function DisaggregateTimeStep

```cpp
static inline SeriesType DisaggregateTimeStep(
    const SeriesType & series,
    const string & argument
)
```


### function AggregateTimeStep

```cpp
static inline void AggregateTimeStep(
    SeriesType & series,
    const string & argument
)
```


### function DisaggregateTimeStep

```cpp
static inline void DisaggregateTimeStep(
    SeriesType & series,
    const string & argument
)
```


### function TransformEachItem

```cpp
static inline void TransformEachItem(
    TSeriesEnsemblePtrType & efts,
    const string & method,
    const string & methodArgument
)
```


### function GetStart

```cpp
static inline ptime GetStart(
    const TSeriesEnsemblePtrType & ensTs,
    size_t index =0
)
```


### function GetEnd

```cpp
static inline ptime GetEnd(
    const TSeriesEnsemblePtrType & ensTs,
    size_t index =0
)
```


### function CreateForecast

```cpp
static inline void CreateForecast(
    TSeriesEnsemblePtrType & forecast,
    const SeriesType & observations,
    const ptime & start,
    size_t length,
    const TimeStep & issueTimeStep,
    size_t leadTime,
    size_t offsetForecasts
)
```


### function CreateForecastPtr

```cpp
static inline TSeriesEnsemblePtrType * CreateForecastPtr(
    const SeriesType & observations,
    const ptime & start,
    size_t length,
    const TimeStep & issueTimeStep,
    size_t leadTime,
    size_t offsetForecasts
)
```


### function CreateForecast

```cpp
static inline TSeriesEnsemblePtrType CreateForecast(
    const SeriesType & observations,
    const ptime & start,
    size_t length,
    const TimeStep & issueTimeStep,
    size_t leadTime,
    size_t offsetForecasts
)
```


### function AreEqual

```cpp
template <typename U >
static inline bool AreEqual(
    const SeriesType & a,
    const U & b,
    bool strict =false,
    double tolerance =1e-12
)
```


### function AreTimeSeriesEqual

```cpp
static inline bool AreTimeSeriesEqual(
    const SeriesType & a,
    const SeriesType & b,
    bool strict =false,
    double tolerance =1e-12
)
```


### function AreTimeSeriesEqual

```cpp
static inline bool AreTimeSeriesEqual(
    const SeriesType & a,
    const SeriesType & b,
    const ptime & from,
    const ptime & to,
    bool strict =false,
    double tolerance =1e-12
)
```


### function AreValueEqual

```cpp
static inline bool AreValueEqual(
    const SeriesType & a,
    const vector< ElementType > & b,
    size_t from =0,
    size_t to =std::numeric_limits< size_t >::max(),
    bool strict =false,
    double tolerance =1e-12
)
```


### function AreEnsembleTimeSeriesEqual

```cpp
static inline bool AreEnsembleTimeSeriesEqual(
    EnsemblePtrType & a,
    EnsemblePtrType & b
)
```


### function AreEnsembleTimeSeriesEqual

```cpp
static inline bool AreEnsembleTimeSeriesEqual(
    EnsembleType & a,
    EnsembleType & b
)
```


### function AreTimeSeriesEnsembleTimeSeriesEqual

```cpp
static inline bool AreTimeSeriesEnsembleTimeSeriesEqual(
    TSeriesEnsemblePtrType & a,
    TSeriesEnsemblePtrType & b
)
```


### function MaskTimeSeries

```cpp
template <typename T  =typename Tts::ElementType>
static inline PtrSeriesType MaskTimeSeries(
    const SeriesType & timeSeries,
    const ptime & start,
    const ptime & end,
    T maskValue
)
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000