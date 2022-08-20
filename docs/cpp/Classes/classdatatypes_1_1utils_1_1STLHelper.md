---
title: datatypes::utils::STLHelper

---

# datatypes::utils::STLHelper






`#include <common.h>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| template <typename K  =string,typename V  =string\> <br>bool | **[HasKey](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-haskey)**(const map< K, V > & dict, const string & key) |
| template <typename K  =string,typename V  =string\> <br>vector< K > | **[GetKeys](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-getkeys)**(const map< K, V > & dict) |
| template <typename K  =string,typename V  =string\> <br>map< K, V > | **[Remap](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-remap)**(const map< K, V > & dict, const map< K, K > & newKeys) |
| template <typename K  =string,typename V  =string\> <br>map< K, V > | **[Zip](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-zip)**(const vector< K > & key, const vector< V > & values) |
| template <typename K  =string,typename V  =string\> <br>vector< V > | **[GetValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-getvalues)**(const map< K, V > & dict) |
| template <typename K  =string,typename V  =string\> <br>vector< V > | **[GetValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-getvalues)**(const map< K, V > & dict, const vector< K > & keys) |
| template <typename U \> <br>bool | **[LessThan](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-lessthan)**(const U & first, const U & second) |
| template <typename U \> <br>bool | **[MoreThan](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-morethan)**(const U & first, const U & second) |
| template <typename K ,typename V \> <br>vector< V > | **[SortValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-sortvalues)**(const std::map< K, V > & in, const vector< K > & order) |
| template <typename T \> <br>vector< T > | **[Serialize](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-serialize)**(const vector< vector< T >> & series) |
| template <typename T ,typename U \> <br>vector< T > | **[SortFromRef](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-sortfromref)**(const vector< T > & in, const vector< U > & reference, std::function< bool(const U &, const U &)> comparer =[STLHelper::LessThan](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-lessthan)< U >) |

## Public Functions Documentation

### function HasKey

```cpp
template <typename K  =string,
typename V  =string>
static inline bool HasKey(
    const map< K, V > & dict,
    const string & key
)
```


### function GetKeys

```cpp
template <typename K  =string,
typename V  =string>
static inline vector< K > GetKeys(
    const map< K, V > & dict
)
```


### function Remap

```cpp
template <typename K  =string,
typename V  =string>
static inline map< K, V > Remap(
    const map< K, V > & dict,
    const map< K, K > & newKeys
)
```


### function Zip

```cpp
template <typename K  =string,
typename V  =string>
static inline map< K, V > Zip(
    const vector< K > & key,
    const vector< V > & values
)
```


### function GetValues

```cpp
template <typename K  =string,
typename V  =string>
static inline vector< V > GetValues(
    const map< K, V > & dict
)
```


### function GetValues

```cpp
template <typename K  =string,
typename V  =string>
static inline vector< V > GetValues(
    const map< K, V > & dict,
    const vector< K > & keys
)
```


### function LessThan

```cpp
template <typename U >
static inline bool LessThan(
    const U & first,
    const U & second
)
```


### function MoreThan

```cpp
template <typename U >
static inline bool MoreThan(
    const U & first,
    const U & second
)
```


### function SortValues

```cpp
template <typename K ,
typename V >
static inline vector< V > SortValues(
    const std::map< K, V > & in,
    const vector< K > & order
)
```


### function Serialize

```cpp
template <typename T >
static inline vector< T > Serialize(
    const vector< vector< T >> & series
)
```


### function SortFromRef

```cpp
template <typename T ,
typename U >
static inline vector< T > SortFromRef(
    const vector< T > & in,
    const vector< U > & reference,
    std::function< bool(const U &, const U &)> comparer =STLHelper::LessThan< U >
)
```


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000