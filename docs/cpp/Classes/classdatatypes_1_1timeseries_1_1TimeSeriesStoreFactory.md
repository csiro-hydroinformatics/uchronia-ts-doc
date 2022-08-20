---
title: datatypes::timeseries::TimeSeriesStoreFactory

---

# datatypes::timeseries::TimeSeriesStoreFactory






`#include <time_series_store.hpp>`

Inherited by [datatypes::tests::TestTimeSeriesStoreFactory](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesStoreFactory/), [datatypes::timeseries::SwiftNetcdfStoreFactory](/cpp/Classes/classdatatypes_1_1timeseries_1_1SwiftNetcdfStoreFactory/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeSeriesStoreFactory](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/#function-~timeseriesstorefactory)**() |
| virtual [TimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)< double > * | **[CreateTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/#function-createtimeseriesensembletimeseriesstore)**(const string & dataId) =0 |
| virtual bool | **[CanCreateTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/#function-cancreatetimeseriesensembletimeseriesstore)**(const string & dataId) =0 |

## Protected Functions

|                | Name           |
| -------------- | -------------- |
| | **[TimeSeriesStoreFactory](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/#function-timeseriesstorefactory)**() |

## Public Functions Documentation

### function ~TimeSeriesStoreFactory

```cpp
virtual ~TimeSeriesStoreFactory()
```


### function CreateTimeSeriesEnsembleTimeSeriesStore

```cpp
virtual TimeSeriesEnsembleTimeSeriesStore< double > * CreateTimeSeriesEnsembleTimeSeriesStore(
    const string & dataId
) =0
```


**Reimplemented by**: [datatypes::tests::TestTimeSeriesStoreFactory::CreateTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesStoreFactory/#function-createtimeseriesensembletimeseriesstore), [datatypes::timeseries::SwiftNetcdfStoreFactory::CreateTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1SwiftNetcdfStoreFactory/#function-createtimeseriesensembletimeseriesstore)


### function CanCreateTimeSeriesEnsembleTimeSeriesStore

```cpp
virtual bool CanCreateTimeSeriesEnsembleTimeSeriesStore(
    const string & dataId
) =0
```


**Reimplemented by**: [datatypes::tests::TestTimeSeriesStoreFactory::CanCreateTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesStoreFactory/#function-cancreatetimeseriesensembletimeseriesstore), [datatypes::timeseries::SwiftNetcdfStoreFactory::CanCreateTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1SwiftNetcdfStoreFactory/#function-cancreatetimeseriesensembletimeseriesstore)


## Protected Functions Documentation

### function TimeSeriesStoreFactory

```cpp
TimeSeriesStoreFactory()
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000