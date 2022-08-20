---
title: datatypes::timeseries::VariableDefinition

---

# datatypes::timeseries::VariableDefinition






`#include <time_series_io.hpp>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-variabledefinition)**(const string & name, const string & precision, const string & dimensions, const string & longName, const string & units, double fillValue, int type, const string & typeDescription, const string & datType, const string & datDescription, const string & locationType) |
| | **[VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-variabledefinition)**(const string & name, const [VariableAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/) & attribs, const string & dimensions, const string & precision =[DATATYPES_DOUBLE_PRECISION_ID](/cpp/Files/common_8h/#define-datatypes-double-precision-id)) |
| int | **[GetPrecision](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-getprecision)**() const |
| | **[VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-variabledefinition)**() |
| | **[VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-variabledefinition)**([VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) && src) |
| | **[VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-variabledefinition)**(const [VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) & src) |
| [VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) & | **[operator=](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-operator=)**([VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) && src) |
| [VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) & | **[operator=](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-operator=)**(const [VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) & src) |
| void | **[Split](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-split)**(const std::map< string, [VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) > & varDefinitions, vector< string > & varNames, std::map< string, [VariableAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/) > & varAttributes) |
| [VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) | **[PointTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-pointtimeseries)**(const string & name, const string & units, const string & longName, int type =0, const string & typeDescription ="<NA>", const string & datType ="<NA>", const string & datDescription ="<NA>", const string & precision =[DATATYPES_DOUBLE_PRECISION_ID](/cpp/Files/common_8h/#define-datatypes-double-precision-id), double fillValue =[DEFAULT_MISSING_DATA_VALUE](/cpp/Files/common_8h/#define-default-missing-data-value), const string & locationType ="Point") |
| [VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) | **[TimeSeriesEnsembleTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-timeseriesensembletimeseries)**(const string & name, const string & units, const string & longName, int type =0, const string & typeDescription ="<NA>", const string & datType ="<NA>", const string & datDescription ="<NA>", const string & precision =[DATATYPES_DOUBLE_PRECISION_ID](/cpp/Files/common_8h/#define-datatypes-double-precision-id), double fillValue =[DEFAULT_MISSING_DATA_VALUE](/cpp/Files/common_8h/#define-default-missing-data-value), const string & locationType ="Point") |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| [VariableAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/) | **[attributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#variable-attributes)**  |
| string | **[Name](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#variable-name)**  |
| string | **[Precision](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#variable-precision)**  |
| string | **[Dimensions](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#variable-dimensions)**  |

## Public Functions Documentation

### function VariableDefinition

```cpp
VariableDefinition(
    const string & name,
    const string & precision,
    const string & dimensions,
    const string & longName,
    const string & units,
    double fillValue,
    int type,
    const string & typeDescription,
    const string & datType,
    const string & datDescription,
    const string & locationType
)
```


### function VariableDefinition

```cpp
VariableDefinition(
    const string & name,
    const VariableAttributes & attribs,
    const string & dimensions,
    const string & precision =DATATYPES_DOUBLE_PRECISION_ID
)
```


### function GetPrecision

```cpp
int GetPrecision() const
```


### function VariableDefinition

```cpp
VariableDefinition()
```


### function VariableDefinition

```cpp
VariableDefinition(
    VariableDefinition && src
)
```


### function VariableDefinition

```cpp
VariableDefinition(
    const VariableDefinition & src
)
```


### function operator=

```cpp
VariableDefinition & operator=(
    VariableDefinition && src
)
```


### function operator=

```cpp
VariableDefinition & operator=(
    const VariableDefinition & src
)
```


### function Split

```cpp
static void Split(
    const std::map< string, VariableDefinition > & varDefinitions,
    vector< string > & varNames,
    std::map< string, VariableAttributes > & varAttributes
)
```


### function PointTimeSeries

```cpp
static VariableDefinition PointTimeSeries(
    const string & name,
    const string & units,
    const string & longName,
    int type =0,
    const string & typeDescription ="<NA>",
    const string & datType ="<NA>",
    const string & datDescription ="<NA>",
    const string & precision =DATATYPES_DOUBLE_PRECISION_ID,
    double fillValue =DEFAULT_MISSING_DATA_VALUE,
    const string & locationType ="Point"
)
```


### function TimeSeriesEnsembleTimeSeries

```cpp
static VariableDefinition TimeSeriesEnsembleTimeSeries(
    const string & name,
    const string & units,
    const string & longName,
    int type =0,
    const string & typeDescription ="<NA>",
    const string & datType ="<NA>",
    const string & datDescription ="<NA>",
    const string & precision =DATATYPES_DOUBLE_PRECISION_ID,
    double fillValue =DEFAULT_MISSING_DATA_VALUE,
    const string & locationType ="Point"
)
```


## Public Attributes Documentation

### variable attributes

```cpp
VariableAttributes attributes;
```


### variable Name

```cpp
string Name;
```


### variable Precision

```cpp
string Precision;
```


### variable Dimensions

```cpp
string Dimensions;
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000