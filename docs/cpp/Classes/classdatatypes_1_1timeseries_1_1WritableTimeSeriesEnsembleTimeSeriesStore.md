---
title: datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore

---

# datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore



 [More...](#detailed-description)


`#include <time_series_store.hpp>`

Inherits from [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore< T >](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/), [datatypes::timeseries::IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/), [datatypes::timeseries::TimeSeriesInfoProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/), [datatypes::timeseries::DataDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/)

## Public Types

|                | Name           |
| -------------- | -------------- |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-seriestype) | **[SeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#using-seriestype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[PtrSeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrseriestype) | **[PtrSeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#using-ptrseriestype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[EnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ensembleptrtype) | **[EnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#using-ensembleptrtype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) | **[PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-tseriesensembleptrtype) | **[TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#using-tseriesensembleptrtype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[PtrTSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrtseriesensembleptrtype) | **[PtrTSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#using-ptrtseriesensembleptrtype)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual | **[~WritableTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-~writabletimeseriesensembletimeseriesstore)**() |
| virtual bool | **[IsActive](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-isactive)**() =0 |
| virtual void | **[Allocate](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-allocate)**(size_t length, [PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) value) =0 |
| void | **[AllocateValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-allocatevalues)**(size_t length, const [PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) * values) |
| virtual void | **[AllocateValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-allocatevalues)**(const vector< [PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) > & values) |
| virtual void | **[SetSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-setseries)**(const string & dataId, [PtrTSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrtseriesensembleptrtype) value) =0 |
| virtual void | **[SetItem](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-setitem)**(const string & dataId, size_t index, [PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) value) =0 |
| virtual void | **[SetItem](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-setitem)**(const string & dataId, size_t index, const [EnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ensembleptrtype) & value) =0 |
| virtual void | **[SetLength](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-setlength)**(size_t ) =0 |
| virtual void | **[SetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-setstart)**(ptime ) =0 |
| virtual void | **[SetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-settimestep)**(const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & ) =0 |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore< T >](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-~timeseriesensembletimeseriesstore)**() |
| virtual [PtrTSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrtseriesensembleptrtype) | **[GetSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getseries)**(const string & dataId) =0 |
| virtual [PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) | **[GetItem](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getitem)**(const string & dataId, size_t fcastIndex) |
| virtual [PtrSeriesType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrseriestype) | **[GetItem](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getitem)**(const string & dataId, size_t fcastIndex, size_t ensIndex) |
| virtual size_t | **[GetEnsembleSize](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getensemblesize)**(const string & dataId, size_t fcastIndex) const |
| virtual [PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) | **[Read](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-read)**(const string & ensembleIdentifier) =0 |
| virtual size_t | **[GetLength](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getlength)**() const =0 |
| virtual ptime | **[GetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getstart)**() const =0 |
| virtual [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-gettimestep)**() const =0 |
| virtual vector< string > | **[GetIdentifiers](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getidentifiers)**() const |

**Public Functions inherited from [datatypes::timeseries::IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-~identifiersprovider)**() |
| virtual vector< string > | **[GetIdentifiers](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-getidentifiers)**() const =0 |
| vector< string > | **[SplitHierarchicalIdentifier](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-splithierarchicalidentifier)**(const string & longId) |
| string | **[GetTopmostIdentifier](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-gettopmostidentifier)**(const string & longId) |
| void | **[CheckNotEmpty](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-checknotempty)**(const string & longId) |

**Public Functions inherited from [datatypes::timeseries::TimeSeriesInfoProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeSeriesInfoProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/#function-~timeseriesinfoprovider)**() |
| virtual size_t | **[GetLength](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/#function-getlength)**() const =0 |
| virtual [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/#function-gettimestep)**() const =0 |
| virtual ptime | **[GetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/#function-getstart)**() const =0 |

**Public Functions inherited from [datatypes::timeseries::DataDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/)**

|                | Name           |
| -------------- | -------------- |
| virtual string | **[GetDataSummary](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatasummary)**() const =0 |
| virtual vector< [DataDimensionDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) > | **[GetDataDimensionsDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatadimensionsdescription)**() const =0 |


## Detailed Description

```cpp
template <typename T >
class datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore;
```

## Public Types Documentation

### using SeriesType

```cpp
using datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore< T >::SeriesType =  typename CommonTypes<T>::SeriesType;
```


### using PtrSeriesType

```cpp
using datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore< T >::PtrSeriesType =  typename CommonTypes<T>::PtrSeriesType;
```


### using EnsemblePtrType

```cpp
using datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore< T >::EnsemblePtrType =  typename CommonTypes<T>::EnsemblePtrType;
```


### using PtrEnsemblePtrType

```cpp
using datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore< T >::PtrEnsemblePtrType =  typename CommonTypes<T>::PtrEnsemblePtrType;
```


### using TSeriesEnsemblePtrType

```cpp
using datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore< T >::TSeriesEnsemblePtrType =  typename CommonTypes<T>::TSeriesEnsemblePtrType;
```


### using PtrTSeriesEnsemblePtrType

```cpp
using datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore< T >::PtrTSeriesEnsemblePtrType =  typename CommonTypes<T>::PtrTSeriesEnsemblePtrType;
```


## Public Functions Documentation

### function ~WritableTimeSeriesEnsembleTimeSeriesStore

```cpp
inline virtual ~WritableTimeSeriesEnsembleTimeSeriesStore()
```


### function IsActive

```cpp
virtual bool IsActive() =0
```


**Reimplemented by**: [datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::IsActive](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-isactive), [datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore::IsActive](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-isactive)


### function Allocate

```cpp
virtual void Allocate(
    size_t length,
    PtrEnsemblePtrType value
) =0
```


**Reimplemented by**: [datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::Allocate](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-allocate), [datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore::Allocate](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-allocate)


### function AllocateValues

```cpp
inline void AllocateValues(
    size_t length,
    const PtrEnsemblePtrType * values
)
```


### function AllocateValues

```cpp
inline virtual void AllocateValues(
    const vector< PtrEnsemblePtrType > & values
)
```


**Reimplemented by**: [datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::AllocateValues](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-allocatevalues), [datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore::AllocateValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-allocatevalues)


### function SetSeries

```cpp
virtual void SetSeries(
    const string & dataId,
    PtrTSeriesEnsemblePtrType value
) =0
```


**Reimplemented by**: [datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::SetSeries](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-setseries), [datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore::SetSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-setseries)


### function SetItem

```cpp
virtual void SetItem(
    const string & dataId,
    size_t index,
    PtrEnsemblePtrType value
) =0
```


**Reimplemented by**: [datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::SetItem](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-setitem), [datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore::SetItem](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-setitem)


### function SetItem

```cpp
virtual void SetItem(
    const string & dataId,
    size_t index,
    const EnsemblePtrType & value
) =0
```


**Reimplemented by**: [datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::SetItem](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-setitem), [datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore::SetItem](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-setitem)


### function SetLength

```cpp
virtual void SetLength(
    size_t 
) =0
```


**Reimplemented by**: [datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore::SetLength](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-setlength), [datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::SetLength](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-setlength)


### function SetStart

```cpp
virtual void SetStart(
    ptime 
) =0
```


**Reimplemented by**: [datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore::SetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-setstart), [datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::SetStart](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-setstart)


### function SetTimeStep

```cpp
virtual void SetTimeStep(
    const TimeStep & 
) =0
```


**Reimplemented by**: [datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::SetTimeStep](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-settimestep), [datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore::SetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-settimestep)


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000