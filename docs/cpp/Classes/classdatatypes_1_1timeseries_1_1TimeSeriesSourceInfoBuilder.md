---
title: datatypes::timeseries::TimeSeriesSourceInfoBuilder
summary: An abstract class to allow callers to inject custom time series data sources into a time series library. 

---

# datatypes::timeseries::TimeSeriesSourceInfoBuilder



An abstract class to allow callers to inject custom time series data sources into a time series library. 


`#include <time_series_store.hpp>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual bool | **[HandlesStorageType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoBuilder/#function-handlesstoragetype)**(const string storageType) const =0 |
| virtual void | **[BuildTimeSeriesSource](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoBuilder/#function-buildtimeseriessource)**(const string & storageType, const string & dataId, const YAML::Node & storage, [TimeSeriesLibraryDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/) & targetContainer) const =0 |

## Public Functions Documentation

### function HandlesStorageType

```cpp
virtual bool HandlesStorageType(
    const string storageType
) const =0
```


### function BuildTimeSeriesSource

```cpp
virtual void BuildTimeSeriesSource(
    const string & storageType,
    const string & dataId,
    const YAML::Node & storage,
    TimeSeriesLibraryDescription & targetContainer
) const =0
```


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000