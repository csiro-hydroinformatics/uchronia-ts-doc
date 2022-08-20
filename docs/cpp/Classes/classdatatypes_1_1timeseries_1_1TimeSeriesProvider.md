---
title: datatypes::timeseries::TimeSeriesProvider
summary: Library of time series, for high level access to sources of univariate, single instance time series that may have varying on-disk representations. 

---

# datatypes::timeseries::TimeSeriesProvider



Library of time series, for high level access to sources of univariate, single instance time series that may have varying on-disk representations.  [More...](#detailed-description)


`#include <time_series_store.hpp>`

Inherits from [datatypes::timeseries::IdentifiersProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeSeriesProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesProvider/#function-~timeseriesprovider)**() |
| virtual [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > * | **[GetSingle](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesProvider/#function-getsingle)**(const string & dataId) =0<br>Gets a single time series out of the library.  |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::IdentifiersProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~IdentifiersProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-~identifiersprovider)**() |
| virtual vector< string > | **[GetIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-getidentifiers)**() const =0 |
| vector< string > | **[SplitHierarchicalIdentifier](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-splithierarchicalidentifier)**(const string & longId) |
| string | **[GetTopmostIdentifier](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-gettopmostidentifier)**(const string & longId) |
| void | **[CheckNotEmpty](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-checknotempty)**(const string & longId) |


## Detailed Description

```cpp
template <typename T >
class datatypes::timeseries::TimeSeriesProvider;
```

Library of time series, for high level access to sources of univariate, single instance time series that may have varying on-disk representations. 

**Template Parameters**: 

  * **T** The element type of the time series dealt with, typically double or float. 

## Public Functions Documentation

### function ~TimeSeriesProvider

```cpp
inline virtual ~TimeSeriesProvider()
```


### function GetSingle

```cpp
virtual TTimeSeries< T > * GetSingle(
    const string & dataId
) =0
```

Gets a single time series out of the library. 

**Parameters**: 

  * **dataId** Identifier for the time series


**Return**: The univariate, single realization time series 

**Reimplemented by**: [datatypes::timeseries::TimeSeriesLibrary::GetSingle](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-getsingle)


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000