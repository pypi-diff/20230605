# Comparing `tmp/run_rx-0.0.4.tar.gz` & `tmp/run_rx-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "run_rx-0.0.4.tar", max compression
+gzip compressed data, was "run_rx-0.0.5.tar", max compression
```

## Comparing `run_rx-0.0.4.tar` & `run_rx-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-05-04 19:54:40.231125 run_rx-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0      901 2023-05-09 22:23:59.643229 run_rx-0.0.4/README.md
--rw-r--r--   0        0        0      298 2023-04-28 22:39:27.166689 run_rx-0.0.4/install/.rxignore
--rw-r--r--   0        0        0      588 2023-03-14 00:53:59.323287 run_rx-0.0.4/install/README.md
--rw-r--r--   0        0        0       98 2023-04-01 19:04:24.721429 run_rx-0.0.4/install/python-cpu
--rw-r--r--   0        0        0       98 2023-04-01 19:04:30.545846 run_rx-0.0.4/install/python-gpu
--rw-r--r--   0        0        0      736 2023-05-09 22:39:24.604555 run_rx-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      300 2023-05-03 20:39:38.474682 run_rx-0.0.4/rx/__main__.py
--rw-r--r--   0        0        0     2406 2023-05-09 22:23:45.102644 run_rx-0.0.4/rx/client/commands/exec.py
--rw-r--r--   0        0        0      989 2023-05-09 22:23:45.103045 run_rx-0.0.4/rx/client/commands/init.py
--rw-r--r--   0        0        0     1970 2023-04-10 18:30:14.435321 run_rx-0.0.4/rx/client/configuration/config_base.py
--rw-r--r--   0        0        0     6945 2023-05-09 22:39:33.336925 run_rx-0.0.4/rx/client/configuration/local.py
--rw-r--r--   0        0        0      481 2023-03-29 19:30:38.625814 run_rx-0.0.4/rx/client/configuration/remote.py
--rw-r--r--   0        0        0     2811 2023-05-09 22:23:45.103366 run_rx-0.0.4/rx/client/executor.py
--rw-r--r--   0        0        0      256 2023-04-10 18:50:33.017005 run_rx-0.0.4/rx/client/grpc_helper.py
--rw-r--r--   0        0        0     5202 2023-05-09 22:23:45.104121 run_rx-0.0.4/rx/client/init_client.py
--rw-r--r--   0        0        0     9492 2023-05-05 21:12:58.788558 run_rx-0.0.4/rx/client/login.py
--rw-r--r--   0        0        0     2029 2023-03-25 18:11:12.345418 run_rx-0.0.4/rx/client/menu.py
--rw-r--r--   0        0        0     1029 2023-05-03 20:09:57.609097 run_rx-0.0.4/rx/client/output_handler.py
--rw-r--r--   0        0        0     2303 2023-05-05 22:11:20.469353 run_rx-0.0.4/rx/client/rsync.py
--rw-r--r--   0        0        0     1579 2023-03-29 19:53:44.892412 run_rx-0.0.4/rx/client/user.py
--rw-r--r--   0        0        0     5866 2023-05-09 18:41:10.568989 run_rx-0.0.4/rx/proto/rx_pb2.py
--rw-r--r--   0        0        0     7595 2023-05-09 18:41:10.570471 run_rx-0.0.4/rx/proto/rx_pb2.pyi
--rw-r--r--   0        0        0    12663 2023-05-09 18:41:10.570796 run_rx-0.0.4/rx/proto/rx_pb2_grpc.py
--rw-r--r--   0        0        0     1819 1970-01-01 00:00:00.000000 run_rx-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-16 20:24:41.276898 run_rx-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     1679 2023-05-19 14:53:21.015913 run_rx-0.0.5/README.md
+-rw-r--r--   0        0        0      313 2023-06-01 23:35:09.526681 run_rx-0.0.5/install/.rxignore
+-rw-r--r--   0        0        0      274 2023-06-04 16:34:29.656668 run_rx-0.0.5/install/README.md
+-rw-r--r--   0        0        0       98 2023-05-16 20:24:41.277933 run_rx-0.0.5/install/python-cpu
+-rw-r--r--   0        0        0       98 2023-05-16 20:24:41.278137 run_rx-0.0.5/install/python-gpu
+-rw-r--r--   0        0        0      736 2023-06-05 01:42:19.164130 run_rx-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-05-16 20:24:41.279362 run_rx-0.0.5/rx/__main__.py
+-rw-r--r--   0        0        0     2799 2023-06-04 17:02:00.126921 run_rx-0.0.5/rx/client/commands/exec.py
+-rw-r--r--   0        0        0     1284 2023-06-01 23:40:03.839582 run_rx-0.0.5/rx/client/commands/init.py
+-rw-r--r--   0        0        0     2109 2023-06-04 16:41:38.419103 run_rx-0.0.5/rx/client/configuration/config_base.py
+-rw-r--r--   0        0        0     7016 2023-06-05 01:42:40.149599 run_rx-0.0.5/rx/client/configuration/local.py
+-rw-r--r--   0        0        0      501 2023-05-16 20:24:41.281326 run_rx-0.0.5/rx/client/configuration/remote.py
+-rw-r--r--   0        0        0     3045 2023-06-04 16:47:27.983133 run_rx-0.0.5/rx/client/executor.py
+-rw-r--r--   0        0        0      256 2023-05-16 20:24:41.281715 run_rx-0.0.5/rx/client/grpc_helper.py
+-rw-r--r--   0        0        0     5353 2023-06-01 23:06:43.816386 run_rx-0.0.5/rx/client/init_client.py
+-rw-r--r--   0        0        0     9694 2023-05-16 20:24:41.282187 run_rx-0.0.5/rx/client/login.py
+-rw-r--r--   0        0        0     2029 2023-05-16 20:24:41.282556 run_rx-0.0.5/rx/client/menu.py
+-rw-r--r--   0        0        0     1092 2023-05-16 20:24:41.282728 run_rx-0.0.5/rx/client/output_handler.py
+-rw-r--r--   0        0        0     3307 2023-06-04 16:44:15.057168 run_rx-0.0.5/rx/client/rsync.py
+-rw-r--r--   0        0        0     1603 2023-05-16 20:24:41.283538 run_rx-0.0.5/rx/client/user.py
+-rw-r--r--   0        0        0     5866 2023-05-09 18:41:10.568989 run_rx-0.0.5/rx/proto/rx_pb2.py
+-rw-r--r--   0        0        0     7595 2023-05-09 18:41:10.570471 run_rx-0.0.5/rx/proto/rx_pb2.pyi
+-rw-r--r--   0        0        0    12663 2023-05-09 18:41:10.570796 run_rx-0.0.5/rx/proto/rx_pb2_grpc.py
+-rw-r--r--   0        0        0     2597 1970-01-01 00:00:00.000000 run_rx-0.0.5/PKG-INFO
```

### Comparing `run_rx-0.0.4/LICENSE.txt` & `run_rx-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.4/pyproject.toml` & `run_rx-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "run-rx"
-version = "0.0.4"
+version = "0.0.5"
 description = "A tool to simplify remote execution"
 authors = ["Kris Chodorow <k.chodorow@gmail.com>"]
 license = "LICENSE.txt"
 readme = "README.md"
 homepage = "https://www.run-rx.com"
 repository = "https://github.com/run-rx/rx"
 packages = [
```

### Comparing `run_rx-0.0.4/rx/client/commands/exec.py` & `run_rx-0.0.5/rx/client/commands/exec.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-"""Rx usage
+"""rx usage
 
-Configure this directory to be able to run on a remote host:
+To set up this directory on a remote host:
 
     rx init
 
 You only have to run this once per directory, similar to `git init`.
 
-To run a command on a configured remote host:
+To run a command on the remote host:
 
     rx CMD
 
+Run 'rx --help' for more options or visit https://www.run-rx.com.
 """
 import pathlib
 import tempfile
 from typing import List
 
 from absl import app
 from absl import logging
 
 from rx.client import executor
 from rx.client import grpc_helper
 from rx.client.commands import init
+from rx.client.configuration import config_base
 from rx.client.configuration import local
 from rx.client.configuration import remote
 
 
 class ExecCommand:
 
   def __init__(self, argv: List[str]):
     self._argv = argv
-    self._config = local.find_local_config(pathlib.Path.cwd())
+    cwd = (
+      pathlib.Path(config_base.RX_ROOT.value) if config_base.RX_ROOT.value else
+      pathlib.Path.cwd())
+    self._config = local.find_local_config(cwd)
 
   def run(self) -> int:
     if self._config is None:
       print ('Run `rx init` first!')
       return -1
     remote_cfg = remote.Remote(self._config.cwd)
     with grpc_helper.get_channel(remote_cfg['grpc_addr']) as ch:
@@ -52,39 +57,45 @@
       # TODO: is there a better way to handle this with absl flags?
       self._argv = self._argv[0].split(' ')
     try:
       return client.exec(self._argv)
     except KeyboardInterrupt:
       client.maybe_kill()
       return executor.SIGINT_CODE
+    except executor.UnreachableError as e:
+      print(
+        f'Worker {e.worker} was unrechable, run `rx init` to get a new '
+        'instance.')
+      return e.code
 
 
 class VersionCommand:
   """Prints the version."""
 
   def run(self):
     print(local.VERSION)
 
 
 def main(argv):
   logging.get_absl_handler().python_handler.use_absl_log_file(
     program_name='rx', log_dir=tempfile.gettempdir())
   if len(argv) == 1:
+    print('No command given.\n')
     app.usage(shorthelp=True)
     return -1
   cmd_to_run = argv[1]
   try:
     if cmd_to_run == 'init':
       cmd = init.InitCommand()
     elif cmd_to_run == 'version':
       cmd = VersionCommand()
     else:
       if cmd_to_run == 'run':
-        # "rx run foo" is generally the same as "rx foo", but the extra "run" can
-        # be handy when running a script called "init", say, on the remote
+        # "rx run foo" is generally the same as "rx foo", but the extra "run"
+        # can be handy when running a script called "init", say, on the remote
         # machine.
         argv = argv[1:]
       cmd = ExecCommand(argv[1:])
     return cmd.run()
   except KeyboardInterrupt:
     return executor.SIGINT_CODE
```

### Comparing `run_rx-0.0.4/rx/client/configuration/config_base.py` & `run_rx-0.0.5/rx/client/configuration/config_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
 RX_DIR = pathlib.Path('.rx')
 
 # Configuration files are placed under a directory with this name (this is just
 # to make development easier, so we can have separate configs for
 # local/dev/prod).
 TREX_HOST = flags.DEFINE_string(
-  'grpc_host', 'trex.run-rx.com', 'GRPC host to connect to.')
+  'trex-host', 'trex.run-rx.com', 'GRPC host to connect to.')
+RX_ROOT = flags.DEFINE_string(
+  'rxroot', None, 'The directory to use as rxroot (defaults to pwd)')
 
 
 class ReadOnlyConfig(abc.Mapping):
   def __init__(self, config_file: pathlib.Path, strict_mode: bool = True):
     self._config_file = config_file
     if not strict_mode and not config_file.exists():
       self._config = {}
@@ -56,14 +58,14 @@
   def __setitem__(self, item, value):
     self._config[item] = value
 
   def __delitem__(self, item):
     self._config.__delitem__(item)
 
 
-def get_config_dir() -> pathlib.Path:
-  """Returns the config directory path, e.g., .rx/localhost/config."""
-  return RX_DIR / TREX_HOST.value / 'config'
+def get_config_dir(rxroot: pathlib.Path) -> pathlib.Path:
+  """Returns the absolute config directory path, e.g., /proj/.rx/t.c/config."""
+  return rxroot / RX_DIR / TREX_HOST.value / 'config'
 
 
 def is_local() -> bool:
   return TREX_HOST.value.startswith('localhost')
```

### Comparing `run_rx-0.0.4/rx/client/configuration/local.py` & `run_rx-0.0.5/rx/client/configuration/local.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,38 +10,39 @@
 from absl import flags
 from absl import logging
 import sty
 
 from rx.client.configuration import config_base
 from rx.proto import rx_pb2
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 
 IGNORE = pathlib.Path('.rxignore')
 
 _REMOTE = flags.DEFINE_string(
-  'remote', 'default',
-  'The remote configuration file to use (see .rx/README.md).')
+  'remote', None,
+  'The path to the remote configuration file to use (see .rx/README.md).')
 _RSYNC_PATH = flags.DEFINE_string('rsync_path', None, 'Path to rsync binary')
 
 _REMOTE_DIR = config_base.RX_DIR / 'remotes'
+_DEFAULT_REMOTE = _REMOTE_DIR / 'default'
 
 
 class LocalConfigWriter(config_base.ReadWriteConfig):
   """This holds all of the configuration options that can be determined from
   the local machine."""
 
   def __init__(self, workspace_dir: pathlib.Path):
-    super().__init__(workspace_dir / _get_local_config_file())
+    super().__init__(_get_local_config_file(workspace_dir))
     self._workspace_dir = workspace_dir
 
   def setup_remote(self):
     """Sets the "remote" field (and color) for the local config."""
-    remote = _REMOTE.value
-    remote_path = self._workspace_dir / _REMOTE_DIR / remote
+    remote = str(_REMOTE.value if _REMOTE.value else _DEFAULT_REMOTE)
+    remote_path = self._workspace_dir / remote
     try:
       with remote_path.open(mode='rt', encoding='utf-8') as fh:
         remote_content = fh.read()
         self._set_color(remote_content)
         self['remote'] = remote
     except FileExistsError:
       raise FileExistsError(
@@ -60,15 +61,15 @@
     self['color'] = {'r': r, 'g': g, 'b': b}
 
 
 class LocalConfig(config_base.ReadOnlyConfig):
   """Create the local configuration."""
 
   def __init__(self, working_dir: pathlib.Path):
-    super().__init__(working_dir / _get_local_config_file())
+    super().__init__(_get_local_config_file(working_dir))
     self._cwd = working_dir
     self.config_dir = self.cwd / config_base.RX_DIR
     self._color = None
 
   @property
   def cwd(self) -> pathlib.Path:
     return self._cwd
@@ -84,15 +85,15 @@
     # TODO: how to automatically determine language?
     if 'python' not in docker_image:
       logging.info('Using a non-Python image. There be dragons here.')
       return rx_pb2.Environment()
     return rx_pb2.Environment(python=rx_pb2.Python())
 
   def get_target_env(self) -> rx_pb2.Environment:
-    remote_file = self.cwd / _REMOTE_DIR / self['remote']
+    remote_file = self.cwd / self['remote']
     try:
       with remote_file.open(mode='rt', encoding='utf-8') as fh:
         remote_config = json.load(fh)
     except json.JSONDecodeError as e:
       logging.exception(f'Could not parse {self["remote"]}')
       raise e
     env = rx_pb2.Environment(alloc=rx_pb2.Remote())
@@ -115,28 +116,28 @@
     color = self['color']
     fg = sty.fg(color['r'], color['g'], color['b'])
     return f'{fg}{s}{sty.rs.fg}'
 
 
 def create_local_config(cwd: pathlib.Path) -> LocalConfig:
   """Gets or creates .rx directory."""
-  config_dir = (cwd / _get_local_config_file()).parent
+  config_dir = _get_local_config_file(cwd).parent
   config_dir.mkdir(exist_ok=True, parents=True)
   with LocalConfigWriter(cwd) as c:
     c.setup_remote()
     c['project_name'] = _find_project_name(cwd)
     c['rsync_path'] = _get_rsync_path()
   return LocalConfig(cwd)
 
 
 def find_local_config(working_dir: pathlib.Path) -> Optional[LocalConfig]:
   """Factory to create a config by looking for .rx."""
-  cfg_path = working_dir / config_base.get_config_dir()
+  cfg_path = config_base.get_config_dir(working_dir)
   for parent in cfg_path.parents:
-    if (parent / config_base.get_config_dir()).exists():
+    if config_base.get_config_dir(parent).exists():
       return LocalConfig(parent)
   return None
 
 
 def get_source_path() -> pathlib.Path:
   """Gets the path bundled client files can be found on."""
   # __file__ is ./rx/client/configuration/local.py, so this resolves to ./.
@@ -196,17 +197,17 @@
   for parent in start_dir.parents:
     if (parent / '.git').exists():
       return start_dir.name
   # Maybe we haven't initialized git yet, use out name.
   return start_dir.name
 
 
-def _get_local_config_file() -> pathlib.Path:
+def _get_local_config_file(rxroot: pathlib.Path) -> pathlib.Path:
   """Return .rx/trex-dev.run-rx.com/config/local."""
-  return config_base.get_config_dir() / 'local'
+  return config_base.get_config_dir(rxroot) / 'local'
 
 
 def _install_file(install_dir, config_dir, base_name):
   """Installs a file if it doesn't already exist."""
   source_path = install_dir / base_name
   destination_path = config_dir / base_name
   if not destination_path.exists():
```

### Comparing `run_rx-0.0.4/rx/client/executor.py` & `run_rx-0.0.5/rx/client/executor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from typing import List
+from typing import List, cast
 
 from absl import logging
 import grpc
 
 from rx.client import login
 from rx.client import output_handler
 from rx.client import rsync
@@ -29,42 +29,42 @@
       remote_cfg: remote.Remote):
     self._uri = remote_cfg['grpc_addr']
     self._rsync = rsync.RsyncClient(local_cfg, remote_cfg)
     self._stub = rx_pb2_grpc.ExecutionServiceStub(channel)
     self._metadata = local.get_grpc_metadata()
     self._local_cfg = local_cfg
     self._remote_cfg = remote_cfg
