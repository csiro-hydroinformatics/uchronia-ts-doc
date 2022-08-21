---
title: datatypes/internals_c_api.hpp

---

# datatypes/internals_c_api.hpp



## Defines

|                | Name           |
| -------------- | -------------- |
|  | **[TIME_SERIES_DYNCAST](/uchronia-ts-doc/cpp/Files/internals__c__api_8hpp/#define-time-series-dyncast)**(x)  |
|  | **[TIME_SERIES_PROVIDER_DYNCAST](/uchronia-ts-doc/cpp/Files/internals__c__api_8hpp/#define-time-series-provider-dyncast)**(x)  |
|  | **[ENSEMBLE_DATA_SET_DYNCAST](/uchronia-ts-doc/cpp/Files/internals__c__api_8hpp/#define-ensemble-data-set-dyncast)**(x)  |
|  | **[ENSEMBLE_FORECAST_TIME_SERIES_DYNCAST](/uchronia-ts-doc/cpp/Files/internals__c__api_8hpp/#define-ensemble-forecast-time-series-dyncast)**(x)  |
|  | **[ENSEMBLE_PTR_TIME_SERIES_DYNCAST](/uchronia-ts-doc/cpp/Files/internals__c__api_8hpp/#define-ensemble-ptr-time-series-dyncast)**(x)  |
|  | **[DATE_TIME_INFO_DYNCAST](/uchronia-ts-doc/cpp/Files/internals__c__api_8hpp/#define-date-time-info-dyncast)**(x)  |
|  | **[TS_GEOMETRY_DYNCAST](/uchronia-ts-doc/cpp/Files/internals__c__api_8hpp/#define-ts-geometry-dyncast)**(x)  |
|  | **[FREE_ARRAY](/uchronia-ts-doc/cpp/Files/internals__c__api_8hpp/#define-free-array)**(x)  |
|  | **[WRAP_DATE_TIME_INFO_PTR](/uchronia-ts-doc/cpp/Files/internals__c__api_8hpp/#define-wrap-date-time-info-ptr)**(x)  |
|  | **[WRAP_TIME_SERIES_PROVIDER_PTR](/uchronia-ts-doc/cpp/Files/internals__c__api_8hpp/#define-wrap-time-series-provider-ptr)**(x)  |
|  | **[WRAP_ENSEMBLE_DATA_SET_PTR](/uchronia-ts-doc/cpp/Files/internals__c__api_8hpp/#define-wrap-ensemble-data-set-ptr)**(x)  |
|  | **[WRAP_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/internals__c__api_8hpp/#define-wrap-time-series-ptr)**(x)  |
|  | **[WRAP_ENSEMBLE_FORECAST_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/internals__c__api_8hpp/#define-wrap-ensemble-forecast-time-series-ptr)**(x)  |
|  | **[WRAP_ENSEMBLE_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/internals__c__api_8hpp/#define-wrap-ensemble-time-series-ptr)**(x)  |




## Macros Documentation

### define TIME_SERIES_DYNCAST

```cpp
#define TIME_SERIES_DYNCAST(
    x
)
CHECKED_RETRIEVE_PTR(DATATYPES_TIME_SERIES_DOUBLE, x)
```


### define TIME_SERIES_PROVIDER_DYNCAST

```cpp
#define TIME_SERIES_PROVIDER_DYNCAST(
    x
)
CHECKED_RETRIEVE_PTR(TimeSeriesProvider<double>, x)
```


### define ENSEMBLE_DATA_SET_DYNCAST

```cpp
#define ENSEMBLE_DATA_SET_DYNCAST(
    x
)
CHECKED_RETRIEVE_PTR(TimeSeriesLibrary, x)
```


### define ENSEMBLE_FORECAST_TIME_SERIES_DYNCAST

```cpp
#define ENSEMBLE_FORECAST_TIME_SERIES_DYNCAST(
    x
)
CHECKED_RETRIEVE_PTR(ENSEMBLE_FORECAST_TIME_SERIES_DOUBLE, x)
```


### define ENSEMBLE_PTR_TIME_SERIES_DYNCAST

```cpp
#define ENSEMBLE_PTR_TIME_SERIES_DYNCAST(
    x
)
CHECKED_RETRIEVE_PTR(DATATYPES_ENSEMBLE_PTR_TIME_SERIES_DOUBLE, x)
```


### define DATE_TIME_INFO_DYNCAST

```cpp
#define DATE_TIME_INFO_DYNCAST(
    x
)
(date_time_to_second*)x
```


### define TS_GEOMETRY_DYNCAST

```cpp
#define TS_GEOMETRY_DYNCAST(
    x
)
x
```


### define FREE_ARRAY

```cpp
#define FREE_ARRAY(
    x
)
delete[] x
```


### define WRAP_DATE_TIME_INFO_PTR

```cpp
#define WRAP_DATE_TIME_INFO_PTR(
    x
)
new reference_handle<date_time_to_second>(x)
```


### define WRAP_TIME_SERIES_PROVIDER_PTR

```cpp
#define WRAP_TIME_SERIES_PROVIDER_PTR(
    x
)
new reference_handle<TimeSeriesProvider<double>>(x)
```


### define WRAP_ENSEMBLE_DATA_SET_PTR

```cpp
#define WRAP_ENSEMBLE_DATA_SET_PTR(
    x
)
new reference_handle<TimeSeriesLibrary>(x)
```


### define WRAP_TIME_SERIES_PTR

```cpp
#define WRAP_TIME_SERIES_PTR(
    x
)
new reference_handle<DATATYPES_TIME_SERIES_DOUBLE>(x)
```


### define WRAP_ENSEMBLE_FORECAST_TIME_SERIES_PTR

```cpp
#define WRAP_ENSEMBLE_FORECAST_TIME_SERIES_PTR(
    x
)
new reference_handle<EnsembleForecastTimeSeries<DATATYPES_TIME_SERIES_DOUBLE>>(x)
```


### define WRAP_ENSEMBLE_TIME_SERIES_PTR

```cpp
#define WRAP_ENSEMBLE_TIME_SERIES_PTR(
    x
)
new reference_handle<DATATYPES_ENSEMBLE_PTR_TIME_SERIES_DOUBLE>(x)
```


## Source code

```cpp
#pragma once

#include "moirai/reference_handle.hpp"
#include "datatypes/extern_c_api_transparent_pointers.h"

#define TIME_SERIES_DYNCAST(x) CHECKED_RETRIEVE_PTR(DATATYPES_TIME_SERIES_DOUBLE, x)
#define TIME_SERIES_PROVIDER_DYNCAST(x) CHECKED_RETRIEVE_PTR(TimeSeriesProvider<double>, x)
#define ENSEMBLE_DATA_SET_DYNCAST(x) CHECKED_RETRIEVE_PTR(TimeSeriesLibrary, x)
#define ENSEMBLE_FORECAST_TIME_SERIES_DYNCAST(x) CHECKED_RETRIEVE_PTR(ENSEMBLE_FORECAST_TIME_SERIES_DOUBLE, x)
#define ENSEMBLE_PTR_TIME_SERIES_DYNCAST(x) CHECKED_RETRIEVE_PTR(DATATYPES_ENSEMBLE_PTR_TIME_SERIES_DOUBLE, x)

#define DATE_TIME_INFO_DYNCAST(x) (date_time_to_second*)x
#define TS_GEOMETRY_DYNCAST(x) x

#define FREE_ARRAY(x) delete[] x

#define WRAP_DATE_TIME_INFO_PTR(x)  new reference_handle<date_time_to_second>(x)
#define WRAP_TIME_SERIES_PROVIDER_PTR(x)  new reference_handle<TimeSeriesProvider<double>>(x)
#define WRAP_ENSEMBLE_DATA_SET_PTR(x)  new reference_handle<TimeSeriesLibrary>(x)
#define WRAP_TIME_SERIES_PTR(x)   new reference_handle<DATATYPES_TIME_SERIES_DOUBLE>(x)
#define WRAP_ENSEMBLE_FORECAST_TIME_SERIES_PTR(x)  new reference_handle<EnsembleForecastTimeSeries<DATATYPES_TIME_SERIES_DOUBLE>>(x)
#define WRAP_ENSEMBLE_TIME_SERIES_PTR(x)  new reference_handle<DATATYPES_ENSEMBLE_PTR_TIME_SERIES_DOUBLE>(x)
```


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000
