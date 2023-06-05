# Comparing `tmp/gentoo_update-0.1.tar.gz` & `tmp/gentoo_update-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentoo_update-0.1.tar", last modified: Sun Jun  4 20:39:19 2023, max compression
+gzip compressed data, was "gentoo_update-0.1.1.tar", last modified: Mon Jun  5 21:44:29 2023, max compression
```

## Comparing `gentoo_update-0.1.tar` & `gentoo_update-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 labbrat   (1000) labbrat   (1000)        0 2023-06-04 20:39:19.718036 gentoo_update-0.1/
--rw-r--r--   0 labbrat   (1000) labbrat   (1000)     1071 2023-06-04 20:26:44.000000 gentoo_update-0.1/LICENSE
--rw-r--r--   0 labbrat   (1000) labbrat   (1000)     1820 2023-06-04 20:39:19.718036 gentoo_update-0.1/PKG-INFO
--rw-r--r--   0 labbrat   (1000) labbrat   (1000)     1382 2023-06-04 20:26:44.000000 gentoo_update-0.1/README.md
-drwxr-xr-x   0 labbrat   (1000) labbrat   (1000)        0 2023-06-04 20:39:19.718036 gentoo_update-0.1/gentoo_update.egg-info/
--rw-r--r--   0 labbrat   (1000) labbrat   (1000)     1820 2023-06-04 20:39:19.000000 gentoo_update-0.1/gentoo_update.egg-info/PKG-INFO
--rw-r--r--   0 labbrat   (1000) labbrat   (1000)      252 2023-06-04 20:39:19.000000 gentoo_update-0.1/gentoo_update.egg-info/SOURCES.txt
--rw-r--r--   0 labbrat   (1000) labbrat   (1000)        1 2023-06-04 20:39:19.000000 gentoo_update-0.1/gentoo_update.egg-info/dependency_links.txt
--rw-r--r--   0 labbrat   (1000) labbrat   (1000)       53 2023-06-04 20:39:19.000000 gentoo_update-0.1/gentoo_update.egg-info/entry_points.txt
--rw-r--r--   0 labbrat   (1000) labbrat   (1000)       14 2023-06-04 20:39:19.000000 gentoo_update-0.1/gentoo_update.egg-info/top_level.txt
--rw-r--r--   0 labbrat   (1000) labbrat   (1000)     6021 2023-06-04 20:26:44.000000 gentoo_update-0.1/gentoo_update.py
--rw-r--r--   0 labbrat   (1000) labbrat   (1000)      611 2023-06-04 20:39:19.718036 gentoo_update-0.1/setup.cfg
--rw-r--r--   0 labbrat   (1000) labbrat   (1000)       38 2023-06-04 20:26:44.000000 gentoo_update-0.1/setup.py
--rwxr-xr-x   0 labbrat   (1000) labbrat   (1000)     4545 2023-06-04 20:26:44.000000 gentoo_update-0.1/updater.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:44:29.005976 gentoo_update-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-05 21:44:20.000000 gentoo_update-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-05 21:44:29.005976 gentoo_update-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-05 21:44:20.000000 gentoo_update-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:44:29.005976 gentoo_update-0.1.1/gentoo_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-05 21:44:28.000000 gentoo_update-0.1.1/gentoo_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-05 21:44:29.000000 gentoo_update-0.1.1/gentoo_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:44:28.000000 gentoo_update-0.1.1/gentoo_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-05 21:44:28.000000 gentoo_update-0.1.1/gentoo_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 21:44:28.000000 gentoo_update-0.1.1/gentoo_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-06-05 21:44:20.000000 gentoo_update-0.1.1/gentoo_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-05 21:44:29.005976 gentoo_update-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 21:44:20.000000 gentoo_update-0.1.1/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4545 2023-06-05 21:44:20.000000 gentoo_update-0.1.1/updater.sh
```

### Comparing `gentoo_update-0.1/LICENSE` & `gentoo_update-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gentoo_update-0.1/PKG-INFO` & `gentoo_update-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentoo_update
-Version: 0.1
+Version: 0.1.1
 Summary: Gentoo Linux updater
 Home-page: https://github.com/Lab-Brat/gentoo_update
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gentoo_update-0.1/README.md` & `gentoo_update-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gentoo_update-0.1/gentoo_update.egg-info/PKG-INFO` & `gentoo_update-0.1.1/gentoo_update.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentoo-update
-Version: 0.1
+Version: 0.1.1
 Summary: Gentoo Linux updater
 Home-page: https://github.com/Lab-Brat/gentoo_update
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gentoo_update-0.1/gentoo_update.py` & `gentoo_update-0.1.1/gentoo_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,26 +45,26 @@
 
     logger.addHandler(terminal_handler)
     logger.addHandler(file_handler)
 
     return logger, log_filename
 
 
-def run_shell_script(script_path, *args):
+def run_shell_script(*args):
     """
     Run a shell script and stream standard output
     and standard error to terminal and a log file.
 
     Args:
         script_path (str): Shell script path.
         *args (str): Arguments for the shell script.
                      They need to be handled by the script.
     """
     logger, log_file = create_logger()
-    command = shlex.split(f"sh {script_path} {' '.join(args)}")
+    command = shlex.split(f"updater.sh {' '.join(args)}")
     with subprocess.Popen(
         command, stdout=subprocess.PIPE, stderr=subprocess.PIPE
     ) as script_stream:
         # Process stdout
         for line in script_stream.stdout:
             logger.info(line.decode().rstrip("\n"))
 
@@ -75,16 +75,15 @@
             stderr_output.append(line)
             logger.error(line)
 
         script_stream.wait()
 
         if script_stream.returncode != 0:
             error_message = (
-                f"{script_path} "
-                "exited with error code {script_stream.returncode}"
+                "updater.sh exited with error code {script_stream.returncode}"
             )
             if stderr_output:
                 stderr_output_message = "n".join(stderr_output)
                 error_message += (
                     f"\nStandard error output:\n{stderr_output_message}"
                 )
             logger.error(error_message)
@@ -153,16 +152,15 @@
         "Default: n\n",
     )
     parser.add_argument(
         "-l",
         "--read-logs",
         default="n",
         choices=["y", "n"],
-        help="Set wether to read elogs after an update.\n"
-        "Default: n\n",
+        help="Set wether to read elogs after an update.\n" "Default: n\n",
     )
     parser.add_argument(
         "-n",
         "--read-news",
         default="n",
         choices=["y", "n"],
         help="Set wether to read news after an update.\n" "Default: n\n",
@@ -196,15 +194,14 @@
     return prefixed_args
 
 
 def main():
     args = create_cli()
 
     run_shell_script(
-        f"{current_path}/updater.sh",
         args.update_mode,
         " ".join(add_prefixes(args.args)) if args.args else "NOARGS",
         args.config_update_mode,
         args.daemon_restart,
         args.clean,
         args.read_logs,
         args.read_news,
```

### Comparing `gentoo_update-0.1/setup.cfg` & `gentoo_update-0.1.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gentoo_update
-version = 0.1
+version = 0.1.1
 description = Gentoo Linux updater
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Lab-Brat
 author_email = labbrat_social@pm.me
 url = https://github.com/Lab-Brat/gentoo_update
 license = MIT
```

### Comparing `gentoo_update-0.1/updater.sh` & `gentoo_update-0.1.1/updater.sh`

 * *Files identical despite different names*

