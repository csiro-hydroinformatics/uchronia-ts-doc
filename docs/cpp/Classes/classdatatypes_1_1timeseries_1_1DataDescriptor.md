---
title: datatypes::timeseries::DataDescriptor

---

# datatypes::timeseries::DataDescriptor






`#include <time_series_store.hpp>`

Inherited by [datatypes::timeseries::EnsembleTimeSeriesStore< double >](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/), [datatypes::timeseries::SingleTimeSeriesStore< double >](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/), [datatypes::timeseries::EnsembleTimeSeriesStore< T >](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/), [datatypes::timeseries::SingleTimeSeriesStore< T >](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/), [datatypes::timeseries::TimeSeriesEnsembleTimeSeriesStore< T >](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual string | **[GetDataSummary](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatasummary)**() const =0 |
| virtual vector< [DataDimensionDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/) > | **[GetDataDimensionsDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/#function-getdatadimensionsdescription)**() const =0 |

## Public Functions Documentation

### function GetDataSummary

```cpp
virtual string GetDataSummary() const =0
```


**Reimplemented by**: [datatypes::tests::TestSingleTimeSeriesStore::GetDataSummary](/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/#function-getdatasummary), [datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::GetDataSummary](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getdatasummary), [datatypes::tests::TestEnsembleTimeSeriesStore::GetDataSummary](/cpp/Classes/classdatatypes_1_1tests_1_1TestEnsembleTimeSeriesStore/#function-getdatasummary), [datatypes::timeseries::NetCdfSingleSeriesStore::GetDataSummary](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-getdatasummary), [datatypes::timeseries::NetCdfEnsembleTimeSeriesStore::GetDataSummary](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfEnsembleTimeSeriesStore/#function-getdatasummary), [datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore::GetDataSummary](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-getdatasummary), [datatypes::timeseries::MultiFileTimeSeriesEnsembleTimeSeriesStore::GetDataSummary](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-getdatasummary), [datatypes::timeseries::MultiFileTimeSeriesEnsembleTimeSeriesStore::GetDataSummary](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-getdatasummary)


### function GetDataDimensionsDescription

```cpp
virtual vector< DataDimensionDescriptor > GetDataDimensionsDescription() const =0
```


**Reimplemented by**: [datatypes::tests::TestSingleTimeSeriesStore::GetDataDimensionsDescription](/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/#function-getdatadimensionsdescription), [datatypes::tests::TestTimeSeriesEnsembleTimeSeriesStore::GetDataDimensionsDescription](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/#function-getdatadimensionsdescription), [datatypes::tests::TestEnsembleTimeSeriesStore::GetDataDimensionsDescription](/cpp/Classes/classdatatypes_1_1tests_1_1TestEnsembleTimeSeriesStore/#function-getdatadimensionsdescription), [datatypes::timeseries::NetCdfSingleSeriesStore::GetDataDimensionsDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/#function-getdatadimensionsdescription), [datatypes::timeseries::NetCdfEnsembleTimeSeriesStore::GetDataDimensionsDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfEnsembleTimeSeriesStore/#function-getdatadimensionsdescription), [datatypes::timeseries::NetCdfTimeSeriesEnsembleTimeSeriesStore::GetDataDimensionsDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/#function-getdatadimensionsdescription), [datatypes::timeseries::MultiFileTimeSeriesEnsembleTimeSeriesStore::GetDataDimensionsDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-getdatadimensionsdescription), [datatypes::timeseries::MultiFileTimeSeriesEnsembleTimeSeriesStore::GetDataDimensionsDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/#function-getdatadimensionsdescription)


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000