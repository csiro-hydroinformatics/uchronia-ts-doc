---
title: datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore
summary: A time series store for unit tests. 

---

# datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore



A time series store for unit tests. 


`#include <datatypes_test_helpers.h>`

Inherits from [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/), [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore< T >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/), [datatypes::timeseries::IdentifiersProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/), [datatypes::timeseries::TimeSeriesInfoProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/), [datatypes::timeseries::DataDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/)

## Public Types

|                | Name           |
| -------------- | -------------- |
| using double | **[T](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-t)**  |
| using [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< [T](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-t) >::[SeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-seriestype) | **[SeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-seriestype)**  |
| using [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< [T](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-t) >::[PtrSeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrseriestype) | **[PtrSeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrseriestype)**  |
| using [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< [T](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-t) >::[EnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ensembleptrtype) | **[EnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ensembleptrtype)**  |
| using [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< [T](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-t) >::[PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) | **[PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype)**  |
| using [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< [T](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-t) >::[TSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-tseriesensembleptrtype) | **[TSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-tseriesensembleptrtype)**  |
| using [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< [T](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-t) >::[PtrTSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrtseriesensembleptrtype) | **[PtrTSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrtseriesensembleptrtype)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[~TestTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-~testtimeseriesensembletimeseriesstore)**() |
| | **[TestTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-testtimeseriesensembletimeseriesstore)**(const string & id ="") |
| | **[TestTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-testtimeseriesensembletimeseriesstore)**(const [TSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-tseriesensembleptrtype) & ensFts, const string & id ="") |
| virtual [PtrTSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrtseriesensembleptrtype) | **[GetSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getseries)**(const string & dataId) |
| [PtrTSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrtseriesensembleptrtype) | **[GetSeriesTestBackend](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getseriestestbackend)**(const string & dataId) |
| [PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) | **[Read](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-read)**(const std::string & ensembleIdentifier) |
| virtual size_t | **[GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getlength)**() const |
| virtual ptime | **[GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getstart)**() const |
| virtual string | **[GetDataSummary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getdatasummary)**() const |
| virtual vector< [DataDimensionDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) > | **[GetDataDimensionsDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getdatadimensionsdescription)**() const |
| virtual [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-gettimestep)**() const |
| virtual bool | **[IsActive](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-isactive)**() |
| virtual void | **[Allocate](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-allocate)**(size_t length, [PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) value) |
| virtual void | **[AllocateValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-allocatevalues)**(const vector< [PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) > & values) |
| virtual void | **[SetSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-setseries)**(const string & dataId, [PtrTSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrtseriesensembleptrtype) value) |
| virtual void | **[SetItem](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-setitem)**(const string & dataId, size_t index, [PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) value) |
| virtual void | **[SetItem](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-setitem)**(const string & dataId, size_t index, const [EnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ensembleptrtype) & value) |
| virtual void | **[SetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-setlength)**(size_t ) |
| virtual void | **[SetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-setstart)**(ptime ) |
| virtual void | **[SetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-settimestep)**(const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & ) |
| virtual [PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) | **[GetItem](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getitem)**(const string & dataId, size_t fcastIndex) override |
| virtual [PtrSeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrseriestype) | **[GetItem](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getitem)**(const string & dataId, size_t fcastIndex, size_t ensIndex) override |
| virtual size_t | **[GetEnsembleSize](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getensemblesize)**(const string & dataId, size_t fcastIndex) const override |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~WritableTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-~writabletimeseriesensembletimeseriesstore)**() |

**Public Functions inherited from [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore< T >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-~timeseriesensembletimeseriesstore)**() |
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


## Public Types Documentation

### using T

```cpp
using datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::T =  double;
```


### using SeriesType

```cpp
using datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::SeriesType =  CommonTypes<T>::SeriesType;
```


### using PtrSeriesType

```cpp
using datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::PtrSeriesType =  CommonTypes<T>::PtrSeriesType;
```


### using EnsemblePtrType

```cpp
using datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::EnsemblePtrType =  CommonTypes<T>::EnsemblePtrType;
```


### using PtrEnsemblePtrType

```cpp
using datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::PtrEnsemblePtrType =  CommonTypes<T>::PtrEnsemblePtrType;
```


### using TSeriesEnsemblePtrType

```cpp
using datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::TSeriesEnsemblePtrType =  CommonTypes<T>::TSeriesEnsemblePtrType;
```


### using PtrTSeriesEnsemblePtrType

```cpp
using datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::PtrTSeriesEnsemblePtrType =  CommonTypes<T>::PtrTSeriesEnsemblePtrType;
```


## Public Functions Documentation

### function ~TestTimeSeriesEnsembleTimeSeriesStore

```cpp
~TestTimeSeriesEnsembleTimeSeriesStore()
```


### function TestTimeSeriesEnsembleTimeSeriesStore

```cpp
TestTimeSeriesEnsembleTimeSeriesStore(
    const string & id =""
)
```


### function TestTimeSeriesEnsembleTimeSeriesStore

```cpp
TestTimeSeriesEnsembleTimeSeriesStore(
    const TSeriesEnsemblePtrType & ensFts,
    const string & id =""
)
```


### function GetSeries

```cpp
virtual PtrTSeriesEnsemblePtrType GetSeries(
    const string & dataId
)
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getseries)


### function GetSeriesTestBackend

```cpp
PtrTSeriesEnsemblePtrType GetSeriesTestBackend(
    const string & dataId
)
```


### function Read

```cpp
PtrEnsemblePtrType Read(
    const std::string & ensembleIdentifier
)
```


### function GetLength

```cpp
virtual size_t GetLength() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getlength)


### function GetStart

```cpp
virtual ptime GetStart() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getstart)


### function GetDataSummary

```cpp
virtual string GetDataSummary() const
```


**Reimplements**: [datatypes::timeseries::DataDescriptor::GetDataSummary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatasummary)


### function GetDataDimensionsDescription

```cpp
virtual vector< DataDimensionDescriptor > GetDataDimensionsDescription() const
```


**Reimplements**: [datatypes::timeseries::DataDescriptor::GetDataDimensionsDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatadimensionsdescription)


### function GetTimeStep

```cpp
virtual TimeStep GetTimeStep() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-gettimestep)


### function IsActive

```cpp
virtual bool IsActive()
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::IsActive](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-isactive)


### function Allocate

```cpp
virtual void Allocate(
    size_t length,
    PtrEnsemblePtrType value
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::Allocate](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-allocate)


### function AllocateValues

```cpp
virtual void AllocateValues(
    const vector< PtrEnsemblePtrType > & values
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::AllocateValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-allocatevalues)


### function SetSeries

```cpp
virtual void SetSeries(
    const string & dataId,
    PtrTSeriesEnsemblePtrType value
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::SetSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-setseries)


### function SetItem

```cpp
virtual void SetItem(
    const string & dataId,
    size_t index,
    PtrEnsemblePtrType value
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::SetItem](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-setitem)


### function SetItem

```cpp
virtual void SetItem(
    const string & dataId,
    size_t index,
    const EnsemblePtrType & value
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::SetItem](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-setitem)


### function SetLength

```cpp
virtual void SetLength(
    size_t 
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::SetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-setlength)


### function SetStart

```cpp
virtual void SetStart(
    ptime 
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::SetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-setstart)


### function SetTimeStep

```cpp
virtual void SetTimeStep(
    const TimeStep & 
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::SetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-settimestep)


### function GetItem

```cpp
virtual PtrEnsemblePtrType GetItem(
    const string & dataId,
    size_t fcastIndex
) override
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetItem](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getitem)


### function GetItem

```cpp
virtual PtrSeriesType GetItem(
    const string & dataId,
    size_t fcastIndex,
    size_t ensIndex
) override
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetItem](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getitem)


### function GetEnsembleSize

```cpp
virtual size_t GetEnsembleSize(
    const string & dataId,
    size_t fcastIndex
) const override
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetEnsembleSize](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getensemblesize)


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000