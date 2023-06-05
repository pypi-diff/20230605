# Comparing `tmp/steam-sdk-2023.6.7.tar.gz` & `tmp/steam-sdk-2023.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam-sdk-2023.6.7.tar", last modified: Mon Jun  5 09:03:29 2023, max compression
+gzip compressed data, was "dist\steam-sdk-2023.6.8.tar", last modified: Mon Jun  5 09:48:41 2023, max compression
```

## Comparing `steam-sdk-2023.6.7.tar` & `steam-sdk-2023.6.8.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.886431 steam-sdk-2023.6.7/
--rw-rw-rw-   0        0        0      122 2023-03-15 09:29:53.000000 steam-sdk-2023.6.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1550 2023-06-05 09:03:29.886431 steam-sdk-2023.6.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-05 09:03:29.886431 steam-sdk-2023.6.7/setup.cfg
--rw-rw-rw-   0        0        0      797 2023-06-05 09:02:36.000000 steam-sdk-2023.6.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.543542 steam-sdk-2023.6.7/steam_sdk/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.557784 steam-sdk-2023.6.7/steam_sdk/analyses/
--rw-rw-rw-   0        0        0   125975 2023-06-05 09:01:13.000000 steam-sdk-2023.6.7/steam_sdk/analyses/AnalysisSTEAM.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.559784 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.561784 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    23368 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.578537 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0    16757 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
--rw-rw-rw-   0        0        0     2800 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
--rw-rw-rw-   0        0        0     6828 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
--rw-rw-rw-   0        0        0    95412 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
--rw-rw-rw-   0        0        0     2652 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
--rw-rw-rw-   0        0        0     2341 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.581674 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    22374 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.590792 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4527 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     2921 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.593792 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
--rw-rw-rw-   0        0        0    29433 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.601911 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4704 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     4852 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.605912 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/custom_function_test_1/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
--rw-rw-rw-   0        0        0     1307 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.627184 steam-sdk-2023.6.7/steam_sdk/builders/
--rw-rw-rw-   0        0        0    12924 2023-05-12 15:08:26.000000 steam-sdk-2023.6.7/steam_sdk/builders/BuilderFiQuS.py
--rw-rw-rw-   0        0        0   162736 2023-05-25 11:58:42.000000 steam-sdk-2023.6.7/steam_sdk/builders/BuilderLEDET.py
--rw-rw-rw-   0        0        0    35640 2023-06-05 07:40:24.000000 steam-sdk-2023.6.7/steam_sdk/builders/BuilderModel.py
--rw-rw-rw-   0        0        0    12686 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/builders/BuilderProteCCT.py
--rw-rw-rw-   0        0        0     6749 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/builders/BuilderPyBBQ.py
--rw-rw-rw-   0        0        0    12076 2023-05-10 14:13:23.000000 steam-sdk-2023.6.7/steam_sdk/builders/BuilderSIGMA.py
--rw-rw-rw-   0        0        0    11689 2023-01-18 15:24:33.000000 steam-sdk-2023.6.7/steam_sdk/builders/SelfMutualInductanceCalculation.py
--rw-rw-rw-   0        0        0     7941 2022-12-19 08:13:58.000000 steam-sdk-2023.6.7/steam_sdk/builders/Solenoids.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/builders/__init__.py
--rw-rw-rw-   0        0        0     8352 2023-03-15 09:29:53.000000 steam-sdk-2023.6.7/steam_sdk/builders/geometricFunctions.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.629304 steam-sdk-2023.6.7/steam_sdk/configs/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.631306 steam-sdk-2023.6.7/steam_sdk/configs/plotters/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/configs/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.638436 steam-sdk-2023.6.7/steam_sdk/configs/tools_defaults/
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.650570 steam-sdk-2023.6.7/steam_sdk/configs/tools_defaults/LEDET/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/configs/tools_defaults/LEDET/__init__.py
--rw-rw-rw-   0        0        0    32991 2023-05-25 11:58:42.000000 steam-sdk-2023.6.7/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
--rw-rw-rw-   0        0        0     1426 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/configs/tools_defaults/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.655570 steam-sdk-2023.6.7/steam_sdk/cosims/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/cosims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.702265 steam-sdk-2023.6.7/steam_sdk/data/
--rw-rw-rw-   0        0        0    10200 2023-05-12 13:31:31.000000 steam-sdk-2023.6.7/steam_sdk/data/DataAnalysis.py
--rw-rw-rw-   0        0        0     7983 2023-05-22 11:27:05.000000 steam-sdk-2023.6.7/steam_sdk/data/DataConductor.py
--rw-rw-rw-   0        0        0     3281 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/data/DataDakota.py
--rw-rw-rw-   0        0        0     2865 2023-04-24 12:48:33.000000 steam-sdk-2023.6.7/steam_sdk/data/DataEventCircuit.py
--rw-rw-rw-   0        0        0     4193 2023-05-09 14:50:49.000000 steam-sdk-2023.6.7/steam_sdk/data/DataEventMagnet.py
--rw-rw-rw-   0        0        0    12762 2023-05-12 15:08:26.000000 steam-sdk-2023.6.7/steam_sdk/data/DataFiQuS.py
--rw-rw-rw-   0        0        0    10823 2023-05-25 11:58:42.000000 steam-sdk-2023.6.7/steam_sdk/data/DataLEDET.py
--rw-rw-rw-   0        0        0     4314 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/data/DataModelCircuit.py
--rw-rw-rw-   0        0        0     5869 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/data/DataModelConductor.py
--rw-rw-rw-   0        0        0    35376 2023-05-25 11:58:27.000000 steam-sdk-2023.6.7/steam_sdk/data/DataModelMagnet.py
--rw-rw-rw-   0        0        0     2636 2023-05-09 14:50:49.000000 steam-sdk-2023.6.7/steam_sdk/data/DataParsimConductor.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/data/DataParsims.py
--rw-rw-rw-   0        0        0     1995 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/data/DataProteCCT.py
--rw-rw-rw-   0        0        0     2105 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/data/DataPyBBQ.py
--rw-rw-rw-   0        0        0     8068 2023-05-25 11:58:27.000000 steam-sdk-2023.6.7/steam_sdk/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     6791 2023-05-09 14:51:04.000000 steam-sdk-2023.6.7/steam_sdk/data/DataSIGMA.py
--rw-rw-rw-   0        0        0     1650 2023-03-15 09:29:53.000000 steam-sdk-2023.6.7/steam_sdk/data/DataSettings.py
--rw-rw-rw-   0        0        0     3204 2023-01-11 12:50:11.000000 steam-sdk-2023.6.7/steam_sdk/data/DataSignal.py
--rw-rw-rw-   0        0        0    23052 2023-05-25 11:58:42.000000 steam-sdk-2023.6.7/steam_sdk/data/DictionaryLEDET.py
--rw-rw-rw-   0        0        0     4482 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/data/DictionaryProteCCT.py
--rw-rw-rw-   0        0        0     2902 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/data/DictionaryPyBBQ.py
--rw-rw-rw-   0        0        0    27819 2023-05-25 11:58:42.000000 steam-sdk-2023.6.7/steam_sdk/data/TemplateLEDET.py
--rw-rw-rw-   0        0        0     7903 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/data/TemplateProteCCT.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.725517 steam-sdk-2023.6.7/steam_sdk/drivers/
--rw-rw-rw-   0        0        0     3151 2022-12-19 08:13:58.000000 steam-sdk-2023.6.7/steam_sdk/drivers/DriverAnalysis.py
--rw-rw-rw-   0        0        0     2711 2022-12-19 08:13:58.000000 steam-sdk-2023.6.7/steam_sdk/drivers/DriverDakota.py
--rw-rw-rw-   0        0        0     1299 2023-03-15 09:29:53.000000 steam-sdk-2023.6.7/steam_sdk/drivers/DriverFiQuS.py
--rw-rw-rw-   0        0        0     3482 2022-12-19 08:13:58.000000 steam-sdk-2023.6.7/steam_sdk/drivers/DriverLEDET.py
--rw-rw-rw-   0        0        0     1924 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/drivers/DriverPSPICE.py
--rw-rw-rw-   0        0        0     2062 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/drivers/DriverProteCCT.py
--rw-rw-rw-   0        0        0     2219 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/drivers/DriverPyBBQ.py
--rw-rw-rw-   0        0        0     4959 2023-06-05 08:15:32.000000 steam-sdk-2023.6.7/steam_sdk/drivers/DriverSIGMA.py
--rw-rw-rw-   0        0        0     1932 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/drivers/DriverXYCE.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/drivers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.780583 steam-sdk-2023.6.7/steam_sdk/parsers/
--rw-rw-rw-   0        0        0     4984 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/parsers/CSD_Reader.py
--rw-rw-rw-   0        0        0      317 2023-03-29 12:41:10.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserCOMSOLToTxt.py
--rw-rw-rw-   0        0        0     2290 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserCond2d.py
--rw-rw-rw-   0        0        0     1081 2023-05-25 11:58:42.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserCsd.py
--rw-rw-rw-   0        0        0     6220 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserCsv.py
--rw-rw-rw-   0        0        0     1650 2023-01-13 08:06:15.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserDakota.py
--rw-rw-rw-   0        0        0     1030 2023-03-15 09:29:53.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserDatToCsv.py
--rw-rw-rw-   0        0        0     8536 2023-03-15 09:29:53.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserExcel.py
--rw-rw-rw-   0        0        0     2287 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserFiQuS.py
--rw-rw-rw-   0        0        0    48055 2023-05-25 11:58:42.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserLEDET.py
--rw-rw-rw-   0        0        0    12436 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserMap2d.py
--rw-rw-rw-   0        0        0    10920 2023-05-12 13:31:31.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserMat.py
--rw-rw-rw-   0        0        0    63401 2023-06-01 14:44:35.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserPSPICE.py
--rw-rw-rw-   0        0        0     4780 2023-03-15 09:29:53.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserPdf.py
--rw-rw-rw-   0        0        0     6838 2023-03-15 09:29:53.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserProteCCT.py
--rw-rw-rw-   0        0        0     2942 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserProtePyBBQ.py
--rw-rw-rw-   0        0        0   109575 2023-06-05 08:54:23.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0     1928 2023-05-09 14:51:03.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserSIGMA.py
--rw-rw-rw-   0        0        0    11707 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserTdms.py
--rw-rw-rw-   0        0        0    55281 2023-03-15 09:29:53.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserXYCE.py
--rw-rw-rw-   0        0        0     4088 2023-03-15 09:29:53.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserYAML.py
--rw-rw-rw-   0        0        0      975 2023-06-02 08:04:34.000000 steam-sdk-2023.6.7/steam_sdk/parsers/ParserYamlToRoxie.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/parsers/__init__.py
--rw-rw-rw-   0        0        0        2 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/parsers/dict_to_in.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.796709 steam-sdk-2023.6.7/steam_sdk/parsims/
--rw-rw-rw-   0        0        0    61782 2023-05-23 14:30:59.000000 steam-sdk-2023.6.7/steam_sdk/parsims/ParsimConductor.py
--rw-rw-rw-   0        0        0      916 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/parsims/ParsimDakota.py
--rw-rw-rw-   0        0        0    72533 2023-05-17 07:23:09.000000 steam-sdk-2023.6.7/steam_sdk/parsims/ParsimEventCircuit.py
--rw-rw-rw-   0        0        0    48206 2023-05-25 08:00:49.000000 steam-sdk-2023.6.7/steam_sdk/parsims/ParsimEventMagnet.py
--rw-rw-rw-   0        0        0     1972 2023-01-25 14:04:47.000000 steam-sdk-2023.6.7/steam_sdk/parsims/ParsimSweep.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/parsims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.807308 steam-sdk-2023.6.7/steam_sdk/plotters/
--rw-rw-rw-   0        0        0     8053 2023-05-12 13:31:31.000000 steam-sdk-2023.6.7/steam_sdk/plotters/PlotterAnalysis.py
--rw-rw-rw-   0        0        0    20392 2023-06-05 08:17:35.000000 steam-sdk-2023.6.7/steam_sdk/plotters/PlotterMap2d.py
--rw-rw-rw-   0        0        0    39596 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/plotters/PlotterModel.py
--rw-rw-rw-   0        0        0    22987 2022-12-19 08:13:58.000000 steam-sdk-2023.6.7/steam_sdk/plotters/PlotterParametric.py
--rw-rw-rw-   0        0        0     8863 2023-05-25 11:58:27.000000 steam-sdk-2023.6.7/steam_sdk/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.811432 steam-sdk-2023.6.7/steam_sdk/postprocs/
--rw-rw-rw-   0        0        0     5564 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/postprocs/PostprocsMetrics.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/postprocs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.871432 steam-sdk-2023.6.7/steam_sdk/utils/
--rw-rw-rw-   0        0        0     2679 2023-03-15 09:29:53.000000 steam-sdk-2023.6.7/steam_sdk/utils/MTF_reading_functions.py
--rw-rw-rw-   0        0        0    14942 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/utils/ModifyModelData.py
--rw-rw-rw-   0        0        0     4762 2023-06-02 08:04:34.000000 steam-sdk-2023.6.7/steam_sdk/utils/ModifyModelDataMagnet.py
--rw-rw-rw-   0        0        0     2745 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/utils/ModifyModelDataconductor.py
--rw-rw-rw-   0        0        0      313 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/utils/NumpyEncoder.py
--rw-rw-rw-   0        0        0     3190 2023-06-05 08:54:23.000000 steam-sdk-2023.6.7/steam_sdk/utils/ParserRoxieHelpers.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0      686 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/utils/clean_NaN_from_signal.py
--rw-rw-rw-   0        0        0     3837 2023-03-15 09:29:53.000000 steam-sdk-2023.6.7/steam_sdk/utils/compare_two_parameters.py
--rw-rw-rw-   0        0        0      590 2023-05-09 14:50:57.000000 steam-sdk-2023.6.7/steam_sdk/utils/create_coordinate_file_SIGMA.py
--rw-rw-rw-   0        0        0     1279 2023-04-24 12:48:33.000000 steam-sdk-2023.6.7/steam_sdk/utils/get_attribute_type.py
--rw-rw-rw-   0        0        0      167 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/utils/isNaN.py
--rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/utils/make_folder_if_not_existing.py
--rw-rw-rw-   0        0        0     4512 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/utils/misc.py
--rw-rw-rw-   0        0        0     1592 2023-04-24 12:48:33.000000 steam-sdk-2023.6.7/steam_sdk/utils/parse_str_to_list.py
--rw-rw-rw-   0        0        0      388 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/utils/rgetattr.py
--rw-rw-rw-   0        0        0      460 2023-01-11 12:50:11.000000 steam-sdk-2023.6.7/steam_sdk/utils/rhasattr.py
--rw-rw-rw-   0        0        0      383 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/utils/sgetattr.py
--rw-rw-rw-   0        0        0      863 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/utils/tic_toc.py
--rw-rw-rw-   0        0        0      168 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/utils/unique.py
--rw-rw-rw-   0        0        0     7005 2023-05-11 09:21:50.000000 steam-sdk-2023.6.7/steam_sdk/utils/utils_PC.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.878431 steam-sdk-2023.6.7/steam_sdk/viewers/
--rw-rw-rw-   0        0        0    35919 2023-03-23 12:53:02.000000 steam-sdk-2023.6.7/steam_sdk/viewers/Viewer.py
--rw-rw-rw-   0        0        0     6127 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/viewers/ViewerMeas.py
--rw-rw-rw-   0        0        0     1667 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/viewers/ViewerSim.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/viewers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.881433 steam-sdk-2023.6.7/steam_sdk/wrappers/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.7/steam_sdk/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.882433 steam-sdk-2023.6.7/steam_sdk/wrappers/java/
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.883432 steam-sdk-2023.6.7/steam_sdk/wrappers/java/SING/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.6.7/steam_sdk/wrappers/java/SING/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.884432 steam-sdk-2023.6.7/steam_sdk/wrappers/java/SING/jars/
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.6.7/steam_sdk/wrappers/java/SING/jars/__init__.py
--rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.6.7/steam_sdk/wrappers/java/__init__.py
--rw-rw-rw-   0        0        0     1834 2022-11-02 10:29:43.000000 steam-sdk-2023.6.7/steam_sdk/wrappers/wrapper_yaml.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:03:29.552665 steam-sdk-2023.6.7/steam_sdk.egg-info/
--rw-rw-rw-   0        0        0     1550 2023-06-05 09:03:26.000000 steam-sdk-2023.6.7/steam_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6763 2023-06-05 09:03:26.000000 steam-sdk-2023.6.7/steam_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 09:03:26.000000 steam-sdk-2023.6.7/steam_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1596 2023-06-05 09:03:26.000000 steam-sdk-2023.6.7/steam_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-05 09:03:26.000000 steam-sdk-2023.6.7/steam_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.359597 steam-sdk-2023.6.8/
+-rw-rw-rw-   0        0        0      122 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1550 2023-06-05 09:48:41.356598 steam-sdk-2023.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-05 09:48:41.359597 steam-sdk-2023.6.8/setup.cfg
+-rw-rw-rw-   0        0        0      797 2023-06-05 09:44:36.000000 steam-sdk-2023.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.102840 steam-sdk-2023.6.8/steam_sdk/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.111985 steam-sdk-2023.6.8/steam_sdk/analyses/
+-rw-rw-rw-   0        0        0   125975 2023-06-05 09:01:13.000000 steam-sdk-2023.6.8/steam_sdk/analyses/AnalysisSTEAM.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.114149 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.118149 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    23368 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.131271 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0    16757 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
+-rw-rw-rw-   0        0        0     2800 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
+-rw-rw-rw-   0        0        0     6828 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
+-rw-rw-rw-   0        0        0    95412 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
+-rw-rw-rw-   0        0        0     2652 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
+-rw-rw-rw-   0        0        0     2341 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.133389 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    22374 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.139389 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4527 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     2921 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.141389 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
+-rw-rw-rw-   0        0        0    29433 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.146735 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4704 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     4852 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.149736 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/custom_function_test_1/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
+-rw-rw-rw-   0        0        0     1307 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.169253 steam-sdk-2023.6.8/steam_sdk/builders/
+-rw-rw-rw-   0        0        0    12924 2023-05-12 15:08:26.000000 steam-sdk-2023.6.8/steam_sdk/builders/BuilderFiQuS.py
+-rw-rw-rw-   0        0        0   162736 2023-05-25 11:58:42.000000 steam-sdk-2023.6.8/steam_sdk/builders/BuilderLEDET.py
+-rw-rw-rw-   0        0        0    35640 2023-06-05 07:40:24.000000 steam-sdk-2023.6.8/steam_sdk/builders/BuilderModel.py
+-rw-rw-rw-   0        0        0    12686 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/builders/BuilderProteCCT.py
+-rw-rw-rw-   0        0        0     6749 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/builders/BuilderPyBBQ.py
+-rw-rw-rw-   0        0        0    12076 2023-05-10 14:13:23.000000 steam-sdk-2023.6.8/steam_sdk/builders/BuilderSIGMA.py
+-rw-rw-rw-   0        0        0    11689 2023-01-18 15:24:33.000000 steam-sdk-2023.6.8/steam_sdk/builders/SelfMutualInductanceCalculation.py
+-rw-rw-rw-   0        0        0     7941 2022-12-19 08:13:58.000000 steam-sdk-2023.6.8/steam_sdk/builders/Solenoids.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/builders/__init__.py
+-rw-rw-rw-   0        0        0     8352 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/builders/geometricFunctions.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.171252 steam-sdk-2023.6.8/steam_sdk/configs/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.172253 steam-sdk-2023.6.8/steam_sdk/configs/plotters/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/configs/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.174387 steam-sdk-2023.6.8/steam_sdk/configs/tools_defaults/
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.176387 steam-sdk-2023.6.8/steam_sdk/configs/tools_defaults/LEDET/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/configs/tools_defaults/LEDET/__init__.py
+-rw-rw-rw-   0        0        0    32991 2023-05-25 11:58:42.000000 steam-sdk-2023.6.8/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
+-rw-rw-rw-   0        0        0     1426 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/configs/tools_defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.178387 steam-sdk-2023.6.8/steam_sdk/cosims/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/cosims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.218748 steam-sdk-2023.6.8/steam_sdk/data/
+-rw-rw-rw-   0        0        0    10200 2023-05-12 13:31:31.000000 steam-sdk-2023.6.8/steam_sdk/data/DataAnalysis.py
+-rw-rw-rw-   0        0        0     7983 2023-05-22 11:27:05.000000 steam-sdk-2023.6.8/steam_sdk/data/DataConductor.py
+-rw-rw-rw-   0        0        0     3281 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/data/DataDakota.py
+-rw-rw-rw-   0        0        0     2865 2023-04-24 12:48:33.000000 steam-sdk-2023.6.8/steam_sdk/data/DataEventCircuit.py
+-rw-rw-rw-   0        0        0     4193 2023-05-09 14:50:49.000000 steam-sdk-2023.6.8/steam_sdk/data/DataEventMagnet.py
+-rw-rw-rw-   0        0        0    12762 2023-05-12 15:08:26.000000 steam-sdk-2023.6.8/steam_sdk/data/DataFiQuS.py
+-rw-rw-rw-   0        0        0    10823 2023-05-25 11:58:42.000000 steam-sdk-2023.6.8/steam_sdk/data/DataLEDET.py
+-rw-rw-rw-   0        0        0     4314 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/data/DataModelCircuit.py
+-rw-rw-rw-   0        0        0     5869 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/data/DataModelConductor.py
+-rw-rw-rw-   0        0        0    35376 2023-05-25 11:58:27.000000 steam-sdk-2023.6.8/steam_sdk/data/DataModelMagnet.py
+-rw-rw-rw-   0        0        0     2636 2023-05-09 14:50:49.000000 steam-sdk-2023.6.8/steam_sdk/data/DataParsimConductor.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/data/DataParsims.py
+-rw-rw-rw-   0        0        0     1995 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/data/DataProteCCT.py
+-rw-rw-rw-   0        0        0     2105 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/data/DataPyBBQ.py
+-rw-rw-rw-   0        0        0     8068 2023-05-25 11:58:27.000000 steam-sdk-2023.6.8/steam_sdk/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     6791 2023-05-09 14:51:04.000000 steam-sdk-2023.6.8/steam_sdk/data/DataSIGMA.py
+-rw-rw-rw-   0        0        0     1650 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/data/DataSettings.py
+-rw-rw-rw-   0        0        0     3204 2023-01-11 12:50:11.000000 steam-sdk-2023.6.8/steam_sdk/data/DataSignal.py
+-rw-rw-rw-   0        0        0    23052 2023-05-25 11:58:42.000000 steam-sdk-2023.6.8/steam_sdk/data/DictionaryLEDET.py
+-rw-rw-rw-   0        0        0     4482 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/data/DictionaryProteCCT.py
+-rw-rw-rw-   0        0        0     2902 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/data/DictionaryPyBBQ.py
+-rw-rw-rw-   0        0        0    27819 2023-05-25 11:58:42.000000 steam-sdk-2023.6.8/steam_sdk/data/TemplateLEDET.py
+-rw-rw-rw-   0        0        0     7903 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/data/TemplateProteCCT.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.235009 steam-sdk-2023.6.8/steam_sdk/drivers/
+-rw-rw-rw-   0        0        0     3151 2022-12-19 08:13:58.000000 steam-sdk-2023.6.8/steam_sdk/drivers/DriverAnalysis.py
+-rw-rw-rw-   0        0        0     2711 2022-12-19 08:13:58.000000 steam-sdk-2023.6.8/steam_sdk/drivers/DriverDakota.py
+-rw-rw-rw-   0        0        0     1299 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/drivers/DriverFiQuS.py
+-rw-rw-rw-   0        0        0     3482 2022-12-19 08:13:58.000000 steam-sdk-2023.6.8/steam_sdk/drivers/DriverLEDET.py
+-rw-rw-rw-   0        0        0     1924 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/drivers/DriverPSPICE.py
+-rw-rw-rw-   0        0        0     2062 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/drivers/DriverProteCCT.py
+-rw-rw-rw-   0        0        0     2219 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/drivers/DriverPyBBQ.py
+-rw-rw-rw-   0        0        0     4959 2023-06-05 08:15:32.000000 steam-sdk-2023.6.8/steam_sdk/drivers/DriverSIGMA.py
+-rw-rw-rw-   0        0        0     1932 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/drivers/DriverXYCE.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/drivers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.275081 steam-sdk-2023.6.8/steam_sdk/parsers/
+-rw-rw-rw-   0        0        0     4984 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/CSD_Reader.py
+-rw-rw-rw-   0        0        0      317 2023-03-29 12:41:10.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserCOMSOLToTxt.py
+-rw-rw-rw-   0        0        0     2290 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserCond2d.py
+-rw-rw-rw-   0        0        0     1081 2023-05-25 11:58:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserCsd.py
+-rw-rw-rw-   0        0        0     6220 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserCsv.py
+-rw-rw-rw-   0        0        0     1650 2023-01-13 08:06:15.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserDakota.py
+-rw-rw-rw-   0        0        0     1030 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserDatToCsv.py
+-rw-rw-rw-   0        0        0     8536 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserExcel.py
+-rw-rw-rw-   0        0        0     2287 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserFiQuS.py
+-rw-rw-rw-   0        0        0    48055 2023-05-25 11:58:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserLEDET.py
+-rw-rw-rw-   0        0        0    12436 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserMap2d.py
+-rw-rw-rw-   0        0        0    10920 2023-05-12 13:31:31.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserMat.py
+-rw-rw-rw-   0        0        0    63401 2023-06-01 14:44:35.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserPSPICE.py
+-rw-rw-rw-   0        0        0     4780 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserPdf.py
+-rw-rw-rw-   0        0        0     6838 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserProteCCT.py
+-rw-rw-rw-   0        0        0     2942 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserProtePyBBQ.py
+-rw-rw-rw-   0        0        0   109575 2023-06-05 08:54:23.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0     1928 2023-05-09 14:51:03.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserSIGMA.py
+-rw-rw-rw-   0        0        0    11707 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserTdms.py
+-rw-rw-rw-   0        0        0    55281 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserXYCE.py
+-rw-rw-rw-   0        0        0     4088 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserYAML.py
+-rw-rw-rw-   0        0        0      975 2023-06-02 08:04:34.000000 steam-sdk-2023.6.8/steam_sdk/parsers/ParserYamlToRoxie.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/__init__.py
+-rw-rw-rw-   0        0        0        2 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsers/dict_to_in.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.286223 steam-sdk-2023.6.8/steam_sdk/parsims/
+-rw-rw-rw-   0        0        0    61782 2023-05-23 14:30:59.000000 steam-sdk-2023.6.8/steam_sdk/parsims/ParsimConductor.py
+-rw-rw-rw-   0        0        0      916 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsims/ParsimDakota.py
+-rw-rw-rw-   0        0        0    72533 2023-05-17 07:23:09.000000 steam-sdk-2023.6.8/steam_sdk/parsims/ParsimEventCircuit.py
+-rw-rw-rw-   0        0        0    48206 2023-05-25 08:00:49.000000 steam-sdk-2023.6.8/steam_sdk/parsims/ParsimEventMagnet.py
+-rw-rw-rw-   0        0        0     1972 2023-01-25 14:04:47.000000 steam-sdk-2023.6.8/steam_sdk/parsims/ParsimSweep.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/parsims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.295355 steam-sdk-2023.6.8/steam_sdk/plotters/
+-rw-rw-rw-   0        0        0     8053 2023-05-12 13:31:31.000000 steam-sdk-2023.6.8/steam_sdk/plotters/PlotterAnalysis.py
+-rw-rw-rw-   0        0        0    20409 2023-06-05 09:18:18.000000 steam-sdk-2023.6.8/steam_sdk/plotters/PlotterMap2d.py
+-rw-rw-rw-   0        0        0    39596 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/plotters/PlotterModel.py
+-rw-rw-rw-   0        0        0    22987 2022-12-19 08:13:58.000000 steam-sdk-2023.6.8/steam_sdk/plotters/PlotterParametric.py
+-rw-rw-rw-   0        0        0     8863 2023-05-25 11:58:27.000000 steam-sdk-2023.6.8/steam_sdk/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.297355 steam-sdk-2023.6.8/steam_sdk/postprocs/
+-rw-rw-rw-   0        0        0     5564 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/postprocs/PostprocsMetrics.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/postprocs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.333167 steam-sdk-2023.6.8/steam_sdk/utils/
+-rw-rw-rw-   0        0        0     2679 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/utils/MTF_reading_functions.py
+-rw-rw-rw-   0        0        0    14942 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/ModifyModelData.py
+-rw-rw-rw-   0        0        0     4762 2023-06-02 08:04:34.000000 steam-sdk-2023.6.8/steam_sdk/utils/ModifyModelDataMagnet.py
+-rw-rw-rw-   0        0        0     2745 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/ModifyModelDataconductor.py
+-rw-rw-rw-   0        0        0      313 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/NumpyEncoder.py
+-rw-rw-rw-   0        0        0     3190 2023-06-05 08:54:23.000000 steam-sdk-2023.6.8/steam_sdk/utils/ParserRoxieHelpers.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0      686 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/clean_NaN_from_signal.py
+-rw-rw-rw-   0        0        0     3837 2023-03-15 09:29:53.000000 steam-sdk-2023.6.8/steam_sdk/utils/compare_two_parameters.py
+-rw-rw-rw-   0        0        0      590 2023-05-09 14:50:57.000000 steam-sdk-2023.6.8/steam_sdk/utils/create_coordinate_file_SIGMA.py
+-rw-rw-rw-   0        0        0     1279 2023-04-24 12:48:33.000000 steam-sdk-2023.6.8/steam_sdk/utils/get_attribute_type.py
+-rw-rw-rw-   0        0        0      167 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/isNaN.py
+-rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/make_folder_if_not_existing.py
+-rw-rw-rw-   0        0        0     4512 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/misc.py
+-rw-rw-rw-   0        0        0     1592 2023-04-24 12:48:33.000000 steam-sdk-2023.6.8/steam_sdk/utils/parse_str_to_list.py
+-rw-rw-rw-   0        0        0      388 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/rgetattr.py
+-rw-rw-rw-   0        0        0      460 2023-01-11 12:50:11.000000 steam-sdk-2023.6.8/steam_sdk/utils/rhasattr.py
+-rw-rw-rw-   0        0        0      383 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/sgetattr.py
+-rw-rw-rw-   0        0        0      863 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/tic_toc.py
+-rw-rw-rw-   0        0        0      168 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/utils/unique.py
+-rw-rw-rw-   0        0        0     7005 2023-05-11 09:21:50.000000 steam-sdk-2023.6.8/steam_sdk/utils/utils_PC.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.346467 steam-sdk-2023.6.8/steam_sdk/viewers/
+-rw-rw-rw-   0        0        0    35919 2023-03-23 12:53:02.000000 steam-sdk-2023.6.8/steam_sdk/viewers/Viewer.py
+-rw-rw-rw-   0        0        0     6127 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/viewers/ViewerMeas.py
+-rw-rw-rw-   0        0        0     1667 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/viewers/ViewerSim.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/viewers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.350467 steam-sdk-2023.6.8/steam_sdk/wrappers/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.6.8/steam_sdk/wrappers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.352467 steam-sdk-2023.6.8/steam_sdk/wrappers/java/
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.353599 steam-sdk-2023.6.8/steam_sdk/wrappers/java/SING/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.6.8/steam_sdk/wrappers/java/SING/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.354599 steam-sdk-2023.6.8/steam_sdk/wrappers/java/SING/jars/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.6.8/steam_sdk/wrappers/java/SING/jars/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.6.8/steam_sdk/wrappers/java/__init__.py
+-rw-rw-rw-   0        0        0     1834 2022-11-02 10:29:43.000000 steam-sdk-2023.6.8/steam_sdk/wrappers/wrapper_yaml.py
+drwxrwxrwx   0        0        0        0 2023-06-05 09:48:41.108985 steam-sdk-2023.6.8/steam_sdk.egg-info/
+-rw-rw-rw-   0        0        0     1550 2023-06-05 09:48:38.000000 steam-sdk-2023.6.8/steam_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6763 2023-06-05 09:48:38.000000 steam-sdk-2023.6.8/steam_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 09:48:38.000000 steam-sdk-2023.6.8/steam_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1596 2023-06-05 09:48:38.000000 steam-sdk-2023.6.8/steam_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-05 09:48:38.000000 steam-sdk-2023.6.8/steam_sdk.egg-info/top_level.txt
```

### Comparing `steam-sdk-2023.6.7/PKG-INFO` & `steam-sdk-2023.6.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2023.6.7
+Version: 2023.6.8
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,STEAM,SDK,API
+Keywords: API,CERN,STEAM,SDK
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
```

### Comparing `steam-sdk-2023.6.7/setup.py` & `steam-sdk-2023.6.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam-sdk',
-    version="2023.6.7",
+    version="2023.6.8",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Source code for APIs for STEAM tools.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_sdk",
     keywords={'STEAM', 'API', 'SDK', 'CERN'},
