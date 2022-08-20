---
title: datatypes::timeseries::TimeStepImplementation

---

# datatypes::timeseries::TimeStepImplementation






`#include <time_step_implementation.h>`

Inherited by [datatypes::timeseries::IrregularTimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/), [datatypes::timeseries::RegularTimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-~timestepimplementation)**() |
| virtual [TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-clone)**() =0 |
| virtual [TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Multiply](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-multiply)**(int mult) const =0 |
| virtual [TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Divide](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-divide)**(int divisor) const =0 |
| virtual [TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Multiply](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-multiply)**(double mult) const =0 |
| virtual bool | **[Equals](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-equals)**([TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * tsImpl) const =0 |
| virtual const ptime | **[AddIntSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-addintsteps)**(const ptime & startTimeStep, int n) const =0 |
| virtual const ptime | **[AddSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-addsteps)**(const ptime & startTimeStep, double mult) const =0 |
| virtual const time_duration | **[GetTimeStepDuration](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-gettimestepduration)**(const ptime & startTimeStep) const =0 |
| virtual const void | **[Increment](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-increment)**(ptime * t) const =0 |
| virtual const ptrdiff_t | **[GetUpperNumSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getuppernumsteps)**(const ptime & start, const ptime & end) const |
| virtual const ptrdiff_t | **[GetNumSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getnumsteps)**(const ptime & start, const ptime & end) const |
| virtual const ptrdiff_t | **[GetOffset](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getoffset)**(const ptime & start, const ptime & end) const |
| virtual bool | **[IsRegular](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-isregular)**() const =0 |
| virtual time_duration | **[GetRegularStepDuration](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getregularstepduration)**() const =0 |
| virtual std::string | **[GetName](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getname)**() const =0 |
| void | **[CheckIsDateTime](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-checkisdatetime)**(const ptime & instant) |

## Protected Functions

|                | Name           |
| -------------- | -------------- |
| virtual const double | **[GetLinearIndexing](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getlinearindexing)**(const ptime & start, const ptime & end) const =0 |

## Public Functions Documentation

### function ~TimeStepImplementation

```cpp
virtual ~TimeStepImplementation()
```


### function Clone

```cpp
virtual TimeStepImplementation * Clone() =0
```


**Reimplemented by**: [datatypes::timeseries::RegularTimeStepImplementation::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-clone), [datatypes::timeseries::MonthlyQppTimeStepImplementation::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-clone), [datatypes::timeseries::IrregularTimeStepImplementation::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-clone)


### function Multiply

```cpp
virtual TimeStepImplementation * Multiply(
    int mult
) const =0
```


**Reimplemented by**: [datatypes::timeseries::RegularTimeStepImplementation::Multiply](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-multiply), [datatypes::timeseries::IrregularTimeStepImplementation::Multiply](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-multiply)


### function Divide

```cpp
virtual TimeStepImplementation * Divide(
    int divisor
) const =0
```


**Reimplemented by**: [datatypes::timeseries::RegularTimeStepImplementation::Divide](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-divide), [datatypes::timeseries::IrregularTimeStepImplementation::Divide](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-divide)


### function Multiply

```cpp
virtual TimeStepImplementation * Multiply(
    double mult
) const =0
```


**Reimplemented by**: [datatypes::timeseries::RegularTimeStepImplementation::Multiply](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-multiply), [datatypes::timeseries::IrregularTimeStepImplementation::Multiply](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-multiply)


### function Equals

```cpp
virtual bool Equals(
    TimeStepImplementation * tsImpl
) const =0
```


**Reimplemented by**: [datatypes::timeseries::RegularTimeStepImplementation::Equals](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-equals), [datatypes::timeseries::MonthlyQppTimeStepImplementation::Equals](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-equals), [datatypes::timeseries::IrregularTimeStepImplementation::Equals](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-equals)


### function AddIntSteps

```cpp
virtual const ptime AddIntSteps(
    const ptime & startTimeStep,
    int n
) const =0
```


**Reimplemented by**: [datatypes::timeseries::RegularTimeStepImplementation::AddIntSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-addintsteps), [datatypes::timeseries::MonthlyQppTimeStepImplementation::AddIntSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-addintsteps), [datatypes::timeseries::IrregularTimeStepImplementation::AddIntSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-addintsteps)


### function AddSteps

```cpp
virtual const ptime AddSteps(
    const ptime & startTimeStep,
    double mult
) const =0
```


**Reimplemented by**: [datatypes::timeseries::RegularTimeStepImplementation::AddSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-addsteps), [datatypes::timeseries::MonthlyQppTimeStepImplementation::AddSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-addsteps), [datatypes::timeseries::IrregularTimeStepImplementation::AddSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-addsteps)


### function GetTimeStepDuration

```cpp
virtual const time_duration GetTimeStepDuration(
    const ptime & startTimeStep
) const =0
```


**Reimplemented by**: [datatypes::timeseries::RegularTimeStepImplementation::GetTimeStepDuration](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-gettimestepduration), [datatypes::timeseries::IrregularTimeStepImplementation::GetTimeStepDuration](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-gettimestepduration), [datatypes::timeseries::MonthlyQppTimeStepImplementation::GetTimeStepDuration](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-gettimestepduration)


### function Increment

```cpp
virtual const void Increment(
    ptime * t
) const =0
```


**Reimplemented by**: [datatypes::timeseries::RegularTimeStepImplementation::Increment](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-increment), [datatypes::timeseries::MonthlyQppTimeStepImplementation::Increment](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-increment), [datatypes::timeseries::IrregularTimeStepImplementation::Increment](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-increment)


### function GetUpperNumSteps

```cpp
virtual const ptrdiff_t GetUpperNumSteps(
    const ptime & start,
    const ptime & end
) const
```


### function GetNumSteps

```cpp
virtual const ptrdiff_t GetNumSteps(
    const ptime & start,
    const ptime & end
) const
```


### function GetOffset

```cpp
virtual const ptrdiff_t GetOffset(
    const ptime & start,
    const ptime & end
) const
```


### function IsRegular

```cpp
virtual bool IsRegular() const =0
```


**Reimplemented by**: [datatypes::timeseries::RegularTimeStepImplementation::IsRegular](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-isregular), [datatypes::timeseries::IrregularTimeStepImplementation::IsRegular](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-isregular)


### function GetRegularStepDuration

```cpp
virtual time_duration GetRegularStepDuration() const =0
```


**Reimplemented by**: [datatypes::timeseries::RegularTimeStepImplementation::GetRegularStepDuration](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-getregularstepduration), [datatypes::timeseries::IrregularTimeStepImplementation::GetRegularStepDuration](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-getregularstepduration)


### function GetName

```cpp
virtual std::string GetName() const =0
```


**Reimplemented by**: [datatypes::timeseries::RegularTimeStepImplementation::GetName](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-getname), [datatypes::timeseries::MonthlyQppTimeStepImplementation::GetName](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-getname), [datatypes::timeseries::IrregularTimeStepImplementation::GetName](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-getname)


### function CheckIsDateTime

```cpp
static void CheckIsDateTime(
    const ptime & instant
)
```


## Protected Functions Documentation

### function GetLinearIndexing

```cpp
virtual const double GetLinearIndexing(
    const ptime & start,
    const ptime & end
) const =0
```


**Reimplemented by**: [datatypes::timeseries::RegularTimeStepImplementation::GetLinearIndexing](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-getlinearindexing), [datatypes::timeseries::MonthlyQppTimeStepImplementation::GetLinearIndexing](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-getlinearindexing), [datatypes::timeseries::IrregularTimeStepImplementation::GetLinearIndexing](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-getlinearindexing)


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000