# Comparing `tmp/google_fhir_core-0.9.2-py3-none-any.whl.zip` & `tmp/google_fhir_core-0.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,95 +1,433 @@
-Zip file size: 323537 bytes, number of entries: 93
--rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/core/__init__.py
--rw-r--r--  2.0 unx    12193 b- defN 23-Apr-17 20:06 google/fhir/core/codes.py
--rw-r--r--  2.0 unx    18626 b- defN 23-Apr-17 20:06 google/fhir/core/extensions.py
--rw-r--r--  2.0 unx     2275 b- defN 23-Apr-17 20:06 google/fhir/core/extensions_test.py
--rw-r--r--  2.0 unx     7281 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_errors.py
--rw-r--r--  2.0 unx     5706 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_errors_test.py
--rw-r--r--  2.0 unx     7054 b- defN 23-Apr-17 20:06 google/fhir/core/references.py
--rw-r--r--  2.0 unx    19632 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/FhirPathLexer.py
--rw-r--r--  2.0 unx    66224 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/FhirPathParser.py
--rw-r--r--  2.0 unx     8088 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/FhirPathVisitor.py
--rw-r--r--  2.0 unx      579 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/__init__.py
--rw-r--r--  2.0 unx    39499 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_ast.py
--rw-r--r--  2.0 unx    12220 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_ast_test.py
--rw-r--r--  2.0 unx    25380 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_bigquery_interpreter.py
--rw-r--r--  2.0 unx    43338 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_bigquery_sql_functions.py
--rw-r--r--  2.0 unx    52892 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_evaluation.py
--rw-r--r--  2.0 unx    25010 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_fhir_path_data_types.py
--rw-r--r--  2.0 unx    59561 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_fhir_path_to_sql_functions.py
--rw-r--r--  2.0 unx    79712 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_interpreter_test_base.py
--rw-r--r--  2.0 unx    12297 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_navigation.py
--rw-r--r--  2.0 unx     8116 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_navigation_test.py
--rw-r--r--  2.0 unx    30292 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_python_interpreter.py
--rw-r--r--  2.0 unx    32521 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_semant.py
--rw-r--r--  2.0 unx    36633 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_semant_test.py
--rw-r--r--  2.0 unx    22613 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_spark_interpreter.py
--rw-r--r--  2.0 unx    13460 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_spark_sql_functions.py
--rw-r--r--  2.0 unx    34114 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_sql_data_types.py
--rw-r--r--  2.0 unx     7696 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_sql_data_types_test.py
--rw-r--r--  2.0 unx     6296 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_structure_definitions.py
--rw-r--r--  2.0 unx     9517 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_utils.py
--rw-r--r--  2.0 unx    11122 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_utils_test.py
--rw-r--r--  2.0 unx    14392 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/context.py
--rw-r--r--  2.0 unx     6461 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/context_test.py
--rw-r--r--  2.0 unx    27062 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/expressions.py
--rw-r--r--  2.0 unx    37619 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/fhir_path.py
--rw-r--r--  2.0 unx     1298 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/fhir_path_options.py
--rw-r--r--  2.0 unx    49814 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/fhir_path_spark_test.py
--rw-r--r--  2.0 unx   214354 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/fhir_path_test.py
--rw-r--r--  2.0 unx    16788 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/fhir_path_test_base.py
--rw-r--r--  2.0 unx    46839 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/fhir_path_validator.py
--rw-r--r--  2.0 unx    56541 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/fhir_path_validator_v2.py
--rw-r--r--  2.0 unx     1945 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/fhir_path_validator_v2_test.py
--rw-r--r--  2.0 unx     5908 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/python_compiled_expressions.py
--rw-r--r--  2.0 unx     3861 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/quantity.py
--rw-r--r--  2.0 unx     4404 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/quantity_test.py
--rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/core/internal/__init__.py
--rw-r--r--  2.0 unx     6663 b- defN 23-Apr-17 20:06 google/fhir/core/internal/_primitive_time_utils.py
--rw-r--r--  2.0 unx    14323 b- defN 23-Apr-17 20:06 google/fhir/core/internal/primitive_handler.py
--rw-r--r--  2.0 unx     8859 b- defN 23-Apr-17 20:06 google/fhir/core/internal/resource_validation.py
--rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/__init__.py
--rw-r--r--  2.0 unx    15207 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/_json_parser.py
--rw-r--r--  2.0 unx    15656 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/_json_printer.py
--rw-r--r--  2.0 unx     6464 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/json_format_test.py
--rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/wrappers/__init__.py
--rw-r--r--  2.0 unx     5417 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/wrappers/_base64_binary.py
--rw-r--r--  2.0 unx     4301 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/wrappers/_date.py
--rw-r--r--  2.0 unx     5736 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/wrappers/_date_time.py
--rw-r--r--  2.0 unx     2408 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/wrappers/_decimal.py
--rw-r--r--  2.0 unx     4502 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/wrappers/_instant.py
--rw-r--r--  2.0 unx    16137 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/wrappers/_primitive_wrappers.py
--rw-r--r--  2.0 unx     4791 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/wrappers/_time.py
--rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/core/proto/__init__.py
--rwxr-xr-x  2.0 unx     7697 b- defN 23-Apr-17 20:06 google/fhir/core/proto/annotations.proto
--rw-r--r--  2.0 unx     9188 b- defN 23-Apr-17 20:07 google/fhir/core/proto/annotations_pb2.py
--rw-r--r--  2.0 unx     1576 b- defN 23-Apr-17 20:06 google/fhir/core/proto/fhirpath_replacement_list.proto
--rw-r--r--  2.0 unx     1411 b- defN 23-Apr-17 20:07 google/fhir/core/proto/fhirpath_replacement_list_pb2.py
--rw-r--r--  2.0 unx     4935 b- defN 23-Apr-17 20:06 google/fhir/core/proto/validation.proto
--rw-r--r--  2.0 unx     2354 b- defN 23-Apr-17 20:07 google/fhir/core/proto/validation_pb2.py
--rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/core/testing/__init__.py
--rw-r--r--  2.0 unx     6706 b- defN 23-Apr-17 20:06 google/fhir/core/testing/protobuf_compare.py
--rw-r--r--  2.0 unx     3745 b- defN 23-Apr-17 20:06 google/fhir/core/testing/testdata_utils.py
--rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/core/utils/__init__.py
--rw-r--r--  2.0 unx    13789 b- defN 23-Apr-17 20:06 google/fhir/core/utils/annotation_utils.py
--rw-r--r--  2.0 unx    15883 b- defN 23-Apr-17 20:06 google/fhir/core/utils/annotation_utils_test.py
--rw-r--r--  2.0 unx    17494 b- defN 23-Apr-17 20:06 google/fhir/core/utils/fhir_package.py
--rw-r--r--  2.0 unx    23767 b- defN 23-Apr-17 20:06 google/fhir/core/utils/fhir_package_test_base.py
--rw-r--r--  2.0 unx     9127 b- defN 23-Apr-17 20:06 google/fhir/core/utils/fhir_types.py
--rw-r--r--  2.0 unx     7750 b- defN 23-Apr-17 20:06 google/fhir/core/utils/fhir_types_test.py
--rw-r--r--  2.0 unx     1637 b- defN 23-Apr-17 20:06 google/fhir/core/utils/path_utils.py
--rw-r--r--  2.0 unx     1922 b- defN 23-Apr-17 20:06 google/fhir/core/utils/path_utils_test.py
--rw-r--r--  2.0 unx    12011 b- defN 23-Apr-17 20:06 google/fhir/core/utils/proto_utils.py
--rw-r--r--  2.0 unx    15754 b- defN 23-Apr-17 20:06 google/fhir/core/utils/proto_utils_test.py
--rw-r--r--  2.0 unx     3040 b- defN 23-Apr-17 20:06 google/fhir/core/utils/resource_utils.py
--rw-r--r--  2.0 unx     3789 b- defN 23-Apr-17 20:06 google/fhir/core/utils/resource_utils_test.py
--rw-r--r--  2.0 unx     1876 b- defN 23-Apr-17 20:06 google/fhir/core/utils/url_utils.py
--rw-r--r--  2.0 unx     1870 b- defN 23-Apr-17 20:06 google/fhir/core/utils/url_utils_test.py
--rwxr-xr-x  2.0 unx     7697 b- defN 23-Apr-17 20:06 google_fhir_core-0.9.2.data/data/annotations.proto
--rw-r--r--  2.0 unx     1576 b- defN 23-Apr-17 20:06 google_fhir_core-0.9.2.data/data/fhirpath_replacement_list.proto
--rw-r--r--  2.0 unx     4935 b- defN 23-Apr-17 20:06 google_fhir_core-0.9.2.data/data/validation.proto
--rw-r--r--  2.0 unx     1311 b- defN 23-Apr-17 20:07 google_fhir_core-0.9.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 20:07 google_fhir_core-0.9.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-17 20:07 google_fhir_core-0.9.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     9443 b- defN 23-Apr-17 20:07 google_fhir_core-0.9.2.dist-info/RECORD
-93 files, 1504118 bytes uncompressed, 308107 bytes compressed:  79.5%
+Zip file size: 1652466 bytes, number of entries: 431
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/__init__.py
+-rw-r--r--  2.0 unx    12193 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/codes.py
+-rw-r--r--  2.0 unx    18626 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/extensions.py
+-rw-r--r--  2.0 unx     2275 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/extensions_test.py
+-rw-r--r--  2.0 unx     7281 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_errors.py
+-rw-r--r--  2.0 unx     5706 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_errors_test.py
+-rw-r--r--  2.0 unx     7054 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/references.py
+-rw-r--r--  2.0 unx    19632 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/FhirPathLexer.py
+-rw-r--r--  2.0 unx    66224 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/FhirPathParser.py
+-rw-r--r--  2.0 unx     8088 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/FhirPathVisitor.py
+-rw-r--r--  2.0 unx      579 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/__init__.py
+-rw-r--r--  2.0 unx    39499 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_ast.py
+-rw-r--r--  2.0 unx    12220 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_ast_test.py
+-rw-r--r--  2.0 unx    25386 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_bigquery_interpreter.py
+-rw-r--r--  2.0 unx    43839 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_bigquery_sql_functions.py
+-rw-r--r--  2.0 unx    54784 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_evaluation.py
+-rw-r--r--  2.0 unx    33516 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_fhir_path_data_types.py
+-rw-r--r--  2.0 unx    11327 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_fhir_path_data_types_test.py
+-rw-r--r--  2.0 unx    59561 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_fhir_path_to_sql_functions.py
+-rw-r--r--  2.0 unx    80507 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_interpreter_test_base.py
+-rw-r--r--  2.0 unx    12297 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_navigation.py
+-rw-r--r--  2.0 unx     8116 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_navigation_test.py
+-rw-r--r--  2.0 unx    30292 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_python_interpreter.py
+-rw-r--r--  2.0 unx    33496 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_semant.py
+-rw-r--r--  2.0 unx    36633 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_semant_test.py
+-rw-r--r--  2.0 unx    24909 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_spark_interpreter.py
+-rw-r--r--  2.0 unx    34795 b- defN 23-May-24 11:23 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_spark_sql_functions.py
+-rw-r--r--  2.0 unx    34090 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_sql_data_types.py
+-rw-r--r--  2.0 unx     7696 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_sql_data_types_test.py
+-rw-r--r--  2.0 unx     6795 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_structure_definitions.py
+-rw-r--r--  2.0 unx     9761 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_utils.py
+-rw-r--r--  2.0 unx    12624 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_utils_test.py
+-rw-r--r--  2.0 unx    15711 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/context.py
+-rw-r--r--  2.0 unx     6529 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/context_test.py
+-rw-r--r--  2.0 unx    27285 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/expressions.py
+-rw-r--r--  2.0 unx    37619 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path.py
+-rw-r--r--  2.0 unx     1298 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_options.py
+-rw-r--r--  2.0 unx    72916 b- defN 23-May-24 11:23 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_spark_test.py
+-rw-r--r--  2.0 unx   236601 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_test.py
+-rw-r--r--  2.0 unx    18356 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_test_base.py
+-rw-r--r--  2.0 unx    46839 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_validator.py
+-rw-r--r--  2.0 unx    61107 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_validator_v2.py
+-rw-r--r--  2.0 unx     1945 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_validator_v2_test.py
+-rw-r--r--  2.0 unx     5908 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/python_compiled_expressions.py
+-rw-r--r--  2.0 unx     3861 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/quantity.py
+-rw-r--r--  2.0 unx     4404 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/quantity_test.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/__init__.py
+-rw-r--r--  2.0 unx     6663 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/_primitive_time_utils.py
+-rw-r--r--  2.0 unx    14323 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/primitive_handler.py
+-rw-r--r--  2.0 unx     8859 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/resource_validation.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/__init__.py
+-rw-r--r--  2.0 unx    15207 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/_json_parser.py
+-rw-r--r--  2.0 unx    15656 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/_json_printer.py
+-rw-r--r--  2.0 unx     6464 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/json_format_test.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/__init__.py
+-rw-r--r--  2.0 unx     5417 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_base64_binary.py
+-rw-r--r--  2.0 unx     4301 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_date.py
+-rw-r--r--  2.0 unx     5736 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_date_time.py
+-rw-r--r--  2.0 unx     2408 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_decimal.py
+-rw-r--r--  2.0 unx     4502 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_instant.py
+-rw-r--r--  2.0 unx    16137 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_primitive_wrappers.py
+-rw-r--r--  2.0 unx     4791 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_time.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/proto/__init__.py
+-rw-r--r--  2.0 unx     9188 b- defN 23-May-24 11:25 build/lib/build/lib/build/lib/build/lib/google/fhir/core/proto/annotations_pb2.py
+-rw-r--r--  2.0 unx     1411 b- defN 23-May-24 11:25 build/lib/build/lib/build/lib/build/lib/google/fhir/core/proto/fhirpath_replacement_list_pb2.py
+-rw-r--r--  2.0 unx     2354 b- defN 23-May-24 11:25 build/lib/build/lib/build/lib/build/lib/google/fhir/core/proto/validation_pb2.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/testing/__init__.py
+-rw-r--r--  2.0 unx     6706 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/testing/protobuf_compare.py
+-rw-r--r--  2.0 unx     3745 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/testing/testdata_utils.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/__init__.py
+-rw-r--r--  2.0 unx    13789 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/annotation_utils.py
+-rw-r--r--  2.0 unx    15883 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/annotation_utils_test.py
+-rw-r--r--  2.0 unx    17494 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/fhir_package.py
+-rw-r--r--  2.0 unx    23767 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/fhir_package_test_base.py
+-rw-r--r--  2.0 unx     9127 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/fhir_types.py
+-rw-r--r--  2.0 unx     7750 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/fhir_types_test.py
+-rw-r--r--  2.0 unx     1637 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/path_utils.py
+-rw-r--r--  2.0 unx     1922 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/path_utils_test.py
+-rw-r--r--  2.0 unx    12011 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/proto_utils.py
+-rw-r--r--  2.0 unx    15754 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/proto_utils_test.py
+-rw-r--r--  2.0 unx     3040 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/resource_utils.py
+-rw-r--r--  2.0 unx     3789 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/resource_utils_test.py
+-rw-r--r--  2.0 unx     1876 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/url_utils.py
+-rw-r--r--  2.0 unx     1870 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/url_utils_test.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/__init__.py
+-rw-r--r--  2.0 unx    12193 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/codes.py
+-rw-r--r--  2.0 unx    18626 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/extensions.py
+-rw-r--r--  2.0 unx     2275 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/extensions_test.py
+-rw-r--r--  2.0 unx     7281 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/fhir_errors.py
+-rw-r--r--  2.0 unx     5706 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/fhir_errors_test.py
+-rw-r--r--  2.0 unx     7054 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/references.py
+-rw-r--r--  2.0 unx    19632 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/FhirPathLexer.py
+-rw-r--r--  2.0 unx    66224 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/FhirPathParser.py
+-rw-r--r--  2.0 unx     8088 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/FhirPathVisitor.py
+-rw-r--r--  2.0 unx      579 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/__init__.py
+-rw-r--r--  2.0 unx    39499 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_ast.py
+-rw-r--r--  2.0 unx    12220 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_ast_test.py
+-rw-r--r--  2.0 unx    25666 b- defN 23-Jun-05 20:08 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_bigquery_interpreter.py
+-rw-r--r--  2.0 unx    43839 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_bigquery_sql_functions.py
+-rw-r--r--  2.0 unx    54784 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_evaluation.py
+-rw-r--r--  2.0 unx    33835 b- defN 23-Jun-05 20:08 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_fhir_path_data_types.py
+-rw-r--r--  2.0 unx    11827 b- defN 23-Jun-05 20:08 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_fhir_path_data_types_test.py
+-rw-r--r--  2.0 unx    59561 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_fhir_path_to_sql_functions.py
+-rw-r--r--  2.0 unx    80507 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_interpreter_test_base.py
+-rw-r--r--  2.0 unx    12297 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_navigation.py
+-rw-r--r--  2.0 unx     8116 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_navigation_test.py
+-rw-r--r--  2.0 unx    30292 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_python_interpreter.py
+-rw-r--r--  2.0 unx    33496 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_semant.py
+-rw-r--r--  2.0 unx    36633 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_semant_test.py
+-rw-r--r--  2.0 unx    24909 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_spark_interpreter.py
+-rw-r--r--  2.0 unx    35878 b- defN 23-Jun-05 20:08 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_spark_sql_functions.py
+-rw-r--r--  2.0 unx    34090 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_sql_data_types.py
+-rw-r--r--  2.0 unx     7696 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_sql_data_types_test.py
+-rw-r--r--  2.0 unx     6795 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_structure_definitions.py
+-rw-r--r--  2.0 unx     9761 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_utils.py
+-rw-r--r--  2.0 unx    12624 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_utils_test.py
+-rw-r--r--  2.0 unx    15711 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/context.py
+-rw-r--r--  2.0 unx     6529 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/context_test.py
+-rw-r--r--  2.0 unx    27285 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/expressions.py
+-rw-r--r--  2.0 unx    37619 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path.py
+-rw-r--r--  2.0 unx     1298 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_options.py
+-rw-r--r--  2.0 unx    72947 b- defN 23-Jun-05 20:08 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_spark_test.py
+-rw-r--r--  2.0 unx   239392 b- defN 23-Jun-05 20:08 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_test.py
+-rw-r--r--  2.0 unx    18356 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_test_base.py
+-rw-r--r--  2.0 unx    46839 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_validator.py
+-rw-r--r--  2.0 unx    61109 b- defN 23-Jun-05 20:08 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_validator_v2.py
+-rw-r--r--  2.0 unx     1945 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_validator_v2_test.py
+-rw-r--r--  2.0 unx     5908 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/python_compiled_expressions.py
+-rw-r--r--  2.0 unx     3861 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/quantity.py
+-rw-r--r--  2.0 unx     4404 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/fhir_path/quantity_test.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/internal/__init__.py
+-rw-r--r--  2.0 unx     6663 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/internal/_primitive_time_utils.py
+-rw-r--r--  2.0 unx    14323 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/internal/primitive_handler.py
+-rw-r--r--  2.0 unx     8859 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/internal/resource_validation.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/__init__.py
+-rw-r--r--  2.0 unx    15207 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/_json_parser.py
+-rw-r--r--  2.0 unx    15656 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/_json_printer.py
+-rw-r--r--  2.0 unx     6464 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/json_format_test.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/__init__.py
+-rw-r--r--  2.0 unx     5417 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_base64_binary.py
+-rw-r--r--  2.0 unx     4301 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_date.py
+-rw-r--r--  2.0 unx     5736 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_date_time.py
+-rw-r--r--  2.0 unx     2408 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_decimal.py
+-rw-r--r--  2.0 unx     4502 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_instant.py
+-rw-r--r--  2.0 unx    16137 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_primitive_wrappers.py
+-rw-r--r--  2.0 unx     4791 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_time.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/proto/__init__.py
+-rw-r--r--  2.0 unx     9188 b- defN 23-May-24 11:25 build/lib/build/lib/build/lib/google/fhir/core/proto/annotations_pb2.py
+-rw-r--r--  2.0 unx     1411 b- defN 23-May-24 11:25 build/lib/build/lib/build/lib/google/fhir/core/proto/fhirpath_replacement_list_pb2.py
+-rw-r--r--  2.0 unx     2354 b- defN 23-May-24 11:25 build/lib/build/lib/build/lib/google/fhir/core/proto/validation_pb2.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/testing/__init__.py
+-rw-r--r--  2.0 unx     6706 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/testing/protobuf_compare.py
+-rw-r--r--  2.0 unx     3745 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/testing/testdata_utils.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/utils/__init__.py
+-rw-r--r--  2.0 unx    13789 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/utils/annotation_utils.py
+-rw-r--r--  2.0 unx    15883 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/utils/annotation_utils_test.py
+-rw-r--r--  2.0 unx    17494 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/utils/fhir_package.py
+-rw-r--r--  2.0 unx    23767 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/utils/fhir_package_test_base.py
+-rw-r--r--  2.0 unx     9127 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/utils/fhir_types.py
+-rw-r--r--  2.0 unx     7750 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/utils/fhir_types_test.py
+-rw-r--r--  2.0 unx     1637 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/utils/path_utils.py
+-rw-r--r--  2.0 unx     1922 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/utils/path_utils_test.py
+-rw-r--r--  2.0 unx    12011 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/utils/proto_utils.py
+-rw-r--r--  2.0 unx    15754 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/core/utils/proto_utils_test.py
+-rw-r--r--  2.0 unx     3040 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/utils/resource_utils.py
+-rw-r--r--  2.0 unx     3789 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/utils/resource_utils_test.py
+-rw-r--r--  2.0 unx     1876 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/utils/url_utils.py
+-rw-r--r--  2.0 unx     1870 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/core/utils/url_utils_test.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/__init__.py
+-rw-r--r--  2.0 unx    12193 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/codes.py
+-rw-r--r--  2.0 unx    18626 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/extensions.py
+-rw-r--r--  2.0 unx     2275 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/extensions_test.py
+-rw-r--r--  2.0 unx     7281 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/fhir_errors.py
+-rw-r--r--  2.0 unx     5706 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/fhir_errors_test.py
+-rw-r--r--  2.0 unx     7054 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/references.py
+-rw-r--r--  2.0 unx    19632 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/fhir_path/FhirPathLexer.py
+-rw-r--r--  2.0 unx    66224 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/fhir_path/FhirPathParser.py
+-rw-r--r--  2.0 unx     8088 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/fhir_path/FhirPathVisitor.py
+-rw-r--r--  2.0 unx      579 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/fhir_path/__init__.py
+-rw-r--r--  2.0 unx    39499 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/_ast.py
+-rw-r--r--  2.0 unx    12220 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/_ast_test.py
+-rw-r--r--  2.0 unx    25666 b- defN 23-Jun-05 20:08 build/lib/build/lib/google/fhir/core/fhir_path/_bigquery_interpreter.py
+-rw-r--r--  2.0 unx    43839 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/_bigquery_sql_functions.py
+-rw-r--r--  2.0 unx    54784 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/_evaluation.py
+-rw-r--r--  2.0 unx    33835 b- defN 23-Jun-05 20:08 build/lib/build/lib/google/fhir/core/fhir_path/_fhir_path_data_types.py
+-rw-r--r--  2.0 unx    11827 b- defN 23-Jun-05 20:08 build/lib/build/lib/google/fhir/core/fhir_path/_fhir_path_data_types_test.py
+-rw-r--r--  2.0 unx    59561 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/_fhir_path_to_sql_functions.py
+-rw-r--r--  2.0 unx    80507 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/_interpreter_test_base.py
+-rw-r--r--  2.0 unx    12297 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/_navigation.py
+-rw-r--r--  2.0 unx     8116 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/fhir_path/_navigation_test.py
+-rw-r--r--  2.0 unx    30292 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/_python_interpreter.py
+-rw-r--r--  2.0 unx    33496 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/_semant.py
+-rw-r--r--  2.0 unx    36633 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/_semant_test.py
+-rw-r--r--  2.0 unx    24909 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/_spark_interpreter.py
+-rw-r--r--  2.0 unx    35878 b- defN 23-Jun-05 20:08 build/lib/build/lib/google/fhir/core/fhir_path/_spark_sql_functions.py
+-rw-r--r--  2.0 unx    34090 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/_sql_data_types.py
+-rw-r--r--  2.0 unx     7696 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/fhir_path/_sql_data_types_test.py
+-rw-r--r--  2.0 unx     6795 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/_structure_definitions.py
+-rw-r--r--  2.0 unx     9761 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/_utils.py
+-rw-r--r--  2.0 unx    12624 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/_utils_test.py
+-rw-r--r--  2.0 unx    15711 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/context.py
+-rw-r--r--  2.0 unx     6529 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/context_test.py
+-rw-r--r--  2.0 unx    27285 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/expressions.py
+-rw-r--r--  2.0 unx    37619 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/fhir_path.py
+-rw-r--r--  2.0 unx     1298 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_options.py
+-rw-r--r--  2.0 unx    72947 b- defN 23-Jun-05 20:08 build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_spark_test.py
+-rw-r--r--  2.0 unx   239392 b- defN 23-Jun-05 20:08 build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_test.py
+-rw-r--r--  2.0 unx    18356 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_test_base.py
+-rw-r--r--  2.0 unx    46839 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_validator.py
+-rw-r--r--  2.0 unx    61109 b- defN 23-Jun-05 20:08 build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_validator_v2.py
+-rw-r--r--  2.0 unx     1945 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_validator_v2_test.py
+-rw-r--r--  2.0 unx     5908 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/python_compiled_expressions.py
+-rw-r--r--  2.0 unx     3861 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/fhir_path/quantity.py
+-rw-r--r--  2.0 unx     4404 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/fhir_path/quantity_test.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/internal/__init__.py
+-rw-r--r--  2.0 unx     6663 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/internal/_primitive_time_utils.py
+-rw-r--r--  2.0 unx    14323 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/internal/primitive_handler.py
+-rw-r--r--  2.0 unx     8859 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/internal/resource_validation.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/internal/json_format/__init__.py
+-rw-r--r--  2.0 unx    15207 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/internal/json_format/_json_parser.py
+-rw-r--r--  2.0 unx    15656 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/internal/json_format/_json_printer.py
+-rw-r--r--  2.0 unx     6464 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/internal/json_format/json_format_test.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/__init__.py
+-rw-r--r--  2.0 unx     5417 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_base64_binary.py
+-rw-r--r--  2.0 unx     4301 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_date.py
+-rw-r--r--  2.0 unx     5736 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_date_time.py
+-rw-r--r--  2.0 unx     2408 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_decimal.py
+-rw-r--r--  2.0 unx     4502 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_instant.py
+-rw-r--r--  2.0 unx    16137 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_primitive_wrappers.py
+-rw-r--r--  2.0 unx     4791 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_time.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/proto/__init__.py
+-rw-r--r--  2.0 unx     9188 b- defN 23-May-24 11:25 build/lib/build/lib/google/fhir/core/proto/annotations_pb2.py
+-rw-r--r--  2.0 unx     1411 b- defN 23-May-24 11:25 build/lib/build/lib/google/fhir/core/proto/fhirpath_replacement_list_pb2.py
+-rw-r--r--  2.0 unx     2354 b- defN 23-May-24 11:25 build/lib/build/lib/google/fhir/core/proto/validation_pb2.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/testing/__init__.py
+-rw-r--r--  2.0 unx     6706 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/testing/protobuf_compare.py
+-rw-r--r--  2.0 unx     3745 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/testing/testdata_utils.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/utils/__init__.py
+-rw-r--r--  2.0 unx    13789 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/utils/annotation_utils.py
+-rw-r--r--  2.0 unx    15883 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/utils/annotation_utils_test.py
+-rw-r--r--  2.0 unx    17494 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/utils/fhir_package.py
+-rw-r--r--  2.0 unx    23767 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/utils/fhir_package_test_base.py
+-rw-r--r--  2.0 unx     9127 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/utils/fhir_types.py
+-rw-r--r--  2.0 unx     7750 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/utils/fhir_types_test.py
+-rw-r--r--  2.0 unx     1637 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/utils/path_utils.py
+-rw-r--r--  2.0 unx     1922 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/utils/path_utils_test.py
+-rw-r--r--  2.0 unx    12011 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/utils/proto_utils.py
+-rw-r--r--  2.0 unx    15754 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/core/utils/proto_utils_test.py
+-rw-r--r--  2.0 unx     3040 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/utils/resource_utils.py
+-rw-r--r--  2.0 unx     3789 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/utils/resource_utils_test.py
+-rw-r--r--  2.0 unx     1876 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/utils/url_utils.py
+-rw-r--r--  2.0 unx     1870 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/core/utils/url_utils_test.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/google/fhir/core/__init__.py
+-rw-r--r--  2.0 unx    12193 b- defN 23-May-18 18:49 build/lib/google/fhir/core/codes.py
+-rw-r--r--  2.0 unx    18626 b- defN 23-May-18 18:51 build/lib/google/fhir/core/extensions.py
+-rw-r--r--  2.0 unx     2275 b- defN 23-May-18 18:49 build/lib/google/fhir/core/extensions_test.py
+-rw-r--r--  2.0 unx     7281 b- defN 23-May-18 18:49 build/lib/google/fhir/core/fhir_errors.py
+-rw-r--r--  2.0 unx     5706 b- defN 23-May-18 18:49 build/lib/google/fhir/core/fhir_errors_test.py
+-rw-r--r--  2.0 unx     7054 b- defN 23-May-18 18:51 build/lib/google/fhir/core/references.py
+-rw-r--r--  2.0 unx    19632 b- defN 23-May-18 18:49 build/lib/google/fhir/core/fhir_path/FhirPathLexer.py
+-rw-r--r--  2.0 unx    66224 b- defN 23-May-18 18:49 build/lib/google/fhir/core/fhir_path/FhirPathParser.py
+-rw-r--r--  2.0 unx     8088 b- defN 23-May-18 18:49 build/lib/google/fhir/core/fhir_path/FhirPathVisitor.py
+-rw-r--r--  2.0 unx      579 b- defN 23-May-18 18:49 build/lib/google/fhir/core/fhir_path/__init__.py
+-rw-r--r--  2.0 unx    39499 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/_ast.py
+-rw-r--r--  2.0 unx    12220 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/_ast_test.py
+-rw-r--r--  2.0 unx    25666 b- defN 23-Jun-05 20:08 build/lib/google/fhir/core/fhir_path/_bigquery_interpreter.py
+-rw-r--r--  2.0 unx    43839 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/_bigquery_sql_functions.py
+-rw-r--r--  2.0 unx    54784 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/_evaluation.py
+-rw-r--r--  2.0 unx    33835 b- defN 23-Jun-05 20:08 build/lib/google/fhir/core/fhir_path/_fhir_path_data_types.py
+-rw-r--r--  2.0 unx    11827 b- defN 23-Jun-05 20:08 build/lib/google/fhir/core/fhir_path/_fhir_path_data_types_test.py
+-rw-r--r--  2.0 unx    59561 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/_fhir_path_to_sql_functions.py
+-rw-r--r--  2.0 unx    80507 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/_interpreter_test_base.py
+-rw-r--r--  2.0 unx    12297 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/_navigation.py
+-rw-r--r--  2.0 unx     8116 b- defN 23-May-18 18:49 build/lib/google/fhir/core/fhir_path/_navigation_test.py
+-rw-r--r--  2.0 unx    30292 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/_python_interpreter.py
+-rw-r--r--  2.0 unx    33496 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/_semant.py
+-rw-r--r--  2.0 unx    36633 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/_semant_test.py
+-rw-r--r--  2.0 unx    24909 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/_spark_interpreter.py
+-rw-r--r--  2.0 unx    35878 b- defN 23-Jun-05 20:08 build/lib/google/fhir/core/fhir_path/_spark_sql_functions.py
+-rw-r--r--  2.0 unx    34090 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/_sql_data_types.py
+-rw-r--r--  2.0 unx     7696 b- defN 23-May-18 18:49 build/lib/google/fhir/core/fhir_path/_sql_data_types_test.py
+-rw-r--r--  2.0 unx     6795 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/_structure_definitions.py
+-rw-r--r--  2.0 unx     9761 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/_utils.py
+-rw-r--r--  2.0 unx    12624 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/_utils_test.py
+-rw-r--r--  2.0 unx    15711 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/context.py
+-rw-r--r--  2.0 unx     6529 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/context_test.py
+-rw-r--r--  2.0 unx    27285 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/expressions.py
+-rw-r--r--  2.0 unx    37619 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/fhir_path.py
+-rw-r--r--  2.0 unx     1298 b- defN 23-May-18 18:49 build/lib/google/fhir/core/fhir_path/fhir_path_options.py
+-rw-r--r--  2.0 unx    72947 b- defN 23-Jun-05 20:08 build/lib/google/fhir/core/fhir_path/fhir_path_spark_test.py
+-rw-r--r--  2.0 unx   239392 b- defN 23-Jun-05 20:08 build/lib/google/fhir/core/fhir_path/fhir_path_test.py
+-rw-r--r--  2.0 unx    18356 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/fhir_path_test_base.py
+-rw-r--r--  2.0 unx    46839 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/fhir_path_validator.py
+-rw-r--r--  2.0 unx    61109 b- defN 23-Jun-05 20:08 build/lib/google/fhir/core/fhir_path/fhir_path_validator_v2.py
+-rw-r--r--  2.0 unx     1945 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/fhir_path_validator_v2_test.py
+-rw-r--r--  2.0 unx     5908 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/python_compiled_expressions.py
+-rw-r--r--  2.0 unx     3861 b- defN 23-May-18 18:49 build/lib/google/fhir/core/fhir_path/quantity.py
+-rw-r--r--  2.0 unx     4404 b- defN 23-May-18 18:51 build/lib/google/fhir/core/fhir_path/quantity_test.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/google/fhir/core/internal/__init__.py
+-rw-r--r--  2.0 unx     6663 b- defN 23-May-18 18:49 build/lib/google/fhir/core/internal/_primitive_time_utils.py
+-rw-r--r--  2.0 unx    14323 b- defN 23-May-18 18:49 build/lib/google/fhir/core/internal/primitive_handler.py
+-rw-r--r--  2.0 unx     8859 b- defN 23-May-18 18:49 build/lib/google/fhir/core/internal/resource_validation.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/google/fhir/core/internal/json_format/__init__.py
+-rw-r--r--  2.0 unx    15207 b- defN 23-May-18 18:49 build/lib/google/fhir/core/internal/json_format/_json_parser.py
+-rw-r--r--  2.0 unx    15656 b- defN 23-May-18 18:49 build/lib/google/fhir/core/internal/json_format/_json_printer.py
+-rw-r--r--  2.0 unx     6464 b- defN 23-May-18 18:49 build/lib/google/fhir/core/internal/json_format/json_format_test.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/google/fhir/core/internal/json_format/wrappers/__init__.py
+-rw-r--r--  2.0 unx     5417 b- defN 23-May-18 18:49 build/lib/google/fhir/core/internal/json_format/wrappers/_base64_binary.py
+-rw-r--r--  2.0 unx     4301 b- defN 23-May-18 18:49 build/lib/google/fhir/core/internal/json_format/wrappers/_date.py
+-rw-r--r--  2.0 unx     5736 b- defN 23-May-18 18:49 build/lib/google/fhir/core/internal/json_format/wrappers/_date_time.py
+-rw-r--r--  2.0 unx     2408 b- defN 23-May-18 18:49 build/lib/google/fhir/core/internal/json_format/wrappers/_decimal.py
+-rw-r--r--  2.0 unx     4502 b- defN 23-May-18 18:49 build/lib/google/fhir/core/internal/json_format/wrappers/_instant.py
+-rw-r--r--  2.0 unx    16137 b- defN 23-May-18 18:49 build/lib/google/fhir/core/internal/json_format/wrappers/_primitive_wrappers.py
+-rw-r--r--  2.0 unx     4791 b- defN 23-May-18 18:49 build/lib/google/fhir/core/internal/json_format/wrappers/_time.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/google/fhir/core/proto/__init__.py
+-rw-r--r--  2.0 unx     9188 b- defN 23-May-24 11:25 build/lib/google/fhir/core/proto/annotations_pb2.py
+-rw-r--r--  2.0 unx     1411 b- defN 23-May-24 11:25 build/lib/google/fhir/core/proto/fhirpath_replacement_list_pb2.py
+-rw-r--r--  2.0 unx     2354 b- defN 23-May-24 11:25 build/lib/google/fhir/core/proto/validation_pb2.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/google/fhir/core/testing/__init__.py
+-rw-r--r--  2.0 unx     6706 b- defN 23-May-18 18:49 build/lib/google/fhir/core/testing/protobuf_compare.py
+-rw-r--r--  2.0 unx     3745 b- defN 23-May-18 18:49 build/lib/google/fhir/core/testing/testdata_utils.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/google/fhir/core/utils/__init__.py
+-rw-r--r--  2.0 unx    13789 b- defN 23-May-18 18:49 build/lib/google/fhir/core/utils/annotation_utils.py
+-rw-r--r--  2.0 unx    15883 b- defN 23-May-18 18:51 build/lib/google/fhir/core/utils/annotation_utils_test.py
+-rw-r--r--  2.0 unx    17494 b- defN 23-May-18 18:51 build/lib/google/fhir/core/utils/fhir_package.py
+-rw-r--r--  2.0 unx    23767 b- defN 23-May-18 18:51 build/lib/google/fhir/core/utils/fhir_package_test_base.py
+-rw-r--r--  2.0 unx     9127 b- defN 23-May-18 18:49 build/lib/google/fhir/core/utils/fhir_types.py
+-rw-r--r--  2.0 unx     7750 b- defN 23-May-18 18:49 build/lib/google/fhir/core/utils/fhir_types_test.py
+-rw-r--r--  2.0 unx     1637 b- defN 23-May-18 18:49 build/lib/google/fhir/core/utils/path_utils.py
+-rw-r--r--  2.0 unx     1922 b- defN 23-May-18 18:49 build/lib/google/fhir/core/utils/path_utils_test.py
+-rw-r--r--  2.0 unx    12011 b- defN 23-May-18 18:49 build/lib/google/fhir/core/utils/proto_utils.py
+-rw-r--r--  2.0 unx    15754 b- defN 23-May-18 18:51 build/lib/google/fhir/core/utils/proto_utils_test.py
+-rw-r--r--  2.0 unx     3040 b- defN 23-May-18 18:49 build/lib/google/fhir/core/utils/resource_utils.py
+-rw-r--r--  2.0 unx     3789 b- defN 23-May-18 18:49 build/lib/google/fhir/core/utils/resource_utils_test.py
+-rw-r--r--  2.0 unx     1876 b- defN 23-May-18 18:49 build/lib/google/fhir/core/utils/url_utils.py
+-rw-r--r--  2.0 unx     1870 b- defN 23-May-18 18:49 build/lib/google/fhir/core/utils/url_utils_test.py
+-rw-r-----  2.0 unx      577 b- defN 23-May-18 18:49 google/fhir/core/__init__.py
+-rw-r-----  2.0 unx    12193 b- defN 23-May-18 18:49 google/fhir/core/codes.py
+-rw-r-----  2.0 unx    18626 b- defN 23-May-18 18:51 google/fhir/core/extensions.py
+-rw-r-----  2.0 unx     2275 b- defN 23-May-18 18:49 google/fhir/core/extensions_test.py
+-rw-r-----  2.0 unx     7281 b- defN 23-May-18 18:49 google/fhir/core/fhir_errors.py
+-rw-r-----  2.0 unx     5706 b- defN 23-May-18 18:49 google/fhir/core/fhir_errors_test.py
+-rw-r-----  2.0 unx     7054 b- defN 23-May-18 18:51 google/fhir/core/references.py
+-rw-r-----  2.0 unx    19632 b- defN 23-May-18 18:49 google/fhir/core/fhir_path/FhirPathLexer.py
+-rw-r-----  2.0 unx    66224 b- defN 23-May-18 18:49 google/fhir/core/fhir_path/FhirPathParser.py
+-rw-r-----  2.0 unx     8088 b- defN 23-May-18 18:49 google/fhir/core/fhir_path/FhirPathVisitor.py
+-rw-r-----  2.0 unx      579 b- defN 23-May-18 18:49 google/fhir/core/fhir_path/__init__.py
+-rw-r-----  2.0 unx    39499 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/_ast.py
+-rw-r-----  2.0 unx    12220 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/_ast_test.py
+-rw-r--r--  2.0 unx    25666 b- defN 23-Jun-05 20:08 google/fhir/core/fhir_path/_bigquery_interpreter.py
+-rw-r-----  2.0 unx    43839 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/_bigquery_sql_functions.py
+-rw-r-----  2.0 unx    54784 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/_evaluation.py
+-rw-r--r--  2.0 unx    33835 b- defN 23-Jun-05 20:08 google/fhir/core/fhir_path/_fhir_path_data_types.py
+-rw-r--r--  2.0 unx    11827 b- defN 23-Jun-05 20:08 google/fhir/core/fhir_path/_fhir_path_data_types_test.py
+-rw-r-----  2.0 unx    59561 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/_fhir_path_to_sql_functions.py
+-rw-r-----  2.0 unx    80507 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/_interpreter_test_base.py
+-rw-r-----  2.0 unx    12297 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/_navigation.py
+-rw-r-----  2.0 unx     8116 b- defN 23-May-18 18:49 google/fhir/core/fhir_path/_navigation_test.py
+-rw-r-----  2.0 unx    30292 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/_python_interpreter.py
+-rw-r-----  2.0 unx    33496 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/_semant.py
+-rw-r-----  2.0 unx    36633 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/_semant_test.py
+-rw-r-----  2.0 unx    24909 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/_spark_interpreter.py
+-rw-r--r--  2.0 unx    35878 b- defN 23-Jun-05 20:08 google/fhir/core/fhir_path/_spark_sql_functions.py
+-rw-r-----  2.0 unx    34090 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/_sql_data_types.py
+-rw-r-----  2.0 unx     7696 b- defN 23-May-18 18:49 google/fhir/core/fhir_path/_sql_data_types_test.py
+-rw-r-----  2.0 unx     6795 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/_structure_definitions.py
+-rw-r-----  2.0 unx     9761 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/_utils.py
+-rw-r-----  2.0 unx    12624 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/_utils_test.py
+-rw-r-----  2.0 unx    15711 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/context.py
+-rw-r-----  2.0 unx     6529 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/context_test.py
+-rw-r-----  2.0 unx    27285 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/expressions.py
+-rw-r-----  2.0 unx    37619 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/fhir_path.py
+-rw-r-----  2.0 unx     1298 b- defN 23-May-18 18:49 google/fhir/core/fhir_path/fhir_path_options.py
+-rw-r--r--  2.0 unx    72947 b- defN 23-Jun-05 20:08 google/fhir/core/fhir_path/fhir_path_spark_test.py
+-rw-r--r--  2.0 unx   239392 b- defN 23-Jun-05 20:08 google/fhir/core/fhir_path/fhir_path_test.py
+-rw-r-----  2.0 unx    18356 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/fhir_path_test_base.py
+-rw-r-----  2.0 unx    46839 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/fhir_path_validator.py
+-rw-r--r--  2.0 unx    61109 b- defN 23-Jun-05 20:08 google/fhir/core/fhir_path/fhir_path_validator_v2.py
+-rw-r-----  2.0 unx     1945 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/fhir_path_validator_v2_test.py
+-rw-r-----  2.0 unx     5908 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/python_compiled_expressions.py
+-rw-r-----  2.0 unx     3861 b- defN 23-May-18 18:49 google/fhir/core/fhir_path/quantity.py
+-rw-r-----  2.0 unx     4404 b- defN 23-May-18 18:51 google/fhir/core/fhir_path/quantity_test.py
+-rw-r-----  2.0 unx      577 b- defN 23-May-18 18:49 google/fhir/core/internal/__init__.py
+-rw-r-----  2.0 unx     6663 b- defN 23-May-18 18:49 google/fhir/core/internal/_primitive_time_utils.py
+-rw-r-----  2.0 unx    14323 b- defN 23-May-18 18:49 google/fhir/core/internal/primitive_handler.py
+-rw-r-----  2.0 unx     8859 b- defN 23-May-18 18:49 google/fhir/core/internal/resource_validation.py
+-rw-r-----  2.0 unx      577 b- defN 23-May-18 18:49 google/fhir/core/internal/json_format/__init__.py
+-rw-r-----  2.0 unx    15207 b- defN 23-May-18 18:49 google/fhir/core/internal/json_format/_json_parser.py
+-rw-r-----  2.0 unx    15656 b- defN 23-May-18 18:49 google/fhir/core/internal/json_format/_json_printer.py
+-rw-r-----  2.0 unx     6464 b- defN 23-May-18 18:49 google/fhir/core/internal/json_format/json_format_test.py
+-rw-r--r--  2.0 unx     3171 b- defN 23-May-18 18:49 google/fhir/core/internal/json_format/wrappers/README.md
+-rw-r-----  2.0 unx      577 b- defN 23-May-18 18:49 google/fhir/core/internal/json_format/wrappers/__init__.py
+-rw-r-----  2.0 unx     5417 b- defN 23-May-18 18:49 google/fhir/core/internal/json_format/wrappers/_base64_binary.py
+-rw-r-----  2.0 unx     4301 b- defN 23-May-18 18:49 google/fhir/core/internal/json_format/wrappers/_date.py
+-rw-r-----  2.0 unx     5736 b- defN 23-May-18 18:49 google/fhir/core/internal/json_format/wrappers/_date_time.py
+-rw-r-----  2.0 unx     2408 b- defN 23-May-18 18:49 google/fhir/core/internal/json_format/wrappers/_decimal.py
+-rw-r-----  2.0 unx     4502 b- defN 23-May-18 18:49 google/fhir/core/internal/json_format/wrappers/_instant.py
+-rw-r-----  2.0 unx    16137 b- defN 23-May-18 18:49 google/fhir/core/internal/json_format/wrappers/_primitive_wrappers.py
+-rw-r-----  2.0 unx     4791 b- defN 23-May-18 18:49 google/fhir/core/internal/json_format/wrappers/_time.py
+-rw-r-----  2.0 unx      577 b- defN 23-May-18 18:49 google/fhir/core/proto/__init__.py
+-rwxr-xr-x  2.0 unx     7697 b- defN 23-May-18 18:51 google/fhir/core/proto/annotations.proto
+-rw-r-----  2.0 unx     9188 b- defN 23-May-24 11:25 google/fhir/core/proto/annotations_pb2.py
+-rw-r--r--  2.0 unx     1576 b- defN 23-May-18 18:49 google/fhir/core/proto/fhirpath_replacement_list.proto
+-rw-r-----  2.0 unx     1411 b- defN 23-May-24 11:25 google/fhir/core/proto/fhirpath_replacement_list_pb2.py
+-rw-r--r--  2.0 unx     4935 b- defN 23-May-18 18:51 google/fhir/core/proto/validation.proto
+-rw-r-----  2.0 unx     2354 b- defN 23-May-24 11:25 google/fhir/core/proto/validation_pb2.py
+-rw-r-----  2.0 unx      577 b- defN 23-May-18 18:49 google/fhir/core/testing/__init__.py
+-rw-r-----  2.0 unx     6706 b- defN 23-May-18 18:49 google/fhir/core/testing/protobuf_compare.py
+-rw-r-----  2.0 unx     3745 b- defN 23-May-18 18:49 google/fhir/core/testing/testdata_utils.py
+-rw-r-----  2.0 unx      577 b- defN 23-May-18 18:49 google/fhir/core/utils/__init__.py
+-rw-r-----  2.0 unx    13789 b- defN 23-May-18 18:49 google/fhir/core/utils/annotation_utils.py
+-rw-r-----  2.0 unx    15883 b- defN 23-May-18 18:51 google/fhir/core/utils/annotation_utils_test.py
+-rw-r-----  2.0 unx    17494 b- defN 23-May-18 18:51 google/fhir/core/utils/fhir_package.py
+-rw-r-----  2.0 unx    23767 b- defN 23-May-18 18:51 google/fhir/core/utils/fhir_package_test_base.py
+-rw-r-----  2.0 unx     9127 b- defN 23-May-18 18:49 google/fhir/core/utils/fhir_types.py
+-rw-r-----  2.0 unx     7750 b- defN 23-May-18 18:49 google/fhir/core/utils/fhir_types_test.py
+-rw-r-----  2.0 unx     1637 b- defN 23-May-18 18:49 google/fhir/core/utils/path_utils.py
+-rw-r-----  2.0 unx     1922 b- defN 23-May-18 18:49 google/fhir/core/utils/path_utils_test.py
+-rw-r-----  2.0 unx    12011 b- defN 23-May-18 18:49 google/fhir/core/utils/proto_utils.py
+-rw-r-----  2.0 unx    15754 b- defN 23-May-18 18:51 google/fhir/core/utils/proto_utils_test.py
+-rw-r-----  2.0 unx     3040 b- defN 23-May-18 18:49 google/fhir/core/utils/resource_utils.py
+-rw-r-----  2.0 unx     3789 b- defN 23-May-18 18:49 google/fhir/core/utils/resource_utils_test.py
+-rw-r-----  2.0 unx     1876 b- defN 23-May-18 18:49 google/fhir/core/utils/url_utils.py
+-rw-r-----  2.0 unx     1870 b- defN 23-May-18 18:49 google/fhir/core/utils/url_utils_test.py
+-rwxr-xr-x  2.0 unx     7697 b- defN 23-May-18 18:51 google_fhir_core-0.9.3.data/data/annotations.proto
+-rw-r--r--  2.0 unx     1576 b- defN 23-May-18 18:49 google_fhir_core-0.9.3.data/data/fhirpath_replacement_list.proto
+-rw-r--r--  2.0 unx     4935 b- defN 23-May-18 18:51 google_fhir_core-0.9.3.data/data/validation.proto
+-rw-r--r--  2.0 unx     1520 b- defN 23-Jun-05 20:34 google_fhir_core-0.9.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 20:34 google_fhir_core-0.9.3.dist-info/WHEEL
+-rw-r-----  2.0 unx       13 b- defN 23-Jun-05 20:34 google_fhir_core-0.9.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    52415 b- defN 23-Jun-05 20:34 google_fhir_core-0.9.3.dist-info/RECORD
+431 files, 7944631 bytes uncompressed, 1564196 bytes compressed:  80.3%
```

## zipnote {}

```diff
@@ -1,7 +1,1015 @@
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/codes.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/extensions.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/extensions_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_errors.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_errors_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/references.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/FhirPathLexer.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/FhirPathParser.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/FhirPathVisitor.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_ast.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_ast_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_bigquery_interpreter.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_bigquery_sql_functions.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_evaluation.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_fhir_path_data_types.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_fhir_path_data_types_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_fhir_path_to_sql_functions.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_interpreter_test_base.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_navigation.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_navigation_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_python_interpreter.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_semant.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_semant_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_spark_interpreter.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_spark_sql_functions.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_sql_data_types.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_sql_data_types_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_structure_definitions.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_utils_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/context.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/context_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/expressions.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_options.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_spark_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_test_base.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_validator.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_validator_v2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_validator_v2_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/python_compiled_expressions.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/quantity.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/fhir_path/quantity_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/_primitive_time_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/primitive_handler.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/resource_validation.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/_json_parser.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/_json_printer.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/json_format_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_base64_binary.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_date.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_date_time.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_decimal.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_instant.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_primitive_wrappers.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_time.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/proto/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/proto/annotations_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/proto/fhirpath_replacement_list_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/proto/validation_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/testing/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/testing/protobuf_compare.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/testing/testdata_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/annotation_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/annotation_utils_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/fhir_package.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/fhir_package_test_base.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/fhir_types.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/fhir_types_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/path_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/path_utils_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/proto_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/proto_utils_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/resource_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/resource_utils_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/url_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/google/fhir/core/utils/url_utils_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/codes.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/extensions.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/extensions_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_errors.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_errors_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/references.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/FhirPathLexer.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/FhirPathParser.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/FhirPathVisitor.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_ast.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_ast_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_bigquery_interpreter.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_bigquery_sql_functions.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_evaluation.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_fhir_path_data_types.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_fhir_path_data_types_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_fhir_path_to_sql_functions.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_interpreter_test_base.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_navigation.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_navigation_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_python_interpreter.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_semant.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_semant_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_spark_interpreter.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_spark_sql_functions.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_sql_data_types.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_sql_data_types_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_structure_definitions.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/_utils_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/context.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/context_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/expressions.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_options.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_spark_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_test_base.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_validator.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_validator_v2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_validator_v2_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/python_compiled_expressions.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/quantity.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/fhir_path/quantity_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/internal/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/internal/_primitive_time_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/internal/primitive_handler.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/internal/resource_validation.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/_json_parser.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/_json_printer.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/json_format_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_base64_binary.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_date.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_date_time.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_decimal.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_instant.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_primitive_wrappers.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_time.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/proto/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/proto/annotations_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/proto/fhirpath_replacement_list_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/proto/validation_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/testing/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/testing/protobuf_compare.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/testing/testdata_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/utils/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/utils/annotation_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/utils/annotation_utils_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/utils/fhir_package.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/utils/fhir_package_test_base.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/utils/fhir_types.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/utils/fhir_types_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/utils/path_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/utils/path_utils_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/utils/proto_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/utils/proto_utils_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/utils/resource_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/utils/resource_utils_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/utils/url_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/core/utils/url_utils_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/codes.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/extensions.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/extensions_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_errors.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_errors_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/references.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/FhirPathLexer.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/FhirPathParser.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/FhirPathVisitor.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_ast.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_ast_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_bigquery_interpreter.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_bigquery_sql_functions.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_evaluation.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_fhir_path_data_types.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_fhir_path_data_types_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_fhir_path_to_sql_functions.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_interpreter_test_base.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_navigation.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_navigation_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_python_interpreter.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_semant.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_semant_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_spark_interpreter.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_spark_sql_functions.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_sql_data_types.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_sql_data_types_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_structure_definitions.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/_utils_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/context.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/context_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/expressions.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/fhir_path.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_options.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_spark_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_test_base.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_validator.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_validator_v2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/fhir_path_validator_v2_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/python_compiled_expressions.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/quantity.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/fhir_path/quantity_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/internal/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/internal/_primitive_time_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/internal/primitive_handler.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/internal/resource_validation.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/internal/json_format/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/internal/json_format/_json_parser.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/internal/json_format/_json_printer.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/internal/json_format/json_format_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_base64_binary.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_date.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_date_time.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_decimal.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_instant.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_primitive_wrappers.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/internal/json_format/wrappers/_time.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/proto/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/proto/annotations_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/proto/fhirpath_replacement_list_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/proto/validation_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/testing/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/testing/protobuf_compare.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/testing/testdata_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/utils/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/utils/annotation_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/utils/annotation_utils_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/utils/fhir_package.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/utils/fhir_package_test_base.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/utils/fhir_types.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/utils/fhir_types_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/utils/path_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/utils/path_utils_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/utils/proto_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/utils/proto_utils_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/utils/resource_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/utils/resource_utils_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/utils/url_utils.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/core/utils/url_utils_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/__init__.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/codes.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/extensions.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/extensions_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_errors.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_errors_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/references.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/FhirPathLexer.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/FhirPathParser.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/FhirPathVisitor.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/__init__.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_ast.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_ast_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_bigquery_interpreter.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_bigquery_sql_functions.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_evaluation.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_fhir_path_data_types.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_fhir_path_data_types_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_fhir_path_to_sql_functions.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_interpreter_test_base.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_navigation.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_navigation_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_python_interpreter.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_semant.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_semant_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_spark_interpreter.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_spark_sql_functions.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_sql_data_types.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_sql_data_types_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_structure_definitions.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_utils.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/_utils_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/context.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/context_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/expressions.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/fhir_path.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/fhir_path_options.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/fhir_path_spark_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/fhir_path_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/fhir_path_test_base.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/fhir_path_validator.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/fhir_path_validator_v2.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/fhir_path_validator_v2_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/python_compiled_expressions.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/quantity.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/fhir_path/quantity_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/internal/__init__.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/internal/_primitive_time_utils.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/internal/primitive_handler.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/internal/resource_validation.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/internal/json_format/__init__.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/internal/json_format/_json_parser.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/internal/json_format/_json_printer.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/internal/json_format/json_format_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/internal/json_format/wrappers/__init__.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/internal/json_format/wrappers/_base64_binary.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/internal/json_format/wrappers/_date.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/internal/json_format/wrappers/_date_time.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/internal/json_format/wrappers/_decimal.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/internal/json_format/wrappers/_instant.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/internal/json_format/wrappers/_primitive_wrappers.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/internal/json_format/wrappers/_time.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/proto/__init__.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/proto/annotations_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/proto/fhirpath_replacement_list_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/proto/validation_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/testing/__init__.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/testing/protobuf_compare.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/testing/testdata_utils.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/utils/__init__.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/utils/annotation_utils.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/utils/annotation_utils_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/utils/fhir_package.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/utils/fhir_package_test_base.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/utils/fhir_types.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/utils/fhir_types_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/utils/path_utils.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/utils/path_utils_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/utils/proto_utils.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/utils/proto_utils_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/utils/resource_utils.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/utils/resource_utils_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/utils/url_utils.py
+Comment: 
+
+Filename: build/lib/google/fhir/core/utils/url_utils_test.py
+Comment: 
+
 Filename: google/fhir/core/__init__.py
 Comment: 
 
 Filename: google/fhir/core/codes.py
 Comment: 
 
 Filename: google/fhir/core/extensions.py
