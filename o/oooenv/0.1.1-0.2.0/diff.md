# Comparing `tmp/oooenv-0.1.1.tar.gz` & `tmp/oooenv-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oooenv-0.1.1.tar", max compression
+gzip compressed data, was "oooenv-0.2.0.tar", max compression
```

## Comparing `oooenv-0.1.1.tar` & `oooenv-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rwxr-xr-x   0        0        0     1073 2023-03-29 17:32:33.108507 oooenv-0.1.1/LICENSE
--rwxr-xr-x   0        0        0     1276 2023-03-29 19:12:03.973032 oooenv-0.1.1/README.md
--rwxr-xr-x   0        0        0        0 2023-03-29 14:28:44.487665 oooenv-0.1.1/oooenv/__init__.py
--rwxr-xr-x   0        0        0        0 2023-03-29 17:14:51.509563 oooenv-0.1.1/oooenv/cli/__init__.py
--rwxr-xr-x   0        0        0     3989 2023-03-29 17:15:51.769639 oooenv-0.1.1/oooenv/cli/main.py
--rwxr-xr-x   0        0        0        0 2023-03-29 14:36:41.949832 oooenv-0.1.1/oooenv/cmds/__init__.py
--rwxr-xr-x   0        0        0      174 2023-03-29 15:00:18.797439 oooenv-0.1.1/oooenv/cmds/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     5103 2023-03-29 17:06:15.560117 oooenv-0.1.1/oooenv/cmds/__pycache__/manage_env_cfg.cpython-310.pyc
--rwxr-xr-x   0        0        0     2841 2023-03-29 15:00:18.802246 oooenv-0.1.1/oooenv/cmds/__pycache__/uno_lnk.cpython-310.pyc
--rwxr-xr-x   0        0        0     4948 2023-03-29 17:06:13.599537 oooenv-0.1.1/oooenv/cmds/manage_env_cfg.py
--rwxr-xr-x   0        0        0     4553 2023-03-29 14:53:05.062246 oooenv-0.1.1/oooenv/cmds/uno_lnk.py
--rwxr-xr-x   0        0        0        0 2023-03-29 14:34:49.616759 oooenv-0.1.1/oooenv/utils/__init__.py
--rwxr-xr-x   0        0        0      175 2023-03-29 15:00:18.812804 oooenv-0.1.1/oooenv/utils/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3710 2023-03-29 15:00:18.815799 oooenv-0.1.1/oooenv/utils/__pycache__/local_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0     1146 2023-03-29 15:00:18.820968 oooenv-0.1.1/oooenv/utils/__pycache__/sys_info.cpython-310.pyc
--rwxr-xr-x   0        0        0     5887 2023-03-29 15:00:18.819281 oooenv-0.1.1/oooenv/utils/__pycache__/uno_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0     3708 2023-03-29 14:34:49.621334 oooenv-0.1.1/oooenv/utils/__pycache__/util.cpython-310.pyc
--rwxr-xr-x   0        0        0     3235 2023-03-29 14:35:38.587736 oooenv-0.1.1/oooenv/utils/local_paths.py
--rwxr-xr-x   0        0        0      745 2023-03-29 14:39:52.953002 oooenv-0.1.1/oooenv/utils/sys_info.py
--rwxr-xr-x   0        0        0     8437 2023-03-29 14:42:52.694789 oooenv-0.1.1/oooenv/utils/uno_paths.py
--rwxr-xr-x   0        0        0      925 2023-03-30 13:12:38.489540 oooenv-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2139 1970-01-01 00:00:00.000000 oooenv-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-04 18:27:08.699098 oooenv-0.2.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-04 18:27:08.700098 oooenv-0.2.0/oooenv/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 18:27:08.701098 oooenv-0.2.0/oooenv/cli/__init__.py
+-rw-r--r--   0        0        0     7915 2023-06-04 22:24:59.402702 oooenv-0.2.0/oooenv/cli/main.py
+-rw-r--r--   0        0        0        0 2023-06-04 18:27:08.702098 oooenv-0.2.0/oooenv/cmds/__init__.py
+-rw-r--r--   0        0        0      174 2023-06-04 18:27:08.703098 oooenv-0.2.0/oooenv/cmds/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5103 2023-06-04 18:27:08.703098 oooenv-0.2.0/oooenv/cmds/__pycache__/manage_env_cfg.cpython-310.pyc
+-rw-r--r--   0        0        0     2841 2023-06-04 18:27:08.704098 oooenv-0.2.0/oooenv/cmds/__pycache__/uno_lnk.cpython-310.pyc
+-rw-r--r--   0        0        0     5767 2023-06-04 21:30:23.424740 oooenv-0.2.0/oooenv/cmds/manage_env_cfg.py
+-rw-r--r--   0        0        0     4627 2023-06-04 18:55:26.719972 oooenv-0.2.0/oooenv/cmds/uno_lnk.py
+-rw-r--r--   0        0        0     1255 2023-06-04 21:24:47.067335 oooenv-0.2.0/oooenv/cmds/updater.py
+-rw-r--r--   0        0        0        0 2023-06-04 18:27:08.705098 oooenv-0.2.0/oooenv/utils/__init__.py
+-rw-r--r--   0        0        0      175 2023-06-04 18:27:08.705098 oooenv-0.2.0/oooenv/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3710 2023-06-04 18:27:08.706099 oooenv-0.2.0/oooenv/utils/__pycache__/local_paths.cpython-310.pyc
+-rw-r--r--   0        0        0     1146 2023-06-04 18:27:08.706099 oooenv-0.2.0/oooenv/utils/__pycache__/sys_info.cpython-310.pyc
+-rw-r--r--   0        0        0     5887 2023-06-04 18:27:08.707099 oooenv-0.2.0/oooenv/utils/__pycache__/uno_paths.cpython-310.pyc
+-rw-r--r--   0        0        0     3708 2023-06-04 18:27:08.707099 oooenv-0.2.0/oooenv/utils/__pycache__/util.cpython-310.pyc
+-rw-r--r--   0        0        0     3169 2023-06-04 18:38:49.468518 oooenv-0.2.0/oooenv/utils/local_paths.py
+-rw-r--r--   0        0        0      773 2023-06-04 18:47:20.056527 oooenv-0.2.0/oooenv/utils/sys_info.py
+-rw-r--r--   0        0        0     8556 2023-06-04 18:46:57.785630 oooenv-0.2.0/oooenv/utils/uno_paths.py
+-rw-r--r--   0        0        0     1419 2023-06-04 20:46:14.586346 oooenv-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1491 2023-06-04 22:31:23.476204 oooenv-0.2.0/README.md
+-rw-r--r--   0        0        0     2550 1970-01-01 00:00:00.000000 oooenv-0.2.0/PKG-INFO
```

### Comparing `oooenv-0.1.1/LICENSE` & `oooenv-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oooenv-0.1.1/README.md` & `oooenv-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -37,15 +37,22 @@
 
 Windows python projects cannot use linking to UNO Files.
 
 In Windows the virtual environment configuration file is manipulated.
 
 The Follow command toggles between original configuration and UNO environment configuration.
 
