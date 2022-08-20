---
title: datatypes::timeseries::MissingValuePolicy
summary: An interface for classes that define missing values in time series. 

---

# datatypes::timeseries::MissingValuePolicy



An interface for classes that define missing values in time series.  [More...](#detailed-description)


`#include <time_series_strategies.hpp>`

Inherited by [datatypes::timeseries::NullPointerIsMissingPolicy< T >](/cpp/Classes/classdatatypes_1_1timeseries_1_1NullPointerIsMissingPolicy/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual | **[~MissingValuePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/#function-~missingvaluepolicy)**() |
| virtual bool | **[IsMissingValue](/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/#function-ismissingvalue)**(const T & a) const =0 |
| virtual T | **[GetMissingValue](/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/#function-getmissingvalue)**() const =0 |
| virtual [MissingValuePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/) * | **[Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/#function-clone)**() const =0 |

## Detailed Description

```cpp
template <typename T >
class datatypes::timeseries::MissingValuePolicy;
```

An interface for classes that define missing values in time series. 

**Template Parameters**: 

  * **T** Generic type parameter. 

## Public Functions Documentation

### function ~MissingValuePolicy

```cpp
inline virtual ~MissingValuePolicy()
```


### function IsMissingValue

```cpp
virtual bool IsMissingValue(
    const T & a
) const =0
```


**Reimplemented by**: [datatypes::timeseries::NullPointerIsMissingPolicy::IsMissingValue](/cpp/Classes/classdatatypes_1_1timeseries_1_1NullPointerIsMissingPolicy/#function-ismissingvalue)


### function GetMissingValue

```cpp
virtual T GetMissingValue() const =0
```


**Reimplemented by**: [datatypes::timeseries::DefaultMissingFloatingPointPolicy::GetMissingValue](/cpp/Classes/classdatatypes_1_1timeseries_1_1DefaultMissingFloatingPointPolicy/#function-getmissingvalue), [datatypes::timeseries::NullPointerIsMissingPolicy::GetMissingValue](/cpp/Classes/classdatatypes_1_1timeseries_1_1NullPointerIsMissingPolicy/#function-getmissingvalue), [datatypes::timeseries::NegativeIsMissingFloadingPointPolicy::GetMissingValue](/cpp/Classes/classdatatypes_1_1timeseries_1_1NegativeIsMissingFloadingPointPolicy/#function-getmissingvalue)


### function Clone

```cpp
virtual MissingValuePolicy * Clone() const =0
```


**Reimplemented by**: [datatypes::timeseries::DefaultMissingFloatingPointPolicy::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1DefaultMissingFloatingPointPolicy/#function-clone), [datatypes::timeseries::NullPointerIsMissingPolicy::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1NullPointerIsMissingPolicy/#function-clone), [datatypes::timeseries::NegativeIsMissingFloadingPointPolicy::Clone](/cpp/Classes/classdatatypes_1_1timeseries_1_1NegativeIsMissingFloadingPointPolicy/#function-clone)


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000