-    self._login = login.LoginManager()
+    self._login = login.LoginManager(local_cfg.cwd)
     self._current_execution_id = None
 
   def exec(self, argv: List[str]) -> int:
     cmd_str = ' '.join(argv)
     logging.info(f'Running `{cmd_str}` on {self._uri}')
 
     self._login.login()
     self._metadata += self._login.grpc_metadata
 
     result = self._rsync.to_remote()
     if result != 0:
-      print('Worker was unrechable, run `rx init` to get a new instance.')
-      return result
+      raise UnreachableError(self._local_cfg["worker_addr"], result)
     result = None
 
     request = rx_pb2.ExecRequest(
       workspace_id=self._remote_cfg['workspace_id'],
       argv=argv,
       rsync_source=self._local_cfg.rsync_source)
 
-    out_handler = output_handler.OutputHandler()
+    out_handler = output_handler.OutputHandler(self._local_cfg.cwd)
     response = None
     try:
       for response in self._stub.Exec(request, metadata=self._metadata):
         self._current_execution_id = response.execution_id
         out_handler.handle(response)
     except grpc.RpcError as e:
+      e = cast(grpc.Call, e)
       sys.stderr.write(f'Error contacting {self._uri}: {e.details()}\n')
       return _NOT_REACHABLE
     except KeyboardInterrupt:
       self.maybe_kill()
       return SIGINT_CODE
     except RuntimeError as e:
       # Bug in grpc, probably.
