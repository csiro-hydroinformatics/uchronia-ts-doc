---
title: datatypes::tests::DataTestHelper

---

# datatypes::tests::DataTestHelper



 [More...](#detailed-description)


`#include <datatypes_test_helpers.hpp>`

## Public Types

|                | Name           |
| -------------- | -------------- |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[SeriesType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-seriestype) | **[SeriesType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-seriestype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[PtrSeriesType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ptrseriestype) | **[PtrSeriesType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ptrseriestype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[EnsembleType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ensembletype) | **[EnsembleType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ensembletype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[EnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ensembleptrtype) | **[EnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ensembleptrtype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ptrensembleptrtype) | **[PtrEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ptrensembleptrtype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-tseriesensembleptrtype) | **[TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-tseriesensembleptrtype)**  |
| using typename [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[PtrTSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ptrtseriesensembleptrtype) | **[PtrTSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ptrtseriesensembleptrtype)**  |
| typedef std::function< T(size_t, size_t, size_t)> | **[FullElementValueFunc](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-fullelementvaluefunc)**  |
| typedef std::function< T(size_t)> | **[ElementValueFunc](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-elementvaluefunc)**  |
| typedef std::function< [SeriesType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-seriestype)(size_t)> | **[EnsembleValueFunc](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-ensemblevaluefunc)**  |
| typedef std::function< [EnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ensembleptrtype)(size_t)> | **[TsEnsembleValueFunc](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-tsensemblevaluefunc)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > | **[Create](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-create)**(T * data, int num, const ptime & start =ptime(date(2000, 1, 1)), const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =TimeStep::GetHourly()) |
| [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > | **[Ramp](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-ramp)**(int num, const ptime & start =ptime(date(2000, 1, 1)), double from =0.0, double increment =1.0) |
| [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > | **[Pulse](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-pulse)**(int length, T value =1, int firstPulse =0, int period =2, const ptime & start =ptime(date(2000, 1, 1)), const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =TimeStep::GetHourly()) |
| [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > | **[GetExpectedTestSingleTimeSeries](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-getexpectedtestsingletimeseries)**(size_t indexInEnsemble, size_t length =[kTimeSeriesLength](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#variable-ktimeserieslength), double constOffset =1, const ptime & startDate =[TEST_START_TIME](/cpp/Files/datatypes__test__helpers_8hpp/#define-test-start-time), const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =TimeStep::GetHourly()) |
| T * | **[Seq](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-seq)**(T from, T by, size_t num) |
| vector< T > | **[SeqVec](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-seqvec)**(T from, T by, size_t num) |
| vector< T > | **[Rep](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-rep)**(T value, size_t num) |
| vector< T > | **[Add](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-add)**(const vector< T > & a, const vector< T > & b) |
| vector< T > | **[Add](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-add)**(const vector< T > & a, const T & b) |
| vector< T > | **[Add](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-add)**(const T & a, const vector< T > & b) |
| vector< T > | **[Mult](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-mult)**(const vector< T > & a, const vector< T > & b) |
| vector< T > | **[Mult](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-mult)**(const vector< T > & a, const T & b) |
| vector< T > | **[Mult](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-mult)**(const T & a, const vector< T > & b) |
| vector< T > | **[Neg](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-neg)**(const vector< T > & a) |
| vector< T * > * | **[Seq](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-seq)**(T from, T by, size_t num, size_t vecSize) |
| void | **[DeleteElements](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-deleteelements)**(vector< T * > & vec) |
| bool | **[AreEqual](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-areequal)**([PtrSeriesType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ptrseriestype) expected, [PtrSeriesType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ptrseriestype) actual) |
| bool | **[AreEqual](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-areequal)**([PtrSeriesType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ptrseriestype) actual, T expected) |
| T | **[DecimalRamp](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-decimalramp)**(size_t fcastIndex, size_t ensIndex, size_t seriesIndex) |
| [ElementValueFunc](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-elementvaluefunc) | **[CreateValueGen](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-createvaluegen)**(size_t fcastIndex, size_t ensIndex, [FullElementValueFunc](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-fullelementvaluefunc) ffun =&[DecimalRamp](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-decimalramp)) |
| T | **[Identity](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-identity)**(size_t i) |
| [EnsembleValueFunc](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-ensemblevaluefunc) | **[CreateTsGen](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-createtsgen)**(const ptime & start, size_t tsLength, size_t fcastIndex, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =TimeStep::GetHourly(), [FullElementValueFunc](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-fullelementvaluefunc) ffun =&[DecimalRamp](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-decimalramp)) |
| [TsEnsembleValueFunc](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-tsensemblevaluefunc) | **[CreateMtsGen](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-createmtsgen)**(size_t ensSize, size_t tsLength, const ptime & start =ptime(date(2000, 1, 1)), const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =TimeStep::GetDaily(), const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStepFcasts =TimeStep::GetHourly(), [FullElementValueFunc](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-fullelementvaluefunc) ffun =&[DecimalRamp](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-decimalramp), int forecastStartOffset =1) |
| [EnsembleValueFunc](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-ensemblevaluefunc) | **[DefaultTsGen](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-defaulttsgen)**() |
| [EnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ensembleptrtype) | **[CreateEnsembleTs](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-createensemblets)**(size_t ensSize, size_t length, const ptime & start, const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep, size_t fcastIndex =0, [FullElementValueFunc](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-fullelementvaluefunc) ffun =&[DecimalRamp](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-decimalramp)) |
| [EnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ensembleptrtype) | **[CreateEnsembleTs](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-createensemblets)**(size_t ensSize, size_t length, const ptime & start =ptime(date(2000, 1, 1)), const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =TimeStep::GetDaily(), [EnsembleValueFunc](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-ensemblevaluefunc) tsGen =[DefaultTsGen](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-defaulttsgen)()) |
| [TsEnsembleValueFunc](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-tsensemblevaluefunc) | **[DefaultMtsGen](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-defaultmtsgen)**() |
| [TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-tseriesensembleptrtype) | **[CreateTsEnsembleTs](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-createtsensemblets)**(size_t length, const ptime & start =ptime(date(2000, 1, 1)), const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =TimeStep::GetDaily(), [TsEnsembleValueFunc](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-tsensemblevaluefunc) mtsGen =[DefaultMtsGen](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-defaultmtsgen)()) |
| [TSeriesEnsemblePtrType](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-tseriesensembleptrtype) | **[CreateTsEnsembleTs](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-createtsensemblets)**(size_t length, size_t ensSize, size_t tsLength, const ptime & start =ptime(date(2000, 1, 1)), const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =TimeStep::GetDaily(), const [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStepFcasts =TimeStep::GetHourly(), [FullElementValueFunc](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-fullelementvaluefunc) ffun =&[DecimalRamp](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-decimalramp), int forecastStartOffset =1) |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| const size_t | **[kTimeSeriesLength](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#variable-ktimeserieslength)**  |

## Detailed Description

```cpp
template <typename T >
class datatypes::tests::DataTestHelper;
```

## Public Types Documentation

### using SeriesType

```cpp
using datatypes::tests::DataTestHelper< T >::SeriesType =  typename CommonTypes<T>::SeriesType;
```


### using PtrSeriesType

```cpp
using datatypes::tests::DataTestHelper< T >::PtrSeriesType =  typename CommonTypes<T>::PtrSeriesType;
```


### using EnsembleType

```cpp
using datatypes::tests::DataTestHelper< T >::EnsembleType =  typename CommonTypes<T>::EnsembleType;
```


### using EnsemblePtrType

```cpp
using datatypes::tests::DataTestHelper< T >::EnsemblePtrType =  typename CommonTypes<T>::EnsemblePtrType;
```


### using PtrEnsemblePtrType

```cpp
using datatypes::tests::DataTestHelper< T >::PtrEnsemblePtrType =  typename CommonTypes<T>::PtrEnsemblePtrType;
```


### using TSeriesEnsemblePtrType

```cpp
using datatypes::tests::DataTestHelper< T >::TSeriesEnsemblePtrType =  typename CommonTypes<T>::TSeriesEnsemblePtrType;
```


### using PtrTSeriesEnsemblePtrType

```cpp
using datatypes::tests::DataTestHelper< T >::PtrTSeriesEnsemblePtrType =  typename CommonTypes<T>::PtrTSeriesEnsemblePtrType;
```


### typedef FullElementValueFunc

```cpp
typedef std::function<T(size_t , size_t , size_t )> datatypes::tests::DataTestHelper< T >::FullElementValueFunc;
```


### typedef ElementValueFunc

```cpp
typedef std::function<T(size_t )> datatypes::tests::DataTestHelper< T >::ElementValueFunc;
```


### typedef EnsembleValueFunc

```cpp
typedef std::function<SeriesType(size_t )> datatypes::tests::DataTestHelper< T >::EnsembleValueFunc;
```


### typedef TsEnsembleValueFunc

```cpp
typedef std::function<EnsemblePtrType(size_t )> datatypes::tests::DataTestHelper< T >::TsEnsembleValueFunc;
```


## Public Functions Documentation

### function Create

```cpp
static TTimeSeries< T > Create(
    T * data,
    int num,
    const ptime & start =ptime(date(2000, 1, 1)),
    const TimeStep & timeStep =TimeStep::GetHourly()
)
```


### function Ramp

```cpp
static TTimeSeries< T > Ramp(
    int num,
    const ptime & start =ptime(date(2000, 1, 1)),
    double from =0.0,
    double increment =1.0
)
```


### function Pulse

```cpp
static TTimeSeries< T > Pulse(
    int length,
    T value =1,
    int firstPulse =0,
    int period =2,
    const ptime & start =ptime(date(2000, 1, 1)),
    const TimeStep & timeStep =TimeStep::GetHourly()
)
```


### function GetExpectedTestSingleTimeSeries

```cpp
static TTimeSeries< T > GetExpectedTestSingleTimeSeries(
    size_t indexInEnsemble,
    size_t length =kTimeSeriesLength,
    double constOffset =1,
    const ptime & startDate =TEST_START_TIME,
    const TimeStep & timeStep =TimeStep::GetHourly()
)
```


### function Seq

```cpp
static T * Seq(
    T from,
    T by,
    size_t num
)
```


### function SeqVec

```cpp
static vector< T > SeqVec(
    T from,
    T by,
    size_t num
)
```


### function Rep

```cpp
static vector< T > Rep(
    T value,
    size_t num
)
```


### function Add

```cpp
static vector< T > Add(
    const vector< T > & a,
    const vector< T > & b
)
```


### function Add

```cpp
static vector< T > Add(
    const vector< T > & a,
    const T & b
)
```


### function Add

```cpp
static vector< T > Add(
    const T & a,
    const vector< T > & b
)
```


### function Mult

```cpp
static vector< T > Mult(
    const vector< T > & a,
    const vector< T > & b
)
```


### function Mult

```cpp
static vector< T > Mult(
    const vector< T > & a,
    const T & b
)
```


### function Mult

```cpp
static vector< T > Mult(
    const T & a,
    const vector< T > & b
)
```


### function Neg

```cpp
static vector< T > Neg(
    const vector< T > & a
)
```


### function Seq

```cpp
static vector< T * > * Seq(
    T from,
    T by,
    size_t num,
    size_t vecSize
)
```


### function DeleteElements

```cpp
static void DeleteElements(
    vector< T * > & vec
)
```


### function AreEqual

```cpp
static bool AreEqual(
    PtrSeriesType expected,
    PtrSeriesType actual
)
```


### function AreEqual

```cpp
static bool AreEqual(
    PtrSeriesType actual,
    T expected
)
```


### function DecimalRamp

```cpp
static inline T DecimalRamp(
    size_t fcastIndex,
    size_t ensIndex,
    size_t seriesIndex
)
```


### function CreateValueGen

```cpp
static inline ElementValueFunc CreateValueGen(
    size_t fcastIndex,
    size_t ensIndex,
    FullElementValueFunc ffun =&DecimalRamp
)
```


### function Identity

```cpp
static inline T Identity(
    size_t i
)
```


### function CreateTsGen

```cpp
static inline EnsembleValueFunc CreateTsGen(
    const ptime & start,
    size_t tsLength,
    size_t fcastIndex,
    const TimeStep & timeStep =TimeStep::GetHourly(),
    FullElementValueFunc ffun =&DecimalRamp
)
```


### function CreateMtsGen

```cpp
static inline TsEnsembleValueFunc CreateMtsGen(
    size_t ensSize,
    size_t tsLength,
    const ptime & start =ptime(date(2000, 1, 1)),
    const TimeStep & timeStep =TimeStep::GetDaily(),
    const TimeStep & timeStepFcasts =TimeStep::GetHourly(),
    FullElementValueFunc ffun =&DecimalRamp,
    int forecastStartOffset =1
)
```


### function DefaultTsGen

```cpp
static inline EnsembleValueFunc DefaultTsGen()
```


### function CreateEnsembleTs

```cpp
static inline EnsemblePtrType CreateEnsembleTs(
    size_t ensSize,
    size_t length,
    const ptime & start,
    const TimeStep & timeStep,
    size_t fcastIndex =0,
    FullElementValueFunc ffun =&DecimalRamp
)
```


### function CreateEnsembleTs

```cpp
static inline EnsemblePtrType CreateEnsembleTs(
    size_t ensSize,
    size_t length,
    const ptime & start =ptime(date(2000, 1, 1)),
    const TimeStep & timeStep =TimeStep::GetDaily(),
    EnsembleValueFunc tsGen =DefaultTsGen()
)
```


### function DefaultMtsGen

```cpp
static inline TsEnsembleValueFunc DefaultMtsGen()
```


### function CreateTsEnsembleTs

```cpp
static inline TSeriesEnsemblePtrType CreateTsEnsembleTs(
    size_t length,
    const ptime & start =ptime(date(2000, 1, 1)),
    const TimeStep & timeStep =TimeStep::GetDaily(),
    TsEnsembleValueFunc mtsGen =DefaultMtsGen()
)
```


### function CreateTsEnsembleTs

```cpp
static inline TSeriesEnsemblePtrType CreateTsEnsembleTs(
    size_t length,
    size_t ensSize,
    size_t tsLength,
    const ptime & start =ptime(date(2000, 1, 1)),
    const TimeStep & timeStep =TimeStep::GetDaily(),
    const TimeStep & timeStepFcasts =TimeStep::GetHourly(),
    FullElementValueFunc ffun =&DecimalRamp,
    int forecastStartOffset =1
)
```


## Public Attributes Documentation

### variable kTimeSeriesLength

```cpp
static const size_t kTimeSeriesLength = 48;
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000