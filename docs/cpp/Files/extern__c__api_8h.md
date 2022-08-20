---
title: datatypes/extern_c_api.h

---

# datatypes/extern_c_api.h

 [More...](#detailed-description)

## Functions

|                | Name           |
| -------------- | -------------- |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) char * | **[GetLastStdExceptionMessage](/cpp/Files/extern__c__api_8h/#function-getlaststdexceptionmessage)**()<br>Gets the last message from an std::exception caught by the uchronia API.  |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) void | **[RegisterExceptionCallback](/cpp/Files/extern__c__api_8h/#function-registerexceptioncallback)**(const void * callback) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) void | **[DisposeSharedPointer](/cpp/Files/extern__c__api_8h/#function-disposesharedpointer)**(VOID_PTR_PROVIDER_PTR ptr)<br>Notifies uchronia that an object managed by an opaque pointer is not used by the caller anymore.  |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) void | **[DeleteAnsiStringArray](/cpp/Files/extern__c__api_8h/#function-deleteansistringarray)**(char ** values, int arrayLength)<br>Deletes the ANSI string array , which has been create by uchronia. Do not use for char** created outside libswift.  |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) void | **[DeleteAnsiString](/cpp/Files/extern__c__api_8h/#function-deleteansistring)**(const char * value)<br>Deletes the ANSI string which has been create by uchronia. Do not use for char* created outside libswift.  |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) void | **[DeleteDoubleArray](/cpp/Files/extern__c__api_8h/#function-deletedoublearray)**(double * value)<br>Dispose of an array of double created via this C API.  |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) void | **[SetTimeSeriesMissingValueValue](/cpp/Files/extern__c__api_8h/#function-settimeseriesmissingvaluevalue)**(double missingValueValue)<br>Sets a value whoch should be considered as a missing value when data is passed to this C API.  |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api)[ENSEMBLE_DATA_SET_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr) | **[LoadEnsembleDataset](/cpp/Files/extern__c__api_8h/#function-loadensembledataset)**(const char * libraryIdentifier, const char * dataPath)<br>Creates a time series library, defined (for now) by a YAML descriptor.  |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api)[ENSEMBLE_DATA_SET_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr) | **[CreateEnsembleDataset](/cpp/Files/extern__c__api_8h/#function-createensembledataset)**(const char * type)<br>Creates a time series library.  |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) char ** | **[GetEnsembleDatasetDataIdentifiers](/cpp/Files/extern__c__api_8h/#function-getensembledatasetdataidentifiers)**([ENSEMBLE_DATA_SET_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr) dataLibrary, int * size)<br>Gets the highest level datasets' IDs known to this library.  |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) char ** | **[GetEnsembleDatasetDataSubIdentifiers](/cpp/Files/extern__c__api_8h/#function-getensembledatasetdatasubidentifiers)**([ENSEMBLE_DATA_SET_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr) dataLibrary, const char * dataCollectionId, int * size)<br>Gets sub identifiers, if any, in a hierarchical ID scheme (e.g. if a collection of streamflows is such that you can ID each series as "streamflow.gauge_id")  |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) char ** | **[GetEnsembleDatasetDataSummaries](/cpp/Files/extern__c__api_8h/#function-getensembledatasetdatasummaries)**([ENSEMBLE_DATA_SET_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr) dataLibrary, int * size) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) time_series_dimensions_description * | **[GetDataDimensionsDescription](/cpp/Files/extern__c__api_8h/#function-getdatadimensionsdescription)**([ENSEMBLE_DATA_SET_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr) dataLibrary, const char * dataId)<br>Gets data dimensions description. This function is useful for wrappers to discover the dimensionality of a data set before trying to load it in memory.  |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) int | **[EnsembleSizeEnsembleTimeSeries](/cpp/Files/extern__c__api_8h/#function-ensemblesizeensembletimeseries)**([ENSEMBLE_PTR_TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-ptr-time-series-ptr) ensSeries) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) void | **[DisposeDataDimensionsDescriptions](/cpp/Files/extern__c__api_8h/#function-disposedatadimensionsdescriptions)**(time_series_dimensions_description * data) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api)[ENSEMBLE_FORECAST_TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) | **[CreateEnsembleForecastTimeSeries](/cpp/Files/extern__c__api_8h/#function-createensembleforecasttimeseries)**(date_time_to_second start, int length, const char * timeStepName) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api)[TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) | **[GetDatasetSingleTimeSeries](/cpp/Files/extern__c__api_8h/#function-getdatasetsingletimeseries)**([ENSEMBLE_DATA_SET_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr) dataLibrary, const char * dataId) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api)[ENSEMBLE_PTR_TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-ptr-time-series-ptr) | **[GetDatasetEnsembleTimeSeries](/cpp/Files/extern__c__api_8h/#function-getdatasetensembletimeseries)**([ENSEMBLE_DATA_SET_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr) dataLibrary, const char * dataEnsembleId) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api)[ENSEMBLE_FORECAST_TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) | **[GetDatasetEnsembleForecastTimeSeries](/cpp/Files/extern__c__api_8h/#function-getdatasetensembleforecasttimeseries)**([ENSEMBLE_DATA_SET_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr) dataLibrary, const char * dataId) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) void | **[SaveSingleTimeSeriesToNetcdf](/cpp/Files/extern__c__api_8h/#function-savesingletimeseriestonetcdf)**([TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) timeSeries, const char * filename, bool overwrite) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) void | **[SaveEnsembleTimeSeriesToNetcdf](/cpp/Files/extern__c__api_8h/#function-saveensembletimeseriestonetcdf)**([ENSEMBLE_PTR_TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-ptr-time-series-ptr) collection, const char * filename, bool overwrite) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) void | **[SaveEnsembleForecastTimeSeriesToNetcdf](/cpp/Files/extern__c__api_8h/#function-saveensembleforecasttimeseriestonetcdf)**([ENSEMBLE_FORECAST_TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) tsEnsTs, const char * filename, bool overwrite) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) bool | **[IsMissingValueItemEnsembleForecastTimeSeries](/cpp/Files/extern__c__api_8h/#function-ismissingvalueitemensembleforecasttimeseries)**([ENSEMBLE_FORECAST_TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) series, int i) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api)[ENSEMBLE_PTR_TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-ptr-time-series-ptr) | **[GetItemEnsembleForecastTimeSeries](/cpp/Files/extern__c__api_8h/#function-getitemensembleforecasttimeseries)**([ENSEMBLE_FORECAST_TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) efts, int i) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api)[TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) | **[TimeSeriesFromEnsembleOfTimeSeries](/cpp/Files/extern__c__api_8h/#function-timeseriesfromensembleoftimeseries)**([ENSEMBLE_PTR_TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-ptr-time-series-ptr) collectionTs, int index) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api)[TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) | **[TimeSeriesFromTimeSeriesOfEnsembleOfTimeSeries](/cpp/Files/extern__c__api_8h/#function-timeseriesfromtimeseriesofensembleoftimeseries)**([ENSEMBLE_FORECAST_TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) efts, int indexInIssueTime, int indexInForecastTime) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) double | **[GetValueFromUnivariateTimeSeries](/cpp/Files/extern__c__api_8h/#function-getvaluefromunivariatetimeseries)**([TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) ts, int index) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) void | **[TransformEachItem](/cpp/Files/extern__c__api_8h/#function-transformeachitem)**([ENSEMBLE_FORECAST_TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) tsEnsTs, const char * method, const char * methodArgument) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) void | **[SetValueToUnivariateTimeSeries](/cpp/Files/extern__c__api_8h/#function-setvaluetounivariatetimeseries)**([TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) ts, int index, double value) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) multi_regular_time_series_data * | **[GetItemEnsembleForecastTimeSeriesAsStructure](/cpp/Files/extern__c__api_8h/#function-getitemensembleforecasttimeseriesasstructure)**([ENSEMBLE_FORECAST_TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) series, int i) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) multi_regular_time_series_data * | **[GetItemEnsembleTimeSeriesAsStructure](/cpp/Files/extern__c__api_8h/#function-getitemensembletimeseriesasstructure)**([ENSEMBLE_PTR_TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-ptr-time-series-ptr) series, int i) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) void | **[SetItemEnsembleForecastTimeSeriesAsStructure](/cpp/Files/extern__c__api_8h/#function-setitemensembleforecasttimeseriesasstructure)**([ENSEMBLE_FORECAST_TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) series, int i, const multi_regular_time_series_data * values) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) void | **[SetItemEnsembleTimeSeriesAsStructure](/cpp/Files/extern__c__api_8h/#function-setitemensembletimeseriesasstructure)**([ENSEMBLE_PTR_TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-ptr-time-series-ptr) collection, int i, const multi_regular_time_series_data * values) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api)[ENSEMBLE_FORECAST_TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) | **[CreatePerfectForecastTimeSeries](/cpp/Files/extern__c__api_8h/#function-createperfectforecasttimeseries)**([TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) observations, date_time_to_second start, int length, const char * timeStepName, int offsetForecasts, int leadTime) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) multi_regular_time_series_data * | **[ToStructEnsembleTimeSeriesData](/cpp/Files/extern__c__api_8h/#function-tostructensembletimeseriesdata)**([ENSEMBLE_PTR_TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-ptr-time-series-ptr) ensSeries) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) multi_regular_time_series_data * | **[ToStructSingleTimeSeriesData](/cpp/Files/extern__c__api_8h/#function-tostructsingletimeseriesdata)**([TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) timeSeries) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api)[ENSEMBLE_PTR_TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-ptr-time-series-ptr) | **[CreateEnsembleTimeSeriesDataFromStruct](/cpp/Files/extern__c__api_8h/#function-createensembletimeseriesdatafromstruct)**(const multi_regular_time_series_data * ensSeries) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api)[TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) | **[CreateSingleTimeSeriesDataFromStruct](/cpp/Files/extern__c__api_8h/#function-createsingletimeseriesdatafromstruct)**(const multi_regular_time_series_data * timeSeries) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) void | **[DisposeMultiTimeSeriesData](/cpp/Files/extern__c__api_8h/#function-disposemultitimeseriesdata)**(multi_regular_time_series_data * data) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) void | **[GetTimeSeriesGeometry](/cpp/Files/extern__c__api_8h/#function-gettimeseriesgeometry)**([TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) timeSeries, [TS_GEOMETRY_PTR](/cpp/Files/extern__c__api__transparent__pointers_8h/#define-ts-geometry-ptr) geom) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) void | **[GetEnsembleForecastTimeSeriesGeometry](/cpp/Files/extern__c__api_8h/#function-getensembleforecasttimeseriesgeometry)**([ENSEMBLE_FORECAST_TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) timeSeries, [TS_GEOMETRY_PTR](/cpp/Files/extern__c__api__transparent__pointers_8h/#define-ts-geometry-ptr) geom) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) void | **[GetTimeSeriesValues](/cpp/Files/extern__c__api_8h/#function-gettimeseriesvalues)**([TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) timeSeries, double * values, int arrayLength) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) int | **[GetNumTimeSeries](/cpp/Files/extern__c__api_8h/#function-getnumtimeseries)**() |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) void | **[GetProviderTsGeometry](/cpp/Files/extern__c__api_8h/#function-getprovidertsgeometry)**([TIME_SERIES_PROVIDER_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-provider-ptr) dataLibrary, const char * variableIdentifier, [TS_GEOMETRY_PTR](/cpp/Files/extern__c__api__transparent__pointers_8h/#define-ts-geometry-ptr) geom) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) void | **[GetProviderTimeSeriesValues](/cpp/Files/extern__c__api_8h/#function-getprovidertimeseriesvalues)**([TIME_SERIES_PROVIDER_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-provider-ptr) dataLibrary, const char * variableIdentifier, double * values, int arrayLength) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api) char ** | **[GetProviderTimeSeriesIdentifiers](/cpp/Files/extern__c__api_8h/#function-getprovidertimeseriesidentifiers)**([TIME_SERIES_PROVIDER_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-provider-ptr) dataLibrary, int * size) |
| [DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api)[TIME_SERIES_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) | **[TimeSeriesFromProviderTs](/cpp/Files/extern__c__api_8h/#function-timeseriesfromproviderts)**([TIME_SERIES_PROVIDER_PTR](/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-provider-ptr) dataLibrary, const char * variableIdentifier) |

## Defines

|                | Name           |
| -------------- | -------------- |
|  | **[DATATYPES_USE_CPP_POINTERS](/cpp/Files/extern__c__api_8h/#define-datatypes-use-cpp-pointers)**  |
|  | **[DATATYPES_API](/cpp/Files/extern__c__api_8h/#define-datatypes-api)**  |

## Detailed Description


API for libswift. This file exposes a common API for interacting with libswift from other tools. 


## Functions Documentation

### function GetLastStdExceptionMessage

```cpp
DATATYPES_API char * GetLastStdExceptionMessage()
```

Gets the last message from an std::exception caught by the uchronia API. 

**Return**: the last standard exception message. 

### function RegisterExceptionCallback

```cpp
DATATYPES_API void RegisterExceptionCallback(
    const void * callback
)
```


### function DisposeSharedPointer

```cpp
DATATYPES_API void DisposeSharedPointer(
    VOID_PTR_PROVIDER_PTR ptr
)
```

Notifies uchronia that an object managed by an opaque pointer is not used by the caller anymore. 

**Parameters**: 

  * **ptr** pointer obtained via the API, such as a MODEL_SIMULATION_PTR. 


### function DeleteAnsiStringArray

```cpp
DATATYPES_API void DeleteAnsiStringArray(
    char ** values,
    int arrayLength
)
```

Deletes the ANSI string array , which has been create by uchronia. Do not use for char** created outside libswift. 

**Parameters**: 

  * **values** pointer to the array to delete (its elements and the array itself). 
  * **arrayLength** Length of the array. 


### function DeleteAnsiString

```cpp
DATATYPES_API void DeleteAnsiString(
    const char * value
)
```

Deletes the ANSI string which has been create by uchronia. Do not use for char* created outside libswift. 

**Parameters**: 

  * **value** a C-style string, which has been create by uchronia. Do not use for char* created elsewhere. 


### function DeleteDoubleArray

```cpp
DATATYPES_API void DeleteDoubleArray(
    double * value
)
```

Dispose of an array of double created via this C API. 

**Parameters**: 

  * **value** If non-null, the value. 


### function SetTimeSeriesMissingValueValue

```cpp
DATATYPES_API void SetTimeSeriesMissingValueValue(
    double missingValueValue
)
```

Sets a value whoch should be considered as a missing value when data is passed to this C API. 

**Parameters**: 

  * **missingValueValue** The missing value. 


### function LoadEnsembleDataset

```cpp
DATATYPES_APIENSEMBLE_DATA_SET_PTR LoadEnsembleDataset(
    const char * libraryIdentifier,
    const char * dataPath
)
```

Creates a time series library, defined (for now) by a YAML descriptor. 

**Parameters**: 

  * **libraryIdentifier** an ID for the library (currently path to a YAML file) 
  * **dataPath** optional root data path for on-disk data, if the YAML file uses relative paths.


**Return**: The ensemble dataset. 

### function CreateEnsembleDataset

```cpp
DATATYPES_APIENSEMBLE_DATA_SET_PTR CreateEnsembleDataset(
    const char * type
)
```

Creates a time series library. 

**Parameters**: 

  * **type** The type of library to create. Currently supports cases for unit tests and time series libraries that can be "recorded to" by modelling engines.


**Return**: The new ensemble dataset. 

### function GetEnsembleDatasetDataIdentifiers

```cpp
DATATYPES_API char ** GetEnsembleDatasetDataIdentifiers(
    ENSEMBLE_DATA_SET_PTR dataLibrary,
    int * size
)
```

Gets the highest level datasets' IDs known to this library. 

**Parameters**: 

  * **dataLibrary** The data library. 
  * **size** Size of the list of IDs


**Return**: Null if it fails, else the ensemble dataset data identifiers. 

### function GetEnsembleDatasetDataSubIdentifiers

```cpp
DATATYPES_API char ** GetEnsembleDatasetDataSubIdentifiers(
    ENSEMBLE_DATA_SET_PTR dataLibrary,
    const char * dataCollectionId,
    int * size
)
```

Gets sub identifiers, if any, in a hierarchical ID scheme (e.g. if a collection of streamflows is such that you can ID each series as "streamflow.gauge_id") 

**Parameters**: 

  * **dataLibrary** The data library. 
  * **dataCollectionId** Main identifier within which to query for sub-identifgiers 
  * **size** Size of the list of sub-IDs


**Return**: Null if it fails, else the dataset data sub identifiers. (e.g. the streamflow gauge idenfiers) 

### function GetEnsembleDatasetDataSummaries

```cpp
DATATYPES_API char ** GetEnsembleDatasetDataSummaries(
    ENSEMBLE_DATA_SET_PTR dataLibrary,
    int * size
)
```


### function GetDataDimensionsDescription

```cpp
DATATYPES_API time_series_dimensions_description * GetDataDimensionsDescription(
    ENSEMBLE_DATA_SET_PTR dataLibrary,
    const char * dataId
)
```

Gets data dimensions description. This function is useful for wrappers to discover the dimensionality of a data set before trying to load it in memory. 

**Parameters**: 

  * **dataLibrary** The data library. 
  * **dataId** Identifier for the data.


**Return**: A struct describing the dimensionality of the data set in the library. 

### function EnsembleSizeEnsembleTimeSeries

```cpp
DATATYPES_API int EnsembleSizeEnsembleTimeSeries(
    ENSEMBLE_PTR_TIME_SERIES_PTR ensSeries
)
```


### function DisposeDataDimensionsDescriptions

```cpp
DATATYPES_API void DisposeDataDimensionsDescriptions(
    time_series_dimensions_description * data
)
```


### function CreateEnsembleForecastTimeSeries

```cpp
DATATYPES_APIENSEMBLE_FORECAST_TIME_SERIES_PTR CreateEnsembleForecastTimeSeries(
    date_time_to_second start,
    int length,
    const char * timeStepName
)
```


### function GetDatasetSingleTimeSeries

```cpp
DATATYPES_APITIME_SERIES_PTR GetDatasetSingleTimeSeries(
    ENSEMBLE_DATA_SET_PTR dataLibrary,
    const char * dataId
)
```


### function GetDatasetEnsembleTimeSeries

```cpp
DATATYPES_APIENSEMBLE_PTR_TIME_SERIES_PTR GetDatasetEnsembleTimeSeries(
    ENSEMBLE_DATA_SET_PTR dataLibrary,
    const char * dataEnsembleId
)
```


### function GetDatasetEnsembleForecastTimeSeries

```cpp
DATATYPES_APIENSEMBLE_FORECAST_TIME_SERIES_PTR GetDatasetEnsembleForecastTimeSeries(
    ENSEMBLE_DATA_SET_PTR dataLibrary,
    const char * dataId
)
```


### function SaveSingleTimeSeriesToNetcdf

```cpp
DATATYPES_API void SaveSingleTimeSeriesToNetcdf(
    TIME_SERIES_PTR timeSeries,
    const char * filename,
    bool overwrite
)
```


### function SaveEnsembleTimeSeriesToNetcdf

```cpp
DATATYPES_API void SaveEnsembleTimeSeriesToNetcdf(
    ENSEMBLE_PTR_TIME_SERIES_PTR collection,
    const char * filename,
    bool overwrite
)
```


### function SaveEnsembleForecastTimeSeriesToNetcdf

```cpp
DATATYPES_API void SaveEnsembleForecastTimeSeriesToNetcdf(
    ENSEMBLE_FORECAST_TIME_SERIES_PTR tsEnsTs,
    const char * filename,
    bool overwrite
)
```


### function IsMissingValueItemEnsembleForecastTimeSeries

```cpp
DATATYPES_API bool IsMissingValueItemEnsembleForecastTimeSeries(
    ENSEMBLE_FORECAST_TIME_SERIES_PTR series,
    int i
)
```


### function GetItemEnsembleForecastTimeSeries

```cpp
DATATYPES_APIENSEMBLE_PTR_TIME_SERIES_PTR GetItemEnsembleForecastTimeSeries(
    ENSEMBLE_FORECAST_TIME_SERIES_PTR efts,
    int i
)
```


### function TimeSeriesFromEnsembleOfTimeSeries

```cpp
DATATYPES_APITIME_SERIES_PTR TimeSeriesFromEnsembleOfTimeSeries(
    ENSEMBLE_PTR_TIME_SERIES_PTR collectionTs,
    int index
)
```


### function TimeSeriesFromTimeSeriesOfEnsembleOfTimeSeries

```cpp
DATATYPES_APITIME_SERIES_PTR TimeSeriesFromTimeSeriesOfEnsembleOfTimeSeries(
    ENSEMBLE_FORECAST_TIME_SERIES_PTR efts,
    int indexInIssueTime,
    int indexInForecastTime
)
```


### function GetValueFromUnivariateTimeSeries

```cpp
DATATYPES_API double GetValueFromUnivariateTimeSeries(
    TIME_SERIES_PTR ts,
    int index
)
```


### function TransformEachItem

```cpp
DATATYPES_API void TransformEachItem(
    ENSEMBLE_FORECAST_TIME_SERIES_PTR tsEnsTs,
    const char * method,
    const char * methodArgument
)
```


### function SetValueToUnivariateTimeSeries

```cpp
DATATYPES_API void SetValueToUnivariateTimeSeries(
    TIME_SERIES_PTR ts,
    int index,
    double value
)
```


### function GetItemEnsembleForecastTimeSeriesAsStructure

```cpp
DATATYPES_API multi_regular_time_series_data * GetItemEnsembleForecastTimeSeriesAsStructure(
    ENSEMBLE_FORECAST_TIME_SERIES_PTR series,
    int i
)
```


### function GetItemEnsembleTimeSeriesAsStructure

```cpp
DATATYPES_API multi_regular_time_series_data * GetItemEnsembleTimeSeriesAsStructure(
    ENSEMBLE_PTR_TIME_SERIES_PTR series,
    int i
)
```


### function SetItemEnsembleForecastTimeSeriesAsStructure

```cpp
DATATYPES_API void SetItemEnsembleForecastTimeSeriesAsStructure(
    ENSEMBLE_FORECAST_TIME_SERIES_PTR series,
    int i,
    const multi_regular_time_series_data * values
)
```


### function SetItemEnsembleTimeSeriesAsStructure

```cpp
DATATYPES_API void SetItemEnsembleTimeSeriesAsStructure(
    ENSEMBLE_PTR_TIME_SERIES_PTR collection,
    int i,
    const multi_regular_time_series_data * values
)
```


### function CreatePerfectForecastTimeSeries

```cpp
DATATYPES_APIENSEMBLE_FORECAST_TIME_SERIES_PTR CreatePerfectForecastTimeSeries(
    TIME_SERIES_PTR observations,
    date_time_to_second start,
    int length,
    const char * timeStepName,
    int offsetForecasts,
    int leadTime
)
```


### function ToStructEnsembleTimeSeriesData

```cpp
DATATYPES_API multi_regular_time_series_data * ToStructEnsembleTimeSeriesData(
    ENSEMBLE_PTR_TIME_SERIES_PTR ensSeries
)
```


### function ToStructSingleTimeSeriesData

```cpp
DATATYPES_API multi_regular_time_series_data * ToStructSingleTimeSeriesData(
    TIME_SERIES_PTR timeSeries
)
```


### function CreateEnsembleTimeSeriesDataFromStruct

```cpp
DATATYPES_APIENSEMBLE_PTR_TIME_SERIES_PTR CreateEnsembleTimeSeriesDataFromStruct(
    const multi_regular_time_series_data * ensSeries
)
```


### function CreateSingleTimeSeriesDataFromStruct

```cpp
DATATYPES_APITIME_SERIES_PTR CreateSingleTimeSeriesDataFromStruct(
    const multi_regular_time_series_data * timeSeries
)
```


### function DisposeMultiTimeSeriesData

```cpp
DATATYPES_API void DisposeMultiTimeSeriesData(
    multi_regular_time_series_data * data
)
```


### function GetTimeSeriesGeometry

```cpp
DATATYPES_API void GetTimeSeriesGeometry(
    TIME_SERIES_PTR timeSeries,
    TS_GEOMETRY_PTR geom
)
```


### function GetEnsembleForecastTimeSeriesGeometry

```cpp
DATATYPES_API void GetEnsembleForecastTimeSeriesGeometry(
    ENSEMBLE_FORECAST_TIME_SERIES_PTR timeSeries,
    TS_GEOMETRY_PTR geom
)
```


### function GetTimeSeriesValues

```cpp
DATATYPES_API void GetTimeSeriesValues(
    TIME_SERIES_PTR timeSeries,
    double * values,
    int arrayLength
)
```


### function GetNumTimeSeries

```cpp
DATATYPES_API int GetNumTimeSeries()
```


### function GetProviderTsGeometry

```cpp
DATATYPES_API void GetProviderTsGeometry(
    TIME_SERIES_PROVIDER_PTR dataLibrary,
    const char * variableIdentifier,
    TS_GEOMETRY_PTR geom
)
```


### function GetProviderTimeSeriesValues

```cpp
DATATYPES_API void GetProviderTimeSeriesValues(
    TIME_SERIES_PROVIDER_PTR dataLibrary,
    const char * variableIdentifier,
    double * values,
    int arrayLength
)
```


### function GetProviderTimeSeriesIdentifiers

```cpp
DATATYPES_API char ** GetProviderTimeSeriesIdentifiers(
    TIME_SERIES_PROVIDER_PTR dataLibrary,
    int * size
)
```


### function TimeSeriesFromProviderTs

```cpp
DATATYPES_APITIME_SERIES_PTR TimeSeriesFromProviderTs(
    TIME_SERIES_PROVIDER_PTR dataLibrary,
    const char * variableIdentifier
)
```




## Macros Documentation

### define DATATYPES_USE_CPP_POINTERS

```cpp
#define DATATYPES_USE_CPP_POINTERS 
```


### define DATATYPES_API

```cpp
#define DATATYPES_API DATATYPES_DLL_LIB
```


## Source code

```cpp

#pragma once

#include "setup_exports.h"

#ifndef DATATYPES_USE_OPAQUE_POINTERS
#ifndef DATATYPES_USE_CPP_POINTERS
#ifndef USING_DATATYPES_CORE
#define DATATYPES_USE_CPP_POINTERS
#endif
#endif
#endif

#include "interop_struct.h"

#if defined(DATATYPES_USE_CPP_POINTERS)

#include "datatypes/extern_c_api_as_transparent.h"

#elif defined(DATATYPES_USE_OPAQUE_POINTERS)

#include "datatypes/extern_c_api_as_opaque.h"

#else
#error macro DATATYPES_USE_OPAQUE_POINTERS or DATATYPES_USE_CPP_POINTERS must be defined
#endif

// see http://msdn.microsoft.com/en-us/library/as6wyhwt.aspx, best practice
#define DATATYPES_API  DATATYPES_DLL_LIB 

#ifdef __cplusplus
extern "C" {
#endif

    // Error handling

    DATATYPES_API char* GetLastStdExceptionMessage();

    DATATYPES_API void RegisterExceptionCallback(const void* callback);

    // Generic memory management.

    DATATYPES_API void DisposeSharedPointer(VOID_PTR_PROVIDER_PTR ptr);

    DATATYPES_API void DeleteAnsiStringArray(char** values, int arrayLength);

    DATATYPES_API void DeleteAnsiString(const char* value);

    DATATYPES_API void DeleteDoubleArray(double* value);


    // Global settings for the C uchronia API


    DATATYPES_API void SetTimeSeriesMissingValueValue(double missingValueValue);

    DATATYPES_API ENSEMBLE_DATA_SET_PTR LoadEnsembleDataset(const char* libraryIdentifier, const char* dataPath);

    DATATYPES_API ENSEMBLE_DATA_SET_PTR CreateEnsembleDataset(const char* type);

    DATATYPES_API char** GetEnsembleDatasetDataIdentifiers(ENSEMBLE_DATA_SET_PTR dataLibrary, int* size);

    DATATYPES_API char** GetEnsembleDatasetDataSubIdentifiers(ENSEMBLE_DATA_SET_PTR dataLibrary, const char* dataCollectionId, int* size);

    DATATYPES_API char** GetEnsembleDatasetDataSummaries(ENSEMBLE_DATA_SET_PTR dataLibrary, int* size);

    DATATYPES_API time_series_dimensions_description* GetDataDimensionsDescription(ENSEMBLE_DATA_SET_PTR dataLibrary, const char* dataId);

    DATATYPES_API int EnsembleSizeEnsembleTimeSeries(ENSEMBLE_PTR_TIME_SERIES_PTR ensSeries);

    DATATYPES_API void DisposeDataDimensionsDescriptions(time_series_dimensions_description* data);

    DATATYPES_API ENSEMBLE_FORECAST_TIME_SERIES_PTR CreateEnsembleForecastTimeSeries(date_time_to_second start, int length, const char* timeStepName);



    DATATYPES_API TIME_SERIES_PTR GetDatasetSingleTimeSeries(ENSEMBLE_DATA_SET_PTR dataLibrary, const char* dataId);
    DATATYPES_API ENSEMBLE_PTR_TIME_SERIES_PTR GetDatasetEnsembleTimeSeries(ENSEMBLE_DATA_SET_PTR dataLibrary, const char* dataEnsembleId);
    // DATATYPES_API FORECAST_TIME_SERIES_DOUBLE_PTR GetDatasetForecastTimeSeries(ENSEMBLE_DATA_SET_PTR dataLibrary, char** identifiers, char** dataId, int size);
    DATATYPES_API ENSEMBLE_FORECAST_TIME_SERIES_PTR GetDatasetEnsembleForecastTimeSeries(ENSEMBLE_DATA_SET_PTR dataLibrary, const char* dataId);

    // These api entry points are TEMPORARY: they must be phased out.
    DATATYPES_API void SaveSingleTimeSeriesToNetcdf(TIME_SERIES_PTR timeSeries, const char* filename, bool overwrite);
    DATATYPES_API void SaveEnsembleTimeSeriesToNetcdf(ENSEMBLE_PTR_TIME_SERIES_PTR collection, const char* filename, bool overwrite);
    DATATYPES_API void SaveEnsembleForecastTimeSeriesToNetcdf(ENSEMBLE_FORECAST_TIME_SERIES_PTR tsEnsTs, const char* filename, bool overwrite);

    DATATYPES_API bool IsMissingValueItemEnsembleForecastTimeSeries(ENSEMBLE_FORECAST_TIME_SERIES_PTR series, int i);

    //Functions that reduce the dimensionality of data, forms of splicing
    DATATYPES_API ENSEMBLE_PTR_TIME_SERIES_PTR GetItemEnsembleForecastTimeSeries(ENSEMBLE_FORECAST_TIME_SERIES_PTR efts, int i);
    DATATYPES_API TIME_SERIES_PTR TimeSeriesFromEnsembleOfTimeSeries(ENSEMBLE_PTR_TIME_SERIES_PTR collectionTs, int index);
    DATATYPES_API TIME_SERIES_PTR TimeSeriesFromTimeSeriesOfEnsembleOfTimeSeries(ENSEMBLE_FORECAST_TIME_SERIES_PTR efts, int indexInIssueTime, int indexInForecastTime );
    DATATYPES_API double GetValueFromUnivariateTimeSeries(TIME_SERIES_PTR ts, int index);

    DATATYPES_API void TransformEachItem(ENSEMBLE_FORECAST_TIME_SERIES_PTR tsEnsTs, const char* method, const char* methodArgument);

    //Functions that set items in data (along the 'first' dimension)
    DATATYPES_API void SetValueToUnivariateTimeSeries(TIME_SERIES_PTR ts, int index, double value);


    // Handling elements in ensemble time series forecasts.
    
    DATATYPES_API multi_regular_time_series_data* GetItemEnsembleForecastTimeSeriesAsStructure(ENSEMBLE_FORECAST_TIME_SERIES_PTR series, int i);
    DATATYPES_API multi_regular_time_series_data* GetItemEnsembleTimeSeriesAsStructure(ENSEMBLE_PTR_TIME_SERIES_PTR series, int i);
    //DATATYPES_API void SetItemEnsembleForecastTimeSeries(ENSEMBLE_FORECAST_TIME_SERIES_PTR series, int i, ENSEMBLE_FORECAST_TIME_SERIES_PTR data);
    DATATYPES_API void SetItemEnsembleForecastTimeSeriesAsStructure(ENSEMBLE_FORECAST_TIME_SERIES_PTR series, int i, const multi_regular_time_series_data*  values);
    DATATYPES_API void SetItemEnsembleTimeSeriesAsStructure(ENSEMBLE_PTR_TIME_SERIES_PTR collection, int i, const multi_regular_time_series_data*  values);

    // Functions that augment the dimensionality of data
    DATATYPES_API ENSEMBLE_FORECAST_TIME_SERIES_PTR CreatePerfectForecastTimeSeries(TIME_SERIES_PTR observations, date_time_to_second start, int length, const char* timeStepName, int offsetForecasts, int leadTime);

    // conversions to structures for conversions to other representations in the language using this C API
    DATATYPES_API multi_regular_time_series_data* ToStructEnsembleTimeSeriesData(ENSEMBLE_PTR_TIME_SERIES_PTR ensSeries);
    DATATYPES_API multi_regular_time_series_data* ToStructSingleTimeSeriesData(TIME_SERIES_PTR timeSeries);
    DATATYPES_API ENSEMBLE_PTR_TIME_SERIES_PTR CreateEnsembleTimeSeriesDataFromStruct(const multi_regular_time_series_data* ensSeries);
    DATATYPES_API TIME_SERIES_PTR CreateSingleTimeSeriesDataFromStruct(const multi_regular_time_series_data* timeSeries);
    DATATYPES_API void DisposeMultiTimeSeriesData(multi_regular_time_series_data* data);

    DATATYPES_API void GetTimeSeriesGeometry(TIME_SERIES_PTR timeSeries, TS_GEOMETRY_PTR geom);
    DATATYPES_API void GetEnsembleForecastTimeSeriesGeometry(ENSEMBLE_FORECAST_TIME_SERIES_PTR timeSeries, TS_GEOMETRY_PTR geom);
    DATATYPES_API void GetTimeSeriesValues(TIME_SERIES_PTR timeSeries, double * values, int arrayLength);
    DATATYPES_API int GetNumTimeSeries();
    // Backward compatibility with SWIFTv1, but functions that may be generic to other persistent data sources

    DATATYPES_API void GetProviderTsGeometry(TIME_SERIES_PROVIDER_PTR dataLibrary, const char* variableIdentifier, TS_GEOMETRY_PTR geom);
    DATATYPES_API void GetProviderTimeSeriesValues(TIME_SERIES_PROVIDER_PTR dataLibrary, const char* variableIdentifier, double * values, int arrayLength);
    DATATYPES_API char** GetProviderTimeSeriesIdentifiers(TIME_SERIES_PROVIDER_PTR dataLibrary, int* size);
    DATATYPES_API TIME_SERIES_PTR TimeSeriesFromProviderTs(TIME_SERIES_PROVIDER_PTR dataLibrary, const char* variableIdentifier);


    // Obsolete and deprecated functions

#ifdef __cplusplus
}
#endif
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000
