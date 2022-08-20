---
title: datatypes::timeseries::MonthlyQppTimeStepImplementation

---

# datatypes::timeseries::MonthlyQppTimeStepImplementation






`#include <time_step_implementation.h>`

Inherits from [datatypes::timeseries::IrregularTimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/), [datatypes::timeseries::TimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual | **[~MonthlyQppTimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-~monthlyqpptimestepimplementation)**() |
| virtual [TimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Clone](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-clone)**() |
| virtual bool | **[Equals](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-equals)**([TimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * tsImpl) const |
| virtual const ptime | **[AddIntSteps](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-addintsteps)**(const ptime & startTimeStep, int n) const |
| virtual const ptime | **[AddSteps](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-addsteps)**(const ptime & startTimeStep, double mult) const |
| virtual const time_duration | **[GetTimeStepDuration](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-gettimestepduration)**(const ptime & startTimeStep) const override |
| virtual const void | **[Increment](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-increment)**(ptime * t) const |
| virtual std::string | **[GetName](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-getname)**() const |

## Protected Functions

|                | Name           |
| -------------- | -------------- |
| virtual const double | **[GetLinearIndexing](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-getlinearindexing)**(const ptime & start, const ptime & end) const |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::IrregularTimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~IrregularTimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-~irregulartimestepimplementation)**() |
| virtual [TimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Multiply](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-multiply)**(int mult) const |
| virtual [TimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Multiply](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-multiply)**(double mult) const |
| virtual [TimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Divide](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-divide)**(int divisor) const |
| virtual bool | **[IsRegular](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-isregular)**() const |
| virtual time_duration | **[GetRegularStepDuration](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-getregularstepduration)**() const |

**Public Functions inherited from [datatypes::timeseries::TimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-~timestepimplementation)**() |
| virtual [TimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Multiply](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-multiply)**(int mult) const =0 |
| virtual [TimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Divide](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-divide)**(int divisor) const =0 |
| virtual [TimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Multiply](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-multiply)**(double mult) const =0 |
| virtual const ptrdiff_t | **[GetUpperNumSteps](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getuppernumsteps)**(const ptime & start, const ptime & end) const |
| virtual const ptrdiff_t | **[GetNumSteps](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getnumsteps)**(const ptime & start, const ptime & end) const |
| virtual const ptrdiff_t | **[GetOffset](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getoffset)**(const ptime & start, const ptime & end) const |
| virtual bool | **[IsRegular](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-isregular)**() const =0 |
| virtual time_duration | **[GetRegularStepDuration](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getregularstepduration)**() const =0 |
| void | **[CheckIsDateTime](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-checkisdatetime)**(const ptime & instant) |


## Public Functions Documentation

### function ~MonthlyQppTimeStepImplementation

```cpp
inline virtual ~MonthlyQppTimeStepImplementation()
```


### function Clone

```cpp
virtual TimeStepImplementation * Clone()
```


**Reimplements**: [datatypes::timeseries::IrregularTimeStepImplementation::Clone](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-clone)


### function Equals

```cpp
virtual bool Equals(
    TimeStepImplementation * tsImpl
) const
```


**Reimplements**: [datatypes::timeseries::IrregularTimeStepImplementation::Equals](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-equals)


### function AddIntSteps

```cpp
virtual const ptime AddIntSteps(
    const ptime & startTimeStep,
    int n
) const
```


**Reimplements**: [datatypes::timeseries::IrregularTimeStepImplementation::AddIntSteps](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-addintsteps)


### function AddSteps

```cpp
virtual const ptime AddSteps(
    const ptime & startTimeStep,
    double mult
) const
```


**Reimplements**: [datatypes::timeseries::IrregularTimeStepImplementation::AddSteps](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-addsteps)


### function GetTimeStepDuration

```cpp
virtual const time_duration GetTimeStepDuration(
    const ptime & startTimeStep
) const override
```


**Reimplements**: [datatypes::timeseries::IrregularTimeStepImplementation::GetTimeStepDuration](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-gettimestepduration)


### function Increment

```cpp
virtual const void Increment(
    ptime * t
) const
```


**Reimplements**: [datatypes::timeseries::IrregularTimeStepImplementation::Increment](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-increment)


### function GetName

```cpp
virtual std::string GetName() const
```


**Reimplements**: [datatypes::timeseries::IrregularTimeStepImplementation::GetName](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-getname)


## Protected Functions Documentation

### function GetLinearIndexing

```cpp
virtual const double GetLinearIndexing(
    const ptime & start,
    const ptime & end
) const
```


**Reimplements**: [datatypes::timeseries::IrregularTimeStepImplementation::GetLinearIndexing](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-getlinearindexing)


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000