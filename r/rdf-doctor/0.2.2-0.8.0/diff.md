# Comparing `tmp/rdf_doctor-0.2.2-py3-none-any.whl.zip` & `tmp/rdf_doctor-0.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,31 @@
-Zip file size: 28305 bytes, number of entries: 14
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-20 08:28 doctor/__init__.py
--rw-r--r--  2.0 unx      619 b- defN 23-May-19 04:24 doctor/consts.py
--rw-r--r--  2.0 unx    22796 b- defN 23-May-18 06:06 doctor/doctor.py
--rw-r--r--  2.0 unx    20305 b- defN 23-Apr-28 02:45 doctor/reference/correct-prefixes.tsv
--rw-r--r--  2.0 unx    36944 b- defN 23-Apr-20 08:28 doctor/reference/rdf-config-prefixes.tsv
--rw-r--r--  2.0 unx    21257 b- defN 23-Apr-20 08:28 doctor/reference/rdf-config-prefixes.yaml
--rw-r--r--  2.0 unx      596 b- defN 23-Apr-28 06:16 doctor/reference/refine-classes.tsv
--rw-r--r--  2.0 unx      678 b- defN 23-May-16 00:01 doctor/reference/refine-prefixes.tsv
--rw-r--r--  2.0 unx     1061 b- defN 23-May-19 04:30 rdf_doctor-0.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     6257 b- defN 23-May-19 04:30 rdf_doctor-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-19 04:30 rdf_doctor-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-May-19 04:30 rdf_doctor-0.2.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-May-19 04:30 rdf_doctor-0.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1191 b- defN 23-May-19 04:30 rdf_doctor-0.2.2.dist-info/RECORD
-14 files, 111855 bytes uncompressed, 26307 bytes compressed:  76.5%
+Zip file size: 38528 bytes, number of entries: 29
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-05 08:08 doctor/__init__.py
+-rw-r--r--  2.0 unx      631 b- defN 23-Jun-05 08:08 doctor/consts.py
+-rw-r--r--  2.0 unx    26420 b- defN 23-Jun-05 08:08 doctor/doctor.py
+-rw-r--r--  2.0 unx    20305 b- defN 23-Jun-05 06:43 doctor/reference/correct-prefixes.tsv
+-rw-r--r--  2.0 unx    36944 b- defN 23-Jun-05 06:43 doctor/reference/rdf-config-prefixes.tsv
+-rw-r--r--  2.0 unx    21257 b- defN 23-Jun-05 06:43 doctor/reference/rdf-config-prefixes.yaml
+-rw-r--r--  2.0 unx       90 b- defN 23-Jun-05 06:43 doctor/reference/refine-classes.tsv
+-rw-r--r--  2.0 unx      679 b- defN 23-Jun-05 06:43 doctor/reference/refine-prefixes.tsv
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 06:43 tests/__init__.py
+-rw-r--r--  2.0 unx      754 b- defN 23-Jun-05 06:43 tests/consts.py
+-rw-r--r--  2.0 unx      958 b- defN 23-Jun-05 06:43 tests/test_fingerprint.py
+-rw-r--r--  2.0 unx     2444 b- defN 23-Jun-05 06:43 tests/test_get_class_comparison_result.py
+-rw-r--r--  2.0 unx     2335 b- defN 23-Jun-05 06:43 tests/test_get_command_line_args.py
+-rw-r--r--  2.0 unx      765 b- defN 23-Jun-05 06:43 tests/test_get_compression_mode.py
+-rw-r--r--  2.0 unx     3256 b- defN 23-Jun-05 06:43 tests/test_get_fingerprint_comparison_result.py
+-rw-r--r--  2.0 unx     3249 b- defN 23-Jun-05 06:43 tests/test_get_input_classes.py
+-rw-r--r--  2.0 unx      745 b- defN 23-Jun-05 06:43 tests/test_get_input_format.py
+-rw-r--r--  2.0 unx     2617 b- defN 23-Jun-05 06:43 tests/test_get_input_prefixes.py
+-rw-r--r--  2.0 unx     2831 b- defN 23-Jun-05 06:43 tests/test_get_markdown_result.py
+-rw-r--r--  2.0 unx      964 b- defN 23-Jun-05 06:43 tests/test_get_prefix_comparison_result.py
+-rw-r--r--  2.0 unx     1396 b- defN 23-Jun-05 06:43 tests/test_get_prefix_reuse_percentage.py
+-rw-r--r--  2.0 unx     4936 b- defN 23-Jun-05 06:43 tests/test_get_suggested_qname.py
+-rw-r--r--  2.0 unx    15594 b- defN 23-Jun-05 06:43 tests/test_validate_command_line_args.py
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jun-05 08:20 rdf_doctor-0.8.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6694 b- defN 23-Jun-05 08:20 rdf_doctor-0.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 08:20 rdf_doctor-0.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 08:20 rdf_doctor-0.8.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 08:20 rdf_doctor-0.8.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-05 08:20 rdf_doctor-0.8.0.dist-info/RECORD
+29 files, 159640 bytes uncompressed, 34398 bytes compressed:  78.5%
```

## zipnote {}

```diff
@@ -18,26 +18,71 @@
 
 Filename: doctor/reference/refine-classes.tsv
 Comment: 
 
 Filename: doctor/reference/refine-prefixes.tsv
 Comment: 
 
