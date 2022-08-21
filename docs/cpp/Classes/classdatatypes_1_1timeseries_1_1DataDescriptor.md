---
title: datatypes::timeseries::DataDescriptor
summary: Minimalist descriptor for a multidimensional time series. 

---

# datatypes::timeseries::DataDescriptor



Minimalist descriptor for a multidimensional time series. 


`#include <time_series_store.hpp>`

Inherited by [datatypes::timeseries::EnsembleTimeSeriesStore< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/), [datatypes::timeseries::SingleTimeSeriesStore< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/), [datatypes::timeseries::EnsembleTimeSeriesStore< T >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/), [datatypes::timeseries::SingleTimeSeriesStore< T >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/), [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore< T >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual string | **[GetDataSummary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatasummary)**() const =0 |
| virtual vector< [DataDimensionDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) > | **[GetDataDimensionsDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatadimensionsdescription)**() const =0 |

## Public Functions Documentation

### function GetDataSummary

```cpp
virtual string GetDataSummary() const =0
```


**Reimplemented by**: [datatypes::tests::TestSingleTimeSeriesStore::GetDataSummary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/#function-getdatasummary), [datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::GetDataSummary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getdatasummary), [datatypes::tests::TestEnsembleTimeSeriesStore::GetDataSummary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestEnsembleTimeSeriesStore/#function-getdatasummary), [datatypes::timeseries::NetCdfSingleSeriesStore::GetDataSummary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-getdatasummary), [datatypes::timeseries::NetCdfEnsembleTimeSeriesStore::GetDataSummary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfEnsembleTimeSeriesStore/#function-getdatasummary), [datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore::GetDataSummary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-getdatasummary), [datatypes::timeseries::MultiFileTimeSeriesEnsembleTimeSeriesStore::GetDataSummary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-getdatasummary), [datatypes::timeseries::MultiFileTimeSeriesEnsembleTimeSeriesStore::GetDataSummary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-getdatasummary)


### function GetDataDimensionsDescription

```cpp
virtual vector< DataDimensionDescriptor > GetDataDimensionsDescription() const =0
```


**Reimplemented by**: [datatypes::tests::TestSingleTimeSeriesStore::GetDataDimensionsDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/#function-getdatadimensionsdescription), [datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::GetDataDimensionsDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getdatadimensionsdescription), [datatypes::tests::TestEnsembleTimeSeriesStore::GetDataDimensionsDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestEnsembleTimeSeriesStore/#function-getdatadimensionsdescription), [datatypes::timeseries::NetCdfSingleSeriesStore::GetDataDimensionsDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-getdatadimensionsdescription), [datatypes::timeseries::NetCdfEnsembleTimeSeriesStore::GetDataDimensionsDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfEnsembleTimeSeriesStore/#function-getdatadimensionsdescription), [datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore::GetDataDimensionsDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-getdatadimensionsdescription), [datatypes::timeseries::MultiFileTimeSeriesEnsembleTimeSeriesStore::GetDataDimensionsDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-getdatadimensionsdescription), [datatypes::timeseries::MultiFileTimeSeriesEnsembleTimeSeriesStore::GetDataDimensionsDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-getdatadimensionsdescription)


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000