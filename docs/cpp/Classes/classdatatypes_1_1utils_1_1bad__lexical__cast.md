---
title: datatypes::utils::bad_lexical_cast
summary: A bad_lexical_cast that inherits from std::exception, unlike Boost's. Needed for graceful C API interop. 

---

# datatypes::utils::bad_lexical_cast



A [bad_lexical_cast]() that inherits from std::exception, unlike Boost's. Needed for graceful C API interop. 


`#include <common.h>`

Inherits from std::invalid_argument

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[bad_lexical_cast](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1bad__lexical__cast/#function-bad-lexical-cast)**(const string & msg) |

## Public Functions Documentation

### function bad_lexical_cast

```cpp
bad_lexical_cast(
    const string & msg
)
```


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000