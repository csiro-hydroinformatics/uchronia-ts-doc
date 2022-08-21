---
title: datatypes::timeseries::DataDimensionDescriptor
summary: Basic descriptor for a named dimension of a data structure (time series). 

---

# datatypes::timeseries::DataDimensionDescriptor



Basic descriptor for a named dimension of a data structure (time series). 


`#include <time_series_store.hpp>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[DataDimensionDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/#function-datadimensiondescriptor)**(const string & type, const string & dimname ="", size_t size =0) |
| | **[DataDimensionDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/#function-datadimensiondescriptor)**(const [DataDimensionDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) & src) |
| | **[DataDimensionDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/#function-datadimensiondescriptor)**([DataDimensionDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) && src) |
| [DataDimensionDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) & | **[operator=](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/#function-operator=)**(const [DataDimensionDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) & src) |
| [DataDimensionDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) & | **[operator=](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/#function-operator=)**([DataDimensionDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) && src) |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| string | **[DimensionType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/#variable-dimensiontype)**  |
| string | **[DimensionName](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/#variable-dimensionname)**  |
| size_t | **[Size](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/#variable-size)**  |

## Public Functions Documentation

### function DataDimensionDescriptor

```cpp
DataDimensionDescriptor(
    const string & type,
    const string & dimname ="",
    size_t size =0
)
```


### function DataDimensionDescriptor

```cpp
DataDimensionDescriptor(
    const DataDimensionDescriptor & src
)
```


### function DataDimensionDescriptor

```cpp
DataDimensionDescriptor(
    DataDimensionDescriptor && src
)
```


### function operator=

```cpp
DataDimensionDescriptor & operator=(
    const DataDimensionDescriptor & src
)
```


### function operator=

```cpp
DataDimensionDescriptor & operator=(
    DataDimensionDescriptor && src
)
```


## Public Attributes Documentation

### variable DimensionType

```cpp
string DimensionType;
```


### variable DimensionName

```cpp
string DimensionName;
```


### variable Size

```cpp
size_t Size = 0;
```


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000