---
title: datatypes::timeseries::RegularTimeStepImplementation

---

# datatypes::timeseries::RegularTimeStepImplementation






`#include <time_step_implementation.h>`

Inherits from [datatypes::timeseries::TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| [RegularTimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/) * | **[GetHourly](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-gethourly)**() |
| [RegularTimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/) * | **[GetDaily](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-getdaily)**() |
| | **[RegularTimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-regulartimestepimplementation)**(const time_duration & stepDuration) |
| virtual | **[~RegularTimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-~regulartimestepimplementation)**() |
| virtual [TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-clone)**() |
| virtual bool | **[Equals](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-equals)**([TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * tsImpl) const |
| virtual [TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Multiply](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-multiply)**(int mult) const |
| virtual [TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Multiply](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-multiply)**(double mult) const |
| virtual [TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * | **[Divide](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-divide)**(int divisor) const |
| virtual const ptime | **[AddIntSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-addintsteps)**(const ptime & startTimeStep, int n) const |
| virtual const ptime | **[AddSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-addsteps)**(const ptime & startTimeStep, double mult) const |
| virtual const time_duration | **[GetTimeStepDuration](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-gettimestepduration)**(const ptime & startTimeStep) const |
| virtual const void | **[Increment](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-increment)**(ptime * t) const |
| virtual bool | **[IsRegular](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-isregular)**() const |
| virtual time_duration | **[GetRegularStepDuration](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-getregularstepduration)**() const |
| virtual std::string | **[GetName](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-getname)**() const |

## Protected Functions

|                | Name           |
| -------------- | -------------- |
| virtual const double | **[GetLinearIndexing](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/#function-getlinearindexing)**(const ptime & start, const ptime & end) const |

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

### function GetHourly

```cpp
static RegularTimeStepImplementation * GetHourly()
```


### function GetDaily

```cpp
static RegularTimeStepImplementation * GetDaily()
```


### function RegularTimeStepImplementation

```cpp
RegularTimeStepImplementation(
    const time_duration & stepDuration
)
```


### function ~RegularTimeStepImplementation

```cpp
virtual ~RegularTimeStepImplementation()
```


### function Clone

```cpp
virtual TimeStepImplementation * Clone()
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-clone)


### function Equals

```cpp
virtual bool Equals(
    TimeStepImplementation * tsImpl
) const
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::Equals](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-equals)


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
) const
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::AddIntSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-addintsteps)


### function AddSteps

```cpp
virtual const ptime AddSteps(
    const ptime & startTimeStep,
    double mult
) const
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::AddSteps](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-addsteps)


### function GetTimeStepDuration

```cpp
virtual const time_duration GetTimeStepDuration(
    const ptime & startTimeStep
) const
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::GetTimeStepDuration](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-gettimestepduration)


### function Increment

```cpp
virtual const void Increment(
    ptime * t
) const
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::Increment](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-increment)


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
virtual std::string GetName() const
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::GetName](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getname)


## Protected Functions Documentation

### function GetLinearIndexing

```cpp
virtual const double GetLinearIndexing(
    const ptime & start,
    const ptime & end
) const
```


**Reimplements**: [datatypes::timeseries::TimeStepImplementation::GetLinearIndexing](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/#function-getlinearindexing)


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000