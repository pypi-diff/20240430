# Comparing `tmp/run_rx-0.0.9.tar.gz` & `tmp/run_rx-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "run_rx-0.0.9.tar", max compression
+gzip compressed data, was "run_rx-0.1.0.tar", max compression
```

## Comparing `run_rx-0.0.9.tar` & `run_rx-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,63 @@
--rw-r--r--   0        0        0     1069 2023-05-16 20:24:41.276898 run_rx-0.0.9/LICENSE.txt
--rw-r--r--   0        0        0     1679 2023-05-19 14:53:21.015913 run_rx-0.0.9/README.md
--rw-r--r--   0        0        0      313 2023-06-01 23:35:09.526681 run_rx-0.0.9/install/.rxignore
--rw-r--r--   0        0        0      274 2023-06-04 16:34:29.656668 run_rx-0.0.9/install/README.md
--rw-r--r--   0        0        0       98 2023-05-16 20:24:41.277933 run_rx-0.0.9/install/python-cpu
--rw-r--r--   0        0        0       98 2023-06-06 18:01:13.521487 run_rx-0.0.9/install/python-gpu
--rw-r--r--   0        0        0      753 2023-06-16 21:15:22.264232 run_rx-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      300 2023-05-16 20:24:41.279362 run_rx-0.0.9/rx/__main__.py
--rw-r--r--   0        0        0     2850 2023-06-15 17:17:43.129031 run_rx-0.0.9/rx/client/commands/exec.py
--rw-r--r--   0        0        0     4059 2023-06-16 19:42:49.623110 run_rx-0.0.9/rx/client/commands/init.py
--rw-r--r--   0        0        0     2109 2023-06-04 16:41:38.419103 run_rx-0.0.9/rx/client/configuration/config_base.py
--rw-r--r--   0        0        0     7359 2023-06-16 21:15:30.004669 run_rx-0.0.9/rx/client/configuration/local.py
--rw-r--r--   0        0        0      641 2023-06-06 18:04:41.546820 run_rx-0.0.9/rx/client/configuration/remote.py
--rw-r--r--   0        0        0      256 2023-05-16 20:24:41.281715 run_rx-0.0.9/rx/client/grpc_helper.py
--rw-r--r--   0        0        0     9852 2023-06-09 00:46:28.253468 run_rx-0.0.9/rx/client/login.py
--rw-r--r--   0        0        0     2673 2023-06-16 19:40:57.513477 run_rx-0.0.9/rx/client/menu.py
--rw-r--r--   0        0        0     1092 2023-05-16 20:24:41.282728 run_rx-0.0.9/rx/client/output_handler.py
--rw-r--r--   0        0        0     3306 2023-06-06 18:01:13.524830 run_rx-0.0.9/rx/client/rsync.py
--rw-r--r--   0        0        0     4771 2023-06-15 20:17:35.649171 run_rx-0.0.9/rx/client/trex_client.py
--rw-r--r--   0        0        0     1603 2023-05-16 20:24:41.283538 run_rx-0.0.9/rx/client/user.py
--rw-r--r--   0        0        0     5565 2023-06-07 13:22:07.723770 run_rx-0.0.9/rx/client/worker_client.py
--rw-r--r--   0        0        0     6391 2023-06-06 22:54:37.232578 run_rx-0.0.9/rx/proto/rx_pb2.py
--rw-r--r--   0        0        0     8466 2023-06-06 22:54:37.232746 run_rx-0.0.9/rx/proto/rx_pb2.pyi
--rw-r--r--   0        0        0    12622 2023-06-06 22:54:37.233305 run_rx-0.0.9/rx/proto/rx_pb2_grpc.py
--rw-r--r--   0        0        0     2635 1970-01-01 00:00:00.000000 run_rx-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-16 20:24:41.276898 run_rx-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      327 2024-03-03 21:30:52.796626 run_rx-0.1.0/install/.rxignore
+-rw-r--r--   0        0        0     2198 2024-02-03 19:55:45.342016 run_rx-0.1.0/pip_readme.md
+-rw-r--r--   0        0        0      795 2024-04-29 23:52:11.293600 run_rx-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-16 13:27:24.756975 run_rx-0.1.0/rx/__init__.py
+-rw-r--r--   0        0        0      269 2023-11-08 18:10:55.603406 run_rx-0.1.0/rx/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-16 13:34:13.562117 run_rx-0.1.0/rx/client/__init__.py
+-rw-r--r--   0        0        0      802 2023-08-24 19:40:33.458484 run_rx-0.1.0/rx/client/browser.py
+-rw-r--r--   0        0        0        0 2023-08-16 13:35:22.013639 run_rx-0.1.0/rx/client/commands/__init__.py
+-rw-r--r--   0        0        0     1618 2024-02-02 23:15:34.159511 run_rx-0.1.0/rx/client/commands/command.py
+-rw-r--r--   0        0        0     4056 2024-03-07 20:25:53.167578 run_rx-0.1.0/rx/client/commands/daemon.py
+-rw-r--r--   0        0        0     3619 2024-02-17 01:52:56.913881 run_rx-0.1.0/rx/client/commands/exec.py
+-rw-r--r--   0        0        0     6190 2024-03-03 20:53:32.251343 run_rx-0.1.0/rx/client/commands/init.py
+-rw-r--r--   0        0        0     2553 2024-02-02 23:15:34.161080 run_rx-0.1.0/rx/client/commands/runner.py
+-rw-r--r--   0        0        0     1076 2024-02-02 23:15:34.161342 run_rx-0.1.0/rx/client/commands/stop.py
+-rw-r--r--   0        0        0     1303 2024-02-02 23:15:34.161610 run_rx-0.1.0/rx/client/commands/subscribe.py
+-rw-r--r--   0        0        0     1320 2024-02-02 23:15:34.162769 run_rx-0.1.0/rx/client/commands/workspace/commit.py
+-rw-r--r--   0        0        0      982 2024-02-02 23:15:34.163059 run_rx-0.1.0/rx/client/commands/workspace/info.py
+-rw-r--r--   0        0        0     2845 2024-03-05 15:59:39.643758 run_rx-0.1.0/rx/client/commands/workspace/port.py
+-rw-r--r--   0        0        0     2572 2024-02-13 22:02:18.807334 run_rx-0.1.0/rx/client/commands/workspace/set_acls.py
+-rw-r--r--   0        0        0      685 2024-02-17 01:52:56.914526 run_rx-0.1.0/rx/client/commands/ws.py
+-rw-r--r--   0        0        0        0 2023-08-16 13:35:31.872789 run_rx-0.1.0/rx/client/configuration/__init__.py
+-rw-r--r--   0        0        0     2390 2024-02-17 01:52:56.915071 run_rx-0.1.0/rx/client/configuration/config_base.py
+-rw-r--r--   0        0        0     7500 2024-04-29 23:52:11.289294 run_rx-0.1.0/rx/client/configuration/local.py
+-rw-r--r--   0        0        0      657 2023-12-24 19:35:00.194898 run_rx-0.1.0/rx/client/configuration/remote.py
+-rw-r--r--   0        0        0      260 2024-02-17 01:52:56.916315 run_rx-0.1.0/rx/client/grpc_helper.py
+-rw-r--r--   0        0        0     9630 2023-12-24 20:55:35.746396 run_rx-0.1.0/rx/client/login.py
+-rw-r--r--   0        0        0     2673 2023-09-21 20:47:26.922392 run_rx-0.1.0/rx/client/menu.py
+-rw-r--r--   0        0        0      753 2024-02-08 19:49:59.443523 run_rx-0.1.0/rx/client/output_handler.py
+-rw-r--r--   0        0        0     1724 2024-01-04 17:06:21.493329 run_rx-0.1.0/rx/client/payment.py
+-rw-r--r--   0        0        0    10576 2024-03-03 20:53:06.876589 run_rx-0.1.0/rx/client/trex_client.py
+-rw-r--r--   0        0        0     1690 2023-12-24 19:53:38.344118 run_rx-0.1.0/rx/client/user.py
+-rw-r--r--   0        0        0     8541 2024-04-22 20:21:51.068679 run_rx-0.1.0/rx/client/worker_client.py
+-rw-r--r--   0        0        0        0 2024-02-17 01:52:56.916836 run_rx-0.1.0/rx/daemon/__init__.py
+-rw-r--r--   0        0        0     2562 2024-04-28 18:39:07.740341 run_rx-0.1.0/rx/daemon/client.py
+-rw-r--r--   0        0        0     2823 2024-03-05 16:36:08.094591 run_rx-0.1.0/rx/daemon/daemon.py
+-rw-r--r--   0        0        0     2178 2024-02-21 21:11:36.691243 run_rx-0.1.0/rx/daemon/interceptors.py
+-rw-r--r--   0        0        0     4101 2024-03-05 15:52:16.314244 run_rx-0.1.0/rx/daemon/manager.py
+-rw-r--r--   0        0        0     1423 2024-02-23 18:27:38.986647 run_rx-0.1.0/rx/daemon/pidfile.py
+-rw-r--r--   0        0        0        0 2024-02-17 01:52:56.918068 run_rx-0.1.0/rx/daemon/port_forwarding/__init__.py
+-rw-r--r--   0        0        0     3598 2024-04-28 18:39:07.740721 run_rx-0.1.0/rx/daemon/port_forwarding/client_socket.py
+-rw-r--r--   0        0        0     3525 2024-04-28 18:39:07.741308 run_rx-0.1.0/rx/daemon/port_forwarding/port_forwarder.py
+-rw-r--r--   0        0        0     2530 2024-04-28 18:39:07.741859 run_rx-0.1.0/rx/daemon/port_forwarding/service.py
+-rw-r--r--   0        0        0     2359 2024-04-28 18:39:07.742340 run_rx-0.1.0/rx/daemon/server.py
+-rw-r--r--   0        0        0        0 2024-02-17 01:52:56.919377 run_rx-0.1.0/rx/proto/__init__.py
+-rw-r--r--   0        0        0     2188 2024-02-21 19:49:39.107970 run_rx-0.1.0/rx/proto/daemon_pb2.py
+-rw-r--r--   0        0        0     1645 2024-02-21 19:49:39.108034 run_rx-0.1.0/rx/proto/daemon_pb2.pyi
+-rw-r--r--   0        0        0     5944 2024-02-21 19:49:39.108095 run_rx-0.1.0/rx/proto/daemon_pb2_grpc.py
+-rw-r--r--   0        0        0    11733 2024-02-21 19:49:39.108613 run_rx-0.1.0/rx/proto/rx_pb2.py
+-rw-r--r--   0        0        0    15980 2024-02-21 19:49:39.108898 run_rx-0.1.0/rx/proto/rx_pb2.pyi
+-rw-r--r--   0        0        0    30107 2024-02-21 19:49:39.109375 run_rx-0.1.0/rx/proto/rx_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-02-02 23:15:34.166034 run_rx-0.1.0/rx/shared/__init__.py
+-rw-r--r--   0        0        0     1366 2024-02-02 23:15:34.166490 run_rx-0.1.0/rx/shared/progress_bar.py
+-rw-r--r--   0        0        0        0 2024-02-02 23:15:34.166915 run_rx-0.1.0/rx/trex/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-02 23:15:34.167013 run_rx-0.1.0/rx/trex/toolchain/__init__.py
+-rw-r--r--   0        0        0     1644 2024-02-02 23:15:34.167382 run_rx-0.1.0/rx/trex/toolchain/lang_detector.py
+-rw-r--r--   0        0        0     1482 2024-02-13 22:02:18.809919 run_rx-0.1.0/rx/trex/toolchain/local_fs.py
+-rw-r--r--   0        0        0      993 2024-02-02 23:15:34.167832 run_rx-0.1.0/rx/trex/toolchain/manifest.py
+-rw-r--r--   0        0        0     1903 2024-02-22 22:06:33.686022 run_rx-0.1.0/rx/trex/toolchain/toolchain.py
+-rw-r--r--   0        0        0        0 2024-02-02 23:15:34.168512 run_rx-0.1.0/rx/worker/__init__.py
+-rw-r--r--   0        0        0     3523 2024-04-22 20:04:26.261856 run_rx-0.1.0/rx/worker/executor.py
+-rw-r--r--   0        0        0     2810 2024-02-17 01:52:56.920498 run_rx-0.1.0/rx/worker/rsync.py
+-rw-r--r--   0        0        0     3157 1970-01-01 00:00:00.000000 run_rx-0.1.0/PKG-INFO
```

### Comparing `run_rx-0.0.9/LICENSE.txt` & `run_rx-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.9/pyproject.toml` & `run_rx-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 [tool.poetry]
 name = "run-rx"
