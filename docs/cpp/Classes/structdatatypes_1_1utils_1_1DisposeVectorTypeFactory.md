---
title: datatypes::utils::DisposeVectorTypeFactory

---

# datatypes::utils::DisposeVectorTypeFactory



 [More...](#detailed-description)


`#include <common.h>`

## Public Types

|                | Name           |
| -------------- | -------------- |
| typedef [IfThenElse](/cpp/Classes/classdatatypes_1_1utils_1_1IfThenElse/)< std::is_pointer< T >::value, [ValueTypeVectorDispose](/cpp/Classes/classdatatypes_1_1utils_1_1ValueTypeVectorDispose/)< T >, [PointerTypeVectorDispose](/cpp/Classes/classdatatypes_1_1utils_1_1PointerTypeVectorDispose/)< T > >::ResultT | **[type](/cpp/Classes/structdatatypes_1_1utils_1_1DisposeVectorTypeFactory/#typedef-type)**  |

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

Updated on 2022-08-20 at 18:35:57 +1000