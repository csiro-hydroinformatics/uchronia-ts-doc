---
title: datatypes::timeseries::io::SwiftNetCDFVariablePersister

---

# datatypes::timeseries::io::SwiftNetCDFVariablePersister



 [More...](#detailed-description)


`#include <time_series_io.hpp>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| int | **[NcGetVara](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFVariablePersister/#function-ncgetvara)**(int ncid, int varid, const size_t * startp, const size_t * countp, ElementType * op) |
| int | **[NcPutVara](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFVariablePersister/#function-ncputvara)**(int ncid, int varid, const size_t * startp, const size_t * countp, const ElementType * op) |

## Detailed Description

```cpp
template <typename ElementType >
class datatypes::timeseries::io::SwiftNetCDFVariablePersister;
```

## Public Functions Documentation

### function NcGetVara

```cpp
static inline int NcGetVara(
    int ncid,
    int varid,
    const size_t * startp,
    const size_t * countp,
    ElementType * op
)
```


### function NcPutVara

```cpp
static inline int NcPutVara(
    int ncid,
    int varid,
    const size_t * startp,
    const size_t * countp,
    const ElementType * op
)
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000