-```ps
+```powershell
 oooenv env -t
 ```
 
-If virtual environment is managed by Poetry then it will be necessary to toggle into original config before running
-`poetry update`.
+To update the configuration to match the installed verison of LibreOffice's python.
+
+This command should not be run until `oooenv env -t` has be run at least once.
+
+```powershell
+oooenv update --update
+```
+
+If virtual environment is managed by Poetry then it will be necessary to toggle into original config before running `poetry update`.
 
 When updates are done just run command again to toggle back to UNO environment configuration.
```

### Comparing `oooenv-0.1.1/oooenv/cmds/__pycache__/manage_env_cfg.cpython-310.pyc` & `oooenv-0.2.0/oooenv/cmds/__pycache__/manage_env_cfg.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oooenv-0.1.1/oooenv/cmds/__pycache__/uno_lnk.cpython-310.pyc` & `oooenv-0.2.0/oooenv/cmds/__pycache__/uno_lnk.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oooenv-0.1.1/oooenv/cmds/manage_env_cfg.py` & `oooenv-0.2.0/oooenv/cmds/manage_env_cfg.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 import os
 import sys
 import subprocess
 from pathlib import Path
-from typing import NamedTuple
+from typing import Dict, NamedTuple, cast
 from ..utils import local_paths
 
 # from ..lib.connect import LoSocketStart
 from ..utils import uno_paths
 
 
 class Version(NamedTuple):
