# Comparing `tmp/cpython_lldb-0.3.1.tar.gz` & `tmp/cpython_lldb-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpython_lldb-0.3.1.tar", max compression
+gzip compressed data, was "cpython_lldb-0.3.2.tar", max compression
```

## Comparing `cpython_lldb-0.3.1.tar` & `cpython_lldb-0.3.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1082 2023-05-12 21:31:27.597205 cpython_lldb-0.3.1/LICENSE
--rw-r--r--   0        0        0     8973 2023-05-12 21:31:27.597205 cpython_lldb-0.3.1/README.md
--rw-r--r--   0        0        0    36903 2023-05-12 21:31:27.597205 cpython_lldb-0.3.1/cpython_lldb.py
--rw-r--r--   0        0        0      802 2023-05-12 21:31:41.266453 cpython_lldb-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     9920 1970-01-01 00:00:00.000000 cpython_lldb-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-05 16:36:52.698127 cpython_lldb-0.3.2/LICENSE
+-rw-r--r--   0        0        0     9009 2023-06-05 16:36:52.698127 cpython_lldb-0.3.2/README.md
+-rw-r--r--   0        0        0    36903 2023-06-05 16:36:52.698127 cpython_lldb-0.3.2/cpython_lldb.py
+-rw-r--r--   0        0        0      800 2023-06-05 16:37:04.730084 cpython_lldb-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     9954 1970-01-01 00:00:00.000000 cpython_lldb-0.3.2/PKG-INFO
```

### Comparing `cpython_lldb-0.3.1/LICENSE` & `cpython_lldb-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cpython_lldb-0.3.1/README.md` & `cpython_lldb-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Overview
 ========
 
 ![build status](https://github.com/malor/cpython-lldb/actions/workflows/tests.yml/badge.svg)
 
 `cpython_lldb` is an LLDB extension for debugging Python programs.
 
-It may be useful for troubleshooting stuck threads and crashes in the interpreter,
-or external libraries. Unlike most Python debuggers, LLDB allows you to attach to
-a running process w/o instrumenting it in advance, or load a coredump and do a
-post-mortem analysis of a problem.
+It can be useful for troubleshooting stuck threads and crashes in the interpreter
+or external libraries. Unlike most Python debuggers, LLDB allows attaching to a
+running process without instrumenting it in advance, as well as loading a process
+coredump to perform an offline (or post-mortem) analysis of a problem.
 
 When analyzing the state of a Python process, normally you would only have
-access to the *intepreter-level* information: every variable would be of type
-PyObject\*, and stack traces would only contain CPython internal calls and
-calls to external libraries. Unless you are a CPython developer troubleshooting
-some bug in the implementation of the interpreter, that is typically not
-very useful. This extension, however, allows you to extract the *application-level*
-information about execution of a program: print the values of variables,
-list the source code, display Python stack traces, etc.
+access to *intepreter-level* information: most variables would be of type
+`PyObject*`, and stack traces would only contain CPython internal calls and
+calls to library functions. Unless you are a CPython developer troubleshooting
+the interpreter implementation, that is typically not very useful. This extension,
+however, allows you to extract *application-level* information about execution of
+a program: print the values of variables, list the source code, display Python
+stack traces, etc.
 
-While CPython itself provides a similar extension for gdb [out of the box](
+While CPython already provides a similar extension for gdb [out of the box](
 https://github.com/python/cpython/blob/master/Tools/gdb/libpython.py),
-one might still prefer to use LLDB as a debugger, e.g. on Mac OS.
+LLDB might be the debugger of choice on some operating systems, e.g.
+on Mac OS.
 
-`cpython_lldb` requires CPython to be built with debugging symbols, which is
-not the case for some Linux distros (most notably Arch Linux). CPython official
-[Docker images](https://hub.docker.com/_/python) are known to work correctly,
-as they are used for integration testing.
+This extension requires CPython to be built with debugging symbols enabled, which
+is not the case for some Linux distros (notably Arch Linux). CPython official
+[Docker images](https://hub.docker.com/_/python) are known to work correctly, as they
+are used for integration testing.
 
 
 Features
 ========
 
 `cpython_lldb` targets CPython 3.5+ and supports the following features:
 
@@ -49,16 +50,16 @@
 
 ```shell
 $ python -m pip install --user cpython-lldb
 $ echo "command script import cpython_lldb" >> ~/.lldbinit
 $ chmod +x ~/.lldbinit
 ```
 
-Alternatively, you can install the extension to some other location on disk
-and tell LLDB to load it from there, e.g. ~/.lldb:
+Alternatively, you can install the extension to some other location and tell LLDB
+to load it from there, e.g. ~/.lldb:
 
 ```shell
 $ mkdir -p ~/.lldb/cpython_lldb
 $ python -m pip install --target ~/.lldb/cpython_lldb cpython-lldb
 $ echo "command script import ~/.lldb/cpython_lldb/cpython_lldb.py" >> ~/.lldbinit
 $ chmod +x ~/.lldbinit
 ```
@@ -76,15 +77,15 @@
   "executable":"/Library/.../Python3.framework/Versions/3.9/bin/python3",
   "language":"python",
   "lldb-pythonpath":"/Library/.../LLDB.framework/Resources/Python",
   "prefix":"/Library/.../Python3.framework/Versions/3.9"
 }
 ```
 Where the value for "executable" is the CPython version that should be used to install
-cpython_lldb for LLDB to be able to successfully import the script:
+`cpython_lldb` for LLDB to be able to successfully import the script:
 ```shell
 $(lldb --print-script-interpreter-info | jq -r .executable) -m pip install cpython_lldb
 ```
 
 Usage
 =====
 
@@ -272,39 +273,38 @@
 on CentOS / Fedora / RHEL do:
 
 ```shell
 $ sudo yum install python-debuginfo
 ```
 
 Other distros, like Arch Linux, do not provide debugging symbols in the package repos. In this case,
-you would need to build CPython from source. Please refer to official [CPython](https://devguide.python.org/setup/#compiling)
-or [distro](https://wiki.archlinux.org/index.php/Debug_-_Getting_Traces) docs for instructions.
+you would need to build CPython from source. Please refer to the official [CPython](https://devguide.python.org/setup/#compiling)
+or [distro](https://wiki.archlinux.org/index.php/Debug_-_Getting_Traces) documentation for instructions.
 
-Alternatively, you can use official CPython [Docker images](https://hub.docker.com/_/python).
+Alternatively, you can use the official CPython [Docker images](https://hub.docker.com/_/python).
 
 
 Broken LLDB scripting
 ---------------------
 
-Some Linux distros (most notably Debian Stretch) are shipped with a version of LLDB in which Python scripting
+Some Linux distros (notably Debian Stretch) are shipped with a version of LLDB in which using Python scripting
 triggers a segmentation fault when executing any non-trivial operation:
 
 ```shell
 $ lldb
 (lldb) script
 Python Interactive Interpreter. To exit, type 'quit()', 'exit()' or Ctrl-D.
 >>> import io
 >>> Segmentation fault
 ```
 
 It's recommended that you use the latest LLDB release from the official [APT repo](https://apt.llvm.org/) instead
 of the one shipped with your distro.
 
-See this [page](https://github.com/vadimcn/vscode-lldb/wiki/Troubleshooting) for advice on
-troubleshooting of LLDB.
+See this [page](https://github.com/vadimcn/vscode-lldb/wiki/Troubleshooting) for advice on troubleshooting LLDB.
 
 Development
 ===========
 
 Running tests
 -------------
```

### Comparing `cpython_lldb-0.3.1/cpython_lldb.py` & `cpython_lldb-0.3.2/cpython_lldb.py`

 * *Files identical despite different names*

### Comparing `cpython_lldb-0.3.1/pyproject.toml` & `cpython_lldb-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cpython-lldb"
-version = "0.3.1"
-description = "LLDB script for debugging of CPython processes"
+version = "0.3.2"
+description = "LLDB extension for debugging Python programs"
 license = "MIT"
 
 authors = [
     "Roman Podoliaka <roman.podoliaka@gmail.com>",
 ]
 
 readme = "README.md"
```

### Comparing `cpython_lldb-0.3.1/PKG-INFO` & `cpython_lldb-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cpython-lldb
-Version: 0.3.1
-Summary: LLDB script for debugging of CPython processes
+Version: 0.3.2
+Summary: LLDB extension for debugging Python programs
 Home-page: https://github.com/malor/cpython-lldb
 License: MIT
 Keywords: debugging,lldb,cpython
 Author: Roman Podoliaka
 Author-email: roman.podoliaka@gmail.com
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*
 Classifier: License :: OSI Approved :: MIT License
@@ -24,36 +24,37 @@
 Overview
 ========
 
 ![build status](https://github.com/malor/cpython-lldb/actions/workflows/tests.yml/badge.svg)
 
 `cpython_lldb` is an LLDB extension for debugging Python programs.
 
-It may be useful for troubleshooting stuck threads and crashes in the interpreter,
-or external libraries. Unlike most Python debuggers, LLDB allows you to attach to
-a running process w/o instrumenting it in advance, or load a coredump and do a
-post-mortem analysis of a problem.
+It can be useful for troubleshooting stuck threads and crashes in the interpreter
+or external libraries. Unlike most Python debuggers, LLDB allows attaching to a
+running process without instrumenting it in advance, as well as loading a process
+coredump to perform an offline (or post-mortem) analysis of a problem.
 
 When analyzing the state of a Python process, normally you would only have
-access to the *intepreter-level* information: every variable would be of type
-PyObject\*, and stack traces would only contain CPython internal calls and
-calls to external libraries. Unless you are a CPython developer troubleshooting
-some bug in the implementation of the interpreter, that is typically not
-very useful. This extension, however, allows you to extract the *application-level*
-information about execution of a program: print the values of variables,
-list the source code, display Python stack traces, etc.
+access to *intepreter-level* information: most variables would be of type
+`PyObject*`, and stack traces would only contain CPython internal calls and
+calls to library functions. Unless you are a CPython developer troubleshooting
+the interpreter implementation, that is typically not very useful. This extension,
+however, allows you to extract *application-level* information about execution of
+a program: print the values of variables, list the source code, display Python
+stack traces, etc.
 
-While CPython itself provides a similar extension for gdb [out of the box](
+While CPython already provides a similar extension for gdb [out of the box](
 https://github.com/python/cpython/blob/master/Tools/gdb/libpython.py),
-one might still prefer to use LLDB as a debugger, e.g. on Mac OS.
+LLDB might be the debugger of choice on some operating systems, e.g.
+on Mac OS.
 
-`cpython_lldb` requires CPython to be built with debugging symbols, which is
-not the case for some Linux distros (most notably Arch Linux). CPython official
-[Docker images](https://hub.docker.com/_/python) are known to work correctly,
-as they are used for integration testing.
+This extension requires CPython to be built with debugging symbols enabled, which
+is not the case for some Linux distros (notably Arch Linux). CPython official
+[Docker images](https://hub.docker.com/_/python) are known to work correctly, as they
+are used for integration testing.
 
 
 Features
 ========
 
 `cpython_lldb` targets CPython 3.5+ and supports the following features:
 
@@ -72,16 +73,16 @@
 
 ```shell
 $ python -m pip install --user cpython-lldb
 $ echo "command script import cpython_lldb" >> ~/.lldbinit
 $ chmod +x ~/.lldbinit
 ```
 
-Alternatively, you can install the extension to some other location on disk
-and tell LLDB to load it from there, e.g. ~/.lldb:
+Alternatively, you can install the extension to some other location and tell LLDB
+to load it from there, e.g. ~/.lldb:
 
 ```shell
 $ mkdir -p ~/.lldb/cpython_lldb
 $ python -m pip install --target ~/.lldb/cpython_lldb cpython-lldb
 $ echo "command script import ~/.lldb/cpython_lldb/cpython_lldb.py" >> ~/.lldbinit
 $ chmod +x ~/.lldbinit
 ```
@@ -99,15 +100,15 @@
   "executable":"/Library/.../Python3.framework/Versions/3.9/bin/python3",
   "language":"python",
   "lldb-pythonpath":"/Library/.../LLDB.framework/Resources/Python",
   "prefix":"/Library/.../Python3.framework/Versions/3.9"
 }
 ```
 Where the value for "executable" is the CPython version that should be used to install
-cpython_lldb for LLDB to be able to successfully import the script:
+`cpython_lldb` for LLDB to be able to successfully import the script:
 ```shell
 $(lldb --print-script-interpreter-info | jq -r .executable) -m pip install cpython_lldb
 ```
 
 Usage
 =====
 
@@ -295,39 +296,38 @@
 on CentOS / Fedora / RHEL do:
 
 ```shell
 $ sudo yum install python-debuginfo
 ```
 
 Other distros, like Arch Linux, do not provide debugging symbols in the package repos. In this case,
-you would need to build CPython from source. Please refer to official [CPython](https://devguide.python.org/setup/#compiling)
-or [distro](https://wiki.archlinux.org/index.php/Debug_-_Getting_Traces) docs for instructions.
+you would need to build CPython from source. Please refer to the official [CPython](https://devguide.python.org/setup/#compiling)
+or [distro](https://wiki.archlinux.org/index.php/Debug_-_Getting_Traces) documentation for instructions.
 
-Alternatively, you can use official CPython [Docker images](https://hub.docker.com/_/python).
+Alternatively, you can use the official CPython [Docker images](https://hub.docker.com/_/python).
 
 
 Broken LLDB scripting
 ---------------------
 
-Some Linux distros (most notably Debian Stretch) are shipped with a version of LLDB in which Python scripting
+Some Linux distros (notably Debian Stretch) are shipped with a version of LLDB in which using Python scripting
 triggers a segmentation fault when executing any non-trivial operation:
 
 ```shell
 $ lldb
 (lldb) script
 Python Interactive Interpreter. To exit, type 'quit()', 'exit()' or Ctrl-D.
 >>> import io
 >>> Segmentation fault
 ```
 
 It's recommended that you use the latest LLDB release from the official [APT repo](https://apt.llvm.org/) instead
 of the one shipped with your distro.
 
-See this [page](https://github.com/vadimcn/vscode-lldb/wiki/Troubleshooting) for advice on
-troubleshooting of LLDB.
+See this [page](https://github.com/vadimcn/vscode-lldb/wiki/Troubleshooting) for advice on troubleshooting LLDB.
 
 Development
 ===========
 
 Running tests
 -------------
```

