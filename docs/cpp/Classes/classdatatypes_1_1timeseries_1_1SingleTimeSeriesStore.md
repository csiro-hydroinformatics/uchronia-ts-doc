---
title: datatypes::timeseries::SingleTimeSeriesStore
summary: Interface definition for storages of single, univariate time series. 

---

# datatypes::timeseries::SingleTimeSeriesStore



Interface definition for storages of single, univariate time series.  [More...](#detailed-description)


`#include <time_series_store.hpp>`

Inherits from [datatypes::timeseries::IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/), [datatypes::timeseries::DataDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/)

Inherited by [datatypes::timeseries::NetCdfSingleSeriesStore< T >](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual | **[~SingleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/#function-~singletimeseriesstore)**() |
| virtual [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > * | **[Read](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/#function-read)**() =0 |
| virtual [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > * | **[Read](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/#function-read)**(const string & collectionIdentifier) =0 |
| virtual [MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > * > * | **[ReadAllCollection](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/#function-readallcollection)**() =0 |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-~identifiersprovider)**() |
| virtual vector< string > | **[GetIdentifiers](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-getidentifiers)**() const =0 |
| vector< string > | **[SplitHierarchicalIdentifier](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-splithierarchicalidentifier)**(const string & longId) |
| string | **[GetTopmostIdentifier](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-gettopmostidentifier)**(const string & longId) |
| void | **[CheckNotEmpty](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-checknotempty)**(const string & longId) |

**Public Functions inherited from [datatypes::timeseries::DataDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/)**

|                | Name           |
| -------------- | -------------- |
| virtual string | **[GetDataSummary](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatasummary)**() const =0 |
| virtual vector< [DataDimensionDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) > | **[GetDataDimensionsDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatadimensionsdescription)**() const =0 |


## Detailed Description

```cpp
template <typename T >
class datatypes::timeseries::SingleTimeSeriesStore;
```

Interface definition for storages of single, univariate time series. 

**Template Parameters**: 

  * **T** The element type of the time series dealt with, typically double or float. 

## Public Functions Documentation

### function ~SingleTimeSeriesStore

```cpp
inline virtual ~SingleTimeSeriesStore()
```


### function Read

```cpp
virtual TTimeSeries< T > * Read() =0
```


**Reimplemented by**: [datatypes::tests::TestSingleTimeSeriesStore::Read](/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/#function-read), [datatypes::timeseries::NetCdfSingleSeriesStore::Read](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-read)


### function Read

```cpp
virtual TTimeSeries< T > * Read(
    const string & collectionIdentifier
) =0
```


**Reimplemented by**: [datatypes::tests::TestSingleTimeSeriesStore::Read](/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/#function-read), [datatypes::timeseries::NetCdfSingleSeriesStore::Read](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-read)


### function ReadAllCollection

```cpp
virtual MultiTimeSeries< TTimeSeries< T > * > * ReadAllCollection() =0
```


**Reimplemented by**: [datatypes::tests::TestSingleTimeSeriesStore::ReadAllCollection](/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/#function-readallcollection), [datatypes::timeseries::NetCdfSingleSeriesStore::ReadAllCollection](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-readallcollection)


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000