@@ -45,14 +1053,17 @@
 
 Filename: google/fhir/core/fhir_path/_evaluation.py
 Comment: 
 
 Filename: google/fhir/core/fhir_path/_fhir_path_data_types.py
 Comment: 
 
+Filename: google/fhir/core/fhir_path/_fhir_path_data_types_test.py
+Comment: 
+
 Filename: google/fhir/core/fhir_path/_fhir_path_to_sql_functions.py
 Comment: 
 
 Filename: google/fhir/core/fhir_path/_interpreter_test_base.py
 Comment: 
 
 Filename: google/fhir/core/fhir_path/_navigation.py
@@ -153,14 +1164,17 @@
 
 Filename: google/fhir/core/internal/json_format/_json_printer.py
 Comment: 
 
 Filename: google/fhir/core/internal/json_format/json_format_test.py
 Comment: 
 
+Filename: google/fhir/core/internal/json_format/wrappers/README.md
+Comment: 
+
 Filename: google/fhir/core/internal/json_format/wrappers/__init__.py
 Comment: 
 
 Filename: google/fhir/core/internal/json_format/wrappers/_base64_binary.py
 Comment: 
 
 Filename: google/fhir/core/internal/json_format/wrappers/_date.py
@@ -252,29 +1266,29 @@
 
 Filename: google/fhir/core/utils/url_utils.py
 Comment: 
 
 Filename: google/fhir/core/utils/url_utils_test.py
 Comment: 
 
-Filename: google_fhir_core-0.9.2.data/data/annotations.proto
+Filename: google_fhir_core-0.9.3.data/data/annotations.proto
 Comment: 
 
-Filename: google_fhir_core-0.9.2.data/data/fhirpath_replacement_list.proto
+Filename: google_fhir_core-0.9.3.data/data/fhirpath_replacement_list.proto
 Comment: 
 
-Filename: google_fhir_core-0.9.2.data/data/validation.proto
+Filename: google_fhir_core-0.9.3.data/data/validation.proto
 Comment: 
 
-Filename: google_fhir_core-0.9.2.dist-info/METADATA
+Filename: google_fhir_core-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: google_fhir_core-0.9.2.dist-info/WHEEL
+Filename: google_fhir_core-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: google_fhir_core-0.9.2.dist-info/top_level.txt
+Filename: google_fhir_core-0.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: google_fhir_core-0.9.2.dist-info/RECORD
+Filename: google_fhir_core-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## google/fhir/core/fhir_path/_bigquery_interpreter.py

```diff
@@ -28,15 +28,25 @@
 from google.fhir.core.fhir_path import expressions
 from google.fhir.core.internal import _primitive_time_utils
 from google.fhir.core.utils import fhir_package
 from google.fhir.r4.terminology import local_value_set_resolver
 
 
 def _escape_identifier(identifier_value: str) -> str:
-  """Returns the value surrounded by backticks if it is a keyword."""
+  """Returns the value in a valid column name format.
+
+  Args:
+    identifier_value: Raw identifier string.
+
+  Returns:
+    If the identifier is a keyword, then it will be surrounded by backticks. If
+    the identifier contains a hyphen, the hyphen will be replaced by an
+    underscore.
+  """
+  identifier_value = identifier_value.replace('-', '_')
   # Keywords are case-insensitive
   if identifier_value.upper() in _sql_data_types.STANDARD_SQL_KEYWORDS:
     return f'`{identifier_value}`'
   return identifier_value  # No-op
 
 
 class BigQuerySqlInterpreter(_evaluation.ExpressionNodeBaseVisitor):
@@ -122,15 +132,15 @@
       self, reference: _evaluation.ExpressionNode
   ) -> _sql_data_types.IdentifierSelect:
     # When $this is used, we need the last identifier from the operand.
     sql_alias = reference.to_fhir_path().split('.')[-1]
     # If the identifier is `$this`, we assume that the repeated field has been
     # unnested upstream so we only need to reference it with its alias:
     # `{}_element_`.
-    if _fhir_path_data_types.is_collection(reference.return_type()):
+    if _fhir_path_data_types.returns_collection(reference.return_type()):
       sql_alias = f'{sql_alias}_element_'
 
     sql_data_type = _sql_data_types.get_standard_sql_data_type(
         reference.return_type()
     )
     return _sql_data_types.IdentifierSelect(
         select_part=_sql_data_types.Identifier(
@@ -590,15 +600,15 @@
     lhs_result = self.visit(union.left)
     rhs_result = self.visit(union.right)
 
     # Supported in FHIRPath, but currently generates invalid Standard SQL.
     if isinstance(
         lhs_result.sql_data_type, _sql_data_types.Struct
     ) or isinstance(rhs_result.sql_data_type, _sql_data_types.Struct):
-      raise TypeError(
+      raise ValueError(
           f'Unsupported `STRUCT` union between {lhs_result}, {rhs_result}.'
       )
 
     sql_alias = 'union_'
     lhs = _sql_data_types.Select(
         select_part=_sql_data_types.Identifier(
             ('lhs_', lhs_result.sql_alias),
```

## google/fhir/core/fhir_path/_bigquery_sql_functions.py

```diff
@@ -355,14 +355,25 @@
       function: _evaluation.MatchesFunction,
       operand_result: Optional[_sql_data_types.Select],
       params_result: List[_sql_data_types.StandardSqlExpression],
   ) -> _sql_data_types.Select:
     if operand_result is None:
       raise ValueError('matches() cannot be called without an operand.')
 
+    # If the input collection contains multiple items, the evaluation of the
+    # expression will end and signal an error to the calling environment.
+    # https://build.fhir.org/ig/HL7/FHIRPath/#matchesregex-string-boolean
+    if _fhir_path_data_types.is_collection(
+        function.parent_node().return_type()
+    ):
+      raise ValueError(
+          'matches() cannot be called on a collection type. '
+          'Must either be scalar or unnested with a function '
+          'like all()'
+      )
     sql_alias = 'matches_'
     sql_data_type = _sql_data_types.Boolean
 
     # If `pattern` is not given, return empty set.
     if not params_result:
       return _sql_data_types.Select(
           select_part=_sql_data_types.RawExpression(
```

## google/fhir/core/fhir_path/_evaluation.py

```diff
@@ -42,14 +42,20 @@
 # pylint: enable=g-import-not-at-top
 
 VALUE_SET_URL = 'http://hl7.org/fhir/StructureDefinition/ValueSet'
 QUANTITY_URL = 'http://hl7.org/fhir/StructureDefinition/Quantity'
 ElementDefinition = message.Message
 
 
+_MAPPING_FUNCTIONS = frozenset([
+    _ast.Function.Name.ALL,
+    _ast.Function.Name.WHERE,
+])
+
+
 @dataclasses.dataclass(frozen=True, order=True)
 class CodeValue:
   """An immutable code,value tuple for local use and set operations."""
 
   system: str
   value: str
 
@@ -520,15 +526,18 @@
     if not isinstance(index.return_type(), _fhir_path_data_types._Integer):
       raise ValueError(
           'Expected index type to be Integer. '
           f'Got {index.return_type()} instead.'
       )
     self._collection = collection
     self._index = index
-    super().__init__(fhir_context, collection.return_type())
+    return_type = collection.return_type().get_new_cardinality_type(
+        _fhir_path_data_types.Cardinality.SCALAR
+    )
+    super().__init__(fhir_context, return_type)
 
   def get_resource_nodes(self) -> List[ExpressionNode]:
     return (
         self.collection.get_resource_nodes() + self.index.get_resource_nodes()
     )
 
   def get_root_node(self) -> ExpressionNode:
@@ -545,15 +554,15 @@
   def index(self) -> LiteralNode:
     return self._index  # pytype: disable=attribute-error
 
   def to_fhir_path(self) -> str:
     return f'{self._collection.to_fhir_path()}[{self.index.to_fhir_path()}]'
 
   def operands(self) -> List[ExpressionNode]:
-    return [self._collection]  # pytype: disable=attribute-error
+    return [self.collection, self.index]
 
   def replace_operand(
       self, expression_to_replace: str, replacement: 'ExpressionNode'
   ) -> None:
     if self._collection.to_fhir_path() == expression_to_replace:  # pytype: disable=attribute-error
       self._collection = replacement
     else:
@@ -1244,27 +1253,52 @@
     return (
         f'{self._left.to_fhir_path()} {self._operator.value} '
         f'{self._right.to_fhir_path()}'
     )
 
 
 class ReferenceNode(ExpressionNode):
-  """Implementation of $this keyword and relative paths."""
+  """Implementation of $this keyword and relative paths.
+
+  ReferenceNodes are used as a way to indicate that the FHIRPath has already
+  been used in a previous context in the FHIRPath. For example, in the FHIRPath
+    Patient.name.all(Patient.name.matches('regex'))
+
+  The second Patient.name gets internally substituted for a ReferenceNode to
+  Patient.name. The interpreter can then recognize that Patient.name has already
+  been resolved and does not need to reresolved if it so chooses.
+
+  An optional argument `element_of_array` will also set the cardinality of the
+  return type to be a CHILD_OF_COLLECTION if the original operand returns a
+  collection because some functions inherently map the expression in the params
+  to each element of the operand. In the above example, Patient.name is a
+  collection according to the FHIR spec, but matches only operates on scalars.
+  In order to check the match of each value in name, all() is used on
+  Patient.name, the second Patient.name is then an unnested reference to the
+  original Patient.name.
+  """
 
   def __init__(
       self,
       fhir_context: context.FhirPathContext,
       reference_node: ExpressionNode,
+      element_of_array: bool = False,
   ) -> None:
     self._reference_node = reference_node
     # If the reference node/caller is a function, then the actual node being
     # referenced is the first non-function caller.
     while isinstance(self._reference_node, FunctionNode):
       self._reference_node = self._reference_node.get_parent_node()
-    super().__init__(fhir_context, reference_node.return_type())
+
+    return_type = reference_node.return_type()
+    if element_of_array and return_type.returns_collection():
+      return_type = return_type.get_new_cardinality_type(
+          _fhir_path_data_types.Cardinality.CHILD_OF_COLLECTION
+      )
+    super().__init__(fhir_context, return_type)
 
   def get_resource_nodes(self) -> List[ExpressionNode]:
     return self._reference_node.get_resource_nodes()
 
   def get_root_node(self) -> ExpressionNode:
     return self._reference_node.get_root_node()
 
@@ -1397,17 +1431,17 @@
 
 class ExpressionNodeBaseVisitor(abc.ABC):
   """Abstract base class that visits the Expression Nodes."""
 
   def visit(self, node: ExpressionNode) -> Any:
     return node.accept(self)
 
-  def visit_children(self, node: ExpressionNode) -> Any:
+  def visit_operands(self, node: ExpressionNode) -> Any:
     result: List[Any] = []
-    for c in node.children():  # pytype: disable=attribute-error
+    for c in node.operands():
       result.append(c.accept(self))
     return result
 
   @abc.abstractmethod
   def visit_root(self, root: RootMessageNode) -> Any:
     pass
 
@@ -1566,14 +1600,17 @@
       )
     else:
       raise ValueError(
           f'Unsupported literal value: {literal} {type(literal.value)}.'
       )
 
   def visit_identifier(self, identifier: _ast.Identifier) -> Any:
+    if identifier.value == '$this':
+      return self._node_context[-1]
+
     return InvokeExpressionNode(
         self._context, identifier.value, self._node_context[-1]
     )
 
   def visit_indexer(self, indexer: _ast.Indexer, **kwargs: Any) -> Any:
     collection_result = self.visit(indexer.collection)
     index_result = self.visit(indexer.index)
@@ -1678,15 +1715,24 @@
 
     # Use the given operand if it exists, otherwise this must have been invoked
     # on the root, so that is the effective operand.
     operand_node = (
         self.visit(operand) if operand is not None else self._node_context[-1]
     )
     params: List[ExpressionNode] = []
+    # Mapping function like all() and where are functions that apply the params
+    # to each element of the operand if the operand is a collection so the
+    # return type of the reference would be a reference to an element of the
+    # array rather than the whole array itself..
+    element_of_array = function_name in _MAPPING_FUNCTIONS
     # For functions, the identifiers can be relative to the operand of the
     # function; not the root FHIR type.
-    self._node_context.append(ReferenceNode(self._context, operand_node))
+    self._node_context.append(
+        ReferenceNode(
+            self._context, operand_node, element_of_array=element_of_array
+        )
+    )
     for param in function.params:
       new_param = self.visit(param)
       params.append(new_param)
     self._node_context.pop()
     return function_class(self._context, operand_node, params)
```

## google/fhir/core/fhir_path/_fhir_path_data_types.py

```diff
@@ -17,20 +17,25 @@
 Scalar types are declared as module-level constants that can be imported by
 dependent modules. Parameterized types such as `Collection` should be
 instantiated directly, so that the relevant contained type information can be
 provided by the caller.
 """
 
 import abc
+import collections
 import copy
+import dataclasses
 import enum
+import itertools
+import re
+from typing import Any, Dict, Iterable, List, Mapping, Optional, Set, Sequence, Tuple, cast, Collection as CollectionType
+
+import stringcase
 
-from typing import Any, Dict, Optional, Set, cast, Collection as CollectionType
 from google.protobuf import message
-from google.fhir.core.fhir_path import _utils
 
 # Tokens that are keywords in FHIRPath.
 # If used as identifier tokens in FHIRPath expressions, they must be escaped
 # with backticks (`).
 RESERVED_FHIR_PATH_KEYWORDS = frozenset([
     '$index',
     '$this',
@@ -61,14 +66,18 @@
     'weeks',
     'xor',
     'year',
     'years',
     'second',
 ])
 
+# Given a type code like http://hl7.org/fhirpath/System.String
+# captures 'String'
+_TYPE_CODE_URI_RE = re.compile(r'^http://hl7.org/fhirpath/System\.(.+)')
+
 
 @enum.unique
 class Cardinality(enum.Enum):
   """Defines the cardinality of a FhirPathDataType.
 
   There are three different cardinalities that need to be captured:
     1. A FHIRPath expression always returns one value (e.g., exists() or
@@ -85,14 +94,54 @@
   COLLECTION = 'collection'
   CHILD_OF_COLLECTION = 'child_of_collection'
 
 
 # TODO(b/202892821): Consolidate with `_sql_data_types.py` functionality.
 
 
+@dataclasses.dataclass(frozen=True)
+class Slice:
+  """A container for all element definitions describing a slice.
+
+  https://build.fhir.org/profiling.html#slicing
+
+  Attributes:
+    slice_def: The element definition describing the slice itself.
+    relative_path: The path to the sliced collection relative to the structure
+      definition defining the slice.
+    slice_rules: Tuples of (relative_path, element_definition) for the element
+      definitions describing the contents of the slice and the path to them
+      relaitve to the structure definition defining the slice.
+  """
+
+  slice_def: message.Message
+  relative_path: str
+  slice_rules: Sequence[Tuple[str, message.Message]]
+
+
+@dataclasses.dataclass
+class _SliceBuilder:
+  """An internal class used to incerementally build Slice instances.
+
+  Its attributes are Optional because the _SliceBuilder class is built
+  incrementally. These attributes are not always available
+  initially. A _SliceBuilder instance should be converted to a Slice
+  instance and then provided to callers.
+  """
+
+  slice_def: Optional[message.Message]
+  relative_path: Optional[str]
+  slice_rules: List[Tuple[str, message.Message]]
+
+  def to_slice(self) -> Slice:
+    assert self.slice_def is not None, 'slice_def is unexpectedly None'
+    assert self.relative_path is not None, 'relative_path is unexpectedly None'
+    return Slice(self.slice_def, self.relative_path, self.slice_rules)
+
+
 class FhirPathDataType(metaclass=abc.ABCMeta):
   """An abstract base class defining a FHIRPath system primitive.
 
   Traversal implicitly converts FHIR types representing primitives to instances
   of `FhirPathDataType` types according to the logic at:
   https://www.hl7.org/fhir/fhirpath.html#types.
 
@@ -100,14 +149,17 @@
     cardinality: Determines how many values are returned for the type.
     root_element_definition: The root element definition that contains
       constraints and restrictions of the particular type.
     comparable: Values of the same type can be compared to each other.
     supported_coercion: A set of `FhirPathDataType`s depicting allowable
       implicit conversion.
     url: The canonical URL reference to the data type.
