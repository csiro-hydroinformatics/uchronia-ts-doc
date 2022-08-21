---
title: datatypes/extern_c_api.h

---

# datatypes/extern_c_api.h

 [More...](#detailed-description)

## Functions

|                | Name           |
| -------------- | -------------- |
| char * | **[GetLastStdExceptionMessage](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-getlaststdexceptionmessage)**()<br>Gets the last message from an std::exception caught by the uchronia API.  |
| void | **[RegisterExceptionCallback](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-registerexceptioncallback)**(const void * callback)<br>Registers a function to call when uchronia has generated a std::exception that has been caught by the API.  |
| void | **[DisposeSharedPointer](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-disposesharedpointer)**(VOID_PTR_PROVIDER_PTR ptr)<br>Notifies uchronia that an object managed by an opaque pointer is not used by the caller anymore.  |
| void | **[DeleteAnsiStringArray](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-deleteansistringarray)**(char ** values, int arrayLength)<br>Deletes the ANSI string array , which has been create by uchronia. Do not use for char** created outside uchronia.  |
| void | **[DeleteAnsiString](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-deleteansistring)**(const char * value)<br>Deletes the ANSI string which has been create by uchronia. Do not use for char* created outside uchronia.  |
| void | **[DeleteDoubleArray](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-deletedoublearray)**(double * value)<br>Dispose of an array of double created via this C API.  |
| void | **[SetTimeSeriesMissingValueValue](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-settimeseriesmissingvaluevalue)**(double missingValueValue)<br>Sets a value whoch should be considered as a missing value when data is passed to this C API.  |
| [ENSEMBLE_DATA_SET_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr) | **[LoadEnsembleDataset](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-loadensembledataset)**(const char * libraryIdentifier, const char * dataPath)<br>Creates a time series library, defined (for now) by a YAML descriptor.  |
| [ENSEMBLE_DATA_SET_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr) | **[CreateEnsembleDataset](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-createensembledataset)**(const char * type)<br>Creates a time series library.  |
| char ** | **[GetEnsembleDatasetDataIdentifiers](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-getensembledatasetdataidentifiers)**([ENSEMBLE_DATA_SET_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr) dataLibrary, int * size)<br>Gets the highest level datasets' IDs known to this library.  |
| char ** | **[GetEnsembleDatasetDataSubIdentifiers](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-getensembledatasetdatasubidentifiers)**([ENSEMBLE_DATA_SET_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr) dataLibrary, const char * dataCollectionId, int * size)<br>Gets sub identifiers, if any, in a hierarchical ID scheme (e.g. if a collection of streamflows is such that you can ID each series as "streamflow.gauge_id")  |
| char ** | **[GetEnsembleDatasetDataSummaries](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-getensembledatasetdatasummaries)**([ENSEMBLE_DATA_SET_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr) dataLibrary, int * size)<br>Get brief summary descriptions of each dataset in a data library.  |
| time_series_dimensions_description * | **[GetDataDimensionsDescription](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-getdatadimensionsdescription)**([ENSEMBLE_DATA_SET_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr) dataLibrary, const char * dataId)<br>Gets data dimensions description. This function is useful for wrappers to discover the dimensionality of a data set before trying to load it in memory.  |
| int | **[EnsembleSizeEnsembleTimeSeries](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-ensemblesizeensembletimeseries)**([ENSEMBLE_PTR_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-ptr-time-series-ptr) ensSeries)<br>Gets the number of ensembles in an ensemble time series.  |
| void | **[DisposeDataDimensionsDescriptions](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-disposedatadimensionsdescriptions)**(time_series_dimensions_description * data)<br>Dispose of a time_series_dimensions_description previously returned by this API.  |
| [ENSEMBLE_FORECAST_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) | **[CreateEnsembleForecastTimeSeries](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-createensembleforecasttimeseries)**(date_time_to_second start, int length, const char * timeStepName)<br>Create a Ensemble Forecast Time Series object. This is a time series of ensembles of time series. The conceptual dimensions are time (forecast issue time), ensemble, and forecast lead time.  |
| [TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) | **[GetDatasetSingleTimeSeries](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-getdatasetsingletimeseries)**([ENSEMBLE_DATA_SET_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr) dataLibrary, const char * dataId)<br>Gets a univariate Time Series out of a data library.  |
| [ENSEMBLE_PTR_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-ptr-time-series-ptr) | **[GetDatasetEnsembleTimeSeries](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-getdatasetensembletimeseries)**([ENSEMBLE_DATA_SET_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr) dataLibrary, const char * dataEnsembleId)<br>Gets a multivariate (ensemble) Time Series out of a data library.  |
| [ENSEMBLE_FORECAST_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) | **[GetDatasetEnsembleForecastTimeSeries](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-getdatasetensembleforecasttimeseries)**([ENSEMBLE_DATA_SET_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr) dataLibrary, const char * dataId)<br>Gets an ensemble forecast time serie (time series of ensemble time series ) out of a data library.  |
| void | **[SaveSingleTimeSeriesToNetcdf](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-savesingletimeseriestonetcdf)**([TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) timeSeries, const char * filename, bool overwrite)<br>Save a time series to a netcdf file with a custom convention on disk. May be deprecated.  |
| void | **[SaveEnsembleTimeSeriesToNetcdf](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-saveensembletimeseriestonetcdf)**([ENSEMBLE_PTR_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-ptr-time-series-ptr) collection, const char * filename, bool overwrite)<br>Save a multivariate time series to a netcdf file with a custom convention on disk. May be deprecated.  |
| void | **[SaveEnsembleForecastTimeSeriesToNetcdf](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-saveensembleforecasttimeseriestonetcdf)**([ENSEMBLE_FORECAST_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) tsEnsTs, const char * filename, bool overwrite)<br>Save a ensemble forecast time series to a netcdf file with a custom convention on disk. May be deprecated.  |
| bool | **[IsMissingValueItemEnsembleForecastTimeSeries](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-ismissingvalueitemensembleforecasttimeseries)**([ENSEMBLE_FORECAST_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) series, int i)<br>Is a value missing, at an issue time in an ensemble forecast time series.  |
| [ENSEMBLE_PTR_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-ptr-time-series-ptr) | **[GetItemEnsembleForecastTimeSeries](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-getitemensembleforecasttimeseries)**([ENSEMBLE_FORECAST_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) efts, int i)<br>Get an item in an ensemble forecast time series object. See also [GetItemEnsembleForecastTimeSeriesAsStructure]().  |
| [TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) | **[TimeSeriesFromEnsembleOfTimeSeries](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-timeseriesfromensembleoftimeseries)**([ENSEMBLE_PTR_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-ptr-time-series-ptr) collectionTs, int index)<br>Gets an univariate time series from an ensemble time series. See also [GetItemEnsembleTimeSeriesAsStructure]().  |
| [TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) | **[TimeSeriesFromTimeSeriesOfEnsembleOfTimeSeries](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-timeseriesfromtimeseriesofensembleoftimeseries)**([ENSEMBLE_FORECAST_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) efts, int indexInIssueTime, int indexInForecastTime)<br>Gets a forecast realisation in an ensemble forecast time series object.  |
| double | **[GetValueFromUnivariateTimeSeries](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-getvaluefromunivariatetimeseries)**([TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) ts, int index)<br>Get the value from univariate time series object.  |
| void | **[TransformEachItem](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-transformeachitem)**([ENSEMBLE_FORECAST_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) tsEnsTs, const char * method, const char * methodArgument)<br>Transform in-place each item (ensemble forecasts) of an ensemble forecast time series.  |
| void | **[SetValueToUnivariateTimeSeries](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-setvaluetounivariatetimeseries)**([TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) ts, int index, double value)<br>Sets a value of an item of a time series.  |
| multi_regular_time_series_data * | **[GetItemEnsembleForecastTimeSeriesAsStructure](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-getitemensembleforecasttimeseriesasstructure)**([ENSEMBLE_FORECAST_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) series, int i)<br>Get the item of an ensemble forecast time series, as an interoperable struct.  |
| multi_regular_time_series_data * | **[GetItemEnsembleTimeSeriesAsStructure](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-getitemensembletimeseriesasstructure)**([ENSEMBLE_PTR_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-ptr-time-series-ptr) series, int i)<br>Get the item of an ensemble time series, as an interoperable struct.  |
| void | **[SetItemEnsembleForecastTimeSeriesAsStructure](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-setitemensembleforecasttimeseriesasstructure)**([ENSEMBLE_FORECAST_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) series, int i, const multi_regular_time_series_data * values)<br>Set the item of an ensemble forecast time series, as an interoperable struct.  |
| void | **[SetItemEnsembleTimeSeriesAsStructure](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-setitemensembletimeseriesasstructure)**([ENSEMBLE_PTR_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-ptr-time-series-ptr) collection, int i, const multi_regular_time_series_data * values)<br>Set the item of an ensemble time series, as an interoperable struct.  |
| [ENSEMBLE_FORECAST_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) | **[CreatePerfectForecastTimeSeries](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-createperfectforecasttimeseries)**([TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) observations, date_time_to_second start, int length, const char * timeStepName, int offsetForecasts, int leadTime) |
| multi_regular_time_series_data * | **[ToStructEnsembleTimeSeriesData](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-tostructensembletimeseriesdata)**([ENSEMBLE_PTR_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-ptr-time-series-ptr) ensSeries)<br>Copy conversion to an interop struct representation.  |
| multi_regular_time_series_data * | **[ToStructSingleTimeSeriesData](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-tostructsingletimeseriesdata)**([TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) timeSeries)<br>Copy conversion to an interop struct representation.  |
| [ENSEMBLE_PTR_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-ptr-time-series-ptr) | **[CreateEnsembleTimeSeriesDataFromStruct](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-createensembletimeseriesdatafromstruct)**(const multi_regular_time_series_data * ensSeries)<br>Copy conversion from an interop struct representation to an opaque object representation.  |
| [TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) | **[CreateSingleTimeSeriesDataFromStruct](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-createsingletimeseriesdatafromstruct)**(const multi_regular_time_series_data * timeSeries)<br>Copy conversion from an interop struct representation to an opaque object representation.  |
| void | **[DisposeMultiTimeSeriesData](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-disposemultitimeseriesdata)**(multi_regular_time_series_data * data)<br>Dispose of the memory held by a multi_regular_time_series_data struct. This multi_regular_time_series_data must have been created via this library API, not elsewhere.  |
| void | **[GetTimeSeriesGeometry](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-gettimeseriesgeometry)**([TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) timeSeries, [TS_GEOMETRY_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__transparent__pointers_8h/#define-ts-geometry-ptr) geom)<br>Get the temporal geometry of a time series object.  |
| void | **[GetEnsembleForecastTimeSeriesGeometry](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-getensembleforecasttimeseriesgeometry)**([ENSEMBLE_FORECAST_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr) timeSeries, [TS_GEOMETRY_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__transparent__pointers_8h/#define-ts-geometry-ptr) geom)<br>Get the temporal geometry of a the main time dimension of an ensemble forecast time series object.  |
| void | **[GetTimeSeriesValues](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-gettimeseriesvalues)**([TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) timeSeries, double * values, int arrayLength)<br>Retrieve the values of a time series. See also [ToStructSingleTimeSeriesData](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-tostructsingletimeseriesdata).  |
| int | **[GetNumTimeSeries](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-getnumtimeseries)**()<br>IGNORE - function unused but for old optional unit tests on reference counting and memory management.  |
| void | **[GetProviderTsGeometry](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-getprovidertsgeometry)**([TIME_SERIES_PROVIDER_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-provider-ptr) dataLibrary, const char * variableIdentifier, [TS_GEOMETRY_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__transparent__pointers_8h/#define-ts-geometry-ptr) geom)<br>Get the temporal geometry of a time series, available by an identifier in a time series provider. Time series providers are a class of objects (data libraries, model simulations) that can provide time series for a given string identifier.  |
| void | **[GetProviderTimeSeriesValues](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-getprovidertimeseriesvalues)**([TIME_SERIES_PROVIDER_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-provider-ptr) dataLibrary, const char * variableIdentifier, double * values, int arrayLength)<br>Get the values a time series, available by an identifier in a time series provider. Time series providers are a class of objects (data libraries, model simulations) that can provide time series for a given string identifier.  |
| char ** | **[GetProviderTimeSeriesIdentifiers](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-getprovidertimeseriesidentifiers)**([TIME_SERIES_PROVIDER_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-provider-ptr) dataLibrary, int * size)<br>Gets the known identifiers of a time series provider (data library items, or model simulation with recorded state variables)  |
| [TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr) | **[TimeSeriesFromProviderTs](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-timeseriesfromproviderts)**([TIME_SERIES_PROVIDER_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-provider-ptr) dataLibrary, const char * variableIdentifier)<br>Gets a univariate time series from a time series provider.  |

## Defines

|                | Name           |
| -------------- | -------------- |
|  | **[DATATYPES_USE_CPP_POINTERS](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#define-datatypes-use-cpp-pointers)**  |
|  | **[DATATYPES_API](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#define-datatypes-api)**  |

## Detailed Description


API for libswift. This file exposes a common API for interacting with libswift from other tools. 


## Functions Documentation

### function GetLastStdExceptionMessage

```cpp
char * GetLastStdExceptionMessage()
```

Gets the last message from an std::exception caught by the uchronia API. 

**Return**: the last standard exception message. 

### function RegisterExceptionCallback

```cpp
void RegisterExceptionCallback(
    const void * callback
)
```

Registers a function to call when uchronia has generated a std::exception that has been caught by the API. 

**Parameters**: 

  * **callback** function pointer. The function must have a signature like void on_error_message(const char* msg); 


### function DisposeSharedPointer

```cpp
void DisposeSharedPointer(
    VOID_PTR_PROVIDER_PTR ptr
)
```

Notifies uchronia that an object managed by an opaque pointer is not used by the caller anymore. 

**Parameters**: 

  * **ptr** pointer obtained via the API, such as a MODEL_SIMULATION_PTR. 


### function DeleteAnsiStringArray

```cpp
void DeleteAnsiStringArray(
    char ** values,
    int arrayLength
)
```

Deletes the ANSI string array , which has been create by uchronia. Do not use for char** created outside uchronia. 

**Parameters**: 

  * **values** pointer to the array to delete (its elements and the array itself). 
  * **arrayLength** Length of the array. 


### function DeleteAnsiString

```cpp
void DeleteAnsiString(
    const char * value
)
```

Deletes the ANSI string which has been create by uchronia. Do not use for char* created outside uchronia. 

**Parameters**: 

  * **value** a C-style string, which has been create by uchronia. Do not use for char* created elsewhere. 


### function DeleteDoubleArray

```cpp
void DeleteDoubleArray(
    double * value
)
```

Dispose of an array of double created via this C API. 

**Parameters**: 

  * **value** If non-null, the value. 


### function SetTimeSeriesMissingValueValue

```cpp
void SetTimeSeriesMissingValueValue(
    double missingValueValue
)
```

Sets a value whoch should be considered as a missing value when data is passed to this C API. 

**Parameters**: 

  * **missingValueValue** The missing value. 


### function LoadEnsembleDataset

```cpp
ENSEMBLE_DATA_SET_PTR LoadEnsembleDataset(
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
ENSEMBLE_DATA_SET_PTR CreateEnsembleDataset(
    const char * type
)
```

Creates a time series library. 

**Parameters**: 

  * **type** The type of library to create. Currently supports cases for unit tests and time series libraries that can be "recorded to" by modelling engines.


**Return**: The new ensemble dataset. 

### function GetEnsembleDatasetDataIdentifiers

```cpp
char ** GetEnsembleDatasetDataIdentifiers(
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
char ** GetEnsembleDatasetDataSubIdentifiers(
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
char ** GetEnsembleDatasetDataSummaries(
    ENSEMBLE_DATA_SET_PTR dataLibrary,
    int * size
)
```

Get brief summary descriptions of each dataset in a data library. 

**Parameters**: 

  * **dataLibrary** data library 
  * **size** number of summaries returned 


**Return**: char** 

### function GetDataDimensionsDescription

```cpp
time_series_dimensions_description * GetDataDimensionsDescription(
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
int EnsembleSizeEnsembleTimeSeries(
    ENSEMBLE_PTR_TIME_SERIES_PTR ensSeries
)
```

Gets the number of ensembles in an ensemble time series. 

**Parameters**: 

  * **ensSeries** ensemble time series 


**Return**: number of ensembles 

### function DisposeDataDimensionsDescriptions

```cpp
void DisposeDataDimensionsDescriptions(
    time_series_dimensions_description * data
)
```

Dispose of a time_series_dimensions_description previously returned by this API. 

**Parameters**: 

  * **data** pointer to the struct to dispose of 


### function CreateEnsembleForecastTimeSeries

```cpp
ENSEMBLE_FORECAST_TIME_SERIES_PTR CreateEnsembleForecastTimeSeries(
    date_time_to_second start,
    int length,
    const char * timeStepName
)
```

Create a Ensemble Forecast Time Series object. This is a time series of ensembles of time series. The conceptual dimensions are time (forecast issue time), ensemble, and forecast lead time. 

**Parameters**: 

  * **start** Start time of the time series along the forecast issue time dimension 
  * **length** Length of the time series along the forecast issue time dimension 
  * **timeStepName** time step identifier along the forecast issue time dimension. Supported includes 'daily', 'hourly', 'monthly', and regular time durations such as '03:00:00' 


**Return**: reference counted wrapper to an ensemble forecast time series. 

### function GetDatasetSingleTimeSeries

```cpp
TIME_SERIES_PTR GetDatasetSingleTimeSeries(
    ENSEMBLE_DATA_SET_PTR dataLibrary,
    const char * dataId
)
```

Gets a univariate Time Series out of a data library. 

**Parameters**: 

  * **dataLibrary** data library 
  * **dataId** identifier 


**Return**: reference counted wrapper to the new object. 

### function GetDatasetEnsembleTimeSeries

```cpp
ENSEMBLE_PTR_TIME_SERIES_PTR GetDatasetEnsembleTimeSeries(
    ENSEMBLE_DATA_SET_PTR dataLibrary,
    const char * dataEnsembleId
)
```

Gets a multivariate (ensemble) Time Series out of a data library. 

**Parameters**: 

  * **dataLibrary** data library 
  * **dataEnsembleId** identifier 


**Return**: reference counted wrapper to the new object. 

### function GetDatasetEnsembleForecastTimeSeries

```cpp
ENSEMBLE_FORECAST_TIME_SERIES_PTR GetDatasetEnsembleForecastTimeSeries(
    ENSEMBLE_DATA_SET_PTR dataLibrary,
    const char * dataId
)
```

Gets an ensemble forecast time serie (time series of ensemble time series ) out of a data library. 

**Parameters**: 

  * **dataLibrary** data library 
  * **dataId** identifier 


**Return**: reference counted wrapper to the new object. 

### function SaveSingleTimeSeriesToNetcdf

```cpp
void SaveSingleTimeSeriesToNetcdf(
    TIME_SERIES_PTR timeSeries,
    const char * filename,
    bool overwrite
)
```

Save a time series to a netcdf file with a custom convention on disk. May be deprecated. 

**Parameters**: 

  * **timeSeries** data to save 
  * **filename** file name 
  * **overwrite** if true, overwrite if the file already exists. 


### function SaveEnsembleTimeSeriesToNetcdf

```cpp
void SaveEnsembleTimeSeriesToNetcdf(
    ENSEMBLE_PTR_TIME_SERIES_PTR collection,
    const char * filename,
    bool overwrite
)
```

Save a multivariate time series to a netcdf file with a custom convention on disk. May be deprecated. 

**Parameters**: 

  * **collection** ensemble time series 
  * **filename** file name 
  * **overwrite** if true, overwrite if the file already exists. 


### function SaveEnsembleForecastTimeSeriesToNetcdf

```cpp
void SaveEnsembleForecastTimeSeriesToNetcdf(
    ENSEMBLE_FORECAST_TIME_SERIES_PTR tsEnsTs,
    const char * filename,
    bool overwrite
)
```

Save a ensemble forecast time series to a netcdf file with a custom convention on disk. May be deprecated. 

**Parameters**: 

  * **tsEnsTs** data to save 
  * **filename** file name 
  * **overwrite** if true, overwrite if the file already exists. 


### function IsMissingValueItemEnsembleForecastTimeSeries

```cpp
bool IsMissingValueItemEnsembleForecastTimeSeries(
    ENSEMBLE_FORECAST_TIME_SERIES_PTR series,
    int i
)
```

Is a value missing, at an issue time in an ensemble forecast time series. 

**Parameters**: 

  * **series** ensemble forecast time series 
  * **i** item index to check 


**Return**: true (non-zero) if the value is missing (e.g. nullptr i.e. no forecast for that issue time) 

### function GetItemEnsembleForecastTimeSeries

```cpp
ENSEMBLE_PTR_TIME_SERIES_PTR GetItemEnsembleForecastTimeSeries(
    ENSEMBLE_FORECAST_TIME_SERIES_PTR efts,
    int i
)
```

Get an item in an ensemble forecast time series object. See also [GetItemEnsembleForecastTimeSeriesAsStructure](). 

**Parameters**: 

  * **efts** ensemble forecast time series 
  * **i** index (issue time) 


**Return**: a multivariate time series, the forecasts for issue time i 

### function TimeSeriesFromEnsembleOfTimeSeries

```cpp
TIME_SERIES_PTR TimeSeriesFromEnsembleOfTimeSeries(
    ENSEMBLE_PTR_TIME_SERIES_PTR collectionTs,
    int index
)
```

Gets an univariate time series from an ensemble time series. See also [GetItemEnsembleTimeSeriesAsStructure](). 

**Parameters**: 

  * **collectionTs** ensemble time series 
  * **index** index in the ensemble dimension 


**Return**: univariate time series 

### function TimeSeriesFromTimeSeriesOfEnsembleOfTimeSeries

```cpp
TIME_SERIES_PTR TimeSeriesFromTimeSeriesOfEnsembleOfTimeSeries(
    ENSEMBLE_FORECAST_TIME_SERIES_PTR efts,
    int indexInIssueTime,
    int indexInForecastTime
)
```

Gets a forecast realisation in an ensemble forecast time series object. 

**Parameters**: 

  * **efts** ensemble forecast time series object 
  * **indexInIssueTime** index (issue time) 
  * **indexInForecastTime** index in the ensemble dimension 


**Return**: univariate time series 

### function GetValueFromUnivariateTimeSeries

```cpp
double GetValueFromUnivariateTimeSeries(
    TIME_SERIES_PTR ts,
    int index
)
```

Get the value from univariate time series object. 

**Parameters**: 

  * **ts** time series 
  * **index** index of interest 


**Return**: time series value at that index 

### function TransformEachItem

```cpp
void TransformEachItem(
    ENSEMBLE_FORECAST_TIME_SERIES_PTR tsEnsTs,
    const char * method,
    const char * methodArgument
)
```

Transform in-place each item (ensemble forecasts) of an ensemble forecast time series. 

**Parameters**: 

  * **tsEnsTs** ensemble forecast time series 
  * **method** a valid transformation method: either 'aggregate' or 'disaggregate' at the time of writing. Exception thrown otherwise. 
  * **methodArgument** a string description of the arguments to the method. Currently supported is the target time step in the aggregation/disaggregation, e.g. to three-hourly with '03:00:00' 


### function SetValueToUnivariateTimeSeries

```cpp
void SetValueToUnivariateTimeSeries(
    TIME_SERIES_PTR ts,
    int index,
    double value
)
```

Sets a value of an item of a time series. 

### function GetItemEnsembleForecastTimeSeriesAsStructure

```cpp
multi_regular_time_series_data * GetItemEnsembleForecastTimeSeriesAsStructure(
    ENSEMBLE_FORECAST_TIME_SERIES_PTR series,
    int i
)
```

Get the item of an ensemble forecast time series, as an interoperable struct. 

**Parameters**: 

  * **series** ensemble forecast time series 
  * **i** item index 


**Return**: pointer to a new multi_regular_time_series_data 

### function GetItemEnsembleTimeSeriesAsStructure

```cpp
multi_regular_time_series_data * GetItemEnsembleTimeSeriesAsStructure(
    ENSEMBLE_PTR_TIME_SERIES_PTR series,
    int i
)
```

Get the item of an ensemble time series, as an interoperable struct. 

**Parameters**: 

  * **series** ensemble time series 
  * **i** item index 


**Return**: pointer to a new multi_regular_time_series_data (univariate series in effect) 

### function SetItemEnsembleForecastTimeSeriesAsStructure

```cpp
void SetItemEnsembleForecastTimeSeriesAsStructure(
    ENSEMBLE_FORECAST_TIME_SERIES_PTR series,
    int i,
    const multi_regular_time_series_data * values
)
```

Set the item of an ensemble forecast time series, as an interoperable struct. 

**Parameters**: 

  * **series** ensemble forecast time series 
  * **i** item index 
  * **values** interoperable multi_regular_time_series_data, expected to represent an ensemble (multivariate) time series 


### function SetItemEnsembleTimeSeriesAsStructure

```cpp
void SetItemEnsembleTimeSeriesAsStructure(
    ENSEMBLE_PTR_TIME_SERIES_PTR collection,
    int i,
    const multi_regular_time_series_data * values
)
```

Set the item of an ensemble time series, as an interoperable struct. 

**Parameters**: 

  * **series** ensemble time series 
  * **i** item index, along the ensemble dimension (i.e. one of the realisations of the ensemble) 
  * **values** interoperable multi_regular_time_series_data, expected to represent an univariate time series 


### function CreatePerfectForecastTimeSeries

```cpp
ENSEMBLE_FORECAST_TIME_SERIES_PTR CreatePerfectForecastTimeSeries(
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
multi_regular_time_series_data * ToStructEnsembleTimeSeriesData(
    ENSEMBLE_PTR_TIME_SERIES_PTR ensSeries
)
```

Copy conversion to an interop struct representation. 

### function ToStructSingleTimeSeriesData

```cpp
multi_regular_time_series_data * ToStructSingleTimeSeriesData(
    TIME_SERIES_PTR timeSeries
)
```

Copy conversion to an interop struct representation. 

### function CreateEnsembleTimeSeriesDataFromStruct

```cpp
ENSEMBLE_PTR_TIME_SERIES_PTR CreateEnsembleTimeSeriesDataFromStruct(
    const multi_regular_time_series_data * ensSeries
)
```

Copy conversion from an interop struct representation to an opaque object representation. 

### function CreateSingleTimeSeriesDataFromStruct

```cpp
TIME_SERIES_PTR CreateSingleTimeSeriesDataFromStruct(
    const multi_regular_time_series_data * timeSeries
)
```

Copy conversion from an interop struct representation to an opaque object representation. 

### function DisposeMultiTimeSeriesData

```cpp
void DisposeMultiTimeSeriesData(
    multi_regular_time_series_data * data
)
```

Dispose of the memory held by a multi_regular_time_series_data struct. This multi_regular_time_series_data must have been created via this library API, not elsewhere. 

### function GetTimeSeriesGeometry

```cpp
void GetTimeSeriesGeometry(
    TIME_SERIES_PTR timeSeries,
    TS_GEOMETRY_PTR geom
)
```

Get the temporal geometry of a time series object. 

**Parameters**: 

  * **timeSeries** time series 
  * **geom** pointer to a regular_time_series_geometry struct, whose values will be written to 


### function GetEnsembleForecastTimeSeriesGeometry

```cpp
void GetEnsembleForecastTimeSeriesGeometry(
    ENSEMBLE_FORECAST_TIME_SERIES_PTR timeSeries,
    TS_GEOMETRY_PTR geom
)
```

Get the temporal geometry of a the main time dimension of an ensemble forecast time series object. 

**Parameters**: 

  * **timeSeries** ensemble forecast time series 
  * **geom** pointer to a regular_time_series_geometry struct, whose values will be written to 


### function GetTimeSeriesValues

```cpp
void GetTimeSeriesValues(
    TIME_SERIES_PTR timeSeries,
    double * values,
    int arrayLength
)
```

Retrieve the values of a time series. See also [ToStructSingleTimeSeriesData](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-tostructsingletimeseriesdata). 

**Parameters**: 

  * **timeSeries** time series 
  * **values** allocated array where values will be written to 
  * **arrayLength** allocated array size. 


### function GetNumTimeSeries

```cpp
int GetNumTimeSeries()
```

IGNORE - function unused but for old optional unit tests on reference counting and memory management. 

### function GetProviderTsGeometry

```cpp
void GetProviderTsGeometry(
    TIME_SERIES_PROVIDER_PTR dataLibrary,
    const char * variableIdentifier,
    TS_GEOMETRY_PTR geom
)
```

Get the temporal geometry of a time series, available by an identifier in a time series provider. Time series providers are a class of objects (data libraries, model simulations) that can provide time series for a given string identifier. 

**Parameters**: 

  * **dataLibrary** data librarytime series provider object, e.g. via an [ENSEMBLE_DATA_SET_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr), or a model simulation in a modelling system such as SWIFT2. 
  * **variableIdentifier** variable identifier 
  * **geom** pointer to a regular_time_series_geometry struct, whose values will be written to 


### function GetProviderTimeSeriesValues

```cpp
void GetProviderTimeSeriesValues(
    TIME_SERIES_PROVIDER_PTR dataLibrary,
    const char * variableIdentifier,
    double * values,
    int arrayLength
)
```

Get the values a time series, available by an identifier in a time series provider. Time series providers are a class of objects (data libraries, model simulations) that can provide time series for a given string identifier. 

**Parameters**: 

  * **dataLibrary** data librarytime series provider object, e.g. via an [ENSEMBLE_DATA_SET_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr), or a model simulation in a modelling system such as SWIFT2. 
  * **variableIdentifier** variable identifier 
  * **values** allocated array where values will be written to 
  * **arrayLength** allocated array size, gotten from [GetProviderTsGeometry](/uchronia-ts-doc/cpp/Files/extern__c__api_8h/#function-getprovidertsgeometry)


### function GetProviderTimeSeriesIdentifiers

```cpp
char ** GetProviderTimeSeriesIdentifiers(
    TIME_SERIES_PROVIDER_PTR dataLibrary,
    int * size
)
```

Gets the known identifiers of a time series provider (data library items, or model simulation with recorded state variables) 

**Parameters**: 

  * **dataLibrary** data librarytime series provider object, e.g. via an [ENSEMBLE_DATA_SET_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr), or a model simulation in a modelling system such as SWIFT2. 
  * **size** number of data identifiers 


**Return**: char** of size 'size' 

### function TimeSeriesFromProviderTs

```cpp
TIME_SERIES_PTR TimeSeriesFromProviderTs(
    TIME_SERIES_PROVIDER_PTR dataLibrary,
    const char * variableIdentifier
)
```

Gets a univariate time series from a time series provider. 

**Parameters**: 

  * **dataLibrary** data librarytime series provider object, e.g. via an [ENSEMBLE_DATA_SET_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr), or a model simulation in a modelling system such as SWIFT2. 
  * **variableIdentifier** variable identifier 


**Return**: reference counted wrapper to a new time series. 



## Macros Documentation

### define DATATYPES_USE_CPP_POINTERS

```cpp
#define DATATYPES_USE_CPP_POINTERS 
```


### define DATATYPES_API

```cpp
#define DATATYPES_API 
```


## Source code

```cpp

#pragma once

#include "datatypes/setup_exports.h"

#ifndef DATATYPES_USE_OPAQUE_POINTERS
#ifndef DATATYPES_USE_CPP_POINTERS
#ifndef USING_DATATYPES_CORE
#define DATATYPES_USE_CPP_POINTERS
#endif
#endif
#endif

#include "datatypes/interop_struct.h"

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

    DATATYPES_API ENSEMBLE_FORECAST_TIME_SERIES_PTR GetDatasetEnsembleForecastTimeSeries(ENSEMBLE_DATA_SET_PTR dataLibrary, const char* dataId);

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

Updated on 2022-08-21 at 18:10:33 +1000
