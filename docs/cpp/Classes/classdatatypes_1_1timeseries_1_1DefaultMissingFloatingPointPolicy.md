---
title: datatypes::timeseries::DefaultMissingFloatingPointPolicy

---

# datatypes::timeseries::DefaultMissingFloatingPointPolicy



 [More...](#detailed-description)


`#include <time_series_strategies.hpp>`

Inherits from [datatypes::timeseries::MissingValuePolicy< double >](/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| bool | **[IsMissingValue](/cpp/Classes/classdatatypes_1_1timeseries_1_1DefaultMissingFloatingPointPolicy/#function-ismissingvalue)**(const T & a) const |
| virtual T | **[GetMissingValue](/cpp/Classes/classdatatypes_1_1timeseries_1_1DefaultMissingFloatingPointPolicy/#function-getmissingvalue)**() const |
| virtual [MissingValuePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/)< T > * | **[Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1DefaultMissingFloatingPointPolicy/#function-clone)**() const |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::MissingValuePolicy< double >](/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~MissingValuePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/#function-~missingvaluepolicy)**() |


## Detailed Description

```cpp
template <typename T  =double>
class datatypes::timeseries::DefaultMissingFloatingPointPolicy;
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


**Reimplements**: [datatypes::timeseries::MissingValuePolicy::GetMissingValue](/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/#function-getmissingvalue)


### function Clone

```cpp
inline virtual MissingValuePolicy< T > * Clone() const
```


**Reimplements**: [datatypes::timeseries::MissingValuePolicy::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/#function-clone)


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000