-Filename: rdf_doctor-0.2.2.dist-info/LICENSE
+Filename: tests/__init__.py
 Comment: 
 
-Filename: rdf_doctor-0.2.2.dist-info/METADATA
+Filename: tests/consts.py
 Comment: 
 
-Filename: rdf_doctor-0.2.2.dist-info/WHEEL
+Filename: tests/test_fingerprint.py
 Comment: 
 
-Filename: rdf_doctor-0.2.2.dist-info/entry_points.txt
+Filename: tests/test_get_class_comparison_result.py
 Comment: 
 
-Filename: rdf_doctor-0.2.2.dist-info/top_level.txt
+Filename: tests/test_get_command_line_args.py
 Comment: 
 
-Filename: rdf_doctor-0.2.2.dist-info/RECORD
+Filename: tests/test_get_compression_mode.py
+Comment: 
+
+Filename: tests/test_get_fingerprint_comparison_result.py
+Comment: 
+
+Filename: tests/test_get_input_classes.py
+Comment: 
+
+Filename: tests/test_get_input_format.py
+Comment: 
+
+Filename: tests/test_get_input_prefixes.py
+Comment: 
+
+Filename: tests/test_get_markdown_result.py
+Comment: 
+
+Filename: tests/test_get_prefix_comparison_result.py
+Comment: 
+
+Filename: tests/test_get_prefix_reuse_percentage.py
+Comment: 
+
+Filename: tests/test_get_suggested_qname.py
+Comment: 
+
+Filename: tests/test_validate_command_line_args.py
+Comment: 
+
+Filename: rdf_doctor-0.8.0.dist-info/LICENSE
+Comment: 
+
+Filename: rdf_doctor-0.8.0.dist-info/METADATA
+Comment: 
+
+Filename: rdf_doctor-0.8.0.dist-info/WHEEL
+Comment: 
+
+Filename: rdf_doctor-0.8.0.dist-info/entry_points.txt
+Comment: 
+
+Filename: rdf_doctor-0.8.0.dist-info/top_level.txt
+Comment: 
+
+Filename: rdf_doctor-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doctor/__init__.py

```diff
@@ -0,0 +1,2 @@
+00000000: 5f5f 7665 7273 696f 6e5f 5f20 3d20 2230  __version__ = "0
+00000010: 2e38 2e30 220a                           .8.0".
```

## doctor/consts.py

```diff
@@ -1,8 +1,8 @@
-VERSION = "0.2.2"
+VERSION_FILE = "__init__.py"
 
 # Report export format
 REPORT_FORMAT_SHEX = "shex"
 REPORT_FORMAT_MD = "md"               # same as markdown
 REPORT_FORMAT_MARKDOWN = "markdown"   # same as md
 
 # Target classes
@@ -17,8 +17,8 @@
 CORRECT_PREFIXES_FILE_PATH = "reference/correct-prefixes.tsv"
 
 # Errata
 CLASS_ERRATA_FILE_PATH = "reference/refine-classes.tsv"
 PREFIX_ERRATA_FILE_PATH = "reference/refine-prefixes.tsv"
 
 # Help link URL
-HELP_LINK_URL = "https://github.com/dbcls/rdf-doctor#output-description"
+HELP_LINK_URL = "https://github.com/dbcls/rdf-doctor#output-description"
```

## doctor/doctor.py