@@ -91,7 +91,14 @@
       return
 
     req = rx_pb2.KillRequest(
       workspace_id=self._remote_cfg['workspace_id'],
       execution_id=self._current_execution_id,
     )
     self._stub.Kill(req, metadata=self._metadata)
+
+
+class UnreachableError(RuntimeError):
+  def __init__(self, worker_addr: str, code: int, *args: object) -> None:
+    super().__init__(*args)
+    self.worker = worker_addr
+    self.code = code
```

### Comparing `run_rx-0.0.4/rx/client/init_client.py` & `run_rx-0.0.5/rx/client/init_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+from typing import cast
 
 from absl import logging
 from google.protobuf import empty_pb2
 import grpc
 
 from rx.client import grpc_helper
 from rx.client import login
@@ -17,15 +18,15 @@
 
 class Client():
   """Handle contacting the remote server."""
 
   def __init__(self, channel: grpc.Channel, local_cfg: local.LocalConfig):
     self._stub = rx_pb2_grpc.SetupServiceStub(channel)
     self._local_cfg = local_cfg
-    self._login = login.LoginManager()
+    self._login = login.LoginManager(local_cfg.cwd)
     self._metadata = local.get_grpc_metadata()
 
   def create_user_or_log_in(self) -> user.User:
     # First, make sure we're logged in with Google.
     try:
       self._login.login()
     except login.AuthError as e:
