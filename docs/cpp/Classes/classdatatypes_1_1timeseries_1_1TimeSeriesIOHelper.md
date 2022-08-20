---
title: datatypes::timeseries::TimeSeriesIOHelper
summary: Representation of an univariate, ensemble time series with a SWIFT netCDF back end. 

---

# datatypes::timeseries::TimeSeriesIOHelper



Representation of an univariate, ensemble time series with a SWIFT netCDF back end.  [More...](#detailed-description)


`#include <time_series_io.hpp>`

## Public Types

|                | Name           |
| -------------- | -------------- |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#using-seriestype) | **[SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#using-seriestype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[PtrSeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#using-ptrseriestype) | **[PtrSeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#using-ptrseriestype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[EnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#using-ensembleptrtype) | **[EnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#using-ensembleptrtype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#using-ptrensembleptrtype) | **[PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#using-ptrensembleptrtype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#using-tseriesensembleptrtype) | **[TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#using-tseriesensembleptrtype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[PtrTSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#using-ptrtseriesensembleptrtype) | **[PtrTSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#using-ptrtseriesensembleptrtype)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#using-seriestype) * | **[Read](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#function-read)**(const string & netCdfFilePath, const string & varName, const string & identifier) |
| void | **[Write](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#function-write)**(const string & varName, std::map< string, [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > * > & recordedTimeSeries, const std::map< string, string > & idMap, const string & filePath) |
| void | **[Write](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#function-write)**([DimensionsDefinitions](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) & dimDefinitions, const map< std::string, [VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) > & varDefinitions, const [GlobalAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) & GlobalAttributes, std::map< string, [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > * > & recordedTimeSeries, const string & filePath) |
| [PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#using-ptrensembleptrtype) | **[ReadForecastTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#function-readforecasttimeseries)**(const string & netCdfFilepath, const string & varName, const string & identifier, int index) |
| [PtrTSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#using-ptrtseriesensembleptrtype) | **[ReadForecastTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#function-readforecasttimeseries)**(const string & netCdfFilepath, const string & varName, const string & identifier) |
| [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#using-seriestype) * | **[Read](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#function-read)**(const string & netCdfFilePath, const string & varName, const string & identifier, const [TimeWindow](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeWindow/)< [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#using-seriestype) > & window) |
| [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#using-seriestype) * | **[ReadDailyToHourly](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#function-readdailytohourly)**(const string & netCdfFilePath, const string & varName, const string & identifier, const [TimeWindow](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeWindow/)< [SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/#using-seriestype) > & window) |

## Detailed Description

```cpp
template <typename T >
class datatypes::timeseries::TimeSeriesIOHelper;
```

Representation of an univariate, ensemble time series with a SWIFT netCDF back end. 

**Template Parameters**: 

  * **T** The type of the elements in the series; typically double or float. 

## Public Types Documentation

### using SeriesType

```cpp
using datatypes::timeseries::TimeSeriesIOHelper< T >::SeriesType =  typename CommonTypes<T>::SeriesType;
```


### using PtrSeriesType

```cpp
using datatypes::timeseries::TimeSeriesIOHelper< T >::PtrSeriesType =  typename CommonTypes<T>::PtrSeriesType;
```


### using EnsemblePtrType

```cpp
using datatypes::timeseries::TimeSeriesIOHelper< T >::EnsemblePtrType =  typename CommonTypes<T>::EnsemblePtrType;
```


### using PtrEnsemblePtrType

```cpp
using datatypes::timeseries::TimeSeriesIOHelper< T >::PtrEnsemblePtrType =  typename CommonTypes<T>::PtrEnsemblePtrType;
```


### using TSeriesEnsemblePtrType

```cpp
using datatypes::timeseries::TimeSeriesIOHelper< T >::TSeriesEnsemblePtrType =  typename CommonTypes<T>::TSeriesEnsemblePtrType;
```


### using PtrTSeriesEnsemblePtrType

```cpp
using datatypes::timeseries::TimeSeriesIOHelper< T >::PtrTSeriesEnsemblePtrType =  typename CommonTypes<T>::PtrTSeriesEnsemblePtrType;
```


## Public Functions Documentation

### function Read

```cpp
static SeriesType * Read(
    const string & netCdfFilePath,
    const string & varName,
    const string & identifier
)
```


### function Write

```cpp
static void Write(
    const string & varName,
    std::map< string, TTimeSeries< T > * > & recordedTimeSeries,
    const std::map< string, string > & idMap,
    const string & filePath
)
```


### function Write

```cpp
static void Write(
    DimensionsDefinitions & dimDefinitions,
    const map< std::string, VariableDefinition > & varDefinitions,
    const GlobalAttributes & GlobalAttributes,
    std::map< string, TTimeSeries< T > * > & recordedTimeSeries,
    const string & filePath
)
```


### function ReadForecastTimeSeries

```cpp
static PtrEnsemblePtrType ReadForecastTimeSeries(
    const string & netCdfFilepath,
    const string & varName,
    const string & identifier,
    int index
)
```


### function ReadForecastTimeSeries

```cpp
static PtrTSeriesEnsemblePtrType ReadForecastTimeSeries(
    const string & netCdfFilepath,
    const string & varName,
    const string & identifier
)
```


### function Read

```cpp
static inline SeriesType * Read(
    const string & netCdfFilePath,
    const string & varName,
    const string & identifier,
    const TimeWindow< SeriesType > & window
)
```


### function ReadDailyToHourly

```cpp
static inline SeriesType * ReadDailyToHourly(
    const string & netCdfFilePath,
    const string & varName,
    const string & identifier,
    const TimeWindow< SeriesType > & window
)
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000