+    child_defs: A mapping of name to element definition for each child element
+      of the structure definition, including slices on extension. Empty for
+      other data types.
   """
 
   _cardinality: Cardinality = Cardinality.SCALAR
   _root_element_definition: message.Message = None
 
   @property
   @abc.abstractmethod
@@ -162,15 +214,16 @@
   def returns_polymorphic(self) -> bool:
     """Indicates if the type returns a polymorphic choice type."""
     return False
 
   def fields(self) -> Set[str]:
     return set()
 
-  def children(self) -> Dict[str, message.Message]:
+  @property
+  def child_defs(self) -> Mapping[str, message.Message]:
     return {}
 
   @property
   def root_element_definition(self) -> Optional[message.Message]:
     return self._root_element_definition
 
   def __init__(self, *, comparable: bool = False) -> None:
@@ -555,68 +608,152 @@
     self._struct_def = cast(Any, struct_def_proto)
     self._url = self._struct_def.url.value
     self._base_type = self._struct_def.type.value
     # For some custom types, the element type differs from the base type.
     self._element_type = element_type if element_type else self._base_type
     self._backbone_element_path = backbone_element_path
 
+    # For backbone elements, prepend their paths with the path to the
+    # root of the backbone element.
     qualified_path = (
         f'{self._element_type}.{self._backbone_element_path}'
         if self._backbone_element_path
         else self._element_type
     )
 
-    # Store the children elements of the structdef.
-    self._children = {}
-    # If there are specified descendants of the structdef then save them as
-    # well.
-    self._required_descendants = {}
+    self._child_defs = {}
+    self._direct_children = []
+    self._other_descendants = []
+    # A map of slice ID (e.g. some.path:SomeSlice) to the _SliceBuilder
+    # object representing that slice.
+    slices: dict[str, _SliceBuilder] = collections.defaultdict(
+        lambda: _SliceBuilder(None, None, [])
+    )
+
     for elem in self._struct_def.snapshot.element:
-      if elem.id.value == qualified_path:
-        self._root_element_definition = elem
+      # Extension.url does not provide any additional meaningful information for
+      # extensions so we will skip it as it also conflicts with
+      # Extension.extension:url if there is a subextension type. More info in
+      # b/284998302
+      if elem.base.path.value == 'Extension.url':
         continue
-      # Paths that look like a.elemValue when qualified_path=a.elem get
-      # misidentified as being a child of a.elem
-      if elem.id.value.startswith(qualified_path + '.'):
-        relative_path = elem.id.value[len(qualified_path) + 1 :]
-        if not relative_path:
-          continue
-        if '.' not in relative_path:
-          name = _utils.trim_name(relative_path)
-          self._children[name] = elem
+
+      path = _get_analytic_path(elem.path.value, elem.id.value)
+
+      if path == qualified_path:
+        if elem.slice_name.value:
+          # This is a slice definition at `qualified_path`, i.e. a
+          # path like <qualified_path>:Slice'
+          slice_def = slices[f':{elem.slice_name.value}']
+          slice_def.slice_def = elem
+          slice_def.relative_path = ''
+        else:
+          self._root_element_definition = elem
+
+        continue
+
+      if re.search(rf'^{qualified_path}\.\w+', path):
+        relative_path = path[len(qualified_path) + 1 :]
+
+        # One path may have multiple element definitions due to
+        # slices. The path will have one element definition providing
+        # its base definition and additional element definitions for
+        # each slice of that path. We only place the base element
+        # definition in the children dictionary, as callers currently
+        # expect to be able to find these definitions in this
+        # dictionary.
+
+        # Check to see if the element id contains a slice ID
+        # (e.g. some.path:SomeSlice) but not a slice on extension.
+        # Capture the slice ID, e.g. 'some.path:SomeSlice' given an id
+        # like 'some.path:SomeSlice.field' so we can later group all
+        # elements describing the same slice together. We use the
+        # closest_slice_ancestor below to aggregate element
+        # definitions describing the same slice. We do not need to do
+        # this for slices on extensions, as they have a unique field
+        # in the analytic schema, and thus are treated as fields
+        # rather than slices.
+        closest_slice_ancestor = re.search(
+            rf'^{qualified_path}[\.]?(.*(?<!.extension):[\w-]+)(?:$|\.)',
+            elem.id.value,
+        )
+        direct_child = '.' not in relative_path
+
+        if direct_child and closest_slice_ancestor is None:
+          assert relative_path not in self.child_defs, (
+              f'{relative_path} found twice among children in structure'
+              f' definition {self._struct_def.url.value}.'
+          )
+          self._child_defs[relative_path] = elem
+
+        if closest_slice_ancestor is not None:
+          # Gather all the element definitions which describe the same
+          # slice into a single data structure.
+          slice_def = slices[closest_slice_ancestor[1]]
+          if elem.slice_name.value:
+            # This is the definition for the slice itself, e.g. Foo.bar:baz.
+            slice_def.slice_def = elem
+            slice_def.relative_path = relative_path
+          else:
+            # This is a constraint describing the slice, e.g. Foo.bar:baz.quux.
+            slice_def.slice_rules.append((relative_path, elem))
+        elif direct_child:
+          self._direct_children.append((relative_path, elem))
         else:
-          names = [_utils.trim_name(n) for n in relative_path.split('.')]
-          self._required_descendants['.'.join(names)] = elem
+          self._other_descendants.append((relative_path, elem))
 
     if not self._root_element_definition:
       raise ValueError(
           f'StructureDataType {self._url} searching on {qualified_path} '
           f' missing root element definition. {self._struct_def}'
       )
 
+    self._slices = tuple(slice_def.to_slice() for slice_def in slices.values())
+
   def __eq__(self, o) -> bool:
     if isinstance(o, StructureDataType):
       return cast(StructureDataType, o).url == self.url
     return False
 
   def __hash__(self) -> int:
     return hash(self.url)
 
   def _class_name(self) -> str:
     return f'<StructureFhirPathDataType(url={self.url})>'
 
   def fields(self) -> Set[str]:
-    return set(self._children.keys())
-
-  def children(self) -> Dict[str, message.Message]:
-    return self._children
+    return set(self._child_defs.keys())
 
   @property
-  def required_descendants(self) -> Dict[str, message.Message]:
-    return self._required_descendants
+  def child_defs(self) -> Mapping[str, message.Message]:
+    return self._child_defs
+
+  def iter_children(self) -> Iterable[Tuple[str, message.Message]]:
+    """Returns an iterator over all direct child element definitions.
+
+    Contains all entries in `child_defs`. Does not contain slices.
+    """
+    return iter(self._direct_children)
+
+  def iter_all_descendants(self) -> Iterable[Tuple[str, message.Message]]:
+    """Returns an iterator over all element definitions.
+
+    Contains all entries in `iter_children`, as well as additional element
+    definitions for elements describing descendants deeper than direct children.
+    Does not contain slices.
+    """
+    return itertools.chain(self._direct_children, self._other_descendants)
+
+  def iter_slices(self) -> Iterable[Slice]:
+    """Returns an iterator over all slices.
+
+    Contains both direction children and descendants deeper than direct
+    children.
+    """
+    return iter(self._slices)
 
 
 class QuantityStructureDataType(StructureDataType, _Quantity):
   """Represents quantity FHIR specification data types."""
 
   _URL = 'http://hl7.org/fhirpath/System.Quantity'
 
@@ -808,14 +945,31 @@
 
 
 def primitive_type_from_type_code(type_code: str) -> Optional[FhirPathDataType]:
   """Returns the FhirPathDataType for the primitive identifed by the URL."""
   return _PRIMITIVE_TYPES_BY_CODE.get(type_code.casefold())
 
 
+def is_type_code_primitive(type_code: str) -> bool:
+  """Indicates if `type_code` refers to a primitive type.
+
+  Args:
+    type_code: The FHIR type code to look up. Could be a value like 'Boolean' or
+      URL like 'http://hl7.org/fhirpath/System.Boolean'
+
+  Returns:
+    True if the type code represents a FHIR primitive and False otherwise.
+  """
+  url_type_code = _TYPE_CODE_URI_RE.search(type_code)
+  if url_type_code is not None:
+    type_code = url_type_code[1]
+
+  return type_code.casefold() in _PRIMITIVE_TYPES_BY_CODE
+
+
 def is_numeric(fhir_type: FhirPathDataType) -> bool:
   return (
       isinstance(fhir_type, _Integer) or isinstance(fhir_type, _Decimal)
   ) or isinstance(fhir_type, _Empty)
 
 
 def is_primitive(fhir_type: FhirPathDataType) -> bool:
@@ -911,7 +1065,80 @@
 
 def returns_collection(return_type: FhirPathDataType) -> bool:
   return return_type and return_type.returns_collection()
 
 
 def is_collection(return_type: FhirPathDataType) -> bool:
   return return_type and return_type.cardinality == Cardinality.COLLECTION
+
+
+# Captures the names appearing after 'extension:' stanzas in IDs.
+_EXTENSION_SLICE_NAMES_RE = re.compile(r'(?:^|\.)extension:([\w-]+)(?=$|\.)')
+# Captures the word 'extension' in dotted paths.
+_EXTENSION_PATH_ELEMENTS_RE = re.compile(r'(?:^|\.)(extension)(?=$|\.)')
+
+
+def _get_analytic_path(path: str, elem_id: str) -> str:
+  """Builds a usable FHIRPath given an element path and id.
+
+  Removes choice type indicators '[x]'
+
+  Some element definitions reference attributes from extension slices. These
+  elements will have ids like 'Foo.extension:someExtension' but
+  paths like 'Foo.extension' We want to treat these paths as
+  'Foo.someExtension' so we replace the 'extension' part of the
+  path with the slice name.
+
+  Args:
+    path: The path attribute from the element definition to clean.
+    elem_id: The id attribute from the element definition to clean.
+
+  Returns:
+    The cleaned path name.
+  """
+  # Use a regex to find all extension slice names in the id.
+  extension_slice_names = _EXTENSION_SLICE_NAMES_RE.findall(elem_id)
+  if extension_slice_names:
+    # Replace each .extension element of the path with the extension
+    # slice name. Use a regex to find the indices of each .extension
+    # part of the path.
+    extension_path_elements = _EXTENSION_PATH_ELEMENTS_RE.finditer(path)
+    index_adjustment = 0
+    for slice_name, path_element in zip(
+        extension_slice_names, extension_path_elements
+    ):
+      # Replace the extension elements with the slice name.
+      start = path_element.start(1) + index_adjustment
+      end = path_element.end(1) + index_adjustment
+      path = path[:start] + slice_name + path[end:]
+
+      # Because we're changing the length of the `path` by
+      # replacing 'extension' with the slice name, we'll need to
+      # take that into account when referencing future indices.
+      index_adjustment += len(slice_name) - 9  # 9 is len('extension')
+
+  # Remove choice type indicators from the path.
+  path = path.replace('[x]', '')
+
+  return path
+
+
+def fixed_field_for_type_code(type_code: str) -> str:
+  """Retrieves the `ElementDefinition.fixed.choice` oneof field for `type_code`.
+
+  Args:
+    type_code: The FHIR type code to look up. Could be a value like 'boolean' or
+      URL like 'http://hl7.org/fhirpath/System.Boolean'
+
+  Returns:
+    The attribute corresponding to this type code on the
+    ElementDefinition.FixedX.choice oneof.
+  """
+  url_type_code = _TYPE_CODE_URI_RE.search(type_code)
+  if url_type_code is not None:
+    type_code = url_type_code[1]
+
+  # Lower-case the first character to avoid leading _ characters from
+  # snake case-ing.
+  fixed_field = stringcase.snakecase(type_code[:1].lower() + type_code[1:])
+  # We special-case 'string' as 'string_value' in the proto.
+  return 'string_value' if fixed_field == 'string' else fixed_field
```

## google/fhir/core/fhir_path/_interpreter_test_base.py

```diff
@@ -83,16 +83,19 @@
   def assert_expression_result(
       self,
       parsed_expression: python_compiled_expressions.PythonCompiledExpression,
       builder: expressions.Builder,
       resource: message.Message,
       expected_result: Union[bool, str, float, int],
   ):
-    # Confirm the expressions themselves match.
-    self.assertEqual(parsed_expression.fhir_path, builder.fhir_path)
+    # $this syntax isn't supported in the builder so skip the fhir path
+    # expression check.
+    if '$this' not in parsed_expression.fhir_path:
+      # Confirm the expressions themselves match.
+      self.assertEqual(parsed_expression.fhir_path, builder.fhir_path)
 
     # Evaluate both the built and parsed expressions and ensure they
     # produce the same result.
     parsed_result = parsed_expression.evaluate(resource)
     built_result = (
         python_compiled_expressions.PythonCompiledExpression.from_builder(
             builder
@@ -1851,14 +1854,25 @@
     self.assert_expression_result(
         self.compile_expression('Patient', "address.all(use = 'home')"),
         pat.address.all(pat.address.use == 'home'),
         patient,
         False,
     )
 
+    # All items match parent reference.
+    pat = self.builder('Patient')
+    self.assert_expression_result(
+        self.compile_expression(
+            'Patient', "address.city.all($this.matches('[a-zA-Z]* City'))"
+        ),
+        pat.address.city.all(pat.address.city.matches('[a-zA-Z]* City')),
+        patient,
+        True,
+    )
+
     # All items match.
     pat = self.builder('Patient')
     self.assert_expression_result(
         self.compile_expression('Patient', 'address.all(use.exists())'),
         pat.address.all(pat.address.use.exists()),
         patient,
         True,
@@ -2231,14 +2245,24 @@
         + active.exists() <ExistsFunction> (
         | + active <InvokeExpressionNode> (
         | | + Patient <RootMessageNode> ()))"""
         ),
         self.builder('Patient').active.exists().debug_string(),
     )
 
