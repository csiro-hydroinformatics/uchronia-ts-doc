---
title: datatypes/io_helper.h

---

# datatypes/io_helper.h



## Namespaces

| Name           |
| -------------- |
| **[datatypes](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes/)**  |
| **[datatypes::io](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1io/)**  |

## Classes

|                | Name           |
| -------------- | -------------- |
| class | **[datatypes::io::IoHelper](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1io_1_1IoHelper/)**  |




## Source code

```cpp
#pragma once
#include <string> 
#include <stdexcept> 
#include <boost/filesystem.hpp>
#include "common.h"

using std::string;

namespace datatypes
{
    namespace io
    {
        class DATATYPES_DLL_LIB IoHelper
        {
        public:
            static const string DefaultFilePattern;
            static bool FileExists(const boost::filesystem::path& p);
            static bool PathExists(const boost::filesystem::path& p);
            static bool DirExists(const boost::filesystem::path& p);
            static string MakeFileName(const string& fileNamePattern, const string& id, const string& pattern = "{0}");
            static bool IsFileNamePattern(const string& s);
        };
    }
}
```


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000
