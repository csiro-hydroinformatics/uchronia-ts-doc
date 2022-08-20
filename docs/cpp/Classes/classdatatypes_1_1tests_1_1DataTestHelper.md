---
title: datatypes::tests::DataTestHelper

---

# datatypes::tests::DataTestHelper



 [More...](#detailed-description)


`#include <datatypes_test_helpers.hpp>`

## Public Types

|                | Name           |
| -------------- | -------------- |
| using typename [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[SeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-seriestype) | **[SeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-seriestype)**  |
| using typename [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[PtrSeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ptrseriestype) | **[PtrSeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ptrseriestype)**  |
| using typename [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[EnsembleType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ensembletype) | **[EnsembleType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ensembletype)**  |
| using typename [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[EnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ensembleptrtype) | **[EnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ensembleptrtype)**  |
| using typename [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ptrensembleptrtype) | **[PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ptrensembleptrtype)**  |
| using typename [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[TSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-tseriesensembleptrtype) | **[TSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-tseriesensembleptrtype)**  |
| using typename [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[PtrTSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ptrtseriesensembleptrtype) | **[PtrTSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ptrtseriesensembleptrtype)**  |
| typedef std::function< T(size_t, size_t, size_t)> | **[FullElementValueFunc](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-fullelementvaluefunc)**  |
| typedef std::function< T(size_t)> | **[ElementValueFunc](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-elementvaluefunc)**  |
| typedef std::function< [SeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-seriestype)(size_t)> | **[EnsembleValueFunc](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-ensemblevaluefunc)**  |
| typedef std::function< [EnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ensembleptrtype)(size_t)> | **[TsEnsembleValueFunc](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-tsensemblevaluefunc)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > | **[Create](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-create)**(T * data, int num, const ptime & start =ptime(date(2000, 1, 1)), const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =TimeStep::GetHourly()) |
| [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > | **[Ramp](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-ramp)**(int num, const ptime & start =ptime(date(2000, 1, 1)), double from =0.0, double increment =1.0) |
| [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > | **[Pulse](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-pulse)**(int length, T value =1, int firstPulse =0, int period =2, const ptime & start =ptime(date(2000, 1, 1)), const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =TimeStep::GetHourly()) |
| [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > | **[GetExpectedTestSingleTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-getexpectedtestsingletimeseries)**(size_t indexInEnsemble, size_t length =[kTimeSeriesLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#variable-ktimeserieslength), double constOffset =1, const ptime & startDate =[TEST_START_TIME](/uchronia-ts-doc/cpp/Files/datatypes__test__helpers_8hpp/#define-test-start-time), const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =TimeStep::GetHourly()) |
| T * | **[Seq](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-seq)**(T from, T by, size_t num) |
| vector< T > | **[SeqVec](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-seqvec)**(T from, T by, size_t num) |
| vector< T > | **[Rep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-rep)**(T value, size_t num) |
| vector< T > | **[Add](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-add)**(const vector< T > & a, const vector< T > & b) |
| vector< T > | **[Add](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-add)**(const vector< T > & a, const T & b) |
| vector< T > | **[Add](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-add)**(const T & a, const vector< T > & b) |
| vector< T > | **[Mult](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-mult)**(const vector< T > & a, const vector< T > & b) |
| vector< T > | **[Mult](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-mult)**(const vector< T > & a, const T & b) |
| vector< T > | **[Mult](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-mult)**(const T & a, const vector< T > & b) |
| vector< T > | **[Neg](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-neg)**(const vector< T > & a) |
| vector< T * > * | **[Seq](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-seq)**(T from, T by, size_t num, size_t vecSize) |
| void | **[DeleteElements](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-deleteelements)**(vector< T * > & vec) |
| bool | **[AreEqual](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-areequal)**([PtrSeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ptrseriestype) expected, [PtrSeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ptrseriestype) actual) |
| bool | **[AreEqual](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-areequal)**([PtrSeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ptrseriestype) actual, T expected) |
| T | **[DecimalRamp](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-decimalramp)**(size_t fcastIndex, size_t ensIndex, size_t seriesIndex) |
| [ElementValueFunc](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-elementvaluefunc) | **[CreateValueGen](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-createvaluegen)**(size_t fcastIndex, size_t ensIndex, [FullElementValueFunc](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-fullelementvaluefunc) ffun =&[DecimalRamp](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-decimalramp)) |
| T | **[Identity](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-identity)**(size_t i) |
| [EnsembleValueFunc](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-ensemblevaluefunc) | **[CreateTsGen](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-createtsgen)**(const ptime & start, size_t tsLength, size_t fcastIndex, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =TimeStep::GetHourly(), [FullElementValueFunc](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-fullelementvaluefunc) ffun =&[DecimalRamp](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-decimalramp)) |
| [TsEnsembleValueFunc](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-tsensemblevaluefunc) | **[CreateMtsGen](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-createmtsgen)**(size_t ensSize, size_t tsLength, const ptime & start =ptime(date(2000, 1, 1)), const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =TimeStep::GetDaily(), const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStepFcasts =TimeStep::GetHourly(), [FullElementValueFunc](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-fullelementvaluefunc) ffun =&[DecimalRamp](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-decimalramp), int forecastStartOffset =1) |
| [EnsembleValueFunc](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-ensemblevaluefunc) | **[DefaultTsGen](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-defaulttsgen)**() |
| [EnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ensembleptrtype) | **[CreateEnsembleTs](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-createensemblets)**(size_t ensSize, size_t length, const ptime & start, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep, size_t fcastIndex =0, [FullElementValueFunc](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-fullelementvaluefunc) ffun =&[DecimalRamp](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-decimalramp)) |
| [EnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-ensembleptrtype) | **[CreateEnsembleTs](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-createensemblets)**(size_t ensSize, size_t length, const ptime & start =ptime(date(2000, 1, 1)), const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =TimeStep::GetDaily(), [EnsembleValueFunc](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-ensemblevaluefunc) tsGen =[DefaultTsGen](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-defaulttsgen)()) |
| [TsEnsembleValueFunc](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-tsensemblevaluefunc) | **[DefaultMtsGen](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-defaultmtsgen)**() |
| [TSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-tseriesensembleptrtype) | **[CreateTsEnsembleTs](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-createtsensemblets)**(size_t length, const ptime & start =ptime(date(2000, 1, 1)), const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =TimeStep::GetDaily(), [TsEnsembleValueFunc](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-tsensemblevaluefunc) mtsGen =[DefaultMtsGen](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-defaultmtsgen)()) |
| [TSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#using-tseriesensembleptrtype) | **[CreateTsEnsembleTs](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-createtsensemblets)**(size_t length, size_t ensSize, size_t tsLength, const ptime & start =ptime(date(2000, 1, 1)), const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep =TimeStep::GetDaily(), const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStepFcasts =TimeStep::GetHourly(), [FullElementValueFunc](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#typedef-fullelementvaluefunc) ffun =&[DecimalRamp](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#function-decimalramp), int forecastStartOffset =1) |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| const size_t | **[kTimeSeriesLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/#variable-ktimeserieslength)**  |

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

Updated on 2022-08-20 at 19:28:22 +1000