# Comparing `tmp/shell_gpt-0.9.1.tar.gz` & `tmp/shell_gpt-0.9.2.tar.gz`

## Comparing `shell_gpt-0.9.1.tar` & `shell_gpt-0.9.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/LICENSE
--rw-r--r--   0        0        0    19376 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/README.md
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/__main__.py
--rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/app.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/cache.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/client.py
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/config.py
--rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/role.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/handlers/__init__.py
--rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/handlers/chat_handler.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/handlers/default_handler.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/handlers/handler.py
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/handlers/repl_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/tests/__init__.py
--rw-r--r--   0        0        0    17250 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/tests/test_integration.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/tests/test_unit.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/LICENSE
--rw-r--r--   0        0        0    19376 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/README.md
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/pyproject.toml
--rw-r--r--   0        0        0    21403 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/LICENSE
+-rw-r--r--   0        0        0    20113 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/README.md
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/__main__.py
+-rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/app.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/cache.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/client.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/config.py
+-rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/role.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/handlers/__init__.py
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/handlers/chat_handler.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/handlers/default_handler.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/handlers/handler.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/handlers/repl_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/tests/__init__.py
+-rw-r--r--   0        0        0    17250 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/tests/test_integration.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/tests/test_unit.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/LICENSE
+-rw-r--r--   0        0        0    20113 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/README.md
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0    22140 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/PKG-INFO
```

### Comparing `shell_gpt-0.9.1/LICENSE` & `shell_gpt-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.1/README.md` & `shell_gpt-0.9.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ShellGPT
 A command-line productivity tool powered by OpenAI's GPT models. As developers, we can leverage AI capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort. ShellGPT is cross-platform compatible and supports all major operating systems, including Linux, macOS, and Windows with all major shells, such as PowerShell, CMD, Bash, Zsh, Fish, and many others.
 
 https://user-images.githubusercontent.com/16740832/231569156-a3a9f9d4-18b1-4fff-a6e1-6807651aa894.mp4
 
 ## Installation
 ```shell
-pip install shell-gpt==0.9.1
+pip install shell-gpt==0.9.2
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
@@ -88,14 +88,26 @@
 ls
 # -> 1.mp4 2.mp4 3.mp4
 sgpt -s "using ffmpeg combine multiple videos into one without audio. Video file names: $(ls -m)"
 # -> ffmpeg -i 1.mp4 -i 2.mp4 -i 3.mp4 -filter_complex "[0:v] [1:v] [2:v] concat=n=3:v=1 [v]" -map "[v]" out.mp4
 # -> [E]xecute, [D]escribe, [A]bort: e
 ...
 ```
+### Shell integration
+Shell integration allows you to use Shell-GPT in your terminal with hotkeys. It is currently available for bash and zsh. It will allow you to have sgpt completions in your shell history, and also edit suggested commands right away.
+
+https://github.com/TheR1D/shell_gpt/assets/16740832/bead0dab-0dd9-436d-88b7-6abfb2c556c1
+
+To install shell integration, run:
+```shell
+sgpt --install-integration
+# Restart your terminal to apply changes.
+```
+This will add few lines to your `.bashrc` or `.zshrc` file. After that, you can use `Ctrl+l` (by default) to invoke Shell-GPT. When you press `Ctrl+l` it will replace you current input line (buffer) with suggested command. You can then edit it and press `Enter` to execute.
+
 ### Generating code
 With `--code` parameters we can query only code as output, for example:
 ```shell
 sgpt --code "Solve classic fizz buzz problem using Python"
 ```
 ```python
 for i in range(1, 101):
```

### Comparing `shell_gpt-0.9.1/pyproject.toml` & `shell_gpt-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.1/sgpt/app.py` & `shell_gpt-0.9.2/sgpt/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,20 @@
 from click.types import Choice
 
 from sgpt.config import cfg
 from sgpt.handlers.chat_handler import ChatHandler
 from sgpt.handlers.default_handler import DefaultHandler
 from sgpt.handlers.repl_handler import ReplHandler
 from sgpt.role import DefaultRoles, SystemRole
-from sgpt.utils import ModelOptions, get_edited_prompt, run_command
+from sgpt.utils import (
+    ModelOptions,
+    get_edited_prompt,
+    install_shell_integration,
+    run_command,
+)
 
 
 def main(
     prompt: str = typer.Argument(
         None,
         show_default=False,
         help="The prompt to generate completions for.",
@@ -111,14 +116,20 @@
     ),
     list_roles: bool = typer.Option(
         False,
         help="List roles.",
         callback=SystemRole.list,
         rich_help_panel="Role Options",
     ),
+    install_integration: bool = typer.Option(
+        False,
+        help="Install shell integration (ZSH and Bash only)",
+        callback=install_shell_integration,
+        hidden=True,  # Hiding since should be used only once.
+    ),
 ) -> None:
     stdin_passed = not sys.stdin.isatty()
 
     if stdin_passed and not repl:
         prompt = f"{sys.stdin.read()}\n\n{prompt or ''}"
 
     if not prompt and not editor and not repl:
