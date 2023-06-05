# Comparing `tmp/pyRDDLGym-1.0.5.tar.gz` & `tmp/pyRDDLGym-1.0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyRDDLGym-1.0.5.tar", last modified: Sun May 21 18:31:13 2023, max compression
+gzip compressed data, was "pyRDDLGym-1.0.55.tar", last modified: Mon Jun  5 13:15:41 2023, max compression
```

## Comparing `pyRDDLGym-1.0.5.tar` & `pyRDDLGym-1.0.55.tar`

### file list

```diff
@@ -1,242 +1,271 @@
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.433329 pyRDDLGym-1.0.5/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1264 2022-12-08 22:55:23.000000 pyRDDLGym-1.0.5/LICENSE.MD
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       87 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/MANIFEST.in
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      911 2023-05-21 18:31:13.433129 pyRDDLGym-1.0.5/PKG-INFO
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     8094 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/README.md
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.389524 pyRDDLGym-1.0.5/pyRDDLGym/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.390646 pyRDDLGym-1.0.5/pyRDDLGym/Core/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.393009 pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     8347 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLDecompiler.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    11135 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLLevelAnalysis.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    17227 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLLiftedModel.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    18950 2023-04-06 22:49:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLModel.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    47583 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLObjectsTracer.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5216 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLValueInitializer.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.393444 pyRDDLGym-1.0.5/pyRDDLGym/Core/Debug/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2168 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Debug/Logger.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-01-27 22:40:35.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Debug/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.393927 pyRDDLGym-1.0.5/pyRDDLGym/Core/Env/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5797 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Env/RDDLConstraints.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    11884 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Env/RDDLEnv.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Env/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.394569 pyRDDLGym-1.0.5/pyRDDLGym/Core/ErrorHandling/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1378 2023-04-20 23:10:37.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/ErrorHandling/RDDLException.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/ErrorHandling/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.395017 pyRDDLGym-1.0.5/pyRDDLGym/Core/Grounder/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    27395 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Grounder/RDDLGrounder.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Grounder/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.397465 pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    20186 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxParameterTuning.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    53645 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlanner.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    11956 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlannerUCT.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    69234 2023-04-07 15:03:00.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLCompiler.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    18972 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLLogic.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    12925 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLModelError.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     6948 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLSimulator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.401663 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1620 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/RDDLReader.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        1 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1146 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/cpf.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    10193 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/domain.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     7819 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/expr.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1293 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/instance.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1221 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/nonfluents.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    38755 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/parser.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)   123443 2023-02-22 22:24:57.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/parsetab.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3242 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/pvariable.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    10773 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/rddl.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      801 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/utils.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.402131 pyRDDLGym-1.0.5/pyRDDLGym/Core/Simulator/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    49061 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Simulator/RDDLSimulator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/Simulator/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/Core/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.402978 pyRDDLGym-1.0.5/pyRDDLGym/Examples/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.383566 pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.403748 pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Continuous/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      238 2023-05-21 18:21:26.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Continuous/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3419 2023-03-21 16:55:28.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Continuous/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      945 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Continuous/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.404717 pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Discrete/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      256 2023-05-21 18:21:26.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Discrete/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3510 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Discrete/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      928 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Discrete/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.405762 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Elevators/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      218 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Elevators/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    10524 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Elevators/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1408 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Elevators/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1628 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Elevators/instance1.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5211 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/ExampleManager.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.406842 pyRDDLGym-1.0.5/pyRDDLGym/Examples/HVAC/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      161 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/HVAC/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5768 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/HVAC/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      364 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/HVAC/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      389 2023-04-07 02:46:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/HVAC/instance1.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      455 2023-04-07 02:46:06.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/HVAC/instance2.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3652 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerator.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.408545 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2687 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/HVACInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1630 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/MarsRoverInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3058 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/MountainCarInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3264 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/PowerGenInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3594 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/RaceCarInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4086 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/RecSimInstanceGen.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2285 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/ReservoirInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1819 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/UAVInstanceGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.408999 pyRDDLGym-1.0.5/pyRDDLGym/Examples/MarsRover/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      210 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/MarsRover/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4495 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/MarsRover/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1411 2023-03-30 14:37:35.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/MarsRover/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.410020 pyRDDLGym-1.0.5/pyRDDLGym/Examples/MountainCar/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      219 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/MountainCar/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4408 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/MountainCar/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2551 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/MountainCar/domain_old.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    14883 2023-04-16 21:02:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/MountainCar/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      960 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/MountainCar/instance0_old.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.384261 pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.410691 pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      101 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2890 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      655 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.411286 pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      105 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1401 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      193 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.384514 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.411853 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Continuous/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      239 2023-05-21 18:21:26.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Continuous/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4403 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Continuous/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1610 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Continuous/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.412541 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Discrete/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      164 2023-05-21 18:21:26.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Discrete/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3383 2023-02-27 22:52:10.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Discrete/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1630 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Discrete/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.413123 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PropDBN/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       87 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PropDBN/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2283 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PropDBN/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      268 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/PropDBN/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.413926 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RaceCar/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      176 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RaceCar/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4995 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RaceCar/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     9478 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RaceCar/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      995 2023-04-07 02:51:57.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RaceCar/instance1.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.415033 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RecSim/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      189 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RecSim/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4153 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RecSim/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1327 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RecSim/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    15525 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RecSim/instance1.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    85747 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/RecSim/instance2.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.385035 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.416040 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Continuous/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      237 2023-05-21 18:21:26.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Continuous/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4435 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Continuous/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      391 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Continuous/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      710 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Continuous/instance1.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.416776 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Discrete/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      162 2023-05-21 18:21:26.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Discrete/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4544 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Discrete/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      390 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Discrete/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      709 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Discrete/instance1.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.417387 pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChain/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      118 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChain/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3550 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChain/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      635 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChain/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.417930 pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChainNet/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      129 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChainNet/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4622 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChainNet/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1747 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChainNet/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.419175 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.385415 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Deprecated/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.420256 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    20730 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     7653 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     9656 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance1.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    24387 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance2.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.420482 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Experiments/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     6386 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Experiments/webster_exp_equal_split.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       91 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    16438 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4951 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    25150 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/instance1.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    23064 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/netgen.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.385822 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.421402 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Continuous/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      241 2023-05-21 18:21:26.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Continuous/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5492 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Continuous/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1053 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Continuous/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1063 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Continuous/instance1.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.422188 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Discrete/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      185 2023-05-21 18:21:26.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Discrete/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5440 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Discrete/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      831 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Discrete/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.422945 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Mixed/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      179 2023-05-21 18:21:26.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Mixed/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5491 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Mixed/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      831 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Mixed/instance0.rddl
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.423667 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Wildfire/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      121 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Wildfire/domain.info
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4280 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Wildfire/domain.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1398 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/Wildfire/instance0.rddl
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Examples/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2603 2023-04-20 22:35:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/GymExample.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5584 2023-04-20 22:35:43.000000 pyRDDLGym-1.0.5/pyRDDLGym/JaxExample.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4439 2023-04-20 22:35:43.000000 pyRDDLGym-1.0.5/pyRDDLGym/JaxLossPlotExample.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1704 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/JaxTuningExample.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.424083 pyRDDLGym-1.0.5/pyRDDLGym/Planner/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3989 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.5/pyRDDLGym/Planner/JaxConfigManager.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Planner/__init__.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.424709 pyRDDLGym-1.0.5/pyRDDLGym/Policies/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1340 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.5/pyRDDLGym/Policies/Agents.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     9818 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Policies/RDDLSimAgent.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/Policies/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      396 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/RDDLSimClientExample.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.428852 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2924 2023-01-23 22:29:35.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/CartPoleViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     7420 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/ChartViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5528 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/ColorViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     8708 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/ElevatorViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    12057 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/HVACViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     6278 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/MarsRoverViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4797 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/MountainCarViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     3950 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/MovieGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     8522 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/PowerGenViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2880 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/RacecarViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     7180 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/RecSimViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    11691 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/ReservoirViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      516 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/StateViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2767 2023-01-23 22:29:35.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/TextViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    20753 2023-03-02 18:32:16.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/TrafficViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     4754 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/UAVsViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5987 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/WildfireViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    20186 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/visualize_dbn.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.430115 pyRDDLGym-1.0.5/pyRDDLGym/XADD/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2383 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.5/pyRDDLGym/XADD/RDDLLevelAnalysisXADD.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    17224 2023-03-22 17:18:24.000000 pyRDDLGym-1.0.5/pyRDDLGym/XADD/RDDLModelXADD.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     6162 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.5/pyRDDLGym/XADD/RDDLSimulatorXADD.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       41 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.5/pyRDDLGym/XADD/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      111 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.5/pyRDDLGym/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      701 2022-12-29 01:36:27.000000 pyRDDLGym-1.0.5/pyRDDLGym/testDiscrete.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.432856 pyRDDLGym-1.0.5/pyRDDLGym/tests/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     7362 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/RDDLGenerator.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/__init__.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)    13792 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/_deprecated.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1265 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/testGymDrone.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1672 2022-10-24 03:39:07.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/testViz.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1267 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/test_basic.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      658 2023-03-22 00:25:03.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/test_dbn_vis.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     1055 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/test_termination.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2534 2023-03-22 00:25:03.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/test_xadd.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     5114 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/unit_test_mars_rover.py
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2782 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.5/pyRDDLGym/tests/unit_test_power_gen.py
-drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-05-21 18:31:13.390508 pyRDDLGym-1.0.5/pyRDDLGym.egg-info/
--rw-r--r--   0 ayaltaitler   (501) staff       (20)      911 2023-05-21 18:31:13.000000 pyRDDLGym-1.0.5/pyRDDLGym.egg-info/PKG-INFO
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     7891 2023-05-21 18:31:13.000000 pyRDDLGym-1.0.5/pyRDDLGym.egg-info/SOURCES.txt
--rw-r--r--   0 ayaltaitler   (501) staff       (20)        1 2023-05-21 18:31:13.000000 pyRDDLGym-1.0.5/pyRDDLGym.egg-info/dependency_links.txt
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       67 2023-05-21 18:31:13.000000 pyRDDLGym-1.0.5/pyRDDLGym.egg-info/requires.txt
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       10 2023-05-21 18:31:13.000000 pyRDDLGym-1.0.5/pyRDDLGym.egg-info/top_level.txt
--rw-r--r--   0 ayaltaitler   (501) staff       (20)       38 2023-05-21 18:31:13.433389 pyRDDLGym-1.0.5/setup.cfg
--rw-r--r--   0 ayaltaitler   (501) staff       (20)     2810 2023-05-21 18:26:33.000000 pyRDDLGym-1.0.5/setup.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.992559 pyRDDLGym-1.0.55/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1264 2022-12-08 22:55:23.000000 pyRDDLGym-1.0.55/LICENSE.MD
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       87 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/MANIFEST.in
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      912 2023-06-05 13:15:41.992269 pyRDDLGym-1.0.55/PKG-INFO
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     8094 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/README.md
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.934797 pyRDDLGym-1.0.55/pyRDDLGym/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.935867 pyRDDLGym-1.0.55/pyRDDLGym/Core/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.938687 pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     8347 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLDecompiler.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    11135 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLLevelAnalysis.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    17227 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLLiftedModel.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    18950 2023-04-06 22:49:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLModel.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    47583 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLObjectsTracer.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5216 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLValueInitializer.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.939254 pyRDDLGym-1.0.55/pyRDDLGym/Core/Debug/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2168 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Debug/Logger.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-01-27 22:40:35.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Debug/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.940372 pyRDDLGym-1.0.55/pyRDDLGym/Core/Env/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5797 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Env/RDDLConstraints.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    12772 2023-06-05 01:19:34.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Env/RDDLEnv.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      413 2023-06-05 01:19:34.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Env/RDDLEnvSeeder.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Env/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.941210 pyRDDLGym-1.0.55/pyRDDLGym/Core/ErrorHandling/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1378 2023-04-20 23:10:37.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/ErrorHandling/RDDLException.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/ErrorHandling/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.941636 pyRDDLGym-1.0.55/pyRDDLGym/Core/Grounder/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    27395 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Grounder/RDDLGrounder.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Grounder/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.944749 pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    29366 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxParameterTuning.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    53812 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlanner.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    11956 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlannerUCT.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    69234 2023-04-07 15:03:00.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLCompiler.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    18972 2023-05-21 18:09:07.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLLogic.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    12925 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLModelError.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     7027 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLSimulator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.948474 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1620 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/RDDLReader.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        1 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1146 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/cpf.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    10193 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/domain.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     7819 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/expr.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1293 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/instance.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1221 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/nonfluents.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    38755 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/parser.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)   123443 2023-02-22 22:24:57.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/parsetab.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3242 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/pvariable.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    10773 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/rddl.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      801 2022-11-16 01:54:24.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/utils.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.949199 pyRDDLGym-1.0.55/pyRDDLGym/Core/Simulator/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    49156 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Simulator/RDDLSimulator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/Simulator/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/Core/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.950142 pyRDDLGym-1.0.55/pyRDDLGym/Examples/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.929194 pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.950858 pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Continuous/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      238 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Continuous/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3419 2023-03-21 16:55:28.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Continuous/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      945 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Continuous/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.951675 pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Discrete/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      256 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Discrete/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3510 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Discrete/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      928 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Discrete/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.952721 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Elevators/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      218 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Elevators/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    10524 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Elevators/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1408 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Elevators/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1628 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Elevators/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5211 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/ExampleManager.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.954631 pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      161 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5768 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      364 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      389 2023-04-07 02:46:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      579 2023-05-25 19:49:15.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/instance1c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      455 2023-04-07 02:46:06.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/instance2.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      963 2023-05-25 19:56:55.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/instance3c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3744 2023-05-31 00:03:12.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/instance5c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3825 2023-05-29 22:41:23.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerator.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.956437 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2687 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/HVACInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1630 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/MarsRoverInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3058 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/MountainCarInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3264 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/PowerGenInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3594 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/RaceCarInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4075 2023-05-29 22:41:23.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/RecSimInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2285 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/ReservoirInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1819 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/UAVInstanceGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.957695 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      210 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4495 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1411 2023-03-30 14:37:35.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      751 2023-05-25 20:01:15.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/instance1c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2211 2023-05-25 20:04:24.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/instance3c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4363 2023-05-31 00:14:18.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/instance5c.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.959830 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      219 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4408 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2551 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/domain_old.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    14883 2023-04-16 21:02:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      960 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/instance0_old.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    15237 2023-05-25 20:08:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/instance1c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    15117 2023-06-05 01:35:32.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/instance3c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    15085 2023-05-31 00:17:03.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/instance5c.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.929876 pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.960562 pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      101 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2890 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      655 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.963374 pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      105 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1401 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      193 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.930128 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.964691 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      239 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4403 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1610 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      791 2023-05-25 20:06:43.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/instance1c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1380 2023-05-25 20:07:33.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/instance3c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2583 2023-05-31 00:14:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/instance5c.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.965391 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Discrete/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      164 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Discrete/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3383 2023-02-27 22:52:10.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Discrete/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1630 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Discrete/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.966051 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PropDBN/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       87 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PropDBN/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2283 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PropDBN/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      268 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/PropDBN/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.967761 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      176 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4995 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     9478 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      995 2023-04-07 02:51:57.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1245 2023-05-25 19:57:11.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/instance1c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2309 2023-05-25 19:59:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/instance3c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3347 2023-05-31 00:07:05.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/instance5c.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.969745 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      189 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4153 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1327 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    15525 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2051 2023-06-01 18:46:28.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance1c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    85747 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance2.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    16852 2023-06-01 18:49:08.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance3c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)   194658 2023-06-01 18:50:40.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance5c.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.930595 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.971450 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      237 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4435 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      391 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      710 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      721 2023-05-25 20:17:38.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/instance1c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2622 2023-05-25 20:19:22.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/instance3c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     8968 2023-05-31 00:28:29.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/instance5c.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.972236 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Discrete/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      162 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Discrete/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4544 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Discrete/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      390 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Discrete/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      709 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Discrete/instance1.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.972794 pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChain/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      118 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChain/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3550 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChain/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      635 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChain/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.973325 pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChainNet/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      129 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChainNet/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4622 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChainNet/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1747 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChainNet/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.974392 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.931002 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Deprecated/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.975403 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    20730 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     7653 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     9656 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    24387 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance2.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.975594 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Experiments/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     6386 2023-03-26 19:09:06.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Experiments/webster_exp_equal_split.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       91 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    16438 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4951 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    25150 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    23064 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/netgen.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.931405 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.977105 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      241 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5492 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1053 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1063 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/instance1.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      600 2023-05-25 20:00:05.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/instance1c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1094 2023-05-25 20:00:46.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/instance3c.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    10413 2023-05-31 00:10:12.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/instance5c.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.979144 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Discrete/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      185 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Discrete/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5440 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Discrete/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      831 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Discrete/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.979944 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Mixed/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      179 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Mixed/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5491 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Mixed/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      831 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Mixed/instance0.rddl
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.980680 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Wildfire/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      121 2023-03-12 16:41:04.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Wildfire/domain.info
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4280 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Wildfire/domain.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1398 2023-03-22 19:40:02.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/Wildfire/instance0.rddl
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Examples/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2655 2023-06-05 01:41:10.000000 pyRDDLGym-1.0.55/pyRDDLGym/GymExample.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     8336 2023-06-05 01:25:16.000000 pyRDDLGym-1.0.55/pyRDDLGym/InstGenExample.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5596 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/JaxExample.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4442 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/JaxLossPlotExample.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2533 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/JaxTuningExample.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.981210 pyRDDLGym-1.0.55/pyRDDLGym/Planner/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4346 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Planner/JaxConfigManager.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Planner/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.981951 pyRDDLGym-1.0.55/pyRDDLGym/Policies/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1381 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Policies/Agents.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     9818 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Policies/RDDLSimAgent.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/Policies/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      396 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/RDDLSimClientExample.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.986752 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2924 2023-01-23 22:29:35.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/CartPoleViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     7420 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/ChartViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5528 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/ColorViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     8708 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/ElevatorViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    12057 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/HVACViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     6278 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/MarsRoverViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4797 2023-04-07 15:12:54.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/MountainCarViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     3950 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/MovieGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     8522 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/PowerGenViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2880 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/RacecarViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     7196 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/RecSimViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    11706 2023-06-04 16:23:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/ReservoirViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      516 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/StateViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2767 2023-01-23 22:29:35.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/TextViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    20753 2023-03-02 18:32:16.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/TrafficViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     4754 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/UAVsViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5987 2023-02-23 16:31:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/WildfireViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    20186 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/visualize_dbn.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.988333 pyRDDLGym-1.0.55/pyRDDLGym/XADD/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2383 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.55/pyRDDLGym/XADD/RDDLLevelAnalysisXADD.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    17224 2023-03-22 17:18:24.000000 pyRDDLGym-1.0.55/pyRDDLGym/XADD/RDDLModelXADD.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     6162 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.55/pyRDDLGym/XADD/RDDLSimulatorXADD.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       41 2022-12-24 22:28:03.000000 pyRDDLGym-1.0.55/pyRDDLGym/XADD/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      111 2023-02-27 22:16:49.000000 pyRDDLGym-1.0.55/pyRDDLGym/__init__.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.991472 pyRDDLGym-1.0.55/pyRDDLGym/tests/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     7362 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/RDDLGenerator.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)    13792 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/_deprecated.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.991931 pyRDDLGym-1.0.55/pyRDDLGym/tests/seeding/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1735 2023-06-05 01:19:34.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/seeding/Seedtest.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 01:19:34.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/seeding/__init__.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      701 2023-05-24 20:09:20.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/testDiscrete.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1265 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/testGymDrone.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1672 2022-10-24 03:39:07.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/testViz.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1267 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/test_basic.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      658 2023-03-22 00:25:03.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/test_dbn_vis.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     1055 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/test_termination.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2534 2023-03-22 00:25:03.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/test_xadd.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     5114 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/unit_test_mars_rover.py
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2782 2022-10-24 04:41:01.000000 pyRDDLGym-1.0.55/pyRDDLGym/tests/unit_test_power_gen.py
+drwxr-xr-x   0 ayaltaitler   (501) staff       (20)        0 2023-06-05 13:15:41.935713 pyRDDLGym-1.0.55/pyRDDLGym.egg-info/
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)      912 2023-06-05 13:15:41.000000 pyRDDLGym-1.0.55/pyRDDLGym.egg-info/PKG-INFO
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     9173 2023-06-05 13:15:41.000000 pyRDDLGym-1.0.55/pyRDDLGym.egg-info/SOURCES.txt
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)        1 2023-06-05 13:15:41.000000 pyRDDLGym-1.0.55/pyRDDLGym.egg-info/dependency_links.txt
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       67 2023-06-05 13:15:41.000000 pyRDDLGym-1.0.55/pyRDDLGym.egg-info/requires.txt
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       10 2023-06-05 13:15:41.000000 pyRDDLGym-1.0.55/pyRDDLGym.egg-info/top_level.txt
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)       38 2023-06-05 13:15:41.992604 pyRDDLGym-1.0.55/setup.cfg
+-rw-r--r--   0 ayaltaitler   (501) staff       (20)     2811 2023-06-05 13:06:40.000000 pyRDDLGym-1.0.55/setup.py
```

### Comparing `pyRDDLGym-1.0.5/LICENSE.MD` & `pyRDDLGym-1.0.55/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/PKG-INFO` & `pyRDDLGym-1.0.55/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRDDLGym
-Version: 1.0.5
+Version: 1.0.55
 Summary: pyRDDLGym: RDDL automatic generation tool for OpenAI Gym
 Home-page: https://github.com/ataitler/pyRDDLGym
 Author: Ayal Taitler, Michael Gimelfarb, Scott Sanner, Jihwan Jeong, Sriram Gopalakrishnan, Martin Mladenov, jack liu
 Author-email: ataitler@gmail.com, mike.gimelfarb@mail.utoronto.ca, ssanner@mie.utoronto.ca, jhjeong@mie.utoronto.ca, sriram.gopalakrishnan@jpmchase.com, mmladenov@google.com, xiaotian.liu@mail.utoronto.ca
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pyRDDLGym-1.0.5/README.md` & `pyRDDLGym-1.0.55/README.md`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLDecompiler.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLDecompiler.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLLevelAnalysis.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLLevelAnalysis.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLLiftedModel.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLLiftedModel.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLModel.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLModel.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLObjectsTracer.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLObjectsTracer.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Compiler/RDDLValueInitializer.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Compiler/RDDLValueInitializer.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Debug/Logger.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Debug/Logger.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Env/RDDLConstraints.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Env/RDDLConstraints.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Env/RDDLEnv.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Env/RDDLEnv.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from pyRDDLGym.Core.ErrorHandling.RDDLException import RDDLInvalidNumberOfArgumentsError
 from pyRDDLGym.Core.ErrorHandling.RDDLException import RDDLTypeError, RDDLLogFolderError
 
 from pyRDDLGym.Core.Compiler.RDDLLiftedModel import RDDLLiftedModel
 from pyRDDLGym.Core.Debug.Logger import Logger, SimLogger
 from pyRDDLGym.Core.Env.RDDLConstraints import RDDLConstraints
+from pyRDDLGym.Core.Env.RDDLEnvSeeder import RDDLEnvSeeder
 from pyRDDLGym.Core.Parser.parser import RDDLParser
 from pyRDDLGym.Core.Parser.RDDLReader import RDDLReader
 from pyRDDLGym.Core.Simulator.RDDLSimulator import RDDLSimulator
 from pyRDDLGym.Visualizer.TextViz import TextVisualizer
 
 
 class RDDLEnv(gym.Env):
@@ -22,37 +23,45 @@
     def __init__(self, domain: str,
                  instance: str=None,
                  enforce_action_constraints: bool=False,
                  enforce_action_count_non_bool: bool=True,
                  debug: bool=False,
                  log: bool=False,
                  simlogname: str=None,
-                 backend: object=RDDLSimulator):
+                 backend: RDDLSimulator=RDDLSimulator,
+                 backend_kwargs: Dict={},
+                 seeds: list=None):
         '''Creates a new gym environment from the given RDDL domain + instance.
         
         :param domain: the RDDL domain
         :param instance: the RDDL instance
         :param enforce_action_constraints: whether to raise an exception if the
         action constraints are violated
         :param enforce_action_count_non_bool: whether to include non-bool actions
         in check that number of nondef actions don't exceed max-nondef-actions
         :param debug: whether to log compilation information to a log file
         :param log: whether to log simulation data to file
         :param backend: the subclass of RDDLSimulator to use as backend for
         simulation (currently supports numpy and Jax)
+        :param backend_kwargs: dictionary of additional named arguments to
+        pass to backend (must not include logger)
+        :param seeds: list of seeds for the cyclic iterator. Will be seeded in the reset function.
         '''
         super(RDDLEnv, self).__init__()
         self.domain_text = domain
         self.instance_text = instance
         self.enforce_action_constraints = enforce_action_constraints
         self.enforce_action_count_non_bool = enforce_action_count_non_bool
 
         # time budget for applications limiting time on episodes.
-        # hardcoded so cannot be changed externally.
-        self.budget = 120
+        # hardcoded so cannot be changed externally for the purpose of the competition.
+        # TODO: add it to the API after the competition
+        self.budget = 240
+        # self.seeds = [list of seeds]
+        self.seeds = RDDLEnvSeeder(seed_list=seeds)
 
         # read and parse domain and instance
         reader = RDDLReader(domain, instance)
         domain = reader.rddltxt
 
         # parse RDDL file
         parser = RDDLParser(lexer=None, verbose=False)
@@ -81,15 +90,15 @@
             simlog_fname = os.path.join(dir, ast.instance.name)
             self.simlogger = SimLogger(f'{simlog_fname}_log.csv')
         # self.simlogger = SimLogger(f'{log_fname}_log.csv') if log else None
         if self.simlogger:
             self.simlogger.clear(overwrite=False)
         
         # define the model sampler and bounds    
-        self.sampler = backend(self.model, logger=logger)
+        self.sampler = backend(self.model, logger=logger, **backend_kwargs)
         bounds = RDDLConstraints(self.sampler).bounds
 
         # set roll-out parameters
         self.horizon = self.model.horizon
         self.discount = self.model.discount
         self.max_allowed_actions = self.model.max_allowed_actions
             
@@ -162,15 +171,20 @@
         self._visualizer = TextVisualizer(self.model)
         self._movie_generator = None
         self.state = None
         self.image = None
         self.window = None
         self.to_render = False
         self.image_size = None
-
+    
+    def seed(self, seed=None):
+        # super(RDDLEnv, self).seed(seed)
+        self.sampler.seed(seed)
+        return [seed]
+    
     def set_visualizer(self, viz, movie_gen=None, movie_per_episode=False, **viz_kwargs):
         self._visualizer = viz(self.model, **viz_kwargs)
         self._movie_generator = movie_gen
         self._movie_per_episode = movie_per_episode
         self._movies = 0
         self.to_render = False
 
@@ -226,15 +240,15 @@
             self.done = True
 
         # for visualization purposes
         self.state = state
 
         return obs, reward, self.done, {}
 
-    def reset(self):
+    def reset(self, seed=None):
         self.total_reward = 0
         self.currentH = 0
         obs, self.done = self.sampler.reset()
         self.state = self.sampler.states
 
         image = self._visualizer.render(self.state)
         if self._movie_generator is not None:
@@ -249,14 +263,21 @@
         if self.simlogger:
             self.trial += 1
             text = '######################################################\n'
             text += 'New Trial\n'
             text += '######################################################'
             self.simlogger.log_free(text)
 
+        if seed is not None:
+            self.seed(seed)
+        else:
+            seed = self.seeds.Next()
+            if seed is not None:
+                self.seed(seed)
+
         return obs
 
     def pilImageToSurface(self, pilImage):
         return pygame.image.fromstring(
             pilImage.tobytes(), pilImage.size, pilImage.mode).convert()
 
     def render(self, to_display=True):
```

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/ErrorHandling/RDDLException.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/ErrorHandling/RDDLException.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Grounder/RDDLGrounder.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Grounder/RDDLGrounder.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxParameterTuning.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxParameterTuning.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,490 +1,729 @@
 from bayes_opt import BayesianOptimization
 from bayes_opt.util import UtilityFunction
 from colorama import init as colorama_init, Back, Fore, Style