```diff
@@ -1,72 +1,101 @@
 import os
 import sys
 import argparse
 import gzip
 import rdflib
 import re
 import csv
-from doctor.consts import VERSION, REPORT_FORMAT_SHEX, REPORT_FORMAT_MD, REPORT_FORMAT_MARKDOWN, \
+import codecs
+from doctor.consts import VERSION_FILE, REPORT_FORMAT_SHEX, REPORT_FORMAT_MD, REPORT_FORMAT_MARKDOWN, \
                             TARGET_CLASS_ALL, EXTENSION_NT, EXTENSION_TTL, EXTENSION_GZ, CORRECT_PREFIXES_FILE_PATH, \
                             CLASS_ERRATA_FILE_PATH, PREFIX_ERRATA_FILE_PATH, HELP_LINK_URL
 from shexer.shaper import Shaper
 from shexer.consts import NT, TURTLE, GZ, MIXED_INSTANCES
 from unidecode import unidecode
 from collections import defaultdict
 from pathlib import Path
 
+
 # Main processing of rdf-doctor
 def doctor():
     args = get_command_line_args(sys.argv[1:])
 
-    result, error_msg = validate_command_line_args(args)
-    if result == False:
+    validation_result, error_msg = validate_command_line_args(args)
+    if validation_result == False:
         print(error_msg)
         return
 
-    compression_mode = get_compression_mode(args.input)
-    input_format = get_input_format(args.input, compression_mode)
+    compression_mode = get_compression_mode(args.input[0])
+    input_format = get_input_format(args.input[0], compression_mode)
+    output_result = []
 
     try:
         # Processing branch by report format
         if args.report == REPORT_FORMAT_SHEX:
             # shex
-            generate_report_shex(args, input_format, compression_mode)
+            output_result = get_shex_result(args, input_format, compression_mode)
+
         elif args.report == REPORT_FORMAT_MARKDOWN or args.report == REPORT_FORMAT_MD:
             # markdown/md
-            generate_report_markdown(args, input_format, compression_mode)
+            for input_file in args.input:
+                output_result.extend(get_markdown_result(input_file, input_format, compression_mode, args.classes, args.prefix_dict, args.class_dict))
+
         else:
             # Else case does not occur.
             # Prevented by validate_command_line_args function.
             raise ValueError(args.report + '" is an unsupported report format. "' + REPORT_FORMAT_SHEX + '" and "' + REPORT_FORMAT_MD+ '"(same as "' + REPORT_FORMAT_MARKDOWN + '") are supported.')
 
+        # Output result to specified destination (standard output or file)
+        if args.output is None:
+            print("".join(output_result))
+        else:
+            with open(args.output, "w", encoding="utf-8") as f:
+                f.write("".join(output_result))
+
     except ValueError as e:
         print(e)
 
     except:
         print("An exception error occurred. Input data format may not be correct. Please review the data.")
 
     return
 
 
+def read(rel_path):
+    here = os.path.abspath(os.path.dirname(__file__))
+    with codecs.open(os.path.join(here, rel_path), 'r') as fp:
+        return fp.read()
+
+
+def get_version(rel_path):
+    for line in read(rel_path).splitlines():
+        if line.startswith('__version__'):
+            delim = '"' if '"' in line else "'"
+            return line.split(delim)[1]
+    else:
+        raise RuntimeError("Unable to find version string.")
+
+
 # Parse command line arguments and get them as ArgumentParser
 def get_command_line_args(args):
     parser = argparse.ArgumentParser(description="Home page: https://github.com/dbcls/rdf-doctor",
                                     usage="rdf-doctor -i RDF-FILE [Options]",
                                     formatter_class=argparse.RawDescriptionHelpFormatter)
 
     # Version info(-v, --version)
     parser.add_argument("-v","--version",
                         action="version",
-                        version="%(prog)s " + VERSION)
+                        version="%(prog)s " + get_version(VERSION_FILE))
 
     # Input RDF file (-i、--input [RDF-FILE]、required)
     parser.add_argument("-i","--input", type=str,
                         required=True,
-                        help="input RDF file(.ttl or .nt or gzipped versions of them)",
+                        nargs="+",
+                        help="input RDF file(s)(.ttl or .nt or gzip-compressed versions of them). Use the same extension when specifying multiple.",
                         metavar="RDF-FILE")
 
     # Report format (-r、--report、default: shex)
     parser.add_argument("-r","--report", type=str,
                         default=REPORT_FORMAT_SHEX,
                         help="set the output format/serializer of report to one of: shex (defalut) or md or markdown(same as md)",
                         metavar="FORMAT")
@@ -79,14 +108,26 @@
     # Target class(-c、--classes、default: all、Multiple can be specified.)
     parser.add_argument("-c","--classes", type=str,
                         default=[TARGET_CLASS_ALL],
                         nargs="+",
                         help="set the target classes to be inspected to one of: all (defalut) or URL1, URL2,...",
                         metavar="URL")
 
+    # Prefix errata file path(-p, --prefix-dict [FILE]、default: reference/refine-prefixes.tsv)
+    parser.add_argument("-p","--prefix-dict", type=str,
+                        default=str(Path(__file__).resolve().parent.joinpath(PREFIX_ERRATA_FILE_PATH)),
+                        help="path to a tab delimited file listing incorrect and correct URI pairs for the prefix (default: predefined file in rdf-doctor)",
+                        metavar="FILE")
+
+    # Class errata file path(-l, --class-dict [FILE]、default: reference/refine-classes.tsv)
+    parser.add_argument("-l","--class-dict", type=str,
+                        default=str(Path(__file__).resolve().parent.joinpath(CLASS_ERRATA_FILE_PATH)),
+                        help="path to a tab delimited file listing incorrect and correct URI pairs for the class (default: predefined file in rdf-doctor)",
+                        metavar="FILE")
+
     return parser.parse_args(args)
 
 
 # Determine if the input file is compressed and get the compression mode ("gz" or None)
 def get_compression_mode(input_file):
     extension = os.path.splitext(input_file)[1]
     if extension == EXTENSION_GZ:
@@ -117,130 +158,154 @@
             # Else case does not occur.
             # Prevented by validate_command_line_args function.
             raise ValueError(extension + '" is an unsupported extension. ".ttl", ".ttl.gz", ".nt" and ".nt.gz" are supported.')
 
 
 # Validate args(input, output, report, classes)
 def validate_command_line_args(args):
-    if args.input is None:
-        # This case does not occur because -i / --input is required as an option when parsing command line arguments.
-        error_msg = "Input file error: No input file specified. (-i [RDF_FILE], --input [RDF_FILE])"
-        return False, error_msg
+    compression_mode = ""
+    input_format = ""
+    for input_file in args.input:
+        if input_file is None:
+            # This case does not occur because -i / --input is required as an option when parsing command line arguments.
+            error_msg = "Input file error: No input file specified. (-i [RDF_FILE], --input [RDF_FILE])"
+            return False, error_msg
 
-    if os.path.isfile(args.input) == False:
-        error_msg = "Input file error: Input file does not exist."
-        return False, error_msg
+        if os.path.isfile(input_file) == False:
+            error_msg = "Input file error: " + input_file + " does not exist."
+            return False, error_msg
+
+        if compression_mode == "":
+            compression_mode = get_compression_mode(input_file)
+        else:
+            if compression_mode != get_compression_mode(input_file):
+                error_msg = "Input file error: If you enter multiple files, please use the same extension."
+                return False, error_msg
+
+        if input_format == "":
+            input_format = get_input_format(input_file, compression_mode)
+        else:
+            if input_format != get_input_format(input_file, compression_mode):
+                error_msg = "Input file error: If you enter multiple files, please use the same extension."
+                return False, error_msg
+
+        # Allow only ".nt" or ".ttl" (and .gz) extensions
+        extension = os.path.splitext(input_file)[1]
+        if extension == EXTENSION_GZ:
+            org_extension = os.path.splitext(os.path.splitext(input_file)[0])[1]
+            # gz
+            if org_extension != EXTENSION_NT and org_extension != EXTENSION_TTL:
+                error_msg = 'Input file error: "' + extension + '" is an unsupported extension. ".ttl", ".ttl.gz", ".nt" and ".nt.gz" are supported.'
+                return False, error_msg
+        elif extension != EXTENSION_NT and extension != EXTENSION_TTL:
+            error_msg = 'Input file error: "' + extension + '" is an unsupported extension. ".ttl", ".ttl.gz", ".nt" and ".nt.gz" are supported.'
+            return False, error_msg
 
     if args.output is not None:
         # Existence check of file output destination directory
-        if os.path.dirname(args.output):
-            if os.path.exists(os.path.dirname(args.output)) == False:
+        output_dir = os.path.dirname(args.output)
+        if output_dir:
+            if os.path.exists(output_dir) == False:
                 error_msg = "Output file error: Output directory does not exist."
                 return False, error_msg
 
             # Check if the file output destination has write permission
-            if os.access(os.path.dirname(args.output), os.W_OK) == False:
+            if os.access(output_dir, os.W_OK) == False:
                 error_msg = "Output file error: You don't have write permission on the output directory."
                 return False, error_msg
 
-    # Report Format only allows "shex" or "md/markdown" or "shex+"
+    # Report Format only allows "shex" or "md/markdown"
     if args.report != REPORT_FORMAT_SHEX and \
         args.report != REPORT_FORMAT_MARKDOWN and \
         args.report != REPORT_FORMAT_MD:
         error_msg = 'Report format error: "' + args.report + '" is an unsupported report format. "' + REPORT_FORMAT_SHEX + '" and "' + REPORT_FORMAT_MD + '"(same as "' + REPORT_FORMAT_MARKDOWN + '") are supported.'
         return False, error_msg
 
-    # Allow only ".nt" or ".ttl" (and .gz) extensions
-    extension = os.path.splitext(args.input)[1]
-    if extension == EXTENSION_GZ:
-        org_extension = os.path.splitext(os.path.splitext(args.input)[0])[1]
-        # gz
-        if org_extension != EXTENSION_NT and org_extension != EXTENSION_TTL:
-            error_msg = 'Input file error: "' + extension + '" is an unsupported extension. ".ttl", ".ttl.gz", ".nt" and ".nt.gz" are supported.'
-            return False, error_msg
-    elif extension != EXTENSION_NT and extension != EXTENSION_TTL:
-        error_msg = 'Input file error: "' + extension + '" is an unsupported extension. ".ttl", ".ttl.gz", ".nt" and ".nt.gz" are supported.'
-        return False, error_msg
-
     # Make an error if another class name is specified with "all"
     if TARGET_CLASS_ALL in args.classes:
         if len(args.classes) != 1:
             error_msg = 'Target class error: If "all" is specified, other classes cannot be specified.'
             return False, error_msg
 
+
+    if os.path.isfile(args.prefix_dict) == False:
+        error_msg = "Prefix dictionary file error: Prefix dictionary does not exist."
+        return False, error_msg
+
+
+    if os.path.isfile(args.class_dict) == False:
+        error_msg = "Class dictionary file error: Class dictionary does not exist."
+        return False, error_msg
+
+
     return True, None
 
 
 # Processing when the report format is "shex"
-def generate_report_shex(args, input_format, compression_mode):
-    shaper_result = get_shaper_result(args, input_format, compression_mode)
+def get_shex_result(args, input_format, compression_mode):
+    input_prefixes = get_input_prefixes_from_multi_files(args.input, compression_mode)
+    shaper_result = get_shaper_result(args, input_format, compression_mode, input_prefixes)
 
     # Suggest QName based on URI of validation expression output by sheXer and correct-prefixes.tsv
     result_suggested_qname = []
-    input_prefixes = get_input_prefixes(args.input, compression_mode)
     correct_prefixes = get_correct_prefixes()
     suggested_qname = get_suggested_qname(shaper_result, input_prefixes, correct_prefixes)
     if len(suggested_qname) != 0:
         result_suggested_qname.append("# There may be a better QName.\n\n")
         result_suggested_qname.append("# Input QName\tSuggested QName\tURI\n")
         result_suggested_qname.extend(["# " + s for s in suggested_qname])
         result_suggested_qname.append("\n")
 
     # List for storing the final result
     shex_final_result = []
     shex_final_result.extend(shaper_result)
     if len(result_suggested_qname) != 0:
         shex_final_result.extend(result_suggested_qname)
 
-    # Output results to specified destination (standard output or file)
-    if args.output is None:
-        print("".join(shex_final_result))
-    else:
-        with open(args.output, "w", encoding="utf-8") as f:
-            f.write("".join(shex_final_result))
+    return shex_final_result
 
 
 # Processing when the report format is "md/markdown"
-def generate_report_markdown(args, input_format, compression_mode):
+def get_markdown_result(input_file, input_format, compression_mode, classes, prefix_dict, class_dict):
 
     # Processing related to prefixes ------------------
     # Get list for result output about prefix reuse rate
     result_prefix_reuse_percentage = []
-    input_prefixes = get_input_prefixes(args.input, compression_mode)
+    input_prefixes = get_input_prefixes(input_file, compression_mode)
     result_prefix_reuse_percentage.append("## Prefix reuse percentage ([?](" + HELP_LINK_URL + "))\n")
     result_prefix_reuse_percentage.append("Percentage of prefixes used in the input file that are included in the predefined prefix list inside rdf-doctor.\n")
     prefix_reuse_percentage = get_prefix_reuse_percentage(input_prefixes)
     if prefix_reuse_percentage == None:
         result_prefix_reuse_percentage.append("```\n")
         result_prefix_reuse_percentage.append("Not calculated because there is no prefix defined.\n")
         result_prefix_reuse_percentage.append("```\n\n")
     else:
         result_prefix_reuse_percentage.append("```\n")
         result_prefix_reuse_percentage.append(str(prefix_reuse_percentage) + "%\n")
         result_prefix_reuse_percentage.append("```\n\n")
 
     # Refer to the errata of prefixes and obtain a list for result output that combines incorrect prefixes and correct prefixes
     result_prefix_errata = []