```

### Comparing `steam-sdk-2023.6.7/steam_sdk/analyses/AnalysisSTEAM.py` & `steam-sdk-2023.6.8/steam_sdk/analyses/AnalysisSTEAM.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py` & `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py` & `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py` & `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py` & `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py` & `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py` & `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py` & `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py` & `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py` & `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py` & `steam-sdk-2023.6.8/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/builders/BuilderFiQuS.py` & `steam-sdk-2023.6.8/steam_sdk/builders/BuilderFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/builders/BuilderLEDET.py` & `steam-sdk-2023.6.8/steam_sdk/builders/BuilderLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/builders/BuilderModel.py` & `steam-sdk-2023.6.8/steam_sdk/builders/BuilderModel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/builders/BuilderProteCCT.py` & `steam-sdk-2023.6.8/steam_sdk/builders/BuilderProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/builders/BuilderPyBBQ.py` & `steam-sdk-2023.6.8/steam_sdk/builders/BuilderPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/builders/BuilderSIGMA.py` & `steam-sdk-2023.6.8/steam_sdk/builders/BuilderSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/builders/SelfMutualInductanceCalculation.py` & `steam-sdk-2023.6.8/steam_sdk/builders/SelfMutualInductanceCalculation.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/builders/Solenoids.py` & `steam-sdk-2023.6.8/steam_sdk/builders/Solenoids.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/builders/geometricFunctions.py` & `steam-sdk-2023.6.8/steam_sdk/builders/geometricFunctions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx` & `steam-sdk-2023.6.8/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/configs/tools_defaults/ToolDefaultReader.py` & `steam-sdk-2023.6.8/steam_sdk/configs/tools_defaults/ToolDefaultReader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/DataAnalysis.py` & `steam-sdk-2023.6.8/steam_sdk/data/DataAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/DataConductor.py` & `steam-sdk-2023.6.8/steam_sdk/data/DataConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/DataDakota.py` & `steam-sdk-2023.6.8/steam_sdk/data/DataDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/DataEventCircuit.py` & `steam-sdk-2023.6.8/steam_sdk/data/DataEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/DataEventMagnet.py` & `steam-sdk-2023.6.8/steam_sdk/data/DataEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/DataFiQuS.py` & `steam-sdk-2023.6.8/steam_sdk/data/DataFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/DataLEDET.py` & `steam-sdk-2023.6.8/steam_sdk/data/DataLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/DataModelCircuit.py` & `steam-sdk-2023.6.8/steam_sdk/data/DataModelCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/DataModelConductor.py` & `steam-sdk-2023.6.8/steam_sdk/data/DataModelConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/DataModelMagnet.py` & `steam-sdk-2023.6.8/steam_sdk/data/DataModelMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/DataParsimConductor.py` & `steam-sdk-2023.6.8/steam_sdk/data/DataParsimConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/DataProteCCT.py` & `steam-sdk-2023.6.8/steam_sdk/data/DataProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/DataPyBBQ.py` & `steam-sdk-2023.6.8/steam_sdk/data/DataPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/DataRoxieParser.py` & `steam-sdk-2023.6.8/steam_sdk/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/DataSIGMA.py` & `steam-sdk-2023.6.8/steam_sdk/data/DataSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/DataSettings.py` & `steam-sdk-2023.6.8/steam_sdk/data/DataSettings.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/DataSignal.py` & `steam-sdk-2023.6.8/steam_sdk/data/DataSignal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/DictionaryLEDET.py` & `steam-sdk-2023.6.8/steam_sdk/data/DictionaryLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/DictionaryProteCCT.py` & `steam-sdk-2023.6.8/steam_sdk/data/DictionaryProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/DictionaryPyBBQ.py` & `steam-sdk-2023.6.8/steam_sdk/data/DictionaryPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/TemplateLEDET.py` & `steam-sdk-2023.6.8/steam_sdk/data/TemplateLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/data/TemplateProteCCT.py` & `steam-sdk-2023.6.8/steam_sdk/data/TemplateProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/drivers/DriverAnalysis.py` & `steam-sdk-2023.6.8/steam_sdk/drivers/DriverAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/drivers/DriverDakota.py` & `steam-sdk-2023.6.8/steam_sdk/drivers/DriverDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/drivers/DriverFiQuS.py` & `steam-sdk-2023.6.8/steam_sdk/drivers/DriverFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/drivers/DriverLEDET.py` & `steam-sdk-2023.6.8/steam_sdk/drivers/DriverLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/drivers/DriverPSPICE.py` & `steam-sdk-2023.6.8/steam_sdk/drivers/DriverPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/drivers/DriverProteCCT.py` & `steam-sdk-2023.6.8/steam_sdk/drivers/DriverProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/drivers/DriverPyBBQ.py` & `steam-sdk-2023.6.8/steam_sdk/drivers/DriverPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/drivers/DriverSIGMA.py` & `steam-sdk-2023.6.8/steam_sdk/drivers/DriverSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/drivers/DriverXYCE.py` & `steam-sdk-2023.6.8/steam_sdk/drivers/DriverXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/CSD_Reader.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/CSD_Reader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/ParserCond2d.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/ParserCond2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/ParserCsd.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/ParserCsd.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/ParserCsv.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/ParserCsv.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/ParserDakota.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/ParserDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/ParserDatToCsv.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/ParserDatToCsv.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/ParserExcel.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/ParserExcel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/ParserFiQuS.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/ParserFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/ParserLEDET.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/ParserLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/ParserMap2d.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/ParserMap2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/ParserMat.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/ParserMat.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/ParserPSPICE.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/ParserPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/ParserPdf.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/ParserPdf.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/ParserProteCCT.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/ParserProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/ParserProtePyBBQ.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/ParserProtePyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/ParserRoxie.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/ParserRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/ParserSIGMA.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/ParserSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/ParserTdms.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/ParserTdms.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/ParserXYCE.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/ParserXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/ParserYAML.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/ParserYAML.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsers/ParserYamlToRoxie.py` & `steam-sdk-2023.6.8/steam_sdk/parsers/ParserYamlToRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsims/ParsimConductor.py` & `steam-sdk-2023.6.8/steam_sdk/parsims/ParsimConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsims/ParsimDakota.py` & `steam-sdk-2023.6.8/steam_sdk/parsims/ParsimDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsims/ParsimEventCircuit.py` & `steam-sdk-2023.6.8/steam_sdk/parsims/ParsimEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsims/ParsimEventMagnet.py` & `steam-sdk-2023.6.8/steam_sdk/parsims/ParsimEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/parsims/ParsimSweep.py` & `steam-sdk-2023.6.8/steam_sdk/parsims/ParsimSweep.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/plotters/PlotterAnalysis.py` & `steam-sdk-2023.6.8/steam_sdk/plotters/PlotterAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/plotters/PlotterMap2d.py` & `steam-sdk-2023.6.8/steam_sdk/plotters/PlotterMap2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,14 +395,15 @@
         fig1.savefig(os.path.join(working_dir_path, "plot_Bmod.png"))
         fig2.savefig(os.path.join(working_dir_path,"plot_B_mod_error.png"))
         fig3.savefig(os.path.join(working_dir_path,"plot_Bx_By.png"))
         fig4.savefig(os.path.join(working_dir_path,"plot_relative_error_x_y.png"))
         fig5.savefig(os.path.join(working_dir_path,"plot_difference_Bx_By.png"))
 
     #displayWaitAndClose(waitTimeBeforeMessage=.1, waitTimeAfterMessage=10)
