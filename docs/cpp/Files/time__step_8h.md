---
title: datatypes/time_step.h

---

# datatypes/time_step.h



## Namespaces

| Name           |
| -------------- |
| **[datatypes](/cpp/Namespaces/namespacedatatypes/)**  |
| **[datatypes::timeseries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/)**  |

## Classes

|                | Name           |
| -------------- | -------------- |
| class | **[datatypes::timeseries::TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/)** <br>Time step handling for time series.  |
| class | **[datatypes::timeseries::TimeSeriesInfoProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/)** <br>An interface definition for classes that can provide essential time series temporal characteristics.  |

## Types

|                | Name           |
| -------------- | -------------- |
| using boost::posix_time::time_duration::sec_type | **[sec_type](/cpp/Files/time__step_8h/#using-sec-type)**  |

## Types Documentation

### using sec_type

```cpp
using sec_type =  boost::posix_time::time_duration::sec_type;
```





## Source code

```cpp
#pragma once

#include "boost/date_time/posix_time/posix_time.hpp"
#include "datatypes/common.h"
#include "datatypes/exception_utilities.h"
#include "datatypes/time_step_implementation.h"

using namespace boost::posix_time;
using sec_type = boost::posix_time::time_duration::sec_type;

namespace datatypes
{
    namespace timeseries
    {
        class DATATYPES_DLL_LIB TimeStep
        {
        public:

            TimeStep(const time_duration& stepDuration);
            TimeStep(TimeStepImplementation* tsi);

            TimeStep(const TimeStep& src);
            TimeStep();
            ~TimeStep();

            TimeStep& operator=(const TimeStep &rhs);

            TimeStep& operator=(const time_duration& stepDuration);

            TimeStep& operator=(const string& stepDuration);

            bool operator==(const TimeStep &rhs) const;

            bool operator!=(const TimeStep &rhs) const;

            TimeStep operator*(int mult) const;

            TimeStep operator*(double mult) const;

            int operator/(const TimeStep& divisor) const;

            TimeStep operator/(int divisor) const;

            time_duration operator%(const TimeStep& other) const;

            bool IsRegular() const;

            time_duration GetRegularStepDuration() const;

            //const ptime AddSteps(const ptime& startTimeStep, sec_type n) const;

            const ptime AddSteps(const ptime& startTimeStep, size_t n) const;

            const ptime AddSteps(const ptime& startTimeStep, int n) const;

            const ptime AddSteps(const ptime& startTimeStep, double mult) const;

            vector<ptime> AddSteps(const ptime& startTimeStep, const vector<double> timeSteps) const;

            vector<ptime> AddSteps(const vector<ptime>& times, double mult) const;

            const time_duration GetTimeStepDuration(const ptime& startTimeStep) const;

            const ptrdiff_t GetUpperNumSteps(const ptime& start, const ptime& end) const;

            const ptrdiff_t GetNumSteps(const ptime& start, const ptime& end) const;
            const ptrdiff_t GetOffset(const ptime& start, const ptime& end) const;

            const void Increment(ptime* t) const;
            static TimeStep Parse(const string& name);
            static TimeStep FromSeconds(unsigned int seconds);

            static TimeStep GetDaily();
            static TimeStep GetHourly();
            static TimeStep GetMonthlyQpp();

            static TimeStep GetUnknown();

            bool IsUnknown() const;

            static ptime CreatePtime(int year, int month, int day, int hour = 0, int minute = 0, int second = 0);
            static ptime PtimeFromIsoString(const string& t);

            static string ToString(const ptime& dt, const string& format = "YYYYMMDDThhmmss");

            string GetName() const;

        private:
            TimeStepImplementation* tsImpl = nullptr;

            void CopyTimeStepImplementation(const TimeStep& src);
            void CheckIsRegular(const string& op) const;

            static const time_duration hourlyTd;
            static const time_duration dailyTd;
            static bool FromGeneralStringPeriod(const string& name, TimeStep& tstep);

        };

        class DATATYPES_DLL_LIB TimeSeriesInfoProvider
        {
        public:
            virtual ~TimeSeriesInfoProvider();
            virtual size_t GetLength() const = 0;
            virtual TimeStep GetTimeStep() const = 0;
            virtual ptime GetStart() const = 0;
        };
    }
}
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000
