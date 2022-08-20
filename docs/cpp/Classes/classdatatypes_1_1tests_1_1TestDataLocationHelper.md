---
title: datatypes::tests::TestDataLocationHelper

---

# datatypes::tests::TestDataLocationHelper






`#include <datatypes_test_helpers.h>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| string | **[ReadEnvironmentVariable](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#function-readenvironmentvariable)**(const string & envVar) |
| string | **[BuildPath](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#function-buildpath)**(const vector< string > & folders) |
| [TimeSeriesLibrary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/) | **[CreateEnsembleTimeSeriesLibrary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#function-createensembletimeserieslibrary)**(string & rainObsId, string & petObsId, string & rainFcastId, string & petFcastId) |
| [TimeSeriesLibrary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/) | **[GetTestTimeSeriesLibrary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#function-gettesttimeserieslibrary)**() |
| vector< string > | **[TestTsLibraryIdentifiers](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#function-testtslibraryidentifiers)**() |
| [TimeSeriesLibrary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/) * | **[CreateTestTimeSeriesLibrary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#function-createtesttimeserieslibrary)**() |
| void | **[MakeTestTimeSeriesLibrary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#function-maketesttimeserieslibrary)**([TimeSeriesLibrary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/) & dataLibrary) |
| vector< string > | **[TestStationIds](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#function-teststationids)**() |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| const string | **[kVarSingleStation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-kvarsinglestation)**  |
| const string | **[kVarMultiStations](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-kvarmultistations)**  |
| const string | **[kFileSingleStation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-kfilesinglestation)**  |
| const string | **[kFileMultiStations](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-kfilemultistations)**  |
| const string | **[kFileAllDataCases](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-kfilealldatacases)**  |
| const string | **[kVar1FcastEns](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-kvar1fcastens)**  |
| const string | **[kVar2FcastEns](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-kvar2fcastens)**  |
| const string | **[kVar1Obs](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-kvar1obs)**  |
| const string | **[kVar2Obs](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-kvar2obs)**  |
| const string | **[kVar1Ens](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-kvar1ens)**  |
| const string | **[kVar2Ens](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-kvar2ens)**  |
| const string | **[kIdentifier1FcastEns](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-kidentifier1fcastens)**  |
| const string | **[kIdentifier2FcastEns](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-kidentifier2fcastens)**  |
| const string | **[kIdentifier1Obs](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-kidentifier1obs)**  |
| const string | **[kIdentifier2Obs](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-kidentifier2obs)**  |
| const string | **[kIdentifier1Ens](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-kidentifier1ens)**  |
| const string | **[kIdentifier2Ens](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-kidentifier2ens)**  |
| const string | **[kSingleStationId](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-ksinglestationid)**  |
| const string | **[kStationIdOne](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-kstationidone)**  |
| const string | **[kStationIdTwo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-kstationidtwo)**  |
| const size_t | **[kTimeSeriesLength](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/#variable-ktimeserieslength)**  |

## Public Functions Documentation

### function ReadEnvironmentVariable

```cpp
static string ReadEnvironmentVariable(
    const string & envVar
)
```


### function BuildPath

```cpp
static string BuildPath(
    const vector< string > & folders
)
```


### function CreateEnsembleTimeSeriesLibrary

```cpp
static TimeSeriesLibrary CreateEnsembleTimeSeriesLibrary(
    string & rainObsId,
    string & petObsId,
    string & rainFcastId,
    string & petFcastId
)
```


### function GetTestTimeSeriesLibrary

```cpp
static TimeSeriesLibrary GetTestTimeSeriesLibrary()
```


### function TestTsLibraryIdentifiers

```cpp
static vector< string > TestTsLibraryIdentifiers()
```


### function CreateTestTimeSeriesLibrary

```cpp
static TimeSeriesLibrary * CreateTestTimeSeriesLibrary()
```


### function MakeTestTimeSeriesLibrary

```cpp
static void MakeTestTimeSeriesLibrary(
    TimeSeriesLibrary & dataLibrary
)
```


### function TestStationIds

```cpp
static vector< string > TestStationIds()
```


## Public Attributes Documentation

### variable kVarSingleStation

```cpp
static const string kVarSingleStation;
```


### variable kVarMultiStations

```cpp
static const string kVarMultiStations;
```


### variable kFileSingleStation

```cpp
static const string kFileSingleStation;
```


### variable kFileMultiStations

```cpp
static const string kFileMultiStations;
```


### variable kFileAllDataCases

```cpp
static const string kFileAllDataCases;
```


### variable kVar1FcastEns

```cpp
static const string kVar1FcastEns;
```


### variable kVar2FcastEns

```cpp
static const string kVar2FcastEns;
```


### variable kVar1Obs

```cpp
static const string kVar1Obs;
```


### variable kVar2Obs

```cpp
static const string kVar2Obs;
```


### variable kVar1Ens

```cpp
static const string kVar1Ens;
```


### variable kVar2Ens

```cpp
static const string kVar2Ens;
```


### variable kIdentifier1FcastEns

```cpp
static const string kIdentifier1FcastEns;
```


### variable kIdentifier2FcastEns

```cpp
static const string kIdentifier2FcastEns;
```


### variable kIdentifier1Obs

```cpp
static const string kIdentifier1Obs;
```


### variable kIdentifier2Obs

```cpp
static const string kIdentifier2Obs;
```


### variable kIdentifier1Ens

```cpp
static const string kIdentifier1Ens;
```


### variable kIdentifier2Ens

```cpp
static const string kIdentifier2Ens;
```


### variable kSingleStationId

```cpp
static const string kSingleStationId;
```


### variable kStationIdOne

```cpp
static const string kStationIdOne;
```


### variable kStationIdTwo

```cpp
static const string kStationIdTwo;
```


### variable kTimeSeriesLength

```cpp
static const size_t kTimeSeriesLength;
```


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000