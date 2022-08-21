---
title: datatypes::timeseries::VariableDefinition

---

# datatypes::timeseries::VariableDefinition






`#include <time_series_io.hpp>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-variabledefinition)**(const string & name, const string & precision, const string & dimensions, const string & longName, const string & units, double fillValue, int type, const string & typeDescription, const string & datType, const string & datDescription, const string & locationType) |
| | **[VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-variabledefinition)**(const string & name, const [VariableAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/) & attribs, const string & dimensions, const string & precision =[DATATYPES_DOUBLE_PRECISION_ID](/uchronia-ts-doc/cpp/Files/common_8h/#define-datatypes-double-precision-id)) |
| int | **[GetPrecision](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-getprecision)**() const |
| | **[VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-variabledefinition)**() |
| | **[VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-variabledefinition)**([VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) && src) |
| | **[VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-variabledefinition)**(const [VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) & src) |
| [VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) & | **[operator=](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-operator=)**([VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) && src) |
| [VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) & | **[operator=](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-operator=)**(const [VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) & src) |
| void | **[Split](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-split)**(const std::map< string, [VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) > & varDefinitions, vector< string > & varNames, std::map< string, [VariableAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/) > & varAttributes) |
| [VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) | **[PointTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-pointtimeseries)**(const string & name, const string & units, const string & longName, int type =0, const string & typeDescription ="<NA>", const string & datType ="<NA>", const string & datDescription ="<NA>", const string & precision =[DATATYPES_DOUBLE_PRECISION_ID](/uchronia-ts-doc/cpp/Files/common_8h/#define-datatypes-double-precision-id), double fillValue =[DEFAULT_MISSING_DATA_VALUE](/uchronia-ts-doc/cpp/Files/common_8h/#define-default-missing-data-value), const string & locationType ="Point") |
| [VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) | **[TimeSeriesEnsembleTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#function-timeseriesensembletimeseries)**(const string & name, const string & units, const string & longName, int type =0, const string & typeDescription ="<NA>", const string & datType ="<NA>", const string & datDescription ="<NA>", const string & precision =[DATATYPES_DOUBLE_PRECISION_ID](/uchronia-ts-doc/cpp/Files/common_8h/#define-datatypes-double-precision-id), double fillValue =[DEFAULT_MISSING_DATA_VALUE](/uchronia-ts-doc/cpp/Files/common_8h/#define-default-missing-data-value), const string & locationType ="Point") |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| [VariableAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/) | **[attributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#variable-attributes)**  |
| string | **[Name](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#variable-name)**  |
| string | **[Precision](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#variable-precision)**  |
| string | **[Dimensions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/#variable-dimensions)**  |

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

Updated on 2022-08-21 at 18:10:33 +1000