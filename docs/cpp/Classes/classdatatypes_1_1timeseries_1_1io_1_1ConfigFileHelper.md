---
title: datatypes::timeseries::io::ConfigFileHelper

---

# datatypes::timeseries::io::ConfigFileHelper






`#include <time_series_io.hpp>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| [TimeSeriesLibraryDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/) | **[LoadTimeSeriesLibraryDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#function-loadtimeserieslibrarydescription)**(const string & filename, const string & dataPath ="", [TimeSeriesSourceInfoBuilder](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoBuilder/) * srcBuilder =nullptr) |
| void | **[SaveTimeSeriesLibraryDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#function-savetimeserieslibrarydescription)**(const [TimeSeriesLibraryDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/) & config, const string & filename) |
| string | **[FileName](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#function-filename)**(const YAML::Node & storage) |
| string | **[FullFileName](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#function-fullfilename)**(const YAML::Node & storage, const [TimeSeriesLibraryDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/) & tsl) |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| const string | **[FileKey](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-filekey)**  |
| const string | **[VarKey](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-varkey)**  |
| const string | **[IdentifierKey](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-identifierkey)**  |
| const string | **[IdDataKey](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-iddatakey)**  |
| const string | **[IndexKey](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-indexkey)**  |
| const string | **[TypeKey](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-typekey)**  |
| const string | **[TimeStepKey](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-timestepkey)**  |
| const string | **[StartKey](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-startkey)**  |
| const string | **[LengthKey](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-lengthkey)**  |
| const string | **[EnsembleSizeKey](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-ensemblesizekey)**  |
| const string | **[EnsembleLengthKey](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-ensemblelengthkey)**  |
| const string | **[EnsembleTimeStepKey](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-ensembletimestepkey)**  |
| const string | **[FilePatternKey](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-filepatternkey)**  |
| const string | **[MappingKey](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-mappingkey)**  |
| const string | **[StorageKey](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-storagekey)**  |
| const string | **[SingleSeriesTypeId](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-singleseriestypeid)**  |
| const string | **[EnsembleSeriesTypeId](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-ensembleseriestypeid)**  |
| const string | **[TimeSeriesEnsemblesTypeId](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-timeseriesensemblestypeid)**  |
| const string | **[SingleSeriesCollectionTypeId](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-singleseriescollectiontypeid)**  |
| const string | **[StorageTypeSingleNetcdfFile](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-storagetypesinglenetcdffile)**  |
| const string | **[StorageTypeMultipleNetcdfFiles](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/#variable-storagetypemultiplenetcdffiles)**  |

## Public Functions Documentation

### function LoadTimeSeriesLibraryDescription

```cpp
static TimeSeriesLibraryDescription LoadTimeSeriesLibraryDescription(
    const string & filename,
    const string & dataPath ="",
    TimeSeriesSourceInfoBuilder * srcBuilder =nullptr
)
```


### function SaveTimeSeriesLibraryDescription

```cpp
static void SaveTimeSeriesLibraryDescription(
    const TimeSeriesLibraryDescription & config,
    const string & filename
)
```


### function FileName

```cpp
static string FileName(
    const YAML::Node & storage
)
```


### function FullFileName

```cpp
static string FullFileName(
    const YAML::Node & storage,
    const TimeSeriesLibraryDescription & tsl
)
```


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


### variable IdDataKey

```cpp
static const string IdDataKey;
```


### variable IndexKey

```cpp
static const string IndexKey;
```


### variable TypeKey

```cpp
static const string TypeKey;
```


### variable TimeStepKey

```cpp
static const string TimeStepKey;
```


### variable StartKey

```cpp
static const string StartKey;
```


### variable LengthKey

```cpp
static const string LengthKey;
```


### variable EnsembleSizeKey

```cpp
static const string EnsembleSizeKey;
```


### variable EnsembleLengthKey

```cpp
static const string EnsembleLengthKey;
```


### variable EnsembleTimeStepKey

```cpp
static const string EnsembleTimeStepKey;
```


### variable FilePatternKey

```cpp
static const string FilePatternKey;
```


### variable MappingKey

```cpp
static const string MappingKey;
```


### variable StorageKey

```cpp
static const string StorageKey;
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