+    # Indexing
+    self.assertMultiLineEqual(
+        textwrap.dedent("""\
+        + address[0] <IndexerNode> (
+        | + address <InvokeExpressionNode> (
+        | | + Patient <RootMessageNode> ())
+        | + 0 <LiteralNode> ())"""),
+        self.builder('Patient').address[0].debug_string(),
+    )
+
     # Multiple arguments
     self.assertMultiLineEqual(
         textwrap.dedent(
             """\
         + subject.idFor('patient') <IdForFunction> (
         | + subject <InvokeExpressionNode> (
         | | + Encounter <RootMessageNode> ())
```

## google/fhir/core/fhir_path/_semant.py

```diff
@@ -127,15 +127,15 @@
     walker = _navigation.FhirStructureDefinitionWalker(
         self._env,
         structure_definition,
         element_definition,
     )
     _ = self.visit(ast, walker=walker)
 
-  def visit_literal(
+  def visit_literal(  # pytype: disable=signature-mismatch  # overriding-parameter-count-checks
       self, literal: _ast.Literal,
       walker: _navigation.FhirStructureDefinitionWalker
   ) -> _fhir_path_data_types.FhirPathDataType:
     if literal.value is None:
       result = _fhir_path_data_types.Empty
     elif isinstance(literal.value, bool):
       result = _fhir_path_data_types.Boolean
@@ -158,15 +158,15 @@
           '', 'Semantic Analysis', f'Unsupported literal value: {literal}.')
       result = _fhir_path_data_types.Empty
 
     return _set_and_return_type(literal, result)
 
   # TODO(b/190679571): Handle choice types, which may have more than one
   # `type.code` value present.
-  def visit_identifier(
+  def visit_identifier(  # pytype: disable=signature-mismatch  # overriding-parameter-count-checks
       self, identifier: _ast.Identifier,
       walker: _navigation.FhirStructureDefinitionWalker
   ) -> _fhir_path_data_types.FhirPathDataType:
 
     # If the identifier is `$this`, then we don't have to advance the
     # message context because `$this` is just a reference to the current
     # identifier.
@@ -201,15 +201,15 @@
     if (_utils.is_repeated_element(walker.element) and
         identifier.value != '$this'):
       data_type = _fhir_path_data_types.Collection(types={data_type})
     return _set_and_return_type(identifier, data_type)
 
   # TODO(b/215533268): Add support in semant.py's visit_indexer for multiple
   # types.
-  def visit_indexer(
+  def visit_indexer(  # pytype: disable=signature-mismatch  # overriding-parameter-count-checks
       self, indexer: _ast.Indexer,
       walker: _navigation.FhirStructureDefinitionWalker
   ) -> _fhir_path_data_types.FhirPathDataType:
     """Performs semantic type checking on `_ast.Indexer`.
 
     This function returns the datatype of an indexed item in the collection.
     If the subject of the indexer is instead a single item, then it returns its
@@ -249,15 +249,15 @@
           '', 'Semantic Analysis',
           f'Expected input collection to have single type, but got:'
           f'... {subject_type.types}.')
       return _set_and_return_type(indexer, _fhir_path_data_types.Empty)
 
     return _set_and_return_type(indexer, subject_type)
 
-  def visit_arithmetic(
+  def visit_arithmetic(  # pytype: disable=signature-mismatch  # overriding-parameter-count-checks
       self, arithmetic: _ast.Arithmetic,
       walker: _navigation.FhirStructureDefinitionWalker
   ) -> _fhir_path_data_types.FhirPathDataType:
     """Performs semantic type checking on `_ast.Arithmetic`.
 
     This function returns the datatype of the result of this Arithmetic
     operation.
@@ -295,15 +295,15 @@
     self._error_reporter.report_fhir_path_error(
         '', 'Semantic Analysis',
         f'Expected operands of compatible type for arithmetic operation but got'
         f': {lhs} {arithmetic.op} {rhs}.')
     return _set_and_return_type(arithmetic, _fhir_path_data_types.Empty)
 
   # TODO(b/210038841): Add support for non-primitive types such as Quantity.
-  def visit_type_expression(
+  def visit_type_expression(  # pytype: disable=signature-mismatch  # overriding-parameter-count-checks
       self, type_expression: _ast.TypeExpression,
       walker: _navigation.FhirStructureDefinitionWalker
   ) -> _fhir_path_data_types.FhirPathDataType:
     """Performs semantic type checking on `_ast.TypeExpression`.
 
     Right now, we only support operations where the lhs (type_specifier) is a
     string reperesenting a Primitive type:
@@ -347,15 +347,15 @@
     else:
       self._error_reporter.report_fhir_path_error(
           '', 'Semantic Analysis',
           f'Expected operand to be one of `is` or `as`, but got:'
           f'... {type_expression.op} ...')
       return _set_and_return_type(type_expression, _fhir_path_data_types.Empty)
 
-  def visit_equality(
+  def visit_equality(  # pytype: disable=signature-mismatch  # overriding-parameter-count-checks
       self, equality: _ast.EqualityRelation,
       walker: _navigation.FhirStructureDefinitionWalker
   ) -> _fhir_path_data_types.FhirPathDataType:
     """Performs semantic type checking on `_ast.EqualityRelation`.
 
     This function either returns an `Empty type` or `Boolean type`.
 
@@ -404,15 +404,15 @@
 
     self._error_reporter.report_fhir_path_error(
         '', 'Semantic Analysis',
         f'Expected operands of compatible type but got: {lhs} '
         f'{equality.op} {rhs}.')
     return _set_and_return_type(equality, _fhir_path_data_types.Empty)
 
-  def visit_comparison(
+  def visit_comparison(  # pytype: disable=signature-mismatch  # overriding-parameter-count-checks
       self, comparison: _ast.Comparison,
       walker: _navigation.FhirStructureDefinitionWalker
   ) -> _fhir_path_data_types.FhirPathDataType:
     """Performs semantic type checking on an instance of `_ast.Comparison`.
 
     For comparison, the following rules apply:
       * Comparsion operations are defined for strings, integers, decimals,
@@ -471,15 +471,15 @@
 
     self._error_reporter.report_fhir_path_error(
         '', 'Semantic Analysis',
         f'Expected operands of compatible type but got: {lhs} '
         f' {comparison.op} {rhs}.')
     return _set_and_return_type(comparison, _fhir_path_data_types.Empty)
 
-  def visit_boolean_logic(
+  def visit_boolean_logic(  # pytype: disable=signature-mismatch  # overriding-parameter-count-checks
       self, boolean_logic: _ast.BooleanLogic,
       walker: _navigation.FhirStructureDefinitionWalker
   ) -> _fhir_path_data_types.FhirPathDataType:
     """Performs semantic type checking on an instance of `_ast.BooleanLogic`.
 
     For all Boolean operators, the collections passed as operands are first
     evaluated as Booleans as described in:
@@ -527,15 +527,15 @@
       return _set_and_return_type(boolean_logic, _fhir_path_data_types.Empty)
 
     # All operands are of scalar type or empty, and therefore will be evaluated
     # according to the Boolean truth tables outlined at:
     # https://hl7.org/fhirpath/#boolean-logic at runtime.
     return _set_and_return_type(boolean_logic, _fhir_path_data_types.Boolean)
 
-  def visit_membership(
+  def visit_membership(  # pytype: disable=signature-mismatch  # overriding-parameter-count-checks
       self, membership: _ast.MembershipRelation,
       walker: _navigation.FhirStructureDefinitionWalker
   ) -> _fhir_path_data_types.FhirPathDataType:
     """Performs semantic type checking on instance of `_ast.MembershipRelation`.
 
     This includes the `in` and `contains` operators.
 
@@ -575,15 +575,15 @@
       return _set_and_return_type(membership, _fhir_path_data_types.Empty)
 
     if operand_to_check == _fhir_path_data_types.Empty:
       return _set_and_return_type(membership, _fhir_path_data_types.Empty)
 
     return _set_and_return_type(membership, _fhir_path_data_types.Boolean)
 
-  def visit_union(
+  def visit_union(  # pytype: disable=signature-mismatch  # overriding-parameter-count-checks
       self, union: _ast.UnionOp,
       walker: _navigation.FhirStructureDefinitionWalker
   ) -> _fhir_path_data_types.FhirPathDataType:
     """Performs semantic type checking on an instance of `_ast.UnionOp`.
 
     The resultant datatype of UnionOp is the union of the datatypes of the `rhs`
     and `lhs`.
@@ -615,15 +615,15 @@
         rhs_type.types if isinstance(rhs_type, _fhir_path_data_types.Collection)
         else {rhs_type})
 
     final_type_set = lhs_type_set.union(rhs_type_set)
     return _set_and_return_type(
         union, _fhir_path_data_types.Collection(types=final_type_set))
 
-  def visit_polarity(
+  def visit_polarity(  # pytype: disable=signature-mismatch  # overriding-parameter-count-checks
       self, polarity: _ast.Polarity,
       walker: _navigation.FhirStructureDefinitionWalker
   ) -> _fhir_path_data_types.FhirPathDataType:
     """Performs semantic type checking on an instance of `_ast.Polarity`.
 
     Polarity expects that its operand is a numeric type:
     `_fhir_path_data_types.Integer` or `_fhir_path_data_types.Decimal`.
@@ -642,15 +642,15 @@
       return _set_and_return_type(polarity, operand)
 
     self._error_reporter.report_fhir_path_error(
         '', 'Semantic Analysis',
         f'Expected numeric operand but got: {polarity.op} {operand}.')
     return _set_and_return_type(polarity, _fhir_path_data_types.Empty)
 
-  def visit_invocation(
+  def visit_invocation(  # pytype: disable=signature-mismatch  # overriding-parameter-count-checks
       self, invocation: _ast.Invocation,
       walker: _navigation.FhirStructureDefinitionWalker
   ) -> _fhir_path_data_types.FhirPathDataType:
     """Performs semantic type checking on an instance of `_ast.Invocation`.
 
     The resultant datatype of this invocation can be gotten from datatype of
     `invocation.rhs`.
@@ -712,15 +712,15 @@
 
     # TODO(b/193046163): Add support for arbitrary leading expressions.
     self._error_reporter.report_fhir_path_error(
         '', 'Semantic Analysis', f'Unable to resolve {invocation.rhs!r}'
         f' in the context of leading expression: {invocation.lhs!r}.')
     return _set_and_return_type(invocation, _fhir_path_data_types.Empty)
 
-  def visit_function(
+  def visit_function(  # pytype: disable=signature-mismatch  # overriding-parameter-count-checks
       self,
       function: _ast.Function,
       walker: _navigation.FhirStructureDefinitionWalker,
       operand: Optional[_ast.Expression] = None,
   ) -> _fhir_path_data_types.FhirPathDataType:
     """Performs semantic type checking on an instance of `_ast.Function`.
```

## google/fhir/core/fhir_path/_spark_interpreter.py

```diff
@@ -20,30 +20,60 @@
 from google.fhir.core.fhir_path import _ast
 from google.fhir.core.fhir_path import _evaluation
 from google.fhir.core.fhir_path import _fhir_path_data_types
 from google.fhir.core.fhir_path import _spark_sql_functions
 from google.fhir.core.fhir_path import _sql_data_types
 from google.fhir.core.fhir_path import expressions
 from google.fhir.core.internal import _primitive_time_utils
+from google.fhir.core.utils import fhir_package
+from google.fhir.r4.terminology import local_value_set_resolver
 
 
 def _escape_identifier(identifier_value: str) -> str:
   """Returns the value surrounded by backticks if it is a keyword."""
   # Keywords are case-insensitive
   if identifier_value.upper() in _sql_data_types.STANDARD_SQL_KEYWORDS:
     return f'`{identifier_value}`'
   return identifier_value  # No-op
 
 
 class SparkSqlInterpreter(_evaluation.ExpressionNodeBaseVisitor):
   """Traverses the ExpressionNode tree and generates Spark SQL recursively.
   """
 
-  def __init__(self):
-    self._use_resource_alias: Optional[bool] = None
+  def __init__(
+      self,
+      use_resource_alias: bool = False,
+      value_set_codes_table: Optional[str] = None,
+      value_set_codes_definitions: Optional[
+          fhir_package.FhirPackageManager
+      ] = None,
+  ) -> None:
+    """Creates a SparkSqlInterpreter.
+
+    Args:
+      use_resource_alias: Determines whether it is necessary to call the
+        resource table directly through an alias.
+      value_set_codes_table: The name of the database table containing value set
+        code definitions. Used when building SQL for memberOf expressions. If
+        given, value set definitions needed for memberOf expressions will be
+        retrieved from this table if they can not be found in
+        `value_set_codes_definitions`. If neither this nor
+        `value_set_codes_definitions` is given, no memberOf SQL will be
+        generated.
+      value_set_codes_definitions: A package manager containing value set
+        definitions which can be used to build SQL for memberOf expressions.
+        These value set definitions can be consulted in favor of using an
+        external `value_set_codes_table`. If neither this nor
+        `value_set_codes_definitions` is given, no memberOf SQL will be
+        generated.
+    """
+    self._use_resource_alias = use_resource_alias
+    self._value_set_codes_table = value_set_codes_table
+    self._value_set_codes_definitions = value_set_codes_definitions
 
   def encode(self,
              builder: expressions.Builder,
              select_scalars_as_array: bool = True,
              use_resource_alias: bool = False) -> str:
     """Returns a Spark SQL encoding of a FHIRPath expression.
 
@@ -73,22 +103,51 @@
     else:
       # Parenthesize raw SELECT so it can plug in anywhere an expression can.
       return f'{result.to_subquery()}'
 
   def visit_root(
       self, root: _evaluation.RootMessageNode
   ) -> Optional[_sql_data_types.IdentifierSelect]:
-    """Translates a FHIRPath root to Standard SQL."""
+    """Translates a FHIRPath root to Spark SQL."""
+    if self._use_resource_alias:
+      return _sql_data_types.IdentifierSelect(
+          _sql_data_types.Identifier(
+              _escape_identifier(root.to_fhir_path()),
+              _sql_data_types.OpaqueStruct,
+          ),
+          from_part=None,
+      )
+    return None
+
+  def visit_reference(
+      self, reference: _evaluation.ExpressionNode
+  ) -> _sql_data_types.IdentifierSelect:
+    """Translates a FHIRPath reference to Spark SQL."""
+    # When $this is used, we need the last identifier from the operand.
+    sql_alias = reference.to_fhir_path().split('.')[-1]
+    # If the identifier is `$this`, we assume that the repeated field has been
+    # unnested upstream so we only need to reference it with its alias:
+    # `{}_element_`.
+    if _fhir_path_data_types.returns_collection(reference.return_type()):
+      sql_alias = f'{sql_alias}_element_'
 
-  def visit_reference(self, reference: _evaluation.ExpressionNode) -> Any:
-    """Translates a FHIRPath reference to Standard SQL."""
+    sql_data_type = _sql_data_types.get_standard_sql_data_type(
+        reference.return_type()
+    )
+    return _sql_data_types.IdentifierSelect(
+        select_part=_sql_data_types.Identifier(
+            _escape_identifier(sql_alias), sql_data_type
+        ),
+        from_part=None,
+        sql_dialect=_sql_data_types.SqlDialect.SPARK,
+    )
 
   def visit_literal(
       self, literal: _evaluation.LiteralNode) -> _sql_data_types.RawExpression:
-    """Translates a FHIRPath literal to Standard SQL."""
+    """Translates a FHIRPath literal to Spark SQL."""
 
     if (literal.return_type() is None or
         isinstance(literal.return_type(), _fhir_path_data_types._Empty)):  # pylint: disable=protected-access
       sql_value = 'NULL'
       sql_data_type = _sql_data_types.Undefined
     # TODO(b/244184211): Make _fhir_path_data_types.FhirPathDataType classes
     # public.
@@ -162,16 +221,15 @@
             select_part=_sql_data_types.Identifier(sql_alias, sql_data_type),
             from_part=parent_result,
             sql_dialect=_sql_data_types.SqlDialect.SPARK,
         )
       else:
         sql_alias = f'{sql_alias}_element_'
         if parent_result:
-          parent_identifier_str = parent_result.sql_alias
-          identifier_str = f'{parent_identifier_str}.{raw_identifier_str}'
+          identifier_str = f'{parent_result.sql_alias}.{raw_identifier_str}'
         else:
           # Identifiers need to be escaped if they are referenced directly.
           identifier_str = f'{_escape_identifier(raw_identifier_str)}'
           return _sql_data_types.IdentifierSelect(
               select_part=_sql_data_types.Identifier(sql_alias, sql_data_type),
               from_part=(
                   f'(SELECT EXPLODE({sql_alias}) AS {sql_alias} '
@@ -189,32 +247,32 @@
           from_part = f'({parent_result}) {from_part}'
 
         return _sql_data_types.IdentifierSelect(
             select_part=_sql_data_types.Identifier(sql_alias, sql_data_type),
             from_part=from_part,
             sql_dialect=_sql_data_types.SqlDialect.SPARK,
         )
-    else:  # Scalar
-      # Append the current identifier to the path chain being selected if there
-      # is a parent. Includes the from & where clauses of the parent.
-      if parent_result:
-        return dataclasses.replace(
-            parent_result,
-            select_part=parent_result.select_part.dot(
-                raw_identifier_str,
-                sql_data_type,
-                sql_alias=_escape_identifier(sql_alias),
-            ))
-      else:
-        return _sql_data_types.IdentifierSelect(
-            select_part=_sql_data_types.Identifier(
-                _escape_identifier(identifier_str), sql_data_type),
-            from_part=parent_result,
-            sql_dialect=_sql_data_types.SqlDialect.SPARK,
-        )
+
+    # Scalar
+    select_part = _sql_data_types.Identifier(
+        _escape_identifier(identifier_str), sql_data_type
+    )
+    if parent_result:
+      select_part = parent_result.select_part.dot(
+          raw_identifier_str,
+          sql_data_type,
+          sql_alias=_escape_identifier(sql_alias),
+      )
+      return dataclasses.replace(parent_result, select_part=select_part)
+
+    return _sql_data_types.IdentifierSelect(
+        select_part=select_part,
+        from_part=None,
+        sql_dialect=_sql_data_types.SqlDialect.SPARK,
+    )
 
   def visit_indexer(self,
                     indexer: _evaluation.IndexerNode) -> _sql_data_types.Select:
     """Translates a FHIRPath indexer expression to Spark SQL.
 
     Args:
       indexer: The `_Indexer` Expression node.
@@ -334,15 +392,15 @@
       nested_query = (
           f'ARRAY({rhs_result})'
           if isinstance(equality.right, _evaluation.LiteralNode)
           else f'ARRAY_AGG({rhs_result.sql_alias}) FROM ({rhs_result})'
       )
       sql_expr = (
           f'ARRAY_EXCEPT('
-          f'(SELECT {lhs_result.sql_alias}), '
+          f'(SELECT ARRAY({lhs_result.sql_alias})), '
           f'(SELECT {nested_query})'
           ')'
       )
       return _sql_data_types.Select(
           select_part=_sql_data_types.FunctionCall(
               name=collection_check_func_name,
               params=[
@@ -350,33 +408,29 @@
                       sql_expr, _sql_data_type=_sql_data_types.Int64
                   ),
                   'x -> x IS NOT NULL',
               ],
               _sql_data_type=sql_data_type,
               _sql_alias=sql_alias,
           ),
-          from_part=(
-              '(SELECT COLLECT_LIST(*) AS'
-              f' {lhs_result.sql_alias} FROM'
-              f' {lhs_result.as_operand()})'
-          ),
+          from_part=f'(SELECT {lhs_result.as_operand()})',
           sql_dialect=_sql_data_types.SqlDialect.SPARK,
       )
 
     elif _fhir_path_data_types.is_scalar(
         equality.left.return_type()
     ) and not _fhir_path_data_types.is_scalar(equality.right.return_type()):
       nested_query = (
           f'ARRAY({lhs_result})'
           if isinstance(equality.left, _evaluation.LiteralNode)
           else f'ARRAY_AGG({lhs_result.sql_alias}) FROM ({lhs_result})'
       )
       sql_expr = (
           'ARRAY_EXCEPT('
-          f'(SELECT {rhs_result.sql_alias}), '
+          f'(SELECT ARRAY({rhs_result.sql_alias})), '
           f'(SELECT {nested_query})'
           ')'
       )
       return _sql_data_types.Select(
           select_part=_sql_data_types.FunctionCall(
               name=collection_check_func_name,
               params=[
@@ -384,19 +438,16 @@
                       sql_expr, _sql_data_type=_sql_data_types.Int64
                   ),
                   'x -> x IS NOT NULL',
               ],
               _sql_data_type=sql_data_type,
               _sql_alias=sql_alias,
           ),
-          from_part=(
-              '(SELECT COLLECT_LIST(*) AS'
-              f' {rhs_result.sql_alias} FROM'
-              f' {rhs_result.as_operand()})'
-          ),
+          from_part=f'(SELECT {rhs_result.as_operand()})',
+
           sql_dialect=_sql_data_types.SqlDialect.SPARK,
       )
     else:
       raise NotImplementedError(
           'Spark SQL does not support equality when both the left and'
           ' right-hand sides are non-scalar'
       )
@@ -511,15 +562,15 @@
 
   def visit_union(
       self, union: _evaluation.UnionNode
   )-> _sql_data_types.UnionExpression:
     """Translates a FHIRPath union to Spark SQL."""
     lhs_result = self.visit(union.left)
     rhs_result = self.visit(union.right)
-    # Supported in FHIRPath, but currently generates invalid Standard SQL.
+    # Supported in FHIRPath, but currently generates invalid Spark SQL.
     if isinstance(
         lhs_result.sql_data_type, _sql_data_types.Struct
     ) or isinstance(rhs_result.sql_data_type, _sql_data_types.Struct):
       raise TypeError(
           f'Unsupported `STRUCT` union between {lhs_result}, {rhs_result}.'
       )
 
@@ -555,20 +606,24 @@
         from_part=None,
         sql_dialect=_sql_data_types.SqlDialect.SPARK)
 
   def visit_function(self, function: _evaluation.FunctionNode) -> Any:
     """Translates a FHIRPath function to Spark SQL."""
     parent_result = self.visit(function.parent_node())
     params_result = [self.visit(p) for p in function.params()]
-    if (isinstance(function, _evaluation.MemberOfFunction) and
-        self._value_set_codes_table):
+    if isinstance(function, _evaluation.MemberOfFunction):
+      kwargs = {}
+      if self._value_set_codes_table is not None:
+        kwargs['value_set_codes_table'] = str(self._value_set_codes_table)
+      if self._value_set_codes_definitions is not None:
+        kwargs['value_set_resolver'] = local_value_set_resolver.LocalResolver(
+            self._value_set_codes_definitions
+        )
       return _spark_sql_functions.FUNCTION_MAP[function.NAME](
-          function,
-          parent_result,
-          params_result,
-          value_set_codes_table=str(self._value_set_codes_table))
+          function, parent_result, params_result, **kwargs
+      )
     func = _spark_sql_functions.FUNCTION_MAP.get(function.NAME)
     return func(function, parent_result, params_result)
 
   def wrap_where_expression(self, where_expression: str) -> str:
     """Wraps where expression to take care of repeated fields."""
     return f'(SELECT EXISTS(*, x -> x IS true) FROM {where_expression})'
```

## google/fhir/core/fhir_path/_spark_sql_functions.py

```diff
@@ -12,21 +12,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Contains classes used for getting Spark SQL equivalents of FHIRPath functions."""
 
 import copy
 import dataclasses
+import functools
+import operator
 from typing import Callable, Collection, Mapping, Optional
 
 import immutabledict
 
+from google.fhir.r4.proto.core.resources import value_set_pb2
 from google.fhir.core.fhir_path import _evaluation
 from google.fhir.core.fhir_path import _fhir_path_data_types
 from google.fhir.core.fhir_path import _sql_data_types
+from google.fhir.core.utils import url_utils
+from google.fhir.r4.terminology import local_value_set_resolver
 
 
 def count_function(
     function: _evaluation.CountFunction,
     operand_result: Optional[_sql_data_types.Select],
     params_result: Collection[_sql_data_types.StandardSqlExpression],
 ) -> _sql_data_types.Select:
@@ -57,14 +62,15 @@
             _sql_data_types.RawExpression(
                 operand_result.sql_alias,
                 _sql_data_type=operand_result.sql_data_type,
             ),
         )),
         from_part=str(operand_result.to_subquery()),
         where_part=operand_result.where_part,
+        sql_dialect=_sql_data_types.SqlDialect.SPARK,
     )
   else:
     # We don't need a sub-query because we already have a FROM.
     return dataclasses.replace(
         operand_result,
         select_part=_sql_data_types.CountCall((operand_result.select_part,)),
     )
@@ -118,14 +124,15 @@
         select_part=_sql_data_types.RawExpression(
             'CASE WHEN COUNT(*) = 0 THEN TRUE ELSE FALSE END',
             _sql_data_type=sql_data_type,
             _sql_alias=sql_alias,
         ),
         from_part=str(operand_result.to_subquery()),
         where_part=f'{operand_result.sql_alias} IS NOT NULL',
+        sql_dialect=_sql_data_types.SqlDialect.SPARK,
     )
 
 
 # TODO(b/244184211): Add support for params
 def exists_function(
     function: _evaluation.ExistsFunction,
     operand_result: Optional[_sql_data_types.Select],
@@ -186,14 +193,15 @@
         select_part=_sql_data_types.RawExpression(
             'CASE WHEN COUNT(*) = 0 THEN FALSE ELSE TRUE END',
             _sql_data_type=sql_data_type,
             _sql_alias=sql_alias,
         ),
         from_part=str(operand_result.to_subquery()),
         where_part=f'{operand_result.sql_alias} IS NOT NULL',
+        sql_dialect=_sql_data_types.SqlDialect.SPARK,
     )
 
 
 def first_function(
     function: _evaluation.FirstFunction,
     operand_result: Optional[_sql_data_types.Select],
     params_result: Collection[_sql_data_types.StandardSqlExpression],
@@ -211,30 +219,44 @@
 
   Returns:
     A compiled Spark SQL expression.
 
   Raises:
     ValueError: When the function is called without an operand
   """
-  del function, params_result  # Unused parameters in this function
+  del params_result  # Unused parameters in this function
   if operand_result is None:
     raise ValueError('first() cannot be called without an operand.')
 
-  # We append a limit 1 to get the first row in row order.
   # Note that if an ARRAY was unnested, row order may not match array order,
   # but for most FHIR this should not matter.
   result = copy.copy(operand_result)
-  return _sql_data_types.Select(
-      select_part=_sql_data_types.RawExpression(
-          sql_expr=f'FIRST({result.sql_alias})',
-          _sql_data_type=result.sql_data_type,
-          _sql_alias=result.sql_alias,
-      ),
-      from_part=f'{result.to_subquery()}',
-  )
+  if _fhir_path_data_types.is_collection(function.parent_node().return_type()):
+    return _sql_data_types.Select(
+        select_part=result.select_part,
+        from_part=(
+            f'(SELECT FIRST({result.sql_alias}) AS {result.sql_alias} FROM'
+            f' {result.to_subquery()})'
+        ),
+        sql_dialect=_sql_data_types.SqlDialect.SPARK,
+    )
+  else:
+    new_alias = result.sql_alias
+    return _sql_data_types.Select(
+        select_part=_sql_data_types.Identifier(
+            (new_alias,),
+            _sql_data_type=result.sql_data_type,
+            _sql_alias=new_alias,
+        ),
+        from_part=(
+            f'(SELECT FIRST({new_alias}) AS {new_alias} FROM'
+            f' {result.to_subquery()})'
+        ),
+        sql_dialect=_sql_data_types.SqlDialect.SPARK,
+    )
 
 
 def has_value_function(
     function: _evaluation.HasValueFunction,
     operand_result: Optional[_sql_data_types.Select],
     params_result: Collection[_sql_data_types.StandardSqlExpression],
 ) -> _sql_data_types.Select:
@@ -318,14 +340,15 @@
     return _sql_data_types.Select(
         select_part=_sql_data_types.RawExpression(
             'NULL',
             _sql_alias=sql_alias,
             _sql_data_type=sql_data_type,
         ),
         from_part=None,
+        sql_dialect=_sql_data_types.SqlDialect.SPARK,
     )
   else:
     param_to_evaluate = [param for param in params_result]
     return dataclasses.replace(
         operand_result,
         select_part=_sql_data_types.FunctionCall(
             name='REGEXP',
@@ -373,18 +396,621 @@
       operand_result,
       select_part=operand_result.select_part.dot(
           attribute, return_type, sql_alias=sql_alias
       ),
   )
 
 
+def id_for_function(
+    function: _evaluation.IdForFunction,
+    operand_result: Optional[_sql_data_types.IdentifierSelect],
+    params_result: Collection[_sql_data_types.StandardSqlExpression],
+) -> _sql_data_types.Select:
+  """Returns the raw ID for a given resource type."""
+  if operand_result is None:
+    raise ValueError('idFor() cannot be called without an operand.')
+
+  if len(params_result) != 1:
+    raise ValueError('IdForFunction must have a resource type parameter.')
+
+  # As described in
+  # https://github.com/FHIR/sql-on-fhir/blob/master/sql-on-fhir.md,
+  # this is a special case where the name of the field is based on the desired
+  # reference target, e.g. patientId or organizationId.
+  resource_type = function.base_type_str
+  # Make the first character lowercase to match the column names.
+  resource_type = resource_type[:1].lower() + resource_type[1:]
+
+  return dataclasses.replace(
+      operand_result,
+      select_part=operand_result.select_part.dot(
+          f'{resource_type}Id', _sql_data_types.String, sql_alias='idFor_'
+      ),
+  )
+
+
+def member_of_function(
+    function: _evaluation.MemberOfFunction,
+    operand_result: _sql_data_types.IdentifierSelect,
+    params_result: Collection[_sql_data_types.StandardSqlExpression],
+    value_set_codes_table: Optional[str] = None,
+    value_set_resolver: Optional[local_value_set_resolver.LocalResolver] = None,
+) -> _sql_data_types.Select:
+  """Generates Spark SQL representing the FHIRPath memberOf() function.
+
+  Returns `TRUE` if the operand is a value in the given valueset.
+
+  See the memberOf function in https://build.fhir.org/fhirpath.html#functions
+  for the full specification.
+
+  The generated SQL assumes the existence of a value set codes table as defined
+  here:
+  https://github.com/FHIR/sql-on-fhir/blob/master/sql-on-fhir.md#valueset-support
+
+  By default, the generated SQL will refer to a value set codes table named
+  VALUESET_VIEW. A value_set_codes_table argument may be supplied to use a
+  different table name. The process executing the generated SQL must have
+  permission to read this table.
+
+  This function takes one param (`valueset`) in addition to the operand. The
+  valueset must be a URI referring to a valueset known in a VALUESET_VIEW table
+  or view so the generator can expand it appropriately.
+
+  The operand may be a String, Code, Coding or CodeableConcept.
+
+  The returned SQL expression is a table of cardinality 1 for non-repeated
+  fields and of cardinality matching the number of elements in repeated fields
+  or fields with repeated parents. The table's value is of `BOOL` type.
+
+  Args:
+    function: The FHIRPath AST `MemberOfFunction` node
+    operand_result: The expression which is being evaluated
+    params_result: The parameter passed in to function
+    value_set_codes_table: The value set codes table to refer to
+    value_set_resolver: The resolver to expand value sets.
+
+  Returns:
+    A compiled Spark SQL expression.
+
+  Raises:
+    ValueError: When the function is called without an operand
+  """
+  del params_result  # Unused parameter in this function
+  operand_node = function.parent_node()
+  operand_type = operand_node.return_type()
+  sql_alias = 'memberof_'
+
+  # See if the value set has a simple definition we can expand
+  # ourselves. If so, expand the value set and generate an IN
+  # expression validating if the codes in the column are members of
+  # the value set.
+  if value_set_resolver is not None:
+    expanded_value_set = value_set_resolver.expand_value_set_url(
+        function.value_set_url
+    )
+    if expanded_value_set is not None:
+      return _member_of_sql_against_inline_value_sets(
+          sql_alias,
+          operand_result,
+          operand_type,
+          expanded_value_set,
+      )
+
+  # If we can't expand the value set ourselves, we fall back to
+  # JOIN-ing against an external value sets table.
+  if value_set_codes_table is not None:
+    return _member_of_sql_against_remote_value_set_table(
+        sql_alias,
+        operand_result,
+        operand_node,
+        operand_type,
+        function.value_set_url,
+        value_set_codes_table,
+    )
+
+  raise ValueError(
+      'Unable to expand value set %s locally and no value set'
+      ' definitions table provided. Unable to generate memberOf SQL.'
+      % function.value_set_url,
+  )
+
+
+def _member_of_sql_against_inline_value_sets(
+    sql_alias: str,
+    operand_result: _sql_data_types.IdentifierSelect,
+    operand_type: _fhir_path_data_types.FhirPathDataType,
+    expanded_value_set: value_set_pb2.ValueSet,
+) -> _sql_data_types.Select:
+  """Generates memberOf SQL using an IN statement."""
+  if isinstance(operand_type, _fhir_path_data_types.String.__class__):
+    # For strings and codes, we can just generate SQL like
+    # SELECT code IN (code1, code2...)
+    params = [
+        _sql_data_types.RawExpression(
+            '"%s"' % concept.code.value, _sql_data_types.String
+        )
+        for concept in expanded_value_set.expansion.contains
+    ]
+
+    return dataclasses.replace(
+        operand_result,
+        select_part=operand_result.select_part.is_null().or_(
+            operand_result.select_part.in_(params), _sql_alias=sql_alias
+        ),
+    )
+  if _fhir_path_data_types.is_coding(operand_type):
+    # Codings include a code system in addition to the code value,
+    # so we have to generate more complex SQL like:
+    # SELECT (system = system1 AND code IN (code1, code2)) OR
+    #        (system = system2 AND code IN (code3, code4))
+    predicate = _build_predicate_for_coding_in_value_set(
+        expanded_value_set, operand_result.select_part
+    )
+    return dataclasses.replace(
+        operand_result,
+        select_part=operand_result.select_part.is_null().or_(
+            predicate, _sql_alias=sql_alias
+        ),
+    )
+
+  if _fhir_path_data_types.is_codeable_concept(operand_type):
+    # Codeable concepts are an array of codings. We need to check if
+    # any of the codings in the array match one of the value set's
+    # bound codings. We generate SQL like:
+    # SELECT EXISTS(
+    #   SELECT 1
+    #   FROM UNNEST(codeable_concept)
+    #   WHERE (system = system1 AND code IN (code1, code2)) OR
+    #         (system = system2 AND code IN (code3, code4))
+    #
+    coding_column = operand_result.select_part.dot(
+        'coding', _sql_data_types.String
+    )
+    predicate = _build_predicate_for_coding_in_value_set(
+        expanded_value_set
+    )
+    return dataclasses.replace(
+        operand_result,
+        select_part=coding_column.is_null().or_(
+            _sql_data_types.RawExpression(
+                (
+                    'EXISTS( ('
+                    'SELECT 1 '
+                    f'FROM EXPLODE({coding_column}) '
+                    f'WHERE {predicate}), x -> x IS NOT NULL)'
+                ),
+                _sql_data_type=_sql_data_types.Boolean,
+            ),
+            _sql_alias=sql_alias,
+        ),
+    )
+
+  raise ValueError(
+      'Unexpected type %s and structure definition %s encountered'
+      % (operand_type, operand_type.url)
+  )
+
+
+def _build_predicate_for_coding_in_value_set(
+    expanded_value_set: value_set_pb2.ValueSet,
+    coding_column: Optional[_sql_data_types.Identifier] = None,
+) -> _sql_data_types.StandardSqlExpression:
+  """Builds a predicate asserting the coding column is bound to the value_set.
+
+  Ensures that the codings contained in `coding_column` are codings found in
+  `expanded_value_set`.
+  Produces SQL like:
+  (`coding_column`.system = system1 AND `coding_column`.code IN (
+    code1, code2)) OR
+  (`coding_column`.system = system2 AND `coding_column`.code IN (
+    code3, code4))
+
+  Args:
+    expanded_value_set: The expanded value set containing the coding values to
+      assert membership against.
+    coding_column: The column containing the coding values. If given, columns
+      `coding_column`.system and `coding_column`.code will be referenced in
+      the predicate. If not given, columns 'system' and 'code' will be
+      referenced.
+
+  Returns:
+    The SQL for the value set binding predicate.
+  """
+  # Group codes per code system.
+  codes_per_system = {}
+  for concept in expanded_value_set.expansion.contains:
+    codes_per_system.setdefault(concept.system.value, []).append(
+        concept.code.value
+    )
+
+  # Sort the code system entries to ensure we build stable SQL.
+  codes_per_system = list(codes_per_system.items())
+  codes_per_system.sort(key=operator.itemgetter(0))
+  for _, codes in codes_per_system:
+    codes.sort()
+
+  # Build a 'system = system AND code IN (codes)' expression per code system
+  if coding_column is None:
+    code_col = _sql_data_types.Identifier('code', _sql_data_types.String)
+    system_col = _sql_data_types.Identifier('system', _sql_data_types.String)
+  else:
+    code_col = coding_column.dot('code', _sql_data_types.String)
+    system_col = coding_column.dot('system', _sql_data_types.String)
+
+  code_system_predicates = []
+  for system, codes in codes_per_system:
+    system = _sql_data_types.RawExpression(
+        '"%s"' % system, _sql_data_types.String
+    )
+    codes = [
+        _sql_data_types.RawExpression('"%s"' % code, _sql_data_types.String)
+        for code in codes
+    ]
+    code_system_predicates.append(
+        system_col.eq_(system).and_(code_col.in_(codes))
+    )
+
+  # OR each of the above predicates.
+  return functools.reduce(
+      lambda acc, pred: acc.or_(pred), code_system_predicates
+  )
+
+
+def _member_of_sql_against_remote_value_set_table(
+    sql_alias: str,
+    operand_result: _sql_data_types.IdentifierSelect,
+    operand_node: _evaluation.ExpressionNode,
+    operand_type: _fhir_path_data_types.FhirPathDataType,
+    value_set_param: str,
+    value_set_codes_table: str,
+) -> _sql_data_types.Select:
+  """Generates memberOf SQL using a JOIN against a terminology table.."""
+  is_collection = _fhir_path_data_types.returns_collection(
+      operand_node.return_type()
+  )
+  is_string_or_code = isinstance(
+      operand_type, _fhir_path_data_types.String.__class__
+  )
+  is_coding = _fhir_path_data_types.is_coding(operand_type)
+  is_codeable_concept = _fhir_path_data_types.is_codeable_concept(
+      operand_type
+  )
+
+  value_set_uri, value_set_version = url_utils.parse_url_version(
+      value_set_param
+  )
+
+  value_set_uri_expr = f"'{value_set_uri}'"
+  if value_set_version:
+    value_set_version_predicate = (
+        f"AND vs.valuesetversion='{value_set_version}' "
+    )
+  else:
+    value_set_version_predicate = ''
+
+  if is_string_or_code and not is_collection:
+    return _sql_data_types.Select(
+        select_part=_sql_data_types.RawExpression(
+            sql_expr=f'ISNOTNULL({sql_alias})',
+            _sql_data_type=_sql_data_types.Boolean,
+            _sql_alias=sql_alias,
+        ),
+        from_part=(
+            f'(SELECT 1 AS {sql_alias} '
+            f'FROM `{value_set_codes_table}` vs '
+            'WHERE '
+            f'vs.valueseturi={value_set_uri_expr} '
+            f'{value_set_version_predicate} '
+            f'AND vs.code={operand_result.select_part}) '
+        ),
+        where_part=operand_result.where_part,
+        sql_dialect=_sql_data_types.SqlDialect.SPARK,
+    )
+  elif is_string_or_code and is_collection:
+    raise NotImplementedError('Not yet implemented for Spark')
+
+  elif is_coding and not is_collection:
+    return _sql_data_types.Select(
+        select_part=_sql_data_types.RawExpression(
+            sql_expr=f'ISNOTNULL({sql_alias})',
+            _sql_data_type=_sql_data_types.Boolean,
+            _sql_alias=sql_alias,
+        ),
+        from_part=(
+            f'(SELECT 1 AS {sql_alias} '
+            f'FROM `{value_set_codes_table}` vs '
+            'WHERE '
+            f'vs.valueseturi={value_set_uri_expr} '
+            f'{value_set_version_predicate} '
+            f'AND vs.system={operand_result.select_part}.system '
+            f'AND vs.code={operand_result.select_part}.code)'
+        ),
+        where_part=operand_result.where_part,
+        sql_dialect=_sql_data_types.SqlDialect.SPARK,
+    )
+  elif is_coding and is_collection:
+    raise NotImplementedError('Not yet implemented for Spark')
+
+  elif is_codeable_concept and not is_collection:
+    return _sql_data_types.Select(
+        select_part=_sql_data_types.RawExpression(
+            sql_expr=f'ISNOTNULL({sql_alias})',
+            _sql_data_type=_sql_data_types.Boolean,
+            _sql_alias=sql_alias,
+        ),
+        from_part=(
+            f'(SELECT 1 AS {sql_alias} '
+            f'FROM (SELECT EXPLODE({operand_result.sql_alias}.coding) '
+            'AS codings '
+            f'FROM {operand_result.to_subquery()} ) '
+            f'INNER JOIN `{value_set_codes_table}` vs '
+            f'ON vs.valueseturi={value_set_uri_expr} '
+            f'{value_set_version_predicate} '
+            'AND vs.system=codings.system '
+            'AND vs.code=codings.code)'
+        ),
+        where_part=operand_result.where_part,
+        sql_dialect=_sql_data_types.SqlDialect.SPARK,
+    )
+  elif is_codeable_concept and is_collection:
+    raise NotImplementedError('Not yet implemented for Spark')
+
+  else:
+    raise ValueError(
+        'Unexpected type %s and structure definition %s encountered'
+        % (operand_type, operand_type.url)
+    )
+
+
+def all_function(
+    function: _evaluation.AllFunction,
+    operand_result: Optional[_sql_data_types.IdentifierSelect],
+    params_result: Collection[_sql_data_types.StandardSqlExpression],
+) -> _sql_data_types.Select:
+  """Generates Spark SQL representing the FHIRPath all() function.
+
+  Returns true if criteria evaluates to true for every item in its operand.
+
+  This function takes one param (`criteria`) in addition to its operand. If
+  operand is not provided, it returns True.
+
+  Args:
+    function: The FHIRPath AST `AllFunction` node
+    operand_result: The expression which is being evaluated
+    params_result: The parameter passed in to function
+
+  Returns:
+    A compiled Spark SQL expression.
+  """
+  sql_alias = 'all_'
+  sql_data_type = _sql_data_types.Boolean
+
+  # If operand or params is not given, return TRUE.
+  if not operand_result or not params_result:
+    return _sql_data_types.Select(
+        select_part=_sql_data_types.RawExpression(
+            'TRUE',
+            _sql_alias=sql_alias,
+            _sql_data_type=_sql_data_types.Boolean,
+        ),
+        from_part=None,
+        sql_dialect=_sql_data_types.SqlDialect.SPARK,
+    )
+  else:
+    criteria = list(params_result)[0]
+
+    # There is an edge case where if the operand(context elemenet) is a
+    # repeated field then using the whole subquery causes a value error.
+    # Because the whole subquery includes `SELECT repeated_field_alias...`
+    # which causes any future reference to a field in repeated_field_alias to
+    # fail, thus we extract and use just the from_clause.
+    context_sql = None
+    where_part = None
+    if _fhir_path_data_types.is_collection(
+        function.parent_node().return_type()
+    ):
+      context_sql = operand_result.from_part
+      where_part = operand_result.where_part
+    else:
+      context_sql = str(operand_result.to_subquery())
+
+    criteria_sql = _sql_data_types.RawExpression(
+        criteria.as_operand(),
+        _sql_alias=sql_alias,
+        _sql_data_type=sql_data_type,
+    ).to_subquery()
+
+    internal_if_null_call = _sql_data_types.FunctionCall(
+        'IFNULL',
+        [criteria_sql, 'FALSE'],
+        _sql_alias=sql_alias,
+        _sql_data_type=sql_data_type,
+    )
+
+    logical_and_call = _sql_data_types.FunctionCall(
+        'BOOL_AND',
+        (internal_if_null_call,),
+        _sql_alias=sql_alias,
+        _sql_data_type=sql_data_type,
+    )
+
+    # Constructs and returns the following sql:
+    # `IF_NULL(LOGICAL_AND(IF_NULL(criteria, False)), True)`.
+    # We need the internal IF_NULL because the all function returns True if
+    # the input param / criteria is NULL
+    return _sql_data_types.Select(
+        select_part=_sql_data_types.FunctionCall(
+            'IFNULL',
+            [logical_and_call, 'TRUE'],
+            _sql_alias=sql_alias,
+            _sql_data_type=sql_data_type,
+        ),
+        from_part=context_sql,
+        where_part=where_part,
+        sql_dialect=_sql_data_types.SqlDialect.SPARK,
+    )
+
+
+def where_function(
+    function: _evaluation.WhereFunction,
+    operand_result: Optional[_sql_data_types.Select],
+    params_result: Collection[_sql_data_types.Select],
+) -> _sql_data_types.Select:
+
+  """Returns a collection of all the items that match the criteria expression.
+
+  This function takes one param (`criteria`) in addition to the operand.
+
+  If the operand is not provided the matches function returns the empty set
+  which in this function translates to NULL.
+
+  Returns an error in the event that the `criteria` param is not provided or its
+  data type is not bool.
+
+
+  Args:
+    function: The FHIRPath AST `WhereFunction` node
+    operand_result: The expression which is being evaluated
+    params_result: The parameter passed in to function
+
+  Returns:
+    A compiled Spark SQL expression.
+  """
+  del function
+  if not operand_result:
+    return _sql_data_types.Select(
+        select_part=_sql_data_types.RawExpression(
+            'NULL',
+            _sql_alias='where_clause_',
+            _sql_data_type=_sql_data_types.Undefined,
+        ),
+        from_part=None,
+        sql_dialect=_sql_data_types.SqlDialect.SPARK,
+    )
+  criteria = list(params_result)[0]
+  where_part = (
+      f'{operand_result.where_part} AND {criteria.as_operand()}'
+      if operand_result.where_part
+      else criteria.as_operand()
+  )
+
+  # Queries without a FROM clause cannot have a WHERE clause. So we create a
+  # dummy FROM clause here if needed.
+  if operand_result.from_part:
+    from_part = operand_result.from_part
+  # Include the asterix in the dummy from clause if the element is a
+  # STRUCT, because it's fields may be accessed in the where clause.
+  elif isinstance(operand_result.sql_data_type, _sql_data_types.Struct):
+    from_part = f'(SELECT {operand_result.select_part}.*)'
+
+  return _sql_data_types.Select(
+      select_part=operand_result.select_part,
+      from_part=from_part,
+      where_part=where_part,
+      sql_dialect=_sql_data_types.SqlDialect.SPARK,
+  )
+
+
+def not_function(
+    function: _evaluation.NotFunction,
+    operand_result: Optional[_sql_data_types.Select],
+    params_result: Collection[_sql_data_types.StandardSqlExpression],
+) -> _sql_data_types.Select:
+  """Generates Spark SQL representing the FHIRPath not() function.
+
+  Returns `TRUE` if the input collection evaluates to `FALSE`.
+
+  The operand is expected to be a table subquery of cardinality 1, whose value
+  is a `BOOL` type. By default, `_NotFunction` will return `FALSE` if given no
+  operator.
+
+  Args:
+    function: The FHIRPath AST `NotFunction` node
+    operand_result: The expression which is being evaluated
+    params_result: The parameter passed in to function
+
+  Returns:
+    A compiled Spark SQL expression.
+
+  Raises:
+    ValueError: When the function is called without an operand
+  """
+  del function, params_result  # Unused parameters in this function
+
+  if operand_result is None:
+    raise ValueError('not() cannot be called without an operand.')
+
+  # TODO(b/234478081):
+  # The spec says: "Returns true if the input collection evaluates to false,
+  # and false if it evaluates to true. Otherwise, the result is empty ({ })"
+  # https://hl7.org/fhirpath/#not-boolean
+  #
+  # For collections, we are returning one value per element in the
+  # collection rather than aggregating the collection elements into a single
+  # boolean value.
+  #
+  # The spec describes how to evaluate collections as single boolean values:
+  # "For all boolean operators, the collections passed as operands are first
+  # evaluated as Booleans (as described in Singleton Evaluation of
+  # Collections). The operators then use three-valued logic to propagate
+  # empty operands.
+  # https://hl7.org/fhirpath/#boolean-logic
+  #
+  # More information here:
+  # https://hl7.org/fhirpath/#singleton-evaluation-of-collections
+  return dataclasses.replace(
+      operand_result,
+      select_part=_sql_data_types.FunctionCall(
+          'NOT',
+          (operand_result.select_part,),
+          _sql_alias='not_',
+          _sql_data_type=_sql_data_types.Boolean,
+      ),
+  )
+
+
+def any_true_function(
+    function: _evaluation.AnyTrueFunction,
+    operand_result: Optional[_sql_data_types.Select],
+    params_result: Collection[_sql_data_types.StandardSqlExpression],
+) -> _sql_data_types.Select:
+
+  """Returns true if any value in the operand collection is TRUE."""
+  del function, params_result
+  if operand_result is None:
+    raise ValueError('anyTrue() cannot be called without an operand.')
+
+  sql_alias = '_anyTrue'
+  return _sql_data_types.Select(
+      select_part=_sql_data_types.FunctionCall(
+          'MAX',
+          (
+              _sql_data_types.RawExpression(
+                  operand_result.sql_alias,
+                  _sql_data_type=operand_result.sql_data_type,
+              ),
+          ),
+          _sql_data_type=_sql_data_types.Boolean,
+          _sql_alias=sql_alias,
+      ),
+      from_part=str(operand_result.to_subquery()),
+      sql_dialect=_sql_data_types.SqlDialect.SPARK,
+  )
+
+
 FUNCTION_MAP: Mapping[str, Callable[..., _sql_data_types.Select]] = (
     immutabledict.immutabledict({
         _evaluation.CountFunction.NAME: count_function,
         _evaluation.EmptyFunction.NAME: empty_function,
         _evaluation.ExistsFunction.NAME: exists_function,
         _evaluation.FirstFunction.NAME: first_function,
         _evaluation.HasValueFunction.NAME: has_value_function,
         _evaluation.MatchesFunction.NAME: matches_function,
-        _evaluation.OfTypeFunction.NAME: of_type_function
+        _evaluation.OfTypeFunction.NAME: of_type_function,
+        _evaluation.NotFunction.NAME: not_function,
+        _evaluation.IdForFunction.NAME: id_for_function,
+        _evaluation.MemberOfFunction.NAME: member_of_function,
+        _evaluation.AllFunction.NAME: all_function,
+        _evaluation.WhereFunction.NAME: where_function,
+        _evaluation.AnyTrueFunction.NAME: any_true_function,
     })
 )
```

## google/fhir/core/fhir_path/_sql_data_types.py

```diff
@@ -733,19 +733,19 @@
     lhs: The left operand.
     rhs: The right operand.
 
   Returns:
     The resulting coerced datatype, if successful.
 
   Raises:
-    TypeError: In the event that coercion is not supported.
-    ValueError: In the event that a coercion cycle is detected.
+    ValueError: In the event that a coercion cycle is detected or coercion is
+      not supported.
   """
   if not is_coercible(lhs, rhs):
-    raise TypeError(
+    raise ValueError(
         f'Unsupported Standard SQL coercion between {lhs} and {rhs}.'
     )
 
   if rhs in lhs.supported_coercion:
     return rhs
   else:  # lhs in rhs.supported_coercion
     return lhs
```

## google/fhir/core/fhir_path/_structure_definitions.py

```diff
@@ -28,29 +28,33 @@
 class Cardinality:
   """ElementDefinition field cardinality.
 
   Attributes:
     min: The minimum cardinality.
     max: The maximum cardinality. A number or *.
   """
+
   min: int
   max: str
 
 
 def build_element_definition(
     *,
     id_: str,
     type_codes: Optional[List[str]],
     cardinality: Cardinality,
     path: Optional[str] = None,
     base_path: Optional[str] = None,
-    constraints: Optional[List[
-        datatypes_pb2.ElementDefinition.Constraint]] = None,
+    constraints: Optional[
+        List[datatypes_pb2.ElementDefinition.Constraint]
+    ] = None,
     content_reference: Optional[str] = None,
     profiles: Optional[List[str]] = None,
+    slice_name: Optional[str] = None,
+    fixed: Optional[datatypes_pb2.ElementDefinition.FixedX] = None,
 ) -> datatypes_pb2.ElementDefinition:
   """Returns an `ElementDefinition` for testing FHIRPath encoding.
 
   The path is derived from the provided `id_`.
 
   Args:
     id_: The dot-separated ('.') unique identifier for inter-element
@@ -63,40 +67,53 @@
       `ElementDefinition`'s `path` will be set to `id_`. Defaults to `None`.
     base_path: An optional string denoting the `ElementDefinition.base.path`. If
       `None`, the returned `ElementDefinition`'s `base.path` will be set to
       `id_`. Defaults to `None`.
     constraints: An optional list of `ElementDefinition.Constraint`
     content_reference: An optional FHIR content reference for the element.
     profiles: An optional list of profile URLs of the `ElementDefinition`.
+    slice_name: An optional value for the slice_name attribute.
+    fixed: An optional Fixed message for the fixed attribute.
 
   Returns:
     An `ElementDefintion` for use as part of a snapshot composition within a
     `StructureDefinition`.
   """
   path = id_ if path is None else path
   base_path = id_ if base_path is None else base_path
   type_codes = [] if type_codes is None else type_codes
-  profiles = [] if profiles is None else [
-      datatypes_pb2.Canonical(value=profile) for profile in profiles
-  ]
+  profiles = (
+      []
+      if profiles is None
+      else [datatypes_pb2.Canonical(value=profile) for profile in profiles]
+  )
   type_ = [
       datatypes_pb2.ElementDefinition.TypeRef(
-          code=datatypes_pb2.Uri(value=code_value), profile=profiles)
+          code=datatypes_pb2.Uri(value=code_value), profile=profiles
+      )
       for code_value in type_codes
   ]
-  return datatypes_pb2.ElementDefinition(
-      id=datatypes_pb2.String(value=id_),
-      path=datatypes_pb2.String(value=path),
-      constraint=constraints,
-      min=datatypes_pb2.UnsignedInt(value=cardinality.min),
-      max=datatypes_pb2.String(value=cardinality.max),
-      base=datatypes_pb2.ElementDefinition.Base(
-          path=datatypes_pb2.String(value=base_path)),
-      content_reference=datatypes_pb2.Uri(value=content_reference),
-      type=type_)
+  kwargs = {
+      'id': datatypes_pb2.String(value=id_),
+      'path': datatypes_pb2.String(value=path),
+      'constraint': constraints,
+      'min': datatypes_pb2.UnsignedInt(value=cardinality.min),
+      'max': datatypes_pb2.String(value=cardinality.max),
+      'base': datatypes_pb2.ElementDefinition.Base(
+          path=datatypes_pb2.String(value=base_path)
+      ),
+      'content_reference': datatypes_pb2.Uri(value=content_reference),
+      'type': type_,
+  }
+  if slice_name is not None:
+    kwargs['slice_name'] = datatypes_pb2.String(value=slice_name)
+  if fixed is not None:
+    kwargs['fixed'] = fixed
+
+  return datatypes_pb2.ElementDefinition(**kwargs)
 
 
 def build_structure_definition(
     *,
     url: str,
     name: str,
     base_definition: str,
@@ -105,27 +122,32 @@
     derivation_code: codes_pb2.TypeDerivationRuleCode.Value,
 ) -> structure_definition_pb2.StructureDefinition:
   """Returns a `StructureDefinition` of a specialization or constraint."""
   return structure_definition_pb2.StructureDefinition(
       id=datatypes_pb2.Id(value=os.path.basename(url)),
       url=datatypes_pb2.Uri(value=url),
       kind=structure_definition_pb2.StructureDefinition.KindCode(
-          value=codes_pb2.StructureDefinitionKindCode.RESOURCE),
+          value=codes_pb2.StructureDefinitionKindCode.RESOURCE
+      ),
       fhir_version=structure_definition_pb2.StructureDefinition.FhirVersionCode(
-          value=codes_pb2.FHIRVersionCode.V_4_0_1),
+          value=codes_pb2.FHIRVersionCode.V_4_0_1
+      ),
       type=datatypes_pb2.Uri(value=type_),
       derivation=structure_definition_pb2.StructureDefinition.DerivationCode(
-          value=derivation_code),
+          value=derivation_code
+      ),
       name=datatypes_pb2.String(value=name),
       abstract=datatypes_pb2.Boolean(value=False),
       base_definition=datatypes_pb2.Canonical(value=base_definition),
       snapshot=structure_definition_pb2.StructureDefinition.Snapshot(
-          element=element_definitions),
+          element=element_definitions
+      ),
       status=structure_definition_pb2.StructureDefinition.StatusCode(
-          value=codes_pb2.PublicationStatusCode.ACTIVE),
+          value=codes_pb2.PublicationStatusCode.ACTIVE
+      ),
   )
 
 
 def build_resource_definition(
     *, id_: str, element_definitions: List[datatypes_pb2.ElementDefinition]
 ) -> structure_definition_pb2.StructureDefinition:
   """Returns a `StructureDefinition` depicting a FHIR resource.
```

## google/fhir/core/fhir_path/_utils.py

```diff
@@ -11,35 +11,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Utilities used across functions in the fhir_path module."""
 
 import itertools
+import re
 from typing import Any, List, Optional, cast
 
 from google.protobuf import message
 from google.fhir.core.utils import proto_utils
 
 # TODO(b/201107372): Update FHIR-agnostic types to a protocol.
 StructureDefinition = message.Message
 ElementDefinition = message.Message
 Constraint = message.Message
 
 
-def trim_name(raw_name: str) -> str:
-  # Trim choice field annotation if present.
-  if raw_name.endswith('[x]'):
-    raw_name = raw_name[:-3]
-  # Trim extension field annotation if present.
-  if raw_name.startswith('extension:'):
-    raw_name = raw_name[10:]
-  return raw_name
-
-
 def is_root_element(element_definition: ElementDefinition) -> bool:
   """Returns `True` if `element_definition` is the root element."""
   path_value: str = cast(Any, element_definition).path.value
   return '.' not in path_value
 
 
 def element_type_code(element_definition: ElementDefinition) -> str:
@@ -67,15 +58,16 @@
 
   Returns:
     A list of strings representing the element's type code values.
   """
   result: List[str] = []
   if proto_utils.field_is_set(element_definition, 'type'):
     type_refs: List[StructureDefinition] = proto_utils.get_value_at_field(
-        element_definition, 'type')
+        element_definition, 'type'
+    )
     result.extend([cast(Any, t).code.value for t in type_refs])
   return result
 
 
 def slice_element_urls(element_definition: ElementDefinition) -> List[str]:
   """Returns the list of profile urls for the given slice element.
 
@@ -85,35 +77,45 @@
 
   Returns:
     A list of strings representing the element's profile urls.
   """
   result: List[str] = []
   if proto_utils.field_is_set(element_definition, 'type'):
     type_refs: List[StructureDefinition] = proto_utils.get_value_at_field(
-        element_definition, 'type')
+        element_definition, 'type'
+    )
     profile_lists = [cast(Any, t).profile for t in type_refs]
     urls = [
         cast(Any, profile).value
         for profile in itertools.chain.from_iterable(profile_lists)
     ]
     result.extend(urls)
   return result
 
 
+_SLICE_ON_EXTENSION_ID_RE = re.compile(r'(^|.)extension:')
+
+
 def is_slice_on_extension(element_definition: message.Message) -> bool:
   """Returns `True` if the given element is describing a slice on an extension.
 
   More information about extensions:
   http://hl7.org/fhir/defining-extensions.html.
 
   Args:
     element_definition: The element definition (element) that we are checking.
   """
   type_codes = element_type_codes(element_definition)
-  return 'Extension' in type_codes and is_slice_element(element_definition)
+  return (
+      'Extension' in type_codes
+      and _SLICE_ON_EXTENSION_ID_RE.search(
+          cast(Any, element_definition).id.value
+      )
+      is not None
+  )
 
 
 def is_slice_element(element_definition: message.Message) -> bool:
   """Returns `True` if the `element_definition` is describing a slice.
 
   More information about slices:
   https://www.hl7.org/fhir/profiling.html#slicing.
@@ -121,14 +123,27 @@
   Args:
     element_definition: The element definition that we are checking.
   """
   id_value = cast(Any, element_definition).id.value
   return ':' in id_value
 
 
+def is_slice_but_not_on_extension(
+    element_definition: message.Message,
+) -> bool:
+  """Returns `True` if the `element_definition` is a slice not on extension.
+
+  Args:
+    element_definition: The element definition that we are checking.
+  """
+  return is_slice_element(element_definition) and not is_slice_on_extension(
+      element_definition
+  )
+
+
 def is_recursive_element(element_definition: message.Message) -> bool:
   """Returns `True` if the `element_definition` describes a recursive element.
 
   A FHIR element is recursive if it is a content reference to an element
   that is an ancestor in the structure definition. For example,
   https://www.hl7.org/fhir/parameters.html has a recursive "part" element.
 
@@ -154,16 +169,19 @@
   Args:
     uri_value: The URI of a data type or resource used for an element. This may
       be a URL or URI.
 
   Returns:
     An absolute URI to the data type or resource.
   """
-  if (uri_value.startswith('http:') or uri_value.startswith('https:') or
-      uri_value.startswith('urn:')):
+  if (
+      uri_value.startswith('http:')
+      or uri_value.startswith('https:')
+      or uri_value.startswith('urn:')
+  ):
     return uri_value  # No-op
   return f'http://hl7.org/fhir/StructureDefinition/{uri_value}'
 
 
 def get_absolute_identifier(root: str, identifier: str) -> str:
   """Returns `identifier` prefixed by '{root}.'."""
   if identifier.startswith(root):
@@ -178,23 +196,26 @@
   # specification: https://www.hl7.org/fhir/elementdefinition.html#min-max.
   if not proto_utils.field_is_set(element_definition, 'max'):
     return False
   max_value: str = cast(Any, element_definition).max.value
   return max_value != '0' and max_value != '1'
 
 
-def get_element(structdef: StructureDefinition,
-                path: str) -> Optional[ElementDefinition]:
+def get_element(
+    structdef: StructureDefinition, path: str
+) -> Optional[ElementDefinition]:
   """Returns the ElementDefintion proto for a path."""
   struct_id = cast(Any, structdef).id.value
   qualified_path = struct_id + '.' + path if path else struct_id
   qualified_choice_path = qualified_path + '[x]'
   for elem in cast(Any, structdef).snapshot.element:
-    if (elem.id.value == qualified_path or
-        elem.id.value == qualified_choice_path):
+    if (
+        elem.id.value == qualified_path
+        or elem.id.value == qualified_choice_path
+    ):
       return elem
 
   return None
 
 
 def is_backbone_element(elem: ElementDefinition) -> bool:
   for elem_type in cast(Any, elem).type:
@@ -204,15 +225,16 @@
 
 
 def is_polymorphic_element(elem: ElementDefinition) -> bool:
   return '[x]' in cast(Any, elem).id.value
 
 
 def get_patient_reference_element_paths(
-    structdef: StructureDefinition) -> List[str]:
+    structdef: StructureDefinition,
+) -> List[str]:
   """Returns all the top level patient elements for a given Reference.
 
   Args:
     structdef: a FHIR StructureDefinition proto.
 
   Returns:
     A list of patients.
@@ -220,21 +242,22 @@
   results = []
   struct_id = cast(Any, structdef).id.value
 
   for elem in cast(Any, structdef).snapshot.element:
     for t in elem.type:
       for tp in t.target_profile:
         if tp.value.endswith('Patient'):
-          results.append(elem.id.value[len(struct_id) + 1:])
+          results.append(elem.id.value[len(struct_id) + 1 :])
 
   return results
 
 
-def get_backbone_element_fields(structdef: StructureDefinition,
-                                path: str) -> List[str]:
+def get_backbone_element_fields(
+    structdef: StructureDefinition, path: str
+) -> List[str]:
   """Returns the field under the path to the given FHIR backbone element.
 
   Args:
     structdef: a FHIR StructureDefinition proto.
     path: a path to a backbone element within the structure definition.
 
   Returns:
