---
title: datatypes::timeseries::MultiFileTimeSeriesEnsembleTimeSeriesStore
summary: An implementation of TimeSeriesEnsembleTimeSeriesStore such that the content of a time series is spread amongst several files. 

---

# datatypes::timeseries::MultiFileTimeSeriesEnsembleTimeSeriesStore



An implementation of [TimeSeriesEnsembleTimeSeriesStore]() such that the content of a time series is spread amongst several files.  [More...](#detailed-description)


`#include <time_series_io.hpp>`

Inherits from [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore< T >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/), [datatypes::timeseries::IdentifiersProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/), [datatypes::timeseries::TimeSeriesInfoProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/), [datatypes::timeseries::DataDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/)

## Public Types

|                | Name           |
| -------------- | -------------- |
| using typename [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[SeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#using-seriestype) | **[SeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#using-seriestype)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[MultiFileTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-multifiletimeseriesensembletimeseriesstore)**()<br>Default constructor. Needed for class member properties; should otherwise not be used.  |
| | **[MultiFileTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-multifiletimeseriesensembletimeseriesstore)**(const string & forecastDataFiles, const string & varName, const string & varIdentifier, int index, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep, const ptime & start, int length, int ensembleSize, int ensembleLength, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & ensembleTimeStep) |
| virtual | **[~MultiFileTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-~multifiletimeseriesensembletimeseriesstore)**() |
| virtual [EnsembleForecastTimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-ensembleforecasttimeseries)< [SeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#using-seriestype) > * | **[GetSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-getseries)**(const string & dataId) |
| virtual [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [SeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#using-seriestype) * > * | **[Read](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-read)**(const string & fileIdentifier) override |
| [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [SeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#using-seriestype) * > * | **[ReadAt](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-readat)**(size_t index) const |
| virtual size_t | **[GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-getlength)**() const |
| virtual [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-gettimestep)**() const |
| virtual ptime | **[GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-getstart)**() const |
| ptime | **[GetEnd](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-getend)**() const |
| string | **[ShortFileNamePattern](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-shortfilenamepattern)**() const |
| virtual string | **[GetDataSummary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-getdatasummary)**() const |
| virtual vector< [DataDimensionDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) > | **[GetDataDimensionsDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-getdatadimensionsdescription)**() const |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| string | **[DatePattern](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#variable-datepattern)**  |
| string | **[FileNamePattern](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#variable-filenamepattern)**  |

## Additional inherited members

**Public Types inherited from [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore< T >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)**

|                | Name           |
| -------------- | -------------- |
| using typename [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[PtrSeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrseriestype) | **[PtrSeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrseriestype)**  |
| using typename [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[EnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ensembleptrtype) | **[EnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ensembleptrtype)**  |
| using typename [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) | **[PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype)**  |
| using typename [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[TSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-tseriesensembleptrtype) | **[TSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-tseriesensembleptrtype)**  |
| using typename [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[PtrTSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrtseriesensembleptrtype) | **[PtrTSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrtseriesensembleptrtype)**  |

**Public Functions inherited from [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore< T >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-~timeseriesensembletimeseriesstore)**() |
| virtual [PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) | **[GetItem](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getitem)**(const string & dataId, size_t fcastIndex) |
| virtual [PtrSeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrseriestype) | **[GetItem](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getitem)**(const string & dataId, size_t fcastIndex, size_t ensIndex) |
| virtual size_t | **[GetEnsembleSize](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getensemblesize)**(const string & dataId, size_t fcastIndex) const |
| virtual vector< string > | **[GetIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getidentifiers)**() const |

**Public Functions inherited from [datatypes::timeseries::IdentifiersProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~IdentifiersProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-~identifiersprovider)**() |
| virtual vector< string > | **[GetIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-getidentifiers)**() const =0 |
| vector< string > | **[SplitHierarchicalIdentifier](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-splithierarchicalidentifier)**(const string & longId) |
| string | **[GetTopmostIdentifier](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-gettopmostidentifier)**(const string & longId) |
| void | **[CheckNotEmpty](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-checknotempty)**(const string & longId) |

**Public Functions inherited from [datatypes::timeseries::TimeSeriesInfoProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeSeriesInfoProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/#function-~timeseriesinfoprovider)**() |


## Detailed Description

```cpp
template <typename T >
class datatypes::timeseries::MultiFileTimeSeriesEnsembleTimeSeriesStore;
```

An implementation of [TimeSeriesEnsembleTimeSeriesStore]() such that the content of a time series is spread amongst several files. 

**Template Parameters**: 

  * **T** The type of each data item this can handle. 

## Public Types Documentation

### using SeriesType

```cpp
using datatypes::timeseries::MultiFileTimeSeriesEnsembleTimeSeriesStore< T >::SeriesType =  typename CommonTypes<T>::SeriesType;
```


## Public Functions Documentation

### function MultiFileTimeSeriesEnsembleTimeSeriesStore

```cpp
inline MultiFileTimeSeriesEnsembleTimeSeriesStore()
```

Default constructor. Needed for class member properties; should otherwise not be used. 

### function MultiFileTimeSeriesEnsembleTimeSeriesStore

```cpp
inline MultiFileTimeSeriesEnsembleTimeSeriesStore(
    const string & forecastDataFiles,
    const string & varName,
    const string & varIdentifier,
    int index,
    const TimeStep & timeStep,
    const ptime & start,
    int length,
    int ensembleSize,
    int ensembleLength,
    const TimeStep & ensembleTimeStep
)
```


### function ~MultiFileTimeSeriesEnsembleTimeSeriesStore

```cpp
inline virtual ~MultiFileTimeSeriesEnsembleTimeSeriesStore()
```


### function GetSeries

```cpp
inline virtual EnsembleForecastTimeSeries< SeriesType > * GetSeries(
    const string & dataId
)
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getseries)


### function Read

```cpp
inline virtual MultiTimeSeries< SeriesType * > * Read(
    const string & fileIdentifier
) override
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::Read](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-read)


### function ReadAt

```cpp
inline MultiTimeSeries< SeriesType * > * ReadAt(
    size_t index
) const
```


### function GetLength

```cpp
inline virtual size_t GetLength() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getlength)


### function GetTimeStep

```cpp
inline virtual TimeStep GetTimeStep() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-gettimestep)


### function GetStart

```cpp
inline virtual ptime GetStart() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getstart)


### function GetEnd

```cpp
inline ptime GetEnd() const
```


### function ShortFileNamePattern

```cpp
inline string ShortFileNamePattern() const
```


### function GetDataSummary

```cpp
inline virtual string GetDataSummary() const
```


**Reimplements**: [datatypes::timeseries::DataDescriptor::GetDataSummary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatasummary)


### function GetDataDimensionsDescription

```cpp
inline virtual vector< DataDimensionDescriptor > GetDataDimensionsDescription() const
```


**Reimplements**: [datatypes::timeseries::DataDescriptor::GetDataDimensionsDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatadimensionsdescription)


## Public Attributes Documentation

### variable DatePattern

```cpp
string DatePattern = "YYYYMMDD";
```


### variable FileNamePattern

```cpp
string FileNamePattern = datatypes::io::IoHelper::DefaultFilePattern;
```


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000