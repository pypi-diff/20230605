# Comparing `tmp/tex-fast-recompile-0.5.0.tar.gz` & `tmp/tex-fast-recompile-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tex-fast-recompile-0.5.0.tar", last modified: Mon Jun  5 15:52:28 2023, max compression
+gzip compressed data, was "tex-fast-recompile-0.5.1.tar", last modified: Mon Jun  5 16:24:47 2023, max compression
```

## Comparing `tex-fast-recompile-0.5.0.tar` & `tex-fast-recompile-0.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-05 15:52:28.104654 tex-fast-recompile-0.5.0/
--rw-r--r--   0 user202729  (1000) user202729  (1000)     1799 2023-01-12 16:09:27.000000 tex-fast-recompile-0.5.0/.gitignore
--rw-r--r--   0 user202729  (1000) user202729  (1000)    19105 2023-01-12 16:09:42.000000 tex-fast-recompile-0.5.0/LICENSE
--rw-r--r--   0 user202729  (1000) user202729  (1000)     6678 2023-06-05 15:52:28.104654 tex-fast-recompile-0.5.0/PKG-INFO
--rw-r--r--   0 user202729  (1000) user202729  (1000)     6214 2023-06-02 05:25:15.000000 tex-fast-recompile-0.5.0/README.md
--rw-r--r--   0 user202729  (1000) user202729  (1000)       45 2023-06-02 08:06:52.000000 tex-fast-recompile-0.5.0/pytest.ini
--rw-r--r--   0 user202729  (1000) user202729  (1000)        9 2023-01-12 17:26:41.000000 tex-fast-recompile-0.5.0/requirements.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)      738 2023-06-05 15:52:28.104654 tex-fast-recompile-0.5.0/setup.cfg
--rw-r--r--   0 user202729  (1000) user202729  (1000)       63 2023-01-12 16:30:18.000000 tex-fast-recompile-0.5.0/setup.py
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-05 15:52:28.101321 tex-fast-recompile-0.5.0/tests/
--rw-r--r--   0 user202729  (1000) user202729  (1000)     4168 2023-06-05 15:49:12.000000 tex-fast-recompile-0.5.0/tests/test_main.py
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-05 15:52:28.101321 tex-fast-recompile-0.5.0/tex/
--rw-r--r--   0 user202729  (1000) user202729  (1000)     4033 2023-06-02 07:59:36.000000 tex-fast-recompile-0.5.0/tex/fastrecompile.sty
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-05 15:52:28.101321 tex-fast-recompile-0.5.0/tex_fast_recompile/
--rw-r--r--   0 user202729  (1000) user202729  (1000)        0 2023-06-02 08:06:32.000000 tex-fast-recompile-0.5.0/tex_fast_recompile/__init__.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)    21472 2023-06-05 15:49:11.000000 tex-fast-recompile-0.5.0/tex_fast_recompile/__main__.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)     4113 2023-02-07 16:26:44.000000 tex-fast-recompile-0.5.0/tex_fast_recompile/latexmk.py
--rw-r--r--   0 user202729  (1000) user202729  (1000)        0 2023-01-12 16:30:32.000000 tex-fast-recompile-0.5.0/tex_fast_recompile/py.typed
--rw-r--r--   0 user202729  (1000) user202729  (1000)     1163 2023-06-02 08:39:53.000000 tex-fast-recompile-0.5.0/tex_fast_recompile/util.py
-drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-05 15:52:28.104654 tex-fast-recompile-0.5.0/tex_fast_recompile.egg-info/
--rw-r--r--   0 user202729  (1000) user202729  (1000)     6678 2023-06-05 15:52:27.000000 tex-fast-recompile-0.5.0/tex_fast_recompile.egg-info/PKG-INFO
--rw-r--r--   0 user202729  (1000) user202729  (1000)      517 2023-06-05 15:52:27.000000 tex-fast-recompile-0.5.0/tex_fast_recompile.egg-info/SOURCES.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)        1 2023-06-05 15:52:27.000000 tex-fast-recompile-0.5.0/tex_fast_recompile.egg-info/dependency_links.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)      133 2023-06-05 15:52:27.000000 tex-fast-recompile-0.5.0/tex_fast_recompile.egg-info/entry_points.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)       30 2023-06-05 15:52:27.000000 tex-fast-recompile-0.5.0/tex_fast_recompile.egg-info/requires.txt
--rw-r--r--   0 user202729  (1000) user202729  (1000)       19 2023-06-05 15:52:27.000000 tex-fast-recompile-0.5.0/tex_fast_recompile.egg-info/top_level.txt
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-05 16:24:47.348035 tex-fast-recompile-0.5.1/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1799 2023-01-12 16:09:27.000000 tex-fast-recompile-0.5.1/.gitignore
+-rw-r--r--   0 user202729  (1000) user202729  (1000)    19105 2023-01-12 16:09:42.000000 tex-fast-recompile-0.5.1/LICENSE
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     6678 2023-06-05 16:24:47.348035 tex-fast-recompile-0.5.1/PKG-INFO
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     6214 2023-06-02 05:25:15.000000 tex-fast-recompile-0.5.1/README.md
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       45 2023-06-02 08:06:52.000000 tex-fast-recompile-0.5.1/pytest.ini
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        9 2023-01-12 17:26:41.000000 tex-fast-recompile-0.5.1/requirements.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      738 2023-06-05 16:24:47.351368 tex-fast-recompile-0.5.1/setup.cfg
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       63 2023-01-12 16:30:18.000000 tex-fast-recompile-0.5.1/setup.py
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-05 16:24:47.344702 tex-fast-recompile-0.5.1/tests/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     5205 2023-06-05 16:22:47.000000 tex-fast-recompile-0.5.1/tests/test_main.py
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-05 16:24:47.344702 tex-fast-recompile-0.5.1/tex/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     4033 2023-06-02 07:59:36.000000 tex-fast-recompile-0.5.1/tex/fastrecompile.sty
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-05 16:24:47.348035 tex-fast-recompile-0.5.1/tex_fast_recompile/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        0 2023-06-02 08:06:32.000000 tex-fast-recompile-0.5.1/tex_fast_recompile/__init__.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)    21348 2023-06-05 16:23:08.000000 tex-fast-recompile-0.5.1/tex_fast_recompile/__main__.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     4113 2023-02-07 16:26:44.000000 tex-fast-recompile-0.5.1/tex_fast_recompile/latexmk.py
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        0 2023-01-12 16:30:32.000000 tex-fast-recompile-0.5.1/tex_fast_recompile/py.typed
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     1163 2023-06-02 08:39:53.000000 tex-fast-recompile-0.5.1/tex_fast_recompile/util.py
+drwxr-xr-x   0 user202729  (1000) user202729  (1000)        0 2023-06-05 16:24:47.348035 tex-fast-recompile-0.5.1/tex_fast_recompile.egg-info/
+-rw-r--r--   0 user202729  (1000) user202729  (1000)     6678 2023-06-05 16:24:46.000000 tex-fast-recompile-0.5.1/tex_fast_recompile.egg-info/PKG-INFO
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      517 2023-06-05 16:24:47.000000 tex-fast-recompile-0.5.1/tex_fast_recompile.egg-info/SOURCES.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)        1 2023-06-05 16:24:46.000000 tex-fast-recompile-0.5.1/tex_fast_recompile.egg-info/dependency_links.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)      133 2023-06-05 16:24:46.000000 tex-fast-recompile-0.5.1/tex_fast_recompile.egg-info/entry_points.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       30 2023-06-05 16:24:46.000000 tex-fast-recompile-0.5.1/tex_fast_recompile.egg-info/requires.txt
+-rw-r--r--   0 user202729  (1000) user202729  (1000)       19 2023-06-05 16:24:46.000000 tex-fast-recompile-0.5.1/tex_fast_recompile.egg-info/top_level.txt
```

### Comparing `tex-fast-recompile-0.5.0/.gitignore` & `tex-fast-recompile-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tex-fast-recompile-0.5.0/LICENSE` & `tex-fast-recompile-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tex-fast-recompile-0.5.0/PKG-INFO` & `tex-fast-recompile-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tex-fast-recompile
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Python module to speed up TeX compilation.
 Home-page: https://github.com/user202729/tex-fast-recompile
 Author: user202729
 License: LPPL 1.3c
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tex-fast-recompile-0.5.0/README.md` & `tex-fast-recompile-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `tex-fast-recompile-0.5.0/setup.cfg` & `tex-fast-recompile-0.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tex-fast-recompile
-version = 0.5.0
+version = 0.5.1
 author = user202729
 description = A Python module to speed up TeX compilation.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = LPPL 1.3c
 url = https://github.com/user202729/tex-fast-recompile
 classifiers =
```

