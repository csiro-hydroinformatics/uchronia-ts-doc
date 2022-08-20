---
title: datatypes::tests::TestEnsembleTimeSeriesStore

---

# datatypes::tests::TestEnsembleTimeSeriesStore






`#include <datatypes_test_helpers.h>`

Inherits from [datatypes::timeseries::EnsembleTimeSeriesStore< double >](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/), [datatypes::timeseries::IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/), [datatypes::timeseries::DataDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[TestEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1tests_1_1TestEnsembleTimeSeriesStore/#function-testensembletimeseriesstore)**(const [MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)<> & data) |
| virtual [MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< double > * > * | **[Read](/cpp/Classes/classdatatypes_1_1tests_1_1TestEnsembleTimeSeriesStore/#function-read)**() |
| virtual string | **[GetDataSummary](/cpp/Classes/classdatatypes_1_1tests_1_1TestEnsembleTimeSeriesStore/#function-getdatasummary)**() const |
| virtual vector< [DataDimensionDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) > | **[GetDataDimensionsDescription](/cpp/Classes/classdatatypes_1_1tests_1_1TestEnsembleTimeSeriesStore/#function-getdatadimensionsdescription)**() const |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::EnsembleTimeSeriesStore< double >](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~EnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/#function-~ensembletimeseriesstore)**() |
| virtual vector< string > | **[GetIdentifiers](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/#function-getidentifiers)**() const |

**Public Functions inherited from [datatypes::timeseries::IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-~identifiersprovider)**() |
| virtual vector< string > | **[GetIdentifiers](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-getidentifiers)**() const =0 |
| vector< string > | **[SplitHierarchicalIdentifier](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-splithierarchicalidentifier)**(const string & longId) |
| string | **[GetTopmostIdentifier](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-gettopmostidentifier)**(const string & longId) |
| void | **[CheckNotEmpty](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-checknotempty)**(const string & longId) |


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


**Reimplements**: [datatypes::timeseries::EnsembleTimeSeriesStore::Read](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/#function-read)


### function GetDataSummary

```cpp
virtual string GetDataSummary() const
```


**Reimplements**: [datatypes::timeseries::DataDescriptor::GetDataSummary](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatasummary)


### function GetDataDimensionsDescription

```cpp
virtual vector< DataDimensionDescriptor > GetDataDimensionsDescription() const
```


**Reimplements**: [datatypes::timeseries::DataDescriptor::GetDataDimensionsDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatadimensionsdescription)


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000