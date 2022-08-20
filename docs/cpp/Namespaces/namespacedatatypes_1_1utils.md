---
title: datatypes::utils

---

# datatypes::utils



## Classes

|                | Name           |
| -------------- | -------------- |
| class | **[datatypes::utils::STLHelper](/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/)**  |
| class | **[datatypes::utils::IfThenElse](/cpp/Classes/classdatatypes_1_1utils_1_1IfThenElse/)**  |
| class | **[datatypes::utils::IfThenElse< true, Ta, Tb >](/cpp/Classes/classdatatypes_1_1utils_1_1IfThenElse_3_01true_00_01Ta_00_01Tb_01_4/)**  |
| class | **[datatypes::utils::IfThenElse< false, Ta, Tb >](/cpp/Classes/classdatatypes_1_1utils_1_1IfThenElse_3_01false_00_01Ta_00_01Tb_01_4/)**  |
| class | **[datatypes::utils::ValueTypeVectorDispose](/cpp/Classes/classdatatypes_1_1utils_1_1ValueTypeVectorDispose/)**  |
| class | **[datatypes::utils::PointerTypeVectorDispose](/cpp/Classes/classdatatypes_1_1utils_1_1PointerTypeVectorDispose/)**  |
| struct | **[datatypes::utils::DisposeVectorTypeFactory](/cpp/Classes/structdatatypes_1_1utils_1_1DisposeVectorTypeFactory/)**  |
| class | **[datatypes::utils::bad_lexical_cast](/cpp/Classes/classdatatypes_1_1utils_1_1bad__lexical__cast/)** <br>A [bad_lexical_cast]() that inherits from std::exception, unlike Boost's. Needed for graceful C API interop.  |
| class | **[datatypes::utils::StringProcessing](/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/)**  |

## Functions

|                | Name           |
| -------------- | -------------- |
| void | **[datatypes_delete_ansi_string_array](/cpp/Namespaces/namespacedatatypes_1_1utils/#function-datatypes-delete-ansi-string-array)**(char ** values, int arrayLength) |
| template <typename T  =double\> <br>vector< T > | **[SeqVec](/cpp/Namespaces/namespacedatatypes_1_1utils/#function-seqvec)**(T from, T by, size_t num) |
| template <typename T \> <br>void | **[DisposeVector](/cpp/Namespaces/namespacedatatypes_1_1utils/#function-disposevector)**(vector< T > & v) |
| template <typename Target \> <br>Target | **[Parse](/cpp/Namespaces/namespacedatatypes_1_1utils/#function-parse)**(const string & strId)<br>Wraps boost::lexical_cast with a try/catch; rethrows an exception that inherits from std::exception and a more useful error message.  |
| template <typename Source \> <br>string | **[ToString](/cpp/Namespaces/namespacedatatypes_1_1utils/#function-tostring)**(const Source & value) |
| template <class TTo \> <br>TTo * | **[ConvertToArray](/cpp/Namespaces/namespacedatatypes_1_1utils/#function-converttoarray)**(const vector< string > & src) |
| template <class TFrom ,class TTo \> <br>TTo * | **[ConvertToArray](/cpp/Namespaces/namespacedatatypes_1_1utils/#function-converttoarray)**(const vector< TFrom > & src) |
| template <class TFrom ,class TTo \> <br>vector< TTo > | **[Convert](/cpp/Namespaces/namespacedatatypes_1_1utils/#function-convert)**(const vector< TFrom > & src) |
| template <class TTo \> <br>vector< TTo > | **[Convert](/cpp/Namespaces/namespacedatatypes_1_1utils/#function-convert)**(const vector< string > & src) |
| template <typename T  =boost::posix_time::ptime\> <br>T | **[CreateTime](/cpp/Namespaces/namespacedatatypes_1_1utils/#function-createtime)**(int year, int month, int day, int hour =0, int minute =0, int second =0) |


## Functions Documentation

### function datatypes_delete_ansi_string_array

```cpp
void datatypes_delete_ansi_string_array(
    char ** values,
    int arrayLength
)
```


### function SeqVec

```cpp
template <typename T  =double>
vector< T > SeqVec(
    T from,
    T by,
    size_t num
)
```


### function DisposeVector

```cpp
template <typename T >
void DisposeVector(
    vector< T > & v
)
```


### function Parse

```cpp
template <typename Target >
static Target Parse(
    const string & strId
)
```

Wraps boost::lexical_cast with a try/catch; rethrows an exception that inherits from std::exception and a more useful error message. 

### function ToString

```cpp
template <typename Source >
static string ToString(
    const Source & value
)
```


### function ConvertToArray

```cpp
template <class TTo >
static TTo * ConvertToArray(
    const vector< string > & src
)
```


### function ConvertToArray

```cpp
template <class TFrom ,
class TTo >
static TTo * ConvertToArray(
    const vector< TFrom > & src
)
```


### function Convert

```cpp
template <class TFrom ,
class TTo >
static vector< TTo > Convert(
    const vector< TFrom > & src
)
```


### function Convert

```cpp
template <class TTo >
vector< TTo > Convert(
    const vector< string > & src
)
```


### function CreateTime

```cpp
template <typename T  =boost::posix_time::ptime>
T CreateTime(
    int year,
    int month,
    int day,
    int hour =0,
    int minute =0,
    int second =0
)
```






-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000