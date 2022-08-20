---
title: datatypes::timeseries::DimensionsDefinitions

---

# datatypes::timeseries::DimensionsDefinitions






`#include <time_series_io.hpp>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[DimensionsDefinitions](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#function-dimensionsdefinitions)**(const size_t ensembleSize, const vector< double > & leadTimeVar, const string & timeUnits, const vector< double > & timeVar, const vector< string > & stationIds =[DEFAULT_STATION_IDENTIFIER](/cpp/Files/common_8h/#define-default-station-identifier), const string & leadTimeUnits ="") |
| | **[DimensionsDefinitions](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#function-dimensionsdefinitions)**(const string & timeUnits, const vector< double > & timeVar, const vector< string > & stationIds =[DEFAULT_STATION_IDENTIFIER](/cpp/Files/common_8h/#define-default-station-identifier), const string & leadTimeUnits ="") |
| | **[DimensionsDefinitions](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#function-dimensionsdefinitions)**(ptime tsEnsStart, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & mainTimeStep, size_t tsLength, size_t ensembleSize, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & fcastTimeStep, size_t leadTimeSize, int fcastOffset =1, const vector< string > & stationIds =[DEFAULT_STATION_IDENTIFIER](/cpp/Files/common_8h/#define-default-station-identifier), const string & leadTimeUnits ="") |
| | **[DimensionsDefinitions](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#function-dimensionsdefinitions)**() |
| | **[DimensionsDefinitions](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#function-dimensionsdefinitions)**([DimensionsDefinitions](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) && src) |
| | **[DimensionsDefinitions](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#function-dimensionsdefinitions)**(const [DimensionsDefinitions](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) & src) |
| [DimensionsDefinitions](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) & | **[operator=](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#function-operator=)**([DimensionsDefinitions](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) && src) |
| [DimensionsDefinitions](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) & | **[operator=](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#function-operator=)**(const [DimensionsDefinitions](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) & src) |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| size_t | **[EnsembleSize](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#variable-ensemblesize)**  |
| vector< double > | **[LeadTimeVar](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#variable-leadtimevar)**  |
| string | **[TimeUnits](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#variable-timeunits)**  |
| vector< double > | **[TimeVar](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#variable-timevar)**  |
| vector< string > | **[StationIds](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#variable-stationids)**  |
| string | **[LeadTimeUnits](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#variable-leadtimeunits)**  |

## Public Functions Documentation

### function DimensionsDefinitions

```cpp
DimensionsDefinitions(
    const size_t ensembleSize,
    const vector< double > & leadTimeVar,
    const string & timeUnits,
    const vector< double > & timeVar,
    const vector< string > & stationIds =DEFAULT_STATION_IDENTIFIER,
    const string & leadTimeUnits =""
)
```


### function DimensionsDefinitions

```cpp
DimensionsDefinitions(
    const string & timeUnits,
    const vector< double > & timeVar,
    const vector< string > & stationIds =DEFAULT_STATION_IDENTIFIER,
    const string & leadTimeUnits =""
)
```


### function DimensionsDefinitions

```cpp
DimensionsDefinitions(
    ptime tsEnsStart,
    const TimeStep & mainTimeStep,
    size_t tsLength,
    size_t ensembleSize,
    const TimeStep & fcastTimeStep,
    size_t leadTimeSize,
    int fcastOffset =1,
    const vector< string > & stationIds =DEFAULT_STATION_IDENTIFIER,
    const string & leadTimeUnits =""
)
```


### function DimensionsDefinitions

```cpp
DimensionsDefinitions()
```


### function DimensionsDefinitions

```cpp
DimensionsDefinitions(
    DimensionsDefinitions && src
)
```


### function DimensionsDefinitions

```cpp
DimensionsDefinitions(
    const DimensionsDefinitions & src
)
```


### function operator=

```cpp
DimensionsDefinitions & operator=(
    DimensionsDefinitions && src
)
```


### function operator=

```cpp
DimensionsDefinitions & operator=(
    const DimensionsDefinitions & src
)
```


## Public Attributes Documentation

### variable EnsembleSize

```cpp
size_t EnsembleSize;
```


### variable LeadTimeVar

```cpp
vector< double > LeadTimeVar;
```


### variable TimeUnits

```cpp
string TimeUnits;
```


### variable TimeVar

```cpp
vector< double > TimeVar;
```


### variable StationIds

```cpp
vector< string > StationIds;
```


### variable LeadTimeUnits

```cpp
string LeadTimeUnits;
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000