-colorama_init()
-from concurrent.futures import as_completed, ProcessPoolExecutor      
+colorama_init()    
 import csv
+import datetime
 import jax
-import multiprocessing
+from multiprocessing import get_context
 import numpy as np
-import optax
 import os
 import time
 from typing import Callable, Dict, Tuple
 import warnings
 warnings.filterwarnings('ignore')
 
 from pyRDDLGym.Core.Env.RDDLEnv import RDDLEnv
-from pyRDDLGym.Core.Jax.JaxRDDLLogic import FuzzyLogic
 from pyRDDLGym.Core.Jax.JaxRDDLBackpropPlanner import JaxRDDLBackpropPlanner
 from pyRDDLGym.Core.Jax.JaxRDDLBackpropPlanner import JaxStraightLinePlan
+from pyRDDLGym.Core.Jax.JaxRDDLBackpropPlanner import JaxDeepReactivePolicy
+
+# do this after imports to prevent it from being overwritten
 np.seterr(all='warn')
 
+# ===============================================================================
+# 
+# GENERIC TUNING MODULE
+# 
+# Currently contains three implementations:
+# 1. straight line plan
+# 2. replanning
+# 3. deep reactive policies
+# 
+# ===============================================================================
+
+
+class JaxParameterTuning:
+    '''A general-purpose class for tuning a Jax planner.'''
+    
+    def __init__(self, env: RDDLEnv,
+                 hyperparams_dict: Dict[str, Tuple[float, float, Callable]],
+                 max_train_epochs: int,
+                 timeout_episode: float,
+                 timeout_tuning: float=np.inf,
+                 verbose: bool=True,
+                 print_step: int=None,
+                 planner_kwargs: Dict={},
+                 plan_kwargs: Dict={},
+                 pool_context: str='spawn',
+                 num_workers: int=1, 
+                 poll_frequency: float=0.2,
+                 gp_iters: int=25,
+                 acquisition=None,
+                 gp_init_kwargs: Dict={},
+                 gp_params: Dict={'n_restarts_optimizer': 10}) -> None:
+        '''Creates a new instance for tuning hyper-parameters for Jax planners
+        on the given RDDL domain and instance.
+        
+        :param env: the RDDLEnv describing the MDP to optimize
+        :param hyperparams_dict: dictionary mapping name of each hyperparameter
+        to a triple, where the first two elements are lower/upper bounds on the
+        parameter value, and the last is a callable mapping the parameter to its
+        RDDL equivalent
+        :param max_train_epochs: the maximum number of iterations of SGD per 
+        step or trial
+        :param timeout_episode: the maximum amount of time to spend training per
+        trial (in seconds)
+        :param timeout_tuning: the maximum amount of time to spend tuning 
+        hyperparameters in general (in seconds)
+        :param verbose: whether to print intermediate results of tuning
+        :param print_step: how often to print training callback
+        :param planner_kwargs: additional arguments to feed to the planner
+        :param plan_kwargs: additional arguments to feed to the plan/policy
+        :param pool_context: context for multiprocessing pool (defaults to 
+        "spawn")
+        :param num_workers: how many points to evaluate in parallel
+        :param poll_frequency: how often (in seconds) to poll for completed
+        jobs, necessary if num_workers > 1
+        :param gp_iters: number of iterations of optimization
+        :param acquisition: acquisition function for Bayesian optimizer
+        :parm gp_init_kwargs: additional parameters to feed to Bayesian 
+        during initialization  
+        :param gp_params: additional parameters to feed to Bayesian optimizer 
+        after initialization optimization
+        '''
+        
+        self.env = env
+        self.hyperparams_dict = hyperparams_dict
+        self.max_train_epochs = max_train_epochs
+        self.timeout_episode = timeout_episode
+        self.timeout_tuning = timeout_tuning
+        self.verbose = verbose
+        self.print_step = print_step
+        self.planner_kwargs = planner_kwargs
+        self.plan_kwargs = plan_kwargs
+        self.pool_context = pool_context
+        self.num_workers = num_workers
+        self.poll_frequency = poll_frequency
+        self.gp_iters = gp_iters
+        self.gp_init_kwargs = gp_init_kwargs
+        self.gp_params = gp_params
+        
+        # create acquisition function
+        if acquisition is None:
+            num_samples = self.gp_iters * self.num_workers
+            acquisition = JaxParameterTuning._annealing_utility(num_samples)
+        self.acquisition = acquisition
+        
+        # create valid color variations for multiprocess output
+        self.colors = JaxParameterTuning._color_variations()
+        self.num_workers = min(num_workers, len(self.colors))
+
+    @staticmethod
+    def _color_variations():
+        foreground = [Fore.BLUE, Fore.CYAN, Fore.GREEN,
+                      Fore.MAGENTA, Fore.RED, Fore.YELLOW]
+        background = [Back.RESET, Back.BLUE, Back.CYAN, Back.GREEN,
+                      Back.MAGENTA, Back.RED, Back.YELLOW]
+        return [(fore, back) 
+                for back in background
+                for fore in foreground
+                if int(back[2:-1]) - int(fore[2:-1]) != 10]
+
+    @staticmethod
+    def _annealing_utility(n_samples, n_delay_samples=0, kappa1=10.0, kappa2=1.0):
+        return UtilityFunction(
+            kind='ucb',
+            kappa=kappa1,
+            kappa_decay=(kappa2 / kappa1) ** (1.0 / (n_samples - n_delay_samples)),
+            kappa_decay_delay=n_delay_samples)
+    
+    def _pickleable_objective_with_kwargs(self):
+        raise NotImplementedError
+    
+    @staticmethod
+    def _wrapped_evaluate(index, params, key, color, func, kwargs):
+        target = func(params=params, kwargs=kwargs, key=key, index=index, color=color)
+        pid = os.getpid()
+        return index, pid, params, target
+
+    def tune(self, key: jax.random.PRNGKey, filename: str) -> Dict[str, object]:
+        '''Tunes the hyper-parameters for Jax planner, returns the best found.'''
+        starttime = time.time()
+        
+        # objective function
+        objective = self._pickleable_objective_with_kwargs()
+        evaluate = JaxParameterTuning._wrapped_evaluate
+            
+        # create optimizer
+        hyperparams_bounds = {
+            name: hparam[:2] 
+            for (name, hparam) in self.hyperparams_dict.items()
+        }
+        optimizer = BayesianOptimization(
+            f=None,  # probe() is not called
+            pbounds=hyperparams_bounds,
+            allow_duplicate_points=True,  # to avoid crash
+            random_state=np.random.RandomState(key),
+            **self.gp_init_kwargs
+        )
+        optimizer.set_gp_params(**self.gp_params)
+        utility = self.acquisition
+        
+        # suggest initial parameters to evaluate
+        num_workers = self.num_workers
+        suggested, kappas = [], []
+        for _ in range(num_workers):
+            utility.update_params()
+            probe = optimizer.suggest(utility)
+            suggested.append(probe)  
+            kappas.append(utility.kappa)
+        
+        # clear and prepare output file
+        filename = self._filename(filename, 'csv')
+        with open(filename, 'w', newline='') as file:
+            writer = csv.writer(file)
+            writer.writerow(
+                ['pid', 'worker', 'iteration', 'target', 'best_target', 'kappa'] + \
+                 list(hyperparams_bounds.keys())
+            )
+                
+        # start multiprocess evaluation
+        colors = self.colors[:num_workers]
+        worker_ids = list(range(num_workers))
+        best_params, best_target = None, -np.inf
+        
+        for it in range(self.gp_iters): 
+            
+            # check if there is enough time left for another iteration
+            currtime = time.time()  
+            elapsed = currtime - starttime
+            if elapsed > self.timeout_tuning - self.timeout_episode:
+                print(f'global time limit reached at iteration {it}, aborting')
+                break
+            
+            # continue with next iteration
+            print('\n' + '*' * 25 + 
+                  '\n' + f'[{datetime.timedelta(seconds=elapsed)}] ' + 
+                  f'starting iteration {it}' + 
+                  '\n' + '*' * 25)
+            key, *subkeys = jax.random.split(key, num=num_workers + 1)
+            rows = [None] * num_workers
+            
+            # create worker pool: note each iteration must wait for all workers
+            # to finish before moving to the next
+            with get_context(self.pool_context).Pool(processes=num_workers) as pool:
+                
+                # assign jobs to worker pool
+                # - each trains on suggested parameters from the last iteration
+                # - this way, since each job finishes asynchronously, these
+                # parameters usually differ across jobs
+                results = [
+                    pool.apply_async(evaluate, worker_args + objective)
+                    for worker_args in zip(worker_ids, suggested, subkeys, colors)
+                ]
+            
+                # wait for all workers to complete
+                while results:
+                    time.sleep(self.poll_frequency)
+                    
+                    # determine which jobs have completed
+                    jobs_done = []
+                    for (i, candidate) in enumerate(results):
+                        if candidate.ready():
+                            jobs_done.append(i)
+                    
+                    # get result from completed jobs
+                    for i in jobs_done[::-1]:
+                        
+                        # extract and register the new evaluation
+                        index, pid, params, target = results.pop(i).get()
+                        optimizer.register(params, target)
+                        
+                        # update acquisition function and suggest a new point
+                        utility.update_params()  
+                        suggested[index] = optimizer.suggest(utility)
+                        old_kappa = kappas[index]
+                        kappas[index] = utility.kappa
+                        
+                        # transform suggestion back to natural space
+                        rddl_params = {
+                            name: pf(params[name])
+                            for (name, (*_, pf)) in self.hyperparams_dict.items()
+                        }
+                        
+                        # update the best suggestion so far
+                        if target > best_target:
+                            best_params, best_target = rddl_params, target
+                        
+                        # write progress to file in real time
+                        rows[index] = [
+                            pid, index, it, target, best_target, old_kappa
+                        ] + list(rddl_params.values())
+                        
+            # write results of all processes in current iteration to file
+            with open(filename, 'a', newline='') as file:
+                writer = csv.writer(file)
+                writer.writerows(rows)
+            
+        self._save_plot(filename)
+        return best_params
+
+    def _filename(self, name, ext):
+        domainName = self.env.model.domainName()
+        instName = self.env.model.instanceName()
+        domainName = ''.join(c for c in domainName if c.isalnum() or c == '_')
+        instName = ''.join(c for c in instName if c.isalnum() or c == '_')
+        filename = f'{name}_{domainName}_{instName}.{ext}'
+        return filename
+    
+    def _save_plot(self, filename):
+        try:
+            import matplotlib.pyplot as plt
+            from sklearn.manifold import MDS
+        except Exception as e:
+            warnings.warn(f'failed to import packages matplotlib or sklearn, '
+                          f'aborting plot of search space\n'
+                          f'{e}', stacklevel=2)
+        else:
+            data = np.loadtxt(filename, delimiter=',', dtype=object)
+            data, target = data[1:, 3:], data[1:, 2]
+            data = data.astype(np.float64)
+            target = target.astype(np.float64)
+            target = (target - np.min(target)) / (np.max(target) - np.min(target))
+            embedding = MDS(n_components=2, normalized_stress='auto')
+            data1 = embedding.fit_transform(data)
+            sc = plt.scatter(data1[:, 0], data1[:, 1], c=target, s=4.,
+                             cmap='seismic', edgecolor='gray',
+                             linewidth=0.01, alpha=0.4)
+            plt.colorbar(sc)
+            plt.savefig(self._filename('gp_points', 'pdf'))
+            plt.clf()
+            plt.close()
+
+# ===============================================================================
+# 
+# STRAIGHT LINE PLANNING
+#
+# ===============================================================================
+
 
