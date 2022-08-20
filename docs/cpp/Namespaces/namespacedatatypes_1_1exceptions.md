---
title: datatypes::exceptions

---

# datatypes::exceptions



## Classes

|                | Name           |
| -------------- | -------------- |
| struct | **[datatypes::exceptions::RangeCheck](/cpp/Classes/structdatatypes_1_1exceptions_1_1RangeCheck/)**  |
| struct | **[datatypes::exceptions::RangeCheck< size_t >](/cpp/Classes/structdatatypes_1_1exceptions_1_1RangeCheck_3_01size__t_01_4/)**  |
| class | **[datatypes::exceptions::ExceptionUtilities](/cpp/Classes/classdatatypes_1_1exceptions_1_1ExceptionUtilities/)**  |
| class | **[datatypes::exceptions::TimeSeriesChecks](/cpp/Classes/classdatatypes_1_1exceptions_1_1TimeSeriesChecks/)**  |

## Functions

|                | Name           |
| -------------- | -------------- |
| template <typename T \> <br>void | **[ThrowNotInRange](/cpp/Namespaces/namespacedatatypes_1_1exceptions/#function-thrownotinrange)**(T value, T bound, const string & variableName, const string & condition, const string & boundType) |


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

Updated on 2022-08-20 at 18:35:57 +1000