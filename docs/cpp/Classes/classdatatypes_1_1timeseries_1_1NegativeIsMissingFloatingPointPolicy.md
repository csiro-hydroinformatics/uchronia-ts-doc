---
title: datatypes::timeseries::NegativeIsMissingFloatingPointPolicy

---

# datatypes::timeseries::NegativeIsMissingFloatingPointPolicy



 [More...](#detailed-description)


`#include <time_series_strategies.hpp>`

Inherits from [datatypes::timeseries::MissingValuePolicy< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| bool | **[IsMissingValue](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NegativeIsMissingFloatingPointPolicy/#function-ismissingvalue)**(const T & a) const |
| virtual T | **[GetMissingValue](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NegativeIsMissingFloatingPointPolicy/#function-getmissingvalue)**() const |
| virtual [MissingValuePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/)< T > * | **[Clone](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NegativeIsMissingFloatingPointPolicy/#function-clone)**() const |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::MissingValuePolicy< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~MissingValuePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/#function-~missingvaluepolicy)**() |


## Detailed Description

```cpp
template <typename T  =double>
class datatypes::timeseries::NegativeIsMissingFloatingPointPolicy;
```

## Public Functions Documentation

### function IsMissingValue

```cpp
inline bool IsMissingValue(
    const T & a
) const
```


### function GetMissingValue

```cpp
inline virtual T GetMissingValue() const
```


**Reimplements**: [datatypes::timeseries::MissingValuePolicy::GetMissingValue](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/#function-getmissingvalue)


### function Clone

```cpp
inline virtual MissingValuePolicy< T > * Clone() const
```


**Reimplements**: [datatypes::timeseries::MissingValuePolicy::Clone](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/#function-clone)


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000