@@ -242,31 +265,34 @@
   """
   results = []
   struct_id = cast(Any, structdef).id.value
   qualified_path = struct_id + '.' + path if path else struct_id
 
   for elem in cast(Any, structdef).snapshot.element:
     if elem.id.value.startswith(qualified_path):
-      relative_path = elem.id.value[len(qualified_path) + 1:]
+      relative_path = elem.id.value[len(qualified_path) + 1 :]
       if relative_path and '.' not in relative_path:
         # Trim choice field annotation if present.
         if relative_path.endswith('[x]'):
           relative_path = relative_path[:-3]
         results.append(relative_path)
 
   return results
 
 
 def get_root_element_definition(
-    structure_definition: StructureDefinition) -> ElementDefinition:
+    structure_definition: StructureDefinition,
+) -> ElementDefinition:
   """Returns the root element definition in a given structure definition."""
 
   root_element: ElementDefinition = None
   for element_definition in cast(Any, structure_definition).snapshot.element:
     if is_root_element(element_definition):
       if root_element is not None:
-        raise ValueError('Expected a single root ElementDefinition but got: '
-                         f'{cast(Any, root_element).id.value!r} and '
-                         f'{cast(Any, element_definition).id.value!r}.')
+        raise ValueError(
+            'Expected a single root ElementDefinition but got: '
+            f'{cast(Any, root_element).id.value!r} and '
+            f'{cast(Any, element_definition).id.value!r}.'
+        )
       root_element = element_definition
 
   return root_element
```

## google/fhir/core/fhir_path/_utils_test.py

```diff
@@ -141,19 +141,63 @@
           element=sdefs.build_element_definition(
               id_='Observation.code:loinc',
               type_codes=['Code'],
               cardinality=sdefs.Cardinality(min=0, max='1'),
           ),
           expected=False,
       ),
+      dict(
+          testcase_name='_withSliceOnNonExtensionElementOfTypeExtension',
+          element=sdefs.build_element_definition(
+              id_='Observation.code:loinc.extension',
+              type_codes=['Extension'],
+              cardinality=sdefs.Cardinality(min=0, max='1'),
+          ),
+          expected=False,
+      ),
   )
   def testIsSliceOnExtensionElement_succeeds(self, element, expected):
     self.assertEqual(_utils.is_slice_on_extension(element), expected)
 
 
+class IsSliceButNotOnExtensionElementTest(parameterized.TestCase):
+
+  @parameterized.named_parameters(
+      dict(
+          testcase_name='_withSliceOnExtensionElement',
+          element=sdefs.build_element_definition(
+              id_='Foo.extension:slice',
+              type_codes=['Extension'],
+              cardinality=sdefs.Cardinality(min=0, max='1'),
+          ),
+          expected=False,
+      ),
+      dict(
+          testcase_name='_withNonSlice',
+          element=sdefs.build_element_definition(
+              id_='Foo.nonSlice',
+              type_codes=['string'],
+              cardinality=sdefs.Cardinality(min=0, max='1'),
+          ),
+          expected=False,
+      ),
+      dict(
+          testcase_name='_withSliceOnNonExtensionElement',
+          element=sdefs.build_element_definition(
+              id_='Observation.code:loinc',
+              type_codes=['Code'],
+              cardinality=sdefs.Cardinality(min=0, max='1'),
+          ),
+          expected=True,
+      ),
+  )
+  def testIsSliceButNotOnExtensionElement_succeeds(self, element, expected):
+    self.assertEqual(_utils.is_slice_but_not_on_extension(element), expected)
+
+
 class IsRecursiveElementTest(absltest.TestCase):
 
   def testRecursiveElement_returnsTrue_withRecursiveElement(self):
     element = sdefs.build_element_definition(
         id_='recursive_elem',
         path='foo.bar.baz',
         content_reference='#foo.bar',
```

## google/fhir/core/fhir_path/context.py

```diff
@@ -243,20 +243,46 @@
       if json_name.casefold() not in possible_types:
         raise ValueError(
             f'Identifier {json_name} not in {possible_types.keys()}'
         )
       return possible_types[json_name.casefold()]
 
     if isinstance(parent, _fhir_path_data_types.StructureDataType):
-      elem = parent.children().get(json_name)
+      elem = parent.child_defs.get(json_name)
       if elem is None:
         raise ValueError(
-            f'Identifier {json_name} not in {parent.children().keys()}'
+            f'Identifier {json_name} not in {parent.child_defs.keys()}'
         )
-      return self.fhir_data_type_generator(elem, json_name, parent)
+      return_type = self.fhir_data_type_generator(elem, json_name, parent)
+      # If the element is a slice on an extension, the element definition for
+      # the slice will actually be on the slice definition instead which is
+      # stored in the value field of the child. This is essentially a shortcut
+      # for Foo.bar:slice.value when accessing Foo.bar.slice.
+      if _utils.is_slice_on_extension(elem):
+        # Complex slices may have its own extensions on it and so will not have
+        # a value field.
+        if 'value' not in return_type.child_defs:
+          return return_type
+        slice_elem = return_type.child_defs['value']
+        return_type = self.fhir_data_type_generator(
+            slice_elem, json_name, parent
+        )
+        # If there is only one type, then extract the type and return it on its
+        # lonesome. This logic only applies to extensions as they will alwyas
+        # have a field called Extension.value[x] regardless if the actual value
+        # is just a single type code. These fields with single type codes get
+        # encoded in BigQuery just the field itself instead of field.value.
+        if (
+            isinstance(return_type, _fhir_path_data_types.PolymorphicDataType)
+            and len(return_type.urls) == 1
+        ):
+          return_type = next(iter(return_type.types().values()))
+
+      return return_type
+
     else:
       raise ValueError(f'Parent {parent} does not contain children.')
 
 
 class MockFhirPathContext(FhirPathContext[_StructDefT, _ValueSetT]):
   """FHIRPath context that simply pulls from a provided list of Structure Definitions."""
```

## google/fhir/core/fhir_path/context_test.py

```diff
@@ -9,19 +9,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for FHIRPath context."""
 
+from typing import BinaryIO
+
 import requests
 import requests_mock
 
 from absl.testing import absltest
-
 # TODO(b/229908551): Eliminate R4-specific tests from this package.
 from google.fhir.r4.proto.core.resources import structure_definition_pb2
 from google.fhir.core.fhir_path import _fhir_path_data_types
 from google.fhir.core.fhir_path import context
 from google.fhir.core.utils import fhir_package
 from google.fhir.r4 import primitive_handler
 from google.fhir.r4 import r4_package
@@ -32,15 +33,18 @@
 
 class FhirPathContextTest(absltest.TestCase):
 
   @classmethod
   def setUpClass(cls):
     super().setUpClass()
     cls._package = r4_package.load_base_r4()