### Comparing `tex-fast-recompile-0.5.0/tests/test_main.py` & `tex-fast-recompile-0.5.1/tests/test_main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 from threading import Timer
 import sys
 import pytest
 from pathlib import Path
 import textwrap
 import subprocess
 from typing import Callable
+import time
+import psutil  # type: ignore
 
 LinePredicate=Callable[[str], bool]
 line_predicates: list[LinePredicate]=[]
 
 def ensure_print_lines(process: subprocess.Popen, expects: list[LinePredicate], kill: bool=True)->None:
 	timer=Timer(1, process.kill)
 	timer.start()
 	expects=expects[::-1]
 	assert process.stdout is not None
+	collected_lines=[]
 	for line in process.stdout:
+		collected_lines.append(line)
 		waiting_for=expects[-1]
 
 		assert waiting_for in line_predicates
 		for remaining in line_predicates:
 			if remaining!=waiting_for: assert not remaining(line), f"Unexpected line {line}"
 
 		if waiting_for(line):
 			expects.pop()
 			if not expects: break
 	else:
 		if not timer.is_alive():
-			assert False, "Timeout without seeing some lines"
+			assert False, f"Timeout without seeing some lines -- seen lines are {collected_lines}"
 		assert False, "Process exit voluntarily but some expected lines are never seen??"
 	timer.cancel()
 	if kill:
 		process.kill()
 
 
 def possible_line_content(f: LinePredicate)->LinePredicate:
