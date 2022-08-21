---
title: datatypes::timeseries::TimeSeriesSourceInfoImpl

---

# datatypes::timeseries::TimeSeriesSourceInfoImpl






`#include <time_series_store.hpp>`

Inherited by [datatypes::timeseries::NetCdfSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeSeriesSourceInfoImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-~timeseriessourceinfoimpl)**() |
| virtual [TimeSeriesSourceInfoImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/) * | **[Clone](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-clone)**() const =0 |
| virtual bool | **[ApplyRootDir](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-applyrootdir)**(const string & rootDir) |
| virtual [SingleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/)< double > * | **[CreateSingleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-createsingletimeseriesstore)**() const |
| virtual [EnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/)< double > * | **[CreateEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-createensembletimeseriesstore)**() const |
| virtual [TimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)< double > * | **[CreateTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-createtimeseriesensembletimeseriesstore)**() const |
| virtual std::map< string, string > | **[GetSerializableConfiguration](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-getserializableconfiguration)**() const |
| string | **[OptionalApplyRootDir](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-optionalapplyrootdir)**(const std::string & rootDir, const std::string & filename, bool checkDirExists =true) |

## Protected Functions

|                | Name           |
| -------------- | -------------- |
| | **[TimeSeriesSourceInfoImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-timeseriessourceinfoimpl)**() |
| | **[TimeSeriesSourceInfoImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-timeseriessourceinfoimpl)**(const [TimeSeriesSourceInfoImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/) & src) |

## Public Functions Documentation

### function ~TimeSeriesSourceInfoImpl

```cpp
virtual ~TimeSeriesSourceInfoImpl()
```


### function Clone

```cpp
virtual TimeSeriesSourceInfoImpl * Clone() const =0
```


**Reimplemented by**: [datatypes::timeseries::NetCdfSourceInfo::Clone](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-clone)


### function ApplyRootDir

```cpp
virtual bool ApplyRootDir(
    const string & rootDir
)
```


**Reimplemented by**: [datatypes::timeseries::NetCdfSourceInfo::ApplyRootDir](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-applyrootdir)


### function CreateSingleTimeSeriesStore

```cpp
virtual SingleTimeSeriesStore< double > * CreateSingleTimeSeriesStore() const
```


**Reimplemented by**: [datatypes::timeseries::NetCdfSourceInfo::CreateSingleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-createsingletimeseriesstore)


### function CreateEnsembleTimeSeriesStore

```cpp
virtual EnsembleTimeSeriesStore< double > * CreateEnsembleTimeSeriesStore() const
```


**Reimplemented by**: [datatypes::timeseries::NetCdfSourceInfo::CreateEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-createensembletimeseriesstore)


### function CreateTimeSeriesEnsembleTimeSeriesStore

```cpp
virtual TimeSeriesEnsembleTimeSeriesStore< double > * CreateTimeSeriesEnsembleTimeSeriesStore() const
```


**Reimplemented by**: [datatypes::timeseries::NetCdfSourceInfo::CreateTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-createtimeseriesensembletimeseriesstore)


### function GetSerializableConfiguration

```cpp
virtual std::map< string, string > GetSerializableConfiguration() const
```


**Reimplemented by**: [datatypes::timeseries::NetCdfSourceInfo::GetSerializableConfiguration](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-getserializableconfiguration)


### function OptionalApplyRootDir

```cpp
static string OptionalApplyRootDir(
    const std::string & rootDir,
    const std::string & filename,
    bool checkDirExists =true
)
```


## Protected Functions Documentation

### function TimeSeriesSourceInfoImpl

```cpp
TimeSeriesSourceInfoImpl()
```


### function TimeSeriesSourceInfoImpl

```cpp
TimeSeriesSourceInfoImpl(
    const TimeSeriesSourceInfoImpl & src
)
```


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000