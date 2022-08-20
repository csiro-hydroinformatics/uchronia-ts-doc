---
title: datatypes::utils::StringProcessing

---

# datatypes::utils::StringProcessing






`#include <common.h>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| vector< string > | **[Split](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#function-split)**(const string & s, const string & separators) |
| string | **[TrimAny](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#function-trimany)**(const string & s, const string & charactersToTrim) |
| vector< string > | **[SplitOnSpaces](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#function-splitonspaces)**(const string & s, bool removeEmptyEntries) |
| vector< string > | **[RemoveEmpty](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#function-removeempty)**(const vector< string > & s) |
| vector< string > | **[Concatenate](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#function-concatenate)**(const vector< vector< string >> & vars) |
| void | **[Concatenate](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#function-concatenate)**(vector< string > & a, const vector< string > & b) |
| bool | **[Contains](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#function-contains)**(const string & toTest, const string & toMatch, bool caseSensitive =true) |
| bool | **[StartsWith](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#function-startswith)**(const string & toTest, const string & toMatch, bool caseSensitive =true) |
| bool | **[Equals](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#function-equals)**(const string & toTest, const string & toMatch, bool caseSensitive =true) |
| bool | **[EqualsAny](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#function-equalsany)**(const string & toTest, const vector< string > & toMatch, bool caseSensitive =true) |
| bool | **[StringPredicate](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#function-stringpredicate)**(const string & toTest, const string & toMatch, boost::function< bool(const string &, const string &)> predicate, bool caseSensitive =true) |
| string | **[Paste](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#function-paste)**(const vector< string > & items, const string & sep ="") |
| vector< string > | **[VPaste](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#function-vpaste)**(const vector< string > & prefixes, const string & postfix, const string & sep ="") |
| vector< string > | **[VPaste](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#function-vpaste)**(const string & prefix, const vector< string > & postfixes, const string & sep ="") |
| bool | **[ContainsAll](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#function-containsall)**(const vector< string > & toTest, const vector< string > & toMatch, bool caseSensitive =true) |
| bool | **[SetEquals](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#function-setequals)**(const vector< string > & toTest, const vector< string > & toMatch, bool caseSensitive =true) |
| vector< string > | **[SetDiff](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#function-setdiff)**(const vector< string > & toTest, const vector< string > & toRemove, bool caseSensitive =true) |
| vector< string > | **[Unique](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#function-unique)**(const vector< string > & set) |
| string | **[BuildIdentifier](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#function-buildidentifier)**(vector< string > & tokens, int fromIndex, int toIndex =-1, const string & sep =[StringProcessing::kElementSeparatorToken](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#variable-kelementseparatortoken)) |
| string | **[BuildIdentifier](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#function-buildidentifier)**(const string & a, const string & b, const string & sep =[StringProcessing::kElementSeparatorToken](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#variable-kelementseparatortoken)) |

## Public Attributes

|                | Name           |
| -------------- | -------------- |
| const string | **[kElementSeparatorToken](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/#variable-kelementseparatortoken)**  |

## Public Functions Documentation

### function Split

```cpp
static vector< string > Split(
    const string & s,
    const string & separators
)
```


### function TrimAny

```cpp
static string TrimAny(
    const string & s,
    const string & charactersToTrim
)
```


### function SplitOnSpaces

```cpp
static vector< string > SplitOnSpaces(
    const string & s,
    bool removeEmptyEntries
)
```


### function RemoveEmpty

```cpp
static vector< string > RemoveEmpty(
    const vector< string > & s
)
```


### function Concatenate

```cpp
static vector< string > Concatenate(
    const vector< vector< string >> & vars
)
```


### function Concatenate

```cpp
static void Concatenate(
    vector< string > & a,
    const vector< string > & b
)
```


### function Contains

```cpp
static bool Contains(
    const string & toTest,
    const string & toMatch,
    bool caseSensitive =true
)
```


### function StartsWith

```cpp
static bool StartsWith(
    const string & toTest,
    const string & toMatch,
    bool caseSensitive =true
)
```


### function Equals

```cpp
static bool Equals(
    const string & toTest,
    const string & toMatch,
    bool caseSensitive =true
)
```


### function EqualsAny

```cpp
static bool EqualsAny(
    const string & toTest,
    const vector< string > & toMatch,
    bool caseSensitive =true
)
```


### function StringPredicate

```cpp
static bool StringPredicate(
    const string & toTest,
    const string & toMatch,
    boost::function< bool(const string &, const string &)> predicate,
    bool caseSensitive =true
)
```


### function Paste

```cpp
static string Paste(
    const vector< string > & items,
    const string & sep =""
)
```


### function VPaste

```cpp
static vector< string > VPaste(
    const vector< string > & prefixes,
    const string & postfix,
    const string & sep =""
)
```


### function VPaste

```cpp
static vector< string > VPaste(
    const string & prefix,
    const vector< string > & postfixes,
    const string & sep =""
)
```


### function ContainsAll

```cpp
static bool ContainsAll(
    const vector< string > & toTest,
    const vector< string > & toMatch,
    bool caseSensitive =true
)
```


### function SetEquals

```cpp
static bool SetEquals(
    const vector< string > & toTest,
    const vector< string > & toMatch,
    bool caseSensitive =true
)
```


### function SetDiff

```cpp
static vector< string > SetDiff(
    const vector< string > & toTest,
    const vector< string > & toRemove,
    bool caseSensitive =true
)
```


### function Unique

```cpp
static vector< string > Unique(
    const vector< string > & set
)
```


### function BuildIdentifier

```cpp
static string BuildIdentifier(
    vector< string > & tokens,
    int fromIndex,
    int toIndex =-1,
    const string & sep =StringProcessing::kElementSeparatorToken
)
```


### function BuildIdentifier

```cpp
static string BuildIdentifier(
    const string & a,
    const string & b,
    const string & sep =StringProcessing::kElementSeparatorToken
)
```


## Public Attributes Documentation

### variable kElementSeparatorToken

```cpp
static const string kElementSeparatorToken;
```


-------------------------------

Updated on 2022-08-20 at 19:28:22 +1000