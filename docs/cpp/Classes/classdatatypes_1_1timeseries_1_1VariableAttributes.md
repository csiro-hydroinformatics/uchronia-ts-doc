---
title: datatypes::timeseries::VariableAttributes
summary: A class to hold the attributes of a netCDF variable stored in the SWIFT netCDF format. 

---

# datatypes::timeseries::VariableAttributes



A class to hold the attributes of a netCDF variable stored in the SWIFT netCDF format. 


`#include <time_series_io.hpp>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| const double | **[DefaultFillValue](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/#function-defaultfillvalue)**() |
| | **[VariableAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/#function-variableattributes)**() |
| | **[VariableAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/#function-variableattributes)**(const string & longName, const string & units, int type, const string & typeDescription, const string & datType, const string & datDescription, const string & locationType, double fillValue) |
| | **[VariableAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/#function-variableattributes)**([VariableAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/) && src) |
| | **[VariableAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/#function-variableattributes)**(const [VariableAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/) & src) |
| [VariableAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/) & | **[operator=](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/#function-operator=)**(const [VariableAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/) & src) |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| string | **[LongName](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/#variable-longname)**  |
| string | **[Units](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/#variable-units)**  |
| int | **[Type](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/#variable-type)**  |
| string | **[TypeDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/#variable-typedescription)**  |
| string | **[LocationType](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/#variable-locationtype)**  |
| string | **[DatType](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/#variable-dattype)**  |
| string | **[DatDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/#variable-datdescription)**  |
| double | **[FillValue](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/#variable-fillvalue)**  |

## Public Functions Documentation

### function DefaultFillValue

```cpp
static const double DefaultFillValue()
```


### function VariableAttributes

```cpp
VariableAttributes()
```


### function VariableAttributes

```cpp
VariableAttributes(
    const string & longName,
    const string & units,
    int type,
    const string & typeDescription,
    const string & datType,
    const string & datDescription,
    const string & locationType,
    double fillValue
)
```


### function VariableAttributes

```cpp
VariableAttributes(
    VariableAttributes && src
)
```


### function VariableAttributes

```cpp
VariableAttributes(
    const VariableAttributes & src
)
```


### function operator=

```cpp
VariableAttributes & operator=(
    const VariableAttributes & src
)
```


## Public Attributes Documentation

### variable LongName

```cpp
string LongName;
```


### variable Units

```cpp
string Units;
```


### variable Type

```cpp
int Type = 0;
```


### variable TypeDescription

```cpp
string TypeDescription;
```


### variable LocationType

```cpp
string LocationType;
```


### variable DatType

```cpp
string DatType;
```


### variable DatDescription

```cpp
string DatDescription;
```


### variable FillValue

```cpp
double FillValue;
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000