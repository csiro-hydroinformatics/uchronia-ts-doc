---
title: datatypes::timeseries::CommonTypes
summary: Typical ensemble and time series data types derived from a fundamental data type for each data item. 

---

# datatypes::timeseries::CommonTypes



Typical ensemble and time series data types derived from a fundamental data type for each data item.  [More...](#detailed-description)


`#include <time_series.hpp>`

## Public Types

|                | Name           |
| -------------- | -------------- |
| using typename [time_series_of](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1time__series__of/)< ElementType >::type | **[SeriesType](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/#using-seriestype)** <br>Type of a time series for this fundamental element type: TTimeSeries<ElementType>  |
| using typename std::add_pointer< [SeriesType](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/#using-seriestype) >::type | **[PtrSeriesType](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/#using-ptrseriestype)** <br>Type of pointer a time series for this fundamental element type: TTimeSeries<ElementType>*.  |
| using typename [ensemble_of](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1ensemble__of/)< [SeriesType](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/#using-seriestype) >::type | **[EnsembleType](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/#using-ensembletype)** <br>Type of [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)<TTimeSeries<ElementType>>  |
| using typename [ensemble_of](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1ensemble__of/)< [PtrSeriesType](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/#using-ptrseriestype) >::type | **[EnsemblePtrType](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/#using-ensembleptrtype)** <br>Type of [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)<TTimeSeries<ElementType>*>  |
| using typename std::add_pointer< [EnsemblePtrType](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/#using-ensembleptrtype) >::type | **[PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/#using-ptrensembleptrtype)** <br>Type of a pointer to a [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)<TTimeSeries<ElementType>*>  |
| using typename [time_series_of](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1time__series__of/)< [PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/#using-ptrensembleptrtype) >::type | **[TSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/#using-tseriesensembleptrtype)** <br>Type of [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)<TTimeSeries<ElementType>*>* >  |
| using typename std::add_pointer< [TSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/#using-tseriesensembleptrtype) >::type | **[PtrTSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/#using-ptrtseriesensembleptrtype)** <br>Type of a pointer to a [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)<TTimeSeries<ElementType>*>* >  |

## Detailed Description

```cpp
template <typename ElementType  =double>
struct datatypes::timeseries::CommonTypes;
```

Typical ensemble and time series data types derived from a fundamental data type for each data item. 

**Template Parameters**: 

  * **ElementType** fundamental data type for each data item. 

## Public Types Documentation

### using SeriesType

```cpp
using datatypes::timeseries::CommonTypes< ElementType >::SeriesType =  typename time_series_of<ElementType>::type;
```

Type of a time series for this fundamental element type: TTimeSeries<ElementType> 

### using PtrSeriesType

```cpp
using datatypes::timeseries::CommonTypes< ElementType >::PtrSeriesType =  typename std::add_pointer<SeriesType>::type;
```

Type of pointer a time series for this fundamental element type: TTimeSeries<ElementType>*. 

### using EnsembleType

```cpp
using datatypes::timeseries::CommonTypes< ElementType >::EnsembleType =  typename ensemble_of<SeriesType>::type;
```

Type of [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)<TTimeSeries<ElementType>> 

### using EnsemblePtrType

```cpp
using datatypes::timeseries::CommonTypes< ElementType >::EnsemblePtrType =  typename ensemble_of<PtrSeriesType>::type;
```

Type of [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)<TTimeSeries<ElementType>*> 

### using PtrEnsemblePtrType

```cpp
using datatypes::timeseries::CommonTypes< ElementType >::PtrEnsemblePtrType =  typename std::add_pointer<EnsemblePtrType>::type;
```

Type of a pointer to a [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)<TTimeSeries<ElementType>*> 

### using TSeriesEnsemblePtrType

```cpp
using datatypes::timeseries::CommonTypes< ElementType >::TSeriesEnsemblePtrType =  typename time_series_of<PtrEnsemblePtrType>::type;
```

Type of [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)<TTimeSeries<ElementType>*>* > 

### using PtrTSeriesEnsemblePtrType

```cpp
using datatypes::timeseries::CommonTypes< ElementType >::PtrTSeriesEnsemblePtrType =  typename std::add_pointer<TSeriesEnsemblePtrType>::type;
```

Type of a pointer to a [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)<TTimeSeries<ElementType>*>* > 

-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000