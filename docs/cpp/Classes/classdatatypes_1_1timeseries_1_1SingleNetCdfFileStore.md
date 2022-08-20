---
title: datatypes::timeseries::SingleNetCdfFileStore

---

# datatypes::timeseries::SingleNetCdfFileStore



 [More...](#detailed-description)


`#include <time_series_io.hpp>`

Inherited by [datatypes::timeseries::NetCdfEnsembleTimeSeriesStore< T >](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfEnsembleTimeSeriesStore/), [datatypes::timeseries::NetCdfSingleSeriesStore< T >](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/)

## Public Functions

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

## Protected Functions

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
| virtual vector< string > | **[GetIdentifiers](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getidentifiers)**() const |
| [SwiftNetCDFAccess](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/) * | **[GetNcAccess](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getncaccess)**() const |
| string & | **[GetFileName](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getfilename)**() |

## Detailed Description

```cpp
template <typename T >
class datatypes::timeseries::SingleNetCdfFileStore;
```

## Public Functions Documentation

### function ~SingleNetCdfFileStore

```cpp
inline virtual ~SingleNetCdfFileStore()
```


### function Close

```cpp
inline virtual void Close()
```


### function HasNcAccess

```cpp
inline bool HasNcAccess()
```


### function GetEnsembleSize

```cpp
inline size_t GetEnsembleSize() const
```


### function GetLeadTimeCount

```cpp
inline size_t GetLeadTimeCount() const
```


### function GetTimeLength

```cpp
inline size_t GetTimeLength() const
```


### function GetTimeStep

```cpp
inline TimeStep GetTimeStep() const
```


### function TimeForIndex

```cpp
inline ptime TimeForIndex(
    size_t timeIndex
) const
```


### function GetTimeDim

```cpp
inline vector< ptime > GetTimeDim() const
```


### function GetLeadTimeDim

```cpp
inline vector< double > GetLeadTimeDim() const
```


### function GetStart

```cpp
inline ptime GetStart() const
```


### function GetEnd

```cpp
inline ptime GetEnd() const
```


### function IndexForIdentifier

```cpp
inline size_t IndexForIdentifier(
    const string & identifier
) const
```


### function GetVarAttributes

```cpp
inline VariableAttributes GetVarAttributes()
```


### function GetGlobalAttributes

```cpp
inline GlobalAttributes GetGlobalAttributes()
```


## Protected Functions Documentation

### function SingleNetCdfFileStore

```cpp
inline SingleNetCdfFileStore()
```


### function SingleNetCdfFileStore

```cpp
inline SingleNetCdfFileStore(
    const string & fname,
    const size_t nEns,
    const vector< double > & leadTimeVar,
    const string & timeUnits,
    const vector< double > & timeVar,
    const vector< string > & stationIds,
    const std::map< string, VariableDefinition > & varDefinitions,
    const GlobalAttributes & globalAttributes,
    const string & ncVarName ="",
    const string & identifier ="",
    const string & leadTimeUnits =""
)
```

Constructor to create a new SWIFT netCDF file. 

**Parameters**: 

  * **filename** name of the new file to create. 
  * **nEns** Size of the ensembles 
  * **nLead** Length of the lead time for each of the time series in the ensemble forecast for a given time. 
  * **timeUnits** Units of the temporal dimension(s). 
  * **timeVar** The values of the "main" time dimension, consistent with the temporal units given with the previous parameter 
  * **stationIds** List of identifiers for the stations. 
  * **leadTimeUnits** Units of the lead time dimension (if applicable) 


### function SingleNetCdfFileStore

```cpp
inline SingleNetCdfFileStore(
    const string & fname,
    const DimensionsDefinitions & dimDefinitions,
    const std::map< string, VariableDefinition > & varDefinitions,
    const GlobalAttributes & globalAttributes,
    const string & ncVarName ="",
    const string & identifier =""
)
```


### function SingleNetCdfFileStore

```cpp
inline SingleNetCdfFileStore(
    const string & fname,
    const string & ncVarName ="",
    const string & identifier ="",
    bool writeMode =false
)
```


### function Init

```cpp
inline void Init(
    const string & filename,
    const DimensionsDefinitions & dimDefinitions,
    const std::map< string, VariableDefinition > & varDefinitions,
    const GlobalAttributes & globalAttributes
)
```


### function MoveFrom

```cpp
inline void MoveFrom(
    SingleNetCdfFileStore & src
)
```


### function CopyFrom

```cpp
inline void CopyFrom(
    const SingleNetCdfFileStore & src
)
```


### function GetNcVarName

```cpp
inline string GetNcVarName(
    bool allowDiscovery =true
) const
```


### function DataSummaryForIdentifier

```cpp
inline string DataSummaryForIdentifier() const
```


### function GetDefaultDataSummary

```cpp
inline string GetDefaultDataSummary() const
```


### function IndexForIdentifier

```cpp
inline size_t IndexForIdentifier(
    bool strict =true
) const
```


### function HasIdentifier

```cpp
inline virtual bool HasIdentifier() const
```


### function GetIdentifier

```cpp
inline virtual string GetIdentifier(
    bool strict =true
) const
```


### function SetIdentifier

```cpp
inline void SetIdentifier(
    string ident
)
```

Sets the current station identifier. 

**Parameters**: 

  * **ident** String identifier to set as the identifier the NetCDF store is to operate on. 


### function GetIdentifiers

```cpp
inline virtual vector< string > GetIdentifiers() const
```


**Reimplemented by**: [datatypes::timeseries::NetCdfSingleSeriesStore::GetIdentifiers](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-getidentifiers), [datatypes::timeseries::NetCdfEnsembleTimeSeriesStore::GetIdentifiers](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfEnsembleTimeSeriesStore/#function-getidentifiers), [datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore::GetIdentifiers](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-getidentifiers)


### function GetNcAccess

```cpp
inline SwiftNetCDFAccess * GetNcAccess() const
```


### function GetFileName

```cpp
inline string & GetFileName()
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000