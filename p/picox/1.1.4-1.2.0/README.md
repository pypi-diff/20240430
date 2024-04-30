# Comparing `tmp/picox-1.1.4.tar.gz` & `tmp/picox-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picox-1.1.4.tar", last modified: Sat Apr 20 21:36:50 2024, max compression
+gzip compressed data, was "picox-1.2.0.tar", last modified: Tue Apr 30 20:47:52 2024, max compression
```

## Comparing `picox-1.1.4.tar` & `picox-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 21:36:50.927449 picox-1.1.4/
--rw-rw-rw-   0        0        0     1075 2024-04-14 14:56:21.000000 picox-1.1.4/LICENCE
--rw-rw-rw-   0        0        0     4990 2024-04-20 21:36:50.927449 picox-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2740 2024-04-20 21:18:31.000000 picox-1.1.4/README.md
--rw-rw-rw-   0        0        0     1099 2024-04-20 21:29:44.000000 picox-1.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-20 21:36:50.927449 picox-1.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-20 21:36:50.877426 picox-1.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-20 21:36:50.894109 picox-1.1.4/src/picox/
--rw-rw-rw-   0        0        0       21 2024-04-20 20:04:02.000000 picox-1.1.4/src/picox/__init__.py
--rw-rw-rw-   0        0        0     3055 2024-04-20 20:04:02.000000 picox-1.1.4/src/picox/cli.py
--rw-rw-rw-   0        0        0     2083 2024-04-20 20:04:02.000000 picox-1.1.4/src/picox/detect.py
--rw-rw-rw-   0        0        0       54 2024-04-19 19:58:56.000000 picox-1.1.4/src/picox/logconfig.py
--rw-rw-rw-   0        0        0    11198 2024-04-20 20:47:32.000000 picox-1.1.4/src/picox/upy.py
-drwxrwxrwx   0        0        0        0 2024-04-20 21:36:50.925769 picox-1.1.4/src/picox.egg-info/
--rw-rw-rw-   0        0        0     4990 2024-04-20 21:36:50.000000 picox-1.1.4/src/picox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2024-04-20 21:36:50.000000 picox-1.1.4/src/picox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 21:36:50.000000 picox-1.1.4/src/picox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-04-20 21:36:50.000000 picox-1.1.4/src/picox.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       85 2024-04-20 21:36:50.000000 picox-1.1.4/src/picox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-20 21:36:50.000000 picox-1.1.4/src/picox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:47:52.410638 picox-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-30 20:47:48.000000 picox-1.2.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-30 20:47:52.410638 picox-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-30 20:47:48.000000 picox-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-30 20:47:48.000000 picox-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 20:47:52.410638 picox-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:47:52.406638 picox-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:47:52.410638 picox-1.2.0/src/picox/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 20:47:48.000000 picox-1.2.0/src/picox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-30 20:47:48.000000 picox-1.2.0/src/picox/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-30 20:47:48.000000 picox-1.2.0/src/picox/detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-30 20:47:48.000000 picox-1.2.0/src/picox/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12425 2024-04-30 20:47:48.000000 picox-1.2.0/src/picox/upy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:47:52.410638 picox-1.2.0/src/picox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-30 20:47:52.000000 picox-1.2.0/src/picox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-30 20:47:52.000000 picox-1.2.0/src/picox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:47:52.000000 picox-1.2.0/src/picox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 20:47:52.000000 picox-1.2.0/src/picox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 20:47:52.000000 picox-1.2.0/src/picox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 20:47:52.000000 picox-1.2.0/src/picox.egg-info/top_level.txt
```

### Comparing `picox-1.1.4/LICENCE` & `picox-1.2.0/LICENCE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2024
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `picox-1.1.4/PKG-INFO` & `picox-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,174 +1,180 @@
-Metadata-Version: 2.1
-Name: picox
-Version: 1.1.4
-Summary: Tools for working with a Rasbperry Pi Pico running MicroPython
-Author: Harvey
-License: MIT License
-        
-        Copyright (c) 2024
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/SparkyTheAlbino/picox
-Project-URL: Documentation, https://github.com/SparkyTheAlbino/picox
-Project-URL: Repository, https://github.com/SparkyTheAlbino/picox.git
-Project-URL: Issues, https://github.com/SparkyTheAlbino/picox/issues
-Keywords: pico,serial,RaspberryPi
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Environment :: Console
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Embedded Systems
-Description-Content-Type: text/markdown
-License-File: LICENCE
-Requires-Dist: pyserial==3.5
-Requires-Dist: pyreadline3==3.4.1; platform_system == "Windows"
-Provides-Extra: dev
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-
-# picox
-`picox` is a tool that facilitates the interaction with Raspberry Pi Pico running MicroPython boards through the terminal or within a Python script. This uses the USB serial port for communication.
-
-Windows, Linux and macOS are supported.
-
-## Features
-- Detect a connected Raspberry Pi Pico device running MicroPython
-- REPL session
-- File operations: Upload, download, execute, and list files on Pi Pico
-- Stop current execution on device
-
-## Known issues
-- REPL can timeout on long operations such as sleep. Its in the nature of how it scans for the end
-- Line endings of files coming out can get a little strange. watch out if there are som extra spaces etc. Best bet is to ensure you always work in the same line endings
-- File operations do not include folder operations __yet__
-
-## Installation
-Install via `pip`:
-
-``` bash 
-pip install picox
-```
-
-
-## CLI Usage
-
-
-### Detecting Pi Pico:
-``` bash
-# get first found device
-picox detect
-
-# get a list of all connected pico devices
-pico detect --all
-
-# Output: COM7 or /dev/ttyUSB0
-```
-
-### REPL session on Pi Pico
-``` bash
-picox repl /dev/ttyUSB0
-```
-
-### Listing files on Pi Pico:
-``` bash
-picox ls /dev/ttyUSB0
-
-# exmaple output:
-# demo.py
-# home.py
-```
-
-### Uploading a file:
-``` bash
-picox upload /dev/ttyUSB0 local.py remote.py --overwrite
-
-# --overrite to force update the file on the Pi Pico
-```
-
-### Downloading a file:
-``` bash
-picox download /dev/ttyUSB0 remote.py local.py
-```
-
-### Executing a file on Pi Pico:
-``` bash
-picox exec /dev/ttyUSB0 remote.py
-```
-
-### Stopping any ongoing operation on Pi Pico:
-``` bash
-picox stop /dev/ttyUSB0
-```
-
-
-## Python Script Usage
-You can also use picox within your Python scripts as follows:
-
-``` python
-from picox import Pico
-from picox.detect import get_first_pico_serial
-
-
-# Init device
-serial_device = get_first_pico_serial()
-pico = Pico(serial_device)
-
-# File listing
-for file in pico.get_file_list():
-    print(file)
-
-# Download
-with open("./local/demo.py", "w") as download_file:
-    pico.download_file("remote_demo.py", download_file)
-
-# Upload
-with open("./local/demo.py", "rb") as upload_file:
-    pico.upload_file(upload_file, "remote_demo.py", overwrite=True)
-
-# Execute
-pico.execute_file("remote_demo.py")
-
-# Halt execution on device
-pico.stop_exec()
-
-# Soft reboot device
-pico.send_soft_reboot()
-```
-
-## Local development
-1. Create virtual env
-``` bash
-python -m venv _env
-```
-2. Activate env
-``` bash
-# Win
-_env/Scripts/activate.ps1
-# nix
-source _env/bin/activate
-```
-3. Install requirements
-``` bash
-pip install -r requirement.txt
-```
-4. Install module editable
-```
-pip install -e .
-```
+Metadata-Version: 2.1
+Name: picox
+Version: 1.2.0
+Summary: Tools for working with a Rasbperry Pi Pico running MicroPython
+Author: Harvey
+License: MIT License
+        
+        Copyright (c) 2024
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: Homepage, https://github.com/SparkyTheAlbino/picox
+Project-URL: Documentation, https://github.com/SparkyTheAlbino/picox
+Project-URL: Repository, https://github.com/SparkyTheAlbino/picox.git
+Project-URL: Issues, https://github.com/SparkyTheAlbino/picox/issues
+Keywords: pico,serial,RaspberryPi
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Environment :: Console
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Embedded Systems
+Description-Content-Type: text/markdown
+License-File: LICENCE
+Requires-Dist: pyserial==3.5
+Requires-Dist: pyreadline3==3.4.1; platform_system == "Windows"
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+
+# picox
+`picox` is a tool that facilitates the interaction with Raspberry Pi Pico running MicroPython boards through the terminal or within a Python script. This uses the USB serial port for communication.
+
+Windows, Linux and macOS are supported.
+
+## Features
+- Detect a connected Raspberry Pi Pico device running MicroPython
+- REPL session
+- File operations: Upload, download, execute, and list files on Pi Pico
+- Stop current execution on device
+
+## Known issues
+- REPL can timeout on long operations such as sleep. Its in the nature of how it scans for the end
+- Line endings of files coming out can get a little strange. watch out if there are som extra spaces etc. Best bet is to ensure you always work in the same line endings
+- File operations do not include folder operations __yet__
+- Most commands will halt what is running on the pico. Such as a detect will stop execution in order to get a good communication test. For a more manual detection, you can use `picox attach <device>` to try and stream stdout from the pico
+
+## Installation
+Install via `pip`:
+
+``` bash 
+pip install picox
+```
+
+
+## CLI Usage
+
+
+### Detecting Pi Pico:
+``` bash
+# get first found device
+picox detect
+
+# get a list of all connected pico devices
+pico detect --all
+
+# Output: COM7 or /dev/ttyUSB0
+```
+
+### REPL session on Pi Pico
+``` bash
+picox repl /dev/ttyUSB0
+```
+
+### View console output from already running pico
+``` bash
+picox attach /dev/ttyUSB0
+```
+
+### Listing files on Pi Pico:
+``` bash
+picox ls /dev/ttyUSB0
+
+# exmaple output:
+# demo.py
+# home.py
+```
+
+### Uploading a file:
+``` bash
+picox upload /dev/ttyUSB0 local.py remote.py --overwrite
+
+# --overrite to force update the file on the Pi Pico
+```
+
+### Downloading a file:
+``` bash
+picox download /dev/ttyUSB0 remote.py local.py
+```
+
+### Executing a file on Pi Pico:
+``` bash
+picox exec /dev/ttyUSB0 remote.py
+```
+
+### Stopping any ongoing operation on Pi Pico:
+``` bash
+picox stop /dev/ttyUSB0
+```
+
+
+## Python Script Usage
+You can also use picox within your Python scripts as follows:
+
+``` python
+from picox import Pico
+from picox.detect import get_first_pico_serial
+
+
+# Init device
+serial_device = get_first_pico_serial()
+pico = Pico(serial_device)
+
+# File listing
+for file in pico.get_file_list():
+    print(file)
+
+# Download
+with open("./local/demo.py", "w") as download_file:
+    pico.download_file("remote_demo.py", download_file)
+
+# Upload
+with open("./local/demo.py", "rb") as upload_file:
+    pico.upload_file(upload_file, "remote_demo.py", overwrite=True)
+
+# Execute
+pico.execute_file("remote_demo.py")
+
+# Halt execution on device
+pico.stop_exec()
+
+# Soft reboot device
+pico.send_soft_reboot()
+```
+
+## Local development
+1. Create virtual env
+``` bash
+python -m venv _env
+```
+2. Activate env
+``` bash
+# Win
+_env/Scripts/activate.ps1
+# nix
+source _env/bin/activate
+```
+3. Install requirements
+``` bash
+pip install -r requirement.txt
+```
+4. Install module editable
+```
+pip install -e .
+```
```

