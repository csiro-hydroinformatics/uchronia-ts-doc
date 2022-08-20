---
title: datatypes::io::IoHelper

---

# datatypes::io::IoHelper






`#include <io_helper.h>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| bool | **[FileExists](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1io_1_1IoHelper/#function-fileexists)**(const boost::filesystem::path & p) |
| bool | **[PathExists](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1io_1_1IoHelper/#function-pathexists)**(const boost::filesystem::path & p) |
| bool | **[DirExists](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1io_1_1IoHelper/#function-direxists)**(const boost::filesystem::path & p) |
| string | **[MakeFileName](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1io_1_1IoHelper/#function-makefilename)**(const string & fileNamePattern, const string & id, const string & pattern ="{0}") |
| bool | **[IsFileNamePattern](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1io_1_1IoHelper/#function-isfilenamepattern)**(const string & s) |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| const string | **[DefaultFilePattern](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1io_1_1IoHelper/#variable-defaultfilepattern)**  |

## Public Functions Documentation

### function FileExists

```cpp
static bool FileExists(
    const boost::filesystem::path & p
)
```


### function PathExists

```cpp
static bool PathExists(
    const boost::filesystem::path & p
)
```


### function DirExists

```cpp
static bool DirExists(
    const boost::filesystem::path & p
)
```


### function MakeFileName

```cpp
static string MakeFileName(
    const string & fileNamePattern,
    const string & id,
    const string & pattern ="{0}"
)
```


### function IsFileNamePattern

```cpp
static bool IsFileNamePattern(
    const string & s
)
```


## Public Attributes Documentation

### variable DefaultFilePattern

```cpp
static const string DefaultFilePattern;
```


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000