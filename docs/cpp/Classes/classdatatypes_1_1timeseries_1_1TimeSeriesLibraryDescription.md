---
title: datatypes::timeseries::TimeSeriesLibraryDescription

---

# datatypes::timeseries::TimeSeriesLibraryDescription






`#include <time_series_store.hpp>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| void | **[AddSingle](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/#function-addsingle)**(const string & dataId, const [TimeSeriesSourceInfo](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/) & t) |
| void | **[AddEnsembleTs](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/#function-addensemblets)**(const string & dataId, const [TimeSeriesSourceInfo](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/) & t) |
| void | **[AddTsEnsembleTs](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/#function-addtsensemblets)**(const string & dataId, const [TimeSeriesSourceInfo](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/) & t) |
| boost::filesystem::path | **[GetFullPath](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/#function-getfullpath)**(const string & relativePath) const |
| string | **[GetRootDirectory](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/#function-getrootdirectory)**() const |
| vector< string > | **[GetDataIdSingle](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/#function-getdataidsingle)**() const |
| vector< string > | **[GetDataIdEnsembleTs](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/#function-getdataidensemblets)**() const |
| vector< string > | **[GetDataIdTsEnsembleTs](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/#function-getdataidtsensemblets)**() const |
| std::map< string, string > | **[GetSerializableConfiguration](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/#function-getserializableconfiguration)**(const string & dataId, const vector< string > & mandatoryKeys =vector< string >({})) const |
| void | **[SetLoadedFileName](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/#function-setloadedfilename)**(const string & fileName) |
| void | **[SetDataPath](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/#function-setdatapath)**(const string & dataPath) |
| string | **[GetDataPath](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/#function-getdatapath)**() const |
| [SingleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/)< double > * | **[CreateSingleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/#function-createsingletimeseriesstore)**(const string & dataId) const |
| [EnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/)< double > * | **[CreateEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/#function-createensembletimeseriesstore)**(const string & dataId) const |
| [TimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)< double > * | **[CreateTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/#function-createtimeseriesensembletimeseriesstore)**(const string & dataId) const |

## Friends

|                | Name           |
| -------------- | -------------- |
| class | **[TimeSeriesLibrary](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/#friend-timeserieslibrary)**  |

## Public Functions Documentation

### function AddSingle

```cpp
void AddSingle(
    const string & dataId,
    const TimeSeriesSourceInfo & t
)
```


### function AddEnsembleTs

```cpp
void AddEnsembleTs(
    const string & dataId,
    const TimeSeriesSourceInfo & t
)
```


### function AddTsEnsembleTs

```cpp
void AddTsEnsembleTs(
    const string & dataId,
    const TimeSeriesSourceInfo & t
)
```


### function GetFullPath

```cpp
boost::filesystem::path GetFullPath(
    const string & relativePath
) const
```


### function GetRootDirectory

```cpp
string GetRootDirectory() const
```


### function GetDataIdSingle

```cpp
vector< string > GetDataIdSingle() const
```


### function GetDataIdEnsembleTs

```cpp
vector< string > GetDataIdEnsembleTs() const
```


### function GetDataIdTsEnsembleTs

```cpp
vector< string > GetDataIdTsEnsembleTs() const
```


### function GetSerializableConfiguration

```cpp
std::map< string, string > GetSerializableConfiguration(
    const string & dataId,
    const vector< string > & mandatoryKeys =vector< string >({})
) const
```


### function SetLoadedFileName

```cpp
void SetLoadedFileName(
    const string & fileName
)
```


### function SetDataPath

```cpp
void SetDataPath(
    const string & dataPath
)
```


### function GetDataPath

```cpp
string GetDataPath() const
```


### function CreateSingleTimeSeriesStore

```cpp
SingleTimeSeriesStore< double > * CreateSingleTimeSeriesStore(
    const string & dataId
) const
```


### function CreateEnsembleTimeSeriesStore

```cpp
EnsembleTimeSeriesStore< double > * CreateEnsembleTimeSeriesStore(
    const string & dataId
) const
```


### function CreateTimeSeriesEnsembleTimeSeriesStore

```cpp
TimeSeriesEnsembleTimeSeriesStore< double > * CreateTimeSeriesEnsembleTimeSeriesStore(
    const string & dataId
) const
```


## Friends

### friend TimeSeriesLibrary

```cpp
friend class TimeSeriesLibrary(
    TimeSeriesLibrary 
);
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000