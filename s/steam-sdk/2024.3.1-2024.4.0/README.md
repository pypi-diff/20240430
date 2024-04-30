# Comparing `tmp/steam-sdk-2024.3.1.tar.gz` & `tmp/steam-sdk-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steam-sdk-2024.3.1.tar", last modified: Mon Mar 25 10:53:01 2024, max compression
+gzip compressed data, was "steam-sdk-2024.4.0.tar", last modified: Tue Apr 30 14:36:32 2024, max compression
```

## Comparing `steam-sdk-2024.3.1.tar` & `steam-sdk-2024.4.0.tar`

### file list

```diff
@@ -1,209 +1,209 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:01.797650 steam-sdk-2024.3.1/
--rw-rw-rw-   0        0        0      264 2023-06-07 14:48:24.000000 steam-sdk-2024.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5753 2024-03-25 10:53:01.795655 steam-sdk-2024.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-03-25 10:53:01.798650 steam-sdk-2024.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1668 2024-03-25 10:04:17.000000 steam-sdk-2024.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:00.082646 steam-sdk-2024.3.1/steam_sdk/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:00.163647 steam-sdk-2024.3.1/steam_sdk/analyses/
--rw-rw-rw-   0        0        0    37559 2024-03-10 18:36:09.000000 steam-sdk-2024.3.1/steam_sdk/analyses/AnalysisEvent.py
--rw-rw-rw-   0        0        0    30832 2024-03-10 18:36:09.000000 steam-sdk-2024.3.1/steam_sdk/analyses/AnalysisEventLHC.py
--rw-rw-rw-   0        0        0   162981 2024-03-25 07:30:21.000000 steam-sdk-2024.3.1/steam_sdk/analyses/AnalysisSTEAM.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:00.165649 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:00.184649 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    23388 2024-01-12 14:29:22.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:00.279647 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0    16777 2024-01-12 14:32:10.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
--rw-rw-rw-   0        0        0     2820 2024-01-12 14:32:10.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
--rw-rw-rw-   0        0        0     6761 2024-01-12 14:32:10.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
--rw-rw-rw-   0        0        0    95432 2024-01-12 14:32:10.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
--rw-rw-rw-   0        0        0     2672 2024-01-12 14:32:10.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
--rw-rw-rw-   0        0        0     2361 2024-01-12 14:29:35.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:00.300647 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    22357 2024-03-11 05:39:28.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:00.360648 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5330 2024-01-12 14:32:10.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4450 2024-01-12 14:32:10.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     2844 2024-01-12 14:32:10.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:00.383646 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
--rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
--rw-rw-rw-   0        0        0    29436 2024-03-11 05:39:28.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:00.413649 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5330 2024-01-12 14:32:09.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4627 2024-01-12 14:32:10.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     4775 2024-01-12 14:32:10.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:00.428648 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/custom_function_test_1/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
--rw-rw-rw-   0        0        0     1307 2022-09-10 00:27:54.000000 steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:00.524651 steam-sdk-2024.3.1/steam_sdk/builders/
--rw-rw-rw-   0        0        0    13175 2024-03-13 09:34:54.000000 steam-sdk-2024.3.1/steam_sdk/builders/BuilderAPDL_CT.py
--rw-rw-rw-   0        0        0     4805 2024-03-22 08:53:57.000000 steam-sdk-2024.3.1/steam_sdk/builders/BuilderCosim.py
--rw-rw-rw-   0        0        0    17741 2024-02-07 15:54:14.000000 steam-sdk-2024.3.1/steam_sdk/builders/BuilderFiQuS.py
--rw-rw-rw-   0        0        0   159399 2024-03-11 05:39:48.000000 steam-sdk-2024.3.1/steam_sdk/builders/BuilderLEDET.py
--rw-rw-rw-   0        0        0    49639 2024-03-25 10:52:36.000000 steam-sdk-2024.3.1/steam_sdk/builders/BuilderModel.py
--rw-rw-rw-   0        0        0    12686 2024-03-13 11:10:16.000000 steam-sdk-2024.3.1/steam_sdk/builders/BuilderProteCCT.py
--rw-rw-rw-   0        0        0     6749 2022-08-22 11:29:04.000000 steam-sdk-2024.3.1/steam_sdk/builders/BuilderPyBBQ.py
--rw-rw-rw-   0        0        0    12985 2024-01-08 08:44:18.000000 steam-sdk-2024.3.1/steam_sdk/builders/BuilderPySIGMA.py
--rw-rw-rw-   0        0        0    11689 2023-01-18 09:46:00.000000 steam-sdk-2024.3.1/steam_sdk/builders/SelfMutualInductanceCalculation.py
--rw-rw-rw-   0        0        0     7941 2022-12-06 11:41:34.000000 steam-sdk-2024.3.1/steam_sdk/builders/Solenoids.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/builders/__init__.py
--rw-rw-rw-   0        0        0     8352 2023-02-02 15:39:34.000000 steam-sdk-2024.3.1/steam_sdk/builders/geometricFunctions.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:00.527650 steam-sdk-2024.3.1/steam_sdk/configs/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:00.541647 steam-sdk-2024.3.1/steam_sdk/configs/tools_defaults/
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:00.543651 steam-sdk-2024.3.1/steam_sdk/configs/tools_defaults/LEDET/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/configs/tools_defaults/LEDET/__init__.py
--rw-rw-rw-   0        0        0     1426 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/configs/tools_defaults/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:00.557660 steam-sdk-2024.3.1/steam_sdk/cosims/
--rw-rw-rw-   0        0        0    14849 2024-03-25 07:30:21.000000 steam-sdk-2024.3.1/steam_sdk/cosims/CoSimPyCoSim.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/cosims/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:00.960650 steam-sdk-2024.3.1/steam_sdk/data/
--rw-rw-rw-   0        0        0     1684 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataAPDLCTOptions.py
--rw-rw-rw-   0        0        0    12184 2024-03-22 11:41:04.000000 steam-sdk-2024.3.1/steam_sdk/data/DataAnalysis.py
--rw-rw-rw-   0        0        0      414 2024-03-06 09:01:34.000000 steam-sdk-2024.3.1/steam_sdk/data/DataCoSim.py
--rw-rw-rw-   0        0        0     9151 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataConductor.py
--rw-rw-rw-   0        0        0      284 2024-03-13 09:34:52.000000 steam-sdk-2024.3.1/steam_sdk/data/DataDakota.py
--rw-rw-rw-   0        0        0     2987 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataEventCircuit.py
--rw-rw-rw-   0        0        0     4636 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataEventMagnet.py
--rw-rw-rw-   0        0        0    76269 2024-03-22 12:27:57.000000 steam-sdk-2024.3.1/steam_sdk/data/DataFiQuS.py
--rw-rw-rw-   0        0        0     7309 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataFiQuSOptions.py
--rw-rw-rw-   0        0        0    16407 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataLEDET.py
--rw-rw-rw-   0        0        0     9528 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataLEDETOptions.py
--rw-rw-rw-   0        0        0     4640 2024-03-21 13:50:31.000000 steam-sdk-2024.3.1/steam_sdk/data/DataModelCircuit.py
--rw-rw-rw-   0        0        0     5216 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataModelCommon.py
--rw-rw-rw-   0        0        0     6621 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataModelConductor.py
--rw-rw-rw-   0        0        0     9648 2024-03-22 15:13:04.000000 steam-sdk-2024.3.1/steam_sdk/data/DataModelCosim.py
--rw-rw-rw-   0        0        0     8020 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataModelMagnet.py
--rw-rw-rw-   0        0        0     4980 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataModelParsimDakota.py
--rw-rw-rw-   0        0        0     2986 2024-03-22 11:45:19.000000 steam-sdk-2024.3.1/steam_sdk/data/DataParsimConductor.py
--rw-rw-rw-   0        0        0     2130 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataProteCCT.py
--rw-rw-rw-   0        0        0     2956 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataProteCCTOptions.py
--rw-rw-rw-   0        0        0     2595 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataPyBBQ.py
--rw-rw-rw-   0        0        0     1508 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataPyBBQOptions.py
--rw-rw-rw-   0        0        0      627 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataPyCoSim.py
--rw-rw-rw-   0        0        0     6552 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataPySIGMA.py
--rw-rw-rw-   0        0        0     2228 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataPySIGMAOptions.py
--rw-rw-rw-   0        0        0      236 2024-02-01 12:22:22.000000 steam-sdk-2024.3.1/steam_sdk/data/DataRoxieParams.py
--rw-rw-rw-   0        0        0     9824 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     2700 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataSettings.py
--rw-rw-rw-   0        0        0     3263 2024-03-21 12:23:41.000000 steam-sdk-2024.3.1/steam_sdk/data/DataSignal.py
--rw-rw-rw-   0        0        0    18457 2023-11-20 11:26:58.000000 steam-sdk-2024.3.1/steam_sdk/data/DictionaryLEDET.py
--rw-rw-rw-   0        0        0     4482 2022-08-23 08:56:30.000000 steam-sdk-2024.3.1/steam_sdk/data/DictionaryProteCCT.py
--rw-rw-rw-   0        0        0     2902 2022-09-28 09:57:32.000000 steam-sdk-2024.3.1/steam_sdk/data/DictionaryPyBBQ.py
--rw-rw-rw-   0        0        0    30311 2023-11-28 14:53:04.000000 steam-sdk-2024.3.1/steam_sdk/data/TemplateLEDET.py
--rw-rw-rw-   0        0        0     7903 2022-03-30 17:37:43.000000 steam-sdk-2024.3.1/steam_sdk/data/TemplateProteCCT.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:01.095647 steam-sdk-2024.3.1/steam_sdk/drivers/
--rw-rw-rw-   0        0        0     3739 2024-01-31 11:21:01.000000 steam-sdk-2024.3.1/steam_sdk/drivers/DriverANSYS.py
--rw-rw-rw-   0        0        0    11263 2024-03-11 12:56:31.000000 steam-sdk-2024.3.1/steam_sdk/drivers/DriverAnalysis.py
--rw-rw-rw-   0        0        0     7651 2024-03-21 09:44:05.000000 steam-sdk-2024.3.1/steam_sdk/drivers/DriverDakota.py
--rw-rw-rw-   0        0        0     3693 2024-03-04 08:12:07.000000 steam-sdk-2024.3.1/steam_sdk/drivers/DriverFiQuS.py
--rw-rw-rw-   0        0        0     3573 2024-02-21 09:04:57.000000 steam-sdk-2024.3.1/steam_sdk/drivers/DriverLEDET.py
--rw-rw-rw-   0        0        0     1894 2024-03-20 11:29:04.000000 steam-sdk-2024.3.1/steam_sdk/drivers/DriverPSPICE.py
--rw-rw-rw-   0        0        0     2062 2022-09-26 06:59:06.000000 steam-sdk-2024.3.1/steam_sdk/drivers/DriverProteCCT.py
--rw-rw-rw-   0        0        0     2219 2022-06-02 08:33:55.000000 steam-sdk-2024.3.1/steam_sdk/drivers/DriverPyBBQ.py
--rw-rw-rw-   0        0        0      517 2024-02-21 14:45:24.000000 steam-sdk-2024.3.1/steam_sdk/drivers/DriverPySIGMA.py
--rw-rw-rw-   0        0        0     1983 2024-03-13 14:05:47.000000 steam-sdk-2024.3.1/steam_sdk/drivers/DriverXYCE.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/drivers/__init__.py
--rw-rw-rw-   0        0        0      723 2024-01-30 11:37:38.000000 steam-sdk-2024.3.1/steam_sdk/drivers/to_DELETE.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:01.335666 steam-sdk-2024.3.1/steam_sdk/parsers/
--rw-rw-rw-   0        0        0     4984 2022-08-22 11:29:04.000000 steam-sdk-2024.3.1/steam_sdk/parsers/CSD_Reader.py
--rw-rw-rw-   0        0        0      315 2023-10-17 12:06:12.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserCOMSOLToTxt.py
--rw-rw-rw-   0        0        0    14353 2024-03-22 08:53:57.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserCOSIM.py
--rw-rw-rw-   0        0        0     2290 2022-06-24 07:36:06.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserCond2d.py
--rw-rw-rw-   0        0        0     1024 2023-10-17 12:06:12.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserCsd.py
--rw-rw-rw-   0        0        0     6188 2023-10-17 12:06:12.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserCsv.py
--rw-rw-rw-   0        0        0     3016 2024-03-13 09:34:52.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserDakota.py
--rw-rw-rw-   0        0        0     8536 2023-02-02 15:29:22.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserExcel.py
--rw-rw-rw-   0        0        0     2614 2024-03-19 10:59:46.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserFiQuS.py
--rw-rw-rw-   0        0        0    29883 2024-03-25 10:19:25.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserLEDET.py
--rw-rw-rw-   0        0        0    12436 2023-11-22 07:56:18.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserMap2d.py
--rw-rw-rw-   0        0        0    14114 2024-03-10 18:37:11.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserMat.py
--rw-rw-rw-   0        0        0    64600 2024-03-21 15:40:45.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserPSPICE.py
--rw-rw-rw-   0        0        0     4706 2023-10-17 12:06:12.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserPdf.py
--rw-rw-rw-   0        0        0     6765 2024-03-13 13:40:54.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserProteCCT.py
--rw-rw-rw-   0        0        0     1758 2023-10-17 12:06:12.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserPyBBQ.py
--rw-rw-rw-   0        0        0     1695 2024-03-19 05:56:37.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserPyCoSim.py
--rw-rw-rw-   0        0        0     3565 2023-10-20 15:49:14.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserPySIGMA.py
--rw-rw-rw-   0        0        0   155263 2024-03-11 05:39:48.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0    11662 2023-10-17 12:06:12.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserTdms.py
--rw-rw-rw-   0        0        0    55675 2024-03-21 15:04:41.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserXYCE.py
--rw-rw-rw-   0        0        0     7792 2024-01-08 08:44:18.000000 steam-sdk-2024.3.1/steam_sdk/parsers/ParserYAML.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/parsers/__init__.py
--rw-rw-rw-   0        0        0      929 2024-03-21 13:47:53.000000 steam-sdk-2024.3.1/steam_sdk/parsers/utils_ParserCircuits.py
--rw-rw-rw-   0        0        0     9029 2024-03-22 12:17:27.000000 steam-sdk-2024.3.1/steam_sdk/parsers/utils_ParserCosims.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:01.394652 steam-sdk-2024.3.1/steam_sdk/parsims/
--rw-rw-rw-   0        0        0    65482 2024-03-22 11:42:32.000000 steam-sdk-2024.3.1/steam_sdk/parsims/ParsimConductor.py
--rw-rw-rw-   0        0        0     2739 2024-03-21 09:44:05.000000 steam-sdk-2024.3.1/steam_sdk/parsims/ParsimDakota.py
--rw-rw-rw-   0        0        0    90102 2024-02-16 08:41:13.000000 steam-sdk-2024.3.1/steam_sdk/parsims/ParsimEventCircuit.py
--rw-rw-rw-   0        0        0    48261 2024-03-18 14:18:48.000000 steam-sdk-2024.3.1/steam_sdk/parsims/ParsimEventMagnet.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/parsims/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:01.411649 steam-sdk-2024.3.1/steam_sdk/parsims/translation_dicts/
--rw-rw-rw-   0        0        0     2329 2023-05-09 19:16:09.000000 steam-sdk-2024.3.1/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
--rw-rw-rw-   0        0        0     2016 2023-05-09 19:16:09.000000 steam-sdk-2024.3.1/steam_sdk/parsims/translation_dicts/event_column_names.yaml
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:01.441657 steam-sdk-2024.3.1/steam_sdk/plotters/
--rw-rw-rw-   0        0        0    29312 2023-07-13 14:20:54.000000 steam-sdk-2024.3.1/steam_sdk/plotters/PlotterAnalysis.py
--rw-rw-rw-   0        0        0    21899 2024-03-25 10:52:36.000000 steam-sdk-2024.3.1/steam_sdk/plotters/PlotterMap2d.py
--rw-rw-rw-   0        0        0    39585 2024-03-25 10:37:11.000000 steam-sdk-2024.3.1/steam_sdk/plotters/PlotterModel.py
--rw-rw-rw-   0        0        0    22987 2022-12-06 11:41:34.000000 steam-sdk-2024.3.1/steam_sdk/plotters/PlotterParametric.py
--rw-rw-rw-   0        0        0    13246 2024-03-25 10:52:36.000000 steam-sdk-2024.3.1/steam_sdk/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:01.453649 steam-sdk-2024.3.1/steam_sdk/postprocs/
--rw-rw-rw-   0        0        0     9725 2024-03-10 18:36:09.000000 steam-sdk-2024.3.1/steam_sdk/postprocs/PostprocsMetrics.py
--rw-rw-rw-   0        0        0        0 2022-09-14 13:30:58.000000 steam-sdk-2024.3.1/steam_sdk/postprocs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:01.749649 steam-sdk-2024.3.1/steam_sdk/utils/
--rw-rw-rw-   0        0        0     2679 2023-03-13 09:01:17.000000 steam-sdk-2024.3.1/steam_sdk/utils/MTF_reading_functions.py
--rw-rw-rw-   0        0        0    15002 2024-01-12 14:37:06.000000 steam-sdk-2024.3.1/steam_sdk/utils/ModifyModelData.py
--rw-rw-rw-   0        0        0     3199 2024-01-12 14:37:06.000000 steam-sdk-2024.3.1/steam_sdk/utils/ModifyModelDataMagnet.py
--rw-rw-rw-   0        0        0     2765 2024-01-12 14:37:06.000000 steam-sdk-2024.3.1/steam_sdk/utils/ModifyModelDataconductor.py
--rw-rw-rw-   0        0        0      313 2022-03-01 14:21:51.000000 steam-sdk-2024.3.1/steam_sdk/utils/NumpyEncoder.py
--rw-rw-rw-   0        0        0     5730 2023-06-20 09:25:09.000000 steam-sdk-2024.3.1/steam_sdk/utils/ParserRoxieHelpers.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0     4994 2024-03-21 19:42:46.000000 steam-sdk-2024.3.1/steam_sdk/utils/attribute_model.py
--rw-rw-rw-   0        0        0      686 2022-06-12 12:41:34.000000 steam-sdk-2024.3.1/steam_sdk/utils/clean_NaN_from_signal.py
--rw-rw-rw-   0        0        0    12832 2023-10-02 06:56:47.000000 steam-sdk-2024.3.1/steam_sdk/utils/compare_simulations.py
--rw-rw-rw-   0        0        0     3837 2023-02-03 13:26:48.000000 steam-sdk-2024.3.1/steam_sdk/utils/compare_two_parameters.py
--rw-rw-rw-   0        0        0      227 2024-01-10 14:12:29.000000 steam-sdk-2024.3.1/steam_sdk/utils/delete_if_existing.py
--rw-rw-rw-   0        0        0      677 2024-03-17 20:35:14.000000 steam-sdk-2024.3.1/steam_sdk/utils/find_delete_files.py
--rw-rw-rw-   0        0        0     1204 2024-03-22 11:11:51.000000 steam-sdk-2024.3.1/steam_sdk/utils/get_attribute_type.py
--rw-rw-rw-   0        0        0      167 2022-06-11 12:54:31.000000 steam-sdk-2024.3.1/steam_sdk/utils/isNaN.py
--rw-rw-rw-   0        0        0      299 2022-04-12 00:42:08.000000 steam-sdk-2024.3.1/steam_sdk/utils/make_folder_if_not_existing.py
--rw-rw-rw-   0        0        0      928 2023-09-25 12:01:38.000000 steam-sdk-2024.3.1/steam_sdk/utils/make_json_schema.py
--rw-rw-rw-   0        0        0     4512 2022-05-02 08:49:48.000000 steam-sdk-2024.3.1/steam_sdk/utils/misc.py
--rw-rw-rw-   0        0        0     1878 2023-11-21 15:44:37.000000 steam-sdk-2024.3.1/steam_sdk/utils/overwrite_files.py
--rw-rw-rw-   0        0        0    11408 2024-01-10 12:09:33.000000 steam-sdk-2024.3.1/steam_sdk/utils/overwrite_output_to_reference_files.py
--rw-rw-rw-   0        0        0     3555 2023-06-13 10:45:51.000000 steam-sdk-2024.3.1/steam_sdk/utils/parse_str_to_list.py
--rw-rw-rw-   0        0        0     1048 2024-03-22 15:24:00.000000 steam-sdk-2024.3.1/steam_sdk/utils/read_settings_file.py
--rw-rw-rw-   0        0        0     3365 2023-12-06 09:10:21.000000 steam-sdk-2024.3.1/steam_sdk/utils/reformat_figure.py
--rw-rw-rw-   0        0        0      388 2022-04-11 18:20:26.000000 steam-sdk-2024.3.1/steam_sdk/utils/rgetattr.py
--rw-rw-rw-   0        0        0      460 2023-01-07 20:16:27.000000 steam-sdk-2024.3.1/steam_sdk/utils/rhasattr.py
--rw-rw-rw-   0        0        0      383 2022-04-11 18:20:26.000000 steam-sdk-2024.3.1/steam_sdk/utils/sgetattr.py
--rw-rw-rw-   0        0        0      863 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/utils/tic_toc.py
--rw-rw-rw-   0        0        0      168 2022-06-07 19:34:59.000000 steam-sdk-2024.3.1/steam_sdk/utils/unique.py
--rw-rw-rw-   0        0        0     7005 2023-05-12 14:38:34.000000 steam-sdk-2024.3.1/steam_sdk/utils/utils_PC.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:01.764652 steam-sdk-2024.3.1/steam_sdk/viewers/
--rw-rw-rw-   0        0        0    39140 2024-02-23 08:10:26.000000 steam-sdk-2024.3.1/steam_sdk/viewers/Viewer.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/viewers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:01.778652 steam-sdk-2024.3.1/steam_sdk/wrappers/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:01.780655 steam-sdk-2024.3.1/steam_sdk/wrappers/java/
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:01.782651 steam-sdk-2024.3.1/steam_sdk/wrappers/java/SING/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/wrappers/java/SING/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:01.784649 steam-sdk-2024.3.1/steam_sdk/wrappers/java/SING/jars/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/wrappers/java/SING/jars/__init__.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.3.1/steam_sdk/wrappers/java/__init__.py
--rw-rw-rw-   0        0        0     1830 2024-01-10 12:13:04.000000 steam-sdk-2024.3.1/steam_sdk/wrappers/wrapper_yaml.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:53:01.785648 steam-sdk-2024.3.1/steam_sdk.egg-info/
--rw-rw-rw-   0        0        0     5753 2024-03-25 10:52:59.000000 steam-sdk-2024.3.1/steam_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7657 2024-03-25 10:52:59.000000 steam-sdk-2024.3.1/steam_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 10:52:59.000000 steam-sdk-2024.3.1/steam_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1745 2024-03-25 10:52:59.000000 steam-sdk-2024.3.1/steam_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-25 10:52:59.000000 steam-sdk-2024.3.1/steam_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.730771 steam-sdk-2024.4.0/
+-rw-rw-rw-   0        0        0      264 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5753 2024-04-30 14:36:32.728771 steam-sdk-2024.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-30 14:36:32.730771 steam-sdk-2024.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1668 2024-04-30 14:29:21.000000 steam-sdk-2024.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.390771 steam-sdk-2024.4.0/steam_sdk/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.411770 steam-sdk-2024.4.0/steam_sdk/analyses/
+-rw-rw-rw-   0        0        0    37589 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/analyses/AnalysisEvent.py
+-rw-rw-rw-   0        0        0    30954 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/analyses/AnalysisEventLHC.py
+-rw-rw-rw-   0        0        0   133599 2024-04-30 14:35:01.000000 steam-sdk-2024.4.0/steam_sdk/analyses/AnalysisSTEAM.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.418774 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.419771 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    23388 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.436769 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0    16777 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
+-rw-rw-rw-   0        0        0     2820 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
+-rw-rw-rw-   0        0        0     6761 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
+-rw-rw-rw-   0        0        0    95432 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
+-rw-rw-rw-   0        0        0     2672 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
+-rw-rw-rw-   0        0        0     2361 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.440770 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    22357 2024-04-11 12:40:24.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.446769 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5330 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4450 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     2844 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.449770 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
+-rw-rw-rw-   0        0        0    29436 2024-04-11 12:41:03.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.456771 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5330 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4627 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     4775 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.459771 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
+-rw-rw-rw-   0        0        0     1307 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.480772 steam-sdk-2024.4.0/steam_sdk/builders/
+-rw-rw-rw-   0        0        0    13175 2024-03-21 12:26:24.000000 steam-sdk-2024.4.0/steam_sdk/builders/BuilderAPDL_CT.py
+-rw-rw-rw-   0        0        0     4805 2024-03-22 11:40:47.000000 steam-sdk-2024.4.0/steam_sdk/builders/BuilderCosim.py
+-rw-rw-rw-   0        0        0    17741 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/builders/BuilderFiQuS.py
+-rw-rw-rw-   0        0        0   160440 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/builders/BuilderLEDET.py
+-rw-rw-rw-   0        0        0    53922 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/builders/BuilderModel.py
+-rw-rw-rw-   0        0        0    12686 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/builders/BuilderProteCCT.py
+-rw-rw-rw-   0        0        0     6749 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/builders/BuilderPyBBQ.py
+-rw-rw-rw-   0        0        0    12487 2024-04-11 12:01:36.000000 steam-sdk-2024.4.0/steam_sdk/builders/BuilderPySIGMA.py
+-rw-rw-rw-   0        0        0    56494 2024-04-30 14:26:16.000000 steam-sdk-2024.4.0/steam_sdk/builders/BuilderTFM.py
+-rw-rw-rw-   0        0        0    11689 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/builders/SelfMutualInductanceCalculation.py
+-rw-rw-rw-   0        0        0     7941 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/builders/Solenoids.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/builders/__init__.py
+-rw-rw-rw-   0        0        0     8352 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/builders/geometricFunctions.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.482772 steam-sdk-2024.4.0/steam_sdk/configs/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.485771 steam-sdk-2024.4.0/steam_sdk/configs/tools_defaults/
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.486771 steam-sdk-2024.4.0/steam_sdk/configs/tools_defaults/LEDET/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/configs/tools_defaults/LEDET/__init__.py
+-rw-rw-rw-   0        0        0     1426 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/configs/tools_defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.494770 steam-sdk-2024.4.0/steam_sdk/cosims/
+-rw-rw-rw-   0        0        0    26984 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/cosims/CoSimPyCoSim.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/cosims/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.567773 steam-sdk-2024.4.0/steam_sdk/data/
+-rw-rw-rw-   0        0        0     1684 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataAPDLCTOptions.py
+-rw-rw-rw-   0        0        0    12969 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/data/DataAnalysis.py
+-rw-rw-rw-   0        0        0      414 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/data/DataCoSim.py
+-rw-rw-rw-   0        0        0     9303 2024-04-05 07:58:47.000000 steam-sdk-2024.4.0/steam_sdk/data/DataConductor.py
+-rw-rw-rw-   0        0        0      308 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/data/DataDakota.py
+-rw-rw-rw-   0        0        0     2987 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataEventCircuit.py
+-rw-rw-rw-   0        0        0     4636 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataEventMagnet.py
+-rw-rw-rw-   0        0        0    86916 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/data/DataFiQuS.py
+-rw-rw-rw-   0        0        0     7309 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataFiQuSOptions.py
+-rw-rw-rw-   0        0        0    16769 2024-04-05 07:58:47.000000 steam-sdk-2024.4.0/steam_sdk/data/DataLEDET.py
+-rw-rw-rw-   0        0        0     9528 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataLEDETOptions.py
+-rw-rw-rw-   0        0        0     5377 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/data/DataModelCircuit.py
+-rw-rw-rw-   0        0        0     5216 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataModelCommon.py
+-rw-rw-rw-   0        0        0     6621 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataModelConductor.py
+-rw-rw-rw-   0        0        0    12150 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/data/DataModelCosim.py
+-rw-rw-rw-   0        0        0     8020 2024-04-30 14:26:16.000000 steam-sdk-2024.4.0/steam_sdk/data/DataModelMagnet.py
+-rw-rw-rw-   0        0        0     6491 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/data/DataModelParsimDakota.py
+-rw-rw-rw-   0        0        0     3008 2024-04-08 08:37:58.000000 steam-sdk-2024.4.0/steam_sdk/data/DataParsimConductor.py
+-rw-rw-rw-   0        0        0     2130 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataProteCCT.py
+-rw-rw-rw-   0        0        0     2956 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataProteCCTOptions.py
+-rw-rw-rw-   0        0        0     2595 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataPyBBQ.py
+-rw-rw-rw-   0        0        0     1508 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataPyBBQOptions.py
+-rw-rw-rw-   0        0        0      766 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/data/DataPyCoSim.py
+-rw-rw-rw-   0        0        0     6552 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataPySIGMA.py
+-rw-rw-rw-   0        0        0     2228 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataPySIGMAOptions.py
+-rw-rw-rw-   0        0        0      236 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/data/DataRoxieParams.py
+-rw-rw-rw-   0        0        0     9824 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0    12404 2024-04-12 18:44:18.000000 steam-sdk-2024.4.0/steam_sdk/data/DataSettings.py
+-rw-rw-rw-   0        0        0     3263 2024-03-19 10:04:08.000000 steam-sdk-2024.4.0/steam_sdk/data/DataSignal.py
+-rw-rw-rw-   0        0        0     5926 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/data/DataTFM.py
+-rw-rw-rw-   0        0        0    18457 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/data/DictionaryLEDET.py
+-rw-rw-rw-   0        0        0     4482 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/data/DictionaryProteCCT.py
+-rw-rw-rw-   0        0        0     2902 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/data/DictionaryPyBBQ.py
+-rw-rw-rw-   0        0        0    30456 2024-04-05 07:58:47.000000 steam-sdk-2024.4.0/steam_sdk/data/TemplateLEDET.py
+-rw-rw-rw-   0        0        0     7903 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/data/TemplateProteCCT.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.580771 steam-sdk-2024.4.0/steam_sdk/drivers/
+-rw-rw-rw-   0        0        0     3739 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/drivers/DriverANSYS.py
+-rw-rw-rw-   0        0        0    13733 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/drivers/DriverAnalysis.py
+-rw-rw-rw-   0        0        0     7448 2024-04-14 11:58:12.000000 steam-sdk-2024.4.0/steam_sdk/drivers/DriverDakota.py
+-rw-rw-rw-   0        0        0     4278 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/drivers/DriverFiQuS.py
+-rw-rw-rw-   0        0        0     3573 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/drivers/DriverLEDET.py
+-rw-rw-rw-   0        0        0     1894 2024-03-21 12:26:24.000000 steam-sdk-2024.4.0/steam_sdk/drivers/DriverPSPICE.py
+-rw-rw-rw-   0        0        0     2275 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/drivers/DriverProteCCT.py
+-rw-rw-rw-   0        0        0     2219 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/drivers/DriverPyBBQ.py
+-rw-rw-rw-   0        0        0      517 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/drivers/DriverPySIGMA.py
+-rw-rw-rw-   0        0        0     1983 2024-03-21 12:26:24.000000 steam-sdk-2024.4.0/steam_sdk/drivers/DriverXYCE.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/drivers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.617769 steam-sdk-2024.4.0/steam_sdk/parsers/
+-rw-rw-rw-   0        0        0     4984 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsers/CSD_Reader.py
+-rw-rw-rw-   0        0        0      315 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserCOMSOLToTxt.py
+-rw-rw-rw-   0        0        0    14173 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserCOSIM.py
+-rw-rw-rw-   0        0        0     2290 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserCond2d.py
+-rw-rw-rw-   0        0        0     1024 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserCsd.py
+-rw-rw-rw-   0        0        0     6302 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserCsv.py
+-rw-rw-rw-   0        0        0     2729 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserDakota.py
+-rw-rw-rw-   0        0        0     8536 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserExcel.py
+-rw-rw-rw-   0        0        0     2614 2024-03-21 12:26:24.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserFiQuS.py
+-rw-rw-rw-   0        0        0     3760 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserFile.py
+-rw-rw-rw-   0        0        0    30071 2024-04-30 14:35:01.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserLEDET.py
+-rw-rw-rw-   0        0        0    18391 2024-04-30 14:35:01.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserMap2d.py
+-rw-rw-rw-   0        0        0    15085 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserMat.py
+-rw-rw-rw-   0        0        0    65009 2024-04-12 18:35:10.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserPSPICE.py
+-rw-rw-rw-   0        0        0     4706 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserPdf.py
+-rw-rw-rw-   0        0        0     6765 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserProteCCT.py
+-rw-rw-rw-   0        0        0     1758 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserPyBBQ.py
+-rw-rw-rw-   0        0        0     1663 2024-04-22 06:54:43.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserPyCoSim.py
+-rw-rw-rw-   0        0        0     4061 2024-04-11 12:27:48.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserPySIGMA.py
+-rw-rw-rw-   0        0        0   155447 2024-04-15 21:11:35.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0    11746 2024-04-12 18:35:10.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserTdms.py
+-rw-rw-rw-   0        0        0    58167 2024-04-30 14:26:16.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserXYCE.py
+-rw-rw-rw-   0        0        0     7770 2024-04-05 07:58:47.000000 steam-sdk-2024.4.0/steam_sdk/parsers/ParserYAML.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsers/__init__.py
+-rw-rw-rw-   0        0        0      929 2024-03-22 11:40:47.000000 steam-sdk-2024.4.0/steam_sdk/parsers/utils_ParserCircuits.py
+-rw-rw-rw-   0        0        0     9687 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/parsers/utils_ParserCosims.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.625769 steam-sdk-2024.4.0/steam_sdk/parsims/
+-rw-rw-rw-   0        0        0    66858 2024-04-15 21:11:35.000000 steam-sdk-2024.4.0/steam_sdk/parsims/ParsimConductor.py
+-rw-rw-rw-   0        0        0     4619 2024-04-14 11:38:50.000000 steam-sdk-2024.4.0/steam_sdk/parsims/ParsimDakota.py
+-rw-rw-rw-   0        0        0    90102 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsims/ParsimEventCircuit.py
+-rw-rw-rw-   0        0        0    48261 2024-03-21 12:26:24.000000 steam-sdk-2024.4.0/steam_sdk/parsims/ParsimEventMagnet.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsims/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.631770 steam-sdk-2024.4.0/steam_sdk/parsims/translation_dicts/
+-rw-rw-rw-   0        0        0     2351 2024-04-08 08:37:58.000000 steam-sdk-2024.4.0/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
+-rw-rw-rw-   0        0        0     2016 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/parsims/translation_dicts/event_column_names.yaml
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.638769 steam-sdk-2024.4.0/steam_sdk/plotters/
+-rw-rw-rw-   0        0        0    29312 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/plotters/PlotterAnalysis.py
+-rw-rw-rw-   0        0        0    20777 2024-04-30 14:35:01.000000 steam-sdk-2024.4.0/steam_sdk/plotters/PlotterMap2d.py
+-rw-rw-rw-   0        0        0    39519 2024-04-15 21:11:35.000000 steam-sdk-2024.4.0/steam_sdk/plotters/PlotterModel.py
+-rw-rw-rw-   0        0        0    22987 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/plotters/PlotterParametric.py
+-rw-rw-rw-   0        0        0    13246 2024-03-26 07:52:01.000000 steam-sdk-2024.4.0/steam_sdk/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.640770 steam-sdk-2024.4.0/steam_sdk/postprocs/
+-rw-rw-rw-   0        0        0    11619 2024-04-30 05:16:26.000000 steam-sdk-2024.4.0/steam_sdk/postprocs/PostprocsMetrics.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/postprocs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.702769 steam-sdk-2024.4.0/steam_sdk/utils/
+-rw-rw-rw-   0        0        0     2679 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/MTF_reading_functions.py
+-rw-rw-rw-   0        0        0      204 2024-04-15 21:11:35.000000 steam-sdk-2024.4.0/steam_sdk/utils/MatrixOperations.py
+-rw-rw-rw-   0        0        0    15002 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/ModifyModelData.py
+-rw-rw-rw-   0        0        0     3201 2024-04-05 07:58:47.000000 steam-sdk-2024.4.0/steam_sdk/utils/ModifyModelDataMagnet.py
+-rw-rw-rw-   0        0        0     2770 2024-04-05 07:58:47.000000 steam-sdk-2024.4.0/steam_sdk/utils/ModifyModelDataconductor.py
+-rw-rw-rw-   0        0        0      313 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/NumpyEncoder.py
+-rw-rw-rw-   0        0        0     5730 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/ParserRoxieHelpers.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0     5806 2024-04-05 07:58:47.000000 steam-sdk-2024.4.0/steam_sdk/utils/attribute_model.py
+-rw-rw-rw-   0        0        0      686 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/clean_NaN_from_signal.py
+-rw-rw-rw-   0        0        0    12832 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/compare_simulations.py
+-rw-rw-rw-   0        0        0     3837 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/compare_two_parameters.py
+-rw-rw-rw-   0        0        0     1650 2024-04-12 18:35:10.000000 steam-sdk-2024.4.0/steam_sdk/utils/correct_RRR_NIST.py
+-rw-rw-rw-   0        0        0      227 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/delete_if_existing.py
+-rw-rw-rw-   0        0        0     1204 2024-03-22 11:42:52.000000 steam-sdk-2024.4.0/steam_sdk/utils/get_attribute_type.py
+-rw-rw-rw-   0        0        0      167 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/isNaN.py
+-rw-rw-rw-   0        0        0      691 2024-04-11 06:51:22.000000 steam-sdk-2024.4.0/steam_sdk/utils/make_folder_if_not_existing.py
+-rw-rw-rw-   0        0        0     4512 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/misc.py
+-rw-rw-rw-   0        0        0     3555 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/parse_str_to_list.py
+-rw-rw-rw-   0        0        0     1596 2024-04-13 18:58:31.000000 steam-sdk-2024.4.0/steam_sdk/utils/read_settings_file.py
+-rw-rw-rw-   0        0        0     3365 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/reformat_figure.py
+-rw-rw-rw-   0        0        0      388 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/rgetattr.py
+-rw-rw-rw-   0        0        0      460 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/rhasattr.py
+-rw-rw-rw-   0        0        0      383 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/sgetattr.py
+-rw-rw-rw-   0        0        0      863 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/tic_toc.py
+-rw-rw-rw-   0        0        0      168 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/unique.py
+-rw-rw-rw-   0        0        0     7005 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/utils/utils_PC.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.704770 steam-sdk-2024.4.0/steam_sdk/viewers/
+-rw-rw-rw-   0        0        0    39140 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/viewers/Viewer.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/viewers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.709769 steam-sdk-2024.4.0/steam_sdk/wrappers/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/wrappers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.717770 steam-sdk-2024.4.0/steam_sdk/wrappers/java/
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.718770 steam-sdk-2024.4.0/steam_sdk/wrappers/java/SING/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/wrappers/java/SING/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.719770 steam-sdk-2024.4.0/steam_sdk/wrappers/java/SING/jars/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/wrappers/java/SING/jars/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/wrappers/java/__init__.py
+-rw-rw-rw-   0        0        0     1830 2024-03-19 09:48:27.000000 steam-sdk-2024.4.0/steam_sdk/wrappers/wrapper_yaml.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:36:32.720770 steam-sdk-2024.4.0/steam_sdk.egg-info/
+-rw-rw-rw-   0        0        0     5753 2024-04-30 14:36:27.000000 steam-sdk-2024.4.0/steam_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7626 2024-04-30 14:36:28.000000 steam-sdk-2024.4.0/steam_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 14:36:27.000000 steam-sdk-2024.4.0/steam_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1745 2024-04-30 14:36:27.000000 steam-sdk-2024.4.0/steam_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-30 14:36:27.000000 steam-sdk-2024.4.0/steam_sdk.egg-info/top_level.txt
```

### Comparing `steam-sdk-2024.3.1/PKG-INFO` & `steam-sdk-2024.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2024.3.1
+Version: 2024.4.0
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
-Keywords: API,SDK,STEAM,CERN
+Keywords: STEAM,API,SDK,CERN
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: gmsh==4.11.1
 Requires-Dist: matplotlib==3.8.3
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: numpy==1.26.4
@@ -24,15 +24,15 @@
 Requires-Dist: matplotlib-inline==0.1.6
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: pysoleno==0.0.8
 Requires-Dist: reportlab==4.1.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: ruamel.yaml.clib==0.2.8
 Requires-Dist: seaborn==0.13.2
-Requires-Dist: STEAM-materials==2023.5.1
+Requires-Dist: STEAM-materials==2024.4.2
 Requires-Dist: svglib==1.5.1
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: steam-pysigma==2024.3.2
 Requires-Dist: pyarrow==15.0.1
 Requires-Dist: tqdm==4.66.2
 Provides-Extra: all
 Requires-Dist: gmsh==4.11.1; extra == "all"
@@ -50,15 +50,15 @@
 Requires-Dist: matplotlib-inline==0.1.6; extra == "all"
 Requires-Dist: openpyxl==3.1.2; extra == "all"
 Requires-Dist: pysoleno==0.0.8; extra == "all"
 Requires-Dist: reportlab==4.1.0; extra == "all"
 Requires-Dist: requests==2.31.0; extra == "all"
 Requires-Dist: ruamel.yaml.clib==0.2.8; extra == "all"
 Requires-Dist: seaborn==0.13.2; extra == "all"
-Requires-Dist: STEAM-materials==2023.5.1; extra == "all"
+Requires-Dist: STEAM-materials==2024.4.2; extra == "all"
 Requires-Dist: svglib==1.5.1; extra == "all"
 Requires-Dist: PyYAML==6.0.1; extra == "all"
 Requires-Dist: steam-pysigma==2024.3.2; extra == "all"
 Requires-Dist: pyarrow==15.0.1; extra == "all"
 Requires-Dist: tqdm==4.66.2; extra == "all"
 Requires-Dist: Markdown==3.5.2; extra == "all"
 Requires-Dist: markdown-include==0.8.1; extra == "all"
```

### Comparing `steam-sdk-2024.3.1/setup.py` & `steam-sdk-2024.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 build_require = ["setuptools==69.2.0"]
 
 all_requirements = required + docs_require + tests_require + build_require
 
 setup(
     name="steam-sdk",
-    version="2024.3.1",
+    version="2024.4.0",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Source code for APIs for STEAM tools.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.cern.ch/steam/steam_sdk",
     keywords={"STEAM", "API", "SDK", "CERN"},
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/analyses/AnalysisEvent.py` & `steam-sdk-2024.4.0/steam_sdk/analyses/AnalysisEvent.py`

 * *Files 1% similar despite different names*

```diff
@@ -435,16 +435,17 @@
 
         This function reads the specified YAML file using ruamel.yaml, iterates through
         the 'ConfigurationList' and 'SignalList' sections, and extracts the 'sim_label'
         field for each signal. It ignores signals ending with '_zoom' and returns a list
         of unique simulation signal labels.
 
         """
-    with open(full_config_file_path, 'r') as file:
-        yaml_data = ruamel.yaml.load(file, ruamel.yaml.RoundTripLoader)
+    with open(full_config_file_path, 'r') as yaml_file:
+        yaml = ruamel.yaml.YAML(typ="safe", pure=True)
+        yaml_data = yaml.load(yaml_file)
 
     signal_keys = []
 
     for config_key, config_value in yaml_data['ConfigurationList'].items():
         if config_key == configuration:
             for signal_key, signal_value in config_value['SignalList'].items():
                 if signal_key.endswith('_zoom'):
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/analyses/AnalysisEventLHC.py` & `steam-sdk-2024.4.0/steam_sdk/analyses/AnalysisEventLHC.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import shutil
 
+from ruamel.yaml import YAML
+
 from steam_sdk.analyses.AnalysisSTEAM import AnalysisSTEAM
 from steam_sdk.analyses.AnalysisEvent import find_IPQ_circuit_type_from_IPQ_parameters_table, \
     get_circuit_name_from_eventfile, generate_unique_event_identifier_from_eventfile, \
     get_signal_keys_from_configurations_file, determine_config_path_and_configuration, \
     get_circuit_type_from_circuit_name, extract_signal_touples_from_config, get_hard_coded_filename_postfix
-from steam_sdk.data.DataAnalysis import ModifyModelMultipleVariables, SetUpFolder, MakeModel, ParsimEvent, \
+from steam_sdk.data.DataAnalysis import ModifyModelMultipleVariables, MakeModel, ParsimEvent, \
     DefaultParsimEventKeys, RunSimulation, RunViewer, CalculateMetrics
 import os
 import ruamel.yaml
 import warnings
 
 
 
@@ -27,19 +29,21 @@
         'output_directory_yaml_files': os.path.join(os.getcwd(), 'output', 'yaml_files'),                               #TODO: put by default every single file in the simulation folder
         'output_directory_parsim_sweep_files': os.path.join(os.getcwd(), 'output', 'parsim_sweep_files'),
         'output_directory_initialization_file_viewer': os.path.join(os.getcwd(), 'output', 'initialization_files_viewer'),
         'path_postmortem_offline_data_folder': None,
         'filepath_to_temp_viewer_csv': None,
         'path_output_pdf_report': None ,
         'metrics_to_calculate':None,
+        'local_library_path': None,
     }
 
     # Fill up non user specific keys of the default dictionary with keys from the settings system.yaml
     with open(settings_file_path, 'r') as yaml_file:
-        settings_file_yaml_data = ruamel.yaml.safe_load(yaml_file)
+        yaml = ruamel.yaml.YAML(typ="safe", pure=True)
+        settings_file_yaml_data = yaml.load(yaml_file)
 
     for key, _ in default_dict_settings_paths.items():
         if key in settings_file_yaml_data and default_dict_settings_paths[key] is None:
             default_dict_settings_paths[key] = settings_file_yaml_data[key]
             print(f"Took over {key} from settings file")
 
     # If user provides a settings dictionary, overwrite the default values with the dictionary, provided by the user
@@ -69,15 +73,15 @@
                 print('{}: {}. Added.'.format(name, value))
         elif name == 'library_path':
             AnalysisSTEAM_object.library_path = default_dict_settings_paths['library_path']
         else:
             print('{}: not found in the settings. Skipped.'.format(name))
 
     # Update data_analysis module settings with entries of the dictionary passed
-    AnalysisSTEAM_object.data_analysis.WorkingFolders.library_path = default_dict_settings_paths['library_path']
+    # AnalysisSTEAM_object.data_analysis.WorkingFolders.library_path = default_dict_settings_paths['library_path']
     AnalysisSTEAM_object.data_analysis.PermanentSettings.PSPICE_path = default_dict_settings_paths['PSPICE_path']
     AnalysisSTEAM_object.data_analysis.PermanentSettings.XYCE_path = default_dict_settings_paths['XYCE_path']
     AnalysisSTEAM_object.data_analysis.PermanentSettings.local_PSPICE_folder = default_dict_settings_paths['local_PSPICE_folder']
     AnalysisSTEAM_object.data_analysis.PermanentSettings.local_XYCE_folder = default_dict_settings_paths['local_XYCE_folder']
 
 def steam_analyze_lhc_event(settings_file_path:str, input_csv_file: str, flag_run_software: bool, flag_calculate_metrics: bool, software: str, overwrite_settings: dict, file_counter: int, modify_model_steps: dict =None):
 
@@ -104,15 +108,14 @@
 
     unique_identifier_event = generate_unique_event_identifier_from_eventfile(
         file_name=os.path.basename(input_csv_file))
 
     #only combination of circuit_name and eventlabel is truely unique since the double circuits
     hard_coded_filename_postfix = get_hard_coded_filename_postfix(unique_identifier_event, circuit_name)
 
-
     if not settings_dictionary['filepath_to_temp_viewer_csv']:
         settings_dictionary['filepath_to_temp_viewer_csv'] = \
             fr"C:\temp{software}\{circuit_type}\{file_counter}\temp_viewer{hard_coded_filename_postfix}.csv"
 
     if not settings_dictionary['path_output_pdf_report']:
         settings_dictionary['path_output_pdf_report'] = \
             fr"C:\temp{software}\{circuit_type}\{file_counter}\report{hard_coded_filename_postfix}.pdf"
@@ -140,36 +143,35 @@
         variables_to_analyze = extract_signal_touples_from_config(full_config_file_path, configuration)
 
     else:
         warnings.warn("no signals from the config file will be included in the model, variables entry will be empty in"
                       " the cir file, causing all signals to be calculated")
 
     aSTEAM.data_analysis.AnalysisStepDefinition = {
-        'setup_folder_PSPICE': SetUpFolder(type='SetUpFolder', simulation_name=circuit_type, software=[software]),
         'makeModel_ref': MakeModel(type='MakeModel', model_name='BM', file_model_data=circuit_type,
-                                   case_model='circuit', software=[software], simulation_name=None,
+                                   case_model='circuit', software=software, simulation_name=None,
                                    simulation_number=None, flag_build=True, verbose=False,
                                    flag_plot_all=False, flag_json=False),
         'modifyModel_probe1': ModifyModelMultipleVariables(type='ModifyModelMultipleVariables', model_name='BM',
                                        variables_to_change=['PostProcess.probe.probe_type'],
-                                       variables_value=[['CSDF']], software=[software], simulation_name=None,
+                                       variables_value=[['CSDF']], software=software, simulation_name=None,
                                        simulation_numbers=[]),
 
         #Here I implement an additional step so that all signals (and only those) are safed in the variables
         'modifyModel_include_config_signals': ModifyModelMultipleVariables(type='ModifyModelMultipleVariables', model_name='BM',
                                                           variables_to_change=['PostProcess.probe.variables'],
-                                                          variables_value=[[signals_to_include]], software=[software],
+                                                          variables_value=[[signals_to_include]], software=software,
                                                           simulation_name=None,
                                                           simulation_numbers=[]),
 
         'runParsimEvent': ParsimEvent(type='ParsimEvent', input_file=input_csv_file,
                                       path_output_event_csv=path_output_parsim_sweep_csv,
                                       path_output_viewer_csv=output_directory_initialization_file_viewer,
                                       simulation_numbers=[file_counter], model_name='BM', case_model='circuit',
-                                      simulation_name=circuit_type, software=[software], t_PC_off=None,
+                                      simulation_name=circuit_type, software=software, t_PC_off=None,
                                       rel_quench_heater_trip_threshold=None, current_polarities_CLIQ=[],
                                       dict_QH_circuits_to_QH_strips={},
                                       default_keys=DefaultParsimEventKeys(local_LEDET_folder=None,
                                                                           path_config_file=None, default_configs=[],
                                                                           path_tdms_files=None,
                                                                           path_output_measurement_files=None,
                                                                           path_output=local_folder),
@@ -186,26 +188,26 @@
                                flag_save_figures=True, viewer_name="viewer_1",
                                path_output_pdf_report=settings_dictionary['path_output_pdf_report']),
 
         "CalculateMetrics": CalculateMetrics(type="CalculateMetrics",
                                              viewer_name="viewer_1",
                                              metrics_name="metrics",
                                              metrics_to_calculate=settings_dictionary['metrics_to_calculate'],
-                                             variables_to_analyze=variables_to_analyze),
-
+                                             variables_to_analyze=variables_to_analyze,
+                                             metrics_output_filepath = os.path.join(local_folder,circuit_type,str(file_counter),"output_metrics.yaml")
+                                             ),
     }
-
     aSTEAM.output_path = local_folder
     if software == 'PSPICE':
         aSTEAM.data_analysis.PermanentSettings.local_PSPICE_folder = local_folder
     elif software == 'XYCE':
         aSTEAM.data_analysis.PermanentSettings.local_XYCE_folder = local_folder
 
-    AnalysisStepSequence = ['setup_folder_PSPICE', 'makeModel_ref', 'modifyModel_probe1',
-                                                 'modifyModel_include_config_signals', 'runParsimEvent']
+    AnalysisStepSequence = ['makeModel_ref', 'modifyModel_probe1', 'modifyModel_include_config_signals',
+                            'runParsimEvent']
 
     if flag_run_software == True: AnalysisStepSequence.append('run_simulation')
 
     # If the flag for running a simulation is set, the run_simulation step will be appended to the analysis step sequence
     if flag_calculate_metrics== True: AnalysisStepSequence.extend(["RunViewer", "CalculateMetrics"])
 
     aSTEAM.data_analysis.AnalysisStepSequence = AnalysisStepSequence
@@ -286,54 +288,57 @@
                                                                               settings_dictionary['directory_config_files'],
                                                                             steam_circuit_type="RCO")
         signals_to_include = get_signal_keys_from_configurations_file(full_config_file_path, configuration = configuration)
     else:
         warnings.warn("no signals from the config file will be included in the model, variables entry will be empty in"
                       " the cir file, causing all signals to be calculated")
 
-    aSTEAM_1.data_analysis.AnalysisStepDefinition = {'setup_folder_PSPICE': SetUpFolder(type='SetUpFolder', simulation_name='RCO', software=[software]),
+    aSTEAM_1.data_analysis.AnalysisStepDefinition = {
          'makeModel_ref': MakeModel(
             type='MakeModel', model_name='BM', file_model_data='RCO',
-            case_model='circuit', software=[software], simulation_name=None,
+            case_model='circuit', software=software, simulation_name=None,
             simulation_number=None, flag_build=True, verbose=False,
             flag_plot_all=False, flag_json=False),
          'modifyModel_probe1': ModifyModelMultipleVariables(
              type='ModifyModelMultipleVariables', model_name='BM',
              variables_to_change=['PostProcess.probe.probe_type'],
-             variables_value=[['CSDF']], software=[software],
+             variables_value=[['CSDF']], software=software,
              simulation_name=None,
              simulation_numbers=[]),
          # Here I implement an additional step so that all signals (and only those) are safed in the variables
          'modifyModel_include_config_signals': ModifyModelMultipleVariables(
              type='ModifyModelMultipleVariables', model_name='BM',
              variables_to_change=['PostProcess.probe.variables'],
-             variables_value=[[signals_to_include]], software=[software],
+             variables_value=[[signals_to_include]], software=software,
              simulation_name=None,
              simulation_numbers=[]),
         'runParsimEvent': ParsimEvent(
             type='ParsimEvent',input_file=input_csv_file,
             path_output_event_csv=path_output_parsim_sweep_RCO_csv, path_output_viewer_csv=None,
             simulation_numbers=[file_counter], model_name='BM', case_model='circuit',
-            simulation_name='RCO', software=[software], t_PC_off=None, rel_quench_heater_trip_threshold=None,
+            simulation_name='RCO', software=software, t_PC_off=None, rel_quench_heater_trip_threshold=None,
             current_polarities_CLIQ=[], dict_QH_circuits_to_QH_strips={},default_keys=DefaultParsimEventKeys(
             local_LEDET_folder=None, path_config_file=None,default_configs=[],path_tdms_files=None,
             path_output_measurement_files=None,path_output=local_folder),
             path_postmortem_offline_data_folder = settings_dictionary['path_postmortem_offline_data_folder'],
             path_to_configurations_folder = settings_dictionary['directory_config_files'],
             filepath_to_temp_viewer_csv = settings_dictionary['filepath_to_temp_viewer_csv']),
         'run_simulation': RunSimulation(type='RunSimulation', software=software, simulation_name='RCO', simulation_numbers=[file_counter])}
     aSTEAM_1.output_path = local_folder
     if software == 'PSPICE':
         aSTEAM_1.data_analysis.PermanentSettings.local_PSPICE_folder = local_folder
     elif software == 'XYCE':
         aSTEAM_1.data_analysis.PermanentSettings.local_XYCE_folder = local_folder
     if flag_run_software == False:
-        aSTEAM_1.data_analysis.AnalysisStepSequence = ['setup_folder_PSPICE', 'makeModel_ref','modifyModel_probe1','modifyModel_include_config_signals', 'runParsimEvent']
+        aSTEAM_1.data_analysis.AnalysisStepSequence = ['makeModel_ref', 'modifyModel_probe1',
+                                                       'modifyModel_include_config_signals', 'runParsimEvent']
     else:
-        aSTEAM_1.data_analysis.AnalysisStepSequence = ['setup_folder_PSPICE', 'makeModel_ref','modifyModel_probe1','modifyModel_include_config_signals','runParsimEvent', 'run_simulation']
+        aSTEAM_1.data_analysis.AnalysisStepSequence = ['makeModel_ref', 'modifyModel_probe1',
+                                                       'modifyModel_include_config_signals', 'runParsimEvent',
+                                                       'run_simulation']
 
     aSTEAM_2 = AnalysisSTEAM()
     update_attributes_from_settings_dictionary(aSTEAM_2, settings_dictionary)
 
     if software == 'PSPICE':
         aSTEAM_2.settings.local_PSPICE_folder = local_folder
     elif software == 'XYCE':
@@ -347,37 +352,37 @@
                                                                               settings_dictionary['directory_config_files'],
                                                                             steam_circuit_type="RCD")
         signals_to_include = get_signal_keys_from_configurations_file(full_config_file_path, configuration = configuration)
     else:
         warnings.warn("no signals from the config file will be included in the model, variables entry will be empty in"
                       " the cir file, causing all signals to be calculated")
 
-    aSTEAM_2.data_analysis.AnalysisStepDefinition = {'setup_folder_PSPICE': SetUpFolder(type='SetUpFolder', simulation_name='RCD', software=[software]),
-                                                     'makeModel_ref': MakeModel(type='MakeModel', model_name='BM', file_model_data='RCD',
-                                                                                case_model='circuit', software=[software], simulation_name=None, simulation_number=None,
+    aSTEAM_2.data_analysis.AnalysisStepDefinition = {
+        'makeModel_ref': MakeModel(type='MakeModel', model_name='BM', file_model_data='RCD',
+                                                                                case_model='circuit', software=software, simulation_name=None, simulation_number=None,
                                                                                 flag_build=True, verbose=False, flag_plot_all=False, flag_json=False),
                                                      'modifyModel_probe1': ModifyModelMultipleVariables(
                                                          type='ModifyModelMultipleVariables', model_name='BM',
                                                          variables_to_change=['PostProcess.probe.probe_type'],
-                                                         variables_value=[['CSDF']], software=[software],
+                                                         variables_value=[['CSDF']], software=software,
                                                          simulation_name=None,
                                                          simulation_numbers=[]),
 
                                                      # Here I implement an additional step so that all signals (and only those) are safed in the variables
                                                      'modifyModel_include_config_signals': ModifyModelMultipleVariables(
                                                          type='ModifyModelMultipleVariables', model_name='BM',
                                                          variables_to_change=['PostProcess.probe.variables'],
-                                                         variables_value=[[signals_to_include]], software=[software],
+                                                         variables_value=[[signals_to_include]], software=software,
                                                          simulation_name=None,
                                                          simulation_numbers=[]),
 
                                                      'runParsimEvent': ParsimEvent(type='ParsimEvent', input_file=input_csv_file,
                                                                                    path_output_event_csv=path_output_parsim_sweep_RCD_csv, path_output_viewer_csv=None,
                                                                                    simulation_numbers=[file_counter], model_name='BM', case_model='circuit',
-                                                                                   simulation_name='RCD', software=[software], t_PC_off=None, rel_quench_heater_trip_threshold=None,
+                                                                                   simulation_name='RCD', software=software, t_PC_off=None, rel_quench_heater_trip_threshold=None,
                                                                                    current_polarities_CLIQ=[], dict_QH_circuits_to_QH_strips={},
                                                                                    default_keys=DefaultParsimEventKeys(local_LEDET_folder=None, path_config_file=None,
                                                                                                                        default_configs=[], path_tdms_files=None,
                                                                                                                        path_output_measurement_files=None,
                                                                                                                        path_output=local_folder),
                                                                                    path_postmortem_offline_data_folder = settings_dictionary['path_postmortem_offline_data_folder'],
                                                                                     path_to_configurations_folder = settings_dictionary['directory_config_files'],
@@ -385,17 +390,20 @@
     'run_simulation': RunSimulation(type='RunSimulation', software=software, simulation_name='RCD', simulation_numbers=[file_counter])}
     aSTEAM_2.output_path = local_folder
     if software == 'PSPICE':
         aSTEAM_2.data_analysis.PermanentSettings.local_PSPICE_folder = local_folder
     elif software == 'XYCE':
         aSTEAM_2.data_analysis.PermanentSettings.local_XYCE_folder = local_folder
     if flag_run_software == False:
-        aSTEAM_2.data_analysis.AnalysisStepSequence = ['setup_folder_PSPICE', 'makeModel_ref','modifyModel_probe1','modifyModel_include_config_signals', 'runParsimEvent']
+        aSTEAM_2.data_analysis.AnalysisStepSequence = ['makeModel_ref', 'modifyModel_probe1',
+                                                       'modifyModel_include_config_signals', 'runParsimEvent']
     else:
-        aSTEAM_2.data_analysis.AnalysisStepSequence = ['setup_folder_PSPICE', 'makeModel_ref', 'modifyModel_probe1','modifyModel_include_config_signals','runParsimEvent', 'run_simulation']
+        aSTEAM_2.data_analysis.AnalysisStepSequence = ['makeModel_ref', 'modifyModel_probe1',
+                                                       'modifyModel_include_config_signals', 'runParsimEvent',
+                                                       'run_simulation']
 
     if input_csv_file.endswith('.csv'):
         # outputfile_1 = os.path.join(os.getcwd(), 'output', 'run_parsim_event_circuit',
         #                             f'TestFile_AnalysisSTEAM_run_parsim_event_circuit_RCO_{file_counter}.yaml')
         # outputfile_2 = os.path.join(os.getcwd(), 'output', 'run_parsim_event_circuit',
         #                             f'TestFile_AnalysisSTEAM_run_parsim_event_circuit_RCD_{file_counter}.yaml')
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/analyses/AnalysisSTEAM.py` & `steam-sdk-2024.4.0/steam_sdk/analyses/AnalysisSTEAM.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 import csv
 import importlib
 import importlib.util
 import os.path
-import pathlib
 import pickle
 import re
+import shutil
 import sys
 import warnings
 from copy import deepcopy
+from pathlib import Path, PurePath
 from typing import Union, List
 
 import numpy as np
+import pandas as pd
 
 from steam_sdk.analyses.AnalysisEvent import find_IPQ_circuit_type_from_IPQ_parameters_table, \
     get_circuit_name_from_eventfile, get_circuit_family_from_circuit_name, create_two_csvs_from_odd_and_even_rows, \
     get_number_of_apertures_from_circuit_family_name, get_number_of_quenching_magnets_from_layoutdetails, \
     get_magnet_types_list, get_number_of_magnets, get_magnet_name, get_circuit_type_from_circuit_name, \
     determine_config_path_and_configuration, write_config_file_for_viewer, \
     generate_unique_event_identifier_from_eventfile
 from steam_sdk.builders.BuilderCosim import BuilderCosim
 from steam_sdk.builders.BuilderModel import BuilderModel
 from steam_sdk.cosims.CoSimPyCoSim import CosimPyCoSim
 from steam_sdk.data.DataAnalysis import DataAnalysis, ModifyModel, ModifyModelMultipleVariables, ParametricSweep, \
-    LoadCircuitParameters, WriteStimulusFile, SetUpFolder, MakeModel, ParsimEvent, DefaultParsimEventKeys, RunSimulation
+    LoadCircuitParameters, WriteStimulusFile, MakeModel, ParsimEvent, DefaultParsimEventKeys, RunSimulation
 from steam_sdk.data.DataSettings import DataSettings
+from steam_sdk.data.DataFiQuS import DataFiQuS
 from steam_sdk.drivers.DriverFiQuS import DriverFiQuS
 from steam_sdk.drivers.DriverLEDET import DriverLEDET
 from steam_sdk.drivers.DriverPSPICE import DriverPSPICE
 from steam_sdk.drivers.DriverPyBBQ import DriverPyBBQ
 from steam_sdk.drivers.DriverPySIGMA import DriverPySIGMA
 from steam_sdk.drivers.DriverXYCE import DriverXYCE
+from steam_sdk.parsers.ParserMap2d import ParserMap2dData
 from steam_sdk.parsers.ParserPSPICE import writeStimuliFromInterpolation
-from steam_sdk.parsers.ParserXYCE import *
-from steam_sdk.parsers.ParserYAML import yaml_to_data
+from steam_sdk.parsers.ParserXYCE import translate_stimulus, get_name_stimulus_folder
+from steam_sdk.parsers.ParserYAML import yaml_to_data, dict_to_yaml
 from steam_sdk.parsims.ParsimConductor import ParsimConductor
 from steam_sdk.parsims.ParsimEventCircuit import ParsimEventCircuit
 from steam_sdk.parsims.ParsimEventMagnet import ParsimEventMagnet
-from steam_sdk.plotters.PlotterMap2d import export_B_field_txt_to_map2d_SIGMA
-from steam_sdk.plotters.PlotterMap2d import generate_report_from_map2d
+from steam_sdk.plotters.PlotterMap2d import PlotterMap2d
+# from steam_sdk.plotters.PlotterFiQuSMultipole import PlotterFiQuSMultipole
 from steam_sdk.postprocs.PostprocsMetrics import PostprocsMetrics
 from steam_sdk.utils import parse_str_to_list
 from steam_sdk.utils.attribute_model import set_attribute_model, get_attribute_model
 from steam_sdk.utils.make_folder_if_not_existing import make_folder_if_not_existing
 from steam_sdk.utils.parse_str_to_list import parse_str_to_list
 from steam_sdk.utils.read_settings_file import read_settings_file
 from steam_sdk.utils.rgetattr import rgetattr
@@ -63,35 +67,36 @@
         Analysis based on STEAM_SDK
         :param file_name_analysis: full path to analysis.yaml input file  # object containing the information read from the analysis input file
         :param verbose: if true, more information is printed to the console
         """
 
         # Initialize
         self.settings = DataSettings()  # object containing the settings acquired during initialization
-        self.library_path = None
+        #self.library_path = None
         if file_path_list_models:
             with open(file_path_list_models, 'rb') as input_dict:
                 self.list_models = pickle.load(input_dict)
         else:
             self.list_models = {}  # this dictionary will be populated with BuilderModel objects and their names
 
         self.list_sims = []  # this list will be populated with integers indicating simulations to run
         self.list_viewers = {}  # this dictionary will be populated with Viewer objects and their names
         self.list_metrics = {}  # this dictionary will be populated with calculated metrics
         self.verbose = verbose
         self.summary = None  # float representing the overall outcome of a simulation for parsims
-        self.postprocess_output = None
         self.file_name_analysis = file_name_analysis
-        self.path_analysis_file = Path(self.file_name_analysis).parent  # Find folder where the input file is located, which will be used as the "anchor" for all input files
-        if isinstance(file_name_analysis, str) or isinstance(file_name_analysis, pathlib.PurePath):
+        self.simulation_numbers_source_tools = {}
+        if file_name_analysis:
+            self.path_analysis_file = str(Path(self.file_name_analysis).resolve())  # Find folder where the input file is located, which will be used as the "anchor" for all input files
+        if isinstance(file_name_analysis, str) or isinstance(file_name_analysis, PurePath):
             self.data_analysis: DataAnalysis = yaml_to_data(file_name_analysis, DataAnalysis)  # Load yaml keys into DataAnalysis dataclass
             # Read analysis settings
-            self._load_settings(self.data_analysis.GeneralParameters.relative_path_settings)
+            self._resolve_settings()
             # Read working folders and set them up
-            self._set_library_folder()
+            self._check_library_folder()
         elif file_name_analysis is None:
             self.data_analysis = DataAnalysis()
             if verbose: print('Empty AnalysisSTEAM() object generated.')
 
 
     def setAttribute(self, dataclassSTEAM, attribute: str, value):
         try:
@@ -101,62 +106,59 @@
 
     def getAttribute(self, dataclassSTEAM, attribute):
         try:
             return getattr(dataclassSTEAM, attribute)
         except:
             return getattr(getattr(self, dataclassSTEAM), attribute)
 
-    def _load_settings(self, relative_path_settings: str):
+    def _resolve_settings(self):
         """
-            ** Read analysis settings **
-            They will be read either form a local settings file (if flag_permanent_settings=False)
-            or from the keys in the input analysis file (if flag_permanent_settings=True)
-            :param relative_path_settings: only used if flag_permanent_settings=False and allows to specify folder containing settings.user_name.yaml
-            :rtype: nothing, saves temporary settings.user_name.yaml on disk
+        ** Resolves analysis settings **
+        They will be read either form a local settings file (if flag_permanent_settings=False)
+        or from the keys in the PermanentSettings input analysis file (if flag_permanent_settings=True)
+        The relative paths in the settings are replaced with absolute paths.
+        :return: Nothing, just loads appropriate settings into self. settings
+        :rtype: None
         """
-
         if self.data_analysis.GeneralParameters.flag_permanent_settings:
-            # Read settings from analysis input file (yaml file)
+            # Use settings from analysis.yaml file PermanentSettings section
             if self.verbose:
                 print('flag_permanent_settings is set to True')
-            data_settings = self.data_analysis.PermanentSettings.__dict__
+            data_settings = self.data_analysis.PermanentSettings
         else:
-            # Read settings from local settings file (yaml file)
-            path_settings, data_settings = read_settings_file(relative_path_settings=relative_path_settings, verbose=False)  # Information will be displayed later, to verbose=False here
+            # Read settings from settings.user.yaml file
             if self.verbose:
-                user_name = os.getlogin()
                 print('flag_permanent_settings is set to False')
-                print('user_name:               {}'.format(user_name))
-                print('relative_path_settings:  {}'.format(relative_path_settings))
-                print('full_path_file_settings: {}'.format(path_settings))
-
-        # Assign the keys read either from permanent-settings or local-settings
-        for name, _ in self.settings.__dict__.items():
-            if name in dict(data_settings):
-                value = dict(data_settings)[name]
-                self.setAttribute(self.settings, name, value)
-                if value:
-                    if self.verbose: print('{} : {}. Added.'.format(name, value))
-            else:
-                if self.verbose: print('{}: not found in the settings. Skipped.'.format(name))
+            relative_path_settings = self.data_analysis.GeneralParameters.relative_path_settings
+            path_settings_folder = str(Path(os.path.join(os.path.dirname(self.path_analysis_file), relative_path_settings)).resolve())
+            data_settings = read_settings_file(absolute_path_settings_folder=path_settings_folder, verbose=False)
+
+        for field_name, field_value in data_settings.dict().items():
+            if field_value:
+                if not os.path.isabs(field_value):
+                    field_value = str(Path(os.path.join(os.path.dirname(self.path_analysis_file), field_value)).resolve())
+                setattr(self.settings, field_name, field_value)
 
-    def _set_library_folder(self):
+    def _check_library_folder(self):
         """
             ** Check if model library folder is present. If not, raise an exception. **
         """
-        # Resolve the library path
-        if self.settings.local_library_path:
-            self.library_path = Path(self.settings.local_library_path).resolve()
-            if not os.path.isdir(self.library_path):
-                raise Exception(f'Defined library folder {self.library_path} does not exist. Key to change: "local_library_path" in the settings.')
-        else:
-            raise Exception(f'Library folder must be defined. Key to change: "local_library_path" in the settings.')
+        if not os.path.isdir(self.settings.local_library_path):
+            raise Exception(f'Defined library folder {self.settings.local_library_path} does not exist. Key to change: "local_library_path" in the settings.')
 
-        if self.verbose:
-            print('Model library path:    {}'.format(self.library_path))
+    #     # Resolve the library path
+    #     if self.settings.local_library_path:
+    #         self.library_path = Path(os.path.join(self.settings.local_library_path)).resolve()
+    #         if not os.path.isdir(self.library_path):
+    #             raise Exception(f'Defined library folder {self.library_path} does not exist. Key to change: "local_library_path" in the settings.')
+    #     else:
+    #         raise Exception(f'Library folder must be defined. Key to change: "local_library_path" in the settings.')
+    #
+    #     if self.verbose:
+    #         print('Model library path:    {}'.format(self.library_path))
 
     def store_model_objects(self, path_output_file: str):
         """
         ** Stores the dictionary of BuilderModel objects in a pickle file at the specified path **
         This can be helpful to load the list of models instead of generating it at every iteration of a parametric simulation or cooperative simulation
         :param path_output_file: full path of file to write
         :type path_output_file str
@@ -180,15 +182,14 @@
         :return: None
         """
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
 
         # Make sure the target folder exists
         make_folder_if_not_existing(os.path.dirname(path_output_file), verbose=verbose)
 
-        #print(self.data_analysis.PermanentSettings.PSPICE_path)
         # Write the STEAM analysis data to a yaml file
         dict_to_yaml({**self.data_analysis.dict()}, path_output_file, list_exceptions=['AnalysisStepSequence',
                                                                                        'variables_to_change'])
         if verbose: print(f'File {path_output_file} saved.')
 
     def run_analysis(self, verbose: bool = None):
         """
@@ -204,45 +205,44 @@
             print('Defined analysis steps (not in sequential order):')
             for def_step in step_definitions:
                 print(f'{def_step}')
 
         # Print analysis sequence
         if verbose: print('Defined sequence of analysis steps:')
         for s, seq_step in enumerate(self.data_analysis.AnalysisStepSequence):
-            if verbose: print('Step {}/{}: {}'.format(s + 1, len(self.data_analysis.AnalysisStepSequence), seq_step))
+            if verbose: print(f'Step {s + 1}/{len(self.data_analysis.AnalysisStepSequence)}: {seq_step}')
 
         # Run analysis (and re-print analysis steps)
         if verbose: print('Analysis started.')
         for s, seq_step in enumerate(self.data_analysis.AnalysisStepSequence):
-            if verbose: print('Step {}/{}: {}'.format(s + 1, len(self.data_analysis.AnalysisStepSequence), seq_step))
+            if verbose: print(f'Step {s + 1}/{len(self.data_analysis.AnalysisStepSequence)}: {seq_step}')
             step = step_definitions[seq_step]  # this is the object containing the information about the current step
             if step.type == 'MakeModel':
                 self.step_make_model(step, verbose=verbose)
-            elif step.type == 'ModifyModel': #
-                self.step_modify_model(step, verbose=verbose)
-            elif step.type == 'ModifyModelMultipleVariables':  #
+            elif step.type == 'ModifyModel':                self.step_modify_model(step, verbose=verbose)
+            elif step.type == 'ModifyModelMultipleVariables':
                 self.step_modify_model_multiple_variables(step, verbose=verbose)
             elif step.type == 'RunSimulation':
                 self.step_run_simulation(step, verbose=verbose)
-            elif step.type == 'PostProcess':
-                self.postprocess_output = self.step_postprocess(step, verbose=verbose)
-            elif step.type == 'SetUpFolder':
+            elif step.type == 'PostProcessCompare':
+                self.step_postprocess_compare(step, verbose=verbose)
+            elif step.type == 'SetUpFolder':  # DO NOT USE THESE STEPS ANYMORE - THEY WILL BE DELETED
                 # self.step_setup_folder(step, verbose=verbose)
                 pass  # trying to see which tests pass without this step being enabled
-            elif step.type == 'AddAuxiliaryFile':
+            elif step.type == 'AddAuxiliaryFile':  # DO NOT USE THESE STEPS ANYMORE - THEY WILL BE DELETED
                 # self.add_auxiliary_file(step, verbose=verbose)
                 pass  # trying to see which tests pass without this step being enabled
             elif step.type == 'CopyFile':
                 self.copy_file_to_target(step, verbose=verbose)
             elif step.type == 'CopyFileRelative':
                 self.copy_file_relative(step, verbose=verbose)
             elif step.type == 'RunCustomPyFunction':
                 self.run_custom_py_function(step, verbose=verbose)
             elif step.type == 'RunViewer':
-                self.run_viewer(step, verbose=verbose) # Add elif plot_map2d,  two paths save plot to folder png
+                self.run_viewer(step, verbose=verbose)  # Add elif plot_map2d,  two paths save plot to folder png
             elif step.type == 'CalculateMetrics':
                 self.calculate_metrics(step, verbose=verbose)
             elif step.type == 'LoadCircuitParameters':
                 self.load_circuit_parameters(step, verbose=verbose)
             elif step.type == 'WriteStimulusFile':
                 self.write_stimuli_from_interpolation(step, verbose=verbose)
             elif step.type == 'ParsimEvent':
@@ -255,22 +255,21 @@
                 raise Exception('Unknown type of analysis step: {}'.format(step.type))
 
     def step_make_model(self, step, verbose: bool = None):
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
         if verbose:
             print('Making model object named {}'.format(str(step.model_name)))
         # Always assume the STEAM models folder structure, which contains subfolders "circuits", "conductors", "cosims", "magnets"
-        file_model_data = os.path.join(self.library_path, f'{step.case_model}s', step.file_model_data, 'input', f'modelData_{step.file_model_data}.yaml')
+        file_model_data = os.path.join(self.settings.local_library_path, f'{step.case_model}s', step.file_model_data, 'input', f'modelData_{step.file_model_data}.yaml')
 
         # Build the model
         if step.case_model == 'cosim':
             BM = BuilderCosim(file_model_data=file_model_data, data_settings=self.settings, verbose=step.verbose)
         else:
-            BM = BuilderModel(file_model_data=file_model_data, case_model=step.case_model, data_settings=self.settings,
-                              results_folder_name='output', verbose=step.verbose)
+            BM = BuilderModel(file_model_data=file_model_data, case_model=step.case_model, data_settings=self.settings, verbose=step.verbose)
 
         # Build simulation file (Call the model builder of the selected tools)
         if step.simulation_number is not None:
             BM = self.setup_sim(BM=BM, step=step, sim_number=step.simulation_number, verbose=step.verbose)
 
         # Add the reference to the model in the dictionary
         self.list_models[step.model_name] = BM
@@ -300,18 +299,19 @@
                 step.model_name]  # original BuilderModel or BuilderCosim object
             case_model = BM.case_model  # model case (magnet, conductor, circuit, cosim)
 
             if 'Conductors[' in step.variable_to_change:  # Special case when the variable to change is the Conductors key
                 if verbose:
                     idx_conductor = int(step.variable_to_change.split('Conductors[')[1].split(']')[0])
                     conductor_variable_to_change = step.variable_to_change.split('].')[1]
-                    print(f'Variable {step.variable_to_change} is treated as a Conductors key. Conductor index: #{idx_conductor}. Conductor variable to change: {conductor_variable_to_change}.')
+                    print(f'Variable {step.variable_to_change} is treated as a Conductors key. Conductor index: #{idx_conductor}. '
+                          f'Conductor variable to change: {conductor_variable_to_change}.')
 
                     old_value = get_attribute_model(case_model, BM, conductor_variable_to_change, idx_conductor)
-                    print('Variable {} changed from {} to {}.'.format(conductor_variable_to_change, old_value, value))
+                    print(f'Variable {conductor_variable_to_change} changed from {old_value} to {value}.')
 
                 if len_new_model_name > 0:  # Make a new copy of the BuilderModel object, and change it
                     self.list_models[step.new_model_name[v]] = deepcopy(BM)
                     BM = self.list_models[step.new_model_name[v]]
 
                     if case_model == 'conductor':
                         rsetattr(BM.conductor_data.Conductors[idx_conductor], conductor_variable_to_change, value)
@@ -345,14 +345,15 @@
             if step.variable_to_change.startswith('Sources.'):
                 BM.set_input_paths()
 
             # Build simulation file
             if len_simulation_numbers > 0:
                 # Set paths of input files
                 BM.set_input_paths()
+                self.simulation_numbers_source_tools[step.simulation_numbers[v]] = step.software
                 BM = self.setup_sim(BM=BM, step=step, sim_number=step.simulation_numbers[v], verbose=step.verbose)
 
     def step_modify_model_multiple_variables(self, step, verbose: bool = None):
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
         if verbose:
             print('Modifying model object named {}'.format(str(step.model_name)))
 
@@ -416,113 +417,100 @@
 
         for sim_name, sim_number in zip(sim_names, sim_numbers):
             if verbose:
                 print('Running simulation of model {} #{} using {}.'.format(simulation_name, sim_number, software))
             # Run simulation
             self.run_sim(software, sim_name, sim_number, simFileType, verbose)
 
-    def step_postprocess(self, step, verbose: bool = None):  # run sequence variable
+    def step_postprocess_compare(self, step, verbose: bool = None):
         """
-        The postprocessing method is for comparing map2d files between FiQuS, SIGMA and ROXIE. It generates 5 difference plots:
-        1) Absolute Bmod difference.
-        2) Difference in Bx and By
-        3) Bx and By
-        4) Bmod
-        5) relative error in Bx and By
+        The postprocessing method is for comparing results between two solutions: e.g., map2d files between FiQuS and SIGMA
+        Supported physical quantities: magnetic_flux_density,
         :param step:
         :param verbose:
         :return:
         """
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
-        if verbose: print('postprocessing')
-        map2d_to_compare = dict()
+        if verbose: print('PostProcessing for comparisons.')
+        new_file_names = {}
 
-        if step.sources:
-            # For now, only two sources can be compared at the same time.
-            if len(step.sources) != 2:
-                raise ValueError("For now it's only supported to compare two map2d files. Change sources in your yaml file.")
-
-            # Unwrap numbers per source
-            for source, source_sim_nbr, fiqus_csv_idx in zip(step.sources, step.sources_sim_nrs, step.sources_FiQuS_csv_idx):
-                source_sim_nbr = source_sim_nbr[0]
-
-                if source.lower() == 'sigma':
-                    if len(fiqus_csv_idx) > 0:
-                        fiqus_csv_idx = fiqus_csv_idx[0]
-                        if fiqus_csv_idx is not None:
-                            warnings.warn(
-                                f"Fiqus csv index is set to other than None for {source}. Observe this is only applicable to FiQuS")
-                    # Check if files exist from SIGMA simulation
-                    local_SIGMA_folder = self._get_local_folder('local_SIGMA_folder')
-                    path_result_txt_Bx = os.path.join(local_SIGMA_folder, f"{step.simulation_name}_{source_sim_nbr}", "output", "mf.Bx.txt")
-                    path_result_txt_By = os.path.join(local_SIGMA_folder, f"{step.simulation_name}_{source_sim_nbr}", "output", "mf.By.txt")
-                    path_new_file = os.path.join(local_SIGMA_folder, f"{step.simulation_name}_{source_sim_nbr}", "output", "B_field_map2d.map2d")
-                    path_reference_roxie = os.path.join(local_SIGMA_folder, f"{step.simulation_name}_{source_sim_nbr}", f"{step.simulation_name}_ROXIE_REFERENCE.map2d")
-
-                    if not os.path.exists(path_result_txt_Bx):
-                        raise Warning(f"No Bx file is found: {path_result_txt_Bx}, please check that simulation ran successfully.")
-                    elif not os.path.exists(path_result_txt_By):
-                        raise Warning(f"No By file is found: {path_result_txt_By}, please check that simulation ran successfully.")
-                    elif not os.path.exists(path_reference_roxie):
-                        print(path_reference_roxie)
-                        raise Warning(f"No Roxie reference file is found: {path_reference_roxie}, please check model_data.yaml in options_sigma that key map2d is specified.")
-                    else:
-                        # Export results to map2d file
-                        try:
-                            export_B_field_txt_to_map2d_SIGMA(path_reference_roxie, path_result_txt_Bx, path_result_txt_By, path_new_file)
-                        except:
-                            print(f"Can't generate map2d output. This can only be done for stationary studies and with the same coordinate in output files and roxie reference")
-
-                elif source.lower() == 'fiqus':
-                    fiqus_csv_idx = fiqus_csv_idx[0]
-                    # Take latest run by reading file.
-                    local_FiQuS_folder = self._get_local_folder('local_FiQuS_folder')
-                    path_log = os.path.join(local_FiQuS_folder, step.simulation_name, f"{step.simulation_name}_{source_sim_nbr}", "csv_run_log.csv")
-                    with open(path_log, 'r', newline='') as csv_file:
-                        reader = csv.reader(csv_file)
-                        rows = list(reader)
-
-                    flattened_rows = [value for sublist in rows for value in sublist]
-                    if fiqus_csv_idx is not None:
-                    # Retrieve the last value from the flattened list
-                        last_line_value = flattened_rows[fiqus_csv_idx]
-                    # If fiqus_csv_idx is None, take latest index
-                    else:
-                        last_line_value = flattened_rows[-1]
-                    path_new_file = os.path.join(last_line_value, step.simulation_name+".map2d")
-                    if not os.path.exists(path_new_file):
-                        raise Warning(f"Output FiQuS file in the location {path_new_file} is not present.")
-
-                elif source.lower() == 'roxie':
-                    # Take latest run by reading file.
-                    if len(fiqus_csv_idx) > 0:
-                        fiqus_csv_idx = fiqus_csv_idx[0]
-                        if fiqus_csv_idx is not None:
-                            warnings.warn(
-                                f"Fiqus csv index is set to other than None for {source}. Observe this is only applicable to FiQuS")
-                    path_new_file = os.path.join(self.library_path, 'magnets', step.simulation_name, 'input',
-                                                 step.simulation_name + ".map2d")
-
-                else:
-                    raise ValueError("Invalid source name.")
+        # Initialize parser object with reference map2d file
+        if step.physical_quantity == 'magnetic_flux_density':
+            ref_map2d = os.path.join(self.settings.local_library_path, 'magnets', step.simulation_name, 'input', step.simulation_name + ".map2d")
+            parser_obj = ParserMap2dData(map2d_input=Path(ref_map2d), output_folder_path=Path(step.path_to_saved_files),
+                                         physical_quantity='magnetic_flux_density')
+
+        def get_solution_folder_path_FiQuS(sim_nbr):
+            path_to_output = os.path.join(self.settings.local_FiQuS_folder, step.simulation_name)
+            path_yaml = os.path.join(path_to_output, f"{step.simulation_name}_{sim_nbr}_FiQuS.yaml")
+            fdm: DataFiQuS = yaml_to_data(path_yaml, DataFiQuS)
+            g_folder = fdm.run.geometry if fdm.run.geometry is not None else '1'
+            m_folder = fdm.run.mesh if fdm.run.mesh is not None else '1'
+            s_folder = fdm.run.solution if fdm.run.solution is not None else '1'
+            return os.path.join(path_to_output, f'Geometry_{g_folder}', f'Mesh_{m_folder}', f'Solution_{s_folder}')
+
+        def check_if_SIGMA_files_exist(sim_nbr):
+            path_result_txt_Bx = os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_nbr}", "output", "mf.Bx.txt")
+            path_result_txt_By = os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_nbr}", "output", "mf.By.txt")
+            if not os.path.exists(path_result_txt_Bx):
+                raise Warning(f"No Bx file is found: {path_result_txt_Bx}, please check that simulation ran successfully.")
+            elif not os.path.exists(path_result_txt_By):
+                raise Warning(f"No By file is found: {path_result_txt_By}, please check that simulation ran successfully.")
+
+        def create_map2d_files():
+            if self.simulation_numbers_source_tools[source_sim_nbr].lower() == 'sigma':
+                check_if_SIGMA_files_exist(sim_nbr=source_sim_nbr)
+                parser_obj.create_map2d_file_from_SIGMA(
+                    results_path=Path(os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{source_sim_nbr}", "output")),
+                    new_file_name=new_file_names[results_name], check_coordinates=True)
+            elif self.simulation_numbers_source_tools[source_sim_nbr].lower() == 'fiqus':
+                parser_obj.create_map2d_file_from_FiQuS(
+                    results_path=Path(os.path.join(get_solution_folder_path_FiQuS(sim_nbr=source_sim_nbr), step.simulation_name + ".map2d")),
+                    new_file_name=new_file_names[results_name])
+            else:
+                raise ValueError("Source tool not yet supported for post-process comparison.")
 
-                map2d_to_compare[source] = path_new_file
+        if isinstance(step.simulation_numbers, int) and step.physical_quantity != 'magnetic_flux_density':
+            raise ValueError("Comparison with ROXIE is only supported for the magnetic flux density.")
 
-            keys_list = list(map2d_to_compare.keys())
-            key1 = keys_list[0]
-            key2 = keys_list[1]
-            value1 = map2d_to_compare[key1]
-            value2 = map2d_to_compare[key2]
-            prefix = f"{step.simulation_name}"
-            exported_stats = generate_report_from_map2d(prefix, step.path_to_saved_files,
-                                                        value1, key1, value2, key2, "coil", save=True)
-            return exported_stats
+        elif isinstance(step.simulation_numbers, int) and step.physical_quantity == 'magnetic_flux_density':
+            source_sim_nbr = step.simulation_numbers
+            results_name = self.simulation_numbers_source_tools[source_sim_nbr] + '_' + str(source_sim_nbr)
+            new_file_names[results_name] = results_name + '.map2d'
+            create_map2d_files()
+
+            # Copy ROXIE reference file
+            shutil.copy(ref_map2d, step.path_to_saved_files)
+
+            PlotterMap2d(parsed_results_path=Path(step.path_to_saved_files)).generate_report_from_map2d(
+                comparison_name=step.simulation_name, file_names=new_file_names, plot_type="coil")
+
+        elif isinstance(step.simulation_numbers, tuple) and step.physical_quantity == 'magnetic_flux_density':
+            for source_sim_nbr in step.simulation_numbers:
+                results_name = self.simulation_numbers_source_tools[source_sim_nbr] + '_' + str(source_sim_nbr)
+                new_file_names[results_name] = results_name + '.map2d'
+                create_map2d_files()
+            PlotterMap2d(parsed_results_path=Path(step.path_to_saved_files)).generate_report_from_map2d(
+                comparison_name=step.simulation_name, file_names=new_file_names, plot_type="coil")
 
-        else:
-            return None
+        elif isinstance(step.simulation_numbers, tuple) and step.physical_quantity == 'temperature':
+            pass
+            # fiqus_solution_folders = {}
+            # for source_sim_nbr in step.simulation_numbers:
+            #     if self.simulation_numbers_source_tools[source_sim_nbr].lower() == 'fiqus':
+            #         results_name = self.simulation_numbers_source_tools[source_sim_nbr] + '_' + str(source_sim_nbr)
+            #         results_paths[results_name] = os.path.join(get_solution_folder_path_FiQuS(sim_nbr=source_sim_nbr))
+            #         fiqus_solution_folders.update({str(source_sim_nbr): results_paths[results_name]})
+            #     else:
+            #         raise ValueError("Source tool not yet supported for post-process comparison.")
+            #
+            # if all([self.simulation_numbers_source_tools[source_sim_nbr].lower() == 'fiqus' for source_sim_nbr in step.simulation_numbers]):
+            #     plot_object = PlotterFiQuSMultipole(solution_folders_paths=fiqus_solution_folders,
+            #                                         physical_quantity_to_initialize_per_solution={sim_nbr: step.physical_quantity for sim_nbr in fiqus_solution_folders.keys()})
+            #     plot_object.plot_time_figure(solution='1', physical_quantity=step.physical_quantity, half_turns=[229, 230, 231])
 
     # def step_setup_folder(self, step, verbose: bool = None):
     #     """
     #     Set up simulation working folder.
     #     The function applies a different logic for each simulation software.
     #     """
     #     verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
@@ -673,29 +661,30 @@
         """
             Copy one file from a location to another (the destination folder can be different from the analysis output folder)
         """
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
 
         def get_full_path(obj):
             paths_out = []
-            for local_tool_folder, simulation_name, remaining_path in zip(obj.local_tool_folders, obj.simulation_names, obj.reminder_paths):
-                if not hasattr(self.data_analysis.PermanentSettings, local_tool_folder):
-                    raise Exception(f'Key {local_tool_folder} is not found in the analysis permanent settings.')
-                if self.data_analysis.GeneralParameters.flag_permanent_settings:
-                    abs_tool_path = self.data_analysis.PermanentSettings.__dict__[local_tool_folder]
-                else:
-                    abs_tool_path = self.settings.__dict__[local_tool_folder]
+            for local_tool_folder, simulation_name, remaining_path in zip(obj.local_tool_folders, obj.simulation_names, obj.remainder_paths):
+                # if not hasattr(self.data_analysis.PermanentSettings, local_tool_folder):
+                #     raise Exception(f'Key {local_tool_folder} is not found in the analysis permanent settings.')
+                # if self.data_analysis.GeneralParameters.flag_permanent_settings:
+                #     abs_tool_path = self.data_analysis.PermanentSettings.__dict__[local_tool_folder]
+                # else:
+                #     abs_tool_path = self.settings.__dict__[local_tool_folder]
+                abs_tool_path = getattr(self.settings, local_tool_folder)
                 if local_tool_folder == 'local_library_path':
                     abs_tool_path = os.path.join(abs_tool_path, f"{self.data_analysis.AnalysisStepDefinition['makeModel'].case_model}s")
-                paths_out.append(str(Path(os.path.join(os.getcwd(), abs_tool_path, simulation_name, remaining_path)).resolve()))
+                paths_out.append(str(Path(os.path.join(abs_tool_path, simulation_name, remaining_path)).resolve()))
             return paths_out
 
         for full_path_file_to_copy, full_path_file_target in zip(get_full_path(step.copy_from), get_full_path(step.copy_to)):
-            print(f'Coping from: {full_path_file_to_copy}')
-            print(f'Coping to: {full_path_file_target}')
+            print(f'Copying from: {full_path_file_to_copy}')
+            print(f'Copying to: {full_path_file_target}')
             # Make sure the target folder exists
             make_folder_if_not_existing(os.path.dirname(full_path_file_target), verbose=verbose)
 
             # Copy file
             try:
                 shutil.copyfile(full_path_file_to_copy, full_path_file_target)
             except shutil.SameFileError:
@@ -911,17 +900,24 @@
         ## return a summary across all signals, across all keys in the metrics --> this is needed for Dakota
         list_metric_values = []
         # calculate mean value across all values in the metrics:
         for event_label, metrics_for_a_event_label in current_list_output_metrics.items():
             for var_to_analyze, metrics_for_a_var_to_analyze in  current_list_output_metrics[event_label].items():
                 # this should be a list across all metrics to calculate:
                 list_metric_values.extend(metrics_for_a_var_to_analyze)
-        software = "PSPICE" #TODO: add software here as a key for a dict, that is passed
-        self.summary =np.mean(list_metric_values)
-        ################################################################################################################
+
+        # Write metrics to a yaml file at a specified path for easier postprocessing if needed
+        if step.metrics_output_filepath and self.list_metrics:
+            data_to_write = self.list_metrics
+            #assert(data == self.list_metrics)
+            dict_to_yaml(data_dict=data_to_write,name_output_file=step.metrics_output_filepath)
+
+        self.summary = {}
+        self.summary['dummy_value'] = np.mean(list_metric_values)
+        ############################################################################# ###################################
 
         return current_list_output_metrics
 
     def load_circuit_parameters(self, step, verbose: bool = None):
         """
         Load global circuit parameters from a .csv file into an existing BuilderModel circuit model
         :param step: STEAM analysis step of type LoadCircuitParameters, which has attributes:
@@ -958,20 +954,20 @@
 
         if step.software == 'COSIM':
             BM = self.setup_sim_COSIM(BM=BM, simulation_name=step.simulation_name, sim_number=sim_number, verbose=verbose)
         elif step.software == 'FiQuS':
             BM = self.setup_sim_FiQuS(BM=BM, simulation_name=step.simulation_name, sim_number=sim_number, verbose=verbose)
         elif step.software == 'LEDET':
             BM = self.setup_sim_LEDET(BM=BM, simulation_name=step.simulation_name, sim_number=sim_number,
-                                      flag_json=step.flag_json, flag_plot_all=step.flag_plot_all, verbose=verbose)
+                                 flag_json=step.flag_json, flag_plot_all=step.flag_plot_all, verbose=verbose)
         elif step.software == 'PSPICE':
             BM = self.setup_sim_PSPICE(BM=BM, simulation_name=step.simulation_name, sim_number=sim_number, verbose=verbose)
         elif step.software == 'SIGMA':
             BM = self.setup_sim_SIGMA(BM=BM, simulation_name=step.simulation_name, sim_number=sim_number,
-                                      flag_plot_all=step.flag_plot_all, verbose=verbose)
+                                 flag_plot_all=step.flag_plot_all, verbose=verbose)
         elif step.software == 'PyBBQ':
             BM = self.setup_sim_PyBBQ(BM=BM, simulation_name=step.simulation_name, sim_number=sim_number, verbose=verbose)
         elif step.software == 'PyCoSim':
             BM = self.setup_sim_PyCoSim(BM=BM, simulation_name=step.simulation_name, sim_number=sim_number, verbose=verbose)
         elif step.software == 'XYCE':
             BM = self.setup_sim_XYCE(BM=BM, simulation_name=step.simulation_name, sim_number=sim_number, verbose=verbose)
         return BM
@@ -979,15 +975,15 @@
     def setup_sim_COSIM(self, BM: BuilderCosim, simulation_name, sim_number, verbose: bool = None):
         """
         Set up a COSIM model in the local COSIM working folder
         Note: The sim_number is assigned to the subfolder name, not to the file name
         """
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
 
-        local_COSIM_folder = self._get_local_folder('local_COSIM_folder')
+        local_COSIM_folder = self.settings.local_COSIM_folder
         local_model_folder = os.path.join(local_COSIM_folder, simulation_name)
         BM.buildCOSIM(sim_name=simulation_name, sim_number=sim_number, output_path=local_model_folder, verbose=verbose)
 
         # Add simulation number to the list
         self.list_sims.append(sim_number)
 
         return BM
@@ -996,21 +992,21 @@
         """
         Set up a FiQuS simulation by copying the last file generated by BuilderModel to the output folder and to the
         local FiQuS working folder.
         The original file is then deleted.
         """
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
 
-        local_FiQuS_folder = self._get_local_folder('local_FiQuS_folder')
-        BM.buildFiQuS(sim_name=simulation_name, sim_number=sim_number, output_path=os.path.join(local_FiQuS_folder, simulation_name),
-                      flag_plot_all=flag_plot_all, verbose=verbose)
+        #local_FiQuS_folder = self._get_local_folder('local_FiQuS_folder')
+        output_path = os.path.join(self.settings.local_FiQuS_folder, simulation_name)
+        BM.buildFiQuS(sim_name=simulation_name, sim_number=sim_number, output_path=output_path, flag_plot_all=flag_plot_all, verbose=verbose)
 
         # Make simulation folder
         #local_model_folder = os.path.join(self.settings.local_FiQuS_folder, simulation_name, f'{simulation_name}_{str(sim_number)}')
-        local_model_folder = os.path.join(local_FiQuS_folder, simulation_name)
+        local_model_folder = os.path.join(self.settings.local_FiQuS_folder, simulation_name)
         make_folder_if_not_existing(local_model_folder)
         sources_folder = os.path.join(local_model_folder, 'sources')
         make_folder_if_not_existing(sources_folder)
         output_folder = os.path.join(local_model_folder, 'output')
         make_folder_if_not_existing(output_folder)
         # If we have a roxie_reference file copy across
         file_name = f"{simulation_name}_{sim_number}_ROXIE_REFERENCE.map2d"
@@ -1057,22 +1053,21 @@
         Set up a LEDET simulation by copying the last file generated by BuilderModel to the output folder and to the
         local LEDET working folder. The original file is then deleted.
         If flag_yaml=True, the model is set up to be run using a yaml input file.
         If flag_json=True, the model is set up to be run using a json input file.
         """
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
 
-        local_LEDET_folder = self._get_local_folder('local_LEDET_folder')
-        local_model_folder = str(Path(local_LEDET_folder / simulation_name / 'Input').resolve())
-        field_maps_folder = Path(local_LEDET_folder / '..' / 'Field maps' / simulation_name).resolve()  # The map2d files are written in a subfolder {simulation_name} inside a folder "Field maps" at the same level as the LEDET folder [this structure is hard-coded in STEAM-LEDET]
-
-        make_folder_if_not_existing(Path(local_LEDET_folder / simulation_name / 'Input').resolve(), verbose=verbose)
-        make_folder_if_not_existing(Path(local_LEDET_folder / simulation_name / 'Input' / 'Control current input').resolve(), verbose=verbose)
-        make_folder_if_not_existing(Path(local_LEDET_folder / simulation_name / 'Input' / 'Initialize variables').resolve(), verbose=verbose)
-        make_folder_if_not_existing(Path(local_LEDET_folder / simulation_name / 'Input' / 'InitializationFiles').resolve(), verbose=verbose)
+        local_model_folder = str(Path(os.path.join(self.settings.local_LEDET_folder, simulation_name, 'Input')).resolve())
+        field_maps_folder = Path(os.path.join(self.settings.local_LEDET_folder, '..', 'Field maps', simulation_name)).resolve()  # The map2d files are written in a subfolder {simulation_name} inside a folder "Field maps" at the same level as the LEDET folder [this structure is hard-coded in STEAM-LEDET]
+
+        make_folder_if_not_existing(Path(os.path.join(self.settings.local_LEDET_folder, simulation_name, 'Input')).resolve(), verbose=verbose)
+        make_folder_if_not_existing(Path(os.path.join(self.settings.local_LEDET_folder, simulation_name, 'Input', 'Control current input')).resolve(), verbose=verbose)
+        make_folder_if_not_existing(Path(os.path.join(self.settings.local_LEDET_folder, simulation_name, 'Input', 'Initialize variables')).resolve(), verbose=verbose)
+        make_folder_if_not_existing(Path(os.path.join(self.settings.local_LEDET_folder, simulation_name, 'Input', 'InitializationFiles')).resolve(), verbose=verbose)
 
         BM.buildLEDET(sim_name=simulation_name, sim_number=sim_number,
                       output_path=local_model_folder, output_path_field_maps=field_maps_folder,
                       flag_json=flag_json, flag_plot_all=flag_plot_all, verbose=verbose)
 
         # Add simulation number to the list
         self.list_sims.append(sim_number)
@@ -1083,33 +1078,33 @@
         """
         Set up a PSPICE simulation in the local PSPICE working folder
         Note: The sim_number is assigned to the subfolder name, not to the file name
         """
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
 
         # Write PSPICE netlist
-        local_PSPICE_folder = self._get_local_folder('local_PSPICE_folder')
+        #local_PSPICE_folder = self._get_local_folder('local_PSPICE_folder')
 
-        local_model_folder = os.path.join(local_PSPICE_folder, simulation_name, str(sim_number))
+        local_model_folder = os.path.join(self.settings.local_PSPICE_folder, simulation_name, str(sim_number))
         BM.buildPSPICE(sim_name=simulation_name, sim_number='', output_path=local_model_folder, verbose=verbose)
 
         # Add simulation number to the list
         self.list_sims.append(sim_number)
 
         return BM
 
     def setup_sim_PyCoSim(self, BM: BuilderCosim, simulation_name, sim_number, verbose: bool = None):
         """
         Set up a PyCoSim model in the local PyCoSim working folder
         Note: The sim_number is assigned to the subfolder name, not to the file name
         """
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
 
-        local_PyCoSim_folder = self._get_local_folder('local_PyCoSim_folder')
-        local_model_folder = os.path.join(local_PyCoSim_folder, simulation_name, 'input')  # TODO TO DISCUSS: MW dislikes 'input', ER likes it
+        #local_PyCoSim_folder = self._get_local_folder('local_PyCoSim_folder')
+        local_model_folder = os.path.join(self.settings.local_PyCoSim_folder, simulation_name, 'input')  # TODO TO DISCUSS: MW dislikes 'input', ER likes it
         BM.buildPyCoSim(sim_name=simulation_name, sim_number=sim_number, output_path=local_model_folder, verbose=verbose)
 
         # Add simulation number to the list
         self.list_sims.append(sim_number)
 
         return BM
 
@@ -1118,18 +1113,18 @@
         """
         Set up a SIGMA simulation by copying the last file generated by BuilderModel to the output folder and to the
         local SIGMA working folder.
         The original file is then deleted.
         """
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
 
-        local_SIGMA_folder = self._get_local_folder('local_SIGMA_folder')
-        local_model_folder = str(Path(local_SIGMA_folder / simulation_name / 'Input').resolve())
+        #local_SIGMA_folder = self._get_local_folder('local_SIGMA_folder')
+        output_path = str(Path(os.path.join(self.settings.local_SIGMA_folder, simulation_name, str(sim_number))).resolve())
         BM.buildPySIGMA(sim_name=simulation_name, sim_number=sim_number,
-                        output_path=local_model_folder,
+                        output_path=output_path,
                         flag_plot_all=flag_plot_all,
                         verbose=verbose)
 
         # Add simulation number to the list
         self.list_sims.append(sim_number)
 
         return BM
@@ -1140,121 +1135,85 @@
         local PSPICE working folder.
         The simulation netlist and auxiliary files are copied in a new numbered subfoldered.
         The original file is then deleted.
         """
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
 
         # Unpack
-        local_XYCE_folder = self._get_local_folder('local_XYCE_folder')
-        local_model_folder = os.path.join(local_XYCE_folder, simulation_name, str(sim_number))
+        #local_XYCE_folder = self._get_local_folder('local_XYCE_folder')
+        local_model_folder = os.path.join(self.settings.local_XYCE_folder, simulation_name, str(sim_number))
         BM.buildXYCE(sim_name=simulation_name, sim_number='', output_path=local_model_folder, verbose=verbose)
 
         # Add simulation number to the list
         self.list_sims.append(sim_number)
 
-        # Edit simulation file
-        file_name_local = os.path.join(local_model_folder, simulation_name + '.cir')
-        self.copy_XYCE_cir(file_name_local, file_name_local)
-        if verbose: print(f'Simulation file {file_name_local} edited.')
-
         return BM
 
-    def copy_XYCE_cir(self, file_name_temp, file_name_local):
-        '''
-            Function that copies the XYCE circuit file from 'file_name_temp' to 'file_name_local' and changes the
-            respective output path for the csd
-        :param file_name_temp: Original circuit file
-        :param file_name_local: Final circuit file
-        :return:
-        '''
-
-        with open(file_name_temp) as f:
-            contents = f.readlines()
-        for k in range(len(contents)):
-            if contents[k].casefold().startswith('.print'):
-                if 'csd' in contents[k]:
-                    type_output = 'csd'
-                elif 'csv' in contents[k]:
-                    type_output = 'csv'
-                elif 'txt' in contents[k]:
-                    type_output = 'txt'
-                else:
-                    raise Exception("Don't understand output type.")
-                print_line = contents[k].split('FILE=')
-                print_line[-1] = f'FILE={file_name_local[:-4]}.{type_output} \n'
-                contents[k] = ''.join(print_line)
-                break
-
-        contents = ''.join(contents)
-        new_file = open(file_name_local, 'w')
-        new_file.write(contents)
-        new_file.close()
-
     def setup_sim_PyBBQ(self, BM: BuilderModel, simulation_name, sim_number, verbose: bool = None):
         """
         Set up a PyBBQ simulation in the local PyBBQ working folder
         Note: The sim_number is assigned to the subfolder name, not to the file name
         """
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
 
-        local_PyBBQ_folder = self._get_local_folder('local_PyBBQ_folder')
-        local_model_folder = os.path.join(local_PyBBQ_folder, simulation_name, str(sim_number))
+        #local_PyBBQ_folder = self._get_local_folder('local_PyBBQ_folder')
+        local_model_folder = os.path.join(self.settings.local_PyBBQ_folder, simulation_name, str(sim_number))
         BM.buildPyBBQ(sim_name=simulation_name, sim_number='', output_path=local_model_folder, verbose=verbose)
 
         # Add simulation number to the list
         self.list_sims.append(sim_number)
 
         return BM
 
     def run_sim(self, software: str, simulation_name: str, sim_number: int, simFileType: str = None,
                 verbose: bool = False):
         """
         Run selected simulation.
         The function applies a different logic for each simulation software.
         """
         if software == 'FiQuS':
-            local_FiQuS_folder = self._get_local_folder('local_FiQuS_folder')
+            #local_FiQuS_folder = self._get_local_folder('local_FiQuS_folder')
             #local_analysis_folder = simulation_name + '_' + str(sim_number)
+            path_folder_FiQuS = os.path.join(self.settings.local_FiQuS_folder, simulation_name)
             dFiQuS = DriverFiQuS(FiQuS_path=self.settings.FiQuS_path,
-                                 path_folder_FiQuS_output=os.path.join(local_FiQuS_folder, simulation_name),
-                                 path_folder_FiQuS_input=os.path.join(local_FiQuS_folder, simulation_name), verbose=verbose,
-                                 GetDP_path=self.settings.GetDP_path)
+                                 path_folder_FiQuS_output=path_folder_FiQuS, path_folder_FiQuS_input=path_folder_FiQuS,
+                                 verbose=verbose, GetDP_path=self.settings.GetDP_path)
             self.summary = dFiQuS.run_FiQuS(sim_file_name=simulation_name + '_' + str(sim_number) + '_FiQuS', return_summary=False)
         elif software == 'LEDET':
-            local_LEDET_folder = self._get_local_folder('local_LEDET_folder')
-            dLEDET = DriverLEDET(path_exe=self.settings.LEDET_path, path_folder_LEDET=local_LEDET_folder, verbose=verbose)
+            #local_LEDET_folder = self._get_local_folder('local_LEDET_folder')
+            dLEDET = DriverLEDET(path_exe=self.settings.LEDET_path, path_folder_LEDET=self.settings.local_LEDET_folder, verbose=verbose)
             self.summary = dLEDET.run_LEDET(simulation_name, str(sim_number), simFileType=simFileType)
         elif software == 'PSPICE':
-            local_PSPICE_folder = self._get_local_folder('local_PSPICE_folder')
-            local_model_folder = Path(local_PSPICE_folder / simulation_name / str(sim_number)).resolve()
+            #local_PSPICE_folder = self._get_local_folder('local_PSPICE_folder')
+            local_model_folder = Path(os.path.join(self.settings.local_PSPICE_folder, simulation_name, str(sim_number))).resolve()
             dPSPICE = DriverPSPICE(path_exe=self.settings.PSPICE_path, path_folder_PSPICE=local_model_folder, verbose=verbose)
             dPSPICE.run_PSPICE(simulation_name, suffix='')
         elif software == 'PyBBQ':
-            local_PyBBQ_folder = self._get_local_folder('local_PyBBQ_folder')
-            local_model_folder_input = os.path.join(local_PyBBQ_folder, simulation_name, str(sim_number))
+            #local_PyBBQ_folder = self._get_local_folder('local_PyBBQ_folder')
+            local_model_folder_input = os.path.join(self.settings.local_PyBBQ_folder, simulation_name, str(sim_number))
             relative_folder_output = os.path.join(simulation_name, str(sim_number))
-            dPyBBQ = DriverPyBBQ(path_exe=self.settings.PyBBQ_path, path_folder_PyBBQ=local_PyBBQ_folder,
+            dPyBBQ = DriverPyBBQ(path_exe=self.settings.PyBBQ_path, path_folder_PyBBQ=self.settings.local_PyBBQ_folder,
                                  path_folder_PyBBQ_input=local_model_folder_input, verbose=verbose)
             dPyBBQ.run_PyBBQ(simulation_name, outputDirectory=relative_folder_output)
         elif software == 'PyCoSim':
-            local_PyCoSim_folder = self._get_local_folder('local_PyCoSim_folder')
-            local_model_folder = os.path.join(local_PyCoSim_folder, simulation_name, 'input')  # TODO TO DISCUSS: MW dislikes 'input', ER likes it
+            #local_PyCoSim_folder = self._get_local_folder('local_PyCoSim_folder')
+            local_model_folder = os.path.join(self.settings.local_PyCoSim_folder, simulation_name, 'input')  # TODO TO DISCUSS: MW dislikes 'input', ER likes it
             pass
             # TODO find a sensible logic for running PyCoSim inside a STEAM analysis: This will be done by calling CosimPyCoSim here
             # path_cosim_data =
             # pyCOSIM = CosimPyCoSim(file_model_data=path_cosim_data, data_settings=self.settings, verbose=verbose)
             # pyCOSIM.run()
         elif software == 'SIGMA':
-            local_SIGMA_folder = self._get_local_folder('local_SIGMA_folder')
-            local_analysis_folder = os.path.join(local_SIGMA_folder, simulation_name, f'{sim_number}')  # TODO note simulation_name was added
+            #local_SIGMA_folder = self._get_local_folder('local_SIGMA_folder')
+            local_analysis_folder = os.path.join(self.settings.local_SIGMA_folder, simulation_name, f'{sim_number}')  # TODO note simulation_name was added
             ds = DriverPySIGMA(path_input_folder=local_analysis_folder)
             ds.run_PySIGMA(simulation_name)
         elif software == 'XYCE':
-            local_XYCE_folder = self._get_local_folder('local_XYCE_folder')
-            local_model_folder = Path(local_XYCE_folder / simulation_name / str(sim_number)).resolve()
+            #local_XYCE_folder = self._get_local_folder('local_XYCE_folder')
+            local_model_folder = Path(os.path.join(self.settings.local_XYCE_folder, simulation_name, str(sim_number))).resolve()
             dXYCE = DriverXYCE(path_exe=self.settings.XYCE_path, path_folder_XYCE=local_model_folder, verbose=verbose)
             dXYCE.run_XYCE(simulation_name, suffix='')
         else:
             raise Exception(f'Software {software} not supported for automated running.')
 
     def write_stimuli_from_interpolation(self, step, verbose: bool = None):
         '''
@@ -1263,57 +1222,55 @@
 
         :param current_level: list, all current level that shall be used for interpolation (each magnet has 1 current level)
         :param n_total_magnets: int, Number of total magnets in the circuit (A stimuli will be written for each, non-quenching = 0)
         :param n_apertures: int, Number of apertures per magnet. A stimuli will be written for each aperture for each magnet
         :param magnets: list, magnet numbers for which the stimuli shall be written
         :param tShift: list, time shift that needs to be applied to each stimuli
         (e.g. if magnet 1 quenches at 0.05s, magnet 2 at 1s etc.), so that the stimuli are applied at the correct time in the simulation
-        :param Outputfile: str, name of the stimuli-file
+        :param output_file: str, name of the stimuli-file
         :param path_resources: str, path to the file with pre-calculated values
         :param InterpolationType: str, either Linear or Spline, type of interpolation
         :param type_stl: str, how to write the stimuli file (either 'a' (append) or 'w' (write))
         :param sparseTimeStepping: int, every x-th time value only a stimuli point is written (to reduce size of stimuli)
         :return:
         '''
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
 
         # Unpack inputs
         current_level = step.current_level
         n_total_magnets = step.n_total_magnets
         n_apertures = step.n_apertures
         magnets = step.magnets
         tShift = step.t_offset
-        Outputfile = step.output_file
+        output_file_path = step.output_file
         path_resources = step.path_interpolation_file
         InterpolationType = step.interpolation_type
         type_stl = step.type_file_writing
         sparseTimeStepping = step.n_sampling
         magnet_type = step.magnet_types
         # Set default values for selected missing inputs
         if not InterpolationType:
             InterpolationType = 'Linear'
         if not type_stl:
             type_stl = 'w'
         if not sparseTimeStepping:
             sparseTimeStepping = 1  # Note: This will ovrewrite the default value of 100 used in the writeStimuliFromInterpolation_general() function
 
         # Call coil-resistance interpolation function
-        writeStimuliFromInterpolation(current_level, n_total_magnets, n_apertures, magnets, tShift, Outputfile,
+        writeStimuliFromInterpolation(current_level, n_total_magnets, n_apertures, magnets, tShift, output_file_path,
                                               path_resources, InterpolationType, type_stl, sparseTimeStepping,
                                               magnet_type)
 
-        if 'XYCE' in Outputfile:
-            output_folder_path = os.path.join(self.output_path, 'Stimulus')
-            if not os.path.exists(output_folder_path):
-                os.makedirs(output_folder_path)
-            #self.extract_stimulus_values(Outputfile, output_folder_path)
-            translate_stimulus('all', Outputfile, output_folder_path)
+        if step.software == 'XYCE':
+            output_folder_path = os.path.join(Path(output_file_path).parent.resolve(), get_name_stimulus_folder())  # This is the folder where the output file will be generated. It contains an hard-coded folder name that is defined in ParserXYCE
+            make_folder_if_not_existing(output_folder_path, verbose=verbose)
+            translate_stimulus('all', input_file_path=output_file_path, output_path=output_folder_path)
 
         if verbose:
-            print(f'Output stimulus file {Outputfile} written.')
+            print(f'Output stimulus file {output_file_path} written.')
 
     def run_parsim_event(self, step, verbose: bool = None):
         '''
         Function to generate steps based on list of events from external file
 
         :param step:
         :param verbose: if true displays more information
@@ -1336,15 +1293,15 @@
         default_keys = step.default_keys
         path_postmortem_offline_data_folder = step.path_postmortem_offline_data_folder
         path_to_configurations_folder = step.path_to_configurations_folder
         filepath_to_temp_viewer_csv = step.filepath_to_temp_viewer_csv
 
         # Resolve path and substitute it
         path_output_from_analysis_file = default_keys.path_output  # TODO this is a workaround (see "default_keys.path_output = path_output_from_analysis_file")
-        default_keys.path_output = str(self._get_local_folder(f'local_{software}_folder'))
+        default_keys.path_output = getattr(self.settings, f'local_{software}_folder')   #str(self._get_local_folder(f'local_{software}_folder'))
 
         # Check inputs
         if not path_output_viewer_csv:
             path_output_viewer_csv = ''
             if verbose: print(f'Key "path_output_viewer_csv" was not defined in the STEAM analysis file: no output viewer files will be generated.')
         # if type(path_output_viewer_csv) == str:
         #     path_output_viewer_csv = [path_output_viewer_csv]  # Make sure this variable is always a list
@@ -1363,46 +1320,53 @@
             pem.read_from_input(path_input_file=input_file, flag_append=False, rel_quench_heater_trip_threshold=rel_quench_heater_trip_threshold)
             pem.write_event_file(simulation_name=simulation_name, simulation_numbers=simulation_numbers,
                                  t_PC_off=t_PC_off, path_outputfile_event_csv=path_output_event_csv,
                                  current_polarities_CLIQ=current_polarities_CLIQ,
                                  dict_QH_circuits_to_QH_strips=dict_QH_circuits_to_QH_strips)
 
             # start parsim sweep step with newly created event file
-            parsim_sweep_step = ParametricSweep(type='ParametricSweep', input_sweep_file=path_output_event_csv,
-                                                model_name=model_name, case_model=case_model, software=software, verbose=verbose)
+            parsim_sweep_step = ParametricSweep(type='ParametricSweep', input_sweep_file=path_output_event_csv, model_name=model_name, case_model=case_model, software=software, verbose=verbose)
             self.run_parsim_sweep(parsim_sweep_step, verbose=verbose)
 
             # TODO: merge list and dict into self.data_analysis
             # TODO: add flag_show_parsim_output ?
             # TODO: add flag to write yaml analysis with all steps
             # TODO: parse Conductor Data - but what are the names in Quenchdict? (Parsim Sweep can handly conductor changes)
 
             # Write a .csv file that can be used to run a STEAM Viewer analysis
             if path_output_viewer_csv:
                 default_keys.path_output = path_output_from_analysis_file  #TODO this is a workaround (See "path_output_from_analysis_file = default_keys.path_output")
                 pem.set_up_viewer(path_output_viewer_csv, default_keys, simulation_numbers, simulation_name, software)
                 if verbose: print(f'File {path_output_viewer_csv} written. It can be used to run a STEAM Viewer analysis.')
         elif case_model == 'circuit':
+            # Determine local software folder:
+            if software == "XYCE":
+                local_software_folder = self.settings.local_XYCE_folder
+            elif software == "PSPICE":
+                local_software_folder = self.settings.local_PSPICE_folder
+            else:
+                raise Exception(f'Software {software} not supported for the ParsimEvent step.')
+
             # Read input file and run the ParsimEvent analysis
-            pec = ParsimEventCircuit(ref_model=self.list_models[model_name], library_path=self.library_path, verbose=verbose)
+            pec = ParsimEventCircuit(ref_model=self.list_models[model_name], library_path=self.settings.local_library_path, verbose=verbose)
             pec.read_from_input(path_input_file=input_file, flag_append=False)
             if simulation_name in ["RQ_47magnets", "RQ_51magnets", "RCBX"]:
                 simulation_numbers = [0 + simulation_numbers[-1], 1 + simulation_numbers[-1]]
                 self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_numbers = simulation_numbers
             pec.write_event_file(simulation_name=simulation_name, simulation_numbers=simulation_numbers,
                                  path_outputfile_event_csv=path_output_event_csv)
 
             quenching_magnet_list = []  # required for families where multiple magnets can quench like RB
             quenching_magnet_time = []
             quenching_current_list = []
             for event_number in range(len(pec.list_events)):  # reading through each row of the event file
                 # get circuit specific information
                 circuit_name = pec.list_events[event_number].GeneralParameters.name
-                circuit_family_name = get_circuit_family_from_circuit_name(circuit_name, self.library_path)
-                circuit_type = get_circuit_type_from_circuit_name(circuit_name, self.library_path, simulation_name)
+                circuit_family_name = get_circuit_family_from_circuit_name(circuit_name, self.settings.local_library_path)
+                circuit_type = get_circuit_type_from_circuit_name(circuit_name, self.settings.local_library_path, simulation_name)
                 magnet_name = get_magnet_name(circuit_name,simulation_name,circuit_type)
                 number_of_magnets = get_number_of_magnets(circuit_name,simulation_name,circuit_type,circuit_family_name)
                 number_of_apertures = get_number_of_apertures_from_circuit_family_name(circuit_family_name)
                 if circuit_family_name == "RB":
                     current_level = pec.list_events[event_number].QuenchEvents[circuit_name].current_at_quench
                     t_PC_off = pec.list_events[0].PoweredCircuits[circuit_name].delta_t_FGC_PIC
                 else:
@@ -1412,42 +1376,42 @@
                 assert(simulation_name==self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name)
                 magnet_types = get_magnet_types_list(number_of_magnets, simulation_name)
 
                 # load circuit parameters step
                 if circuit_family_name == "RQ":
                     circuit_name_1 = circuit_name.replace(".", "D_")
                     circuit_name_2 = circuit_name.replace(".", "F_")
-                    load_circuit_parameters_step_1 = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(self.library_path, f"circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_1)
-                    load_circuit_parameters_step_2 = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(self.library_path, f"circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_2)
+                    load_circuit_parameters_step_1 = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(self.settings.local_library_path, f"circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_1)
+                    load_circuit_parameters_step_2 = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(self.settings.local_library_path, f"circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_2)
                     position = pec.list_events[event_number].QuenchEvents[circuit_name].magnet_electrical_position
-                    quenching_magnet = [get_number_of_quenching_magnets_from_layoutdetails(position, circuit_family_name,library_path=self.library_path)]
+                    quenching_magnet = [get_number_of_quenching_magnets_from_layoutdetails(position, circuit_family_name,library_path=self.settings.local_library_path)]
                     # modify model diode step used to change diodes across the quenching magnets with heating
                     modify_model_diode_step = ModifyModel(type='ModifyModel', model_name=model_name, variable_to_change=f'Netlist[x_D{quenching_magnet[0]}].value', variable_value=[
                         "RQ_Protection_Diode"], simulation_numbers=[], simulation_name=simulation_name, software=software)
                 elif circuit_type == "RCBX":
                     circuit_name_1 = circuit_name.replace("X", "XH")
                     circuit_name_2 = circuit_name.replace("X", "XV")
-                    load_circuit_parameters_step_1 = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(self.library_path, f"circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_1)
-                    load_circuit_parameters_step_2 = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(self.library_path, f"circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_2)
+                    load_circuit_parameters_step_1 = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(self.settings.local_library_path, f"circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_1)
+                    load_circuit_parameters_step_2 = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(self.settings.local_library_path, f"circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_2)
                 elif circuit_type in ["RCD", "RCO"]:
                     if "-" in circuit_name:
                         parts = circuit_name.split("-")
                         last_part = parts[-1]
                         circuit_name_RCD = parts[0] + "." + last_part.split(".")[1]
                         circuit_name_RCO = last_part
                     elif "." in circuit_name:
                         circuit_name_RCD = circuit_name.replace(".", "D.", 1)
                         circuit_name_RCO = circuit_name.replace(".", "O.", 1)
                     temp_circuit_name = circuit_name_RCD if circuit_type == "RCD" else circuit_name_RCO
-                    load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(self.library_path, f"circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=temp_circuit_name)
+                    load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(self.settings.local_library_path, f"circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=temp_circuit_name)
                 elif circuit_family_name == "RB":
                     if event_number == len(pec.list_events) - 1:
-                        load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(self.library_path, f"circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name)
+                        load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(self.settings.local_library_path, f"circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name)
                 else:
-                    load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(self.library_path, f"circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name)
+                    load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(self.settings.local_library_path, f"circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name)
 
                 # choosing stimulus output file location
                 if circuit_family_name == "IPD":
                     stimulus_output_file = os.path.join(default_keys.path_output, f'{circuit_family_name}', f"{self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_numbers[0]}", 'coil_resistances.stl')
                 elif circuit_family_name == "RQ":
                     stimulus_output_file_1 = os.path.join(default_keys.path_output, f'{circuit_type}', f"{self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_numbers[0]}", 'coil_resistances.stl')
                     stimulus_output_file_2 = os.path.join(default_keys.path_output, f'{circuit_type}', f"{self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_numbers[1]}", 'coil_resistances.stl')
@@ -1469,96 +1433,92 @@
                     stimulus_output_file = os.path.join(default_keys.path_output, 'RQS_R_LxBx', f"{self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_numbers[0]}", 'coil_resistances.stl')
                 else:
                     stimulus_output_file = os.path.join(default_keys.path_output, f'{circuit_type}', f"{self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_numbers[0]}", 'coil_resistances.stl')
 
                 # making appropriate directory if it doesn't exist for the stimulus output file
                 if circuit_family_name == "RQ" or circuit_type == "RCBX":
                     for file_path in [stimulus_output_file_1, stimulus_output_file_2]:
-                        directory = os.path.dirname(file_path)
-                        if not os.path.exists(directory):
-                            os.makedirs(directory)
-                else:
-                    if circuit_family_name == "RB":
-                        if event_number == len(pec.list_events) - 1:
-                            directory = os.path.dirname(stimulus_output_file)
-                            if not os.path.exists(directory):
-                                os.makedirs(directory)
-                    else:
-                        directory = os.path.dirname(stimulus_output_file)
-                        if not os.path.exists(directory):
-                            os.makedirs(directory)
+                        make_folder_if_not_existing(os.path.dirname(file_path))
+                elif circuit_family_name == "RB" and event_number == len(pec.list_events) - 1 or circuit_family_name != "RB":
+                    make_folder_if_not_existing(os.path.dirname(stimulus_output_file))
+                else: pass
 
                 # write stimulus file step
                 if circuit_family_name == "RQ":
                     if pec.list_events[event_number].QuenchEvents[circuit_name].quench_cause == "No quench":
                         current_level = [0]*len(quenching_magnet)
-                    write_stimuli_file_step_1 = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file_1, path_interpolation_file=[os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]], magnets=quenching_magnet, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=100, magnet_types=magnet_types)
-                    write_stimuli_file_step_2 = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file_2, path_interpolation_file=[os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]], magnets=quenching_magnet, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=100, magnet_types=magnet_types)
+                    write_stimuli_file_step_1 = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file_1, path_interpolation_file=[os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]], magnets=quenching_magnet, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=100, magnet_types=magnet_types)
+                    write_stimuli_file_step_2 = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file_2, path_interpolation_file=[os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]], magnets=quenching_magnet, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=100, magnet_types=magnet_types)
                 elif circuit_type == "RCBX":
                     if pec.list_events[event_number].QuenchEvents[circuit_name].quench_cause == "No quench":
                         current_level = [0, 0]
-                    write_stimuli_file_step_1 = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file_1, path_interpolation_file=[os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[0]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level[0])], magnets=magnets_list, t_offset=[t_PC_off[0]], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
-                    write_stimuli_file_step_2 = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file_2, path_interpolation_file=[os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level[1])], magnets=magnets_list, t_offset=[t_PC_off[1]], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step_1 = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file_1, path_interpolation_file=[os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[0]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level[0])], magnets=magnets_list, t_offset=[t_PC_off[0]], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step_2 = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file_2, path_interpolation_file=[os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level[1])], magnets=magnets_list, t_offset=[t_PC_off[1]], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 elif circuit_family_name == "RQX":
                     if pec.list_events[event_number].QuenchEvents[circuit_name].quench_cause == "No quench":
                         current_level = [0] * len(magnets_list)
                     current_level = [current_level[0]+current_level[1], current_level[0]+current_level[2], current_level[0]+current_level[2], current_level[0]] #see schematic
-                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=current_level, magnets=magnets_list, t_offset=[t_PC_off]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=current_level, magnets=magnets_list, t_offset=[t_PC_off]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 elif circuit_family_name == "IPQ" and number_of_magnets == 2:
                     if pec.list_events[event_number].QuenchEvents[circuit_name].quench_cause == "No quench":
                         current_level = [0] * len(magnets_list)
-                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=current_level, magnets=magnets_list, t_offset=[t_PC_off]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=current_level, magnets=magnets_list, t_offset=[t_PC_off]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 elif circuit_family_name == "IPQ" and number_of_magnets == 1:
                     if pec.list_events[event_number].QuenchEvents[circuit_name].quench_cause == "No quench":
                         current_level = [0] * len(magnets_list)
-                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]], magnets=magnets_list, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]], magnets=magnets_list, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 elif circuit_type in ["RCS", "RO_13magnets", "RO_8magnets", "RSD_12magnets", "RSD_11magnets", "RSF_10magnets", "RSF_9magnets", "RQTL9", "RQT"] or (circuit_type == "RQ6" and circuit_family_name == "600A") or circuit_name.startswith("RQS.A"):
                     if pec.list_events[event_number].QuenchEvents[circuit_name].quench_cause == "No quench":
                         current_level = 0
-                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level)]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off[0]]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level)]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off[0]]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 elif circuit_name.startswith(("RQS.R", "RQS.L", "RSS")):
                     if pec.list_events[event_number].QuenchEvents[circuit_name].quench_cause == "No quench":
                         current_level = 0
-                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level)]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level)]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 elif circuit_type == "RB":
-                    position = pec.list_events[event_number].QuenchEvents[circuit_name].magnet_electrical_position
-                    quenching_magnet = [get_number_of_quenching_magnets_from_layoutdetails(position, circuit_family_name,library_path=self.library_path)]
-                    quenching_magnet_list.append(quenching_magnet[0])
-                    quenching_magnet_time.append(pec.list_events[event_number].QuenchEvents[circuit_name].delta_t_iQPS_PIC)
+                    if not pec.list_events[event_number].QuenchEvents[circuit_name].quench_cause == "No quench":
+                        position = pec.list_events[event_number].QuenchEvents[circuit_name].magnet_electrical_position
+                        quenching_magnet = [get_number_of_quenching_magnets_from_layoutdetails(position, circuit_family_name,library_path=self.settings.local_library_path)]
+                        quenching_magnet_list.append(quenching_magnet[0])
+                        quenching_magnet_time.append(pec.list_events[event_number].QuenchEvents[circuit_name].delta_t_iQPS_PIC)
+                        # modify model diode step used to change diodes across the quenching magnets with heating
+                        modify_model_diode_step = ModifyModel(type='ModifyModel', model_name=model_name,
+                                                              variable_to_change=f'Netlist[x_D{quenching_magnet[0]}].value',
+                                                              variable_value=[
+                                                                  "RB_Protection_Diode"], simulation_numbers=[],
+                                                              simulation_name=simulation_name, software=software)
                     quenching_current_list.append(current_level)
-                    # modify model diode step used to change diodes across the quenching magnets with heating
-                    modify_model_diode_step = ModifyModel(type='ModifyModel', model_name=model_name, variable_to_change=f'Netlist[x_D{quenching_magnet[0]}].value', variable_value=[
-                        "RB_Protection_Diode"], simulation_numbers=[], simulation_name=simulation_name, software=software)
                     if event_number == len(pec.list_events) - 1:
-                        zipped_lists = zip(quenching_magnet_list, quenching_magnet_time, quenching_current_list)
-                        sorted_lists = sorted(zipped_lists, key=lambda x: x[0])
-                        quenching_magnet_list, quenching_magnet_time, quenching_current_list = zip(*sorted_lists)
+                        if not pec.list_events[event_number].QuenchEvents[circuit_name].quench_cause == "No quench":
+                            zipped_lists = zip(quenching_magnet_list, quenching_magnet_time, quenching_current_list)
+                            sorted_lists = sorted(zipped_lists, key=lambda x: x[0])
+                            quenching_magnet_list, quenching_magnet_time, quenching_current_list = zip(*sorted_lists)
                         if pec.list_events[event_number].QuenchEvents[circuit_name].quench_cause == "No quench":
                             quenching_current_list = [0]*len(quenching_current_list)
-                        write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=quenching_current_list, magnets=quenching_magnet_list, t_offset=quenching_magnet_time, interpolation_type='Linear', type_file_writing='w', n_sampling=100, magnet_types=magnet_types)
+                        write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=quenching_current_list, magnets=quenching_magnet_list, t_offset=quenching_magnet_time, interpolation_type='Linear', type_file_writing='w', n_sampling=100, magnet_types=magnet_types)
                 elif circuit_type == "RCD":
                     if pec.list_events[event_number].QuenchEvents[circuit_name].quench_cause == "No quench":
                         current_level = [0, 0]
-                    # write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level[1])]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off[0]]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    # write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level[1])]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off[0]]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                     n_required_coil_resistance_signals = 2
                     magnets_list = [1, 2]
                     magnet_types = [1, 2]
-                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=n_required_coil_resistance_signals, n_apertures=number_of_apertures, current_level=[abs(current_level[1])]*n_required_coil_resistance_signals, magnets=magnets_list, t_offset=[t_PC_off[0]]*n_required_coil_resistance_signals, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=n_required_coil_resistance_signals, n_apertures=number_of_apertures, current_level=[abs(current_level[1])]*n_required_coil_resistance_signals, magnets=magnets_list, t_offset=[t_PC_off[0]]*n_required_coil_resistance_signals, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 elif circuit_type == "RCO":
                     if pec.list_events[event_number].QuenchEvents[circuit_name].quench_cause == "No quench":
                         current_level = [0, 0]
-                    # write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level[0])]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off[0]]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    # write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level[0])]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off[0]]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                     n_required_coil_resistance_signals = 2
                     magnets_list = [1, 2]
                     magnet_types = [1, 2]
-                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=n_required_coil_resistance_signals, n_apertures=number_of_apertures, current_level=[abs(current_level[0])]*n_required_coil_resistance_signals, magnets=magnets_list, t_offset=[t_PC_off[0]]*n_required_coil_resistance_signals, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=n_required_coil_resistance_signals, n_apertures=number_of_apertures, current_level=[abs(current_level[0])]*n_required_coil_resistance_signals, magnets=magnets_list, t_offset=[t_PC_off[0]]*n_required_coil_resistance_signals, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 else:
                     if pec.list_events[event_number].QuenchEvents[circuit_name].quench_cause == "No quench":
                         current_level = 0
-                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(self.library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level)], magnets=magnets_list, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(self.settings.local_library_path,'circuits','coil_resistances_to_interpolate',f'interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level)], magnets=magnets_list, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
 
                 # parsim sweep step with newly created event file
                 if circuit_family_name == "RQ" or circuit_type == "RCBX":
                     output_files = create_two_csvs_from_odd_and_even_rows(path_output_event_csv)
                     parsim_sweep_step_1 = ParametricSweep(type='ParametricSweep', input_sweep_file=output_files[0],
                                                         model_name=model_name, case_model=case_model, software=software, verbose=verbose)
                     parsim_sweep_step_2 = ParametricSweep(type='ParametricSweep', input_sweep_file=output_files[1],
@@ -1607,15 +1567,16 @@
                         # but not both. In either case, we have to reverse the direction of the crowbar, either to adapt to
                         # the negative current for RCBXV or to turn it back in the positive direction after it was reversed
                         # for the simulation of RCBXH.
                         self.reverse_crowbar(temp_current_level = -1 ,model_name = model_name, #hard coded negative current level to force the reversal in such case
                                              simulation_name = simulation_name, software = software, verbose = verbose)
                     self.run_parsim_sweep(parsim_sweep_step_2, verbose=verbose)
                 elif circuit_type == "RB":
-                    self.step_modify_model(modify_model_diode_step, verbose=verbose)  # diode is changed for each row of the event file
+                    if not pec.list_events[event_number].QuenchEvents[circuit_name].quench_cause == "No quench":
+                        self.step_modify_model(modify_model_diode_step, verbose=verbose)  # diode is changed for each row of the event file
                     if event_number == len(pec.list_events)-1:  # the simulation runs correctly only at the end
                         self.load_circuit_parameters(load_circuit_parameters_step, verbose=verbose)
                         self.write_stimuli_from_interpolation(write_stimuli_file_step, verbose=verbose)
                         #Note: RB circuits do not have the generic crowbar, so we do not have to reverse it here as for RCBX
                         self.run_parsim_sweep(parsim_sweep_step, verbose=verbose)
                 else:
                     self.load_circuit_parameters(load_circuit_parameters_step, verbose=verbose)
@@ -1630,27 +1591,20 @@
                                          simulation_name=simulation_name, software=software, verbose=verbose)
 
                     self.run_parsim_sweep(parsim_sweep_step, verbose=verbose)
 
                 # write an input file for the viewer here:
                 # file will by default be saved in the simulation folder
                 if path_postmortem_offline_data_folder:
-                    if software == "XYCE":
-                        temp_working_directory = self.data_analysis.PermanentSettings.local_XYCE_folder
-                    elif software == "PSPICE":
-                        temp_working_directory = self.data_analysis.PermanentSettings.local_PSPICE_folder
-                    else:
-                        temp_working_directory = "None"
-
                     unique_identifier = generate_unique_event_identifier_from_eventfile(os.path.basename(input_file),
                                                                                         verbose=True)
                     write_config_file_for_viewer(circuit_type = circuit_type, simulation_numbers = simulation_numbers,
                                                  circuit_name = circuit_name, circuit_family = circuit_family_name,
                                                  t_PC_off = t_PC_off, path_to_configurations_folder = path_to_configurations_folder,
-                                                 temp_working_directory = temp_working_directory, path_postmortem_offline_data_folder = path_postmortem_offline_data_folder,
+                                                 temp_working_directory = local_software_folder, path_postmortem_offline_data_folder = path_postmortem_offline_data_folder,
                                      unique_identifier = unique_identifier, filepath_to_temp_viewer_csv = filepath_to_temp_viewer_csv)
         else:
             raise Exception(f'case_model {case_model} not supported by ParsimEvent.')
 
         if verbose:
             print(f'ParsimEvent called using input file {input_file}.')
 
@@ -1912,509 +1866,25 @@
             if revert:
                 self.list_models[model_name] = deepcopy(local_model_copy)
                 del local_model_copy
 
         if verbose:
             print(f'Parsim Event called using input file {input_sweep_file}.')
 
-    def steam_analyze_lhc_event(self, input_csv_file: str, flag_run_software: bool, software: str, dict_settings_paths: dict, file_counter: int):
-        aSTEAM = AnalysisSTEAM()
-
-        # Assign the keys read either from permanent-settings or local-settings TODO: later in inititalization of subclass
-        for name, _ in dict_settings_paths.items():
-            if name in  aSTEAM.settings.__dict__:
-                print(f"Found {name} in settings")
-                value = dict_settings_paths[name]
-                aSTEAM.setAttribute(aSTEAM.settings, name, value)
-                if value:
-                    print('{} : {}. Added.'.format(name, value))
-            elif name == 'library_path':
-                aSTEAM.library_path = dict_settings_paths['library_path']
-            else:
-                print('{}: not found in the settings. Skipped.'.format(name))
-
-        aSTEAM.data_analysis.WorkingFolders.library_path = dict_settings_paths['library_path']
-        aSTEAM.data_analysis.PermanentSettings.PSPICE_path = dict_settings_paths['PSPICE_path']
-        aSTEAM.data_analysis.PermanentSettings.XYCE_path = dict_settings_paths['XYCE_path']
-        aSTEAM.data_analysis.PermanentSettings.PSPICE_library_path = dict_settings_paths['PSPICE_library_path']
-        aSTEAM.data_analysis.PermanentSettings.local_PSPICE_folder = dict_settings_paths['local_PSPICE_folder']
-        aSTEAM.data_analysis.PermanentSettings.local_XYCE_folder = dict_settings_paths['local_XYCE_folder']
-
-
-        if software == 'PSPICE':
-            local_folder = aSTEAM.settings.local_PSPICE_folder
-            print(f"Changed local folder to {local_folder}")
-        elif software == 'XYCE':
-            local_folder = aSTEAM.settings.local_XYCE_folder
-            print(f"Changed local folder to {local_folder}")
-
-        circuit_name = get_circuit_name_from_eventfile(event_file=os.path.join(os.getcwd(), input_csv_file))
-        if circuit_name.startswith("RCD"):
-            aSTEAM.analyze_RCD_RCO_event(os.path.join(os.getcwd(), input_csv_file), local_folder, flag_run_software, software, file_counter,dict_settings_paths)
-        elif circuit_name.startswith(("RD1", "RD2", "RD3", "RD4")):
-            circuit_type = "IPD"
-            aSTEAM.analyze_circuit_event(os.path.join(os.getcwd(), input_csv_file), local_folder, circuit_type, flag_run_software, software, file_counter,dict_settings_paths)
-        elif circuit_name.startswith(("RQ4", "RQ5", "RQ7", "RQ8", "RQ9", "RQ10")) or (circuit_name.startswith("RQ6.") and len(circuit_name) == 6):
-            circuit_type = find_IPQ_circuit_type_from_IPQ_parameters_table(os.path.join( aSTEAM.library_path, f"circuits/circuit_parameters/IPQ_circuit_parameters.csv"), input_csv_file.split("\\")[-1].split("_")[0])
-            print(circuit_type)
-            aSTEAM.analyze_circuit_event(os.path.join(os.getcwd(), input_csv_file), local_folder, circuit_type, flag_run_software, software, file_counter,dict_settings_paths)
-        else:
-            # circuit_type = get_circuit_type(circuit_name,  aSTEAM.library_path) OLD
-            circuit_type = get_circuit_type_from_circuit_name(circuit_name,  aSTEAM.library_path)
-            aSTEAM.analyze_circuit_event(os.path.join(os.getcwd(), input_csv_file), local_folder, circuit_type, flag_run_software, software, file_counter,dict_settings_paths)
-
-    def analyze_circuit_event(self, input_csv_file: str, local_folder: str,circuit_type: str, flag_run_software: bool, software: str, file_counter: int,dict_settings_paths: dict):
-        #file_counter = 1
-        #file_name_analysis = os.path.join(os.getcwd(), "analysisSTEAM_settings.yaml") #file containing settings paths
-        unique_identifier_event = os.path.splitext(os.path.basename(input_csv_file))[0]
-
-        output_directory_yaml_files = dict_settings_paths['output_directory_yaml_files']
-        output_directory_event_files = dict_settings_paths['output_directory_event_files']
-
-        yaml_file_name = f'Infile_{software}_{unique_identifier_event}_{file_counter}.yaml'
-        event_file_name = f'Eventfile_{software}_{unique_identifier_event}_{file_counter}.csv'
-
-        path_output_yaml_file = os.path.join(output_directory_yaml_files,yaml_file_name)
-        path_output_event_csv = os.path.join(output_directory_event_files,event_file_name)
-
-        self.data_analysis.AnalysisStepDefinition = {
-            'setup_folder_PSPICE': SetUpFolder(type='SetUpFolder', simulation_name=circuit_type, software=software),
-            'makeModel_ref': MakeModel(type='MakeModel', model_name='BM', file_model_data=circuit_type,
-                                       case_model='circuit', software=software, simulation_name=None,
-                                       simulation_number=None, flag_build=True, verbose=False,
-                                       flag_plot_all=False, flag_json=False),
-            'modifyModel_probe': ModifyModelMultipleVariables(type='ModifyModelMultipleVariables', model_name='BM',
-                                           variables_to_change=['PostProcess.probe.probe_type'],
-                                                              variables_value=[['CSDF']], software=software,
-                                                              simulation_name=None,
-                                           simulation_numbers=[]),
-            'runParsimEvent': ParsimEvent(type='ParsimEvent', input_file=input_csv_file,
-                                          path_output_event_csv=path_output_event_csv, path_output_viewer_csv=None,
-                                          simulation_numbers=[file_counter], model_name='BM', case_model='circuit',
-                                          simulation_name=circuit_type, software=software, t_PC_off=None,
-                                          rel_quench_heater_trip_threshold=None, current_polarities_CLIQ=[],
-                                          dict_QH_circuits_to_QH_strips={},
-                                          default_keys=DefaultParsimEventKeys(local_LEDET_folder=None,
-                                                                              path_config_file=None, default_configs=[],
-                                                                              path_tdms_files=None,
-                                                                              path_output_measurement_files=None,
-                                                                              path_output=local_folder)),
-            'run_simulation': RunSimulation(type='RunSimulation', software=software, simulation_name=circuit_type, simulation_numbers=[file_counter])}
-
-        self.output_path = local_folder
-        if software == 'PSPICE':
-            self.data_analysis.PermanentSettings.local_PSPICE_folder = local_folder
-        elif software == 'XYCE':
-            self.data_analysis.PermanentSettings.local_XYCE_folder = local_folder
-        if flag_run_software== False:
-            self.data_analysis.AnalysisStepSequence = ['setup_folder_PSPICE', 'makeModel_ref', 'modifyModel_probe', 'runParsimEvent']
-        else:
-            self.data_analysis.AnalysisStepSequence = ['setup_folder_PSPICE', 'makeModel_ref', 'modifyModel_probe', 'runParsimEvent', 'run_simulation']
-
-        if software == 'PSPICE':
-            local_PSPICE_folder = self._get_local_folder('local_PSPICE_folder')
-            list_output_file = [
-                os.path.join(local_PSPICE_folder, f'{circuit_type}', f'{file_counter}', f'{circuit_type}.cir')]
-        elif software == 'XYCE':
-            local_XYCE_folder = self._get_local_folder('local_XYCE_folder')
-            list_output_file = [
-                os.path.join(local_XYCE_folder, f'{circuit_type}', f'{file_counter}', f'{circuit_type}.cir')]
-
-        if os.path.exists(path_output_yaml_file): os.remove(path_output_yaml_file)
-        for file in list_output_file:
-            if os.path.exists(file): os.remove(file)
-
-        # act
-        #print(self.data_analysis.PermanentSettings.PSPICE_path)
-        self.write_analysis_file(path_output_file=path_output_yaml_file)
-        self.run_analysis(verbose= True)
-
-
-
-    def analyze_RCD_RCO_event(self, input_csv_file: str, local_folder: str, flag_run_software: bool, software: str, file_counter: int, dict_settings_paths: dict):
-
-        unique_identifier_event = os.path.splitext(os.path.basename(input_csv_file))[0]
-
-        output_directory_yaml_files = dict_settings_paths['output_directory_yaml_files']
-        output_directory_event_files = dict_settings_paths['output_directory_event_files']
-
-        yaml_file_name = f'Infile_{software}_{unique_identifier_event}_{file_counter}.yaml'
-        event_file_name_RCO = f'Eventfile_RCO_{software}_{unique_identifier_event}_{file_counter}.csv'
-        event_file_name_RCD = f'Eventfile_RCD_{software}_{unique_identifier_event}_{file_counter}.csv'
-
-        path_output_yaml_file = os.path.join(output_directory_yaml_files,yaml_file_name)
-        path_output_event_RCO_csv = os.path.join(output_directory_event_files, event_file_name_RCO)
-        path_output_event_RCD_csv = os.path.join(output_directory_event_files, event_file_name_RCD)
-
-        # arrange
-        file_name_analysis = os.path.join(os.getcwd(), "analysisSTEAM_settings.yaml") #file containing settings paths
-        aSTEAM_1 = AnalysisSTEAM(file_name_analysis=file_name_analysis)
-        if software == 'PSPICE':
-            aSTEAM_1.settings.local_PSPICE_folder = local_folder
-        elif software == 'XYCE':
-            aSTEAM_1.settings.local_XYCE_folder = local_folder
-        aSTEAM_1.data_analysis.AnalysisStepDefinition = {
-            'setup_folder_PSPICE': SetUpFolder(type='SetUpFolder', simulation_name='RCO', software=software),
-            'makeModel_ref': MakeModel(type='MakeModel', model_name='BM', file_model_data='RCO', case_model='circuit',
-                                       software=software, simulation_name=None, simulation_number=None, flag_build=True,
-                                       verbose=False, flag_plot_all=False, flag_json=False),
-            'runParsimEvent': ParsimEvent(type='ParsimEvent', input_file=input_csv_file,
-                                          path_output_event_csv=path_output_event_RCO_csv, path_output_viewer_csv=None,
-                                          simulation_numbers=[file_counter], model_name='BM', case_model='circuit',
-                                          simulation_name='RCO', software=software, t_PC_off=None,
-                                          rel_quench_heater_trip_threshold=None, current_polarities_CLIQ=[],
-                                          dict_QH_circuits_to_QH_strips={},
-                                          default_keys=DefaultParsimEventKeys(local_LEDET_folder=None,
-                                                                              path_config_file=None, default_configs=[],
-                                                                              path_tdms_files=None,
-                                                                              path_output_measurement_files=None,
-                                                                              path_output=local_folder)),
-            'run_simulation': RunSimulation(type='RunSimulation', software=software, simulation_name='RCO',
-                                            simulation_numbers=[file_counter])}
-        aSTEAM_1.output_path = local_folder
-        if software == 'PSPICE':
-            aSTEAM_1.data_analysis.PermanentSettings.local_PSPICE_folder = local_folder
-        elif software == 'XYCE':
-            aSTEAM_1.data_analysis.PermanentSettings.local_XYCE_folder = local_folder
-        if flag_run_software == False:
-            aSTEAM_1.data_analysis.AnalysisStepSequence = ['setup_folder_PSPICE', 'makeModel_ref', 'runParsimEvent']
-        else:
-            aSTEAM_1.data_analysis.AnalysisStepSequence = ['setup_folder_PSPICE', 'makeModel_ref', 'runParsimEvent', 'run_simulation']
-
-        aSTEAM_2 = AnalysisSTEAM(file_name_analysis=file_name_analysis)
-        if software == 'PSPICE':
-            aSTEAM_2.settings.local_PSPICE_folder = local_folder
-        elif software == 'XYCE':
-            aSTEAM_2.settings.local_XYCE_folder = local_folder
-        aSTEAM_2.data_analysis.AnalysisStepDefinition = {
-            'setup_folder_PSPICE': SetUpFolder(type='SetUpFolder', simulation_name='RCD', software=software),
-            'makeModel_ref': MakeModel(type='MakeModel', model_name='BM', file_model_data='RCD', case_model='circuit',
-                                       software=software, simulation_name=None, simulation_number=None, flag_build=True,
-                                       verbose=False, flag_plot_all=False, flag_json=False),
-            'runParsimEvent': ParsimEvent(type='ParsimEvent', input_file=input_csv_file,
-                                          path_output_event_csv=path_output_event_RCD_csv, path_output_viewer_csv=None,
-                                          simulation_numbers=[file_counter], model_name='BM', case_model='circuit',
-                                          simulation_name='RCD', software=software, t_PC_off=None,
-                                          rel_quench_heater_trip_threshold=None, current_polarities_CLIQ=[],
-                                          dict_QH_circuits_to_QH_strips={},
-                                          default_keys=DefaultParsimEventKeys(local_LEDET_folder=None,
-                                                                              path_config_file=None, default_configs=[],
-                                                                              path_tdms_files=None,
-                                                                              path_output_measurement_files=None,
-                                                                              path_output=local_folder)),
-            'run_simulation': RunSimulation(type='RunSimulation', software=software, simulation_name='RCD',
-                                            simulation_numbers=[file_counter])}
-        aSTEAM_2.output_path = local_folder
-        if software == 'PSPICE':
-            aSTEAM_2.data_analysis.PermanentSettings.local_PSPICE_folder = local_folder
-        elif software == 'XYCE':
-            aSTEAM_2.data_analysis.PermanentSettings.local_XYCE_folder = local_folder
-        if flag_run_software == False:
-            aSTEAM_2.data_analysis.AnalysisStepSequence = ['setup_folder_PSPICE', 'makeModel_ref', 'runParsimEvent']
-        else:
-            aSTEAM_2.data_analysis.AnalysisStepSequence = ['setup_folder_PSPICE', 'makeModel_ref', 'runParsimEvent', 'run_simulation']
-
-        if input_csv_file.endswith('.csv'):
-            outputfile_1 = os.path.join(os.getcwd(), 'output', 'run_parsim_event_circuit',
-                                        f'TestFile_AnalysisSTEAM_run_parsim_event_circuit_RCO_{file_counter}.yaml')
-            outputfile_2 = os.path.join(os.getcwd(), 'output', 'run_parsim_event_circuit',
-                                        f'TestFile_AnalysisSTEAM_run_parsim_event_circuit_RCD_{file_counter}.yaml')
-            if software == 'PSPICE':
-                list_output_file = [
-                    os.path.join(aSTEAM_1.settings.local_PSPICE_folder, 'RCO', f'{file_counter}', 'RCO.cir'),
-                    os.path.join(aSTEAM_2.settings.local_PSPICE_folder, 'RCD', f'{file_counter}', 'RCD.cir')]
-            elif software == 'XYCE':
-                list_output_file = [
-                    os.path.join(aSTEAM_1.settings.local_XYCE_folder, 'RCO', f'{file_counter}', 'RCO.cir'),
-                    os.path.join(aSTEAM_2.settings.local_XYCE_folder, 'RCD', f'{file_counter}', 'RCD.cir')]
-            if os.path.exists(outputfile_1): os.remove(outputfile_1)
-            if os.path.exists(outputfile_2): os.remove(outputfile_2)
-            for file in list_output_file:
-                if os.path.exists(file): os.remove(file)
-
-            # act
-            aSTEAM_1.write_analysis_file(path_output_file=outputfile_1)
-            aSTEAM_1.run_analysis()
-
-            aSTEAM_2.write_analysis_file(path_output_file=outputfile_2)
-            aSTEAM_2.run_analysis()
-
-
-    # def __get_circuit_family_name(self, circuit_name: str):
-    #     if circuit_name.startswith("RCBH") or circuit_name.startswith("RCBV"):
-    #         return "60A"
-    #     elif circuit_name.startswith("RD"):
-    #         return "IPD"
-    #     elif circuit_name.startswith("RQX"):
-    #         return "RQX"
-    #     elif circuit_name.startswith(("RQ4", "RQ5", "RQ7", "RQ8", "RQ9", "RQ10")) or (circuit_name.startswith("RQ6.") and len(circuit_name) == 6):
-    #         return "IPQ"
-    #     elif circuit_name.startswith(("RQT12", "RQT13", "RQS", "RSS", "RQTL7", "RQTL8", "RQTL10", "RQTL11", "RCBX", "RQSX3", "RCS", "ROD", "ROF", "RSD", "RSF", "RQTL9", "RQTD", "RQTF", "RCD", "RCO", "RC.")) or (circuit_name.startswith("RQ6.") and len(circuit_name) == 8):
-    #         return "600A"
-    #     elif circuit_name.startswith("RQ"):
-    #         return "RQ"
-    #     elif circuit_name.startswith(("RCBY", "RCBC", "RCTX")):
-    #         return "80-120A"
-    #     elif circuit_name.startswith("RB"):
-    #         return "RB"
-
-    # def __get_magnet_name(self, circuit_name: str, simulation_name: str, circuit_type: str):
-    #     #assert (simulation_name == self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name)
-    #     #assert (circuit_type == self.__get_circuit_type(circuit_name, self.library_path))
-    #     #assert (True == False)
-    #
-    #     if circuit_name.startswith("RCBH") or circuit_name.startswith("RCBV"):
-    #         return "MCBH"
-    #     elif circuit_name.startswith("RD"):
-    #         #circuit_type = self.__get_circuit_type(circuit_name, self.library_path)
-    #         magnet_dict = {"RD1": "MBX", "RD2": "MBRC", "RD3": "MBRS", "RD4": "MBRB"}
-    #         return magnet_dict.get(circuit_type, "")
-    #     elif circuit_name.startswith("RQX"):
-    #         return ["MQXA", "MQXB"]
-    #     elif circuit_name.startswith(("RQ4", "RQ5", "RQ7", "RQ8", "RQ9", "RQ10")) or (circuit_name.startswith("RQ6.") and len(circuit_name) == 6):
-    #         magnet_dict = {"IPQ_RQ4_2_2xRPHH_2xMQY": "MQY", "IPQ_RQ4_4_2xRPHH_4xMQY": ["MQY", "MQY"], "IPQ_RQ5_2_2xRPHGB_2xMQML": "MQML", "IPQ_RQ5_2_2xRPHH_2xMQY": "MQY", "IPQ_RQ5_4_2xRPHGB_4xMQM": ["MQM", "MQM"], "IPQ_RQ5_4_2xRPHH_4xMQY": ["MQY", "MQY"], "IPQ_RQ6_2_2xRPHGB_2xMQML": "MQML", "IPQ_RQ6_2_2xRPHGB_2xMQY": "MQY", "IPQ_RQ6_4_2xRPHGB_2xMQM_2xMQML": ["MQM", "MQML"], "IPQ_RQ7_2_2xRPHGA_2xMQM": "MQM", "IPQ_RQ7_4_2xRPHGA_4xMQM": ["MQM", "MQM"], "IPQ_RQ8_2_2xRPHGA_2xMQML": "MQML", "IPQ_RQ9_4_2xRPHGA_2xMQM_2xMQMC": ["MQM", "MQMC"], "IPQ_RQ10_2_2xRPHGA_2xMQML": "MQML"}
-    #         return magnet_dict.get(simulation_name, "")
-    #     elif circuit_name.startswith("RQ6.") and len(circuit_name) == 8:
-    #         return ["MQTLH", "MQTLH_quenchback"]
-    #     elif circuit_name.startswith(("RQTL7", "RQTL8", "RQTL10", "RQTL11")):
-    #         return "MQTLI"
-    #     elif circuit_name.startswith("RQTL9"):
-    #         return ["MQTLI", "MQTLI_quenchback"]
-    #     elif circuit_name.startswith("RQSX3"):
-    #         return "MQSX"
-    #     elif circuit_name.startswith("RQS"):
-    #         return ["MQS", "MQS_quenchback"]
-    #     elif circuit_name.startswith(("RQT12", "RQT13")):
-    #         return "MQT"
-    #     elif circuit_name.startswith(("RQTD", "RQTF")):
-    #         return ["MQT", "MQT_quenchback"]
-    #     elif circuit_name.startswith("RQ"):
-    #         return "MQ"
-    #     elif circuit_name.startswith("RCBY"):
-    #         return "MCBYH"
-    #     elif circuit_name.startswith("RCBC"):
-    #         return "MCBCH"
-    #     elif circuit_name.startswith("RCS"):
-    #         return ["MCS", "MCS_quenchback"]
-    #     elif circuit_name.startswith("RB"):
-    #         return "MB"
-    #     elif circuit_name.startswith("RCBX"):
-    #         return ["MCBXH", "MCBXV"]
-    #     elif circuit_name.startswith("RSS"):
-    #         return ["MSS", "MSS_quenchback"]
-    #     elif circuit_name.startswith(("ROD", "ROF")):
-    #         return ["MO", "MO_quenchback"]
-    #     elif circuit_name.startswith(("RSD", "RSF")):
-    #         return ["MS", "MS_quenchback"]
-    #     elif simulation_name == "RCD":
-    #         return ["MCD", "MCD_quenchback"]
-    #     elif simulation_name == "RCO":
-    #         return ["MCO", "MCO_quenchback"]
-
-    # def __get_number_of_magnets(self,circuit_name: str, simulation_name: str, circuit_type: str):
-    #     circuit_family_name = get_circuit_family_from_circuit_name(circuit_name)
-    #     #circuit_type = self.__get_circuit_type(circuit_name, self.library_path)
-    #     if circuit_type in ["RCS", "RB"]:
-    #         return 154
-    #     elif circuit_type in ["RCD", "RCO"]:
-    #         return 77
-    #     elif circuit_name.startswith("RQ6.") and len(circuit_name) == 8:
-    #         return 6
-    #     elif circuit_name.startswith(("RQS.R", "RQS.L", "RQTL9")):
-    #         return 2
-    #     elif circuit_name.startswith(("RQS.A", "RSS", "RQX")):
-    #         return 4
-    #     elif circuit_name.startswith(("RQTD", "RQTF")):
-    #         return 8
-    #     elif circuit_family_name in ["60A", "IPD", "80-120A", "600A"]:
-    #         return 1
-    #     elif circuit_type == "RQ_47magnets":
-    #         return 47
-    #     elif circuit_type == "RQ_51magnets":
-    #         return 51
-    #     elif circuit_family_name == "IPQ":
-    #         return int(int(re.search(r'_(\d+)_', simulation_name).group(1))/2)
-
-    # def __get_number_of_apertures(self, circuit_name: str):
-    #     circuit_family_name = get_circuit_family_from_circuit_name(circuit_name)
-    #     if circuit_family_name in ["IPQ", "RB"]:
-    #         return 2
-    #     else:
-    #         return 1
-
     def __get_magnets_list(self, number_of_magnets: int):
         list = []
         for i in range(1, number_of_magnets+1):
             list.append(i)
         return list
 
-    # def __get_magnet_types_list(self, number_of_magnets: int, simulation_name: str):
-    #     list = []
-    #     if number_of_magnets == 4 and simulation_name.startswith("RQX"): #to be improved
-    #         list = [1, 2, 2, 1]
-    #     elif simulation_name.startswith("IPQ") and number_of_magnets == 2:
-    #         list = [1, 2]
-    #     elif simulation_name.startswith("RB"):
-    #         for i in range(1, number_of_magnets+1):
-    #             list.append(1)
-    #     elif number_of_magnets in [154, 13, 8, 77, 6, 12, 11, 10, 9, 4, 2]:
-    #         list = [1] + [2] * (number_of_magnets - 1)
-    #     else:
-    #         for i in range(1, number_of_magnets+1):
-    #             list.append(1)
-    #     return list
-
-    # def __get_circuit_type(self, circuit_name: str, library_path, simulation_name: str = None):
-    #     # if simulation_name:
-    #     #     assert(self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name == simulation_name)
-    #     #     #assert(True == False)
-    #     if circuit_name.startswith("RCBH") or circuit_name.startswith("RCBV"):
-    #         return "RCB"
-    #     elif circuit_name.startswith(("RD1", "RD2", "RD3", "RD4")):
-    #         return {"RD1": "RD1", "RD2": "RD2", "RD3": "RD3", "RD4": "RD4"}.get(circuit_name[:3], "No match found")
-    #     elif circuit_name.startswith("RQX"):
-    #         return "RQX"
-    #     elif circuit_name.startswith(("RQ4", "RQ5", "RQ6", "RQ7", "RQ8", "RQ9", "RQ10")):
-    #         return circuit_name.split(".")[0]
-    #     elif circuit_name.startswith(("RQT12", "RQT13")):
-    #         return "RQT_12_13"
-    #     elif circuit_name.startswith(("RQTL7", "RQTL8", "RQTL10", "RQTL11")):
-    #         return "RQTL_7_8_10_11"
-    #     elif circuit_name.startswith("RQTL9"):
-    #         return "RQTL9"
-    #     elif circuit_name.startswith(("RQTD", "RQTF")):
-    #         return "RQT"
-    #     elif circuit_name.startswith("RQSX3"):
-    #         return "RQSX3"
-    #     elif circuit_name.startswith("RQS"):
-    #         return "RQS"
-    #     elif circuit_name.startswith("RQ."):
-    #         circuit_name_temp = circuit_name.replace(".", "D_")
-    #         magnet_number = find_n_magnets_in_circuit(os.path.join(library_path, f"circuits/circuit_parameters/RQ_circuit_parameters.csv"), circuit_name_temp)
-    #         return f"RQ_{magnet_number}magnets"
-    #     elif circuit_name.startswith("RCS"):
-    #         return "RCS"
-    #     elif circuit_name.startswith("RB"):
-    #         return "RB"
-    #     elif circuit_name.startswith("RCBX"):
-    #         return "RCBX"
-    #     elif circuit_name.startswith("RCBC"):
-    #         return "RCBC"
-    #     elif circuit_name.startswith("RCBY"):
-    #         return "RCBY"
-    #     elif circuit_name.startswith("RSS"):
-    #         return "RSS"
-    #     elif circuit_name.startswith(("RSD")):
-    #         magnet_number = find_n_magnets_in_circuit(os.path.join(library_path, f"circuits/circuit_parameters/600A_circuit_parameters.csv"), circuit_name)
-    #         return f"RSD_{magnet_number}magnets"
-    #     elif circuit_name.startswith(("RSF")):
-    #         magnet_number = find_n_magnets_in_circuit(os.path.join(library_path, f"circuits/circuit_parameters/600A_circuit_parameters.csv"), circuit_name)
-    #         return f"RSF_{magnet_number}magnets"
-    #     elif circuit_name.startswith(("RO")):
-    #         magnet_number = find_n_magnets_in_circuit(os.path.join(library_path, f"circuits/circuit_parameters/600A_circuit_parameters.csv"), circuit_name)
-    #         return f"RO_{magnet_number}magnets"
-    #     elif simulation_name == "RCD": #improvement pending
-    #         return "RCD"
-    #     elif simulation_name == "RCO": #improvement pending
-    #         return "RCO"
-
-    # def __get_quenching_magnet_number(self, position: str, circuit_family_name: str,library_path):
-    #     df = pd.read_csv(os.path.join(library_path, 'circuits', 'circuit_parameters', f"{circuit_family_name}_LayoutDetails.csv"))
-    #     mask = df['Magnet'].str.split('.').str[1] == position
-    #     result = df.loc[mask, '#Electric_circuit'].iloc[0]
-    #     return result
-
-    # def __split_csv(self, input_file_name):
-    #     # Create empty lists to hold the odd and even rows
-    #     odd_rows = []
-    #     even_rows = []
-    #
-    #     # Open the input CSV file and read in the rows
-    #     with open(input_file_name, 'r') as input_file:
-    #         reader = csv.reader(input_file)
-    #
-    #         # Save the header row
-    #         header = next(reader)
-    #
-    #         # Loop over the remaining rows and append them to the odd or even list
-    #         for i, row in enumerate(reader):
-    #             if i % 2 == 0:
-    #                 even_rows.append(row)
-    #             else:
-    #                 odd_rows.append(row)
-    #
-    #     # Write the odd and even rows to separate output files
-    #     output_odd_file_name = 'output_odd.csv'
-    #     with open(output_odd_file_name, 'w', newline='') as output_odd_file:
-    #         writer_odd = csv.writer(output_odd_file)
-    #         writer_odd.writerow(header)
-    #         writer_odd.writerows(odd_rows)
-    #
-    #     output_even_file_name = 'output_even.csv'
-    #     with open(output_even_file_name, 'w', newline='') as output_even_file:
-    #         writer_even = csv.writer(output_even_file)
-    #         writer_even.writerow(header)
-    #         writer_even.writerows(even_rows)
-    #
-    #     # Return a list of the output file names
-    #     return [output_even_file_name, output_odd_file_name]
-
-    # def __find_magnets(self, filename, key):
-    #     with open(filename, 'r') as file:
-    #         reader = csv.DictReader(file)
-    #         for row in reader:
-    #             if row['circuit'] == key:
-    #                 return row['NumberOfMagnets']
-    #         return None
-
-    # def __find_circuit_model(self, filename, key):
-    #     with open(filename, 'r') as file:
-    #         reader = csv.DictReader(file)
-    #         for row in reader:
-    #             if row['circuit'] == key:
-    #                 return row['circuit_type']
-    #         return None
-
-    # def __get_first_circuit_name(self, csv_file):
-    #     with open(csv_file, 'r') as file:
-    #         reader = csv.DictReader(file)
-    #         for row in reader:
-    #             first_entry = row.get("Circuit Name")
-    #             if first_entry:
-    #                 return first_entry
-
-    def extract_stimulus_values(self, stl_file, output_folder):
-        stimulus_pattern = re.compile(r'\.STIMULUS\s+(\S+)\s+PWL\s+([\s\S]*?)(?=\.STIMULUS|\Z)', re.IGNORECASE)
-        value_pattern = re.compile(r'\(\s*([\d.]+)\s*[s]?,\s*([\d.]+)\s*\)')
-
-        with open(stl_file, 'r') as file:
-            contents = file.read()
-
-        stimuli = stimulus_pattern.findall(contents)
-        for stimulus in stimuli:
-            stimulus_name = stimulus[0]
-            stimulus_values = stimulus[1]
-
-            values = value_pattern.findall(stimulus_values)
-            values = [(value[0], value[1]) for value in values]  # Remove 's' from the first entry
-
-            csv_file_name = stimulus_name + '.csv'
-            csv_file_path = os.path.join(output_folder, csv_file_name)
-
-            with open(csv_file_path, 'w', newline='') as csv_file:
-                writer = csv.writer(csv_file)
-                writer.writerows(values)
-
-            print(f"Created CSV file: {csv_file_path}")
-
-    def _get_local_folder(self, selected_local_folder: str):
-        '''
-        ** Return the local tool folder after resolving the logic **
-        - The path to the selected local tool folder is read from the settings
-        - If the path is absolute, the path is simply returned
-        - If the path is relative, the path is resolved with respect to location of the original STEAM analysis yaml file (self.path_analysis_file)
-        :param selected_local_folder: Selected local folder to load from the settings
-        :return:
-        '''
-        path_from_settings = getattr(self.settings, selected_local_folder)
-        local_model_folder = Path(path_from_settings) if os.path.isabs(path_from_settings) else Path(os.getcwd() / Path(path_from_settings)).resolve()
-        return local_model_folder
+    # def _get_local_folder(self, selected_local_folder: str):
+    #     '''
+    #     ** Return the local tool folder after resolving the logic **
+    #     - The path to the selected local tool folder is read from the settings
+    #     - If the path is absolute, the path is simply returned
+    #     - If the path is relative, the path is resolved with respect to location of the original STEAM analysis yaml file (self.path_analysis_file)
+    #     :param selected_local_folder: Selected local folder to load from the settings
+    #     :return:
+    #     '''
+    #     path_from_settings = getattr(self.settings, selected_local_folder)
+    #     local_model_folder = Path(path_from_settings) if os.path.isabs(path_from_settings) else Path(os.path.join(os.path.dirname(self.path_analysis_file), Path(path_from_settings))).resolve()
+    #     return local_model_folder
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py` & `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py` & `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py` & `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py` & `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py` & `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py` & `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py` & `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py` & `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py` & `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py` & `steam-sdk-2024.4.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/builders/BuilderAPDL_CT.py` & `steam-sdk-2024.4.0/steam_sdk/builders/BuilderAPDL_CT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/builders/BuilderCosim.py` & `steam-sdk-2024.4.0/steam_sdk/builders/BuilderCosim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/builders/BuilderFiQuS.py` & `steam-sdk-2024.4.0/steam_sdk/builders/BuilderFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/builders/BuilderLEDET.py` & `steam-sdk-2024.4.0/steam_sdk/builders/BuilderLEDET.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from steam_sdk.data.DataRoxieParser import RoxieData
 from steam_sdk.data.TemplateLEDET import get_template_LEDET_inputs_sheet, get_template_LEDET_options_sheet, \
     get_template_LEDET_plots_sheet, get_template_LEDET_variables_sheet
 from steam_sdk.parsers.ParserRoxie import ParserRoxie
 from steam_sdk.plotters.PlotterModel import PlotterModel
 
 
+
 class BuilderLEDET:
     """
         Class to generate LEDET models
     """
 
     def __init__(self, path_input_file: Path = None, input_model_data=None,
                  input_roxie_data: RoxieData = None, input_map2d: str = None,
@@ -198,28 +199,30 @@
             :param path_map2d: Input .map2d file. Note: By default, read the .map2d file defined in the yaml input file
             :type path_map2d: Path
 
             :return: None
         """
         pR = ParserRoxie()
         (nT, nStrands_inGroup_ROXIE, polarities_inGroup, strandToHalfTurn, strandToGroup, indexTstart, indexTstop,
-         x_strands, y_strands, I_strands) = pR.loadParametersFromMap2d(model_data=self.model_data,
+         x_strands, y_strands, I_strands, Bx, By) = pR.loadParametersFromMap2d(model_data=self.model_data,
                                                                        path_input_file=self.path_input_file,
                                                                     path_map2d=path_map2d)
 
         self.setAttribute(self.Inputs,    'nT', nT)
         self.setAttribute(self.Auxiliary, 'nStrands_inGroup_ROXIE', nStrands_inGroup_ROXIE)
         self.setAttribute(self.Inputs,    'polarities_inGroup', polarities_inGroup)
         self.setAttribute(self.Auxiliary, 'strandToHalfTurn', strandToHalfTurn)
         self.setAttribute(self.Auxiliary, 'strandToGroup', strandToGroup)
         self.setAttribute(self.Auxiliary, 'indexTstart', indexTstart)
         self.setAttribute(self.Auxiliary, 'indexTstop', indexTstop)
         self.setAttribute(self.Auxiliary, 'x_strands', x_strands)
         self.setAttribute(self.Auxiliary, 'y_strands', y_strands)
         self.setAttribute(self.Auxiliary, 'I_strands', I_strands)
+        self.setAttribute(self.Auxiliary, 'Bx', Bx)
+        self.setAttribute(self.Auxiliary, 'By', By)
 
         if flag_plot:
             PM = PlotterModel(self.roxie_data)
             PM.plot_conductor_numbering(self.model_data, strandToGroup, strandToHalfTurn, polarities_inGroup, x_strands, y_strands)
 
     def get_roxie_param(self, roxie_param=None, flag_plot: bool = False):
         """
@@ -351,15 +354,17 @@
         self.Lp_s_inGroup = np.array([])
         self.R_c_inGroup = np.array([])
         self.overwrite_f_internalVoids_inGroup = np.array([])
         self.overwrite_f_externalVoids_inGroup = np.array([])
         # Initialize Strand variables that need to be set by this method
         self.SCtype_inGroup = np.array([], dtype=np.uint32)
         self.STtype_inGroup = np.array([], dtype=np.uint32)
+        self.dcore_inGroup = np.array([])
         self.ds_inGroup = np.array([])
+        self.dfilamentary_inGroup = np.array([])
         self.f_SC_strand_inGroup = np.array([])
         self.RRR_Cu_inGroup = np.array([])
         self.Lp_f_inGroup = np.array([])
         self.f_ro_eff_inGroup = np.array([])
         self.df_inGroup = np.array([])
         # Initialize Jc-fit variables that need to be set by this method
         self.Tc0_NbTi_ht_inGroup = np.array([])
@@ -417,14 +422,16 @@
         self.setAttribute(self.Inputs, 'R_c_inGroup', self.R_c_inGroup)
         self.setAttribute(self.Inputs, 'overwrite_f_internalVoids_inGroup', self.overwrite_f_internalVoids_inGroup)
         self.setAttribute(self.Inputs, 'overwrite_f_externalVoids_inGroup', self.overwrite_f_externalVoids_inGroup)
         # Assign loaded Strand variables
         self.setAttribute(self.Inputs, 'SCtype_inGroup', self.SCtype_inGroup)
         self.setAttribute(self.Inputs, 'STtype_inGroup', self.STtype_inGroup)
         self.setAttribute(self.Inputs, 'ds_inGroup', self.ds_inGroup)
+        self.setAttribute(self.Inputs, 'dcore_inGroup', self.dcore_inGroup)
+        self.setAttribute(self.Inputs, 'dfilamentary_inGroup', self.dfilamentary_inGroup)
         self.setAttribute(self.Inputs, 'f_SC_strand_inGroup', self.f_SC_strand_inGroup)
         self.setAttribute(self.Inputs, 'RRR_Cu_inGroup', self.RRR_Cu_inGroup)
         self.setAttribute(self.Inputs, 'Lp_f_inGroup', self.Lp_f_inGroup)
         self.setAttribute(self.Inputs, 'f_ro_eff_inGroup', self.f_ro_eff_inGroup)
         self.setAttribute(self.Inputs, 'df_inGroup', self.df_inGroup)
         # Assign loaded Jc-fit variables
         self.setAttribute(self.Inputs, 'Tc0_NbTi_ht_inGroup', self.Tc0_NbTi_ht_inGroup)
@@ -513,27 +520,31 @@
             self.STtype_inGroup      = np.append(self.STtype_inGroup,      DictionaryLEDET.lookupStabilizer(conductor.strand.material_stabilizer))
             self.ds_inGroup          = np.append(self.ds_inGroup,          conductor.strand.diameter)
             self.f_SC_strand_inGroup = np.append(self.f_SC_strand_inGroup, 1 / (1 + conductor.strand.Cu_noCu_in_strand))  # f_SC=1/(1+Cu_noCu)
             self.RRR_Cu_inGroup      = np.append(self.RRR_Cu_inGroup,      conductor.strand.RRR)
             self.Lp_f_inGroup        = np.append(self.Lp_f_inGroup,        conductor.strand.fil_twist_pitch)
             self.f_ro_eff_inGroup    = np.append(self.f_ro_eff_inGroup,    conductor.strand.f_Rho_effective)
             self.df_inGroup          = np.append(self.df_inGroup,          conductor.strand.filament_diameter)
+            self.dcore_inGroup       = np.append(self.dcore_inGroup,       np.array(conductor.strand.diameter_core, dtype=float))
+            self.dfilamentary_inGroup= np.append(self.dfilamentary_inGroup,np.array(conductor.strand.diameter_filamentary, dtype=float))
         elif type_strand == 'Rectangular':
             self.SCtype_inGroup      = np.append(self.SCtype_inGroup,      DictionaryLEDET.lookupSuperconductor(conductor.strand.material_superconductor))
             self.STtype_inGroup      = np.append(self.STtype_inGroup,      DictionaryLEDET.lookupStabilizer(conductor.strand.material_stabilizer))
             if conductor.strand.bare_corner_radius:     # if bare corner radius is specified take it into account
                 wire_area = (conductor.strand.bare_width * conductor.strand.bare_height) - ((4 - np.pi) * conductor.strand.bare_corner_radius ** 2)
             else:   # if it is None, treat it as zero and and conductor as perfectly rectangular
                 wire_area = conductor.strand.bare_width * conductor.strand.bare_height
             self.ds_inGroup          = np.append(self.ds_inGroup,          np.sqrt(wire_area * 4 / np.pi))
             self.f_SC_strand_inGroup = np.append(self.f_SC_strand_inGroup, 1 / (1 + conductor.strand.Cu_noCu_in_strand))  # f_SC=1/(1+Cu_noCu)
             self.RRR_Cu_inGroup      = np.append(self.RRR_Cu_inGroup,      conductor.strand.RRR)
             self.Lp_f_inGroup        = np.append(self.Lp_f_inGroup,        conductor.strand.fil_twist_pitch)
             self.f_ro_eff_inGroup    = np.append(self.f_ro_eff_inGroup,    conductor.strand.f_Rho_effective)
             self.df_inGroup          = np.append(self.df_inGroup,          conductor.strand.filament_diameter)
+            # self.dfilamentary_inGroup = np.append(self.dfilamentary_inGroup, conductor.strand.diameter_filamentary)
+            # self.dcore_inGroup = np.append(self.dcore_inGroup, conductor.strand.diameter_core)
         else:
             raise Exception('Group #{}. Selected strand type ({}) is not supported.'.format(conductor_id, type_strand))
 
 
     def loadJcFitData(self, conductor_id):
         '''
             Load the Jc-fit parameters for one group from DataModelMagnet keys, and append them to the respective self variables
@@ -1325,29 +1336,31 @@
                                                        np.linspace(1, int(nHalfTurns / 2), int(nHalfTurns/2))))
         self.setAttribute(self.Inputs, 'HalfTurnToInductanceBlock', HalfTurnToInductanceBlock)
 
         if self.verbose:
             print('')
             print('Total magnet self-inductance per unit length: ' + str(L_magnet) + ' H/m')
 
-        # Write a csv file with the self-mutual inductance per unit length between each turn
+        # If self-mutual inductance matrix too large, set M_m to 0 and LEDET will read from the .csv file instead
+        if M_turns.shape[0] >= 201:
+            M_InductanceBlock_m = np.array([0])
+            self.setAttribute(self.Inputs, 'M_InductanceBlock_m', M_InductanceBlock_m)  # TODO: change test_BuilderModel to reflect this change
+
+        # If the csv_write_path is set to 'skip', no csv file will be written.
+        if str(csv_write_path).casefold()=='skip':
+            return
+        # If not provided, use standard path - otherwise the provided path
         if not csv_write_path:
             csv_write_path = os.path.join(name_magnet + '_selfMutualInductanceMatrix.csv')
         with open(csv_write_path, 'w', newline='') as file:
             reader = csv.writer(file)
             reader.writerow(["Self- and mutual inductances per unit length between each turn [H/m]"])
             for i in range(M_turns.shape[0]):
                 reader.writerow(M_turns[i])
 
-        # If self-mutual inductance matrix too large, set M_m to 0 and LEDET will read from the .csv file instead
-        if M_turns.shape[0] >= 201:
-            M_InductanceBlock_m = np.array([0])
-            self.setAttribute(self.Inputs, 'M_InductanceBlock_m', M_InductanceBlock_m)  # TODO: change test_BuilderModel to reflect this change
-
-
     def setSelfMutualInductances(self):
         '''
         Assign self-mutual inductance parameters (this is used when inductance calculation is not enabled
         :return:
         '''
 
         # Defining to which inductive block each half-turn belongs
@@ -1357,30 +1370,30 @@
             HalfTurnToInductanceBlock = self.Auxiliary.overwrite_HalfTurnToInductanceBlock
         else:
             if magnet_type == 'multipole':
                 HalfTurnToInductanceBlock = np.concatenate((np.linspace(1, int(nHalfTurns / 2), int(nHalfTurns / 2)), np.linspace(1, int(nHalfTurns / 2), int(nHalfTurns / 2))))
             elif (magnet_type == 'solenoid') or (magnet_type == 'busbar'):
                 HalfTurnToInductanceBlock = np.linspace(1, int(nHalfTurns), int(nHalfTurns))
             elif magnet_type in ['CCT_straight']:
-                selfMutualInductanceMatrix_csv = Path.joinpath(self.path_input_file,
-                                                               f'{self.model_data.GeneralParameters.magnet_name}_selfMutualInductanceMatrix_{str(self.model_data.Options_LEDET.input_generation_options.selfMutualInductanceFileNumber)}.csv')
-                df = pd.read_csv(selfMutualInductanceMatrix_csv, delimiter=',', engine='python', skiprows = 1, header = None)
-                self.Auxiliary.overwrite_inductance_coil_sections = float(df.to_numpy().sum())  # [:-1] to remove last nan
-                HalfTurnToInductanceBlock = [df.to_numpy()] # set to empty as it is later overwritten for CCT_straight by method self.assignCCTValuesWindings()
+                # selfMutualInductanceMatrix_csv = Path.joinpath(self.path_input_file,
+                #                                                f'{self.model_data.GeneralParameters.magnet_name}_selfMutualInductanceMatrix_{str(self.model_data.Options_LEDET.input_generation_options.selfMutualInductanceFileNumber)}.csv')
+                # df = pd.read_csv(selfMutualInductanceMatrix_csv, delimiter=',', engine='python', skiprows = 1, header = None)
+                # self.Auxiliary.overwrite_inductance_coil_sections = float(df.to_numpy().sum())  # [:-1] to remove last nan
+                HalfTurnToInductanceBlock = []  # set to empty as it is later overwritten for CCT_straight by method self.assignCCTValuesWindings()
             elif magnet_type in ['CWS']:
-                selfMutualInductanceMatrix_csv = Path.joinpath(self.path_input_file,
-                                                               f'{self.model_data.GeneralParameters.magnet_name}_selfMutualInductanceMatrix_{str(self.model_data.Options_LEDET.input_generation_options.selfMutualInductanceFileNumber)}.csv')
-                df = pd.read_csv(selfMutualInductanceMatrix_csv, delimiter=',', engine='python', skiprows=1, header=None)
-                self.Auxiliary.overwrite_inductance_coil_sections = df.to_numpy()  # [:-1] to remove last nan
-                fL_I_fL_L_file = Path.joinpath(self.path_input_file,
-                                               f'{self.model_data.GeneralParameters.magnet_name}_fL_I_fL_L_{str(self.model_data.Options_LEDET.input_generation_options.selfMutualInductanceFileNumber)}.csv')
-                df_fL_I_fL_L = pd.read_csv(fL_I_fL_L_file, delimiter=',', engine='python')
-                self.setAttribute(self.Inputs, 'fL_I', df_fL_I_fL_L['fL_I'].to_numpy())
-                self.setAttribute(self.Inputs, 'fL_L', df_fL_I_fL_L['fL_L'].to_numpy())
-                HalfTurnToInductanceBlock = [df.to_numpy()]
+                # selfMutualInductanceMatrix_csv = Path.joinpath(self.path_input_file,
+                #                                                f'{self.model_data.GeneralParameters.magnet_name}_selfMutualInductanceMatrix_{str(self.model_data.Options_LEDET.input_generation_options.selfMutualInductanceFileNumber)}.csv')
+                # df = pd.read_csv(selfMutualInductanceMatrix_csv, delimiter=',', engine='python', skiprows=1, header=None)
+                # self.Auxiliary.overwrite_inductance_coil_sections = df.to_numpy()  # [:-1] to remove last nan
+                # fL_I_fL_L_file = Path.joinpath(self.path_input_file,
+                #                                f'{self.model_data.GeneralParameters.magnet_name}_fL_I_fL_L_{str(self.model_data.Options_LEDET.input_generation_options.selfMutualInductanceFileNumber)}.csv')
+                # df_fL_I_fL_L = pd.read_csv(fL_I_fL_L_file, delimiter=',', engine='python')
+                # self.setAttribute(self.Inputs, 'fL_I', df_fL_I_fL_L['fL_I'].to_numpy())
+                # self.setAttribute(self.Inputs, 'fL_L', df_fL_I_fL_L['fL_L'].to_numpy())
+                HalfTurnToInductanceBlock = []  # set to empty as it is later overwritten
             else:
                 raise Exception(f'Magnet type not recognized: {magnet_type}.')
 
         # Self-mutual inductances between coil sections, per unit length [H/m]
         self.setAttribute(self.Inputs, 'M_m', self.Auxiliary.overwrite_inductance_coil_sections)
         self.setAttribute(self.Inputs, 'HalfTurnToInductanceBlock', HalfTurnToInductanceBlock)
         self.setAttribute(self.Inputs, 'M_InductanceBlock_m', 0)  # This entry will tell LEDET to read the turn-to-turn inductances from the auxiliary .csv file
@@ -2564,7 +2577,8 @@
 #                 print(k, self.getAttribute(variableGroup, k))
 #         else:
 #             for k in variableGroup:
 #                 if k == 'overwrite_f_internalVoids_inGroup' and len(self.getAttribute(variableGroup, k))==0: continue
 #                 if k == 'overwrite_f_externalVoids_inGroup' and len(self.getAttribute(variableGroup, k))==0: continue
 #                 print(variableLabels[k])
 #                 print(k, variableGroup[k])
+
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/builders/BuilderModel.py` & `steam-sdk-2024.4.0/steam_sdk/builders/BuilderModel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import datetime
 import os
 import shutil
 from pathlib import Path
 from typing import Union
 
 import numpy as np
+
 from steam_pysigma.MainPySIGMA import MainPySIGMA
 
 from steam_sdk.builders.BuilderAPDL_CT import BuilderAPDL_CT
 from steam_sdk.builders.BuilderFiQuS import BuilderFiQuS
 from steam_sdk.builders.BuilderLEDET import BuilderLEDET
 from steam_sdk.builders.BuilderProteCCT import BuilderProteCCT
 from steam_sdk.builders.BuilderPyBBQ import BuilderPyBBQ
 from steam_sdk.builders.BuilderPySIGMA import BuilderPySIGMA
+from steam_sdk.builders.BuilderTFM import BuilderTFM
 from steam_sdk.data.DataModelCircuit import DataModelCircuit
 from steam_sdk.data.DataModelConductor import DataModelConductor
 from steam_sdk.data.DataModelMagnet import DataModelMagnet
 from steam_sdk.data.DataRoxieParser import RoxieData
 from steam_sdk.data.DataRoxieParams import RoxieParams
 from steam_sdk.data.DataSettings import DataSettings
 from steam_sdk.parsers.ParserCsv import find_by_position, find_column_list
 from steam_sdk.parsers.ParserFiQuS import ParserFiQuS
 from steam_sdk.parsers.ParserLEDET import ParserLEDET, copy_modified_map2d_ribbon_cable, copy_map2d
-from steam_sdk.parsers.ParserMap2d import getParametersFromMap2d
+from steam_sdk.parsers.ParserMap2d import ParserMap2dFile
 from steam_sdk.parsers.ParserPSPICE import ParserPSPICE
 from steam_sdk.parsers.ParserProteCCT import ParserProteCCT
 from steam_sdk.parsers.ParserPyBBQ import ParserPyBBQ
 from steam_sdk.parsers.ParserPySIGMA import ParserPySIGMA
 from steam_sdk.parsers.ParserRoxie import ParserRoxie, RoxieList
 from steam_sdk.parsers.ParserXYCE import ParserXYCE
 from steam_sdk.parsers.ParserYAML import yaml_to_data
@@ -37,39 +39,34 @@
 
 
 class BuilderModel:
     """
         Class to generate STEAM models, which can be later on written to input files of supported programs
     """
 
-    def __init__(self,
-                 file_model_data: str = None,
-                 case_model: str = 'magnet',
-                 data_settings: DataSettings = None,
-                 results_folder_name: str = None,
-                 verbose: bool = False):
-        """
-            Builder object to generate models from STEAM simulation tools specified by user
-
-            :param file_model_data: path to folder with input data (roxie files, geometry, modelData.yaml = config from userinput)
-            :param case_model: defines whether it is a magnet, a conductor or a circuit
-            :param data_settings: DataSettings object containing all settings, previously read from user specific settings.SYSTEM.yaml file or from a STEAM analysis permanent settings
-            :param verbose: to display internal processes (output of status & error messages) for troubleshooting
-            :param local_folder_output: if set to true the path from settings file is used for each tool. If false the output_path is used.
-            :param results_folder_name: full path to where the output files will go - used in PySIGMA at the moment
+    def __init__(self, file_model_data: str = None, case_model: str = 'magnet', data_settings: DataSettings = None, verbose: bool = False):
+        """
+        Builder object to generate models for STEAM simulation tools specified by user
+        :param file_model_data: path to input yaml file
+        :type file_model_data: str
+        :param case_model: defines whether it is a magnet, a conductor or a circuit. Default is 'magnet
+        :type case_model: str
+        :param data_settings: DataSettings object containing all settings, previously read from user specific settings.SYSTEM.yaml file or from a STEAM analysis permanent settings
+        :type data_settings: DataSettings
+        :param verbose: if true display internal processes (output of status & error messages) for troubleshooting
+        :type verbose: bool
         """
 
         # Unpack arguments
         if file_model_data:
             self.file_model_data: str = file_model_data
         else:
             raise Exception('No file_model_data .yaml input file provided.')
         self.case_model = case_model
         self.settings_dict = data_settings
-        self.results_folder_name = results_folder_name
         self.verbose: bool = verbose
 
         if self.verbose:
             print(f'case_model: {self.case_model}')
             print('Settings:')
             [print(attr, getattr(self.settings_dict, attr)) for attr in
              self.settings_dict.__dict__.keys()]  # Print all settings
@@ -88,14 +85,15 @@
 
             # Load model data from the input .yaml file
             self.loadModelData()
 
             # Set paths of input files
             self.set_input_paths()
 
+
         ### Case of a circuit model
         elif self.case_model == 'circuit':
             # Initialize
             self.circuit_data: DataModelCircuit = DataModelCircuit()
 
             # Load model data from the input .yaml file
             self.loadModelData()
@@ -477,18 +475,16 @@
                     # TODO: geometry when conductor has a combination of ribbon and non-ribbon cables
 
                     # List of flags that are True is the cable type is "Ribbon"
                     list_flag_ribbon = []
                     for i, cond in enumerate(self.model_data.CoilWindings.conductor_to_group):
                         list_flag_ribbon.append(self.model_data.Conductors[cond - 1].cable.type == 'Ribbon')
 
-                    nT_from_original_map2d, nStrands_inGroup_original_map2d, _, _, _, _, _, _ = getParametersFromMap2d(
-                        map2dFile=self.path_map2d,
-                        headerLines=self.model_data.Options_LEDET.field_map_files.headerLines,
-                        verbose=verbose)
+                    nT_from_original_map2d, nStrands_inGroup_original_map2d, _, _, _, _, _, _ =\
+                        ParserMap2dFile(map2dFile=self.path_map2d).getParametersFromMap2d(headerLines=self.model_data.Options_LEDET.field_map_files.headerLines)
 
                     n_groups_original_file = len(nT_from_original_map2d)
                     geometry_ribbon_cable = []
 
                     for i in range(n_groups_original_file):
                         list = [None, None]
                         list[0] = int(nStrands_inGroup_original_map2d[i])  # layers
@@ -671,33 +667,14 @@
         path_file_name = os.path.join(output_path, f'{sim_name}{sim_suffix}.cir')  # full path of the PSPICE netlist to write
         parser_pspice.write2pspice(full_path_file_name=path_file_name, verbose=verbose)
         if verbose: print(f'Simulation file {path_file_name} generated.')
 
         # Copy additional files
         parser_pspice.copy_additional_files(output_path=output_path, verbose=verbose)
 
-    def buildXYCE(self, sim_name: str, sim_number: Union[int, str], output_path: str, verbose: bool = None):
-        """
-            Build a XYCE circuit netlist model
-            :param sim_name: Simulation name that will be used to write the output file
-            :param sim_number: Simulation number or string that will be used to write the output file
-            :param output_path: Output folder
-            :param verbose: If True, display logging information
-        """
-        verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
-        sim_suffix = f'_{sim_number}' if isinstance(sim_number, int) else sim_number
-        make_folder_if_not_existing(output_path, verbose=verbose)
-
-        # Write output .cir file
-        parser_xyce = ParserXYCE(circuit_data=self.circuit_data, path_input=self.path_input_file, output_path=output_path)
-        path_file_name = os.path.join(output_path, f'{sim_name}{sim_suffix}.cir')  # full path of the XYCE netlist to write
-        parser_xyce.write2XYCE(path_file_name, verbose=verbose)
-        parser_xyce.copy_additional_files(flag_translate=True, verbose=verbose)
-        parser_xyce.resolve_paths_netlist(path_file_name)
-
     def buildPyBBQ(self, sim_name: str, sim_number: Union[int, str], output_path: str, verbose: bool = None):
         """
             Build a PyBBQ model
             :param sim_name: Simulation name that will be used to write the output file
             :param sim_number: Simulation number or string that will be used to write the output file
             :param output_path: Output folder
             :param verbose: If True, display logging information
@@ -710,51 +687,134 @@
         builder_PyBBQ = BuilderPyBBQ(input_model_data=self.conductor_data, flag_build=True, verbose=verbose)
 
         # Write output yaml file
         parser_PyBBQ = ParserPyBBQ(builder_PyBBQ)
         path_file_name = os.path.join(output_path, f'{conductor_name}{sim_suffix}.yaml')  # full path of the PyBBQ input file to write
         parser_PyBBQ.writePyBBQ2yaml(full_path_file_name=path_file_name, verbose=verbose)
 
-    def buildPySIGMA(self, sim_name: str, sim_number: Union[int, str], output_path: str, make_bh_copy=True,
+    def buildPySIGMA(self, sim_name: str, sim_number: Union[int, str], output_path: str,
                      flag_plot_all: bool = False, verbose: bool = None):
         """
-            Build a pySIGMA input files
-            :param sim_name: Simulation name that will be used to write the output file
-            :param sim_number: Simulation number or string that will be used to write the output file
-            :param output_path: Output folder
-            :param make_bh_copy: TODO
-            :param flag_plot_all: Display figures
-            :param verbose: If True, display logging information
+        Write PySIGMA input files
+        :param sim_name: Simulation name that will be used to write the output file
+        :type sim_name: str
+        :param sim_number: Simulation number or string that will be used to write the output file
+        :type sim_number: Union[int, str]
+        :param output_path: Output folder
+        :type output_path: str
+        :param flag_plot_all: Display figures
+        :type flag_plot_all: bool
+        :param verbose: If True, display logging information
+        :type verbose: bool
+        :return: Nothing, writes PySIGMA yaml input file and all other required files
+        :rtype: None
         """
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
         sim_suffix = f'_{sim_number}' if isinstance(sim_number, int) else sim_number  # TODO DISCUSS
         make_folder_if_not_existing(output_path, verbose=verbose)
 
         # Load model data from the input ROXIE files
         if self.model_data.GeneralParameters.magnet_type in ['multipole', 'busbar']:
             self.loadRoxieData()
         # Calculate half-turn electrical order
         self.calc_electrical_order(flag_plot=flag_plot_all, verbose=verbose)
 
         # output_path = os.path.join(self.settings_dict.local_SIGMA_folder, f'{sim_name}{sim_suffix}')
 
-        builder_PySIGMA = BuilderPySIGMA(model_data=self.model_data, roxie_data=self.roxie_data, path_model_folder=self.path_input_file, make_bh_copy=make_bh_copy)
+        builder_PySIGMA = BuilderPySIGMA(model_data=self.model_data, roxie_data=self.roxie_data, path_model_folder=self.path_input_file)
         self.parser_SIGMA = ParserPySIGMA(builder_PySIGMA, output_path=output_path)
         self.parser_SIGMA.writeSIGMA2yaml(simulation_name=f'{sim_name}{sim_suffix}')  # TODO DISCUSS
         coordinate_file_path = self.parser_SIGMA.coordinate_file_preprocess(model_data=self.model_data)
         # Call mainPySIGMA which generates the Java files.
         input_yaml_file_path = os.path.join(output_path, f'{sim_name}{sim_suffix}.yaml')  # TODO DISCUSS
         mps = MainPySIGMA(model_folder=output_path)  # TODO DISCUSS
-        mps.build(input_yaml_file_path=input_yaml_file_path, input_coordinates_path=coordinate_file_path, results_folder_name=self.results_folder_name, settings=self.settings_dict)  # TODO DISCUSS
+        mps.build(input_yaml_file_path=input_yaml_file_path, input_coordinates_path=coordinate_file_path, results_folder_name='output', settings=self.settings_dict)  # TODO DISCUSS
 
         if flag_plot_all:
             PlotterRoxie.plot_all(self.roxie_data)
             PM = PlotterModel(self.roxie_data)
             PM.plot_all(self.model_data)
 
+    def buildTFM(self, output_path: str, T: float, flag_PC:bool = False, flag_IFCC:bool = False, flag_ISCC:bool = False,
+                                flag_Wedges:bool = False, flag_ColdBore:bool = False, flag_EC:bool = False, flag_Roxie:bool = False,
+                                flag_BS: bool = False, flag_Mutual: bool = False, Field_interp_value: float = None):
+        """
+            Building a TFM model
+        """
+
+        magnet_name = self.model_data.GeneralParameters.magnet_name
+        builder_ledet = BuilderLEDET(path_input_file=self.path_input_file, input_model_data=self.model_data,
+                                     input_map2d=self.path_map2d, flag_build=True, input_roxie_data=self.roxie_data,
+                                     smic_write_path='skip')
+        self.builderTFM = BuilderTFM(magnet_name=magnet_name, builder_LEDET=builder_ledet, T=T, output_path=output_path,
+                                    flag_PC=flag_PC, flag_IFCC=flag_IFCC, flag_ISCC=flag_ISCC,
+                                    flag_Wedges=flag_Wedges, flag_ColdBore=flag_ColdBore, flag_EC=flag_EC, flag_Roxie=flag_Roxie,
+                                    flag_BS=flag_BS, Field_interp_value=Field_interp_value, flag_Mutual=flag_Mutual)
+
+    def buildXYCE(self, sim_name: str, sim_number: Union[int, str], output_path: str, verbose: bool = None):
+        """
+            Build a XYCE circuit netlist model
+            :param sim_name: Simulation name that will be used to write the output file
+            :param sim_number: Simulation number or string that will be used to write the output file
+            :param output_path: Output folder
+            :param verbose: If True, display logging information
+        """
+        verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
+        sim_suffix = f'_{sim_number}' if isinstance(sim_number, int) else sim_number
+        make_folder_if_not_existing(output_path, verbose=verbose)
+
+        if self.circuit_data.TFM != None:
+            TFM = self.circuit_data.TFM
+            # Save each element inside TFM which is not Magnet (flags, T, M_IF_PC) inside the GlobalParameters class of circuit_data
+            # format: 'flag_PC' = value
+            for key, value in TFM.__dict__.items():
+                if key != 'Magnets':
+                    self.circuit_data.GlobalParameters.global_parameters[key] = value
+                    if key == 'T':
+                        if value is not None:
+                            T = value
+                        else:
+                            T = 1.9
+
+            Magnets = self.circuit_data.TFM.Magnets
+            for key, Magnet in Magnets.items():
+                # For each magnet element, calls TFM to build the model
+                file_model_data_TFM = os.path.join(self.settings_dict.local_library_path,  'magnets', Magnet.name, 'input', f'modelData_{Magnet.name}.yaml')
+                bM_TFM = BuilderModel(file_model_data=file_model_data_TFM)
+                output_path_TFM = os.path.join(output_path, 'TFM_' + key)
+                if Magnet.Field_interp_value is None:
+                    Magnet.Field_interp_value = T
+                bM_TFM.buildTFM(output_path=output_path_TFM, T=T, flag_PC=TFM.flag_PC, flag_IFCC=TFM.flag_IFCC, flag_ISCC=TFM.flag_ISCC,
+                                flag_Wedges=TFM.flag_Wedges, flag_ColdBore=TFM.flag_ColdBore, flag_EC=TFM.flag_EC, flag_Roxie=TFM.flag_Roxie,
+                                flag_BS = TFM.flag_BS,  Field_interp_value=Magnet.Field_interp_value, flag_Mutual = TFM.flag_Mutual)
+                # Save the library in which the magnet models have been created
+                if output_path_TFM not in self.circuit_data.Libraries.component_libraries:
+                    self.circuit_data.Libraries.component_libraries.append(output_path_TFM)
+                if output_path_TFM not in self.circuit_data.GeneralParameters.additional_files:
+                    self.circuit_data.GeneralParameters.additional_files.append(output_path_TFM)
+                # Add the corresponding Lmag and C_ground of each magnet to the global parameters in the format 'Lmag_x_Magnet_1' = value
+                self.circuit_data.GlobalParameters.global_parameters[f'L_mag_{key}'] = Magnet.L_mag
+                self.circuit_data.GlobalParameters.global_parameters[f'C_ground_{key}'] = Magnet.C_ground
+                self.circuit_data.GlobalParameters.global_parameters[f'Field_interp_value_{key}'] = Magnet.Field_interp_value
+
+                # Add for each magnet the corresponding Lmag and C_ground to the netlist parameters in the format 'Lmag' = 'Lmag_x_Magnet_1'
+                self.circuit_data.Netlist[key].parameters['L_mag']= f'L_mag_{key}'
+                self.circuit_data.Netlist[key].parameters['C_ground'] = f'C_ground_{key}'
+                self.circuit_data.Netlist[key].parameters['Field_interp_value'] = f'Field_interp_value_{key}'
+                for flag in TFM.__dict__.keys():
+                    if flag != 'Magnets':
+                        # Add for each magnet the corresponding flags to the netlist parameters in the format  'flag_PC' = 'flag_PC'
+                        self.circuit_data.Netlist[key].parameters[flag] = flag
+
+        # Write output .cir file
+        parser_xyce = ParserXYCE(circuit_data=self.circuit_data, path_input=self.path_input_file, output_path=output_path)
+        path_file_name = os.path.join(output_path, f'{sim_name}{sim_suffix}.cir')  # full path of the XYCE netlist to write
+        parser_xyce.write2XYCE(path_file_name, flag_resolve_library_paths=True, flag_copy_additional_files=True, verbose=verbose)
+
+
     def load_circuit_parameters_from_csv(self, input_file_name: str, selected_circuit_name: str = None, verbose: bool = False):
         '''
             Load circuit parameters from a csv file into a case=circuit object
             :param input_file_name: full path to the csv file
             :param selected_circuit_name: name of the circuit name whose parameters will be loaded
         '''
         verbose = verbose if verbose is not None else self.verbose  # if verbose is not defined, take its value from self
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/builders/BuilderProteCCT.py` & `steam-sdk-2024.4.0/steam_sdk/builders/BuilderProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/builders/BuilderPyBBQ.py` & `steam-sdk-2024.4.0/steam_sdk/builders/BuilderPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/builders/BuilderPySIGMA.py` & `steam-sdk-2024.4.0/steam_sdk/builders/BuilderPySIGMA.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,30 +8,24 @@
 
 
 class BuilderPySIGMA:
     """
         Class to generate FiQuS models
     """
 
-    def __init__(self,
-                 model_data: DataModelMagnet = None,
-                 roxie_data=None,
-                 path_model_folder=None,
-                 make_bh_copy=None):
+    def __init__(self, model_data: DataModelMagnet = None, roxie_data=None, path_model_folder=None):
         """
         Object is initialized by defining FiQuS variable structure and file template.
         :param model_data: DataModelMagnet object
         :param roxie_data: RoxieData object
         :param path_model_folder: full path to model folder
-        :param make_bh_copy: if set to true, later parser will copy the bh curve roxie file to the model folder. Here this input is set to adjust path to the bh curve in the model data
         """
 
         # Data structure
         self.path_model_folder = path_model_folder
-        self.make_bh_copy = make_bh_copy
         self.data_SIGMA = DataPySIGMA(magnet={'type': model_data.GeneralParameters.magnet_type})
         self.data_SIGMA_geo = MultipoleRoxieGeometry()
         self.data_SIGMA_geo.Roxie_Data = RoxieData(**roxie_data.dict())
         self.data_SIGMA_set = MultipoleSettings()
         self.model_data=model_data
 
         # set file
@@ -101,19 +95,15 @@
                 conductor.Jc_fit.C2_CUDI1 = cond.Jc_fit.C2_CUDI1
             else:
                 conductor.Jc_fit.C1_CUDI1 = 0.0
                 conductor.Jc_fit.C2_CUDI1 = 0.0
 
 
         # --------- sources  ----------
-        if make_bh_copy:
-            absolute_roxie_path = str(Path(model_data.Sources.BH_fromROXIE).name)
-        else:
-            absolute_roxie_path = str(Path(self.path_model_folder, model_data.Sources.BH_fromROXIE).resolve())
-        self.data_SIGMA.Sources.bh_curve_source = absolute_roxie_path
+        self.data_SIGMA.Sources.bh_curve_source = str(Path(self.path_model_folder, model_data.Sources.BH_fromROXIE).resolve())
 
         # --------- general params  ----------
         self.data_SIGMA.GeneralParameters.magnet_name = model_data.GeneralParameters.magnet_name
         self.data_SIGMA.GeneralParameters.T_initial = model_data.GeneralParameters.T_initial
         self.data_SIGMA.GeneralParameters.magnetic_length = model_data.GeneralParameters.magnetic_length
 
         # --------- power supply  ----------
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/builders/SelfMutualInductanceCalculation.py` & `steam-sdk-2024.4.0/steam_sdk/builders/SelfMutualInductanceCalculation.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/builders/Solenoids.py` & `steam-sdk-2024.4.0/steam_sdk/builders/Solenoids.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/builders/geometricFunctions.py` & `steam-sdk-2024.4.0/steam_sdk/builders/geometricFunctions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/configs/tools_defaults/ToolDefaultReader.py` & `steam-sdk-2024.4.0/steam_sdk/configs/tools_defaults/ToolDefaultReader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/cosims/CoSimPyCoSim.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/ParserCOSIM.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,293 +1,281 @@
+import json
 import os
-import shutil
-from pathlib import Path
-from typing import Union, List
+from typing import Union
 
 from steam_sdk.data.DataCoSim import NSTI
-from steam_sdk.data.DataFiQuS import DataFiQuS
-from steam_sdk.data.DataModelCosim import sim_FiQuS, sim_LEDET, sim_PSPICE, sim_XYCE, sim_Generic, FileToCopy
-from steam_sdk.data.DataPyCoSim import DataPyCoSim
+from steam_sdk.data.DataModelCosim import DataModelCosim, sim_PSPICE
 from steam_sdk.data.DataSettings import DataSettings
-from steam_sdk.drivers.DriverFiQuS import DriverFiQuS
-from steam_sdk.drivers.DriverLEDET import DriverLEDET
-from steam_sdk.drivers.DriverPSPICE import DriverPSPICE
-from steam_sdk.drivers.DriverXYCE import DriverXYCE
-from steam_sdk.parsers.ParserYAML import yaml_to_data
 from steam_sdk.parsers.utils_ParserCosims import write_model_input_files
 from steam_sdk.utils.make_folder_if_not_existing import make_folder_if_not_existing
 
 
-class CosimPyCoSim:
+class ParserCOSIM:
     """
-        Class to run a co-operative simulation
+        Class with methods to read/write COSIM information from/to other programs
     """
 
-    def __init__(self,
-                 file_model_data: str,
-                 sim_number: int,
-                 data_settings: DataSettings = None,
-                 verbose: bool = False
-                 ):
-        """
-            Builder object to generate models from STEAM simulation tools specified by user
-
-            file_model_data: path to folder with input data (DataPyCoSim yaml input file)
-            sim_number: number of the simulation
-            :param data_settings: DataSettings object containing all settings, previously read from user specific settings.SYSTEM.yaml file or from a STEAM analysis permanent settings
-            verbose: to display internal processes (output of status & error messages) for troubleshooting
-
-            Notes:
-            The PyCoSim folder structure will be as follows:
-            - local_PyCoSim is the main folder
-              - COSIM_NAME
-                - SOFTWARE_FOLDER
-                  - SIMULATION_NAME
-                    - {COSIM_NUMBER}_{SIMULATION_NUMBER}_{TIME_WINDOW_NUMBER}_{ITERATION_NUMBER}
-
-            Example 1:
-            - C:\local_PyCoSim
-              - RQX
-                - LEDET
-                  - MQXA
-                    - Field Maps
-                    - 55_1_1_1\LEDET\Input
-                  - MQXA
-                    - 55_2_1_1
-                  - MQXB
-                    - 55_1_1_1
-                  - MQXB
-                    - 55_2_1_1
-
-            Example 1:
-            - C:\local_PyCoSim
-              - RQX
-                - FiQuS
-                  - MQXA
-                    - G1
-                      - M1
-                        - 55_1_1_1
-                - LEDET
-                  - MQXB
-                    - Field Maps
-                    - 55
-                     - 1_1_1\LEDET\Input
-                - PSPICE
-                  - RQX_cosim
-                    - 55_1_1_1
-
-            D:\library_mesh
-
-        """
-        # Load data from input file
-        self.cosim_data: DataPyCoSim = yaml_to_data(file_model_data, DataPyCoSim)
-        self.local_PyCoSim_folder = Path(data_settings.local_PyCoSim_folder).resolve()
-        self.sim_number = sim_number
+    def __init__(self, cosim_data: DataModelCosim, data_settings: DataSettings = None):
+        '''
+        :param cosim_data: DataModelCosim object containing co-simulation parameter structure
+        :param data_settings: DataSettings object containing all settings, previously read from user specific settings.SYSTEM.yaml file or from a STEAM analysis permanent settings
+        '''
+
+        # Load co-simulation data from the BuilderModel object
+        self.cosim_data = cosim_data
         self.data_settings = data_settings
-        self.verbose = verbose
-        self.summary = {}  # This will be populated with a summary of simulation results (mainly used ofr DAKOTA)
 
+    def write_cosim_model(self, sim_name: str, sim_number: int, output_path_COSIM_folder: str, verbose: bool = None):
+        '''
+        :param sim_name: Simulation name that will be used to write the output file
+        :param sim_number: Simulation number that will be used to write the output file
+        :param output_path_COSIM_folder: Output folder
+        :param verbose: If True, display logging information
+        :return:
+        '''
+        # Assign variable to self to guarantee consistency between the methods
+        self.local_COSIM_folder = output_path_COSIM_folder
+        self.cosim_name = sim_name
+        self.sim_number = sim_number
+        # self.sim_suffix = f'_{sim_number}' if isinstance(sim_number, int) else sim_number
+        make_folder_if_not_existing(output_path_COSIM_folder, verbose=verbose)
+
+        # Write COSIM configuration file
+        self.write_config_file(verbose=verbose)
+
+        # Write COSIM submodels
+        for model_name, model in self.cosim_data.Simulations.items():
+            if verbose: (f'{model_name}, {model}')
+            if model.type == 'FiQuS':
+                self.write_model_FiQuS()
+            elif model.type == 'LEDET':
+                self.write_model_LEDET(model=model, output_path=output_path_COSIM_folder, verbose=verbose)
+            elif model.type == 'PSPICE':
+                self.write_model_PSPICE(model=model, output_path=output_path_COSIM_folder, verbose=verbose)
+            elif model.type == 'XYCE':
+                self.write_model_XYCE()
+
+    def write_config_file(self, output_file_name: str = 'COSIMConfig.json', verbose: bool = False):
+        '''
+        ** Write COSIM configuration file **
+        '''
+        # Calculate variables
+        coSimulationDir = self.reformat_path(os.path.join(self.local_COSIM_folder, self.cosim_name, str(self.sim_number), 'Output')) + '\\'
+        t_0 = self.cosim_data.Settings.Time_Windows.t_0
+        t_end = self.cosim_data.Settings.Time_Windows.t_end
+        executionOrder = self.cosim_data.Settings.Options_run.executionOrder
+        executeCleanRun = self.cosim_data.Settings.Options_run.executeCleanRun
+        coSimulationModelSolvers, coSimulationModelDirs, coSimulationModelConfigs, coSimulationPortDefinitions = [], [], [], []
+        convergenceVariables, relTolerance, absTolerance, t_step_max = [], [], [], []
+        for model_name, model in self.cosim_data.Simulations.items():
+            coSimulationModelSolvers.append(model.type)
+            coSimulationModelDirs.append(self.reformat_path(os.path.join(self.local_COSIM_folder, self.cosim_name, str(self.sim_number), 'Input', model_name)) + '\\')
+            coSimulationModelConfigs.append(f'{model_name}_config.json')
+            coSimulationPortDefinitions.append(f'{model_name}_InputOutputPortDefinition.json')
+            convergenceVariables.append(self.cosim_data.Settings.Convergence.convergenceVariables[model_name])
+            relTolerance.append(self.cosim_data.Settings.Convergence.relTolerance[model_name])
+            absTolerance.append(self.cosim_data.Settings.Convergence.absTolerance[model_name])
+            t_step_max.append(self.cosim_data.Settings.Time_Windows.t_step_max[model_name])
+
+        # Dictionary to write
+        dict_cosim_config = {
+                "coSimulationDir": coSimulationDir,
+                "coSimulationModelSolvers": coSimulationModelSolvers,
+                "coSimulationModelDirs": coSimulationModelDirs,
+                "coSimulationModelConfigs": coSimulationModelConfigs,
+                "coSimulationPortDefinitions": coSimulationPortDefinitions,
+                "convergenceVariables": convergenceVariables,
+                "t_0": t_0,
+                "t_end": t_end,
+                "t_step_max": t_step_max,
+                "relTolerance": relTolerance,
+                "absTolerance": absTolerance,
+                "executionOrder": executionOrder,
+                "executeCleanRun": executeCleanRun
+        }
+
+        # Serializing json
+        json_cosim_config = json.dumps(dict_cosim_config, indent=4)
+
+        # Writing to .json file
+        path_output_file = os.path.join(self.local_COSIM_folder, self.cosim_name, str(self.sim_number), 'Input', output_file_name)
+        make_folder_if_not_existing(os.path.dirname(path_output_file), verbose=verbose)
+        with open(path_output_file, "w") as outfile:
+            outfile.write(json_cosim_config)
         if verbose:
-            print(f'PyCoSim initialized with input file {file_model_data}.')
-            print(f'Local PyCoSim folder is {self.local_PyCoSim_folder}')
+            print(f'File {path_output_file} written.')
 
-    def run(self):
-        """
-        This runs co-sim
-        """
-        # Read initial
-        # A1 Make the folder structure
-        # A2 Make the input files for the pre-run simulation
-        # A3 Run the pre-run input files
-        # B Start a while loop with some convergence criteria
-        #   B0 If present, check output to see if convergence is met
-        #   B1 Make new folders
-        #   B2 Make new input files using output of previous simulation
-        #   B3 Run the new input files
-        # C1 Make the folder structure for the final run
-        # C2 Make the input files for the final-run simulation
-        # C3 Run the final-run input files
-
-        if self.verbose: print(f'Co-simulation {self.cosim_data.GeneralParameters.cosim_name} {self.sim_number} started.')
-        self.nsti = NSTI(self.sim_number, 0, 0, 0)
-
-        # Pre-cosim
-        for model_set, model in enumerate(self.cosim_data.Simulations.values()):
-            self.nsti.update(self.sim_number, model_set, 0, 0)  # Initial time window and iteration  # cosim_nsti --> N=Simulation number. S=Simulation set. T=Time window. I=Iteration.
-            write_model_input_files(cosim_data=self.cosim_data, model_name=model.name, model=model,
-                                    cosim_software='PyCoSim', local_cosim_folder=self.local_PyCoSim_folder,
-                                    data_settings=self.data_settings,
-                                    nsti=self.nsti, verbose=self.verbose)
-            # TODO Pass input/output
-            # if flag_run_precosim...
-            if model.flag_run_pre_cosim:
-                if self.verbose: print(f'Model {model.name}. Simulation set {self.nsti.s}. Pre-cosim simulation.')
-
-                self._run_sim(model=model)
-                # TODO add some basic check that the simulation run wihout errors
-                self._copy_files(model=model)
-                # self._copy_variables(model_name=model_name, model=model, verbose=verbose) #TODO implentation needed
-
-        # Co-simulation
-        # Loop through time windows
-        for model_set, model in enumerate(self.cosim_data.Simulations.values()):
-            # Reset convergence variables
-            flag_converge, current_iteration = False, 0
-            # Loop until convergence is found
-            while flag_converge == False:
-                for tw, time_wind in enumerate(self.cosim_data.Settings.Time_Windows):
-                    self.nsti.update(self.sim_number, model_set, tw + 1, current_iteration)
-                    if self.verbose: print(f'Model {model.name}. Simulation set {self.nsti.s}. Time window {self.nsti.t}. Iteration {self.nsti.i}.')
-                    # TODO Get input/output
-                    # Make model
-
-                    # TODO Pass input/output
-                    if model.flag_run_cosim:
-                        write_model_input_files(cosim_data=self.cosim_data, model_name=model.name, model=model,
-                                                cosim_software='PyCoSim', data_settings=self.data_settings,
-                                                nsti=self.nsti, verbose=self.verbose)
-                        # TODO Run model
-                        # TODO add some basic check that the simulation run wihout errors
-                # TODO check convergence
-                if 2 == 2:
-                    flag_converge = True
-                    if self.verbose: print(f'Model {model.name}. Simulation set {self.nsti.s}. Time window {self.nsti.t}. Convergence reached at iteration {self.nsti.i}.')  # Add info about convergence crirteria
-                else:
-                    current_iteration = current_iteration + 1
-
-        # Post-cosim
-        for model_set, model in enumerate(self.cosim_data.Simulations.values()):
-            if self.cosim_data.Settings.Options_run.executeCleanRun[model_set]:
-                self.nsti.update(self.sim_number, model_set, len(self.cosim_data.Settings.Time_Windows.t_0) + 1, 0)
-                if self.verbose: print(f'Model {model.name}. Simulation set {self.nsti.s}. Post-cosim simulation.')
-                # TODO Get input/output
-                # Make model
-                write_model_input_files(cosim_data=self.cosim_data, model_name=model.name, model=model,
-                                        cosim_software='PyCoSim', data_settings=self.data_settings,
-                                        nsti=self.nsti, verbose=self.verbose)
-                if model.flag_run_post_cosim:
-
-                    pass
-                    # TODO Run model
-                    # TODO add some basic check that the simulation run wihout errors
-
-        if self.verbose: print(f'Co-simulation {self.cosim_data.GeneralParameters.cosim_name} {self.sim_number} finished.')
-
-
-    def _run_sim(self, model: Union[sim_FiQuS, sim_LEDET, sim_PSPICE, sim_XYCE]):
-        """
-        Run selected simulation.
-        The function applies a different logic for each simulation software.
-        """
-
-        # Define local folder
-        local_folder = self.__find_local_target_folder(model=model)
-
-        # run simulation
-        if model.type == 'FiQuS':
-            dFiQuS = DriverFiQuS(path_folder_FiQuS_input=local_folder, path_folder_FiQuS_output=local_folder,
-                                 FiQuS_path=self.data_settings.FiQuS_path, GetDP_path=self.data_settings.GetDP_path, verbose=self.verbose)
-            self.summary[model.name] = dFiQuS.run_FiQuS(sim_file_name=f'{model.modelName}_{self.nsti.n_s_t_i}_FiQuS')
-        elif model.type == 'LEDET':
-            dLEDET = DriverLEDET(path_exe=self.data_settings.LEDET_path, path_folder_LEDET=local_folder, verbose=self.verbose)
-            dLEDET.run_LEDET(nameMagnet=model.modelName, simsToRun=str(model.simulationNumber), simFileType='.xlsx')  # simFileType is hard-coded
-        elif model.type == 'PSPICE':
-            dPSPICE = DriverPSPICE(path_exe=self.data_settings.PSPICE_path, path_folder_PSPICE=local_folder, verbose=self.verbose)
-            dPSPICE.run_PSPICE(nameCircuit=model.modelName, suffix='')
-        elif model.type == 'XYCE':
-            dXYCE = DriverXYCE(path_exe=self.data_settings.XYCE_path, path_folder_XYCE=local_folder, verbose=self.verbose)
-            dXYCE.run_XYCE(nameCircuit=model.modelName, suffix='')
-        else:
-            raise Exception(f'Software {model.type} not supported for automated running.')
-
-
-    def _copy_files(self, model: Union[sim_Generic, sim_FiQuS, sim_LEDET, sim_PSPICE, sim_XYCE]):
-        '''
-        This function copies files across from the output of one model to another.
-        :param model_name:
-        :param model:
-        :param verbose:
-        :return:
+    def write_model_FiQuS(self):
         '''
+        ** COSIM does not support FiQuS at the moment **
+        '''
+        raise Exception('ParserCOSIM does not support FiQuS model generation.')
+
+    def write_model_LEDET(self, model, output_path: str, verbose: bool = False):
+        '''
+        ** Write selected LEDET model **
+        :param output_path: Output folder
+        '''
+        # Unpack input
+        magnet_name = model.modelName
+
+        # Make subfolders
+        path_submodel_folder = os.path.join(self.local_COSIM_folder, self.cosim_name, str(self.sim_number), 'Input', model.name)
+        make_folder_if_not_existing(path_submodel_folder, verbose=verbose)
+        make_folder_if_not_existing(os.path.join(path_submodel_folder, 'LEDET', magnet_name, 'Input'), verbose=verbose)
+        make_folder_if_not_existing(os.path.join(path_submodel_folder, 'LEDET', magnet_name, 'Input', 'Control current input'), verbose=verbose)
+        make_folder_if_not_existing(os.path.join(path_submodel_folder, 'LEDET', magnet_name, 'Input', 'Initialize variables'), verbose=verbose)
+        make_folder_if_not_existing(os.path.join(path_submodel_folder, 'LEDET', magnet_name, 'Input', 'InitializationFiles'), verbose=verbose)
+        make_folder_if_not_existing(os.path.join(path_submodel_folder, 'Field maps', magnet_name), verbose=verbose)
+        # Make configuration file
+        path_config_file = os.path.join(path_submodel_folder, f'{model.name}_config.json')
+        self.write_config_file_ledet(output_file=path_config_file,
+                                     LEDET_path=self.reformat_path(
+                                         self.cosim_data.Options_COSIM.solverPaths[model.name]),
+                                     magnet_name=magnet_name, sim_set_number=str(self.sim_number))
+        # Make input/output port definition file
+        path_ports_file = os.path.join(path_submodel_folder, f'{model.name}_InputOutputPortDefinition.json')
+        self.write_ports_file(output_file=path_ports_file, model_name=model.name)
+        # Make input files, self-mutual inductance files, magnetic field map files. Save them to the COSIM subfolder
+        write_model_input_files(cosim_data=self.cosim_data, model=model, cosim_software='COSIM',
+                                data_settings=self.data_settings, nsti=NSTI(self.sim_number, None, 0, None),
+                                verbose=verbose)
+
+    def write_model_PSPICE(self, model, output_path: str, verbose: bool = False):
+        '''
+        ** Write selected PSPICE model **
+        :param output_path: Output folder
+        '''
+        # Make subfolders
+        path_submodel_folder = os.path.join(self.local_COSIM_folder, self.cosim_name, str(self.sim_number), 'Input', model.name)
+        make_folder_if_not_existing(path_submodel_folder, verbose=verbose)
+        # Make configuration file
+        path_config_file = os.path.join(path_submodel_folder, f'{model.name}_config.json')
+        self.write_config_file_pspice(output_file=path_config_file, model=model, solver_path=
+        self.cosim_data.Options_COSIM.solverPaths[model.name])
+        # Make input/output port definition file
+        path_ports_file = os.path.join(path_submodel_folder, f'{model.name}_InputOutputPortDefinition.json')
+        self.write_ports_file(output_file=path_ports_file, model_name=model.name)
+        # Make input netlist files, auxiliary files. Save them to the COSIM subfolder. Delete temporary files.
+        write_model_input_files(cosim_data=self.cosim_data, model=model, cosim_software='COSIM',
+                                data_settings=self.data_settings, nsti=NSTI(self.sim_number, None, 0, None),
+                                verbose=verbose)
+
+    def write_model_XYCE(self):
+        '''
+        ** COSIM does not support XYCE at the moment **
+        '''
+        raise Exception('ParserCOSIM does not support XYCE model generation.')
+
+
+    @staticmethod
+    def reformat_path(path: str):
+        '''
+        Reformat a string defining a path so that all delimiters are double slashes
+        :param path: string defining the original path
+        :return: str
+        '''
+
+        return os.path.normpath(path).replace(os.sep, '\\')
+
+    @staticmethod
+    def write_config_file_ledet(output_file: str, LEDET_path: str, magnet_name: str, sim_set_number: int):
+        '''
+        Write the LEDET configuration .json file
+        :param output_file: Target file
+        :param LEDET_path: Path to PSPICE executable
+        :param sim_set_number: Number of the simulation set, i.e. number of the LEDET simulation used in the COSIM model
+        :return: None
+        '''
+
+        # Dictionary to write
+        dict_ledet_config = {
+            "solverPath": f"{LEDET_path}",
+            "modelFolder": "LEDET",
+            "modelName": f"{magnet_name}",
+            "simulationNumber": f"{sim_set_number}"
+        }
+
+        # Serializing json
+        json_ledet_config = json.dumps(dict_ledet_config, indent=4)
+
+        # Writing to .json file
+        with open(output_file, "w") as outfile:
+            outfile.write(json_ledet_config)
+
+    @staticmethod
+    def write_config_file_pspice(output_file: str, model: sim_PSPICE, solver_path: str):
+        '''
+        Write the PSPICE configuration .json file
+        :param output_file: Target file
+        :param model: sim_PSPICE object containing the information about this model
+        :param solver_path: path to the solver to be used in the simulation
+        :return: None
+        '''
+        # Unpack inputs
+        solver_path = ParserCOSIM.reformat_path(solver_path)
+        modelName = model.modelName
+        configurationFileName = model.configurationFileName
+        externalStimulusFileName = model.externalStimulusFileName
+        initial_conditions = model.initialConditions
+        skipBiasPointCalculation = model.skipBiasPointCalculation
+
+        # Write a list of initial conditions
+        string_initial_conditions = [f'{ic_name}={ic}' for ic_name, ic in initial_conditions.items()]
+
+        # Dictionary to write
+        dict_pspice_config = {
+            "solverPath": solver_path,
+            "modelName": f'{modelName}.cir',
+            "configurationFileName": configurationFileName,
+            "externalStimulusFileName": externalStimulusFileName,
+            "initialConditions": string_initial_conditions,
+            "skipBiasPointCalculation": skipBiasPointCalculation,
+        }
+
+        # Serializing json
+        json_pspice_config = json.dumps(dict_pspice_config, indent=4)
+
+        # Writing to .json file
+        with open(output_file, "w") as outfile:
+            outfile.write(json_pspice_config)
+
+    def write_ports_file(self, output_file: str, model_name: str):
+        '''
+            Write the input/output port configuration .json file
+            This method does not depend on the software tool
+            :param output_file: Target file
+            :return: None
+        '''
+
+        list_of_dict_ports = []
+        for port_name, port in self.cosim_data.PortDefinition.items():
+            if model_name in port.Models:
+                port_info = port.Models[model_name]
+
+                # Dictionary to write
+                dict_ports = {
+                    "name": port_name,
+                    "components": port_info.components,
+                    "inputs": [],
+                    "outputs": [],
+                }
+                for input_name, input in port_info.inputs.items():
+                    dict_ports["inputs"].append({
+                        "couplingParameter": input.variable_coupling_parameter,
+                        "labels": input.variable_names,
+                        "types": input.variable_types})
+                for output_name, output in port_info.outputs.items():
+                    dict_ports["outputs"].append({
+                        "couplingParameter": output.variable_coupling_parameter,
+                        "labels": output.variable_names,
+                        "types": output.variable_types})
+                list_of_dict_ports.append(dict_ports)
+
+        # Writing to .json file
+        with open(output_file, "w") as outfile:
+            # Serializing json
+            for dict_ports in list_of_dict_ports:
+                json_ports = json.dumps(dict_ports, indent=4)
+                outfile.write(json_ports)
+                outfile.write('\n')
 
-        # Get list of files to copy, which depends on the current co-simulation state
-        if self.nsti.t == 0:
-            files_to_copy: List[FileToCopy] = model.files_to_copy_after.pre_cosim
-        elif self.nsti.t > len(self.cosim_data.Settings.Time_Windows.t_0):
-            files_to_copy: List[FileToCopy] = model.files_to_copy_after.post_cosim
-        else:
-            files_to_copy: List[FileToCopy] = model.files_to_copy_after.cosim
-
-        if len(files_to_copy) > 0:
-            # Define local folder
-            local_folder = self.__find_local_source_folder(model=model)
-
-            # Copy files
-            for file_to_copy in files_to_copy:
-                if file_to_copy.old_file_name_relative_path:
-                    original_file = Path(Path(local_folder), file_to_copy.old_file_name_relative_path).resolve()
-                    target_local_folder = self.__find_local_target_folder(model=self.cosim_data.Simulations[
-                        file_to_copy.target_model])
-                    if not file_to_copy.new_file_name_relative_path:
-                        file_to_copy.new_file_name_relative_path = file_to_copy.old_file_name_relative_path
-                    target_file = Path(Path(target_local_folder), file_to_copy.new_file_name_relative_path).resolve()
-                    make_folder_if_not_existing(os.path.dirname(target_file), verbose=self.verbose)
-                    if self.verbose: print(f'Copy file {original_file} to file {target_file}.')
-                    shutil.copyfile(original_file, target_file)
-
-    def __find_local_source_folder(self, model: Union[sim_FiQuS, sim_LEDET, sim_PSPICE, sim_XYCE]):
-        '''
-        Function to find the path to the local folder, which has a different logic for each simulation tool
-        :param model: Current simulation model
-        :return: Path to the local folder of the current simulation model
-        '''
-        local_folder_prefix = os.path.join(self.local_PyCoSim_folder,
-                                           self.cosim_data.GeneralParameters.cosim_name,
-                                           model.type,
-                                           model.modelName)
-        if model.type == 'FiQuS':
-            fiqus_input_file_path = os.path.join(local_folder_prefix, f'{model.modelName}_{self.nsti.n_s_t_i}_FiQuS.yaml')
-            fiqus_data: DataFiQuS = yaml_to_data(fiqus_input_file_path, DataFiQuS)
-            if fiqus_data.run.type in ['geometry_only']:
-                return os.path.join(local_folder_prefix, f'Geometry_{fiqus_data.run.geometry}')
-            elif fiqus_data.run.type in ['start_from_yaml', 'solve_with_post_process_python']:
-                return os.path.join(local_folder_prefix, f'Geometry_{fiqus_data.run.geometry}', f'Mesh_{fiqus_data.run.mesh}', f'Solution_{fiqus_data.run.solution}')
-        elif model.type == 'LEDET':
-            pass
-        elif model.type == 'PSPICE':
-            pass
-        elif model.type == 'XYCE':
-            pass
-        else:
-            raise Exception(f'Software {model.type} not supported for automated running.')
-
-
-    def __find_local_target_folder(self, model: Union[sim_FiQuS, sim_LEDET, sim_PSPICE, sim_XYCE]):
-        '''
-        Function to find the path to the local folder, which has a different logic for each simulation tool
-        :param model: Current simulation model
-        :return: Path to the local folder of the current simulation model
-        '''
-
-        # Define local folder
-        local_folder_prefix = os.path.join(self.local_PyCoSim_folder,
-                                           self.cosim_data.GeneralParameters.cosim_name,
-                                           model.type)
-        if model.type == 'FiQuS':
-            local_folder = os.path.join(local_folder_prefix, f'{model.modelName}')
-        elif model.type == 'LEDET':
-            local_folder = os.path.join(local_folder_prefix, str(self.nsti.n), f'{model.modelName}')
-        elif model.type in ['PSPICE', 'XYCE']:
-            local_folder = os.path.join(local_folder_prefix, self.nsti.n_s_t_i, model.modelName, str(model.simulationNumber))
-        local_folder = str(Path.resolve(Path(local_folder)))
-        return local_folder
-
-
-    def _check_convergence(self):
-        """
-        This functionality is not coded yet
-        :return:
-        :rtype:
-        """
-        # check whether converge criteria are met
-        flag_converged = False
-        return flag_converged
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataAPDLCTOptions.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataAPDLCTOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataAnalysis.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataAnalysis.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-from dataclasses import Field
-from pathlib import Path
-from typing import List, Union, Literal, Dict, Optional
+from typing import List, Union, Literal, Dict, Tuple, Optional
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field, ConfigDict
 
 from steam_sdk.data.DataSettings import DataSettings
 
 
 ############################
 # General parameters
 class ModelClass(BaseModel):
@@ -21,15 +19,18 @@
 
 class General(BaseModel):
     """
         Level 1: Class for general information on the case study
     """
     analysis_name: Optional[str] = None
     flag_permanent_settings: Optional[bool] = None
-    relative_path_settings: Optional[str] = None
+    relative_path_settings: Optional[str] = Field(default=None,
+                                              title="Relative path to settings file",
+                                              description="Relative path to settings.user.yaml file. It is relative to folder with analysis.yaml file",
+                                              examples=[r"../builders/model_library", r"C:\STEAM\model_library"])
     # relative_path_settings: Optional[str] = Field(default=None, description="This key is only used if flag_permanent_settings=False. It defines the relative path to the folder where the settings file is contained. This file is named settings.{user}.yaml, where {user} is the current user name.")
     model: ModelClass = ModelClass()
 
 class StrandCriticalCurrentMeasurement(BaseModel):
     """
         Level 1: Class for essential parameters for a critical current measurement to adjust Jc fit parameters
     """
@@ -52,14 +53,15 @@
     case_model: Optional[str] = None
     software: Optional[str] = None
     simulation_name: Optional[str] = None
     simulation_number: Optional[int] = None
     flag_json: Optional[bool] = None
     flag_plot_all: Optional[bool] = None
     verbose: Optional[bool] = None
+    model_config = ConfigDict(protected_namespaces=())
 
 
 class ModifyModel(BaseModel):
     """
         Level 2: Analysis step to modify an existing BuilderModel object by changing one variable
     """
     type: Literal['ModifyModel']
@@ -69,14 +71,16 @@
     new_model_name: List[str] = []  # if not empty, new copies of the model object will be built
     simulation_numbers: List[int] = []  # if not empty, simulation files will be built
     simulation_name: Optional[str] = None
     software: Optional[str] = None
     flag_json: Optional[bool] = None
     flag_plot_all: Optional[bool] = None
     verbose: Optional[bool] = None
+    model_config = ConfigDict(protected_namespaces=())
+
 
 
 class ModifyModelMultipleVariables(BaseModel):
     """
         Level 2: Analysis step to modify an existing BuilderModel object by changing a list of variables
     """
     type: Literal['ModifyModelMultipleVariables']
@@ -86,14 +90,15 @@
     new_model_name: List[str] = []  # if not empty, new copies of the model object will be built
     simulation_numbers: List[int] = []  # if not empty, simulation files will be built
     simulation_name: Optional[str] = None
     software: Optional[str] = None
     flag_json: Optional[bool] = None
     flag_plot_all: Optional[bool] = None
     verbose: Optional[bool] = None
+    model_config = ConfigDict(protected_namespaces=())
 
 
 class SetUpFolder(BaseModel):
     """
         Level 2: Analysis step to set up the folder structure for the required simulation software
     """
     type: Literal['SetUpFolder']
@@ -121,15 +126,15 @@
     full_path_file_to_copy: Optional[str] = None
     full_path_file_target: Optional[str] = None
 
 
 class CopyFileRelativeEntries(BaseModel):
     local_tool_folders: List[str] = []
     simulation_names: List[str] = []
-    reminder_paths:  List[str] = []
+    remainder_paths:  List[str] = []
 
 
 class CopyFileRelative(BaseModel):
     """
         Level 2: Analysis step to copy one file from a location to another
     """
     type: Literal['CopyFileRelative']
@@ -144,28 +149,25 @@
     type: Literal['RunSimulation']
     software: Optional[str] = None
     simulation_name: Optional[str] = None
     simulation_numbers: List[int] = []
     simFileType: Optional[str] = None
 
 
-class PostProcess(BaseModel):
+class PostProcessCompare(BaseModel):
     """
         Level 2: Analysis step to run a simulation file
     """
-    type: Literal['PostProcess']
-    sources: List[str] = []
-    sources_FiQuS_csv_idx: List[List[int]] = [[]]
-    sources_sim_nrs: List[List[int]] = [[]]
+    type: Literal['PostProcessCompare']
+    physical_quantity: Optional[str] = None
+    simulation_numbers: Optional[
+        Union[Tuple[int, int], int]] = None  # if only an int is provided, the other results are taken from ROXIE
     simulation_name: Optional[str] = None
     path_to_saved_files: Optional[str] = None
 
-    # software: Optional[str] = None
-    # simulation_name: Optional[str] = None
-    # simulation_numbers: List[int] = []
 
 class RunCustomPyFunction(BaseModel):
     """
         Level 2: Analysis step to run a custom Python function
     """
     type: Literal['RunCustomPyFunction']
     flag_enable: Optional[bool] = None
@@ -196,24 +198,26 @@
         Level 2: Analysis step to calculate metrics (usually to compare two or more measured and/or simulated signals)
     """
     type: Literal['CalculateMetrics']
     viewer_name: Optional[str] = None
     metrics_name: Optional[str] = None
     metrics_to_calculate: List[str] = []
     variables_to_analyze: List[List[str]] = [[]]
+    metrics_output_filepath: Optional[str] = None
 
 
 class LoadCircuitParameters(BaseModel):
     """
         Level 2: Analysis step to load global circuit parameters from a .csv file
     """
     type: Literal['LoadCircuitParameters']
     model_name: Optional[str] = None
     path_file_circuit_parameters: Optional[str] = None
     selected_circuit_name: Optional[str] = None
+    model_config = ConfigDict(protected_namespaces=())
 
 
 class WriteStimulusFile(BaseModel):
     """
         Level 2: Analysis step to write stimulus file from coil resistance csv file
     """
     type: Literal['WriteStimulusFile']
@@ -224,14 +228,15 @@
     current_level: List[float] = []
     magnets: List[int] = []
     t_offset: List[float] = []
     interpolation_type: Optional[str] = None  # 'Linear' or 'Spline'
     type_file_writing: Optional[str] = None  # 'w' or 'a'
     n_sampling: Optional[int] = None
     magnet_types: List[int] = []
+    software: Optional[str] = None
 
 
 class DefaultParsimEventKeys(BaseModel):
     """
         Level 3: Class for default keys of ParsimEventMagnet
     """
     local_LEDET_folder: Optional[str] = None
@@ -259,27 +264,28 @@
     rel_quench_heater_trip_threshold: Optional[float] = None
     current_polarities_CLIQ: List[int] = []  # TODO: consider making list of lists
     dict_QH_circuits_to_QH_strips: Dict[str, List[int]] = {}
     default_keys: DefaultParsimEventKeys = DefaultParsimEventKeys()
     path_postmortem_offline_data_folder: Optional[str] = None
     path_to_configurations_folder: Optional[str] = None
     filepath_to_temp_viewer_csv: Optional[str] = None
+    model_config = ConfigDict(protected_namespaces=())
 
 
 class ParametricSweep(BaseModel):
     """
         Level 2: Analysis step to write stimulus file from sweep input csv file
     """
     type: Literal['ParametricSweep']
     input_sweep_file: Optional[str] = None
     model_name: Optional[str] = None
     case_model: Optional[str] = None
     software: Optional[str] = None
     verbose: Optional[bool] = None
-
+    model_config = ConfigDict(protected_namespaces=())
 
 class ParsimConductor(BaseModel):
     """
         Level 2: Analysis step to write stimulus file from coil csv file
     """
     type: Literal['ParsimConductor']
     model_name: Optional[str] = None
@@ -288,14 +294,15 @@
     magnet_name: Optional[str] = None
     software: Optional[str] = None
     simulation_number: Optional[int] = None
     strand_critical_current_measurements: List[StrandCriticalCurrentMeasurement] = []
     groups_to_coils: Dict[str, List[int]] = {}
     length_to_coil: Dict[str, float] = {}
     path_output_sweeper_csv: Optional[str] = None
+    model_config = ConfigDict(protected_namespaces=())
 
 # class AnalysisStep(BaseModel):
 #     """
 #         Level 1: Class for information on the analysis step
 #         Objects of this class will be defined in AnalysisStepDefinition
 #     """
 #     step: Union[MakeModel, ModifyModel, ModifyModelMultipleVariables, SetUpFolder, ChangeAuxiliaryFile, RunSimulation, PostProcess] = {}
@@ -315,11 +322,11 @@
 
         :return: DataModelCircuit object
     '''
 
     GeneralParameters: General = General()
     PermanentSettings: DataSettings = DataSettings()
     AnalysisStepDefinition: Dict[str, Union[MakeModel, ModifyModel, ModifyModelMultipleVariables, SetUpFolder,
-                                            AddAuxiliaryFile, CopyFile, CopyFileRelative, RunSimulation, PostProcess, RunCustomPyFunction,
+                                            AddAuxiliaryFile, CopyFile, CopyFileRelative, RunSimulation, PostProcessCompare, RunCustomPyFunction,
                                             RunViewer, CalculateMetrics, LoadCircuitParameters, WriteStimulusFile,
                                             ParsimEvent, ParametricSweep, ParsimConductor]] = {}
     AnalysisStepSequence: List[str] = []  # Here the analysis steps are defined, in execution order. Names must be defined in AnalysisStepDefinition. Repetitions ARE allowed.
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataConductor.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataConductor.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,16 @@
 
 class Round(BaseModel):
     """
         Level 2: Class for strand parameters
     """
     type: Literal['Round']
     diameter: Optional[float] = None  # ds_inGroup (LEDET), DConductor (BBQ), DStrand (ProteCCT)
+    diameter_core:  Optional[float] = None  # dcore_inGroup (LEDET)
+    diameter_filamentary:  Optional[float] = None  # dfilamentary_inGroup (LEDET)
     Cu_noCu_in_strand: Optional[float] = None
     RRR: Optional[float] = None  # RRR_Cu_inGroup (LEDET), RRRStrand (ProteCCT)
     T_ref_RRR_high: Optional[float] = None  # TupRRR (SIGMA), Reference temperature for RRR measurements
     T_ref_RRR_low: Optional[float] = None  # CURRENTLY NOT USED
     fil_twist_pitch: Optional[float] = None
     f_Rho_effective: Optional[float] = None
     material_superconductor: Optional[str] = None
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataEventCircuit.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataEventMagnet.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataFiQuSOptions.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataFiQuSOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataLEDET.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataLEDET.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,18 @@
     I00: Optional[float] = None
     GroupToCoilSection: np.ndarray = field(default_factory=lambda: np.array([]))
     polarities_inGroup: np.ndarray = field(default_factory=lambda: np.array([]))
     nT: np.ndarray = field(default_factory=lambda: np.array([]))
     nStrands_inGroup: np.ndarray = field(default_factory=lambda: np.array([]))
     l_mag_inGroup: np.ndarray = field(default_factory=lambda: np.array([]))
     ds_inGroup: np.ndarray = field(default_factory=lambda: np.array([]))
+     # Start new keys for TFMData
+    dfilamentary_inGroup: np.ndarray = field(default_factory=lambda: np.array([]))
+    dcore_inGroup: np.ndarray = field(default_factory=lambda: np.array([]))
+    # End new keys for TFMData
     f_SC_strand_inGroup: np.ndarray = field(default_factory=lambda: np.array([]))
     f_ro_eff_inGroup: np.ndarray = field(default_factory=lambda: np.array([]))
     Lp_f_inGroup: np.ndarray = field(default_factory=lambda: np.array([]))
     RRR_Cu_inGroup: np.ndarray = field(default_factory=lambda: np.array([]))
     SCtype_inGroup: np.ndarray = field(default_factory=lambda: np.array([]))
     STtype_inGroup: np.ndarray = field(default_factory=lambda: np.array([]))
     insulationType_inGroup: np.ndarray = field(default_factory=lambda: np.array([]))
@@ -251,7 +255,9 @@
     overwrite_inductance_coil_sections: np.ndarray = field(default_factory=lambda: np.array([[]]))
     overwrite_HalfTurnToInductanceBlock: np.ndarray = field(default_factory=lambda: np.array([[]]))
     # The following parameters are needed for self-mutual inductance calculation
     nStrands_inGroup_ROXIE: np.ndarray = field(default_factory=lambda: np.array([]))
     x_strands: np.ndarray = field(default_factory=lambda: np.array([]))  # TODO: add correct keys based on the ParserROXIE() parameters
     y_strands: np.ndarray = field(default_factory=lambda: np.array([]))  # TODO: add correct keys based on the ParserROXIE() parameters
     I_strands: np.ndarray = field(default_factory=lambda: np.array([]))  # TODO: add correct keys based on the ParserROXIE() parameters
+    Bx: np.ndarray = field(default_factory=lambda: np.array([])) 
+    By: np.ndarray = field(default_factory=lambda: np.array([]))
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataLEDETOptions.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataLEDETOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataModelCircuit.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataModelCircuit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from pydantic import BaseModel, create_model
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 
 ############################
 # General parameters
 class Model(BaseModel):
     """
         Level 2: Class for information on the model
     """
     name: Optional[str] = None
     version: Optional[str] = None
     case: Optional[str] = None
     state: Optional[str] = None
 
+
 class General(BaseModel):
     """
         Level 1: Class for general information on the case study
     """
     circuit_name: Optional[str] = None
     model: Model = Model()
     additional_files: List[str] = []  # These files will be physically copied to the output folder
@@ -27,14 +28,15 @@
 class Auxiliary_Files(BaseModel):
     """
         Level 1: Class for general information on the case study
         Note: These entries will be written in the netlist, but no further action will be taken (see General.additional_files)
     """
     files_to_include: List[str] = []
 
+
 ############################
 # Stimuli
 class StimuliClass(BaseModel):
     """
         Level 1: Stimulus files
     """
     stimulus_files: List[str] = []
@@ -45,22 +47,44 @@
 class LibrariesClass(BaseModel):
     """
         Level 1: Component libraries
     """
     component_libraries: List[str] = []
 
 
+class Magnet(BaseModel):
+    name: Optional[str] = None
+    L_mag: Optional[float] = None
+    C_ground: Optional[float] =None
+    Field_interp_value: Optional[float] = None
+
+class TFMClass(BaseModel):
+    flag_PC: Optional[bool] = False
+    flag_IFCC: Optional[bool] = False
+    flag_ISCC: Optional[bool] = False
+    flag_Wedges: Optional[bool] = False
+    flag_ColdBore: Optional[bool] = False
+    flag_EC: Optional[bool] = False
+    flag_BS: Optional[bool] = False
+    flag_Roxie: Optional[bool] = False
+    flag_Mutual: Optional[bool] = False
+    M_IF_PC: Optional[float] = None
+    T: Optional[float] = None
+    Magnets: Dict[str, Magnet] = {}
+
+
 ############################
 # Global parameters
 class Global_Parameters(BaseModel):
     """
         Level 1: Global circuit parameters
     """
     global_parameters: Optional[dict] = None
 
+
 ############################
 # Initial conditions
 class InitialConditionsClass(BaseModel):
     """
         Level 1: Initial conditions parameters
     """
     initial_conditions: Optional[dict] = None
@@ -76,18 +100,19 @@
 #         return object.__setattr__(self, key, value)
 
 class Component(BaseModel):
     """
         Level 2: Circuit component
     """
     type: Optional[str] = None
-    nodes: List[str] = []
+    nodes: List[Union[str, int]] = []
     value: Optional[str] = None
     parameters: Optional[dict] = dict()
 
+
 ############################
 # Simulation options
 class OptionsClass(BaseModel):
     """
         Level 1: Simulation options
     """
     options_simulation: Optional[dict] = None
@@ -98,50 +123,54 @@
 ############################
 # Analysis settings
 class SimulationTime(BaseModel):
     """
         Level 2: Simulation time settings
     """
     time_start: Optional[float] = None
-    time_end:   Optional[float] = None
+    time_end: Optional[float] = None
     min_time_step: Optional[float] = None
     time_schedule: Optional[dict] = None
 
+
 class SimulationFrequency(BaseModel):
     """
         Level 2: Simulation frequency settings
     """
     frequency_step: Optional[str] = None
-    frequency_points:   Optional[float] = None
+    frequency_points: Optional[float] = None
     frequency_start: Optional[str] = None
     frequency_end: Optional[str] = None
 
+
 class AnalysisClass(BaseModel):
     """
         Level 1: Analysis settings
     """
     analysis_type: Optional[str] = None
     simulation_time: Optional[SimulationTime] = SimulationTime()
     simulation_frequency: Optional[SimulationFrequency] = SimulationFrequency()
 
+
 ############################
 # Post-processing settings
 class Settings_Probe(BaseModel):
     """
         Level 2: Probe settings
     """
     probe_type: Optional[str] = None
     variables: List[str] = []
 
+
 class PostProcessClass(BaseModel):
     """
         Level 1: Post-processing settings
     """
     probe: Settings_Probe = Settings_Probe()
- 
+
 
 ############################
 # Highest level
 class DataModelCircuit(BaseModel):
     '''
         **Class for the circuit netlist inputs**
 
@@ -161,7 +190,8 @@
     Libraries: LibrariesClass = LibrariesClass()
     GlobalParameters: Global_Parameters = Global_Parameters()
     InitialConditions: InitialConditionsClass = InitialConditionsClass()
     Netlist: Dict[str, Component] = {}
     Options: OptionsClass = OptionsClass()
     Analysis: AnalysisClass = AnalysisClass()
     PostProcess: PostProcessClass = PostProcessClass()
+    TFM: Optional[TFMClass] = None
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataModelCommon.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataModelCommon.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataModelConductor.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataModelConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataModelCosim.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataModelCosim.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import (List, Union, Dict, Literal, Optional)
 
-from pydantic import BaseModel, Field, validator
+from pydantic import BaseModel, Field, validator, ConfigDict
 
 
 ############################
 # General parameters
 class Model(BaseModel):
     """
         Level 2: Class for information on the model
@@ -31,38 +31,51 @@
 #     local_PyCoSim_folder: str = None
 #     path_model_folder: str = None  # TODO: maybe this key should be deleted, since each model could be read from different libraries for different models, see key "modelFolder"
 #     settings_file_path: str = Field(default=None, description="relative path to settings file with file name of settings.user.yaml. This relative path is folder path")
 
 ############################
 # Simulation configurations - one for simulation tool
 
+class ConvergenceChecks(BaseModel):
+    """
+        Level 2: Class to define convergence checks to perform
+    """
+    file_name_relative_path: Optional[str] = Field(default=None, description="Name of the file with variable from which the convergence should be read")
+    flag_add_nsti_to_file_name: Optional[bool] = Field(default=None, description="If True, add an NSTI suffix between the base name and the extension of the file name. The NSTI refers to the source model. NSTI: N=simulation number. S=simulation set. T=time window. I=Iteration number")
+    var_name: Optional[str] = Field(default=None, description="Name of the convergence variable")
+    time_var_name: Optional[str] = Field(default=None, description="Name of the variable defining the time verctor. If defined, the variable values will be interpolated over the time vector before being compared.")
+    relative_tolerance: Optional[float] = Field(default=None, description="Relative tolerance applied to the convergence check (either relative_tolerance or absolute_tolerance must be fulfilled to pass the convergence check)")
+    absolute_tolerance: Optional[float] = Field(default=None, description="Absolute tolerance applied to the convergence check (either relative_tolerance or absolute_tolerance must be fulfilled to pass the convergence check)")
+
 class ParametersToModify(BaseModel):
     """
         Level 2: Class to define parameters to modify
     """
     variables_to_change: List[str] = []
     variables_values: List = []
 
 class FileToCopy(BaseModel):
     old_file_name_relative_path: Optional[str] = Field(default=None, description="Name of the file to copy")
+    flag_add_nsti_to_old_file_name: Optional[bool] = Field(default=None, description="If True, add an NSTI suffix between the base name and the extension of the old file name. The NSTI refers to the source model. NSTI: N=simulation number. S=simulation set. T=time window. I=Iteration number")
     target_model: Optional[str] = Field(default=None, description="Name of the simulation model")
-    new_file_name_relative_path: Optional[
-        str] = Field(default=None, description="New name of the file to copy. If null, don't change the name")
+    new_file_name_relative_path: Optional[str] = Field(default=None, description="New name of the file to copy. If null, don't change the name")
+    flag_add_nsti_to_new_file_name: Optional[bool] = Field(default=None, description="If True, add an NSTI suffix between the base name and the extension of the new file name. The NSTI refers to the target model, not the source model. NSTI: N=simulation number. S=simulation set. T=time window. I=Iteration number")
 
 class FilesToCopy(BaseModel):
     pre_cosim: List[FileToCopy] = Field(default=[FileToCopy()], description="Files to copy after the pre-cosimulation")
     cosim: List[FileToCopy] = Field(default=[FileToCopy()], description="Files to copy after the cosimulation")
     post_cosim: List[FileToCopy] = Field(default=[FileToCopy()], description="Files to copy after the post-cosimulation")
 
 class VariableToCopy(BaseModel):
-    file_name_relative_path: Optional[
-        str] = Field(default=None, description="Path of the file that contains the variable to copy (supported formats: .csd, .csv, .mat)")
+    file_name_relative_path: Optional[str] = Field(default=None, description="Path of the file that contains the variable to copy (supported formats: .csd, .csv, .mat)")
+    flag_add_nsti_to_file_name: Optional[bool] = Field(default=None, description="If True, add an NSTI suffix between the base name and the extension of the file name. The NSTI refers to the source model. NSTI: N=simulation number. S=simulation set. T=time window. I=Iteration number")
     var_name: Optional[str] = Field(default=None, description="Name of the variable to copy (header name is a .csv or .csd file, or variable name in a .mat file")
     target_model: Optional[str] = Field(default=None, description="Name of the simulation model")
     model_var_name: Optional[str] = Field(default=None, description="Name of the BuilderModel key to which the variable value will be assigned")
+    model_config = ConfigDict(protected_namespaces=())
 
 class VariablesToCopy(BaseModel):
     pre_cosim: List[VariableToCopy] = Field(default=[VariableToCopy()], description="Variables to copy after the pre-cosimulation")
     cosim: List[VariableToCopy] = Field(default=[VariableToCopy()], description="Variables to copy after the cosimulation")
     post_cosim: List[VariableToCopy] = Field(default=[VariableToCopy()], description="Variables to copy after the post-cosimulation")
 
 
@@ -73,14 +86,15 @@
     name: Optional[str] = None
     modelFolder: Optional[str] = None  # TODO: is this needed?
     modelName: Optional[str] = None
     modelCase: Optional[str] = None
     flag_run_pre_cosim: Optional[bool] = Field(default=None, description="Flag to enable (True) or disable (false) pre-cosim solution")
     flag_run_cosim: Optional[bool] = Field(default=None, description="Flag to enable (True) or disable (false) cosim solution")
     flag_run_post_cosim: Optional[bool] = Field(default=None, description="Flag to enable (True) or disable (False) post-cosim solution")
+    convergence_checks_cosim: List[ConvergenceChecks] = Field(default=[], description="List of convergence checks to perform during each time window (all variable checks must be fulfilled to pass the convergence check)")
     variables_to_modify_pre_cosim: ParametersToModify = ParametersToModify()
     variables_to_modify_cosim: ParametersToModify = ParametersToModify()
     variables_to_modify_post_cosim: ParametersToModify = ParametersToModify()
     files_to_copy_after: FilesToCopy = FilesToCopy()
     variables_to_copy_after: VariablesToCopy = VariablesToCopy()
 
 class sim_FiQuS(sim_Generic): # TODO add/edit keys
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataModelMagnet.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataModelMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataModelParsimDakota.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataModelParsimDakota.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,20 +20,21 @@
 class MultiDimParStudyVar(BaseModel):
     """
         Class for FiQuS multipole
     """
     data_points: Optional[int] = None
     bounds: Bound = Bound()
 
-class OptppQNewtonParStudyVar(BaseModel):
+class VariablesWithInitialBounds(BaseModel):
     """
-        Class for FiQuS multipole
+        Dataclass for variables that need initial bounds, e.g. for local optimization
     """
-    initial_point: float = Field(default=None, description="Smart sentence from dakota manual")
+    initial_point: float = Field(default=None, description="First design point the algorithm chooses for a variable")
     bounds: Bound = Bound()
+    scale_type: Optional[str] = None
     #descriptors: str = Field(default=None, description="Smart sentence from dakota manual")
 
 class Sampling(BaseModel):
     """
         Class for FiQuS multipole
     """
     type: Literal['sampling']
@@ -48,41 +49,62 @@
         Class for FiQuS multipole
     """
     type: Literal['multidim_parameter_study']
     variables: Dict[str, MultiDimParStudyVar] = {}
 
 class OptppQNewton(BaseModel):
     """
-        Class for FiQuS multipole
+        Data class of the coliny_pattern_search algorithm OptppQNewton
     """
     type: Literal['optpp_q_newton']
     convergence_tolerance: float = Field(default=None, description="Smart sentence from dakota manual")
-    variables: Dict[str, OptppQNewtonParStudyVar] = {}
+    gradient_tolerance: float = Field(default=None, description="Threshold value on the L2 norm of the objective function"
+                                                                "gradient that indicates convergence to a stationary point.")
+    variables: Dict[str, VariablesWithInitialBounds] = {}
     #samples: Optional[int] = None
     #seed: Optional[int] = None
 
     #response_levels: Optional[float] = None
 
+class coliny_pattern_search(BaseModel):
+    """
+        Data class of the coliny_pattern_search algorithm
+    """
+    type: Literal['coliny_pattern_search']
+    initial_delta: float = Field(default=None, description="Difference between two initial steps")
+    solution_target: float = Field(default=None, description="Stopping criteria based on objective function value ")
+    contraction_factor: float = Field(default=None, description="Amount by which step length is rescaled ")
+    max_iterations: int = Field(default=None, description="Number of iterations allowed for optimizers and adaptive UQ methods")
+    max_function_evaluations: int = Field(default=None, description="Number of function evaluations allowed for optimizers")
+    variable_tolerance: float = Field(default=None, description="Step length-based stopping criteria for derivative-free optimizers")
+    variables: Dict[str, VariablesWithInitialBounds] = {}
+    #samples: Optional[int] = None
+    #seed: Optional[int] = None
+
+    #response_levels: Optional[float] = None
+
+
+
 
 class Response(BaseModel):
     """
         Class for FiQuS multipole
     """
     response: Optional[str] = None  # Union[ResponseFunction, ObjectiveFunction] = {'type': 'response_functions'}
     descriptors: Optional[List[str]] = None
 
 
 # First Level
 class DataModelParsimDakota(BaseModel):
     parsim_name: str = Field(default=None, description="Name of the study. This is folder name in which the files will be saved in the local_Dakota_folder")
     sim_number_offset: int = Field(default=None, description="This number is added to the simulation numbers used by the tool and Dakota. THis is to enable not overwriting simulations in the tool folder")
     evaluation_concurrency: int = Field(default=None, description="Number of concurrent executions. ")
-    study: Union[MultiDimParStudy, Sampling, OptppQNewton] = {'type': 'multidim_parameter_study'}
+    study: Union[MultiDimParStudy, Sampling, OptppQNewton,coliny_pattern_search] = {'Type of study (algorithm) selected for the optimization/parameter study.'}
     responses: Response = Response()
-    analysis_yaml_file_name: str = Field(default=None, description="name of analysis file to use in Dakota simulation, for the moment, the file needs to be in the same folder as Dakota input yaml")
+    relative_path_analysis_file: str = Field(default=None, description="Relative path (in relation to dakota input yaml) to analysis file, including the file name and extension")
     initial_steps_list: List[str] = Field(default=None, description="List of initial steps to be performed before Dakota is running (looping)")
     iterable_steps_list: List[str] = Field(default=None, description="List of steps to repeat in the analysis when Dakota is running (looping)")
     python_path_dakota: str = Field(default="python.exe", description="Path to the python.exe, that Dakota should use for running driver_link.py")
 
 # from steam_sdk.data.DataAnalysis import WorkingFolders
 # from steam_sdk.data.DataSettings import DataSettings
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataParsimConductor.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataParsimConductor.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 
 
 class ConductorSample(BaseModel):
     ID: Optional[str] = None  # TODO currenty unused
     Ra: Optional[float] = None
     Rc: Optional[float] = None
     number_of_strands: Optional[int] = None
-    width: Optional[float] = None
-    height: Optional[float] = None
+    bare_cable_width: Optional[float] = None
+    bare_cable_height: Optional[float] = None
     strand_twist_pitch: Optional[float] = None
     filament_twist_pitch: Optional[float] = None
     RRR: Optional[float] = None
     Cu_noCu: Optional[float] = None
     # critical current measurement attributes
     Tc0: Optional[float] = None
     Bc20: Optional[float] = None
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataProteCCT.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataProteCCTOptions.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataProteCCTOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataPyBBQ.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataPyBBQOptions.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataPyBBQOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataPySIGMA.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataPySIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataPySIGMAOptions.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataPySIGMAOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataRoxieParser.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DataSignal.py` & `steam-sdk-2024.4.0/steam_sdk/data/DataSignal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DictionaryLEDET.py` & `steam-sdk-2024.4.0/steam_sdk/data/DictionaryLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DictionaryProteCCT.py` & `steam-sdk-2024.4.0/steam_sdk/data/DictionaryProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/DictionaryPyBBQ.py` & `steam-sdk-2024.4.0/steam_sdk/data/DictionaryPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/TemplateLEDET.py` & `steam-sdk-2024.4.0/steam_sdk/data/TemplateLEDET.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,16 @@
         [None, None, 'Conductor parameters'],
         ['GroupToCoilSection', None, 'Define the coil section where each group of cables is located'],
         ['polarities_inGroup', None, 'Polarity of the current in each group of strands'],
         ['nT', None, 'Number of half-turns in each group'],
         ['nStrands_inGroup', None, 'Number of strands in each cable belonging to a particular group'],
         ['l_mag_inGroup', None, 'length of each half turn [m] (default=l_magnet)'],
         ['ds_inGroup', None, 'strand diameter [m]'],
+        ['dfilamentary_inGroup', None, 'strand filamentary matrix diameter [m]'],
+        ['dcore_inGroup', None, 'strand core diameter [m]'],
         ['f_SC_strand_inGroup', None, 'fraction of superconductor in the strands [-]'],
         ['f_ro_eff_inGroup', None, 'Effective transverse resistivity parameter (default=1)'],
         ['Lp_f_inGroup', None, 'Filament twist-pitch [m]'],
         ['RRR_Cu_inGroup', None, 'RRR of the conductor in each group of cables [-]'],
         ['SCtype_inGroup', None, 'type of superconductor (1=Nb-Ti, 2=Nb3Sn with Summers\' fit, 3 = BSCCO2212, 4 = Nb3Sn with Bordini\' fit)'],
         ['STtype_inGroup', None, 'type of stabilizer (1=Cu, 2=Ag, 3=Stainless steel, 4=Iron, 5=BeCu)'],
         ['insulationType_inGroup', None, 'Type of cable insulation (1=G10, 2=kapton)'],
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/data/TemplateProteCCT.py` & `steam-sdk-2024.4.0/steam_sdk/data/TemplateProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/drivers/DriverANSYS.py` & `steam-sdk-2024.4.0/steam_sdk/drivers/DriverANSYS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/drivers/DriverAnalysis.py` & `steam-sdk-2024.4.0/steam_sdk/drivers/DriverAnalysis.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import multiprocessing
 import os
 import sys
+import traceback
 import warnings
+from multiprocessing import freeze_support
 from pathlib import Path
 import numpy as np
 import re
 
 from steam_sdk.data.DataAnalysis import DataAnalysis
 from steam_sdk.data.DataSettings import DataSettings
 from steam_sdk.parsers.ParserYAML import yaml_to_data
@@ -47,18 +50,18 @@
                     step.variables_value[index] = [str(Path(step.variables_value[index][0]).resolve())]
             elif step.type in ['ModifyModel']:
                 if 'Options_FiQuS.multipole.postproc.compare_to_ROXIE' in step.variable_to_change:
                     index = step.variable_to_change.index('Options_FiQuS.multipole.postproc.compare_to_ROXIE')
                     step.variable_value[index] = str(Path(step.variable_value[index][0]).resolve())
 
         if data_analysis.GeneralParameters.flag_permanent_settings:  # use settings from analysis file
-            data_settings: DataSettings = DataSettings(**data_analysis.PermanentSettings.__dict__)
+            data_settings: DataSettings = DataSettings(**data_analysis.PermanentSettings.dict())
         else:
-            _, data_settings = read_settings_file(
-                relative_path_settings=data_analysis.GeneralParameters.relative_path_settings,
+            data_settings = read_settings_file(
+                absolute_path_settings_folder=data_analysis.GeneralParameters.relative_path_settings,
                 verbose=False)  # Information will be displayed later, to verbose=False here
         path_dakota_python = os.path.join(Path(data_settings.Dakota_path).parent.parent, 'share\dakota\Python')
         print('path_dakota_python:        {}'.format(path_dakota_python))
         sys.path.insert(0, path_dakota_python)      # this is ugly, but dakota does not distribute proper python library to use and install via PyPi
         from dakota.interfacing import read_parameters_file
 
         params, result_for_dakota = read_parameters_file(parameters_file=parameters_file, results_file=results_file)  # inputs, outputs
@@ -138,18 +141,37 @@
 
                 if step.type == 'ParsimEvent':
                     # update the path to the temp viewer input file
                     pattern = r'\\(\d+)\\'
                     old_filepath_to_viewer_input = step.filepath_to_temp_viewer_csv
                     new_filepath_to_viewer_input = re.sub(pattern, fr'\\{iteration_number}\\', old_filepath_to_viewer_input)
                     if old_filepath_to_viewer_input == new_filepath_to_viewer_input:
-                        warnings.warn("Step ParsimEvent:Temporary viewer input file is not simulation number specific "
+                        warnings.warn("Step ParsimEvent: Temporary viewer input file is not simulation number specific "
                                       "--> add a simulation number to the filepath to make it iteratable")
                     step.filepath_to_temp_viewer_csv = new_filepath_to_viewer_input
 
+                    old_path_output_event_csv = step.path_output_event_csv
+                    new_path_output_event_csv = re.sub(pattern, fr'\\{iteration_number}\\',
+                                                          old_path_output_event_csv)
+                    if old_path_output_event_csv == new_path_output_event_csv:
+                        warnings.warn("Step ParsimEvent: The path to the parsim sweep file to be written is not simulation "
+                                      "number specific --> add a simulation number to the filepath to make it iteratable")
+                    step.path_output_event_csv = new_path_output_event_csv
+
+
+                    old_path_output_viewer_csv = step.path_output_viewer_csv
+                    new_path_output_viewer_csv = re.sub(pattern, fr'\\{iteration_number}\\',
+                                                       old_path_output_viewer_csv)
+                    if old_path_output_viewer_csv== new_path_output_viewer_csv:
+                        warnings.warn(
+                            "Step ParsimEvent: The path to the viewer csv to be written is not simulation "
+                            "number specific --> add a simulation number to the filepath to make it iteratable")
+                    step.path_output_viewer_csv = new_path_output_viewer_csv
+
+
             if step.type == 'RunViewer':
                 # update the path to the temp viewer input file
                 pattern = r'\\(\d+)\\'
                 old_file_name_transients = step.file_name_transients
                 new_file_name_transients = re.sub(pattern, fr'\\{iteration_number}\\', old_file_name_transients)
                 if old_file_name_transients == new_file_name_transients:
                     warnings.warn("Step RunViewer: Temporary viewer input file is not simulation number specific "
@@ -161,29 +183,43 @@
                 old_filepath_to_report = step.path_output_pdf_report
                 new_filepath_to_report = re.sub(pattern, fr'\\{iteration_number}\\', old_filepath_to_report)
                 if old_filepath_to_report == new_filepath_to_report:
                     warnings.warn("Step RunViewer: Path to report is not simulation number specific "
                                   "--> add a simulation number to the filepath to make it iteratable")
                 step.path_output_pdf_report = new_filepath_to_report
 
+            if step.type == 'CalculateMetrics':
+                # update the path to the temp viewer input file
+                if step.metrics_output_filepath:
+                    pattern = r'\\(\d+)\\'
+                    old_metrics_output_filepath = step.metrics_output_filepath
+                    new_metrics_output_filepath = re.sub(pattern, fr'\\{iteration_number}\\', old_metrics_output_filepath)
+                    if old_metrics_output_filepath == new_metrics_output_filepath:
+                        warnings.warn("Step CalculateMetrics: Metrics_output_filepath key is not simulation number specific "
+                                      "--> add a simulation number to the filepath to make it iteratable")
+                    step.metrics_output_filepath = new_metrics_output_filepath
+
         # file path for this analysis iteration
         analysis_yaml_path_this_iteration = f'{self.analysis_yaml_path[:-(4+len(str(self.sim_number_offset)))]}_{iteration_number}.yaml'
 
         # write analysis input
         model_data_to_yaml(data_analysis, analysis_yaml_path_this_iteration)
 
-        # Run analysis
-        a = AnalysisSTEAM(file_name_analysis=analysis_yaml_path_this_iteration, file_path_list_models=None,
-                          verbose=True)
-        a.run_analysis()
-
-        # Write back to DAKOTA
-        for i, label in enumerate(result_for_dakota):
-            if isinstance(a.summary, dict): # TODO: make sure this dict is existent also for XYCE and then remove this statement
-                if result_for_dakota[label].asv.function:
-                    result_for_dakota[label].function = np.format_float_positional(a.summary[label], precision=4)
-            else:
-                result_for_dakota[label].function = 0
-            result_for_dakota.write()
+        try:
+            # Run analysis
+            a = AnalysisSTEAM(file_name_analysis=analysis_yaml_path_this_iteration, file_path_list_models=None,
+                              verbose=True)
+            a.run_analysis()
+            for i, label in enumerate(result_for_dakota):
+                if isinstance(a.summary, dict):  # TODO: make sure this dict is existent also for XYCE and then remove this statement
+                    if result_for_dakota[label].asv.function:
+                        result_for_dakota[label].function = np.format_float_positional(a.summary[label], precision=9)
+                else:
+                    result_for_dakota[label].function = 0
+        except Exception as e:
+            print(f"The following Exception occured in iteration-number {iteration_number}: {e}")
+            traceback.print_exc()
+            result_for_dakota.fail()
+        result_for_dakota.write()
 
         # return 1 so Dakota knows that this driver analysis did not crash
         return 1
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/drivers/DriverDakota.py` & `steam-sdk-2024.4.0/steam_sdk/drivers/DriverDakota.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,16 +35,16 @@
         self.analysis_yaml_path = analysis_yaml_path
         self.data_model_dakota = data_model_dakota
         self.settings = settings
         self.verbose = verbose
 
         #self.builder_model_obj_path = os.path.join(self.settings.local_Dakota_folder, 'temp.pkl')
 
-        self.analysis_yaml_local_path = os.path.join(os.path.join(self.settings.local_Dakota_folder, self.data_model_dakota.parsim_name), os.path.basename(self.analysis_yaml_path))
-
+        self.output_path = os.path.dirname(self.analysis_yaml_path)
+        self.analysis_file_name = os.path.basename(self.analysis_yaml_path)
         # this is running by default these functions at the initialization of the class
         self._run_pre_dakota_non_iterable_steps()
         self._write_driver_link()
         self._run_dakota_iterable_steps()
 
     def _run_pre_dakota_non_iterable_steps(self):
         """
@@ -90,41 +90,41 @@
                 elif len(step.simulation_numbers) == 1:
                     step.simulation_numbers = [init_sim_num_w_offset]
                 else:
                     raise Exception(f'Analysis file with multiple simulation numbers can not be used in dakota. Change {step_name}.simulation_numbers={step.simulation_numbers} to a list with single entry')
 
         data_analysis.GeneralParameters.relative_path_settings = os.path.join(Path(os.path.dirname(self.analysis_yaml_path), Path(data_analysis.GeneralParameters.relative_path_settings)).resolve())
 
-        self.analysis_yaml_local_path = f'{self.analysis_yaml_local_path[:-5]}_{init_sim_num_w_offset}.yaml'
-        model_data_to_yaml(data_analysis, self.analysis_yaml_local_path)
+        analysis_file_path = f'{self.analysis_yaml_path[:-5]}_{init_sim_num_w_offset}.yaml'
+        model_data_to_yaml(data_analysis, analysis_file_path)
 
         if len(self.data_model_dakota.initial_steps_list) > 0:
-            a = AnalysisSTEAM(file_name_analysis=self.analysis_yaml_local_path, verbose=self.verbose)
+            a = AnalysisSTEAM(file_name_analysis=analysis_file_path, verbose=self.verbose)
             a.run_analysis(verbose=self.verbose)
             #a.store_model_objects(path_output_file=os.path.join(os.path.dirname(self.analysis_yaml_local_path), 'temp.pkl'))
 
 
     def _write_driver_link(self):
         """
         Writes driver_link.py file that is used to serve as a black box script for running Driver Analysis of SDK
         :return: Nothing, writes file on disk in the local_Dakota_folder
         :rtype: None
         """
-        path_to_driver_link = os.path.join(os.path.dirname(self.analysis_yaml_local_path), 'driver_link.py')
+        path_to_driver_link = os.path.join(self.output_path, 'driver_link.py')
         with open(path_to_driver_link, 'w') as f:
             f.write('from steam_sdk.drivers.DriverAnalysis import DriverAnalysis')
-            f.write(f'\nda = DriverAnalysis(analysis_yaml_path=r"{self.analysis_yaml_local_path}", iterable_steps={self.data_model_dakota.iterable_steps_list}, sim_number_offset={self.data_model_dakota.sim_number_offset})')
+            f.write(f'\nda = DriverAnalysis(analysis_yaml_path=r"{self.analysis_yaml_path}", iterable_steps={self.data_model_dakota.iterable_steps_list}, sim_number_offset={self.data_model_dakota.sim_number_offset})')
             f.write('\nda.run()')
 
 
     def _run_dakota_iterable_steps(self):
         """
         Runs dakota.exe with the input file specified. This will use DriverAnalysis and iterable_steps
         """
         # Change folder to local_Dakota_folder i.e. where the driver_link.py was saved, otherwise Dakota will not find it
-        os.chdir(os.path.dirname(self.analysis_yaml_local_path))
-        print(f'`Changed working directory to: {os.path.dirname(self.analysis_yaml_local_path)}')
+        os.chdir(self.output_path)
+        print(f'`Changed working directory to: {self.output_path}')
 
         # Call dakota and give up control of the flow from now on as Dakota takes over from now on. It will call driver_link and DriverAnalysis of the SDK to be able to run the analysis.
-        input_file_path = os.path.join(os.path.dirname(self.analysis_yaml_local_path), "dakota_in.in")
+        input_file_path = os.path.join(self.output_path, "dakota_in.in")
         print(f'Calling Dakota with {input_file_path}')
         subprocess.call([self.settings.Dakota_path, '-i', input_file_path])
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/drivers/DriverFiQuS.py` & `steam-sdk-2024.4.0/steam_sdk/drivers/DriverFiQuS.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from operator import call
 import os
 import sys
 import subprocess
 import json
 
 
 class DriverFiQuS:
@@ -43,34 +44,46 @@
         """
         Method to run FiQuS with a given input file name. The run type is specified in the input file.
         :param return_summary: summary of relevant parameters
         :rtype return_summary: dict
         :param sim_file_name: name of the input file (without .yaml) that must be inside the path_folder_FiQuS_input specified in the initialization
         :type sim_file_name: str
         """
-        call_commands_list = [
-            sys.executable,
-            os.path.join(self.FiQuS_path, 'fiqus', 'MainFiQuS.py'),
-            '--in', os.path.join(self.path_folder_FiQuS_input, sim_file_name + '.yaml'),
-            '--out', self.path_folder_FiQuS_output,
-            '--getdp', self.GetDP_path,
-        ]
-        if self.verbose:
-            print(f'Calling MainFiQuS via Python Subprocess.call() with: {" ".join(call_commands_list)}')
-        try:
-            result = subprocess.call(call_commands_list)
-        except subprocess.CalledProcessError as e:
-            # Handle exceptions if the command fails
-            print("Error:", e)
-            if result != 0:
-                raise _error_handler(call_commands_list, result, "Command failed.")
-            return result
-        except subprocess.CalledProcessError as e:
-            # Handle exceptions if the command fails
-            raise _error_handler(call_commands_list, e.returncode, e.stderr)
+        if 'pypi' in self.FiQuS_path:
+            from fiqus.MainFiQuS import MainFiQuS
+            try:
+                MainFiQuS(
+                    input_file_path=os.path.join(self.path_folder_FiQuS_input, sim_file_name + '.yaml'),
+                    model_folder=self.path_folder_FiQuS_output,
+                    GetDP_path=self.GetDP_path,
+                )
+            except Exception as e:
+                print(f"Error: {e}")
+        else:
+            call_commands_list = [
+                sys.executable,
+                os.path.join(self.FiQuS_path, 'fiqus', 'MainFiQuS.py'),
+                '--in', os.path.join(self.path_folder_FiQuS_input, sim_file_name + '.yaml'),
+                '--out', self.path_folder_FiQuS_output,
+                '--getdp', self.GetDP_path,
+            ]
+            if self.verbose:
+                print(f'Calling MainFiQuS via Python Subprocess.call() with: {" ".join(call_commands_list)}')
+            try:
+                result = subprocess.call(call_commands_list)
+            except subprocess.CalledProcessError as e:
+                # Handle exceptions if the command fails
+                print("Error:", e)
+                if result != 0:
+                    raise _error_handler(call_commands_list, result, "Command failed.")
+                return result
+            except subprocess.CalledProcessError as e:
+                # Handle exceptions if the command fails
+                raise _error_handler(call_commands_list, e.returncode, e.stderr)
+            
         if return_summary:
             summary = json.load(open(f"{os.path.join(self.path_folder_FiQuS_output, sim_file_name)}.json"))
             return summary
 
 class _error_handler(Exception):
     def __init__(self, command, return_code, stderr):
         self.command = command
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/drivers/DriverLEDET.py` & `steam-sdk-2024.4.0/steam_sdk/drivers/DriverLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/drivers/DriverPSPICE.py` & `steam-sdk-2024.4.0/steam_sdk/drivers/DriverPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/drivers/DriverProteCCT.py` & `steam-sdk-2024.4.0/steam_sdk/drivers/DriverProteCCT.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,14 +22,18 @@
         ** Run ProteCCT model **
         :param simFileName: Name of the simulation file to run
         :param outputDirectory: Relative path of the input directory with respect to path_folder_ProteCCT
         :param outputDirectory: Relative path of the output directory with respect to path_folder_ProteCCT
         :return:
         '''
 
+        # Quick workaround to allow running the simulation no matter whether simFileName contains ".xlsx" or not
+        if simFileName.endswith('.xlsx'):
+            simFileName = simFileName.strip('.xlsx')
+
         full_path_input  = os.path.join(self.path_folder_ProteCCT, inputDirectory, simFileName + '.xlsx')
         full_path_output = os.path.join(self.path_folder_ProteCCT, outputDirectory)
 
         if not os.path.isdir(full_path_output):
             print("Output folder {} does not exist. Making it now".format(full_path_output))
             Path(full_path_output).mkdir(parents=True)
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/drivers/DriverPyBBQ.py` & `steam-sdk-2024.4.0/steam_sdk/drivers/DriverPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/drivers/DriverPySIGMA.py` & `steam-sdk-2024.4.0/steam_sdk/drivers/DriverPySIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/drivers/DriverXYCE.py` & `steam-sdk-2024.4.0/steam_sdk/drivers/DriverXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/CSD_Reader.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/CSD_Reader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/ParserCond2d.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/ParserCond2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/ParserCsd.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/ParserCsd.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/ParserCsv.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/ParserCsv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import os
+from typing import Dict
+
 import numpy as np
 import pandas as pd
 import ruamel.yaml
 import csv
 from steam_sdk.parsers.ParserYAML import dict_to_yaml
+from steam_sdk.utils.make_folder_if_not_existing import make_folder_if_not_existing
 
 
 def getSpecificSignalCSV(path_sim, model_name, simNumber, list_Signals):
 
     simulationSignalsToPlot = pd.DataFrame()
 
     for i in range(len(simNumber)):
@@ -32,22 +35,23 @@
     '''
     Reads a csv file and returns a dataframe with the selected signals
     :param full_name_file: full path to the csv file
     :param list_signals: list of signals to read
     :return: dataframe with the selected signals
     '''
 
-    if type(list_signals) == str: list_signals = [list_signals]           # If only one signal is passed as an argument, make it a list
+    # If only one signal is passed as an argument, make it a list
+    if type(list_signals) == str:
+        list_signals = [list_signals]
 
     all_signals_df = pd.read_csv(full_name_file)                          # read file into a dataframe
     all_signals_df.columns = all_signals_df.columns.str.replace(' ', '')  # eliminate whitespaces from the column names
     list_signals = [x.replace(' ', '') for x in list_signals]             # eliminate whitespaces from the signal names as well
     return all_signals_df[list_signals]
 
-
 def load_global_parameters_from_csv(filename: str, circuit_name: str, steam_models_path: str, case_model: str, flag_write_file:bool=False):
     '''
         Reads a csv file and circuit name and checks that the global parameters for the circuit are consistent with the csv file. If not, changes are made in the circuit parameters
         :param filename: full path to the csv file
         :param circuit_name: circuit name eg. RCS.A12B1
         :param steam_models_path: path to steam models
         :param case_model: folder within steam models eg. circuit or magnet
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/ParserDakota.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/ParserDakota.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,39 +8,38 @@
 from steam_sdk.utils.make_folder_if_not_existing import make_folder_if_not_existing
 
 class ParserDakota:
 
     @staticmethod
     def assemble_in_file(
             data_model_dakota: DataModelParsimDakota,
-            settings: DataSettings,
-            dakota_in_folder_path: str = None,
-            output_file_name = None
+            dakota_working_folder: str = None,
+            dakota_file_name: str = "dakota_in.in"
             ):
         """
         Generates Dakota compatible input file (with the .in extension) from TEAM SDK Dakota yaml file. It uses the template file of .in file.
         :param data_model_dakota: data class of data model dakota
         :type data_model_dakota: List[str]
-        :param settings: settings object
-        :type settings: DataSettings
-        :param dakota_in_folder_path: optional output path (mostly used for testing)
-        :param output_file_name: allows changing output file name (mostly used for testing)
-        :type output_file_name: str
-        :type dakota_in_folder_path: str
+        :param dakota_working_folder: optional output path (mostly used for testing)
+        :type dakota_working_folder: str
+        :param dakota_file_name: optional output path (mostly used for testing)
+        :type dakota_file_name: str
         :return: Writes .in file to disk
         :rtype: None
         """
 
         # prepare dakota data for easier looping in the template
         dd = DataDakota()
         for name, var in data_model_dakota.study.variables.items():
             if data_model_dakota.study.type == 'multidim_parameter_study':
                 dd.partitions.append(var.data_points - 1)
-            elif data_model_dakota.study.type == 'optpp_q_newton':
+            elif data_model_dakota.study.type in ['optpp_q_newton','coliny_pattern_search']:
                 dd.initial_point.append(var.initial_point)
+                if(var.scale_type):
+                    dd.scaling.append(var.scale_type)
                 #dd.descriptors.append(var.descriptors)
             dd.lower_bounds.append(var.bounds.min)
             dd.upper_bounds.append(var.bounds.max)
 
         # load template
         loader = FileSystemLoader(templates.__path__)
         env = Environment(loader=loader, variable_start_string='<<', variable_end_string='>>',
@@ -49,17 +48,12 @@
         template = 'template_Dakota.in'
         in_template = env.get_template(template)
 
         # propagate data in the template
         output_from_parsed_template = in_template.render(dmd=data_model_dakota, dd=dd)
 
         # prepare output folder and file path
-        if not dakota_in_folder_path:
-            dakota_in_folder_path = os.path.join(settings.local_Dakota_folder, data_model_dakota.parsim_name)
-        make_folder_if_not_existing(dakota_in_folder_path)
-        if not output_file_name:
-            output_file_name = "dakota_in.in"
-        dakota_in_output_file_path = os.path.join(dakota_in_folder_path, output_file_name)
+        dakota_in_output_file_path = os.path.join(dakota_working_folder, dakota_file_name)
 
         # save output file in the dakota_in_output_folder_path
         with open(dakota_in_output_file_path, "w") as tf:
             tf.write(output_from_parsed_template)
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/ParserExcel.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/ParserExcel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/ParserFiQuS.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/ParserFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/ParserLEDET.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/ParserLEDET.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 import openpyxl
 import json
 import ruamel.yaml
 
 from steam_sdk.builders.BuilderLEDET import BuilderLEDET
 from steam_sdk.data.DataLEDET import LEDETInputs, LEDETOptions, LEDETPlots, LEDETVariables
 from steam_sdk.data.TemplateLEDET import get_template_LEDET_inputs_sheet, get_template_LEDET_options_sheet, get_template_LEDET_plots_sheet, get_template_LEDET_variables_sheet
-from steam_sdk.parsers import ParserMap2d
+from steam_sdk.parsers.ParserMap2d import ParserMap2dFile, ParserMap2dData
 from steam_sdk.parsers.ParserExcel import read_row, write2Excel
 from steam_sdk.parsers.ParserYAML import dict_to_yaml
 from steam_sdk.utils.NumpyEncoder import NumpyEncoder
 from steam_sdk.utils.rgetattr import rgetattr
 from steam_sdk.utils.sgetattr import rsetattr
 from steam_sdk.utils.compare_two_parameters import compare_two_parameters
+from steam_sdk.utils.MatrixOperations import multiply_column_by_value
 
 
 class ParserLEDET:
     """
         Class with methods to read/write LEDET information from/to other programs
     """
 
@@ -157,15 +158,15 @@
         template_LEDET_inputs_sheet    = get_template_LEDET_inputs_sheet()
         template_LEDET_options_sheet   = get_template_LEDET_options_sheet()
         template_LEDET_plots_sheet     = get_template_LEDET_plots_sheet()
         template_LEDET_variables_sheet = get_template_LEDET_variables_sheet()
 
         # Define optional variables, which will be written only if present in the dataclass
         optional_variables_input_sheet  = _getOptionalVariables_input()
-        optional_variables_output_sheet = _getOptionalVariables_output()
+        optional_variables_options_sheet = _getOptionalVariables_options()
 
         ### Inputs sheet
         name_sheet_inputs = 'Inputs'  # This defines the name of the sheet and also of the variable group
         LEDET_inputs_sheet = []
         for row in template_LEDET_inputs_sheet:
             name, description = row[0], row[2]
 
@@ -184,15 +185,15 @@
                     continue
                 elif isinstance(value, np.ndarray) and value.shape[0] == 0:
                     if verbose: print('Variable {} is optional and has 0 elements, hence it will be skipped.'.format(name))
                     continue
                 elif value is None:
                     if verbose: print('Variable {} is optional and has 0 elements, hence it will be skipped.'.format(name))
                     continue
-                elif isinstance(value, np.ndarray) and np.all(np.isnan(value)):
+                elif isinstance(value, np.ndarray) and np.all(np.isnan(value.astype(float))):
                     if verbose: print('Variable {} is optional and has only NaN elements, hence it will be skipped.'.format(name))
                     continue
 
             # Assign value to the variable sheet
             LEDET_inputs_sheet.append([name, value, description])
 
         ### Options sheet
@@ -206,15 +207,15 @@
                 LEDET_options_sheet.append(row)  # Leave the row unchanged
                 continue  # stop treating this row: go to the next row
 
             # Get value of the current parameter
             value = self.builder_ledet.getAttribute(name_sheet_options, name)
 
             # Skip optional variables if they have 0 elements
-            if name in optional_variables_output_sheet:
+            if name in optional_variables_options_sheet:
                 if isinstance(value, list) and len(value) == 0:
                     if verbose: print('Variable {} is optional and has 0 elements, hence it will be skipped.'.format(name))
                     continue
                 elif isinstance(value, np.ndarray) and value.shape[0] == 0:
                     if verbose: print('Variable {} is optional and has 0 elements, hence it will be skipped.'.format(name))
                     continue
                 elif value is None:
@@ -276,26 +277,26 @@
         '''
 
         # Unpack variables
         builder_ledet = self.builder_ledet
 
         # Define optional variables, which will be written only if present in the dataclass
         optional_variables_input_sheet = _getOptionalVariables_input()
-        optional_variables_output_sheet = _getOptionalVariables_output()
+        optional_variables_options_sheet = _getOptionalVariables_options()
 
         # Write LEDET data into a dictionary
         ledet_data_dict = {
             **builder_ledet.Inputs.__dict__,
             **builder_ledet.Options.__dict__,
             **builder_ledet.Plots.__dict__,
             **builder_ledet.Variables.__dict__}  # to add program-specific variables
 
         # Skip optional variables if they have 0 elements, or if they are all NaN
         for name, value in ledet_data_dict.copy().items():
-            if (name in optional_variables_input_sheet) or (name in optional_variables_output_sheet):
+            if (name in optional_variables_input_sheet) or (name in optional_variables_options_sheet):
                 if isinstance(value, list) and len(value) == 0:
                     if verbose: print('Variable {} is optional and has 0 elements, hence it will be skipped.'.format(name))
                     del ledet_data_dict[name]
                 elif isinstance(value, np.ndarray) and value.shape[0] == 0:
                     if verbose: print('Variable {} is optional and has 0 elements, hence it will be skipped.'.format(name))
                     del ledet_data_dict[name]
                 elif value is None:
@@ -333,26 +334,26 @@
         '''
 
         # Unpack variables
         builder_ledet = self.builder_ledet
 
         # Define optional variables, which will be written only if present in the dataclass
         optional_variables_input_sheet = _getOptionalVariables_input()
-        optional_variables_output_sheet = _getOptionalVariables_output()
+        optional_variables_options_sheet = _getOptionalVariables_options()
 
         # Write LEDET data into a dictionary
         ledet_data_dict = {
             **builder_ledet.Inputs.__dict__,
             **builder_ledet.Options.__dict__,
             **builder_ledet.Plots.__dict__,
             **builder_ledet.Variables.__dict__}  # to add program-specific variables
 
         # Skip optional variables if they have 0 elements, or if they are all NaN
         for name, value in ledet_data_dict.copy().items():
-            if (name in optional_variables_input_sheet) or (name in optional_variables_output_sheet):
+            if (name in optional_variables_input_sheet) or (name in optional_variables_options_sheet):
                 if isinstance(value, list) and len(value) == 0:
                     if verbose: print('Variable {} is optional and has 0 elements, hence it will be skipped.'.format(name))
                     del ledet_data_dict[name]
                 elif isinstance(value, np.ndarray) and value.shape[0] == 0:
                     if verbose: print('Variable {} is optional and has 0 elements, hence it will be skipped.'.format(name))
                     del ledet_data_dict[name]
                 elif value is None:
@@ -464,34 +465,36 @@
     #######################  Helper methods - END  #######################
 
 
 #######################  Helper functions - START  #######################
 def _getOptionalVariables_input():
     # Define optional variables, which will be written only if present in the dataclass
     optional_variables_input_sheet = [
+        'dcore_inGroup',
+        'dfilamentary_inGroup',
         'alpha_Nb3Sn_inGroup',
         'f_scaling_Jc_BSCCO2212_inGroup',
         'overwrite_f_internalVoids_inGroup', 'overwrite_f_externalVoids_inGroup',
         'f_RRR1_Cu_inGroup', 'f_RRR2_Cu_inGroup', 'f_RRR3_Cu_inGroup',
         'RRR1_Cu_inGroup', 'RRR2_Cu_inGroup', 'RRR3_Cu_inGroup',
         'R_EE_power',
         ]
     return optional_variables_input_sheet
 
 
-def _getOptionalVariables_output():
-    optional_variables_output_sheet = [
+def _getOptionalVariables_options():
+    optional_variables_options_sheet = [
         'fieldMapNumber',
         'selfMutualInductanceFileNumber',
         'flag_calculateMagneticField',
         'flag_controlInductiveVoltages',
         'flag_controlMagneticField',
         'flag_controlBoundaryTemperatures',
         ]
-    return optional_variables_output_sheet
+    return optional_variables_options_sheet
 
 
 def CompareLEDETParameters(fileA: str, fileB: str, max_relative_error: float=1E-5, verbose=False):
     '''
         Compare all the variables imported from two LEDET Excel input files
         Returns True if the two files contain LEDET parameters that differ by less than a certain relative error. Returns False otherwise.
     '''
@@ -604,23 +607,20 @@
         suffix_self = "_WithSelfField"
     else:
         suffix_self = "_NoSelfField"
 
     suffix_complete = suffix + suffix_iron + suffix_self + suffix_map2d_set
     file_name_output = magnet_name + suffix_complete + ".map2d"
 
-    # Get data of (old) ROXIE file
-    content_ROXIE_file = open(map2d_file_name, "r").read().split("\n")
-
     # Parse to ParserMap2d
-    NewMap2d = ParserMap2d.modify_map2d_ribbon_cable(map2d_file_name, geometry_ribbon_cable, list_flag_ribbon)
+    NewMap2d = ParserMap2dFile(map2dFile=Path(map2d_file_name)).modify_map2d_ribbon_cable(
+        geometry_ribbon_cable=geometry_ribbon_cable, list_flag_ribbon=list_flag_ribbon)
     # Multiply 3rd,4th and 7th column to not have SI-Units
-    ParserMap2d.multiply_column_by_value(NewMap2d, 3, 1000)
-    ParserMap2d.multiply_column_by_value(NewMap2d, 4, 1000)
-    ParserMap2d.multiply_column_by_value(NewMap2d, 7, 1000000)
+    multiply_column_by_value(matrix=NewMap2d, column_number=3, multiplication_factor=1000)
+    multiply_column_by_value(matrix=NewMap2d, column_number=4, multiplication_factor=1000)
+    multiply_column_by_value(matrix=NewMap2d, column_number=7, multiplication_factor=1000000)
     # Create .map2d file from ParserMap2d_
-    ParserMap2d.create_map2d_file(NewMap2d, header_line=content_ROXIE_file[0],
-                                  output_file_location=Path(output_path, file_name_output),
-                                  new_file_name=file_name_output,verbose=verbose)
+    ParserMap2dData(map2d_input=NewMap2d, output_folder_path=Path(output_path),
+                    physical_quantity='magnetic_flux_density').create_map2d_file_from_matrix(file_name=file_name_output)
 
     return file_name_output
 #######################  Helper functions - END  #######################
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/ParserMat.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/ParserMat.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,25 +150,28 @@
 
             simulationSignal = simulationSignal.flatten()
             df = pd.DataFrame({label_signal: simulationSignal})
             df_signals = pd.concat([df_signals, df], axis=1)
     return df_signals
 
 
-def get_signals_from_mat_to_dict(full_name_file: str, list_signals, bool_transpose: bool = True):
+def get_signals_from_mat_to_dict(full_name_file: str, list_signals, bool_transpose: bool = True,
+                                 dict_variable_types: dict = {}):
     '''
     Reads a mat file and returns a dataframe with the selected signals
 
     Note: The selected signals can also be define with a special syntax that allows accessing one certain row or column (1-indexed).
           Example: U_CoilSections(:,2) allows reading the 2nd column of the variable named U_CoilSections
           Example: U_CoilSections(3,:) allows reading the 3rd row of the variable named U_CoilSections
           Multiple columns/rows selection not currently supported  #TODO it would be nice to add
 
     :param full_name_file: full path to the mat file
     :param list_signals: list of signals to read
+    :param dict_variable_types: Optional variable to define the type of variable to read from a .mat file (the values in the dictionary can be "0D", "1D", or "2D")
+    :type dict_variable_types: dict
     :return: dict with the selected signals
     '''
 
     with h5py.File(full_name_file, 'r') as simulationSignals:
         dict_signals = {}
         number_of_time_steps = len(simulationSignals['time_vector'])  #TODO it is bad to hard-code this logic!
         for label_signal in list_signals:
@@ -176,15 +179,14 @@
                 # Special case: Only certain columns will be read
                 label_signal_split = label_signal.split('(')
                 signal        = label_signal_split[0]
                 rows_columns  = label_signal_split[1].rstrip(')').split(',')
                 label_rows    = rows_columns[0]
                 label_columns = rows_columns[1]
 
-
                 # Find slice of selected rows
                 if label_rows == ':':
                     rows = slice(0, simulationSignals[signal].shape[1])
                 elif ':' in label_rows:
                     raise Exception('Multiple rows selection not currently supported.')
                     # label_rows_split = label_rows.split(':')
                     # rows = slice(int(label_rows_split[0]) - 1, int(label_rows_split[1]) - 1)
@@ -210,14 +212,26 @@
                 # Regular case: One-column signal is read
                 if bool_transpose:
                     simulationSignal = np.array(simulationSignals[label_signal]).T
                 else:
                     simulationSignal = np.array(simulationSignals[label_signal])
 
             dict_signals[label_signal] = simulationSignal
+
+        # Optional: Adjust each variable to the correct type (0D, 1D, 2D)
+        for signal, signal_type in dict_variable_types.items():
+            if signal_type == '0D':
+                dict_signals[signal] = dict_signals[signal][0, 0]
+            elif signal_type == '1D':
+                if dict_signals[signal].shape[0] == 1:
+                    dict_signals[signal] = dict_signals[signal][0]  # get the first column
+                elif dict_signals[signal].shape[1] == 1:
+                    dict_signals[signal] = dict_signals[signal].T[0]  # transpose and get first column
+            elif signal_type == '2D':
+                dict_signals[signal] = np.array(dict_signals[signal])
     return dict_signals
 
 
 def print_shapes_of_entries(simulationSignals):
     shapes_dict = {}
     for key, value in simulationSignals.items():
         # Check if the value is a dataset
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/ParserPSPICE.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/ParserPSPICE.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import pandas as pd
 from scipy.interpolate import UnivariateSpline
 from scipy.interpolate import interp1d
 
 from steam_sdk.data.DataModelCircuit import DataModelCircuit, Component
 from steam_sdk.parsers.ParserYAML import dict_to_yaml, model_data_to_yaml
 from steam_sdk.parsers.utils_ParserCircuits import read_circuit_data_from_model_data
+from steam_sdk.utils.make_folder_if_not_existing import make_folder_if_not_existing
 
 
 class ParserPSPICE:
     """
         Class with methods to read/write PSPICE information from/to other programs
     """
 
@@ -378,14 +379,15 @@
         '''
         ** Writes a PSPICE netlist file **
 
         :param full_path_file_name:
         :param verbose:
         :return:
         '''
+        make_folder_if_not_existing(os.path.dirname(full_path_file_name), verbose=verbose)
 
         # Prepare header
         time_start = datetime.datetime.now()
         rows_header = [
             add_comment('PSPICE Netlist Simulation File'),
             add_comment(f'Generated at {time_start} at CERN using STEAM_SDK'),
             add_comment('Authors: STEAM Team'),
@@ -648,14 +650,16 @@
         '''
             Copy additional files
             :param output_path: Output folder
             :param verbose: If True, display logging information
         :return: Number of copied files
         '''
 
+        make_folder_if_not_existing(output_path, verbose=verbose)
+
         list_files_to_copy = self.circuit_data.GeneralParameters.additional_files
         # Special case: Copy coil_resistances.stl file as well (this file is used for co-simulations)
         list_files_to_copy.append('coil_resistances.stl')
 
         for file_to_copy in list_files_to_copy:
             if not os.path.isabs(file_to_copy) and self.path_input:
                 # If the provided path is relative, use the path_input as the root folder (if available)
@@ -1024,14 +1028,17 @@
     (e.g. if there are three items in the path_resources list and four magnets, then magnet_type can be [2,2,1,1] or [1,2,3,3] telling us which path_resource file to use for each magnet
     :param Type: str, either Linear or Spline, type of interpolation
     :param type_stl: str, how to write the stimuli file (either 'a' (append) or 'w' (write))
     :param sparseTimeStepping: int, every x-th time value only a stimuli point is written (to reduce size of stimuli)
     : param time_additional_zero_resistance: float, this defines the time shift of an additional point that is added before the first coil resistance row
     :return:
     '''
+
+    make_folder_if_not_existing(os.path.dirname(Outputfile), verbose=False)
+
     # Check inputs and set default values
     if type(path_resources) == str:
         path_resources = [path_resources] * len(magnets)  # make a list out of the string
 
     if not magnet_type:
         magnet_type = [1] * len(magnets)  # make a list of 1's (to maintain the same behavior as the older version fo the function)
 
@@ -1156,14 +1163,16 @@
     :param current_levels: list with defined current levels
     :param list_times: list of lists, where each list defines the time vector at one current level 
     :param list_coil_resistances: list of lists, where each list defines the time vector at one current level
     :param format: string defining the format for the written variables
     :return: 
     '''
 
+    make_folder_if_not_existing(os.path.dirname(path_csv_file), verbose=False)
+
     columns_to_write = []
     for c, current in enumerate(current_levels):
         time_to_write = [format.format(t) for t in list_times[c]]
         R_to_write = [format.format(t) for t in list_coil_resistances[c]]
         columns_to_write.append([current, "time_vector"] + time_to_write)  # TODO remove the call to int() once the interpolation function can deal with it
         columns_to_write.append(["", "R_CoilSections_1"] + R_to_write)
         columns_to_write.append(["", ""] + len(list_times[c]) * [None])
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/ParserPdf.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/ParserPdf.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/ParserProteCCT.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/ParserProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/ParserPyBBQ.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/ParserPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/ParserPyCoSim.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/ParserPyCoSim.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import os.path
-
 from steam_sdk.data.DataModelCosim import DataModelCosim
 from steam_sdk.data.DataPyCoSim import DataPyCoSim
-from steam_sdk.parsers.ParserYAML import dict_to_yaml, model_data_to_yaml
+from steam_sdk.parsers.ParserYAML import model_data_to_yaml
 
 
 class ParserPyCoSim:
     """
         Class with methods to write PyCoSim input files
     """
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/ParserPySIGMA.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/ParserPySIGMA.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,83 @@
 import os
 import shutil
 import pandas as pd
 from pathlib import Path
 
+from steam_sdk.data.DataModelMagnet import DataModelMagnet
 from steam_sdk.parsers.ParserYAML import dict_to_yaml
 from steam_sdk.utils.make_folder_if_not_existing import make_folder_if_not_existing
 
 
 class ParserPySIGMA:
     """
         Class with methods to write SIGMA input files from sdk model data file
     """
 
-    def __init__(self, builder_SIGMA, output_path=None):
+    def __init__(self, builder_SIGMA: object, output_path: str):
         """
         Initialization using a BuilderFiQuS object containing FiQuS parameter structure
         :param builder_SIGMA: BuilderFiQuS object
+        :type builder_SIGMA: object
         :param output_path: full path to the output folder
+        :type output_path: str
         """
-
         self.builder_SIGMA = builder_SIGMA
         self.output_path = output_path
         make_folder_if_not_existing(output_path)
         self.attributes = ['data_SIGMA', 'data_SIGMA_geo', 'data_SIGMA_set']
         self.file_exts = ['yaml', 'geom', 'set']
 
-    def writeSIGMA2yaml(self, simulation_name=None):
+    def writeSIGMA2yaml(self, simulation_name=str):
         """
         ** Writes SIGMA input files **
-
         :param simulation_name: This is used in analysis steam to change yaml name from magnet name to simulation name
+        :type simulation_name: str
         :return:  Nothing, writes files to output folder.
+        :rtype None
         """
 
           # If the output folder is not an empty string, and it does not exist, make it
         for attribute, file_ext in zip(self.attributes, self.file_exts):
             yaml_file_name = f'{simulation_name}.{file_ext}'
             dict_to_yaml(getattr(self.builder_SIGMA, attribute).dict(), os.path.join(self.output_path, yaml_file_name), list_exceptions=[])
 
-        if self.builder_SIGMA.make_bh_copy:
-            source_path = Path(os.path.join(self.builder_SIGMA.path_model_folder, self.builder_SIGMA.model_data.Sources.BH_fromROXIE)).resolve()
-            destination_path = os.path.join(self.output_path, self.builder_SIGMA.data_SIGMA.Sources.bh_curve_source)
-            shutil.copy2(source_path, destination_path)
+        #if self.builder_SIGMA.make_bh_copy:
+        source_path = Path(os.path.join(self.builder_SIGMA.path_model_folder, self.builder_SIGMA.data_SIGMA.Sources.bh_curve_source)).resolve()
+        destination_path = os.path.join(self.output_path, Path(self.builder_SIGMA.data_SIGMA.Sources.bh_curve_source).name)
+        shutil.copy2(source_path, destination_path)
 
-
-    def coordinate_file_preprocess(self, model_data=None):
+    def coordinate_file_preprocess(self, model_data: DataModelMagnet):
         """
         Function to copy map2d file and create coordinates.csv file.
+        :param model_data: Magnet model data
+        :type model_data: DataModelMagnet
+        :return: Nothing, just copies files
+        :rtype: None
         """
         magnet_name = model_data.GeneralParameters.magnet_name
         if model_data.Options_SIGMA.postprocessing.out_2D_at_points.coordinate_source is None:
             if model_data.Options_SIGMA.postprocessing.out_2D_at_points.map2d is not None:
                 source_map2d_path = Path(os.path.join(self.builder_SIGMA.path_model_folder, model_data.Options_SIGMA.postprocessing.out_2D_at_points.map2d)).resolve()
                 destination_map2d_path = os.path.join(self.output_path, magnet_name + "_ROXIE_REFERENCE.map2d")
                 shutil.copyfile(source_map2d_path, destination_map2d_path)
                 coordinate_file_path = os.path.join(self.output_path, magnet_name + "_ROXIE_COORD.csv")
                 self.create_coordinate_file(destination_map2d_path, coordinate_file_path)
                 return coordinate_file_path
 
-    def create_coordinate_file(self, path_map2d, coordinate_file_path):
+    @staticmethod
+    def create_coordinate_file(path_map2d: str, coordinate_file_path: str):
         """
         Creates a csv file with same coordinates as the map2d.
-
-        :param path_map2d: Map2d file to read coordinates from
+        :param path_map2d: map2d file to read coordinates from
+        :type path_map2d: str
         :param coordinate_file_path: Path to csv filw to be created
-        :return:
+        :type coordinate_file_path: str
+        :return: Nothing, write on disk
+        :rtype: None
         """
         df = pd.read_csv(path_map2d, delim_whitespace=True)
         df_new = pd.DataFrame()
         df_new["X-POS/MM"] = df["X-POS/MM"].apply(lambda x: x / 1000)
         df_new["Y-POS/MM"] = df["Y-POS/MM"].apply(lambda x: x / 1000)
         df_new.to_csv(coordinate_file_path, header=None, index=False)
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/ParserRoxie.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/ParserRoxie.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # import os
-import os
-from pathlib import Path
+import copy
 import math
+import os
 from math import *
+from pathlib import Path
+from typing import Dict, Union
+
 import numpy as np
 import yaml
-from typing import Dict, Union
+from matplotlib.patches import Arc
+
 # from matplotlib import cm
 # from matplotlib.colors import Normalize
 # from matplotlib import pyplot as plt, lines, patches
 # from matplotlib.lines import Line2D
 from steam_sdk.builders import geometricFunctions as gf
 from steam_sdk.data import DataRoxieParser as pd
-from matplotlib.patches import Arc
-from steam_sdk.data.DataModelMagnet import DataModelMagnet
-from steam_sdk.data.DataModelConductor import DataModelConductor
 from steam_sdk.data.DataConductor import Conductor, Rutherford
-from steam_sdk.parsers.ParserMap2d import getParametersFromMap2d
+from steam_sdk.data.DataModelConductor import DataModelConductor
+from steam_sdk.data.DataModelMagnet import DataModelMagnet
+from steam_sdk.parsers.ParserMap2d import ParserMap2dFile
 from steam_sdk.parsers.ParserYAML import yaml_to_data
 from steam_sdk.utils.ParserRoxieHelpers import find_iH_oH_iL_oL
-import copy
+from steam_sdk.utils.make_folder_if_not_existing import make_folder_if_not_existing
 
 
 def arc_angle_between_point_and_abscissa(p, c):
     """
         Returns the angle of an arc with center c and endpoints at (cx + radius, cy) and (px, py)
         :param p: list of x and y coordinates of a point
         :param c: list of x and y coordinates of the arc center
@@ -172,23 +175,23 @@
         """
         # Acquire required parameters
         if path_map2d is None:
             path_map2d: Path = Path.joinpath(path_input_file,
                                              model_data.Sources.magnetic_field_fromROXIE)  # By default, read the .map2d file defined in the yaml input file
         headerLines: int = model_data.Options_LEDET.field_map_files.headerLines
 
-        nT, nStrands_inGroup_ROXIE, polarities_inGroup, strandToHalfTurn, strandToGroup, x_strands, y_strands, I_strands \
-            = getParametersFromMap2d(map2dFile=path_map2d, headerLines=headerLines, verbose=verbose)
+        nT, nStrands_inGroup_ROXIE, polarities_inGroup, strandToHalfTurn, strandToGroup, x_strands, y_strands, I_strands, Bx, By \
+            = ParserMap2dFile(map2dFile=path_map2d).getParametersFromMap2d(headerLines=headerLines)
 
         indexTstop = np.cumsum(nT).tolist()
         indexTstart = [1]
         for i in range(len(nT) - 1):
             indexTstart.extend([indexTstart[i] + nT[i]])
 
-        return nT, nStrands_inGroup_ROXIE, polarities_inGroup, strandToHalfTurn, strandToGroup, indexTstart, indexTstop, x_strands, y_strands, I_strands
+        return nT, nStrands_inGroup_ROXIE, polarities_inGroup, strandToHalfTurn, strandToGroup, indexTstart, indexTstop, x_strands, y_strands, I_strands, Bx, By
 
     def getIronYokeDataFromIronFile(self, iron_content: str = None, verbose: bool = False):
         """
             **Parse the content of the entire .iron file and store it in a IronDatabase object**
 
             Function returns a IronDatabase object that contains information about the iron yoke
 
@@ -625,14 +628,15 @@
 
     def write_cadata_file(self, output_file_name: str):
         '''
         Write a valid cadata file with the parameters (compatible with ROXIE version 11)
         :param output_file_name: path to the output file
         :return:
         '''
+        make_folder_if_not_existing(os.path.dirname(output_file_name), verbose=False)
 
         # Unpack input
         insulations = self.rawData.cadata.insul
         remfits     = self.rawData.cadata.remfit
         filaments   = self.rawData.cadata.filament
         strands     = self.rawData.cadata.strand
         transients  = self.rawData.cadata.transient
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/ParserTdms.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/ParserTdms.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,16 @@
 
     def writeTdmsToCsv(self, path_output: str, dictionary: Dict):
         """
             This function writes the signals of the signal_data dictionary of this class of a .tdms file to a specific csv file.
             dictionary for header with names of the groups and signal that are used in the .tdms file
             header: Groupname_signalname, ....
         """
+        make_folder_if_not_existing(os.path.dirname(path_output), verbose=False)
+
         # Get signal
         # signal_output = getspecificSignal(path_tdms, group_name, signal_name)
         # np.savetxt(path_output, signal_output, delimiter=",")
         # headers, units,...
         header = []
         for group in dictionary.keys():
             for channel in dictionary[group]:
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/ParserXYCE.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/ParserXYCE.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,30 +7,32 @@
 from pathlib import Path
 
 import pandas as pd
 
 from steam_sdk.data.DataModelCircuit import DataModelCircuit, Component
 from steam_sdk.parsers.ParserYAML import dict_to_yaml
 from steam_sdk.parsers.utils_ParserCircuits import read_circuit_data_from_model_data
+from steam_sdk.utils.make_folder_if_not_existing import make_folder_if_not_existing
 
 
 class ParserXYCE:
     """
         Class with methods to read/write XYCE information from/to other programs
     """
 
     def __init__(self, circuit_data: DataModelCircuit, path_input: Path = None, output_path: str = ''):
         """
             Initialization using a DataModelCircuit object containing circuit netlist structure
         """
-
         self.circuit_data: DataModelCircuit = circuit_data
         self.path_input: str = path_input
         self.output_path: str = output_path
 
+        make_folder_if_not_existing(output_path, verbose=True)
+
 
     def read_netlist(self, full_path_file_name: str, flag_acquire_auxiliary_files: bool = False, verbose: bool = False):
         '''
         ** Reads a XYCE netlist file **
 
         :param full_path_file_name:
         :param flag_acquire_auxiliary_files: If True, add list of additional files to circuit_data
@@ -358,24 +360,42 @@
         self.flag_read_parametrized_component = False
         self.flag_read_options = False
         self.flag_read_autoconverge = False
         self.flag_read_time_schedule = False
         self.flag_read_probe = False
         self.name_last_component = None  # this is used to have the name of the latest added component (used to read the parameters of parametrized component over multiple rows)
 
-
-    def write2XYCE(self, full_path_file_name: str, verbose: bool = False):
+    def write2XYCE(self, full_path_file_name: str,
+                   flag_copy_additional_files: bool = False,
+                   flag_resolve_library_paths: bool = False,
+                   verbose: bool = False):
         '''
         ** Writes a XYCE netlist file **
 
-        :param full_path_file_name:
-        :param verbose:
+        :param full_path_file_name: Full path to the netlist file to write
+        :param flag_copy_additional_files: If True, copy additional files specified in the data model input yaml file
+        :param flag_resolve_library_paths: If True, edit the paths to component libraries (XYCE requires absolute paths to be defined)
+        :param verbose: If True, display logging information
         :return:
         '''
-        current_path = Path(full_path_file_name).parent.resolve()
+        file_name = os.path.basename(full_path_file_name)
+        output_path = Path(full_path_file_name).parent.resolve()  # This is the folder where the output file will be generated
+        make_folder_if_not_existing(output_path, verbose=verbose)
+
+        # Copy additional files
+        if flag_copy_additional_files:
+            if verbose:
+                print('Copy additional files.')
+            self._copy_additional_files(flag_translate=True, verbose=verbose)
+
+        # Resolve library paths (XYCE requires absolute paths)
+        if flag_resolve_library_paths:
+            if verbose:
+                print('Resolve library paths (XYCE requires absolute paths).')
+            self._resolve_library_paths(verbose=verbose)
 
         # Title of the circuit
         row_title = [f'{self.circuit_data.GeneralParameters.circuit_name} \n']
 
         # Prepare header
         time_start = datetime.datetime.now()
         rows_header = [
@@ -449,15 +469,15 @@
                     raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(s+1, type))
                 if verbose: print('Netlist entry {} in position #{} is treated as a standard component.'.format(name, s + 1))
                 rows_netlist.append(add_standard_component(name, nodes, value))
             elif type == 'stimulus-controlled component':
                 if name == None or nodes == None or value == None:
                     raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(s+1, type))
                 if verbose: print('Netlist entry {} in position #{} is treated as a stimulus-controlled component.'.format(name, s + 1))
-                rows_netlist.append(add_stimulus_controlled_component(name, nodes, value, output_path = current_path))
+                rows_netlist.append(add_stimulus_controlled_component(name, nodes, value, output_path=output_path))
             elif type == 'pulsed-source component':
                 if name == None or nodes == None or value == None:
                     raise Exception('Netlist component in position #{} is of type {} and requires name, nodes, and value.'.format(s+1, type))
                 if verbose: print('Netlist entry {} in position #{} is treated as a pulsed-source component.'.format(name, s + 1))
                 rows_netlist.append(add_pulsed_source_component(name, nodes, value))
             elif type == 'controlled-source component':
                 if name == None or nodes == None or value == None:
@@ -482,36 +502,43 @@
             else:
                 raise Exception ('Netlist entry {} in position #{} has an unknown type: {}.'.format(name, s+1, type))
 
         # Prepare options - Simulation options
         rows_options = []
         options = self.circuit_data.Options.options_simulation
 
-        keywords_timeInt = ['METHOD', 'RELTOL', 'ABSTOL', 'RESTARTSTEPSCALE'] # Not complete list, but most used
-        keywords_NonLinSolv = ['NLSTRATEGY', 'SEARCHMETHOD', 'CONTINUATION', 'RELTOL', 'ABSTOL', 'DELTAXTOL', 'RHSTOL']
+        keywords_timeInt = ['method', 'reltol', 'abstol', 'restartstepscale', 'nlnearconv'] # Not complete list, but most used
+        keywords_NonLinSolv = ['nlstrategy', 'searchmethod', 'continuation', 'reltol', 'abstol', 'deltaxtol', 'rhstol']
         keywords_LinSolv = ['type']
+        keywords_NonLinTranSolv = ['NOX','RHSTOL']
 
         if options:
             # Add comment and .OPTIONS command before the first entry
             rows_options.append(add_comment('**** Simulation parameters ****'))  # Add header of this section
 
-            overlap_timeInt = [i for i in keywords_timeInt if i in list(options.keys())]
-            overlap_NonLinSolv = [i for i in keywords_NonLinSolv if i in list(options.keys())]
-            overlap_LinSolv = [i for i in keywords_LinSolv if i in list(options.keys())]
+            overlap_timeInt = [i for i in list(options.keys()) if i.casefold()  in keywords_timeInt]
+            overlap_NonLinSolv = [i for i in list(options.keys()) if i.casefold()  in keywords_NonLinSolv]
+            overlap_NonLinTranSolv = [i for i in list(options.keys()) if i.casefold() in keywords_NonLinTranSolv]
+            overlap_LinSolv = [i for i in list(options.keys()) if i.casefold()  in keywords_LinSolv]
 
             if overlap_timeInt:
                 rows_options.append('.OPTIONS TIMEINT')  # Add header of this section
                 # Add option entries
                 for name in overlap_timeInt:
                     rows_options.append(add_option(name, options[name]))
             if overlap_NonLinSolv:
                 rows_options.append('.OPTIONS NONLIN')  # Add header of this section
                 # Add option entries
                 for name in overlap_NonLinSolv:
                     rows_options.append(add_option(name, options[name]))
+            if overlap_NonLinTranSolv:
+                rows_options.append('.OPTIONS NONLIN-TRAN')  # Add header of this section
+                # Add option entries
+                for name in overlap_NonLinSolv:
+                    rows_options.append(add_option(name, options[name]))
             if overlap_LinSolv:
                 rows_options.append('.OPTIONS LINSOL')  # Add header of this section
                 # Add option entries
                 for name in overlap_LinSolv:
                     rows_options.append(add_option(name, options[name]))
 
 
@@ -564,16 +591,17 @@
             raise Exception('Analysis entry has an unknown type: {}.'.format(analysis_type))
 
         # Prepare post-processing settings
         rows_post_processing = []
         probe_type = self.circuit_data.PostProcess.probe.probe_type
         probe_variables = self.circuit_data.PostProcess.probe.variables
         if probe_type:
-            rows_post_processing.append(add_probe(probe_type, probe_variables, self.circuit_data.Analysis.analysis_type,
-                                                  os.path.join(current_path, self.circuit_data.GeneralParameters.circuit_name)))
+            rows_post_processing.append(add_probe(probe_type=probe_type, probe_variables=probe_variables,
+                                                  analysis_type=self.circuit_data.Analysis.analysis_type,
+                                                  csd_path=os.path.join(output_path, os.path.splitext(file_name)[0])))
 
         # Prepare file end
         rows_file_end = [add_end_file()]
 
         # Assemble all rows to write
         rows_to_write = \
             row_title + \
@@ -629,79 +657,70 @@
             ]
 
         all_data_dict = {**self.circuit_data.dict()}
         dict_to_yaml(all_data_dict, full_path_file_name, list_exceptions=list_exceptions)
         if verbose:
             print('New file ' + full_path_file_name + ' generated.')
 
-
-    def copy_additional_files(self, flag_translate: bool = False, verbose: bool = False):
+    def _copy_additional_files(self, flag_translate: bool = False, verbose: bool = False):
         '''
             Copy additional files
         :return: Number of copied files
         '''
         for file_to_copy in self.circuit_data.GeneralParameters.additional_files+self.circuit_data.Stimuli.stimulus_files:
             if not os.path.isabs(file_to_copy) and self.path_input:
                 # If the provided path is relative, use the path_input as the root folder (if available)
                 if file_to_copy in self.circuit_data.GeneralParameters.additional_files:
                     file_to_copy_relative = Path(os.path.join(self.path_input, file_to_copy)).resolve()
                 else:
                     file_to_copy_relative = Path(os.path.join(self.output_path, file_to_copy)).resolve()
                 if verbose:
-                    print('Relative path changed from {} to {}.'.format(file_to_copy, file_to_copy_relative))
+                    print(f'Relative path changed from {file_to_copy} to {file_to_copy_relative}.')
                 file_to_copy = file_to_copy_relative
                 
             file_name = ntpath.basename(file_to_copy)
             file_to_write = os.path.join(self.output_path, file_name)
             if os.path.isfile(os.path.join(file_to_copy)):
                 if verbose: print('File {} exists'.format(file_to_copy))
             else:
                 if verbose: print('File {} does not exist. Skipped.'.format(file_to_copy))
                 continue
-            if os.path.isdir(self.output_path):
-                if verbose: print('Dir {} exists'.format(self.output_path))
-            else:
-                if verbose: print('Dir {} does not exist. Skipped.'.format(self.output_path))
-                continue
             if flag_translate and str(file_to_copy).endswith('.lib'):
                 ## TODO: Temporary fix, until merged libraries!
                 if 'converter' in str(file_to_copy):   #generic_power_converters_XYCE.lib is used as PC library by XYCE instead of generic_power_converters.lib which is used by PSPICE
                     file_to_copy = list(file_to_copy)  #this if statement is used to make that change in library while using XYCE
                     file_to_copy.insert(-4, '_XYCE')
                     file_to_copy = ''.join(file_to_copy)
                 translate_library_PSPICE_2_XYCE(file_to_copy, file_to_write.replace('PSPICE','XYCE'))
             elif flag_translate and str(file_to_copy).endswith('.stl'):
                 # path_stl = str(Path(file_to_write+'/..').resolve())
-                path_stl = str(Path(file_to_write+'/..'+'/Stimulus').resolve())
-                if not os.path.exists(path_stl):
-                    os.mkdir(path_stl)
-                translate_stimulus('all', file_to_copy, path_output=path_stl)
+                path_stl = str(Path(file_to_write + '/..' + '/' + get_name_stimulus_folder()).resolve())
+                make_folder_if_not_existing(path_stl, verbose=verbose)
+                translate_stimulus('all', input_file_path=file_to_copy, output_path=path_stl)
             else:
-                shutil.copyfile(Path(file_to_copy), Path(file_to_write))
+                if not Path(file_to_copy)==Path(file_to_write):
+                    shutil.copyfile(Path(file_to_copy), Path(file_to_write))
 
             if verbose:
-                print('Additional file copied from {} to {}.'.format(file_to_copy, file_to_write))
+                print(f'Additional file copied from {file_to_copy} to {file_to_write}.')
         return len(self.circuit_data.GeneralParameters.additional_files)
 
-
-    def resolve_paths_netlist(self, full_path_file_name: str):
+    def _resolve_library_paths(self, verbose: bool = False):
         '''
         Helper function that resolves the library paths to the new, translated versions.
 
-        :param full_path_file_name: Name of the circuit file
+        :param verbose: If True, display logging information
         :return:
         '''
-        for i in range(len(self.circuit_data.Libraries.component_libraries)):
-            file_name = ntpath.basename(self.circuit_data.Libraries.component_libraries[i])
-            self.circuit_data.Libraries.component_libraries[
-                i] = str(Path(os.path.join(self.output_path, file_name)).resolve())
-
-        self.write2XYCE(full_path_file_name)
-
-        return
+        for i, old_path in enumerate(self.circuit_data.Libraries.component_libraries):
+            file_name = ntpath.basename(old_path)
+            new_path = str(Path(os.path.join(self.output_path, file_name)).resolve())
+            self.circuit_data.Libraries.component_libraries[i] = new_path
+            if verbose:
+                print(f'Changed path {old_path} to {new_path}.')
 
 
 #######################  Helper functions - START  #######################
 def add_comment(text: str):
     ''' Format comment row '''
     if text[0] == '*':
         return text  # If the input string starts with a "*", leave it unchanged (it is already a comment)
@@ -725,71 +744,78 @@
     ''' Format global parameters row '''
     formatted_text = '+ ' + name + '={' + str(value) + '}'
     return formatted_text
 
 
 def add_standard_component(name: str, nodes: list, value: str):
     ''' Format standard component netlist row '''
+    nodes = [str(x) for x in nodes]
     str_nodes = " ".join(nodes)  # string with space-separated nodes
     formatted_text = name + ' ' + str_nodes + ' ' + '{' + str(value) + '}'
     return formatted_text
 
 
 def add_nonlinear_source_component(name: str, nodes: list, value: str):
     ''' Format nonlinear-source component netlist row '''
+    nodes = [str(x) for x in nodes]
     str_nodes = " ".join(nodes)  # string with space-separated nodes
     formatted_text = name + ' ' + str_nodes + ' ' + str(value)
     return formatted_text
 
 
 def add_controlled_source_component(name: str, nodes: list, value: str):
     ''' Format controlled-source component netlist row '''
+    nodes = [str(x) for x in nodes]
     str_nodes = " ".join(nodes)  # string with space-separated nodes
     str_stimulus = 'VALUE ' + '{' + value + '}'
     if name.startswith('E'):
         str_stimulus = str_stimulus + ' smoothbsrc=1'
     formatted_text = name + ' ' + str_nodes + ' ' + str_stimulus
     return formatted_text
 
 
 def add_stimulus_controlled_component(name: str, nodes: list, value: str, output_path = ''):
     ''' Format stimulus-controlled component netlist row '''
+    nodes = [str(x) for x in nodes]
     str_nodes = " ".join(nodes)  # string with space-separated nodes
     if len(value.split(' '))==1:
         output_path = str(output_path).replace(os.sep, '/')
         str_stimulus = 'PWL FILE ' + output_path + '/Stimulus/' + value + '.csv'
     else:
         str_stimulus = 'PWL ' + value
     formatted_text = name + ' ' + str_nodes + ' ' + str_stimulus
     return formatted_text
 
 
 def add_pulsed_source_component(name: str, nodes: list, value: str):
     ''' Format stimulus-controlled component netlist row '''
+    nodes = [str(x) for x in nodes]
     str_nodes = " ".join(nodes)  # string with space-separated nodes
     str_stimulus = 'PULSE ' + value
     formatted_text = name + ' ' + str_nodes + ' ' + str_stimulus
     return formatted_text
 
 def add_option(name: str, value: str):
     ''' Format option row '''
-    formatted_text = '+ ' + name + '=' + value
+    formatted_text = '+ ' + name + '=' + str(value)
     return formatted_text
 
 
 def add_transient_source_component(name: str, nodes: list, value: str):
     ''' Format controlled-source component netlist row '''
+    nodes = [str(x) for x in nodes]
     str_nodes = " ".join(nodes)  # string with space-separated nodes
     str_stimulus = 'AC ' + '{' + value + '}'
     formatted_text = name + ' ' + str_nodes + ' ' + str_stimulus
     return formatted_text
 
 
 def add_parametrized_component(name: str, nodes: list, value: str, parameters: dict):
     ''' Format parametrized component netlist row '''
+    nodes = [str(x) for x in nodes]
     str_nodes = " ".join(nodes)  # string with space-separated nodes
     formatted_component = name + ' ' + str_nodes + ' ' + value  # First row, which defines the component
     if parameters:
         formatted_component = formatted_component + '\n'
         formatted_parameters = '+ PARAMS:'  # First part of the string in the second row, which defines the component parameters
         for name_parameters, value_parameters in parameters.items():
             formatted_parameters = formatted_parameters + ' ' + name_parameters + '={' + value_parameters + '}'
@@ -880,14 +906,16 @@
 
     :param in_file_library: Name of the input library
     :param out_file_library: Path to the translated, output library
     :param verbose:
     :return:
     """
     output_path = str(Path(out_file_library).parent.absolute())
+    make_folder_if_not_existing(output_path, verbose=verbose)
+
     with open(in_file_library) as f:
         lines = f.readlines()
         flag_inModel = 0
         flag_inSubckt = 0
         idx_start = []
         idx_end = []
         for i in range(len(lines)):
@@ -922,15 +950,15 @@
     return
 
 
 def translate_model_PSPICE_2_XYCE(model: str, output_path: str = ''):
     """
     Function that converts a PSPICE model to a XYCE model
 
-    :param model: str, containing the whole model as a string, lines seperated by \n
+    :param model: str, containing the whole model as a string, lines separated by \n
     :rtype: str, the changed model as a str
     """
 
     model_split = model.split('\n')
 
     list_possible_components = ['r','l','c','x','k','d','p','o','s','w','v','i']
     list_possible_sources = ['v','i']
@@ -995,15 +1023,15 @@
                 value = line_split[-1]
                 line_split = [x+' ' for x in line_split]
 
 
             line = ''.join(line_split[:-1])
             line_split = line.split(' ')
             line_split_eff = line_split[:-1]
-            line_split_eff = [l.replace('(', '').replace(')', '') for l in line_split_eff if l]
+            line_split_eff = [l.replace('(', '').replace(')', '') if l and not '{' in l else l for l in line_split_eff]
             line_split[:-1] = line_split_eff
             line = ' '.join(line_split)+' '+value
             if line.startswith('E') and not 'TABLE' in line and 'VALUE' in line:
                 line = line + ' smoothbsrc=1'
         elif line.startswith('.model') or line.startswith('.MODEL') or flag_inModel:
             # In XYCE models, the parameters are not allowed to be seperated by commas
             flag_inModel = True
@@ -1021,15 +1049,15 @@
                 line = ''.join(line)
             line_split = line.replace('\t',' ').split(' ')
             if 'IC' in line_split[-1]:
                 idx_l = 3
             else:
                 idx_l = 1
             line_split_eff = line_split[:-idx_l]
-            line_split_eff = [l.replace('(','').replace(')','') for l in line_split_eff if l]
+            line_split_eff = [l.replace('(','').replace(')','') if l and not '{' in l else l for l in line_split_eff]
             line_split[:-idx_l] = line_split_eff
             line = ' '.join(line_split)
         model_split[i] = line
     model = '\n'.join(model_split)
     return model, flag_Added
 
 
@@ -1041,46 +1069,49 @@
     '''
     line_split = line.split('=')
     line_nodes = line_split[0].split(' ')
     line_nodes = [x.replace('(', '').replace(')', '') for x in line_nodes if x]
     in_line = ' '.join(line_nodes[:-1])
 
     if origin_stl:
-        origin_stl = origin_stl.replace(os.sep, '/')+'/'+'Stimulus'+'/'+line_split[-1][1:] + '.csv'
+        origin_stl = origin_stl.replace(os.sep, '/') + '/' + get_name_stimulus_folder() + '/' + line_split[-1][
+                                                                                                1:] + '.csv'
     else:
         origin_stl = line_split[-1][1:] + '.csv'
     new_stl_line = in_line + ' PWL FILE ' + origin_stl
     return new_stl_line
 
 
-def translate_stimulus(stl_name, stl_file: str, path_output: str = ''):
+def translate_stimulus(stl_name, input_file_path: str, output_path: str = ''):
     '''
-    Function that translates a single, list of stimuli or all stimuli in the file
+    Function that translates a single list of stimuli or all stimuli in the file
     (if stl_name is only a single string, if it's a list or if the keyword 'all' is provided)
     to an each independent .csv file, which can be used by PWL controlled XYCE sources
-    :param stl_name:
-    :param stl_file:
-    :param path_output:
+    :param stl_name: list of stimuli to process
+    :param input_file_path: name of the original stimulus file (usually this is a PSPICE-compatible file)
+    :param output_path: Full path to the folder where the converted XYCE-compatible csv files will be generated
     :return:
     '''
-    with open(stl_file, 'r') as f:
+    make_folder_if_not_existing(output_path, verbose=False)
+
+    # Read the original stimulus file (usually this is a PSPICE-compatible file)
+    with open(input_file_path, 'r') as f:
         lines = f.readlines()
 
     if stl_name=='all':
         stl_name = []
         for line in lines:
             if '.STIMULUS' in line:
                 line_split = line.split(' ')
                 stl_name.append(line_split[1])
 
     if isinstance(stl_name, str):
         stl_name = [stl_name]
 
-    for k in range(len(stl_name)):
-        stl = stl_name[k]
+    for stl in stl_name:
         time = []
         value = []
         flag_inStl = False
         for i in range(len(lines)):
             line = lines[i]
             if line.startswith(f'.STIMULUS {stl}') and not flag_inStl:
                 flag_inStl = True
@@ -1092,17 +1123,17 @@
                 value.append(float(line_split[1]))
             if (not line or line.startswith(f'.STIMULUS') or line=='\n') and (flag_inStl):
                 flag_inStl = False
                 break
 
         df_stl = pd.DataFrame.from_dict({'Time': time,'Value': value})
 
-        if path_output:
-            outputfile = os.path.join(path_output,stl+'.csv')
-        else:
-            outputfile =  os.path.join(os.getcwd(),stl+'.csv')
-        df_stl.to_csv(outputfile, header=False, index=False )
-        print(f'{outputfile} was translated.')
+        output_file_path = os.path.join(output_path, stl + '.csv')
+        df_stl.to_csv(output_file_path, header=False, index=False)
+        print(f'{output_file_path} was translated.')
     return
 
 
+def get_name_stimulus_folder():
+    return 'Stimulus'
+
 #######################  Helper functions - END  #######################
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/ParserYAML.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/ParserYAML.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,16 +168,16 @@
                     if value.alias:
                         currentDictionaryKey = value.alias
                     else:
                         currentDictionaryKey = currentPydanticKey
                 else:
                     currentDictionaryKey = currentPydanticKey
 
-                if value.field_info.description:
-                    description = value.field_info.description.replace("\n", " ")
+                if value.description:
+                    description = value.description.replace("\n", " ")
                     ruamel_yaml_object.yaml_add_eol_comment(
                         description,
                         currentDictionaryKey,
                     )
 
                 if hasattr(getattr(model, currentPydanticKey), "__fields__"):
                     new_ruamel_yaml_object = iterate_fields(
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/utils_ParserCircuits.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/utils_ParserCircuits.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsers/utils_ParserCosims.py` & `steam-sdk-2024.4.0/steam_sdk/parsers/utils_ParserCosims.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,88 +1,92 @@
 import os
-import shutil
 from pathlib import Path
 from typing import Union
 
 from steam_sdk.builders.BuilderModel import BuilderModel
 from steam_sdk.data.DataCoSim import NSTI
-from steam_sdk.data.DataModelCosim import DataModelCosim
+from steam_sdk.data.DataModelCosim import DataModelCosim, ParametersToModify
 from steam_sdk.data.DataModelCosim import sim_FiQuS, sim_LEDET, sim_PSPICE, sim_XYCE
 from steam_sdk.data.DataSettings import DataSettings
 from steam_sdk.utils.attribute_model import get_attribute_model, set_attribute_model
-from steam_sdk.utils.delete_if_existing import delete_if_existing
-from steam_sdk.utils.make_folder_if_not_existing import make_folder_if_not_existing
 from steam_sdk.utils.sgetattr import rsetattr
 
 
 def write_model_input_files(cosim_data: DataModelCosim,
-                            model_name: str,
                             model: Union[sim_FiQuS, sim_LEDET, sim_PSPICE, sim_XYCE],
                             cosim_software: str,
-                            local_cosim_folder: str,
                             data_settings: DataSettings,
+                            extra_variables_to_change: ParametersToModify = ParametersToModify(),
                             nsti: NSTI = None,
                             verbose: bool = False):
     '''
     Make all required input files for the selected model. Save them to the COSIM subfolder. Delete temporary files.
     This method does not depend on the software tool
     :param cosim_data TODO
-    :param model_name: Name of the model
     :param model: Object defining the model information
     :param cosim_software: Name of the software (supported: COSIM, PyCosim)
-    :param local_cosim_folder: Output co-simulation folder
     :param data_settings: DataSettings object containing all settings, previously read from user specific settings.SYSTEM.yaml file or from a STEAM analysis permanent settings
-    :param verbose: If True, display information while running
-    :param nsti:  N=Simulation number, S=Simulation set, T=Time window, I=Iteration
+    :param nsti: NSTI parameters. N=Simulation number, S=Simulation set, T=Time window, I=Iteration
     :type nsti: NSTI
+    :param extra_variables_to_change Additional parameters to change. These will be changed AFTER the parameter changes defined by model.variables_to_modify_pre_cosim, model.variables_to_modify_cosim, or model.variables_to_modify_post_cosim
+    :param verbose: If True, display information while running
     :return:
     '''
     # Unpack input
-    file_model_data = model.modelName
+    model_data_name = model.modelName
     case_model = model.modelCase
     software = model.type
     simulation_name = model.modelName
-    simulation_number = model.simulationNumber if hasattr(model, 'simulationNumber') else None  # PSPICE netlists don't have number
+    # simulation_number = model.simulationNumber if hasattr(model, 'simulationNumber') else None  # PSPICE netlists don't have number
     # TODO variables_to_change, variables_values should be defined based on a new argmetn 1,2,3... defining whether it's pre-cosim, cosim, or post-cosim
     if nsti.t == 0:  # Before the first time window
         variables_to_change = model.variables_to_modify_pre_cosim.variables_to_change
         variables_values = model.variables_to_modify_pre_cosim.variables_values
     elif nsti.t > len(cosim_data.Settings.Time_Windows.t_0):  # Final simulation after the last time window
         variables_to_change = model.variables_to_modify_post_cosim.variables_to_change
         variables_values = model.variables_to_modify_post_cosim.variables_values
+        # for variable in model.variables_to_modify_post_cosim.variables_to_change:
+            # if  flag...
+            #     variables_to_change = model.variables_to_modify_post_cosim.variables_to_change
+            #     variables_values = model.variables_to_modify_post_cosim.variables_values
     else:  # Co-simulation
         variables_to_change = model.variables_to_modify_cosim.variables_to_change
         variables_values = model.variables_to_modify_cosim.variables_values
+    # Add extra variables to change
+    variables_to_change = variables_to_change + extra_variables_to_change.variables_to_change
+    variables_values = variables_values + extra_variables_to_change.variables_values
     library_path = model.modelFolder  # TODO: maybe the following key should be deleted: cosim_data.Folders.path_model_folder
     cosim_name = cosim_data.GeneralParameters.cosim_name
     cosim_number = str(nsti.n)
 
     # Define folder paths
     if cosim_software == 'COSIM':
+        local_cosim_folder = data_settings.local_COSIM_folder
         if software == 'FiQuS':
             raise ValueError(f'FiQuS does not support COSIM. Please use PyCoSim instead')
         elif software == 'LEDET':
-            local_folder = os.path.join(local_cosim_folder, cosim_name, cosim_number, 'Input', model_name, 'LEDET')
+            local_folder = os.path.join(local_cosim_folder, cosim_name, cosim_number, 'Input', model.name, 'LEDET')
         elif software == 'PSPICE':
-            local_folder = os.path.join(local_cosim_folder, cosim_name, cosim_number, 'Input', model_name)
+            local_folder = os.path.join(local_cosim_folder, cosim_name, cosim_number, 'Input', model.name)
         if software == 'XYCE':
-            local_folder = os.path.join(local_cosim_folder, cosim_name, cosim_number, 'Input', model_name)
+            local_folder = os.path.join(local_cosim_folder, cosim_name, cosim_number, 'Input', model.name)
     elif cosim_software == 'PyCoSim':
+        local_cosim_folder = data_settings.local_PyCoSim_folder
         local_folder_prefix = os.path.join(local_cosim_folder, cosim_name, software)
         if software == 'FiQuS':
             local_folder = os.path.join(local_folder_prefix, model.modelName) # use model set in the input folder name
         elif software == 'LEDET':
             local_folder = os.path.join(local_folder_prefix, str(nsti.n))
         elif software in ['PSPICE', 'XYCE']:
             local_folder = os.path.join(local_folder_prefix, str(nsti.n))  #TODO double check
     else:
          raise Exception(f'Co-simulation software {cosim_software} not supported.')
 
     # Always assume the STEAM models folder structure, which contains subfolders "circuits", "conductors", "cosims", "magnets"
-    file_model_data = os.path.join(library_path, f'{case_model}s', file_model_data, 'input', f'modelData_{file_model_data}.yaml')
+    file_model_data = os.path.join(library_path, f'{case_model}s', model_data_name, 'input', f'modelData_{model_data_name}.yaml')
     # Make BuilderModel object
     BM = BuilderModel(file_model_data=file_model_data, case_model=case_model, data_settings=data_settings, verbose=verbose)
     # Edit BuilderModel object with the variable changes set in the input file
     if not len(variables_to_change) == len(variables_values):
         raise Exception(f'Variables variables_to_change and variables_values must have the same length.')
     for v, (variable_to_change, value) in enumerate(zip(variables_to_change, variables_values)):
         if verbose:
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsims/ParsimConductor.py` & `steam-sdk-2024.4.0/steam_sdk/parsims/ParsimConductor.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 from steammaterials.STEAM_materials import STEAM_materials
 
 from steam_sdk.data.DataAnalysis import StrandCriticalCurrentMeasurement
 from steam_sdk.data.DataConductor import Conductor
 from steam_sdk.data.DataModelMagnet import DataModelMagnet
 from steam_sdk.data.DataParsimConductor import ConductorSample
 from steam_sdk.data.DataParsimConductor import DataParsimConductor, IcMeasurement, Coil, StrandGeometry
-from steam_sdk.parsers.ParserMap2d import getParametersFromMap2d
+from steam_sdk.parsers.ParserMap2d import ParserMap2dFile
+from steam_sdk.utils.correct_RRR_NIST import correct_RRR_NIST
 from steam_sdk.utils.get_attribute_type import get_attribute_type
 from steam_sdk.utils.make_folder_if_not_existing import make_folder_if_not_existing
 from steam_sdk.utils.parse_str_to_list import parse_str_to_list
 from steam_sdk.utils.rhasattr import rhasattr
 from steam_sdk.utils.sgetattr import rsetattr, rgetattr
 
 
@@ -453,15 +454,15 @@
         :param conductor_sample: A ConductorSample object containing sample data for the conductor
         :param coil_name: The name of the coil
         :param original_conductor: The original conductor object, needed for getting parameters if they are not beeing changed, meaning not present in conductor_sample
         :param coil: The Coil object to get the RT resistance measurement values
         """
 
         # calculate correction factor strand twist-pitch with bare cable width and strand twist pitch
-        bare_cable_width = conductor_sample.width
+        bare_cable_width = conductor_sample.bare_cable_width
         if not bare_cable_width: bare_cable_width = original_conductor.cable.bare_cable_width
         if not bare_cable_width: raise Exception('Could not find bare cable width in conductor database and in original conductor.')
         if original_conductor.cable.type == 'Ribbon':
             f_twist_pitch = 1.0
         else:
             strand_twist_pitch = conductor_sample.strand_twist_pitch
             if not strand_twist_pitch: strand_twist_pitch = original_conductor.cable.strand_twist_pitch
@@ -483,46 +484,53 @@
         fCu = Cu_noCu / (1 + Cu_noCu)
         A_strand = calc_strand_area(conductor_sample.strand_geometry, original_conductor)
         n_strands = conductor_sample.number_of_strands
         if not n_strands: n_strands = original_conductor.cable.n_strands
         if not n_strands: Exception('Could not find number of strands in conductor database and in original conductor.')
         A_cond = A_strand * n_strands
 
-        # calculate rho with c function
+        # Calculate rho with C function
         temperature = coil.T_ref_coil_resistance
         if not temperature: temperature = 293.0
         mag_field = coil.B_resistance_meas
         if not mag_field: mag_field = 0.0
         RRR = conductor_sample.RRR
         if not RRR: RRR = original_conductor.strand.RRR
         if not RRR: raise Exception('Could not find RRR in conductor database and in original conductor.')
-        Tup_RRR = coil.T_ref_RRR_high
-        if not Tup_RRR: Tup_RRR = original_conductor.strand.T_ref_RRR_high
-        if not Tup_RRR: Tup_RRR = 293.0
-        rho_param = np.vstack((temperature, mag_field, RRR, Tup_RRR))  # create parameter v stack for c function
+        # Define temperatures at which the RRR is defined (if not assigned, assign default values)
+        T_ref_RRR_high = coil.T_ref_RRR_high
+        if not T_ref_RRR_high: T_ref_RRR_high = original_conductor.strand.T_ref_RRR_high
+        if not T_ref_RRR_high: T_ref_RRR_high = 293.0
+        T_ref_RRR_low = coil.T_ref_RRR_low
+        if not T_ref_RRR_low: T_ref_RRR_low = original_conductor.strand.T_ref_RRR_low
+        if not T_ref_RRR_low: T_ref_RRR_low = 4.0
+        # Find correction factor for the RRR to use in the NIST fit of copper electrical resistivity
+        f_correction_RRR, corrected_RRR = correct_RRR_NIST(RRR=RRR, T_ref_high=T_ref_RRR_high, T_ref_low=T_ref_RRR_low)
+        # Calculate copper electrical resistivity
+        rho_param = np.vstack((temperature, mag_field, corrected_RRR))  # create parameter v stack for c function
         CFUN_path = os.path.dirname(steammaterials.__file__)  # get path to steam materials library
-        CFUN_rhoCuNIST = STEAM_materials('CFUN_rhoCu_v1', rho_param.shape[0], rho_param.shape[1], CFUN_path)
+        CFUN_rhoCuNIST = STEAM_materials('CFUN_rhoCu_NIST_v1', rho_param.shape[0], rho_param.shape[1], CFUN_path)
         rho = CFUN_rhoCuNIST.evaluate(rho_param)[0]  # evaluate rho function with the parameters
 
-        # calculate the length
+        # calculate the coil length to match the measured room-temperature resistance, and divided it by the number of half-turns
         L = R_RT * fCu * A_cond / (rho * f_twist_pitch)
         L_ht = L / number_of_ht
         return L_ht
 
     def __read_num_ht_per_group(self):
         """
         Reads the number of half-turns per group either from the map2d file or from the model_data's CoilWindings attribute.
         If neither is available, raises an exception.
 
         :return: A list containing the number of half-turns for each group.
         """
         if self.model_data.Sources.magnetic_field_fromROXIE:
             path_map2d = Path(self.path_input_dir, self.model_data.Sources.magnetic_field_fromROXIE).resolve()
             # number_of_ht has as many elements as groups. Each element defines the number of half-turns in that group
-            number_of_hts, _, _, _, _, _, _, _ = getParametersFromMap2d(map2dFile=path_map2d)  # TODO number_of_hts is block number for HOC magnets
+            number_of_hts, _, _, _, _, _, _, _, _, _ = ParserMap2dFile(map2dFile=path_map2d).getParametersFromMap2d()  # TODO number_of_hts is block number for HOC magnets
             if len(number_of_hts) != self.number_of_groups: raise Exception(f'The number of groups given to ParsimConductor ({self.number_of_groups}) is different then the number of groups specified in the map2d file "{path_map2d}" ({len(number_of_hts)})')
         else:
             number_of_hts = self.model_data.CoilWindings.n_half_turn_in_group
             if not number_of_hts: raise Exception('Number of half turns per group could not be specified. CoilWindings.n_half_turn_in_group is empty in modelData.')
             if len(number_of_hts) != self.number_of_groups: raise Exception('The number of groups given to ParsimConductor is different then the length of CoilWindings.n_half_turn_in_group in modelData.')
         return number_of_hts
 
@@ -534,45 +542,43 @@
         :param dict_sweeper: The input dictionary where the sweeper entries will be stored in the format {attributeNameDataModelMagnet: newValue}.
         :param flag_optimize_fCu: If set to True, fCu will be optimized with the coil resistance measurement at room temperature.
         :param rel_warning_limit: function raises warning in console when values are changed for more/less then this relative value
         """
         # parameter dict for creating the column names of sweeper csv file
         dict_param = {
             # format {attribute_name_of_ConductorSample_object: attribute_name_of_Conductor_from_DataModelMagnet_object}
+            'bare_cable_width': 'cable.bare_cable_width',
+            'bare_cable_height': 'cable.bare_cable_height',
+            'number_of_strands': 'cable.n_strands',
+            'strand_twist_pitch': 'cable.strand_twist_pitch',
+            'Ra': 'cable.Ra',
+            'Rc': 'cable.Rc',
             'strand_geometry.diameter': 'strand.diameter',
             'strand_geometry.bare_width': 'strand.bare_width',
             'strand_geometry.bare_height': 'strand.bare_height',
-            'width': 'cable.width_core',  # TODO: is this correct? or bare_cable_width?
-            'height': 'cable.height_core',  # TODO: is this correct?
-            'f_rho_eff': 'strand.f_Rho_effective',
-            'Ra': 'cable.Ra',
-            'Rc': 'cable.Rc',
+            'Cu_noCu': 'strand.Cu_noCu_in_strand',
             'RRR': 'strand.RRR',
+            'f_rho_eff': 'strand.f_Rho_effective',
+            'filament_twist_pitch': 'strand.fil_twist_pitch',
             'Bc20': 'Jc_fit.Tc0_CUDI1',
             'Tc0': 'Jc_fit.Bc20_CUDI1',
-            'number_of_strands': 'cable.n_strands',
-            'Cu_noCu': 'strand.Cu_noCu_in_strand',
-            'width': 'cable.bare_cable_width',
-            'filament_twist_pitch': 'strand.fil_twist_pitch',
-            'strand_twist_pitch': 'cable.strand_twist_pitch',
         }
 
         # looping through the coil list
         for coil_name, coil in self.data_parsim_conductor.Coils.items():
             idx = self.dict_coilName_to_conductorIndex[coil_name]
             sweeper_cond_name = f'Conductors[{idx}].'
 
             # parse data from DataParsimConductor to strings for sweeper csv and store them in dict_sweeper
             for sample_attribute_name, conductor_attribute_name in dict_param.items():
                 val = getattr_from_list(coil.conductorSamples, sample_attribute_name, coil.weight_factors)
                 if val:
                     # check if the original conductor has the attribute that will be changed to avoid errors when running parsim sweeper
                     if not rhasattr(self.model_data.Conductors[idx], conductor_attribute_name):
-                        raise Exception(
-                            f'Tried to change conductor attribute "{conductor_attribute_name}" that is not specified for the conductor of coil {coil_name}.')
+                        raise Exception(f'Tried to change conductor attribute "{conductor_attribute_name}" that is not specified for the conductor of coil {coil_name}.')
                     # append value to sweeper dict
                     dict_sweeper[sweeper_cond_name + conductor_attribute_name] = val
 
             # insert Jc fit value(s) depending on their fitting function (usual Bottura, CUDI1, CUDI3 for NbTi and Summers, Bordini for Nb3Sn)
             Jc_dict_list = []
             for conductor_sample in coil.conductorSamples:
                 # calculate the parameters for Jc fit for every conductor sample of this coil
@@ -595,17 +601,17 @@
                 # check if RT measurement is defined
                 if not coil.coil_resistance_room_T:
                     warnings.warn(f'No room temperature resistance measurement for coil "{coil_name}" was found in database. Not optimizing fraction of copper.')
                     continue
                 # calculate Cu_noCu for every conductor sample and use mean value
                 list_optimized_Cu_noCu = []
                 for sample in coil.conductorSamples:
-                    list_optimized_Cu_noCu.append(
-                        self.__calculate_fCu_with_resistance_meas(sample, coil_name, self.model_data.Conductors[idx],
-                                                                  coil))
+                    list_optimized_Cu_noCu.append(self.__calculate_fCu_with_resistance_meas(sample, coil_name,
+                                                                                            self.model_data.Conductors[
+                                                                                                idx], coil))
                 # if the Cu no Cu ratio could be parsed directly from a column, overwrite it with optimized value
                 dict_sweeper[sweeper_cond_name + 'strand.Cu_noCu_in_strand'] = np.mean(list_optimized_Cu_noCu)
 
     def __calculate_fCu_with_resistance_meas(self, conductor_sample: ConductorSample, coil_name: str,
                                              original_conductor: Conductor, coil: Coil):
         """
         Optimizes the fraction of copper (fCu) using the room temperature resistance measurements using the formula:
@@ -614,15 +620,15 @@
         :param conductor_sample: A ConductorSample object containing sample data for the conductor
         :param coil_name: The name of the coil
         :param original_conductor: The original conductor object, needed for getting parameters if they are not being changed, meaning not present in conductor_sample
         :param coil: The Coil object to get the RT resistance measurement values
         """
 
         # calculate correction factor strand twist-pitch with bare cable width and strand twist pitch
-        bare_cable_width = conductor_sample.width
+        bare_cable_width = conductor_sample.bare_cable_width
         if not bare_cable_width: bare_cable_width = original_conductor.cable.bare_cable_width
         if not bare_cable_width: raise Exception('Could not find bare cable width in conductor database and in original conductor.')
         if original_conductor.cable.type == 'Ribbon':
             f_twist_pitch = 1.0
         else:
             strand_twist_pitch = conductor_sample.strand_twist_pitch
             if not strand_twist_pitch: strand_twist_pitch = original_conductor.cable.strand_twist_pitch
@@ -635,28 +641,35 @@
         if not R_RT: raise Exception(f'No room temperature measurement provided for coil {coil_name}')
         A_strand = calc_strand_area(conductor_sample.strand_geometry, original_conductor)
         n_strands = conductor_sample.number_of_strands
         if not n_strands: n_strands = original_conductor.cable.n_strands
         if not n_strands: raise Exception('Could not find number of strands in conductor database and in original conductor.')
         A_cond = A_strand * n_strands
 
-        # calculate rho with c function
+        # Calculate rho with C function
         temperature = coil.T_ref_coil_resistance
         if not temperature: temperature = 293.0
         mag_field = coil.B_resistance_meas
         if not mag_field: mag_field = 0.0
         RRR = conductor_sample.RRR
         if not RRR: RRR = original_conductor.strand.RRR
         if not RRR: raise Exception('Could not find RRR in conductor database and in original conductor.')
-        Tup_RRR = coil.T_ref_RRR_high
-        if not Tup_RRR: Tup_RRR = original_conductor.strand.T_ref_RRR_high
-        if not Tup_RRR: Tup_RRR = 293.0
-        rho_param = np.vstack((temperature, mag_field, RRR, Tup_RRR))  # create parameter v stack for c function
+        # Define temperatures at which the RRR is defined (if not assigned, assign default values)
+        T_ref_RRR_high = coil.T_ref_RRR_high
+        if not T_ref_RRR_high: T_ref_RRR_high = original_conductor.strand.T_ref_RRR_high
+        if not T_ref_RRR_high: T_ref_RRR_high = 293.0
+        T_ref_RRR_low = coil.T_ref_RRR_low
+        if not T_ref_RRR_low: T_ref_RRR_low = original_conductor.strand.T_ref_RRR_low
+        if not T_ref_RRR_low: T_ref_RRR_low = 4.0
+        # Find correction factor for the RRR to use in the NIST fit of copper electrical resistivity
+        f_correction_RRR, corrected_RRR = correct_RRR_NIST(RRR=RRR, T_ref_high=T_ref_RRR_high, T_ref_low=T_ref_RRR_low)
+        # Calculate copper electrical resistivity
+        rho_param = np.vstack((temperature, mag_field, corrected_RRR))  # create parameter v stack for c function
         CFUN_path = os.path.dirname(steammaterials.__file__)  # get path to steam materials library
-        CFUN_rhoCuNIST = STEAM_materials('CFUN_rhoCu_v1', rho_param.shape[0], rho_param.shape[1], CFUN_path)
+        CFUN_rhoCuNIST = STEAM_materials('CFUN_rhoCu_NIST_v1', rho_param.shape[0], rho_param.shape[1], CFUN_path)
         rho = CFUN_rhoCuNIST.evaluate(rho_param)[0]  # evaluate rho function with the parameters
 
         # calculte fCu
         fCu = L_coil * rho * f_twist_pitch / (R_RT * A_cond)
         Cu_noCu_new = fCu / (1 - fCu)
 
         # compare new value with old one
@@ -911,15 +924,15 @@
         else:
             diameter = strand_geometry.diameter
 
         # calculate area of circle
         A = np.pi * diameter ** 2 / 4
     elif original_conductor.strand.type == 'Rectangular':
 
-        # if height/width is not changed in conductor database, use the one form modeldata
+        # if height/width is not changed in conductor database, use the one from modeldata
         if not strand_geometry.bare_height:
             h = original_conductor.strand.bare_height
         else:
             h = strand_geometry.bare_height
         if not strand_geometry.bare_width:
             w = original_conductor.strand.bare_width
         else:
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsims/ParsimEventCircuit.py` & `steam-sdk-2024.4.0/steam_sdk/parsims/ParsimEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsims/ParsimEventMagnet.py` & `steam-sdk-2024.4.0/steam_sdk/parsims/ParsimEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml` & `steam-sdk-2024.4.0/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     - bare strand height [m]
     - bare strand height [mm]
     - strand height
     - strand height [m]
     - strand height [mm]
     - Bare strand height [m]
     - Strand height [mm]
-  width:
+  bare_cable_width:
     - width [m]
     - width [mm]
     - width
     - Width
     - Width [m]
     - Width [mm]
   strand_twist_pitch:
@@ -80,15 +80,15 @@
     - RRR
     - Estimated coil RRR
   Cu_noCu:
     - Ave Cu/noCu
     - Copper to non-Copper ratio
     - Cu/noCu
     - Cu_noCu
-  height:
+  bare_cable_height:
     - Height [m]
     - Height [mm]
     - Height
 Coil:
   coil_resistance_room_T:
     - RT coil resistance [Ohm]
   Cu_noCu_resistance_meas:
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/parsims/translation_dicts/event_column_names.yaml` & `steam-sdk-2024.4.0/steam_sdk/parsims/translation_dicts/event_column_names.yaml`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/plotters/PlotterAnalysis.py` & `steam-sdk-2024.4.0/steam_sdk/plotters/PlotterAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/plotters/PlotterMap2d.py` & `steam-sdk-2024.4.0/steam_sdk/plotters/PlotterMap2d.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,473 +1,420 @@
 import os
-
+from pathlib import Path
 import matplotlib.lines as lines
 import matplotlib.patches as patches
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
-from matplotlib.colors import LogNorm
-import matplotlib.cm as cm
-#from steam_sdk.plotters.PlotterRoxie import plotEdges
-from steam_sdk.utils.misc import displayWaitAndClose
 
-def export_B_field_txt_to_map2d_SIGMA(path_map2d_roxie, path_result_txt_Bx, path_result_txt_By, path_new_file):
-    """
-    Copy content of reference map2d file and overwrites Bx and By values which are replaced values from
-    comsol output txt file and writes to a new map2d file.
-    :param path_map2d: Path to reference map2d from which all values apart from Bx and By is copied from
-    :param path_result: Comsol output txt file with evaluated B-field
-    :param path_new_file: Path to new map2d file where new B-field is stored
-    :return:
-    """
-    df_reference = pd.read_csv(path_map2d_roxie, delim_whitespace=True)
-    with open(path_result_txt_Bx) as file:  # opens a text file
-        lines = [line.strip().split() for line in file if not "%" in line]  # loops over each line
-
-    df_txt_Bx = pd.DataFrame(lines, columns=["x", "y", "Bx"])
-
-    df_txt_Bx = df_txt_Bx.apply(pd.to_numeric)
-
-    with open(path_result_txt_By) as file:  # opens a text file
-        lines = [line.strip().split() for line in file if not "%" in line]  # loops over each line
-
-    df_txt_By = pd.DataFrame(lines, columns=["x", "y", "By"])
-    df_txt_By = df_txt_By.apply(pd.to_numeric)
-
-    # Verify all evaluate field at same coordinates!
-
-    x_tol, y_tol = 1e-10, 1e-10
-    x_ref, y_ref = df_reference['X-POS/MM'] / 1000, df_reference['Y-POS/MM'] / 1000
-
-    if ((x_ref - df_txt_Bx['x']).abs().max() < x_tol) and \
-            ((x_ref - df_txt_By['x']).abs().max() < x_tol) and \
-            ((y_ref - df_txt_Bx['y']).abs().max() < y_tol) and \
-            ((y_ref - df_txt_By['y']).abs().max() < y_tol):
-        print("All dataframes have the same x and y coordinates.")
-    else:
-        raise ValueError("Error: Not all dataframes have the same x and y coordinates. Can't compare map2ds!")
-
-    # Create new map2d
-    with open(path_new_file, 'w') as file:
-        file.write("  BL.   COND.    NO.    X-POS/MM     Y-POS/MM    BX/T       BY/T"
-                   "      AREA/MM**2 CURRENT FILL FAC.\n\n")
-        content = []
-        for index, row in df_reference.iterrows():
-            bl, cond, no, x, y, Bx, By, area, curr, fill, fac = row
-            bl = int(bl)
-            cond = int(cond)
-            no = int(no)
-            x = f"{x:.4f}"
-            y = f"{y:.4f}"
-            Bx = df_txt_Bx["Bx"].iloc[index]
-            Bx = f"{Bx:.4f}"
-            By = df_txt_By["By"].iloc[index]
-            By = f"{By:.4f}"
-            area = f"{area:.4f}"
-            curr = f"{curr:.2f}"
-            fill = f"{fill:.4f}"
-            content.append(
-                "{0:>6}{1:>6}{2:>7}{3:>13}{4:>13}{5:>11}{6:>11}{7:>11}{8:>9}{9:>8}\n".format(bl, cond, no, x, y, Bx,
-                                                                                             By,
-                                                                                             area, curr, fill))
-        file.writelines(content)
-
-def plot_multiple_areas(ax, areas, color=None):
-    """
-    Functions takes in a list of area objects and plot them on axis ax.
-    :param ax: Axis to create plots.
-    :param areas: list of SIGMA area objects.
-    :param color: Color of the object
-    :return:
-    """
-    for area in areas:
-        if color:
-            plot_area(ax, area, color)
-        else:
-            plot_area(ax, area)
 
-def plot_area(ax, area, color=None):
+class PlotterMap2d:
     """
-    Plots one SIGMA area object on axis ax
-    :param ax: Axis to create plots.
-    :param area: SIGMA area object.
-    :param color: Color of the object
-    :return:
+    Class for plotting map2d data
     """
-    if not color:
-        color = 'black'
-    points = []
-    hls = area.getHyperLines()
-    for hl in hls:
-        last_dot_index = hl.toString().rfind('.')
-        at_index = hl.toString().find('@')
-        class_name = hl.toString()[last_dot_index + 1:at_index]
-        if class_name == 'Line':
-            points.append([hl.getKp1().getX(), hl.getKp1().getY()])
-            points.append([hl.getKp2().getX(), hl.getKp2().getY()])
-        elif class_name == 'Arc':
-            start_angle = np.arctan2(hl.getKp1().getY() - hl.getKpc().getY(),
-                                     hl.getKp1().getX() - hl.getKpc().getX()) * 180 / np.pi
-            end_angle = start_angle + hl.getDTheta() * 180 / np.pi
-            r = np.sqrt((hl.getKp1().getY() - hl.getKpc().getY()) ** 2 + (hl.getKp1().getX() - hl.getKpc().getX()) ** 2)
-            ax.add_patch(patches.Arc([hl.getKpc().getX(), hl.getKpc().getY()], 2 * r, 2 * r, 0,
-                                     min(start_angle, end_angle), max(start_angle, end_angle), color=color))
-        elif class_name == 'Circumference':
-            r = hl.getRadius()
-            ax.add_patch(patches.Arc([hl.getCenter().getX(), hl.getCenter().getY()], 2 * r, 2 * r, 0, 0, 360))
-        else:
-            raise ValueError('Not supported Hyperline object!')
-
-    ax.add_line(lines.Line2D([points[0][0], points[3][0]], [points[0][1], points[3][1]], color=color))
-    ax.add_line(lines.Line2D([points[1][0], points[2][0]], [points[1][1], points[2][1]], color=color))
-
-def write_result_summary(df, n1, n2):
-    with open("error_summary.txt", "a") as myfile:
-        mean_Bmod_error = (df["Bmod_error"]).mean() * 1000
-        abs_mean_Bmod_error = abs(df["Bmod_error"]).mean() * 1000
-        std_Bmod_error = (df["Bmod_error"]).std() * 1000
-        max_Bmod_error = abs(df["Bmod_error"]).max() * 1000
-        min_Bmod_error = abs(df["Bmod_error"]).min() * 1000
-        myfile.write(f"{n1*n2} {mean_Bmod_error} {std_Bmod_error} {abs_mean_Bmod_error} {max_Bmod_error} {min_Bmod_error}\n")
-        max_index = abs(df["Bmod_error"]).idxmax()
-        print(f"Absolute Bmod error mean: {abs_mean_Bmod_error}")
-
-        print(f"Absolute Bmod error mean max index : {max_index}")
-
-def plot_Bmod(df, map2d_name1, map2d_name2, fig, ax, type, cmap='plasma'):
-    fig.suptitle(f"Bmod: {map2d_name1} and {map2d_name2} (mT)")
-    ax[0, 0].set_title(f"Bmod: {map2d_name1} (mT)")
-    ax[0, 0].set_xlabel('x-coordinate/mm')
-    ax[0, 0].set_ylabel('y-coordinate/mm')
-    ax[0, 1].set_title(f"Bmod: {map2d_name2} (mT)")
-    ax[0, 1].set_xlabel('x-coordinate/mm')
-    ax[0, 1].set_ylabel('y-coordinate/mm')
-    ax[1, 0].plot(df["Bmod1"] * 1000, '.')
-    ax[1, 0].set_title(f"Bmod scatter: {map2d_name1} (mT)")
-    ax[1, 0].set_xlabel('Strand number')
-    ax[1, 0].set_ylabel(f'Bmod scatter: {map2d_name1} (mT)')
-    ax[1, 1].plot(df["Bmod2"] * 1000, '.')
-    ax[1, 1].set_xlabel('Strand number')
-    ax[1, 1].set_ylabel('Scatter Bmod (mT)')
-    ax[1, 1].set_title(f"Bmod scatter: {map2d_name2} (mT)")
-    ax[0, 0].set_aspect("equal")
-    ax[0, 1].set_aspect("equal")
-    if(type=="coil"):
-        f11 = ax[0, 0].scatter(df["x"], df['y'], c=df["Bmod1"] * 1000, cmap=cmap)
-        f12 = ax[0, 1].scatter(df["x"], df['y'], c=df["Bmod2"] * 1000, cmap=cmap)
-        fig.colorbar(f11, ax=ax[0, 0])
-        fig.colorbar(f12, ax=ax[0, 1])
-    elif(type=="mesh"):
-        x = np.array(df['x'].tolist())
-        y = np.array(df['y'].tolist())
-        z1 = np.array(df['Bmod1'].tolist())*1000
-        z2 = np.array(df['Bmod2'].tolist())*1000
-        np.random.seed(1234)  # fix seed for reproducibility
-
-        tpc1 = ax[0, 0].tripcolor(x, y, z1, shading='gouraud', cmap=cmap)
-        tpc2 = ax[0, 1].tripcolor(x, y, z2, shading='gouraud', cmap=cmap)
-
-        fig.colorbar(tpc1)
-        fig.colorbar(tpc2)
-
-
-
-def plot_B_mod_error(df, map2d_name1, map2d_name2, fig, ax, type, cmap='winter'):
-    fig.suptitle(f"Bmod error: {map2d_name1} - {map2d_name2} (mT)")
-    ax[0].set_title(f"Bmod error (mT)")
-    ax[0].set_xlabel('x-coordinate/mm', fontsize=9)
-    ax[0].set_ylabel('y-coordinate/mm', fontsize=9)
-    ax[0].set_aspect("equal")
-    ax[1].set_title(f"Bmod error scatter (mT)")
-
-    ax[1].set_xlabel('x')
-    ax[1].set_ylabel('y')
-    ax[1].plot(df["Bmod_error"] * 1000, '.')
-    if(type=="coil"):
-        f11 = ax[0].scatter(df["x"], df['y'], c=df["Bmod_error"] * 1000, cmap=cmap)
-        fig.colorbar(f11, ax=ax[0])
-    elif(type=="mesh"):
-        x = np.array(df['x'].tolist())
-        y = np.array(df['y'].tolist())
-        z1 = np.array(df['Bmod_error'].tolist())*1000
-
-        np.random.seed(1234)  # fix seed for reproducibility
-
-        tpc = ax[0].tripcolor(x, y, z1, shading='gouraud', cmap=cmap)
-        fig.colorbar(tpc)
-
-
-def plot_relative_error_x_y(df, map2d_name1, map2d_name2, fig, ax, type, cmap='CMRmap'):
-    if df['rel_err_x'] is not None and df['rel_err_y'] is not None:
-        fig.suptitle(f"Relative error: {map2d_name1} and {map2d_name2} (T)")
-        ax[0, 0].set_aspect("equal")
-        ax[0, 1].set_aspect("equal")
 
-        ax[0, 0].set_title(f"Relative error Bx %")
+    def __init__(
+            self,
+            parsed_results_path: Path,
+            verbose: bool = True
+    ):
+        """
+        :param parsed_results_path: full path to Analysis PostProcess output folder
+        """
+        self.parsed_results_path = parsed_results_path
+
+    def plot_multiple_areas(self, ax, areas, color=None):
+        """
+        Functions takes in a list of area objects and plot them on axis ax.
+        :param ax: Axis to create plots.
+        :param areas: list of SIGMA area objects.
+        :param color: Color of the object
+        :return:
+        """
+        for area in areas:
+            if color:
+                self.plot_area(ax, area, color)
+            else:
+                self.plot_area(ax, area)
+
+    def plot_area(self, ax, area, color=None):
+        """
+        Plots one SIGMA area object on axis ax
+        :param ax: Axis to create plots.
+        :param area: SIGMA area object.
+        :param color: Color of the object
+        :return:
+        """
+        if not color:
+            color = 'black'
+        points = []
+        hls = area.getHyperLines()
+        for hl in hls:
+            last_dot_index = hl.toString().rfind('.')
+            at_index = hl.toString().find('@')
+            class_name = hl.toString()[last_dot_index + 1:at_index]
+            if class_name == 'Line':
+                points.append([hl.getKp1().getX(), hl.getKp1().getY()])
+                points.append([hl.getKp2().getX(), hl.getKp2().getY()])
+            elif class_name == 'Arc':
+                start_angle = np.arctan2(hl.getKp1().getY() - hl.getKpc().getY(),
+                                         hl.getKp1().getX() - hl.getKpc().getX()) * 180 / np.pi
+                end_angle = start_angle + hl.getDTheta() * 180 / np.pi
+                r = np.sqrt((hl.getKp1().getY() - hl.getKpc().getY()) ** 2 + (hl.getKp1().getX() - hl.getKpc().getX()) ** 2)
+                ax.add_patch(patches.Arc([hl.getKpc().getX(), hl.getKpc().getY()], 2 * r, 2 * r, 0,
+                                         min(start_angle, end_angle), max(start_angle, end_angle), color=color))
+            elif class_name == 'Circumference':
+                r = hl.getRadius()
+                ax.add_patch(patches.Arc([hl.getCenter().getX(), hl.getCenter().getY()], 2 * r, 2 * r, 0, 0, 360))
+            else:
+                raise ValueError('Not supported Hyperline object!')
+
+        ax.add_line(lines.Line2D([points[0][0], points[3][0]], [points[0][1], points[3][1]], color=color))
+        ax.add_line(lines.Line2D([points[1][0], points[2][0]], [points[1][1], points[2][1]], color=color))
+
+    def write_result_summary(self, df, n1, n2):
+        with open("error_summary.txt", "a") as myfile:
+            mean_Bmod_error = (df["Bmod_error"]).mean() * 1000
+            abs_mean_Bmod_error = abs(df["Bmod_error"]).mean() * 1000
+            std_Bmod_error = (df["Bmod_error"]).std() * 1000
+            max_Bmod_error = abs(df["Bmod_error"]).max() * 1000
+            min_Bmod_error = abs(df["Bmod_error"]).min() * 1000
+            myfile.write(
+                f"{n1 * n2} {mean_Bmod_error} {std_Bmod_error} {abs_mean_Bmod_error} {max_Bmod_error} {min_Bmod_error}\n")
+            max_index = abs(df["Bmod_error"]).idxmax()
+            print(f"Absolute Bmod error mean: {abs_mean_Bmod_error}")
+
+            print(f"Absolute Bmod error mean max index : {max_index}")
+
+    def plot_Bmod(self, df, map2d_name1, map2d_name2, fig, ax, type, cmap='plasma'):
+        fig.suptitle(f"Bmod: {map2d_name1} and {map2d_name2} (mT)")
+        ax[0, 0].set_title(f"Bmod: {map2d_name1} (mT)")
         ax[0, 0].set_xlabel('x-coordinate/mm')
         ax[0, 0].set_ylabel('y-coordinate/mm')
-        ax[0, 1].set_title(f"Relative error By %")
+        ax[0, 1].set_title(f"Bmod: {map2d_name2} (mT)")
         ax[0, 1].set_xlabel('x-coordinate/mm')
         ax[0, 1].set_ylabel('y-coordinate/mm')
-
-        ax[1, 0].plot(df["rel_err_x"] * 100, '.')
-        ax[1, 0].set_title(f"Scatter Relative error  Bx %")
+        ax[1, 0].plot(df["Bmod1"] * 1000, '.')
+        ax[1, 0].set_title(f"Bmod scatter: {map2d_name1} (mT)")
         ax[1, 0].set_xlabel('Strand number')
-        ax[1, 0].set_ylabel('Relative error Bx %')
-        ax[1, 1].plot(df["rel_err_y"] * 100, '.')
+        ax[1, 0].set_ylabel(f'Bmod scatter: {map2d_name1} (mT)')
+        ax[1, 1].plot(df["Bmod2"] * 1000, '.')
         ax[1, 1].set_xlabel('Strand number')
-        ax[1, 1].set_ylabel('Relative error By %')
-        ax[1, 1].set_title(f"Scatter Relative error  By %")
-        if(type=="coil"):
-            f31 = ax[0, 0].scatter(df["x"], df['y'], c=df["rel_err_x"] * 100, cmap=cmap)
-            f32 = ax[0, 1].scatter(df["x"], df['y'], c=df["rel_err_y"] * 100, cmap=cmap)
-            fig.colorbar(f31, ax=ax[0, 0])
-            fig.colorbar(f32, ax=ax[0, 1])
-        elif(type=="mesh"):
+        ax[1, 1].set_ylabel('Scatter Bmod (mT)')
+        ax[1, 1].set_title(f"Bmod scatter: {map2d_name2} (mT)")
+        ax[0, 0].set_aspect("equal")
+        ax[0, 1].set_aspect("equal")
+        if type == "coil":
+            f11 = ax[0, 0].scatter(df["x"], df['y'], c=df["Bmod1"] * 1000, cmap=cmap)
+            f12 = ax[0, 1].scatter(df["x"], df['y'], c=df["Bmod2"] * 1000, cmap=cmap)
+            fig.colorbar(f11, ax=ax[0, 0])
+            fig.colorbar(f12, ax=ax[0, 1])
+        elif type == "mesh":
             x = np.array(df['x'].tolist())
             y = np.array(df['y'].tolist())
-            z1 = np.array(df['rel_err_x'].tolist())*100
-            z2 = np.array(df['rel_err_y'].tolist())*100
+            z1 = np.array(df['Bmod1'].tolist()) * 1000
+            z2 = np.array(df['Bmod2'].tolist()) * 1000
             np.random.seed(1234)  # fix seed for reproducibility
 
             tpc1 = ax[0, 0].tripcolor(x, y, z1, shading='gouraud', cmap=cmap)
             tpc2 = ax[0, 1].tripcolor(x, y, z2, shading='gouraud', cmap=cmap)
 
             fig.colorbar(tpc1)
             fig.colorbar(tpc2)
 
+    def plot_B_mod_error(self, df, map2d_name1, map2d_name2, fig, ax, type, cmap='winter'):
+        fig.suptitle(f"Bmod error: {map2d_name1} - {map2d_name2} (mT)")
+        ax[0].set_title(f"Bmod error (mT)")
+        ax[0].set_xlabel('x-coordinate/mm', fontsize=9)
+        ax[0].set_ylabel('y-coordinate/mm', fontsize=9)
+        ax[0].set_aspect("equal")
+        ax[1].set_title(f"Bmod error scatter (mT)")
+
+        ax[1].set_xlabel('x')
+        ax[1].set_ylabel('y')
+        ax[1].plot(df["Bmod_error"] * 1000, '.')
+        if type == "coil":
+            f11 = ax[0].scatter(df["x"], df['y'], c=df["Bmod_error"] * 1000, cmap=cmap)
+            fig.colorbar(f11, ax=ax[0])
+        elif type == "mesh":
+            x = np.array(df['x'].tolist())
+            y = np.array(df['y'].tolist())
+            z1 = np.array(df['Bmod_error'].tolist()) * 1000
 
-def plot_Bx_By(df, map2d_name1, map2d_name2, fig, ax, type, cmap='seismic', plot_coil=False):
-    fig.suptitle(f"Bx and By field: {map2d_name1} and {map2d_name2} (mT)", fontsize=12)
+            np.random.seed(1234)  # fix seed for reproducibility
 
-    ax[0, 0].set_title(f"Bx {map2d_name1} (mT)", fontsize=10)
-    ax[0, 0].set_ylabel('y-coordinate/mm', fontsize=9)
-    ax[0, 0].set_aspect("equal")
-    ax[0, 1].set_aspect("equal")
-    ax[1, 0].set_aspect("equal")
-    ax[1, 1].set_aspect("equal")
-    ax[0, 1].set_title(f"By {map2d_name1} (mT)", fontsize=10)
-    ax[0, 1].set_ylabel('y-coordinate/mm', fontsize=9)
-
-    ax[1, 0].set_title(f"Bx {map2d_name2} (mT)", fontsize=10)
-    ax[1, 0].set_xlabel('x-coordinate/mm', fontsize=9)
-    ax[1, 0].set_ylabel('y-coordinate/mm', fontsize=9)
-    ax[1, 1].set_title(f"By {map2d_name2} (mT)", fontsize=10)
-    ax[1, 1].set_xlabel('x-coordinate/mm', fontsize=9)
-    ax[1, 1].set_ylabel('y-coordinate/mm', fontsize=9)
-    ax[2, 0].set_title(f"Bx scatter (mT)", fontsize=14, loc='left')
-    ax[2, 0].set_ylabel('Bx scatter (mT)', fontsize=9)
-    ax[2, 0].plot(df["Bx1"] * 1000, '.', color='b', label=f"{map2d_name1}")
-    ax[2, 0].plot(df["Bx2"] * 1000, '.', color='r', label=f"{map2d_name2}")
-    ax[2, 1].set_title(f"By scatter (mT)", fontsize=14, loc='left')
-    ax[2, 1].set_ylabel('By scatter (mT)', fontsize=9)
-
-    ax[2, 1].plot(df["By1"] * 1000, '.', color='b', label=f"{map2d_name1}")
-    ax[2, 1].plot(df["By2"] * 1000, '.', color='r', label=f"{map2d_name2}")
-    ax[2, 0].legend()
-    ax[2, 1].legend()
-
-    if(type == "coil"):
-        f41 = ax[0, 0].scatter(df["x"], df['y'], c=df["Bx1"] * 1000, cmap=cmap)
-        f42 = ax[0, 1].scatter(df["x"], df['y'], c=df["By1"] * 1000, cmap=cmap)
-        f43 = ax[1, 0].scatter(df["x"], df['y'], c=df["Bx2"] * 1000, cmap=cmap)
-        f44 = ax[1, 1].scatter(df["x"], df['y'], c=df["By2"] * 1000, cmap=cmap)
-        fig.colorbar(f41, ax=ax[0, 0])
-        fig.colorbar(f42, ax=ax[0, 1])
-        fig.colorbar(f43, ax=ax[1, 0])
-        fig.colorbar(f44, ax=ax[1, 1])
-    elif(type=="mesh"):
-        x = np.array(df['x'].tolist())
-        y = np.array(df['y'].tolist())
-        Bx1 = np.array(df['Bx1'].tolist())*1000
-        By1 = np.array(df['By1'].tolist())*1000
-        Bx2 = np.array(df['Bx2'].tolist())*1000
-        By2 = np.array(df['By2'].tolist())*1000
-        np.random.seed(1234)  # fix seed for reproducibility
-
-        tpc1 = ax[0, 0].tripcolor(x, y, Bx1, shading='gouraud', cmap=cmap)
-        tpc2 = ax[0, 1].tripcolor(x, y, By1, shading='gouraud', cmap=cmap)
-        tpc3 = ax[1, 0].tripcolor(x, y, Bx2, shading='gouraud', cmap=cmap)
-        tpc4 = ax[1, 1].tripcolor(x, y, By2, shading='gouraud', cmap=cmap)
-
-        fig.colorbar(tpc1, ax=ax[0, 0])
-        fig.colorbar(tpc2, ax=ax[0, 1])
-        fig.colorbar(tpc3, ax=ax[1, 0])
-        fig.colorbar(tpc4, ax=ax[1, 1])
-
-
-def plot_difference_Bx_By(df, map2d_name1, map2d_name2, fig, ax, type, cmap='seismic', plot_coil=False):
-    fig.suptitle(f"Difference: {map2d_name1} - {map2d_name2} (mT)")
-    ax[0, 0].set_title(f"Difference Bx (mT)")
-    ax[0, 0].set_xlabel('x-coordinate/mm')
-    ax[0, 0].set_ylabel('y-coordinate/mm')
-    ax[0, 1].set_title(f"Difference By (mT)")
-    ax[0, 1].set_xlabel('x-coordinate/mm')
-    ax[0, 1].set_ylabel('y-coordinate/mm')
-    ax[1, 0].plot(df["diff_x"] * 1000, '.')
-    ax[1, 0].set_title(f"Scatter difference Bx (mT)")
-    ax[1, 0].set_xlabel('Strand number')
-    ax[1, 0].set_ylabel('Difference Bx (mT)')
-    ax[1, 1].plot(df["diff_y"] * 1000, '.')
-    ax[1, 1].set_xlabel('Strand number')
-    ax[1, 1].set_ylabel('Scatter difference By (mT)')
-    ax[1, 1].set_title(f"Scatter difference By (mT)")
-    ax[0, 0].set_aspect("equal")
-    ax[0, 1].set_aspect("equal")
-    if(type=="coil"):
-        f11 = ax[0, 0].scatter(df["x"], df['y'], c=df["diff_x"] * 1000, cmap=cmap)
-        f12 = ax[0, 1].scatter(df["x"], df['y'], c=df["diff_y"] * 1000, cmap=cmap)
-        fig.colorbar(f11, ax=ax[0, 0])
-        fig.colorbar(f12, ax=ax[0, 1])
-    elif(type=="mesh"):
-
-        x = np.array(df['x'].tolist())
-        y = np.array(df['y'].tolist())
-        diff_x = np.array(df['diff_x'].tolist())*1000
-        diff_y = np.array(df['diff_y'].tolist())*1000
-
-        np.random.seed(1234)  # fix seed for reproducibility
-        tpc1 = ax[0, 0].tripcolor(x, y, diff_x, shading='gouraud', cmap=cmap)
-        tpc2 = ax[0, 1].tripcolor(x, y, diff_y, shading='gouraud', cmap=cmap)
-
-        fig.colorbar(tpc1, ax=ax[0, 0])
-        fig.colorbar(tpc2, ax=ax[0, 1])
-
-
-
-def get_df_map2d(map2d_file_path1, map2d_file_path2):
-
-    df1 = pd.read_csv(map2d_file_path1, delim_whitespace=True)
-    df2 = pd.read_csv(map2d_file_path2, delim_whitespace=True)
-    df = pd.DataFrame()
-    df['x'] = df1["X-POS/MM"]
-    df['y'] = df1["Y-POS/MM"]
-    df["Bx1"] = df1["BX/T"]
-    df["By1"] = df1["BY/T"]
-
-    df["Bx2"] = df2["BX/T"]
-    df["By2"] = df2["BY/T"]
-    df = df.apply(pd.to_numeric)
-    df["diff_x"] = df["Bx1"] - df["Bx2"]
-    df["diff_y"] = df["By1"] - df["By2"]
-    try:
-        df["rel_err_x"] = abs((df["Bx1"] - df["Bx2"]) / df["Bx2"])
-    except:
-        print("Can't create rel_err_x plots")
-        df["rel_err_x"] = None
-    try:
-        df["rel_err_y"] = abs((df["By1"] - df["By2"]) / df["By2"])
-    except:
-        print("Can't create rel_err_y plots")
-        df["rel_err_y"] = None
-    df["abs_err_x"] = abs(df["Bx1"] - df["Bx2"])
-    df["abs_err_y"] = abs(df["By1"] - df["By2"])
-    df["Bmod1"] = np.sqrt(df["Bx1"] ** 2 + df["By1"] ** 2)
-    df["Bmod2"] = np.sqrt(df["Bx2"] ** 2 + df["By2"] ** 2)
-    df["Bmod_error"] = abs(df["Bmod1"] - df["Bmod2"])
-    return df
+            tpc = ax[0].tripcolor(x, y, z1, shading='gouraud', cmap=cmap)
+            fig.colorbar(tpc)
 
-def generate_report_from_map2d(prefix, working_dir_path, map2d_file_path1, map2d_name1, map2d_file_path2, map2d_name2, type, save=False):
-    """
-    Generate plots for comparing two map2d files. Method generates the following plots:
-    Bmod fields, Bmod error, relative error Bx/By, Bx/By field, Bx/By error, absolut difference Bx/By
-    :param map2d_file_path1: Path to map2d file nr 1
-    :param map2d_name1: String name of map2d nr 1 (e.g SIGMA/ROXIE)
-    :param map2d_file_path2: Path to map2d file nr 2
-    :param map2d_name2: String name of map2d nr 1 (e.g SIGMA/ROXIE)
-    :return:
-    """
-    df=get_df_map2d(map2d_file_path1, map2d_file_path2)
-    fig1, ax1 = plt.subplots(2, 2, figsize=(12, 12))
-    fig2, ax2 = plt.subplots(1, 2, figsize=(12, 12))
-    fig3, ax3 = plt.subplots(3, 2, figsize=(12, 12))
-    fig4, ax4 = plt.subplots(2, 2, figsize=(12, 12))
-    fig5, ax5 = plt.subplots(2, 2, figsize=(12, 12))
-    plot_Bmod(df, map2d_name1, map2d_name2, fig1, ax1, type)
-    plot_B_mod_error(df,map2d_name1, map2d_name2, fig2, ax2, type)
-    plot_Bx_By(df, map2d_name1, map2d_name2, fig3, ax3, type)
-    text1 = f"{map2d_name1} file path: {map2d_file_path1}"
-    text2 = f"{map2d_name2} file path: {map2d_file_path2}"
-    x_pos = 0.5  # X position of the text (0.0 to 1.0)
-    y_pos = 0.05  #
-    fig5.text(x_pos, y_pos, text1, ha='center')
-
-# Add the second line of text
-    fig5.text(x_pos, y_pos - 0.03, text2, ha='center')
-
-# Show the figure
-    try:
-        plot_relative_error_x_y(df, map2d_name1, map2d_name2, fig4, ax4, type)
-    except:
-        print("Couldn't generate relative error plots.")
-    plot_difference_Bx_By(df, map2d_name1, map2d_name2, fig5, ax5, type)
-    print("----Bmod error description----- ")
-    print(df["Bmod_error"].describe())
-    print(df["Bmod_error"].nlargest(10))
-
-    print("----Rel error x description----- ")
-    print(df["rel_err_x"].describe())
-    print(df["rel_err_x"].nlargest(10))
-    print("----Rel error y description----- ")
-    print(df["rel_err_y"].describe())
-    print(df["rel_err_y"].nlargest(10))
-    to_export = {'B_mod_diff_max' : df["Bmod_error"].max(),'B_mod_diff_mean' : df["Bmod_error"].mean(),
-                 'B_mod_diff_std' : df["Bmod_error"].std(),
-                 'B_x_diff_max' : abs(df["diff_x"]).max(),'B_x_diff_mean' : abs(df["diff_x"]).mean(),
-                 'B_x_diff_std' : abs(df["diff_x"]).std(),
-                 'B_y_diff_max' : abs(df["diff_y"]).max(),'B_y_diff_mean' : abs(df["diff_y"]).mean(),
-                 'B_y_diff_std' :abs(df["diff_y"]).std()}
-
-    if save:
-        fig1.savefig(os.path.join(working_dir_path, f"{prefix}_plot_Bmod_{map2d_name1}_{map2d_name2}.png"))
-        fig2.savefig(os.path.join(working_dir_path,f"{prefix}_plot_B_mod_error_{map2d_name1}_{map2d_name2}.png"))
-        fig3.savefig(os.path.join(working_dir_path,f"{prefix}_plot_Bx_By_{map2d_name1}_{map2d_name2}.png"))
-        fig4.savefig(os.path.join(working_dir_path,f"{prefix}_plot_relative_error_x_y_{map2d_name1}_{map2d_name2}.png"))
-        fig5.savefig(os.path.join(working_dir_path,f"{prefix}_plot_difference_Bx_By_{map2d_name1}_{map2d_name2}.png"))
-
-    # displayWaitAndClose(waitTimeBeforeMessage=.1, waitTimeAfterMessage=0.5)
-    plt.close('all')
-    return to_export
-
-def plot_roxie_coil(roxie_data):
-    xPos = []
-    yPos = []
-    xBarePos = []
-    yBarePos = []
-    iPos = []
-    for coil_nr, coil in roxie_data.coil.coils.items():
-        for pole_nr, pole in coil.poles.items():
-            for layer_nr, layer in pole.layers.items():
-                for winding_key, winding in layer.windings.items():
-                    for block_key, block in winding.blocks.items():
-                        for halfTurn_nr, halfTurn in block.half_turns.items():
-                            insu = halfTurn.corners.insulated
-                            bare = halfTurn.corners.bare
-                            xPos.append([insu.iH.x, insu.oH.x, insu.oL.x, insu.iL.x])
-                            yPos.append([insu.iH.y, insu.oH.y, insu.oL.y, insu.iL.y])
-                            xBarePos.append([bare.iH.x, bare.oH.x, bare.oL.x, bare.iL.x])
-                            yBarePos.append([bare.iH.y, bare.oH.y, bare.oL.y, bare.iL.y])
-                            iPos.append(block.current_sign)
-    return (xPos, yPos, xBarePos, yBarePos, iPos)
-
-def plotEdges(xPos, yPos, xBarePos, yBarePos, iPos, ax):
-    # Plot edges
-    for c, (cXPos, cYPos) in enumerate(zip(xPos, yPos)):
-        pt1, pt2, pt3, pt4 = [cXPos[0]*1000, cYPos[0]*1000], [cXPos[1]*1000, cYPos[1]*1000], [cXPos[2]*1000, cYPos[2]*1000], [cXPos[3]*1000, cYPos[3]*1000]
-        points = [pt1, pt2, pt3, pt4]*1000
-        if iPos[c] > 0:
-            line = patches.Polygon(points, facecolor='k', zorder=1, fill=False)
-        else:
-            line = patches.Polygon(points, facecolor='k', zorder=1, fill=False)
-        ax.add_patch(line)
-
-    for c, (cXBarePos, cYBarePos) in enumerate(zip(xBarePos, yBarePos)):
-        pt1, pt2, pt3, pt4 = [cXBarePos[0]*1000, cYBarePos[0]*1000], [cXBarePos[1]*1000, cYBarePos[1]*1000], \
-                             [cXBarePos[2]*1000, cYBarePos[2]*1000],[cXBarePos[3]*1000, cYBarePos[3]*1000]
-        points = [pt1, pt2, pt3, pt4]
-        if iPos[c] > 0:
-            line = patches.Polygon(points, facecolor='k', zorder=1, fill=False)
-        else:
-            line = patches.Polygon(points, facecolor='k',  zorder=1, fill=False)
-        ax.add_patch(line)
+    def plot_relative_error_x_y(self, df, map2d_name1, map2d_name2, fig, ax, type, cmap='CMRmap'):
+        if df['rel_err_x'] is not None and df['rel_err_y'] is not None:
+            fig.suptitle(f"Relative error: {map2d_name1} and {map2d_name2} (T)")
+            ax[0, 0].set_aspect("equal")
+            ax[0, 1].set_aspect("equal")
+
+            ax[0, 0].set_title(f"Relative error Bx %")
+            ax[0, 0].set_xlabel('x-coordinate/mm')
+            ax[0, 0].set_ylabel('y-coordinate/mm')
+            ax[0, 1].set_title(f"Relative error By %")
+            ax[0, 1].set_xlabel('x-coordinate/mm')
+            ax[0, 1].set_ylabel('y-coordinate/mm')
+
+            ax[1, 0].plot(df["rel_err_x"] * 100, '.')
+            ax[1, 0].set_title(f"Scatter Relative error  Bx %")
+            ax[1, 0].set_xlabel('Strand number')
+            ax[1, 0].set_ylabel('Relative error Bx %')
+            ax[1, 1].plot(df["rel_err_y"] * 100, '.')
+            ax[1, 1].set_xlabel('Strand number')
+            ax[1, 1].set_ylabel('Relative error By %')
+            ax[1, 1].set_title(f"Scatter Relative error  By %")
+            if type == "coil":
+                f31 = ax[0, 0].scatter(df["x"], df['y'], c=df["rel_err_x"] * 100, cmap=cmap)
+                f32 = ax[0, 1].scatter(df["x"], df['y'], c=df["rel_err_y"] * 100, cmap=cmap)
+                fig.colorbar(f31, ax=ax[0, 0])
+                fig.colorbar(f32, ax=ax[0, 1])
+            elif type == "mesh":
+                x = np.array(df['x'].tolist())
+                y = np.array(df['y'].tolist())
+                z1 = np.array(df['rel_err_x'].tolist()) * 100
+                z2 = np.array(df['rel_err_y'].tolist()) * 100
+                np.random.seed(1234)  # fix seed for reproducibility
+
+                tpc1 = ax[0, 0].tripcolor(x, y, z1, shading='gouraud', cmap=cmap)
+                tpc2 = ax[0, 1].tripcolor(x, y, z2, shading='gouraud', cmap=cmap)
+
+                fig.colorbar(tpc1)
+                fig.colorbar(tpc2)
+
+    def plot_Bx_By(self, df, map2d_name1, map2d_name2, fig, ax, type, cmap='seismic', plot_coil=False):
+        fig.suptitle(f"Bx and By field: {map2d_name1} and {map2d_name2} (mT)", fontsize=12)
+
+        ax[0, 0].set_title(f"Bx {map2d_name1} (mT)", fontsize=10)
+        ax[0, 0].set_ylabel('y-coordinate/mm', fontsize=9)
+        ax[0, 0].set_aspect("equal")
+        ax[0, 1].set_aspect("equal")
+        ax[1, 0].set_aspect("equal")
+        ax[1, 1].set_aspect("equal")
+        ax[0, 1].set_title(f"By {map2d_name1} (mT)", fontsize=10)
+        ax[0, 1].set_ylabel('y-coordinate/mm', fontsize=9)
+
+        ax[1, 0].set_title(f"Bx {map2d_name2} (mT)", fontsize=10)
+        ax[1, 0].set_xlabel('x-coordinate/mm', fontsize=9)
+        ax[1, 0].set_ylabel('y-coordinate/mm', fontsize=9)
+        ax[1, 1].set_title(f"By {map2d_name2} (mT)", fontsize=10)
+        ax[1, 1].set_xlabel('x-coordinate/mm', fontsize=9)
+        ax[1, 1].set_ylabel('y-coordinate/mm', fontsize=9)
+        ax[2, 0].set_title(f"Bx scatter (mT)", fontsize=14, loc='left')
+        ax[2, 0].set_ylabel('Bx scatter (mT)', fontsize=9)
+        ax[2, 0].plot(df["Bx1"] * 1000, '.', color='b', label=f"{map2d_name1}")
+        ax[2, 0].plot(df["Bx2"] * 1000, '.', color='r', label=f"{map2d_name2}")
+        ax[2, 1].set_title(f"By scatter (mT)", fontsize=14, loc='left')
+        ax[2, 1].set_ylabel('By scatter (mT)', fontsize=9)
+
+        ax[2, 1].plot(df["By1"] * 1000, '.', color='b', label=f"{map2d_name1}")
+        ax[2, 1].plot(df["By2"] * 1000, '.', color='r', label=f"{map2d_name2}")
+        ax[2, 0].legend()
+        ax[2, 1].legend()
+
+        if type == "coil":
+            f41 = ax[0, 0].scatter(df["x"], df['y'], c=df["Bx1"] * 1000, cmap=cmap)
+            f42 = ax[0, 1].scatter(df["x"], df['y'], c=df["By1"] * 1000, cmap=cmap)
+            f43 = ax[1, 0].scatter(df["x"], df['y'], c=df["Bx2"] * 1000, cmap=cmap)
+            f44 = ax[1, 1].scatter(df["x"], df['y'], c=df["By2"] * 1000, cmap=cmap)
+            fig.colorbar(f41, ax=ax[0, 0])
+            fig.colorbar(f42, ax=ax[0, 1])
+            fig.colorbar(f43, ax=ax[1, 0])
+            fig.colorbar(f44, ax=ax[1, 1])
+        elif type == "mesh":
+            x = np.array(df['x'].tolist())
+            y = np.array(df['y'].tolist())
+            Bx1 = np.array(df['Bx1'].tolist()) * 1000
+            By1 = np.array(df['By1'].tolist()) * 1000
+            Bx2 = np.array(df['Bx2'].tolist()) * 1000
+            By2 = np.array(df['By2'].tolist()) * 1000
+            np.random.seed(1234)  # fix seed for reproducibility
+
+            tpc1 = ax[0, 0].tripcolor(x, y, Bx1, shading='gouraud', cmap=cmap)
+            tpc2 = ax[0, 1].tripcolor(x, y, By1, shading='gouraud', cmap=cmap)
+            tpc3 = ax[1, 0].tripcolor(x, y, Bx2, shading='gouraud', cmap=cmap)
+            tpc4 = ax[1, 1].tripcolor(x, y, By2, shading='gouraud', cmap=cmap)
+
+            fig.colorbar(tpc1, ax=ax[0, 0])
+            fig.colorbar(tpc2, ax=ax[0, 1])
+            fig.colorbar(tpc3, ax=ax[1, 0])
+            fig.colorbar(tpc4, ax=ax[1, 1])
+
+    def plot_difference_Bx_By(self, df, map2d_name1, map2d_name2, fig, ax, type, cmap='seismic', plot_coil=False):
+        fig.suptitle(f"Difference: {map2d_name1} - {map2d_name2} (mT)")
+        ax[0, 0].set_title(f"Difference Bx (mT)")
+        ax[0, 0].set_xlabel('x-coordinate/mm')
+        ax[0, 0].set_ylabel('y-coordinate/mm')
+        ax[0, 1].set_title(f"Difference By (mT)")
+        ax[0, 1].set_xlabel('x-coordinate/mm')
+        ax[0, 1].set_ylabel('y-coordinate/mm')
+        ax[1, 0].plot(df["diff_x"] * 1000, '.')
+        ax[1, 0].set_title(f"Scatter difference Bx (mT)")
+        ax[1, 0].set_xlabel('Strand number')
+        ax[1, 0].set_ylabel('Difference Bx (mT)')
+        ax[1, 1].plot(df["diff_y"] * 1000, '.')
+        ax[1, 1].set_xlabel('Strand number')
+        ax[1, 1].set_ylabel('Scatter difference By (mT)')
+        ax[1, 1].set_title(f"Scatter difference By (mT)")
+        ax[0, 0].set_aspect("equal")
+        ax[0, 1].set_aspect("equal")
+        if (type == "coil"):
+            f11 = ax[0, 0].scatter(df["x"], df['y'], c=df["diff_x"] * 1000, cmap=cmap)
+            f12 = ax[0, 1].scatter(df["x"], df['y'], c=df["diff_y"] * 1000, cmap=cmap)
+            fig.colorbar(f11, ax=ax[0, 0])
+            fig.colorbar(f12, ax=ax[0, 1])
+        elif (type == "mesh"):
+
+            x = np.array(df['x'].tolist())
+            y = np.array(df['y'].tolist())
+            diff_x = np.array(df['diff_x'].tolist()) * 1000
+            diff_y = np.array(df['diff_y'].tolist()) * 1000
+
+            np.random.seed(1234)  # fix seed for reproducibility
+            tpc1 = ax[0, 0].tripcolor(x, y, diff_x, shading='gouraud', cmap=cmap)
+            tpc2 = ax[0, 1].tripcolor(x, y, diff_y, shading='gouraud', cmap=cmap)
+
+            fig.colorbar(tpc1, ax=ax[0, 0])
+            fig.colorbar(tpc2, ax=ax[0, 1])
 
+    def get_df_map2d(self, map2d_files):
 
+        df1 = pd.read_csv(map2d_files[0], delim_whitespace=True)
+        df2 = pd.read_csv(map2d_files[1], delim_whitespace=True)
+        df = pd.DataFrame()
+        df['x'] = df1["X-POS/MM"]
+        df['y'] = df1["Y-POS/MM"]
+        df["Bx1"] = df1["BX/T"]
+        df["By1"] = df1["BY/T"]
+
+        df["Bx2"] = df2["BX/T"]
+        df["By2"] = df2["BY/T"]
+        df = df.apply(pd.to_numeric)
+        df["diff_x"] = df["Bx1"] - df["Bx2"]
+        df["diff_y"] = df["By1"] - df["By2"]
+        try:
+            df["rel_err_x"] = abs((df["Bx1"] - df["Bx2"]) / df["Bx2"])
+        except:
+            print("Can't create rel_err_x plots")
+            df["rel_err_x"] = None
+        try:
+            df["rel_err_y"] = abs((df["By1"] - df["By2"]) / df["By2"])
+        except:
+            print("Can't create rel_err_y plots")
+            df["rel_err_y"] = None
+        df["abs_err_x"] = abs(df["Bx1"] - df["Bx2"])
+        df["abs_err_y"] = abs(df["By1"] - df["By2"])
+        df["Bmod1"] = np.sqrt(df["Bx1"] ** 2 + df["By1"] ** 2)
+        df["Bmod2"] = np.sqrt(df["Bx2"] ** 2 + df["By2"] ** 2)
+        df["Bmod_error"] = abs(df["Bmod1"] - df["Bmod2"])
+        return df
+
+    def generate_report_from_map2d(self, comparison_name: str, file_names: dict, plot_type: str, save: bool = True):
+        """
+        Generate plots for comparing two map2d files. Method generates the following plots:
+        Bmod fields, Bmod error, relative error Bx/By, Bx/By field, Bx/By error, absolut difference Bx/By
+        :return:
+        """
+        sources = list(file_names.keys())
+        paths = [os.path.join(self.parsed_results_path, name) for name in file_names.values()]
+        df = self.get_df_map2d(paths)
+        fig1, ax1 = plt.subplots(2, 2, figsize=(12, 12))
+        fig2, ax2 = plt.subplots(1, 2, figsize=(12, 12))
+        fig3, ax3 = plt.subplots(3, 2, figsize=(12, 12))
+        fig4, ax4 = plt.subplots(2, 2, figsize=(12, 12))
+        fig5, ax5 = plt.subplots(2, 2, figsize=(12, 12))
+        self.plot_Bmod(df, sources[0], sources[1], fig1, ax1, plot_type)
+        self.plot_B_mod_error(df, sources[0], sources[1], fig2, ax2, plot_type)
+        self.plot_Bx_By(df, sources[0], sources[1], fig3, ax3, plot_type)
+        text1 = f"{sources[0]} file path: {paths[0]}"
+        text2 = f"{sources[1]} file path: {paths[1]}"
+        x_pos = 0.5  # X position of the text (0.0 to 1.0)
+        y_pos = 0.05  #
+        fig5.text(x_pos, y_pos, text1, ha='center')
+
+        # Add the second line of text
+        fig5.text(x_pos, y_pos - 0.03, text2, ha='center')
+
+        # Show the figure
+        try:
+            self.plot_relative_error_x_y(df, sources[0], sources[1], fig4, ax4, plot_type)
+        except:
+            print("Couldn't generate relative error plots.")
+        self.plot_difference_Bx_By(df, sources[0], sources[1], fig5, ax5, plot_type)
+        print("----Bmod error description----- ")
+        print(df["Bmod_error"].describe())
+        print(df["Bmod_error"].nlargest(10))
+
+        print("----Rel error x description----- ")
+        print(df["rel_err_x"].describe())
+        print(df["rel_err_x"].nlargest(10))
+        print("----Rel error y description----- ")
+        print(df["rel_err_y"].describe())
+        print(df["rel_err_y"].nlargest(10))
+        to_export = {'B_mod_diff_max': df["Bmod_error"].max(), 'B_mod_diff_mean': df["Bmod_error"].mean(),
+                     'B_mod_diff_std': df["Bmod_error"].std(),
+                     'B_x_diff_max': abs(df["diff_x"]).max(), 'B_x_diff_mean': abs(df["diff_x"]).mean(),
+                     'B_x_diff_std': abs(df["diff_x"]).std(),
+                     'B_y_diff_max': abs(df["diff_y"]).max(), 'B_y_diff_mean': abs(df["diff_y"]).mean(),
+                     'B_y_diff_std': abs(df["diff_y"]).std()}
+
+        if save:
+            fig1.savefig(
+                os.path.join(self.parsed_results_path, f"{comparison_name}_plot_Bmod_{sources[0]}_{sources[1]}.png"))
+            fig2.savefig(os.path.join(self.parsed_results_path,
+                                      f"{comparison_name}_plot_B_mod_error_{sources[0]}_{sources[1]}.png"))
+            fig3.savefig(
+                os.path.join(self.parsed_results_path, f"{comparison_name}_plot_Bx_By_{sources[0]}_{sources[1]}.png"))
+            fig4.savefig(os.path.join(self.parsed_results_path,
+                                      f"{comparison_name}_plot_relative_error_x_y_{sources[0]}_{sources[1]}.png"))
+            fig5.savefig(os.path.join(self.parsed_results_path,
+                                      f"{comparison_name}_plot_difference_Bx_By_{sources[0]}_{sources[1]}.png"))
+
+        # displayWaitAndClose(waitTimeBeforeMessage=.1, waitTimeAfterMessage=0.5)
+        plt.close('all')
+        return to_export
+
+    def plot_roxie_coil(self, roxie_data):
+        xPos = []
+        yPos = []
+        xBarePos = []
+        yBarePos = []
+        iPos = []
+        for coil_nr, coil in roxie_data.coil.coils.items():
+            for pole_nr, pole in coil.poles.items():
+                for layer_nr, layer in pole.layers.items():
+                    for winding_key, winding in layer.windings.items():
+                        for block_key, block in winding.blocks.items():
+                            for halfTurn_nr, halfTurn in block.half_turns.items():
+                                insu = halfTurn.corners.insulated
+                                bare = halfTurn.corners.bare
+                                xPos.append([insu.iH.x, insu.oH.x, insu.oL.x, insu.iL.x])
+                                yPos.append([insu.iH.y, insu.oH.y, insu.oL.y, insu.iL.y])
+                                xBarePos.append([bare.iH.x, bare.oH.x, bare.oL.x, bare.iL.x])
+                                yBarePos.append([bare.iH.y, bare.oH.y, bare.oL.y, bare.iL.y])
+                                iPos.append(block.current_sign)
+        return (xPos, yPos, xBarePos, yBarePos, iPos)
+
+    def plotEdges(self, xPos, yPos, xBarePos, yBarePos, iPos, ax):
+        # Plot edges
+        for c, (cXPos, cYPos) in enumerate(zip(xPos, yPos)):
+            pt1, pt2, pt3, pt4 = [cXPos[0] * 1000, cYPos[0] * 1000], [cXPos[1] * 1000, cYPos[1] * 1000], [
+                cXPos[2] * 1000, cYPos[2] * 1000], [cXPos[3] * 1000, cYPos[3] * 1000]
+            points = [pt1, pt2, pt3, pt4] * 1000
+            if iPos[c] > 0:
+                line = patches.Polygon(points, facecolor='k', zorder=1, fill=False)
+            else:
+                line = patches.Polygon(points, facecolor='k', zorder=1, fill=False)
+            ax.add_patch(line)
+
+        for c, (cXBarePos, cYBarePos) in enumerate(zip(xBarePos, yBarePos)):
+            pt1, pt2, pt3, pt4 = [cXBarePos[0] * 1000, cYBarePos[0] * 1000], [cXBarePos[1] * 1000, cYBarePos[1] * 1000], \
+                                 [cXBarePos[2] * 1000, cYBarePos[2] * 1000], [cXBarePos[3] * 1000, cYBarePos[3] * 1000]
+            points = [pt1, pt2, pt3, pt4]
+            if iPos[c] > 0:
+                line = patches.Polygon(points, facecolor='k', zorder=1, fill=False)
+            else:
+                line = patches.Polygon(points, facecolor='k', zorder=1, fill=False)
+            ax.add_patch(line)
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/plotters/PlotterModel.py` & `steam-sdk-2024.4.0/steam_sdk/plotters/PlotterModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
 from steam_sdk.data import DataModelMagnet
 from steam_sdk.data.DataRoxieParser import RoxieData
 from steam_sdk.parsers.ParserRoxie import RoxieList
 from steam_sdk.utils.misc import displayWaitAndClose, find_indices
 from steam_sdk.plotters import PlotterRoxie
-from steam_sdk.parsers.ParserMap2d import getParametersFromMap2d
 
 
 class PlotterModel:
     def __init__(self, roxie_data: RoxieData = None):
         if roxie_data:
             RL = RoxieList(roxie_data)
             self.x_insulated = RL.x_insulated
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/plotters/PlotterParametric.py` & `steam-sdk-2024.4.0/steam_sdk/plotters/PlotterParametric.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/plotters/PlotterRoxie.py` & `steam-sdk-2024.4.0/steam_sdk/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/postprocs/PostprocsMetrics.py` & `steam-sdk-2024.4.0/steam_sdk/postprocs/PostprocsMetrics.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,90 +23,68 @@
         # Define inputs
         self.metrics_to_do = metrics_to_do
         self.var_to_interpolate = var_to_interpolate
         self.var_to_interpolate_ref = var_to_interpolate_ref
         self.time_vector = time_vector
         self.time_vector_ref = time_vector_ref
 
-        # Convert variables to np.array, if needed
-        self.var_to_interpolate = [np.array(v) for v in self.var_to_interpolate]
-        self.var_to_interpolate_ref = [np.array(v) for v in self.var_to_interpolate_ref]
-        self.time_vector = [np.array(v) for v in self.time_vector]
-        self.time_vector_ref = [np.array(v) for v in self.time_vector_ref]
+        # Convert variables to a list if needed
+        self.var_to_interpolate = self._convert_to_list(self.var_to_interpolate)
+        self.var_to_interpolate_ref = self._convert_to_list(self.var_to_interpolate_ref)
+        self.time_vector = self._convert_to_list(self.time_vector)
+        self.time_vector_ref = self._convert_to_list(self.time_vector_ref)
 
         if flag_run:
             self.run_metrics()
 
     def run_metrics(self):
-
         """
             Function to initiate interpolation, start the different metrics and append the result to the output
         """
-        # unpack inputs
-        metrics_to_do = self.metrics_to_do
-        var_of_interest = self.var_to_interpolate
-        var_ref = self.var_to_interpolate_ref
-        time_vector = self.time_vector
-        time_vector_ref = self.time_vector_ref
-
         # variables which need to be interpolated
-        list_metrics_that_need_interpolation = ['maximum_abs_error', 'RMSE', 'RELATIVE_RMSE', 'RMSE_ratio', 'MARE','MARE_1S']
-        # list_metrics_that_need_interpolation_ref = ['maximum_abs_error', 'RMSE', 'RELATIVE_RMSE','RMSE_ratio','MARE']
-        # --> Having two lists here doesnt make any sense because for comparative metrics we ALWAYS have to do both interpolations
-
+        list_metrics_that_need_interpolation = ['maximum_abs_error', 'RMSE', 'RELATIVE_RMSE', 'RMSE_ratio',
+                                                'RELATIVE_RMSE_AFTER_t_PC_off', 'MARE','MARE_1S']
          # For metrics that need interpolation of both simulation data and reference data:
-        if any(n in metrics_to_do for n in set(list_metrics_that_need_interpolation)):
-            # If in the touples of timestep and datapoint at least one value is NaN, then we remove the whole row from both lists
-            var_of_interest, time_vector = zip(*[var_pair for var_pair in zip(var_of_interest, time_vector) if
-                                                 not any(np.isnan(value) for value in var_pair)])
-            var_ref, time_vector_ref = zip(*[(var, time) for var, time in zip(var_ref, time_vector_ref) if
-                                             not any(np.isnan(value) for value in (var, time))])
-
-            # Get the equaly spaced timestamps within the time interval of the reference data for possible interpolations
-            time_stamps_ref = np.linspace(time_vector_ref[0], time_vector_ref[-1], num=len(time_vector_ref))
-
-            # Interpolate the simulation data to the timestamps of the reference data
-            var_of_interest = self._interpolation(time_stamps_ref, time_vector, var_of_interest)
-            var_ref = self._interpolation(time_stamps_ref, time_vector_ref, var_ref)
-
-            # We only want to consider those parts of the interpolated datasets, where the original data overlapped, because
-            # outside this region, the interpolation might be very wrong:
-            # Determine start and end of the reference dataset
-            start_ref = min(time_vector_ref)
-            end_ref = max(time_vector_ref)
-            # Determine start and end of the simulated dataset
-            start_interest = min(time_vector)
-            end_interest = max(time_vector)
-
-            # Determine their overlap
-            end_overlap = min(end_ref, end_interest)
-            start_overlap = max(start_ref, start_interest)
-
-            # Create a subset of data that only contains the region of the interpolation, where the initial datasets overlapped
-            var_of_interest_overlap, time_stamps_overlap, var_ref_overlap = [], [], []
-            for index, timestep in enumerate(time_stamps_ref):
-                if (start_overlap <= timestep and timestep <= end_overlap):
-                    var_of_interest_overlap.append(var_of_interest[index])
-                    time_stamps_overlap.append(time_stamps_ref[index])
-                    var_ref_overlap.append(var_ref[index])
+        if any(n in self.metrics_to_do for n in set(list_metrics_that_need_interpolation)):
+
+            # Clean arrays
+            var_to_interpolate_cleaned, time_vector_cleaned = self.clean_array_touple(
+                self.var_to_interpolate,
+                self.time_vector)
+            var_to_interpolate_ref_cleaned, time_vector_ref_cleaned = self.clean_array_touple(
+                self.var_to_interpolate_ref,
+                self.time_vector_ref)
+
+            var_of_interest_overlap, time_stamps_overlap, var_ref_overlap = self.get_overlap(
+                time_vector_ref=time_vector_ref_cleaned,time_vector_interest = time_vector_cleaned,
+                var_ref = var_to_interpolate_ref_cleaned,var_interest = var_to_interpolate_cleaned)
 
             # Use only this region of the overlap to calculate the metrics:
             var_of_interest = np.array(var_of_interest_overlap)
             var_ref = np.array(var_ref_overlap)
             time_stamps_overlap = np.array(time_stamps_overlap)
+            time_vector = np.array(time_vector_cleaned)
+            time_vector_ref = np.array(time_vector_ref_cleaned)
+        else:
+            var_of_interest = np.array(self.var_to_interpolate)
+            var_ref  = np.array(self.var_to_interpolate_ref)
+            time_vector = np.array(self.time_vector)
+            time_vector_ref = np.array(self.time_vector_ref)
 
         # evaluating which metrics will be done and appending results to metrics_result
         self.metrics_result = []
-        for metric in metrics_to_do:
+        for metric in self.metrics_to_do:
             if metric == 'maximum_abs_error':
-                result = self._maximum_abs_error(var_of_interest, var_ref)
+                result = self._maximum_abs_error(var_of_interest,var_ref )
             elif metric == 'RMSE':
                 result = self._RMSE(var_of_interest, var_ref)
             elif metric == 'RELATIVE_RMSE':
                 result = self._RELATIVE_RMSE(var_of_interest, var_ref)
+            elif metric == 'RELATIVE_RMSE_AFTER_t_PC_off':
+                result = self._RELATIVE_RMSE_AFTER_t_PC_off(var_of_interest, var_ref,time_stamps_overlap)
             elif metric == 'RMSE_ratio':
                 result = self._RMSE_ratio(var_of_interest, var_ref)
             elif metric == 'MARE':
                 result = self._MARE(var_of_interest, var_ref) # Calculate Mean Absolute Relative Error (MARE)
             elif metric == 'MARE_1S':
                 result = self._MARE_1S(var_of_interest,var_ref,time_stamps_overlap)
             elif metric == 'quench_load_error':
@@ -127,98 +105,156 @@
             function to interpolate a variable
         """
 
         return np.interp(linspace_time_stamps, time_vector, var_to_interpolate) if len(
             var_to_interpolate) != 0 else []
 
     @staticmethod
-    def _maximum_abs_error(y, y_ref):
-
+    def _maximum_abs_error(y, y_ref)-> float:
         """
             function to calculate the absolute error between simulation and measurement
         """
 
-        return max(abs(y - y_ref))
+        return float(max(abs(y - y_ref)))
 
     @staticmethod
-    def _RMSE(y, y_ref):
+    def _RMSE(y, y_ref)-> float:
 
         """
             function to calculate the RMSE between simulation and measurement
         """
 
-        return np.sqrt(((y - y_ref) ** 2).mean()) # np.sqrt(mean_squared_error(y, y_ref))
+        return float(np.sqrt(((y - y_ref) ** 2).mean()) )# np.sqrt(mean_squared_error(y, y_ref))
 
     @staticmethod
-    def _RELATIVE_RMSE(y, y_ref):
+    def _RELATIVE_RMSE(y, y_ref)-> float:
 
         """
             function to calculate the RMSE between simulation and measurement, but normalized to the maximum reference value
         """
         avoid_zero_division = 1e-10
         max_abs_y_ref = np.max(np.abs(y_ref)) + avoid_zero_division
         RELATIVE_RMSE = np.sqrt(((y - y_ref) ** 2).mean())/max_abs_y_ref
 
-        return RELATIVE_RMSE # np.sqrt(mean_squared_error(y, y_ref))
+        return float(RELATIVE_RMSE) # np.sqrt(mean_squared_error(y, y_ref))
+
+    def _RELATIVE_RMSE_AFTER_t_PC_off(self, y, y_ref,time_stamps_overlap)-> float:
+        y_after_t_PC_off = []
+        y_ref_after_t_PC_off = []
+
+        for index, timestamp in enumerate(time_stamps_overlap):
+            if (0 <= timestamp):
+                y_after_t_PC_off.append(y[index])
+                y_ref_after_t_PC_off.append(y_ref[index])
+
+        y_after_t_PC_off = np.array(y_after_t_PC_off)
+        y_ref_after_t_PC_off = np.array(y_ref_after_t_PC_off)
+
+        avoid_zero_division = 1e-10
+        max_abs_y_ref_after_t_PC_off = np.max(np.abs(y_ref_after_t_PC_off)) + avoid_zero_division
+        RELATIVE_RMSE_AFTER_t_PC_off = np.sqrt(((y_after_t_PC_off - y_ref_after_t_PC_off) ** 2).mean()) / max_abs_y_ref_after_t_PC_off
+
+        return float(RELATIVE_RMSE_AFTER_t_PC_off)  # np.sqrt(mean_squared_error(y, y_ref))
 
     @staticmethod
-    def _MARE(y,y_ref):
+    def _MARE(y,y_ref) -> float:
         "Calculate Mean Absolute Relative Error (MARE)"
         avoid_zero_division = 1e-10
         MARE = np.abs((y - y_ref)/(y_ref+avoid_zero_division)).mean()
-        return MARE
+        return float(MARE)
 
-    def _MARE_1S(self, y,y_ref,time_stamps_overlap):
+    def _MARE_1S(self, y,y_ref,time_stamps_overlap)-> float:
         "Calculate Mean Absolute Relative Error (MARE) 1S arround the switchoff time t_PC_off"
         y_around_t_PC_off = []
         y_ref_around_t_PC_off = []
 
         for index, timestamp in enumerate(time_stamps_overlap):
             if(-1 <= timestamp <= 1):
                 y_around_t_PC_off.append(y[index])
                 y_ref_around_t_PC_off.append(y_ref[index])
 
         y_around_t_PC_off = np.array(y_around_t_PC_off)
         y_ref_around_t_PC_off = np.array(y_ref_around_t_PC_off)
 
         avoid_zero_division = 1e-10
         MARE_1S_AROUND_T_PC_OFF = np.abs((y_around_t_PC_off - y_ref_around_t_PC_off)/(y_ref_around_t_PC_off+avoid_zero_division)).mean()
-        return MARE_1S_AROUND_T_PC_OFF
+        return float(MARE_1S_AROUND_T_PC_OFF)
 
-    def _RMSE_ratio(self, y, y_ref):
+    def _RMSE_ratio(self, y, y_ref)-> float:
 
         """
             function to calculate the RMSE divided by the peak value of the measurement between simulation and measurement
         """
 
-        return np.sqrt(((y - y_ref) ** 2).mean())/self._peak_value(y_ref)
+        return float(np.sqrt(((y - y_ref) ** 2).mean())/self._peak_value(y_ref))
 
-    def _quench_load_error(self, time_vector, Ia, time_vector_ref, Ia_ref):
+    def _quench_load_error(self, time_vector, Ia, time_vector_ref, Ia_ref)-> float:
 
         """
             function to calculate the quench load error between simulation and measurement
         """
 
-        return self._quench_load(time_vector, Ia) - self._quench_load(time_vector_ref, Ia_ref)
+        return float(self._quench_load(time_vector, Ia) - self._quench_load(time_vector_ref, Ia_ref))
 
     @staticmethod
-    def _quench_load(time_vector, Ia):
+    def _quench_load(time_vector, Ia)-> float:
 
         """
             function to calculate the quench load of a current
         """
 
         dt = [*np.diff(time_vector), 0]
         quench_load_sum = np.cumsum((Ia ** 2) * dt)
         quench_load = quench_load_sum[-1]
 
-        return quench_load
+        return float(quench_load)
 
     @staticmethod
-    def _peak_value(signal):
+    def _peak_value(signal)-> float:
 
         """
             function to calculate the peak value of a signal
         """
 
-        return max(signal)
+        return float(max(signal))
+
+    @staticmethod
+    def clean_array_touple(array1, array2):
+        # If in the touples of timestep and datapoint at least one value is NaN, then we remove the whole row from both lists
+        array1_cleaned, array2_cleaned = zip(*[var_pair for var_pair in zip(array1, array2) if
+                                               all((isinstance(value, (int, float)) and not np.isnan(value)) for value
+                                                   in var_pair)])
+        return list(array1_cleaned), list(array2_cleaned)
+
+    @staticmethod
+    def _convert_to_list(obj):
+        if isinstance(obj, np.ndarray):
+            return obj.tolist()
+        else:
+            return obj
+
+    @staticmethod
+    def get_overlap(time_vector_ref, time_vector_interest, var_ref, var_interest):
+        # create a sample set of equally spaced timepoints that has the intervall and resolution of the reference data
+        equally_spaced_timestamps = np.linspace(time_vector_ref[0], time_vector_ref[-1],
+                                                num=len(time_vector_ref))
+        # interpolate both variables to these timestamps
+        var_interest_interpolatet = np.interp(equally_spaced_timestamps, time_vector_interest, var_interest)
+        var_ref_interpolatet = np.interp(equally_spaced_timestamps, time_vector_ref, var_ref)
+        # outside this region, the interpolation might be very wrong:
+        # Determine start and end of the reference dataset
+        start_ref = min(time_vector_ref)
+        end_ref = max(time_vector_ref)
+        # Determine start and end of the simulated dataset
+        start_interest = min(time_vector_interest)
+        end_interest = max(time_vector_interest)
+        # Determine their overlap
+        end_overlap = min(end_ref, end_interest)
+        start_overlap = max(start_ref, start_interest)
+        var_of_interest_overlap, time_stamps_overlap, var_ref_overlap = [], [], []
+        for index, timestep in enumerate(equally_spaced_timestamps):
+            if (start_overlap <= timestep and timestep <= end_overlap):
+                var_of_interest_overlap.append(var_interest_interpolatet[index])
+                var_ref_overlap.append(var_ref_interpolatet[index])
+                time_stamps_overlap.append(equally_spaced_timestamps[index])
 
+        return var_of_interest_overlap, time_stamps_overlap, var_ref_overlap
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/utils/MTF_reading_functions.py` & `steam-sdk-2024.4.0/steam_sdk/utils/MTF_reading_functions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/utils/ModifyModelData.py` & `steam-sdk-2024.4.0/steam_sdk/utils/ModifyModelData.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/utils/ModifyModelDataMagnet.py` & `steam-sdk-2024.4.0/steam_sdk/utils/ModifyModelDataMagnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 if __name__ == "__main__":  # pragma: no cover
     # path_to_models = Path.joinpath(
     #     Path(__file__).parent.parent.parent,
     #     "C:\\Users\emm\cernbox\SWAN_projects\steam_models\magnets",
     # )
     path_to_models = Path.joinpath(
-        Path(__file__).parent.parent.parent, r"E:\Python\steam_models\magnets")
+        Path(__file__).parent.parent.parent, r"D:\Code_new\steam_models\magnets")
 
     # path_to_models = Path.joinpath(
     #     Path(__file__).parent.parent.parent, "tests/builders/model_library/magnets"
     # )
     model_names = [x.parts[-1] for x in Path(path_to_models).iterdir() if x.is_dir()]
     #model_names = ['MCBRD']
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/utils/ModifyModelDataconductor.py` & `steam-sdk-2024.4.0/steam_sdk/utils/ModifyModelDataconductor.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from pathlib import Path
 import yaml
 
 from steam_sdk.data.DataModelConductor import DataModelConductor
 from steam_sdk.parsers.ParserYAML import dict_to_yaml
 
 if __name__ == "__main__":  # pragma: no cover
-    path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'C:\\Users\emm\cernbox\SWAN_projects\steam_models\conductors')
-    path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'tests/builders/model_library/conductors')
+    path_models = Path.joinpath(Path(__file__).parent.parent.parent, r"D:\Code_new\steam_sdk\tests\builders\model_library\conductors")
+    # path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'tests/builders/model_library/conductors')
     models = [x.parts[-1] for x in Path(path_models).iterdir() if x.is_dir()]
 
     for mm in models:
         # Read file
         file_model_data = Path.joinpath(path_models, mm, 'input', 'modelData_' + mm + '.yaml')
         if os.path.isfile(file_model_data):
             # Load yaml keys into DataAnalysis dataclass
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/utils/ParserRoxieHelpers.py` & `steam-sdk-2024.4.0/steam_sdk/utils/ParserRoxieHelpers.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/utils/attribute_model.py` & `steam-sdk-2024.4.0/steam_sdk/utils/attribute_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,18 +26,23 @@
         if idx_conductor is None:  # Standard case when the variable to change is not the Conductors key
             value = rgetattr(builder_model.conductor_data, name_variable)
         else:
             value = rgetattr(builder_model.conductor_data.Conductors[idx_conductor], name_variable)
     elif case_model == 'circuit':
         # If the attribute is a dict, and a certain key of this dict has been specified for change,
         # the following piece of code will be run:
-        if "Netlist[" in name_variable and "]" in name_variable:  # this means an entry of a dict was defined.
+        if "Netlist[" in name_variable and "]" in name_variable:  # Special case: this means an entry Netlist was defined.
             component_name = name_variable.split("Netlist[")[1].split(']')[0]
             component_attribute = name_variable.split("Netlist[")[1].split(']')[1].strip('.')
             value = getattr(builder_model.circuit_data.Netlist[component_name], component_attribute)
+        elif "[" in name_variable and "]" in name_variable:  # this means an entry of a dict was defined.
+            dict_name = name_variable.split("[")[0]
+            dict_entries = rgetattr(builder_model.circuit_data, dict_name)
+            dict_key = re.search(r"\[(.*?)\]", name_variable).group(1)
+            value = dict_entries[dict_key]
         else:
             value = rgetattr(builder_model.circuit_data, name_variable)
     else:
         raise Exception(f'Model type not supported: case_model={case_model}')
     return value
 
 
@@ -64,16 +69,22 @@
         if idx_conductor is None:  # Standard case when the variable to change is not the Conductors key
             rsetattr(builder_model.conductor_data, name_variable, value_variable)
         else:
             rsetattr(builder_model.conductor_data.Conductors[idx_conductor], name_variable, value_variable)
     elif case_model == 'circuit':
         # If the attribute is a dict, and a certain key of this dict has been specified for change,
         # the following piece of code will be run:
-        if "Netlist[" in name_variable and "]" in name_variable:  # this means an entry of a dict was defined.
+        if "Netlist[" in name_variable and "]" in name_variable:  # Special case: this means an entry Netlist was defined.
             component_name = name_variable.split("Netlist[")[1].split(']')[0]
             component_attribute = name_variable.split("Netlist[")[1].split(']')[1].strip('.')
             setattr(builder_model.circuit_data.Netlist[component_name], component_attribute, value_variable)
             rsetattr(builder_model.circuit_data, 'Netlist', builder_model.circuit_data.Netlist)
+        elif "[" in name_variable and "]" in name_variable:  # this means an entry of a dict was defined.
+            dict_name = name_variable.split("[")[0]
+            dict_key = re.search(r"\[(.*?)\]", name_variable).group(1)
+            dict_entries = rgetattr(builder_model.circuit_data, dict_name)
+            dict_entries[dict_key] = value_variable
+            rsetattr(builder_model.circuit_data, dict_name, dict_entries)
         else:
             rsetattr(builder_model.circuit_data, name_variable, value_variable)
     else:
         raise Exception(f'Model type not supported: case_model={case_model}')
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/utils/clean_NaN_from_signal.py` & `steam-sdk-2024.4.0/steam_sdk/utils/clean_NaN_from_signal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/utils/compare_simulations.py` & `steam-sdk-2024.4.0/steam_sdk/utils/compare_simulations.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/utils/compare_two_parameters.py` & `steam-sdk-2024.4.0/steam_sdk/utils/compare_two_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/utils/get_attribute_type.py` & `steam-sdk-2024.4.0/steam_sdk/utils/get_attribute_type.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/utils/misc.py` & `steam-sdk-2024.4.0/steam_sdk/utils/misc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/utils/parse_str_to_list.py` & `steam-sdk-2024.4.0/steam_sdk/utils/parse_str_to_list.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/utils/read_settings_file.py` & `steam-sdk-2024.4.0/steam_sdk/utils/read_settings_file.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 import os
-from pathlib import Path
 
 from steam_sdk.data.DataSettings import DataSettings
 from steam_sdk.parsers.ParserYAML import yaml_to_data
 
 
-def read_settings_file(relative_path_settings: str = None, verbose: bool = False):
+# def read_settings_file(relative_path_settings: str = None, verbose: bool = False):
+#     user_name = os.getlogin()
+#     if verbose:
+#         print('user_name:   {}'.format(user_name))
+#     if not relative_path_settings:
+#         relative_path_settings = '../'
+#     path_settings_folder = Path(os.getcwd() / Path(relative_path_settings)).resolve()
+#     settings_file = Path.joinpath(path_settings_folder, f"settings.{user_name}.yaml")
+#     if not Path.exists(settings_file):
+#         raise Exception(f'Settings file not found at: {settings_file}')
+#     data_settings: DataSettings = yaml_to_data(settings_file, DataSettings)
+#
+#     if verbose:
+#         print(f'path_settings: {path_settings_folder}')
+#         print(f'path to settings file: {settings_file}')
+#
+#     return data_settings
+
+def read_settings_file(absolute_path_settings_folder: str = None, verbose: bool = False):
     user_name = os.getlogin()
     if verbose:
         print('user_name:   {}'.format(user_name))
-    if not relative_path_settings:
-        relative_path_settings = '../'
-    path_settings = Path(os.getcwd() / Path(relative_path_settings)).resolve()
-    settings_file = Path.joinpath(path_settings, f"settings.{user_name}.yaml")
-    if not Path.exists(settings_file):
-        raise Exception(f'Settings file not found at this path: {settings_file}')
-        # settings_file = Path.joinpath(Path(os.getcwd()).parent, "settings.SYSTEM.yaml")
-    data_settings = yaml_to_data(settings_file, DataSettings)
+    settings_file = os.path.join(absolute_path_settings_folder, f"settings.{user_name}.yaml")
+    if not os.path.exists(settings_file):
+        raise Exception(f'Settings file not found at: {settings_file}')
+    data_settings: DataSettings = yaml_to_data(settings_file, DataSettings)
 
-    # Display defined paths
     if verbose:
-        print(f'path_settings: {path_settings}')
+        print(f'path_settings: {absolute_path_settings_folder}')
         print(f'path to settings file: {settings_file}')
 
-    return path_settings, data_settings
+    return data_settings
```

### Comparing `steam-sdk-2024.3.1/steam_sdk/utils/reformat_figure.py` & `steam-sdk-2024.4.0/steam_sdk/utils/reformat_figure.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/utils/tic_toc.py` & `steam-sdk-2024.4.0/steam_sdk/utils/tic_toc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/utils/utils_PC.py` & `steam-sdk-2024.4.0/steam_sdk/utils/utils_PC.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/viewers/Viewer.py` & `steam-sdk-2024.4.0/steam_sdk/viewers/Viewer.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk/wrappers/wrapper_yaml.py` & `steam-sdk-2024.4.0/steam_sdk/wrappers/wrapper_yaml.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.3.1/steam_sdk.egg-info/PKG-INFO` & `steam-sdk-2024.4.0/steam_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2024.3.1
+Version: 2024.4.0
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
-Keywords: API,SDK,STEAM,CERN
+Keywords: STEAM,API,SDK,CERN
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: gmsh==4.11.1
 Requires-Dist: matplotlib==3.8.3
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: numpy==1.26.4
@@ -24,15 +24,15 @@
 Requires-Dist: matplotlib-inline==0.1.6
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: pysoleno==0.0.8
 Requires-Dist: reportlab==4.1.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: ruamel.yaml.clib==0.2.8
 Requires-Dist: seaborn==0.13.2
-Requires-Dist: STEAM-materials==2023.5.1
+Requires-Dist: STEAM-materials==2024.4.2
 Requires-Dist: svglib==1.5.1
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: steam-pysigma==2024.3.2
 Requires-Dist: pyarrow==15.0.1
 Requires-Dist: tqdm==4.66.2
 Provides-Extra: all
 Requires-Dist: gmsh==4.11.1; extra == "all"
@@ -50,15 +50,15 @@
 Requires-Dist: matplotlib-inline==0.1.6; extra == "all"
 Requires-Dist: openpyxl==3.1.2; extra == "all"
 Requires-Dist: pysoleno==0.0.8; extra == "all"
 Requires-Dist: reportlab==4.1.0; extra == "all"
 Requires-Dist: requests==2.31.0; extra == "all"
 Requires-Dist: ruamel.yaml.clib==0.2.8; extra == "all"
 Requires-Dist: seaborn==0.13.2; extra == "all"
-Requires-Dist: STEAM-materials==2023.5.1; extra == "all"
+Requires-Dist: STEAM-materials==2024.4.2; extra == "all"
 Requires-Dist: svglib==1.5.1; extra == "all"
 Requires-Dist: PyYAML==6.0.1; extra == "all"
 Requires-Dist: steam-pysigma==2024.3.2; extra == "all"
 Requires-Dist: pyarrow==15.0.1; extra == "all"
 Requires-Dist: tqdm==4.66.2; extra == "all"
 Requires-Dist: Markdown==3.5.2; extra == "all"
 Requires-Dist: markdown-include==0.8.1; extra == "all"
```

### Comparing `steam-sdk-2024.3.1/steam_sdk.egg-info/SOURCES.txt` & `steam-sdk-2024.4.0/steam_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 steam_sdk/builders/BuilderCosim.py
 steam_sdk/builders/BuilderFiQuS.py
 steam_sdk/builders/BuilderLEDET.py
 steam_sdk/builders/BuilderModel.py
 steam_sdk/builders/BuilderProteCCT.py
 steam_sdk/builders/BuilderPyBBQ.py
 steam_sdk/builders/BuilderPySIGMA.py
+steam_sdk/builders/BuilderTFM.py
 steam_sdk/builders/SelfMutualInductanceCalculation.py
 steam_sdk/builders/Solenoids.py
 steam_sdk/builders/__init__.py
 steam_sdk/builders/geometricFunctions.py
 steam_sdk/configs/__init__.py
 steam_sdk/configs/tools_defaults/ToolDefaultReader.py
 steam_sdk/configs/tools_defaults/__init__.py
@@ -77,14 +78,15 @@
 steam_sdk/data/DataPyCoSim.py
 steam_sdk/data/DataPySIGMA.py
 steam_sdk/data/DataPySIGMAOptions.py
 steam_sdk/data/DataRoxieParams.py
 steam_sdk/data/DataRoxieParser.py
 steam_sdk/data/DataSettings.py
 steam_sdk/data/DataSignal.py
+steam_sdk/data/DataTFM.py
 steam_sdk/data/DictionaryLEDET.py
 steam_sdk/data/DictionaryProteCCT.py
 steam_sdk/data/DictionaryPyBBQ.py
 steam_sdk/data/TemplateLEDET.py
 steam_sdk/data/TemplateProteCCT.py
 steam_sdk/data/__init__.py
 steam_sdk/drivers/DriverANSYS.py
@@ -94,24 +96,24 @@
 steam_sdk/drivers/DriverLEDET.py
 steam_sdk/drivers/DriverPSPICE.py
 steam_sdk/drivers/DriverProteCCT.py
 steam_sdk/drivers/DriverPyBBQ.py
 steam_sdk/drivers/DriverPySIGMA.py
 steam_sdk/drivers/DriverXYCE.py
 steam_sdk/drivers/__init__.py
-steam_sdk/drivers/to_DELETE.py
 steam_sdk/parsers/CSD_Reader.py
 steam_sdk/parsers/ParserCOMSOLToTxt.py
 steam_sdk/parsers/ParserCOSIM.py
 steam_sdk/parsers/ParserCond2d.py
 steam_sdk/parsers/ParserCsd.py
 steam_sdk/parsers/ParserCsv.py
 steam_sdk/parsers/ParserDakota.py
 steam_sdk/parsers/ParserExcel.py
 steam_sdk/parsers/ParserFiQuS.py
+steam_sdk/parsers/ParserFile.py
 steam_sdk/parsers/ParserLEDET.py
 steam_sdk/parsers/ParserMap2d.py
 steam_sdk/parsers/ParserMat.py
 steam_sdk/parsers/ParserPSPICE.py
 steam_sdk/parsers/ParserPdf.py
 steam_sdk/parsers/ParserProteCCT.py
 steam_sdk/parsers/ParserPyBBQ.py
@@ -136,33 +138,31 @@
 steam_sdk/plotters/PlotterModel.py
 steam_sdk/plotters/PlotterParametric.py
 steam_sdk/plotters/PlotterRoxie.py
 steam_sdk/plotters/__init__.py
 steam_sdk/postprocs/PostprocsMetrics.py
 steam_sdk/postprocs/__init__.py
 steam_sdk/utils/MTF_reading_functions.py
+steam_sdk/utils/MatrixOperations.py
 steam_sdk/utils/ModifyModelData.py
 steam_sdk/utils/ModifyModelDataMagnet.py
 steam_sdk/utils/ModifyModelDataconductor.py
 steam_sdk/utils/NumpyEncoder.py
 steam_sdk/utils/ParserRoxieHelpers.py
 steam_sdk/utils/__init__.py
 steam_sdk/utils/attribute_model.py
 steam_sdk/utils/clean_NaN_from_signal.py
 steam_sdk/utils/compare_simulations.py
 steam_sdk/utils/compare_two_parameters.py
+steam_sdk/utils/correct_RRR_NIST.py
 steam_sdk/utils/delete_if_existing.py
-steam_sdk/utils/find_delete_files.py
 steam_sdk/utils/get_attribute_type.py
 steam_sdk/utils/isNaN.py
 steam_sdk/utils/make_folder_if_not_existing.py
-steam_sdk/utils/make_json_schema.py
 steam_sdk/utils/misc.py
-steam_sdk/utils/overwrite_files.py
-steam_sdk/utils/overwrite_output_to_reference_files.py
 steam_sdk/utils/parse_str_to_list.py
 steam_sdk/utils/read_settings_file.py
 steam_sdk/utils/reformat_figure.py
 steam_sdk/utils/rgetattr.py
 steam_sdk/utils/rhasattr.py
 steam_sdk/utils/sgetattr.py
 steam_sdk/utils/tic_toc.py
```

### Comparing `steam-sdk-2024.3.1/steam_sdk.egg-info/requires.txt` & `steam-sdk-2024.4.0/steam_sdk.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 matplotlib-inline==0.1.6
 openpyxl==3.1.2
 pysoleno==0.0.8
 reportlab==4.1.0
 requests==2.31.0
 ruamel.yaml.clib==0.2.8
 seaborn==0.13.2
-STEAM-materials==2023.5.1
+STEAM-materials==2024.4.2
 svglib==1.5.1
 PyYAML==6.0.1
 steam-pysigma==2024.3.2
 pyarrow==15.0.1
 tqdm==4.66.2
 
 [all]
@@ -40,15 +40,15 @@
 matplotlib-inline==0.1.6
 openpyxl==3.1.2
 pysoleno==0.0.8
 reportlab==4.1.0
 requests==2.31.0
 ruamel.yaml.clib==0.2.8
 seaborn==0.13.2
-STEAM-materials==2023.5.1
+STEAM-materials==2024.4.2
 svglib==1.5.1
 PyYAML==6.0.1
 steam-pysigma==2024.3.2
 pyarrow==15.0.1
 tqdm==4.66.2
 Markdown==3.5.2
 markdown-include==0.8.1
```

