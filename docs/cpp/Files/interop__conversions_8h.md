---
title: datatypes/interop_conversions.h

---

# datatypes/interop_conversions.h



## Namespaces

| Name           |
| -------------- |
| **[cinterop::utils](/uchronia-ts-doc/cpp/Namespaces/namespacecinterop_1_1utils/)**  |

## Functions

|                | Name           |
| -------------- | -------------- |
| [TimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) | **[CreateTimeSeries](/uchronia-ts-doc/cpp/Files/interop__conversions_8h/#function-createtimeseries)**(double * values, const regular_time_series_geometry & g)<br>Helper function for C API interop conversions.  |
| [TimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) | **[CreateTimeSeries](/uchronia-ts-doc/cpp/Files/interop__conversions_8h/#function-createtimeseries)**(double * values, [TS_GEOMETRY_PTR](/uchronia-ts-doc/cpp/Files/extern__c__api__transparent__pointers_8h/#define-ts-geometry-ptr) geom)<br>Helper function for C API interop conversions.  |
| [TimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) | **[CreateTimeSeries](/uchronia-ts-doc/cpp/Files/interop__conversions_8h/#function-createtimeseries)**(const multi_regular_time_series_data & g)<br>Helper function for C API interop conversions.  |
| [TimeSeriesEnsemble](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-timeseriesensemble)< [TimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) > | **[ToTimeSeriesEnsemble](/uchronia-ts-doc/cpp/Files/interop__conversions_8h/#function-totimeseriesensemble)**(const multi_regular_time_series_data & rawData)<br>Helper function for C API interop conversions.  |
| [TimeSeriesEnsemble](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-timeseriesensemble)< [TimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) > * | **[ToTimeSeriesEnsemblePtr](/uchronia-ts-doc/cpp/Files/interop__conversions_8h/#function-totimeseriesensembleptr)**(const multi_regular_time_series_data & rawData)<br>Helper function for C API interop conversions.  |
| multi_regular_time_series_data * | **[ToMultiTimeSeriesDataPtr](/uchronia-ts-doc/cpp/Files/interop__conversions_8h/#function-tomultitimeseriesdataptr)**(const [TimeSeriesEnsemble](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-timeseriesensemble)< [TimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) > & mts)<br>Helper function for C API interop conversions.  |
| multi_regular_time_series_data * | **[ToMultiTimeSeriesDataPtr](/uchronia-ts-doc/cpp/Files/interop__conversions_8h/#function-tomultitimeseriesdataptr)**(const [TimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) & ts)<br>Helper function for C API interop conversions.  |
| [TimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) * | **[SingleTsPtrFromMultiTimeSeriesData](/uchronia-ts-doc/cpp/Files/interop__conversions_8h/#function-singletsptrfrommultitimeseriesdata)**(const multi_regular_time_series_data & ts)<br>Helper function for C API interop conversions.  |
| [TimeSeriesEnsemble](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-timeseriesensemble)< [TimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) > * | **[MultiTsPtrFromMultiTimeSeriesData](/uchronia-ts-doc/cpp/Files/interop__conversions_8h/#function-multitsptrfrommultitimeseriesdata)**(const multi_regular_time_series_data & ts)<br>Helper function for C API interop conversions.  |
| [TimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) | **[SingleTsFromMultiTimeSeriesData](/uchronia-ts-doc/cpp/Files/interop__conversions_8h/#function-singletsfrommultitimeseriesdata)**(const multi_regular_time_series_data & ts)<br>Helper function for C API interop conversions.  |
| [TimeSeriesEnsemble](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-timeseriesensemble)< [TimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) > | **[MultiTsFromMultiTimeSeriesData](/uchronia-ts-doc/cpp/Files/interop__conversions_8h/#function-multitsfrommultitimeseriesdata)**(const multi_regular_time_series_data & ts)<br>Helper function for C API interop conversions.  |
| time_series_dimensions_description * | **[ToTimeSeriesDimensionDescriptions](/uchronia-ts-doc/cpp/Files/interop__conversions_8h/#function-totimeseriesdimensiondescriptions)**(vector< [DataDimensionDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) > & mts)<br>Helper function for C API interop conversions.  |
| void | **[CopyToMultiTimeSeriesData](/uchronia-ts-doc/cpp/Files/interop__conversions_8h/#function-copytomultitimeseriesdata)**(const [TimeSeriesEnsemble](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-timeseriesensemble)< [TimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) > & mts, multi_regular_time_series_data & result)<br>Helper function for C API interop conversions.  |
| void | **[CopyToMultiTimeSeriesData](/uchronia-ts-doc/cpp/Files/interop__conversions_8h/#function-copytomultitimeseriesdata)**(const [TimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) & ts, multi_regular_time_series_data & result)<br>Helper function for C API interop conversions.  |
| void | **[CopyFromMultiTimeSeriesData](/uchronia-ts-doc/cpp/Files/interop__conversions_8h/#function-copyfrommultitimeseriesdata)**(const multi_regular_time_series_data & interopdata, [TimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) & ts)<br>Helper function for C API interop conversions.  |
| void | **[CopyFromMultiTimeSeriesData](/uchronia-ts-doc/cpp/Files/interop__conversions_8h/#function-copyfrommultitimeseriesdata)**(const multi_regular_time_series_data & interopdata, [TimeSeriesEnsemble](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-timeseriesensemble)< [TimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) > & mts)<br>Helper function for C API interop conversions.  |
| double ** | **[ToRawData](/uchronia-ts-doc/cpp/Files/interop__conversions_8h/#function-torawdata)**(const [TimeSeriesEnsemble](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-timeseriesensemble)< [TimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) > & mts)<br>Helper function for C API interop conversions.  |
| double * | **[ToRawData](/uchronia-ts-doc/cpp/Files/interop__conversions_8h/#function-torawdata)**(const [TimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) & ts)<br>Helper function for C API interop conversions.  |
| void | **[DisposeMultiTimeSeriesData](/uchronia-ts-doc/cpp/Files/interop__conversions_8h/#function-disposemultitimeseriesdata)**(multi_regular_time_series_data * d)<br>Helper function for C API interop conversions.  |
| void | **[DisposeTimeSeriesDimensionDescriptions](/uchronia-ts-doc/cpp/Files/interop__conversions_8h/#function-disposetimeseriesdimensiondescriptions)**(time_series_dimensions_description * d)<br>Helper function for C API interop conversions.  |


## Functions Documentation

### function CreateTimeSeries

```cpp
TimeSeries CreateTimeSeries(
    double * values,
    const regular_time_series_geometry & g
)
```

Helper function for C API interop conversions. 

### function CreateTimeSeries

```cpp
TimeSeries CreateTimeSeries(
    double * values,
    TS_GEOMETRY_PTR geom
)
```

Helper function for C API interop conversions. 

### function CreateTimeSeries

```cpp
TimeSeries CreateTimeSeries(
    const multi_regular_time_series_data & g
)
```

Helper function for C API interop conversions. 

### function ToTimeSeriesEnsemble

```cpp
TimeSeriesEnsemble< TimeSeries > ToTimeSeriesEnsemble(
    const multi_regular_time_series_data & rawData
)
```

Helper function for C API interop conversions. 

### function ToTimeSeriesEnsemblePtr

```cpp
TimeSeriesEnsemble< TimeSeries > * ToTimeSeriesEnsemblePtr(
    const multi_regular_time_series_data & rawData
)
```

Helper function for C API interop conversions. 

### function ToMultiTimeSeriesDataPtr

```cpp
multi_regular_time_series_data * ToMultiTimeSeriesDataPtr(
    const TimeSeriesEnsemble< TimeSeries > & mts
)
```

Helper function for C API interop conversions. 

### function ToMultiTimeSeriesDataPtr

```cpp
multi_regular_time_series_data * ToMultiTimeSeriesDataPtr(
    const TimeSeries & ts
)
```

Helper function for C API interop conversions. 

### function SingleTsPtrFromMultiTimeSeriesData

```cpp
TimeSeries * SingleTsPtrFromMultiTimeSeriesData(
    const multi_regular_time_series_data & ts
)
```

Helper function for C API interop conversions. 

### function MultiTsPtrFromMultiTimeSeriesData

```cpp
TimeSeriesEnsemble< TimeSeries > * MultiTsPtrFromMultiTimeSeriesData(
    const multi_regular_time_series_data & ts
)
```

Helper function for C API interop conversions. 

### function SingleTsFromMultiTimeSeriesData

```cpp
TimeSeries SingleTsFromMultiTimeSeriesData(
    const multi_regular_time_series_data & ts
)
```

Helper function for C API interop conversions. 

### function MultiTsFromMultiTimeSeriesData

```cpp
TimeSeriesEnsemble< TimeSeries > MultiTsFromMultiTimeSeriesData(
    const multi_regular_time_series_data & ts
)
```

Helper function for C API interop conversions. 

### function ToTimeSeriesDimensionDescriptions

```cpp
time_series_dimensions_description * ToTimeSeriesDimensionDescriptions(
    vector< DataDimensionDescriptor > & mts
)
```

Helper function for C API interop conversions. 

### function CopyToMultiTimeSeriesData

```cpp
void CopyToMultiTimeSeriesData(
    const TimeSeriesEnsemble< TimeSeries > & mts,
    multi_regular_time_series_data & result
)
```

Helper function for C API interop conversions. 

### function CopyToMultiTimeSeriesData

```cpp
void CopyToMultiTimeSeriesData(
    const TimeSeries & ts,
    multi_regular_time_series_data & result
)
```

Helper function for C API interop conversions. 

### function CopyFromMultiTimeSeriesData

```cpp
void CopyFromMultiTimeSeriesData(
    const multi_regular_time_series_data & interopdata,
    TimeSeries & ts
)
```

Helper function for C API interop conversions. 

### function CopyFromMultiTimeSeriesData

```cpp
void CopyFromMultiTimeSeriesData(
    const multi_regular_time_series_data & interopdata,
    TimeSeriesEnsemble< TimeSeries > & mts
)
```

Helper function for C API interop conversions. 

### function ToRawData

```cpp
double ** ToRawData(
    const TimeSeriesEnsemble< TimeSeries > & mts
)
```

Helper function for C API interop conversions. 

### function ToRawData

```cpp
double * ToRawData(
    const TimeSeries & ts
)
```

Helper function for C API interop conversions. 

### function DisposeMultiTimeSeriesData

```cpp
void DisposeMultiTimeSeriesData(
    multi_regular_time_series_data * d
)
```

Helper function for C API interop conversions. 

### function DisposeTimeSeriesDimensionDescriptions

```cpp
void DisposeTimeSeriesDimensionDescriptions(
    time_series_dimensions_description * d
)
```

Helper function for C API interop conversions. 



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

Updated on 2022-08-21 at 18:10:33 +1000