@@ -22,47 +22,73 @@
 def get_uno_python_exe() -> str:
     """
     Gets Python Exe Path
 
     Raises:
         Exception: If not on Windows.
     """
+    # sourcery skip: raise-specific-error
     if sys.platform != "win32":
         raise Exception("Method only support Windows")
     p = Path(uno_paths.get_soffice_install_path(), "program", "python.exe")
     return str(p)
 
 
 def get_uno_python_ver() -> Version:
-    """Gets Uno Python Version"""
+    """
+    Gets Uno Python Version
+
+    Raises: Exception if not on Windows.
+    """
     python_exe = get_uno_python_exe()
     output = subprocess.check_output([python_exe, "--version"]).decode("UTF8").strip()
     # something like Python 3.8.10
     parts = output.split()
     major, minor, rev = parts[1].split(".")
     return Version(major=int(major), minor=int(minor), revision=int(rev))
 
 
-def read_pyvenv_cfg(fnm: str = "pyvenv.cfg") -> dict:
+def read_pyvenv_cfg(fnm: str = "pyvenv.cfg") -> Dict[str, str]:
     pyvenv_cfg = _get_pyvenv_cfg_path(fnm=fnm)
     result = {}
     with open(pyvenv_cfg, "r") as file:
         # strip of new line and remove anything after #
         # # for comment
         data = (row.partition("#")[0].rstrip() for row in file)
         # chain generator
         # remove empty lines
         data = (row for row in data if row)
-        # each line should now be key value pairs seperated by =
+        # each line should now be key value pairs separated by =
         for row in data:
             key, value = row.split("=")
             result[key.strip()] = value.strip()
     return result
 
 
+def get_libreoffice_py_ver_from_cfg(fnm: str = "pyvenv_uno.cfg") -> Version:
+    """
+    Gets LibreOffice Python Version from passed in cfg file.
+
+    Args:
+        fnm (str, optional): Config to get version from. Defaults to "pyvenv_uno.cfg".
+
+    Raises:
+        ValueError: if version_info not found in cfg.
+
+    Returns:
+        Version: Version of LibreOffice Python found in cfg.
+    """
+    cfg = read_pyvenv_cfg(fnm=fnm)
+    version_info = cast(str, cfg.get("version_info", ""))
+    if not version_info:
+        raise ValueError(f"version_info not found in {fnm}")
+    major, minor, revision, _ = version_info.split(".", maxsplit=3)
+    return Version(major=int(major), minor=int(minor), revision=int(revision))
+
+
 def is_env_uno_python(cfg: dict | None = None) -> bool:
     if cfg is None:
         cfg = read_pyvenv_cfg()
     home = cfg.get("home", "")
     if not home:
         return False
     lo_path = _get_lo_path()
@@ -75,19 +101,17 @@
     if is_env_uno_python(cfg):
         dst = src.parent / "pyvenv_uno.cfg"
     else:
         dst = src.parent / "pyvenv_orig.cfg"
     local_paths.copy_file(src=src, dst=dst)
 
 
-def _save_config(cfg: dict, fnm: str = "pyvenv.cfg"):
-    lst = []
-    for k, v in cfg.items():
-        lst.append(f"{k} = {v}")
-    if len(lst) > 0:
+def save_config(cfg: Dict[str, str], fnm: str = "pyvenv.cfg"):
+    lst = [f"{k} = {v}" for k, v in cfg.items()]
+    if lst:
         lst.append("")
     f_out = _get_venv_path() / fnm
     with open(f_out, "w") as file:
         file.write("\n".join(lst))
     print("Saved cfg")
 
 
