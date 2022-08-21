---
title: datatypes::timeseries::SwiftNetcdfStoreFactory

---

# datatypes::timeseries::SwiftNetcdfStoreFactory






`#include <time_series_io.hpp>`

Inherits from [datatypes::timeseries::TimeSeriesStoreFactory](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[SwiftNetcdfStoreFactory](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SwiftNetcdfStoreFactory/#function-swiftnetcdfstorefactory)**(const string & path, [DataGeometryProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataGeometryProvider/) * dgp) |
| | **[~SwiftNetcdfStoreFactory](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SwiftNetcdfStoreFactory/#function-~swiftnetcdfstorefactory)**() |
| virtual [TimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)< double > * | **[CreateTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SwiftNetcdfStoreFactory/#function-createtimeseriesensembletimeseriesstore)**(const string & dataId) |
| virtual bool | **[CanCreateTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SwiftNetcdfStoreFactory/#function-cancreatetimeseriesensembletimeseriesstore)**(const string & dataId) |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::TimeSeriesStoreFactory](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeSeriesStoreFactory](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/#function-~timeseriesstorefactory)**() |

**Protected Functions inherited from [datatypes::timeseries::TimeSeriesStoreFactory](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/)**

|                | Name           |
| -------------- | -------------- |
| | **[TimeSeriesStoreFactory](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/#function-timeseriesstorefactory)**() |


## Public Functions Documentation

### function SwiftNetcdfStoreFactory

```cpp
SwiftNetcdfStoreFactory(
    const string & path,
    DataGeometryProvider * dgp
)
```


### function ~SwiftNetcdfStoreFactory

```cpp
~SwiftNetcdfStoreFactory()
```


### function CreateTimeSeriesEnsembleTimeSeriesStore

```cpp
virtual TimeSeriesEnsembleTimeSeriesStore< double > * CreateTimeSeriesEnsembleTimeSeriesStore(
    const string & dataId
)
```


**Reimplements**: [datatypes::timeseries::TimeSeriesStoreFactory::CreateTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/#function-createtimeseriesensembletimeseriesstore)


### function CanCreateTimeSeriesEnsembleTimeSeriesStore

```cpp
virtual bool CanCreateTimeSeriesEnsembleTimeSeriesStore(
    const string & dataId
)
```


**Reimplements**: [datatypes::timeseries::TimeSeriesStoreFactory::CanCreateTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/#function-cancreatetimeseriesensembletimeseriesstore)


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000