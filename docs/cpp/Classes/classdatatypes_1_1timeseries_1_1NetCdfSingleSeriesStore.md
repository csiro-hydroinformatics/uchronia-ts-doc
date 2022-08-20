---
title: datatypes::timeseries::NetCdfSingleSeriesStore

---

# datatypes::timeseries::NetCdfSingleSeriesStore



 [More...](#detailed-description)


`#include <time_series_io.hpp>`

Inherits from [datatypes::timeseries::SingleTimeSeriesStore< T >](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/), [datatypes::timeseries::SingleNetCdfFileStore< T >](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/), [datatypes::timeseries::IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/), [datatypes::timeseries::DataDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[NetCdfSingleSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-netcdfsingleseriesstore)**(const string & filename, const size_t nEns, const vector< double > & leadTimeVar, const string & timeUnits, const vector< double > & timeVar, const vector< string > & stationIds, const std::map< string, [VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) > & varDefinitions, const string & ncVarName, const string & identifier ="", const string & leadTimeUnits ="") |
| | **[NetCdfSingleSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-netcdfsingleseriesstore)**(const string & filename, const [DimensionsDefinitions](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) & dimDefinitions, const std::map< string, [VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) > & varDefinitions, const [GlobalAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) & globalAttributes, const string & ncVarName, const string & identifier ="") |
| | **[NetCdfSingleSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-netcdfsingleseriesstore)**(const string & fname) |
| | **[NetCdfSingleSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-netcdfsingleseriesstore)**(const string & fname, const string & ncVarName, const string & identifier ="") |
| [NetCdfSingleSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/) & | **[operator=](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-operator=)**([NetCdfSingleSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/) && src) |
| [NetCdfSingleSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/) & | **[operator=](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-operator=)**(const [NetCdfSingleSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/) & src) |
| | **[NetCdfSingleSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-netcdfsingleseriesstore)**([NetCdfSingleSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/) && src) |
| | **[NetCdfSingleSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-netcdfsingleseriesstore)**(const [NetCdfSingleSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/) & src) |
| virtual string | **[GetDataSummary](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-getdatasummary)**() const |
| virtual vector< [DataDimensionDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) > | **[GetDataDimensionsDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-getdatadimensionsdescription)**() const |
| virtual [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > * | **[Read](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-read)**() |
| virtual [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > * | **[Read](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-read)**(const string & identifier) |
| virtual [MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > * > * | **[ReadAllCollection](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-readallcollection)**() |
| void | **[Write](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-write)**([TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > * timeSeries) |
| vector< [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > * > | **[ReorderPerIdentifier](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-reorderperidentifier)**(const std::map< string, [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > * > & toSave) |
| vector< T > | **[Serialize](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-serialize)**(const vector< [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > * > & series) |
| void | **[WriteToIdentifiers](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-writetoidentifiers)**(const std::map< string, [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > * > & toSave) |
| void | **[WriteToNcVariables](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-writetoncvariables)**(const std::map< string, [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > * > & toSave) |
| virtual vector< string > | **[GetIdentifiers](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-getidentifiers)**() const |
| string | **[Dimensions](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-dimensions)**() |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::SingleTimeSeriesStore< T >](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~SingleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/#function-~singletimeseriesstore)**() |

**Public Functions inherited from [datatypes::timeseries::SingleNetCdfFileStore< T >](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~SingleNetCdfFileStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-~singlenetcdffilestore)**() |
| virtual void | **[Close](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-close)**() |
| bool | **[HasNcAccess](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-hasncaccess)**() |
| size_t | **[GetEnsembleSize](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getensemblesize)**() const |
| size_t | **[GetLeadTimeCount](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getleadtimecount)**() const |
| size_t | **[GetTimeLength](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-gettimelength)**() const |
| [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetTimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-gettimestep)**() const |
| ptime | **[TimeForIndex](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-timeforindex)**(size_t timeIndex) const |
| vector< ptime > | **[GetTimeDim](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-gettimedim)**() const |
| vector< double > | **[GetLeadTimeDim](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getleadtimedim)**() const |
| ptime | **[GetStart](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getstart)**() const |
| ptime | **[GetEnd](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getend)**() const |
| size_t | **[IndexForIdentifier](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-indexforidentifier)**(const string & identifier) const |
| [VariableAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/) | **[GetVarAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getvarattributes)**() |
| [GlobalAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) | **[GetGlobalAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getglobalattributes)**() |

**Protected Functions inherited from [datatypes::timeseries::SingleNetCdfFileStore< T >](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/)**

|                | Name           |
| -------------- | -------------- |
| | **[SingleNetCdfFileStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-singlenetcdffilestore)**() |
| | **[SingleNetCdfFileStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-singlenetcdffilestore)**(const string & fname, const size_t nEns, const vector< double > & leadTimeVar, const string & timeUnits, const vector< double > & timeVar, const vector< string > & stationIds, const std::map< string, [VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) > & varDefinitions, const [GlobalAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) & globalAttributes, const string & ncVarName ="", const string & identifier ="", const string & leadTimeUnits ="")<br>Constructor to create a new SWIFT netCDF file.  |
| | **[SingleNetCdfFileStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-singlenetcdffilestore)**(const string & fname, const [DimensionsDefinitions](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) & dimDefinitions, const std::map< string, [VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) > & varDefinitions, const [GlobalAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) & globalAttributes, const string & ncVarName ="", const string & identifier ="") |
| | **[SingleNetCdfFileStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-singlenetcdffilestore)**(const string & fname, const string & ncVarName ="", const string & identifier ="", bool writeMode =false) |
| void | **[Init](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-init)**(const string & filename, const [DimensionsDefinitions](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) & dimDefinitions, const std::map< string, [VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) > & varDefinitions, const [GlobalAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) & globalAttributes) |
| void | **[MoveFrom](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-movefrom)**([SingleNetCdfFileStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/) & src) |
| void | **[CopyFrom](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-copyfrom)**(const [SingleNetCdfFileStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/) & src) |
| string | **[GetNcVarName](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getncvarname)**(bool allowDiscovery =true) const |
| string | **[DataSummaryForIdentifier](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-datasummaryforidentifier)**() const |
| string | **[GetDefaultDataSummary](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getdefaultdatasummary)**() const |
| size_t | **[IndexForIdentifier](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-indexforidentifier)**(bool strict =true) const |
| virtual bool | **[HasIdentifier](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-hasidentifier)**() const |
| virtual string | **[GetIdentifier](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getidentifier)**(bool strict =true) const |
| void | **[SetIdentifier](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-setidentifier)**(string ident)<br>Sets the current station identifier.  |
| [SwiftNetCDFAccess](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/) * | **[GetNcAccess](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getncaccess)**() const |
| string & | **[GetFileName](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getfilename)**() |

**Public Functions inherited from [datatypes::timeseries::IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-~identifiersprovider)**() |
| vector< string > | **[SplitHierarchicalIdentifier](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-splithierarchicalidentifier)**(const string & longId) |
| string | **[GetTopmostIdentifier](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-gettopmostidentifier)**(const string & longId) |
| void | **[CheckNotEmpty](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-checknotempty)**(const string & longId) |


## Detailed Description

```cpp
template <typename T >
class datatypes::timeseries::NetCdfSingleSeriesStore;
```

## Public Functions Documentation

### function NetCdfSingleSeriesStore

```cpp
inline NetCdfSingleSeriesStore(
    const string & filename,
    const size_t nEns,
    const vector< double > & leadTimeVar,
    const string & timeUnits,
    const vector< double > & timeVar,
    const vector< string > & stationIds,
    const std::map< string, VariableDefinition > & varDefinitions,
    const string & ncVarName,
    const string & identifier ="",
    const string & leadTimeUnits =""
)
```


### function NetCdfSingleSeriesStore

```cpp
inline NetCdfSingleSeriesStore(
    const string & filename,
    const DimensionsDefinitions & dimDefinitions,
    const std::map< string, VariableDefinition > & varDefinitions,
    const GlobalAttributes & globalAttributes,
    const string & ncVarName,
    const string & identifier =""
)
```


### function NetCdfSingleSeriesStore

```cpp
inline NetCdfSingleSeriesStore(
    const string & fname
)
```


### function NetCdfSingleSeriesStore

```cpp
inline NetCdfSingleSeriesStore(
    const string & fname,
    const string & ncVarName,
    const string & identifier =""
)
```


### function operator=

```cpp
inline NetCdfSingleSeriesStore & operator=(
    NetCdfSingleSeriesStore && src
)
```


### function operator=

```cpp
inline NetCdfSingleSeriesStore & operator=(
    const NetCdfSingleSeriesStore & src
)
```


### function NetCdfSingleSeriesStore

```cpp
inline NetCdfSingleSeriesStore(
    NetCdfSingleSeriesStore && src
)
```


### function NetCdfSingleSeriesStore

```cpp
inline NetCdfSingleSeriesStore(
    const NetCdfSingleSeriesStore & src
)
```


### function GetDataSummary

```cpp
inline virtual string GetDataSummary() const
```


**Reimplements**: [datatypes::timeseries::DataDescriptor::GetDataSummary](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatasummary)


### function GetDataDimensionsDescription

```cpp
inline virtual vector< DataDimensionDescriptor > GetDataDimensionsDescription() const
```


**Reimplements**: [datatypes::timeseries::DataDescriptor::GetDataDimensionsDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatadimensionsdescription)


### function Read

```cpp
inline virtual TTimeSeries< T > * Read()
```


**Reimplements**: [datatypes::timeseries::SingleTimeSeriesStore::Read](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/#function-read)


### function Read

```cpp
inline virtual TTimeSeries< T > * Read(
    const string & identifier
)
```


**Reimplements**: [datatypes::timeseries::SingleTimeSeriesStore::Read](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/#function-read)


### function ReadAllCollection

```cpp
inline virtual MultiTimeSeries< TTimeSeries< T > * > * ReadAllCollection()
```


**Reimplements**: [datatypes::timeseries::SingleTimeSeriesStore::ReadAllCollection](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/#function-readallcollection)


### function Write

```cpp
inline void Write(
    TTimeSeries< T > * timeSeries
)
```


### function ReorderPerIdentifier

```cpp
inline vector< TTimeSeries< T > * > ReorderPerIdentifier(
    const std::map< string, TTimeSeries< T > * > & toSave
)
```


### function Serialize

```cpp
inline vector< T > Serialize(
    const vector< TTimeSeries< T > * > & series
)
```


### function WriteToIdentifiers

```cpp
inline void WriteToIdentifiers(
    const std::map< string, TTimeSeries< T > * > & toSave
)
```


### function WriteToNcVariables

```cpp
inline void WriteToNcVariables(
    const std::map< string, TTimeSeries< T > * > & toSave
)
```


### function GetIdentifiers

```cpp
inline virtual vector< string > GetIdentifiers() const
```


**Reimplements**: [datatypes::timeseries::SingleNetCdfFileStore::GetIdentifiers](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getidentifiers)


### function Dimensions

```cpp
static inline string Dimensions()
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000