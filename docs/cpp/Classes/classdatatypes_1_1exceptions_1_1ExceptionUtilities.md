---
title: datatypes::exceptions::ExceptionUtilities

---

# datatypes::exceptions::ExceptionUtilities






`#include <exception_utilities.h>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| void | **[ThrowInvalidArgument](/cpp/Classes/classdatatypes_1_1exceptions_1_1ExceptionUtilities/#function-throwinvalidargument)**(const string & msg ="Invalid argument") |
| void | **[ThrowInvalidOperation](/cpp/Classes/classdatatypes_1_1exceptions_1_1ExceptionUtilities/#function-throwinvalidoperation)**(const string & msg ="Invalid operation") |
| void | **[ThrowInvalidArgumentModelVariableId](/cpp/Classes/classdatatypes_1_1exceptions_1_1ExceptionUtilities/#function-throwinvalidargumentmodelvariableid)**(const string & variableId) |
| void | **[ThrowNotImplemented](/cpp/Classes/classdatatypes_1_1exceptions_1_1ExceptionUtilities/#function-thrownotimplemented)**(const string & msg ="Not implemented") |
| void | **[ThrowNotSupported](/cpp/Classes/classdatatypes_1_1exceptions_1_1ExceptionUtilities/#function-thrownotsupported)**(const string & typeName, const string & methodName) |
| void | **[ThrowNotSupported](/cpp/Classes/classdatatypes_1_1exceptions_1_1ExceptionUtilities/#function-thrownotsupported)**(const string & msg) |
| void | **[ThrowOutOfRange](/cpp/Classes/classdatatypes_1_1exceptions_1_1ExceptionUtilities/#function-throwoutofrange)**(const string & msg ="Operation led to a state out of range") |
| template <typename T \> <br>void | **[CheckInRange](/cpp/Classes/classdatatypes_1_1exceptions_1_1ExceptionUtilities/#function-checkinrange)**(T value, T min, T max, const string & variableName) |
| void | **[CheckFileExists](/cpp/Classes/classdatatypes_1_1exceptions_1_1ExceptionUtilities/#function-checkfileexists)**(const boost::filesystem::path & p) |
| void | **[CheckFileDoesNotExist](/cpp/Classes/classdatatypes_1_1exceptions_1_1ExceptionUtilities/#function-checkfiledoesnotexist)**(const boost::filesystem::path & p) |
| void | **[CheckExists](/cpp/Classes/classdatatypes_1_1exceptions_1_1ExceptionUtilities/#function-checkexists)**(const boost::filesystem::path & p) |

## Public Functions Documentation

### function ThrowInvalidArgument

```cpp
static inline void ThrowInvalidArgument(
    const string & msg ="Invalid argument"
)
```


### function ThrowInvalidOperation

```cpp
static inline void ThrowInvalidOperation(
    const string & msg ="Invalid operation"
)
```


### function ThrowInvalidArgumentModelVariableId

```cpp
static inline void ThrowInvalidArgumentModelVariableId(
    const string & variableId
)
```


### function ThrowNotImplemented

```cpp
static inline void ThrowNotImplemented(
    const string & msg ="Not implemented"
)
```


### function ThrowNotSupported

```cpp
static inline void ThrowNotSupported(
    const string & typeName,
    const string & methodName
)
```


### function ThrowNotSupported

```cpp
static inline void ThrowNotSupported(
    const string & msg
)
```


### function ThrowOutOfRange

```cpp
static inline void ThrowOutOfRange(
    const string & msg ="Operation led to a state out of range"
)
```


### function CheckInRange

```cpp
template <typename T >
static inline void CheckInRange(
    T value,
    T min,
    T max,
    const string & variableName
)
```


### function CheckFileExists

```cpp
static inline void CheckFileExists(
    const boost::filesystem::path & p
)
```


### function CheckFileDoesNotExist

```cpp
static inline void CheckFileDoesNotExist(
    const boost::filesystem::path & p
)
```


### function CheckExists

```cpp
static inline void CheckExists(
    const boost::filesystem::path & p
)
```


-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000