```

### Comparing `shell_gpt-0.9.1/sgpt/cache.py` & `shell_gpt-0.9.2/sgpt/cache.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.1/sgpt/client.py` & `shell_gpt-0.9.2/sgpt/client.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.1/sgpt/config.py` & `shell_gpt-0.9.2/sgpt/config.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.1/sgpt/role.py` & `shell_gpt-0.9.2/sgpt/role.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.1/sgpt/utils.py` & `shell_gpt-0.9.2/sgpt/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -61,7 +61,23 @@
     def wrapper(cls: Any, value: str) -> None:
         if not value:
             return
         func(cls, value)
         raise typer.Exit()
 
     return wrapper
+
+
+@option_callback
+def install_shell_integration(*_args: Any) -> None:
+    """
+    Installs shell integration. Currently only supports Linux.
+    Allows user to get shell completions in terminal by using hotkey.
+    Allows user to edit shell command right away in terminal.
+    """
+    # TODO: Add support for Windows.
+    # TODO: Implement updates.
+    if platform.system() == "Windows":
+        typer.echo("Windows is not supported yet.")
+    else:
+        url = "https://raw.githubusercontent.com/TheR1D/shell_gpt/shell-integrations/install.sh"
+        os.system(f'sh -c "$(curl -fsSL {url})"')
```

### Comparing `shell_gpt-0.9.1/sgpt/handlers/chat_handler.py` & `shell_gpt-0.9.2/sgpt/handlers/chat_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.1/sgpt/handlers/default_handler.py` & `shell_gpt-0.9.2/sgpt/handlers/default_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.1/sgpt/handlers/handler.py` & `shell_gpt-0.9.2/sgpt/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.1/sgpt/handlers/repl_handler.py` & `shell_gpt-0.9.2/sgpt/handlers/repl_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.1/tests/test_integration.py` & `shell_gpt-0.9.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.1/tests/test_unit.py` & `shell_gpt-0.9.2/tests/test_unit.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.1/PKG-INFO` & `shell_gpt-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell_gpt
-Version: 0.9.1
+Version: 0.9.2
 Summary: A command-line productivity tool powered by OpenAI GPT models, will help you accomplish your tasks faster and more efficiently.
 Project-URL: homepage, https://github.com/ther1d/shell_gpt
 Project-URL: repository, https://github.com/ther1d/shell_gpt
 Project-URL: documentation, https://github.com/TheR1D/shell_gpt/blob/main/README.md
 Author-email: Farkhod Sadykov <farkhod@sadykov.dev>
 License-Expression: MIT
 License-File: LICENSE
@@ -45,15 +45,15 @@
 # ShellGPT
 A command-line productivity tool powered by OpenAI's GPT models. As developers, we can leverage AI capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort. ShellGPT is cross-platform compatible and supports all major operating systems, including Linux, macOS, and Windows with all major shells, such as PowerShell, CMD, Bash, Zsh, Fish, and many others.
 
 https://user-images.githubusercontent.com/16740832/231569156-a3a9f9d4-18b1-4fff-a6e1-6807651aa894.mp4
 
 ## Installation
 ```shell
-pip install shell-gpt==0.9.1
+pip install shell-gpt==0.9.2
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
@@ -132,14 +132,26 @@
 ls
 # -> 1.mp4 2.mp4 3.mp4
 sgpt -s "using ffmpeg combine multiple videos into one without audio. Video file names: $(ls -m)"
 # -> ffmpeg -i 1.mp4 -i 2.mp4 -i 3.mp4 -filter_complex "[0:v] [1:v] [2:v] concat=n=3:v=1 [v]" -map "[v]" out.mp4
 # -> [E]xecute, [D]escribe, [A]bort: e
 ...
 ```
+### Shell integration
+Shell integration allows you to use Shell-GPT in your terminal with hotkeys. It is currently available for bash and zsh. It will allow you to have sgpt completions in your shell history, and also edit suggested commands right away.
+
+https://github.com/TheR1D/shell_gpt/assets/16740832/bead0dab-0dd9-436d-88b7-6abfb2c556c1
+
+To install shell integration, run:
+```shell
+sgpt --install-integration
+# Restart your terminal to apply changes.
+```
+This will add few lines to your `.bashrc` or `.zshrc` file. After that, you can use `Ctrl+l` (by default) to invoke Shell-GPT. When you press `Ctrl+l` it will replace you current input line (buffer) with suggested command. You can then edit it and press `Enter` to execute.
+
 ### Generating code
 With `--code` parameters we can query only code as output, for example:
 ```shell
 sgpt --code "Solve classic fizz buzz problem using Python"
 ```
 ```python
 for i in range(1, 101):
```

