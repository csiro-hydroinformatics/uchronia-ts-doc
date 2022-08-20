---
title: datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore
summary: A time series store for unit tests. 

---

# datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore



A time series store for unit tests. 


`#include <datatypes_test_helpers.h>`

Inherits from [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore< double >](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/), [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore< T >](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/), [datatypes::timeseries::IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/), [datatypes::timeseries::TimeSeriesInfoProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/), [datatypes::timeseries::DataDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/)

## Public Types

|                | Name           |
| -------------- | -------------- |
| using double | **[T](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-t)**  |
| using [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< [T](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-t) >::[SeriesType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-seriestype) | **[SeriesType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-seriestype)**  |
| using [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< [T](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-t) >::[PtrSeriesType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrseriestype) | **[PtrSeriesType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrseriestype)**  |
| using [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< [T](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-t) >::[EnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ensembleptrtype) | **[EnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ensembleptrtype)**  |
| using [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< [T](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-t) >::[PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) | **[PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype)**  |
| using [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< [T](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-t) >::[TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-tseriesensembleptrtype) | **[TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-tseriesensembleptrtype)**  |
| using [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< [T](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-t) >::[PtrTSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrtseriesensembleptrtype) | **[PtrTSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrtseriesensembleptrtype)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[~TestTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-~testtimeseriesensembletimeseriesstore)**() |
| | **[TestTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-testtimeseriesensembletimeseriesstore)**(const string & id ="") |
| | **[TestTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-testtimeseriesensembletimeseriesstore)**(const [TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-tseriesensembleptrtype) & ensFts, const string & id ="") |
| virtual [PtrTSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrtseriesensembleptrtype) | **[GetSeries](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getseries)**(const string & dataId) |
| [PtrTSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrtseriesensembleptrtype) | **[GetSeriesTestBackend](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getseriestestbackend)**(const string & dataId) |
| [PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) | **[Read](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-read)**(const std::string & ensembleIdentifier) |
| virtual size_t | **[GetLength](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getlength)**() const |
| virtual ptime | **[GetStart](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getstart)**() const |
| virtual string | **[GetDataSummary](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getdatasummary)**() const |
| virtual vector< [DataDimensionDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) > | **[GetDataDimensionsDescription](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getdatadimensionsdescription)**() const |
| virtual [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetTimeStep](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-gettimestep)**() const |
| virtual bool | **[IsActive](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-isactive)**() |
| virtual void | **[Allocate](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-allocate)**(size_t length, [PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) value) |
| virtual void | **[AllocateValues](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-allocatevalues)**(const vector< [PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) > & values) |
| virtual void | **[SetSeries](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-setseries)**(const string & dataId, [PtrTSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrtseriesensembleptrtype) value) |
| virtual void | **[SetItem](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-setitem)**(const string & dataId, size_t index, [PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) value) |
| virtual void | **[SetItem](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-setitem)**(const string & dataId, size_t index, const [EnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ensembleptrtype) & value) |
| virtual void | **[SetLength](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-setlength)**(size_t ) |
| virtual void | **[SetStart](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-setstart)**(ptime ) |
| virtual void | **[SetTimeStep](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-settimestep)**(const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & ) |
| virtual [PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) | **[GetItem](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getitem)**(const string & dataId, size_t fcastIndex) override |
| virtual [PtrSeriesType](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#using-ptrseriestype) | **[GetItem](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getitem)**(const string & dataId, size_t fcastIndex, size_t ensIndex) override |
| virtual size_t | **[GetEnsembleSize](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getensemblesize)**(const string & dataId, size_t fcastIndex) const override |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore< double >](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~WritableTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-~writabletimeseriesensembletimeseriesstore)**() |

**Public Functions inherited from [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore< T >](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-~timeseriesensembletimeseriesstore)**() |
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


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getseries)


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


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetLength](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getlength)


### function GetStart

```cpp
virtual ptime GetStart() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getstart)


### function GetDataSummary

```cpp
virtual string GetDataSummary() const
```


**Reimplements**: [datatypes::timeseries::DataDescriptor::GetDataSummary](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatasummary)


### function GetDataDimensionsDescription

```cpp
virtual vector< DataDimensionDescriptor > GetDataDimensionsDescription() const
```


**Reimplements**: [datatypes::timeseries::DataDescriptor::GetDataDimensionsDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatadimensionsdescription)


### function GetTimeStep

```cpp
virtual TimeStep GetTimeStep() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-gettimestep)


### function IsActive

```cpp
virtual bool IsActive()
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::IsActive](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-isactive)


### function Allocate

```cpp
virtual void Allocate(
    size_t length,
    PtrEnsemblePtrType value
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::Allocate](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-allocate)


### function AllocateValues

```cpp
virtual void AllocateValues(
    const vector< PtrEnsemblePtrType > & values
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::AllocateValues](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-allocatevalues)


### function SetSeries

```cpp
virtual void SetSeries(
    const string & dataId,
    PtrTSeriesEnsemblePtrType value
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::SetSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-setseries)


### function SetItem

```cpp
virtual void SetItem(
    const string & dataId,
    size_t index,
    PtrEnsemblePtrType value
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::SetItem](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-setitem)


### function SetItem

```cpp
virtual void SetItem(
    const string & dataId,
    size_t index,
    const EnsemblePtrType & value
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::SetItem](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-setitem)


### function SetLength

```cpp
virtual void SetLength(
    size_t 
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::SetLength](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-setlength)


### function SetStart

```cpp
virtual void SetStart(
    ptime 
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::SetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-setstart)


### function SetTimeStep

```cpp
virtual void SetTimeStep(
    const TimeStep & 
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::SetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-settimestep)


### function GetItem

```cpp
virtual PtrEnsemblePtrType GetItem(
    const string & dataId,
    size_t fcastIndex
) override
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetItem](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getitem)


### function GetItem

```cpp
virtual PtrSeriesType GetItem(
    const string & dataId,
    size_t fcastIndex,
    size_t ensIndex
) override
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetItem](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getitem)


### function GetEnsembleSize

```cpp
virtual size_t GetEnsembleSize(
    const string & dataId,
    size_t fcastIndex
) const override
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetEnsembleSize](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getensemblesize)


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000