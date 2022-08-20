---
title: datatypes/extern_c_api_transparent_pointers.h

---

# datatypes/extern_c_api_transparent_pointers.h



## Defines

|                | Name           |
| -------------- | -------------- |
|  | **[DATATYPES_TIME_SERIES_DOUBLE](/uchronia-ts-doc/cpp/Files/extern__c__api__transparent__pointers_8h/#define-datatypes-time-series-double)**  |
|  | **[DATATYPES_TIME_SERIES_DOUBLE_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__transparent__pointers_8h/#define-datatypes-time-series-double-ptr)**  |
|  | **[DATATYPES_ENSEMBLE_TIME_SERIES_DOUBLE](/uchronia-ts-doc/cpp/Files/extern__c__api__transparent__pointers_8h/#define-datatypes-ensemble-time-series-double)**  |
|  | **[DATATYPES_ENSEMBLE_PTR_TIME_SERIES_DOUBLE](/uchronia-ts-doc/cpp/Files/extern__c__api__transparent__pointers_8h/#define-datatypes-ensemble-ptr-time-series-double)**  |
|  | **[ENSEMBLE_FORECAST_TIME_SERIES_DOUBLE](/uchronia-ts-doc/cpp/Files/extern__c__api__transparent__pointers_8h/#define-ensemble-forecast-time-series-double)**  |
|  | **[TS_GEOMETRY_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__transparent__pointers_8h/#define-ts-geometry-ptr)**  |
|  | **[MULTI_REGULAR_SERIES_STRUCT_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__transparent__pointers_8h/#define-multi-regular-series-struct-ptr)**  |
|  | **[DATE_TIME_INFO_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__transparent__pointers_8h/#define-date-time-info-ptr)**  |
|  | **[TIME_SERIES_TRANSPARENT_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__transparent__pointers_8h/#define-time-series-transparent-ptr)**  |
|  | **[ENSEMBLE_DATA_SET_TRANSPARENT_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__transparent__pointers_8h/#define-ensemble-data-set-transparent-ptr)**  |
|  | **[ENSEMBLE_FORECAST_TIME_SERIES_TRANSPARENT_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__transparent__pointers_8h/#define-ensemble-forecast-time-series-transparent-ptr)**  |
|  | **[ENSEMBLE_TIME_SERIES_TRANSPARENT_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__transparent__pointers_8h/#define-ensemble-time-series-transparent-ptr)**  |
|  | **[ENSEMBLE_PTR_TIME_SERIES_TRANSPARENT_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__transparent__pointers_8h/#define-ensemble-ptr-time-series-transparent-ptr)**  |
|  | **[TIME_SERIES_PROVIDER_TRANSPARENT_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__transparent__pointers_8h/#define-time-series-provider-transparent-ptr)**  |




## Macros Documentation

### define DATATYPES_TIME_SERIES_DOUBLE

```cpp
#define DATATYPES_TIME_SERIES_DOUBLE TimeSeries
```


### define DATATYPES_TIME_SERIES_DOUBLE_PTR

```cpp
#define DATATYPES_TIME_SERIES_DOUBLE_PTR DATATYPES_TIME_SERIES_DOUBLE*
```


### define DATATYPES_ENSEMBLE_TIME_SERIES_DOUBLE

```cpp
#define DATATYPES_ENSEMBLE_TIME_SERIES_DOUBLE MultiTimeSeries<DATATYPES_TIME_SERIES_DOUBLE>
```


### define DATATYPES_ENSEMBLE_PTR_TIME_SERIES_DOUBLE

```cpp
#define DATATYPES_ENSEMBLE_PTR_TIME_SERIES_DOUBLE MultiTimeSeries<DATATYPES_TIME_SERIES_DOUBLE_PTR>
```


### define ENSEMBLE_FORECAST_TIME_SERIES_DOUBLE

```cpp
#define ENSEMBLE_FORECAST_TIME_SERIES_DOUBLE EnsembleForecastTimeSeries<DATATYPES_TIME_SERIES_DOUBLE>
```


### define TS_GEOMETRY_PTR

```cpp
#define TS_GEOMETRY_PTR regular_time_series_geometry*
```


### define MULTI_REGULAR_SERIES_STRUCT_PTR

```cpp
#define MULTI_REGULAR_SERIES_STRUCT_PTR multi_regular_time_series_data*
```


### define DATE_TIME_INFO_PTR

```cpp
#define DATE_TIME_INFO_PTR date_time_to_second*
```


### define TIME_SERIES_TRANSPARENT_PTR

```cpp
#define TIME_SERIES_TRANSPARENT_PTR reference_handle<DATATYPES_TIME_SERIES_DOUBLE>*
```


### define ENSEMBLE_DATA_SET_TRANSPARENT_PTR

```cpp
#define ENSEMBLE_DATA_SET_TRANSPARENT_PTR reference_handle<TimeSeriesLibrary>*
```


### define ENSEMBLE_FORECAST_TIME_SERIES_TRANSPARENT_PTR

```cpp
#define ENSEMBLE_FORECAST_TIME_SERIES_TRANSPARENT_PTR reference_handle<ENSEMBLE_FORECAST_TIME_SERIES_DOUBLE>*
```


### define ENSEMBLE_TIME_SERIES_TRANSPARENT_PTR

```cpp
#define ENSEMBLE_TIME_SERIES_TRANSPARENT_PTR reference_handle<DATATYPES_ENSEMBLE_TIME_SERIES_DOUBLE>*
```


### define ENSEMBLE_PTR_TIME_SERIES_TRANSPARENT_PTR

```cpp
#define ENSEMBLE_PTR_TIME_SERIES_TRANSPARENT_PTR reference_handle<DATATYPES_ENSEMBLE_PTR_TIME_SERIES_DOUBLE>*
```


### define TIME_SERIES_PROVIDER_TRANSPARENT_PTR

```cpp
#define TIME_SERIES_PROVIDER_TRANSPARENT_PTR reference_handle<TimeSeriesProvider<double>>*
```


## Source code

```cpp
// This file deliberately does not have a #pragma once directive

#include "datatypes/setup_exports.h"
#include "datatypes/interop_struct.h"
#include "datatypes/time_series_store.hpp"
#include "moirai/reference_handle.hpp"

using namespace datatypes::timeseries;

#define DATATYPES_TIME_SERIES_DOUBLE TimeSeries
#define DATATYPES_TIME_SERIES_DOUBLE_PTR DATATYPES_TIME_SERIES_DOUBLE*
#define DATATYPES_ENSEMBLE_TIME_SERIES_DOUBLE MultiTimeSeries<DATATYPES_TIME_SERIES_DOUBLE>
#define DATATYPES_ENSEMBLE_PTR_TIME_SERIES_DOUBLE MultiTimeSeries<DATATYPES_TIME_SERIES_DOUBLE_PTR>
#define ENSEMBLE_FORECAST_TIME_SERIES_DOUBLE EnsembleForecastTimeSeries<DATATYPES_TIME_SERIES_DOUBLE>

#define TS_GEOMETRY_PTR  regular_time_series_geometry*
#define MULTI_REGULAR_SERIES_STRUCT_PTR multi_regular_time_series_data*
#define DATE_TIME_INFO_PTR  date_time_to_second*

// Definitions of macros for reference_handle<>

using moirai::reference_handle;

#define TIME_SERIES_TRANSPARENT_PTR  reference_handle<DATATYPES_TIME_SERIES_DOUBLE>*
#define ENSEMBLE_DATA_SET_TRANSPARENT_PTR  reference_handle<TimeSeriesLibrary>*
#define ENSEMBLE_FORECAST_TIME_SERIES_TRANSPARENT_PTR  reference_handle<ENSEMBLE_FORECAST_TIME_SERIES_DOUBLE>*
#define ENSEMBLE_TIME_SERIES_TRANSPARENT_PTR  reference_handle<DATATYPES_ENSEMBLE_TIME_SERIES_DOUBLE>*
#define ENSEMBLE_PTR_TIME_SERIES_TRANSPARENT_PTR  reference_handle<DATATYPES_ENSEMBLE_PTR_TIME_SERIES_DOUBLE>*
#define TIME_SERIES_PROVIDER_TRANSPARENT_PTR  reference_handle<TimeSeriesProvider<double>>*
```


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000
