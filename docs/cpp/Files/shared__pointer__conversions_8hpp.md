---
title: datatypes/shared_pointer_conversions.hpp

---

# datatypes/shared_pointer_conversions.hpp



## Namespaces

| Name           |
| -------------- |
| **[moirai](/cpp/Namespaces/namespacemoirai/)**  |

## Classes

|                | Name           |
| -------------- | -------------- |
| struct | **[moirai::known_conversions< TimeSeriesProvider< double > >](/cpp/Classes/structmoirai_1_1known__conversions_3_01TimeSeriesProvider_3_01double_01_4_01_4/)**  |




## Source code

```cpp
#pragma once

#include "datatypes/setup_exports.h"
#include "moirai/reference_handle.hpp"

namespace moirai
{
    template<> struct known_conversions<TimeSeriesProvider<double>>
    {
        static TimeSeriesProvider<double>* dyn_cast(void* p, const typeinfo& tinfo)
        {
            return as_type<TimeSeriesLibrary>(p, tinfo);
        }
    };
}
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000
