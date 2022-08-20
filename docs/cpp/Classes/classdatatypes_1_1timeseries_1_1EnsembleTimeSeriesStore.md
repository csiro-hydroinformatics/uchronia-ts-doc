---
title: datatypes::timeseries::EnsembleTimeSeriesStore
summary: Interface definition for storages of ensembles of univariate time series. 

---

# datatypes::timeseries::EnsembleTimeSeriesStore



Interface definition for storages of ensembles of univariate time series.  [More...](#detailed-description)


`#include <time_series_store.hpp>`

Inherits from [datatypes::timeseries::IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/), [datatypes::timeseries::DataDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/)

Inherited by [datatypes::timeseries::NetCdfEnsembleTimeSeriesStore< T >](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfEnsembleTimeSeriesStore/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual | **[~EnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/#function-~ensembletimeseriesstore)**() |
| virtual [MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > * > * | **[Read](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/#function-read)**() =0 |
| virtual vector< string > | **[GetIdentifiers](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/#function-getidentifiers)**() const |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-~identifiersprovider)**() |
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
class datatypes::timeseries::EnsembleTimeSeriesStore;
```

Interface definition for storages of ensembles of univariate time series. 

**Template Parameters**: 

  * **T** The element type of the time series dealt with, typically double or float. 

## Public Functions Documentation

### function ~EnsembleTimeSeriesStore

```cpp
inline virtual ~EnsembleTimeSeriesStore()
```


### function Read

```cpp
virtual MultiTimeSeries< TTimeSeries< T > * > * Read() =0
```


**Reimplemented by**: [datatypes::tests::TestEnsembleTimeSeriesStore::Read](/cpp/Classes/classdatatypes_1_1tests_1_1TestEnsembleTimeSeriesStore/#function-read), [datatypes::timeseries::NetCdfEnsembleTimeSeriesStore::Read](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfEnsembleTimeSeriesStore/#function-read)


### function GetIdentifiers

```cpp
inline virtual vector< string > GetIdentifiers() const
```


**Reimplements**: [datatypes::timeseries::IdentifiersProvider::GetIdentifiers](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-getidentifiers)


**Reimplemented by**: [datatypes::timeseries::NetCdfEnsembleTimeSeriesStore::GetIdentifiers](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfEnsembleTimeSeriesStore/#function-getidentifiers)


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000