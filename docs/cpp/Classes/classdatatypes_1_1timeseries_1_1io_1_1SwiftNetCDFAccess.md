---
title: datatypes::timeseries::io::SwiftNetCDFAccess
summary: Class responsible for the low-level read/write operations from/to a SWIFT netCDF file. 

---

# datatypes::timeseries::io::SwiftNetCDFAccess



Class responsible for the low-level read/write operations from/to a SWIFT netCDF file. 


`#include <time_series_io.hpp>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[SwiftNetCDFAccess](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-swiftnetcdfaccess)**(const string & filename, bool lazyLoad =false)<br>Constructor to wrap an existing SWIFT netCDF file.  |
| | **[SwiftNetCDFAccess](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-swiftnetcdfaccess)**(const string & filename, const size_t nEns, const vector< double > & leadTimeVar, const string & timeUnits, const vector< double > & timeVar, const vector< string > & stationIds, const std::map< string, [VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) > & varDefinitions, const [GlobalAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) & globalAttributes, const string & leadTimeUnits ="")<br>**  |
| | **[SwiftNetCDFAccess](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-swiftnetcdfaccess)**(const string & filename, const [DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) & dimDefinitions, const std::map< string, [VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) > & varDefinitions, const [GlobalAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) & globalAttributes) |
| | **[~SwiftNetCDFAccess](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-~swiftnetcdfaccess)**() |
| size_t | **[GetEnsembleSize](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getensemblesize)**()<br>Gets ensemble size.  |
| size_t | **[GetEnsembleSize](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getensemblesize)**(const string & ncVarName) |
| size_t | **[GetLeadTimeCount](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getleadtimecount)**()<br>Gets the lengths of the lead time dimension.  |
| size_t | **[GetLeadTimeCount](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getleadtimecount)**(const string & ncVarName) |
| size_t | **[GetTimeLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-gettimelength)**() const<br>Gets the lengths of the main time dimension.  |
| vector< ptime > | **[GetTimeDim](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-gettimedim)**()<br>Gets the vector with the values of the main time dimension.  |
| ptime | **[GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getstart)**()<br>Gets the first time in the main time dimension of this netCDF data set.  |
| ptime | **[GetEnd](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getend)**()<br>Gets the last time in the main time dimension of this netCDF data set.  |
| size_t | **[IndexForIdentifier](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-indexforidentifier)**(const string & identifier) const<br>Corresponding index for a string identifier for a variable in this data set.  |
| size_t | **[GetNumIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getnumidentifiers)**() const |
| vector< string > | **[GetIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getidentifiers)**() const |
| ptime | **[TimeForIndex](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-timeforindex)**(size_t timeIndex)<br>Time value for an index of the time dimension.  |
| template <typename ElementType \> <br>vector< ElementType * > * | **[GetForecasts](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getforecasts)**(const string & varName, size_t stationIndex, size_t timeIndex)<br>Gets the values of an ensemble forecast for a variable, for a starting date in the main time dimension.  |
| template <typename ElementType \> <br>vector< ElementType * > * | **[GetEnsemble](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getensemble)**(const string & varName, size_t stationIndex) |
| template <typename ElementType \> <br>vector< ElementType > | **[GetValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getvalues)**(const string & varName, size_t stationIndex)<br>Gets the values of a variable stored as an non-ensemble series.  |
| template <typename ElementType \> <br>vector< ElementType > | **[GetValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getvalues)**(const string & varName) |
| template <typename ElementType \> <br>[TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< ElementType > * | **[GetSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getseries)**(const string & varName, size_t stationIndex) |
| template <typename ElementType \> <br>[MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< ElementType > * > * | **[GetSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getseries)**(const string & varName) |
| template <typename ElementType \> <br>[MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< ElementType > * > * | **[GetEnsembleSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getensembleseries)**(const string & varName, size_t stationIndex) |
| template <typename ElementType \> <br>void | **[SetForecasts](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-setforecasts)**(const string & varName, size_t stationIndex, size_t timeIndex, vector< ElementType * > & values)<br>Sets the values for an ensemble forecast, for a variable, for a starting date in the main time dimension.  |
| template <typename ElementType \> <br>void | **[SetEnsembles](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-setensembles)**(const string & varName, size_t stationIndex, vector< ElementType * > & values) |
| template <typename ElementType \> <br>void | **[SetValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-setvalues)**(const string & varName, size_t stationIndex, const vector< ElementType > & values) |
| template <typename ElementType \> <br>void | **[SetValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-setvalues)**(const string & varName, const vector< ElementType > & values) |
| vector< int > | **[GetVarDims](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getvardims)**(int varNumDims) |
| vector< int > | **[GetVarDims](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getvardims)**(const string & varName) |
| vector< string > | **[ReadVariableNames](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-readvariablenames)**(bool removeDimVars =true) |
| vector< string > | **[ReadAttributeNames](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-readattributenames)**(const string & varName) |
| string | **[ReadStringAttribute](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-readstringattribute)**(int varId, const string & attName, bool throwIfNotFound =false, string defaultValue ="") |
| string | **[ReadStringAttribute](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-readstringattribute)**(const string & varName, const string & attName, bool throwIfNotFound =false, string defaultValue ="") |
| double | **[ReadNumericAttribute](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-readnumericattribute)**(int varId, const string & attName, bool throwIfNotFound =false, double defaultValue =0.0) |
| double | **[ReadNumericAttribute](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-readnumericattribute)**(const string & varName, const string & attName, bool throwIfNotFound =false, double defaultValue =0.0) |
| [VariableAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/) | **[ReadAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-readattributes)**(const string & varName) |
| [GlobalAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) | **[ReadGlobalAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-readglobalattributes)**() |
| [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-gettimestep)**() |
| [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetLeadTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getleadtimestep)**() |
| std::pair< ptime, [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) > | **[GetLeadTimeGeometry](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getleadtimegeometry)**(const ptime & issueTime) |
| vector< double > | **[GetLeadTimeDim](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getleadtimedim)**() |
| [GlobalAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) | **[GetGlobalAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getglobalattributes)**() |
| [VariableAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/) | **[GetAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-getattributes)**(const string & varName) |
| void | **[CheckCompliance](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-checkcompliance)**(const string & filename, int majorVersion, int minorVersion, vector< string > & warnings, vector< string > & errors) |
| template <typename ElementType \> <br>string | **[CreateTimeUnitsAttribute](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-createtimeunitsattribute)**(const [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< ElementType > & tSeries) |
| std::pair< vector< double >, vector< double > > | **[CreateTimeVectors](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-createtimevectors)**(const ptime & start, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep, size_t tsLength, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & leadTimeStep, size_t leadTimeSize, int fcastOffset =1) |
| vector< double > | **[CreateTimeVector](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-createtimevector)**(const ptime & start, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep, const ptime & origin, const time_duration & timeStepAxis, const size_t length) |
| vector< double > | **[CreateTimeVector](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-createtimevector)**(const ptime & start, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep, const ptime & origin, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStepAxis, const size_t length) |
| vector< double > | **[CreateTimeVector](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-createtimevector)**(const ptime & start, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep, const size_t length) |
| template <typename ElementType \> <br>vector< double > | **[CreateTimeVector](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-createtimevector)**(const [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< ElementType > & tSeries) |
| template <typename ElementType \> <br>vector< double > | **[CreateTimeVector](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-createtimevector)**(const [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< ElementType > & tSeries, const ptime & origin, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStepAxis) |
| template <typename T \> <br>ptime | **[StartCoordinate](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-startcoordinate)**(const ptime & origin, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep, const vector< T > & timeCoords) |
| std::pair< ptime, [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) > | **[CreateTimeGeometry](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-createtimegeometry)**(const string & axisDefinition, const vector< double > & timeCoords) |
| string | **[GetTimeStepName](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-gettimestepname)**(const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| string | **[CreateTimeUnitsAttribute](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-createtimeunitsattribute)**(const ptime & utcStart, const string & units) |
| string | **[CreateTimeUnitsAttribute](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-createtimeunitsattribute)**(const ptime & utcStart, const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| ptime | **[ParseStartDate](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-parsestartdate)**(const string & unitsAttribute) |
| string | **[ParseTimeUnits](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-parsetimeunits)**(const string & unitsAttribute) |
| string | **[CreateLeadTimeUnitsAttribute](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-createleadtimeunitsattribute)**(const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| template <class TFrom ,class TTo \> <br>vector< TTo > | **[Convert](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-convert)**(const vector< TFrom > & from, const std::function< TTo(const TFrom &)> & f) |
| time_duration | **[CreateTimeUnits](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-createtimeunits)**(const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & timeStep) |
| void | **[SetTimeOffsetIn](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-settimeoffsetin)**(const time_duration & td) |
| void | **[SetTimeOffsetOut](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#function-settimeoffsetout)**(const time_duration & td) |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| time_duration | **[TimeOffsetIn](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#variable-timeoffsetin)**  |
| time_duration | **[TimeOffsetOut](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/#variable-timeoffsetout)**  |

## Public Functions Documentation

### function SwiftNetCDFAccess

```cpp
SwiftNetCDFAccess(
    const string & filename,
    bool lazyLoad =false
)
```

Constructor to wrap an existing SWIFT netCDF file. 

**Parameters**: 

  * **filename** SWIFT netCDF file. 


### function SwiftNetCDFAccess

```cpp
SwiftNetCDFAccess(
    const string & filename,
    const size_t nEns,
    const vector< double > & leadTimeVar,
    const string & timeUnits,
    const vector< double > & timeVar,
    const vector< string > & stationIds,
    const std::map< string, VariableDefinition > & varDefinitions,
    const GlobalAttributes & globalAttributes,
    const string & leadTimeUnits =""
)
```

** 

### function SwiftNetCDFAccess

```cpp
SwiftNetCDFAccess(
    const string & filename,
    const DimensionsDefinitions & dimDefinitions,
    const std::map< string, VariableDefinition > & varDefinitions,
    const GlobalAttributes & globalAttributes
)
```


### function ~SwiftNetCDFAccess

```cpp
~SwiftNetCDFAccess()
```


### function GetEnsembleSize

```cpp
size_t GetEnsembleSize()
```

Gets ensemble size. 

**Return**: The ensemble size. 

### function GetEnsembleSize

```cpp
size_t GetEnsembleSize(
    const string & ncVarName
)
```


### function GetLeadTimeCount

```cpp
size_t GetLeadTimeCount()
```

Gets the lengths of the lead time dimension. 

**Return**: The lead time length. 

### function GetLeadTimeCount

```cpp
size_t GetLeadTimeCount(
    const string & ncVarName
)
```


### function GetTimeLength

```cpp
size_t GetTimeLength() const
```

Gets the lengths of the main time dimension. 

**Return**: The time length. 

### function GetTimeDim

```cpp
vector< ptime > GetTimeDim()
```

Gets the vector with the values of the main time dimension. 

**Return**: the values of the main time dimension 

### function GetStart

```cpp
ptime GetStart()
```

Gets the first time in the main time dimension of this netCDF data set. 

**Return**: The start date of the data set. 

### function GetEnd

```cpp
ptime GetEnd()
```

Gets the last time in the main time dimension of this netCDF data set. 

**Return**: The end date of the data set. 

### function IndexForIdentifier

```cpp
size_t IndexForIdentifier(
    const string & identifier
) const
```

Corresponding index for a string identifier for a variable in this data set. 

**Parameters**: 

  * **identifier** The identifier.


**Return**: An int. 

### function GetNumIdentifiers

```cpp
size_t GetNumIdentifiers() const
```


### function GetIdentifiers

```cpp
vector< string > GetIdentifiers() const
```


### function TimeForIndex

```cpp
ptime TimeForIndex(
    size_t timeIndex
)
```

Time value for an index of the time dimension. 

**Parameters**: 

  * **timeIndex** Zero-based index of the time.


**Return**: A ptime. 

### function GetForecasts

```cpp
template <typename ElementType >
inline vector< ElementType * > * GetForecasts(
    const string & varName,
    size_t stationIndex,
    size_t timeIndex
)
```

Gets the values of an ensemble forecast for a variable, for a starting date in the main time dimension. 

**Parameters**: 

  * **varName** Name of the variable. 
  * **stationIndex** The catchment number. 
  * **timeIndex** Zero-based index of the time dimension.


**Template Parameters**: 

  * **ElementType** type of element expected for this variable. 


**Return**: null if it fails, else the forecasts. 

### function GetEnsemble

```cpp
template <typename ElementType >
inline vector< ElementType * > * GetEnsemble(
    const string & varName,
    size_t stationIndex
)
```


### function GetValues

```cpp
template <typename ElementType >
inline vector< ElementType > GetValues(
    const string & varName,
    size_t stationIndex
)
```

Gets the values of a variable stored as an non-ensemble series. 

**Parameters**: 

  * **varName** Name of the variable. 
  * **stationIndex** The catchment number.


**Template Parameters**: 

  * **ElementType** type of element expected for this variable. 


**Return**: All the values for the time series defined with this variable name. 

### function GetValues

```cpp
template <typename ElementType >
inline vector< ElementType > GetValues(
    const string & varName
)
```


### function GetSeries

```cpp
template <typename ElementType >
inline TTimeSeries< ElementType > * GetSeries(
    const string & varName,
    size_t stationIndex
)
```


### function GetSeries

```cpp
template <typename ElementType >
inline MultiTimeSeries< TTimeSeries< ElementType > * > * GetSeries(
    const string & varName
)
```


### function GetEnsembleSeries

```cpp
template <typename ElementType >
inline MultiTimeSeries< TTimeSeries< ElementType > * > * GetEnsembleSeries(
    const string & varName,
    size_t stationIndex
)
```


### function SetForecasts

```cpp
template <typename ElementType >
inline void SetForecasts(
    const string & varName,
    size_t stationIndex,
    size_t timeIndex,
    vector< ElementType * > & values
)
```

Sets the values for an ensemble forecast, for a variable, for a starting date in the main time dimension. 

**Parameters**: 

  * **varName** Name of the variable. 
  * **stationIndex** The catchment number. 
  * **timeIndex** Zero-based index of the time. 
  * **values** [in] the values to write to file. 


**Template Parameters**: 

  * **ElementType** type of element expected for this variable. 


### function SetEnsembles

```cpp
template <typename ElementType >
inline void SetEnsembles(
    const string & varName,
    size_t stationIndex,
    vector< ElementType * > & values
)
```


### function SetValues

```cpp
template <typename ElementType >
inline void SetValues(
    const string & varName,
    size_t stationIndex,
    const vector< ElementType > & values
)
```


### function SetValues

```cpp
template <typename ElementType >
inline void SetValues(
    const string & varName,
    const vector< ElementType > & values
)
```


### function GetVarDims

```cpp
vector< int > GetVarDims(
    int varNumDims
)
```


### function GetVarDims

```cpp
vector< int > GetVarDims(
    const string & varName
)
```


### function ReadVariableNames

```cpp
vector< string > ReadVariableNames(
    bool removeDimVars =true
)
```


### function ReadAttributeNames

```cpp
vector< string > ReadAttributeNames(
    const string & varName
)
```


### function ReadStringAttribute

```cpp
string ReadStringAttribute(
    int varId,
    const string & attName,
    bool throwIfNotFound =false,
    string defaultValue =""
)
```


### function ReadStringAttribute

```cpp
string ReadStringAttribute(
    const string & varName,
    const string & attName,
    bool throwIfNotFound =false,
    string defaultValue =""
)
```


### function ReadNumericAttribute

```cpp
double ReadNumericAttribute(
    int varId,
    const string & attName,
    bool throwIfNotFound =false,
    double defaultValue =0.0
)
```


### function ReadNumericAttribute

```cpp
double ReadNumericAttribute(
    const string & varName,
    const string & attName,
    bool throwIfNotFound =false,
    double defaultValue =0.0
)
```


### function ReadAttributes

```cpp
VariableAttributes ReadAttributes(
    const string & varName
)
```


### function ReadGlobalAttributes

```cpp
GlobalAttributes ReadGlobalAttributes()
```


### function GetTimeStep

```cpp
TimeStep GetTimeStep()
```


### function GetLeadTimeStep

```cpp
TimeStep GetLeadTimeStep()
```


### function GetLeadTimeGeometry

```cpp
std::pair< ptime, TimeStep > GetLeadTimeGeometry(
    const ptime & issueTime
)
```


### function GetLeadTimeDim

```cpp
vector< double > GetLeadTimeDim()
```


### function GetGlobalAttributes

```cpp
GlobalAttributes GetGlobalAttributes()
```


### function GetAttributes

```cpp
VariableAttributes GetAttributes(
    const string & varName
)
```


### function CheckCompliance

```cpp
static void CheckCompliance(
    const string & filename,
    int majorVersion,
    int minorVersion,
    vector< string > & warnings,
    vector< string > & errors
)
```


### function CreateTimeUnitsAttribute

```cpp
template <typename ElementType >
static inline string CreateTimeUnitsAttribute(
    const TTimeSeries< ElementType > & tSeries
)
```


### function CreateTimeVectors

```cpp
static std::pair< vector< double >, vector< double > > CreateTimeVectors(
    const ptime & start,
    const TimeStep & timeStep,
    size_t tsLength,
    const TimeStep & leadTimeStep,
    size_t leadTimeSize,
    int fcastOffset =1
)
```


### function CreateTimeVector

```cpp
static vector< double > CreateTimeVector(
    const ptime & start,
    const TimeStep & timeStep,
    const ptime & origin,
    const time_duration & timeStepAxis,
    const size_t length
)
```


### function CreateTimeVector

```cpp
static vector< double > CreateTimeVector(
    const ptime & start,
    const TimeStep & timeStep,
    const ptime & origin,
    const TimeStep & timeStepAxis,
    const size_t length
)
```


### function CreateTimeVector

```cpp
static vector< double > CreateTimeVector(
    const ptime & start,
    const TimeStep & timeStep,
    const size_t length
)
```


### function CreateTimeVector

```cpp
template <typename ElementType >
static inline vector< double > CreateTimeVector(
    const TTimeSeries< ElementType > & tSeries
)
```


### function CreateTimeVector

```cpp
template <typename ElementType >
static inline vector< double > CreateTimeVector(
    const TTimeSeries< ElementType > & tSeries,
    const ptime & origin,
    const TimeStep & timeStepAxis
)
```


### function StartCoordinate

```cpp
template <typename T >
static inline ptime StartCoordinate(
    const ptime & origin,
    const TimeStep & timeStep,
    const vector< T > & timeCoords
)
```


### function CreateTimeGeometry

```cpp
static std::pair< ptime, TimeStep > CreateTimeGeometry(
    const string & axisDefinition,
    const vector< double > & timeCoords
)
```


### function GetTimeStepName

```cpp
static string GetTimeStepName(
    const TimeStep & timeStep
)
```


### function CreateTimeUnitsAttribute

```cpp
static string CreateTimeUnitsAttribute(
    const ptime & utcStart,
    const string & units
)
```


### function CreateTimeUnitsAttribute

```cpp
static string CreateTimeUnitsAttribute(
    const ptime & utcStart,
    const TimeStep & timeStep
)
```


### function ParseStartDate

```cpp
static ptime ParseStartDate(
    const string & unitsAttribute
)
```


### function ParseTimeUnits

```cpp
static string ParseTimeUnits(
    const string & unitsAttribute
)
```


### function CreateLeadTimeUnitsAttribute

```cpp
static string CreateLeadTimeUnitsAttribute(
    const TimeStep & timeStep
)
```


### function Convert

```cpp
template <class TFrom ,
class TTo >
static inline vector< TTo > Convert(
    const vector< TFrom > & from,
    const std::function< TTo(const TFrom &)> & f
)
```


### function CreateTimeUnits

```cpp
static time_duration CreateTimeUnits(
    const TimeStep & timeStep
)
```


### function SetTimeOffsetIn

```cpp
static void SetTimeOffsetIn(
    const time_duration & td
)
```


### function SetTimeOffsetOut

```cpp
static void SetTimeOffsetOut(
    const time_duration & td
)
```


## Public Attributes Documentation

### variable TimeOffsetIn

```cpp
static time_duration TimeOffsetIn;
```


### variable TimeOffsetOut

```cpp
static time_duration TimeOffsetOut;
```


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000