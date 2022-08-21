---
title: datatypes::tests::TestEnsembleTimeSeriesStore

---

# datatypes::tests::TestEnsembleTimeSeriesStore






`#include <datatypes_test_helpers.h>`

Inherits from [datatypes::timeseries::EnsembleTimeSeriesStore< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/), [datatypes::timeseries::IdentifiersProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/), [datatypes::timeseries::DataDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[TestEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestEnsembleTimeSeriesStore/#function-testensembletimeseriesstore)**(const [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)<> & data) |
| virtual [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< double > * > * | **[Read](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestEnsembleTimeSeriesStore/#function-read)**() |
| virtual string | **[GetDataSummary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestEnsembleTimeSeriesStore/#function-getdatasummary)**() const |
| virtual vector< [DataDimensionDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) > | **[GetDataDimensionsDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestEnsembleTimeSeriesStore/#function-getdatadimensionsdescription)**() const |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::EnsembleTimeSeriesStore< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~EnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/#function-~ensembletimeseriesstore)**() |
| virtual vector< string > | **[GetIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/#function-getidentifiers)**() const |

**Public Functions inherited from [datatypes::timeseries::IdentifiersProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~IdentifiersProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-~identifiersprovider)**() |
| virtual vector< string > | **[GetIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-getidentifiers)**() const =0 |
| vector< string > | **[SplitHierarchicalIdentifier](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-splithierarchicalidentifier)**(const string & longId) |
| string | **[GetTopmostIdentifier](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-gettopmostidentifier)**(const string & longId) |
| void | **[CheckNotEmpty](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-checknotempty)**(const string & longId) |


## Public Functions Documentation

### function TestEnsembleTimeSeriesStore

```cpp
TestEnsembleTimeSeriesStore(
    const MultiTimeSeries<> & data
)
```


### function Read

```cpp
virtual MultiTimeSeries< TTimeSeries< double > * > * Read()
```


**Reimplements**: [datatypes::timeseries::EnsembleTimeSeriesStore::Read](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/#function-read)


### function GetDataSummary

```cpp
virtual string GetDataSummary() const
```


**Reimplements**: [datatypes::timeseries::DataDescriptor::GetDataSummary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatasummary)


### function GetDataDimensionsDescription

```cpp
virtual vector< DataDimensionDescriptor > GetDataDimensionsDescription() const
```


**Reimplements**: [datatypes::timeseries::DataDescriptor::GetDataDimensionsDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatadimensionsdescription)


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000