-version = "0.0.9"
+version = "0.1.0"
 description = "A tool to simplify remote execution"
 authors = ["Kris Chodorow <k.chodorow@gmail.com>"]
 license = "LICENSE.txt"
-readme = "README.md"
+readme = "pip_readme.md"
 homepage = "https://www.run-rx.com"
 repository = "https://github.com/run-rx/rx"
 packages = [
     { include = "rx" },
 ]
 include = [
   "rx/proto/*.py",
   "rx/proto/*.pyi",
   "install/*",
 ]
 exclude = [
-  "**/*_test.py",
+  "**/test_*.py",
   "rx/proto/*.proto",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 absl-py = "^1.4.0"
 grpcio = "^1.54.0"
 protobuf = "^4.22.3"
 PyJWT = "^2.6.0"
+PyYAML = "^6.0.1"
 requests = "^2.30.0"
-sty = "^1.0.4"
 tqdm = "^4.65.0"
 
 [tool.poetry.scripts]
 rx = 'rx.client.commands.exec:run'
+rx-daemon = 'rx.daemon.server:run'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `run_rx-0.0.9/rx/client/commands/exec.py` & `run_rx-0.1.0/rx/client/commands/runner.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,105 +1,79 @@
-"""rx usage
+import argparse
 
-To set up this directory on a remote host:
-
-    rx init
-
-You only have to run this once per directory, similar to `git init`.
-
-To run a command on the remote host:
-
-    rx CMD
-
-Run 'rx --help' for more options or visit https://www.run-rx.com.
-"""
-import pathlib
-import tempfile
-from typing import List
-
-from absl import app
 from absl import logging
 
+from rx.client import trex_client
 from rx.client import worker_client
 from rx.client import grpc_helper
-from rx.client.commands import init
+from rx.client.commands import command
 from rx.client.configuration import config_base
-from rx.client.configuration import local
-from rx.client.configuration import remote
 
 
-class ExecCommand:
+class RunCommand(command.Command):
 
-  def __init__(self, argv: List[str]):
-    self._argv = argv
-    cwd = (
-      pathlib.Path(config_base.RX_ROOT.value) if config_base.RX_ROOT.value else
-      pathlib.Path.cwd())
-    self._config = local.find_local_config(cwd)
-
-  def run(self) -> int:
-    if self._config is None:
-      print ('Run `rx init` first!')
-      return -1
-    remote_cfg = remote.Remote(self._config.cwd)
-    with grpc_helper.get_channel(remote_cfg.worker_addr) as ch:
-      client = worker_client.create_authed_client(ch, self._config)
+  def __init__(self, cmdline: command.CommandLine):
+    super().__init__(cmdline)
+    self._argv = cmdline.remainder
+
+  def _run(self) -> int:
+    with grpc_helper.get_channel(self.remote_config.worker_addr) as ch:
+      client = worker_client.create_authed_client(ch, self.local_config)
       return self._try_exec(client)
 
   def _try_exec(self, client: worker_client.Client) -> int:
     """Sends the command to the server."""
     if len(self._argv) < 1:
       print('No command given.')
       return 1
 
     if len(self._argv) == 1:
       # If this is a quoted arg, break it into pieces. E.g., to pass "ls -l" it
       # must be quoted so that absl doesn't try to capture the -l.
       # TODO: is there a better way to handle this with absl flags?
       self._argv = self._argv[0].split(' ')
     try:
-      return client.exec(self._argv)
+      return client.exec(list(self._argv))
     except KeyboardInterrupt:
       client.maybe_kill()
       return worker_client.SIGINT_CODE
-    except worker_client.UnreachableError as e:
-      print(
-        f'Worker {e.worker} was unrechable, run `rx init` to get a new '
-        'instance.')
+    except worker_client.RsyncError as e:
+      # Fallthrough - retry
+      logging.info('Rsync error: %s', e)
+      pass
+    except worker_client.WorkerError as e:
+      print(e)
       return e.code
 
-
-class VersionCommand:
-  """Prints the version."""
-
-  def run(self) -> int:
-    print(local.VERSION)
-    return 0
-
-
-def main(argv):
-  logging.get_absl_handler().python_handler.use_absl_log_file(
-    program_name='rx', log_dir=tempfile.gettempdir())
-  if len(argv) == 1:
-    print('No command given.\n')
-    app.usage(shorthelp=True)
-    return -1
-  cmd_to_run = argv[1]
-  try:
-    if cmd_to_run == 'init':
-      cmd = init.InitCommand()
-    elif cmd_to_run == 'version':
-      cmd = VersionCommand()
+    # Fallthrough from retry.
+    print('Error syncing code to your worker, checking with the scheduler...')
+    return self.maybe_unfreeze()
+
+  def maybe_unfreeze(self) -> int:
+    # Connect to trex.
+    with grpc_helper.get_channel(config_base.TREX_HOST.value) as ch:
+      cli = trex_client.create_authed_client(ch, self.local_config)
+      try:
+        result = cli.get_info(self.remote_config.workspace_id)
+      except trex_client.TrexError as e:
+        print(f'{e}, run `rx init` to get a new instance')
+        return -1
+      if result.state == 'frozen':
+        result = cli.unfreeze(self.remote_config.workspace_id)
+      else:
+        print('Worker was unrechable, run `rx init` to get a new instance.')
+        return -1
+    if result.code == 0:
+      print(
+        'Done! Please rerun this command to use your newly restored workspace.')
     else:
-      if cmd_to_run == 'run':
-        # "rx run foo" is generally the same as "rx foo", but the extra "run"
-        # can be handy when running a script called "init", say, on the remote
-        # machine.
-        argv = argv[1:]
-      cmd = ExecCommand(argv[1:])
-    return cmd.run()
-  except KeyboardInterrupt:
-    return worker_client.SIGINT_CODE
+      print(
+        f'Error setting up this workspace on a new machine: {result.message}')
+    return result.code
 
 
-def run():
-  app.run(main)
+def add_parser(subparsers: argparse._SubParsersAction):
+  (
+    subparsers
+    .add_parser('run', help='Runs a command')
+    .set_defaults(cmd=RunCommand)
+  )
```

### Comparing `run_rx-0.0.9/rx/client/configuration/config_base.py` & `run_rx-0.1.0/rx/client/configuration/config_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import abc
-import json
 import pathlib
 from types import TracebackType
 from typing import Optional, Type
 
 from absl import flags
+import yaml
 
 RX_DIR = pathlib.Path('.rx')
 
 # Configuration files are placed under a directory with this name (this is just
 # to make development easier, so we can have separate configs for
 # local/dev/prod).
 TREX_HOST = flags.DEFINE_string(
@@ -16,19 +16,22 @@
 RX_ROOT = flags.DEFINE_string(
   'rxroot', None, 'The directory to use as rxroot (defaults to pwd)')
 
 
 class ReadOnlyConfig(abc.Mapping):
   def __init__(self, config_file: pathlib.Path, strict_mode: bool = True):
     self._config_file = config_file
-    if not strict_mode and not config_file.exists():
-      self._config = {}
-      return
-    with self._config_file.open(mode='rt', encoding='utf-8') as fh:
-      self._config = json.load(fh)
+    if config_file.exists():
+      with self._config_file.open(mode='rt', encoding='utf-8') as fh:
+        self._config = yaml.safe_load(fh)
+    else:
+      if strict_mode:
+        raise ConfigNotFoundError(config_file)
+      else:
+        self._config = {}
 
   def __getitem__(self, item):
     assert item in self._config, (
       f'Could not access key {item} in {self._config_file}')
     return self._config[item]
 
   def __iter__(self):
@@ -45,27 +48,35 @@
 
   def __enter__(self):
     return self
 
   def __exit__(self, exctype: Optional[Type[BaseException]],
              excinst: Optional[BaseException],
              exctb: Optional[TracebackType]) -> bool:
+    del excinst
+    del exctb
     if exctype is None:
       # Keep config file up-to-date.
       with self._config_file.open(mode='wt', encoding='utf-8') as fh:
-        json.dump(self._config, fh)
+        yaml.safe_dump(self._config, fh)
     return False
 
   def __setitem__(self, item, value):
     self._config[item] = value
 
   def __delitem__(self, item):
     self._config.__delitem__(item)
 
 
 def get_config_dir(rxroot: pathlib.Path) -> pathlib.Path:
   """Returns the absolute config directory path, e.g., /proj/.rx/t.c/config."""
   return rxroot / RX_DIR / TREX_HOST.value / 'config'
 
 
-def is_local() -> bool:
-  return TREX_HOST.value.startswith('localhost')
+def is_local(addr: str) -> bool:
+  return addr.startswith('localhost') or addr == '127.0.0.1'
+
+
+class ConfigNotFoundError(FileNotFoundError):
+  def __init__(self, pth: pathlib.Path, *args: object) -> None:
+    super().__init__(*args)
+    self.path = pth
```

### Comparing `run_rx-0.0.9/rx/client/configuration/local.py` & `run_rx-0.1.0/rx/client/configuration/local.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,137 +1,94 @@
 """All of the info we can get without going to the server."""
-import hashlib
-import json
+import dataclasses
 import pathlib
 import shutil
 import subprocess
-from typing import Optional, Tuple
+from typing import Any, Dict, Optional, Tuple
 import uuid
 
 from absl import flags
 from absl import logging
-import sty
+import yaml
 
 from rx.client.configuration import config_base
 from rx.proto import rx_pb2
 
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 
+# Port the rx-daemon listens on.
+DEFAULT_DAEMON_PORT = 8478
 IGNORE = pathlib.Path('.rxignore')
+REMOTE_DIR = config_base.RX_DIR / 'remotes'
 
 _REMOTE = flags.DEFINE_string(
   'remote', None,
   'The path to the remote configuration file to use (see .rx/README.md).')
 _RSYNC_PATH = flags.DEFINE_string('rsync_path', None, 'Path to rsync binary')
 
-_REMOTE_DIR = config_base.RX_DIR / 'remotes'
-_DEFAULT_REMOTE = _REMOTE_DIR / 'default'
+_DEFAULT_REMOTE = REMOTE_DIR / 'default'
 
 
-class LocalConfigWriter(config_base.ReadWriteConfig):
-  """This holds all of the configuration options that can be determined from
-  the local machine."""
-
-  def __init__(self, workspace_dir: pathlib.Path):
-    super().__init__(get_local_config_path(workspace_dir))
-    self._workspace_dir = workspace_dir
-
-  def setup_remote(self):
-    """Sets the "remote" field (and color) for the local config."""
-    remote = str(_REMOTE.value if _REMOTE.value else _DEFAULT_REMOTE)
-    remote_path = self._workspace_dir / remote
-    try:
-      with remote_path.open(mode='rt', encoding='utf-8') as fh:
-        remote_content = fh.read()
-        self._set_color(remote_content)
-        self['remote'] = remote
-    except FileExistsError:
-      raise FileExistsError(
-        f'Could not find remote config: {remote_path} does not exist')
-
-  def _set_color(self, s: str):
-    """Generate a random color based on the remote config."""
-    h = hashlib.blake2s(digest_size=3)
-    h.update(s.encode())
-    hash_val = int(h.hexdigest(), 16)
-    r = hash_val & 255
-    hash_val = hash_val >> 8
-    g = hash_val & 255
-    hash_val = hash_val >> 8
-    b = hash_val & 255
-    self['color'] = {'r': r, 'g': g, 'b': b}
-
-
-class LocalConfig(config_base.ReadOnlyConfig):
+@dataclasses.dataclass(frozen=True)
+class LocalConfig:
   """Create the local configuration."""
-
-  def __init__(self, working_dir: pathlib.Path):
-    super().__init__(get_local_config_path(working_dir))
-    self._cwd = working_dir
-    self.config_dir = self.cwd / config_base.RX_DIR
-    self._color = None
-
-  @property
-  def cwd(self) -> pathlib.Path:
-    return self._cwd
+  cwd: pathlib.Path
+  project_name: str
+  rsync_path: str
+  remote: str = str(_DEFAULT_REMOTE)
+  should_sync: bool = True
+  daemon_port: int = DEFAULT_DAEMON_PORT
 
   @property
   def rsync_source(self) -> rx_pb2.RsyncSource:
     return rx_pb2.RsyncSource(
       machine_id=uuid.getnode(),
       directory=str(self.cwd),
     )
 
-  def _get_source_env(self, docker_image: str) -> rx_pb2.Environment:
-    # TODO: how to automatically determine language?
-    if 'python' not in docker_image:
-      logging.info('Using a non-Python image. There be dragons here.')
-      return rx_pb2.Environment()
-    return rx_pb2.Environment(python=rx_pb2.Python())
-
   def get_target_env(self) -> rx_pb2.Environment:
-    remote_file = self.cwd / self['remote']
+    remote_file: pathlib.Path = self.cwd / self.remote
+    if not remote_file.exists():
+      return rx_pb2.Environment()
     try:
       with remote_file.open(mode='rt', encoding='utf-8') as fh:
-        remote_config = json.load(fh)
-    except json.JSONDecodeError as e:
-      logging.exception(f'Could not parse {self["remote"]}')
-      raise e
-    env = rx_pb2.Environment(alloc=rx_pb2.Remote())
-    if 'image' not in remote_config or 'docker' not in remote_config['image']:
-      raise ConfigError(
-        f'Remote config {self["remote"]} must contain "image": '
-        '{"docker": "<docker image>"}')
-    docker_image = remote_config['image']['docker']
-    env.alloc.image.CopyFrom(rx_pb2.Remote.Image(
-      docker=docker_image,
-    ))
-    if 'hardware' in remote_config and 'processor' in remote_config['hardware']:
-      env.alloc.hardware.CopyFrom(rx_pb2.Remote.Hardware(
-        processor=remote_config['hardware']['processor']
-      ))
-    env.MergeFrom(self._get_source_env(docker_image))
-    return env
-
-  def color_str(self, s: str) -> str:
-    color = self['color']
-    fg = sty.fg(color['r'], color['g'], color['b'])
-    return f'{fg}{s}{sty.rs.fg}'
-
-
-def create_local_config(rxroot: pathlib.Path) -> LocalConfig:
-  """Gets or creates .rx directory."""
-  _install_local_files(rxroot)
+        remote_config = yaml.safe_load(fh)
+    except yaml.YAMLError as e:
+      raise ConfigError(f'Could not parse yaml in {remote_file}: {e}')
+    return env_dict_to_pb(remote_config)
+
+  def store(self):
+    cfg_file = get_local_config_path(self.cwd)
+    with cfg_file.open(mode='wt', encoding='utf-8') as fh:
+      yaml.safe_dump({
+        'remote': self.remote,
+        'project_name': self.project_name,
+        'rsync_path': self.rsync_path,
+        'should_sync': self.should_sync,
+        'daemon_port': self.daemon_port,
+      }, fh)
+
+  def get_daemon_pid_file(self) -> pathlib.Path:
+    return config_base.get_config_dir(self.cwd) / 'daemon.pid'
+
+
+def create_local_config(rxroot: pathlib.Path, should_sync: bool) -> LocalConfig:
+  """Gets or creates .rx directory and local config."""
   config_dir = get_local_config_path(rxroot).parent
+  _install_rxignore(rxroot)
   config_dir.mkdir(exist_ok=True, parents=True)
-  with LocalConfigWriter(rxroot) as c:
-    c.setup_remote()
-    c['project_name'] = _find_project_name(rxroot)
-    c['rsync_path'] = _get_rsync_path()
-  return LocalConfig(rxroot)
+  cfg = LocalConfig(
+    cwd=rxroot,
+    remote=str(_REMOTE.value if _REMOTE.value else _DEFAULT_REMOTE),
+    project_name=_find_project_name(rxroot),
+    rsync_path=_get_rsync_path(),
+    should_sync=should_sync,
+  )
+  cfg.store()
+  return cfg
 
 
 def find_rxroot(working_dir: pathlib.Path) -> Optional[pathlib.Path]:
   """Finds the rxroot, if it exists."""
   cfg_path = config_base.get_config_dir(working_dir)
   for parent in cfg_path.parents:
     if config_base.get_config_dir(parent).exists():
@@ -140,53 +97,83 @@
 
 
 def find_local_config(working_dir: pathlib.Path) -> Optional[LocalConfig]:
   """Factory to create a config by looking for .rx."""
   cfg_path = config_base.get_config_dir(working_dir)
   for parent in cfg_path.parents:
     if config_base.get_config_dir(parent).exists():
-      return LocalConfig(parent)
+      return load_config(parent)
   return None
 
 
+def get_local_config() -> LocalConfig:
+  """Returns the local config, if it exists, otherwise raises ConfigNotFound."""
+  if config_base.RX_ROOT.value:
+    rxroot = pathlib.Path(config_base.RX_ROOT.value)
+  else:
+    rxroot = find_rxroot(pathlib.Path.cwd())
+    if not rxroot:
+      raise config_base.ConfigNotFoundError(
+        pathlib.Path('.'), 'Run `rx init` first!')
+  cfg = find_local_config(rxroot)
+  if not cfg:
+    raise config_base.ConfigNotFoundError(rxroot, 'Run `rx init` first!')
+  return cfg
+
+
 def get_source_path() -> pathlib.Path:
   """Gets the path bundled client files can be found on."""
   # __file__ is ./rx/client/configuration/local.py, so this resolves to ./.
   return pathlib.Path(__file__).resolve().parent.parent.parent.parent
 
 
 def get_grpc_metadata() -> Tuple[Tuple[str, str]]:
   return (('cv', VERSION),)
 
 
-def _install_local_files(rxroot: pathlib.Path):
-  # Output directory.
-  (rxroot / 'rx-out').mkdir(exist_ok=True)
-
-  install_dir = pathlib.Path(get_source_path() / 'install')
-
-  _install_file(install_dir, rxroot, IGNORE)
-
-  config_dir = rxroot / config_base.RX_DIR
-  config_dir.mkdir(exist_ok=True, parents=True)
-  _install_file(install_dir, config_dir, 'README.md')
-
-  remotes = rxroot / _REMOTE_DIR
-  remotes.mkdir(exist_ok=True, parents=True)
-
-  # Copy built-in configs.
-  _install_file(install_dir, remotes, 'python-cpu')
-  _install_file(install_dir, remotes, 'python-gpu')
-  # Create soft link.
-  default_config = remotes / 'default'
-  if default_config.exists():
-    # Don't undo someone else's config.
-    return
-  # .rx/remote/default -> python-cpu
-  default_config.symlink_to('python-cpu')
+def env_dict_to_pb(env_dict: Optional[Dict[str, Any]]) -> rx_pb2.Environment:
+  env_pb = rx_pb2.Environment()
+  if not env_dict:
+    # Empty config comes in as None.
+    return env_pb
+  if 'remote' in env_dict:
+    remote_dict = env_dict['remote']
+    remote_pb = rx_pb2.Remote()
+    if 'hardware' in remote_dict:
+      remote_pb.hardware.CopyFrom(rx_pb2.Hardware(**remote_dict['hardware']))
+    if 'toolchain' in remote_dict:
+      for tool in remote_dict['toolchain']:
+        remote_pb.toolchain.append(rx_pb2.Tool(**tool))
+    env_pb.remote.CopyFrom(remote_pb)
+  if 'image' in env_dict:
+    image_dict = env_dict['image']
+    image_pb = rx_pb2.Image()
+    if 'registry' in image_dict:
+      image_pb.registry = image_dict['registry']
+    if 'repository' in image_dict:
+      image_pb.repository = image_dict['repository']
+    if 'tag' in image_dict:
+      image_pb.tag = str(image_dict['tag'])
+    if 'environment_variables' in image_dict:
+      for k, v in image_dict['environment_variables'].items():
+        if isinstance(v, bool):
+          # YAML is a bit too helpful about type conversions.
+          v = 'true' if v else 'false'
+        image_pb.environment_variables[k] = str(v)
+    if 'ports' in image_dict:
+      ports = image_dict['ports']
+      # Ports might be a single key-value pair due to user entry.
+      if isinstance(ports, int):
+        image_pb.ports.append(ports)
+      elif isinstance(ports, list):
+        image_pb.ports.extend(image_dict['ports'])
+      else:
+        raise ConfigError(f'Invalid port config: {ports}')
+    env_pb.image.CopyFrom(image_pb)
+  return env_pb
 
 
 def _get_rsync_path() -> str:
   """Make sure rsync is installed."""
   if _RSYNC_PATH.value:
     return _RSYNC_PATH.value
   try:
@@ -207,22 +194,36 @@
   for parent in start_dir.parents:
     if (parent / '.git').exists():
       return start_dir.name
   # Maybe we haven't initialized git yet, use out name.
   return start_dir.name
 
 
+def _install_rxignore(rxroot: pathlib.Path):
+  source_path = get_source_path() / 'install' / IGNORE
+  destination_path = rxroot / IGNORE
+  if not destination_path.exists():
+    shutil.copy(source_path, destination_path)
+
+
+def load_config(rxroot: pathlib.Path) -> LocalConfig:
+  cfg_path = get_local_config_path(rxroot)
+  if not cfg_path.exists():
+    raise config_base.ConfigNotFoundError(cfg_path)
+  try:
+    with cfg_path.open(mode='rt', encoding='utf-8') as fh:
+      cfg: Dict[str, Any] = yaml.safe_load(fh)
+  except yaml.YAMLError as e:
+    raise ConfigError(f'Could not parse yaml in {cfg_path}: {e}')
+  cfg['cwd'] = rxroot
+  # Get all of the field names we expect.
+  fields = [f.name for f in dataclasses.fields(LocalConfig)]
+  return LocalConfig(**{k: v for k, v in cfg.items() if k in fields})
+
+
 def get_local_config_path(rxroot: pathlib.Path) -> pathlib.Path:
   """Return .rx/trex-dev.run-rx.com/config/local."""
   return config_base.get_config_dir(rxroot) / 'local'
 
 
-def _install_file(install_dir, config_dir, base_name):
-  """Installs a file if it doesn't already exist."""
-  source_path = install_dir / base_name
-  destination_path = config_dir / base_name
-  if not destination_path.exists():
-    shutil.copy(source_path, destination_path)
-
-
 class ConfigError(RuntimeError):
   pass
```

### Comparing `run_rx-0.0.9/rx/client/configuration/remote.py` & `run_rx-0.1.0/rx/client/configuration/remote.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 class Remote(config_base.ReadOnlyConfig):
   def __init__(self, working_dir: pathlib.Path):
     super().__init__(_get_remote_config_file(working_dir))
 
   @property
   def workspace_id(self):
-    return self['workspace_id']
+    return self._config['workspace_id']
 
   @property
   def worker_addr(self):
-    return self['worker_addr']
+    return self._config['worker_addr']
 
 
 class WritableRemote(config_base.ReadWriteConfig):
   def __init__(self, working_dir: pathlib.Path):
     super().__init__(_get_remote_config_file(working_dir))
```

### Comparing `run_rx-0.0.9/rx/client/login.py` & `run_rx-0.1.0/rx/client/login.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,38 +17,35 @@
 is more "user-facing."
 """
 import functools
 import http.cookies
 import http.server
 import json
 import pathlib
-import platform
 import subprocess
 import threading
 import time
 from typing import Any, Dict, Tuple
 from urllib import parse
 
 from absl import flags
 from absl import logging
 import jwt
 import requests
 from requests import exceptions
+import yaml
 
+from rx.client import browser
 from rx.client.configuration import config_base
 
 _DO_AUTH = flags.DEFINE_bool(
   'do_auth', True, 'Skip auth for offline development')
 _AUTH_EMAIL = flags.DEFINE_string(
   'auth_email', None, 'Email to use for offline development')
 
-_DARWIN = 'Darwin'
-_LINUX = 'Linux'
-_WINDOWS = 'Windows'
-
 # From https://console.developers.google.com/apis/credentials
 _CLIENT_ID = '909912915303-enmim0gms3hfsdv7c9m6p79vovjkf4vd.apps.googleusercontent.com'
 _CLIENT_SECRET = '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'
 
 
 class Handler(http.server.SimpleHTTPRequestHandler):
   """Handle the response from accounts.google.com."""
@@ -61,14 +58,17 @@
     parsed_url = parse.urlparse(self.path)
     code = parse.parse_qs(parsed_url.query)['code'][0]
     self._holder.set_code(code)
     self.send_response(200)
     self.end_headers()
     self.wfile.write(b'All set, feel free to close this tab')
 
+  def log_message(self, format: str, *args: Any) -> None:
+    logging.info(format, *args)
+
 
 class CodeHolder:
   def __init__(self) -> None:
     self._code_is_set = threading.Event()
     self._code = None
 
   @property
@@ -131,71 +131,60 @@
     return self._access_token
 
   def open_browser(self):
     """Opens the browser to the login page."""
     while self._server is None:
       time.sleep(1)
     url = self._create_login_url()
-    system = platform.system()
-    if system == _DARWIN:
-      cmd = ['open', url]
-    elif system == _LINUX:
-      cmd = ['xdg-open', url]
-    elif system == _WINDOWS:
-      logging.info(
-          'I can\'t imagine this is going to work on Windows, but feel free to '
-          'give it a try and report back')
-      cmd = ['cmd', '/c', 'start', url.replace('&', '^&')]
-    else:
-      raise RuntimeError(f'Unsupported system: {system}')
     try:
-      subprocess.run(cmd, check=True, capture_output=True)
+      browser.open_browser(url)
     except subprocess.CalledProcessError as e:
-      if e.stdout:
-        print(e.stdout)
       self._server.shutdown()
       raise AuthError(f'Error opening browser: {e}')
     except FileNotFoundError as e:
       self._server.shutdown()
       raise AuthError(
-        f'Could not find browser-opening program {cmd[0]}, are you in an SSH '
+        f'Could not find browser-opening program, are you in an SSH '
         'session?')
 
   def refresh_access_token(self):
     """Refreshes the access token when it expires."""
     refresh_file = _get_refresh_token_file(self._rxroot)
     if not refresh_file.exists():
       # Access token was expired but the refresh token doesn't exist. Just start
       # over.
       _delete_auth_files(self._rxroot)
       raise AuthError('Could not log in, please try again.')
     with open(refresh_file, mode='rt', encoding='utf-8') as fh:
-      refresh_token = json.load(fh)
+      refresh_token = yaml.safe_load(fh)
     data = {
       'client_id': _CLIENT_ID,
       'client_secret': _CLIENT_SECRET,
       'grant_type': 'refresh_token',
       'refresh_token': refresh_token['refresh_token']
     }
     try:
       resp = requests.post(
         'https://oauth2.googleapis.com/token', data=data, timeout=10)
     except exceptions.ConnectionError:
       raise AuthError(
-        f'Unable to connect to oauth2.googleapis.com, is your internet up?')
+        'Unable to connect to oauth2.googleapis.com, is your internet up?')
+    except exceptions.ReadTimeout:
+      raise AuthError(
+        'Timed out connecting to oauth2.googleapis.com, is your internet up?')
     if resp.status_code != 200:
       # Refreshing went wrong, remove everything!
       _delete_auth_files(self._rxroot)
       raise AuthError(
         f'Unable to refresh log in: {resp.reason} [{resp.status_code}]\n' +
         resp.text)
-    access_token = _get_access_token_file(self._rxroot)
-    with access_token.open(mode='wt', encoding='utf-8') as fh:
-      fh.write(resp.text)
+    access_token_file = _get_access_token_file(self._rxroot)
     self._access_token = json.loads(resp.text)
+    with access_token_file.open(mode='wt', encoding='utf-8') as fh:
+      yaml.safe_dump(self._access_token, fh)
 
   def start_server(self):
     """Starts a local server in a separate thread."""
     th = threading.Thread(target=self._start_local_server)
     th.start()
 
   def validate_login(self):
@@ -237,21 +226,21 @@
       'redirect_uri': f'http://localhost:{self._port}'
     }
     resp = requests.post(
       'https://oauth2.googleapis.com/token', data=data, timeout=10)
     if resp.status_code != 200:
       raise AuthError(
         f'Unable to log in: {resp.reason} [{resp.status_code}]\n{resp.text}')
-    access_token = _get_access_token_file(self._rxroot)
-    with access_token.open(mode='wt', encoding='utf-8') as fh:
-      fh.write(resp.text)
-    refresh = _get_refresh_token_file(self._rxroot)
-    with refresh.open(mode='wt', encoding='utf-8') as fh:
-      fh.write(resp.text)
+    access_token_file = _get_access_token_file(self._rxroot)
     self._access_token = json.loads(resp.text)
+    with access_token_file.open(mode='wt', encoding='utf-8') as fh:
+      yaml.safe_dump(self._access_token, fh)
+    refresh_file = _get_refresh_token_file(self._rxroot)
+    with refresh_file.open(mode='wt', encoding='utf-8') as fh:
+      yaml.safe_dump(self._access_token, fh)
 
   def _start_local_server(self):
     """Starts the server."""
     partial_handler = functools.partial(Handler, self._code_holder)
     self._server = http.server.HTTPServer(('localhost', 0), partial_handler)
     self._port = self._server.server_port
     self._server.serve_forever()
@@ -280,19 +269,19 @@
 def needs_login(rxroot: pathlib.Path) -> bool:
   return not (
     _get_access_token_file(rxroot).exists() and
     _get_refresh_token_file(rxroot).exists())
 
 
 def _get_access_token_file(rxroot: pathlib.Path) -> pathlib.Path:
-  return config_base.get_config_dir(rxroot) / 'user/access-token'
+  return config_base.get_config_dir(rxroot) / 'user/access-token.yaml'
 
 
 def _get_refresh_token_file(rxroot: pathlib.Path) -> pathlib.Path:
-  return config_base.get_config_dir(rxroot) / 'user/.refresh-token'
+  return config_base.get_config_dir(rxroot) / 'user/.refresh-token.yaml'
 
 
 def _no_auth_login() -> Dict[str, Any]:
   """Returns an auth token with email: foo@example.com."""
   assert not _DO_AUTH.value and _AUTH_EMAIL.value is not None
   id_token = jwt.encode({'email': _AUTH_EMAIL.value}, 'abc123')
   return {
```

### Comparing `run_rx-0.0.9/rx/client/menu.py` & `run_rx-0.1.0/rx/client/menu.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.9/rx/client/output_handler.py` & `run_rx-0.1.0/rx/client/output_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,27 @@
 """Handle outputs from the server."""
 import pathlib
-import sys
-from typing import List
+from typing import Set
 
-from rx.client import rsync
+from rx.worker import rsync
 from rx.proto import rx_pb2
 
 
 class OutputHandler:
   """Handle output files and stdout/err."""
 
   def __init__(self, rxroot: pathlib.Path) -> None:
     self._rxroot = rxroot
-    self._current_outputs = set()
-
-  @property
-  def remote_paths(self) -> List[str]:
-    return sorted([f'{o}' for o in self._current_outputs])
+    self._current_outputs: Set[pathlib.Path] = set()
 
   def handle(self, resp: rx_pb2.ExecResponse):
-    """Shows output & error streams and creates output files."""
-    if resp.stdout:
-      sys.stdout.buffer.write(resp.stdout)
-      sys.stdout.flush()
-    if resp.stderr:
-      sys.stderr.buffer.write(resp.stderr)
-      sys.stderr.flush()
+    """Creates output files."""
     for pth_str in resp.output_files:
       self._current_outputs.add(pathlib.Path(pth_str))
 
   def write_outputs(self, rsync_client: rsync.RsyncClient):
     if not self._current_outputs:
       return
-    rsync_client.from_remote('rx-out', self._rxroot / pathlib.Path('rx-out'))
-    print('Created outputs:')
-    for pth in self.remote_paths:
+    rsync_client.from_remote('.', self._rxroot)
+    print('Changed:')
+    for pth in sorted(self._current_outputs):
       print(f'  {pth}')
```

### Comparing `run_rx-0.0.9/rx/client/user.py` & `run_rx-0.1.0/rx/client/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,17 +15,21 @@
 class CreateUser(config_base.ReadWriteConfig):
   def __init__(self, cwd: pathlib.Path):
     super().__init__(_get_user_config(cwd))
 
 
 class User(config_base.ReadOnlyConfig):
   """User info."""
-  def __init__(self, cwd: pathlib.Path, email: str):
+  def __init__(
+      self,
+      cwd: pathlib.Path,
+      email: Optional[str] = None,
+      strict: bool = True):
     super().__init__(_get_user_config(cwd))
-    if email != self['email']:
+    if strict and email != self._config['email']:
       raise RuntimeError(f'Mismatched emails: {email} vs. {self["email"]}')
 
 
 def has_config(cwd: pathlib.Path) -> bool:
   return _get_user_config(cwd).exists()
 
 
@@ -46,8 +50,8 @@
       print('Error: username too long.')
     else:
       print('Error: username must contain only alphanumeric characters.')
   return is_valid
 
 
 def _get_user_config(rxroot: pathlib.Path) -> pathlib.Path:
-  return rxroot / config_base.get_config_dir(rxroot) / 'user/config'
+  return rxroot / config_base.get_config_dir(rxroot) / 'user/config.yaml'
```

### Comparing `run_rx-0.0.9/rx/proto/rx_pb2.py` & `run_rx-0.1.0/rx/proto/rx_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,65 +10,99 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11rx/proto/rx.proto\x12\x02rx\x1a\x1bgoogle/protobuf/empty.proto\"\x95\x01\n\x06Remote\x12\x1f\n\x05image\x18\x01 \x01(\x0b\x32\x10.rx.Remote.Image\x12%\n\x08hardware\x18\x02 \x01(\x0b\x32\x13.rx.Remote.Hardware\x1a$\n\x05Image\x12\x0e\n\x06\x64ocker\x18\x01 \x01(\t\x12\x0b\n\x03tag\x18\x02 \x01(\t\x1a\x1d\n\x08Hardware\x12\x11\n\tprocessor\x18\x01 \x01(\t\"\x08\n\x06Python\"D\n\x0b\x45nvironment\x12\x19\n\x05\x61lloc\x18\x01 \x01(\x0b\x32\n.rx.Remote\x12\x1a\n\x06python\x18\x02 \x01(\x0b\x32\n.rx.Python\"?\n\x05\x44\x65lta\x12\x10\n\x08\x61\x64\x64_path\x18\x01 \x03(\t\x12\x0f\n\x07\x61\x64\x64_dir\x18\x02 \x03(\t\x12\x13\n\x0bremove_path\x18\x03 \x03(\t\"U\n\x17\x44ockerImagePullProgress\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\r\n\x05total\x18\x03 \x01(\x05\x12\x0f\n\x07\x63urrent\x18\x04 \x01(\x05\"7\n\x06Result\x12\x1c\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x0e.rx.StatusCode\x12\x0f\n\x07message\x18\x02 \x01(\t\"H\n\x0bRsyncSource\x12\x12\n\nmachine_id\x18\x01 \x01(\x03\x12\x11\n\tdirectory\x18\x02 \x01(\t\x12\x12\n\npublic_key\x18\x03 \x01(\x0c\")\n\x10RsyncDestination\x12\x15\n\rdaemon_module\x18\x01 \x01(\t\"X\n\x0b\x45xecRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\x12\x0c\n\x04\x61rgv\x18\x02 \x03(\t\x12%\n\x0crsync_source\x18\x03 \x01(\x0b\x32\x0f.rx.RsyncSource\"v\n\x0c\x45xecResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x14\n\x0c\x65xecution_id\x18\x02 \x01(\t\x12\x0e\n\x06stdout\x18\x03 \x01(\x0c\x12\x0e\n\x06stderr\x18\x04 \x01(\x0c\x12\x14\n\x0coutput_files\x18\x05 \x03(\t\"?\n\x0fGetUserResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x10\n\x08username\x18\x02 \x01(\t\"o\n\x0bInitRequest\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12%\n\x0crsync_source\x18\x02 \x01(\x0b\x32\x0f.rx.RsyncSource\x12#\n\ntarget_env\x18\x03 \x01(\x0b\x32\x0f.rx.Environment\"\x7f\n\x0cInitResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12(\n\nrsync_dest\x18\x02 \x01(\x0b\x32\x14.rx.RsyncDestination\x12\x13\n\x0bworker_addr\x18\x03 \x01(\t\x12\x14\n\x0cworkspace_id\x18\x04 \x01(\t\"*\n\x12InstallDepsRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\"A\n\x13InstallDepsResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x0e\n\x06stdout\x18\x02 \x01(\x0c\"9\n\x0bKillRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\x12\x14\n\x0c\x65xecution_id\x18\x02 \x01(\t\"&\n\x12SetUsernameRequest\x12\x10\n\x08username\x18\x01 \x01(\t\"1\n\x13SetUsernameResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\")\n\x11WorkerInitRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\"d\n\x12WorkerInitResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x32\n\rpull_progress\x18\x02 \x01(\x0b\x32\x1b.rx.DockerImagePullProgress*O\n\nStatusCode\x12\x06\n\x02OK\x10\x00\x12\x0b\n\x07UNKNOWN\x10\x01\x12\x0b\n\x07INVALID\x10\x02\x12\r\n\tNOT_FOUND\x10\x03\x12\x10\n\x0cUNAUTHORIZED\x10\x04\x32\xf3\x01\n\x10\x45xecutionService\x12\x39\n\x04Init\x12\x15.rx.WorkerInitRequest\x1a\x16.rx.WorkerInitResponse\"\x00\x30\x01\x12\x42\n\x0bInstallDeps\x12\x16.rx.InstallDepsRequest\x1a\x17.rx.InstallDepsResponse\"\x00\x30\x01\x12-\n\x04\x45xec\x12\x0f.rx.ExecRequest\x1a\x10.rx.ExecResponse\"\x00\x30\x01\x12\x31\n\x04Kill\x12\x0f.rx.KillRequest\x1a\x16.google.protobuf.Empty\"\x00\x32\xb7\x01\n\x0cSetupService\x12\x38\n\x07GetUser\x12\x16.google.protobuf.Empty\x1a\x13.rx.GetUserResponse\"\x00\x12+\n\x04Init\x12\x0f.rx.InitRequest\x1a\x10.rx.InitResponse\"\x00\x12@\n\x0bSetUsername\x12\x16.rx.SetUsernameRequest\x1a\x17.rx.SetUsernameResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11rx/proto/rx.proto\x12\x02rx\x1a\x1bgoogle/protobuf/empty.proto\"\x1d\n\x08Hardware\x12\x11\n\tprocessor\x18\x01 \x01(\t\"\xca\x01\n\x05Image\x12\x10\n\x08registry\x18\x01 \x01(\t\x12\x12\n\nrepository\x18\x02 \x01(\t\x12\x0b\n\x03tag\x18\x03 \x01(\t\x12\r\n\x05ports\x18\x04 \x03(\x05\x12\x42\n\x15\x65nvironment_variables\x18\x05 \x03(\x0b\x32#.rx.Image.EnvironmentVariablesEntry\x1a;\n\x19\x45nvironmentVariablesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"%\n\x04Tool\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\"E\n\x06Remote\x12\x1e\n\x08hardware\x18\x01 \x01(\x0b\x32\x0c.rx.Hardware\x12\x1b\n\ttoolchain\x18\x02 \x03(\x0b\x32\x08.rx.Tool\"C\n\x0b\x45nvironment\x12\x1a\n\x06remote\x18\x01 \x01(\x0b\x32\n.rx.Remote\x12\x18\n\x05image\x18\x02 \x01(\x0b\x32\t.rx.Image\"?\n\x05\x44\x65lta\x12\x10\n\x08\x61\x64\x64_path\x18\x01 \x03(\t\x12\x0f\n\x07\x61\x64\x64_dir\x18\x02 \x03(\t\x12\x13\n\x0bremove_path\x18\x03 \x03(\t\"Q\n\x13\x44ockerImageProgress\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\r\n\x05total\x18\x03 \x01(\x03\x12\x0f\n\x07\x63urrent\x18\x04 \x01(\x03\"%\n\rSubscribeInfo\x12\x14\n\x0cpayment_link\x18\x01 \x01(\t\"7\n\x06Result\x12\x1c\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x0e.rx.StatusCode\x12\x0f\n\x07message\x18\x02 \x01(\t\"H\n\x0bRsyncSource\x12\x12\n\nmachine_id\x18\x01 \x01(\x03\x12\x11\n\tdirectory\x18\x02 \x01(\t\x12\x12\n\npublic_key\x18\x03 \x01(\x0c\"(\n\tGitSource\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x63ommit\x18\x02 \x01(\t\")\n\x10RsyncDestination\x12\x15\n\rdaemon_module\x18\x01 \x01(\t\":\n\tExecution\x12\x0b\n\x03\x63md\x18\x01 \x01(\t\x12\x10\n\x08start_ts\x18\x02 \x01(\x03\x12\x0e\n\x06\x65nd_ts\x18\x03 \x01(\x03\"&\n\x0eGenericRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\"-\n\x0fGenericResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\"x\n\x0b\x45xecRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\x12\x0c\n\x04\x61rgv\x18\x02 \x03(\t\x12)\n\x0crsync_source\x18\x03 \x01(\x0b\x32\x0f.rx.RsyncSourceB\x02\x18\x01\x12\x0b\n\x03\x63wd\x18\x04 \x01(\t\x12\r\n\x05stdin\x18\x05 \x01(\x0c\"\x89\x01\n\x0c\x45xecResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x14\n\x0c\x65xecution_id\x18\x02 \x01(\t\x12\x0e\n\x06stdout\x18\x03 \x01(\x0c\x12\x0e\n\x06stderr\x18\x04 \x01(\x0c\x12\x14\n\x0coutput_files\x18\x05 \x03(\t\x12\x11\n\texit_code\x18\x06 \x01(\x05\"G\n\x12PortForwardRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\r\n\x05\x66rame\x18\x03 \x01(\x0c\"@\n\x13PortForwardResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\r\n\x05\x66rame\x18\x02 \x01(\x0c\"a\n\x18GetSubscribeInfoResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12)\n\x0esubscribe_info\x18\x02 \x01(\x0b\x32\x11.rx.SubscribeInfo\"?\n\x0fGetUserResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x10\n\x08username\x18\x02 \x01(\t\"\x8b\x01\n\x18GetWorkspaceInfoResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\r\n\x05state\x18\x02 \x01(\t\x12\x1e\n\x07history\x18\x03 \x03(\x0b\x32\r.rx.Execution\x12$\n\x0b\x65nvironment\x18\x04 \x01(\x0b\x32\x0f.rx.Environment\"\xa7\x01\n\x0bInitRequest\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12%\n\x0crsync_source\x18\x02 \x01(\x0b\x32\x0f.rx.RsyncSource\x12#\n\ntarget_env\x18\x03 \x01(\x0b\x32\x0f.rx.Environment\x12\x13\n\x0bsource_type\x18\x04 \x01(\t\x12!\n\ngit_source\x18\x05 \x01(\x0b\x32\r.rx.GitSource\"\x7f\n\x0cInitResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12(\n\nrsync_dest\x18\x02 \x01(\x0b\x32\x14.rx.RsyncDestination\x12\x13\n\x0bworker_addr\x18\x03 \x01(\t\x12\x14\n\x0cworkspace_id\x18\x04 \x01(\t\"A\n\x13InstallDepsResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x0e\n\x06stdout\x18\x02 \x01(\x0c\"9\n\x0bKillRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\x12\x14\n\x0c\x65xecution_id\x18\x02 \x01(\t\"C\n\x10UnfreezeResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x13\n\x0bworker_addr\x18\x02 \x01(\t\"\x8e\x01\n\x0eSetAclsRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x13\n\x0bresource_id\x18\x03 \x01(\t\x12\x12\n\nvisibility\x18\x04 \x01(\t\x12\x12\n\nadd_reader\x18\x05 \x01(\t\x12\x12\n\nadd_writer\x18\x06 \x01(\t\"R\n\x0fSetAclsResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x12\n\nvisibility\x18\x02 \x01(\t\x12\x0f\n\x07readers\x18\x03 \x03(\t\"&\n\x12SetUsernameRequest\x12\x10\n\x08username\x18\x01 \x01(\t\"O\n\x13\x43ommitStreamRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\x12\x14\n\x0corganization\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\"b\n\x14\x43ommitStreamResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12.\n\rpush_progress\x18\x02 \x01(\x0b\x32\x17.rx.DockerImageProgress\"L\n\x14\x43ommitFinishResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x18\n\x05image\x18\x02 \x01(\x0b\x32\t.rx.Image\"1\n\x0bStopRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\x12\x0c\n\x04save\x18\x02 \x01(\x08\"t\n\x0cStopResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12.\n\rpush_progress\x18\x02 \x01(\x0b\x32\x17.rx.DockerImageProgress\x12\x18\n\x05image\x18\x03 \x01(\x0b\x32\t.rx.Image\"`\n\x12WorkerInitResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12.\n\rpull_progress\x18\x02 \x01(\x0b\x32\x17.rx.DockerImageProgress*\x92\x01\n\nStatusCode\x12\x06\n\x02OK\x10\x00\x12\x0b\n\x07UNKNOWN\x10\x01\x12\x0b\n\x07INVALID\x10\x02\x12\r\n\tNOT_FOUND\x10\x03\x12\x10\n\x0cUNAUTHORIZED\x10\x04\x12\x19\n\x15SUBSCRIPTION_REQUIRED\x10\x05\x12\n\n\x06\x45\x41GAIN\x10\x0b\x12\x0e\n\nEADDRINUSE\x10p\x12\n\n\x05MOVED\x10\xad\x02\x32\xed\x02\n\x10\x45xecutionService\x12\x36\n\x04Init\x12\x12.rx.GenericRequest\x1a\x16.rx.WorkerInitResponse\"\x00\x30\x01\x12>\n\x0bInstallDeps\x12\x12.rx.GenericRequest\x1a\x17.rx.InstallDepsResponse\"\x00\x30\x01\x12/\n\x04\x45xec\x12\x0f.rx.ExecRequest\x1a\x10.rx.ExecResponse\"\x00(\x01\x30\x01\x12\x31\n\x04Kill\x12\x0f.rx.KillRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x37\n\nSetupRsync\x12\x12.rx.GenericRequest\x1a\x13.rx.GenericResponse\"\x00\x12\x44\n\x0bPortForward\x12\x16.rx.PortForwardRequest\x1a\x17.rx.PortForwardResponse\"\x00(\x01\x30\x01\x32\xef\x05\n\x0cSetupService\x12\x42\n\x11\x43heckSubscription\x12\x16.google.protobuf.Empty\x1a\x13.rx.GenericResponse\"\x00\x12\x45\n\x0c\x43ommitStream\x12\x17.rx.CommitStreamRequest\x1a\x18.rx.CommitStreamResponse\"\x00\x30\x01\x12>\n\x0c\x43ommitFinish\x12\x12.rx.GenericRequest\x1a\x18.rx.CommitFinishResponse\"\x00\x12J\n\x10GetSubscribeInfo\x12\x16.google.protobuf.Empty\x1a\x1c.rx.GetSubscribeInfoResponse\"\x00\x12\x38\n\x07GetUser\x12\x16.google.protobuf.Empty\x1a\x13.rx.GetUserResponse\"\x00\x12\x46\n\x10GetWorkspaceInfo\x12\x12.rx.GenericRequest\x1a\x1c.rx.GetWorkspaceInfoResponse\"\x00\x12+\n\x04Init\x12\x0f.rx.InitRequest\x1a\x10.rx.InitResponse\"\x00\x12\x38\n\x08Unfreeze\x12\x12.rx.GenericRequest\x1a\x14.rx.UnfreezeResponse\"\x00\x30\x01\x12\x34\n\x07SetAcls\x12\x12.rx.SetAclsRequest\x1a\x13.rx.SetAclsResponse\"\x00\x12<\n\x0bSetUsername\x12\x16.rx.SetUsernameRequest\x1a\x13.rx.GenericResponse\"\x00\x12-\n\x04Stop\x12\x0f.rx.StopRequest\x1a\x10.rx.StopResponse\"\x00\x30\x01\x12<\n\x0bUnsubscribe\x12\x16.google.protobuf.Empty\x1a\x13.rx.GenericResponse\"\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'rx.proto.rx_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _STATUSCODE._serialized_start=1535
-  _STATUSCODE._serialized_end=1614
-  _REMOTE._serialized_start=55
-  _REMOTE._serialized_end=204
-  _REMOTE_IMAGE._serialized_start=137
-  _REMOTE_IMAGE._serialized_end=173
-  _REMOTE_HARDWARE._serialized_start=175
-  _REMOTE_HARDWARE._serialized_end=204
-  _PYTHON._serialized_start=206
-  _PYTHON._serialized_end=214
-  _ENVIRONMENT._serialized_start=216
-  _ENVIRONMENT._serialized_end=284
-  _DELTA._serialized_start=286
-  _DELTA._serialized_end=349
-  _DOCKERIMAGEPULLPROGRESS._serialized_start=351
-  _DOCKERIMAGEPULLPROGRESS._serialized_end=436
-  _RESULT._serialized_start=438
-  _RESULT._serialized_end=493
-  _RSYNCSOURCE._serialized_start=495
-  _RSYNCSOURCE._serialized_end=567
-  _RSYNCDESTINATION._serialized_start=569
-  _RSYNCDESTINATION._serialized_end=610
-  _EXECREQUEST._serialized_start=612
-  _EXECREQUEST._serialized_end=700
-  _EXECRESPONSE._serialized_start=702
-  _EXECRESPONSE._serialized_end=820
-  _GETUSERRESPONSE._serialized_start=822
-  _GETUSERRESPONSE._serialized_end=885
-  _INITREQUEST._serialized_start=887
-  _INITREQUEST._serialized_end=998
-  _INITRESPONSE._serialized_start=1000
-  _INITRESPONSE._serialized_end=1127
-  _INSTALLDEPSREQUEST._serialized_start=1129
-  _INSTALLDEPSREQUEST._serialized_end=1171
-  _INSTALLDEPSRESPONSE._serialized_start=1173
-  _INSTALLDEPSRESPONSE._serialized_end=1238
-  _KILLREQUEST._serialized_start=1240
-  _KILLREQUEST._serialized_end=1297
-  _SETUSERNAMEREQUEST._serialized_start=1299
-  _SETUSERNAMEREQUEST._serialized_end=1337
-  _SETUSERNAMERESPONSE._serialized_start=1339
-  _SETUSERNAMERESPONSE._serialized_end=1388
-  _WORKERINITREQUEST._serialized_start=1390
-  _WORKERINITREQUEST._serialized_end=1431
-  _WORKERINITRESPONSE._serialized_start=1433
-  _WORKERINITRESPONSE._serialized_end=1533
-  _EXECUTIONSERVICE._serialized_start=1617
-  _EXECUTIONSERVICE._serialized_end=1860
-  _SETUPSERVICE._serialized_start=1863
-  _SETUPSERVICE._serialized_end=2046
+  _IMAGE_ENVIRONMENTVARIABLESENTRY._options = None
+  _IMAGE_ENVIRONMENTVARIABLESENTRY._serialized_options = b'8\001'
+  _EXECREQUEST.fields_by_name['rsync_source']._options = None
+  _EXECREQUEST.fields_by_name['rsync_source']._serialized_options = b'\030\001'
+  _STATUSCODE._serialized_start=3016
+  _STATUSCODE._serialized_end=3162
+  _HARDWARE._serialized_start=54
+  _HARDWARE._serialized_end=83
+  _IMAGE._serialized_start=86
+  _IMAGE._serialized_end=288
+  _IMAGE_ENVIRONMENTVARIABLESENTRY._serialized_start=229
+  _IMAGE_ENVIRONMENTVARIABLESENTRY._serialized_end=288
+  _TOOL._serialized_start=290
+  _TOOL._serialized_end=327
+  _REMOTE._serialized_start=329
+  _REMOTE._serialized_end=398
+  _ENVIRONMENT._serialized_start=400
+  _ENVIRONMENT._serialized_end=467
+  _DELTA._serialized_start=469
+  _DELTA._serialized_end=532
+  _DOCKERIMAGEPROGRESS._serialized_start=534
+  _DOCKERIMAGEPROGRESS._serialized_end=615
+  _SUBSCRIBEINFO._serialized_start=617
+  _SUBSCRIBEINFO._serialized_end=654
+  _RESULT._serialized_start=656
+  _RESULT._serialized_end=711
+  _RSYNCSOURCE._serialized_start=713
+  _RSYNCSOURCE._serialized_end=785
+  _GITSOURCE._serialized_start=787
+  _GITSOURCE._serialized_end=827
+  _RSYNCDESTINATION._serialized_start=829
+  _RSYNCDESTINATION._serialized_end=870
+  _EXECUTION._serialized_start=872
+  _EXECUTION._serialized_end=930
+  _GENERICREQUEST._serialized_start=932
+  _GENERICREQUEST._serialized_end=970
+  _GENERICRESPONSE._serialized_start=972
+  _GENERICRESPONSE._serialized_end=1017
+  _EXECREQUEST._serialized_start=1019
+  _EXECREQUEST._serialized_end=1139
+  _EXECRESPONSE._serialized_start=1142
+  _EXECRESPONSE._serialized_end=1279
+  _PORTFORWARDREQUEST._serialized_start=1281
+  _PORTFORWARDREQUEST._serialized_end=1352
+  _PORTFORWARDRESPONSE._serialized_start=1354
+  _PORTFORWARDRESPONSE._serialized_end=1418
+  _GETSUBSCRIBEINFORESPONSE._serialized_start=1420
+  _GETSUBSCRIBEINFORESPONSE._serialized_end=1517
+  _GETUSERRESPONSE._serialized_start=1519
+  _GETUSERRESPONSE._serialized_end=1582
+  _GETWORKSPACEINFORESPONSE._serialized_start=1585
+  _GETWORKSPACEINFORESPONSE._serialized_end=1724
+  _INITREQUEST._serialized_start=1727
+  _INITREQUEST._serialized_end=1894
+  _INITRESPONSE._serialized_start=1896
+  _INITRESPONSE._serialized_end=2023
+  _INSTALLDEPSRESPONSE._serialized_start=2025
+  _INSTALLDEPSRESPONSE._serialized_end=2090
+  _KILLREQUEST._serialized_start=2092
+  _KILLREQUEST._serialized_end=2149
+  _UNFREEZERESPONSE._serialized_start=2151
+  _UNFREEZERESPONSE._serialized_end=2218
+  _SETACLSREQUEST._serialized_start=2221
+  _SETACLSREQUEST._serialized_end=2363
+  _SETACLSRESPONSE._serialized_start=2365
+  _SETACLSRESPONSE._serialized_end=2447
+  _SETUSERNAMEREQUEST._serialized_start=2449
+  _SETUSERNAMEREQUEST._serialized_end=2487
+  _COMMITSTREAMREQUEST._serialized_start=2489
+  _COMMITSTREAMREQUEST._serialized_end=2568
+  _COMMITSTREAMRESPONSE._serialized_start=2570
+  _COMMITSTREAMRESPONSE._serialized_end=2668
+  _COMMITFINISHRESPONSE._serialized_start=2670
+  _COMMITFINISHRESPONSE._serialized_end=2746
+  _STOPREQUEST._serialized_start=2748
+  _STOPREQUEST._serialized_end=2797
+  _STOPRESPONSE._serialized_start=2799
+  _STOPRESPONSE._serialized_end=2915
+  _WORKERINITRESPONSE._serialized_start=2917
+  _WORKERINITRESPONSE._serialized_end=3013
+  _EXECUTIONSERVICE._serialized_start=3165
+  _EXECUTIONSERVICE._serialized_end=3530
+  _SETUPSERVICE._serialized_start=3533
+  _SETUPSERVICE._serialized_end=4284
 # @@protoc_insertion_point(module_scope)
```

### Comparing `run_rx-0.0.9/rx/proto/rx_pb2.pyi` & `run_rx-0.1.0/rx/proto/rx_pb2.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -2,110 +2,221 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
+EADDRINUSE: StatusCode
+EAGAIN: StatusCode
 INVALID: StatusCode
+MOVED: StatusCode
 NOT_FOUND: StatusCode
 OK: StatusCode
+SUBSCRIPTION_REQUIRED: StatusCode
 UNAUTHORIZED: StatusCode
 UNKNOWN: StatusCode
 
+class CommitFinishResponse(_message.Message):
+    __slots__ = ["image", "result"]
+    IMAGE_FIELD_NUMBER: _ClassVar[int]
+    RESULT_FIELD_NUMBER: _ClassVar[int]
+    image: Image
+    result: Result
+    def __init__(self, result: _Optional[_Union[Result, _Mapping]] = ..., image: _Optional[_Union[Image, _Mapping]] = ...) -> None: ...
+
+class CommitStreamRequest(_message.Message):
+    __slots__ = ["name", "organization", "workspace_id"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    ORGANIZATION_FIELD_NUMBER: _ClassVar[int]
+    WORKSPACE_ID_FIELD_NUMBER: _ClassVar[int]
+    name: str
+    organization: str
+    workspace_id: str
+    def __init__(self, workspace_id: _Optional[str] = ..., organization: _Optional[str] = ..., name: _Optional[str] = ...) -> None: ...
+
+class CommitStreamResponse(_message.Message):
+    __slots__ = ["push_progress", "result"]
+    PUSH_PROGRESS_FIELD_NUMBER: _ClassVar[int]
+    RESULT_FIELD_NUMBER: _ClassVar[int]
+    push_progress: DockerImageProgress
+    result: Result
+    def __init__(self, result: _Optional[_Union[Result, _Mapping]] = ..., push_progress: _Optional[_Union[DockerImageProgress, _Mapping]] = ...) -> None: ...
+
 class Delta(_message.Message):
     __slots__ = ["add_dir", "add_path", "remove_path"]
     ADD_DIR_FIELD_NUMBER: _ClassVar[int]
     ADD_PATH_FIELD_NUMBER: _ClassVar[int]
     REMOVE_PATH_FIELD_NUMBER: _ClassVar[int]
     add_dir: _containers.RepeatedScalarFieldContainer[str]
     add_path: _containers.RepeatedScalarFieldContainer[str]
     remove_path: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, add_path: _Optional[_Iterable[str]] = ..., add_dir: _Optional[_Iterable[str]] = ..., remove_path: _Optional[_Iterable[str]] = ...) -> None: ...
 
-class DockerImagePullProgress(_message.Message):
+class DockerImageProgress(_message.Message):
     __slots__ = ["current", "id", "status", "total"]
     CURRENT_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     TOTAL_FIELD_NUMBER: _ClassVar[int]
     current: int
     id: str
     status: str
     total: int
     def __init__(self, id: _Optional[str] = ..., status: _Optional[str] = ..., total: _Optional[int] = ..., current: _Optional[int] = ...) -> None: ...
 
 class Environment(_message.Message):
-    __slots__ = ["alloc", "python"]
-    ALLOC_FIELD_NUMBER: _ClassVar[int]
-    PYTHON_FIELD_NUMBER: _ClassVar[int]
-    alloc: Remote
-    python: Python
-    def __init__(self, alloc: _Optional[_Union[Remote, _Mapping]] = ..., python: _Optional[_Union[Python, _Mapping]] = ...) -> None: ...
+    __slots__ = ["image", "remote"]
+    IMAGE_FIELD_NUMBER: _ClassVar[int]
+    REMOTE_FIELD_NUMBER: _ClassVar[int]
+    image: Image
+    remote: Remote
+    def __init__(self, remote: _Optional[_Union[Remote, _Mapping]] = ..., image: _Optional[_Union[Image, _Mapping]] = ...) -> None: ...
 
 class ExecRequest(_message.Message):
-    __slots__ = ["argv", "rsync_source", "workspace_id"]
+    __slots__ = ["argv", "cwd", "rsync_source", "stdin", "workspace_id"]
     ARGV_FIELD_NUMBER: _ClassVar[int]
+    CWD_FIELD_NUMBER: _ClassVar[int]
     RSYNC_SOURCE_FIELD_NUMBER: _ClassVar[int]
+    STDIN_FIELD_NUMBER: _ClassVar[int]
     WORKSPACE_ID_FIELD_NUMBER: _ClassVar[int]
     argv: _containers.RepeatedScalarFieldContainer[str]
+    cwd: str
     rsync_source: RsyncSource
+    stdin: bytes
     workspace_id: str
-    def __init__(self, workspace_id: _Optional[str] = ..., argv: _Optional[_Iterable[str]] = ..., rsync_source: _Optional[_Union[RsyncSource, _Mapping]] = ...) -> None: ...
+    def __init__(self, workspace_id: _Optional[str] = ..., argv: _Optional[_Iterable[str]] = ..., rsync_source: _Optional[_Union[RsyncSource, _Mapping]] = ..., cwd: _Optional[str] = ..., stdin: _Optional[bytes] = ...) -> None: ...
 
 class ExecResponse(_message.Message):
-    __slots__ = ["execution_id", "output_files", "result", "stderr", "stdout"]
+    __slots__ = ["execution_id", "exit_code", "output_files", "result", "stderr", "stdout"]
     EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
+    EXIT_CODE_FIELD_NUMBER: _ClassVar[int]
     OUTPUT_FILES_FIELD_NUMBER: _ClassVar[int]
     RESULT_FIELD_NUMBER: _ClassVar[int]
     STDERR_FIELD_NUMBER: _ClassVar[int]
     STDOUT_FIELD_NUMBER: _ClassVar[int]
     execution_id: str
+    exit_code: int
     output_files: _containers.RepeatedScalarFieldContainer[str]
     result: Result
     stderr: bytes
     stdout: bytes
-    def __init__(self, result: _Optional[_Union[Result, _Mapping]] = ..., execution_id: _Optional[str] = ..., stdout: _Optional[bytes] = ..., stderr: _Optional[bytes] = ..., output_files: _Optional[_Iterable[str]] = ...) -> None: ...
+    def __init__(self, result: _Optional[_Union[Result, _Mapping]] = ..., execution_id: _Optional[str] = ..., stdout: _Optional[bytes] = ..., stderr: _Optional[bytes] = ..., output_files: _Optional[_Iterable[str]] = ..., exit_code: _Optional[int] = ...) -> None: ...
+
+class Execution(_message.Message):
+    __slots__ = ["cmd", "end_ts", "start_ts"]
+    CMD_FIELD_NUMBER: _ClassVar[int]
+    END_TS_FIELD_NUMBER: _ClassVar[int]
+    START_TS_FIELD_NUMBER: _ClassVar[int]
+    cmd: str
+    end_ts: int
+    start_ts: int
+    def __init__(self, cmd: _Optional[str] = ..., start_ts: _Optional[int] = ..., end_ts: _Optional[int] = ...) -> None: ...
+
+class GenericRequest(_message.Message):
+    __slots__ = ["workspace_id"]
+    WORKSPACE_ID_FIELD_NUMBER: _ClassVar[int]
+    workspace_id: str
+    def __init__(self, workspace_id: _Optional[str] = ...) -> None: ...
+
+class GenericResponse(_message.Message):
+    __slots__ = ["result"]
+    RESULT_FIELD_NUMBER: _ClassVar[int]
+    result: Result
+    def __init__(self, result: _Optional[_Union[Result, _Mapping]] = ...) -> None: ...
+
+class GetSubscribeInfoResponse(_message.Message):
+    __slots__ = ["result", "subscribe_info"]
+    RESULT_FIELD_NUMBER: _ClassVar[int]
+    SUBSCRIBE_INFO_FIELD_NUMBER: _ClassVar[int]
+    result: Result
+    subscribe_info: SubscribeInfo
+    def __init__(self, result: _Optional[_Union[Result, _Mapping]] = ..., subscribe_info: _Optional[_Union[SubscribeInfo, _Mapping]] = ...) -> None: ...
 
 class GetUserResponse(_message.Message):
     __slots__ = ["result", "username"]
     RESULT_FIELD_NUMBER: _ClassVar[int]
     USERNAME_FIELD_NUMBER: _ClassVar[int]
     result: Result
     username: str
     def __init__(self, result: _Optional[_Union[Result, _Mapping]] = ..., username: _Optional[str] = ...) -> None: ...
 
+class GetWorkspaceInfoResponse(_message.Message):
+    __slots__ = ["environment", "history", "result", "state"]
+    ENVIRONMENT_FIELD_NUMBER: _ClassVar[int]
+    HISTORY_FIELD_NUMBER: _ClassVar[int]
+    RESULT_FIELD_NUMBER: _ClassVar[int]
+    STATE_FIELD_NUMBER: _ClassVar[int]
+    environment: Environment
+    history: _containers.RepeatedCompositeFieldContainer[Execution]
+    result: Result
+    state: str
+    def __init__(self, result: _Optional[_Union[Result, _Mapping]] = ..., state: _Optional[str] = ..., history: _Optional[_Iterable[_Union[Execution, _Mapping]]] = ..., environment: _Optional[_Union[Environment, _Mapping]] = ...) -> None: ...
+
+class GitSource(_message.Message):
+    __slots__ = ["commit", "url"]
+    COMMIT_FIELD_NUMBER: _ClassVar[int]
+    URL_FIELD_NUMBER: _ClassVar[int]
+    commit: str
+    url: str
+    def __init__(self, url: _Optional[str] = ..., commit: _Optional[str] = ...) -> None: ...
+
+class Hardware(_message.Message):
+    __slots__ = ["processor"]
+    PROCESSOR_FIELD_NUMBER: _ClassVar[int]
+    processor: str
+    def __init__(self, processor: _Optional[str] = ...) -> None: ...
+
+class Image(_message.Message):
+    __slots__ = ["environment_variables", "ports", "registry", "repository", "tag"]
+    class EnvironmentVariablesEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    ENVIRONMENT_VARIABLES_FIELD_NUMBER: _ClassVar[int]
+    PORTS_FIELD_NUMBER: _ClassVar[int]
+    REGISTRY_FIELD_NUMBER: _ClassVar[int]
+    REPOSITORY_FIELD_NUMBER: _ClassVar[int]
+    TAG_FIELD_NUMBER: _ClassVar[int]
+    environment_variables: _containers.ScalarMap[str, str]
+    ports: _containers.RepeatedScalarFieldContainer[int]
+    registry: str
+    repository: str
+    tag: str
+    def __init__(self, registry: _Optional[str] = ..., repository: _Optional[str] = ..., tag: _Optional[str] = ..., ports: _Optional[_Iterable[int]] = ..., environment_variables: _Optional[_Mapping[str, str]] = ...) -> None: ...
+
 class InitRequest(_message.Message):
-    __slots__ = ["project_name", "rsync_source", "target_env"]
+    __slots__ = ["git_source", "project_name", "rsync_source", "source_type", "target_env"]
+    GIT_SOURCE_FIELD_NUMBER: _ClassVar[int]
     PROJECT_NAME_FIELD_NUMBER: _ClassVar[int]
     RSYNC_SOURCE_FIELD_NUMBER: _ClassVar[int]
+    SOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
     TARGET_ENV_FIELD_NUMBER: _ClassVar[int]
+    git_source: GitSource
     project_name: str
     rsync_source: RsyncSource
+    source_type: str
     target_env: Environment
-    def __init__(self, project_name: _Optional[str] = ..., rsync_source: _Optional[_Union[RsyncSource, _Mapping]] = ..., target_env: _Optional[_Union[Environment, _Mapping]] = ...) -> None: ...
+    def __init__(self, project_name: _Optional[str] = ..., rsync_source: _Optional[_Union[RsyncSource, _Mapping]] = ..., target_env: _Optional[_Union[Environment, _Mapping]] = ..., source_type: _Optional[str] = ..., git_source: _Optional[_Union[GitSource, _Mapping]] = ...) -> None: ...
 
 class InitResponse(_message.Message):
     __slots__ = ["result", "rsync_dest", "worker_addr", "workspace_id"]
     RESULT_FIELD_NUMBER: _ClassVar[int]
     RSYNC_DEST_FIELD_NUMBER: _ClassVar[int]
     WORKER_ADDR_FIELD_NUMBER: _ClassVar[int]
     WORKSPACE_ID_FIELD_NUMBER: _ClassVar[int]
     result: Result
     rsync_dest: RsyncDestination
     worker_addr: str
     workspace_id: str
     def __init__(self, result: _Optional[_Union[Result, _Mapping]] = ..., rsync_dest: _Optional[_Union[RsyncDestination, _Mapping]] = ..., worker_addr: _Optional[str] = ..., workspace_id: _Optional[str] = ...) -> None: ...
 
-class InstallDepsRequest(_message.Message):
-    __slots__ = ["workspace_id"]
-    WORKSPACE_ID_FIELD_NUMBER: _ClassVar[int]
-    workspace_id: str
-    def __init__(self, workspace_id: _Optional[str] = ...) -> None: ...
-
 class InstallDepsResponse(_message.Message):
     __slots__ = ["result", "stdout"]
     RESULT_FIELD_NUMBER: _ClassVar[int]
     STDOUT_FIELD_NUMBER: _ClassVar[int]
     result: Result
     stdout: bytes
     def __init__(self, result: _Optional[_Union[Result, _Mapping]] = ..., stdout: _Optional[bytes] = ...) -> None: ...
@@ -114,37 +225,39 @@
     __slots__ = ["execution_id", "workspace_id"]
     EXECUTION_ID_FIELD_NUMBER: _ClassVar[int]
     WORKSPACE_ID_FIELD_NUMBER: _ClassVar[int]
     execution_id: str
     workspace_id: str
     def __init__(self, workspace_id: _Optional[str] = ..., execution_id: _Optional[str] = ...) -> None: ...
 
-class Python(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
+class PortForwardRequest(_message.Message):
+    __slots__ = ["frame", "port", "workspace_id"]
+    FRAME_FIELD_NUMBER: _ClassVar[int]
+    PORT_FIELD_NUMBER: _ClassVar[int]
+    WORKSPACE_ID_FIELD_NUMBER: _ClassVar[int]
+    frame: bytes
+    port: int
+    workspace_id: str
+    def __init__(self, workspace_id: _Optional[str] = ..., port: _Optional[int] = ..., frame: _Optional[bytes] = ...) -> None: ...
+
+class PortForwardResponse(_message.Message):
+    __slots__ = ["frame", "result"]
+    FRAME_FIELD_NUMBER: _ClassVar[int]
+    RESULT_FIELD_NUMBER: _ClassVar[int]
+    frame: bytes
+    result: Result
+    def __init__(self, result: _Optional[_Union[Result, _Mapping]] = ..., frame: _Optional[bytes] = ...) -> None: ...
 
 class Remote(_message.Message):
-    __slots__ = ["hardware", "image"]
-    class Hardware(_message.Message):
-        __slots__ = ["processor"]
-        PROCESSOR_FIELD_NUMBER: _ClassVar[int]
-        processor: str
-        def __init__(self, processor: _Optional[str] = ...) -> None: ...
-    class Image(_message.Message):
-        __slots__ = ["docker", "tag"]
-        DOCKER_FIELD_NUMBER: _ClassVar[int]
-        TAG_FIELD_NUMBER: _ClassVar[int]
-        docker: str
-        tag: str
-        def __init__(self, docker: _Optional[str] = ..., tag: _Optional[str] = ...) -> None: ...
+    __slots__ = ["hardware", "toolchain"]
     HARDWARE_FIELD_NUMBER: _ClassVar[int]
-    IMAGE_FIELD_NUMBER: _ClassVar[int]
-    hardware: Remote.Hardware
-    image: Remote.Image
-    def __init__(self, image: _Optional[_Union[Remote.Image, _Mapping]] = ..., hardware: _Optional[_Union[Remote.Hardware, _Mapping]] = ...) -> None: ...
+    TOOLCHAIN_FIELD_NUMBER: _ClassVar[int]
+    hardware: Hardware
+    toolchain: _containers.RepeatedCompositeFieldContainer[Tool]
+    def __init__(self, hardware: _Optional[_Union[Hardware, _Mapping]] = ..., toolchain: _Optional[_Iterable[_Union[Tool, _Mapping]]] = ...) -> None: ...
 
 class Result(_message.Message):
     __slots__ = ["code", "message"]
     CODE_FIELD_NUMBER: _ClassVar[int]
     MESSAGE_FIELD_NUMBER: _ClassVar[int]
     code: StatusCode
     message: str
@@ -162,35 +275,89 @@
     MACHINE_ID_FIELD_NUMBER: _ClassVar[int]
     PUBLIC_KEY_FIELD_NUMBER: _ClassVar[int]
     directory: str
     machine_id: int
     public_key: bytes
     def __init__(self, machine_id: _Optional[int] = ..., directory: _Optional[str] = ..., public_key: _Optional[bytes] = ...) -> None: ...
 
+class SetAclsRequest(_message.Message):
+    __slots__ = ["add_reader", "add_writer", "resource_id", "resource_type", "visibility", "workspace_id"]
+    ADD_READER_FIELD_NUMBER: _ClassVar[int]
+    ADD_WRITER_FIELD_NUMBER: _ClassVar[int]
+    RESOURCE_ID_FIELD_NUMBER: _ClassVar[int]
+    RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
+    VISIBILITY_FIELD_NUMBER: _ClassVar[int]
+    WORKSPACE_ID_FIELD_NUMBER: _ClassVar[int]
+    add_reader: str
+    add_writer: str
+    resource_id: str
+    resource_type: str
+    visibility: str
+    workspace_id: str
+    def __init__(self, workspace_id: _Optional[str] = ..., resource_type: _Optional[str] = ..., resource_id: _Optional[str] = ..., visibility: _Optional[str] = ..., add_reader: _Optional[str] = ..., add_writer: _Optional[str] = ...) -> None: ...
+
+class SetAclsResponse(_message.Message):
+    __slots__ = ["readers", "result", "visibility"]
+    READERS_FIELD_NUMBER: _ClassVar[int]
+    RESULT_FIELD_NUMBER: _ClassVar[int]
+    VISIBILITY_FIELD_NUMBER: _ClassVar[int]
+    readers: _containers.RepeatedScalarFieldContainer[str]
+    result: Result
+    visibility: str
+    def __init__(self, result: _Optional[_Union[Result, _Mapping]] = ..., visibility: _Optional[str] = ..., readers: _Optional[_Iterable[str]] = ...) -> None: ...
+
 class SetUsernameRequest(_message.Message):
     __slots__ = ["username"]
     USERNAME_FIELD_NUMBER: _ClassVar[int]
     username: str
     def __init__(self, username: _Optional[str] = ...) -> None: ...
 
-class SetUsernameResponse(_message.Message):
-    __slots__ = ["result"]
+class StopRequest(_message.Message):
+    __slots__ = ["save", "workspace_id"]
+    SAVE_FIELD_NUMBER: _ClassVar[int]
+    WORKSPACE_ID_FIELD_NUMBER: _ClassVar[int]
+    save: bool
+    workspace_id: str
+    def __init__(self, workspace_id: _Optional[str] = ..., save: bool = ...) -> None: ...
+
+class StopResponse(_message.Message):
+    __slots__ = ["image", "push_progress", "result"]
+    IMAGE_FIELD_NUMBER: _ClassVar[int]
+    PUSH_PROGRESS_FIELD_NUMBER: _ClassVar[int]
     RESULT_FIELD_NUMBER: _ClassVar[int]
+    image: Image
+    push_progress: DockerImageProgress
     result: Result
-    def __init__(self, result: _Optional[_Union[Result, _Mapping]] = ...) -> None: ...
+    def __init__(self, result: _Optional[_Union[Result, _Mapping]] = ..., push_progress: _Optional[_Union[DockerImageProgress, _Mapping]] = ..., image: _Optional[_Union[Image, _Mapping]] = ...) -> None: ...
 
-class WorkerInitRequest(_message.Message):
-    __slots__ = ["workspace_id"]
-    WORKSPACE_ID_FIELD_NUMBER: _ClassVar[int]
-    workspace_id: str
-    def __init__(self, workspace_id: _Optional[str] = ...) -> None: ...
+class SubscribeInfo(_message.Message):
+    __slots__ = ["payment_link"]
+    PAYMENT_LINK_FIELD_NUMBER: _ClassVar[int]
+    payment_link: str
+    def __init__(self, payment_link: _Optional[str] = ...) -> None: ...
+
+class Tool(_message.Message):
+    __slots__ = ["name", "version"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    VERSION_FIELD_NUMBER: _ClassVar[int]
+    name: str
+    version: str
+    def __init__(self, name: _Optional[str] = ..., version: _Optional[str] = ...) -> None: ...
+
+class UnfreezeResponse(_message.Message):
+    __slots__ = ["result", "worker_addr"]
+    RESULT_FIELD_NUMBER: _ClassVar[int]
+    WORKER_ADDR_FIELD_NUMBER: _ClassVar[int]
+    result: Result
+    worker_addr: str
+    def __init__(self, result: _Optional[_Union[Result, _Mapping]] = ..., worker_addr: _Optional[str] = ...) -> None: ...
 
 class WorkerInitResponse(_message.Message):
     __slots__ = ["pull_progress", "result"]
     PULL_PROGRESS_FIELD_NUMBER: _ClassVar[int]
     RESULT_FIELD_NUMBER: _ClassVar[int]
-    pull_progress: DockerImagePullProgress
+    pull_progress: DockerImageProgress
     result: Result
-    def __init__(self, result: _Optional[_Union[Result, _Mapping]] = ..., pull_progress: _Optional[_Union[DockerImagePullProgress, _Mapping]] = ...) -> None: ...
+    def __init__(self, result: _Optional[_Union[Result, _Mapping]] = ..., pull_progress: _Optional[_Union[DockerImageProgress, _Mapping]] = ...) -> None: ...
 
 class StatusCode(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
```

### Comparing `run_rx-0.0.9/PKG-INFO` & `run_rx-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,91 @@
 Metadata-Version: 2.1
 Name: run-rx
-Version: 0.0.9
+Version: 0.1.0
 Summary: A tool to simplify remote execution
 Home-page: https://www.run-rx.com
 License: LICENSE.txt
 Author: Kris Chodorow
 Author-email: k.chodorow@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
+Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: absl-py (>=1.4.0,<2.0.0)
 Requires-Dist: grpcio (>=1.54.0,<2.0.0)
 Requires-Dist: protobuf (>=4.22.3,<5.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
-Requires-Dist: sty (>=1.0.4,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/run-rx/rx
 Description-Content-Type: text/markdown
 
-# rx
-
-[rx](https://www.run-rx.com) is a command-line tool to help make remote
-execution easy.
-
-When you run rx it creates a private hosted environment in the cloud where all
-of your source code is automatically synced and any packages you need are
-installed. It automatically syncs output back to your machine and syncs local
-changes to your cloud instance.
-
-Right now rx is free to use, please give it a try and [let us know](mailto:eng@run-rx.com) what you think!
-
-## Installation
-
-Install via pip:
-
-    pip install run-rx
-
-rx also requires rsync to run, make sure you have it installed:
-
-    which rsync
-
-If not, check out [its website](https://rsync.samba.org/download.html) or your
-favorite package manager to install.
+[rx](https://www.run-rx.com) is a command-line tool that makes it easy to
+create, use, and share development environments. It integrates with whatever
+tools you're currently using and gives you a long-running VM in the cloud that
+is kept in sync with your local machine.
 
 ## Usage
 
 In the directory containing your project (often your git root), run:
 
     rx init
 
 This will prompt you to log in (or create an account) and allocate a machine
 in the cloud for you to use. Then it will copy your project from your local
 machine to the cloud instance and install any packages that your project needs.
 
-It may take several minutes to allocate a machine, copy your source code, and install packages (depending on your project).
+It may take several minutes to allocate a machine, copy your source code, and
+install packages (depending on your project).
 
 Once rx finishes initializing, you can run any command on your remote worker
 by prefixing it with "rx":
 
     rx python my-script.py
     rx ps ax
     rx 'echo $PATH > my-path.txt'
 
-Check out the [getting-started](https://github.com/run-rx/getting-started) repository for more examples.
+Check out the [getting-started](https://www.run-rx.com/getting-started/)
+section for more examples.
+
+## What rx does
+
+When you run rx it takes care of a bunch of cloud setup tasks on your behalf:
+
+* It creates a private hosted environment for your project in the cloud.
+* It copies your source code into that environment.
+* It installs any dependencies your project needs.
+
+Then, every time you run a command, it automatically syncs local changes to
+your cloud instance and syncs outputs back to your local machine. rx hosts
+your environment on our own cloud instances, so you never have to worry about
+setup or teardown.
+
+Check out the [getting started](https://www.run-rx.com/getting-started) guide
+to start using rx in less than five minutes.
+
+*Note: the `rx` binary is a thin client and does not run commands on your local
+machine: it sends them to your cloud instance and runs them there.*
+
+We'd love to hear what you think of rx and how you're using it! Please let us
+know by emailing eng@run-rx.com or filing an issue on
+[GitHub](https://github.com/run-rx/rx/issues)!
 
 ## Feedback
 
 Feel free to [file an issue](https://github.com/run-rx/rx/issues) if you have
-any questions or problems!
+any questions or problems.
 
-## Testing
+## Running tests
 
-To run tests, use:
+Run tests with:
 
 ```
-pip install -r test_requirements.txt
-PYTHONPATH=. pytest
+pip install -r requirements_dev.txt
+python run_tests.py
 ```
```

