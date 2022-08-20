---
title: datatypes::timeseries

---

# datatypes::timeseries



## Namespaces

| Name           |
| -------------- |
| **[datatypes::timeseries::io](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries_1_1io/)**  |

## Classes

|                | Name           |
| -------------- | -------------- |
| struct | **[datatypes::timeseries::DefaultMissingValuePolicyTypeFactory](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1DefaultMissingValuePolicyTypeFactory/)**  |
| class | **[datatypes::timeseries::TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)** <br>A template for univariate, single realisasion time series.  |
| class | **[datatypes::timeseries::MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)** <br>Template for time series with multiple values at time point; e.g. to hold multiple realizations of time series in an ensemble.  |
| struct | **[datatypes::timeseries::time_series_of](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1time__series__of/)**  |
| struct | **[datatypes::timeseries::ensemble_of](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1ensemble__of/)**  |
| struct | **[datatypes::timeseries::item_type_of](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1item__type__of/)**  |
| struct | **[datatypes::timeseries::CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)** <br>Typical ensemble and time series data types derived from a fundamental data type for each data item.  |
| class | **[datatypes::timeseries::TimeSeriesOperations](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/)**  |
| class | **[datatypes::timeseries::TimeWindow](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeWindow/)** <br>An object that represents a time window, defining subset/trim operations on time series.  |
| class | **[datatypes::timeseries::GlobalAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/)** <br>A class to hold the global attributes of a file stored in the SWIFT netCDF format.  |
| class | **[datatypes::timeseries::VariableAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/)** <br>A class to hold the attributes of a netCDF variable stored in the SWIFT netCDF format.  |
| class | **[datatypes::timeseries::VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/)**  |
| class | **[datatypes::timeseries::DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/)**  |
| class | **[datatypes::timeseries::DataGeometryProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataGeometryProvider/)**  |
| class | **[datatypes::timeseries::TimeSeriesIOHelper](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/)** <br>Representation of an univariate, ensemble time series with a SWIFT netCDF back end.  |
| class | **[datatypes::timeseries::SingleNetCdfFileStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/)**  |
| class | **[datatypes::timeseries::NetCdfSingleSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/)**  |
| class | **[datatypes::timeseries::NetCdfEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfEnsembleTimeSeriesStore/)**  |
| class | **[datatypes::timeseries::EagerWriter](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/)**  |
| class | **[datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/)**  |
| class | **[datatypes::timeseries::MultiFileTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/)** <br>An implementation of [TimeSeriesEnsembleTimeSeriesStore]() such that the content of a time series is spread amongst several files.  |
| class | **[datatypes::timeseries::MultiFileTsStorage](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/)** <br>An implementation of [StoragePolicy]() such that the content of a time series is spread amongst several files.  |
| class | **[datatypes::timeseries::TimeSeriesLibraryFactory](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/)**  |
| class | **[datatypes::timeseries::SwiftNetcdfStoreFactory](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SwiftNetcdfStoreFactory/)**  |
| class | **[datatypes::timeseries::IdentifiersProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/)** <br>An interface definition for objects that can provide hierarchical identification.  |
| class | **[datatypes::timeseries::TimeSeriesProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesProvider/)** <br>Library of time series, for high level access to sources of univariate, single instance time series that may have varying on-disk representations.  |
| class | **[datatypes::timeseries::DataDimensionDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/)**  |
| class | **[datatypes::timeseries::DataDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/)**  |
| class | **[datatypes::timeseries::SingleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/)** <br>Interface definition for storages of single, univariate time series.  |
| class | **[datatypes::timeseries::EnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/)** <br>Interface definition for storages of ensembles of univariate time series.  |
| class | **[datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)** <br>Interface definition for storages of time series of ensembles of time series.  |
| class | **[datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/)**  |
| class | **[datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/)**  |
| class | **[datatypes::timeseries::TTimeSeriesLibrary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/)**  |
| class | **[datatypes::timeseries::TimeSeriesSourceInfoImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/)**  |
| class | **[datatypes::timeseries::TimeSeriesSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/)**  |
| class | **[datatypes::timeseries::NetCdfSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/)**  |
| class | **[datatypes::timeseries::TimeSeriesLibraryDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/)**  |
| class | **[datatypes::timeseries::TimeSeriesSourceInfoBuilder](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoBuilder/)** <br>An abstract class to allow callers to inject custom time series data sources into a time series library.  |
| class | **[datatypes::timeseries::TimeSeriesStoreFactory](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/)**  |
| class | **[datatypes::timeseries::TimeSeriesLibrary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/)** <br>Library of time series, for high level access to sources of time series that nmay have varying on-disk representations.  |
| class | **[datatypes::timeseries::StoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)** <br>An interface for classes that can handle the storage of data for time series.  |
| class | **[datatypes::timeseries::MissingValuePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/)** <br>An interface for classes that define missing values in time series.  |
| class | **[datatypes::timeseries::DefaultMissingFloatingPointPolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DefaultMissingFloatingPointPolicy/)**  |
| class | **[datatypes::timeseries::NullPointerIsMissingPolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NullPointerIsMissingPolicy/)**  |
| class | **[datatypes::timeseries::NegativeIsMissingFloadingPointPolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NegativeIsMissingFloadingPointPolicy/)**  |
| class | **[datatypes::timeseries::StlVectorStorage](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/)**  |
| class | **[datatypes::timeseries::SharedVectorStorage](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SharedVectorStorage/)** <br>A storage strategy for time serie such that data is a shared state amongst several time series.  |
| class | **[datatypes::timeseries::MemoryCachingStorageWriter](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/)**  |
| class | **[datatypes::timeseries::EnsembleStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)**  |
| class | **[datatypes::timeseries::StdVectorEnsembleStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/)**  |
| class | **[datatypes::timeseries::TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/)** <br>Time step handling for time series.  |
| class | **[datatypes::timeseries::TimeSeriesInfoProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/)** <br>An interface definition for classes that can provide essential time series temporal characteristics.  |
| class | **[datatypes::timeseries::TimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/)**  |
| class | **[datatypes::timeseries::RegularTimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/)**  |
| class | **[datatypes::timeseries::IrregularTimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/)**  |
| class | **[datatypes::timeseries::MonthlyQppTimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/)**  |

