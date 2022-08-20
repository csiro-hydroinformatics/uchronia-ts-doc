---
title: datatypes::timeseries::DimensionsDefinitions

---

# datatypes::timeseries::DimensionsDefinitions






`#include <time_series_io.hpp>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#function-dimensionsdefinitions)**(const size_t ensembleSize, const vector< double > & leadTimeVar, const string & timeUnits, const vector< double > & timeVar, const vector< string > & stationIds =[DEFAULT_STATION_IDENTIFIER](/uchronia-ts-doc/cpp/Files/common_8h/#define-default-station-identifier), const string & leadTimeUnits ="") |
| | **[DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#function-dimensionsdefinitions)**(const string & timeUnits, const vector< double > & timeVar, const vector< string > & stationIds =[DEFAULT_STATION_IDENTIFIER](/uchronia-ts-doc/cpp/Files/common_8h/#define-default-station-identifier), const string & leadTimeUnits ="") |
| | **[DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#function-dimensionsdefinitions)**(ptime tsEnsStart, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & mainTimeStep, size_t tsLength, size_t ensembleSize, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & fcastTimeStep, size_t leadTimeSize, int fcastOffset =1, const vector< string > & stationIds =[DEFAULT_STATION_IDENTIFIER](/uchronia-ts-doc/cpp/Files/common_8h/#define-default-station-identifier), const string & leadTimeUnits ="") |
| | **[DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#function-dimensionsdefinitions)**() |
| | **[DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#function-dimensionsdefinitions)**([DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) && src) |
| | **[DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#function-dimensionsdefinitions)**(const [DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) & src) |
| [DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) & | **[operator=](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#function-operator=)**([DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) && src) |
| [DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) & | **[operator=](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#function-operator=)**(const [DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) & src) |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| size_t | **[EnsembleSize](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#variable-ensemblesize)**  |
| vector< double > | **[LeadTimeVar](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#variable-leadtimevar)**  |
| string | **[TimeUnits](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#variable-timeunits)**  |
| vector< double > | **[TimeVar](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#variable-timevar)**  |
| vector< string > | **[StationIds](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#variable-stationids)**  |
| string | **[LeadTimeUnits](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/#variable-leadtimeunits)**  |

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

Updated on 2022-08-20 at 19:28:22 +1000