-    prefix_comparison_result = get_prefix_comparison_result(input_prefixes)
+    prefix_comparison_result = get_prefix_comparison_result(input_prefixes, prefix_dict)
     # When there is data to output
     if len(prefix_comparison_result) != 0:
         result_prefix_errata.append("Found prefixes that looks incorrect.\n")
         result_prefix_errata.append("```\n")
         result_prefix_errata.append("Prefix\tInput URI\tSuggested URI\n")
         result_prefix_errata.extend(prefix_comparison_result)
         result_prefix_errata.append("```\n\n")
     # -------------------------------------------------
 
     # Processing related to classes -------------------
-    input_classes = get_input_classes(args.input, input_format, compression_mode, args.classes)
+    input_classes = get_input_classes(input_file, input_format, compression_mode, classes)
 
     # Refers to the errata list of the class, acquires the list for result output that combines the incorrect class and the correct class,
     # and returns the class corresponding to each key in fingerprint format stored in dictionary format.
     result_class_errata = []
-    class_comparison_result, fingerprint_class_dict = get_class_comparison_result(input_classes, defaultdict(list))
+    class_comparison_result, fingerprint_class_dict = get_class_comparison_result(input_classes, defaultdict(list), class_dict)
     # When there is data to output
     if len(class_comparison_result) != 0:
         result_class_errata.append("Found class names that looks incorrect.\n")
         result_class_errata.append("```\n")
         result_class_errata.append("Input class name\tSuggested class name\n")
         result_class_errata.extend(class_comparison_result)
         result_class_errata.append("```\n\n")