@@ -110,59 +134,60 @@
         dst = env_path / "pyvenv.cfg"
         local_paths.copy_file(src=src, dst=dst)
         print("Set to Original Environment")
         return
 
     src = env_path / "pyvenv_orig.cfg"
     if not src.exists():
-        _save_config(cfg=cfg, fnm="pyvenv_orig.cfg")
+        save_config(cfg=cfg, fnm="pyvenv_orig.cfg")
 
     uno_cfg = env_path / "pyvenv_uno.cfg"
     if not uno_cfg.exists():
-        # need to create the file.
-        ver = str(get_uno_python_ver())
-        hm = _get_lo_path()
-        if "version" in cfg:
-            del cfg["version"]
-        cfg["home"] = hm
-        cfg["implementation"] = "CPython"
-        cfg["version_info"] = f"{ver}.final.0"
-        cfg["include-system-site-packages"] = "false"
-        cfg["base-prefix"] = f"{hm}\\python-core-{ver}"
-        cfg["base-exec-prefix"] = f"{hm}\\python-core-{ver}"
-        cfg["base-executable"] = f"{hm}\\python.exe"
-        _save_config(cfg=cfg, fnm="pyvenv_uno.cfg")
-
+        _set_config_save(cfg)
     src = env_path / "pyvenv_uno.cfg"
     dst = env_path / "pyvenv.cfg"
     local_paths.copy_file(src=src, dst=dst)
     print("Set to UNO Environment")
 
 
+def _set_config_save(cfg):
+    # need to create the file.
+    ver = str(get_uno_python_ver())
+    hm = _get_lo_path()
+    if "version" in cfg:
+        del cfg["version"]
+    cfg["home"] = hm
+    cfg["implementation"] = "CPython"
+    cfg["version_info"] = f"{ver}.final.0"
+    cfg["include-system-site-packages"] = "false"
+    cfg["base-prefix"] = f"{hm}\\python-core-{ver}"
+    cfg["base-exec-prefix"] = f"{hm}\\python-core-{ver}"
+    cfg["base-executable"] = f"{hm}\\python.exe"
+    save_config(cfg=cfg, fnm="pyvenv_uno.cfg")
+
+
 def _get_lo_path() -> str:
     lo_path = os.environ.get("ODEV_CONN_SOFFICE", None)
     if lo_path:
         index = lo_path.rfind("program")
-        if index > -1:
-            lo_path = lo_path[: index + 7]
-        else:
-            lo_path = None
+        lo_path = lo_path[: index + 7] if index > -1 else None
     if not lo_path:
         lo_path = str(uno_paths.get_soffice_install_path() / "program")
     return lo_path
 
 
 def _get_venv_path() -> Path:
-    vpath = os.environ.get("VIRTUAL_ENV", None)
-    if vpath is None:
+    v_path = os.environ.get("VIRTUAL_ENV", None)
+    if v_path is None:
         raise ValueError("Unable to get Virtual Environment Path")
-    return Path(vpath)
+    return Path(v_path)
 
 
 def _get_pyvenv_cfg_path(fnm: str = "pyvenv.cfg") -> Path:
-    vpath = _get_venv_path()
-    pyvenv_cfg = Path(vpath, fnm)
+    # sourcery skip: raise-specific-error
+    v_path = _get_venv_path()
+    pyvenv_cfg = Path(v_path, fnm)
     if not pyvenv_cfg.exists():
         raise FileNotFoundError(str(pyvenv_cfg))
     if not pyvenv_cfg.is_file():
         raise Exception(f'Not a file: "{pyvenv_cfg}"')
     return pyvenv_cfg
```

### Comparing `oooenv-0.1.1/oooenv/cmds/uno_lnk.py` & `oooenv-0.2.0/oooenv/cmds/uno_lnk.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,29 +15,30 @@
 from typing import Optional
 from pathlib import Path
 from ..utils import local_paths
 from ..utils import uno_paths
 
 
 def add_links(uno_src_dir: Optional[str] = None):
