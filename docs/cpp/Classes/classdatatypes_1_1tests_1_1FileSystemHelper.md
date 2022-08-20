---
title: datatypes::tests::FileSystemHelper

---

# datatypes::tests::FileSystemHelper






`#include <datatypes_test_helpers.h>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| boost::filesystem::path | **[GetTempFile](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1FileSystemHelper/#function-gettempfile)**(const string & format ="%%%%%%%%%%%%.tmp") |
| boost::filesystem::path | **[GetTempDir](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1FileSystemHelper/#function-gettempdir)**(const string & format ="%%%%%%%%%%%%") |
| void | **[Remove](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1FileSystemHelper/#function-remove)**(const boost::filesystem::path & p) |
| void | **[Remove](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1FileSystemHelper/#function-remove)**(const string & p) |
| bool | **[Exists](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1FileSystemHelper/#function-exists)**(const string & p) |
| bool | **[Exists](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1FileSystemHelper/#function-exists)**(const boost::filesystem::path & p) |

## Public Functions Documentation

### function GetTempFile

```cpp
static boost::filesystem::path GetTempFile(
    const string & format ="%%%%%%%%%%%%.tmp"
)
```


### function GetTempDir

```cpp
static boost::filesystem::path GetTempDir(
    const string & format ="%%%%%%%%%%%%"
)
```


### function Remove

```cpp
static void Remove(
    const boost::filesystem::path & p
)
```


### function Remove

```cpp
static void Remove(
    const string & p
)
```


### function Exists

```cpp
static bool Exists(
    const string & p
)
```


### function Exists

```cpp
static bool Exists(
    const boost::filesystem::path & p
)
```


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000