### Comparing `picox-1.1.4/pyproject.toml` & `picox-1.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-[build-system]
-requires = ["setuptools", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "picox"
-version = "1.1.4"
-authors = [{name = "Harvey"}]
-description = "Tools for working with a Rasbperry Pi Pico running MicroPython"
-readme = "README.md"
-license = {file = "LICENCE"}
-dependencies = [
-    "pyserial == 3.5",
-    'pyreadline3 == 3.4.1 ; platform_system == "Windows"',
-]
-classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Environment :: Console",
-    "Operating System :: OS Independent",
-    "Topic :: Software Development :: Embedded Systems",
-]
-keywords = ["pico", "serial", "RaspberryPi"]
-
-[project.optional-dependencies]
-dev = ['build', 'twine']
-
-[project.scripts]
-picox = "picox.cli:main"
-
-[project.urls]
-Homepage = "https://github.com/SparkyTheAlbino/picox"
-Documentation = "https://github.com/SparkyTheAlbino/picox"
-Repository = "https://github.com/SparkyTheAlbino/picox.git"
-Issues = "https://github.com/SparkyTheAlbino/picox/issues"
+[build-system]
+requires = ["setuptools", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "picox"
+version = "1.2.0"
+authors = [{name = "Harvey"}]
+description = "Tools for working with a Rasbperry Pi Pico running MicroPython"
+readme = "README.md"
+license = {file = "LICENCE"}
+dependencies = [
+    "pyserial == 3.5",
+    'pyreadline3 == 3.4.1 ; platform_system == "Windows"',
+]
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Environment :: Console",
+    "Operating System :: OS Independent",
+    "Topic :: Software Development :: Embedded Systems",
+]
+keywords = ["pico", "serial", "RaspberryPi"]
+
+[project.optional-dependencies]
+dev = ['build', 'twine']
+
+[project.scripts]
+picox = "picox.cli:main"
+
+[project.urls]
+Homepage = "https://github.com/SparkyTheAlbino/picox"
+Documentation = "https://github.com/SparkyTheAlbino/picox"
+Repository = "https://github.com/SparkyTheAlbino/picox.git"
+Issues = "https://github.com/SparkyTheAlbino/picox/issues"
```

### Comparing `picox-1.1.4/src/picox/detect.py` & `picox-1.2.0/src/picox/detect.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,80 @@
-import glob
-import platform
-from typing import List, Optional
-
-import serial
-import serial.tools.list_ports
-
-from .upy import Pico
-
-
-def get_serial_ports() -> List[str]:
-    """
-    Get USB serial devices for your OS
-    raises:
-        NotImplimentedError - If not Windows, Linux or macOS
-    """
-    match platform.system():
-        case "Windows":
-            ports = serial.tools.list_ports.comports()
-            return [port.device for port in ports if "USB Serial Device" in port.description]
-        case "Linux":
-            return glob.glob('/dev/ttyACM*')
-        case "Darwin":
-            return glob.glob('/dev/tty.usb*')
-        case _:
-            raise NotImplementedError("Unsupported OS")
-
-def is_pico(device: str):
-    """
-    Try to determine if USB serial device is a Pi Pico device
-    args:
-        device (str): USB serial device to test
-    """
-    try:
-        pico = Pico(device, serial_read_timeout=1, serial_write_timeout=1)
-        pico.send_stop_exec()
-        pico.send_enter()
-        return pico.coms_test()
-    except Exception as err:
-        return False
-
-def search_ports_for_pico(serial_devices: List[str]) -> List[str]:
-    """
-    Iterate over list of strings and try to communicate on those USB serial ports with a Pi Pico
-    """
-    for device in serial_devices:
-        if is_pico(device):
-            return device
-    else:
-        return None
-    
-def get_first_pico_serial() -> Optional[str]:
-    """
-    Get ports + detect pico
-    returns:
-        str: serial device name or None
-    """
-    serial_devices = get_serial_ports()
-    for device in serial_devices:
-        if is_pico(device):
-            return device
-    else:
-        return None
-
-def get_all_pico_serial() -> List:
-    """
-    Get ports then return all detected pico devices
-    """
-    serial_devices = get_serial_ports()
-    pico_devices = []
-    for serial_device in serial_devices:
-        if is_pico(serial_device):
-            pico_devices.append(serial_device)
+import glob
+import platform
+from typing import List, Optional
+
+import serial
+import serial.tools.list_ports
+
+from .upy import Pico
+from .logconfig import LOGGER
+
+
+def get_serial_ports() -> List[str]:
+    """
+    Get USB serial devices for your OS
+    raises:
+        NotImplementedError - If not Windows, Linux or macOS
+    """
+    match platform.system():
+        case "Windows":
+            ports = serial.tools.list_ports.comports()
+            return [port.device for port in ports if "USB Serial Device" in port.description]
+        case "Linux":
+            return glob.glob('/dev/ttyACM*')
+        case "Darwin":
+            return glob.glob('/dev/tty.usb*')
+        case _:
+            raise NotImplementedError("Unsupported OS")
+
+def is_pico(device: str):
+    """
+    Try to determine if USB serial device is a Pi Pico device
+    args:
+        device (str): USB serial device to test
+    """
+    try:
+        Pico(
+            device,
+            serial_read_timeout=1,
+            serial_write_timeout=1,
+        )
+    except Exception as err:
+        if "[Errno 13]" in str(err):
+            LOGGER.warning(f"[{device}] :: Permission denied!")
+        return False
+    else:
+        return True
+
+def search_ports_for_pico(serial_devices: List[str]) -> List[str]:
+    """
+    Iterate over list of strings and try to communicate on those USB serial ports with a Pi Pico
+    """
+    for device in serial_devices:
+        if is_pico(device):
+            return device
+    else:
+        return None
+    
+def get_first_pico_serial() -> Optional[str]:
+    """
+    Get ports + detect pico
+    returns:
+        str: serial device name or None
+    """
+    serial_devices = get_serial_ports()
+    for device in serial_devices:
+        if is_pico(device):
+            return device
+    else:
+        return None
+
+def get_all_pico_serial() -> List:
+    """
+    Get ports then return all detected pico devices
+    """
+    serial_devices = get_serial_ports()
+    pico_devices = []
+    for serial_device in serial_devices:
+        if is_pico(serial_device):
+            pico_devices.append(serial_device)
     return pico_devices