@@ -40,14 +41,17 @@
     username = self._get_username()
     if not user.has_config(self._local_cfg.cwd):
       with user.CreateUser(self._local_cfg.cwd) as c:
         c['username'] = username
         c['email'] = email
     return user.User(self._local_cfg.cwd, email)
 
+  def dry_run(self):
+    rsync.dry_run(self._local_cfg)
+
   def init(self) -> int:
     try:
       target_env = self._local_cfg.get_target_env()
     except local.ConfigError as e:
       raise InitError(str(e), -1)
     if target_env.alloc.hardware.processor == 'gpu':
       print('rx only works with CPUs at the moment, but I appreciate your '
@@ -61,14 +65,15 @@
     sys.stdout.write('Finding a remote worker... ')
     sys.stdout.flush()
     try:
       # Five minute timeout.
       resp = self._stub.Init(req, metadata=self._metadata, timeout=(5 * 60))
       sys.stdout.write('Done.\n')
     except grpc.RpcError as e:
+      e = cast(grpc.Call, e)
       raise InitError(f'Could not initialize worker: {e.details()}', -1)
     if resp.result.code != 0:
       raise InitError(resp.result.message, -1)
 
     # TODO: create a threaded UserStatus class with __enter__/__exit__.
     sys.stdout.write('Copying source code... ')
     sys.stdout.flush()
@@ -106,36 +111,38 @@
     return self._create_username()
 
   def _get_username_from_rx(self) -> str:
     try:
       resp = self._stub.GetUser(
         empty_pb2.Empty(), metadata=self._metadata, timeout=_TIMEOUT)
     except grpc.RpcError as e:
+      e = cast(grpc.Call, e)
       raise InitError(f'Could not get user from rx: {e.details()}', -1)
     return resp.username
 
   def _run_initial_rsync(self):
-    self._rsync = rsync.RsyncClient(
+    r = rsync.RsyncClient(
       self._local_cfg, remote.Remote(self._local_cfg.cwd))
-    return_code = self._rsync.to_remote()
+    return_code = r.to_remote()
     if return_code == 0:
-      logging.info('Copied files to %s', self._rsync.host)
+      logging.info('Copied files to %s', r.host)
 
   def _install_deps(self, grpc_addr: str, workspace_id: str) -> int:
     channel = grpc_helper.get_channel(grpc_addr)
     stub = rx_pb2_grpc.ExecutionServiceStub(channel)
     req = rx_pb2.InstallDepsRequest(workspace_id=workspace_id)
     resp = None
     try:
       for resp in stub.InstallDeps(
         req, metadata=self._metadata, timeout=(10 * 60)):
         if resp.stdout:
           sys.stdout.buffer.write(resp.stdout)
           sys.stdout.buffer.flush()
     except grpc.RpcError as e:
+      e = cast(grpc.Call, e)
       raise InitError(e.details(), -1)
     if resp and resp.HasField('result') and resp.result.code:
       raise InitError(resp.result.message, resp.result.code)
     return 0
 
 
 class InitError(RuntimeError):
```

### Comparing `run_rx-0.0.4/rx/client/login.py` & `run_rx-0.0.5/rx/client/login.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 import platform
 import subprocess
 import threading
 import time
 from typing import Any, Dict, Tuple
 from urllib import parse
 
-from absl import app
 from absl import flags
 from absl import logging
 import jwt
 import requests
 from requests import exceptions
 
 from rx.client.configuration import config_base
@@ -84,20 +83,21 @@
   def wait(self):
     self._code_is_set.wait()
 
 
 class LoginManager:
   """Handle browser login."""
 
-  def __init__(self) -> None:
+  def __init__(self, rxroot: pathlib.Path) -> None:
+    self._rxroot = rxroot
     self._server = None
     self._port = 0
     self._code_holder = CodeHolder()
     self._access_token = config_base.ReadOnlyConfig(
-      _get_access_token_file(), strict_mode=False)
+      _get_access_token_file(rxroot), strict_mode=False)
     if not _DO_AUTH.value:
       self.login = _no_auth_login
 
   @property
   def grpc_metadata(self) -> Tuple[Tuple[str, str]]:
     """Returns the signed ID token."""
     return (('id-token', self._access_token['id_token']),)
@@ -116,15 +116,15 @@
       "access_token": "abc...123",
       "expires_in": 3599,
       "scope": "openid https://www.googleapis.com/auth/userinfo.email",
       "token_type": "Bearer",
       "id_token": "<base64-encoded 3-part string>",
     }
     """
-    user_dir = config_base.get_config_dir() / 'user'
+    user_dir = config_base.get_config_dir(self._rxroot) / 'user'
     if not user_dir.exists():
       user_dir.mkdir(parents=True, exist_ok=True)
     if not self._access_token:
       self.start_server()
       self.open_browser()
       self.wait_for_login()
     self.validate_login()
@@ -158,19 +158,19 @@
       self._server.shutdown()
       raise AuthError(
         f'Could not find browser-opening program {cmd[0]}, are you in an SSH '
         'session?')
 
   def refresh_access_token(self):
     """Refreshes the access token when it expires."""
-    refresh_file = _get_refresh_token_file()
+    refresh_file = _get_refresh_token_file(self._rxroot)
     if not refresh_file.exists():
       # Access token was expired but the refresh token doesn't exist. Just start
       # over.
-      _delete_auth_files()
+      _delete_auth_files(self._rxroot)
       raise AuthError('Could not log in, please try again.')
     with open(refresh_file, mode='rt', encoding='utf-8') as fh:
       refresh_token = json.load(fh)
     data = {
       'client_id': _CLIENT_ID,
       'client_secret': _CLIENT_SECRET,
       'grant_type': 'refresh_token',
@@ -180,33 +180,34 @@
       resp = requests.post(
         'https://oauth2.googleapis.com/token', data=data, timeout=10)
     except exceptions.ConnectionError:
       raise AuthError(
         f'Unable to connect to oauth2.googleapis.com, is your internet up?')
     if resp.status_code != 200:
       # Refreshing went wrong, remove everything!
-      _delete_auth_files()
+      _delete_auth_files(self._rxroot)
       raise AuthError(
         f'Unable to refresh log in: {resp.reason} [{resp.status_code}]\n' +
         resp.text)
-    with _get_access_token_file().open(mode='wt', encoding='utf-8') as fh:
+    access_token = _get_access_token_file(self._rxroot)
+    with access_token.open(mode='wt', encoding='utf-8') as fh:
       fh.write(resp.text)
     self._access_token = json.loads(resp.text)
 
   def start_server(self):
     """Starts a local server in a separate thread."""
     th = threading.Thread(target=self._start_local_server)
     th.start()
 
   def validate_login(self):
     assert self._access_token
     try:
       id_token = decode_id_token(self._access_token['id_token'])
     except ValueError as e:
-      _delete_auth_files()
+      _delete_auth_files(self._rxroot)
       logging.exception(e)
       raise AuthError('Could not read token, please try logging in again.')
     if is_expired(id_token):
       self.refresh_access_token()
 
   def wait_for_login(self):
     """Shuts down the server after login."""
@@ -236,54 +237,56 @@
       'redirect_uri': f'http://localhost:{self._port}'
     }
     resp = requests.post(
       'https://oauth2.googleapis.com/token', data=data, timeout=10)
     if resp.status_code != 200:
       raise AuthError(
         f'Unable to log in: {resp.reason} [{resp.status_code}]\n{resp.text}')
-    with _get_access_token_file().open(mode='wt', encoding='utf-8') as fh:
+    access_token = _get_access_token_file(self._rxroot)
+    with access_token.open(mode='wt', encoding='utf-8') as fh:
       fh.write(resp.text)
-    with _get_refresh_token_file().open(mode='wt', encoding='utf-8') as fh:
+    refresh = _get_refresh_token_file(self._rxroot)
+    with refresh.open(mode='wt', encoding='utf-8') as fh:
       fh.write(resp.text)
     self._access_token = json.loads(resp.text)
 
   def _start_local_server(self):
     """Starts the server."""
     partial_handler = functools.partial(Handler, self._code_holder)
     self._server = http.server.HTTPServer(('localhost', 0), partial_handler)
     self._port = self._server.server_port
     self._server.serve_forever()
 
 
-def _delete_auth_files():
+def _delete_auth_files(rxroot: pathlib.Path):
   """Remove all files associated with logging in."""
-  if _get_refresh_token_file().exists():
-    _get_refresh_token_file().unlink()
-  if _get_access_token_file().exists():
-    _get_access_token_file().unlink()
+  if _get_refresh_token_file(rxroot).exists():
+    _get_refresh_token_file(rxroot).unlink()
+  if _get_access_token_file(rxroot).exists():
+    _get_access_token_file(rxroot).unlink()
 
 
 def is_expired(id_token: Dict[str, Any]) -> bool:
   """Returns if the access token is expired."""
   exp = id_token['exp']
   now = time.time()
   return now > exp
 
 
 def decode_id_token(b64: str) -> Dict[str, Any]:
   """The id_token field is a base64 encoded, .-delimited string."""
   return jwt.decode(b64, options={'verify_signature': False})
 
 
-def _get_access_token_file() -> pathlib.Path:
-  return config_base.get_config_dir() / 'user/access-token'
+def _get_access_token_file(rxroot: pathlib.Path) -> pathlib.Path:
+  return config_base.get_config_dir(rxroot) / 'user/access-token'
 
 
-def _get_refresh_token_file() -> pathlib.Path:
-  return config_base.get_config_dir() / 'user/.refresh-token'
+def _get_refresh_token_file(rxroot: pathlib.Path) -> pathlib.Path:
+  return config_base.get_config_dir(rxroot) / 'user/.refresh-token'
 
 
 def _no_auth_login() -> Dict[str, Any]:
   """Returns an auth token with email: foo@example.com."""
   assert not _DO_AUTH.value and _AUTH_EMAIL.value is not None
   id_token = jwt.encode({'email': _AUTH_EMAIL.value}, 'abc123')
   return {
@@ -293,17 +296,7 @@
     'token_type': 'Bearer',
     'id_token': id_token,
   }
 
 
 class AuthError(RuntimeError):
   pass
-
-
-def main(argv):
-  del argv
-  mf = LoginManager()
-  mf.login()
-
-
-if __name__ == '__main__':
-  app.run(main)
```

### Comparing `run_rx-0.0.4/rx/client/menu.py` & `run_rx-0.0.5/rx/client/menu.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.4/rx/client/output_handler.py` & `run_rx-0.0.5/rx/client/output_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from rx.client import rsync
 from rx.proto import rx_pb2
 
 
 class OutputHandler:
   """Handle output files and stdout/err."""
 
-  def __init__(self) -> None:
+  def __init__(self, rxroot: pathlib.Path) -> None:
+    self._rxroot = rxroot
     self._current_outputs = set()
 
   @property
   def remote_paths(self) -> List[str]:
     return sorted([f'{o}' for o in self._current_outputs])
 
   def handle(self, resp: rx_pb2.ExecResponse):
@@ -27,11 +28,11 @@
       sys.stderr.flush()
     for pth_str in resp.output_files:
       self._current_outputs.add(pathlib.Path(pth_str))
 
   def write_outputs(self, rsync_client: rsync.RsyncClient):
     if not self._current_outputs:
       return
-    rsync_client.from_remote('rx-out', pathlib.Path('rx-out'))
+    rsync_client.from_remote('rx-out', self._rxroot / pathlib.Path('rx-out'))
     print('Created outputs:')
     for pth in self.remote_paths:
       print(f'  {pth}')
```

### Comparing `run_rx-0.0.4/rx/client/rsync.py` & `run_rx-0.0.5/rx/client/rsync.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,49 @@
 from collections import abc
 import pathlib
 import subprocess
+import tempfile
 from typing import List
 
 from absl import logging
 
 from rx.client.configuration import config_base
 from rx.client.configuration import local
 
+def dry_run(local_cfg: local.LocalConfig):
+  dest = tempfile.mkdtemp()
+  cmd = [
+      local_cfg['rsync_path'],
+      '--archive',
+      '--compress',
+      '--delete',
+      '--dry-run',
+      f'--exclude-from={local_cfg.cwd / local.IGNORE}',
+      '--itemize-changes',
+      f'{local_cfg.cwd}/',
+      str(dest)]
+  result = subprocess.run(cmd, check=True, capture_output=True)
+  stdout = result.stdout.decode('utf-8')
+  print('Uploading:')
+  for ln in stdout.split('\n'):
+    delta = ln.split(' ')
+    if len(delta) < 2 or delta[1] == './':
+      continue
+    filename = delta[1]
+    tab_count = 1 + filename.count('/')
+    is_dir = False
+    if filename.endswith('/'):
+      is_dir = True
+      tab_count -= 1
+    tabs = '  ' * tab_count
+    slash = '/' if is_dir else ''
+    pretty_name = f'{pathlib.Path(filename).name}{slash}'
+    # TODO: handle file deletion.
+    print(f'{tabs}{pretty_name}')
+
 
 class RsyncClient:
   """Rsync tools."""
 
   def __init__(
       self, local_cfg: local.LocalConfig, remote_cfg: abc.Mapping):
     self._sync_dir = local_cfg.cwd
@@ -33,14 +65,15 @@
   @property
   def _upload_path(self) -> pathlib.Path:
     return pathlib.Path(self._cfg['daemon_module'])
 
   def from_remote(self, source: str, dest: pathlib.Path) -> int:
     """Copies output files from the remote machine to dest."""
     assert dest.is_dir(), f'Destination {dest} must be a directory'
+    assert dest.is_absolute(), f'Destination {dest} must be absolute'
     remote_path = self._upload_path / source
     daemon = f'{self._daemon_addr}::{remote_path}/'
     cmd = [
         self._rsync_path,
         '--archive',
         '--compress',
         '--delete',
@@ -75,9 +108,9 @@
     if e.returncode == 10:
       # Worker was unreachable.
       logging.error('stderr: %s', e.stderr)
     if e.returncode is None:
       return -1
     return e.returncode
   if result.stdout:
-    print(f'stdout: {result.stdout}')
+    print(f'stdout: {result.stdout.decode("utf-8")}')
   return 0
```

### Comparing `run_rx-0.0.4/rx/client/user.py` & `run_rx-0.0.5/rx/client/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 from rx.client.configuration import config_base
 
 _VALID_USERNAME = re.compile(r'^[a-zA-Z][\w]{2,14}$')
 
 
 class CreateUser(config_base.ReadWriteConfig):
   def __init__(self, cwd: pathlib.Path):
-    super().__init__(cwd / _get_user_config())
+    super().__init__(_get_user_config(cwd))
 
 
 class User(config_base.ReadOnlyConfig):
   """User info."""
   def __init__(self, cwd: pathlib.Path, email: str):
-    super().__init__(cwd / _get_user_config())
+    super().__init__(_get_user_config(cwd))
     if email != self['email']:
       raise RuntimeError(f'Mismatched emails: {email} vs. {self["email"]}')
 
 
 def has_config(cwd: pathlib.Path) -> bool:
-  return (cwd / _get_user_config()).exists()
+  return _get_user_config(cwd).exists()
 
 
 def username_prompt(email: str) -> str:
   """Prompts the user to choose a username."""
   return menu.string_prompt(
       f'Choose a username for {email}', validation=username_validator)
 
@@ -45,9 +45,9 @@
     elif username is not None and len(username) > 15:
       print('Error: username too long.')
     else:
       print('Error: username must contain only alphanumeric characters.')
   return is_valid
 
 
-def _get_user_config() -> pathlib.Path:
-  return config_base.get_config_dir() / 'user/config'
+def _get_user_config(rxroot: pathlib.Path) -> pathlib.Path:
+  return rxroot / config_base.get_config_dir(rxroot) / 'user/config'
```

### Comparing `run_rx-0.0.4/rx/proto/rx_pb2.py` & `run_rx-0.0.5/rx/proto/rx_pb2.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.4/rx/proto/rx_pb2.pyi` & `run_rx-0.0.5/rx/proto/rx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.4/rx/proto/rx_pb2_grpc.py` & `run_rx-0.0.5/rx/proto/rx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.4/PKG-INFO` & `run_rx-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: run-rx
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool to simplify remote execution
 Home-page: https://www.run-rx.com
 License: LICENSE.txt
 Author: Kris Chodorow
 Author-email: k.chodorow@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
@@ -21,57 +21,62 @@
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: sty (>=1.0.4,<2.0.0)
 Project-URL: Repository, https://github.com/run-rx/rx
 Description-Content-Type: text/markdown
 
 # rx
 
-Remote execution made easy.
+[rx](https://www.run-rx.com) is a command-line tool to help make remote
+execution easy.
+
+When you run rx it creates a private hosted environment in the cloud where all
+of your source code is automatically synced and any packages you need are
+installed. It automatically syncs output back to your machine and syncs local
+changes to your cloud instance.
+
+Right now rx is free to use, please give it a try and [let us know](mailto:eng@run-rx.com) what you think!
 
 ## Installation
 
-Install the latest release from pip:
+Install via pip:
 
     pip install run-rx
 
-rx uses rsync for downloads, so make sure rsync is installed on your
-system:
+rx also requires rsync to run, make sure you have it installed:
 
     which rsync
 
-If it isn't, install it with your favorite package manager:
+If not, check out [its website](https://rsync.samba.org/download.html) or your
+favorite package manager to install.
 
-    brew install rsync
-    yum install rsync
-    apt-get install rsync
-    # ...you get the idea
+## Usage
 
-## Use
+In the directory containing your project (often your git root), run:
 
-In you project's main directory, run:
+    rx init
 
-```
-rx init
-```
+This will prompt you to log in (or create an account) and allocate a machine
+in the cloud for you to use. Then it will copy your project from your local
+machine to the cloud instance and install any packages that your project needs.
 
-You only have to do this once per project (similar to `git init`).
+It may take several minutes to allocate a machine, copy your source code, and install packages (depending on your project).
 
-To execute commands on a remote machine, prefix them with `rx`:
+Once rx finishes initializing, you can run any command on your remote worker
+by prefixing it with "rx":
 
-```
-rx python foo.py
-rx ls
-rx 'echo $PATH > my-path'
-```
+    rx python my-script.py
+    rx ps ax
+    rx 'echo $PATH > my-path.txt'
 
 Check out the [getting-started](https://github.com/run-rx/getting-started) repository for more examples.
 
 ## Feedback
 
-Please file an [issue](https://github.com/run-rx/rx/issues).
+Feel free to [file an issue](https://github.com/run-rx/rx/issues) if you have
+any questions or problems!
 
 ## Testing
 
 To run tests, use:
 
 ```
 pip install -r test_requirements.txt
```