## Types

|                | Name           |
| -------------- | -------------- |
| typedef [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< double > | **[TimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries)**  |
| template <typename ItemType \> <br>using [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< ItemType * > | **[PointerTypeTimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-pointertypetimeseries)**  |
| template <typename Tts  =TimeSeries\> <br>using [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< Tts * > | **[MultiTimeSeriesPtr](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-multitimeseriesptr)**  |
| template <typename Tts  =TimeSeries\> <br>using [PointerTypeTimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-pointertypetimeseries)< Tts > | **[ForecastTimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-forecasttimeseries)**  |
| template <typename Tts  =TimeSeries\> <br>using [MultiTimeSeriesPtr](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-multitimeseriesptr)< Tts > | **[TimeSeriesEnsemble](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-timeseriesensemble)**  |
| template <typename Tts  =TimeSeries\> <br>using [PointerTypeTimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-pointertypetimeseries)< [MultiTimeSeriesPtr](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-multitimeseriesptr)< Tts > > | **[EnsembleForecastTimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-ensembleforecasttimeseries)**  |

## Functions

|                | Name           |
| -------------- | -------------- |
| template <typename T \> <br>[MissingValuePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/)< T > * | **[DefaultMissingValuePolicy](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#function-defaultmissingvaluepolicy)**()<br>Default missing value policy.  |
| template <typename T \> <br>[StoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)< T > * | **[DefaultStoragePolicy](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#function-defaultstoragepolicy)**()<br>Default strategy for storing time series data.  |
| template <typename T \> <br>[TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > | **[operator<<](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#function-operator<<)**(const [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > & a, const [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > & b) |
| template <typename From ,typename To \> <br>To | **[GetMetadataFrom](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#function-getmetadatafrom)**(const From & ens) |
| template <typename ElementType \> <br>[DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) | **[DimensionsFromSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#function-dimensionsfromseries)**(const [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< ElementType > & ts, const size_t ensembleSize =1, const size_t leadTimeSize =1, const vector< string > & stationIds =[DEFAULT_STATION_IDENTIFIER](/uchronia-ts-doc/cpp/Files/common_8h/#define-default-station-identifier)) |
| template <typename ElementType \> <br>[DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) | **[DimensionsFromSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#function-dimensionsfromseries)**([EnsembleForecastTimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-ensembleforecasttimeseries)<> & tsEns, const vector< string > & stationIds =[DEFAULT_STATION_IDENTIFIER](/uchronia-ts-doc/cpp/Files/common_8h/#define-default-station-identifier)) |
| template <typename ElementType \> <br>[DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) | **[DimensionsFromSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#function-dimensionsfromseries)**(const vector< [EnsembleForecastTimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-ensembleforecasttimeseries)<>::ElementType > & values, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & tsEnsTstep =[TimeStep::GetUnknown](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-getunknown)(), const ptime & tsEnsStart =not_a_date_time, const vector< string > & stationIds =[DEFAULT_STATION_IDENTIFIER](/uchronia-ts-doc/cpp/Files/common_8h/#define-default-station-identifier), int fcastOffset =1) |
| template <typename TElement \> <br>[DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) | **[DimensionsFromPointTimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#function-dimensionsfrompointtimeseries)**(const [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< TElement > & ts) |

## Types Documentation

### typedef TimeSeries

```cpp
typedef TTimeSeries< double > datatypes::timeseries::TimeSeries;
```


### using PointerTypeTimeSeries

```cpp
template <typename ItemType >
using datatypes::timeseries::PointerTypeTimeSeries = typedef TTimeSeries < ItemType* >;
```


### using MultiTimeSeriesPtr

```cpp
template <typename Tts  =TimeSeries>
using datatypes::timeseries::MultiTimeSeriesPtr = typedef MultiTimeSeries < Tts* >;
```


### using ForecastTimeSeries

```cpp
template <typename Tts  =TimeSeries>
using datatypes::timeseries::ForecastTimeSeries = typedef PointerTypeTimeSeries < Tts >;
```


### using TimeSeriesEnsemble

```cpp
template <typename Tts  =TimeSeries>
using datatypes::timeseries::TimeSeriesEnsemble = typedef MultiTimeSeriesPtr < Tts >;
```


### using EnsembleForecastTimeSeries

```cpp
template <typename Tts  =TimeSeries>
using datatypes::timeseries::EnsembleForecastTimeSeries = typedef PointerTypeTimeSeries < MultiTimeSeriesPtr<Tts> >;
```



## Functions Documentation

### function DefaultMissingValuePolicy

```cpp
template <typename T >
MissingValuePolicy< T > * DefaultMissingValuePolicy()
```

Default missing value policy. 

**Template Parameters**: 

  * **T** Generic type parameter, the type of the elements of the time series


**Return**: A new object inheriting from [MissingValuePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/)<T>*> 



```
    A function that returnes a suitable default object to handle 
    time series behaviors with respect to missing values
```


### function DefaultStoragePolicy

```cpp
template <typename T >
StoragePolicy< T > * DefaultStoragePolicy()
```

Default strategy for storing time series data. 

**Template Parameters**: 

  * **T** Generic type parameter, the type of the elements of the time series


**Return**: A new object inheriting from [StoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)<T>*> 



```
    A function that returnes a suitable default object to handle
    the storage of time series data. The default is in memory vector.
```


### function operator<<

```cpp
template <typename T >
TTimeSeries< T > operator<<(
    const TTimeSeries< T > & a,
    const TTimeSeries< T > & b
)
```


### function GetMetadataFrom

```cpp
template <typename From ,
typename To >
To GetMetadataFrom(
    const From & ens
)
```


### function DimensionsFromSeries

```cpp
template <typename ElementType >
DimensionsDefinitions DimensionsFromSeries(
    const TTimeSeries< ElementType > & ts,
    const size_t ensembleSize =1,
    const size_t leadTimeSize =1,
    const vector< string > & stationIds =DEFAULT_STATION_IDENTIFIER
)
```


### function DimensionsFromSeries

```cpp
template <typename ElementType >
DimensionsDefinitions DimensionsFromSeries(
    EnsembleForecastTimeSeries<> & tsEns,
    const vector< string > & stationIds =DEFAULT_STATION_IDENTIFIER
)
```


### function DimensionsFromSeries

```cpp
template <typename ElementType >
DimensionsDefinitions DimensionsFromSeries(
    const vector< EnsembleForecastTimeSeries<>::ElementType > & values,
    const TimeStep & tsEnsTstep =TimeStep::GetUnknown(),
    const ptime & tsEnsStart =not_a_date_time,
    const vector< string > & stationIds =DEFAULT_STATION_IDENTIFIER,
    int fcastOffset =1
)
```


### function DimensionsFromPointTimeSeries

```cpp
template <typename TElement >
DimensionsDefinitions DimensionsFromPointTimeSeries(
    const TTimeSeries< TElement > & ts
)
```






-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000