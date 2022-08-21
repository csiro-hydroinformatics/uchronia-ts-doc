---
title: datatypes::timeseries::TimeStep
summary: Time step handling for time series. 

---

# datatypes::timeseries::TimeStep



Time step handling for time series.  [More...](#detailed-description)


`#include <time_step.h>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-timestep)**(const time_duration & stepDuration)<br>Define a time step where every step is a fixed time duration.  |
| | **[TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-timestep)**([TimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/) * tsi) |
| | **[TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-timestep)**(const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & src)<br>Copy constructor.  |
| | **[TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-timestep)**() |
| | **[~TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-~timestep)**() |
| [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & | **[operator=](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-operator=)**(const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & rhs) |
| [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & | **[operator=](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-operator=)**(const time_duration & stepDuration)<br>Assignment operator.  |
| [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & | **[operator=](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-operator=)**(const string & stepDuration) |
| bool | **[operator==](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-operator==)**(const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & rhs) const |
| bool | **[operator!=](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-operator!=)**(const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & rhs) const |
| [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[operator*](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-operator*)**(int mult) const<br>Multiplication operator, using the time_duration multiplication operator.  |
| [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[operator*](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-operator*)**(double mult) const |
| int | **[operator/](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-operator/)**(const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & divisor) const |
| [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[operator/](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-operator/)**(int divisor) const |
| time_duration | **[operator%](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-operator%)**(const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & other) const |
| bool | **[IsRegular](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-isregular)**() const<br>Query if this time step is defined by a time duration in the true sense (day, week). Monthly time step would return false;.  |
| time_duration | **[GetRegularStepDuration](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-getregularstepduration)**() const<br>Gets the underlying time_duration for this time step. Exception thrown if not a regular time step.  |
| const ptime | **[AddSteps](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-addsteps)**(const ptime & startTimeStep, size_t n) const |
| const ptime | **[AddSteps](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-addsteps)**(const ptime & startTimeStep, int n) const |
| const ptime | **[AddSteps](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-addsteps)**(const ptime & startTimeStep, double mult) const<br>Adds a number of steps to an instant, which can be non-integer for regular time steps. Behavior TBC for irregular time steps.  |
| vector< ptime > | **[AddSteps](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-addsteps)**(const ptime & startTimeStep, const vector< double > timeSteps) const<br>Vectorized version of shifting time steps. Adds a number of steps to an instant, which can be non-integer for regular time steps. Behavior TBC for irregular time steps.  |
| vector< ptime > | **[AddSteps](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-addsteps)**(const vector< ptime > & times, double mult) const |
| const time_duration | **[GetTimeStepDuration](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-gettimestepduration)**(const ptime & startTimeStep) const<br>Given an instant, what is the next time instant according to this present Time step.  |
| const ptrdiff_t | **[GetUpperNumSteps](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-getuppernumsteps)**(const ptime & start, const ptime & end) const<br>Gets the minimum number of time steps covering a time interval.  |
| const ptrdiff_t | **[GetNumSteps](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-getnumsteps)**(const ptime & start, const ptime & end) const<br>Gets the maximum number of time steps from a starting instant to not get beyond an instant in time, 'end'.  |
| const ptrdiff_t | **[GetOffset](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-getoffset)**(const ptime & start, const ptime & end) const |
| const void | **[Increment](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-increment)**(ptime * t) const<br>Increments an instant by one time step.  |
| bool | **[IsUnknown](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-isunknown)**() const<br>Query if this object is the time step value "unknown".  |
| string | **[GetName](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-getname)**() const |
| [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[Parse](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-parse)**(const string & name) |
| [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[FromSeconds](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-fromseconds)**(unsigned int seconds) |
| [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetDaily](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-getdaily)**() |
| [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetHourly](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-gethourly)**() |
| [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetMonthlyQpp](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-getmonthlyqpp)**() |
| [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetUnknown](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-getunknown)**()<br>Gets an instance of time step that is unknown. This value is indented for use in methods as a default parameter value.  |
| ptime | **[CreatePtime](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-createptime)**(int year, int month, int day, int hour =0, int minute =0, int second =0) |
| ptime | **[PtimeFromIsoString](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-ptimefromisostring)**(const string & t) |
| string | **[ToString](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/#function-tostring)**(const ptime & dt, const string & format ="YYYYMMDDThhmmss") |

## Detailed Description

```cpp
class datatypes::timeseries::TimeStep;
```

Time step handling for time series. 



```
    A TimeStep is responsible for the definition of time steps in time series 
    and the associated calculations for determining time instants and durations
```

## Public Functions Documentation

### function TimeStep

```cpp
TimeStep(
    const time_duration & stepDuration
)
```

Define a time step where every step is a fixed time duration. 

**Parameters**: 

  * **stepDuration** Duration of the step. 


### function TimeStep

```cpp
TimeStep(
    TimeStepImplementation * tsi
)
```


### function TimeStep

```cpp
TimeStep(
    const TimeStep & src
)
```

Copy constructor. 

**Parameters**: 

  * **src** [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) to copy. 


### function TimeStep

```cpp
TimeStep()
```


### function ~TimeStep

```cpp
~TimeStep()
```


### function operator=

```cpp
TimeStep & operator=(
    const TimeStep & rhs
)
```


### function operator=

```cpp
TimeStep & operator=(
    const time_duration & stepDuration
)
```

Assignment operator. 

**Parameters**: 

  * **stepDuration** Duration of the step.


**Return**: A reference to this object. 

### function operator=

```cpp
TimeStep & operator=(
    const string & stepDuration
)
```


### function operator==

```cpp
bool operator==(
    const TimeStep & rhs
) const
```


### function operator!=

```cpp
bool operator!=(
    const TimeStep & rhs
) const
```


### function operator*

```cpp
TimeStep operator*(
    int mult
) const
```

Multiplication operator, using the time_duration multiplication operator. 

**Parameters**: 

  * **mult** The multiplier.


**Return**: The result of the operation. 

Multiplication operator, using the time_duration multiplication operator if the argument is an integer.


### function operator*

```cpp
TimeStep operator*(
    double mult
) const
```


### function operator/

```cpp
int operator/(
    const TimeStep & divisor
) const
```


### function operator/

```cpp
TimeStep operator/(
    int divisor
) const
```


### function operator%

```cpp
time_duration operator%(
    const TimeStep & other
) const
```


### function IsRegular

```cpp
bool IsRegular() const
```

Query if this time step is defined by a time duration in the true sense (day, week). Monthly time step would return false;. 

**Return**: true if regular, false if not. 

### function GetRegularStepDuration

```cpp
time_duration GetRegularStepDuration() const
```

Gets the underlying time_duration for this time step. Exception thrown if not a regular time step. 

**Return**: The regular step duration. 

### function AddSteps

```cpp
const ptime AddSteps(
    const ptime & startTimeStep,
    size_t n
) const
```


### function AddSteps

```cpp
const ptime AddSteps(
    const ptime & startTimeStep,
    int n
) const
```


### function AddSteps

```cpp
const ptime AddSteps(
    const ptime & startTimeStep,
    double mult
) const
```

Adds a number of steps to an instant, which can be non-integer for regular time steps. Behavior TBC for irregular time steps. 

**Parameters**: 

  * **startTimeStep** The start time step. 
  * **mult** The number of steps added.


**Return**: A ptime. 

### function AddSteps

```cpp
vector< ptime > AddSteps(
    const ptime & startTimeStep,
    const vector< double > timeSteps
) const
```

Vectorized version of shifting time steps. Adds a number of steps to an instant, which can be non-integer for regular time steps. Behavior TBC for irregular time steps. 

**Parameters**: 

  * **startTimeStep** The start time step. 
  * **timeSteps** The time steps.


**Return**: A vector<ptime> 

### function AddSteps

```cpp
vector< ptime > AddSteps(
    const vector< ptime > & times,
    double mult
) const
```


### function GetTimeStepDuration

```cpp
const time_duration GetTimeStepDuration(
    const ptime & startTimeStep
) const
```

Given an instant, what is the next time instant according to this present Time step. 

**Parameters**: 

  * **startTimeStep** The start time step.


**Return**: The time step duration. 

### function GetUpperNumSteps

```cpp
const ptrdiff_t GetUpperNumSteps(
    const ptime & start,
    const ptime & end
) const
```

Gets the minimum number of time steps covering a time interval. 

**Parameters**: 

  * **start** The start of the time interval 
  * **end** The end of the time interval


**Return**: the number of steps needed to get beyond 'end' 

### function GetNumSteps

```cpp
const ptrdiff_t GetNumSteps(
    const ptime & start,
    const ptime & end
) const
```

Gets the maximum number of time steps from a starting instant to not get beyond an instant in time, 'end'. 

**Parameters**: 

  * **start** The start of the time interval 
  * **end** The end of the time interval


**Return**: the number of steps needed to not get beyond 'end' 

### function GetOffset

```cpp
const ptrdiff_t GetOffset(
    const ptime & start,
    const ptime & end
) const
```


### function Increment

```cpp
const void Increment(
    ptime * t
) const
```

Increments an instant by one time step. 

**Parameters**: 

  * **t** If non-null, the ptime to process. 


### function IsUnknown

```cpp
bool IsUnknown() const
```

Query if this object is the time step value "unknown". 

**Return**: true if unknown, false if not. 

### function GetName

```cpp
string GetName() const
```


### function Parse

```cpp
static TimeStep Parse(
    const string & name
)
```


### function FromSeconds

```cpp
static TimeStep FromSeconds(
    unsigned int seconds
)
```


### function GetDaily

```cpp
static TimeStep GetDaily()
```


### function GetHourly

```cpp
static TimeStep GetHourly()
```


### function GetMonthlyQpp

```cpp
static TimeStep GetMonthlyQpp()
```


### function GetUnknown

```cpp
static TimeStep GetUnknown()
```

Gets an instance of time step that is unknown. This value is indented for use in methods as a default parameter value. 

**Return**: The "unknown" value of the time step 

### function CreatePtime

```cpp
static ptime CreatePtime(
    int year,
    int month,
    int day,
    int hour =0,
    int minute =0,
    int second =0
)
```


### function PtimeFromIsoString

```cpp
static ptime PtimeFromIsoString(
    const string & t
)
```


### function ToString

```cpp
static string ToString(
    const ptime & dt,
    const string & format ="YYYYMMDDThhmmss"
)
```


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000