---
title: datatypes::timeseries::MonthlyQppTimeStepImplementation

---

# datatypes::timeseries::MonthlyQppTimeStepImplementation






`#include <time_step_implementation.h>`

Inherits from [datatypes::timeseries::IrregularTimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/), [datatypes::timeseries::TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual | **[~MonthlyQppTimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-~monthlyqpptimestepimplementation)**() |
| virtual [TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-clone)**() |
| virtual bool | **[Equals](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-equals)**([TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * tsImpl) const |
| virtual const ptime | **[AddIntSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-addintsteps)**(const ptime & startTimeStep, int n) const |
| virtual const ptime | **[AddSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-addsteps)**(const ptime & startTimeStep, double mult) const |
| virtual const time_duration | **[GetTimeStepDuration](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-gettimestepduration)**(const ptime & startTimeStep) const override |
| virtual const void | **[Increment](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-increment)**(ptime * t) const |
| virtual std::string | **[GetName](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-getname)**() const |

## Protected Functions

|                | Name           |
| -------------- | -------------- |
| virtual const double | **[GetLinearIndexing](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/#function-getlinearindexing)**(const ptime & start, const ptime & end) const |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::IrregularTimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~IrregularTimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-~irregulartimestepimplementation)**() |
| virtual [TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Multiply](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-multiply)**(int mult) const |
| virtual [TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Multiply](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-multiply)**(double mult) const |
| virtual [TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Divide](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-divide)**(int divisor) const |
| virtual bool | **[IsRegular](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-isregular)**() const |
| virtual time_duration | **[GetRegularStepDuration](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-getregularstepduration)**() const |

**Public Functions inherited from [datatypes::timeseries::TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-~timestepimplementation)**() |
| virtual [TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Multiply](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-multiply)**(int mult) const =0 |
| virtual [TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Divide](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-divide)**(int divisor) const =0 |
| virtual [TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Multiply](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-multiply)**(double mult) const =0 |
| virtual const ptrdiff_t | **[GetUpperNumSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getuppernumsteps)**(const ptime & start, const ptime & end) const |
| virtual const ptrdiff_t | **[GetNumSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getnumsteps)**(const ptime & start, const ptime & end) const |
| virtual const ptrdiff_t | **[GetOffset](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getoffset)**(const ptime & start, const ptime & end) const |
| virtual bool | **[IsRegular](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-isregular)**() const =0 |
| virtual time_duration | **[GetRegularStepDuration](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getregularstepduration)**() const =0 |
| void | **[CheckIsDateTime](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-checkisdatetime)**(const ptime & instant) |


## Public Functions Documentation

### function ~MonthlyQppTimeStepImplementation

```cpp
inline virtual ~MonthlyQppTimeStepImplementation()
```


### function Clone

```cpp
virtual TimeStepImplementation * Clone()
```


**Reimplements**: [datatypes::timeseries::IrregularTimeStepImplementation::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-clone)


### function Equals

```cpp
virtual bool Equals(
    TimeStepImplementation * tsImpl
) const
```


**Reimplements**: [datatypes::timeseries::IrregularTimeStepImplementation::Equals](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-equals)


### function AddIntSteps

```cpp
virtual const ptime AddIntSteps(
    const ptime & startTimeStep,
    int n
) const
```


**Reimplements**: [datatypes::timeseries::IrregularTimeStepImplementation::AddIntSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-addintsteps)


### function AddSteps

```cpp
virtual const ptime AddSteps(
    const ptime & startTimeStep,
    double mult
) const
```


**Reimplements**: [datatypes::timeseries::IrregularTimeStepImplementation::AddSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-addsteps)


### function GetTimeStepDuration

```cpp
virtual const time_duration GetTimeStepDuration(
    const ptime & startTimeStep
) const override
```


**Reimplements**: [datatypes::timeseries::IrregularTimeStepImplementation::GetTimeStepDuration](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-gettimestepduration)


### function Increment

```cpp
virtual const void Increment(
    ptime * t
) const
```


**Reimplements**: [datatypes::timeseries::IrregularTimeStepImplementation::Increment](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-increment)


### function GetName

```cpp
virtual std::string GetName() const
```


**Reimplements**: [datatypes::timeseries::IrregularTimeStepImplementation::GetName](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-getname)


## Protected Functions Documentation

### function GetLinearIndexing

```cpp
virtual const double GetLinearIndexing(
    const ptime & start,
    const ptime & end
) const
```


**Reimplements**: [datatypes::timeseries::IrregularTimeStepImplementation::GetLinearIndexing](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/#function-getlinearindexing)


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000