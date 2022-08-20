---
title: Classes

---

# Classes




* **namespace [boost::gregorian](/cpp/Namespaces/namespaceboost_1_1gregorian/)** 
* **namespace [boost::posix_time](/cpp/Namespaces/namespaceboost_1_1posix__time/)** 
* **namespace [cinterop](/cpp/Namespaces/namespacecinterop/)** 
    * **namespace [statistics](/cpp/Namespaces/namespacecinterop_1_1statistics/)** 
    * **namespace [timeseries](/cpp/Namespaces/namespacecinterop_1_1timeseries/)** 
* **namespace [cinterop::utils](/cpp/Namespaces/namespacecinterop_1_1utils/)** 
* **namespace [datatypes](/cpp/Namespaces/namespacedatatypes/)** 
    * **namespace [exceptions](/cpp/Namespaces/namespacedatatypes_1_1exceptions/)** 
        * **class [ExceptionUtilities](/cpp/Classes/classdatatypes_1_1exceptions_1_1ExceptionUtilities/)** 
        * **struct [RangeCheck](/cpp/Classes/structdatatypes_1_1exceptions_1_1RangeCheck/)** 
        * **struct [RangeCheck< size_t >](/cpp/Classes/structdatatypes_1_1exceptions_1_1RangeCheck_3_01size__t_01_4/)** 
        * **class [TimeSeriesChecks](/cpp/Classes/classdatatypes_1_1exceptions_1_1TimeSeriesChecks/)** 
    * **namespace [interop](/cpp/Namespaces/namespacedatatypes_1_1interop/)** 
        * **class [MissingValueHandling](/cpp/Classes/classdatatypes_1_1interop_1_1MissingValueHandling/)** 
    * **namespace [io](/cpp/Namespaces/namespacedatatypes_1_1io/)** 
        * **class [IoHelper](/cpp/Classes/classdatatypes_1_1io_1_1IoHelper/)** 
    * **namespace [tests](/cpp/Namespaces/namespacedatatypes_1_1tests/)** 
        * **class [DataTestHelper](/cpp/Classes/classdatatypes_1_1tests_1_1DataTestHelper/)** 
        * **class [FileSystemHelper](/cpp/Classes/classdatatypes_1_1tests_1_1FileSystemHelper/)** 
        * **class [TempFileCleaner](/cpp/Classes/classdatatypes_1_1tests_1_1TempFileCleaner/)** 
        * **class [TestDataLocationHelper](/cpp/Classes/classdatatypes_1_1tests_1_1TestDataLocationHelper/)** 
        * **class [TestEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1tests_1_1TestEnsembleTimeSeriesStore/)** 
        * **class [TestSingleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1tests_1_1TestSingleTimeSeriesStore/)** 
        * **class [TestTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesEnsembleTimeSeriesStore/)** <br>A time series store for unit tests. 
        * **class [TestTimeSeriesStoreFactory](/cpp/Classes/classdatatypes_1_1tests_1_1TestTimeSeriesStoreFactory/)** 
    * **namespace [timeseries](/cpp/Namespaces/namespacedatatypes_1_1timeseries/)** 
        * **struct [CommonTypes](/cpp/Classes/structdatatypes_1_1timeseries_1_1CommonTypes/)** <br>Typical ensemble and time series data types derived from a fundamental data type for each data item. 
        * **class [DataDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDescriptor/)** 
        * **class [DataDimensionDescriptor](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataDimensionDescriptor/)** 
        * **class [DataGeometryProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1DataGeometryProvider/)** 
        * **class [DefaultMissingFloatingPointPolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1DefaultMissingFloatingPointPolicy/)** 
        * **struct [DefaultMissingValuePolicyTypeFactory](/cpp/Classes/structdatatypes_1_1timeseries_1_1DefaultMissingValuePolicyTypeFactory/)** 
        * **class [DimensionsDefinitions](/cpp/Classes/classdatatypes_1_1timeseries_1_1DimensionsDefinitions/)** 
        * **class [EagerWriter](/cpp/Classes/classdatatypes_1_1timeseries_1_1EagerWriter/)** 
        * **class [EnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleStoragePolicy/)** 
        * **class [EnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1EnsembleTimeSeriesStore/)** <br>Interface definition for storages of ensembles of univariate time series. 
        * **class [GlobalAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1GlobalAttributes/)** <br>A class to hold the global attributes of a file stored in the SWIFT netCDF format. 
        * **class [IdentifiersProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1IdentifiersProvider/)** <br>An interface definition for objects that can provide hierarchical identification. 
        * **class [IrregularTimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1IrregularTimeStepImplementation/)** 
        * **class [MemoryCachingStorageWriter](/cpp/Classes/classdatatypes_1_1timeseries_1_1MemoryCachingStorageWriter/)** 
        * **class [MissingValuePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1MissingValuePolicy/)** <br>An interface for classes that define missing values in time series. 
        * **class [MonthlyQppTimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1MonthlyQppTimeStepImplementation/)** 
        * **class [MultiFileTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTimeSeriesEnsembleTimeSeriesStore/)** <br>An implementation of [TimeSeriesEnsembleTimeSeriesStore]() such that the content of a time series is spread amongst several files. 
        * **class [MultiFileTsStorage](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiFileTsStorage/)** <br>An implementation of [StoragePolicy]() such that the content of a time series is spread amongst several files. 
        * **class [MultiTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1MultiTimeSeries/)** <br>Template for time series with multiple values at time point; e.g. to hold multiple realizations of time series in an ensemble. 
        * **class [NegativeIsMissingFloadingPointPolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1NegativeIsMissingFloadingPointPolicy/)** 
        * **class [NetCdfEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfEnsembleTimeSeriesStore/)** 
        * **class [NetCdfSingleSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSingleSeriesStore/)** 
        * **class [NetCdfSourceInfo](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfSourceInfo/)** 
        * **class [NetCdfTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1NetCdfTimeSeriesEnsembleTimeSeriesStore/)** 
        * **class [NullPointerIsMissingPolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1NullPointerIsMissingPolicy/)** 
        * **class [RegularTimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1RegularTimeStepImplementation/)** 
        * **class [SharedVectorStorage](/cpp/Classes/classdatatypes_1_1timeseries_1_1SharedVectorStorage/)** <br>A storage strategy for time serie such that data is a shared state amongst several time series. 
            * **class [SharedData](/cpp/Classes/classdatatypes_1_1timeseries_1_1SharedVectorStorage_1_1SharedData/)** 
        * **class [SingleNetCdfFileStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleNetCdfFileStore/)** 
        * **class [SingleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1SingleTimeSeriesStore/)** <br>Interface definition for storages of single, univariate time series. 
        * **class [StdVectorEnsembleStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StdVectorEnsembleStoragePolicy/)** 
        * **class [StlVectorStorage](/cpp/Classes/classdatatypes_1_1timeseries_1_1StlVectorStorage/)** 
        * **class [StoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1StoragePolicy/)** <br>An interface for classes that can handle the storage of data for time series. 
        * **class [SwiftNetcdfStoreFactory](/cpp/Classes/classdatatypes_1_1timeseries_1_1SwiftNetcdfStoreFactory/)** 
        * **class [TTimeSeries](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeries/)** <br>A template for univariate, single realisasion time series. 
        * **class [TTimeSeriesLibrary](/cpp/Classes/classdatatypes_1_1timeseries_1_1TTimeSeriesLibrary/)** 
        * **class [TimeSeriesEnsembleTimeSeriesStoragePolicy](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStoragePolicy/)** 
        * **class [TimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesEnsembleTimeSeriesStore/)** <br>Interface definition for storages of time series of ensembles of time series. 
        * **class [TimeSeriesIOHelper](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesIOHelper/)** <br>Representation of an univariate, ensemble time series with a SWIFT netCDF back end. 
        * **class [TimeSeriesInfoProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesInfoProvider/)** <br>An interface definition for classes that can provide essential time series temporal characteristics. 
        * **class [TimeSeriesLibrary](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibrary/)** <br>Library of time series, for high level access to sources of time series that nmay have varying on-disk representations. 
        * **class [TimeSeriesLibraryDescription](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryDescription/)** 
        * **class [TimeSeriesLibraryFactory](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesLibraryFactory/)** 
        * **class [TimeSeriesOperations](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesOperations/)** 
        * **class [TimeSeriesProvider](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesProvider/)** <br>Library of time series, for high level access to sources of univariate, single instance time series that may have varying on-disk representations. 
        * **class [TimeSeriesSourceInfo](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfo/)** 
        * **class [TimeSeriesSourceInfoBuilder](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoBuilder/)** <br>An abstract class to allow callers to inject custom time series data sources into a time series library. 
        * **class [TimeSeriesSourceInfoImpl](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesSourceInfoImpl/)** 
        * **class [TimeSeriesStoreFactory](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeSeriesStoreFactory/)** 
        * **class [TimeStep](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStep/)** <br>Time step handling for time series. 
        * **class [TimeStepImplementation](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeStepImplementation/)** 
        * **class [TimeWindow](/cpp/Classes/classdatatypes_1_1timeseries_1_1TimeWindow/)** <br>An object that represents a time window, defining subset/trim operations on time series. 
        * **class [VariableAttributes](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableAttributes/)** <br>A class to hold the attributes of a netCDF variable stored in the SWIFT netCDF format. 
        * **class [VariableDefinition](/cpp/Classes/classdatatypes_1_1timeseries_1_1VariableDefinition/)** 
        * **class [WritableTimeSeriesEnsembleTimeSeriesStore](/cpp/Classes/classdatatypes_1_1timeseries_1_1WritableTimeSeriesEnsembleTimeSeriesStore/)** 
        * **struct [ensemble_of](/cpp/Classes/structdatatypes_1_1timeseries_1_1ensemble__of/)** 
        * **namespace [io](/cpp/Namespaces/namespacedatatypes_1_1timeseries_1_1io/)** 
            * **class [ConfigFileHelper](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1ConfigFileHelper/)** 
            * **class [SwiftNetCDFAccess](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFAccess/)** <br>Class responsible for the low-level read/write operations from/to a SWIFT netCDF file. 
            * **class [SwiftNetCDFVariablePersister](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFVariablePersister/)** 
            * **class [SwiftNetCDFVariablePersister< double >](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFVariablePersister_3_01double_01_4/)** 
            * **class [SwiftNetCDFVariablePersister< float >](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFVariablePersister_3_01float_01_4/)** 
            * **class [SwiftNetCDFVariablePersister< int >](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFVariablePersister_3_01int_01_4/)** 
            * **class [SwiftNetCDFVariablePersister< long >](/cpp/Classes/classdatatypes_1_1timeseries_1_1io_1_1SwiftNetCDFVariablePersister_3_01long_01_4/)** 
        * **struct [item_type_of](/cpp/Classes/structdatatypes_1_1timeseries_1_1item__type__of/)** 
        * **struct [time_series_of](/cpp/Classes/structdatatypes_1_1timeseries_1_1time__series__of/)** 
    * **namespace [utils](/cpp/Namespaces/namespacedatatypes_1_1utils/)** 
        * **struct [DisposeVectorTypeFactory](/cpp/Classes/structdatatypes_1_1utils_1_1DisposeVectorTypeFactory/)** 
        * **class [IfThenElse](/cpp/Classes/classdatatypes_1_1utils_1_1IfThenElse/)** 
        * **class [IfThenElse< false, Ta, Tb >](/cpp/Classes/classdatatypes_1_1utils_1_1IfThenElse_3_01false_00_01Ta_00_01Tb_01_4/)** 
        * **class [IfThenElse< true, Ta, Tb >](/cpp/Classes/classdatatypes_1_1utils_1_1IfThenElse_3_01true_00_01Ta_00_01Tb_01_4/)** 
        * **class [PointerTypeVectorDispose](/cpp/Classes/classdatatypes_1_1utils_1_1PointerTypeVectorDispose/)** 
        * **class [STLHelper](/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper/)** 
            * **class [Comparer](/cpp/Classes/classdatatypes_1_1utils_1_1STLHelper_1_1Comparer/)** 
        * **class [StringProcessing](/cpp/Classes/classdatatypes_1_1utils_1_1StringProcessing/)** 
        * **class [ValueTypeVectorDispose](/cpp/Classes/classdatatypes_1_1utils_1_1ValueTypeVectorDispose/)** 
        * **class [bad_lexical_cast](/cpp/Classes/classdatatypes_1_1utils_1_1bad__lexical__cast/)** <br>A [bad_lexical_cast]() that inherits from std::exception, unlike Boost's. Needed for graceful C API interop. 
* **namespace [moirai](/cpp/Namespaces/namespacemoirai/)** 
    * **struct [known_conversions< TimeSeriesProvider< double > >](/cpp/Classes/structmoirai_1_1known__conversions_3_01TimeSeriesProvider_3_01double_01_4_01_4/)** 
* **namespace [std](/cpp/Namespaces/namespacestd/)** 



-------------------------------

Updated on 2022-08-20 at 18:35:57 +1000
