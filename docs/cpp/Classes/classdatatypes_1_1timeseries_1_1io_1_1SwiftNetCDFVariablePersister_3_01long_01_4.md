---
title: datatypes::timeseries::io::SwiftNetCDFVariablePersister< long >

---

# datatypes::timeseries::io::SwiftNetCDFVariablePersister< long >






`#include <time_series_io.hpp>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| int | **[NcGetVara](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFVariablePersister_3_01long_01_4/#function-ncgetvara)**(int ncid, int varid, const size_t * startp, const size_t * countp, long * op) |
| int | **[NcPutVara](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFVariablePersister_3_01long_01_4/#function-ncputvara)**(int ncid, int varid, const size_t * startp, const size_t * countp, const long * op) |

## Public Functions Documentation

### function NcGetVara

```cpp
static inline int NcGetVara(
    int ncid,
    int varid,
    const size_t * startp,
    const size_t * countp,
    long * op
)
```


### function NcPutVara

```cpp
static inline int NcPutVara(
    int ncid,
    int varid,
    const size_t * startp,
    const size_t * countp,
    const long * op
)
```


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000