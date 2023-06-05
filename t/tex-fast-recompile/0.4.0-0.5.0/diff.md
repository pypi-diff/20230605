# Comparing `tmp/tex-fast-recompile-0.4.0.tar.gz` & `tmp/tex-fast-recompile-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tex-fast-recompile-0.4.0.tar", last modified: Sun Jan 15 05:09:11 2023, max compression
+gzip compressed data, was "tex-fast-recompile-0.5.0.tar", last modified: Mon Jun  5 15:52:28 2023, max compression
```

## Comparing `tex-fast-recompile-0.4.0.tar` & `tex-fast-recompile-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-01-15 05:09:11.228809 tex-fast-recompile-0.4.0/
--rw-r--r--   0 user202729  (1000) user202729  (1000)     1799 2023-01-12 16:09:27.000000 tex-fast-recompile-0.4.0/.gitignore
--rw-r--r--   0 user202729  (1000) user202729  (1000)    19105 2023-01-12 16:09:42.000000 tex-fast-recompile-0.4.0/LICENSE
--rw-r--r--   0 user202729  (1000) user202729  (1000)     4819 2023-01-15 05:09:11.228809 tex-fast-recompile-0.4.0/PKG-INFO
--rw-r--r--   0 user202729  (1000) user202729  (1000)     4355 2023-01-15 05:08:38.000000 tex-fast-recompile-0.4.0/README.md
--rw-r--r--   0 user202729  (1000) user202729  (1000)        9 2023-01-12 17:26:41.000000 tex-fast-recompile-0.4.0/requirements.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)      723 2023-01-15 05:09:11.228809 tex-fast-recompile-0.4.0/setup.cfg
--rw-r--r--   0 user202729  (1000) user202729  (1000)       63 2023-01-12 16:30:18.000000 tex-fast-recompile-0.4.0/setup.py
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-01-15 05:09:11.225476 tex-fast-recompile-0.4.0/tex/
--rw-r--r--   0 user202729  (1000) user202729  (1000)     2264 2023-01-12 17:45:49.000000 tex-fast-recompile-0.4.0/tex/fastrecompile.sty
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-01-15 05:09:11.225476 tex-fast-recompile-0.4.0/tex_fast_recompile/
--rw-r--r--   0 user202729  (1000) user202729  (1000)    11236 2023-01-15 05:05:10.000000 tex-fast-recompile-0.4.0/tex_fast_recompile/__main__.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)     4088 2023-01-15 05:00:32.000000 tex-fast-recompile-0.4.0/tex_fast_recompile/latexmk.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)        0 2023-01-12 16:30:32.000000 tex-fast-recompile-0.4.0/tex_fast_recompile/py.typed
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-01-15 05:09:11.228809 tex-fast-recompile-0.4.0/tex_fast_recompile.egg-info/
--rw-r--r--   0 user202729  (1000) user202729  (1000)     4819 2023-01-15 05:09:11.000000 tex-fast-recompile-0.4.0/tex_fast_recompile.egg-info/PKG-INFO
--rw-r--r--   0 user202729  (1000) user202729  (1000)      429 2023-01-15 05:09:11.000000 tex-fast-recompile-0.4.0/tex_fast_recompile.egg-info/SOURCES.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)        1 2023-01-15 05:09:11.000000 tex-fast-recompile-0.4.0/tex_fast_recompile.egg-info/dependency_links.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)      133 2023-01-15 05:09:11.000000 tex-fast-recompile-0.4.0/tex_fast_recompile.egg-info/entry_points.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)       16 2023-01-15 05:09:11.000000 tex-fast-recompile-0.4.0/tex_fast_recompile.egg-info/requires.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)       19 2023-01-15 05:09:11.000000 tex-fast-recompile-0.4.0/tex_fast_recompile.egg-info/top_level.txt
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-05 15:52:28.104654 tex-fast-recompile-0.5.0/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1799 2023-01-12 16:09:27.000000 tex-fast-recompile-0.5.0/.gitignore
+-rw-r--r--   0 user202729  (1000) user202729  (1000)    19105 2023-01-12 16:09:42.000000 tex-fast-recompile-0.5.0/LICENSE
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     6678 2023-06-05 15:52:28.104654 tex-fast-recompile-0.5.0/PKG-INFO
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     6214 2023-06-02 05:25:15.000000 tex-fast-recompile-0.5.0/README.md
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       45 2023-06-02 08:06:52.000000 tex-fast-recompile-0.5.0/pytest.ini
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        9 2023-01-12 17:26:41.000000 tex-fast-recompile-0.5.0/requirements.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      738 2023-06-05 15:52:28.104654 tex-fast-recompile-0.5.0/setup.cfg
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       63 2023-01-12 16:30:18.000000 tex-fast-recompile-0.5.0/setup.py
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-05 15:52:28.101321 tex-fast-recompile-0.5.0/tests/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     4168 2023-06-05 15:49:12.000000 tex-fast-recompile-0.5.0/tests/test_main.py
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-05 15:52:28.101321 tex-fast-recompile-0.5.0/tex/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     4033 2023-06-02 07:59:36.000000 tex-fast-recompile-0.5.0/tex/fastrecompile.sty
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-05 15:52:28.101321 tex-fast-recompile-0.5.0/tex_fast_recompile/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        0 2023-06-02 08:06:32.000000 tex-fast-recompile-0.5.0/tex_fast_recompile/__init__.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)    21472 2023-06-05 15:49:11.000000 tex-fast-recompile-0.5.0/tex_fast_recompile/__main__.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     4113 2023-02-07 16:26:44.000000 tex-fast-recompile-0.5.0/tex_fast_recompile/latexmk.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        0 2023-01-12 16:30:32.000000 tex-fast-recompile-0.5.0/tex_fast_recompile/py.typed
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1163 2023-06-02 08:39:53.000000 tex-fast-recompile-0.5.0/tex_fast_recompile/util.py
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-05 15:52:28.104654 tex-fast-recompile-0.5.0/tex_fast_recompile.egg-info/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     6678 2023-06-05 15:52:27.000000 tex-fast-recompile-0.5.0/tex_fast_recompile.egg-info/PKG-INFO
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      517 2023-06-05 15:52:27.000000 tex-fast-recompile-0.5.0/tex_fast_recompile.egg-info/SOURCES.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        1 2023-06-05 15:52:27.000000 tex-fast-recompile-0.5.0/tex_fast_recompile.egg-info/dependency_links.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      133 2023-06-05 15:52:27.000000 tex-fast-recompile-0.5.0/tex_fast_recompile.egg-info/entry_points.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       30 2023-06-05 15:52:27.000000 tex-fast-recompile-0.5.0/tex_fast_recompile.egg-info/requires.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       19 2023-06-05 15:52:27.000000 tex-fast-recompile-0.5.0/tex_fast_recompile.egg-info/top_level.txt
```

### Comparing `tex-fast-recompile-0.4.0/.gitignore` & `tex-fast-recompile-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tex-fast-recompile-0.4.0/LICENSE` & `tex-fast-recompile-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tex-fast-recompile-0.4.0/PKG-INFO` & `tex-fast-recompile-0.5.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: tex-fast-recompile
-Version: 0.4.0
-Summary: A Python module to speed up TeX compilation.
-Home-page: https://github.com/user202729/tex-fast-recompile
-Author: user202729
-License: LPPL 1.3c
-Classifier: License :: OSI Approved
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Text Processing :: Markup :: LaTeX
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # tex-fast-recompile
 
 A Python module to speed up TeX compilation.
 
 This is similar to the [`mylatexformat` TeX package](https://ctan.org/pkg/mylatexformat) that it works by "speed up" some "preamble",
 but unlike using "precompiled preamble" i.e. custom TeX format,
 this package works with *every* package including package that executes some Lua code, or load OpenType font.
@@ -28,17 +14,22 @@
 * https://github.com/user202729/tex-fast-recompile
 
 You also need to install the helper TeX package `fastrecompile.sty`, which can be found in the `tex/` directory.
 Refer to https://tex.stackexchange.com/q/1137/250119 for installation instruction.
 
 (currently the TeX package is not available on CTAN)
 
-
 ## Usage
 
+### Note for Vim users
+
+If update performance appears slow, try disabling `writebackup`, or set `backupcopy=yes`.
+(this issue happened once for me, and I haven't been able to reproduce it so far. Alternatively just try
+restarting your computer.)
+
 ### Normal mode
 
 If installed properly, an executable `tex_fast_recompile` should be available on your command-line.
 
 Run `tex_fast_recompile --help` to view the available options.
 
 For example you can use it as follows:
@@ -50,33 +41,69 @@
 to compile `a.tex` to `a.pdf` and automatically watch it on changes.
 
 Usually prepending it to your LaTeX compilation command suffices.
 
 ### LaTeXmk emulation mode
 
 For compatibility with e.g. `vimtex` plugin, an executable `tex_fast_recompile_latexmk` is provided, which takes arguments similar to that of `latexmk`.
-(but it does not do multiple compilation passes or invoke bibliography/indexing commands etc., and the simulation might not be complete)
+(but it does not invoke bibliography/indexing commands/automatically detect changes to dependent files etc., and the simulation might not be complete)
 
 Run `tex_fast_recompile_latexmk --help` to view the available options. (should be similar to `latexmk`'s accepted options)
 
 For VimTeX usage, putting the following configuration in `.vimrc` usually suffices:
 
 ```vim
-let g:vimtex_compiler_method='latexmk'
 let g:vimtex_compiler_latexmk = { 'executable' : 'tex_fast_recompile_latexmk' }
 ```
 
 ## Limitations
 
+* If VimTeX is used, the latexmk (emulation) is forcefully killed when compilation stops.
+In that case, the temporary directory is not cleaned, and over time it may clutter the temporary directory.
+
+  (this has a partial workaround, that is new process spawned will clean up previous process' temporary directories)
 * Any file `\input` in the preamble must not be changed. (when the preamble changes, the program will automatically detect that)
 * You must not read from the terminal anywhere in the preamble, such as with functions `\read -1 to ...` or `\ior_get_term:nN ...`.
 (if you're not sure what this mean, you should be safe)
+* The latexmk emulation mode does not necessarily recompile the file sufficiently many times when references changed.
+(as such it might be convenient to use `silence` package to suppress the `rerunfilecheck` warnings
+such as:
+
+```latex
+\WarningFilter{latex}{Reference `}
+\WarningFilter{latex}{Citation `}
+\WarningFilter{latex}{There were undefined references}
+\WarningFilter{latex}{Label(s) may have changed}
+\WarningFilter{rerunfilecheck}{}
+```
+
+While the first filter may be overly broad, for the purpose of fast preview it isn't too important.)
 
 ## Advanced notes
 
+### Explicitly specify preamble ending location
+
+You can put `\fastrecompileendpreamble` on a single line to mark the end of the "fixed preamble" part.
+
+Or equivalently, `\csname fastrecompileendpreamble\endcsname` (note that there must be no space before the `\endcsname`) --
+this is the same as above, but will just silently do nothing instead of complaining about `\fastrecompileendpreamble` being not defined
+if this program is not used.
+
+Note that:
+
+* `\fastrecompileendpreamble` must appear at most once in the *main* file.
+* There must be nothing else on the line that contains `\fastrecompileendpreamble`.
+* SyncTeX features of the text part in the "preamble" may not be correct.
+
+Normally, this is assumed to be right before the `\begin{document}` line (or `\AtEndPreamble`),
+but if you either
+* use the `--copy-output` option (and only read the copied output), or
+* there's no package that outputs something at the start of the document (such as `hyperref`),
+then you can move the `\fastrecompileendpreamble` to after the `\begin{document}` line.
+
 ### Extra note
 
 If you want to read the log file, refer to the help of `--copy-log` option.
 
 It's possible to print out some content in the "preamble" part, but if you do so...
 
 ```tex
@@ -91,42 +118,21 @@
 456
 
 \end{document}
 ```
 
 you must also use the `--copy-output` option if you want to view the resulting PDF.
 
-### `--no-add-package` mode
-
-Behind the scene, some magic is done on your TeX file.
+### Internal note
 
-If you want to do that manually, you need to modify your TeX file as follows:
-
-```tex
-\documentclass{article}
-\usepackage{fastrecompile}  % manually add the package here
-% other preamble lines...
-\begin{document}
-
-% put the line below where the preamble ends:
-\fastrecompileendpreamble
-
-...
-
-\end{document}
-```
-
-then compile your document with `--no-add-package` flag added.
-
-Note that:
-
-* `\fastrecompileendpreamble` must appear exactly once in the *main* file.
-* There must be nothing else on the line that contains `\fastrecompileendpreamble`.
-* SyncTeX features of the text part in the "preamble" may not be correct.
+The module used to create a temporary file instead of `\input` the original file with `begindocument/end` hook,
+but with the `--recorder` flag then `\currfileabspath` will be wrong in the preamble,
+and `@@input` does not update the file name when the actual file is `\input`-ed.
 
+With the handler moved to `\AtEndPreamble` instead of `\AtBeginDocument` there are some spurious messages... (not critical)
 
 ### How does it work?
 
 The principle is very simple. Notice that while the user want fast refresh, the file does not change very frequently.
 
 As such, we start the compiler _before_ the file has changed to process the "preamble", then when the file changed we
 continue processing the rest of the file.
```

### Comparing `tex-fast-recompile-0.4.0/setup.cfg` & `tex-fast-recompile-0.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tex-fast-recompile
-version = 0.4.0
+version = 0.5.0
 author = user202729
 description = A Python module to speed up TeX compilation.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = LPPL 1.3c
 url = https://github.com/user202729/tex-fast-recompile
 classifiers = 
@@ -13,14 +13,15 @@
 	Programming Language :: Python :: 3
 	Topic :: Text Processing :: Markup :: LaTeX
 
 [options]
 packages = tex_fast_recompile
 install_requires = 
 	watchdog~=2.1.2
+	psutil~=5.9.4
 
 [options.entry_points]
 console_scripts = 
 	tex_fast_recompile = tex_fast_recompile.__main__:main
 	tex_fast_recompile_latexmk = tex_fast_recompile.latexmk:main
 
 [egg_info]
```

### Comparing `tex-fast-recompile-0.4.0/tex_fast_recompile/latexmk.py` & `tex-fast-recompile-0.5.0/tex_fast_recompile/latexmk.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,17 +55,17 @@
 		need to handle the following
 
 		"$compiling_cmd = ($compiling_cmd ? $compiling_cmd . " ; " : "") . "echo vimtex_compiler_callback_compiling""
 		"$success_cmd = ($success_cmd ? $success_cmd . " ; " : "") . "echo vimtex_compiler_callback_success""
 		"$failure_cmd = ($failure_cmd ? $failure_cmd . " ; " : "") . "echo vimtex_compiler_callback_failure""
 		"""
 		for part_before, part_after, arg_name in (
-				('$compiling_cmd = ($compiling_cmd ? $compiling_cmd . " ; " : "") . "', '"', None),
-				('$success_cmd = ($success_cmd ? $success_cmd . " ; " : "") . "', '"', "--success-cmd"),
-				('$failure_cmd = ($failure_cmd ? $failure_cmd . " ; " : "") . "', '"', "--failure-cmd"),
+				('$compiling_cmd = ($compiling_cmd ? $compiling_cmd . " ; " : "") . "', '"', "--compiling-cmd"),
+				('$success_cmd = ($success_cmd ? $success_cmd . " ; " : "") . "',       '"', "--success-cmd"),
+				('$failure_cmd = ($failure_cmd ? $failure_cmd . " ; " : "") . "',       '"', "--failure-cmd"),
 				):
 			if arg.startswith(part_before) and arg.endswith(part_after):
 				if arg_name is not None:
 					tex_fast_recompile_args.append(f"{arg_name}={arg[len(part_before):-len(part_after)]}")
 				break
 		else:
 			raise ValueError(f"Unknown argument -e {arg}")
```

### Comparing `tex-fast-recompile-0.4.0/tex_fast_recompile.egg-info/PKG-INFO` & `tex-fast-recompile-0.5.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tex-fast-recompile
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python module to speed up TeX compilation.
 Home-page: https://github.com/user202729/tex-fast-recompile
 Author: user202729
 License: LPPL 1.3c
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -28,17 +28,22 @@
 * https://github.com/user202729/tex-fast-recompile
 
 You also need to install the helper TeX package `fastrecompile.sty`, which can be found in the `tex/` directory.
 Refer to https://tex.stackexchange.com/q/1137/250119 for installation instruction.
 
 (currently the TeX package is not available on CTAN)
 
-
 ## Usage
 
+### Note for Vim users
+
+If update performance appears slow, try disabling `writebackup`, or set `backupcopy=yes`.
+(this issue happened once for me, and I haven't been able to reproduce it so far. Alternatively just try
+restarting your computer.)
+
 ### Normal mode
 
 If installed properly, an executable `tex_fast_recompile` should be available on your command-line.
 
 Run `tex_fast_recompile --help` to view the available options.
 
 For example you can use it as follows:
@@ -50,33 +55,69 @@
 to compile `a.tex` to `a.pdf` and automatically watch it on changes.
 
 Usually prepending it to your LaTeX compilation command suffices.
 
 ### LaTeXmk emulation mode
 
 For compatibility with e.g. `vimtex` plugin, an executable `tex_fast_recompile_latexmk` is provided, which takes arguments similar to that of `latexmk`.
-(but it does not do multiple compilation passes or invoke bibliography/indexing commands etc., and the simulation might not be complete)
+(but it does not invoke bibliography/indexing commands/automatically detect changes to dependent files etc., and the simulation might not be complete)
 
 Run `tex_fast_recompile_latexmk --help` to view the available options. (should be similar to `latexmk`'s accepted options)
 
 For VimTeX usage, putting the following configuration in `.vimrc` usually suffices:
 
 ```vim
-let g:vimtex_compiler_method='latexmk'
 let g:vimtex_compiler_latexmk = { 'executable' : 'tex_fast_recompile_latexmk' }
 ```
 
 ## Limitations
 
+* If VimTeX is used, the latexmk (emulation) is forcefully killed when compilation stops.
+In that case, the temporary directory is not cleaned, and over time it may clutter the temporary directory.
+
+  (this has a partial workaround, that is new process spawned will clean up previous process' temporary directories)
 * Any file `\input` in the preamble must not be changed. (when the preamble changes, the program will automatically detect that)
 * You must not read from the terminal anywhere in the preamble, such as with functions `\read -1 to ...` or `\ior_get_term:nN ...`.
 (if you're not sure what this mean, you should be safe)
+* The latexmk emulation mode does not necessarily recompile the file sufficiently many times when references changed.
+(as such it might be convenient to use `silence` package to suppress the `rerunfilecheck` warnings
+such as:
+
+```latex
+\WarningFilter{latex}{Reference `}
+\WarningFilter{latex}{Citation `}
+\WarningFilter{latex}{There were undefined references}
+\WarningFilter{latex}{Label(s) may have changed}
+\WarningFilter{rerunfilecheck}{}
+```
+
+While the first filter may be overly broad, for the purpose of fast preview it isn't too important.)
 
 ## Advanced notes
 
+### Explicitly specify preamble ending location
+
+You can put `\fastrecompileendpreamble` on a single line to mark the end of the "fixed preamble" part.
+
+Or equivalently, `\csname fastrecompileendpreamble\endcsname` (note that there must be no space before the `\endcsname`) --
+this is the same as above, but will just silently do nothing instead of complaining about `\fastrecompileendpreamble` being not defined
+if this program is not used.
+
+Note that:
+
+* `\fastrecompileendpreamble` must appear at most once in the *main* file.
+* There must be nothing else on the line that contains `\fastrecompileendpreamble`.
+* SyncTeX features of the text part in the "preamble" may not be correct.
+
+Normally, this is assumed to be right before the `\begin{document}` line (or `\AtEndPreamble`),
+but if you either
+* use the `--copy-output` option (and only read the copied output), or
+* there's no package that outputs something at the start of the document (such as `hyperref`),
+then you can move the `\fastrecompileendpreamble` to after the `\begin{document}` line.
+
 ### Extra note
 
 If you want to read the log file, refer to the help of `--copy-log` option.
 
 It's possible to print out some content in the "preamble" part, but if you do so...
 
 ```tex
@@ -91,42 +132,21 @@
 456
 
 \end{document}
 ```
 
 you must also use the `--copy-output` option if you want to view the resulting PDF.
 
-### `--no-add-package` mode
-
-Behind the scene, some magic is done on your TeX file.
-
-If you want to do that manually, you need to modify your TeX file as follows:
+### Internal note
 
-```tex
-\documentclass{article}
-\usepackage{fastrecompile}  % manually add the package here
-% other preamble lines...
-\begin{document}
-
-% put the line below where the preamble ends:
-\fastrecompileendpreamble
-
-...
-
-\end{document}
-```
-
-then compile your document with `--no-add-package` flag added.
-
-Note that:
-
-* `\fastrecompileendpreamble` must appear exactly once in the *main* file.
-* There must be nothing else on the line that contains `\fastrecompileendpreamble`.
-* SyncTeX features of the text part in the "preamble" may not be correct.
+The module used to create a temporary file instead of `\input` the original file with `begindocument/end` hook,
+but with the `--recorder` flag then `\currfileabspath` will be wrong in the preamble,
+and `@@input` does not update the file name when the actual file is `\input`-ed.
 
+With the handler moved to `\AtEndPreamble` instead of `\AtBeginDocument` there are some spurious messages... (not critical)
 
 ### How does it work?
 
 The principle is very simple. Notice that while the user want fast refresh, the file does not change very frequently.
 
 As such, we start the compiler _before_ the file has changed to process the "preamble", then when the file changed we
 continue processing the rest of the file.
```