-    cls._package_manager = fhir_package.FhirPackageManager([cls._package])
+    us_core = []
+    cls._package_manager = fhir_package.FhirPackageManager(
+        [cls._package, us_core]
+    )
 
   def testStructDefLoad_FromFhirPackage_succeeds(self):
     test_context = context.LocalFhirPathContext(self._package)
     from_unqualified = test_context.get_structure_definition('Patient')
     self.assertEqual(from_unqualified.url.value, _PATIENT_STRUCTDEF_URL)
     from_qualified = test_context.get_structure_definition(
         _PATIENT_STRUCTDEF_URL
```

## google/fhir/core/fhir_path/expressions.py

```diff
@@ -281,15 +281,17 @@
     Args:
       criteria: An expression containing the matching logic to be applied.
 
     Returns:
       An expression that returns True if all items in the parent meet the
       criteria.
     """
-    param_nodes = self._function_args_to_nodes(self._node, [criteria])
+    param_nodes = self._function_args_to_nodes(
+        self._node, [criteria], element_of_array=True
+    )
     return Builder(
         _evaluation.AllFunction(self._node.context, self._node, param_nodes),
         self._handler,
     )
 
   def exists(self) -> 'Builder':
     """The FHIRPath exists() function.
@@ -450,15 +452,17 @@
 
     Args:
       criteria: An expression builder containing the filtering logic.
 
     Returns:
       An expression that contains the items that match the given criteria.
     """
-    param_nodes = self._function_args_to_nodes(self._node, [criteria])
+    param_nodes = self._function_args_to_nodes(
+        self._node, [criteria], element_of_array=True
+    )
     return self._builder(
         _evaluation.WhereFunction(self._node.context, self._node, param_nodes)
     )
 
   def anyTrue(self) -> 'Builder':  # pylint: disable=invalid-name
     """The FHIRPath anyTrue() function.
 
@@ -492,15 +496,18 @@
       An integer representation of its operand.
     """
     return self._builder(
         _evaluation.ToIntegerFunction(self._node.context, self._node, [])
     )
 
   def _function_args_to_nodes(
-      self, operand_node: _evaluation.ExpressionNode, args: List[Any]
+      self,
+      operand_node: _evaluation.ExpressionNode,
+      args: List[Any],
+      element_of_array: bool = False,
   ) -> List[_evaluation.ExpressionNode]:
     """Converts builder args to FHIRPath expressions into evaluation nodes."""
     params: List[_evaluation.ExpressionNode] = []
     for arg in args:
       if (
           isinstance(arg, message.Message)
           and annotation_utils.is_resource(arg)
@@ -526,15 +533,19 @@
         # For example, the "where" expression builder in
         # `patient.address.where(patient.address.use = 'home')` is built from
         # patient, but should be evaluated in the context of address.
 
         localized = arg.get_node().deepcopy()
         localized.replace_operand(
             operand_node.to_fhir_path(),
-            _evaluation.ReferenceNode(self._node.context, operand_node),
+            _evaluation.ReferenceNode(
+                self._node.context,
+                operand_node,
+                element_of_array=element_of_array,
+            ),
         )
         params.append(localized)
       else:
         # All other types are treated as literals.
         rhs_message = self._primitive_to_message(arg)
         fhir_path_str = self._primitive_to_fhir_path(arg)
         primitive_type = _fhir_path_data_types.primitive_type_from_type_code(
@@ -701,15 +712,15 @@
     """Returns a map from the base choice field name to the field types."""
     node_type = self._node.return_type()
     if not isinstance(node_type, _fhir_path_data_types.StructureDataType):
       return {}
 
     children = cast(
         _fhir_path_data_types.StructureDataType, node_type
-    ).children()
+    ).child_defs
     choice_fields = collections.defaultdict(list)
     for name, elem_def in children.items():
       # Include field and type codes for choice types (fields with > 1 type),
       # such as Observation values Quantity, CodeableConcept, etc.
       if len(elem_def.type) > 1:
         for type_code in elem_def.type:
           choice_fields[name].append(type_code.code.value)
```

## google/fhir/core/fhir_path/fhir_path_spark_test.py

```diff
@@ -10,21 +10,29 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests Python FHIRPath functionality for Spark."""
 
-from google.protobuf import message
+from typing import Optional
+import unittest.mock
+
 from absl.testing import absltest
 from absl.testing import parameterized
+
+from google.fhir.r4.proto.core.resources import value_set_pb2
+
 from google.fhir.core.fhir_path import _spark_interpreter
 from google.fhir.core.fhir_path import fhir_path_test_base
 
 
+from google.fhir.core.utils import fhir_package
+
+
 _WITH_FHIRPATH_V2_DATETIME_LITERAL_SUCCEEDS_CASES = [
     {
         'testcase_name': '_withNull',
         'fhir_path_expression': '{ }',
         'expected_sql_expression': (
             '(SELECT COLLECT_LIST(literal_) '
             'FROM (SELECT NULL AS literal_) '
@@ -671,76 +679,61 @@
             'WHERE eq_ IS NOT NULL)'
         ),
     },
     {
         'testcase_name': '_withScalarComplexComparisonRightSideScalar',
         'fhir_path_expression': "bar.bats.struct.value = '123'",
         'expected_sql_expression': (
-            '(SELECT COLLECT_LIST(eq_) '
-            'FROM (SELECT NOT EXISTS('
-            " ARRAY_EXCEPT((SELECT value), (SELECT ARRAY('123'))),"
-            ' x -> x IS NOT NULL) AS eq_ '
-            'FROM (SELECT COLLECT_LIST(*) AS value '
-            'FROM (SELECT bats_element_.struct.value '
-            'FROM (SELECT bar) LATERAL VIEW POSEXPLODE(bar.bats) '
-            'AS index_bats_element_, bats_element_)))'
+            '(SELECT COLLECT_LIST(eq_) FROM (SELECT NOT EXISTS('
+            " ARRAY_EXCEPT((SELECT ARRAY(value)), (SELECT ARRAY('123'))), x ->"
+            ' x IS NOT NULL) AS eq_ FROM (SELECT (SELECT'
+            ' bats_element_.struct.value FROM (SELECT bar) LATERAL VIEW'
+            ' POSEXPLODE(bar.bats) AS index_bats_element_, bats_element_)))'
             ' WHERE eq_ IS NOT NULL)'
         ),
     },
     {
         'testcase_name': '_withScalarComplexComparisonLeftSideScalar',
         'fhir_path_expression': " '123' = bar.bats.struct.value",
         'expected_sql_expression': (
-            '(SELECT COLLECT_LIST(eq_) '
-            'FROM (SELECT NOT EXISTS('
-            " ARRAY_EXCEPT((SELECT value), (SELECT ARRAY('123'))),"
-            ' x -> x IS NOT NULL) AS eq_ '
-            'FROM (SELECT COLLECT_LIST(*) AS value '
-            'FROM (SELECT bats_element_.struct.value '
-            'FROM (SELECT bar) LATERAL VIEW POSEXPLODE(bar.bats) '
-            'AS index_bats_element_, bats_element_)))'
+            '(SELECT COLLECT_LIST(eq_) FROM (SELECT NOT EXISTS('
+            " ARRAY_EXCEPT((SELECT ARRAY(value)), (SELECT ARRAY('123'))), x ->"
+            ' x IS NOT NULL) AS eq_ FROM (SELECT (SELECT'
+            ' bats_element_.struct.value FROM (SELECT bar) LATERAL VIEW'
+            ' POSEXPLODE(bar.bats) AS index_bats_element_, bats_element_)))'
             ' WHERE eq_ IS NOT NULL)'
         ),
     },
     {
         'testcase_name': '_withScalarComplexComparisonRightSideUnion',
         'fhir_path_expression': "bar.bats.struct.value = ('abc' | '123')",
         'expected_sql_expression': (
-            '(SELECT COLLECT_LIST(eq_) '
-            'FROM (SELECT NOT EXISTS('
-            ' ARRAY_EXCEPT((SELECT value), (SELECT ARRAY_AGG(union_) '
-            'FROM (SELECT lhs_.literal_ AS union_ '
-            "FROM (SELECT 'abc' AS literal_) AS lhs_ "
-            'UNION DISTINCT SELECT rhs_.literal_ AS union_ '
-            "FROM (SELECT '123' AS literal_) AS rhs_))),"
-            ' x -> x IS NOT NULL) AS eq_ '
-            'FROM (SELECT COLLECT_LIST(*) AS value '
-            'FROM (SELECT bats_element_.struct.value '
-            'FROM (SELECT bar) LATERAL VIEW POSEXPLODE(bar.bats) '
-            'AS index_bats_element_, bats_element_)))'
-            ' WHERE eq_ IS NOT NULL)'
+            '(SELECT COLLECT_LIST(eq_) FROM (SELECT NOT EXISTS('
+            ' ARRAY_EXCEPT((SELECT ARRAY(value)), (SELECT ARRAY_AGG(union_)'
+            " FROM (SELECT lhs_.literal_ AS union_ FROM (SELECT 'abc' AS"
+            ' literal_) AS lhs_ UNION DISTINCT SELECT rhs_.literal_ AS union_'
+            " FROM (SELECT '123' AS literal_) AS rhs_))), x -> x IS NOT NULL)"
+            ' AS eq_ FROM (SELECT (SELECT bats_element_.struct.value FROM'
+            ' (SELECT bar) LATERAL VIEW POSEXPLODE(bar.bats) AS'
+            ' index_bats_element_, bats_element_))) WHERE eq_ IS NOT NULL)'
         ),
     },
     {
         'testcase_name': '_withScalarComplexComparisonLeftSideUnion',
         'fhir_path_expression': "('abc' | '123') = bar.bats.struct.value",
         'expected_sql_expression': (
-            '(SELECT COLLECT_LIST(eq_) '
-            'FROM (SELECT NOT EXISTS('
-            ' ARRAY_EXCEPT((SELECT value), (SELECT ARRAY_AGG(union_) '
-            'FROM (SELECT lhs_.literal_ AS union_ '
-            "FROM (SELECT 'abc' AS literal_) AS lhs_ "
-            'UNION DISTINCT SELECT rhs_.literal_ AS union_ '
-            "FROM (SELECT '123' AS literal_) AS rhs_))),"
-            ' x -> x IS NOT NULL) AS eq_ '
-            'FROM (SELECT COLLECT_LIST(*) AS value '
-            'FROM (SELECT bats_element_.struct.value '
-            'FROM (SELECT bar) LATERAL VIEW POSEXPLODE(bar.bats) '
-            'AS index_bats_element_, bats_element_)))'
-            ' WHERE eq_ IS NOT NULL)'
+            '(SELECT COLLECT_LIST(eq_) FROM (SELECT NOT EXISTS('
+            ' ARRAY_EXCEPT((SELECT ARRAY(value)), (SELECT ARRAY_AGG(union_)'
+            " FROM (SELECT lhs_.literal_ AS union_ FROM (SELECT 'abc' AS"
+            ' literal_) AS lhs_ UNION DISTINCT SELECT rhs_.literal_ AS union_'
+            " FROM (SELECT '123' AS literal_) AS rhs_))), x -> x IS NOT NULL)"
+            ' AS eq_ FROM (SELECT (SELECT bats_element_.struct.value FROM'
+            ' (SELECT bar) LATERAL VIEW POSEXPLODE(bar.bats) AS'
+            ' index_bats_element_, bats_element_))) WHERE eq_ IS NOT'
+            ' NULL)'
         ),
     },
 ]
 
 _WITH_FHIRPATH_V2_FHIRPATH_MEMBER_ACCESS_SUCCEEDS_CASES = [
     {
         'testcase_name': '_withSingleMemberAccess',
@@ -910,17 +903,17 @@
         'testcase_name': '_ArrayWithMessageChoice_andEquality',
         'fhir_path_expression': (
             "multipleChoiceExample.ofType('CodeableConcept').coding.system ="
             " 'test'"
         ),
         'expected_sql_expression': (
             '(SELECT COLLECT_LIST(eq_) FROM (SELECT NOT EXISTS('
-            " ARRAY_EXCEPT((SELECT system), (SELECT ARRAY('test'))), x -> x IS"
-            ' NOT NULL) AS eq_ FROM (SELECT COLLECT_LIST(*) AS system FROM'
-            ' (SELECT coding_element_.system FROM (SELECT'
+            " ARRAY_EXCEPT((SELECT ARRAY(system)), (SELECT ARRAY('test'))), x"
+            ' -> x IS NOT NULL) AS eq_ FROM (SELECT (SELECT'
+            ' coding_element_.system FROM (SELECT'
             ' multipleChoiceExample_element_.CodeableConcept AS ofType_ FROM'
             ' (SELECT EXPLODE(multipleChoiceExample_element_) AS'
             ' multipleChoiceExample_element_ FROM (SELECT multipleChoiceExample'
             ' AS multipleChoiceExample_element_))) LATERAL VIEW'
             ' POSEXPLODE(ofType_.coding) AS index_coding_element_,'
             ' coding_element_))) WHERE eq_ IS NOT NULL)'
         ),
@@ -969,31 +962,78 @@
             'AS empty_ FROM (SELECT bats_element_.struct '
             'FROM (SELECT bar) LATERAL VIEW POSEXPLODE(bar.bats) AS '
             'index_bats_element_, bats_element_) '
             'WHERE `struct` IS NOT NULL) WHERE empty_ IS NOT NULL)'
         ),
     },
     {
+        'testcase_name': '_withMemberExistsNot',
+        'fhir_path_expression': 'bar.exists().not()',
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(not_) FROM (SELECT NOT( bar IS NOT NULL) AS'
+            ' not_) WHERE not_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withNestedMemberExistsNot',
+        'fhir_path_expression': 'bar.bats.exists().not()',
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(not_) FROM (SELECT NOT( CASE WHEN COUNT(*) ='
+            ' 0 THEN FALSE ELSE TRUE END) AS not_ FROM (SELECT bats_element_'
+            ' FROM (SELECT bar) LATERAL VIEW POSEXPLODE(bar.bats) AS'
+            ' index_bats_element_, bats_element_) WHERE bats_element_ IS NOT'
+            ' NULL) WHERE not_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withDeepestNestedMemberSqlKeywordExistsNot',
+        'fhir_path_expression': 'bar.bats.struct.exists().not()',
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(not_) FROM (SELECT NOT( CASE WHEN COUNT(*) ='
+            ' 0 THEN FALSE ELSE TRUE END) AS not_ FROM (SELECT'
+            ' bats_element_.struct FROM (SELECT bar) LATERAL VIEW'
+            ' POSEXPLODE(bar.bats) AS index_bats_element_, bats_element_) WHERE'
+            ' `struct` IS NOT NULL) WHERE not_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withLogicOnExists',
+        'fhir_path_expression': (
+            '(bar.bats.struct.value.exists() and'
+            ' bar.bats.struct.anotherValue.exists()).not()'
+        ),
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(not_) FROM (SELECT NOT( (SELECT CASE WHEN'
+            ' COUNT(*) = 0 THEN FALSE ELSE TRUE END AS exists_ FROM (SELECT'
+            ' bats_element_.struct.value FROM (SELECT bar) LATERAL VIEW'
+            ' POSEXPLODE(bar.bats) AS index_bats_element_, bats_element_) WHERE'
+            ' value IS NOT NULL) AND (SELECT CASE WHEN COUNT(*) = 0 THEN FALSE'
+            ' ELSE TRUE END AS exists_ FROM (SELECT'
+            ' bats_element_.struct.anotherValue FROM (SELECT bar) LATERAL VIEW'
+            ' POSEXPLODE(bar.bats) AS index_bats_element_, bats_element_) WHERE'
+            ' anotherValue IS NOT NULL)) AS not_) WHERE not_ IS NOT NULL)'
+        ),
+    },
+    {
         'testcase_name': '_withFirst',
         'fhir_path_expression': 'bar.bats.first()',
         'expected_sql_expression': (
-            '(SELECT COLLECT_LIST(bats_element_) '
-            'FROM (SELECT FIRST(bats_element_) AS bats_element_ '
-            'FROM (SELECT bats_element_ FROM (SELECT bar) '
-            'LATERAL VIEW POSEXPLODE(bar.bats) AS index_bats_element_, '
-            'bats_element_)) WHERE bats_element_ IS NOT NULL)'
+            '(SELECT COLLECT_LIST(bats_element_) FROM (SELECT bats_element_'
+            ' FROM (SELECT FIRST(bats_element_) AS bats_element_ FROM (SELECT'
+            ' bats_element_ FROM (SELECT bar) LATERAL VIEW POSEXPLODE(bar.bats)'
+            ' AS index_bats_element_, bats_element_))) WHERE bats_element_ IS'
+            ' NOT NULL)'
         ),
     },
     {
         'testcase_name': '_withFirstOnNonCollection',
         'fhir_path_expression': 'bar.first()',
         'expected_sql_expression': (
-            '(SELECT COLLECT_LIST(bar) '
-            'FROM (SELECT FIRST(bar) AS bar '
-            'FROM (SELECT bar)) WHERE bar IS NOT NULL)'
+            '(SELECT COLLECT_LIST(bar) FROM (SELECT bar FROM (SELECT FIRST(bar)'
+            ' AS bar FROM (SELECT bar))) WHERE bar IS NOT NULL)'
         ),
     },
     {
         'testcase_name': '_withMemberHasValue',
         'fhir_path_expression': 'bar.hasValue()',
         'expected_sql_expression': (
             '(SELECT COLLECT_LIST(has_value_) '
@@ -1076,31 +1116,351 @@
             'AS exists_ FROM (SELECT bats_element_.div '
             'FROM (SELECT bar) LATERAL VIEW POSEXPLODE(bar.bats) AS '
             'index_bats_element_, bats_element_) '
             'WHERE div IS NOT NULL) '
             'WHERE exists_ IS NOT NULL)'
         ),
     },
+    {
+        'testcase_name': '_withAllAndIdentifier',
+        'fhir_path_expression': "bat.struct.all(anotherValue = '')",
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(all_) FROM (SELECT IFNULL( BOOL_AND( IFNULL('
+            " (SELECT (`struct`.anotherValue = '') AS all_), FALSE)), TRUE) AS"
+            ' all_ FROM (SELECT bat.struct)) WHERE all_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withAllAndRepeatedSubfieldPrimitiveOnlyComparison',
+        'fhir_path_expression': "bar.bats.struct.all( value = '' )",
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(all_) FROM (SELECT IFNULL( BOOL_AND( IFNULL('
+            ' (SELECT (SELECT NOT EXISTS( ARRAY_EXCEPT((SELECT ARRAY(value)),'
+            " (SELECT ARRAY(''))), x -> x IS NOT NULL) AS eq_ FROM (SELECT"
+            ' struct_element_.value)) AS all_), FALSE)), TRUE) AS all_ FROM'
+            ' (SELECT bats_element_.struct FROM (SELECT bar) LATERAL VIEW'
+            ' POSEXPLODE(bar.bats) AS index_bats_element_, bats_element_))'
+            ' WHERE all_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withAllAndRepeatedOperandUsesExistFunction',
+        'fhir_path_expression': 'bar.all( bats.exists() )',
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(all_) FROM (SELECT IFNULL( BOOL_AND( IFNULL('
+            ' (SELECT (SELECT CASE WHEN COUNT(*) = 0 THEN FALSE ELSE TRUE END'
+            ' AS exists_ FROM (SELECT bats_element_ FROM (SELECT bar) LATERAL'
+            ' VIEW POSEXPLODE(bar.bats) AS index_bats_element_, bats_element_)'
+            ' WHERE bats_element_ IS NOT NULL) AS all_), FALSE)), TRUE) AS all_'
+            ' FROM (SELECT bar)) WHERE all_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withAllAndRepeatedParent',
+        'fhir_path_expression': 'bar.bats.all(struct.exists() )',
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(all_) FROM (SELECT IFNULL( BOOL_AND( IFNULL('
+            ' (SELECT (SELECT CASE WHEN COUNT(*) = 0 THEN FALSE ELSE TRUE END'
+            ' AS exists_ FROM (SELECT bats_element_.struct) WHERE `struct` IS'
+            ' NOT NULL) AS all_), FALSE)), TRUE) AS all_ FROM (SELECT bar)'
+            ' LATERAL VIEW POSEXPLODE(bar.bats) AS index_bats_element_,'
+            ' bats_element_) WHERE all_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withAllWithNoOperand',
+        'fhir_path_expression': 'all(bar.exists())',
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(all_) FROM (SELECT TRUE AS all_) WHERE all_'
+            ' IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_ArrayMatchesAll',
+        'fhir_path_expression': "inline.numbers.all($this.matches('regex'))",
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(all_) FROM (SELECT IFNULL( BOOL_AND( IFNULL('
+            " (SELECT REGEXP( numbers_element_, 'regex') AS all_), FALSE)),"
+            ' TRUE) AS all_ FROM (SELECT inline) LATERAL VIEW'
+            ' POSEXPLODE(inline.numbers) AS index_numbers_element_,'
+            ' numbers_element_) WHERE all_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withScalarCodeMemberOf',
+        'fhir_path_expression': (
+            "codeFlavor.code.memberOf('http://value.set/id')"
+        ),
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(memberof_) FROM (SELECT ISNOTNULL(memberof_)'
+            ' AS memberof_ FROM (SELECT 1 AS memberof_ FROM `VALUESET_VIEW` vs'
+            " WHERE vs.valueseturi='http://value.set/id'  AND"
+            ' vs.code=codeFlavor.code) ) WHERE memberof_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withScalarCodeMemberOfValueSetVersion',
+        'fhir_path_expression': (
+            "codeFlavor.code.memberOf('http://value.set/id|1.0')"
+        ),
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(memberof_) FROM (SELECT ISNOTNULL(memberof_)'
+            ' AS memberof_ FROM (SELECT 1 AS memberof_ FROM `VALUESET_VIEW` vs'
+            " WHERE vs.valueseturi='http://value.set/id' AND"
+            " vs.valuesetversion='1.0'  AND vs.code=codeFlavor.code) ) WHERE"
+            ' memberof_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withScalarCodingMemberOf',
+        'fhir_path_expression': (
+            "codeFlavor.coding.memberOf('http://value.set/id')"
+        ),
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(memberof_) FROM (SELECT ISNOTNULL(memberof_)'
+            ' AS memberof_ FROM (SELECT 1 AS memberof_ FROM `VALUESET_VIEW` vs'
+            " WHERE vs.valueseturi='http://value.set/id'  AND"
+            ' vs.system=codeFlavor.coding.system AND'
+            ' vs.code=codeFlavor.coding.code)) WHERE memberof_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withScalarCodingMemberOfValueSetVersion',
+        'fhir_path_expression': (
+            "codeFlavor.coding.memberOf('http://value.set/id|1.0')"
+        ),
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(memberof_) FROM (SELECT ISNOTNULL(memberof_)'
+            ' AS memberof_ FROM (SELECT 1 AS memberof_ FROM `VALUESET_VIEW` vs'
+            " WHERE vs.valueseturi='http://value.set/id' AND"
+            " vs.valuesetversion='1.0'  AND vs.system=codeFlavor.coding.system"
+            ' AND vs.code=codeFlavor.coding.code)) WHERE memberof_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withScalarCodeableConceptMemberOf',
+        'fhir_path_expression': (
+            "codeFlavor.codeableConcept.memberOf('http://value.set/id')"
+        ),
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(memberof_) FROM (SELECT ISNOTNULL(memberof_)'
+            ' AS memberof_ FROM (SELECT 1 AS memberof_ FROM (SELECT'
+            ' EXPLODE(codeableConcept.coding) AS codings FROM (SELECT'
+            ' codeFlavor.codeableConcept) ) INNER JOIN `VALUESET_VIEW` vs ON'
+            " vs.valueseturi='http://value.set/id'  AND"
+            ' vs.system=codings.system AND vs.code=codings.code)) WHERE'
+            ' memberof_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withScalarOfTypeCodeableConceptMemberOf',
+        'fhir_path_expression': "codeFlavor.ofType('codeableConcept').memberOf('http://value.set/id')",
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(memberof_) FROM (SELECT ISNOTNULL(memberof_)'
+            ' AS memberof_ FROM (SELECT 1 AS memberof_ FROM (SELECT'
+            ' EXPLODE(ofType_.coding) AS codings FROM (SELECT'
+            ' codeFlavor.codeableConcept AS ofType_) ) INNER JOIN'
+            " `VALUESET_VIEW` vs ON vs.valueseturi='http://value.set/id'  AND"
+            ' vs.system=codings.system AND vs.code=codings.code)) WHERE'
+            ' memberof_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withWhereAndNoOperand',
+        'fhir_path_expression': 'where(true)',
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(where_clause_) '
+            'FROM (SELECT NULL AS where_clause_) '
+            'WHERE where_clause_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withWhere',
+        'fhir_path_expression': "bat.struct.where(value='')",
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(`struct`) '
+            'FROM (SELECT bat.struct '
+            'FROM (SELECT bat.struct.*) '
+            "WHERE (`struct`.value = '')) "
+            'WHERE `struct` IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withWhereAndEmpty',
+        'fhir_path_expression': "bat.struct.where(value='').empty())",
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(empty_) '
+            'FROM (SELECT bat.struct IS NULL AS empty_ '
+            'FROM (SELECT bat.struct.*) '
+            "WHERE (`struct`.value = '')) "
+            'WHERE empty_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withChainedWhere',
+        'fhir_path_expression': (
+            "bat.struct.where(value='').where(anotherValue='')"
+        ),
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(`struct`) '
+            'FROM (SELECT bat.struct '
+            'FROM (SELECT bat.struct.*) '
+            "WHERE (`struct`.value = '') "
+            "AND (`struct`.anotherValue = '')) "
+            'WHERE `struct` IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withComplexWhere',
+        'fhir_path_expression': (
+            "bat.struct.where(value='' and anotherValue=''))"
+        ),
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(`struct`) '
+            'FROM (SELECT bat.struct '
+            'FROM (SELECT bat.struct.*) '
+            "WHERE (`struct`.value = '') "
+            "AND (`struct`.anotherValue = '')) "
+            'WHERE `struct` IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withWhereAndRepeated',
+        'fhir_path_expression': 'bar.bats.where( struct.exists() )',
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(bats_element_) FROM (SELECT bats_element_'
+            ' FROM (SELECT bar) LATERAL VIEW POSEXPLODE(bar.bats) AS'
+            ' index_bats_element_, bats_element_ WHERE (SELECT CASE WHEN'
+            ' COUNT(*) = 0 THEN FALSE ELSE TRUE END AS exists_ FROM (SELECT'
+            ' bats_element_.struct) WHERE `struct` IS NOT NULL)) WHERE'
+            ' bats_element_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withRetrieveNestedField',
+        'fhir_path_expression': "bat.struct.where(value='').anotherValue",
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(anotherValue) '
+            'FROM (SELECT bat.struct.anotherValue '
+            'FROM (SELECT bat.struct.*) '
+            "WHERE (`struct`.value = '')) "
+            'WHERE anotherValue IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withMultipleWhereClauseAndRetrieveNestedField',
+        'fhir_path_expression': (
+            "bat.struct.where(value='').where(anotherValue='').anotherValue"
+        ),
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(anotherValue) '
+            'FROM (SELECT bat.struct.anotherValue '
+            'FROM (SELECT bat.struct.*) '
+            "WHERE (`struct`.value = '') AND (`struct`.anotherValue = '')) "
+            'WHERE anotherValue IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withRetrieveNestedFieldExists',
+        'fhir_path_expression': (
+            "bat.struct.where(value='').anotherValue.exists()"
+        ),
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(exists_) '
+            'FROM (SELECT CASE WHEN COUNT(*) = 0 '
+            'THEN FALSE ELSE TRUE END AS exists_ '
+            'FROM (SELECT bat.struct.anotherValue '
+            "FROM (SELECT bat.struct.*) WHERE (`struct`.value = '')) "
+            'WHERE anotherValue IS NOT NULL) '
+            'WHERE exists_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_ArrayWithMessageChoice_andWhere',
+        'fhir_path_expression': (
+            "multipleChoiceExample.ofType('CodeableConcept').coding.where(system"
+            " = 'test')"
+        ),
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(coding_element_) FROM (SELECT coding_element_'
+            ' FROM (SELECT multipleChoiceExample_element_.CodeableConcept AS'
+            ' ofType_ FROM (SELECT EXPLODE(multipleChoiceExample_element_) AS'
+            ' multipleChoiceExample_element_ FROM (SELECT multipleChoiceExample'
+            ' AS multipleChoiceExample_element_))) LATERAL VIEW'
+            ' POSEXPLODE(ofType_.coding) AS index_coding_element_,'
+            ' coding_element_ WHERE (SELECT NOT EXISTS( ARRAY_EXCEPT((SELECT'
+            " ARRAY(system)), (SELECT ARRAY('test'))), x -> x IS NOT NULL) AS"
+            ' eq_ FROM (SELECT coding_element_.system))) WHERE coding_element_'
+            ' IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_ScalarWithRepeatedMessageChoice_andWhere',
+        'fhir_path_expression': (
+            "choiceExample.ofType('CodeableConcept').coding.where(system ="
+            " 'test')"
+        ),
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(coding_element_) FROM (SELECT'
+            ' coding_element_ FROM (SELECT choiceExample.CodeableConcept AS'
+            ' ofType_) LATERAL VIEW POSEXPLODE(ofType_.coding) AS'
+            ' index_coding_element_, coding_element_ WHERE (SELECT NOT EXISTS('
+            " ARRAY_EXCEPT((SELECT ARRAY(system)), (SELECT ARRAY('test'))), x"
+            ' -> x IS NOT NULL) AS eq_ FROM (SELECT coding_element_.system)))'
+            ' WHERE coding_element_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withAnyTrue',
+        'fhir_path_expression': 'boolList.anyTrue()',
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(_anyTrue) FROM (SELECT MAX('
+            ' boolList_element_) AS _anyTrue FROM (SELECT boolList_element_'
+            ' FROM (SELECT EXPLODE(boolList_element_) AS boolList_element_ FROM'
+            ' (SELECT boolList AS boolList_element_)))) WHERE _anyTrue IS NOT'
+            ' NULL)'
+        ),
+    },
 ]
 
 _WITH_FHIRPATH_V2_FHIRPATH_NOOPERAND_RAISES_ERROR = [
     {'testcase_name': '_withCount', 'fhir_path_expression': 'count()'},
     {'testcase_name': '_withEmpty', 'fhir_path_expression': 'empty()'},
     {'testcase_name': '_withExists', 'fhir_path_expression': 'exists()'},
     {'testcase_name': '_withFirst', 'fhir_path_expression': 'first()'},
     {'testcase_name': '_withHasValue', 'fhir_path_expression': 'hasValue()'},
     {'testcase_name': '_withMatches', 'fhir_path_expression': 'matches()'},
     {'testcase_name': '_withOfType', 'fhir_path_expression': 'ofType()'},
+    {'testcase_name': '_withIdFor', 'fhir_path_expression': 'idFor()'},
+    {'testcase_name': '_withAll', 'fhir_path_expression': 'all()'},
+    {'testcase_name': '_withMemberOf', 'fhir_path_expression': 'memberOf()'},
+    {'testcase_name': '_withNot', 'fhir_path_expression': 'not()'},
+    {'testcase_name': '_withAnyTrue', 'fhir_path_expression': 'anyTrue()'},
 ]
 
-_WITH_FHIRPATH_V2_FHIRPATH_EXISTS_WITH_PARAM_RAISES_ERROR = [
+_WITH_FHIRPATH_V2_FHIRPATH_FUNCTION_INVOCATION_RAISES_VALUE_ERROR = [
     {
         'testcase_name': '_withArrayScalarMemberExists',
         'fhir_path_expression': 'bar.exists(struct)'
     },
+    {
+        'testcase_name': '_withWhereFunctionAndNoCriteria',
+        'fhir_path_expression': 'bat.struct.where()'
+    },
+    {
+        'testcase_name': '_withWhereFunctionAndNonBoolCriteria',
+        'fhir_path_expression': 'bat.struct.where(value)'
+    },
+]
+
+_WITH_FHIRPATH_V2_FHIRPATH_FUNCTION_INVOCATION_RAISES_NOT_IMPLEMENTED_ERROR = [
+    {
+        'testcase_name': '_withWhereAndRepeatedAndExists',
+        'fhir_path_expression': 'bar.bats.where( struct = struct ).exists()'
+    },
 ]
 
 _WITH_FHIRPATH_V2_FHIRPATH_MEMBER_FUNCTION_UNION_FUNCTION_SUCCEEDS_CASES = [
     {
         'testcase_name': '_withIntegerUnion',
         'fhir_path_expression': '3 | 4',
         'expected_sql_expression': (
@@ -1141,209 +1501,391 @@
             'SELECT rhs_.literal_ AS union_ '
             'FROM (SELECT \'Bats\' AS literal_) AS rhs_) '
             'WHERE union_ IS NOT NULL)'
         ),
     },
 ]
 
+_WITH_FHIRPATH_V2_FHIRPATH_MEMBER_OF_VECTOR_EXPRESSIONS_RAISES_ERROR = [
+    {
+        'testcase_name': '_withVectorCodeMemberOf',
+        'fhir_path_expression': (
+            "codeFlavors.code.memberOf('http://value.set/id')"
+        ),
+    },
+    {
+        'testcase_name': '_withVectorCodeableConceptMemberOf',
+        'fhir_path_expression': (
+            "codeFlavors.codeableConcept.memberOf('http://value.set/id')"
+        ),
+    },
+    {
+        'testcase_name': '_withVectorCodingMemberOf',
+        'fhir_path_expression': (
+            "codeFlavors.coding.memberOf('http://value.set/id')"
+        ),
+    },
+    {
+        'testcase_name': '_withVectorOfTypeCodeableConceptMemberOf',
+        'fhir_path_expression': "codeFlavors.ofType('codeableConcept').memberOf('http://value.set/id')",
+    },
+]
+
+_WITH_FHIRPATH_V2_MEMBER_OF_AGAINST_LOCAL_VALUESET_DEFINITIONS_SUCCEEDS_CASES = [
+    {
+        'testcase_name': '_withScalarCodeMemberOf',
+        'fhir_path_expression': (
+            "codeFlavor.code.memberOf('http://value.set/1')"
+        ),
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(memberof_) FROM (SELECT (codeFlavor.code IS'
+            ' NULL) OR (codeFlavor.code IN ("code_1", "code_2")) AS memberof_)'
+            ' WHERE memberof_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withScalarCodeMemberOfAnotherValueSet',
+        'fhir_path_expression': (
+            "codeFlavor.code.memberOf('http://value.set/2')"
+        ),
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(memberof_) FROM (SELECT (codeFlavor.code IS'
+            ' NULL) OR (codeFlavor.code IN ("code_3", "code_4", "code_5")) AS'
+            ' memberof_) WHERE memberof_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withVectorCodeMemberOf',
+        'fhir_path_expression': (
+            "codeFlavors.code.memberOf('http://value.set/1')"
+        ),
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(memberof_) FROM (SELECT'
+            ' (codeFlavors_element_.code IS NULL) OR (codeFlavors_element_.code'
+            ' IN ("code_1", "code_2")) AS memberof_ FROM (SELECT'
+            ' EXPLODE(codeFlavors_element_) AS codeFlavors_element_ FROM'
+            ' (SELECT codeFlavors AS codeFlavors_element_))) WHERE memberof_ IS'
+            ' NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withScalarCodingMemberOf',
+        'fhir_path_expression': (
+            "codeFlavor.coding.memberOf('http://value.set/2')"
+        ),
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(memberof_) FROM (SELECT (codeFlavor.coding IS'
+            ' NULL) OR (((codeFlavor.coding.system = "system_3") AND'
+            ' (codeFlavor.coding.code IN ("code_3", "code_4"))) OR'
+            ' ((codeFlavor.coding.system = "system_5") AND'
+            ' (codeFlavor.coding.code IN ("code_5")))) AS memberof_) WHERE'
+            ' memberof_ IS NOT NULL)'
+        ),
+    },
+    {
+        'testcase_name': '_withScalarCodeableConceptMemberOf',
+        'fhir_path_expression': (
+            "codeFlavor.codeableConcept.memberOf('http://value.set/2')"
+        ),
+        'expected_sql_expression': (
+            '(SELECT COLLECT_LIST(memberof_) FROM (SELECT'
+            ' (codeFlavor.codeableConcept.coding IS NULL) OR EXISTS( (SELECT 1'
+            ' FROM EXPLODE(codeFlavor.codeableConcept.coding) WHERE'
+            ' ((system = "system_3") AND (code IN ("code_3", "code_4"))) OR'
+            ' ((system = "system_5") AND (code IN ("code_5")))), x -> x IS NOT'
+            ' NULL) AS memberof_) WHERE memberof_ IS NOT NULL)'
+        ),
+    },
+]
+
 
 class FhirPathSparkSqlEncoderTest(
     fhir_path_test_base.FhirPathTestBase, parameterized.TestCase
 ):
   """Unit tests for `fhir_path.FhirPathSparkSqlEncoder`."""
 
   def assertEvaluationNodeSqlCorrect(
       self,
-      structdef: message.Message,
+      structdef_name: str,
       fhir_path_expression: str,
       expected_sql_expression: str,
       select_scalars_as_array: bool = True,
+      use_resource_alias: bool = False,
+      value_set_codes_definitions: Optional[
+          fhir_package.FhirPackageManager
+      ] = None,
   ) -> None:
-    builder = self.create_builder_from_str(structdef, fhir_path_expression)
+    builder = self.create_builder_from_str(structdef_name, fhir_path_expression)
 
-    actual_sql_expression = _spark_interpreter.SparkSqlInterpreter().encode(
-        builder, select_scalars_as_array=select_scalars_as_array
+    actual_sql_expression = _spark_interpreter.SparkSqlInterpreter(
+        value_set_codes_table='VALUESET_VIEW',
+        value_set_codes_definitions=value_set_codes_definitions,
+    ).encode(
+        builder,
+        select_scalars_as_array=select_scalars_as_array,
+        use_resource_alias=use_resource_alias,
     )
     self.assertEqual(
         actual_sql_expression.replace('\n', ' '), expected_sql_expression
     )
 
   @parameterized.named_parameters(
       _WITH_FHIRPATH_V2_DATETIME_LITERAL_SUCCEEDS_CASES
   )
   def testEncode_withFhirPathV2DateTimeLiteral_succeeds(
       self, fhir_path_expression: str, expected_sql_expression: str
   ):
     self.assertEvaluationNodeSqlCorrect(
-        None, fhir_path_expression, expected_sql_expression
+        'Foo', fhir_path_expression, expected_sql_expression
     )
 
   @parameterized.named_parameters(_WITH_FHIRPATH_V2_ARITHMETIC_SUCCEEDS_CASES)
   def testEncode_withFhirPathV2LiteralArithmetic_succeeds(
       self, fhir_path_expression: str, expected_sql_expression: str
   ):
     self.assertEvaluationNodeSqlCorrect(
-        structdef=None,
+        structdef_name='Foo',
         fhir_path_expression=fhir_path_expression,
         expected_sql_expression=expected_sql_expression,
-        select_scalars_as_array=True,
     )
 
   @parameterized.named_parameters(_WITH_FHIRPATH_V2_INDEXER_SUCCEEDS_CASES)
   def testEncode_withFhirPathV2LiteralIndexer_succeeds(
       self, fhir_path_expression: str, expected_sql_expression: str
   ):
     self.assertEvaluationNodeSqlCorrect(
-        structdef=None,
+        structdef_name='Foo',
         fhir_path_expression=fhir_path_expression,
         expected_sql_expression=expected_sql_expression,
-        select_scalars_as_array=True,
     )
 
   @parameterized.named_parameters(_WITH_FHIRPATH_V2_BOOLEAN_SUCCEEDS_CASES)
   def testEncode_withFhirPathV2LiteralBoolean_succeeds(
       self, fhir_path_expression: str, expected_sql_expression: str
   ):
     self.assertEvaluationNodeSqlCorrect(
-        structdef=None,
+        structdef_name='Foo',
         fhir_path_expression=fhir_path_expression,
         expected_sql_expression=expected_sql_expression,
-        select_scalars_as_array=True,
     )
 
   @parameterized.named_parameters(_WITH_FHIRPATH_V2_COMPARISON_SUCCEEDS_CASES)
   def testEncode_withFhirPathV2LiteralComparison_succeeds(
       self, fhir_path_expression: str, expected_sql_expression: str
   ):
     self.assertEvaluationNodeSqlCorrect(
-        structdef=self.foo,
+        structdef_name='Foo',
         fhir_path_expression=fhir_path_expression,
         expected_sql_expression=expected_sql_expression,
-        select_scalars_as_array=True,
     )
 
   @parameterized.named_parameters(_WITH_FHIRPATH_V2_POLARITY_SUCCEEDS_CASES)
   def testEncode_withFhirPathV2LiteralPolarity_succeeds(
       self, fhir_path_expression: str, expected_sql_expression: str
   ):
     self.assertEvaluationNodeSqlCorrect(
-        structdef=None,
+        structdef_name='Foo',
         fhir_path_expression=fhir_path_expression,
         expected_sql_expression=expected_sql_expression,
-        select_scalars_as_array=True,
     )
     self.assertEvaluationNodeSqlCorrect(
-        structdef=self.foo,
+        structdef_name='Foo',
         fhir_path_expression=fhir_path_expression,
         expected_sql_expression=expected_sql_expression,
-        select_scalars_as_array=True,
     )
 
   @parameterized.named_parameters(_WITH_FHIRPATH_V2_EQUALITY_SUCCEEDS_CASES)
   def testEncode_withFhirPathV2LiteralEquality_succeeds(
       self,
       fhir_path_expression: str,
       expected_sql_expression: str,
-      select_scalars_as_array=True,
   ):
     self.assertEvaluationNodeSqlCorrect(
-        structdef=self.foo,
+        structdef_name='Foo',
         fhir_path_expression=fhir_path_expression,
         expected_sql_expression=expected_sql_expression,
-        select_scalars_as_array=select_scalars_as_array,
     )
 
   @parameterized.named_parameters(_WITH_FHIRPATH_V2_MEMBERSHIP_SUCCEEDS_CASES)
   def testEncode_withFhirPathV2LiteralMembershipRelation_succeeds(
       self, fhir_path_expression: str, expected_sql_expression: str
   ):
     self.assertEvaluationNodeSqlCorrect(
-        structdef=None,
+        structdef_name='Foo',
         fhir_path_expression=fhir_path_expression,
         expected_sql_expression=expected_sql_expression,
-        select_scalars_as_array=True,
     )
 
   @parameterized.named_parameters(
       _WITH_FHIRPATH_V2_FHIRPATH_MEMBER_ACCESS_SUCCEEDS_CASES
   )
   def testEncode_withFhirPathV2MemberAccess_succeeds(
       self, fhir_path_expression: str, expected_sql_expression: str
   ):
     self.assertEvaluationNodeSqlCorrect(
-        structdef=self.foo,
+        structdef_name='Foo',
         fhir_path_expression=fhir_path_expression,
         expected_sql_expression=expected_sql_expression,
-        select_scalars_as_array=True,
     )
 
   @parameterized.named_parameters(
       _WITH_FHIRPATH_V2_FHIRPATH_OFTYPE_FUNCTION_SUCCEEDS_CASES
   )
   def testEncode_withFhirPathV2OfTypeInvocation_succeeds(
       self, fhir_path_expression: str, expected_sql_expression: str
   ):
     self.assertEvaluationNodeSqlCorrect(
-        structdef=self.foo,
+        structdef_name='Foo',
         fhir_path_expression=fhir_path_expression,
         expected_sql_expression=expected_sql_expression,
-        select_scalars_as_array=True,
     )
 
   @parameterized.named_parameters(
       _WITH_FHIRPATH_V2_FHIRPATH_FUNCTION_INVOCATION_SUCCEEDS_CASES
   )
   def testEncode_withFhirPathV2FunctionInvocation_succeeds(
       self, fhir_path_expression: str, expected_sql_expression: str
   ):
     self.assertEvaluationNodeSqlCorrect(
-        structdef=self.foo,
+        structdef_name='Foo',
         fhir_path_expression=fhir_path_expression,
         expected_sql_expression=expected_sql_expression,
         select_scalars_as_array=True,
     )
 
   @parameterized.named_parameters(
+      _WITH_FHIRPATH_V2_MEMBER_OF_AGAINST_LOCAL_VALUESET_DEFINITIONS_SUCCEEDS_CASES
+  )
+  def testEncode_withFhirPathV2MemberFunctionAgainstLocalValueSetDefinitions_succeeds(
+      self, fhir_path_expression: str, expected_sql_expression: str
+  ):
+    expanded_value_set_1 = value_set_pb2.ValueSet()
+    expanded_value_set_1.url.value = 'http://value.set/1'
+
+    code_1 = expanded_value_set_1.expansion.contains.add()
+    code_1.code.value = 'code_1'
+    code_1.system.value = 'system_1'
+
+    code_2 = expanded_value_set_1.expansion.contains.add()
+    code_2.code.value = 'code_2'
+    code_2.system.value = 'system_2'
+
+    expanded_value_set_2 = value_set_pb2.ValueSet()
+    expanded_value_set_2.url.value = 'http://value.set/2'
+
+    # The following two codes are in the same code system.
+    code_3 = expanded_value_set_2.expansion.contains.add()
+    code_3.code.value = 'code_3'
+    code_3.system.value = 'system_3'
+
+    code_4 = expanded_value_set_2.expansion.contains.add()
+    code_4.code.value = 'code_4'
+    code_4.system.value = 'system_3'
+
+    code_4 = expanded_value_set_2.expansion.contains.add()
+    code_4.code.value = 'code_5'
+    code_4.system.value = 'system_5'
+
+    self.assertEvaluationNodeSqlCorrect(
+        'Foo',
+        fhir_path_expression,
+        expected_sql_expression,
+        # Build a mock package manager which returns resources for the value
+        # sets above.
+        value_set_codes_definitions=unittest.mock.Mock(
+            get_resource={
+                expanded_value_set_1.url.value: expanded_value_set_1,
+                expanded_value_set_2.url.value: expanded_value_set_2,
+            }.get
+        ),
+    )
+
+  @parameterized.named_parameters(
       _WITH_FHIRPATH_V2_FHIRPATH_NOOPERAND_RAISES_ERROR
   )
   def testEncode_withFhirPathFunctionNoOperand_raisesError(
       self, fhir_path_expression: str
   ):
     with self.assertRaises(ValueError):
-      builder = self.create_builder_from_str(self.foo, fhir_path_expression)
+      builder = self.create_builder_from_str('Foo', fhir_path_expression)
       _spark_interpreter.SparkSqlInterpreter().encode(builder)
 
   @parameterized.named_parameters(
-      _WITH_FHIRPATH_V2_FHIRPATH_EXISTS_WITH_PARAM_RAISES_ERROR
+      _WITH_FHIRPATH_V2_FHIRPATH_FUNCTION_INVOCATION_RAISES_VALUE_ERROR
   )
-  def testEncode_withFhirPathFunctionExistsWithParam_raisesError(
+  def testEncode_withFhirPathFunctionInvocation_raisesValueError(
       self, fhir_path_expression: str
   ):
     with self.assertRaises(ValueError):
-      builder = self.create_builder_from_str(self.foo, fhir_path_expression)
-      self.spark_interpreter.encode(builder)
+      self.create_builder_from_str('Foo', fhir_path_expression)
+
+  @parameterized.named_parameters(
+      _WITH_FHIRPATH_V2_FHIRPATH_FUNCTION_INVOCATION_RAISES_NOT_IMPLEMENTED_ERROR
+  )
+  def testEncode_withFhirPathFunctionInvocation_raisesNotImplementedError(
+      self, fhir_path_expression: str
+  ):
+    with self.assertRaises(NotImplementedError):
+      builder = self.create_builder_from_str('Foo', fhir_path_expression)
+
+      _spark_interpreter.SparkSqlInterpreter().encode(builder)
+
+  @parameterized.named_parameters(
+      _WITH_FHIRPATH_V2_FHIRPATH_MEMBER_OF_VECTOR_EXPRESSIONS_RAISES_ERROR
+  )
+  def testEncode_withFhirPathV2MemberOfFunctionWithVectorExpression_raisesError(
+      self, fhir_path_expression: str
+  ):
+    with self.assertRaises(NotImplementedError):
+      builder = self.create_builder_from_str('Foo', fhir_path_expression)
+      _spark_interpreter.SparkSqlInterpreter(
+          value_set_codes_table='VALUESET_VIEW'
+      ).encode(builder)
 
   def testEncode_withFhirPathV2SelectScalarsAsArrayFalseForLiteral_succeeds(
       self,
   ):
     fhir_path_expression = 'true'
     expected_sql_expression = '(SELECT TRUE AS literal_)'
     self.assertEvaluationNodeSqlCorrect(
-        structdef=self.foo,
+        structdef_name='Foo',
         fhir_path_expression=fhir_path_expression,
         expected_sql_expression=expected_sql_expression,
         select_scalars_as_array=False,
     )
 
   @parameterized.named_parameters(
       _WITH_FHIRPATH_V2_FHIRPATH_MEMBER_FUNCTION_UNION_FUNCTION_SUCCEEDS_CASES
   )
   def testEncode_withFhirPathMemberV2LiteralUnion_succeeds(
       self, fhir_path_expression: str, expected_sql_expression: str
   ):
     self.assertEvaluationNodeSqlCorrect(
-        structdef=self.foo,
+        structdef_name='Foo',
         fhir_path_expression=fhir_path_expression,
         expected_sql_expression=expected_sql_expression,
-        select_scalars_as_array=True)
+    )
+
+  def testEncode_withFhirPathMemberV2LiteralRoot_succeeds(self):
+    expected_sql_expression = (
+        '(SELECT COLLECT_LIST(bar) FROM (SELECT Foo.bar) WHERE bar IS NOT NULL)'
+    )
+    self.assertEvaluationNodeSqlCorrect(
+        structdef_name='Foo',
+        fhir_path_expression='Foo.bar',
+        expected_sql_expression=expected_sql_expression,
+        use_resource_alias=True,
+    )
+
+  def testEncode_withFhirPathMemberV2IdFor_succeeds(self):
+    self.assertEvaluationNodeSqlCorrect(
+        structdef_name='Foo',
+        fhir_path_expression="bar.idFor('Bats')",
+        expected_sql_expression=(
+            '(SELECT COLLECT_LIST(idFor_) FROM (SELECT bar.batsId AS'
+            ' idFor_) WHERE idFor_ IS NOT NULL)'
+        ),
+    )
+
+
 if __name__ == '__main__':
   absltest.main()
```

## google/fhir/core/fhir_path/fhir_path_test.py

```diff
@@ -12,83 +12,88 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests Python FHIRPath functionality."""
 
 import copy
 import textwrap
-from typing import cast, Dict, List, Optional
+from typing import Dict, List, Optional, cast
 import unittest.mock
 
 from google.cloud import bigquery
 
-from google.protobuf import message
 from absl.testing import absltest
 from absl.testing import parameterized
 from google.fhir.core.proto import fhirpath_replacement_list_pb2
 from google.fhir.core.proto import validation_pb2
 from google.fhir.r4.proto.core import codes_pb2
 from google.fhir.r4.proto.core import datatypes_pb2
 from google.fhir.r4.proto.core.resources import structure_definition_pb2
 from google.fhir.r4.proto.core.resources import value_set_pb2
 from google.fhir.core import fhir_errors
+# TODO(b/268404151): Remove copybara once core/execution is supported.
 from google.fhir.core.fhir_path import _bigquery_interpreter
 from google.fhir.core.fhir_path import _structure_definitions as sdefs
+from google.fhir.core.fhir_path import context as context_lib
 from google.fhir.core.fhir_path import fhir_path
 from google.fhir.core.fhir_path import fhir_path_options
 from google.fhir.core.fhir_path import fhir_path_test_base
 from google.fhir.core.fhir_path import fhir_path_validator
 from google.fhir.core.fhir_path import fhir_path_validator_v2
+# TODO(b/268404151): Remove copybara once core/execution is supported.
 from google.fhir.r4 import primitive_handler
+
+
 # TODO(b/244184211): Make FHIR-version agnostic (e.g. parameterize on module?)
 # TODO(b/197976399): Move unit tests to snapshot testing framework.
 
 # TODO(b/249835149): Add corresponding tests internally for all examples in the
 # public FHIR views.
 
 
 class FhirPathStandardSqlEncoderTest(
     fhir_path_test_base.FhirPathTestBase, parameterized.TestCase
 ):
   """Unit tests for `fhir_path.FhirPathStandardSqlEncoder`."""
 
   def assertEvaluationNodeSqlCorrect(
       self,
-      structdef: message.Message,
+      structdef_name: str,
       fhir_path_expression: str,
       expected_sql_expression: str,
       select_scalars_as_array: bool = True,
+      check_elm_nodes: bool = False,
       **bq_interpreter_args,
   ) -> None:
-    builder = self.create_builder_from_str(structdef, fhir_path_expression)
+    builder = self.create_builder_from_str(structdef_name, fhir_path_expression)
 
     actual_sql_expression = _bigquery_interpreter.BigQuerySqlInterpreter(
         **bq_interpreter_args
     ).encode(builder, select_scalars_as_array=select_scalars_as_array)
 
     self.assertEqual(actual_sql_expression, expected_sql_expression)
 
   def testElementDefs_inBuilder(self):
     """Tests passing element defs to children identifiers."""
     fhir_path_expression = 'bar.bats.struct.value'
-    builder = self.create_builder_from_str(self.foo, fhir_path_expression)
+    builder = self.create_builder_from_str('Foo', fhir_path_expression)
 
     expected_element_def = sdefs.build_element_definition(
         id_='Struct.value',
         type_codes=['string'],
         cardinality=sdefs.Cardinality(min=0, max='1'),
     )
     self.assertEqual(
         builder.return_type.root_element_definition, expected_element_def
     )
 
   def testElementDefs_notInBuilder(self):
     """Tests that element defs will not exist if a function is called on the builder."""
     fhir_path_expression = 'bar.bats.struct'
-    builder = self.create_builder_from_str(self.foo, fhir_path_expression)
+    builder = self.create_builder_from_str('Foo', fhir_path_expression)
     expected_element_def = sdefs.build_element_definition(
         id_='Struct',
         type_codes=None,
         cardinality=sdefs.Cardinality(min=0, max='1'),
     )
 
     self.assertEqual(
@@ -445,27 +450,31 @@
           expected_sql_expression=textwrap.dedent("""\
           ARRAY(SELECT eq_
           FROM (SELECT (SAFE_CAST('2015-02-04T14:34:28+00:00' AS TIMESTAMP) = SAFE_CAST('2015-02-04T14:00:00+00:00' AS TIMESTAMP)) AS eq_)
           WHERE eq_ IS NOT NULL)"""),
       ),
   )
   def testEncode_withFhirPathV2DateTimeLiteral_succeeds(
-      self, fhir_path_expression: str, expected_sql_expression: str
+      self,
+      fhir_path_expression: str,
+      expected_sql_expression: str,
   ):
     self.assertEvaluationNodeSqlCorrect(
-        None, fhir_path_expression, expected_sql_expression
+        'Foo',
+        fhir_path_expression,
+        expected_sql_expression,
     )
 
   def testEncode_withFhirPathV2SelectScalarsAsArrayFalseForLiteral_succeeds(
       self,
   ):
     fhir_path_expression = 'true'
     expected_sql_expression = '(SELECT TRUE AS literal_)'
     self.assertEvaluationNodeSqlCorrect(
-        structdef=self.foo,
+        structdef_name='Foo',
         fhir_path_expression=fhir_path_expression,
         expected_sql_expression=expected_sql_expression,
         select_scalars_as_array=False,
     )
 
   def testEncode_SelectScalarsAsArrayFalseForLiteral_succeeds(self):
     actual_sql_expression = self.fhir_path_encoder.encode(
@@ -485,15 +494,15 @@
         structure_definition=self.foo,
         element_definition=None,
         fhir_path_expression=fhir_path_expression,
         select_scalars_as_array=False,
     )
     self.assertEqual(actual_sql_expression, expected_sql_expression)
     self.assertEvaluationNodeSqlCorrect(
-        self.foo,
+        'Foo',
         fhir_path_expression,
         expected_sql_expression,
         select_scalars_as_array=False,
     )
 
   @parameterized.named_parameters(
       dict(
@@ -639,15 +648,17 @@
     actual_sql_expression = self.fhir_path_encoder.encode(
         structure_definition=self.foo,
         element_definition=self.foo_root,
         fhir_path_expression=fhir_path_expression,
     )
     self.assertEqual(actual_sql_expression, expected_sql_expression)
     self.assertEvaluationNodeSqlCorrect(
-        None, fhir_path_expression, expected_sql_expression
+        'Foo',
+        fhir_path_expression,
+        expected_sql_expression,
     )
 
   @parameterized.named_parameters(
       dict(
           testcase_name='_withBooleanAnd',
           fhir_path_expression='true and false',
           expected_sql_expression=textwrap.dedent("""\
@@ -710,14 +721,22 @@
           fhir_path_expression='true xor false',
           expected_sql_expression=textwrap.dedent("""\
           ARRAY(SELECT logic_
           FROM (SELECT (TRUE <> FALSE) AS logic_)
           WHERE logic_ IS NOT NULL)"""),
       ),
       dict(
+          testcase_name='_withBooleanImplies',
+          fhir_path_expression='true implies false',
+          expected_sql_expression=textwrap.dedent("""\
+          ARRAY(SELECT logic_
+          FROM (SELECT (NOT TRUE OR FALSE) AS logic_)
+          WHERE logic_ IS NOT NULL)"""),
+      ),
+      dict(
           testcase_name='_withBooleanRelationBetweenStringInteger',
           fhir_path_expression="3 and 'true'",
           expected_sql_expression=textwrap.dedent("""\
           ARRAY(SELECT logic_
           FROM (SELECT ((3 IS NOT NULL) AND ('true' IS NOT NULL)) AS logic_)
           WHERE logic_ IS NOT NULL)"""),
       ),
@@ -732,15 +751,17 @@
       actual_sql_expression = self.fhir_path_encoder.encode(
           structure_definition=self.foo,
           element_definition=self.foo_root,
           fhir_path_expression=fhir_path_expression,
       )
       self.assertEqual(actual_sql_expression, expected_sql_expression)
     self.assertEvaluationNodeSqlCorrect(
-        self.foo, fhir_path_expression, expected_sql_expression
+        'Foo',
+        fhir_path_expression,
+        expected_sql_expression,
     )
 
   # TODO(b/191895721): Verify order-dependence of equivalence vs. equality
   @parameterized.named_parameters(
       dict(
           testcase_name='_withIntegerEqual',
           fhir_path_expression='3 = 4',
@@ -757,23 +778,25 @@
           FROM (SELECT (3 = 4) AS eq_)
           WHERE eq_ IS NOT NULL)"""),
       ),
       dict(
           testcase_name='_withDateTimeEqual',
           fhir_path_expression='@2015-02-04T14:34:28 = @2015-02-04T14',
           different_from_v2=True,
+          check_elm_nodes=False,
           expected_sql_expression=textwrap.dedent("""\
           ARRAY(SELECT eq_
           FROM (SELECT ('2015-02-04T14:34:28' = '2015-02-04T14') AS eq_)
           WHERE eq_ IS NOT NULL)"""),
       ),
       dict(
           testcase_name='_withDateTimeEquivalent',
           fhir_path_expression='@2015-02-04T14:34:28 ~ @2015-02-04T14',
           different_from_v2=True,
+          check_elm_nodes=False,
           expected_sql_expression=textwrap.dedent("""\
           ARRAY(SELECT eq_
           FROM (SELECT ('2015-02-04T14:34:28' = '2015-02-04T14') AS eq_)
           WHERE eq_ IS NOT NULL)"""),
       ),
       dict(
           testcase_name='_withIntegerNotEqualTo',
@@ -793,24 +816,28 @@
       ),
   )
   def testEncode_withFhirPathLiteralEqualityRelation_succeeds(
       self,
       fhir_path_expression: str,
       expected_sql_expression: str,
       different_from_v2: bool = True,
+      check_elm_nodes: bool = True,
   ):
     actual_sql_expression = self.fhir_path_encoder.encode(
         structure_definition=self.foo,
         element_definition=self.foo_root,
         fhir_path_expression=fhir_path_expression,
     )
     self.assertEqual(actual_sql_expression, expected_sql_expression)
     if not different_from_v2:
       self.assertEvaluationNodeSqlCorrect(
-          None, fhir_path_expression, expected_sql_expression
+          'Foo',
+          fhir_path_expression,
+          expected_sql_expression,
+          check_elm_nodes=check_elm_nodes,
       )
 
   @parameterized.named_parameters(
       dict(
           testcase_name='_withEquals_andIdentifierAndStringLiteral',
           fhir_path_expression="text = ''",
           expected_sql_expression=textwrap.dedent("""\
@@ -864,24 +891,28 @@
           expected_sql_expression=textwrap.dedent("""\
           ARRAY(SELECT eq_
           FROM (SELECT ((text IS NULL) = TRUE) AS eq_)
           WHERE eq_ IS NOT NULL)"""),
       ),
   )
   def testEncode_withFhirPathEqualityRelation_succeeds(
-      self, fhir_path_expression: str, expected_sql_expression: str
+      self,
+      fhir_path_expression: str,
+      expected_sql_expression: str,
   ):
     actual_sql_expression = self.fhir_path_encoder.encode(
         structure_definition=self.div,
         element_definition=self.div_root,
         fhir_path_expression=fhir_path_expression,
     )
     self.assertEqual(actual_sql_expression, expected_sql_expression)
     self.assertEvaluationNodeSqlCorrect(
-        self.div, fhir_path_expression, expected_sql_expression
+        'Div',
+        fhir_path_expression,
+        expected_sql_expression,
     )
 
   @parameterized.named_parameters(
       dict(
           testcase_name='_withIntegerIn',
           fhir_path_expression='3 in 4',
           expected_sql_expression=textwrap.dedent("""\
@@ -906,15 +937,15 @@
     actual_sql_expression = self.fhir_path_encoder.encode(
         structure_definition=self.foo,
         element_definition=self.foo_root,
         fhir_path_expression=fhir_path_expression,
     )
     self.assertEqual(actual_sql_expression, expected_sql_expression)
     self.assertEvaluationNodeSqlCorrect(
-        None, fhir_path_expression, expected_sql_expression
+        'Foo', fhir_path_expression, expected_sql_expression
     )
 
   @parameterized.named_parameters(
       dict(
           testcase_name='_withIntegerUnion',
           fhir_path_expression='3 | 4',
           expected_sql_expression=textwrap.dedent("""\
@@ -961,15 +992,15 @@
     actual_sql_expression = self.fhir_path_encoder.encode(
         structure_definition=self.foo,
         element_definition=self.foo_root,
         fhir_path_expression=fhir_path_expression,
     )
     self.assertEqual(actual_sql_expression, expected_sql_expression)
     self.assertEvaluationNodeSqlCorrect(
-        self.foo, fhir_path_expression, expected_sql_expression
+        'Foo', fhir_path_expression, expected_sql_expression
     )
 
   @parameterized.named_parameters(
       dict(
           testcase_name='_withIntegerPositivePolarity',
           fhir_path_expression='+5',
           expected_sql_expression=textwrap.dedent("""\
@@ -1056,15 +1087,15 @@
     actual_sql_expression = self.fhir_path_encoder.encode(
         structure_definition=self.foo,
         element_definition=self.foo_root,
         fhir_path_expression=fhir_path_expression,
     )
     self.assertEqual(actual_sql_expression, expected_sql_expression)
     self.assertEvaluationNodeSqlCorrect(
-        None, fhir_path_expression, expected_sql_expression
+        'Foo', fhir_path_expression, expected_sql_expression
     )
 
   @parameterized.named_parameters(
       dict(
           testcase_name='_withIntegerIndexer',
           fhir_path_expression='7[0]',
           expected_sql_expression=textwrap.dedent("""\
@@ -1107,15 +1138,43 @@
     actual_sql_expression = self.fhir_path_encoder.encode(
         structure_definition=self.foo,
         element_definition=self.foo_root,
         fhir_path_expression=fhir_path_expression,
     )
     self.assertEqual(actual_sql_expression, expected_sql_expression)
     self.assertEvaluationNodeSqlCorrect(
-        self.foo, fhir_path_expression, expected_sql_expression
+        'Foo', fhir_path_expression, expected_sql_expression
+    )
+
+  @parameterized.named_parameters(
+      dict(
+          testcase_name='_indexField',
+          fhir_path_expression='codeFlavors[0]',
+          expected_sql_expression=textwrap.dedent("""\
+          ARRAY(SELECT indexed_codeFlavors_element_
+          FROM (SELECT codeFlavors_element_ AS indexed_codeFlavors_element_
+          FROM (SELECT ROW_NUMBER() OVER() AS row_,
+          codeFlavors_element_
+          FROM (SELECT codeFlavors_element_
+          FROM UNNEST(codeFlavors) AS codeFlavors_element_ WITH OFFSET AS element_offset)) AS inner_tbl
+          WHERE (inner_tbl.row_ - 1) = 0)
+          WHERE indexed_codeFlavors_element_ IS NOT NULL)"""),
+      ),
+  )
+  def testEncode_withFhirPathIndexField_succeeds(
+      self, fhir_path_expression: str, expected_sql_expression: str
+  ):
+    actual_sql_expression = self.fhir_path_encoder.encode(
+        structure_definition=self.foo,
+        element_definition=self.foo_root,
+        fhir_path_expression=fhir_path_expression,
+    )
+    self.assertEqual(actual_sql_expression, expected_sql_expression)
+    self.assertEvaluationNodeSqlCorrect(
+        'Foo', fhir_path_expression, expected_sql_expression
     )
 
   @parameterized.named_parameters(
       dict(testcase_name='_withExists', fhir_path_expression='exists()'),
       dict(testcase_name='_withNot', fhir_path_expression='not()'),
       dict(testcase_name='_withEmpty', fhir_path_expression='empty()'),
       dict(testcase_name='_withCount', fhir_path_expression='count()'),
@@ -1134,15 +1193,15 @@
     with self.assertRaises(ValueError):
       self.fhir_path_encoder.encode(
           structure_definition=self.foo,
           element_definition=self.foo_root,
           fhir_path_expression=fhir_path_expression,
       )
 
-    builder = self.create_builder_from_str(self.foo, fhir_path_expression)
+    builder = self.create_builder_from_str('Foo', fhir_path_expression)
     with self.assertRaises(ValueError):
       _bigquery_interpreter.BigQuerySqlInterpreter().encode(builder)
 
   @parameterized.named_parameters(
       dict(
           testcase_name='_withNot',
           fhir_path_expression="(' ' contains 'history').not()",
@@ -1160,31 +1219,31 @@
     actual_sql_expression = self.fhir_path_encoder.encode(
         structure_definition=self.foo,
         element_definition=self.foo_root,
         fhir_path_expression=fhir_path_expression,
     )
     self.assertEqual(actual_sql_expression, expected_sql_expression)
     self.assertEvaluationNodeSqlCorrect(
-        self.foo, fhir_path_expression, expected_sql_expression
+        'Foo', fhir_path_expression, expected_sql_expression
     )
 
   @parameterized.named_parameters(
       dict(
-          testcase_name='_withCollectionsANdScalarsAsArrayTrue',
+          testcase_name='_withCollectionsAndScalarsAsArrayTrue',
           fhir_path_expression='bar.bats',
           select_scalars_as_array=True,
           expected_sql_expression=textwrap.dedent("""\
           ARRAY(SELECT bats_element_
           FROM (SELECT bats_element_
           FROM (SELECT bar),
           UNNEST(bar.bats) AS bats_element_ WITH OFFSET AS element_offset)
           WHERE bats_element_ IS NOT NULL)"""),
       ),
       dict(
-          testcase_name='_withCollectionsANdScalarsAsArrayFalse',
+          testcase_name='_withCollectionsAndScalarsAsArrayFalse',
           fhir_path_expression='bar.bats',
           select_scalars_as_array=False,
           expected_sql_expression=textwrap.dedent("""\
           ARRAY(SELECT bats_element_
           FROM (SELECT bats_element_
           FROM (SELECT bar),
           UNNEST(bar.bats) AS bats_element_ WITH OFFSET AS element_offset)
@@ -1219,14 +1278,33 @@
           testcase_name='_withScalarComparisonAndScalarsAsArrayFalse',
           fhir_path_expression="inline.value = 'abc'",
           select_scalars_as_array=False,
           expected_sql_expression=textwrap.dedent("""\
           (SELECT (inline.value = 'abc') AS eq_)"""),
       ),
       dict(
+          testcase_name='_withArrayEqualityAsArrayFalse',
+          fhir_path_expression='bar.bats.struct.value = stringList',
+          select_scalars_as_array=False,
+          expected_sql_expression=textwrap.dedent(
+              """\
+          (SELECT NOT EXISTS(
+          SELECT lhs_.*
+          FROM (SELECT ROW_NUMBER() OVER() AS row_, value
+          FROM (SELECT bats_element_.struct.value
+          FROM (SELECT bar),
+          UNNEST(bar.bats) AS bats_element_ WITH OFFSET AS element_offset)) AS lhs_
+          EXCEPT DISTINCT
+          SELECT rhs_.*
+          FROM (SELECT ROW_NUMBER() OVER() AS row_, stringList_element_
+          FROM (SELECT stringList_element_
+          FROM UNNEST(stringList) AS stringList_element_ WITH OFFSET AS element_offset)) AS rhs_) AS eq_)"""
+          ),
+      ),
+      dict(
           testcase_name='_withScalarComplexComparisonAndScalarsAsArrayFalse',
           fhir_path_expression="bar.bats.struct.value = ('abc' | '123')",
           select_scalars_as_array=False,
           expected_sql_expression=textwrap.dedent("""\
           (SELECT NOT EXISTS(
           SELECT lhs_.*
           FROM (SELECT ROW_NUMBER() OVER() AS row_, value
@@ -1258,15 +1336,18 @@
         structure_definition=self.foo,
         element_definition=self.foo_root,
         fhir_path_expression=fhir_path_expression,
         **kwargs,
     )
     self.assertEqual(actual_sql_expression, expected_sql_expression)
     self.assertEvaluationNodeSqlCorrect(
-        self.foo, fhir_path_expression, expected_sql_expression, **kwargs
+        'Foo',
+        fhir_path_expression,
+        expected_sql_expression,
+        **kwargs,
     )
 
   @parameterized.named_parameters(
       dict(
           testcase_name='_withChoiceNoType',
           fhir_path_expression='choiceExample',
           # Return full choice structure if no sub-type is specified.
@@ -1359,14 +1440,29 @@
           (SELECT EXISTS(
           SELECT ofType_
           FROM (SELECT multipleChoiceExample_element_.CodeableConcept AS ofType_
           FROM UNNEST(multipleChoiceExample) AS multipleChoiceExample_element_ WITH OFFSET AS element_offset)
           WHERE ofType_ IS NOT NULL) AS exists_)"""),
       ),
       dict(
+          testcase_name='_ArrayMatchesAll',
+          fhir_path_expression="inline.numbers.all($this.matches('regex'))",
+          select_scalars_as_array=False,
+          expected_sql_expression=textwrap.dedent(
+              """\
+              (SELECT IFNULL(
+              LOGICAL_AND(
+              IFNULL(
+              (SELECT REGEXP_CONTAINS(
+              numbers_element_, 'regex') AS all_), FALSE)), TRUE) AS all_
+              FROM (SELECT inline),
+              UNNEST(inline.numbers) AS numbers_element_ WITH OFFSET AS element_offset)"""
+          ),
+      ),
+      dict(
           testcase_name='_ArrayWithMessageChoice_andIdentifier',
           fhir_path_expression=(
               "multipleChoiceExample.ofType('CodeableConcept').coding.system"
           ),
           select_scalars_as_array=False,
           only_works_in_v2=True,
           expected_sql_expression=textwrap.dedent("""\
@@ -1462,15 +1558,15 @@
         fhir_path_expression=fhir_path_expression,
         **kwargs,
     )
 
     if not only_works_in_v2:
       self.assertEqual(actual_sql_expression, expected_sql_expression)
     self.assertEvaluationNodeSqlCorrect(
-        self.foo, fhir_path_expression, expected_sql_expression, **kwargs
+        'Foo', fhir_path_expression, expected_sql_expression, **kwargs
     )
 
   @parameterized.named_parameters(
       dict(
           testcase_name='_withStringField_generatesCastSql',
           fhir_path_expression='bat.struct.value.toInteger()',
           expected_sql_expression=textwrap.dedent("""\
@@ -1507,27 +1603,27 @@
         structure_definition=self.foo,
         element_definition=self.foo_root,
         fhir_path_expression=fhir_path_expression,
     )
 
     self.assertEqual(actual_sql_expression, expected_sql_expression)
     self.assertEvaluationNodeSqlCorrect(
-        self.foo, fhir_path_expression, expected_sql_expression
+        'Foo', fhir_path_expression, expected_sql_expression
     )
 
   def testEncode_ToIntegerValidation_withParamsProvided_raisesError(self):
     with self.assertRaises(ValueError):
       self.fhir_path_encoder.encode(
           structure_definition=self.foo,
           element_definition=self.foo_root,
           fhir_path_expression='bat.struct.value.toInteger(123)',
       )
 
     with self.assertRaises(ValueError):
-      self.create_builder_from_str(self.foo, 'bat.struct.value.toInteger(123)')
+      self.create_builder_from_str('Foo', 'bat.struct.value.toInteger(123)')
 
   @parameterized.named_parameters(
       dict(
           testcase_name='_withNot',
           fhir_path_expression="' '.contains('history').not()",
       )
   )
@@ -1539,15 +1635,15 @@
           structure_definition=self.foo,
           element_definition=self.foo_root,
           fhir_path_expression=fhir_path_expression,
       )
 
   def testEncode_withUnsupportedExistsParameter(self):
     builder = self.create_builder_from_str(
-        self.foo, 'bar.bats.struct.exists(true)'
+        'Foo', 'bar.bats.struct.exists(true)'
     )
     with self.assertRaisesRegex(ValueError, 'Unsupported FHIRPath expression'):
       _bigquery_interpreter.BigQuerySqlInterpreter().encode(
           builder, select_scalars_as_array=True
       )
 
   @parameterized.named_parameters(
@@ -1634,15 +1730,15 @@
           structure_definition=self.foo,
           element_definition=self.foo_root,
           fhir_path_expression=fhir_path_expression,
       )
       self.assertEqual(actual_sql_expression, expected_sql_expression)
 
     self.assertEvaluationNodeSqlCorrect(
-        self.foo, fhir_path_expression, expected_sql_expression
+        'Foo', fhir_path_expression, expected_sql_expression
     )
 
   @parameterized.named_parameters(
       dict(
           testcase_name='_withDeepestNestedMemberSqlKeywordExists',
           fhir_path_expression='bar.bats.struct.exists()',
           expected_sql_expression=textwrap.dedent("""\
@@ -2052,15 +2148,15 @@
     actual_sql_expression = fhir_path_encoder.encode(
         structure_definition=self.foo,
         element_definition=self.foo_root,
         fhir_path_expression=fhir_path_expression,
     )
     self.assertEqual(actual_sql_expression, expected_sql_expression)
     self.assertEvaluationNodeSqlCorrect(
-        self.foo,
+        'Foo',
         fhir_path_expression,
         expected_sql_expression,
         value_set_codes_table='VALUESET_VIEW',
     )
 
   @parameterized.named_parameters(
       dict(
@@ -2161,15 +2257,15 @@
         structure_definition=self.foo,
         element_definition=self.foo_root,
         fhir_path_expression=fhir_path_expression,
     )
     self.assertEqual(actual_sql_expression, expected_sql_expression)
 
     self.assertEvaluationNodeSqlCorrect(
-        self.foo,
+        'Foo',
         fhir_path_expression,
         expected_sql_expression,
         # Build a mock package manager which returns resources for the value
         # sets above.
         value_set_codes_definitions=unittest.mock.Mock(
             get_resource={
                 expanded_value_set_1.url.value: expanded_value_set_1,
@@ -2485,15 +2581,15 @@
         fhir_path_expression=fhir_path_expression,
     )
     self.assertEqual(actual_sql_expression, expected_sql_expression)
 
     if not different_in_v2:
       expected_sql_expression_v2 = expected_sql_expression
     self.assertEvaluationNodeSqlCorrect(
-        self.foo, fhir_path_expression, expected_sql_expression_v2
+        'Foo', fhir_path_expression, expected_sql_expression_v2
     )
 
   @parameterized.named_parameters(
       dict(
           testcase_name='_withSimpleIdentifier',
           fhir_path_expression='bar',
       ),
@@ -2534,14 +2630,18 @@
           fhir_path_expression='3 | bar.bats.struct',
       ),
       dict(
           testcase_name='_withInvalidEqualityBetweenStructs',
           fhir_path_expression='bar.bats = bar.bats.struct',
       ),
       dict(
+          testcase_name='_withMatchesFunctionAndRepeatedOperand',
+          fhir_path_expression="bar.bats.matches('[a-zA-Z0-9]*')",
+      ),
+      dict(
           testcase_name='_withInvalidEqualityBetweenStructLiteral',
           fhir_path_expression='bar.bats = 2',
       ),
       dict(
           testcase_name='_withInvalidEqualityBetweenLiteralStruct',
           fhir_path_expression='3 = bar.bats.struct',
       ),
@@ -2565,42 +2665,128 @@
       dict(
           testcase_name='_withSingleMemberAccessLeadingExpression',
           fhir_path_expression='(true or false).bar',
       ),
       dict(
           testcase_name='_withReferenceTypeLackingIdFor',
           fhir_path_expression='ref',
+          only_v1=True,
       ),
   )
   def testEncode_withUnsupportedFhirPathExpression_raisesTypeError(
-      self, fhir_path_expression: str
+      self, fhir_path_expression: str, only_v1: bool = False
   ):
     """Tests FHIRPath expressions that are unsupported for Standard SQL."""
     with self.assertRaises(TypeError) as te:
       _ = self.fhir_path_encoder.encode(
           structure_definition=self.foo,
           element_definition=self.foo_root,
           fhir_path_expression=fhir_path_expression,
       )
     self.assertIsInstance(te.exception, TypeError)
 
+    if only_v1:
+      return
+
+    # V2 test
+    with self.assertRaises(ValueError) as te:
+      builder = self.create_builder_from_str('Foo', fhir_path_expression)
+      _ = _bigquery_interpreter.BigQuerySqlInterpreter().encode(builder)
+    self.assertIsInstance(te.exception, ValueError)
+
+  @parameterized.named_parameters(
+      dict(
+          testcase_name='_withAllAndMatches',
+          invalid_fhir_path_expression="stringList.matches('regex')",
+          fhir_path_expression="stringList.all($this.matches('regex'))",
+          expected_sql_expression=textwrap.dedent("""\
+            ARRAY(SELECT all_
+            FROM (SELECT IFNULL(
+            LOGICAL_AND(
+            IFNULL(
+            (SELECT REGEXP_CONTAINS(
+            stringList_element_, 'regex') AS all_), FALSE)), TRUE) AS all_
+            FROM UNNEST(stringList) AS stringList_element_ WITH OFFSET AS element_offset)
+            WHERE all_ IS NOT NULL)"""),
+      ),
+      dict(
+          testcase_name='_withAllNestedArithmeticLogic',
+          invalid_fhir_path_expression='inline.numbers + 3 > 4',
+          fhir_path_expression='inline.numbers.all($this + 3 > 4)',
+          expected_sql_expression=textwrap.dedent("""\
+            ARRAY(SELECT all_
+            FROM (SELECT IFNULL(
+            LOGICAL_AND(
+            IFNULL(
+            (SELECT ((numbers_element_ + 3) > 4) AS all_), FALSE)), TRUE) AS all_
+            FROM (SELECT inline),
+            UNNEST(inline.numbers) AS numbers_element_ WITH OFFSET AS element_offset)
+            WHERE all_ IS NOT NULL)"""),
+      ),
+      dict(
+          testcase_name='_withWhereAndMemberOf',
+          invalid_fhir_path_expression=(
+              "codingList.memberOf('http://value.set/id'))"
+          ),
+          fhir_path_expression=(
+              "codingList.where($this.memberOf('http://value.set/id'))"
+          ),
+          expected_sql_expression=textwrap.dedent("""\
+            ARRAY(SELECT codingList_element_
+            FROM (SELECT codingList_element_
+            FROM UNNEST(codingList) AS codingList_element_ WITH OFFSET AS element_offset
+            WHERE (SELECT matches.element_offset IS NOT NULL AS memberof_
+            FROM (SELECT element_offset
+            FROM None) AS all_
+            LEFT JOIN (SELECT element_offset
+            FROM UNNEST(ARRAY(SELECT element_offset FROM (
+            SELECT element_offset
+            FROM None
+            INNER JOIN `VALUESET_VIEW` vs ON
+            vs.valueseturi='http://value.set/id'
+            AND vs.system=codingList_element_.system
+            AND vs.code=codingList_element_.code
+            ))) AS element_offset
+            ) AS matches
+            ON all_.element_offset=matches.element_offset
+            ORDER BY all_.element_offset))
+            WHERE codingList_element_ IS NOT NULL)"""),
+      ),
+  )
+  def testEncode_withArray_succeeds(
+      self,
+      invalid_fhir_path_expression: str,
+      fhir_path_expression: str,
+      expected_sql_expression: str,
+  ):
+    # V2 test
+    with self.assertRaises(ValueError) as te:
+      builder = self.create_builder_from_str(
+          'Foo', invalid_fhir_path_expression
+      )
+      _ = _bigquery_interpreter.BigQuerySqlInterpreter().encode(builder)
+    self.assertIsInstance(te.exception, ValueError)
+
+    self.assertEvaluationNodeSqlCorrect(
+        'Foo',
+        fhir_path_expression,
+        expected_sql_expression,
+        value_set_codes_table='VALUESET_VIEW',
+    )
+
   @parameterized.named_parameters(
       dict(
           testcase_name='_withWhereFunctionAndNoCriteria',
           fhir_path_expression='bat.struct.where()',
       ),
       dict(
           testcase_name='_withWhereFunctionAndNonBoolCriteria',
           fhir_path_expression='bat.struct.where(value)',
       ),
       dict(
-          testcase_name='_withMatchesFunctionAndRepeatedOperand',
-          fhir_path_expression="bar.bats.matches('*')",
-      ),
-      dict(
           testcase_name='_withAllFunctionAndNoCriteria',
           fhir_path_expression='bat.struct.all()',
       ),
       dict(
           testcase_name='_withMemberOfFunctionAndNoValueSet',
           fhir_path_expression='codeFlavor.code.memberOf()',
       ),
@@ -2627,14 +2813,19 @@
       _ = self.fhir_path_encoder.encode(
           structure_definition=self.foo,
           element_definition=self.foo_root,
           fhir_path_expression=fhir_path_expression,
       )
     self.assertIsInstance(te.exception, TypeError)
 
+    # V2 test
+    with self.assertRaises(ValueError) as te:
+      _ = self.create_builder_from_str('Foo', fhir_path_expression)
+    self.assertIsInstance(te.exception, ValueError)
+
   @parameterized.named_parameters(
       dict(
           testcase_name='_withUnknownValueSet',
           fhir_path_expression=(
               "codeFlavor.code.memberOf('http://value.set/id')"
           ),
           options=fhir_path_options.SqlValidationOptions(
@@ -2740,14 +2931,19 @@
       _ = self.fhir_path_encoder.encode(
           structure_definition=self.foo,
           element_definition=self.foo_root,
           fhir_path_expression=fhir_path_expression,
       )
     self.assertIsInstance(ve.exception, ValueError)
 
+    # V2 test
+    with self.assertRaises(ValueError) as te:
+      _ = self.create_builder_from_str('Foo', fhir_path_expression)
+    self.assertIsInstance(te.exception, ValueError)
+
   @parameterized.named_parameters(
       dict(
           testcase_name='_withInvalidInvocationInternalExpression',
           fhir_path_expression='foo.bar.exists().(2+3)',
       ),
       dict(
           testcase_name='_withInvalidInvocationNoIdentifier',
@@ -2765,26 +2961,31 @@
       _ = self.fhir_path_encoder.encode(
           structure_definition=self.foo,
           element_definition=self.foo_root,
           fhir_path_expression=fhir_path_expression,
       )
     self.assertIsInstance(ve.exception, ValueError)
 
+    # V2 test
+    with self.assertRaises(ValueError) as te:
+      _ = self.create_builder_from_str('Foo', fhir_path_expression)
+    self.assertIsInstance(te.exception, ValueError)
+
   @parameterized.named_parameters(
       dict(
           testcase_name='_withWhereFunctionAndNoCriteria',
           fhir_path_expression='bat.struct.where()',
       ),
       dict(
           testcase_name='_withWhereFunctionAndNonBoolCriteria',
           fhir_path_expression='bat.struct.where(value)',
       ),
       dict(
           testcase_name='_withMatchesFunctionAndRepeatedOperand',
-          fhir_path_expression="bar.bats.matches('*')",
+          fhir_path_expression="bar.bats.matches('regex')",
       ),
       dict(
           testcase_name='_withMemberOfFunctionAndNoValueSet',
           fhir_path_expression='codeFlavor.code.memberOf()',
       ),
       dict(
           testcase_name='_withMemberOfFunctionAndNonStringValueSet',
@@ -2849,27 +3050,37 @@
         id_='Foo', type_codes=None, cardinality=sdefs.Cardinality(0, '1')
     )
     soft_delete_slice = sdefs.build_element_definition(
         id_='Foo.bar:softDelete',
         path='Foo.bar',
         type_codes=['Bar'],
         cardinality=sdefs.Cardinality(0, '*'),
+        slice_name='softDelete',
     )
     resource = sdefs.build_resource_definition(
         id_='Foo', element_definitions=[root, soft_delete_slice]
     )
     fhir_path_encoder = fhir_path.FhirPathStandardSqlEncoder([resource])
     with self.assertRaises(ValueError) as ve:
       _ = fhir_path_encoder.encode(
           structure_definition=resource,
           element_definition=root,
           fhir_path_expression='bar.exists()',
       )
+
     self.assertIsInstance(ve.exception, ValueError)
 
+    # V2 test
+    mock_context = context_lib.MockFhirPathContext([resource])
+    with self.assertRaises(ValueError) as te:
+      _ = self.create_builder_from_str(
+          'Foo', 'bar.exists()', fhir_context=mock_context
+      )
+    self.assertIsInstance(te.exception, ValueError)
+
   def testEncode_withInlineProfiledElement_succeeds(self):
     """Creates a simple one-off resource graph with an inline profile.
 
     This ensures that, when "walking" a FHIR resource graph during FHIRPath
     Standard SQL encoding:
       (1) Check inline children for <curr_path>.<identifier>
       (2) Check children from the field's type for <type>.<identifier>
@@ -3502,26 +3713,167 @@
         cardinality=sdefs.Cardinality(0, '*'),
         constraints=[constraint],
     )
     foo = sdefs.build_resource_definition(
         id_='Foo', element_definitions=[foo_root, extension_slice]
     )
 
+    # Extension resource.
+    extension_root_element = sdefs.build_element_definition(
+        id_='Extension',
+        type_codes=None,
+        cardinality=sdefs.Cardinality(min=0, max='1'),
+    )
+    value_element_definition = sdefs.build_element_definition(
+        id_='Extension.value[x]',
+        type_codes=['string'],
+        cardinality=sdefs.Cardinality(min=1, max='1'),
+    )
+    extension = sdefs.build_resource_definition(
+        id_='Extension',
+        element_definitions=[
+            extension_root_element,
+            value_element_definition,
+        ],
+    )
+
     # Stand up encoder
     error_reporter = fhir_errors.ListErrorReporter()
     encoder = fhir_path_validator.FhirProfileStandardSqlEncoder(
         unittest.mock.Mock(iter_structure_definitions=lambda: [foo]),
         error_reporter,
     )
 
     actual_bindings = encoder.encode(foo)
     self.assertEmpty(error_reporter.warnings)
     self.assertEmpty(error_reporter.errors)
     self.assertLen(actual_bindings, 1)
 
+    # Stand up v2 encoder
+    error_reporter = fhir_errors.ListErrorReporter()
+    encoder = fhir_path_validator_v2.FhirProfileStandardSqlEncoder(
+        unittest.mock.Mock(iter_structure_definitions=lambda: [foo, extension]),
+        primitive_handler.PrimitiveHandler(),
+        error_reporter,
+    )
+
+    actual_bindings = encoder.encode(foo)
+    self.assertEmpty(error_reporter.warnings)
+    self.assertEmpty(error_reporter.errors)
+    self.assertLen(actual_bindings, 1)
+
+  def testSkipSlice_withSliceOnExtensionWithHyphen_andValidResource_isNotSkipped(
+      self,
+  ):
+    # Set up resource with a defined constraint
+    constraint = self.build_constraint(fhir_path_expression='false')
+    foo_root = sdefs.build_element_definition(
+        id_='Foo', type_codes=None, cardinality=sdefs.Cardinality(0, '1')
+    )
+    extension_slice = sdefs.build_element_definition(
+        id_='Foo.extension:softDelete-hyphen',
+        path='Foo.extension',
+        type_codes=['Extension'],
+        cardinality=sdefs.Cardinality(0, '*'),
+        constraints=[constraint],
+    )
+    foo = sdefs.build_resource_definition(
+        id_='Foo', element_definitions=[foo_root, extension_slice]
+    )
+
+    # Extension resource.
+    extension_root_element = sdefs.build_element_definition(
+        id_='Extension',
+        type_codes=None,
+        cardinality=sdefs.Cardinality(min=0, max='1'),
+    )
+    value_element_definition = sdefs.build_element_definition(
+        id_='Extension.value[x]',
+        type_codes=['string'],
+        cardinality=sdefs.Cardinality(min=1, max='1'),
+    )
+    extension = sdefs.build_resource_definition(
+        id_='Extension',
+        element_definitions=[
+            extension_root_element,
+            value_element_definition,
+        ],
+    )
+
+    # Stand up v2 encoder
+    error_reporter = fhir_errors.ListErrorReporter()
+    encoder = fhir_path_validator_v2.FhirProfileStandardSqlEncoder(
+        unittest.mock.Mock(iter_structure_definitions=lambda: [foo, extension]),
+        primitive_handler.PrimitiveHandler(),
+        error_reporter,
+    )
+
+    actual_bindings = encoder.encode(foo)
+    self.assertEmpty(error_reporter.warnings)
+    self.assertEmpty(error_reporter.errors)
+    self.assertLen(actual_bindings, 1)
+    self.assertEqual(
+        actual_bindings[0].column_name, 'foo_softdelete_hyphen_key_1'
+    )
+
+  def testSkipExtensionUrlField(self):
+    # Set up resource with a defined constraint
+    constraint = self.build_constraint(fhir_path_expression='false')
+    foo_root = sdefs.build_element_definition(
+        id_='Foo', type_codes=None, cardinality=sdefs.Cardinality(0, '1')
+    )
+    extension_slice = sdefs.build_element_definition(
+        id_='Foo.extension:url',
+        path='Foo.extension',
+        type_codes=['Extension'],
+        cardinality=sdefs.Cardinality(0, '*'),
+        constraints=[constraint],
+    )
+    foo = sdefs.build_resource_definition(
+        id_='Foo', element_definitions=[foo_root, extension_slice]
+    )
+
+    # Extension resource.
+    extension_root_element = sdefs.build_element_definition(
+        id_='Extension',
+        type_codes=None,
+        cardinality=sdefs.Cardinality(min=0, max='1'),
+    )
+    url_element_definition = sdefs.build_element_definition(
+        id_='Extension.url',
+        type_codes=['string'],
+        cardinality=sdefs.Cardinality(min=1, max='1'),
+    )
+    value_element_definition = sdefs.build_element_definition(
+        id_='Extension.value[x]',
+        type_codes=['string'],
+        cardinality=sdefs.Cardinality(min=1, max='1'),
+    )
+    extension = sdefs.build_resource_definition(
+        id_='Extension',
+        element_definitions=[
+            extension_root_element,
+            value_element_definition,
+            url_element_definition,
+        ],
+    )
+
+    # Stand up v2 encoder
+    error_reporter = fhir_errors.ListErrorReporter()
+    encoder = fhir_path_validator_v2.FhirProfileStandardSqlEncoder(
+        unittest.mock.Mock(iter_structure_definitions=lambda: [foo, extension]),
+        primitive_handler.PrimitiveHandler(),
+        error_reporter,
+    )
+
+    actual_bindings = encoder.encode(foo)
+    self.assertEmpty(error_reporter.warnings)
+    self.assertEmpty(error_reporter.errors)
+    self.assertLen(actual_bindings, 1)
+
   def testChoiceType_thatIsAlso_sliceOnExtension_skipsRegexValidation(self):
     # Set up resource.
     foo_root = sdefs.build_element_definition(
         id_='Foo', type_codes=None, cardinality=sdefs.Cardinality(0, '1')
     )
     extension_slice = sdefs.build_element_definition(
         id_='Foo.extension:softDelete',
@@ -3588,14 +3940,49 @@
             'Validation Error: Foo; Element `Foo.softDelete` with type codes: '
             + "['string', 'int'], is a choice type which is not currently "
             + 'supported.'
         ],
     )
     self.assertEmpty(actual_bindings)
 
+    error_reporter = fhir_errors.ListErrorReporter()
+    encoder = fhir_path_validator_v2.FhirProfileStandardSqlEncoder(
+        unittest.mock.Mock(
+            iter_structure_definitions=lambda: [  # pylint: disable=g-long-lambda
+                foo,
+                custom_extension,
+                string_struct,
+            ]
+        ),
+        primitive_handler.PrimitiveHandler(),
+        error_reporter,
+        options=fhir_path_validator_v2.SqlGenerationOptions(
+            add_primitive_regexes=True
+        ),
+    )
+
+    actual_bindings = encoder.encode(foo)
+    self.assertEmpty(error_reporter.warnings)
+    self.assertEqual(
+        error_reporter.errors,
+        [
+            # Adding `+` to get rid of `implicit-str-concat` inside list
+            # warning.
+            'FHIR Path Error: Foo.softDelete; softDelete; Element '
+            + '`softDelete` is a choice type which is not currently supported.'
+        ],
+    )
+    # Check that the only binding is over the choice type.
+    self.assertLen(actual_bindings, 1)
+    self.assertEqual(
+        actual_bindings[0].fhir_path_expression,
+        "softDelete.ofType('string').exists().toInteger() + "
+        "softDelete.ofType('int').exists().toInteger() <= 1",
+    )
+
   def testNonChoiceType_thatIsAlso_sliceOnExtension_makesRegexValidation(self):
     # Set up resource.
     foo_root = sdefs.build_element_definition(
         id_='Foo', type_codes=None, cardinality=sdefs.Cardinality(0, '1')
     )
     extension_slice = sdefs.build_element_definition(
         id_='Foo.extension:softDelete',
@@ -3823,30 +4210,36 @@
 
     # Ensure that we only produce a single Standard SQL requirement, and that
     # an error is logged since we were given a duplicate constraint.
     actual_bindings = encoder.encode(foo)
     self.assertEmpty(error_reporter.warnings)
     self.assertEmpty(error_reporter.errors)
     self.assertLen(actual_bindings, 2)
-    self.assertEqual(actual_bindings[0].fhir_path_expression, '4 + 5')
+    self.assertCountEqual(
+        [binding.fhir_path_expression for binding in actual_bindings],
+        ['2 + 3', '4 + 5'],
+    )
 
     # Test with v2
     encoder = fhir_path_validator_v2.FhirProfileStandardSqlEncoder(
         unittest.mock.Mock(iter_structure_definitions=lambda: [foo]),
         primitive_handler.PrimitiveHandler(),
         error_reporter,
         options=cast(fhir_path_validator_v2.SqlGenerationOptions, options),
     )
 
     actual_bindings = encoder.encode(foo)
     self.assertEmpty(error_reporter.warnings)
     self.assertEmpty(error_reporter.errors)
     self.assertLen(actual_bindings, 2)
 
-    self.assertEqual(actual_bindings[0].fhir_path_expression, '4 + 5')
+    self.assertCountEqual(
+        [binding.fhir_path_expression for binding in actual_bindings],
+        ['2 + 3', '4 + 5'],
+    )
 
   def testEncode_withReplacement_andNoElementPath_replacesConstraint(self):
     first_constraint = self.build_constraint(
         fhir_path_expression='1 + 1', key='some-key'
     )
     second_constraint = self.build_constraint(
         fhir_path_expression='1 + 1', key='other-key'
@@ -4181,23 +4574,194 @@
         id_='RepeatedReferenceTest',
         element_definitions=[
             repeated_reference_test_root,
             repeated_reference_test_bar_element_definition,
         ],
     )
 
+    # Definitions needed for slices on codeable concept tests.
+    coding = sdefs.build_resource_definition(
+        id_='Coding',
+        element_definitions=[
+            sdefs.build_element_definition(
+                id_='Coding',
+                type_codes=None,
+                cardinality=sdefs.Cardinality(min=1, max='1'),
+            ),
+            sdefs.build_element_definition(
+                id_='Coding.system',
+                type_codes=['uri'],
+                cardinality=sdefs.Cardinality(min=0, max='1'),
+            ),
+            sdefs.build_element_definition(
+                id_='Coding.code',
+                type_codes=['code'],
+                cardinality=sdefs.Cardinality(min=0, max='1'),
+            ),
+            sdefs.build_element_definition(
+                id_='Coding.version',
+                type_codes=['string'],
+                cardinality=sdefs.Cardinality(min=0, max='1'),
+            ),
+        ],
+    )
+
+    codeable_concept = sdefs.build_resource_definition(
+        id_='CodeableConcept',
+        element_definitions=[
+            sdefs.build_element_definition(
+                id_='CodeableConcept',
+                type_codes=None,
+                cardinality=sdefs.Cardinality(min=1, max='1'),
+            ),
+            sdefs.build_element_definition(
+                id_='CodeableConcept.coding',
+                type_codes=['Coding'],
+                cardinality=sdefs.Cardinality(min=0, max='*'),
+            ),
+        ],
+    )
+
+    codeable_concept_slice_test = sdefs.build_resource_definition(
+        id_='CodeableConceptSliceTest',
+        element_definitions=[
+            sdefs.build_element_definition(
+                id_='CodeableConceptSliceTest',
+                type_codes=None,
+                cardinality=sdefs.Cardinality(min=1, max='1'),
+            ),
+            sdefs.build_element_definition(
+                id_='CodeableConceptSliceTest.code',
+                type_codes=['CodeableConcept'],
+                cardinality=sdefs.Cardinality(min=0, max='1'),
+            ),
+            # Define a required slice on code.coding named 'SolarSystem'
+            sdefs.build_element_definition(
+                id_='CodeableConceptSliceTest.code.coding:SolarSystem',
+                path='CodeableConceptSliceTest.code.coding',
+                type_codes=['Coding'],
+                cardinality=sdefs.Cardinality(min=1, max='1'),
+                slice_name='SolarSystem',
+            ),
+            # code can be anything.
+            sdefs.build_element_definition(
+                id_='CodeableConceptSliceTest.code.coding:SolarSystem.code',
+                path='CodeableConceptSliceTest.code.coding.code',
+                type_codes=['code'],
+                cardinality=sdefs.Cardinality(min=1, max='1'),
+            ),
+            # Fix a 'system' attribute on the slice.
+            sdefs.build_element_definition(
+                id_='CodeableConceptSliceTest.code.coding:SolarSystem.system',
+                path='CodeableConceptSliceTest.code.coding.system',
+                type_codes=['uri'],
+                cardinality=sdefs.Cardinality(min=1, max='1'),
+                fixed=datatypes_pb2.ElementDefinition.FixedX(
+                    uri=datatypes_pb2.Uri(value='milky_way')
+                ),
+            ),
+            # Fix a 'version' attribute on the slice.
+            sdefs.build_element_definition(
+                id_='CodeableConceptSliceTest.code.coding:SolarSystem.version',
+                path='CodeableConceptSliceTest.code.coding.version',
+                type_codes=['string'],
+                cardinality=sdefs.Cardinality(min=1, max='1'),
+                fixed=datatypes_pb2.ElementDefinition.FixedX(
+                    string_value=datatypes_pb2.String(value='final_frontier')
+                ),
+            ),
+            # Define another slice on code.coding named 'Whatever.'
+            # The slice has a min cardinality of 0, so it should not
+            # generate any constraints.
+            sdefs.build_element_definition(
+                id_='CodeableConceptSliceTest.code.coding:Whatever',
+                path='CodeableConceptSliceTest.code.coding',
+                type_codes=['Coding'],
+                cardinality=sdefs.Cardinality(min=0, max='*'),
+                slice_name='SolarSystem',
+            ),
+            # Fix a 'system' attribute on the slice, but it doesn't
+            # matter because the slice itself is not required.
+            sdefs.build_element_definition(
+                id_='CodeableConceptSliceTest.code.coding:Whatever.system',
+                path='CodeableConceptSliceTest.code.coding.system',
+                type_codes=['uri'],
+                cardinality=sdefs.Cardinality(min=1, max='1'),
+                fixed=datatypes_pb2.ElementDefinition.FixedX(
+                    uri=datatypes_pb2.Uri(value='whatever')
+                ),
+            ),
+        ],
+    )
+
+    backbone_resource = sdefs.build_resource_definition(
+        id_='BackboneElement',
+        element_definitions=[
+            sdefs.build_element_definition(
+                id_='BackboneElement',
+                type_codes=None,
+                cardinality=sdefs.Cardinality(min=0, max='1'),
+            )
+        ],
+    )
+
+    codeable_concept_backbone_slice_test = sdefs.build_resource_definition(
+        id_='CodeableConceptBackboneSliceTest',
+        element_definitions=[
+            sdefs.build_element_definition(
+                id_='CodeableConceptBackboneSliceTest',
+                type_codes=None,
+                cardinality=sdefs.Cardinality(min=1, max='1'),
+            ),
+            # Define a backbone element named 'contact.'
+            sdefs.build_element_definition(
+                id_='CodeableConceptBackboneSliceTest.contact',
+                type_codes=['BackboneElement'],
+                cardinality=sdefs.Cardinality(0, '*'),
+            ),
+            sdefs.build_element_definition(
+                id_='CodeableConceptBackboneSliceTest.contact.name',
+                type_codes=['string'],
+                cardinality=sdefs.Cardinality(0, '1'),
+            ),
+            # Define a slice off the collection of 'contact' backbone elements.
+            sdefs.build_element_definition(
+                id_='CodeableConceptBackboneSliceTest.contact:BackboneSlice',
+                path='CodeableConceptBackboneSliceTest.contact',
+                type_codes=['BackboneElement'],
+                cardinality=sdefs.Cardinality(2, '*'),
+                slice_name='BackboneSlice',
+            ),
+            # Fix the names in this slice.
+            sdefs.build_element_definition(
+                id_='CodeableConceptBackboneSliceTest.contact:BackboneSlice.name',
+                path='CodeableConceptBackboneSliceTest.contact.name',
+                type_codes=['string'],
+                cardinality=sdefs.Cardinality(1, '1'),
+                fixed=datatypes_pb2.ElementDefinition.FixedX(
+                    string_value=datatypes_pb2.String(value='skeleton')
+                ),
+            ),
+        ],
+    )
+
     all_resources = [
         choice_test,
         nested_choice_test,
         nest_choice,
         patient_datatype,
         device_datatype,
         reference_datatype,
         reference_test,
         repeated_reference_test,
+        coding,
+        codeable_concept,
+        codeable_concept_slice_test,
+        backbone_resource,
+        codeable_concept_backbone_slice_test,
     ]
     cls.resources = {resource.url.value: resource for resource in all_resources}
 
   @parameterized.named_parameters(
       dict(
           testcase_name='_withChoiceType_encodesChoiceTypeExclusivity',
           base_id='ChoiceTest',
@@ -4276,14 +4840,94 @@
               IFNULL(
               (SELECT ((CAST(
               bar_element_.deviceId IS NOT NULL AS INT64) + CAST(
               bar_element_.patientId IS NOT NULL AS INT64)) <= 1) AS all_), FALSE)), TRUE) AS all_
               FROM UNNEST(bar) AS bar_element_ WITH OFFSET AS element_offset)
               WHERE all_ IS NOT NULL)) AS result_)"""),
       ),
+      dict(
+          testcase_name='_withCodeableConceptSlice_encodesSystemRequirement',
+          base_id='CodeableConceptSliceTest',
+          context_element_path='CodeableConceptSliceTest',
+          fields_referenced_by_expression=[
+              'code.coding',
+              'code.coding.system',
+              'code.coding.version',
+          ],
+          fhir_path_expression=(
+              "code.coding.where(system = 'milky_way' and version ="
+              " 'final_frontier').exists() and code.coding.where(system ="
+              " 'milky_way' and version = 'final_frontier').count() <= 1"
+          ),
+          expected_sql_expression=textwrap.dedent("""\
+              (SELECT IFNULL(LOGICAL_AND(result_), TRUE)
+              FROM UNNEST(ARRAY(SELECT logic_
+              FROM (SELECT (EXISTS(
+              SELECT coding_element_
+              FROM (SELECT coding_element_
+              FROM (SELECT code),
+              UNNEST(code.coding) AS coding_element_ WITH OFFSET AS element_offset
+              WHERE (NOT EXISTS(
+              SELECT lhs_.*
+              FROM (SELECT ROW_NUMBER() OVER() AS row_, system
+              FROM (SELECT system)) AS lhs_
+              EXCEPT DISTINCT
+              SELECT rhs_.*
+              FROM (SELECT ROW_NUMBER() OVER() AS row_, literal_
+              FROM (SELECT 'milky_way' AS literal_)) AS rhs_) AND NOT EXISTS(
+              SELECT lhs_.*
+              FROM (SELECT ROW_NUMBER() OVER() AS row_, version
+              FROM (SELECT version)) AS lhs_
+              EXCEPT DISTINCT
+              SELECT rhs_.*
+              FROM (SELECT ROW_NUMBER() OVER() AS row_, literal_
+              FROM (SELECT 'final_frontier' AS literal_)) AS rhs_)))
+              WHERE coding_element_ IS NOT NULL) AND ((SELECT COUNT(
+              coding_element_) AS count_
+              FROM (SELECT code),
+              UNNEST(code.coding) AS coding_element_ WITH OFFSET AS element_offset
+              WHERE (NOT EXISTS(
+              SELECT lhs_.*
+              FROM (SELECT ROW_NUMBER() OVER() AS row_, system
+              FROM (SELECT system)) AS lhs_
+              EXCEPT DISTINCT
+              SELECT rhs_.*
+              FROM (SELECT ROW_NUMBER() OVER() AS row_, literal_
+              FROM (SELECT 'milky_way' AS literal_)) AS rhs_) AND NOT EXISTS(
+              SELECT lhs_.*
+              FROM (SELECT ROW_NUMBER() OVER() AS row_, version
+              FROM (SELECT version)) AS lhs_
+              EXCEPT DISTINCT
+              SELECT rhs_.*
+              FROM (SELECT ROW_NUMBER() OVER() AS row_, literal_
+              FROM (SELECT 'final_frontier' AS literal_)) AS rhs_))) <= 1)) AS logic_)
+              WHERE logic_ IS NOT NULL)) AS result_)"""),
+      ),
+      dict(
+          testcase_name=(
+              '_withCodeableConceptBackboneSlice_encodesSystemRequirement'
+          ),
+          base_id='CodeableConceptBackboneSliceTest',
+          context_element_path='CodeableConceptBackboneSliceTest.contact',
+          fields_referenced_by_expression=['contact', 'contact.name'],
+          fhir_path_expression="contact.where(name = 'skeleton').count() >= 2",
+          expected_sql_expression=textwrap.dedent("""\
+          (SELECT IFNULL(LOGICAL_AND(result_), TRUE)
+          FROM (SELECT ARRAY(SELECT comparison_
+          FROM (SELECT ((SELECT COUNT(
+          where_clause_) AS count_
+          FROM (SELECT NULL AS where_clause_)) >= 2) AS comparison_)
+          WHERE comparison_ IS NOT NULL) AS subquery_
+          FROM (SELECT AS VALUE ctx_element_
+          FROM UNNEST(ARRAY(SELECT contact_element_
+          FROM (SELECT contact_element_
+          FROM UNNEST(contact) AS contact_element_ WITH OFFSET AS element_offset)
+          WHERE contact_element_ IS NOT NULL)) AS ctx_element_)),
+          UNNEST(subquery_) AS result_)"""),
+      ),
   )
   def testEncode(
       self,
       base_id: str,
       context_element_path: str,
       expected_sql_expression: str,
       fhir_path_expression: str,
@@ -4292,14 +4936,17 @@
     """Ensures we enforce an exclusivity constraint among choice type options."""
     error_reporter_v2 = fhir_errors.ListErrorReporter()
     all_resources = list(self.resources.values())
     encoder_v2 = fhir_path_validator_v2.FhirProfileStandardSqlEncoder(
         unittest.mock.Mock(iter_structure_definitions=lambda: all_resources),
         primitive_handler.PrimitiveHandler(),
         error_reporter_v2,
+        options=fhir_path_validator_v2.SqlGenerationOptions(
+            verbose_error_reporting=True
+        ),
     )
 
     resource = self.resources[
         f'http://hl7.org/fhir/StructureDefinition/{base_id}'
     ]
 
     actual_bindings_v2 = encoder_v2.encode(resource)
@@ -4417,22 +5064,22 @@
 
     # We should have one constraint each from visiting
     # RiskAssessment.basedOn.identifier and
     # RiskAssessment.basedOn.identifier.assigner. We should have
     # stopped recursing before visiting
     # RiskAssessment.basedOn.identifier.assigner.identifier
     self.assertLen(actual_bindings, 2)
-    self.assertListEqual(
+    self.assertCountEqual(
         [binding.element_path for binding in actual_bindings],
         [
             'RiskAssessment.basedOn.identifier',
             'RiskAssessment.basedOn.identifier.assigner',
         ],
     )
-    self.assertListEqual(
+    self.assertCountEqual(
         [binding.fhir_path_key for binding in actual_bindings],
         ['from-reference', 'from-identifier'],
     )
 
 
 class FhirProfileStandardSqlEncoderTest(FhirProfileStandardSqlEncoderTestBase):
   """A suite of tests against resources with scalar and repeated fields.
```

## google/fhir/core/fhir_path/fhir_path_test_base.py

```diff
@@ -10,17 +10,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Module for encapsulating  synthetic resources for FHIRPath traversal."""
 
-from typing import List
+from typing import List, Optional
 
-from google.protobuf import message
 from google.fhir.r4.proto.core import codes_pb2
 from google.fhir.r4.proto.core import datatypes_pb2
 from google.fhir.r4.proto.core.resources import structure_definition_pb2
 from google.fhir.core.fhir_path import _fhir_path_data_types
 from google.fhir.core.fhir_path import _structure_definitions as sdefs
 from google.fhir.core.fhir_path import context as context_lib
 from google.fhir.core.fhir_path import expressions
@@ -45,14 +44,16 @@
       repeated int numbers;
     }
     InlineElement inline;
 
     CodeFlavor codeFlavor;
     repeated CodeFlavor codeFlavors;
     repeated bool boolList;
+    repeated string stringList;
+    repeated Coding codingList;
 
     ChoiceType choiceExample['string', 'integer', 'CodeableConcept']
     repeated ChoiceType multipleChoiceExample['string', 'integer',
       'CodeableConcept']
   }
   Bar {
     repeated Bats bats;
@@ -102,14 +103,25 @@
           sdefs.build_element_definition(
               id_='string',
               type_codes=None,
               cardinality=sdefs.Cardinality(min=0, max='1'),
           )
       ],
   )
+  # integer datatype
+  integer_datatype = sdefs.build_resource_definition(
+      id_='integer',
+      element_definitions=[
+          sdefs.build_element_definition(
+              id_='integer',
+              type_codes=None,
+              cardinality=sdefs.Cardinality(min=0, max='1'),
+          )
+      ],
+  )
   # reference datatype
   reference_datatype = sdefs.build_resource_definition(
       id_='Reference',
       element_definitions=[
           sdefs.build_element_definition(
               id_='Reference',
               type_codes=None,
@@ -227,14 +239,24 @@
       cardinality=sdefs.Cardinality(min=0, max='*'),
   )
   bool_list_definition = sdefs.build_element_definition(
       id_='Foo.boolList',
       type_codes=['boolean'],
       cardinality=sdefs.Cardinality(min=0, max='*'),
   )
+  string_list_definition = sdefs.build_element_definition(
+      id_='Foo.stringList',
+      type_codes=['string'],
+      cardinality=sdefs.Cardinality(min=0, max='*'),
+  )
+  coding_list_definition = sdefs.build_element_definition(
+      id_='Foo.codingList',
+      type_codes=['Coding'],
+      cardinality=sdefs.Cardinality(min=0, max='*'),
+  )
   foo = sdefs.build_resource_definition(
       id_='Foo',
       element_definitions=[
           foo_root_element_definition,
           bar_element_definition,
           bat_element_definition,
           reference_element_definition,
@@ -243,14 +265,16 @@
           inline_numbers_element_definition,
           choice_value_element_definition,
           multiple_choice_value_element_definition,
           date_value_element_definition,
           code_flavor_element_definition,
           code_flavors_element_definition,
           bool_list_definition,
+          string_list_definition,
+          coding_list_definition,
       ],
   )
 
   # Bar resource
   bar_root_element_definition = sdefs.build_element_definition(
       id_='Bar', type_codes=None, cardinality=sdefs.Cardinality(min=0, max='1')
   )
@@ -432,14 +456,15 @@
           codeable_concept_root_element_definition,
           codeable_concept_coding_system_element_definition,
       ],
   )
 
   # Set resources for test
   resources = [
+      integer_datatype,
       string_datatype,
       reference_datatype,
       patient_datatype,
       device_datatype,
       observation_datatype,
       foo,
       bar,
@@ -459,23 +484,46 @@
   struct_element_def = struct_element_definition
   fhir_path_encoder = fhir_path.FhirPathStandardSqlEncoder(resources)
 
   div = div
   div_root = div_root_element_definition
 
   def create_builder_from_str(
-      self, structdef: message.Message, fhir_path_expression: str
+      self,
+      structdef_name: str,
+      fhir_path_expression: str,
+      fhir_context: Optional[context_lib.FhirPathContext] = None,
   ) -> expressions.Builder:
+    """Creates an expression Builder from a FHIRPath string.
+
+    Args:
+      structdef_name: Name of the resource for the fhir_path_expression.
+        Structure Definition is fetched from the fhir_context.
+      fhir_path_expression: A FHIR path string to parse.
+      fhir_context: An optional context to use. If not specified, will use
+        self.context by default.
+
+    Returns:
+      An equivalent expressions.Builder to the fhir_path_expression.
+    """
     structdef_type = None
-    if structdef:
-      structdef_type = _fhir_path_data_types.StructureDataType(structdef)
+    if not fhir_context:
+      fhir_context = self.context
+
+    structdef = fhir_context.get_structure_definition(structdef_name)
+    if not structdef:
+      raise ValueError(
+          f'Structdef {structdef_name} was not found in the provided context.'
+      )
+
+    structdef_type = _fhir_path_data_types.StructureDataType(structdef)
 
     return expressions.from_fhir_path_expression(
         fhir_path_expression,
-        self.context,
+        fhir_context,
         structdef_type,
         primitive_handler.PrimitiveHandler(),
     )
 
   @classmethod
   def build_constraint(
       cls,
```

## google/fhir/core/fhir_path/fhir_path_validator_v2.py

```diff
@@ -14,16 +14,17 @@
 # limitations under the License.
 """Functionality for validating FHIRPath resources using SQL."""
 
 import dataclasses
 import functools
 import itertools
 import operator
+import re
 import traceback
-from typing import Any, Collection, Iterable, List, Optional, Set, cast, Dict
+from typing import Any, Collection, Iterable, List, Optional, Set, Tuple, cast, Dict
 
 from google.cloud import bigquery
 
 from google.protobuf import message
 from google.fhir.core.proto import fhirpath_replacement_list_pb2
 from google.fhir.core.proto import validation_pb2
 from google.fhir.core import codes
@@ -173,17 +174,20 @@
   """
   if isinstance(builder.get_node(), _evaluation.RootMessageNode):
     return ''
   # The last node will be the last path token.
   return builder.get_node().to_path_token()
 
 
+_BAD_SQL_CHARACTERS = re.compile(r'(-|\.|:)')
+
+
 def _path_to_sql_column_name(path: str) -> str:
   """Given a path to an `ElementDefinition`, returns a SQL column name."""
-  return path.lower().replace('.', '_')
+  return _BAD_SQL_CHARACTERS.sub('_', path.lower())
 
 
 def _key_to_sql_column_name(key: str) -> str:
   """Given a constraint key, returns a SQL column name."""
   return key.lower().replace('-', '_')
 
 
@@ -344,27 +348,36 @@
 
     self._ctx: List[expressions.Builder] = []
     self._in_progress: Set[_PathStep] = set()
     self._element_id_to_regex_map: Dict[str, _RegexInfo] = {}
     self._regex_columns_generated = set()
     # Used to track duplicate requirements.
     self._requirement_column_names: Set[str] = set()
+    # Used to avoid visiting the same element definitions multiple times.
+    self._visited_element_definitions: Set[Tuple[str, str]] = set()
+    # Likewise for slices.
+    self._visited_slices: Set[Tuple[str, str]] = set()
 
   def _get_new_child_builder(
-      self, builder: expressions.Builder, name: str
+      self, builder: expressions.Builder, path: str
   ) -> Optional[expressions.Builder]:
-    try:
-      return builder.__getattr__(name)
-    except (AttributeError, ValueError) as e:
-      self._error_reporter.report_fhir_path_error(
-          self._abs_path_invocation(builder),
-          f'{builder}.{name}',
-          str(e),
-      )
-    return None
+    """Creates a new builder by following `path` from `builder`."""
+    child_builder = builder
+    for path_element in path.split('.'):
+      try:
+        child_builder = child_builder.__getattr__(path_element)
+      except (AttributeError, ValueError) as e:
+        self._error_reporter.report_fhir_path_error(
+            self._abs_path_invocation(builder),
+            f'{child_builder}.{path_element}',
+            str(e),
+        )
+        return None
+
+    return child_builder
 
   def _abs_path_invocation(self, builder: expressions.Builder) -> str:
     """Returns the absolute path invocation given the traversal context."""
     if not builder:
       return ''
 
     if not self._ctx:
@@ -676,30 +689,19 @@
     # If this is an extension, we don't want to access its children/fields.
     # TODO(b/200575760): Add support for complex extensions and the fields
     # inside them.
     if builder.return_type.element_type == 'Extension':
       return []
 
     encoded_requirements: List[validation_pb2.SqlRequirement] = []
-    children = builder.return_type.children()
-    for name, child_message in children.items():
-      child_builder = self._get_new_child_builder(builder, name)
-      if not child_builder:
-        continue
-
-      requirement = self._encode_required_field(
-          name, builder, child_builder, child_message
-      )
-      if requirement:
-        encoded_requirements.append(requirement)
 
-    # Sometimes a struct_def can specify requirements for their descendants.
-    # Encode them as a part of its children.
-    required_descendants = builder.return_type.required_descendants
-    for name, desc_message in required_descendants.items():
+    # Sometimes a struct_def can specify requirements for their
+    # descendants, so we look through all descendant element
+    # definitions, not just the direct children.
+    for name, desc_message in builder.return_type.iter_all_descendants():
       containing_type_builder = builder
       child_builder = containing_type_builder
       paths = name.split('.')
       for path in paths:
         if isinstance(
             child_builder.return_type,
             _fhir_path_data_types.StructureDataType,
@@ -878,14 +880,172 @@
             fhir_path_expression=result.builder.fhir_path,
             fields_referenced_by_expression=_fields_referenced_by_expression(
                 result.builder.fhir_path
             ),
         )
     ]
 
+  def _encode_slice_definition(
+      self,
+      root_builder: expressions.Builder,
+      slice_: _fhir_path_data_types.Slice,
+  ) -> List[validation_pb2.SqlRequirement]:
+    """Encodes constraints for slices.
+
+    Args:
+      root_builder: The builder representing a path to the structure definition
+        defining the slice.
+      slice_: A slice defined by the structure definition at `root_builder`.
+
+    Returns:
+      A constraint enforcing the cardinality of `slice_` if `slice_` imposes a
+      non-zero or non-* min or max cardinality. Otherwise, an empty list.
+    """
+    if slice_.relative_path:
+      slice_builder = self._get_new_child_builder(
+          root_builder, slice_.relative_path
+      )
+    else:
+      slice_builder = root_builder
+
+    if slice_builder is None:
+      return []
+
+    # Find any fixed values set by the slice's element definitions.
+    element_constraints = []
+    for rule_path, rule_def in slice_.slice_rules:
+      constraint = self._constraint_from_slice_element(
+          root_builder, rule_path, rule_def
+      )
+      if constraint is not None:
+        element_constraints.append(constraint)
+
+    # If the slice has no fixed values, there's no constraint to build.
+    if not element_constraints:
+      return []
+
+    # 'and' together each of the fixed value constraints.
+    element_predicate = functools.reduce(operator.and_, element_constraints)
+    elements_in_slice = slice_builder.where(element_predicate)
+
+    # Ensure the number of elements in the slice is between min and max.
+    slice_constraints = []
+
+    min_size = cast(Any, slice_.slice_def).min.value
+    if min_size == 1:
+      slice_constraints.append(elements_in_slice.exists())
+    elif min_size > 1:
+      slice_constraints.append(elements_in_slice.count() >= min_size)
+
+    # max_size may be '*' or the string representation of an integer.
+    max_size = cast(Any, slice_.slice_def).max.value
+    if max_size.isdigit():
+      slice_constraints.append(elements_in_slice.count() <= int(max_size))
+
+    # If neither min nor max size are set, there's no constraint to build.
+    if not slice_constraints:
+      return []
+
+    # 'and' together the min and max size constraints.
+    slice_constraint = functools.reduce(operator.and_, slice_constraints)
+    constraint_sql = self._encode_fhir_path_builder_constraint(
+        slice_constraint, root_builder
+    )
+    if constraint_sql is None:
+      return []
+
+    slice_id = cast(Any, slice_.slice_def).id.value
+    slice_path = self._abs_path_invocation(root_builder)
+    slice_name = cast(Any, slice_.slice_def).slice_name.value
+    column_name = (
+        f'{_path_to_sql_column_name(slice_path)}'
+        f'_{_path_to_sql_column_name(slice_id)}'
+        '_slice_cardinality'
+    )
+    description = (
+        f'Slice {slice_id} requires at least {min_size} and at most'
+        f' {max_size} elements in {slice_builder} to conform to slice'
+        f' {slice_name}.'
+    )
+    return [
+        validation_pb2.SqlRequirement(
+            column_name=column_name,
+            sql_expression=constraint_sql.sql,
+            severity=validation_pb2.ValidationSeverity.SEVERITY_ERROR,
+            type=validation_pb2.ValidationType.VALIDATION_TYPE_CARDINALITY,
+            element_path=slice_path,
+            description=description,
+            fhir_path_key=column_name.replace('_', '-'),
+            fhir_path_expression=slice_constraint.fhir_path,
+            fields_referenced_by_expression=_fields_referenced_by_expression(
+                slice_constraint.fhir_path
+            ),
+        )
+    ]
+
+  def _constraint_from_slice_element(
+      self,
+      root_builder: expressions.Builder,
+      rule_path: str,
+      rule_def: ElementDefinition,
+  ) -> Optional[expressions.Builder]:
+    """Creates a constraint for the component slice element definition.
+
+    If the element definition contains a 'fixed' value, stating that members of
+    the slice must have a value for that field with a given value, returns an
+    expression stating that the element definition's field must be that fixed
+    value.
+
+    Args:
+      root_builder: The builder representing a path to the structure definition
+        defining the slice.
+      rule_path: The path to the element definition `rule_def` relative to
+        `root_builder`.
+      rule_def: An element definition representing one rule describing slice
+        membership.
+
+    Returns:
+      An expression stating the constraint or None if the `rule_def` does not
+      contain a constraint.
+    """
+    rule_def = cast(Any, rule_def)
+
+    # If the slice isn't fixing a value, there's no constraint to generate.
+    if not rule_def.HasField('fixed'):
+      return None
+
+    rule_builder = self._get_new_child_builder(root_builder, rule_path)
+    if rule_builder is None:
+      return None
+
+    type_codes = _utils.element_type_codes(rule_def)
+    if len(type_codes) > 1:
+      self._error_reporter.report_conversion_error(
+          self._abs_path_invocation(rule_builder),
+          f'Slice {rule_def.id.value} on choice type unsupported.',
+      )
+      return None
+
+    element_type = type_codes[0]
+    if not _fhir_path_data_types.is_type_code_primitive(element_type):
+      self._error_reporter.report_fhir_path_warning(
+          self._abs_path_invocation(rule_builder),
+          rule_def.id.value,
+          (
+              f'Slice fixing value of type {element_type} not yet supported.'
+              ' Only slices fixing primitive types are currently supported.'
+          ),
+      )
+      return None
+
+    fixed_field = _fhir_path_data_types.fixed_field_for_type_code(element_type)
+    fixed_value = getattr(rule_def.fixed, fixed_field).value
+    expression: expressions.Builder = rule_builder == fixed_value
+    return expression
+
   def _encode_reference_type_constraints(
       self, builder: expressions.Builder, elem: message.Message
   ) -> List[validation_pb2.SqlRequirement]:
     """Generates constraints for reference types.
 
     Ensures that a reference type only has a value for one of the resourceId
     columns across each of the possible resources the reference can link.
@@ -958,99 +1118,31 @@
             fhir_path_expression=constraint.fhir_path,
             fields_referenced_by_expression=_fields_referenced_by_expression(
                 constraint.fhir_path
             ),
         )
     ]
 
-  def get_type_codes_from_slice_element(
-      self, element_definition: ElementDefinition
-  ) -> List[str]:
-    """Returns the type codes of slice elements."""
-    element_definition_path = _get_analytic_path(element_definition)
-
-    # This function currently only supports getting type codes from slices on
-    # extensions.
-    if not _utils.is_slice_on_extension(element_definition):
-      self._error_reporter.report_conversion_error(
-          element_definition_path,
-          (
-              'Attempted to get type code from slice of non-extension.'
-              ' Which is not supported.'
-          ),
-      )
-      return []
-
-    urls = _utils.slice_element_urls(element_definition)
-    # TODO(b/190679571): Handle choice types.
-    if not urls:
-      raise ValueError(
-          'Unable to get url for slice on extension with id: '
-          f'{_get_analytic_path(element_definition)}'
-      )
-
-    if len(urls) > 1:
-      raise ValueError(
-          'Expected element with only one url but got: '
-          f'{urls}, is this a choice type?'
-      )
-
-    url = urls[0]
-    slice_struct_def = self._context.get_structure_definition(url)
-    if not slice_struct_def:
-      raise ValueError(f'Expected a structure definition for {url}.')
-    slice_builder = expressions.Builder(
-        _evaluation.RootMessageNode(
-            self._context,
-            _fhir_path_data_types.StructureDataType(slice_struct_def),
-        ),
-        self._primitive_handler,
-    )  # maybe memoize this.
-
-    # Get the value element from the slice's children.
-    value_element = slice_builder.return_type.children().get('value')
-
-    if value_element is None or _is_disabled(value_element):
-      # At this point, the current element is a slice on an extension that has
-      # no valid `Extension.value[x]` element, so we assume it is a complex
-      # extension.
-      # TODO(b/200575760): Handle complex extensions.
-      self._error_reporter.report_fhir_path_error(
-          self._abs_path_invocation(slice_builder),
-          str(slice_builder),
-          'Current element is a complex extension not supported yet.',
-      )
-      return []
-    else:
-      return _utils.element_type_codes(value_element)
-
   # TODO(b/207690471): Move important ElementDefinition (and other) functions
   # to their respective utility modules and unit test their public facing apis .
   def _get_regex_from_element(
       self, builder: expressions.Builder, elem: ElementDefinition
   ) -> Optional[_RegexInfo]:
     """Returns the regex of this element_definition if available."""
     element_definition = cast(Any, elem)
-    type_codes = _utils.element_type_codes(element_definition)
-
-    if _utils.is_slice_on_extension(element_definition):
-      type_codes = self.get_type_codes_from_slice_element(element_definition)
-
-    if not _is_elem_supported(element_definition):
-      return None
+    type_codes = _utils.element_type_codes(
+        builder.return_type.root_element_definition
+    )
 
     if not type_codes:
       return None
     if len(type_codes) > 1:
-      raise ValueError(
-          'Expected element with only one type code but got: '
-          f'{type_codes}, is this a choice type?'
-      )
-    current_type_code = type_codes[0]
+      raise ValueError(f'Expected 1 type code, got {type_codes} for {builder}')
 
+    current_type_code = type_codes[0]
     element_id: str = element_definition.id.value
     # TODO(b/208620019): Look more into how this section handles multithreading.
     # If we have memoised the regex of this element, then just return it.
     if element_id in self._element_id_to_regex_map:
       return self._element_id_to_regex_map[element_id]
 
     # Ignore regexes on primitive types that are not represented as strings.
@@ -1114,15 +1206,14 @@
     Args:
       builder: The current builder to encode regexes for.
 
     Returns:
       A list of `SqlRequirement`s representing requirements generated from
       primitive fields on the element that have regexes .
     """
-
     element_definition_path = self._abs_path_invocation(builder)
     # TODO(b/206986228): Remove this key after we start taking profiles into
     # account when encoding constraints for fields.
     if 'comparator' in element_definition_path.split('.'):
       return []
 
     if not isinstance(
@@ -1137,36 +1228,43 @@
     # If this is an extension, we don't want to access its children/fields.
     # TODO(b/200575760): Add support for complex extensions and the fields
     # inside them.
     if cast(Any, struct_def).type.value == 'Extension':
       return []
 
     encoded_requirements: List[validation_pb2.SqlRequirement] = []
-    children = builder.return_type.children()
-    for name, child_message in children.items():
+    for name, child_message in builder.return_type.iter_children():
       child = cast(Any, child_message)
 
-      # TODO(b/190679571): Handle choice types, which may have more than one
-      # `type.code` value present.
-      # If this element is a choice type, a slice (that is not on an extension)
-      # or is disabled, then don't encode requirements for it.
-      # TODO(b/202564733): Properly handle slices on non-simple extensions.
-      if '[x]' in _get_analytic_path(child) or _is_disabled(child):
+      if _is_disabled(child):
         continue
 
       if not _is_elem_supported(child):
         continue
 
       child_builder = self._get_new_child_builder(builder, name)
       if not child_builder:
         continue
 
+      # TODO(b/190679571): Handle choice types, which may have more than one
+      # `type.code` value present.
+      # TODO(b/202564733): Properly handle slices on non-simple extensions.
+      if child_builder.return_type.returns_polymorphic():
+        self._error_reporter.report_fhir_path_error(
+            self._abs_path_invocation(child_builder),
+            str(child_builder),
+            f'Element `{child_builder}` is a choice type which is not currently'
+            ' supported.',
+        )
+        continue
+
       primitive_regex_info = self._get_regex_from_element(
           child_builder, child_message
       )
+
       if primitive_regex_info is None:
         continue  # Unable to find primitive regexes for this child element.
 
       primitive_regex = primitive_regex_info.regex
       regex_type_code = primitive_regex_info.type_code
 
       constraint_key = f'{name}-matches-{regex_type_code}-regex'
@@ -1283,45 +1381,65 @@
       # inside them.
       if (
           struct_type.element_type == 'Extension'
           or struct_type.element_type == 'Resource'
       ):
         return result
 
-      for child, elem in struct_type.children().items():
+      for child, elem in struct_type.iter_all_descendants():
         # TODO(b/200575760): Add support for more complicated fields
         if (
-            ':' in child
-            or child == 'extension'
+            child == 'extension'
             or child == 'link'
             or '#' in cast(Any, elem).content_reference.value
         ):
           continue
 
         new_builder = self._get_new_child_builder(builder, child)
         if not new_builder:
           continue
 
+        # Ensure we don't visit the same element via the same FHIR
+        # path multiple times.
+        elem_visit = (self._abs_path_invocation(new_builder), elem.id.value)
+        if elem_visit in self._visited_element_definitions:
+          continue
+        self._visited_element_definitions.add(elem_visit)
+
         # TODO(b/200575760): Add support polymorphic choice types
         if not new_builder.return_type.root_element_definition:
           self._error_reporter.report_validation_error(
               child, 'Root element definition of child is None.'
           )
           # Early-exit if Root element definition of child is None.
           return result
 
-        if isinstance(
+        is_struct_def = isinstance(
             new_builder.return_type, _fhir_path_data_types.StructureDataType
-        ):
+        )
+        if is_struct_def:
           result += self._encode_structure_definition(new_builder, elem)
         else:
           result += self._encode_element_definition_of_builder(
               new_builder, elem
           )
 
+      for slice_def in struct_type.iter_slices():
+        # Ensure we don't visit the same slice via the same FHIR path
+        # multiple times.
+        slice_visit = (
+            self._abs_path_invocation(new_builder),
+            slice_def.slice_def.id.value,
+        )
+        if slice_visit in self._visited_slices:
+          continue
+        self._visited_slices.add(slice_visit)
+
+        result += self._encode_slice_definition(builder, slice_def)
+
     return result
 
   def _encode_value_set_bindings(
       self, builder: expressions.Builder, element_definition: ElementDefinition
   ) -> List[validation_pb2.SqlRequirement]:
     """Encode .memberOf calls implied by elements bound to value sets."""
     if isinstance(
@@ -1452,18 +1570,23 @@
       result = self._encode_structure_definition(builder)
       # Removes duplicates (Same SQL Expression) from our list of requirements.
       result = list(
           {
               requirement.sql_expression: requirement for requirement in result
           }.values()
       )
+      # Sort so the results are consistent for diff tests.
+      result.sort(key=operator.attrgetter('column_name'))
+
     finally:
       self._ctx.clear()
       self._in_progress.clear()
       self._requirement_column_names.clear()
+      self._visited_element_definitions.clear()
+      self._visited_slices.clear()
       self._element_id_to_regex_map.clear()
       self._regex_columns_generated.clear()
     return result
 
 
 def _fields_referenced_by_expression(
     fhir_path_expression: str,
```

## Comparing `google_fhir_core-0.9.2.data/data/annotations.proto` & `google_fhir_core-0.9.3.data/data/annotations.proto`

 * *Files identical despite different names*

## Comparing `google_fhir_core-0.9.2.data/data/fhirpath_replacement_list.proto` & `google_fhir_core-0.9.3.data/data/fhirpath_replacement_list.proto`

 * *Files identical despite different names*

## Comparing `google_fhir_core-0.9.2.data/data/validation.proto` & `google_fhir_core-0.9.3.data/data/validation.proto`

 * *Files identical despite different names*

## Comparing `google_fhir_core-0.9.2.dist-info/METADATA` & `google_fhir_core-0.9.3.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-fhir-core
-Version: 0.9.2
+Version: 0.9.3
 Summary: Core components for working with FHIR.
 Home-page: https://github.com/google/fhir-py
 Download-URL: https://github.com/google-py/fhir/releases
 Author: Google LLC
 Author-email: google-fhir-pypi@google.com
 License: Apache 2.0
 Keywords: google,fhir,python,healthcare
@@ -16,17 +16,22 @@
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 Requires-Dist: absl-py (~=1.1)
 Requires-Dist: antlr4-python3-runtime (~=4.9.3)
 Requires-Dist: immutabledict (~=2.2)
 Requires-Dist: protobuf (~=3.19)
 Requires-Dist: python-dateutil (~=2.8)
+Requires-Dist: stringcase (==1.2.0)
 Requires-Dist: backports.zoneinfo (~=0.2.1) ; python_version < "3.9"
 Provides-Extra: bigquery
 Requires-Dist: google-cloud-bigquery (~=3.1) ; extra == 'bigquery'
-Requires-Dist: sqlalchemy-bigquery (~=1.4) ; extra == 'bigquery'
 Requires-Dist: sqlalchemy (~=1.4) ; extra == 'bigquery'
+Requires-Dist: sqlalchemy-bigquery (~=1.4) ; extra == 'bigquery'
+Provides-Extra: spark
+Requires-Dist: sqlalchemy (~=1.4) ; extra == 'spark'
+Requires-Dist: pandas (>=1.5) ; extra == 'spark'
+Requires-Dist: pyhive (>=0.6) ; extra == 'spark'
 
 Core logic for working with FHIR data.
 
 Most users will not use this directly, but may use `google.fhir.views` or
 other higher-level libraries for working with FHIR data at scale.
```

