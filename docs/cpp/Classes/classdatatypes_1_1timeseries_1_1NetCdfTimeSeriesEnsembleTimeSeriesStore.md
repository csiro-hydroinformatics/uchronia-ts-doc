---
title: datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore

---

# datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore



 [More...](#detailed-description)


`#include <time_series_io.hpp>`

Inherits from [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/), [datatypes::timeseries::SingleNetCdfFileStore< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/), [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore< T >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/), [datatypes::timeseries::IdentifiersProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/), [datatypes::timeseries::TimeSeriesInfoProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/), [datatypes::timeseries::DataDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/)

## Public Types

|                | Name           |
| -------------- | -------------- |
| using typename [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[SeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#using-seriestype) | **[SeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#using-seriestype)**  |
| using typename [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[PtrSeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#using-ptrseriestype) | **[PtrSeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#using-ptrseriestype)**  |
| using typename [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[EnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#using-ensembleptrtype) | **[EnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#using-ensembleptrtype)**  |
| using typename [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) | **[PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype)**  |
| using typename [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[TSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#using-tseriesensembleptrtype) | **[TSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#using-tseriesensembleptrtype)**  |
| using typename [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)< T >::[PtrTSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#using-ptrtseriesensembleptrtype) | **[PtrTSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#using-ptrtseriesensembleptrtype)**  |
| using typename EnsemblePtrType::ElementType | **[ElementType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#using-elementtype)**  |

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[NetCdfTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-netcdftimeseriesensembletimeseriesstore)**(const string & filename, const size_t nEns, const vector< double > & leadTimeVar, const string & timeUnits, const vector< double > & timeVar, const vector< string > & stationIds, const std::map< string, [VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) > & varDefinitions, const [GlobalAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) & globalAttributes, const string & ncVarName, const string & identifier ="") |
| | **[NetCdfTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-netcdftimeseriesensembletimeseriesstore)**(const string & filename, const [DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) & dimDefinitions, const std::map< string, [VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) > & varDefinitions, const [GlobalAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) & globalAttributes, const string & ncVarName, const string & identifier ="") |
| | **[NetCdfTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-netcdftimeseriesensembletimeseriesstore)**(const string & fname, const string & ncVarName, const string & varIdentifier, bool writeMode =false) |
| virtual [EnsembleForecastTimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#using-ensembleforecasttimeseries)< [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > > * | **[GetSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-getseries)**(const string & dataId) |
| virtual vector< string > | **[GetIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-getidentifiers)**() const |
| void | **[SetIdentifier](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-setidentifier)**(string ident)<br>Sets the current station identifier.  |
| [PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) | **[GetForecasts](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-getforecasts)**(size_t i)<br>Gets the ensemble forecast for a given index in the time dimension.  |
| void | **[SetForecasts](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-setforecasts)**(size_t i, [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [TimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) * > * forecasts) |
| virtual | **[~NetCdfTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-~netcdftimeseriesensembletimeseriesstore)**() |
| virtual [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)< [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)< T > * > * | **[Read](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-read)**(const string & ensembleIdentifier) override |
| size_t | **[GetIndexForTime](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-getindexfortime)**(const ptime & dateIndex) |
| ptime | **[GetTimeForIndex](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-gettimeforindex)**(size_t index) |
| virtual size_t | **[GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-getlength)**() const |
| virtual [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-gettimestep)**() const |
| [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) | **[GetLeadTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-getleadtimestep)**() const |
| virtual ptime | **[GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-getstart)**() const |
| ptime | **[GetEnd](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-getend)**() const |
| virtual string | **[GetDataSummary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-getdatasummary)**() const |
| virtual vector< [DataDimensionDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) > | **[GetDataDimensionsDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-getdatadimensionsdescription)**() const |
| virtual void | **[Allocate](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-allocate)**(size_t length, [PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) value) |
| virtual void | **[AllocateValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-allocatevalues)**(const vector< [PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) > & values) |
| virtual void | **[SetSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-setseries)**(const string & dataId, [PtrTSeriesEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#using-ptrtseriesensembleptrtype) value) |
| virtual void | **[SetItem](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-setitem)**(const string & dataId, size_t index, [PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) value) |
| virtual void | **[SetItem](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-setitem)**(const string & dataId, size_t index, const [EnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#using-ensembleptrtype) & value) |
| virtual void | **[SetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-setlength)**(size_t length) |
| virtual void | **[SetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-setstart)**(ptime start) |
| virtual void | **[SetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-settimestep)**(const [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/) & ) |
| virtual bool | **[IsActive](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-isactive)**() |
| string | **[Dimensions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-dimensions)**() |

## Additional inherited members

**Public Functions inherited from [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~WritableTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-~writabletimeseriesensembletimeseriesstore)**() |

**Public Functions inherited from [datatypes::timeseries::SingleNetCdfFileStore< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~SingleNetCdfFileStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-~singlenetcdffilestore)**() |
| virtual void | **[Close](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-close)**() |
| bool | **[HasNcAccess](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-hasncaccess)**() |
| size_t | **[GetEnsembleSize](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getensemblesize)**() const |
| size_t | **[GetLeadTimeCount](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getleadtimecount)**() const |
| size_t | **[GetTimeLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-gettimelength)**() const |
| ptime | **[TimeForIndex](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-timeforindex)**(size_t timeIndex) const |
| vector< ptime > | **[GetTimeDim](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-gettimedim)**() const |
| vector< double > | **[GetLeadTimeDim](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getleadtimedim)**() const |
| size_t | **[IndexForIdentifier](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-indexforidentifier)**(const string & identifier) const |
| [VariableAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/) | **[GetVarAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getvarattributes)**() |
| [GlobalAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) | **[GetGlobalAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getglobalattributes)**() |

**Protected Functions inherited from [datatypes::timeseries::SingleNetCdfFileStore< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/)**

|                | Name           |
| -------------- | -------------- |
| | **[SingleNetCdfFileStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-singlenetcdffilestore)**() |
| | **[SingleNetCdfFileStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-singlenetcdffilestore)**(const string & fname, const size_t nEns, const vector< double > & leadTimeVar, const string & timeUnits, const vector< double > & timeVar, const vector< string > & stationIds, const std::map< string, [VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) > & varDefinitions, const [GlobalAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) & globalAttributes, const string & ncVarName ="", const string & identifier ="", const string & leadTimeUnits ="")<br>Constructor to create a new SWIFT netCDF file.  |
| | **[SingleNetCdfFileStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-singlenetcdffilestore)**(const string & fname, const [DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) & dimDefinitions, const std::map< string, [VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) > & varDefinitions, const [GlobalAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) & globalAttributes, const string & ncVarName ="", const string & identifier ="") |
| | **[SingleNetCdfFileStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-singlenetcdffilestore)**(const string & fname, const string & ncVarName ="", const string & identifier ="", bool writeMode =false) |
| void | **[Init](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-init)**(const string & filename, const [DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/) & dimDefinitions, const std::map< string, [VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/) > & varDefinitions, const [GlobalAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/) & globalAttributes) |
| void | **[MoveFrom](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-movefrom)**([SingleNetCdfFileStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/) & src) |
| void | **[CopyFrom](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-copyfrom)**(const [SingleNetCdfFileStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/) & src) |
| string | **[GetNcVarName](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getncvarname)**(bool allowDiscovery =true) const |
| string | **[DataSummaryForIdentifier](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-datasummaryforidentifier)**() const |
| string | **[GetDefaultDataSummary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getdefaultdatasummary)**() const |
| size_t | **[IndexForIdentifier](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-indexforidentifier)**(bool strict =true) const |
| virtual bool | **[HasIdentifier](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-hasidentifier)**() const |
| virtual string | **[GetIdentifier](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getidentifier)**(bool strict =true) const |
| [SwiftNetCDFAccess](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/) * | **[GetNcAccess](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getncaccess)**() const |
| string & | **[GetFileName](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getfilename)**() |

**Public Functions inherited from [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore< T >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-~timeseriesensembletimeseriesstore)**() |
| virtual [PtrEnsemblePtrType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrensembleptrtype) | **[GetItem](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getitem)**(const string & dataId, size_t fcastIndex) |
| virtual [PtrSeriesType](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#using-ptrseriestype) | **[GetItem](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getitem)**(const string & dataId, size_t fcastIndex, size_t ensIndex) |
| virtual size_t | **[GetEnsembleSize](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getensemblesize)**(const string & dataId, size_t fcastIndex) const |

**Public Functions inherited from [datatypes::timeseries::IdentifiersProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~IdentifiersProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-~identifiersprovider)**() |
| vector< string > | **[SplitHierarchicalIdentifier](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-splithierarchicalidentifier)**(const string & longId) |
| string | **[GetTopmostIdentifier](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-gettopmostidentifier)**(const string & longId) |
| void | **[CheckNotEmpty](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/#function-checknotempty)**(const string & longId) |

**Public Functions inherited from [datatypes::timeseries::TimeSeriesInfoProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~TimeSeriesInfoProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/#function-~timeseriesinfoprovider)**() |


## Detailed Description

```cpp
template <typename T  =double>
class datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore;
```

## Public Types Documentation

### using SeriesType

```cpp
using datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore< T >::SeriesType =  typename CommonTypes<T>::SeriesType;
```


### using PtrSeriesType

```cpp
using datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore< T >::PtrSeriesType =  typename CommonTypes<T>::PtrSeriesType;
```


### using EnsemblePtrType

```cpp
using datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore< T >::EnsemblePtrType =  typename CommonTypes<T>::EnsemblePtrType;
```


### using PtrEnsemblePtrType

```cpp
using datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore< T >::PtrEnsemblePtrType =  typename CommonTypes<T>::PtrEnsemblePtrType;
```


### using TSeriesEnsemblePtrType

```cpp
using datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore< T >::TSeriesEnsemblePtrType =  typename CommonTypes<T>::TSeriesEnsemblePtrType;
```


### using PtrTSeriesEnsemblePtrType

```cpp
using datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore< T >::PtrTSeriesEnsemblePtrType =  typename CommonTypes<T>::PtrTSeriesEnsemblePtrType;
```


### using ElementType

```cpp
using datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore< T >::ElementType =  typename EnsemblePtrType::ElementType;
```


## Public Functions Documentation

### function NetCdfTimeSeriesEnsembleTimeSeriesStore

```cpp
inline NetCdfTimeSeriesEnsembleTimeSeriesStore(
    const string & filename,
    const size_t nEns,
    const vector< double > & leadTimeVar,
    const string & timeUnits,
    const vector< double > & timeVar,
    const vector< string > & stationIds,
    const std::map< string, VariableDefinition > & varDefinitions,
    const GlobalAttributes & globalAttributes,
    const string & ncVarName,
    const string & identifier =""
)
```


### function NetCdfTimeSeriesEnsembleTimeSeriesStore

```cpp
inline NetCdfTimeSeriesEnsembleTimeSeriesStore(
    const string & filename,
    const DimensionsDefinitions & dimDefinitions,
    const std::map< string, VariableDefinition > & varDefinitions,
    const GlobalAttributes & globalAttributes,
    const string & ncVarName,
    const string & identifier =""
)
```


### function NetCdfTimeSeriesEnsembleTimeSeriesStore

```cpp
inline NetCdfTimeSeriesEnsembleTimeSeriesStore(
    const string & fname,
    const string & ncVarName,
    const string & varIdentifier,
    bool writeMode =false
)
```


### function GetSeries

```cpp
inline virtual EnsembleForecastTimeSeries< TTimeSeries< T > > * GetSeries(
    const string & dataId
)
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getseries)


### function GetIdentifiers

```cpp
inline virtual vector< string > GetIdentifiers() const
```


**Reimplements**: [datatypes::timeseries::SingleNetCdfFileStore::GetIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/#function-getidentifiers)


### function SetIdentifier

```cpp
inline void SetIdentifier(
    string ident
)
```

Sets the current station identifier. 

**Parameters**: 

  * **ident** String identifier to set as the identifier the NetCDF store is to operate on. 


### function GetForecasts

```cpp
inline PtrEnsemblePtrType GetForecasts(
    size_t i
)
```

Gets the ensemble forecast for a given index in the time dimension. 

**Parameters**: 

  * **i** Zero-based index of the time step of interest.


**Return**: a pointer to a new [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/). 

### function SetForecasts

```cpp
inline void SetForecasts(
    size_t i,
    MultiTimeSeries< TimeSeries * > * forecasts
)
```


### function ~NetCdfTimeSeriesEnsembleTimeSeriesStore

```cpp
inline virtual ~NetCdfTimeSeriesEnsembleTimeSeriesStore()
```


### function Read

```cpp
inline virtual MultiTimeSeries< TTimeSeries< T > * > * Read(
    const string & ensembleIdentifier
) override
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::Read](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-read)


### function GetIndexForTime

```cpp
inline size_t GetIndexForTime(
    const ptime & dateIndex
)
```


### function GetTimeForIndex

```cpp
inline ptime GetTimeForIndex(
    size_t index
)
```


### function GetLength

```cpp
inline virtual size_t GetLength() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getlength)


### function GetTimeStep

```cpp
inline virtual TimeStep GetTimeStep() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-gettimestep)


### function GetLeadTimeStep

```cpp
inline TimeStep GetLeadTimeStep() const
```


### function GetStart

```cpp
inline virtual ptime GetStart() const
```


**Reimplements**: [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore::GetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/#function-getstart)


### function GetEnd

```cpp
inline ptime GetEnd() const
```


### function GetDataSummary

```cpp
inline virtual string GetDataSummary() const
```


**Reimplements**: [datatypes::timeseries::DataDescriptor::GetDataSummary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatasummary)


### function GetDataDimensionsDescription

```cpp
inline virtual vector< DataDimensionDescriptor > GetDataDimensionsDescription() const
```


**Reimplements**: [datatypes::timeseries::DataDescriptor::GetDataDimensionsDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatadimensionsdescription)


### function Allocate

```cpp
inline virtual void Allocate(
    size_t length,
    PtrEnsemblePtrType value
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::Allocate](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-allocate)


### function AllocateValues

```cpp
inline virtual void AllocateValues(
    const vector< PtrEnsemblePtrType > & values
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::AllocateValues](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-allocatevalues)


### function SetSeries

```cpp
inline virtual void SetSeries(
    const string & dataId,
    PtrTSeriesEnsemblePtrType value
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::SetSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-setseries)


### function SetItem

```cpp
inline virtual void SetItem(
    const string & dataId,
    size_t index,
    PtrEnsemblePtrType value
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::SetItem](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-setitem)


### function SetItem

```cpp
inline virtual void SetItem(
    const string & dataId,
    size_t index,
    const EnsemblePtrType & value
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::SetItem](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-setitem)


### function SetLength

```cpp
inline virtual void SetLength(
    size_t length
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::SetLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-setlength)


### function SetStart

```cpp
inline virtual void SetStart(
    ptime start
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::SetStart](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-setstart)


### function SetTimeStep

```cpp
inline virtual void SetTimeStep(
    const TimeStep & 
)
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::SetTimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-settimestep)


### function IsActive

```cpp
inline virtual bool IsActive()
```


**Reimplements**: [datatypes::timeseries::WritableTimeSeriesEnsembleTimeSeriesStore::IsActive](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/#function-isactive)


### function Dimensions

```cpp
static inline string Dimensions()
```


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000