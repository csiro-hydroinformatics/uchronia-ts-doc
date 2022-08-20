---
title: datatypes::timeseries::MissingValuePolicy
summary: An interface for classes that define missing values in time series. 

---

# datatypes::timeseries::MissingValuePolicy



An interface for classes that define missing values in time series.  [More...](#detailed-description)


`#include <time_series_strategies.hpp>`

Inherited by [datatypes::timeseries::NullPointerIsMissingPolicy< T >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NullPointerIsMissingPolicy/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual | **[~MissingValuePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/#function-~missingvaluepolicy)**() |
| virtual bool | **[IsMissingValue](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/#function-ismissingvalue)**(const T & a) const =0 |
| virtual T | **[GetMissingValue](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/#function-getmissingvalue)**() const =0 |
| virtual [MissingValuePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/) * | **[Clone](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/#function-clone)**() const =0 |

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


**Reimplemented by**: [datatypes::timeseries::NullPointerIsMissingPolicy::IsMissingValue](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NullPointerIsMissingPolicy/#function-ismissingvalue)


### function GetMissingValue

```cpp
virtual T GetMissingValue() const =0
```


**Reimplemented by**: [datatypes::timeseries::DefaultMissingFloatingPointPolicy::GetMissingValue](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DefaultMissingFloatingPointPolicy/#function-getmissingvalue), [datatypes::timeseries::NullPointerIsMissingPolicy::GetMissingValue](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NullPointerIsMissingPolicy/#function-getmissingvalue), [datatypes::timeseries::NegativeIsMissingFloadingPointPolicy::GetMissingValue](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NegativeIsMissingFloadingPointPolicy/#function-getmissingvalue)


### function Clone

```cpp
virtual MissingValuePolicy * Clone() const =0
```


**Reimplemented by**: [datatypes::timeseries::DefaultMissingFloatingPointPolicy::Clone](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DefaultMissingFloatingPointPolicy/#function-clone), [datatypes::timeseries::NullPointerIsMissingPolicy::Clone](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NullPointerIsMissingPolicy/#function-clone), [datatypes::timeseries::NegativeIsMissingFloadingPointPolicy::Clone](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NegativeIsMissingFloadingPointPolicy/#function-clone)


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000