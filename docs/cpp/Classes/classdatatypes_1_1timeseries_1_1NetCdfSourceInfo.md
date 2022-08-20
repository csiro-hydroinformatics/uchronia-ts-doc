---
title: datatypes::timeseries::NetCdfSourceInfo

---

# datatypes::timeseries::NetCdfSourceInfo






`#include <time_series_store.hpp>`

Inherits from [datatypes::timeseries::TimeSeriesSourceInfoImpl](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[NetCdfSourceInfo](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-netcdfsourceinfo)**() |
| | **[NetCdfSourceInfo](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-netcdfsourceinfo)**(const string & dataId, const string & fileName, const string & ncVarName, const string & identifier ="", int index =-1, const string & storageType ="", const string & timeStep ="", const string & start ="", int length =-1, int ensembleSize =-1, int ensembleLength =-1, const string & ensembleTimeStep ="", const string & containingDirectory ="") |
| | **[NetCdfSourceInfo](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-netcdfsourceinfo)**(const string & dataId, const string & fileName, const string & ncVarName, const string & identifier, int index, const string & storageType, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep, const ptime & start, int length, int ensembleSize, int ensembleLength, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & ensembleTimeStep) |
| virtual [TimeSeriesSourceInfoImpl](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/) * | **[Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-clone)**() const |
| virtual bool | **[ApplyRootDir](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-applyrootdir)**(const string & rootDir) |
| virtual [SingleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/)< double > * | **[CreateSingleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-createsingletimeseriesstore)**() const |
| virtual [EnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/)< double > * | **[CreateEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-createensembletimeseriesstore)**() const |
| virtual [TimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)< double > * | **[CreateTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-createtimeseriesensembletimeseriesstore)**() const |
| virtual std::map< string, string > | **[GetSerializableConfiguration](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-getserializableconfiguration)**() const |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| const string | **[FileKey](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#variable-filekey)**  |
| const string | **[VarKey](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#variable-varkey)**  |
| const string | **[IdentifierKey](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#variable-identifierkey)**  |
| const string | **[IndexKey](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#variable-indexkey)**  |
| const string | **[TypeKey](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#variable-typekey)**  |
| const string | **[StorageTypeSingleNetcdfFile](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#variable-storagetypesinglenetcdffile)**  |
| const string | **[StorageTypeMultipleNetcdfFiles](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#variable-storagetypemultiplenetcdffiles)**  |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::TimeSeriesSourceInfoImpl](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeSeriesSourceInfoImpl](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-~timeseriessourceinfoimpl)**() |
| string | **[OptionalApplyRootDir](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-optionalapplyrootdir)**(const std::string & rootDir, const std::string & filename, bool checkDirExists =true) |

**Protected Functions inherited from [datatypes::timeseries::TimeSeriesSourceInfoImpl](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/)**

|                | Name           |
| -------------- | -------------- |
| | **[TimeSeriesSourceInfoImpl](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-timeseriessourceinfoimpl)**() |
| | **[TimeSeriesSourceInfoImpl](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-timeseriessourceinfoimpl)**(const [TimeSeriesSourceInfoImpl](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/) & src) |


## Public Functions Documentation

### function NetCdfSourceInfo

```cpp
inline NetCdfSourceInfo()
```


### function NetCdfSourceInfo

```cpp
NetCdfSourceInfo(
    const string & dataId,
    const string & fileName,
    const string & ncVarName,
    const string & identifier ="",
    int index =-1,
    const string & storageType ="",
    const string & timeStep ="",
    const string & start ="",
    int length =-1,
    int ensembleSize =-1,
    int ensembleLength =-1,
    const string & ensembleTimeStep ="",
    const string & containingDirectory =""
)
```


### function NetCdfSourceInfo

```cpp
NetCdfSourceInfo(
    const string & dataId,
    const string & fileName,
    const string & ncVarName,
    const string & identifier,
    int index,
    const string & storageType,
    const TimeStep & timeStep,
    const ptime & start,
    int length,
    int ensembleSize,
    int ensembleLength,
    const TimeStep & ensembleTimeStep
)
```


### function Clone

```cpp
virtual TimeSeriesSourceInfoImpl * Clone() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesSourceInfoImpl::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-clone)


### function ApplyRootDir

```cpp
virtual bool ApplyRootDir(
    const string & rootDir
)
```


**Reimplements**: [datatypes::timeseries::TimeSeriesSourceInfoImpl::ApplyRootDir](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-applyrootdir)


### function CreateSingleTimeSeriesStore

```cpp
virtual SingleTimeSeriesStore< double > * CreateSingleTimeSeriesStore() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesSourceInfoImpl::CreateSingleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-createsingletimeseriesstore)


### function CreateEnsembleTimeSeriesStore

```cpp
virtual EnsembleTimeSeriesStore< double > * CreateEnsembleTimeSeriesStore() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesSourceInfoImpl::CreateEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-createensembletimeseriesstore)


### function CreateTimeSeriesEnsembleTimeSeriesStore

```cpp
virtual TimeSeriesEnsembleTimeSeriesStore< double > * CreateTimeSeriesEnsembleTimeSeriesStore() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesSourceInfoImpl::CreateTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-createtimeseriesensembletimeseriesstore)


### function GetSerializableConfiguration

```cpp
virtual std::map< string, string > GetSerializableConfiguration() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesSourceInfoImpl::GetSerializableConfiguration](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-getserializableconfiguration)


## Public Attributes Documentation

### variable FileKey

```cpp
static const string FileKey;
```


### variable VarKey

```cpp
static const string VarKey;
```


### variable IdentifierKey

```cpp
static const string IdentifierKey;
```


### variable IndexKey

```cpp
static const string IndexKey;
```


### variable TypeKey

```cpp
static const string TypeKey;
```


### variable StorageTypeSingleNetcdfFile

```cpp
static const string StorageTypeSingleNetcdfFile;
```


### variable StorageTypeMultipleNetcdfFiles

```cpp
static const string StorageTypeMultipleNetcdfFiles;
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000