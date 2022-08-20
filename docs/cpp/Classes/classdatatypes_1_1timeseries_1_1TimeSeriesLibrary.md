---
title: datatypes::timeseries::TimeSeriesLibrary
summary: Library of time series, for high level access to sources of time series that nmay have varying on-disk representations. 

---

# datatypes::timeseries::TimeSeriesLibrary



Library of time series, for high level access to sources of time series that nmay have varying on-disk representations.  [More...](#detailed-description)


`#include <time_series_store.hpp>`

Inherits from [datatypes::timeseries::TimeSeriesProvider< double >](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesProvider/), [datatypes::timeseries::TTimeSeriesLibrary< double >](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/), [datatypes::timeseries::IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[TimeSeriesLibrary](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-timeserieslibrary)**([TimeSeriesStoreFactory](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/) * storeCreator =nullptr) |
| | **[TimeSeriesLibrary](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-timeserieslibrary)**(const [TimeSeriesLibraryDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/) & description) |
| virtual | **[~TimeSeriesLibrary](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-~timeserieslibrary)**() |
| void | **[Close](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-close)**() |
| [TimeSeriesLibrary](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/) & | **[operator=](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-operator=)**([TimeSeriesLibrary](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/) && src) |
| | **[TimeSeriesLibrary](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-timeserieslibrary)**([TimeSeriesLibrary](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/) && src)<br>Constructor using the move semantics.  |
| [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< double > * | **[GetSingle](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-getsingle)**(const string & dataId, boost::function< [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< double > *([TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< double > *)> & tsTransform)<br>Gets a single time series out of the library.  |
| virtual vector< string > | **[GetIdentifiers](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-getidentifiers)**() const |
| vector< string > | **[GetIdentifiers](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-getidentifiers)**(const string & dataId) const |
| string | **[GetDataSummary](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-getdatasummary)**(const string & dataId) |
| vector< [DataDimensionDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) > | **[GetDataDimensionsDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-getdatadimensionsdescription)**(const string & dataId) |
| virtual [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< double > * | **[GetSingle](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-getsingle)**(const string & dataId)<br>Gets a single time series out of the library.  |
| virtual [MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< double > * > * | **[GetCollection](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-getcollection)**(const string & dataId)<br>Gets a collection of time series out of the library, where each item is for a given station ID.  |
| virtual [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< double > * | **[GetSingle](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-getsingle)**(const string & dataId, const string & collectionIdentifier)<br>**  |
| [MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< double > * > * | **[GetEnsemble](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-getensemble)**(const string & dataId, const string & dataItemIdentifier) |
| virtual [MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< double > * > * | **[GetEnsembleTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-getensembletimeseries)**(const string & dataId) |
| virtual [MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< double > * > * | **[GetAllTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-getalltimeseries)**(const string & dataId) |
| virtual [EnsembleForecastTimeSeries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-ensembleforecasttimeseries)< [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< double > > * | **[GetTimeSeriesEnsembleTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-gettimeseriesensembletimeseries)**(const string & dataId) |
| void | **[AddSource](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-addsource)**(const string & dataId, [SingleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/)< double > * store) |
| void | **[AddSource](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-addsource)**(const string & dataId, [EnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/)< double > * store) |
| void | **[AddSource](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-addsource)**(const string & dataId, [TimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)< double > * dataAccess) |
| bool | **[CanCreateTimeSeriesEnsembleSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-cancreatetimeseriesensembleseriesstore)**(const string & dataId) |
| void | **[CreateTimeSeriesEnsembleSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-createtimeseriesensembleseriesstore)**(const string & dataId) |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::TimeSeriesProvider< double >](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesProvider/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeSeriesProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesProvider/#function-~timeseriesprovider)**() |

**Public Types inherited from [datatypes::timeseries::TTimeSeriesLibrary< double >](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/)**

|                | Name           |
| -------------- | -------------- |
| typedef [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > | **[TS](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#typedef-ts)**  |
| typedef [MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [TS](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#typedef-ts) * > | **[MTS](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#typedef-mts)**  |

**Public Functions inherited from [datatypes::timeseries::TTimeSeriesLibrary< double >](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TTimeSeriesLibrary](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#function-~ttimeserieslibrary)**() |
| virtual [TimeSeriesProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesProvider/)< T > * | **[GetProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#function-getprovider)**(const string & dataId) |

**Public Functions inherited from [datatypes::timeseries::IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-~identifiersprovider)**() |
| vector< string > | **[SplitHierarchicalIdentifier](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-splithierarchicalidentifier)**(const string & longId) |
| string | **[GetTopmostIdentifier](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-gettopmostidentifier)**(const string & longId) |
| void | **[CheckNotEmpty](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-checknotempty)**(const string & longId) |


## Detailed Description

```cpp
class datatypes::timeseries::TimeSeriesLibrary;
```

Library of time series, for high level access to sources of time series that nmay have varying on-disk representations. 

**Template Parameters**: 

  * **T** The element type of the time series dealt with, typically double or float. 

## Public Functions Documentation

### function TimeSeriesLibrary

```cpp
TimeSeriesLibrary(
    TimeSeriesStoreFactory * storeCreator =nullptr
)
```


### function TimeSeriesLibrary

```cpp
TimeSeriesLibrary(
    const TimeSeriesLibraryDescription & description
)
```


### function ~TimeSeriesLibrary

```cpp
virtual ~TimeSeriesLibrary()
```


### function Close

```cpp
void Close()
```


### function operator=

```cpp
TimeSeriesLibrary & operator=(
    TimeSeriesLibrary && src
)
```


### function TimeSeriesLibrary

```cpp
TimeSeriesLibrary(
    TimeSeriesLibrary && src
)
```

Constructor using the move semantics. 

**Parameters**: 

  * **src** time series library from which to move data. 


**Remark**: C++ for the Impatient Appendix A. A Painless Introduction to Rvalue References (C++11) See also [http://stackoverflow.com/a/3109981/2752565](http://stackoverflow.com/a/3109981/2752565) for information on move semantic 

### function GetSingle

```cpp
TTimeSeries< double > * GetSingle(
    const string & dataId,
    boost::function< TTimeSeries< double > *(TTimeSeries< double > *)> & tsTransform
)
```

Gets a single time series out of the library. 

**Parameters**: 

  * **dataId** Identifier for the time series 
  * **tsTransform** If non-null, a time series transformation to perform on the raw data retrieved for dataId.


**Return**: The univariate, single realization time series 

### function GetIdentifiers

```cpp
virtual vector< string > GetIdentifiers() const
```


**Reimplements**: [datatypes::timeseries::TTimeSeriesLibrary::GetIdentifiers](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#function-getidentifiers)


### function GetIdentifiers

```cpp
vector< string > GetIdentifiers(
    const string & dataId
) const
```


### function GetDataSummary

```cpp
string GetDataSummary(
    const string & dataId
)
```


### function GetDataDimensionsDescription

```cpp
vector< DataDimensionDescriptor > GetDataDimensionsDescription(
    const string & dataId
)
```


### function GetSingle

```cpp
virtual TTimeSeries< double > * GetSingle(
    const string & dataId
)
```

Gets a single time series out of the library. 

**Parameters**: 

  * **dataId** Identifier for the time series


**Return**: The univariate, single realization time series 

**Reimplements**: [datatypes::timeseries::TimeSeriesProvider::GetSingle](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesProvider/#function-getsingle)


### function GetCollection

```cpp
virtual MultiTimeSeries< TTimeSeries< double > * > * GetCollection(
    const string & dataId
)
```

Gets a collection of time series out of the library, where each item is for a given station ID. 

**Parameters**: 

  * **dataId** Identifier for the time series


**Return**: The collection of univariate, single realization time series 

**Reimplements**: [datatypes::timeseries::TTimeSeriesLibrary::GetCollection](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#function-getcollection)


### function GetSingle

```cpp
virtual TTimeSeries< double > * GetSingle(
    const string & dataId,
    const string & collectionIdentifier
)
```

** 

**Parameters**: 

  * **dataId** Identifier for the collection of time series 
  * **collectionIdentifier** Identifier for the item to retrieve in the collection. Typically, a station identifier


**Return**: The univariate, single realization time series 

**Reimplements**: [datatypes::timeseries::TTimeSeriesLibrary::GetSingle](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#function-getsingle)


Gets a single time series out of the library


### function GetEnsemble

```cpp
MultiTimeSeries< TTimeSeries< double > * > * GetEnsemble(
    const string & dataId,
    const string & dataItemIdentifier
)
```


### function GetEnsembleTimeSeries

```cpp
virtual MultiTimeSeries< TTimeSeries< double > * > * GetEnsembleTimeSeries(
    const string & dataId
)
```


**Reimplements**: [datatypes::timeseries::TTimeSeriesLibrary::GetEnsembleTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#function-getensembletimeseries)


### function GetAllTimeSeries

```cpp
virtual MultiTimeSeries< TTimeSeries< double > * > * GetAllTimeSeries(
    const string & dataId
)
```


**Reimplements**: [datatypes::timeseries::TTimeSeriesLibrary::GetAllTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#function-getalltimeseries)


### function GetTimeSeriesEnsembleTimeSeries

```cpp
virtual EnsembleForecastTimeSeries< TTimeSeries< double > > * GetTimeSeriesEnsembleTimeSeries(
    const string & dataId
)
```


**Reimplements**: [datatypes::timeseries::TTimeSeriesLibrary::GetTimeSeriesEnsembleTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#function-gettimeseriesensembletimeseries)


### function AddSource

```cpp
void AddSource(
    const string & dataId,
    SingleTimeSeriesStore< double > * store
)
```


### function AddSource

```cpp
void AddSource(
    const string & dataId,
    EnsembleTimeSeriesStore< double > * store
)
```


### function AddSource

```cpp
void AddSource(
    const string & dataId,
    TimeSeriesEnsembleTimeSeriesStore< double > * dataAccess
)
```


### function CanCreateTimeSeriesEnsembleSeriesStore

```cpp
bool CanCreateTimeSeriesEnsembleSeriesStore(
    const string & dataId
)
```


### function CreateTimeSeriesEnsembleSeriesStore

```cpp
void CreateTimeSeriesEnsembleSeriesStore(
    const string & dataId
)
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000