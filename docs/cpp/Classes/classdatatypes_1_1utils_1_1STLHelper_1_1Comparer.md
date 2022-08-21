---
title: datatypes::utils::STLHelper::Comparer

---

# datatypes::utils::STLHelper::Comparer



 [More...](#detailed-description)

## Public Types

|                | Name           |
| -------------- | -------------- |
| typedef vector< U >::const_iterator | **[const_iterator](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper_1_1Comparer/#typedef-const-iterator)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[Comparer](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper_1_1Comparer/#function-comparer)**(std::function< bool(const U &, const U &)> & valueCompare) |
| bool | **[operator()](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper_1_1Comparer/#function-operator())**(const std::pair< size_t, const_iterator > & a, const std::pair< size_t, const_iterator > & b) |

## Detailed Description

```cpp
template <typename U >
class datatypes::utils::STLHelper::Comparer;
```

## Public Types Documentation

### typedef const_iterator

```cpp
typedef vector<U>::const_iterator datatypes::utils::STLHelper::Comparer< U >::const_iterator;
```


## Public Functions Documentation

### function Comparer

```cpp
inline Comparer(
    std::function< bool(const U &, const U &)> & valueCompare
)
```


### function operator()

```cpp
inline bool operator()(
    const std::pair< size_t, const_iterator > & a,
    const std::pair< size_t, const_iterator > & b
)
```


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000