-def train_epoch(key, policy_hyperparams, subs, planner, timeout,
-                 max_train_epochs, verbose, print_step, color, guess=None): 
+def train_epoch(key, model_params, policy_hyperparams, subs, planner, timeout,
+                 max_train_epochs, verbose, print_step, index, color, guess=None): 
     colorstr = f'{color[0]}{color[1]}'
     starttime = None
     for (it, callback) in enumerate(planner.optimize(
         key=key,
         epochs=max_train_epochs,
         step=1,
+        model_params=model_params,
         policy_hyperparams=policy_hyperparams,
         subs=subs,
         guess=guess
     )):
         if starttime is None:
             starttime = time.time()
         currtime = time.time()  
         elapsed = currtime - starttime    
-        if verbose and print_step is not None and it > 0 and it % print_step == 0:
-            print(f'|------ {colorstr}' 
-                  '[{:.4f} s] step={} train_return={:.6f} test_return={:.6f}'.format(
+        if verbose and print_step is not None and print_step > 0 \
+        and it > 0 and it % print_step == 0:
+            print(f'|------ [{index}] {colorstr}' 
+                  '[{:.4f} s] step={} train_return={:.6f} test_return={:.6f} best_return={:.6f}'.format(
+                      index,
                       elapsed,
                       str(callback['iteration']).rjust(4),
                       callback['train_return'],
-                      callback['test_return']) + 
+                      callback['test_return'],
+                      callback['best_return']) + 
                   f'{Style.RESET_ALL}')
         if not np.isfinite(callback['train_return']):
             if verbose:
-                print(f'|------ {colorstr}'
-                      f'aborting due to NaN or inf value!'
+                print(f'|------ [{index}] {colorstr}'
+                      f'warning: training aborted due to NaN or inf value'
                       f'{Style.RESET_ALL}')
             break
         if elapsed >= timeout:
             break
     return callback
 
-       
-def objective_slp(std, lr, w, wa, key, std_space, lr_space, w_space, wa_space,
-                  model, wrap_sigmoid, eval_horizon, action_bounds, planner_kwargs,
-                  timeout_episode, max_train_epochs, verbose, print_step,
-                  color=(Fore.RESET, Back.RESET)):
-            
+
+def objective_slp(params, kwargs, key, index, color=(Fore.RESET, Back.RESET)):
+                    
     # transform hyper-parameters to natural space
-    std = std_space[2](std)
-    lr = lr_space[2](lr)
-    w = w_space[2](w)
-    if wa is not None:
-        wa = wa_space[2](wa)            
-    if verbose:
-        colorstr = f'{color[0]}{color[1]}'
-        print(f'| {colorstr}'
+    param_values = [
+        pmap(params[name])
+        for (name, (*_, pmap)) in kwargs['hyperparams_dict'].items()
+    ]
+    
+    # unpack hyper-parameters
+    if kwargs['wrapped_bool_actions']:
+        std, lr, w, wa = param_values
+    else:
+        std, lr, w = param_values
+        wa = None
+                      
+    if kwargs['verbose']:
+        print(f'| [{index}] {color[0]}{color[1]}'
                 f'optimizing SLP with PRNG key={key}, ' 
                 f'std={std}, lr={lr}, w={w}, wa={wa}...{Style.RESET_ALL}')
-            
+        
     # initialize planner
     planner = JaxRDDLBackpropPlanner(
-        rddl=model,
+        rddl=kwargs['rddl'],
         plan=JaxStraightLinePlan(
             initializer=jax.nn.initializers.normal(std),
-            wrap_sigmoid=wrap_sigmoid),
-        rollout_horizon=eval_horizon,
-        action_bounds=action_bounds,
-        optimizer=optax.rmsprop,
+            **kwargs['plan_kwargs']),
         optimizer_kwargs={'learning_rate': lr},
-        logic=FuzzyLogic(weight=w),
-        **planner_kwargs)
-    policy_hyperparams = {name: wa for name in action_bounds}
-            
+        **kwargs['planner_kwargs'])
+                    
     # perform training
     callback = train_epoch(
         key=key,
-        policy_hyperparams=policy_hyperparams,
+        model_params={name: w for name in planner.compiled.model_params},
+        policy_hyperparams={name: wa for name in kwargs['wrapped_bool_actions']},
         subs=None,
         planner=planner,
-        timeout=timeout_episode,
-        max_train_epochs=max_train_epochs,
-        verbose=verbose,
-        print_step=print_step,
+        timeout=kwargs['timeout_episode'],
+        max_train_epochs=kwargs['max_train_epochs'],
+        verbose=kwargs['verbose'],
+        print_step=kwargs['print_step'],
+        index=index,
         color=color,
         guess=None)
     total_reward = float(callback['best_return'])
-    if verbose:
-        print(f'| {colorstr}'
+            
+    if kwargs['verbose']:
+        print(f'| [{index}] {color[0]}{color[1]}'
                 f'done optimizing SLP, '
                 f'total reward={total_reward}{Style.RESET_ALL}')
     return total_reward
 
+        
+def power_ten(x):
+    return 10.0 ** x
 
-def objective_mpc(std, lr, w, wa, T, key, std_space, lr_space, w_space, wa_space,
-                  T_space, domain, instance, model, wrap_sigmoid,
-                  eval_horizon, eval_trials, use_guess_last_epoch,
-                  action_bounds, planner_kwargs,
-                  timeout_episode, timeout_epoch, max_train_epochs,
-                  verbose, print_step, color=(Fore.RESET, Back.RESET)):
     
+class JaxParameterTuningSLP(JaxParameterTuning):
+    
+    def __init__(self, *args,
+                 hyperparams_dict: Dict[str, Tuple[float, float, Callable]]={
+                    'std': (-5., 0., power_ten),
+                    'lr': (-5., 0., power_ten),
+                    'w': (0., 5., power_ten),
+                    'wa': (0., 5., power_ten)
+                 },
+                 **kwargs) -> None:
+        '''Creates a new tuning class for straight line planners.
+        
+        :param *args: arguments to pass to parent class
+        :param hyperparams_dict: same as parent class, but here must contain
+        weight initialization (std), learning rate (lr), model weight (w), and
+        action weight (wa) if wrap_sigmoid and boolean action fluents exist
+        :param **kwargs: keyword arguments to pass to parent class
+        '''
+        
+        super(JaxParameterTuningSLP, self).__init__(
+            *args, hyperparams_dict=hyperparams_dict, **kwargs)
+        
+        # action parameters required if wrap_sigmoid and boolean action exists
+        self.wrapped_bool_actions = []
+        if self.plan_kwargs.get('wrap_sigmoid', True):
+            for var in self.env.model.actions:
+                if self.env.model.variable_ranges[var] == 'bool':
+                    self.wrapped_bool_actions.append(var)
+        if not self.wrapped_bool_actions:
+            self.hyperparams_dict.pop('wa', None)
+        
+    def _pickleable_objective_with_kwargs(self):
+        objective_fn = objective_slp
+        
+        # duplicate planner and plan keyword arguments must be removed
+        plan_kwargs = self.plan_kwargs.copy()
+        plan_kwargs.pop('initializer', None) 
+               
+        planner_kwargs = self.planner_kwargs.copy()
+        planner_kwargs.pop('rddl', None)
+        planner_kwargs.pop('plan', None)
+        planner_kwargs.pop('optimizer_kwargs', None)
+                    
+        kwargs = {
+            'rddl': self.env.model,
+            'hyperparams_dict': self.hyperparams_dict,
+            'timeout_episode': self.timeout_episode,
+            'max_train_epochs': self.max_train_epochs,
+            'planner_kwargs': planner_kwargs,
+            'plan_kwargs': plan_kwargs,
+            'verbose': self.verbose,
+            'print_step': self.print_step,
+            'wrapped_bool_actions': self.wrapped_bool_actions
+        }
+        return objective_fn, kwargs
+
+# ===============================================================================
+# 
+# REPLANNING
+#
+# ===============================================================================
+
+
+def objective_replan(params, kwargs, key, index, color=(Fore.RESET, Back.RESET)):
+
     # transform hyper-parameters to natural space
-    std = std_space[2](std)
-    lr = lr_space[2](lr)
-    w = w_space[2](w)
-    if wa is not None:
-        wa = wa_space[2](wa)
-    T = T_space[2](T)        
-        
-    if verbose:
-        colorstr = f'{color[0]}{color[1]}'
-        print(f'| {colorstr}'
+    param_values = [
+        pmap(params[name])
+        for (name, (*_, pmap)) in kwargs['hyperparams_dict'].items()
+    ]
+    
+    # unpack hyper-parameters
+    if kwargs['wrapped_bool_actions']:
+        std, lr, w, wa, T = param_values
+    else:
+        std, lr, w, T = param_values
+        wa = None
+        
+    if kwargs['verbose']:
+        print(f'| [{index}] {color[0]}{color[1]}'
               f'optimizing MPC with PRNG key={key}, ' 
               f'std={std}, lr={lr}, w={w}, wa={wa}, T={T}...'
               f'{Style.RESET_ALL}')
-    
+
     # initialize planner
     planner = JaxRDDLBackpropPlanner(
-        rddl=model,
+        rddl=kwargs['rddl'],
         plan=JaxStraightLinePlan(
             initializer=jax.nn.initializers.normal(std),
-            wrap_sigmoid=wrap_sigmoid),
+            **kwargs['plan_kwargs']),
         rollout_horizon=T,
-        action_bounds=action_bounds,
-        optimizer=optax.rmsprop,
         optimizer_kwargs={'learning_rate': lr},
-        logic=FuzzyLogic(weight=w),
-        **planner_kwargs)
-    policy_hyperparams = {name: wa for name in action_bounds}
+        **kwargs['planner_kwargs'])
+    policy_hyperparams = {name: wa for name in kwargs['wrapped_bool_actions']}
+    model_params = {name: w for name in planner.compiled.model_params}
     
     # initialize env for evaluation (need fresh copy to avoid concurrency)
-    env = RDDLEnv(domain=domain,
-                  instance=instance,
+    env = RDDLEnv(domain=kwargs['domain'],
+                  instance=kwargs['instance'],
                   enforce_action_constraints=True)
-    
-    # perform training and collect rewards
+
+    # perform training
     average_reward = 0.0
-    for trial in range(eval_trials):
-        if verbose:
-            print(f'|--- {colorstr}'
+    for trial in range(kwargs['eval_trials']):
+        
+        # start the next trial
+        if kwargs['verbose']:
+            print(f'|--- [{index}] {color[0]}{color[1]}'
                   f'starting trial {trial + 1} '
                   f'with PRNG key={key}...{Style.RESET_ALL}')
+            
         total_reward = 0.0
         guess = None
         env.reset() 
         starttime = time.time()
-        for _ in range(eval_horizon):
+        for _ in range(kwargs['eval_horizon']):
             currtime = time.time()
             elapsed = currtime - starttime            
-            if elapsed < timeout_episode:
+            if elapsed < kwargs['timeout_episode']:
                 subs = env.sampler.subs
-                timeout = min(timeout_episode - elapsed, timeout_epoch)
+                timeout = min(kwargs['timeout_episode'] - elapsed,
+                              kwargs['timeout_epoch'])
                 key, subkey1, subkey2 = jax.random.split(key, num=3)
                 callback = train_epoch(
                     key=subkey1,
+                    model_params=model_params,
                     policy_hyperparams=policy_hyperparams,
                     subs=subs,
                     planner=planner,
                     timeout=timeout,
-                    max_train_epochs=max_train_epochs,
-                    verbose=verbose,
+                    max_train_epochs=kwargs['max_train_epochs'],
+                    verbose=kwargs['verbose'],
                     print_step=None,
+                    index=index,
                     color=color,
                     guess=guess)
                 params = callback['best_params']
                 action = planner.get_action(subkey2, params, 0, subs)
-                if use_guess_last_epoch:
+                if kwargs['use_guess_last_epoch']:
                     guess = planner.plan.guess_next_epoch(params)
             else:
                 action = {}            
             _, reward, done, _ = env.step(action)
             total_reward += reward 
             if done: 
                 break  
-        if verbose:
-            print(f'|--- {colorstr}'
+            
+        # update average reward across trials
+        if kwargs['verbose']:
+            print(f'|--- [{index}] {color[0]}{color[1]}'
                   f'done trial {trial + 1}, '
                   f'total reward={total_reward}{Style.RESET_ALL}')
-        average_reward += total_reward / eval_trials
-    if verbose:
-        print(f'| {colorstr}'
+        average_reward += total_reward / kwargs['eval_trials']
+        
+    if kwargs['verbose']:
+        print(f'| [{index}] {color[0]}{color[1]}'
               f'done optimizing MPC, '
               f'average reward={average_reward}{Style.RESET_ALL}')
     return average_reward
-    
-
-def evaluate(args):
-    params, index, key, color, func, kwargs = args
-    func_kwargs = {**params, **kwargs}
-    target = func(key=key, color=color, **func_kwargs)
-    pid = os.getpid()
-    return pid, index, params, target
-
 
-def power_ten(x):
-    return 10.0 ** x
-
-
-def annealing_utility(n_samples, n_delay_samples=0, kappa1=10.0, kappa2=1.0):
-    return UtilityFunction(
-        kind='ucb',
-        kappa=kappa1,
-        kappa_decay=(kappa2 / kappa1) ** (1.0 / (n_samples - n_delay_samples)),
-        kappa_decay_delay=n_delay_samples
-    )
     
+class JaxParameterTuningSLPReplan(JaxParameterTuningSLP):
     
-class JaxParameterTuning:
-    '''A general-purpose class for tuning a Jax planner.'''
-    
-    def __init__(self, env: RDDLEnv,
-                 action_bounds: Dict[str, Tuple[float, float]],
-                 max_train_epochs: int,
-                 timeout_episode: float,
-                 timeout_epoch: float,
-                 stddev_space: Tuple[float, float, Callable]=(-5., 0., power_ten),
-                 lr_space: Tuple[float, float, Callable]=(-5., 0., power_ten),
-                 model_weight_space: Tuple[float, float, Callable]=(0., 5., power_ten),
-                 action_weight_space: Tuple[float, float, Callable]=(0., 5., power_ten),
-                 lookahead_space: Tuple[float, float]=(1, 100, int),
-                 num_workers: int=1,
-                 gp_iters: int=25,
-                 acquisition=None,
-                 gp_params: Dict={'n_restarts_optimizer': 10},
-                 eval_horizon: int=None,
+    def __init__(self, timeout_epoch: float,
+                 *args,
+                 hyperparams_dict: Dict[str, Tuple[float, float, Callable]]={
+                    'std': (-5., 0., power_ten),
+                    'lr': (-5., 0., power_ten),
+                    'w': (0., 5., power_ten),
+                    'wa': (0., 5., power_ten),
+                    'T': (1, 100, int)
+                 },
                  eval_trials: int=5,
-                 print_step: int=None,
-                 verbose: bool=True,
-                 wrap_sigmoid: bool=True,
                  use_guess_last_epoch: bool=True,
-                 planner_kwargs: Dict={}) -> None:
-        '''Creates a new instance for tuning hyper-parameters for Jax planners
-        on the given RDDL domain and instance.
+                 **kwargs) -> None:
+        '''Creates a new tuning class for straight line planners.
         
-        :param env: the RDDLEnv describing the MDP to optimize
-        :param action_bounds: the bounds on the actions
-        :param max_train_epochs: the maximum number of iterations of SGD per 
-        step or trial
-        :param timeout_episode: the maximum amount of time to spend training per
-        trial (in seconds)
         :param timeout_epoch: the maximum amount of time to spend training per
-        decision epoch (in seconds, for MPC only)
-        :param stddev_space: set of initializer standard deviations for the 
-        policy or plan parameters (uses Gaussian noise) to tune
-        :param lr_space: set of learning rates for SGD (uses rmsprop by 
-        default) to tune
-        :param model_weight_space: set of model weight parameters for continuous 
-        relaxation to tune
-        :param action_weight_space: sigmoid weights for boolean actions to tune
-        :param lookahead_space: set of possible lookahead horizons for MPC to
-        tune
-        :param num_workers: how many points to evaluate in parallel
-        :param gp_iters: number of iterations of optimization
-        :param acquisition: acquisition function for Bayesian optimizer
-        :param gp_params: additional parameters to feed to Bayesian optimizer
-        :param eval_horizon: maximum number of decision epochs to evaluate (also
-        applies for training if using straight-line planning)
-        :param eval_trials: how many trials to perform for MPC (batch size has
-        the same effect for non-MPC)
-        :param print_step: how often to print training callback
-        :param verbose: whether to print intermediate results of tuning
-        :param wrap_sigmoid: whether to wrap bool action-fluents with sigmoid
-        :param use_guess_last_epoch: for MPC approach, use the trained parameters
-        from previous epoch to seed next epoch actions
-        :param planner_kwargs: additional arguments to feed to the planner
+        decision time step
+        :param *args: arguments to pass to parent class
+        :param hyperparams_dict: same as parent class, but here must contain
+        weight initialization (std), learning rate (lr), model weight (w), 
+        action weight (wa) if wrap_sigmoid and boolean action fluents exist, and
+        lookahead horizon (T)
+        :param eval_trials: how many trials to perform independent training
+        in order to estimate the return for each set of hyper-parameters
+        :param use_guess_last_epoch: use the trained parameters from previous 
+        decision to warm-start next decision
+        :param **kwargs: keyword arguments to pass to parent class
         '''
-        self.env = env
-        self.action_bounds = action_bounds
-        self.max_train_epochs = max_train_epochs
-        self.timeout_episode = timeout_episode
+        
+        super(JaxParameterTuningSLPReplan, self).__init__(
+            *args, hyperparams_dict=hyperparams_dict, **kwargs)
+        
         self.timeout_epoch = timeout_epoch
-        self.evaluation_horizon = eval_horizon
-        if eval_horizon is None:
-            self.evaluation_horizon = env.horizon
-        self.evaluation_trials = eval_trials
-        self.stddev_space = stddev_space
-        self.lr_space = lr_space
-        self.model_weight_space = model_weight_space
-        self.action_weight_space = action_weight_space
-        self.lookahead_space = lookahead_space
-        self.gp_iters = gp_iters
-        self.gp_params = gp_params
-        self.print_step = print_step
-        self.verbose = verbose
-        self.wrap_sigmoid = wrap_sigmoid
+        self.eval_trials = eval_trials
         self.use_guess_last_epoch = use_guess_last_epoch
-        self.planner_kwargs = planner_kwargs
         
-        # check if action parameters are required
-        self.use_wa_param = False
-        if self.wrap_sigmoid:
-            for var in self.env.model.actions:
-                if self.env.model.variable_ranges[var] == 'bool':
-                    self.use_wa_param = True
-                    break
-        
-        # project search space back to parameter space
-        self._map = {'std': stddev_space[2],
-                     'lr': lr_space[2],
-                     'w': model_weight_space[2],
-                     'wa': action_weight_space[2],
-                     'T': lookahead_space[2]}
+    def _pickleable_objective_with_kwargs(self):
+        objective_fn = objective_replan
+            
+        # duplicate planner and plan keyword arguments must be removed
+        plan_kwargs = self.plan_kwargs.copy()
+        plan_kwargs.pop('initializer', None)
         
-        # yields 36 valid format variations
-        foreground = [Fore.BLUE, Fore.CYAN, Fore.GREEN,
-                      Fore.MAGENTA, Fore.RED, Fore.YELLOW]
-        background = [Back.RESET, Back.BLUE, Back.CYAN, Back.GREEN,
-                      Back.MAGENTA, Back.RED, Back.YELLOW]
-        self.colors = []
-        for back in background:
-            for fore in foreground:
-                if int(back[2:-1]) - int(fore[2:-1]) != 10:
-                    self.colors.append((fore, back))
-        self.num_workers = min(num_workers, len(self.colors))
+        planner_kwargs = self.planner_kwargs.copy()
+        planner_kwargs.pop('rddl', None)
+        planner_kwargs.pop('plan', None)
+        planner_kwargs.pop('rollout_horizon', None)
+        planner_kwargs.pop('optimizer_kwargs', None)
+                        
+        kwargs = {
+            'rddl': self.env.model,
+            'domain': self.env.domain_text,
+            'instance': self.env.instance_text,
+            'hyperparams_dict': self.hyperparams_dict,
+            'timeout_episode': self.timeout_episode,
+            'max_train_epochs': self.max_train_epochs,
+            'planner_kwargs': planner_kwargs,
+            'plan_kwargs': plan_kwargs,
+            'verbose': self.verbose,
+            'print_step': self.print_step,
+            'wrapped_bool_actions': self.wrapped_bool_actions,
+            'timeout_epoch': self.timeout_epoch,
+            'eval_trials': self.eval_trials,
+            'eval_horizon': self.env.horizon,
+            'use_guess_last_epoch': self.use_guess_last_epoch
+        }
+        return objective_fn, kwargs
+
+# ===============================================================================
+# 
+# DEEP REACTIVE POLICIES
+#
+# ===============================================================================
+
+
+def objective_drp(params, kwargs, key, index, color=(Fore.RESET, Back.RESET)):
+                    
+    # transform hyper-parameters to natural space
+    param_values = [
+        pmap(params[name])
+        for (name, (*_, pmap)) in kwargs['hyperparams_dict'].items()
+    ]
+    
+    # unpack hyper-parameters
+    lr, w, layers, neurons = param_values
+                      
+    if kwargs['verbose']:
+        print(f'| [{index}] {color[0]}{color[1]}'
+                f'optimizing DRP with PRNG key={key}, ' 
+                f'lr={lr}, w={w}, layers={layers}, neurons={neurons}...{Style.RESET_ALL}')
+           
+    # initialize planner
+    planner = JaxRDDLBackpropPlanner(
+        rddl=kwargs['rddl'],
+        plan=JaxDeepReactivePolicy(
+            topology=[neurons] * layers,
+            **kwargs['plan_kwargs']),
+        optimizer_kwargs={'learning_rate': lr},
+        **kwargs['planner_kwargs'])
     
-        if acquisition is None:
-            acquisition = annealing_utility(self.gp_iters * self.num_workers)
-        self.acquisition = acquisition
+    # perform training
+    callback = train_epoch(
+        key=key,
+        model_params={name: w for name in planner.compiled.model_params},
+        policy_hyperparams={name: None for name in planner._action_bounds},
+        subs=None,
+        planner=planner,
+        timeout=kwargs['timeout_episode'],
+        max_train_epochs=kwargs['max_train_epochs'],
+        verbose=kwargs['verbose'],
+        print_step=kwargs['print_step'],
+        index=index,
+        color=color,
+        guess=None)
+    total_reward = float(callback['best_return'])
+            
+    if kwargs['verbose']:
+        print(f'| [{index}] {color[0]}{color[1]}'
+                f'done optimizing DRP, '
+                f'total reward={total_reward}{Style.RESET_ALL}')
+    return total_reward
 
-    def _filename(self, name, ext):
-        domainName = self.env.model.domainName()
-        instName = self.env.model.instanceName()
-        domainName = ''.join(c for c in domainName if c.isalnum() or c == '_')
-        instName = ''.join(c for c in instName if c.isalnum() or c == '_')
-        filename = f'{name}_{domainName}_{instName}.{ext}'
-        return filename
+
+def power_two_int(x):
+    return 2 ** int(x)
+
+
+class JaxParameterTuningDRP(JaxParameterTuning):
     
-    def _save_plot(self, name):
-        try:
-            import matplotlib.pyplot as plt
-            from sklearn.manifold import MDS
-            filename = self._filename(name, 'csv')
-        except Exception as e:
-            print('failed to import packages for plotting search space:')
-            print(e)
-            print('aborting plot of search space')
-        else:
-            data = np.loadtxt(filename, delimiter=',', dtype=object)
-            data, target = data[1:, 3:], data[1:, 2]
-            data = data.astype(np.float64)
-            target = target.astype(np.float64)
-            target = (target - np.min(target)) / (np.max(target) - np.min(target))
-            embedding = MDS(n_components=2, normalized_stress='auto')
-            data1 = embedding.fit_transform(data)
-            sc = plt.scatter(data1[:, 0], data1[:, 1], c=target, s=4.,
-                             cmap='seismic', edgecolor='gray',
-                             linewidth=0.01, alpha=0.4)
-            plt.colorbar(sc)
-            plt.savefig(self._filename('gp_points', 'pdf'))
-            plt.clf()
-            plt.close()
-       
-    def _bayes_optimize(self, key, name, mpc): 
+    def __init__(self, *args,
+                 hyperparams_dict: Dict[str, Tuple[float, float, Callable]]={
+                    'lr': (-6., 0., power_ten),
+                    'w': (0., 5., power_ten),
+                    'layers': (1., 3., int),
+                    'neurons': (1., 9., power_two_int)
+                 },
+                 **kwargs) -> None:
+        '''Creates a new tuning class for deep reactive policies.
         
-        # set the bounds on variables
-        pbounds = {'std': self.stddev_space[:2],
-                   'lr': self.lr_space[:2],
-                   'w': self.model_weight_space[:2]}
-        if self.use_wa_param:
-            pbounds['wa'] = self.action_weight_space[:2]
-        if mpc:
-            pbounds['T'] = self.lookahead_space[:2]
-            
-        # set non changing variables
-        kwargs = {'std_space': self.stddev_space,
-                  'lr_space': self.lr_space,
-                  'w_space': self.model_weight_space,
-                  'wa_space': self.action_weight_space,
-                  'model': self.env.model,
-                  'wrap_sigmoid': self.wrap_sigmoid,
-                  'eval_horizon': self.evaluation_horizon,
-                  'action_bounds': self.action_bounds,
-                  'planner_kwargs': self.planner_kwargs,
-                  'timeout_episode': self.timeout_episode,
-                  'max_train_epochs': self.max_train_epochs,
-                  'verbose': self.verbose,
-                  'print_step': self.print_step}  
-        if not self.use_wa_param:
-            kwargs['wa'] = None
-        if mpc:
-            kwargs['T_space'] = self.lookahead_space
-            kwargs['domain'] = self.env.domain_text
-            kwargs['instance'] = self.env.instance_text
-            kwargs['eval_trials'] = self.evaluation_trials
-            kwargs['use_guess_last_epoch'] = self.use_guess_last_epoch
-            kwargs['timeout_epoch'] = self.timeout_epoch
-                
-        # create optimizer
-        optimizer = BayesianOptimization(
-            f=None,  # probe() is not called
-            pbounds=pbounds,
-            allow_duplicate_points=True,  # to avoid crash
-            random_state=np.random.RandomState(key)
-        )
-        optimizer.set_gp_params(**self.gp_params)
-        utility = self.acquisition
+        :param *args: arguments to pass to parent class
+        :param hyperparams_dict: same as parent class, but here must contain
+        learning rate (lr), model weight (w), number of hidden layers (layers) 
+        and number of neurons per hidden layer (neurons)
+        :param **kwargs: keyword arguments to pass to parent class
+        '''
         
-        # suggest initial parameters to evaluate
-        num_workers = self.num_workers
-        suggested, kappas = [], []
-        for _ in range(num_workers):
-            utility.update_params()
-            suggested.append(optimizer.suggest(utility))  
-            kappas.append(utility.kappa)          
+        super(JaxParameterTuningDRP, self).__init__(
+            *args, hyperparams_dict=hyperparams_dict, **kwargs)
+    
+    def _pickleable_objective_with_kwargs(self):
+        objective_fn = objective_drp
         
-        # saving to file
-        keys = list(pbounds.keys())
-        filename = self._filename(name, 'csv')
-        with open(filename, 'w', newline='') as file:
-            writer = csv.writer(file)
-            writer.writerow(
-                ['pid', 'worker', 'iteration',
-                 'target', 'best_target', 'kappa'] + keys)
-        file = open(filename, 'a', newline='')
-        writer = csv.writer(file)        
-        lock = multiprocessing.Manager().Lock()
-        
-        # continue with multi-process evaluation
-        objective = objective_mpc if mpc else objective_slp
-        best_target = -np.inf
-        colors = self.colors[:num_workers]
+        # duplicate planner and plan keyword arguments must be removed
+        plan_kwargs = self.plan_kwargs.copy()
+        plan_kwargs.pop('topology', None)
         
-        for it in range(self.gp_iters): 
-            print('\n' + '*' * 25 + 
-                  '\n' + f'starting iteration {it}' + 
-                  '\n' + '*' * 25)
-            key, *subkeys = jax.random.split(key, num=num_workers + 1)
-            
-            # create worker pool: note each iteration must wait for all workers
-            # to finish before moving to the next
-            with ProcessPoolExecutor(max_workers=num_workers) as executor:
-                
-                # each worker evaluates planner for a suggested parameter dict
-                jobs = [
-                    executor.submit(
-                        evaluate, tuple(worker_args) + (objective, kwargs)) 
-                    for worker_args in zip(
-                        suggested, range(num_workers), subkeys, colors)
-                ]
-                
-                # on completion of each job...
-                for job in as_completed(jobs):
-                    
-                    # extract and register the new evaluation
-                    pid, index, params, target = job.result()
-                    optimizer.register(params, target)
-                    
-                    # update acquisition function and suggest a new point
-                    utility.update_params()  
-                    suggested[index] = optimizer.suggest(utility)
-                    old_kappa = kappas[index]
-                    kappas[index] = utility.kappa
-                    best_target = max(best_target, target)
-                    
-                    # write progress to file in real time
-                    with lock:
-                        writer.writerow(
-                            [pid, index, it, target, best_target, old_kappa] + \
-                            [self._map[k](params[k]) for k in keys]
-                        )
-                
-        # close file stream, save plot
-        file.close()
-        self._save_plot(name)
-
-    def tune_slp(self, key: jax.random.PRNGKey) -> None:
-        '''Tunes the hyper-parameters for Jax planner using straight-line 
-        planning approach.'''
-        self._bayes_optimize(key, 'gp_slp', False)
-    
-    def tune_mpc(self, key: jax.random.PRNGKey) -> None:
-        '''Tunes the hyper-parameters for Jax planner using MPC/receding horizon
-        planning approach.'''
-        self._bayes_optimize(key, 'gp_mpc', True)
-    
+        planner_kwargs = self.planner_kwargs.copy()
+        planner_kwargs.pop('rddl', None)
+        planner_kwargs.pop('plan', None)
+        planner_kwargs.pop('optimizer_kwargs', None)
+                     
+        kwargs = {
+            'rddl': self.env.model,
+            'hyperparams_dict': self.hyperparams_dict,
+            'timeout_episode': self.timeout_episode,
+            'max_train_epochs': self.max_train_epochs,
+            'planner_kwargs': planner_kwargs,
+            'plan_kwargs': plan_kwargs,
+            'verbose': self.verbose,
+            'print_step': self.print_step
+        }
+        return objective_fn, kwargs
```

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlanner.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlanner.py`

 * *Files 0% similar despite different names*

```diff
@@ -969,38 +969,41 @@
         
         return init_train, init_test
     
     def optimize(self, key: random.PRNGKey,
                  epochs: int,
                  step: int=1,
                  plot_step: int=None,
+                 model_params: Dict[str, object]=None,
                  policy_hyperparams: Dict[str, object]=None,
                  subs: Dict[str, object]=None,
                  guess: Dict[str, object]=None) -> Iterable[Dict[str, object]]:
         ''' Compute an optimal straight-line plan.
         
         :param key: JAX PRNG key
         :param epochs: the maximum number of steps of gradient descent
         :param step: frequency the callback is provided back to the user
         :param plot_step: frequency to plot the plan and save result to disk
+        :param model_params: optional model-parameters to override default
         :param policy_hyperparams: hyper-parameters for the policy/plan, such as
         weights for sigmoid wrapping boolean actions
         :param subs: dictionary mapping initial state and non-fluents to 
         their values: if None initializes all variables from the RDDL instance
         :param guess: initial policy parameters: if None will use the initializer
         specified in this instance
         '''
         
         # compute a batched version of the initial values
         if subs is None:
             subs = self.test_compiled.init_values
         train_subs, test_subs = self._batched_init_subs(subs)
         
         # initialize, model parameters
-        model_params = self.compiled.model_params
+        if model_params is None:
+            model_params = self.compiled.model_params
         model_params_test = self.test_compiled.model_params
         
         # initialize policy parameters
         if guess is None:
             key, subkey = random.split(key)
             policy_params, opt_state = self.initialize(
                 subkey, policy_hyperparams, train_subs)
```

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlannerUCT.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLBackpropPlannerUCT.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLCompiler.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLCompiler.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLLogic.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLLogic.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLModelError.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLModelError.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Jax/JaxRDDLSimulator.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Jax/JaxRDDLSimulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import jax
-import numpy as np
-np.seterr(all='raise')
+import time
 from typing import Dict
 
 from pyRDDLGym.Core.ErrorHandling.RDDLException import RDDLActionPreconditionNotSatisfiedError
 from pyRDDLGym.Core.ErrorHandling.RDDLException import RDDLInvalidExpressionError
 from pyRDDLGym.Core.ErrorHandling.RDDLException import RDDLStateInvariantNotSatisfiedError
 
 from pyRDDLGym.Core.Compiler.RDDLLiftedModel import RDDLLiftedModel
@@ -32,23 +31,26 @@
         the Jax program: unlike the numpy sim, errors cannot be caught in the 
         middle of evaluating a Jax expression; instead they are accumulated and
         returned to the user upon complete evaluation of the expression
         :param logger: to log information about compilation to file
         :param **compiler_args: keyword arguments to pass to the Jax compiler
         '''
         if key is None:
-            seed = np.random.randint(0, 2 ** 31 - 1)
-            key = jax.random.PRNGKey(seed)
+            key = jax.random.PRNGKey(round(time.time() * 1000))
         self.key = key
         self.raise_error = raise_error
         self.compiler_args = compiler_args
         
         # generate direct sampling with default numpy RNG and operations
         super(JaxRDDLSimulator, self).__init__(rddl, logger=logger)
     
+    def seed(self, seed: int) -> None:
+        super(JaxRDDLSimulator, self).seed(seed)
+        self.key = jax.random.PRNGKey(seed)
+        
     def _compile(self):
         rddl = self.rddl
         
         # compilation
         if self.logger is not None:
             self.logger.clear()
         compiled = JaxRDDLCompiler(rddl, logger=self.logger, **self.compiler_args)
```

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/RDDLReader.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/RDDLReader.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/cpf.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/cpf.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/domain.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/domain.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/expr.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/expr.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/instance.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/instance.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/nonfluents.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/nonfluents.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/parser.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/parsetab.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/parsetab.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/pvariable.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/pvariable.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/rddl.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/rddl.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Parser/utils.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Parser/utils.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Core/Simulator/RDDLSimulator.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Core/Simulator/RDDLSimulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,17 @@
             'pow': np.power,
             'log': lambda x, y: np.log(x) / np.log(y),
             'hypot': np.hypot
         }
         self.CONTROL_OPS = {'if': np.where,
                             'switch': np.select}
     
+    def seed(self, seed: int) -> None:
+        self.rng = np.random.default_rng(seed)
+        
     def _compile(self):
         rddl = self.rddl
         
         # compile initial values
         if self.logger is not None:
             self.logger.clear()
         initializer = RDDLValueInitializer(rddl, logger=self.logger)
```

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Continuous/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Continuous/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Continuous/instance0.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Continuous/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Discrete/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Discrete/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/CartPole/Discrete/instance0.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/CartPole/Discrete/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Elevators/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Elevators/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Elevators/instance0.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Elevators/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Elevators/instance1.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Elevators/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/ExampleManager.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/ExampleManager.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/HVAC/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/HVAC/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerator.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerator.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,13 +88,18 @@
         return value
         
     def save_instance(self, instance: int, params: Dict[str, object], path=None) -> None:
         if path == None:
             path = os.path.dirname(os.path.abspath(__file__))
             path = os.path.join(path, self.get_env_path())
 
+        dir = path
         path = os.path.join(path, f'instance{instance}.rddl')
         rddl = self.generate_instance(instance, params)
+        isExist = os.path.exists(dir)
+        if not isExist:
+            # Create a new directory because it does not exist
+            os.makedirs(dir)
         with open(path, 'w') as text_file:
             text_file.write(rddl)
         print(f'saved RDDL file to {path}.')
```

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/HVACInstanceGenerator.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/HVACInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/MarsRoverInstanceGenerator.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/MarsRoverInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/MountainCarInstanceGenerator.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/MountainCarInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/PowerGenInstanceGenerator.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/PowerGenInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/RaceCarInstanceGenerator.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/RaceCarInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/RecSimInstanceGen.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/RecSimInstanceGenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         provider_clusters, num_users, user_stddev
     )
 
     # Begin instance generation.
     # Objects.
     providers = [f'p{i+1}' for i in range(num_provider_clusters)]
     users = [f'c{i+1}' for i in range(num_users)]
-    features = ', '.join(['f1', 'f2'])
+    features = ['f1', 'f2']
     items = [f'i{i+1}' for i in range(num_docs)]
     # Non-fluents.
     nonfluents = {}
     for i, user in enumerate(users):
       nonfluents[f'CONSUMER-AFFINITY({user}, f1)'] = user_locs[i][0].numpy()
       nonfluents[f'CONSUMER-AFFINITY({user}, f2)'] = user_locs[i][1].numpy()
     for i, provider in enumerate(providers):
```

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/ReservoirInstanceGenerator.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/ReservoirInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/InstanceGenerators/UAVInstanceGenerator.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/InstanceGenerators/UAVInstanceGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/MarsRover/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/MarsRover/instance0.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/MarsRover/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/MountainCar/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/MountainCar/domain_old.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/domain_old.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/MountainCar/instance0.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/MountainCar/instance0_old.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/MountainCar/instance0_old.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/instance0.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Continuous/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Continuous/instance0.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Continuous/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Discrete/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Discrete/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/PowerGen/Discrete/instance0.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/PowerGen/Discrete/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/PropDBN/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/PropDBN/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/RaceCar/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/RaceCar/instance0.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/RaceCar/instance1.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/RaceCar/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/RecSim/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/RecSim/instance0.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/RecSim/instance1.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/RecSim/instance2.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/RecSim/instance2.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Continuous/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Continuous/instance1.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Continuous/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Discrete/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Discrete/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Reservoir/Discrete/instance1.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Reservoir/Discrete/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChain/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChain/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChain/instance0.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChain/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChainNet/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChainNet/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/SupplyChainNet/instance0.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/SupplyChainNet/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance0.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance1.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance2.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance2.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/Experiments/webster_exp_equal_split.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/Experiments/webster_exp_equal_split.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/instance0.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/instance1.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Traffic/netgen.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Traffic/netgen.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Continuous/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Continuous/instance0.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Continuous/instance1.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Continuous/instance1.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Discrete/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Discrete/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Discrete/instance0.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Discrete/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Mixed/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Mixed/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/UAV/Mixed/instance0.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/UAV/Mixed/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Wildfire/domain.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Wildfire/domain.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Examples/Wildfire/instance0.rddl` & `pyRDDLGym-1.0.55/pyRDDLGym/Examples/Wildfire/instance0.rddl`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/GymExample.py` & `pyRDDLGym-1.0.55/pyRDDLGym/GymExample.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,23 +16,25 @@
     log = False if method_name is None else True
     myEnv = RDDLEnv.RDDLEnv(domain=EnvInfo.get_domain(), 
                             instance=EnvInfo.get_instance(inst),
                             enforce_action_constraints=False,
                             debug=False,
                             log=log,
                             simlogname=method_name)
+    myEnv.seed(42)
     
     # set up the environment visualizer
     # frames_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'Visualizer', 'Frames')
     myEnv.set_visualizer(EnvInfo.get_visualizer())
                         # movie_gen=MovieGenerator(frames_path, ENV, 200), movie_per_episode=True)
     
     # set up an example aget
     agent = RandomAgent(action_space=myEnv.action_space, 
-                        num_actions=myEnv.numConcurrentActions)
+                        num_actions=myEnv.numConcurrentActions,
+                        seed=42)
 
     for episode in range(episodes):
         total_reward = 0
         state = myEnv.reset()
         for step in range(myEnv.horizon):
             myEnv.render()
             action = agent.sample_action()
```

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/JaxExample.py` & `pyRDDLGym-1.0.55/pyRDDLGym/JaxExample.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     #                           batch_size=64, logic=planner.logic)
     # error.summarize(key, params)
     # error.sensitivity(key, params)
     return params
 
 
 def slp_no_replan(env, trials, timeout, timeout_ps, save):
-    myEnv, planner, train_args, (dom, inst) = JaxConfigManager.get(f'{env}.cfg')
+    myEnv, planner, _, _, train_args, (dom, inst) = JaxConfigManager.get(f'{env}.cfg')
     key = train_args['key']    
     
     rewards = np.zeros((myEnv.horizon, trials))
     for trial in range(trials):
         print('\n' + '*' * 30 + '\n' + f'starting trial {trial + 1}\n' + '*' * 30)
         train_args['key'] = key
         params = slp_train(planner, timeout, **train_args)
@@ -81,15 +81,15 @@
         
     myEnv.close()
     if save:
         np.savetxt(f'{dom}_{inst}_slp.csv', rewards, delimiter=',')
 
     
 def slp_replan(env, trials, timeout, timeout_ps, save):
-    myEnv, planner, train_args, (dom, inst) = JaxConfigManager.get(f'{env}.cfg')
+    myEnv, planner, _, _, train_args, (dom, inst) = JaxConfigManager.get(f'{env}.cfg')
     key = train_args['key']
     
     rewards = np.zeros((myEnv.horizon, trials))
     for trial in range(trials):
         print('\n' + '*' * 30 + '\n' + f'starting trial {trial + 1}\n' + '*' * 30)
         total_reward = 0
         state = myEnv.reset()
```

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/JaxLossPlotExample.py` & `pyRDDLGym-1.0.55/pyRDDLGym/JaxLossPlotExample.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,15 @@
     count_entries = sum(sizes.values())
     return shapes, starts, sizes, count_entries
 
     
 def loss_surface(problem, w=None, wa=None, train=True):
     
     # create the planning problem but non-aggregated return
-    _, planner, train_args, _ = JaxConfigManager.get(
-        f'{problem}.cfg')
+    _, planner, _, _, train_args, _ = JaxConfigManager.get(f'{problem}.cfg')
     
     model_params = planner.compiled.model_params
     if w is not None:
         model_params = {name: w for name in model_params}
         
     hyperparams = train_args.get('policy_hyperparams', {})
     if wa is not None:
@@ -91,15 +90,15 @@
 
 
 def run_experiment(problem, probname,
                    xmax=25.0, n=500, iters=100,
                    ws=[(100.0, 5.0), (100.0, 5.0), (10000.0, 100.0)]):
     
     # solve with default parameters
-    _, planner, train_args, _ = JaxConfigManager.get(f'{problem}.cfg')
+    _, planner, _, _, train_args, _ = JaxConfigManager.get(f'{problem}.cfg')
     sol_params = slp_train(planner, 60, **train_args)
     
     # reshape to solution vector
     _, starts, sizes, count_entries = _shape_info(planner)
     center = np.zeros((count_entries,))
     for name, value in sol_params.items():
         start = starts[name]
```

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Planner/JaxConfigManager.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Planner/JaxConfigManager.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,93 +9,102 @@
 
 from pyRDDLGym.Core.Env.RDDLEnv import RDDLEnv
 from pyRDDLGym.Core.Jax import JaxRDDLBackpropPlanner
 from pyRDDLGym.Core.Jax import JaxRDDLLogic
 from pyRDDLGym.Examples.ExampleManager import ExampleManager
 
 
-def get(path: str, **optional_args) -> Dict[str, object]:
-    
-    # read the config file
+def load_config_file(path: str):
     path = os.path.join(os.path.dirname(os.path.abspath(__file__)), path)
     config = configparser.RawConfigParser()
     config.optionxform = str 
     config.read(path)
     args = {k: literal_eval(v) 
             for section in config.sections()
-                for (k, v) in config.items(section)}
-    
-    # read the environment settings
-    env_args = {k: args[k] for (k, v) in config.items('Environment')}
-    use_repo = env_args.get('check_rddlrepository', False)
-    if 'check_rddlrepository' in env_args:
-        del env_args['check_rddlrepository']
-    
-    # try to read from rddlrepository
-    domain_name = env_args['domain']
-    inst_name = env_args['instance']
-    try:
-        if not use_repo:
+            for (k, v) in config.items(section)}
+    return config, args
+
+
+def read_config_sections(config, args):
+    env_args = {k: args[k] for (k, _) in config.items('Environment')} 
+    model_args = {k: args[k] for (k, _) in config.items('Model')}
+    planner_args = {k: args[k] for (k, _) in config.items('Optimizer')}
+    train_args = {k: args[k] for (k, _) in config.items('Training')}
+    return env_args, model_args, planner_args, train_args
+
+
+def load_rddl_files(check_external, domain_name, inst_name):
+    try: 
+        # try to read from external rddlrepository  
+        if not check_external:
             raise Exception
-        warnings.warn(f'reading domain {domain_name} from rddlrepository...',
-                      stacklevel=2)
+        warnings.warn(f'reading {domain_name} from rddlrepository...', stacklevel=2)
         from rddlrepository.Manager.RDDLRepoManager import RDDLRepoManager
         manager = RDDLRepoManager()
         EnvInfo = manager.get_problem(domain_name)
-    except:
+    except: 
+        # default to embedded RDDL manager
         warnings.warn(f'failed to read from rddlrepository, '
-                      f'reading domain {domain_name} from Examples...',
-                      stacklevel=2)
-        EnvInfo = ExampleManager.GetEnvInfo(domain_name)
-    
-    env_args['domain'] = EnvInfo.get_domain()
-    env_args['instance'] = EnvInfo.get_instance(inst_name)
-        
+                      f'reading {domain_name} from Examples...', stacklevel=2)
+        EnvInfo = ExampleManager.GetEnvInfo(domain_name)        
+    domain = EnvInfo.get_domain()
+    instance = EnvInfo.get_instance(inst_name)
+    return domain, instance
+
+
+def get(path: str, 
+        new_env_kwargs={}, new_logic_kwargs={}, 
+        new_plan_kwargs={}, new_planner_kwargs={}) -> Dict[str, object]:
+    
+    # load the config file
+    config, args = load_config_file(path)
+    env_args, model_args, planner_args, train_args = read_config_sections(config, args)
+    
+    # read the environment settings
+    check_external = env_args.pop('check_rddlrepository', False)
+    domain_name = env_args['domain']
+    inst_name = env_args['instance']
+    env_args['domain'], env_args['instance'] = load_rddl_files(
+        check_external, domain_name, inst_name)
+    env_args.update(new_env_kwargs)
     myEnv = RDDLEnv(**env_args)
-    # myEnv.set_visualizer(EnvInfo.get_visualizer())
+    planner_args['rddl'] = myEnv.model
     
     # read the model settings
-    model_args = {k: args[k] for (k, v) in config.items('Model')}
-    tnorm = getattr(JaxRDDLLogic, model_args['tnorm'])(
-        **model_args['tnorm_kwargs'])
-    logic = getattr(JaxRDDLLogic, model_args['logic'])(
-        tnorm=tnorm, **model_args['logic_kwargs'])
+    tnorm_name = model_args['tnorm']
+    tnorm_kwargs = model_args['tnorm_kwargs']
+    logic_name = model_args['logic']
+    logic_kwargs = model_args['logic_kwargs']
+    logic_kwargs['tnorm'] = getattr(JaxRDDLLogic, tnorm_name)(**tnorm_kwargs)
+    logic_kwargs.update(new_logic_kwargs)
+    planner_args['logic'] = getattr(JaxRDDLLogic, logic_name)(**logic_kwargs)
     
     # read the optimizer settings
-    opt_args = {k: args[k] for (k, v) in config.items('Optimizer')}
-    opt_args['rddl'] = myEnv.model
-    if 'method_kwargs' in opt_args and 'initializer' in opt_args['method_kwargs']:
-        init_method = opt_args['method_kwargs']['initializer']
-        initializer = getattr(initializers, init_method)
-        try:       
-            initializer = initializer(
-                **opt_args['method_kwargs']['initializer_kwargs'])
+    plan_method = planner_args.pop('method')
+    plan_kwargs = planner_args.pop('method_kwargs', {})  
+    
+    if 'initializer' in plan_kwargs:  # weight initialization
+        init_name = plan_kwargs['initializer']
+        init_class = getattr(initializers, init_name)
+        init_kwargs = plan_kwargs.pop('initializer_kwargs', {})
+        try: 
+            plan_kwargs['initializer'] = init_class(**init_kwargs)
         except:
-            warnings.warn(f'warning: initializer <{init_method}> '
-                          f'cannot take arguments, ignoring them.', stacklevel=2)
-        opt_args['method_kwargs']['initializer'] = initializer
-        if 'initializer_kwargs' in opt_args['method_kwargs']:
-            del opt_args['method_kwargs']['initializer_kwargs']
-            
-    if 'method_kwargs' in opt_args and 'activation' in opt_args['method_kwargs']:
-        opt_args['method_kwargs']['activation'] = getattr(
-            jax.nn, opt_args['method_kwargs']['activation'])
-        
-    opt_args['plan'] = getattr(JaxRDDLBackpropPlanner, opt_args['method'])(
-        **opt_args['method_kwargs'])
-    opt_args['optimizer'] = getattr(optax, opt_args['optimizer'])
-    opt_args['logic'] = logic
-    
-    del opt_args['method']
-    del opt_args['method_kwargs']
-    if optional_args is not None:
-        for name, value in optional_args.items():
-            opt_args[name] = value
-    optimizer = JaxRDDLBackpropPlanner.JaxRDDLBackpropPlanner(**opt_args)
+            warnings.warn(f'ignoring arguments for initializer <{init_name}>',
+                          stacklevel=2)
+            plan_kwargs['initializer'] = init_class
+               
+    if 'activation' in plan_kwargs:  # activation function
+        plan_kwargs['activation'] = getattr(jax.nn, plan_kwargs['activation'])
+    
+    plan_kwargs.update(new_plan_kwargs)
+    planner_args['plan'] = getattr(JaxRDDLBackpropPlanner, plan_method)(**plan_kwargs)
+    planner_args['optimizer'] = getattr(optax, planner_args['optimizer'])
+    planner_args.update(new_planner_kwargs)
+    planner = JaxRDDLBackpropPlanner.JaxRDDLBackpropPlanner(**planner_args)
     
-    # read the train/test arguments
-    train_args = {k: args[k] for (k, v) in config.items('Training')}
+    # read the training settings
     train_args['key'] = jax.random.PRNGKey(train_args['key'])
     
-    return myEnv, optimizer, train_args, (domain_name, inst_name)
-
+    return myEnv, planner, planner_args, plan_kwargs, train_args, \
+        (domain_name, inst_name)
```

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Policies/Agents.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Policies/Agents.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,21 +11,22 @@
         pass
 
 
 class RandomAgent(BaseAgent):
     def __init__(self, action_space, num_actions=1, seed=None):
         self.action_space = action_space
         self.num_actions = num_actions
+        self.rng = random.Random(seed)
         if seed is not None:
             self.action_space.seed(seed)
 
     def sample_action(self, state=None):
         s = self.action_space.sample()
         action = {}
-        selected_actions = random.sample(list(s), self.num_actions)
+        selected_actions = self.rng.sample(list(s), self.num_actions)
         for sample in selected_actions:
             if isinstance(self.action_space[sample], gym.spaces.Box):
                 action[sample] = s[sample][0].item()
             elif isinstance(self.action_space[sample], gym.spaces.Discrete):
                 action[sample] = s[sample]
                 # if str(self.action_space[sample]) == 'Discrete(2)':
                 #     action[sample] = bool(s[sample])
```

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Policies/RDDLSimAgent.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Policies/RDDLSimAgent.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/CartPoleViz.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/CartPoleViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/ChartViz.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/ChartViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/ColorViz.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/ColorViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/ElevatorViz.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/ElevatorViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/HVACViz.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/HVACViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/MarsRoverViz.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/MarsRoverViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/MountainCarViz.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/MountainCarViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/MovieGenerator.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/MovieGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/PowerGenViz.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/PowerGenViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/RacecarViz.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/RacecarViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/RecSimViz.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/RecSimViz.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         # print(self._creator_satisfaction)
         rel_sizes = rel_sizes / np.sum(rel_sizes)
         # print(self._user_interests)
         if self._user_plot is None:
             self._user_plot = self._ax_scatter.scatter(
                 self._user_interests[:, 0],
                 self._user_interests[:, 1],
-                s=reward,
+                s=np.maximum(reward, 0.),
                 c=20 * np.sqrt(np.maximum(reward, 0.)),
                 cmap='plasma',
                 edgecolors='black')
         # print(self._creator_means[:, 0],
         #     self._creator_means[:, 1], rel_sizes)
         self._creator_plot = self._ax_scatter.scatter(
             self._creator_means[:, 0],
```

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/ReservoirViz.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/ReservoirViz.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,15 +217,15 @@
         lineR = plt.Line2D((init_x + interval, init_x + interval), (init_y, init_y + interval), color='black', lw=0.5)
         lineB = plt.Line2D((init_x, init_x + interval), (init_y, init_y), color='black', lw=0.5)
 
         water_rect = plt.Rectangle((init_x, init_y), interval, rlevel / 120 * interval, fc='royalblue')
         res_rect = plt.Rectangle((init_x, init_y), interval, interval, fc='lightgrey', alpha=0.5)
         # scale_rect = plt.Rectangle((init_x, init_y + interval), interval/2, interval/4, fc='deepskyblue', alpha=rain_scale/50)
         shape_rect = plt.Rectangle((init_x, init_y + interval), interval, interval / 4, fc='darkcyan',
-                                   alpha=rain_shape / 50)
+                                   alpha=np.clip(rain_shape / 50, 0, 1))
 
         ax.add_line(line_max)
         ax.add_line(line_up)
         ax.add_line(line_low)
         ax.add_line(lineL)
         ax.add_line(lineR)
         ax.add_line(lineB)
```

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/StateViz.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/StateViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/TextViz.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/TextViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/TrafficViz.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/TrafficViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/UAVsViz.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/UAVsViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/WildfireViz.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/WildfireViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/Visualizer/visualize_dbn.py` & `pyRDDLGym-1.0.55/pyRDDLGym/Visualizer/visualize_dbn.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/XADD/RDDLLevelAnalysisXADD.py` & `pyRDDLGym-1.0.55/pyRDDLGym/XADD/RDDLLevelAnalysisXADD.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/XADD/RDDLModelXADD.py` & `pyRDDLGym-1.0.55/pyRDDLGym/XADD/RDDLModelXADD.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/XADD/RDDLSimulatorXADD.py` & `pyRDDLGym-1.0.55/pyRDDLGym/XADD/RDDLSimulatorXADD.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/testDiscrete.py` & `pyRDDLGym-1.0.55/pyRDDLGym/tests/testDiscrete.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/tests/RDDLGenerator.py` & `pyRDDLGym-1.0.55/pyRDDLGym/tests/RDDLGenerator.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/tests/_deprecated.py` & `pyRDDLGym-1.0.55/pyRDDLGym/tests/_deprecated.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/tests/testGymDrone.py` & `pyRDDLGym-1.0.55/pyRDDLGym/tests/testGymDrone.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/tests/testViz.py` & `pyRDDLGym-1.0.55/pyRDDLGym/tests/testViz.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/tests/test_basic.py` & `pyRDDLGym-1.0.55/pyRDDLGym/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/tests/test_dbn_vis.py` & `pyRDDLGym-1.0.55/pyRDDLGym/tests/test_dbn_vis.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/tests/test_termination.py` & `pyRDDLGym-1.0.55/pyRDDLGym/tests/test_termination.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/tests/test_xadd.py` & `pyRDDLGym-1.0.55/pyRDDLGym/tests/test_xadd.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/tests/unit_test_mars_rover.py` & `pyRDDLGym-1.0.55/pyRDDLGym/tests/unit_test_mars_rover.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym/tests/unit_test_power_gen.py` & `pyRDDLGym-1.0.55/pyRDDLGym/tests/unit_test_power_gen.py`

 * *Files identical despite different names*

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym.egg-info/PKG-INFO` & `pyRDDLGym-1.0.55/pyRDDLGym.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRDDLGym
-Version: 1.0.5
+Version: 1.0.55
 Summary: pyRDDLGym: RDDL automatic generation tool for OpenAI Gym
 Home-page: https://github.com/ataitler/pyRDDLGym
 Author: Ayal Taitler, Michael Gimelfarb, Scott Sanner, Jihwan Jeong, Sriram Gopalakrishnan, Martin Mladenov, jack liu
 Author-email: ataitler@gmail.com, mike.gimelfarb@mail.utoronto.ca, ssanner@mie.utoronto.ca, jhjeong@mie.utoronto.ca, sriram.gopalakrishnan@jpmchase.com, mmladenov@google.com, xiaotian.liu@mail.utoronto.ca
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pyRDDLGym-1.0.5/pyRDDLGym.egg-info/SOURCES.txt` & `pyRDDLGym-1.0.55/pyRDDLGym.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 LICENSE.MD
 MANIFEST.in
 README.md
 setup.py
 pyRDDLGym/GymExample.py
+pyRDDLGym/InstGenExample.py
 pyRDDLGym/JaxExample.py
 pyRDDLGym/JaxLossPlotExample.py
 pyRDDLGym/JaxTuningExample.py
 pyRDDLGym/RDDLSimClientExample.py
 pyRDDLGym/__init__.py
-pyRDDLGym/testDiscrete.py
 pyRDDLGym.egg-info/PKG-INFO
 pyRDDLGym.egg-info/SOURCES.txt
 pyRDDLGym.egg-info/dependency_links.txt
 pyRDDLGym.egg-info/requires.txt
 pyRDDLGym.egg-info/top_level.txt
 pyRDDLGym/Core/__init__.py
 pyRDDLGym/Core/Compiler/RDDLDecompiler.py
@@ -22,14 +22,15 @@
 pyRDDLGym/Core/Compiler/RDDLObjectsTracer.py
 pyRDDLGym/Core/Compiler/RDDLValueInitializer.py
 pyRDDLGym/Core/Compiler/__init__.py
 pyRDDLGym/Core/Debug/Logger.py
 pyRDDLGym/Core/Debug/__init__.py
 pyRDDLGym/Core/Env/RDDLConstraints.py
 pyRDDLGym/Core/Env/RDDLEnv.py
+pyRDDLGym/Core/Env/RDDLEnvSeeder.py
 pyRDDLGym/Core/Env/__init__.py
 pyRDDLGym/Core/ErrorHandling/RDDLException.py
 pyRDDLGym/Core/ErrorHandling/__init__.py
 pyRDDLGym/Core/Grounder/RDDLGrounder.py
 pyRDDLGym/Core/Grounder/__init__.py
 pyRDDLGym/Core/Jax/JaxParameterTuning.py
 pyRDDLGym/Core/Jax/JaxRDDLBackpropPlanner.py
@@ -66,60 +67,81 @@
 pyRDDLGym/Examples/Elevators/domain.rddl
 pyRDDLGym/Examples/Elevators/instance0.rddl
 pyRDDLGym/Examples/Elevators/instance1.rddl
 pyRDDLGym/Examples/HVAC/domain.info
 pyRDDLGym/Examples/HVAC/domain.rddl
 pyRDDLGym/Examples/HVAC/instance0.rddl
 pyRDDLGym/Examples/HVAC/instance1.rddl
+pyRDDLGym/Examples/HVAC/instance1c.rddl
 pyRDDLGym/Examples/HVAC/instance2.rddl
+pyRDDLGym/Examples/HVAC/instance3c.rddl
+pyRDDLGym/Examples/HVAC/instance5c.rddl
 pyRDDLGym/Examples/InstanceGenerators/HVACInstanceGenerator.py
 pyRDDLGym/Examples/InstanceGenerators/MarsRoverInstanceGenerator.py
 pyRDDLGym/Examples/InstanceGenerators/MountainCarInstanceGenerator.py
 pyRDDLGym/Examples/InstanceGenerators/PowerGenInstanceGenerator.py
 pyRDDLGym/Examples/InstanceGenerators/RaceCarInstanceGenerator.py
-pyRDDLGym/Examples/InstanceGenerators/RecSimInstanceGen.py
+pyRDDLGym/Examples/InstanceGenerators/RecSimInstanceGenerator.py
 pyRDDLGym/Examples/InstanceGenerators/ReservoirInstanceGenerator.py
 pyRDDLGym/Examples/InstanceGenerators/UAVInstanceGenerator.py
 pyRDDLGym/Examples/InstanceGenerators/__init__.py
 pyRDDLGym/Examples/MarsRover/domain.info
 pyRDDLGym/Examples/MarsRover/domain.rddl
 pyRDDLGym/Examples/MarsRover/instance0.rddl
+pyRDDLGym/Examples/MarsRover/instance1c.rddl
+pyRDDLGym/Examples/MarsRover/instance3c.rddl
+pyRDDLGym/Examples/MarsRover/instance5c.rddl
 pyRDDLGym/Examples/MountainCar/domain.info
 pyRDDLGym/Examples/MountainCar/domain.rddl
 pyRDDLGym/Examples/MountainCar/domain_old.rddl
 pyRDDLGym/Examples/MountainCar/instance0.rddl
 pyRDDLGym/Examples/MountainCar/instance0_old.rddl
+pyRDDLGym/Examples/MountainCar/instance1c.rddl
+pyRDDLGym/Examples/MountainCar/instance3c.rddl
+pyRDDLGym/Examples/MountainCar/instance5c.rddl
 pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/domain.info
 pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/domain.rddl
 pyRDDLGym/Examples/NewLanguageExamples/NewLanguage/instance0.rddl
 pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/domain.info
 pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/domain.rddl
 pyRDDLGym/Examples/NewLanguageExamples/NewtonZero/instance0.rddl
 pyRDDLGym/Examples/PowerGen/Continuous/domain.info
 pyRDDLGym/Examples/PowerGen/Continuous/domain.rddl
 pyRDDLGym/Examples/PowerGen/Continuous/instance0.rddl
+pyRDDLGym/Examples/PowerGen/Continuous/instance1c.rddl
+pyRDDLGym/Examples/PowerGen/Continuous/instance3c.rddl
+pyRDDLGym/Examples/PowerGen/Continuous/instance5c.rddl
 pyRDDLGym/Examples/PowerGen/Discrete/domain.info
 pyRDDLGym/Examples/PowerGen/Discrete/domain.rddl
 pyRDDLGym/Examples/PowerGen/Discrete/instance0.rddl
 pyRDDLGym/Examples/PropDBN/domain.info
 pyRDDLGym/Examples/PropDBN/domain.rddl
 pyRDDLGym/Examples/PropDBN/instance0.rddl
 pyRDDLGym/Examples/RaceCar/domain.info
 pyRDDLGym/Examples/RaceCar/domain.rddl
 pyRDDLGym/Examples/RaceCar/instance0.rddl
 pyRDDLGym/Examples/RaceCar/instance1.rddl
+pyRDDLGym/Examples/RaceCar/instance1c.rddl
+pyRDDLGym/Examples/RaceCar/instance3c.rddl
+pyRDDLGym/Examples/RaceCar/instance5c.rddl
 pyRDDLGym/Examples/RecSim/domain.info
 pyRDDLGym/Examples/RecSim/domain.rddl
 pyRDDLGym/Examples/RecSim/instance0.rddl
 pyRDDLGym/Examples/RecSim/instance1.rddl
+pyRDDLGym/Examples/RecSim/instance1c.rddl
 pyRDDLGym/Examples/RecSim/instance2.rddl
+pyRDDLGym/Examples/RecSim/instance3c.rddl
+pyRDDLGym/Examples/RecSim/instance5c.rddl
 pyRDDLGym/Examples/Reservoir/Continuous/domain.info
 pyRDDLGym/Examples/Reservoir/Continuous/domain.rddl
 pyRDDLGym/Examples/Reservoir/Continuous/instance0.rddl
 pyRDDLGym/Examples/Reservoir/Continuous/instance1.rddl
+pyRDDLGym/Examples/Reservoir/Continuous/instance1c.rddl
+pyRDDLGym/Examples/Reservoir/Continuous/instance3c.rddl
+pyRDDLGym/Examples/Reservoir/Continuous/instance5c.rddl
 pyRDDLGym/Examples/Reservoir/Discrete/domain.info
 pyRDDLGym/Examples/Reservoir/Discrete/domain.rddl
 pyRDDLGym/Examples/Reservoir/Discrete/instance0.rddl
 pyRDDLGym/Examples/Reservoir/Discrete/instance1.rddl
 pyRDDLGym/Examples/SupplyChain/domain.info
 pyRDDLGym/Examples/SupplyChain/domain.rddl
 pyRDDLGym/Examples/SupplyChain/instance0.rddl
@@ -137,14 +159,17 @@
 pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance1.rddl
 pyRDDLGym/Examples/Traffic/Deprecated/GenericPhasingScheme/instance2.rddl
 pyRDDLGym/Examples/Traffic/Experiments/webster_exp_equal_split.rddl
 pyRDDLGym/Examples/UAV/Continuous/domain.info
 pyRDDLGym/Examples/UAV/Continuous/domain.rddl
 pyRDDLGym/Examples/UAV/Continuous/instance0.rddl
 pyRDDLGym/Examples/UAV/Continuous/instance1.rddl
+pyRDDLGym/Examples/UAV/Continuous/instance1c.rddl
+pyRDDLGym/Examples/UAV/Continuous/instance3c.rddl
+pyRDDLGym/Examples/UAV/Continuous/instance5c.rddl
 pyRDDLGym/Examples/UAV/Discrete/domain.info
 pyRDDLGym/Examples/UAV/Discrete/domain.rddl
 pyRDDLGym/Examples/UAV/Discrete/instance0.rddl
 pyRDDLGym/Examples/UAV/Mixed/domain.info
 pyRDDLGym/Examples/UAV/Mixed/domain.rddl
 pyRDDLGym/Examples/UAV/Mixed/instance0.rddl
 pyRDDLGym/Examples/Wildfire/domain.info
@@ -177,15 +202,18 @@
 pyRDDLGym/XADD/RDDLLevelAnalysisXADD.py
 pyRDDLGym/XADD/RDDLModelXADD.py
 pyRDDLGym/XADD/RDDLSimulatorXADD.py
 pyRDDLGym/XADD/__init__.py
 pyRDDLGym/tests/RDDLGenerator.py
 pyRDDLGym/tests/__init__.py
 pyRDDLGym/tests/_deprecated.py
+pyRDDLGym/tests/testDiscrete.py
 pyRDDLGym/tests/testGymDrone.py
 pyRDDLGym/tests/testViz.py
 pyRDDLGym/tests/test_basic.py
 pyRDDLGym/tests/test_dbn_vis.py
 pyRDDLGym/tests/test_termination.py
 pyRDDLGym/tests/test_xadd.py
 pyRDDLGym/tests/unit_test_mars_rover.py
-pyRDDLGym/tests/unit_test_power_gen.py
+pyRDDLGym/tests/unit_test_power_gen.py
+pyRDDLGym/tests/seeding/Seedtest.py
+pyRDDLGym/tests/seeding/__init__.py
```

### Comparing `pyRDDLGym-1.0.5/setup.py` & `pyRDDLGym-1.0.55/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from setuptools import setup, find_packages
 
 # with open("README.md", "r", encoding="utf-8") as fh:
 #     long_description = fh.read()
 
 setup(
       name='pyRDDLGym',
-      version='1.0.5',
+      version='1.0.55',
       author="Ayal Taitler, Michael Gimelfarb, Scott Sanner, Jihwan Jeong, Sriram Gopalakrishnan, Martin Mladenov, jack liu",
       author_email="ataitler@gmail.com, mike.gimelfarb@mail.utoronto.ca, ssanner@mie.utoronto.ca, jhjeong@mie.utoronto.ca, sriram.gopalakrishnan@jpmchase.com, mmladenov@google.com, xiaotian.liu@mail.utoronto.ca",
       description="pyRDDLGym: RDDL automatic generation tool for OpenAI Gym",
       # long_description=long_description,
       license="MIT License",
       url="https://github.com/ataitler/pyRDDLGym",
       packages=find_packages(),
```