+    # sourcery skip: extract-duplicate-method
     if isinstance(uno_src_dir, str):
         str_cln = uno_src_dir.strip()
         if len(str_cln) == 0:
             p_uno_dir = uno_paths.get_uno_path()
         else:
             p_uno_dir = Path(str_cln)
             if not p_uno_dir.exists():
                 raise FileNotFoundError(f"Uno Source Dir not found: {uno_src_dir}")
             if not p_uno_dir.is_dir():
                 raise NotADirectoryError(f"UNO source is not a Directory: {uno_src_dir}")
     else:
         p_uno_dir = uno_paths.get_uno_path()
-    p_site_dir = local_paths.get_site_packeges_dir()
+    p_site_dir = local_paths.get_site_packages_dir()
     if p_site_dir is None:
-        print("Unable to find site_packages direct in virtual enviornment")
+        print("Unable to find site_packages direct in virtual environment")
         return
 
     p_uno = Path(p_uno_dir, "uno.py")
     p_uno_helper = Path(p_uno_dir, "unohelper.py")
 
     if p_uno.exists():
         dest = Path(p_site_dir, "uno.py")
@@ -65,35 +66,35 @@
             # OSError: [WinError 1314] A required privilege is not held by the client
             print(f"Unable to create system link for  '{p_uno_helper.name}'. Attempting copy.")
             shutil.copy2(p_uno_helper, dest)
             print(f"Copied file: {p_uno_helper} -> {dest}")
     else:
         print(f"{p_uno_helper.name} not found.")
     return
-    p_scriptforge = Path(uno_paths.get_lo_path(), "scriptforge.py")
-    if p_scriptforge.exists():
-        dest = Path(p_site_dir, "scriptforge.py")
-        try:
-            os.symlink(src=p_scriptforge, dst=dest)
-            print(f"Created system link: {p_scriptforge} -> {dest}")
-        except FileExistsError:
-            print(f"File already exist: {dest}")
-        except OSError:
-            # OSError: [WinError 1314] A required privilege is not held by the client
-            print(f"Unable to create system link for  '{p_scriptforge.name}'. Attempting copy.")
-            shutil.copy2(p_scriptforge, dest)
-            print(f"Copied file: {p_scriptforge} -> {dest}")
-    else:
-        print(f"{p_scriptforge.name} not found.")
+    # p_scriptforge = Path(uno_paths.get_lo_path(), "scriptforge.py")
+    # if p_scriptforge.exists():
+    #     dest = Path(p_site_dir, "scriptforge.py")
+    #     try:
+    #         os.symlink(src=p_scriptforge, dst=dest)
+    #         print(f"Created system link: {p_scriptforge} -> {dest}")
+    #     except FileExistsError:
+    #         print(f"File already exist: {dest}")
+    #     except OSError:
+    #         # OSError: [WinError 1314] A required privilege is not held by the client
+    #         print(f"Unable to create system link for  '{p_scriptforge.name}'. Attempting copy.")
+    #         shutil.copy2(p_scriptforge, dest)
+    #         print(f"Copied file: {p_scriptforge} -> {dest}")
+    # else:
+    #     print(f"{p_scriptforge.name} not found.")
 
 
 def remove_links():
-    p_site_dir = local_paths.get_site_packeges_dir()
+    p_site_dir = local_paths.get_site_packages_dir()
     if p_site_dir is None:
-        print("Unable to find site_packages direct in virtual enviornment")
+        print("Unable to find site_packages direct in virtual environment")
         return
 
     uno_path = Path(p_site_dir, "uno.py")
     if uno_path.exists():
         os.remove(uno_path)
         print("removed uno.py")
     else:
@@ -101,29 +102,29 @@
     unohelper_path = Path(p_site_dir, "unohelper.py")
     if unohelper_path.exists():
         os.remove(unohelper_path)
         print("removed unohelper.py")
     else:
         print("unohelper.py does not exist in virtual env.")
     return
