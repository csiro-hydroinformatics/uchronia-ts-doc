---
title: datatypes/interop_conversions.h

---

# datatypes/interop_conversions.h



## Namespaces

| Name           |
| -------------- |
| **[cinterop::utils](/cpp/Namespaces/namespacecinterop_1_1utils/)**  |

## Functions

|                | Name           |
| -------------- | -------------- |
| [DATATYPES_DLL_LIB](/cpp/Files/setup__exports_8h/#define-datatypes-dll-lib)[TimeSeries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) | **[CreateTimeSeries](/cpp/Files/interop__conversions_8h/#function-createtimeseries)**(double * values, const regular_time_series_geometry & g) |
| [DATATYPES_DLL_LIB](/cpp/Files/setup__exports_8h/#define-datatypes-dll-lib)[TimeSeries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) | **[CreateTimeSeries](/cpp/Files/interop__conversions_8h/#function-createtimeseries)**(double * values, [TS_GEOMETRY_PTR](/cpp/Files/extern__c__api__transparent__pointers_8h/#define-ts-geometry-ptr) geom) |
| [DATATYPES_DLL_LIB](/cpp/Files/setup__exports_8h/#define-datatypes-dll-lib)[TimeSeries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) | **[CreateTimeSeries](/cpp/Files/interop__conversions_8h/#function-createtimeseries)**(const multi_regular_time_series_data & g) |
| [DATATYPES_DLL_LIB](/cpp/Files/setup__exports_8h/#define-datatypes-dll-lib)[TimeSeriesEnsemble](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-timeseriesensemble)< [TimeSeries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) > | **[ToTimeSeriesEnsemble](/cpp/Files/interop__conversions_8h/#function-totimeseriesensemble)**(const multi_regular_time_series_data & rawData) |
| [DATATYPES_DLL_LIB](/cpp/Files/setup__exports_8h/#define-datatypes-dll-lib)[TimeSeriesEnsemble](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-timeseriesensemble)< [TimeSeries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) > * | **[ToTimeSeriesEnsemblePtr](/cpp/Files/interop__conversions_8h/#function-totimeseriesensembleptr)**(const multi_regular_time_series_data & rawData) |
| [DATATYPES_DLL_LIB](/cpp/Files/setup__exports_8h/#define-datatypes-dll-lib) multi_regular_time_series_data * | **[ToMultiTimeSeriesDataPtr](/cpp/Files/interop__conversions_8h/#function-tomultitimeseriesdataptr)**(const [TimeSeriesEnsemble](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-timeseriesensemble)< [TimeSeries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) > & mts) |
| [DATATYPES_DLL_LIB](/cpp/Files/setup__exports_8h/#define-datatypes-dll-lib) multi_regular_time_series_data * | **[ToMultiTimeSeriesDataPtr](/cpp/Files/interop__conversions_8h/#function-tomultitimeseriesdataptr)**(const [TimeSeries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) & ts) |
| [DATATYPES_DLL_LIB](/cpp/Files/setup__exports_8h/#define-datatypes-dll-lib)[TimeSeries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) * | **[SingleTsPtrFromMultiTimeSeriesData](/cpp/Files/interop__conversions_8h/#function-singletsptrfrommultitimeseriesdata)**(const multi_regular_time_series_data & ts) |
| [DATATYPES_DLL_LIB](/cpp/Files/setup__exports_8h/#define-datatypes-dll-lib)[TimeSeriesEnsemble](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-timeseriesensemble)< [TimeSeries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) > * | **[MultiTsPtrFromMultiTimeSeriesData](/cpp/Files/interop__conversions_8h/#function-multitsptrfrommultitimeseriesdata)**(const multi_regular_time_series_data & ts) |
| [DATATYPES_DLL_LIB](/cpp/Files/setup__exports_8h/#define-datatypes-dll-lib)[TimeSeries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) | **[SingleTsFromMultiTimeSeriesData](/cpp/Files/interop__conversions_8h/#function-singletsfrommultitimeseriesdata)**(const multi_regular_time_series_data & ts) |
| [DATATYPES_DLL_LIB](/cpp/Files/setup__exports_8h/#define-datatypes-dll-lib)[TimeSeriesEnsemble](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-timeseriesensemble)< [TimeSeries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) > | **[MultiTsFromMultiTimeSeriesData](/cpp/Files/interop__conversions_8h/#function-multitsfrommultitimeseriesdata)**(const multi_regular_time_series_data & ts) |
| [DATATYPES_DLL_LIB](/cpp/Files/setup__exports_8h/#define-datatypes-dll-lib) time_series_dimensions_description * | **[ToTimeSeriesDimensionDescriptions](/cpp/Files/interop__conversions_8h/#function-totimeseriesdimensiondescriptions)**(vector< [DataDimensionDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) > & mts) |
| [DATATYPES_DLL_LIB](/cpp/Files/setup__exports_8h/#define-datatypes-dll-lib) void | **[CopyToMultiTimeSeriesData](/cpp/Files/interop__conversions_8h/#function-copytomultitimeseriesdata)**(const [TimeSeriesEnsemble](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-timeseriesensemble)< [TimeSeries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) > & mts, multi_regular_time_series_data & result) |
| [DATATYPES_DLL_LIB](/cpp/Files/setup__exports_8h/#define-datatypes-dll-lib) void | **[CopyToMultiTimeSeriesData](/cpp/Files/interop__conversions_8h/#function-copytomultitimeseriesdata)**(const [TimeSeries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) & ts, multi_regular_time_series_data & result) |
| [DATATYPES_DLL_LIB](/cpp/Files/setup__exports_8h/#define-datatypes-dll-lib) void | **[CopyFromMultiTimeSeriesData](/cpp/Files/interop__conversions_8h/#function-copyfrommultitimeseriesdata)**(const multi_regular_time_series_data & interopdata, [TimeSeries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) & ts) |
| [DATATYPES_DLL_LIB](/cpp/Files/setup__exports_8h/#define-datatypes-dll-lib) void | **[CopyFromMultiTimeSeriesData](/cpp/Files/interop__conversions_8h/#function-copyfrommultitimeseriesdata)**(const multi_regular_time_series_data & interopdata, [TimeSeriesEnsemble](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-timeseriesensemble)< [TimeSeries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) > & mts) |
| [DATATYPES_DLL_LIB](/cpp/Files/setup__exports_8h/#define-datatypes-dll-lib) double ** | **[ToRawData](/cpp/Files/interop__conversions_8h/#function-torawdata)**(const [TimeSeriesEnsemble](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-timeseriesensemble)< [TimeSeries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) > & mts) |
| [DATATYPES_DLL_LIB](/cpp/Files/setup__exports_8h/#define-datatypes-dll-lib) double * | **[ToRawData](/cpp/Files/interop__conversions_8h/#function-torawdata)**(const [TimeSeries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) & ts) |
| [DATATYPES_DLL_LIB](/cpp/Files/setup__exports_8h/#define-datatypes-dll-lib) void | **[DisposeMultiTimeSeriesData](/cpp/Files/interop__conversions_8h/#function-disposemultitimeseriesdata)**(multi_regular_time_series_data * d) |
| [DATATYPES_DLL_LIB](/cpp/Files/setup__exports_8h/#define-datatypes-dll-lib) void | **[DisposeTimeSeriesDimensionDescriptions](/cpp/Files/interop__conversions_8h/#function-disposetimeseriesdimensiondescriptions)**(time_series_dimensions_description * d) |


## Functions Documentation

### function CreateTimeSeries

```cpp
DATATYPES_DLL_LIBTimeSeries CreateTimeSeries(
    double * values,
    const regular_time_series_geometry & g
)
```


### function CreateTimeSeries

```cpp
DATATYPES_DLL_LIBTimeSeries CreateTimeSeries(
    double * values,
    TS_GEOMETRY_PTR geom
)
```


### function CreateTimeSeries

```cpp
DATATYPES_DLL_LIBTimeSeries CreateTimeSeries(
    const multi_regular_time_series_data & g
)
```


### function ToTimeSeriesEnsemble

```cpp
DATATYPES_DLL_LIBTimeSeriesEnsemble< TimeSeries > ToTimeSeriesEnsemble(
    const multi_regular_time_series_data & rawData
)
```


### function ToTimeSeriesEnsemblePtr

```cpp
DATATYPES_DLL_LIBTimeSeriesEnsemble< TimeSeries > * ToTimeSeriesEnsemblePtr(
    const multi_regular_time_series_data & rawData
)
```


### function ToMultiTimeSeriesDataPtr

```cpp
DATATYPES_DLL_LIB multi_regular_time_series_data * ToMultiTimeSeriesDataPtr(
    const TimeSeriesEnsemble< TimeSeries > & mts
)
```


### function ToMultiTimeSeriesDataPtr

```cpp
DATATYPES_DLL_LIB multi_regular_time_series_data * ToMultiTimeSeriesDataPtr(
    const TimeSeries & ts
)
```


### function SingleTsPtrFromMultiTimeSeriesData

```cpp
DATATYPES_DLL_LIBTimeSeries * SingleTsPtrFromMultiTimeSeriesData(
    const multi_regular_time_series_data & ts
)
```


### function MultiTsPtrFromMultiTimeSeriesData

```cpp
DATATYPES_DLL_LIBTimeSeriesEnsemble< TimeSeries > * MultiTsPtrFromMultiTimeSeriesData(
    const multi_regular_time_series_data & ts
)
```


### function SingleTsFromMultiTimeSeriesData

```cpp
DATATYPES_DLL_LIBTimeSeries SingleTsFromMultiTimeSeriesData(
    const multi_regular_time_series_data & ts
)
```


### function MultiTsFromMultiTimeSeriesData

```cpp
DATATYPES_DLL_LIBTimeSeriesEnsemble< TimeSeries > MultiTsFromMultiTimeSeriesData(
    const multi_regular_time_series_data & ts
)
```


### function ToTimeSeriesDimensionDescriptions

```cpp
DATATYPES_DLL_LIB time_series_dimensions_description * ToTimeSeriesDimensionDescriptions(
    vector< DataDimensionDescriptor > & mts
)
```


### function CopyToMultiTimeSeriesData

```cpp
DATATYPES_DLL_LIB void CopyToMultiTimeSeriesData(
    const TimeSeriesEnsemble< TimeSeries > & mts,
    multi_regular_time_series_data & result
)
```


### function CopyToMultiTimeSeriesData

```cpp
DATATYPES_DLL_LIB void CopyToMultiTimeSeriesData(
    const TimeSeries & ts,
    multi_regular_time_series_data & result
)
```


### function CopyFromMultiTimeSeriesData

```cpp
DATATYPES_DLL_LIB void CopyFromMultiTimeSeriesData(
    const multi_regular_time_series_data & interopdata,
    TimeSeries & ts
)
```


### function CopyFromMultiTimeSeriesData

```cpp
DATATYPES_DLL_LIB void CopyFromMultiTimeSeriesData(
    const multi_regular_time_series_data & interopdata,
    TimeSeriesEnsemble< TimeSeries > & mts
)
```


### function ToRawData

```cpp
DATATYPES_DLL_LIB double ** ToRawData(
    const TimeSeriesEnsemble< TimeSeries > & mts
)
```


### function ToRawData

```cpp
DATATYPES_DLL_LIB double * ToRawData(
    const TimeSeries & ts
)
```


### function DisposeMultiTimeSeriesData

```cpp
DATATYPES_DLL_LIB void DisposeMultiTimeSeriesData(
    multi_regular_time_series_data * d
)
```


### function DisposeTimeSeriesDimensionDescriptions

```cpp
DATATYPES_DLL_LIB void DisposeTimeSeriesDimensionDescriptions(
    time_series_dimensions_description * d
)
```




## Source code

```cpp
#pragma once

#include "cinterop/c_cpp_interop.hpp"
#include "datatypes/common.h"
#include "datatypes/time_series_io.hpp"
#include "datatypes/internals_c_api.hpp"

using namespace cinterop::utils;
using namespace datatypes::timeseries;

DATATYPES_DLL_LIB TimeSeries CreateTimeSeries(double * values, const regular_time_series_geometry& g);
DATATYPES_DLL_LIB TimeSeries CreateTimeSeries(double * values, TS_GEOMETRY_PTR geom);
DATATYPES_DLL_LIB TimeSeries CreateTimeSeries(const multi_regular_time_series_data& g);
DATATYPES_DLL_LIB TimeSeriesEnsemble<TimeSeries> ToTimeSeriesEnsemble(const multi_regular_time_series_data& rawData);
DATATYPES_DLL_LIB TimeSeriesEnsemble<TimeSeries>* ToTimeSeriesEnsemblePtr(const multi_regular_time_series_data& rawData);
DATATYPES_DLL_LIB multi_regular_time_series_data* ToMultiTimeSeriesDataPtr(const TimeSeriesEnsemble<TimeSeries>& mts);
DATATYPES_DLL_LIB multi_regular_time_series_data* ToMultiTimeSeriesDataPtr(const TimeSeries& ts);
DATATYPES_DLL_LIB TimeSeries* SingleTsPtrFromMultiTimeSeriesData(const multi_regular_time_series_data& ts);
DATATYPES_DLL_LIB TimeSeriesEnsemble<TimeSeries>* MultiTsPtrFromMultiTimeSeriesData(const multi_regular_time_series_data& ts);
DATATYPES_DLL_LIB TimeSeries SingleTsFromMultiTimeSeriesData(const multi_regular_time_series_data& ts);
DATATYPES_DLL_LIB TimeSeriesEnsemble<TimeSeries> MultiTsFromMultiTimeSeriesData(const multi_regular_time_series_data& ts);
DATATYPES_DLL_LIB time_series_dimensions_description* ToTimeSeriesDimensionDescriptions(vector<DataDimensionDescriptor>& mts);
DATATYPES_DLL_LIB void CopyToMultiTimeSeriesData(const TimeSeriesEnsemble<TimeSeries>& mts, multi_regular_time_series_data& result);
DATATYPES_DLL_LIB void CopyToMultiTimeSeriesData(const TimeSeries& ts, multi_regular_time_series_data& result);
DATATYPES_DLL_LIB void CopyFromMultiTimeSeriesData(const multi_regular_time_series_data& interopdata, TimeSeries& ts);
DATATYPES_DLL_LIB void CopyFromMultiTimeSeriesData(const multi_regular_time_series_data& interopdata, TimeSeriesEnsemble<TimeSeries>& mts);
DATATYPES_DLL_LIB double** ToRawData(const TimeSeriesEnsemble<TimeSeries>& mts);
DATATYPES_DLL_LIB double* ToRawData(const TimeSeries& ts);
DATATYPES_DLL_LIB void DisposeMultiTimeSeriesData(multi_regular_time_series_data* d);
DATATYPES_DLL_LIB void DisposeTimeSeriesDimensionDescriptions(time_series_dimensions_description* d);
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000
