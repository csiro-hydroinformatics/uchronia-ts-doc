---
title: datatypes::interop::MissingValueHandling
summary: Ways for wrappers to specify to this API what special numeric value to use as 'missing value' code in time series interop. 

---

# datatypes::interop::MissingValueHandling



Ways for wrappers to specify to this API what special numeric value to use as 'missing value' code in time series interop. 


`#include <common.h>`

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| std::atomic< double > | **[TimeSeriesMissingValueValue](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1interop_1_1MissingValueHandling/#variable-timeseriesmissingvaluevalue)** <br>The time series missing value.  |

## Public Attributes Documentation

### variable TimeSeriesMissingValueValue

```cpp
static std::atomic< double > TimeSeriesMissingValueValue;
```

The time series missing value. 

-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000