-    scriptforge_path = Path(p_site_dir, "scriptforge.py")
-    if scriptforge_path.exists():
-        os.remove(scriptforge_path)
-        print("removed scriptforge.py")
-    else:
-        print("scriptforge.py does not exist in virtual env.")
+    # scriptforge_path = Path(p_site_dir, "scriptforge.py")
+    # if scriptforge_path.exists():
+    #     os.remove(scriptforge_path)
+    #     print("removed scriptforge.py")
+    # else:
+    #     print("scriptforge.py does not exist in virtual env.")
 
 
 def main():
     if len(sys.argv) == 2:
         arg = sys.argv[1]
-        if arg == "-r" or arg == "--remove":
+        if arg in ["-r", "--remove"]:
             remove_links()
             return
-        if arg == "-a" or arg == "-add":
+        if arg in ["-a", "-add"]:
             add_links()
             return
     print("for add links use -a or --add\nfor remove use -r or --remove")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `oooenv-0.1.1/oooenv/utils/__pycache__/local_paths.cpython-310.pyc` & `oooenv-0.2.0/oooenv/utils/__pycache__/local_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oooenv-0.1.1/oooenv/utils/__pycache__/sys_info.cpython-310.pyc` & `oooenv-0.2.0/oooenv/utils/__pycache__/sys_info.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oooenv-0.1.1/oooenv/utils/__pycache__/uno_paths.cpython-310.pyc` & `oooenv-0.2.0/oooenv/utils/__pycache__/uno_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oooenv-0.1.1/oooenv/utils/__pycache__/util.cpython-310.pyc` & `oooenv-0.2.0/oooenv/utils/__pycache__/util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oooenv-0.1.1/oooenv/utils/local_paths.py` & `oooenv-0.2.0/oooenv/utils/local_paths.py`

 * *Files 10% similar despite different names*

```diff
@@ -72,62 +72,57 @@
     expand = None
     if isinstance(path, str):
         expand = path.startswith("~")
         p = Path(path)
     elif isinstance(path, Path):
         p = path
     else:
-        lst = [s for s in path]
+        lst = list(path)
     if p is None:
-        if len(lst) == 0:
+        if not lst:
             raise ValueError("lst arg is zero length")
         arg = lst[0]
         expand = arg.startswith("~")
         p = Path(*lst)
-    else:
-        if expand is None:
-            pstr = str(p)
-            expand = pstr.startswith("~")
+    elif expand is None:
+        p_str = str(p)
+        expand = p_str.startswith("~")
     if expand:
         p = p.expanduser()
-    if ensure_absolute is True and p.is_absolute() is False:
+    if ensure_absolute and p.is_absolute() is False:
         p = Path(get_root(), p)
     return p
 
 
 def get_virtual_env_path() -> str:
     """
     Gets the Virtual Environment Path
 
     Returns:
-        str: Viruatl Environment Path
+        str: Virtual Environment Path
 
     Note:
         If unable to get virtual path from Environment then ``sys.base_exec_prefix`` is returned.
     """
-    spath = os.environ.get("VIRTUAL_ENV", None)
-    if spath is not None:
-        return spath
-    return sys.base_exec_prefix
+    s_path = os.environ.get("VIRTUAL_ENV", None)
+    return s_path if s_path is not None else sys.base_exec_prefix
 
 
-def get_site_packeges_dir() -> Union[Path, None]:
+def get_site_packages_dir() -> Union[Path, None]:
     """
     Gets the ``site-packages`` directory for current python environment.
 
     Returns:
         Union[Path, None]: site-packages dir if found; Otherwise, None.
     """
     v_path = get_virtual_env_path()
     p_site = Path(v_path, "Lib", "site-packages")
     if p_site.exists() and p_site.is_dir():
         return p_site
 
     ver = f"{sys.version_info[0]}.{sys.version_info[1]}"
     p_site = Path(v_path, "lib", f"python{ver}", "site-packages")
-    if p_site.exists() and p_site.is_dir():
-        return p_site
-    return None
+    return p_site if p_site.exists() and p_site.is_dir() else None
 
 
 def copy_file(src: str | Path, dst: str | Path):
     shutil.copy2(src=src, dst=dst)
```