@@ -255,15 +320,15 @@
         result_class_fingerprint.extend(fingerprint_comparison_result)
         result_class_fingerprint.append("\n```\n\n")
     # -------------------------------------------------
 
     # List for storing the final result
     md_final_result = []
 
-    md_final_result.append("# Report on " + os.path.basename(args.input) + "\n\n")
+    md_final_result.append("# Report on " + os.path.basename(input_file) + "\n\n")
 
     # Merge result
     md_final_result.extend(result_prefix_reuse_percentage)
 
     prefix_result_exists = len(result_prefix_errata) != 0
     if prefix_result_exists:
         md_final_result.append("## Refine prefixes ([?](" + HELP_LINK_URL + "))\n")
@@ -271,36 +336,44 @@
 
     class_result_exists = len(result_class_errata) != 0 or len(result_class_fingerprint) != 0
     if class_result_exists:
         md_final_result.append("## Refine classes ([?](" + HELP_LINK_URL + "))\n")
         md_final_result.extend(result_class_errata)
         md_final_result.extend(result_class_fingerprint)
 
-    # Output results to specified destination (standard output or file)
-    if args.output is None:
-        print("".join(md_final_result))
-    else:
-        with open(args.output, "w", encoding="utf-8") as f:
-            f.write("".join(md_final_result))
+    return md_final_result
+
 
 # Call the shex_graph method of shexer's shaper class and output the result
