---
title: datatypes/common.h

---

# datatypes/common.h



## Namespaces

| Name           |
| -------------- |
| **[datatypes](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes/)**  |
| **[datatypes::utils](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1utils/)**  |
| **[datatypes::interop](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1interop/)**  |
| **[boost::posix_time](/uchronia-ts-doc/cpp/Namespaces/namespaceboost_1_1posix__time/)**  |
| **[boost::gregorian](/uchronia-ts-doc/cpp/Namespaces/namespaceboost_1_1gregorian/)**  |

## Classes

|                | Name           |
| -------------- | -------------- |
| class | **[datatypes::utils::STLHelper](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/)** <br>Helper functions with features found in other languages but not found in the C++ standard template library. Many of these features are not used in this library (uchronia) as such, but are here as a place of convenience for dependent modelling libraries.  |
| class | **[datatypes::utils::IfThenElse< true, Ta, Tb >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1IfThenElse_3_01true_00_01Ta_00_01Tb_01_4/)** <br>partial specialization: true yields second argument  |
| class | **[datatypes::utils::IfThenElse< false, Ta, Tb >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1IfThenElse_3_01false_00_01Ta_00_01Tb_01_4/)** <br>partial specialization: true yields third argument  |
| class | **[datatypes::utils::ValueTypeVectorDispose](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1ValueTypeVectorDispose/)**  |
| class | **[datatypes::utils::PointerTypeVectorDispose](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1PointerTypeVectorDispose/)**  |
| struct | **[datatypes::utils::DisposeVectorTypeFactory](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1utils_1_1DisposeVectorTypeFactory/)** <br>Template program; Type type is a class suitable to dispose of object T, whether it is a vector of value types, or a vector where items are pointers requiring the delete operator. Used to dispose of items in a templated time series, with items of either value or pointer types.  |
| class | **[datatypes::utils::bad_lexical_cast](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1bad__lexical__cast/)** <br>A [bad_lexical_cast]() that inherits from std::exception, unlike Boost's. Needed for graceful C API interop.  |
| class | **[datatypes::utils::StringProcessing](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/)** <br>Helper class with string processing related functions. These emulate methods found in other languages such as C#, R, etc.  |
| class | **[datatypes::interop::MissingValueHandling](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1interop_1_1MissingValueHandling/)** <br>Ways for wrappers to specify to this API what special numeric value to use as 'missing value' code in time series interop.  |

## Defines

