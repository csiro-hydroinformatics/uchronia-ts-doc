---
title: datatypes::tests

---

# datatypes::tests



## Classes

|                | Name           |
| -------------- | -------------- |
| class | **[datatypes::tests::FileSystemHelper](/cpp/Classes/classdatatypes_1_1tests_1_1FileSystemHelper/)**  |
| class | **[datatypes::tests::TempFileCleaner](/cpp/Classes/classdatatypes_1_1tests_1_1TempFileCleaner/)**  |
| class | **[datatypes::tests::TestDataLocationHelper](/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/)**  |
| class | **[datatypes::tests::TestSingleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/)**  |
| class | **[datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/)** <br>A time series store for unit tests.  |
| class | **[datatypes::tests::TestEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1tests_1_1TestEnsembleTimeSeriesStore/)**  |
| class | **[datatypes::tests::TestTimeSeriesStoreFactory](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesStoreFactory/)**  |
| class | **[datatypes::tests::DataTestHelper](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/)**  |

## Functions

|                | Name           |
| -------------- | -------------- |
| template <typename T \> <br>bool | **[AreEqual](/cpp/Namespaces/namespacedatatypes_1_1tests/#function-areequal)**(const vector< T > & a, const vector< T > & b, bool strict =false, double tolerance =1e-12) |
| template <typename T \> <br>bool | **[AllEqual](/cpp/Namespaces/namespacedatatypes_1_1tests/#function-allequal)**(const vector< T > & values, T testValue) |
| template <typename T \> <br>bool | **[VectorEqual](/cpp/Namespaces/namespacedatatypes_1_1tests/#function-vectorequal)**(const vector< T > & a, const vector< T > & b) |


## Functions Documentation

### function AreEqual

```cpp
template <typename T >
bool AreEqual(
    const vector< T > & a,
    const vector< T > & b,
    bool strict =false,
    double tolerance =1e-12
)
```


### function AllEqual

```cpp
template <typename T >
bool AllEqual(
    const vector< T > & values,
    T testValue
)
```


### function VectorEqual

```cpp
template <typename T >
bool VectorEqual(
    const vector< T > & a,
    const vector< T > & b
)
```






-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000