---
title: datatypes::utils::DisposeVectorTypeFactory

---

# datatypes::utils::DisposeVectorTypeFactory



 [More...](#detailed-description)


`#include <common.h>`

## Public Types

|                | Name           |
| -------------- | -------------- |
| typedef [IfThenElse](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1IfThenElse/)< std::is_pointer< T >::value, [ValueTypeVectorDispose](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1ValueTypeVectorDispose/)< T >, [PointerTypeVectorDispose](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1PointerTypeVectorDispose/)< T > >::ResultT | **[type](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1utils_1_1DisposeVectorTypeFactory/#typedef-type)**  |

## Detailed Description

```cpp
template <typename T >
struct datatypes::utils::DisposeVectorTypeFactory;
```

## Public Types Documentation

### typedef type

```cpp
typedef IfThenElse< std::is_pointer<T>::value, ValueTypeVectorDispose<T>, PointerTypeVectorDispose<T> >::ResultT datatypes::utils::DisposeVectorTypeFactory< T >::type;
```


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000