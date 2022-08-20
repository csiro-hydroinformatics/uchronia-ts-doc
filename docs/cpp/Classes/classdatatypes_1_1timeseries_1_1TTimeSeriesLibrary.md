---
title: datatypes::timeseries::TTimeSeriesLibrary

---

# datatypes::timeseries::TTimeSeriesLibrary



 [More...](#detailed-description)


`#include <time_series_store.hpp>`

## Public Types

|                | Name           |
| -------------- | -------------- |
| typedef [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > | **[TS](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#typedef-ts)**  |
| typedef [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [TS](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#typedef-ts) * > | **[MTS](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#typedef-mts)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TTimeSeriesLibrary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#function-~ttimeserieslibrary)**() |
| virtual [TS](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#typedef-ts) * | **[GetSingle](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#function-getsingle)**(const string & dataId) |
| virtual [TS](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#typedef-ts) * | **[GetSingle](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#function-getsingle)**(const string & dataId, const string & collectionIdentifier) |
| virtual [MTS](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#typedef-mts) * | **[GetCollection](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#function-getcollection)**(const string & dataId) |
| virtual [TimeSeriesProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesProvider/)< T > * | **[GetProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#function-getprovider)**(const string & dataId) |
| virtual [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [TS](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#typedef-ts) * > * | **[GetEnsembleTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#function-getensembletimeseries)**(const string & dataId) |
| virtual [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [TS](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#typedef-ts) * > * | **[GetAllTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#function-getalltimeseries)**(const string & dataId) |
| virtual [EnsembleForecastTimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-ensembleforecasttimeseries)< [TS](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#typedef-ts) > * | **[GetTimeSeriesEnsembleTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#function-gettimeseriesensembletimeseries)**(const string & dataId) |
| virtual vector< string > | **[GetIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/#function-getidentifiers)**() const |

## Detailed Description

```cpp
template <typename T >
class datatypes::timeseries::TTimeSeriesLibrary;
```

## Public Types Documentation

### typedef TS

```cpp
typedef TTimeSeries<T> datatypes::timeseries::TTimeSeriesLibrary< T >::TS;
```


### typedef MTS

```cpp
typedef MultiTimeSeries<TS*> datatypes::timeseries::TTimeSeriesLibrary< T >::MTS;
```


## Public Functions Documentation

### function ~TTimeSeriesLibrary

```cpp
inline virtual ~TTimeSeriesLibrary()
```


### function GetSingle

```cpp
inline virtual TS * GetSingle(
    const string & dataId
)
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesLibrary::GetSingle](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-getsingle)


### function GetSingle

```cpp
inline virtual TS * GetSingle(
    const string & dataId,
    const string & collectionIdentifier
)
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesLibrary::GetSingle](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-getsingle)


### function GetCollection

```cpp
inline virtual MTS * GetCollection(
    const string & dataId
)
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesLibrary::GetCollection](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-getcollection)


### function GetProvider

```cpp
inline virtual TimeSeriesProvider< T > * GetProvider(
    const string & dataId
)
```


### function GetEnsembleTimeSeries

```cpp
inline virtual MultiTimeSeries< TS * > * GetEnsembleTimeSeries(
    const string & dataId
)
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesLibrary::GetEnsembleTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-getensembletimeseries)


### function GetAllTimeSeries

```cpp
inline virtual MultiTimeSeries< TS * > * GetAllTimeSeries(
    const string & dataId
)
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesLibrary::GetAllTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-getalltimeseries)


### function GetTimeSeriesEnsembleTimeSeries

```cpp
inline virtual EnsembleForecastTimeSeries< TS > * GetTimeSeriesEnsembleTimeSeries(
    const string & dataId
)
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesLibrary::GetTimeSeriesEnsembleTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-gettimeseriesensembletimeseries)


### function GetIdentifiers

```cpp
inline virtual vector< string > GetIdentifiers() const
```


**Reimplemented by**: [datatypes::timeseries::TimeSeriesLibrary::GetIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/#function-getidentifiers)


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000