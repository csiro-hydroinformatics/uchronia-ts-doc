---
title: datatypes::timeseries::SwiftNetcdfStoreFactory

---

# datatypes::timeseries::SwiftNetcdfStoreFactory






`#include <time_series_io.hpp>`

Inherits from [datatypes::timeseries::TimeSeriesStoreFactory](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[SwiftNetcdfStoreFactory](/cpp/Classes/classdatatypes_1_1timeseries_1_1SwiftNetcdfStoreFactory/#function-swiftnetcdfstorefactory)**(const string & path, [DataGeometryProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataGeometryProvider/) * dgp) |
| | **[~SwiftNetcdfStoreFactory](/cpp/Classes/classdatatypes_1_1timeseries_1_1SwiftNetcdfStoreFactory/#function-~swiftnetcdfstorefactory)**() |
| virtual [TimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)< double > * | **[CreateTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1SwiftNetcdfStoreFactory/#function-createtimeseriesensembletimeseriesstore)**(const string & dataId) |
| virtual bool | **[CanCreateTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1SwiftNetcdfStoreFactory/#function-cancreatetimeseriesensembletimeseriesstore)**(const string & dataId) |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::TimeSeriesStoreFactory](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeSeriesStoreFactory](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/#function-~timeseriesstorefactory)**() |

**Protected Functions inherited from [datatypes::timeseries::TimeSeriesStoreFactory](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/)**

|                | Name           |
| -------------- | -------------- |
| | **[TimeSeriesStoreFactory](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/#function-timeseriesstorefactory)**() |


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


**Reimplements**: [datatypes::timeseries::TimeSeriesStoreFactory::CreateTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/#function-createtimeseriesensembletimeseriesstore)


### function CanCreateTimeSeriesEnsembleTimeSeriesStore

```cpp
virtual bool CanCreateTimeSeriesEnsembleTimeSeriesStore(
    const string & dataId
)
```


**Reimplements**: [datatypes::timeseries::TimeSeriesStoreFactory::CanCreateTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/#function-cancreatetimeseriesensembletimeseriesstore)


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000