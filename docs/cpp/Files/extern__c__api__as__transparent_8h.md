---
title: datatypes/extern_c_api_as_transparent.h

---

# datatypes/extern_c_api_as_transparent.h



## Defines

|                | Name           |
| -------------- | -------------- |
|  | **[TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-ptr)**  |
|  | **[ENSEMBLE_DATA_SET_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-data-set-ptr)**  |
|  | **[ENSEMBLE_FORECAST_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-forecast-time-series-ptr)**  |
|  | **[ENSEMBLE_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-time-series-ptr)**  |
|  | **[ENSEMBLE_PTR_TIME_SERIES_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-ensemble-ptr-time-series-ptr)**  |
|  | **[TIME_SERIES_PROVIDER_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__as__transparent_8h/#define-time-series-provider-ptr)**  |




## Macros Documentation

### define TIME_SERIES_PTR

```cpp
#define TIME_SERIES_PTR TIME_SERIES_TRANSPARENT_PTR
```


### define ENSEMBLE_DATA_SET_PTR

```cpp
#define ENSEMBLE_DATA_SET_PTR ENSEMBLE_DATA_SET_TRANSPARENT_PTR
```


### define ENSEMBLE_FORECAST_TIME_SERIES_PTR

```cpp
#define ENSEMBLE_FORECAST_TIME_SERIES_PTR ENSEMBLE_FORECAST_TIME_SERIES_TRANSPARENT_PTR
```


### define ENSEMBLE_TIME_SERIES_PTR

```cpp
#define ENSEMBLE_TIME_SERIES_PTR ENSEMBLE_TIME_SERIES_TRANSPARENT_PTR
```


### define ENSEMBLE_PTR_TIME_SERIES_PTR

```cpp
#define ENSEMBLE_PTR_TIME_SERIES_PTR ENSEMBLE_PTR_TIME_SERIES_TRANSPARENT_PTR
```


### define TIME_SERIES_PROVIDER_PTR

```cpp
#define TIME_SERIES_PROVIDER_PTR TIME_SERIES_PROVIDER_TRANSPARENT_PTR
```


## Source code

```cpp
#pragma once

#include "moirai/extern_c_api_as_transparent.h"
#include "extern_c_api_transparent_pointers.h"

#define TIME_SERIES_PTR                         TIME_SERIES_TRANSPARENT_PTR
#define ENSEMBLE_DATA_SET_PTR                   ENSEMBLE_DATA_SET_TRANSPARENT_PTR 
#define ENSEMBLE_FORECAST_TIME_SERIES_PTR       ENSEMBLE_FORECAST_TIME_SERIES_TRANSPARENT_PTR             
#define ENSEMBLE_TIME_SERIES_PTR                ENSEMBLE_TIME_SERIES_TRANSPARENT_PTR    
#define ENSEMBLE_PTR_TIME_SERIES_PTR            ENSEMBLE_PTR_TIME_SERIES_TRANSPARENT_PTR    
#define TIME_SERIES_PROVIDER_PTR                TIME_SERIES_PROVIDER_TRANSPARENT_PTR    
```


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000
