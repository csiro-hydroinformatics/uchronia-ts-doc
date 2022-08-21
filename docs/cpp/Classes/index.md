---
title: Classes

---

# Classes




* **namespace [boost::gregorian](/uchronia-ts-doc/cpp/Namespaces/namespaceboost_1_1gregorian/)** 
* **namespace [boost::posix_time](/uchronia-ts-doc/cpp/Namespaces/namespaceboost_1_1posix__time/)** 
* **namespace [cinterop](/uchronia-ts-doc/cpp/Namespaces/namespacecinterop/)** 
    * **namespace [statistics](/uchronia-ts-doc/cpp/Namespaces/namespacecinterop_1_1statistics/)** 
    * **namespace [timeseries](/uchronia-ts-doc/cpp/Namespaces/namespacecinterop_1_1timeseries/)** 
* **namespace [cinterop::utils](/uchronia-ts-doc/cpp/Namespaces/namespacecinterop_1_1utils/)** 
* **namespace [datatypes](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes/)** 
    * **namespace [exceptions](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1exceptions/)** <br>Helper function to build consistent informative error messages in exceptions with commonalities. 
        * **class [ExceptionUtilities](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1exceptions_1_1ExceptionUtilities/)** 
        * **struct [RangeCheck](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1exceptions_1_1RangeCheck/)** 
        * **struct [RangeCheck< size_t >](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1exceptions_1_1RangeCheck_3_01size__t_01_4/)** 
        * **class [TimeSeriesChecks](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1exceptions_1_1TimeSeriesChecks/)** 
    * **namespace [interop](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1interop/)** 
        * **class [MissingValueHandling](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1interop_1_1MissingValueHandling/)** <br>Ways for wrappers to specify to this API what special numeric value to use as 'missing value' code in time series interop. 
    * **namespace [io](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1io/)** 
        * **class [IoHelper](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1io_1_1IoHelper/)** 
    * **namespace [tests](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1tests/)** 
        * **class [DataTestHelper](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/)** 
        * **class [FileSystemHelper](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1FileSystemHelper/)** 
        * **class [TempFileCleaner](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TempFileCleaner/)** 
        * **class [TestDataLocationHelper](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/)** 
        * **class [TestEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestEnsembleTimeSeriesStore/)** 
        * **class [TestSingleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/)** 
        * **class [TestTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/)** <br>A time series store for unit tests. 
        * **class [TestTimeSeriesStoreFactory](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesStoreFactory/)** 
    * **namespace [timeseries](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries/)** 
        * **struct [CommonTypes](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)** <br>Typical ensemble and time series data types derived from a fundamental data type for each data item. 
        * **class [DataDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/)** <br>Minimalist descriptor for a multidimensional time series. 
        * **class [DataDimensionDescriptor](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/)** <br>Basic descriptor for a named dimension of a data structure (time series). 
        * **class [DataGeometryProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DataGeometryProvider/)** 
        * **class [DefaultMissingFloatingPointPolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DefaultMissingFloatingPointPolicy/)** 
        * **struct [DefaultMissingValuePolicyTypeFactory](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1DefaultMissingValuePolicyTypeFactory/)** 
        * **class [DimensionsDefinitions](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/)** 
        * **class [EagerWriter](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/)** 
        * **class [EnsembleStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)** <br>An interface for classes that can handle the storage of data for ensemble time series. 
        * **class [EnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/)** <br>Interface definition for storages of ensembles of univariate time series. 
        * **class [GlobalAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/)** <br>A class to hold the global attributes of a file stored in the SWIFT netCDF format. 
        * **class [IdentifiersProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/)** <br>An interface definition for objects that can provide hierarchical identification. 
        * **class [IrregularTimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/)** 
        * **class [MemoryCachingStorageWriter](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/)** 
        * **class [MissingValuePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/)** <br>An interface for classes that define missing values in time series. 
        * **class [MonthlyQppTimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/)** 
        * **class [MultiFileTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/)** <br>An implementation of [TimeSeriesEnsembleTimeSeriesStore]() such that the content of a time series is spread amongst several files. 
        * **class [MultiFileTsStorage](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/)** <br>An implementation of [StoragePolicy]() such that the content of a time series is spread amongst several files. 
        * **class [MultiTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)** <br>Template for time series with multiple values at time point; e.g. to hold multiple realizations of time series in an ensemble. 
        * **class [NegativeIsMissingFloatingPointPolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NegativeIsMissingFloatingPointPolicy/)** 
        * **class [NetCdfEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfEnsembleTimeSeriesStore/)** 
        * **class [NetCdfSingleSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/)** 
        * **class [NetCdfSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/)** 
        * **class [NetCdfTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/)** 
        * **class [NullPointerIsMissingPolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1NullPointerIsMissingPolicy/)** 
        * **class [RegularTimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/)** 
        * **class [SharedVectorStorage](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SharedVectorStorage/)** <br>A storage strategy for time serie such that data is a shared state amongst several time series. 
            * **class [SharedData](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SharedVectorStorage_1_1SharedData/)** 
        * **class [SingleNetCdfFileStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/)** 
        * **class [SingleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/)** <br>Interface definition for storages of single, univariate time series. 
        * **class [StdVectorEnsembleStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/)** <br>std::vector based storage policy 
        * **class [StlVectorStorage](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/)** <br>Storage policy; data items are stored in standard template library std::vector. 
        * **class [StoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)** <br>An interface for classes that can handle the storage of data for time series. 
        * **class [SwiftNetcdfStoreFactory](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1SwiftNetcdfStoreFactory/)** 
        * **class [TTimeSeries](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)** <br>A template for univariate, single realisasion time series. 
        * **class [TTimeSeriesLibrary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/)** 
        * **class [TimeSeriesEnsembleTimeSeriesStoragePolicy](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/)** 
        * **class [TimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)** <br>Interface definition for storages of time series of ensembles of time series. 
        * **class [TimeSeriesIOHelper](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/)** <br>Representation of an univariate, ensemble time series with a SWIFT netCDF back end. 
        * **class [TimeSeriesInfoProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/)** <br>An interface definition for classes that can provide essential time series temporal characteristics. 
        * **class [TimeSeriesLibrary](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/)** <br>Library of time series, for high level access to sources of time series that nmay have varying on-disk representations. 
        * **class [TimeSeriesLibraryDescription](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/)** 
        * **class [TimeSeriesLibraryFactory](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/)** 
        * **class [TimeSeriesOperations](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/)** 
        * **class [TimeSeriesProvider](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesProvider/)** <br>Library of time series, for high level access to sources of univariate, single instance time series that may have varying on-disk representations. 
        * **class [TimeSeriesSourceInfo](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/)** 
        * **class [TimeSeriesSourceInfoBuilder](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoBuilder/)** <br>An abstract class to allow callers to inject custom time series data sources into a time series library. 
        * **class [TimeSeriesSourceInfoImpl](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/)** 
        * **class [TimeSeriesStoreFactory](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/)** 
        * **class [TimeStep](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/)** <br>Time step handling for time series. 
        * **class [TimeStepImplementation](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/)** 
        * **class [TimeWindow](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeWindow/)** <br>An object that represents a time window, defining subset/trim operations on time series. 
        * **class [VariableAttributes](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/)** <br>A class to hold the attributes of a netCDF variable stored in the SWIFT netCDF format. 
        * **class [VariableDefinition](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/)** 
        * **class [WritableTimeSeriesEnsembleTimeSeriesStore](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/)** <br>Interface definition for writeable storages of time series of ensembles of time series. 
        * **struct [ensemble_of](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1ensemble__of/)** 
        * **namespace [io](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1timeseries_1_1io/)** 
            * **class [ConfigFileHelper](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/)** 
            * **class [SwiftNetCDFAccess](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/)** <br>Class responsible for the low-level read/write operations from/to a SWIFT netCDF file. 
            * **class [SwiftNetCDFVariablePersister](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFVariablePersister/)** 
            * **class [SwiftNetCDFVariablePersister< double >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFVariablePersister_3_01double_01_4/)** 
            * **class [SwiftNetCDFVariablePersister< float >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFVariablePersister_3_01float_01_4/)** 
            * **class [SwiftNetCDFVariablePersister< int >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFVariablePersister_3_01int_01_4/)** 
            * **class [SwiftNetCDFVariablePersister< long >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFVariablePersister_3_01long_01_4/)** 
        * **struct [item_type_of](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1item__type__of/)** 
        * **struct [time_series_of](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1timeseries_1_1time__series__of/)** 
    * **namespace [utils](/uchronia-ts-doc/cpp/Namespaces/namespacedatatypes_1_1utils/)** 
        * **struct [DisposeVectorTypeFactory](/uchronia-ts-doc/cpp/Classes/structdatatypes_1_1utils_1_1DisposeVectorTypeFactory/)** <br>Template program; Type type is a class suitable to dispose of object T, whether it is a vector of value types, or a vector where items are pointers requiring the delete operator. Used to dispose of items in a templated time series, with items of either value or pointer types. 
        * **class [IfThenElse](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1IfThenElse/)** <br>Yield second or third argument depending on first argument. Could not find an easy to use if_then_else in the STL or Boost. [IfThenElse]() will probably be replaced. Primary template: yield second or third argument depending on first argument. 
        * **class [IfThenElse< false, Ta, Tb >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1IfThenElse_3_01false_00_01Ta_00_01Tb_01_4/)** <br>partial specialization: true yields third argument 
        * **class [IfThenElse< true, Ta, Tb >](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1IfThenElse_3_01true_00_01Ta_00_01Tb_01_4/)** <br>partial specialization: true yields second argument 
        * **class [PointerTypeVectorDispose](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1PointerTypeVectorDispose/)** 
        * **class [STLHelper](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/)** <br>Helper functions with features found in other languages but not found in the C++ standard template library. Many of these features are not used in this library (uchronia) as such, but are here as a place of convenience for dependent modelling libraries. 
            * **class [Comparer](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper_1_1Comparer/)** 
        * **class [StringProcessing](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/)** <br>Helper class with string processing related functions. These emulate methods found in other languages such as C#, R, etc. 
        * **class [ValueTypeVectorDispose](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1ValueTypeVectorDispose/)** 
        * **class [bad_lexical_cast](/uchronia-ts-doc/cpp/Classes/classdatatypes_1_1utils_1_1bad__lexical__cast/)** <br>A [bad_lexical_cast]() that inherits from std::exception, unlike Boost's. Needed for graceful C API interop. 
* **namespace [moirai](/uchronia-ts-doc/cpp/Namespaces/namespacemoirai/)** 
    * **struct [known_conversions< TimeSeriesProvider< double > >](/uchronia-ts-doc/cpp/Classes/structmoirai_1_1known__conversions_3_01TimeSeriesProvider_3_01double_01_4_01_4/)** 
* **namespace [std](/uchronia-ts-doc/cpp/Namespaces/namespacestd/)** 



-------------------------------

Updated on 2022-08-21 at 18:10:33 +1000
