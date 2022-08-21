---
title: datatypes::timeseries::DefaultMissingValuePolicyTypeFactory

---

# datatypes::timeseries::DefaultMissingValuePolicyTypeFactory



 [More...](#detailed-description)


`#include <time_series.hpp>`

## Public Types

|                | Name           |
| -------------- | -------------- |
| typedef [IfThenElse](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1IfThenElse/)< std::is_pointer< T >::value, [NullPointerIsMissingPolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NullPointerIsMissingPolicy/)< T >, [DefaultMissingFloatingPointPolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DefaultMissingFloatingPointPolicy/)< T > >::ResultT | **[type](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1DefaultMissingValuePolicyTypeFactory/#typedef-type)**  |

## Detailed Description

```cpp
template <typename T >
struct datatypes::timeseries::DefaultMissingValuePolicyTypeFactory;
```

## Public Types Documentation

### typedef type

```cpp
typedef IfThenElse< std::is_pointer<T>::value, NullPointerIsMissingPolicy<T>, DefaultMissingFloatingPointPolicy<T> >::ResultT datatypes::timeseries::DefaultMissingValuePolicyTypeFactory< T >::type;
```


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000