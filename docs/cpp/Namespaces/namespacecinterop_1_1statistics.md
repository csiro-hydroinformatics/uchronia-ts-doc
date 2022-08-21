---
title: cinterop::statistics

---

# cinterop::statistics



## Functions

|                | Name           |
| -------------- | -------------- |
| statistic_definition * | **[to_statistic_definition_ptr< TimeSeries >](/uchronia-ts-doc/cpp/Namespaces/namespacecinterop_1_1statistics/#function-to-statistic-definition-ptr<-timeseries->)**(const std::string & model_variable_id, const std::string & statistic_identifier, const std::string & objective_identifier, const std::string & objective_name, const date_time_to_second & start, const date_time_to_second & end, const [TimeSeries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/#typedef-timeseries) & time_series_data)<br>Template specialisation for cinterop::statistics::to_statistic_definition_ptr.  |


## Functions Documentation

### function to_statistic_definition_ptr< TimeSeries >

```cpp
inline statistic_definition * to_statistic_definition_ptr< TimeSeries >(
    const std::string & model_variable_id,
    const std::string & statistic_identifier,
    const std::string & objective_identifier,
    const std::string & objective_name,
    const date_time_to_second & start,
    const date_time_to_second & end,
    const TimeSeries & time_series_data
)
```

Template specialisation for cinterop::statistics::to_statistic_definition_ptr. 





-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000