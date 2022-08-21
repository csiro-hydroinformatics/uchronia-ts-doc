---
title: datatypes::timeseries::io::SwiftNetCDFVariablePersister< float >

---

# datatypes::timeseries::io::SwiftNetCDFVariablePersister< float >






`#include <time_series_io.hpp>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| int | **[NcGetVara](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFVariablePersister_3_01float_01_4/#function-ncgetvara)**(int ncid, int varid, const size_t * startp, const size_t * countp, float * op) |
| int | **[NcPutVara](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFVariablePersister_3_01float_01_4/#function-ncputvara)**(int ncid, int varid, const size_t * startp, const size_t * countp, const float * op) |

## Public Functions Documentation

### function NcGetVara

```cpp
static inline int NcGetVara(
    int ncid,
    int varid,
    const size_t * startp,
    const size_t * countp,
    float * op
)
```


### function NcPutVara

```cpp
static inline int NcPutVara(
    int ncid,
    int varid,
    const size_t * startp,
    const size_t * countp,
    const float * op
)
```


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000