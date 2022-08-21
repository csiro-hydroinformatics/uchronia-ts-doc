---
title: datatypes::utils::DisposeVectorTypeFactory
summary: Template program; Type type is a class suitable to dispose of object T, whether it is a vector of value types, or a vector where items are pointers requiring the delete operator. Used to dispose of items in a templated time series, with items of either value or pointer types. 

---

# datatypes::utils::DisposeVectorTypeFactory



Template program; Type type is a class suitable to dispose of object T, whether it is a vector of value types, or a vector where items are pointers requiring the delete operator. Used to dispose of items in a templated time series, with items of either value or pointer types.  [More...](#detailed-description)


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

Template program; Type type is a class suitable to dispose of object T, whether it is a vector of value types, or a vector where items are pointers requiring the delete operator. Used to dispose of items in a templated time series, with items of either value or pointer types. 

**Template Parameters**: 

  * **T** type of items in the vector to clear/dispose of. 

## Public Types Documentation

### typedef type

```cpp
typedef IfThenElse< std::is_pointer<T>::value, ValueTypeVectorDispose<T>, PointerTypeVectorDispose<T> >::ResultT datatypes::utils::DisposeVectorTypeFactory< T >::type;
```


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000