-def get_shaper_result(args, input_format, compression_mode):
+def get_shaper_result(args, input_format, compression_mode, input_prefixes):
     # Set parameters when calling the shaper class depending on whether the class is specified as an argument
     if TARGET_CLASS_ALL in args.classes:
         target_classes = None
         all_classes_mode = True
     else:
         target_classes = args.classes
         all_classes_mode = False
 
+    namespaces_dict = {}
+    for input_prefix in input_prefixes:
+        namespaces_dict[input_prefix[1]] = input_prefix[0].replace(":","")
+
+    if len(args.input) == 1:
+        graph_file_input = args.input[0]
+        graph_list_of_files_input = None
+    else:
+        graph_file_input = None
+        graph_list_of_files_input = args.input
     # Init shexer's shaper class
-    shaper = Shaper(graph_file_input=args.input,
+    shaper = Shaper(graph_file_input=graph_file_input,
+                    graph_list_of_files_input=graph_list_of_files_input,
                     target_classes=target_classes,
                     all_classes_mode=all_classes_mode,
                     input_format=input_format,
+                    namespaces_dict=namespaces_dict,
                     compression_mode=compression_mode,
                     instances_report_mode=MIXED_INSTANCES,
                     detect_minimal_iri=True)
 
     return shaper.shex_graph(string_output=True)
 
 
@@ -357,58 +430,59 @@
     for row in qres:
         input_classes.append(f"{row.class_name}")
 
     return input_classes
 
 
 # Return class errata in a two-dimensional array
-def get_class_errata():
-    with open(Path(__file__).resolve().parent.joinpath(CLASS_ERRATA_FILE_PATH), mode="r", newline="\n", encoding="utf-8") as f:
+def get_class_errata(class_errata_file):
+    with open(class_errata_file, mode="r", newline="\n", encoding="utf-8") as f:
         tsv_reader = csv.reader(f, delimiter="\t")
         class_errata = [row for row in tsv_reader]
 
     return class_errata
 
 
 # Return prefix errata in a two-dimensional array
-def get_prefix_errata():
-    with open(Path(__file__).resolve().parent.joinpath(PREFIX_ERRATA_FILE_PATH), mode="r", newline="\n", encoding="utf-8") as f:
+def get_prefix_errata(prefix_errata_file):
+    with open(prefix_errata_file, mode="r", newline="\n", encoding="utf-8") as f:
         tsv_reader = csv.reader(f, delimiter="\t")
         prefix_errata = [row for row in tsv_reader]
 
     return prefix_errata
 
 
-# Refers to the errata list of the class, acquires the list for result output that combines the incorrect class and the correct class,
-# and returns the class corresponding to each key in fingerprint format stored in dictionary format.
-def get_class_comparison_result(input_classes, fingerprint_class_dict):
-    class_errata = get_class_errata()
+# Get a combined list of incorrect and correct classes obtained by referencing the class errata list.
+# Create a dictionary with a class corresponding to each key in the stored fingerprint format.
+# Return the two.
+def get_class_comparison_result(input_classes, fingerprint_class_dict, class_errata_file):
+    class_errata = get_class_errata(class_errata_file)
     class_comparison_result = []
 
     # Perform clustering by fingerprint for the acquired class name
-    for cls in input_classes:
-        fingerprint_class_dict[fingerprint(cls)].append(cls)
+    for input_class in input_classes:
+        fingerprint_class_dict[fingerprint(input_class)].append(input_class)
         for eratta in class_errata:
-            if cls == eratta[0]:
-                class_comparison_result.append(cls+"\t"+eratta[1]+"\n")
+            if input_class == eratta[0]:
+                class_comparison_result.append(input_class+"\t"+eratta[1]+"\n")
                 break
 
     return class_comparison_result, fingerprint_class_dict
 
 
 # Refer to the errata of prefixes and obtain a list that combines incorrect prefixes and correct prefixes
-def get_prefix_comparison_result(input_prefixes):
-    prefix_errata = get_prefix_errata()
+def get_prefix_comparison_result(input_prefixes, prefix_errata_file):
+    prefix_errata = get_prefix_errata(prefix_errata_file)
     prefix_comparison_result = []
 
     # Perform clustering by fingerprint for the acquired class name
-    for prefix in input_prefixes:
+    for input_prefix in input_prefixes:
         for eratta in prefix_errata:
-            if prefix[1] == eratta[0] and eratta[1] != "":
-                prefix_comparison_result.append(str(prefix[0]+"\t"+prefix[1]+"\t"+eratta[1]+"\n"))
+            if input_prefix[1] == eratta[0] and eratta[1] != "":
+                prefix_comparison_result.append(str(input_prefix[0]+"\t"+input_prefix[1]+"\t"+eratta[1]+"\n"))
                 break
 
     return prefix_comparison_result
 
 
 # Get the output result when there are multiple different strings with the same key for the class
 def get_fingerprint_comparison_result(fingerprint_class_dict):
@@ -420,29 +494,15 @@
                 fingerprint_comparison_result.append("\n")
             for v in value:
                 fingerprint_comparison_result.append("\n"+v)
 
     return fingerprint_comparison_result
 
 
-# Get the output result when there are multiple different strings with the same key for the class, as a commnet
-def get_fingerprint_comparison_result_as_comment(fingerprint_class_dict):
-    fingerprint_comparison_result = []
-    # Extract if there are multiple different strings with the same key
-    for value in fingerprint_class_dict.values():
-        if len(value) >= 2:
-            if len(fingerprint_comparison_result) != 0:
-                fingerprint_comparison_result.append("\n")
-            for v in value:
-                fingerprint_comparison_result.append("\n"+"# "+v)
-
-    return fingerprint_comparison_result
-
-
-# Get the prefixes contained within the input file
+# Get the prefixes contained within the input file (from single file)
 def get_input_prefixes(input_file, compression_mode):
     if compression_mode != None:
         with gzip.open(input_file, mode="rt", encoding="utf-8") as f:
             data = f.read().splitlines()
     else:
         with open(input_file, mode="r", newline="\n", encoding="utf-8") as f:
             data = f.read().splitlines()
@@ -455,14 +515,36 @@
             uri = line_mod[line_mod.find("<")+1:line_mod.find(">")]
             if [qname, uri] not in input_prefixes:
                 input_prefixes.append([qname, uri])
 
     return input_prefixes
 
 
+# Get the prefixes contained within the input files (from mauti files)
+def get_input_prefixes_from_multi_files(input_files, compression_mode):
+    input_prefixes = []
+    for input_file in input_files:
+        if compression_mode != None:
+            with gzip.open(input_file, mode="rt", encoding="utf-8") as f:
+                data = f.read().splitlines()
+        else:
+            with open(input_file, mode="r", newline="\n", encoding="utf-8") as f:
+                data = f.read().splitlines()
+
+        for line in data:
+            if ("@prefix" in line or "@PREFIX" in line):
+                line_mod = line.replace("@prefix", "").replace("@PREFIX", "").replace(" ", "").replace("\t","")
+                qname = line_mod[:line_mod.find(":")+1]
+                uri = line_mod[line_mod.find("<")+1:line_mod.find(">")]
+                if [qname, uri] not in input_prefixes:
+                    input_prefixes.append([qname, uri])
+
+    return input_prefixes
+
+
 # Get the correct prefix from a prepared prefix list
 def get_correct_prefixes():
     with open(Path(__file__).resolve().parent.joinpath(CORRECT_PREFIXES_FILE_PATH), mode="r", newline="\n", encoding="utf-8") as f:
         tsv_reader = csv.reader(f, delimiter="\t")
         correct_prefixes = [row for row in tsv_reader]
 
     return correct_prefixes
```

## doctor/reference/refine-classes.tsv

```diff
@@ -1,8 +1 @@
-http://xmlns.com/foaf/0.1#Person	http://xmlns.com/foaf/0.1/Person
-http://xmlns.com/foaf/0.1/PErson	http://xmlns.com/foaf/0.1/Person
-http://xmlns.com/foaf/0.1/Parson	http://xmlns.com/foaf/0.1/Person
-http://xmlns.com/foaf/0.1/PERSON	http://xmlns.com/foaf/0.1/Person
-http://xmlns.com/foaf/0.1#Document	http://xmlns.com/foaf/0.1/Document
-http://xmlns.com/foaf/0.1/Docment	http://xmlns.com/foaf/0.1/Document
-http://xmlns.com/foaf/0.1/DOCUMENT	http://xmlns.com/foaf/0.1/Document
-http://www.ebi.ac.uk/chebi/searchId.do?chebiId=CHEBI%3APErson	http://www.ebi.ac.uk/chebi/searchId.do?chebiId=CHEBI%3APerson
+http://purl.jp/knapsack/resource#KNApSAcKReference  http://purl.org/ontology/bibo/Article
```

## doctor/reference/refine-prefixes.tsv

 * *Ordering differences only*

```diff
@@ -3,8 +3,8 @@
 http://identifiers.org/dbsnp/	https://identifiers.org/dbsnp:
 http://identifiers.org/dbsnp	https://identifiers.org/dbsnp:
 http://purl.jp/bio/10/dbsnp/	https://identifiers.org/dbsnp:
 http://identifiers.org/chebi/CHEBI:	http://purl.obolibrary.org/obo/CHEBI_
 http://purl.obolibrary.org/obo/chebi/	http://purl.obolibrary.org/obo/CHEBI_
 http://purl.obolibrary.org/obo/chebi.	http://purl.obolibrary.org/obo/CHEBI_
 http://purl.obolibrary.org/obo/chebi#	http://purl.obolibrary.org/obo/CHEBI_
-http://rdf.ebi.ac.uk/resource/chembl/molecule/CHEMBL	
+http://rdf.ebi.ac.uk/resource/chembl/molecule/CHEMBL
```

## Comparing `rdf_doctor-0.2.2.dist-info/LICENSE` & `rdf_doctor-0.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rdf_doctor-0.2.2.dist-info/METADATA` & `rdf_doctor-0.8.0.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdf-doctor
-Version: 0.2.2
+Version: 0.8.0
 Summary: Validate RDF data, report problems, and support creation of more accurate data
 Home-page: https://github.com/dbcls/rdf-doctor
 Author: DBCLS
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -46,25 +46,29 @@
 ## Command Line Interface
 ```
 $ rdf-doctor --help
 usage: rdf-doctor -i RDF-FILE [Options]
 
 Home page: https://github.com/dbcls/rdf-doctor
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
-  -i RDF-FILE, --input RDF-FILE
-                        input RDF file(.ttl or .nt or gziped versions of them)
+  -i RDF-FILE [RDF-FILE ...], --input RDF-FILE [RDF-FILE ...]
+                        input RDF file(s)(.ttl or .nt or gzip-compressed versions of them). Use the same extension when specifying multiple.
   -r FORMAT, --report FORMAT
                         set the output format/serializer of report to one of: shex (defalut) or md or markdown(same as md)
   -o FILE, --output FILE
                         write to file instead of stdout
   -c URL [URL ...], --classes URL [URL ...]
                         set the target classes to be inspected to one of: all (defalut) or URL1, URL2,...
+  -p FILE, --prefix-dict FILE
+                        path to a tab delimited file listing incorrect and correct URI pairs for the prefix (default: predefined file in rdf-doctor)
+  -l FILE, --class-dict FILE
+                        path to a tab delimited file listing incorrect and correct URI pairs for the class (default: predefined file in rdf-doctor)
 ```
 
 ## See Also
 - [1] https://github.com/DaniFdezAlvarez/shexer
 - [2] http://shex.io/shex-primer/#combined-constraints
 - [3] https://openrefine.org/docs/technical-reference/clustering-in-depth#fingerprint
```

