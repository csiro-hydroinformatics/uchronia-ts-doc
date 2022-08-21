---
title: datatypes::utils::STLHelper
summary: Helper functions with features found in other languages but not found in the C++ standard template library. Many of these features are not used in this library (uchronia) as such, but are here as a place of convenience for dependent modelling libraries. 

---

# datatypes::utils::STLHelper



Helper functions with features found in other languages but not found in the C++ standard template library. Many of these features are not used in this library (uchronia) as such, but are here as a place of convenience for dependent modelling libraries. 


`#include <common.h>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| template <typename K  =string,typename V  =string\> <br>bool | **[HasKey](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-haskey)**(const map< K, V > & dict, const string & key)<br>is a key present in a dictionary (map)  |
| template <typename K  =string,typename V  =string\> <br>vector< K > | **[GetKeys](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-getkeys)**(const map< K, V > & dict)<br>Gets the keys present in a dictionary (map)  |
| template <typename K  =string,typename V  =string\> <br>map< K, V > | **[Remap](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-remap)**(const map< K, V > & dict, const map< K, K > & newKeys)<br>Change the keys of a dictionary with new keys, remaping.  |
| template <typename K  =string,typename V  =string\> <br>map< K, V > | **[Zip](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-zip)**(const vector< K > & key, const vector< V > & values) |
| template <typename K  =string,typename V  =string\> <br>vector< V > | **[GetValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-getvalues)**(const map< K, V > & dict)<br>Gets the values of a dictionary (map)  |
| template <typename K  =string,typename V  =string\> <br>vector< V > | **[GetValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-getvalues)**(const map< K, V > & dict, const vector< K > & keys)<br>Gets the values of a dictionary (map), for a set of keys.  |
| template <typename U \> <br>bool | **[LessThan](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-lessthan)**(const U & first, const U & second) |
| template <typename U \> <br>bool | **[MoreThan](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-morethan)**(const U & first, const U & second) |
| template <typename K ,typename V \> <br>vector< V > | **[SortValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-sortvalues)**(const std::map< K, V > & in, const vector< K > & order)<br>Gets the values of a dictionary (map), in the order specified by a set of keys.  |
| template <typename T \> <br>vector< T > | **[Serialize](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-serialize)**(const vector< vector< T >> & series)<br>Flatten jagged vectors to a one dimension vector.  |
| template <typename T ,typename U \> <br>vector< T > | **[SortFromRef](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-sortfromref)**(const vector< T > & in, const vector< U > & reference, std::function< bool(const U &, const U &)> comparer =[STLHelper::LessThan](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/#function-lessthan)< U >)<br>Reorder the values in one vector, based on the sorting of a second vector, using a specified comparer. Acknowledgements: derived from [http://stackoverflow.com/a/236199/2752565](http://stackoverflow.com/a/236199/2752565), Konrad Rudolph.  |

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

is a key present in a dictionary (map) 

### function GetKeys

```cpp
template <typename K  =string,
typename V  =string>
static inline vector< K > GetKeys(
    const map< K, V > & dict
)
```

Gets the keys present in a dictionary (map) 

### function Remap

```cpp
template <typename K  =string,
typename V  =string>
static inline map< K, V > Remap(
    const map< K, V > & dict,
    const map< K, K > & newKeys
)
```

Change the keys of a dictionary with new keys, remaping. 

**Parameters**: 

  * **dict** 
  * **newKeys** 


**Template Parameters**: 

  * **K** key type 
  * **V** value type 


**Return**: map<K, V> 

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

Gets the values of a dictionary (map) 

### function GetValues

```cpp
template <typename K  =string,
typename V  =string>
static inline vector< V > GetValues(
    const map< K, V > & dict,
    const vector< K > & keys
)
```

Gets the values of a dictionary (map), for a set of keys. 

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

Gets the values of a dictionary (map), in the order specified by a set of keys. 

### function Serialize

```cpp
template <typename T >
static inline vector< T > Serialize(
    const vector< vector< T >> & series
)
```

Flatten jagged vectors to a one dimension vector. 

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

Reorder the values in one vector, based on the sorting of a second vector, using a specified comparer. Acknowledgements: derived from [http://stackoverflow.com/a/236199/2752565](http://stackoverflow.com/a/236199/2752565), Konrad Rudolph. 

-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000