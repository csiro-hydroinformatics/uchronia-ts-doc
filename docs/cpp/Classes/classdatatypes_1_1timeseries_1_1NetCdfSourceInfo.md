---
title: datatypes::timeseries::NetCdfSourceInfo

---

# datatypes::timeseries::NetCdfSourceInfo






`#include <time_series_store.hpp>`

Inherits from [datatypes::timeseries::TimeSeriesSourceInfoImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[NetCdfSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-netcdfsourceinfo)**() |
| | **[NetCdfSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-netcdfsourceinfo)**(const string & dataId, const string & fileName, const string & ncVarName, const string & identifier ="", int index =-1, const string & storageType ="", const string & timeStep ="", const string & start ="", int length =-1, int ensembleSize =-1, int ensembleLength =-1, const string & ensembleTimeStep ="", const string & containingDirectory ="") |
| | **[NetCdfSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-netcdfsourceinfo)**(const string & dataId, const string & fileName, const string & ncVarName, const string & identifier, int index, const string & storageType, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep, const ptime & start, int length, int ensembleSize, int ensembleLength, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & ensembleTimeStep) |
| virtual [TimeSeriesSourceInfoImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/) * | **[Clone](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-clone)**() const |
| virtual bool | **[ApplyRootDir](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-applyrootdir)**(const string & rootDir) |
| virtual [SingleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/)< double > * | **[CreateSingleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-createsingletimeseriesstore)**() const |
| virtual [EnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/)< double > * | **[CreateEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-createensembletimeseriesstore)**() const |
| virtual [TimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)< double > * | **[CreateTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-createtimeseriesensembletimeseriesstore)**() const |
| virtual std::map< string, string > | **[GetSerializableConfiguration](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#function-getserializableconfiguration)**() const |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| const string | **[FileKey](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#variable-filekey)**  |
| const string | **[VarKey](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#variable-varkey)**  |
| const string | **[IdentifierKey](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#variable-identifierkey)**  |
| const string | **[IndexKey](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#variable-indexkey)**  |
| const string | **[TypeKey](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#variable-typekey)**  |
| const string | **[StorageTypeSingleNetcdfFile](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#variable-storagetypesinglenetcdffile)**  |
| const string | **[StorageTypeMultipleNetcdfFiles](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/#variable-storagetypemultiplenetcdffiles)**  |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::TimeSeriesSourceInfoImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeSeriesSourceInfoImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-~timeseriessourceinfoimpl)**() |
| string | **[OptionalApplyRootDir](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-optionalapplyrootdir)**(const std::string & rootDir, const std::string & filename, bool checkDirExists =true) |

**Protected Functions inherited from [datatypes::timeseries::TimeSeriesSourceInfoImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/)**

|                | Name           |
| -------------- | -------------- |
| | **[TimeSeriesSourceInfoImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-timeseriessourceinfoimpl)**() |
| | **[TimeSeriesSourceInfoImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-timeseriessourceinfoimpl)**(const [TimeSeriesSourceInfoImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/) & src) |


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


**Reimplements**: [datatypes::timeseries::TimeSeriesSourceInfoImpl::Clone](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-clone)


### function ApplyRootDir

```cpp
virtual bool ApplyRootDir(
    const string & rootDir
)
```


**Reimplements**: [datatypes::timeseries::TimeSeriesSourceInfoImpl::ApplyRootDir](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-applyrootdir)


### function CreateSingleTimeSeriesStore

```cpp
virtual SingleTimeSeriesStore< double > * CreateSingleTimeSeriesStore() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesSourceInfoImpl::CreateSingleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-createsingletimeseriesstore)


### function CreateEnsembleTimeSeriesStore

```cpp
virtual EnsembleTimeSeriesStore< double > * CreateEnsembleTimeSeriesStore() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesSourceInfoImpl::CreateEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-createensembletimeseriesstore)


### function CreateTimeSeriesEnsembleTimeSeriesStore

```cpp
virtual TimeSeriesEnsembleTimeSeriesStore< double > * CreateTimeSeriesEnsembleTimeSeriesStore() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesSourceInfoImpl::CreateTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-createtimeseriesensembletimeseriesstore)


### function GetSerializableConfiguration

```cpp
virtual std::map< string, string > GetSerializableConfiguration() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesSourceInfoImpl::GetSerializableConfiguration](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/#function-getserializableconfiguration)


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

Updated on 2022-08-20 at 19:28:22 +1000