+    plt.close()
 
 def plot_roxie_coil(roxie_data):
     xPos = []
     yPos = []
     xBarePos = []
     yBarePos = []
     iPos = []
```

### Comparing `steam-sdk-2023.6.7/steam_sdk/plotters/PlotterModel.py` & `steam-sdk-2023.6.8/steam_sdk/plotters/PlotterModel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/plotters/PlotterParametric.py` & `steam-sdk-2023.6.8/steam_sdk/plotters/PlotterParametric.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/plotters/PlotterRoxie.py` & `steam-sdk-2023.6.8/steam_sdk/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/postprocs/PostprocsMetrics.py` & `steam-sdk-2023.6.8/steam_sdk/postprocs/PostprocsMetrics.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/utils/MTF_reading_functions.py` & `steam-sdk-2023.6.8/steam_sdk/utils/MTF_reading_functions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/utils/ModifyModelData.py` & `steam-sdk-2023.6.8/steam_sdk/utils/ModifyModelData.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/utils/ModifyModelDataMagnet.py` & `steam-sdk-2023.6.8/steam_sdk/utils/ModifyModelDataMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/utils/ModifyModelDataconductor.py` & `steam-sdk-2023.6.8/steam_sdk/utils/ModifyModelDataconductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/utils/ParserRoxieHelpers.py` & `steam-sdk-2023.6.8/steam_sdk/utils/ParserRoxieHelpers.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/utils/clean_NaN_from_signal.py` & `steam-sdk-2023.6.8/steam_sdk/utils/clean_NaN_from_signal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/utils/compare_two_parameters.py` & `steam-sdk-2023.6.8/steam_sdk/utils/compare_two_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/utils/create_coordinate_file_SIGMA.py` & `steam-sdk-2023.6.8/steam_sdk/utils/create_coordinate_file_SIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/utils/get_attribute_type.py` & `steam-sdk-2023.6.8/steam_sdk/utils/get_attribute_type.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/utils/misc.py` & `steam-sdk-2023.6.8/steam_sdk/utils/misc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/utils/parse_str_to_list.py` & `steam-sdk-2023.6.8/steam_sdk/utils/parse_str_to_list.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/utils/tic_toc.py` & `steam-sdk-2023.6.8/steam_sdk/utils/tic_toc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/utils/utils_PC.py` & `steam-sdk-2023.6.8/steam_sdk/utils/utils_PC.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/viewers/Viewer.py` & `steam-sdk-2023.6.8/steam_sdk/viewers/Viewer.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/viewers/ViewerMeas.py` & `steam-sdk-2023.6.8/steam_sdk/viewers/ViewerMeas.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/viewers/ViewerSim.py` & `steam-sdk-2023.6.8/steam_sdk/viewers/ViewerSim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk/wrappers/wrapper_yaml.py` & `steam-sdk-2023.6.8/steam_sdk/wrappers/wrapper_yaml.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk.egg-info/PKG-INFO` & `steam-sdk-2023.6.8/steam_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2023.6.7
+Version: 2023.6.8
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,STEAM,SDK,API
+Keywords: API,CERN,STEAM,SDK
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
```

### Comparing `steam-sdk-2023.6.7/steam_sdk.egg-info/SOURCES.txt` & `steam-sdk-2023.6.8/steam_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.6.7/steam_sdk.egg-info/requires.txt` & `steam-sdk-2023.6.8/steam_sdk.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -82,8 +82,8 @@
 tqdm==4.64.1
 traitlets==5.4.0
 typing_extensions==4.3.0
 urllib3==1.26.12
 watchdog==2.1.9
 wcwidth==0.2.5
 zipp==3.8.1
-steam-pysigma==2023.6.2
+steam-pysigma==2023.6.3
```

