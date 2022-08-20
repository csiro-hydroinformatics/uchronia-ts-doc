---
title: datatypes::timeseries::TimeSeriesLibraryFactory

---

# datatypes::timeseries::TimeSeriesLibraryFactory






`#include <time_series_io.hpp>`

## Public Types

|                | Name           |
| -------------- | -------------- |
| using [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< double > * | **[PtrSeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/#using-ptrseriestype)**  |
| using [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< double > | **[SeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/#using-seriestype)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| [TimeSeriesLibrary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/) | **[CreateLibrary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/#function-createlibrary)**(const [TimeSeriesLibraryDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/) & description) |
| [TimeSeriesLibrary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/) * | **[CreateLibraryPtr](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/#function-createlibraryptr)**(const [TimeSeriesLibraryDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/) & description) |
| [TimeSeriesLibrary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/) | **[LoadTimeSeriesLibrary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/#function-loadtimeserieslibrary)**(const string & filepath, const string & dataPath ="") |
| [TimeSeriesLibrary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/) * | **[LoadTimeSeriesLibraryPtr](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/#function-loadtimeserieslibraryptr)**(const string & filepath, const string & dataPath ="") |
| [TimeSeriesLibrary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/) * | **[CreateTimeSeriesLibraryPtr](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/#function-createtimeserieslibraryptr)**(const string & type) |
| [SingleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/)< double > * | **[CreateTsSource](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/#function-createtssource)**(const string & ncFilename, const string & ncVarName, const string & ncIdentifier) |
| [EnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/)< double > * | **[CreateEnsTsSource](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/#function-createenstssource)**(const string & ncFilename, const string & ncVarName, const string & ncIdentifier) |
| [TimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)< double > * | **[CreateTsEnsTsSource](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/#function-createtsenstssource)**(const string & ncFilename, const string & ncVarName, const string & ncIdentifier) |
| [EnsembleForecastTimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-ensembleforecasttimeseries)< [SeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/#using-seriestype) > * | **[LoadTsEnsTs](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/#function-loadtsensts)**(const string & ncFilename, const string & ncVarName, const string & ncIdentifier, const string & dataId) |
| [TimeSeriesSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/) | **[CreateNetcdfSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/#function-createnetcdfsourceinfo)**(const string & dataId, const string & storageType, const string & ncFilename, const string & ncVarName, const string & ncIdentifier) |
| [TimeSeriesSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/) | **[CreateNetcdfSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/#function-createnetcdfsourceinfo)**(const string & dataId, const string & storageType, const string & ncFilename, const string & ncVarName, const string & ncIdentifier, int index, const string & timeStep, const string & start, int length, int ensembleSize) |
| [TimeSeriesSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/) | **[CreateNetcdfSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/#function-createnetcdfsourceinfo)**(const string & dataId, const string & storageType, const string & ncFilename, const string & ncVarName, const string & ncIdentifier, int index, const string & timeStep, const string & start, int length, int ensembleSize, int ensembleLength, const string & ensembleTimeStep) |
| bool | **[HasTimeSeriesSourceInfoBuilderRegistered](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/#function-hastimeseriessourceinfobuilderregistered)**() |
| void | **[RegisterTimeSeriesSourceInfoBuilder](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/#function-registertimeseriessourceinfobuilder)**([TimeSeriesSourceInfoBuilder](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoBuilder/) * srcBuilder) |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| const string | **[kTestRecorderKey](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/#variable-ktestrecorderkey)**  |
| const string | **[kTimeSeriesEnsemblesKey](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/#variable-ktimeseriesensembleskey)**  |

## Public Types Documentation

### using PtrSeriesType

```cpp
using datatypes::timeseries::TimeSeriesLibraryFactory::PtrSeriesType =  TTimeSeries<double>*;
```


### using SeriesType

```cpp
using datatypes::timeseries::TimeSeriesLibraryFactory::SeriesType =  TTimeSeries<double>;
```


## Public Functions Documentation

### function CreateLibrary

```cpp
static TimeSeriesLibrary CreateLibrary(
    const TimeSeriesLibraryDescription & description
)
```


### function CreateLibraryPtr

```cpp
static TimeSeriesLibrary * CreateLibraryPtr(
    const TimeSeriesLibraryDescription & description
)
```


### function LoadTimeSeriesLibrary

```cpp
static TimeSeriesLibrary LoadTimeSeriesLibrary(
    const string & filepath,
    const string & dataPath =""
)
```


### function LoadTimeSeriesLibraryPtr

```cpp
static TimeSeriesLibrary * LoadTimeSeriesLibraryPtr(
    const string & filepath,
    const string & dataPath =""
)
```


### function CreateTimeSeriesLibraryPtr

```cpp
static TimeSeriesLibrary * CreateTimeSeriesLibraryPtr(
    const string & type
)
```


### function CreateTsSource

```cpp
static SingleTimeSeriesStore< double > * CreateTsSource(
    const string & ncFilename,
    const string & ncVarName,
    const string & ncIdentifier
)
```


### function CreateEnsTsSource

```cpp
static EnsembleTimeSeriesStore< double > * CreateEnsTsSource(
    const string & ncFilename,
    const string & ncVarName,
    const string & ncIdentifier
)
```


### function CreateTsEnsTsSource

```cpp
static TimeSeriesEnsembleTimeSeriesStore< double > * CreateTsEnsTsSource(
    const string & ncFilename,
    const string & ncVarName,
    const string & ncIdentifier
)
```


### function LoadTsEnsTs

```cpp
static EnsembleForecastTimeSeries< SeriesType > * LoadTsEnsTs(
    const string & ncFilename,
    const string & ncVarName,
    const string & ncIdentifier,
    const string & dataId
)
```


### function CreateNetcdfSourceInfo

```cpp
static TimeSeriesSourceInfo CreateNetcdfSourceInfo(
    const string & dataId,
    const string & storageType,
    const string & ncFilename,
    const string & ncVarName,
    const string & ncIdentifier
)
```


### function CreateNetcdfSourceInfo

```cpp
static TimeSeriesSourceInfo CreateNetcdfSourceInfo(
    const string & dataId,
    const string & storageType,
    const string & ncFilename,
    const string & ncVarName,
    const string & ncIdentifier,
    int index,
    const string & timeStep,
    const string & start,
    int length,
    int ensembleSize
)
```


### function CreateNetcdfSourceInfo

```cpp
static TimeSeriesSourceInfo CreateNetcdfSourceInfo(
    const string & dataId,
    const string & storageType,
    const string & ncFilename,
    const string & ncVarName,
    const string & ncIdentifier,
    int index,
    const string & timeStep,
    const string & start,
    int length,
    int ensembleSize,
    int ensembleLength,
    const string & ensembleTimeStep
)
```


### function HasTimeSeriesSourceInfoBuilderRegistered

```cpp
static bool HasTimeSeriesSourceInfoBuilderRegistered()
```


### function RegisterTimeSeriesSourceInfoBuilder

```cpp
static void RegisterTimeSeriesSourceInfoBuilder(
    TimeSeriesSourceInfoBuilder * srcBuilder
)
```


## Public Attributes Documentation

### variable kTestRecorderKey

```cpp
static const string kTestRecorderKey;
```


### variable kTimeSeriesEnsemblesKey

```cpp
static const string kTimeSeriesEnsemblesKey;
```


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000