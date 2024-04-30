# Comparing `tmp/pm2-0.0.3.tar.gz` & `tmp/pm2-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm2-0.0.3.tar", last modified: Mon Mar 25 13:29:19 2024, max compression
+gzip compressed data, was "pm2-0.0.4.tar", last modified: Tue Apr 30 09:31:04 2024, max compression
```

## Comparing `pm2-0.0.3.tar` & `pm2-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 13:29:19.400897 pm2-0.0.3/
--rw-rw-rw-   0        0        0    35802 2024-03-25 12:38:03.000000 pm2-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     4907 2024-03-25 13:29:19.398870 pm2-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3222 2024-03-25 12:51:25.000000 pm2-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-25 13:29:19.315073 pm2-0.0.3/pm2/
--rw-rw-rw-   0        0        0    10252 2024-03-25 13:20:11.000000 pm2-0.0.3/pm2/__init__.py
--rw-rw-rw-   0        0        0        0 2024-03-25 12:40:39.000000 pm2-0.0.3/pm2/__main__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 13:29:19.395878 pm2-0.0.3/pm2.egg-info/
--rw-rw-rw-   0        0        0     4907 2024-03-25 13:29:18.000000 pm2-0.0.3/pm2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-03-25 13:29:18.000000 pm2-0.0.3/pm2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 13:29:18.000000 pm2-0.0.3/pm2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-25 13:29:18.000000 pm2-0.0.3/pm2.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       22 2024-03-25 13:29:18.000000 pm2-0.0.3/pm2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-03-25 13:29:18.000000 pm2-0.0.3/pm2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-25 13:29:19.400897 pm2-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1999 2024-03-25 13:16:02.000000 pm2-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 09:31:04.151445 pm2-0.0.4/
+-rw-rw-rw-   0        0        0    35803 2024-04-30 09:18:53.000000 pm2-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4840 2024-04-30 09:31:04.097407 pm2-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3318 2024-04-30 09:18:53.000000 pm2-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 09:31:04.047449 pm2-0.0.4/pm2/
+-rw-rw-rw-   0        0        0    10307 2024-04-30 09:23:19.000000 pm2-0.0.4/pm2/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 09:18:53.000000 pm2-0.0.4/pm2/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 09:31:04.091451 pm2-0.0.4/pm2.egg-info/
+-rw-rw-rw-   0        0        0     4840 2024-04-30 09:31:03.000000 pm2-0.0.4/pm2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-04-30 09:31:03.000000 pm2-0.0.4/pm2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 09:31:03.000000 pm2-0.0.4/pm2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-30 09:28:40.000000 pm2-0.0.4/pm2.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       22 2024-04-30 09:31:03.000000 pm2-0.0.4/pm2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-30 09:31:03.000000 pm2-0.0.4/pm2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 09:31:04.152408 pm2-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2052 2024-04-30 09:22:44.000000 pm2-0.0.4/setup.py
```

### Comparing `pm2-0.0.3/LICENSE` & `pm2-0.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -667,8 +667,8 @@
 <https://www.gnu.org/licenses/>.
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `pm2-0.0.3/PKG-INFO` & `pm2-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pm2
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python wrapper for PM2
 Home-page: https://github.com/y4kupkaya/pm2
 Author: y4kupkaya
 Author-email: contact@yakupkaya.net.tr
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Keywords: process-manager,pm2,pm2-py
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,16 +27,14 @@
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aylak==0.0.6
-Requires-Dist: aiofiles
 
 
 # PM2 Python Library for Process Management
 
 ## Introduction
 
 This Python library provides a seamless integration with PM2, enabling users to automate the launching and management of processes using PM2 through Python. Designed to cater to developers and system administrators who require a programmable interface to control their processes with the power and flexibility of Python, this library simplifies interactions with PM2, making it more accessible and versatile.
@@ -128,17 +126,17 @@
 
 Contributions are welcome! If you would like to contribute, please follow these steps:
 
 1. Fork the repository.
 2. Create a new branch for your feature.
 3. Add your changes and commit them.
 4. Push to your branch.
-5. Create a pull request. 
+5. Create a pull request.
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](https://github.com/y4kupkaya/pm2-python-lib/LICENSE) file for details.
+This project is licensed under the MIT License - see the [LICENSE](https://github.com/y4kupkaya/pm2/LICENSE) file for details.
 
 ## Acknowledgments
 
 - Thanks to the PM2 team for creating such a powerful process manager.
-- This library was inspired by the need to simplify process management in Python projects. 
+- This library was inspired by the need to simplify process management in Python projects.
```

