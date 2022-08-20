---
title: datatypes::tests::TestTimeSeriesStoreFactory

---

# datatypes::tests::TestTimeSeriesStoreFactory






`#include <datatypes_test_helpers.h>`

Inherits from [datatypes::timeseries::TimeSeriesStoreFactory](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[TestTimeSeriesStoreFactory](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesStoreFactory/#function-testtimeseriesstorefactory)**() |
| | **[~TestTimeSeriesStoreFactory](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesStoreFactory/#function-~testtimeseriesstorefactory)**() |
| virtual [TimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)< double > * | **[CreateTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesStoreFactory/#function-createtimeseriesensembletimeseriesstore)**(const string & dataId) |
| virtual bool | **[CanCreateTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesStoreFactory/#function-cancreatetimeseriesensembletimeseriesstore)**(const string & dataId) |

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

### function TestTimeSeriesStoreFactory

```cpp
TestTimeSeriesStoreFactory()
```


### function ~TestTimeSeriesStoreFactory

```cpp
~TestTimeSeriesStoreFactory()
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

Updated on 2022-08-20 at 19:28:22 +1000