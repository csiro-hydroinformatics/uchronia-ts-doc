---
title: datatypes::tests::TestSingleTimeSeriesStore

---

# datatypes::tests::TestSingleTimeSeriesStore






`#include <datatypes_test_helpers.h>`

Inherits from [datatypes::timeseries::SingleTimeSeriesStore< double >](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/), [datatypes::timeseries::IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/), [datatypes::timeseries::DataDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[TestSingleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/#function-testsingletimeseriesstore)**(const vector< double > & values, const ptime & startDate, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =TimeStep::GetHourly()) |
| | **[TestSingleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/#function-testsingletimeseriesstore)**(const [TimeSeries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) & series) |
| virtual string | **[GetDataSummary](/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/#function-getdatasummary)**() const |
| virtual vector< [DataDimensionDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) > | **[GetDataDimensionsDescription](/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/#function-getdatadimensionsdescription)**() const |
| virtual [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< double > * | **[Read](/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/#function-read)**() |
| virtual [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< double > * | **[Read](/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/#function-read)**(const string & blah) |
| virtual [MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< double > * > * | **[ReadAllCollection](/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/#function-readallcollection)**() |
| virtual std::vector< std::string > | **[GetIdentifiers](/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/#function-getidentifiers)**() const |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::SingleTimeSeriesStore< double >](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~SingleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/#function-~singletimeseriesstore)**() |

**Public Functions inherited from [datatypes::timeseries::IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-~identifiersprovider)**() |
| vector< string > | **[SplitHierarchicalIdentifier](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-splithierarchicalidentifier)**(const string & longId) |
| string | **[GetTopmostIdentifier](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-gettopmostidentifier)**(const string & longId) |
| void | **[CheckNotEmpty](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-checknotempty)**(const string & longId) |


## Public Functions Documentation

### function TestSingleTimeSeriesStore

```cpp
TestSingleTimeSeriesStore(
    const vector< double > & values,
    const ptime & startDate,
    const TimeStep & timeStep =TimeStep::GetHourly()
)
```


### function TestSingleTimeSeriesStore

```cpp
TestSingleTimeSeriesStore(
    const TimeSeries & series
)
```


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


### function Read

```cpp
virtual TTimeSeries< double > * Read()
```


**Reimplements**: [datatypes::timeseries::SingleTimeSeriesStore::Read](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/#function-read)


### function Read

```cpp
virtual TTimeSeries< double > * Read(
    const string & blah
)
```


**Reimplements**: [datatypes::timeseries::SingleTimeSeriesStore::Read](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/#function-read)


### function ReadAllCollection

```cpp
virtual MultiTimeSeries< TTimeSeries< double > * > * ReadAllCollection()
```


**Reimplements**: [datatypes::timeseries::SingleTimeSeriesStore::ReadAllCollection](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/#function-readallcollection)


### function GetIdentifiers

```cpp
virtual std::vector< std::string > GetIdentifiers() const
```


**Reimplements**: [datatypes::timeseries::IdentifiersProvider::GetIdentifiers](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-getidentifiers)


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000