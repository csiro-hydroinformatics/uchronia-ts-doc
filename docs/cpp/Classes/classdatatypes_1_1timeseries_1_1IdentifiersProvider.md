---
title: datatypes::timeseries::IdentifiersProvider
summary: An interface definition for objects that can provide hierarchical identification. 

---

# datatypes::timeseries::IdentifiersProvider



An interface definition for objects that can provide hierarchical identification.  [More...](#detailed-description)


`#include <time_series_store.hpp>`

Inherited by [datatypes::timeseries::EnsembleTimeSeriesStore< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/), [datatypes::timeseries::SingleTimeSeriesStore< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/), [datatypes::timeseries::TimeSeriesProvider< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesProvider/), [datatypes::timeseries::EnsembleTimeSeriesStore< T >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/), [datatypes::timeseries::SingleTimeSeriesStore< T >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/), [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore< T >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/), [datatypes::timeseries::TimeSeriesProvider< T >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesProvider/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual | **[~IdentifiersProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-~identifiersprovider)**() |
| virtual vector< string > | **[GetIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-getidentifiers)**() const =0 |
| vector< string > | **[SplitHierarchicalIdentifier](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-splithierarchicalidentifier)**(const string & longId) |
| string | **[GetTopmostIdentifier](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-gettopmostidentifier)**(const string & longId) |
| void | **[CheckNotEmpty](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-checknotempty)**(const string & longId) |

## Detailed Description

```cpp
class datatypes::timeseries::IdentifiersProvider;
```

An interface definition for objects that can provide hierarchical identification. 



```
    A parent class for objects that can provide hierarchical identification. 
    For instance a dot-separated identification scheme such as "category.subcatcgory.catchment.instant_flow"
```

## Public Functions Documentation

### function ~IdentifiersProvider

```cpp
inline virtual ~IdentifiersProvider()
```


### function GetIdentifiers

```cpp
virtual vector< string > GetIdentifiers() const =0
```


**Reimplemented by**: [datatypes::tests::TestSingleTimeSeriesStore::GetIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/#function-getidentifiers), [datatypes::timeseries::NetCdfSingleSeriesStore::GetIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-getidentifiers), [datatypes::timeseries::NetCdfEnsembleTimeSeriesStore::GetIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfEnsembleTimeSeriesStore/#function-getidentifiers), [datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore::GetIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-getidentifiers), [datatypes::timeseries::EnsembleTimeSeriesStore::GetIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/#function-getidentifiers), [datatypes::timeseries::EnsembleTimeSeriesStore::GetIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/#function-getidentifiers), [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getidentifiers), [datatypes::timeseries::TimeSeriesLibrary::GetIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-getidentifiers)


### function SplitHierarchicalIdentifier

```cpp
static vector< string > SplitHierarchicalIdentifier(
    const string & longId
)
```


### function GetTopmostIdentifier

```cpp
static string GetTopmostIdentifier(
    const string & longId
)
```


### function CheckNotEmpty

```cpp
static void CheckNotEmpty(
    const string & longId
)
```


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000