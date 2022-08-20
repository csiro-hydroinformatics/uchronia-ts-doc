---
title: datatypes::timeseries::DefaultMissingValuePolicyTypeFactory

---

# datatypes::timeseries::DefaultMissingValuePolicyTypeFactory



 [More...](#detailed-description)


`#include <time_series.hpp>`

## Public Types

|                | Name           |
| -------------- | -------------- |
| typedef [IfThenElse](/cpp/Classes/classdatatypes_1_1utils_1_1IfThenElse/)< std::is_pointer< T >::value, [NullPointerIsMissingPolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1NullPointerIsMissingPolicy/)< T >, [DefaultMissingFloatingPointPolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1DefaultMissingFloatingPointPolicy/)< T > >::ResultT | **[type](/cpp/Classes/structdatatypes_1_1timeseries_1_1DefaultMissingValuePolicyTypeFactory/#typedef-type)**  |

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

Updated on 2022-08-20 at 18:35:57 +1000