```

### Comparing `picox-1.1.4/src/picox/upy.py` & `picox-1.2.0/src/picox/upy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,270 +1,299 @@
-import ast
-import time
-import re
-import platform
-from enum import Enum
-from typing import IO, Optional
-from itertools import cycle
-
-import serial
-
-from .logconfig import LOGGER
-
-
-# Constants for communication patterns
-TERMINATOR = '\r\n'  
-UPY_PROMPT = "\r\n>>>"  
-BLOCK_PROMPT = "..."  
-EOR_MARKER = "---f81b734f-7be3-4747-ae0b-c449006b33dd---"
-EOR_TOKEN  = f"{EOR_MARKER}{UPY_PROMPT}"
-EOR_MARKER_COMMAND = f";print('{EOR_MARKER}')"
-EOM_MARKER = f';pass;pass;pass;pass{EOR_MARKER_COMMAND}'
-RE_MATCH_BACKSPACE_BEGINNING = re.compile('^' + re.escape("\x08") + '+')
-
-class MicroPython_Version(Enum):
-    """Enumeration of supported MicroPython versions."""
-    v1_21_0 = "1.21.0"
-
-
-class Pico:
-    """Manage communications with a MicroPython RP2040 device via serial."""
-    def __init__(self, 
-                 serial_port: str, 
-                 micropython_version: MicroPython_Version = MicroPython_Version.v1_21_0, 
-                 start_closed: bool=False,
-                 auto_halt: bool=True,
-                 skip_coms_test: bool=False,
-                 serial_read_timeout: int=15, 
-                 serial_write_timeout: Optional[int]=None
-                 ):
-        """
-        New RP2040 device running MicroPython.
-        args:
-            serial_port (str): serial device of Pico
-            micropython_version (str): Version of MicroPython on device. Does not currently matter
-            start_closed (bool): Creates object without opening the serial port
-            auto_halt (bool): Automatically stop exec and soft reboot the device when creating object
-            skip_coms_test (bool) : Skip a coms test that verifies the coms is good between the computer and Pico
-            serial_read_timeout (int): Read timeout supplied to serial.Serial
-            serial_write_timeout (int): Write timeout supplied to serial.Serial
-        """
-        self._serial_read_timeout = serial_read_timeout
-        self._serial_write_timeout = serial_write_timeout
-        self._upy_version = micropython_version
-        self._serial_port = serial_port
-        self._serial = None
-        if not start_closed:
-            # Open the serial device here
-            self._open_serial()
-
-            # Send stop and reboot to reset Pico state
-            if auto_halt:
-                self.send_stop_exec()
-                self.send_soft_reboot()
-
-            # Run a sanity test to ensure the serial device responds as expected (e.g. does it run micropython)
-            if not skip_coms_test:
-                if not self.coms_test():
-                    raise IOError("Did not get expected response from device during coms test")
-
-    def _open_serial(self):
-        """Initializes the serial connection with the specified parameters."""
-        self._serial = serial.Serial(
-            port=self._serial_port, 
-            baudrate=115200, 
-            timeout=self._serial_read_timeout,
-            write_timeout=0.5
-        )
-
-    def _serial_read(self, eor_token: str = EOR_TOKEN) -> bytearray:
-        """Reads from serial until the end-of-response token is encountered."""
-        response = self._serial.read_until(eor_token.encode("utf8")).strip()
-        LOGGER.debug(f"RECV {self._serial_port} :: {response}")
-        return response
-
-    def _repl_read(self, wait_interval: float = 0.2) -> str:
-        """Attempts to read from the REPL prompt"""
-        response = ""
-        end_markers = (UPY_PROMPT, BLOCK_PROMPT)
-        self._serial.timeout = wait_interval
-        start_time = time.monotonic()
-
-        for end_marker in cycle(end_markers):
-            if (time.monotonic() - start_time) > self._serial_read_timeout:
-                break
-            try:
-                response += self._serial_read(eor_token=end_marker).decode("utf-8")
-            except serial.SerialTimeoutException:
-                pass
-            else:
-                time.sleep(0.1)
-                if not self._serial.in_waiting:
-                    break
-
-        self._serial.timeout = self._serial_read_timeout
-        if not response:
-            raise serial.SerialTimeoutException("Timeout while reading from serial.")
-        return response
-
-    def _serial_write(self, command: bytes):
-        """Writes a command to the serial port after clearing the input and output buffers."""
-        self._serial.reset_output_buffer()
-        self._serial.reset_input_buffer()
-        LOGGER.debug(f"SEND {self._serial_port} :: {command}")
-        self._serial.write(command)
-
-    def _extract_response_payload(self, response: str, start_marker: str, end_marker: str) -> Optional[str]:
-        """Extracts a payload from a response delimited by specified start and end markers."""
-        last_start_index = response.rfind(start_marker)
-        if last_start_index == -1:
-            return ""
-        start_index = last_start_index + len(start_marker)
-
-        last_end_index = response.rfind(end_marker)
-        if last_end_index == -1 or last_end_index < start_index:
-            # Could not find end tag - lets see if we can find the UPY prompt
-            if response.endswith(UPY_PROMPT):
-                return response[start_index:]
-            else:
-                return "" # Could not find a valid end marker
-        
-        return response[start_index:last_end_index]
-
-    def _clean_response(self, response: str) -> str:
-        """Cleans up the response string from a MicroPython device to remove unnecessary prompts and markers."""
-        response = self._extract_response_payload(response, EOM_MARKER, EOR_MARKER)
-        response = response.lstrip()
-
-        if platform.system() == "Windows":
-            # Windows does odd things with line endings
-            response = response.replace("\r\r\n", "\n")
-        if response.startswith(BLOCK_PROMPT):
-            # Block prompt can add '...', spaces and newlines
-            try:
-                # Sometimes this part can be a char out!
-                if response[5].isspace():
-                    response = response[6:]
-                else:
-                    response = response[5:]
-            except IndexError as err:
-                raise ValueError(f'Unable to parse response :: {err}')
-        if response.endswith("\r\n"):
-            response = response[:-2] # Take only the last newline off
-        return response
-
-    def _communicate(self,
-                     command: str, 
-                     is_block_command: bool = False, 
-                     ignore_response: bool = False
-                     ) -> Optional[str]:
-        """Handles the sending and receiving of a command to/from the MicroPython device."""
-        command += EOM_MARKER + TERMINATOR
-        if is_block_command:
-            command += TERMINATOR
-
-        self._serial_write(command.encode("utf8"))
-
-        if not ignore_response:
-            if response := self._serial_read().decode():
-                return self._clean_response(response)
-            else:
-                raise Exception("No response when expected")
-        return None
-
-    def get_file_list(self):
-        """ Get a list of files stored on the device """
-        string_list = self._communicate('import os; os.listdir()')
-        
-        # Ensure response looks like a list
-        if not string_list:
-            raise RuntimeError("Empty response from Pico")
-        if string_list[0] != "[" and string_list[-1] != "]":
-            raise RuntimeError(f"Did not get back a list from file listing command :: {string_list}")
-        else:
-            return ast.literal_eval(string_list) if string_list else []
-
-    def stop_exec(self):
-        """ Stop execution and press enter """
-        self.send_stop_exec()
-        self.send_enter()
-
-    def send_stop_exec(self):
-        """ Send keyboard interrupt to stop execution """
-        self._serial_write(b'\x03')  # Ctrl+C -> stop execution
-        time.sleep(0.2) # Give the device time to respond and be flushed
-
-    def send_soft_reboot(self):
-        """ Send soft reboot command (Ctrl+D) """
-        self._serial_write(b'\x04')  # Ctrl+D -> Soft reboot if nothing executing and blank REPL
-        time.sleep(0.2) # Give the device time to respond and be flushed
-
-    def send_enter(self):
-        """ Send a blank enter to exit a block statement """
-        self._serial_write(b'\r\n')
-        
-    def coms_test(self):
-        response = self._communicate("x = 1 + 1; print(x)")
-        return response == "2"
-
-    def run_python_command(self, command, block_command=False):
-        """ Run a generic python command """
-        return self._communicate(command, block_command)
-
-    def download_file(self, pico_filename, save_fp: IO[str]):
-        """ Download a file from the Pico to the host """
-
-        if pico_filename not in self.get_file_list():
-            raise FileNotFoundError(f"File '{pico_filename}' does not exist on Pico")
-
-        file_data = self._communicate(
-            f'with open("{pico_filename}", "r") as f: print(f.read(), end="")',
-            is_block_command=True
-        )
-        save_fp.write(file_data)
-
-    def upload_file(self, local_fp: IO[bytes], pico_file_path, overwrite=False):
-        """ Upload a file from the host to the Pico """
-        if pico_file_path in self.get_file_list():
-            if not overwrite:
-                raise FileExistsError(f"File '{pico_file_path}' already exists on the Pico. Set overwrite=True to overwrite.")
-            else:
-                self._communicate(f"import os; os.remove('{pico_file_path}')")
-
-        # Read the file data from the host
-        local_data = local_fp.read()
-
-        # Upload the file to the pico
-        self._communicate(
-            f'with open("{pico_file_path}", "wb") as f: f.write({local_data})',
-            is_block_command=True
-        )
-
-    def execute_file(self, file_name):
-        LOGGER.debug(f"Executing file {file_name}")
-        self.send_stop_exec()
-        return self._communicate(f'exec(open("{file_name}").read())', ignore_response=True)
-
-    def start_repl(self):
-        # import readline to support familiar command input (arrows, history)
-        if platform.system == "Windows":
-            import pyreadline3
-        else:
-            import readline
-
-        self.send_stop_exec()
-        self.send_soft_reboot()
-
-        # Read serial here to get prompt
-        prompt = self._serial_read(eor_token=UPY_PROMPT).decode("utf-8")
-        while True:
-            raw_command = input(f"{prompt} ")
-            if raw_command == "exit()":
-                raise SystemExit
-
-            command = f"{raw_command}\r" # Add an enter to submit
-            self._serial_write(command.encode("utf-8"))
-            prompt = self._repl_read()
-            # Sometimes a backspace character appears at the left, remove it
-            prompt = re.sub(RE_MATCH_BACKSPACE_BEGINNING, "", prompt)
-            # Remove the command from the response
+import ast
+import time
+import re
+import platform
+from enum import Enum
+from typing import IO, Optional
+from itertools import cycle
+
+import serial
+
+from .logconfig import LOGGER
+
+
+# Constants for communication patterns
+TERMINATOR = '\r\n'  
+UPY_PROMPT = "\r\n>>>"  
+BLOCK_PROMPT = "..."  
+EOR_MARKER = "---f81b734f-7be3-4747-ae0b-c449006b33dd---"
+EOR_TOKEN  = f"{EOR_MARKER}{UPY_PROMPT}"
+EOR_MARKER_COMMAND = f";print('{EOR_MARKER}')"
+EOM_MARKER = f';pass;pass;pass;pass{EOR_MARKER_COMMAND}'
+RE_MATCH_BACKSPACE_BEGINNING = re.compile('^' + re.escape("\x08") + '+')
+
+class MicroPython_Version(Enum):
+    """Enumeration of supported MicroPython versions."""
+    v1_21_0 = "1.21.0"
+
+
+class Pico:
+    """Manage communications with a MicroPython RP2040 device via serial."""
+    def __init__(self, 
+                 serial_port: str, 
+                 micropython_version: MicroPython_Version = MicroPython_Version.v1_21_0, 
+                 start_closed: bool=False,
+                 skip_stop_exec: bool=False,
+                 skip_coms_test: bool=False,
+                 serial_read_timeout: int=15, 
+                 serial_write_timeout: Optional[int]=None
+                 ):
+        """
+        New RP2040 device running MicroPython.
+        args:
+            serial_port (str): serial device of Pico
+            micropython_version (str): Version of MicroPython on device. Does not currently matter
+            start_closed (bool): Creates object without opening the serial port
+            skip_stop_exec (bool): Skip stopping execution of pico running code. Good if your Pico has a main autoexec script
+            skip_coms_test (bool) : Skip a coms test that verifies the coms is good between the computer and Pico
+            serial_read_timeout (int): Read timeout supplied to serial.Serial
+            serial_write_timeout (int): Write timeout supplied to serial.Serial
+        """
+        self._serial_read_timeout = serial_read_timeout
+        self._serial_write_timeout = serial_write_timeout
+        self._upy_version = micropython_version
+        self._serial_port = serial_port
+        self._serial = None
+        if not start_closed:
+            # Open the serial device here
+            self._open_serial()
+
+            # Send stop and reboot to reset Pico state
+            if not skip_stop_exec:
+                self.stop_exec()
+
+            # Run a sanity test to ensure the serial device responds as expected (e.g. does it run micropython)
+            if not skip_coms_test:
+                if not self.coms_test():
+                    raise IOError("Did not get expected response from device during coms test")
+
+    def _open_serial(self):
+        """Initializes the serial connection with the specified parameters."""
+        self._serial = serial.Serial(
+            port=self._serial_port, 
+            baudrate=115200, 
+            timeout=self._serial_read_timeout,
+            write_timeout=0.5
+        )
+
+    def _serial_read(self, eor_token: str = EOR_TOKEN) -> bytearray:
+        """Reads from serial until the end-of-response token is encountered."""
+        response = self._serial.read_until(eor_token.encode("utf8")).strip()
+        LOGGER.debug(f"RECV {self._serial_port} :: {response}")
+        return response
+    
+    def _serial_read_endless(self):
+        """Endless read from serial, useful for viewing all console output"""
+        self._serial.timeout = 0
+        while True:
+            bytes_to_read = self._serial.in_waiting
+            if data_from_serial := self._serial.read(bytes_to_read).decode("utf-8"):
+                print(f"{data_from_serial}")
+            else:
+                time.sleep(0.1)
+
+    def _repl_read(self, wait_interval: float = 0.2) -> str:
+        """Attempts to read from the REPL prompt"""
+        response = ""
+        end_markers = (UPY_PROMPT, BLOCK_PROMPT)
+        self._serial.timeout = wait_interval
+        start_time = time.monotonic()
+
+        for end_marker in cycle(end_markers):
+            if (time.monotonic() - start_time) > self._serial_read_timeout:
+                break
+            try:
+                response += self._serial_read(eor_token=end_marker).decode("utf-8")
+            except serial.SerialTimeoutException:
+                pass
+            else:
+                time.sleep(0.1)
+                if not self._serial.in_waiting:
+                    break
+
+        self._serial.timeout = self._serial_read_timeout
+        if not response:
+            raise serial.SerialTimeoutException("Timeout while reading from serial.")
+        return response
+
+    def _serial_write(self, command: bytes):
+        """Writes a command to the serial port after clearing the input and output buffers."""
+        self._serial.reset_output_buffer()
+        self._serial.reset_input_buffer()
+        LOGGER.debug(f"SEND {self._serial_port} :: {command}")
+        self._serial.write(command)
+
+    def _extract_response_payload(self, response: str, start_marker: str, end_marker: str) -> Optional[str]:
+        """Extracts a payload from a response delimited by specified start and end markers."""
+        last_start_index = response.rfind(start_marker)
+        if last_start_index == -1:
+            return ""
+        start_index = last_start_index + len(start_marker)
+
+        last_end_index = response.rfind(end_marker)
+        if last_end_index == -1 or last_end_index < start_index:
+            # Could not find end tag - lets see if we can find the UPY prompt
+            if response.endswith(UPY_PROMPT):
+                return response[start_index:]
+            else:
+                return "" # Could not find a valid end marker
+        
+        return response[start_index:last_end_index]
+
+    def _clean_response(self, response: str) -> str:
+        """Cleans up the response string from a MicroPython device to remove unnecessary prompts and markers."""
+        response = self._extract_response_payload(response, EOM_MARKER, EOR_MARKER)
+        response = response.lstrip()
+
+        if platform.system() == "Windows":
+            # Windows does odd things with line endings
+            response = response.replace("\r\r\n", "\n")
+        if response.startswith(BLOCK_PROMPT):
+            # Block prompt can add '...', spaces and newlines
+            try:
+                # Sometimes this part can be a char out!
+                if response[5].isspace():
+                    response = response[6:]
+                else:
+                    response = response[5:]
+            except IndexError as err:
+                raise ValueError(f'Unable to parse response :: {err}')
+        if response.endswith("\r\n"):
+            response = response[:-2] # Take only the last newline off
+        return response
+
+    def _communicate(self,
+                     command: str, 
+                     is_block_command: bool = False, 
+                     ignore_response: bool = False
+                     ) -> Optional[str]:
+        """Handles the sending and receiving of a command to/from the MicroPython device."""
+        command += EOM_MARKER + TERMINATOR
+        if is_block_command:
+            command += TERMINATOR
+
+        self._serial_write(command.encode("utf8"))
+
+        if not ignore_response:
+            if response := self._serial_read().decode():
+                return self._clean_response(response)
+            else:
+                raise Exception("No response when expected")
+        return None
+
+    def get_file_list(self):
+        """ Get a list of files stored on the device """
+        string_list = self._communicate('import os; os.listdir()')
+        
+        # Ensure response looks like a list
+        if not string_list:
+            raise RuntimeError("Empty response from Pico")
+        if string_list[0] != "[" and string_list[-1] != "]":
+            raise RuntimeError(f"Did not get back a list from file listing command :: {string_list}")
+        else:
+            return ast.literal_eval(string_list) if string_list else []
+
+    def stop_exec(self):
+        """ Stop execution by a combinatino of reboot and Ctrl+C. Flushes buffers afterwards to get device in known state """
+        self._send_stop_exec(quantity=5)
+        self._send_soft_reboot()
+        time.sleep(0.2)
+        self._send_stop_exec(quantity=5) # If there is an auto boot script, this will clear it
+        time.sleep(0.2)
+        self._send_enter()
+        self._serial.reset_input_buffer()
+        self._serial.reset_output_buffer()
+
+    def _send_stop_exec(self, quantity=1):
+        """ Send keyboard interrupt to stop execution 
+        args:
+            quantity (int) : How many Ctrl+C to send
+        """
+        LOGGER.debug("Sending stop exec (Ctrl+C) to Pico")
+        for _ in range(quantity):
+            self._serial_write(b'\x03')  # Ctrl+C -> stop execution
+
+    def _send_soft_reboot(self):
+        """ Send soft reboot command (Ctrl+D) """
+        LOGGER.debug("Sending soft reboot to Pico (Ctrl+D)")
+        self._serial_write(b'\x04')  # Ctrl+D -> Soft reboot if nothing executing and blank REPL
+
+    def _send_enter(self):
+        """ Send a blank enter to exit a block statement """
+        self._serial_write(b'\r\n')
+        
+    def coms_test(self):
+        response = self._communicate("x = 1 + 1; print(x)")
+        return response == "2"
+
+    def run_python_command(self, command, block_command=False):
+        """ Run a generic python command """
+        return self._communicate(command, block_command)
+
+    def download_file(self, pico_filename, save_fp: IO[str]):
+        """ Download a file from the Pico to the host """
+        download_failed_marker = f"DOWNLOAD{EOR_MARKER}ERROR"
+
+        if pico_filename not in self.get_file_list():
+            raise FileNotFoundError(f"File '{pico_filename}' does not exist on Pico")
+
+        file_data = self._communicate(
+            f"exec(\"try:\\n  with open('{pico_filename}', 'r') as f: print(f.read(), end='')\\nexcept Exception as e: print(f'{download_failed_marker}{{str(e)}}')\")",
+            is_block_command=True
+        )
+        if file_data.startswith(download_failed_marker):
+            LOGGER.error(f"Upload was not successful: {file_data.replace(download_failed_marker, '')}")
+        save_fp.write(file_data)
+        #TODO better exception handling...
+
+    def upload_file(self, local_fp: IO[bytes], pico_file_path, overwrite=False):
+        """ Upload a file from the host to the Pico """
+        if pico_file_path in self.get_file_list():
+            if not overwrite:
+                raise FileExistsError(f"File '{pico_file_path}' already exists on the Pico. Set overwrite=True to overwrite.")
+            else:
+                self._communicate(f"import os; os.remove('{pico_file_path}')")
+
+        # Read the file data from the host
+        local_data = local_fp.read()
+
+        # Upload the file to the pico
+        result = self._communicate(
+            f'with open("{pico_file_path}", "wb") as f: f.write({local_data})',
+            is_block_command=True
+        )
+        LOGGER.debug(f"Response from upload: {result}")
+        if "Traceback" in result:
+            LOGGER.error(f"Pico raised Exception during upload :: {result}")
+
+    def execute_file(self, file_name):
+        LOGGER.debug(f"Executing file {file_name}")
+        self.stop_exec()
+        return self._communicate(f'exec(open("{file_name}").read())', ignore_response=True)
+
+    def start_console_attach(self):
+        LOGGER.info(f"Starting console read from device {self._serial_port}...")
+        self._serial_read_endless()
+
+    def start_repl(self):
+        # import readline to support familiar command input (arrows, history)
+        if platform.system == "Windows":
+            import pyreadline3
+        else:
+            import readline
+
+        self.stop_exec()
+
+        # Read serial here to get prompt
+        prompt = self._serial_read(eor_token=UPY_PROMPT).decode("utf-8")
+        while True:
+            raw_command = input(f"{prompt} ")
+            if raw_command == "exit()":
+                raise SystemExit
+
+            command = f"{raw_command}\r" # Add an enter to submit
+            self._serial_write(command.encode("utf-8"))
+            prompt = self._repl_read()
+            # Sometimes a backspace character appears at the left, remove it
+            prompt = re.sub(RE_MATCH_BACKSPACE_BEGINNING, "", prompt)
+            # Remove the command from the response
             prompt = prompt.replace(raw_command.strip(), "").strip()