### Comparing `oooenv-0.1.1/oooenv/utils/sys_info.py` & `oooenv-0.2.0/oooenv/utils/sys_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from enum import Enum
 
 
 class SysInfo:
     """System Info related"""
 
     class PlatformEnum(str, Enum):
+        """Platform Enum"""
         UNKNOWN = "Unknown"
         WINDOWS = "Windows"
         MAC = "Darwin"
         LINUX = "Linux"
 
     @staticmethod
     def get_platform() -> SysInfo.PlatformEnum:
```

### Comparing `oooenv-0.1.1/oooenv/utils/uno_paths.py` & `oooenv-0.2.0/oooenv/utils/uno_paths.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,47 +30,48 @@
 
     For windows this will be something like: ``C:\\Program Files\\LibreOffice``.
     For Linux this will be something like: ``/usr/lib/libreoffice``
 
     Returns:
         Path: install as Path.
     """
+    # sourcery skip: assign-if-exp, extract-duplicate-method, extract-method, hoist-statement-from-if, inline-immediately-returned-variable, low-code-quality
     global _INSTALL_PATH
     if _INSTALL_PATH is not None:
         return _INSTALL_PATH
     if PLATFORM == SysInfo.PlatformEnum.WINDOWS:
-        # get the path location from registery
+        # get the path location from Registry
         value = ""
         for _key in (
             # LibreOffice 3.4.5,6,7 on Windows
             "SOFTWARE\\LibreOffice\\UNO\\InstallPath",
             # OpenOffice 3.3
             "SOFTWARE\\OpenOffice.org\\UNO\\InstallPath",
         ):
             try:
                 value = winreg.QueryValue(winreg.HKEY_LOCAL_MACHINE, _key)
             except Exception as detail:
                 value = ""
-                _errMess = "%s" % detail
+                # _errMess = "%s" % detail
             else:
                 break  # first existing key will do
         if value != "":
             _INSTALL_PATH = Path("\\".join(value.split("\\")[:-1]))  # drop the program
             return _INSTALL_PATH
 
-        # failed to get path from registery. Going Manual
+        # failed to get path from Registry. Going Manual
         soffice = "soffice.exe"
         p_sf = Path(os.environ["PROGRAMFILES"], "LibreOffice", "program", soffice)
-        if p_sf.exists() is False or p_sf.is_file() is False:
+        if not p_sf.exists() or not p_sf.is_file():
             p_sf = Path(os.environ["PROGRAMFILES(X86)"], "LibreOffice", "program", soffice)
-        if p_sf.exists() is False or p_sf.is_file() is False:
+        if not p_sf.exists() or not p_sf.is_file():
             # perhaps running a developer version.
             # C:\Program Files\LibreOfficeDev 7\program
             p_sf = Path(os.environ["PROGRAMFILES"], "LibreOfficeDev 7", "program", soffice)
-        if p_sf.exists() is False or p_sf.is_file() is False:
+        if not p_sf.exists() or not p_sf.is_file():
             p_sf = Path(os.environ["PROGRAMFILES(X86)"], "LibreOfficeDev 7", "program", soffice)
         if not p_sf.exists():
             raise FileNotFoundError(f"LibreOffice '{p_sf}' not found.")
         if not p_sf.is_file():
             raise IsADirectoryError(f"LibreOffice '{p_sf}' is not a file.")
         # drop \program\soffice.exe
         # expect C:\Program Files\LibreOffice
@@ -130,18 +131,19 @@
     Raises:
         FileNotFoundError: if path is not found
         NotADirectoryError: if path is not a directory
 
     Returns:
         Path: First found path.
     """
+    # sourcery skip: extract-duplicate-method
     if PLATFORM == SysInfo.PlatformEnum.WINDOWS:
 
         p_uno = Path(os.environ["PROGRAMFILES"], "LibreOffice", "program")
-        if p_uno.exists() is False or p_uno.is_dir() is False:
+        if not p_uno.exists() or not p_uno.is_dir():
             p_uno = Path(os.environ["PROGRAMFILES(X86)"], "LibreOffice", "program")
         if not p_uno.exists():
             raise FileNotFoundError("Uno Source Dir not found.")
         if not p_uno.is_dir():
             raise NotADirectoryError("UNO source is not a Directory")
         return p_uno
     elif PLATFORM == SysInfo.PlatformEnum.MAC:
