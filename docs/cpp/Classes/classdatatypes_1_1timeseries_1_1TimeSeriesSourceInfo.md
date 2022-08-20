---
title: datatypes::timeseries::TimeSeriesSourceInfo

---

# datatypes::timeseries::TimeSeriesSourceInfo






`#include <time_series_store.hpp>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[TimeSeriesSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/#function-timeseriessourceinfo)**(const [TimeSeriesSourceInfoImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/) & t) |
| | **[TimeSeriesSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/#function-timeseriessourceinfo)**(const [TimeSeriesSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/) & src) |
| | **[TimeSeriesSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/#function-timeseriessourceinfo)**() |
| virtual | **[~TimeSeriesSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/#function-~timeseriessourceinfo)**() |
| | **[TimeSeriesSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/#function-timeseriessourceinfo)**([TimeSeriesSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/) && src) |
| [TimeSeriesSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/) & | **[operator=](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/#function-operator=)**(const [TimeSeriesSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/) & src) |
| [TimeSeriesSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/) & | **[operator=](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/#function-operator=)**([TimeSeriesSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/) && src) |
| [SingleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/)< double > * | **[CreateSingleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/#function-createsingletimeseriesstore)**() const |
| [EnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/)< double > * | **[CreateEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/#function-createensembletimeseriesstore)**() const |
| [TimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)< double > * | **[CreateTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/#function-createtimeseriesensembletimeseriesstore)**() const |
| bool | **[ApplyRootDir](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/#function-applyrootdir)**(const string & rootDir) |
| std::map< string, string > | **[GetSerializableConfiguration](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/#function-getserializableconfiguration)**() const |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| const string | **[IdDataKey](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/#variable-iddatakey)**  |
| const string | **[SingleSeriesTypeId](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/#variable-singleseriestypeid)**  |
| const string | **[EnsembleSeriesTypeId](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/#variable-ensembleseriestypeid)**  |
| const string | **[TimeSeriesEnsemblesTypeId](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/#variable-timeseriesensemblestypeid)**  |
| const string | **[SingleSeriesCollectionTypeId](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/#variable-singleseriescollectiontypeid)**  |

## Public Functions Documentation

### function TimeSeriesSourceInfo

```cpp
TimeSeriesSourceInfo(
    const TimeSeriesSourceInfoImpl & t
)
```


### function TimeSeriesSourceInfo

```cpp
TimeSeriesSourceInfo(
    const TimeSeriesSourceInfo & src
)
```


### function TimeSeriesSourceInfo

```cpp
TimeSeriesSourceInfo()
```


### function ~TimeSeriesSourceInfo

```cpp
virtual ~TimeSeriesSourceInfo()
```


### function TimeSeriesSourceInfo

```cpp
TimeSeriesSourceInfo(
    TimeSeriesSourceInfo && src
)
```


### function operator=

```cpp
TimeSeriesSourceInfo & operator=(
    const TimeSeriesSourceInfo & src
)
```


### function operator=

```cpp
TimeSeriesSourceInfo & operator=(
    TimeSeriesSourceInfo && src
)
```


### function CreateSingleTimeSeriesStore

```cpp
SingleTimeSeriesStore< double > * CreateSingleTimeSeriesStore() const
```


### function CreateEnsembleTimeSeriesStore

```cpp
EnsembleTimeSeriesStore< double > * CreateEnsembleTimeSeriesStore() const
```


### function CreateTimeSeriesEnsembleTimeSeriesStore

```cpp
TimeSeriesEnsembleTimeSeriesStore< double > * CreateTimeSeriesEnsembleTimeSeriesStore() const
```


### function ApplyRootDir

```cpp
bool ApplyRootDir(
    const string & rootDir
)
```


### function GetSerializableConfiguration

```cpp
std::map< string, string > GetSerializableConfiguration() const
```


## Public Attributes Documentation

### variable IdDataKey

```cpp
static const string IdDataKey;
```


### variable SingleSeriesTypeId

```cpp
static const string SingleSeriesTypeId;
```


### variable EnsembleSeriesTypeId

```cpp
static const string EnsembleSeriesTypeId;
```


### variable TimeSeriesEnsemblesTypeId

```cpp
static const string TimeSeriesEnsemblesTypeId;
```


### variable SingleSeriesCollectionTypeId

```cpp
static const string SingleSeriesCollectionTypeId;
```


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000