|                | Name           |
| -------------- | -------------- |
|  | **[DEFAULT_MISSING_DATA_VALUE](/uchronia-ts-doc/cpp/Files/common_8h/#define-default-missing-data-value)**  |
|  | **[DEFAULT_STATION_IDENTIFIER](/uchronia-ts-doc/cpp/Files/common_8h/#define-default-station-identifier)**  |
|  | **[STRDUP](/uchronia-ts-doc/cpp/Files/common_8h/#define-strdup)**  |
|  | **[STLSTR_TO_ANSISTR](/uchronia-ts-doc/cpp/Files/common_8h/#define-stlstr-to-ansistr)**(x)  |
|  | **[DATATYPES_DOUBLE_PRECISION_ID](/uchronia-ts-doc/cpp/Files/common_8h/#define-datatypes-double-precision-id)**  |
|  | **[DATATYPES_SINGLE_PRECISION_ID](/uchronia-ts-doc/cpp/Files/common_8h/#define-datatypes-single-precision-id)**  |
|  | **[DATATYPES_FOUR_DIMENSIONS_DATA](/uchronia-ts-doc/cpp/Files/common_8h/#define-datatypes-four-dimensions-data)**  |
|  | **[DATATYPES_THREE_DIMENSIONS_DATA](/uchronia-ts-doc/cpp/Files/common_8h/#define-datatypes-three-dimensions-data)**  |
|  | **[DATATYPES_TWO_DIMENSIONS_DATA](/uchronia-ts-doc/cpp/Files/common_8h/#define-datatypes-two-dimensions-data)**  |
|  | **[SWIFT_TIME_UNIT_MINUTE](/uchronia-ts-doc/cpp/Files/common_8h/#define-swift-time-unit-minute)**  |
|  | **[SWIFT_TIME_UNIT_HOUR](/uchronia-ts-doc/cpp/Files/common_8h/#define-swift-time-unit-hour)**  |
|  | **[SWIFT_TIME_UNIT_DAY](/uchronia-ts-doc/cpp/Files/common_8h/#define-swift-time-unit-day)**  |
|  | **[SWIFT_TIME_UNIT_MONTH](/uchronia-ts-doc/cpp/Files/common_8h/#define-swift-time-unit-month)**  |
|  | **[FILE_KEY](/uchronia-ts-doc/cpp/Files/common_8h/#define-file-key)**  |
|  | **[ID_DATA_KEY](/uchronia-ts-doc/cpp/Files/common_8h/#define-id-data-key)**  |
|  | **[VAR_KEY](/uchronia-ts-doc/cpp/Files/common_8h/#define-var-key)**  |
|  | **[IDENTIFIER_KEY](/uchronia-ts-doc/cpp/Files/common_8h/#define-identifier-key)**  |
|  | **[INDEX_KEY](/uchronia-ts-doc/cpp/Files/common_8h/#define-index-key)**  |
|  | **[TYPE_KEY](/uchronia-ts-doc/cpp/Files/common_8h/#define-type-key)**  |
|  | **[SINGLE_SERIES_COLLECTION_TYPE_ID](/uchronia-ts-doc/cpp/Files/common_8h/#define-single-series-collection-type-id)** <br>A string identifier for a multivariate time series (structurally an ensemble, but not semantically, e.g. TS for multiple sites)  |
|  | **[SINGLE_SERIES_TYPE_ID](/uchronia-ts-doc/cpp/Files/common_8h/#define-single-series-type-id)** <br>A string identifier for a single univariate time series.  |
|  | **[ENSEMBLE_SERIES_TYPE_ID](/uchronia-ts-doc/cpp/Files/common_8h/#define-ensemble-series-type-id)** <br>A string identifier for ensemble of time series (e.g. ensemble forecasts for one lead time)  |
|  | **[TIME_SERIES_ENSEMBLE_SERIES_TYPE_ID](/uchronia-ts-doc/cpp/Files/common_8h/#define-time-series-ensemble-series-type-id)** <br>A string identifier for time series of ensemble of time series (e.g. ensemble forecasts time series)  |
|  | **[TIME_SERIES_SERIES_COLLECTION_TYPE_ID](/uchronia-ts-doc/cpp/Files/common_8h/#define-time-series-series-collection-type-id)** <br>A string identifier for time series of collection of time series (e.g. forecasts for multiple sites)  |
|  | **[STORAGE_TYPE_SINGLE_NETCDF_FILE](/uchronia-ts-doc/cpp/Files/common_8h/#define-storage-type-single-netcdf-file)** <br>A string identifier for time series stored in a single netcdf file.  |
|  | **[STORAGE_TYPE_MULTIPLE_NETCDF_FILES](/uchronia-ts-doc/cpp/Files/common_8h/#define-storage-type-multiple-netcdf-files)** <br>A string identifier for time series stored in a multiple netcdf files with a date pattern.  |




## Macros Documentation

### define DEFAULT_MISSING_DATA_VALUE

```cpp
#define DEFAULT_MISSING_DATA_VALUE -9999.0
```


### define DEFAULT_STATION_IDENTIFIER

```cpp
#define DEFAULT_STATION_IDENTIFIER { "0" }
```


### define STRDUP

```cpp
#define STRDUP strdup
```


### define STLSTR_TO_ANSISTR

```cpp
#define STLSTR_TO_ANSISTR(
    x
)
STRDUP(x.c_str())
```


### define DATATYPES_DOUBLE_PRECISION_ID

```cpp
#define DATATYPES_DOUBLE_PRECISION_ID "double"
```


### define DATATYPES_SINGLE_PRECISION_ID

```cpp
#define DATATYPES_SINGLE_PRECISION_ID "single"
```


### define DATATYPES_FOUR_DIMENSIONS_DATA

```cpp
#define DATATYPES_FOUR_DIMENSIONS_DATA "4"
```


### define DATATYPES_THREE_DIMENSIONS_DATA

```cpp
#define DATATYPES_THREE_DIMENSIONS_DATA "3"
```


### define DATATYPES_TWO_DIMENSIONS_DATA

```cpp
#define DATATYPES_TWO_DIMENSIONS_DATA "2"
```


### define SWIFT_TIME_UNIT_MINUTE

```cpp
#define SWIFT_TIME_UNIT_MINUTE string("minute")
```


### define SWIFT_TIME_UNIT_HOUR

```cpp
#define SWIFT_TIME_UNIT_HOUR string("hour")
```


### define SWIFT_TIME_UNIT_DAY

```cpp
#define SWIFT_TIME_UNIT_DAY string("day")
```


### define SWIFT_TIME_UNIT_MONTH

```cpp
#define SWIFT_TIME_UNIT_MONTH string("month")
```


### define FILE_KEY

```cpp
#define FILE_KEY "File"
```


### define ID_DATA_KEY

```cpp
#define ID_DATA_KEY "Id"
```


### define VAR_KEY

```cpp
#define VAR_KEY "Var"
```


### define IDENTIFIER_KEY

```cpp
#define IDENTIFIER_KEY "Identifier"
```


### define INDEX_KEY

```cpp
#define INDEX_KEY "Index"
```


### define TYPE_KEY

```cpp
#define TYPE_KEY "Type"
```


### define SINGLE_SERIES_COLLECTION_TYPE_ID

```cpp
#define SINGLE_SERIES_COLLECTION_TYPE_ID "single_collection"
```

A string identifier for a multivariate time series (structurally an ensemble, but not semantically, e.g. TS for multiple sites) 

### define SINGLE_SERIES_TYPE_ID

```cpp
#define SINGLE_SERIES_TYPE_ID "single"
```

A string identifier for a single univariate time series. 

### define ENSEMBLE_SERIES_TYPE_ID

```cpp
#define ENSEMBLE_SERIES_TYPE_ID "ensemble_ts"
```

A string identifier for ensemble of time series (e.g. ensemble forecasts for one lead time) 

### define TIME_SERIES_ENSEMBLE_SERIES_TYPE_ID

```cpp
#define TIME_SERIES_ENSEMBLE_SERIES_TYPE_ID "ts_ensemble_ts"
```

A string identifier for time series of ensemble of time series (e.g. ensemble forecasts time series) 

### define TIME_SERIES_SERIES_COLLECTION_TYPE_ID

```cpp
#define TIME_SERIES_SERIES_COLLECTION_TYPE_ID "ts_ts_collection"
```

A string identifier for time series of collection of time series (e.g. forecasts for multiple sites) 

### define STORAGE_TYPE_SINGLE_NETCDF_FILE

```cpp
#define STORAGE_TYPE_SINGLE_NETCDF_FILE "single_nc_file"
```

A string identifier for time series stored in a single netcdf file. 

### define STORAGE_TYPE_MULTIPLE_NETCDF_FILES

```cpp
#define STORAGE_TYPE_MULTIPLE_NETCDF_FILES "multiple_nc_files_filename_date_pattern"
```

A string identifier for time series stored in a multiple netcdf files with a date pattern. 

## Source code

```cpp
#pragma once
#include <stdio.h>
#include <atomic>
#include <string> 
#include <vector>
#include <map> 
#include <boost/function.hpp>
#include <boost/lexical_cast.hpp>
#include <boost/date_time/gregorian/gregorian.hpp>
#include <boost/date_time/posix_time/posix_time.hpp>

#include <datatypes/setup_exports.h>

#ifdef _MSC_VER
#  pragma warning(push)
// class blah needs to have dll-interface to be used by clients of class blah
#  pragma warning(disable : 4251 4231 4660 4275)
#endif

#define DEFAULT_MISSING_DATA_VALUE -9999.0
#define DEFAULT_STATION_IDENTIFIER { "0" }

// You can define the following to activate the Visual Leak Detector tool for visual C++
// https://vld.codeplex.com
//#define DATATYPES_USE_VLD

#ifdef DATATYPES_USE_VLD
  #include <vld.h>
#endif

#ifdef _WIN32
  #define STRDUP _strdup
#else
  #define STRDUP strdup
#endif

#define STLSTR_TO_ANSISTR(x) STRDUP(x.c_str())

using std::string;
using std::vector;
using std::map;
using std::pair;

using namespace boost::posix_time;
using namespace boost::gregorian;

#define DATATYPES_DOUBLE_PRECISION_ID "double"
#define DATATYPES_SINGLE_PRECISION_ID "single"

#define DATATYPES_FOUR_DIMENSIONS_DATA "4"
#define DATATYPES_THREE_DIMENSIONS_DATA "3"
#define DATATYPES_TWO_DIMENSIONS_DATA "2"

#define SWIFT_TIME_UNIT_MINUTE string("minute")
#define SWIFT_TIME_UNIT_HOUR string("hour")
#define SWIFT_TIME_UNIT_DAY string("day")
#define SWIFT_TIME_UNIT_MONTH string("month")

// macros for strings used as structuring identifiers or keys in std::map

#define FILE_KEY       "File"
#define ID_DATA_KEY       "Id"
#define VAR_KEY        "Var"
#define IDENTIFIER_KEY "Identifier"
#define INDEX_KEY      "Index"
#define TYPE_KEY       "Type"

#define SINGLE_SERIES_COLLECTION_TYPE_ID       "single_collection"

#define SINGLE_SERIES_TYPE_ID                  "single"

#define ENSEMBLE_SERIES_TYPE_ID                "ensemble_ts"

#define TIME_SERIES_ENSEMBLE_SERIES_TYPE_ID    "ts_ensemble_ts"

#define TIME_SERIES_SERIES_COLLECTION_TYPE_ID  "ts_ts_collection"

#define STORAGE_TYPE_SINGLE_NETCDF_FILE        "single_nc_file"

#define STORAGE_TYPE_MULTIPLE_NETCDF_FILES     "multiple_nc_files_filename_date_pattern"


namespace datatypes
{
    namespace utils
    {

        void datatypes_delete_ansi_string_array(char** values, int arrayLength);

        class STLHelper
        {
        private:
            STLHelper();

            template <typename U>
            class Comparer
            {
                std::function<bool(const U&, const U&)>& valueCompare;
            public:
                Comparer(std::function<bool(const U&, const U&)>& valueCompare) : valueCompare(valueCompare)
                {
                }
                typedef typename vector<U>::const_iterator const_iterator;
                bool operator()(
                    const std::pair<size_t, const_iterator>& a,
                    const std::pair<size_t, const_iterator>& b)
                {
                    return valueCompare(*(a.second), *(b.second));
                }
            };


        public:
            template<typename K = string, typename V = string>
            static bool HasKey(const map<K, V>& dict, const string& key)
            {
                return(dict.find(key) != dict.end());
            }
            template<typename K = string, typename V = string>
            static vector<K> GetKeys(const map<K, V>& dict)
            {
                vector<K> res;
                res.reserve(dict.size());
                for (auto& kvpair : dict)
                    res.push_back(kvpair.first);
                return res;
            }

            template<typename K = string, typename V = string>
            static map<K, V> Remap(const map<K, V>& dict, const map<K, K>& newKeys)
            {
                map<K, V> res;
                for (const auto& kvpair : dict)
                {
                    K newKey = newKeys.at(kvpair.first);
                    res[newKey] = kvpair.second;
                }
                return res;
            }

            template<typename K = string, typename V = string>
            static map<K, V> Zip(const vector<K>& key, const vector<V>& values)
            {
                map<K, V> res;
                if (key.size() > values.size()) throw std::logic_error("Zip function must have less keys than values");
                for (size_t i = 0; i < key.size(); i++)
                    res[key[i]] = values[i];
                return res;
            }

            template<typename K = string, typename V = string>
            static vector<V> GetValues(const map<K, V>& dict)
            {
                vector<V> res;
                res.reserve(dict.size());
                for (auto& kvpair : dict)
                    res.push_back(kvpair.second);
                return res;
            }

            template<typename K = string, typename V = string>
            static vector<V> GetValues(const map<K, V>& dict, const vector<K>& keys)
            {
                vector<V> res;
                res.reserve(keys.size());
                for (auto& k : keys)
                    res.push_back(dict.at(k));
                return res;
            }

            template <typename U>
            static bool LessThan(const U& first, const U& second)
            {
                return first < second;
            }

            template <typename U>
            static bool MoreThan(const U& first, const U& second)
            {
                return first > second;
            }

            template <typename K, typename V>
            static vector<V> SortValues(
                const std::map<K,V>& in,
                const vector<K>& order)
            {
                vector<V> result;
                for(auto& k : order)
                { 
                    if (!HasKey(in, k))
                        throw std::logic_error("No entry in std::map for key " + k);
                    result.push_back(in.at(k));
                }
                return result;
            }

            template <typename T>
            static vector<T> Serialize(const vector<vector<T>>& series)
            {
                vector<T> result;
                for (size_t i = 0; i < series.size(); i++)
                {
                    auto& v = series[i];
                    auto n = result.size();
                    auto m = v.size();
                    result.resize(n + m);
                    std::copy(v.begin(), v.end(), result.begin() + n);
                }
                return result;
            }

            template <typename T, typename U>
            static vector<T> SortFromRef(
                const vector<T>& in,
                const vector<U>& reference,
                std::function<bool(const U&, const U&)> comparer = STLHelper::LessThan<U>)
            {
                // Attribution: derived from http://stackoverflow.com/a/236199/2752565, Konrad Rudolph

                typedef typename vector<U>::const_iterator myiter;
                vector<std::pair<size_t, myiter>> order(reference.size());

                size_t n = 0;
                for (myiter it = reference.begin(); it != reference.end(); ++it, ++n)
                    order[n] = std::make_pair(n, it);


                Comparer<U> ordering(comparer);

                sort(order.begin(), order.end(), ordering);

                vector<T> ret(in.size());

                size_t const size = in.size();
                for (size_t i = 0; i < size; ++i)
                    ret[i] = in[order[i].first];

                return ret;
            }
        };

        template<typename T = double>
        vector<T>  SeqVec(T from, T by, size_t num)
        {
            vector<T> data;
            data.resize(num);
            for (size_t i = 0; i < num; i++)
                data[i] = from + ((T)i)*by;
            return data;
        }

        // Template metaprogramming
        

        template<bool C, typename Ta, typename Tb>
        class IfThenElse;

        template<typename Ta, typename Tb>
        class IfThenElse < true, Ta, Tb > {
        public:
            typedef Ta ResultT;
        };

        template<typename Ta, typename Tb>
        class IfThenElse < false, Ta, Tb > {
        public:
            typedef Tb ResultT;
        };

        template <typename T>
        class ValueTypeVectorDispose
        {
        public:
            static void Dispose(vector<T>& a) { a.clear(); }
        };

        template <typename T>
        class PointerTypeVectorDispose
        {
        public:
            static void Dispose(vector<T>& a)
            {
                for (size_t i = 0; i < a.size(); i++)
                {
                    auto p = a[i];
                    if (p != nullptr)
                        delete p;
                }
                a.clear();
            }
        };

        template <typename T>
        struct DisposeVectorTypeFactory {
            typedef typename IfThenElse<
                std::is_pointer<T>::value,
                ValueTypeVectorDispose<T>,
                PointerTypeVectorDispose<T>
            >::ResultT type;
        };


        template <typename T>
        void DisposeVector(vector<T>& v)
        {
            using U = typename datatypes::utils::DisposeVectorTypeFactory<T>::type;
            U::Dispose(v);
        }

        class DATATYPES_DLL_LIB bad_lexical_cast : public std::invalid_argument
        {
        public:
            bad_lexical_cast(const string& msg);
        };

        template <typename Target>
        static Target Parse(const string& strId)
        {
            try {
                return boost::lexical_cast<Target>(strId);
            }
            catch (boost::bad_lexical_cast&)
            {
                throw datatypes::utils::bad_lexical_cast(string("Failed to parse '") + strId + string("' as a ") + string(typeid(Target).name()));
            }
        }

        template <typename Source>
        static string ToString(const Source& value)
        {
            try {
                return boost::lexical_cast<string>(value);
            }
            catch (boost::bad_lexical_cast&)
            {
                throw datatypes::utils::bad_lexical_cast(string("Failed to convert a value of type '") + string(typeid(Source).name()) + string("' to a string"));
            }
        }

        template<class TTo>
        static TTo* ConvertToArray(const vector<string>& src)
        {
            string& strId;
            TTo* result = new TTo[src.size()];
            try {
                for (int i = 0; i < src.size(); i++)
                {
                    strId = src[i];
                    result[i] = boost::lexical_cast<TTo>(strId);
                }
                return result;
            }
            catch (boost::bad_lexical_cast & c)
            {
                delete result;
                throw datatypes::utils::bad_lexical_cast(string("Failed to parse '") + strId + string("' in an vector as a ") + string(typeid(TTo).name()));
            }
        }

        template<class TFrom, class TTo>
        static TTo* ConvertToArray(const vector<TFrom>& src)
        {
            TTo* result = new TTo[src.size()];
            try {
                for (int i = 0; i < src.size(); i++)
                {
                    result[i] = (TTo)src[i];
                }
                return result;
            }
            catch (std::exception& c)
            {
                delete result;
                throw datatypes::utils::bad_lexical_cast(string("Failed to convert vector of ") +
                    string(typeid(TFrom).name()) +
                    string(" to an array of ") +
                    string(typeid(TTo).name()));
            }
        }

        template<class TFrom, class TTo>
        static vector<TTo> Convert(const vector<TFrom>& src)
        {
            vector<TTo> result(src.size());
            try {
                for (int i = 0; i < src.size(); i++)
                    result[i] = (TTo)src[i];
                return result;
            }
            catch (std::exception&)
            {
                string msg = (string("Failed to convert vector of ") +
                    string(typeid(TFrom).name()) +
                    string(" to a vector of ") +
                    string(typeid(TTo).name()));

                throw datatypes::utils::bad_lexical_cast(msg);
            }
        }

        template<class TTo>
        vector<TTo> Convert(const vector<string> & src)
        {
            string strId;
            vector<TTo> result(src.size());
            try {
                for (int i = 0; i < src.size(); i++)
                {
                    strId = src[i];
                    result[i] = boost::lexical_cast<TTo>(strId);
                }
                return result;
            }
            catch (boost::bad_lexical_cast&)
            {
                throw datatypes::utils::bad_lexical_cast(string("Failed to parse '") + strId + string("' in an vector as a ") + string(typeid(TTo).name()));
            }
        }

        class DATATYPES_DLL_LIB StringProcessing
        {
        public:
            static vector<string> Split(const string& s, const string& separators);
            static string TrimAny(const string& s, const string& charactersToTrim);
            static vector<string> SplitOnSpaces(const string& s, bool removeEmptyEntries);
            static vector<string> RemoveEmpty(const vector<string>& s);

            static vector<string> Concatenate(const vector<vector<string>>& vars);
            static void Concatenate(vector<string>& a, const vector<string>& b);


            //          static bool Contains(const string& toTest, const vector<string>& toMatch, bool caseSensitive = true);
            static bool Contains(const string& toTest, const string& toMatch, bool caseSensitive = true);
            static bool StartsWith(const string& toTest, const string& toMatch, bool caseSensitive = true);
            static bool Equals(const string& toTest, const string& toMatch, bool caseSensitive = true);
            static bool EqualsAny(const string& toTest, const vector<string>& toMatch, bool caseSensitive = true);
            static bool StringPredicate(const string& toTest, const string& toMatch, boost::function<bool(const string&, const string&)> predicate, bool caseSensitive = true);
            static string Paste(const vector<string>& items, const string& sep = "");
            static vector<string> VPaste(const vector<string>& prefixes, const string& postfix, const string& sep = "");
            static vector<string> VPaste(const string& prefix, const vector<string>& postfixes, const string& sep = "");
            static bool ContainsAll(const vector<string>& toTest, const vector<string>& toMatch, bool caseSensitive = true);
            static bool SetEquals(const vector<string>& toTest, const vector<string>& toMatch, bool caseSensitive = true);
            static vector<string> SetDiff(const vector<string>& toTest, const vector<string>& toRemove, bool caseSensitive = true);
            static vector<string> Unique(const vector<string>& set);

            static const string kElementSeparatorToken;
            static string BuildIdentifier(vector<string> &tokens, int fromIndex, int toIndex = -1, const string& sep=StringProcessing::kElementSeparatorToken);
            static string BuildIdentifier(const string &a, const string &b, const string& sep = StringProcessing::kElementSeparatorToken);


        private:
            static bool funContains(const string& toTest, const string& toMatch);
            static bool funStartsWith(const string& toTest, const string& toMatch);
            static bool funEquals(const string& toTest, const string& toMatch);
        };

        template<typename T=boost::posix_time::ptime>
        T CreateTime(int year, int month, int day, int hour = 0, int minute = 0, int second = 0)
        {
            using namespace boost::gregorian;
            return T(date(year, month, day), hours(hour) + minutes(minute) + seconds(second));
        }
    }

    namespace interop
    {
        class DATATYPES_DLL_LIB MissingValueHandling
        {
            // https://jira.csiro.au/browse/WIRADA-416
        public:
            static std::atomic<double> TimeSeriesMissingValueValue;
        };
    }

}
```


-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000
