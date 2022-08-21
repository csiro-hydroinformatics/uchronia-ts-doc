---
title: datatypes::tests

---

# datatypes::tests



## Classes

|                | Name           |
| -------------- | -------------- |
| class | **[datatypes::tests::FileSystemHelper](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1FileSystemHelper/)**  |
| class | **[datatypes::tests::TempFileCleaner](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TempFileCleaner/)**  |
| class | **[datatypes::tests::TestDataLocationHelper](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/)**  |
| class | **[datatypes::tests::TestSingleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/)**  |
| class | **[datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/)** <br>A time series store for unit tests.  |
| class | **[datatypes::tests::TestEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestEnsembleTimeSeriesStore/)**  |
| class | **[datatypes::tests::TestTimeSeriesStoreFactory](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesStoreFactory/)**  |
| class | **[datatypes::tests::DataTestHelper](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/)**  |

## Functions

|                | Name           |
| -------------- | -------------- |
| template <typename T \> <br>bool | **[AreEqual](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1tests/#function-areequal)**(const vector< T > & a, const vector< T > & b, bool strict =false, double tolerance =1e-12) |
| template <typename T \> <br>bool | **[AllEqual](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1tests/#function-allequal)**(const vector< T > & values, T testValue) |
| template <typename T \> <br>bool | **[VectorEqual](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1tests/#function-vectorequal)**(const vector< T > & a, const vector< T > & b) |


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

Updated on 2022-08-21 at 18:10:33 +1000