@@ -45,14 +49,17 @@
 def expect_success(line: str)->bool:
 	return "========success" in line
 
 @possible_line_content
 def expect_rerunning(line: str)->bool:
 	return "Rerunning" in line
 
+@possible_line_content
+def expect_preamble_changed(line: str)->bool:
+	return "Preamble changed" in line
 
 
 
 def ensure_pdf_content_file(file: Path, content: str)->None:
 	txt_file=file.with_suffix(".txt")
 	pdf_file=file.with_suffix(".pdf")
 	txt_file.unlink(missing_ok=True)
@@ -136,13 +143,41 @@
 			\end{document}
 			""",
 			filename=filename+".tex",
 			extra_args=["--temp-output-directory"] if temp_output_directory else [],
 			)
 	if not valid:
 		process.wait(timeout=2)
+		assert process.stderr
 		assert "AssertionError" in process.stderr.read()
 		return
 	ensure_print_lines(process, [expect_success])
 	process.kill()
 	ensure_pdf_content_file(tmp_path/"output"/(filename+".pdf"), "helloworld")
 
+def test_subprocess_killed_on_preamble_change(tmp_path: Path)->None:
+	file, process=prepare_process(tmp_path, r"""
+	\documentclass{article}
+	\begin{document}
+	helloworld
+	\end{document}
+	""")
+	ensure_print_lines(process, [expect_success], kill=False)
+
+	time.sleep(1)
+	assert count_child_processes(process)==1
+
+	file.write_text(textwrap.dedent(r"""
+	\documentclass{article}
+	\usepackage{amsmath}
+	\begin{document}
+	helloworld
+	\end{document}
+	"""))
+	ensure_print_lines(process, [expect_preamble_changed, expect_success], kill=False)
+	time.sleep(1)
+	assert count_child_processes(process)==1  # if this is 2 then there's the resource leak
+	process.kill()
+
+def count_child_processes(process: subprocess.Popen)->int:
+	return len(psutil.Process(process.pid).children(recursive=True))
+
```

### Comparing `tex-fast-recompile-0.5.0/tex/fastrecompile.sty` & `tex-fast-recompile-0.5.1/tex/fastrecompile.sty`

 * *Files identical despite different names*

### Comparing `tex-fast-recompile-0.5.0/tex_fast_recompile/__main__.py` & `tex-fast-recompile-0.5.1/tex_fast_recompile/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,28 +198,29 @@
 		command+=self.extra_args
 		if self.mylatexformat_status is MyLatexFormatStatus.precompile: command.append("&"+self.executable)
 		elif self.mylatexformat_status is MyLatexFormatStatus.use: command.append("&"+self.jobname)
 		command.append(compiling_filename)
 		command+=self.extra_commands
 
 		process=subprocess.Popen(command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, env=self.env)
-		self._process: Optional[subprocess.Popen[bytes]]=process
+		self._process: subprocess.Popen[bytes]=process
 		assert process.stdin is not None
 
 		self._copy_stdout_thread: Optional[threading.Thread]=None
+		self._finished=False
 
 	def finish(self)->bool:
 		"""
 		Returns whether the compiler returns 0.
 		Note that it's possible for the compiler to return 0 and yet the compilation failed, if no PDF is generated.
 		"""
-		process=self._process
-		assert process is not None
-		self._process=None
+		assert not self._finished
+		self._finished=True
 
+		process=self._process
 		# check if the preamble is still the same
 		if self._preamble_at_start!=extract_preamble(Path(self.filename).read_text(encoding='u8')):
 			raise PreambleChangedError()
 
 		if self.mylatexformat_status is MyLatexFormatStatus.precompile:
 			# don't need to send extra line, finish is finish
 			process.wait()
@@ -240,15 +241,14 @@
 
 		self.compiling_callback()
 
 		# start a new thread to copy process stdout to sys.stdout
 		# the copy should be done such that partially-written lines get copied immediately when they're written
 		def copy_stdout_work()->None:
 			while True:
-				assert process is not None
 				assert process.stdout is not None
 				# this is a bit inefficient in that it reads one byte at a time
 				# but I don't know how to do it better
 				content=process.stdout.read(1)
 				if content==b"":
 					break
 				sys.stdout.buffer.write(content)
@@ -258,16 +258,15 @@
 
 		# wait for the process to finish
 		process.wait()
 
 		return process.returncode==0
 
 	def __exit__(self, exc_type, exc_value, traceback)->None:
-		if self._process is not None:
-			self._process.kill()  # may happen if the user send KeyboardInterrupt or the preamble changed
+		self._process.kill()
 		if self._copy_stdout_thread is not None:
 			self._copy_stdout_thread.join()
 
 tmpdir=Path(tempfile.gettempdir())/".tex-fast-recompile-tmp"
 tmpdir.mkdir(parents=True, exist_ok=True)
```

### Comparing `tex-fast-recompile-0.5.0/tex_fast_recompile/latexmk.py` & `tex-fast-recompile-0.5.1/tex_fast_recompile/latexmk.py`

 * *Files identical despite different names*

### Comparing `tex-fast-recompile-0.5.0/tex_fast_recompile/util.py` & `tex-fast-recompile-0.5.1/tex_fast_recompile/util.py`

 * *Files identical despite different names*

### Comparing `tex-fast-recompile-0.5.0/tex_fast_recompile.egg-info/PKG-INFO` & `tex-fast-recompile-0.5.1/tex_fast_recompile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tex-fast-recompile
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Python module to speed up TeX compilation.
 Home-page: https://github.com/user202729/tex-fast-recompile
 Author: user202729
 License: LPPL 1.3c
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tex-fast-recompile-0.5.0/tex_fast_recompile.egg-info/SOURCES.txt` & `tex-fast-recompile-0.5.1/tex_fast_recompile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

