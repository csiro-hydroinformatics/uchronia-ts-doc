---
title: datatypes::timeseries::IrregularTimeStepImplementation

---

# datatypes::timeseries::IrregularTimeStepImplementation






`#include <time_step_implementation.h>`

Inherits from [datatypes::timeseries::TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/)

Inherited by [datatypes::timeseries::MonthlyQppTimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual | **[~IrregularTimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-~irregulartimestepimplementation)**() |
| virtual [TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-clone)**() =0 |
| virtual bool | **[Equals](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-equals)**([TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * tsImpl) const =0 |
| virtual [TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Multiply](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-multiply)**(int mult) const |
| virtual [TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Multiply](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-multiply)**(double mult) const |
| virtual [TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Divide](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-divide)**(int divisor) const |
| virtual const ptime | **[AddIntSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-addintsteps)**(const ptime & startTimeStep, int n) const =0 |
| virtual const ptime | **[AddSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-addsteps)**(const ptime & startTimeStep, double mult) const =0 |
| virtual const time_duration | **[GetTimeStepDuration](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-gettimestepduration)**(const ptime & startTimeStep) const |
| virtual const void | **[Increment](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-increment)**(ptime * t) const =0 |
| virtual bool | **[IsRegular](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-isregular)**() const |
| virtual time_duration | **[GetRegularStepDuration](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-getregularstepduration)**() const |
| virtual std::string | **[GetName](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-getname)**() const =0 |

## Protected Functions

|                | Name           |
| -------------- | -------------- |
| virtual const double | **[GetLinearIndexing](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-getlinearindexing)**(const ptime & start, const ptime & end) const =0 |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-~timestepimplementation)**() |
| virtual const ptrdiff_t | **[GetUpperNumSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getuppernumsteps)**(const ptime & start, const ptime & end) const |
| virtual const ptrdiff_t | **[GetNumSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getnumsteps)**(const ptime & start, const ptime & end) const |
| virtual const ptrdiff_t | **[GetOffset](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getoffset)**(const ptime & start, const ptime & end) const |
| void | **[CheckIsDateTime](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-checkisdatetime)**(const ptime & instant) |


## Public Functions Documentation

### function ~IrregularTimeStepImplementation

```cpp
inline virtual ~IrregularTimeStepImplementation()
```


### function Clone

```cpp
virtual TimeStepImplementation * Clone() =0
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-clone)


**Reimplemented by**: [datatypes::timeseries::MonthlyQppTimeStepImplementation::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-clone)


### function Equals

```cpp
virtual bool Equals(
    TimeStepImplementation * tsImpl
) const =0
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::Equals](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-equals)


**Reimplemented by**: [datatypes::timeseries::MonthlyQppTimeStepImplementation::Equals](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-equals)


### function Multiply

```cpp
virtual TimeStepImplementation * Multiply(
    int mult
) const
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::Multiply](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-multiply)


### function Multiply

```cpp
virtual TimeStepImplementation * Multiply(
    double mult
) const
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::Multiply](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-multiply)


### function Divide

```cpp
virtual TimeStepImplementation * Divide(
    int divisor
) const
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::Divide](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-divide)


### function AddIntSteps

```cpp
virtual const ptime AddIntSteps(
    const ptime & startTimeStep,
    int n
) const =0
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::AddIntSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-addintsteps)


**Reimplemented by**: [datatypes::timeseries::MonthlyQppTimeStepImplementation::AddIntSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-addintsteps)


### function AddSteps

```cpp
virtual const ptime AddSteps(
    const ptime & startTimeStep,
    double mult
) const =0
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::AddSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-addsteps)


**Reimplemented by**: [datatypes::timeseries::MonthlyQppTimeStepImplementation::AddSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-addsteps)


### function GetTimeStepDuration

```cpp
virtual const time_duration GetTimeStepDuration(
    const ptime & startTimeStep
) const
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::GetTimeStepDuration](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-gettimestepduration)


**Reimplemented by**: [datatypes::timeseries::MonthlyQppTimeStepImplementation::GetTimeStepDuration](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-gettimestepduration)


### function Increment

```cpp
virtual const void Increment(
    ptime * t
) const =0
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::Increment](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-increment)


**Reimplemented by**: [datatypes::timeseries::MonthlyQppTimeStepImplementation::Increment](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-increment)


### function IsRegular

```cpp
virtual bool IsRegular() const
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::IsRegular](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-isregular)


### function GetRegularStepDuration

```cpp
virtual time_duration GetRegularStepDuration() const
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::GetRegularStepDuration](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getregularstepduration)


### function GetName

```cpp
virtual std::string GetName() const =0
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::GetName](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getname)


**Reimplemented by**: [datatypes::timeseries::MonthlyQppTimeStepImplementation::GetName](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-getname)


## Protected Functions Documentation

### function GetLinearIndexing

```cpp
virtual const double GetLinearIndexing(
    const ptime & start,
    const ptime & end
) const =0
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::GetLinearIndexing](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getlinearindexing)


**Reimplemented by**: [datatypes::timeseries::MonthlyQppTimeStepImplementation::GetLinearIndexing](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-getlinearindexing)


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000