```

### Comparing `picox-1.1.4/src/picox.egg-info/PKG-INFO` & `picox-1.2.0/src/picox.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,174 +1,180 @@
-Metadata-Version: 2.1
-Name: picox
-Version: 1.1.4
-Summary: Tools for working with a Rasbperry Pi Pico running MicroPython
-Author: Harvey
-License: MIT License
-        
-        Copyright (c) 2024
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/SparkyTheAlbino/picox
-Project-URL: Documentation, https://github.com/SparkyTheAlbino/picox
-Project-URL: Repository, https://github.com/SparkyTheAlbino/picox.git
-Project-URL: Issues, https://github.com/SparkyTheAlbino/picox/issues
-Keywords: pico,serial,RaspberryPi
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Environment :: Console
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Embedded Systems
-Description-Content-Type: text/markdown
-License-File: LICENCE
-Requires-Dist: pyserial==3.5
-Requires-Dist: pyreadline3==3.4.1; platform_system == "Windows"
-Provides-Extra: dev
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-
-# picox
-`picox` is a tool that facilitates the interaction with Raspberry Pi Pico running MicroPython boards through the terminal or within a Python script. This uses the USB serial port for communication.
-
-Windows, Linux and macOS are supported.
-
-## Features
-- Detect a connected Raspberry Pi Pico device running MicroPython
-- REPL session
-- File operations: Upload, download, execute, and list files on Pi Pico
-- Stop current execution on device
-
-## Known issues
-- REPL can timeout on long operations such as sleep. Its in the nature of how it scans for the end
-- Line endings of files coming out can get a little strange. watch out if there are som extra spaces etc. Best bet is to ensure you always work in the same line endings
-- File operations do not include folder operations __yet__
-
-## Installation
-Install via `pip`:
-
-``` bash 
-pip install picox
-```
-
-
-## CLI Usage
-
-
-### Detecting Pi Pico:
-``` bash
-# get first found device
-picox detect
-
-# get a list of all connected pico devices
-pico detect --all
-
-# Output: COM7 or /dev/ttyUSB0
-```
-
-### REPL session on Pi Pico
-``` bash
-picox repl /dev/ttyUSB0
-```
-
-### Listing files on Pi Pico:
-``` bash
-picox ls /dev/ttyUSB0
-
-# exmaple output:
-# demo.py
-# home.py
-```
-
-### Uploading a file:
-``` bash
-picox upload /dev/ttyUSB0 local.py remote.py --overwrite
-
-# --overrite to force update the file on the Pi Pico
-```
-
-### Downloading a file:
-``` bash
-picox download /dev/ttyUSB0 remote.py local.py
-```
-
-### Executing a file on Pi Pico:
-``` bash
-picox exec /dev/ttyUSB0 remote.py
-```
-
-### Stopping any ongoing operation on Pi Pico:
-``` bash
-picox stop /dev/ttyUSB0
-```
-
-
-## Python Script Usage
-You can also use picox within your Python scripts as follows:
-
-``` python
-from picox import Pico
-from picox.detect import get_first_pico_serial
-
-
-# Init device
-serial_device = get_first_pico_serial()
-pico = Pico(serial_device)
-
-# File listing
-for file in pico.get_file_list():
-    print(file)
-
-# Download
-with open("./local/demo.py", "w") as download_file:
-    pico.download_file("remote_demo.py", download_file)
-
-# Upload
-with open("./local/demo.py", "rb") as upload_file:
-    pico.upload_file(upload_file, "remote_demo.py", overwrite=True)
-
-# Execute
-pico.execute_file("remote_demo.py")
-
-# Halt execution on device
-pico.stop_exec()
-
-# Soft reboot device
-pico.send_soft_reboot()
-```
-
-## Local development
-1. Create virtual env
-``` bash
-python -m venv _env
-```
-2. Activate env
-``` bash
-# Win
-_env/Scripts/activate.ps1
-# nix
-source _env/bin/activate
-```
-3. Install requirements
-``` bash
-pip install -r requirement.txt
-```
-4. Install module editable
-```
-pip install -e .
-```
+Metadata-Version: 2.1
+Name: picox
+Version: 1.2.0
+Summary: Tools for working with a Rasbperry Pi Pico running MicroPython
+Author: Harvey
+License: MIT License
+        
+        Copyright (c) 2024
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: Homepage, https://github.com/SparkyTheAlbino/picox
+Project-URL: Documentation, https://github.com/SparkyTheAlbino/picox
+Project-URL: Repository, https://github.com/SparkyTheAlbino/picox.git
+Project-URL: Issues, https://github.com/SparkyTheAlbino/picox/issues
+Keywords: pico,serial,RaspberryPi
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Environment :: Console
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Embedded Systems
+Description-Content-Type: text/markdown
+License-File: LICENCE
+Requires-Dist: pyserial==3.5
+Requires-Dist: pyreadline3==3.4.1; platform_system == "Windows"
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+
+# picox
+`picox` is a tool that facilitates the interaction with Raspberry Pi Pico running MicroPython boards through the terminal or within a Python script. This uses the USB serial port for communication.
+
+Windows, Linux and macOS are supported.
+
+## Features
+- Detect a connected Raspberry Pi Pico device running MicroPython
+- REPL session
+- File operations: Upload, download, execute, and list files on Pi Pico
+- Stop current execution on device
+
+## Known issues
+- REPL can timeout on long operations such as sleep. Its in the nature of how it scans for the end
+- Line endings of files coming out can get a little strange. watch out if there are som extra spaces etc. Best bet is to ensure you always work in the same line endings
+- File operations do not include folder operations __yet__
+- Most commands will halt what is running on the pico. Such as a detect will stop execution in order to get a good communication test. For a more manual detection, you can use `picox attach <device>` to try and stream stdout from the pico
+
+## Installation
+Install via `pip`:
+
+``` bash 
+pip install picox
+```
+
+
+## CLI Usage
+
+
+### Detecting Pi Pico:
+``` bash
+# get first found device
+picox detect
+
+# get a list of all connected pico devices
+pico detect --all
+
+# Output: COM7 or /dev/ttyUSB0
+```
+
+### REPL session on Pi Pico
+``` bash
+picox repl /dev/ttyUSB0
+```
+
+### View console output from already running pico
+``` bash
+picox attach /dev/ttyUSB0
+```
+
+### Listing files on Pi Pico:
+``` bash
+picox ls /dev/ttyUSB0
+
+# exmaple output:
+# demo.py
+# home.py
+```
+
+### Uploading a file:
+``` bash
+picox upload /dev/ttyUSB0 local.py remote.py --overwrite
+
+# --overrite to force update the file on the Pi Pico
+```
+
+### Downloading a file:
+``` bash
+picox download /dev/ttyUSB0 remote.py local.py
+```
+
+### Executing a file on Pi Pico:
+``` bash
+picox exec /dev/ttyUSB0 remote.py
+```
+
+### Stopping any ongoing operation on Pi Pico:
+``` bash
+picox stop /dev/ttyUSB0
+```
+
+
+## Python Script Usage
+You can also use picox within your Python scripts as follows:
+
+``` python
+from picox import Pico
+from picox.detect import get_first_pico_serial
+
+
+# Init device
+serial_device = get_first_pico_serial()
+pico = Pico(serial_device)
+
+# File listing
+for file in pico.get_file_list():
+    print(file)
+
+# Download
+with open("./local/demo.py", "w") as download_file:
+    pico.download_file("remote_demo.py", download_file)
+
+# Upload
+with open("./local/demo.py", "rb") as upload_file:
+    pico.upload_file(upload_file, "remote_demo.py", overwrite=True)
+
+# Execute
+pico.execute_file("remote_demo.py")
+
+# Halt execution on device
+pico.stop_exec()
+
+# Soft reboot device
+pico.send_soft_reboot()
+```
+
+## Local development
+1. Create virtual env
+``` bash
+python -m venv _env
+```
+2. Activate env
+``` bash
+# Win
+_env/Scripts/activate.ps1
+# nix
+source _env/bin/activate
+```
+3. Install requirements
+``` bash
+pip install -r requirement.txt
+```
+4. Install module editable
+```
+pip install -e .
+```
```

