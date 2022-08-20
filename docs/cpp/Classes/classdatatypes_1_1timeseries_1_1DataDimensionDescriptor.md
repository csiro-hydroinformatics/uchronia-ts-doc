---
title: datatypes::timeseries::DataDimensionDescriptor

---

# datatypes::timeseries::DataDimensionDescriptor






`#include <time_series_store.hpp>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[DataDimensionDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/#function-datadimensiondescriptor)**(const string & type, const string & dimname ="", size_t size =0) |
| | **[DataDimensionDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/#function-datadimensiondescriptor)**(const [DataDimensionDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) & src) |
| | **[DataDimensionDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/#function-datadimensiondescriptor)**([DataDimensionDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) && src) |
| [DataDimensionDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) & | **[operator=](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/#function-operator=)**(const [DataDimensionDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) & src) |
| [DataDimensionDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) & | **[operator=](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/#function-operator=)**([DataDimensionDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) && src) |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| string | **[DimensionType](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/#variable-dimensiontype)**  |
| string | **[DimensionName](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/#variable-dimensionname)**  |
| size_t | **[Size](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/#variable-size)**  |

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

Updated on 2022-08-20 at 18:35:57 +1000