---
title: datatypes::exceptions
summary: Helper function to build consistent informative error messages in exceptions with commonalities. 

---

# datatypes::exceptions

Helper function to build consistent informative error messages in exceptions with commonalities. 

## Classes

|                | Name           |
| -------------- | -------------- |
| struct | **[datatypes::exceptions::RangeCheck](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1exceptions_1_1RangeCheck/)**  |
| struct | **[datatypes::exceptions::RangeCheck< size_t >](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1exceptions_1_1RangeCheck_3_01size__t_01_4/)**  |
| class | **[datatypes::exceptions::ExceptionUtilities](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1exceptions_1_1ExceptionUtilities/)**  |
| class | **[datatypes::exceptions::TimeSeriesChecks](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1exceptions_1_1TimeSeriesChecks/)**  |

## Functions

|                | Name           |
| -------------- | -------------- |
| template <typename T \> <br>void | **[ThrowNotInRange](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1exceptions/#function-thrownotinrange)**(T value, T bound, const string & variableName, const string & condition, const string & boundType) |


## Functions Documentation

### function ThrowNotInRange

```cpp
template <typename T >
static void ThrowNotInRange(
    T value,
    T bound,
    const string & variableName,
    const string & condition,
    const string & boundType
)
```






-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000