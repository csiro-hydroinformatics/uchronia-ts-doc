---
title: datatypes::timeseries::NullPointerIsMissingPolicy

---

# datatypes::timeseries::NullPointerIsMissingPolicy



 [More...](#detailed-description)


`#include <time_series_strategies.hpp>`

Inherits from [datatypes::timeseries::MissingValuePolicy< T >](/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual bool | **[IsMissingValue](/cpp/Classes/classdatatypes_1_1timeseries_1_1NullPointerIsMissingPolicy/#function-ismissingvalue)**(const T & a) const |
| virtual T | **[GetMissingValue](/cpp/Classes/classdatatypes_1_1timeseries_1_1NullPointerIsMissingPolicy/#function-getmissingvalue)**() const |
| virtual [MissingValuePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/)< T > * | **[Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1NullPointerIsMissingPolicy/#function-clone)**() const |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::MissingValuePolicy< T >](/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~MissingValuePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/#function-~missingvaluepolicy)**() |


## Detailed Description

```cpp
template <typename T >
class datatypes::timeseries::NullPointerIsMissingPolicy;
```

## Public Functions Documentation

### function IsMissingValue

```cpp
inline virtual bool IsMissingValue(
    const T & a
) const
```


**Reimplements**: [datatypes::timeseries::MissingValuePolicy::IsMissingValue](/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/#function-ismissingvalue)


### function GetMissingValue

```cpp
inline virtual T GetMissingValue() const
```


**Reimplements**: [datatypes::timeseries::MissingValuePolicy::GetMissingValue](/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/#function-getmissingvalue)


### function Clone

```cpp
inline virtual MissingValuePolicy< T > * Clone() const
```


**Reimplements**: [datatypes::timeseries::MissingValuePolicy::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/#function-clone)


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000