@@ -184,15 +186,15 @@
             if os.path.islink(s):
                 # follow link
                 p_sf = Path(os.path.realpath(s)).parent
             else:
                 p_sf = Path(s).parent
         if p_sf is None:
             p_sf = Path("/usr/bin/soffice")
-            if p_sf.exists() is False or p_sf.is_file() is False:
+            if not p_sf.exists() or not p_sf.is_file():
                 raise FileNotFoundError("LibreOffice Source Dir not found.")
             p_sf = p_sf.parent
 
         if not p_sf.exists():
             raise FileNotFoundError("LibreOffice Source Dir not found.")
         if not p_sf.is_dir():
             raise NotADirectoryError("LibreOffice source is not a Directory")
@@ -213,39 +215,38 @@
     Raises:
         FileNotFoundError: In Windows if ``python.exe`` is not found.
         NotADirectoryError: In Windows if ``python.exe`` is not a file.
 
     Returns:
         str: file location of python executable.
     """
-    if PLATFORM == SysInfo.PlatformEnum.WINDOWS:
-        p = Path(get_lo_path(), "python.exe")
-
-        if not p.exists():
-            raise FileNotFoundError("LibreOffice python executable not found.")
-        if not p.is_file():
-            raise NotADirectoryError("LibreOffice  python executable is not a file")
-        return str(p)
-    else:
+    if PLATFORM != SysInfo.PlatformEnum.WINDOWS:
         return sys.executable
+    p = Path(get_lo_path(), "python.exe")
+
+    if not p.exists():
+        raise FileNotFoundError("LibreOffice python executable not found.")
+    if not p.is_file():
+        raise NotADirectoryError("LibreOffice  python executable is not a file")
+    return str(p)
 
 
 @overload
 def mkdirp(dest_dir: str) -> None:
     ...
 
 
 @overload
 def mkdirp(dest_dir: Path) -> None:
     ...
 
 
 def mkdirp(dest_dir: Union[str, os.PathLike]) -> None:
     """
-    Creates path and subpaths not existing.
+    Creates path and subpath not existing.
 
     Args:
         dest_dir (str | PathLike]): PathLike object
     """
     # Python ≥ 3.5
     pth = Path(dest_dir)
     if not pth.is_absolute():
```

### Comparing `oooenv-0.1.1/PKG-INFO` & `oooenv-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: oooenv
-Version: 0.1.1
-Summary: Configures a project environment for LibreOffice UNO.
+Version: 0.2.0
+Summary: Configures a project python environment for LibreOffice UNO.
 Home-page: https://github.com/Amourspirit/python_oooenv
 License: MIT
-Keywords: libreoffice,macro,uno,ooouno
+Keywords: libreoffice,macro,uno,ooouno,venv
 Author: :Barry-Thomas-Paul: Moss
 Author-email: vibrationoflife@protonmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Office/Business
 Project-URL: Documentation, https://github.com/Amourspirit/python_oooenv
 Project-URL: Repository, https://github.com/Amourspirit/python_oooenv
 Description-Content-Type: text/markdown
 
 # OOOENV
 
 This project is strictly for LibreOffice python projects that need to set UNO environment.
@@ -58,16 +62,23 @@
 
 Windows python projects cannot use linking to UNO Files.
 
 In Windows the virtual environment configuration file is manipulated.
 
 The Follow command toggles between original configuration and UNO environment configuration.
 
-```ps
+```powershell
 oooenv env -t
 ```
 
-If virtual environment is managed by Poetry then it will be necessary to toggle into original config before running
-`poetry update`.
+To update the configuration to match the installed verison of LibreOffice's python.
+
+This command should not be run until `oooenv env -t` has be run at least once.
+
+```powershell
+oooenv update --update
+```
+
+If virtual environment is managed by Poetry then it will be necessary to toggle into original config before running `poetry update`.
 
 When updates are done just run command again to toggle back to UNO environment configuration.
```

