---
title: datatypes::timeseries::GlobalAttributes
summary: A class to hold the global attributes of a file stored in the SWIFT netCDF format. 

---

# datatypes::timeseries::GlobalAttributes



A class to hold the global attributes of a file stored in the SWIFT netCDF format. 


`#include <time_series_io.hpp>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[GlobalAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/#function-globalattributes)**() |
| | **[GlobalAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/#function-globalattributes)**(const string & title, const string & institution, const string & source, const string & catchment, double stfConventionVersion, const string & stfNcSpec, const string & comment, const string & history) |
| | **[GlobalAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/#function-globalattributes)**([GlobalAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) && src) |
| | **[GlobalAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/#function-globalattributes)**(const [GlobalAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) & src) |
| [GlobalAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) & | **[operator=](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/#function-operator=)**(const [GlobalAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) & src) |
| [GlobalAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) | **[CreateDefault](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/#function-createdefault)**() |
| [GlobalAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) | **[CreateDefault](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/#function-createdefault)**(const string & catchment) |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| string | **[Title](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/#variable-title)**  |
| string | **[Institution](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/#variable-institution)**  |
| string | **[Source](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/#variable-source)**  |
| string | **[Catchment](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/#variable-catchment)**  |
| double | **[STFConventionVersion](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/#variable-stfconventionversion)**  |
| string | **[STFNCSpec](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/#variable-stfncspec)**  |
| string | **[Comment](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/#variable-comment)**  |
| string | **[History](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/#variable-history)**  |

## Public Functions Documentation

### function GlobalAttributes

```cpp
GlobalAttributes()
```


### function GlobalAttributes

```cpp
GlobalAttributes(
    const string & title,
    const string & institution,
    const string & source,
    const string & catchment,
    double stfConventionVersion,
    const string & stfNcSpec,
    const string & comment,
    const string & history
)
```


### function GlobalAttributes

```cpp
GlobalAttributes(
    GlobalAttributes && src
)
```


### function GlobalAttributes

```cpp
GlobalAttributes(
    const GlobalAttributes & src
)
```


### function operator=

```cpp
GlobalAttributes & operator=(
    const GlobalAttributes & src
)
```


### function CreateDefault

```cpp
static GlobalAttributes CreateDefault()
```


### function CreateDefault

```cpp
static GlobalAttributes CreateDefault(
    const string & catchment
)
```


## Public Attributes Documentation

### variable Title

```cpp
string Title;
```


### variable Institution

```cpp
string Institution;
```


### variable Source

```cpp
string Source;
```


### variable Catchment

```cpp
string Catchment;
```


### variable STFConventionVersion

```cpp
double STFConventionVersion;
```


### variable STFNCSpec

```cpp
string STFNCSpec;
```


### variable Comment

```cpp
string Comment;
```


### variable History

```cpp
string History;
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000