### Comparing `pm2-0.0.3/README.md` & `pm2-0.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-
-# PM2 Python Library for Process Management
-
-## Introduction
-
-This Python library provides a seamless integration with PM2, enabling users to automate the launching and management of processes using PM2 through Python. Designed to cater to developers and system administrators who require a programmable interface to control their processes with the power and flexibility of Python, this library simplifies interactions with PM2, making it more accessible and versatile.
-
-## Features
-
-- **Easy Process Management:** Start, stop, restart, and delete processes with simple Python functions.
-- **Automatic Process Launch:** Automatically launch multiple processes with predefined configurations.
-- **Real-time Process Monitoring:** Retrieve real-time information about process status, CPU, and memory usage.
-- **Flexible Configuration:** Configure processes programmatically, including environment variables, names, and log file locations.
-- **Event Handling:** Listen to and handle PM2 events directly within your Python scripts.
-
-## Installation
-
-To install the PM2 Python Library, run the following command:
-
-```bash
-pip install pm2
-```
-
-## Quick Start
-
-To get started with the PM2 Python Library, here's a simple example that demonstrates how to start a process:
-
-```python
-from pm2 import PM2, AioPM2
-import asyncio
-
-pm2 = PM2()
-aiopm2 = AioPM2()
-
-
-# Sync Methods
-def pm2_manager():
-    # List all processes
-    processes = pm2.list()
-    print(processes)
-
-    # Start a process
-    pm2.start(
-        "your_script.py",
-        name="Script-Name",
-        extra_args=["-arg1", "value1"],
-        name="YourProcessName",
-    )
-    # Restart a process
-    pm2.restart(name="Script-Name")  # or pid=12345 or pm_id=1
-
-    # Stop a process
-    pm2.stop(name="Script-Name")  # or pid=12345 or pm_id=1
-
-    # Delete a process
-    pm2.delete(name="Script-Name")  # or pid=12345 or pm_id=1
-
-
-# Async Methods
-async def pm2_manager():
-    # List all processes
-    processes = await aiopm2.list()
-    print(processes)
-
-    # Start a process
-    await aiopm2.start(
-        "your_script.py",
-        name="Script-Name",
-        extra_args=["-arg1", "value1"],
-        name="Script-Name",
-    )
-
-    # Restart a process
-    await aiopm2.restart(name="Script-Name")  # or pid=12345 or pm_id=1
-
-    # Stop a process
-    await aiopm2.stop(name="Script-Name")  # or pid=12345 or pm_id=1
-
-    # Delete a process
-    await aiopm2.delete(name="Script-Name")  # or pid=12345 or pm_id=1
-
-
-# Run the function
-pm2_manager()
-# or
-asyncio.run(pm2_manager())
-```
-
-Replace `'your_script.py'`, `'Script-Name'`, and the args as necessary to fit your needs.
-
-## Contributing
-
-Contributions are welcome! If you would like to contribute, please follow these steps:
-
-1. Fork the repository.
-2. Create a new branch for your feature.
-3. Add your changes and commit them.
-4. Push to your branch.
-5. Create a pull request. 
-
-## License
-
-This project is licensed under the MIT License - see the [LICENSE](https://github.com/y4kupkaya/pm2-python-lib/LICENSE) file for details.
-
-## Acknowledgments
-
-- Thanks to the PM2 team for creating such a powerful process manager.
-- This library was inspired by the need to simplify process management in Python projects. 
+
+# PM2 Python Library for Process Management
+
+## Introduction
+
+This Python library provides a seamless integration with PM2, enabling users to automate the launching and management of processes using PM2 through Python. Designed to cater to developers and system administrators who require a programmable interface to control their processes with the power and flexibility of Python, this library simplifies interactions with PM2, making it more accessible and versatile.
+
+## Features
+
+- **Easy Process Management:** Start, stop, restart, and delete processes with simple Python functions.
+- **Automatic Process Launch:** Automatically launch multiple processes with predefined configurations.
+- **Real-time Process Monitoring:** Retrieve real-time information about process status, CPU, and memory usage.
+- **Flexible Configuration:** Configure processes programmatically, including environment variables, names, and log file locations.
+- **Event Handling:** Listen to and handle PM2 events directly within your Python scripts.
+
+## Installation
+
+To install the PM2 Python Library, run the following command:
+
+```bash
+pip install pm2
+```
+
+## Quick Start
+
+To get started with the PM2 Python Library, here's a simple example that demonstrates how to start a process:
+
+```python
+from pm2 import PM2, AioPM2
+import asyncio
+
+pm2 = PM2()
+aiopm2 = AioPM2()
+
+
+# Sync Methods
+def pm2_manager():
+    # List all processes
+    processes = pm2.list()
+    print(processes)
+
+    # Start a process
+    pm2.start(
+        "your_script.py",
+        name="Script-Name",
+        extra_args=["-arg1", "value1"],
+        name="YourProcessName",
+    )
+    # Restart a process
+    pm2.restart(name="Script-Name")  # or pid=12345 or pm_id=1
+
+    # Stop a process
+    pm2.stop(name="Script-Name")  # or pid=12345 or pm_id=1
+
+    # Delete a process
+    pm2.delete(name="Script-Name")  # or pid=12345 or pm_id=1
+
+
+# Async Methods
+async def pm2_manager():
+    # List all processes
+    processes = await aiopm2.list()
+    print(processes)
+
+    # Start a process
+    await aiopm2.start(
+        "your_script.py",
+        name="Script-Name",
+        extra_args=["-arg1", "value1"],
+        name="Script-Name",
+    )
+
+    # Restart a process
+    await aiopm2.restart(name="Script-Name")  # or pid=12345 or pm_id=1
+
+    # Stop a process
+    await aiopm2.stop(name="Script-Name")  # or pid=12345 or pm_id=1
+
+    # Delete a process
+    await aiopm2.delete(name="Script-Name")  # or pid=12345 or pm_id=1
+
+
+# Run the function
+pm2_manager()
+# or
+asyncio.run(pm2_manager())
+```
+
+Replace `'your_script.py'`, `'Script-Name'`, and the args as necessary to fit your needs.
+
+## Contributing
+
+Contributions are welcome! If you would like to contribute, please follow these steps:
+
+1. Fork the repository.
+2. Create a new branch for your feature.
+3. Add your changes and commit them.
+4. Push to your branch.
+5. Create a pull request.
+
+## License
+
+This project is licensed under the MIT License - see the [LICENSE](https://github.com/y4kupkaya/pm2/LICENSE) file for details.
+
+## Acknowledgments
+
+- Thanks to the PM2 team for creating such a powerful process manager.
+- This library was inspired by the need to simplify process management in Python projects.
```

### Comparing `pm2-0.0.3/pm2/__init__.py` & `pm2-0.0.4/pm2/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,308 +1,302 @@
-# !/usr/bin/env python3
-# -*- coding: utf-8 -*-
-r"""PM2 Python Library for Process Management
-
-This exports:
-    - PM2
-    - AioPM2
-    - PM2Process
-    - PathIsFolderError
-    
-Example:
-    ```python
-    from pm2 import PM2, AioPM2, PM2Process, PathIsFolderError
-    import asyncio
-
-    async def main() -> PM2Process:
-        pm2 = AioPM2()
-        try:
-            process = await pm2.start("path/to/your/file.py", name="my-process")
-        except PathIsFolderError as e:
-            print(e)
-        print(process)
-        await pm2.restart(name="my-process")
-        return process
-    ```
-"""
-
-import asyncio
-import os
-import subprocess
-from json import dumps, loads
-from time import time
-from typing import Any, List, Optional
-
-import aiofiles
-from aylak.rich.console import Console
-
-console = Console()
-
-__version__ = "0.0.3"
-
-
-class PathIsFolderError(Exception):
-    pass
-
-
-class PM2Process:
-    pid: int = 0
-    name: str = ""
-    status: str = "online"
-    pm_id: int = 0
-    monit: dict = {}
-    autorestart: bool = False
-    namespace: str = "default"
-    version: str = "N/A"
-    mode: str = "fork"
-    uptime: int = 0
-    created_at: int = 0
-    restart: int = 0
-    user: str = ""
-    cwd: str = ""
-    exec_path: str = ""
-    virtual_env: str = ""
-    out_log: str = ""
-    err_log: str = ""
-    full_json: dict = {}
-
-    def __init__(self, json_data: dict) -> None:
-        self.name = json_data["name"]
-        if json_data["pid"]:
-            self.pid = json_data["pid"]
-        if json_data["pm_id"]:
-            self.pm_id = json_data["pm_id"]
-        self.monit = json_data["monit"]
-        self.autorestart = json_data["pm2_env"]["autorestart"]
-        self.namespace = json_data["pm2_env"]["namespace"]
-        if "versioning" in json_data["pm2_env"]:
-            self.version = json_data["pm2_env"]["versioning"]
-        self.mode = json_data["pm2_env"]["exec_mode"]
-        self.uptime = int(time() - round(json_data["pm2_env"]["pm_uptime"] / 1000))
-        if json_data["pm2_env"]["created_at"]:
-            self.created_at = int(round(json_data["pm2_env"]["created_at"] / 1000))
-        self.restart = json_data["pm2_env"]["restart_time"]
-        self.status = json_data["pm2_env"]["status"]
-        self.user = json_data["pm2_env"]["username"]
-        self.json_data = json_data
-        self.cwd = json_data["pm2_env"].get("pw_cwd")
-        self.exec_path = json_data["pm2_env"].get("pm_exec_path")
-        self.virtual_env = json_data["pm2_env"].get("env", {}).get("VIRTUAL_ENV")
-        self.out_log = json_data["pm2_env"].get("pm_out_log_path")
-        self.err_log = json_data["pm2_env"].get("pm_err_log_path")
-        self.full_json = json_data
-
-    def __str__(self):
-        return f"{self.json()}"
-
-    def __repr__(self):
-        return f"<PM2Process {self.name} ({self.pid}) ({self.status})>"
-
-    def json(self, markup_print: bool = False):
-        if markup_print:
-            console.print_json(data=self.full_json)
-        return dumps(self.full_json, indent=4, ensure_ascii=True)
-
-
-class AioPM2:
-    def __init__(self, command_path: str = "pm2") -> None:
-        self.COMMAND = [command_path]
-        pass
-
-    async def execute_command(self, cmd: List[str]) -> tuple[str, str]:
-        try:
-            process = await asyncio.create_subprocess_exec(
-                *cmd, stdout=asyncio.subprocess.PIPE, stderr=asyncio.subprocess.PIPE
-            )
-            stdout, stderr = await process.communicate()
-            if process.returncode != 0:
-                raise Exception(f"Command failed with error: {stderr.decode()}")
-            return stdout.decode(), stderr.decode()
-        except Exception as e:
-            print(f"An error occurred: {e}")
-            return "", str(e)
-
-    async def list(self) -> List[PM2Process]:
-        stdout, stderr = await self.execute_command(self.COMMAND + ["jlist"])
-        return [PM2Process(process) for process in loads(stdout)]
-
-    async def get(
-        self,
-        pid: int = None,
-        pm_id: int = None,
-        name: str = None,
-    ) -> PM2Process:
-        processes = await self.list()
-        for process in processes:
-            if (
-                (pid and process.pid == pid)
-                or (pm_id and process.pm_id == pm_id)
-                or (name and process.name == name)
-            ):
-                return process
-        return None
-
-    async def start(
-        self, path: str, name: str = None, extra_args: List[str] = None
-    ) -> Optional[PM2Process]:
-        extra_args = extra_args or []
-        if os.path.isdir(path):
-            if "__main__.py" in os.listdir(path):
-                path = os.path.join(path, "__main__.py")
-            else:
-                raise PathIsFolderError("Path is a folder; a file is expected.")
-        cmd = (
-            self.COMMAND
-            + ["start", path]
-            + (["--name", name] if name else [])
-            + extra_args
-        )
-        await self.execute_command(cmd)
-        return await self.get(
-            pm_id=max([process.pm_id for process in await self.list()])
-        )
-
-    async def modify_process(
-        self,
-        action: str,
-        pid: int = None,
-        pm_id: int = None,
-        name: str = None,
-        extra_args: List[str] = None,
-    ) -> bool:
-        extra_args = extra_args or []
-        process = await self.get(pid=pid, pm_id=pm_id, name=name)
-        if process:
-            cmd = self.COMMAND + [action, str(process.pm_id)] + extra_args
-            await self.execute_command(cmd)
-            return await self.get(pid=pid, pm_id=pm_id, name=name)
-        return False
-
-    async def stop(
-        self, pid: int = None, pm_id: int = None, name: str = None
-    ) -> PM2Process:
-        return await self.modify_process("stop", pid, pm_id, name)
-
-    async def restart(
-        self, pid: int = None, pm_id: int = None, name: str = None
-    ) -> PM2Process:
-        return await self.modify_process("restart", pid, pm_id, name)
-
-    async def delete(
-        self, pid: int = None, pm_id: int = None, name: str = None
-    ) -> PM2Process:
-        return await self.modify_process("delete", pid, pm_id, name)
-
-    async def logs(
-        self,
-        lines: int = 500,
-        pid: int = None,
-        pm_id: int = None,
-        name: str = None,
-        errors: bool = False,
-    ) -> str:
-        process = await self.get(pid=pid, pm_id=pm_id, name=name)
-        async with aiofiles.open(process.out_log, "r", encoding="utf-8") as f:
-            out_log = "\n".join(await f.readlines()[-lines:])
-        async with aiofiles.open(process.err_log, "r", encoding="utf-8") as f:
-            err_log = "\n".join(await f.readlines()[-lines:])
-        return (out_log, err_log) if errors else out_log
-
-
-# sync PM2
-class PM2:
-    def __init__(self, command_path: str = "pm2") -> None:
-        self.COMMAND = [command_path]
-        pass
-
-    def execute_command(self, cmd: List[str]) -> tuple[str, str]:
-        try:
-            process = subprocess.Popen(
-                cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE
-            )
-            stdout, stderr = process.communicate()
-            if process.returncode != 0:
-                raise Exception(f"Command failed with error: {stderr.decode()}")
-            return stdout.decode(), stderr.decode()
-        except Exception as e:
-            print(f"An error occurred: {e}")
-            return "", str(e)
-
-    def list(self) -> List[PM2Process]:
-        stdout, stderr = self.execute_command(self.COMMAND + ["jlist"])
-        return [PM2Process(process) for process in loads(stdout)]
-
-    def get(
-        self,
-        pid: int = None,
-        pm_id: int = None,
-        name: str = None,
-    ) -> PM2Process:
-        processes = self.list()
-        for process in processes:
-            if (
-                (pid and process.pid == pid)
-                or (pm_id and process.pm_id == pm_id)
-                or (name and process.name == name)
-            ):
-                return process
-        return None
-
-    def start(
-        self, path: str, name: str = None, extra_args: List[str] = None
-    ) -> Optional[PM2Process]:
-        extra_args = extra_args or []
-        if os.path.isdir(path):
-            if "__main__.py" in os.listdir(
-                path
-            ):  # TODO: Folder initialization for languages ​​other than Python will be added
-                path = os.path.join(path, "__main__.py")
-            else:
-                raise PathIsFolderError("Path is a folder; a file is expected.")
-        cmd = (
-            self.COMMAND
-            + ["start", path]
-            + (["--name", name] if name else [])
-            + extra_args
-        )
-        self.execute_command(cmd)
-        return self.get(pm_id=max([process.pm_id for process in self.list()]))
-
-    def modify_process(
-        self,
-        action: str,
-        pid: int = None,
-        pm_id: int = None,
-        name: str = None,
-        extra_args: List[str] = None,
-    ) -> bool:
-        extra_args = extra_args or []
-        process = self.get(pid=pid, pm_id=pm_id, name=name)
-        if process:
-            cmd = self.COMMAND + [action, str(process.pm_id)] + extra_args
-            self.execute_command(cmd)
-            return self.get(pid=pid, pm_id=pm_id, name=name)
-        return False
-
-    def stop(self, pid: int = None, pm_id: int = None, name: str = None) -> bool:
-        return self.modify_process("stop", pid, pm_id, name)
-
-    def restart(self, pid: int = None, pm_id: int = None, name: str = None) -> bool:
-        return self.modify_process("restart", pid, pm_id, name)
-
-    def delete(self, pid: int = None, pm_id: int = None, name: str = None) -> bool:
-        return self.modify_process("delete", pid, pm_id, name)
-
-    def logs(
-        self,
-        lines: int = 500,
-        pid: int = None,
-        pm_id: int = None,
-        name: str = None,
-        errors: bool = False,
-    ) -> str:
-        process = self.get(pid=pid, pm_id=pm_id, name=name)
-        with open(process.out_log, "r", encoding="utf-8") as f:
-            out_log = "\n".join(f.readlines()[-lines:])
-        with open(process.err_log, "r", encoding="utf-8") as f:
-            err_log = "\n".join(f.readlines()[-lines:])
-        return (out_log, err_log) if errors else out_log
+# !/usr/bin/env python3
+# -*- coding: utf-8 -*-
+r"""PM2 Python Library for Process Management
+
+This exports:
+    - PM2
+    - AioPM2
+    - PM2Process
+    - PathIsFolderError
+    
+Example:
+    ```python
+    from pm2 import PM2, AioPM2, PM2Process, PathIsFolderError
+    import asyncio
+
+    async def main() -> PM2Process:
+        pm2 = AioPM2()
+        try:
+            process = await pm2.start("path/to/your/file.py", name="my-process")
+        except PathIsFolderError as e:
+            print(e)
+        print(process)
+        await pm2.restart(name="my-process")
+        return process
+    ```
+"""
+
+import asyncio
+import os
+import subprocess
+from json import dumps, loads
+from time import time
+from typing import Any, List, Optional
+
+import aiofiles
+from aylak.rich.console import Console
+
+console = Console()
+
+__version__ = "0.0.4"
+
+
+class PathIsFolderError(Exception):
+    pass
+
+
+class PM2Process:
+    pid: int = 0
+    name: str = ""
+    status: str = "online"
+    pm_id: int = 0
+    monit: dict = {}
+    autorestart: bool = False
+    namespace: str = "default"
+    version: str = "N/A"
+    mode: str = "fork"
+    uptime: int = 0
+    created_at: int = 0
+    restart: int = 0
+    user: str = ""
+    cwd: str = ""
+    exec_path: str = ""
+    virtual_env: str = ""
+    out_log: str = ""
+    err_log: str = ""
+    full_json: dict = {}
+
+    def __init__(self, json_data: dict) -> None:
+        self.name = json_data["name"]
+        if json_data["pid"]:
+            self.pid = json_data["pid"]
+        if json_data["pm_id"]:
+            self.pm_id = json_data["pm_id"]
+        self.monit = json_data["monit"]
+        self.autorestart = json_data["pm2_env"]["autorestart"]
+        self.namespace = json_data["pm2_env"]["namespace"]
+        if "versioning" in json_data["pm2_env"]:
+            self.version = json_data["pm2_env"]["versioning"]
+        self.mode = json_data["pm2_env"]["exec_mode"]
+        self.uptime = int(time() - round(json_data["pm2_env"]["pm_uptime"] / 1000))
+        if json_data["pm2_env"]["created_at"]:
+            self.created_at = int(round(json_data["pm2_env"]["created_at"] / 1000))
+        self.restart = json_data["pm2_env"]["restart_time"]
+        self.status = json_data["pm2_env"]["status"]
+        self.user = json_data["pm2_env"]["username"]
+        self.json_data = json_data
+        self.cwd = json_data["pm2_env"].get("pw_cwd")
+        self.exec_path = json_data["pm2_env"].get("pm_exec_path")
+        self.virtual_env = json_data["pm2_env"].get("env", {}).get("VIRTUAL_ENV")
+        self.out_log = json_data["pm2_env"].get("pm_out_log_path")
+        self.err_log = json_data["pm2_env"].get("pm_err_log_path")
+        self.full_json = json_data
+
+    def __str__(self):
+        return f"{self.json()}"
+
+    def __repr__(self):
+        return f"<PM2Process {self.name} ({self.pid}) ({self.status})>"
+
+    def json(self, markup_print: bool = False):
+        if markup_print:
+            console.print_json(data=self.full_json)
+        return dumps(self.full_json, indent=4, ensure_ascii=True)
+
+
+class AioPM2:
+    def __init__(self, command_path: str = "pm2") -> None:
+        self.COMMAND = [command_path]
+        pass
+
+    async def execute_command(self, cmd: List[str]) -> tuple[str, str]:
+        process = await asyncio.create_subprocess_shell(
+            " ".join(cmd),
+            stdout=asyncio.subprocess.PIPE,
+            stderr=asyncio.subprocess.PIPE,
+        )
+        stdout, stderr = await process.communicate()
+        if process.returncode != 0:
+            raise Exception(f"Command failed with error: {stderr.decode()}")
+        return stdout.decode(), stderr.decode()
+
+    async def list(self) -> List[PM2Process]:
+        stdout, stderr = await self.execute_command(self.COMMAND + ["jlist"])
+        return [PM2Process(process) for process in loads(stdout)]
+
+    async def get(
+        self,
+        pid: int = None,
+        pm_id: int = None,
+        name: str = None,
+    ) -> PM2Process:
+        processes = await self.list()
+        for process in processes:
+            if (
+                (pid and process.pid == pid)
+                or (pm_id and process.pm_id == pm_id)
+                or (name and process.name == name)
+            ):
+                return process
+        return None
+
+    async def start(
+        self, path: str, name: str = None, extra_args: List[str] = None
+    ) -> Optional[PM2Process]:
+        extra_args = extra_args or []
+        if os.path.isdir(path):
+            if "__main__.py" in os.listdir(path):
+                path = os.path.join(path, "__main__.py")
+            else:
+                raise PathIsFolderError("Path is a folder; a file is expected.")
+        cmd = (
+            self.COMMAND
+            + ["start", path]
+            + (["--name", name] if name else [])
+            + extra_args
+        )
+        await self.execute_command(cmd)
+        return await self.get(
+            pm_id=max([process.pm_id for process in await self.list()])
+        )
+
+    async def modify_process(
+        self,
+        action: str,
+        pid: int = None,
+        pm_id: int = None,
+        name: str = None,
+        extra_args: List[str] = None,
+    ) -> bool:
+        extra_args = extra_args or []
+        process = await self.get(pid=pid, pm_id=pm_id, name=name)
+        if process:
+            cmd = self.COMMAND + [action, str(process.pm_id)] + extra_args
+            await self.execute_command(cmd)
+            return await self.get(pid=pid, pm_id=pm_id, name=name)
+        return False
+
+    async def stop(
+        self, pid: int = None, pm_id: int = None, name: str = None
+    ) -> PM2Process:
+        return await self.modify_process("stop", pid, pm_id, name)
+
+    async def restart(
+        self, pid: int = None, pm_id: int = None, name: str = None
+    ) -> PM2Process:
+        return await self.modify_process("restart", pid, pm_id, name)
+
+    async def delete(
+        self, pid: int = None, pm_id: int = None, name: str = None
+    ) -> PM2Process:
+        return await self.modify_process("delete", pid, pm_id, name)
+
+    async def logs(
+        self,
+        lines: int = 500,
+        pid: int = None,
+        pm_id: int = None,
+        name: str = None,
+        errors: bool = False,
+    ) -> str:
+        process = await self.get(pid=pid, pm_id=pm_id, name=name)
+        async with aiofiles.open(process.out_log, "r", encoding="utf-8") as f:
+            out_log = "\n".join(await f.readlines()[-lines:])
+        async with aiofiles.open(process.err_log, "r", encoding="utf-8") as f:
+            err_log = "\n".join(await f.readlines()[-lines:])
+        return (out_log, err_log) if errors else out_log
+
+
+# sync PM2
+class PM2:
+    def __init__(self, command_path: str = "pm2") -> None:
+        self.COMMAND = [command_path]
+        pass
+
+    def execute_command(self, cmd: List[str]) -> tuple[str, str]:
+        process = subprocess.Popen(
+            cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True
+        )
+        stdout, stderr = process.communicate()
+        if process.returncode != 0:
+            raise Exception(f"Command failed with error: {stderr.decode()}")
+        return stdout.decode(), stderr.decode()
+
+    def list(self) -> List[PM2Process]:
+        stdout, stderr = self.execute_command(self.COMMAND + ["jlist"])
+        return [PM2Process(process) for process in loads(stdout)]
+
+    def get(
+        self,
+        pid: int = None,
+        pm_id: int = None,
+        name: str = None,
+    ) -> PM2Process:
+        processes = self.list()
+        for process in processes:
+            if (
+                (pid and process.pid == pid)
+                or (pm_id and process.pm_id == pm_id)
+                or (name and process.name == name)
+            ):
+                return process
+        return None
+
+    def start(
+        self, path: str, name: str = None, extra_args: List[str] = None
+    ) -> Optional[PM2Process]:
+        extra_args = extra_args or []
+        if os.path.isdir(path):
+            if "__main__.py" in os.listdir(
+                path
+            ):  # TODO: Folder initialization for languages ​​other than Python will be added
+                path = os.path.join(path, "__main__.py")
+            else:
+                raise PathIsFolderError("Path is a folder; a file is expected.")
+        cmd = (
+            self.COMMAND
+            + ["start", path]
+            + (["--name", name] if name else [])
+            + extra_args
+        )
+        self.execute_command(cmd)
+        return self.get(pm_id=max([process.pm_id for process in self.list()]))
+
+    def modify_process(
+        self,
+        action: str,
+        pid: int = None,
+        pm_id: int = None,
+        name: str = None,
+        extra_args: List[str] = None,
+    ) -> bool:
+        extra_args = extra_args or []
+        process = self.get(pid=pid, pm_id=pm_id, name=name)
+        if process:
+            cmd = self.COMMAND + [action, str(process.pm_id)] + extra_args
+            self.execute_command(cmd)
+            return self.get(pid=pid, pm_id=pm_id, name=name)
+        return False
+
+    def stop(self, pid: int = None, pm_id: int = None, name: str = None) -> bool:
+        return self.modify_process("stop", pid, pm_id, name)
+
+    def restart(self, pid: int = None, pm_id: int = None, name: str = None) -> bool:
+        return self.modify_process("restart", pid, pm_id, name)
+
+    def delete(self, pid: int = None, pm_id: int = None, name: str = None) -> bool:
+        return self.modify_process("delete", pid, pm_id, name)
+
+    def logs(
+        self,
+        lines: int = 500,
+        pid: int = None,
+        pm_id: int = None,
+        name: str = None,
+        errors: bool = False,
+    ) -> str:
+        process = self.get(pid=pid, pm_id=pm_id, name=name)
+        with open(process.out_log, "r", encoding="utf-8") as f:
+            out_log = "\n".join(f.readlines()[-lines:])
+        with open(process.err_log, "r", encoding="utf-8") as f:
+            err_log = "\n".join(f.readlines()[-lines:])
+        return (out_log, err_log) if errors else out_log
```

### Comparing `pm2-0.0.3/pm2.egg-info/PKG-INFO` & `pm2-0.0.4/pm2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pm2
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python wrapper for PM2
 Home-page: https://github.com/y4kupkaya/pm2
 Author: y4kupkaya
 Author-email: contact@yakupkaya.net.tr
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Keywords: process-manager,pm2,pm2-py
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,16 +27,14 @@
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aylak==0.0.6
-Requires-Dist: aiofiles
 
 
 # PM2 Python Library for Process Management
 
 ## Introduction
 
 This Python library provides a seamless integration with PM2, enabling users to automate the launching and management of processes using PM2 through Python. Designed to cater to developers and system administrators who require a programmable interface to control their processes with the power and flexibility of Python, this library simplifies interactions with PM2, making it more accessible and versatile.
@@ -128,17 +126,17 @@
 
 Contributions are welcome! If you would like to contribute, please follow these steps:
 
 1. Fork the repository.
 2. Create a new branch for your feature.
 3. Add your changes and commit them.
 4. Push to your branch.
-5. Create a pull request. 
+5. Create a pull request.
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](https://github.com/y4kupkaya/pm2-python-lib/LICENSE) file for details.
+This project is licensed under the MIT License - see the [LICENSE](https://github.com/y4kupkaya/pm2/LICENSE) file for details.
 
 ## Acknowledgments
 
 - Thanks to the PM2 team for creating such a powerful process manager.
-- This library was inspired by the need to simplify process management in Python projects. 
+- This library was inspired by the need to simplify process management in Python projects.
```

### Comparing `pm2-0.0.3/setup.py` & `pm2-0.0.4/setup.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-# !/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from setuptools import find_packages, setup
-import re
-
-
-requirements = ["aylak==0.0.6", "aiofiles"]
-
-with open("pm2/__init__.py", encoding="utf-8") as f:
-    version = re.findall(r"__version__ = \"(.+)\"", f.read())[0]
-
-with open("README.md", encoding="utf-8") as f:
-    long_description = f.read()
-
-setup(
-    name="pm2",
-    version=version,
-    url="https://github.com/y4kupkaya/pm2",
-    description="Python wrapper for PM2",
-    keywords=["process-manager", "pm2", "pm2-py"],
-    author="y4kupkaya",
-    author_email="contact@yakupkaya.net.tr",
-    license="GNU AFFERO GENERAL PUBLIC LICENSE (v3)",
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "Natural Language :: English",
-        "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: Implementation",
-        "Programming Language :: Python :: Implementation :: CPython",
-        "Programming Language :: Python :: Implementation :: PyPy",
-        "Topic :: Internet",
-        "Topic :: Communications",
-        "Topic :: Communications :: Chat",
-        "Topic :: Software Development :: Libraries",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-        "Topic :: Software Development :: Libraries :: Application Frameworks",
-    ],
-    packages=find_packages(),
-    python_requires=">=3.10",
-    install_requires=requirements,
-    zip_safe=False,
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-)
+# !/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from setuptools import find_packages, setup
+import re
+
+
+requirements = ["aylak==0.0.6", "aiofiles"]
+
+with open("pm2/__init__.py", encoding="utf-8") as f:
+    version = re.findall(r"__version__ = \"(.+)\"", f.read())[0]
+
+with open("README.md", encoding="utf-8") as f:
+    long_description = f.read()
+
+setup(
+    name="pm2",
+    version=version,
+    url="https://github.com/y4kupkaya/pm2",
+    description="Python wrapper for PM2",
+    keywords=["process-manager", "pm2", "pm2-py"],
+    author="y4kupkaya",
+    author_email="contact@yakupkaya.net.tr",
+    license="GNU AFFERO GENERAL PUBLIC LICENSE (v3)",
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Natural Language :: English",
+        "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: Implementation",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
+        "Topic :: Internet",
+        "Topic :: Communications",
+        "Topic :: Communications :: Chat",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Topic :: Software Development :: Libraries :: Application Frameworks",
+    ],
+    packages=find_packages(),
+    python_requires=">=3.10",
+    install_requires=requirements,
+    zip_safe=False,
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+)
```

