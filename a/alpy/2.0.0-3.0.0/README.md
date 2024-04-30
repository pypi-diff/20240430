# Comparing `tmp/alpy-2.0.0.tar.gz` & `tmp/alpy-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpy-2.0.0.tar", last modified: Sun May 28 13:44:42 2023, max compression
+gzip compressed data, was "alpy-3.0.0.tar", last modified: Tue Apr 30 10:45:44 2024, max compression
```

## Comparing `alpy-2.0.0.tar` & `alpy-3.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 13:44:42.864233 alpy-2.0.0/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-05-28 13:44:41.000000 alpy-2.0.0/COPYING
--rw-r--r--   0 root         (0) root         (0)    15489 2023-05-28 13:44:42.864233 alpy-2.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    14412 2023-05-28 13:44:41.000000 alpy-2.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 13:44:42.863233 alpy-2.0.0/alpy/
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-05-28 13:44:41.000000 alpy-2.0.0/alpy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      196 2023-05-28 13:44:41.000000 alpy-2.0.0/alpy/config.py
--rw-rw-rw-   0 root         (0) root         (0)     6167 2023-05-28 13:44:41.000000 alpy-2.0.0/alpy/console.py
--rw-rw-rw-   0 root         (0) root         (0)     9103 2023-05-28 13:44:41.000000 alpy-2.0.0/alpy/container.py
--rw-rw-rw-   0 root         (0) root         (0)    11164 2023-05-28 13:44:41.000000 alpy-2.0.0/alpy/node.py
--rw-rw-rw-   0 root         (0) root         (0)     5156 2023-05-28 13:44:41.000000 alpy-2.0.0/alpy/pexpect_log.py
--rw-rw-rw-   0 root         (0) root         (0)     9508 2023-05-28 13:44:41.000000 alpy-2.0.0/alpy/qemu.py
--rw-rw-rw-   0 root         (0) root         (0)     4594 2023-05-28 13:44:41.000000 alpy-2.0.0/alpy/remote_shell.py
--rw-rw-rw-   0 root         (0) root         (0)     1490 2023-05-28 13:44:41.000000 alpy-2.0.0/alpy/run.py
--rw-rw-rw-   0 root         (0) root         (0)     5286 2023-05-28 13:44:41.000000 alpy-2.0.0/alpy/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 13:44:42.864233 alpy-2.0.0/alpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15489 2023-05-28 13:44:42.000000 alpy-2.0.0/alpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      325 2023-05-28 13:44:42.000000 alpy-2.0.0/alpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 13:44:42.000000 alpy-2.0.0/alpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-28 13:44:42.000000 alpy-2.0.0/alpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-28 13:44:42.000000 alpy-2.0.0/alpy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-28 13:44:42.864233 alpy-2.0.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1385 2023-05-28 13:44:41.000000 alpy-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:45:44.696021 alpy-3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2024-04-30 10:45:33.000000 alpy-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15718 2024-04-30 10:45:44.696021 alpy-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    14412 2024-04-30 10:45:33.000000 alpy-3.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:45:44.694021 alpy-3.0.0/alpy/
+-rw-rw-rw-   0 root         (0) root         (0)       89 2024-04-30 10:45:33.000000 alpy-3.0.0/alpy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-04-30 10:45:33.000000 alpy-3.0.0/alpy/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6167 2024-04-30 10:45:33.000000 alpy-3.0.0/alpy/console.py
+-rw-rw-rw-   0 root         (0) root         (0)     9144 2024-04-30 10:45:33.000000 alpy-3.0.0/alpy/container.py
+-rw-rw-rw-   0 root         (0) root         (0)    11250 2024-04-30 10:45:33.000000 alpy-3.0.0/alpy/node.py
+-rw-rw-rw-   0 root         (0) root         (0)     5156 2024-04-30 10:45:33.000000 alpy-3.0.0/alpy/pexpect_log.py
+-rw-rw-rw-   0 root         (0) root         (0)     9517 2024-04-30 10:45:33.000000 alpy-3.0.0/alpy/qemu.py
+-rw-rw-rw-   0 root         (0) root         (0)     4594 2024-04-30 10:45:33.000000 alpy-3.0.0/alpy/remote_shell.py
+-rw-rw-rw-   0 root         (0) root         (0)     1490 2024-04-30 10:45:33.000000 alpy-3.0.0/alpy/run.py
+-rw-rw-rw-   0 root         (0) root         (0)     5286 2024-04-30 10:45:33.000000 alpy-3.0.0/alpy/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:45:44.696021 alpy-3.0.0/alpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15718 2024-04-30 10:45:44.000000 alpy-3.0.0/alpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2024-04-30 10:45:44.000000 alpy-3.0.0/alpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 10:45:44.000000 alpy-3.0.0/alpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-30 10:45:44.000000 alpy-3.0.0/alpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-30 10:45:44.000000 alpy-3.0.0/alpy.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2024-04-30 10:45:33.000000 alpy-3.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 10:45:44.696021 alpy-3.0.0/setup.cfg
```

### Comparing `alpy-2.0.0/COPYING` & `alpy-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alpy-2.0.0/PKG-INFO` & `alpy-3.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: alpy
-Version: 2.0.0
+Version: 3.0.0
 Summary: Library for testing network virtual appliances using Docker
-Home-page: https://gitlab.com/abogdanenko/alpy
-Author: Alexey Bogdanenko
-Author-email: alexey@bogdanenko.com
+Author-email: Alexey Bogdanenko <alexey@bogdanenko.com>
+Project-URL: Changelog, https://gitlab.com/abogdanenko/alpy/-/blob/main/CHANGELOG.md
+Project-URL: Homepage, https://gitlab.com/abogdanenko/alpy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-License-File: COPYING
+License-File: LICENSE
+Requires-Dist: docker
+Requires-Dist: pexpect
+Requires-Dist: qmp
 
 ####
 Alpy
 ####
 
 *Test network virtual appliance using Docker containers*
```

### Comparing `alpy-2.0.0/README.rst` & `alpy-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `alpy-2.0.0/alpy/console.py` & `alpy-3.0.0/alpy/console.py`

 * *Files identical despite different names*

### Comparing `alpy-2.0.0/alpy/container.py` & `alpy-3.0.0/alpy/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,15 @@
     :param image: ID or name of Docker image containing *ip* executable, for
        example, "busybox:latest"
     :type image: str
     :param timeout: maximum number of seconds to wait. The function waits for
        the temporary container to configure the interface.
     :type timeout: int
     """
+    # pylint: disable=too-many-arguments
     add_ip_address(
         container_name,
         address,
         docker_client=docker_client,
         image=image,
         timeout=timeout,
     )
```

### Comparing `alpy-2.0.0/alpy/node.py` & `alpy-3.0.0/alpy/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         docker_client,
         node_container_name,
         interface_name,
         timeout,
         busybox_image,
         iproute2_image,
     ):
+        # pylint: disable=too-many-arguments
         self._docker_client = docker_client
         self._join_node_ns = "container:" + node_container_name
         self._interface_name = interface_name
         self._timeout = timeout
         self._busybox_image = busybox_image
         self._iproute2_image = iproute2_image
         self._interface_in_host_namespace = False
@@ -232,14 +233,15 @@
     :type timeout: int
     :return: a node
     :rtype: :py:class:`alpy.node.Node`
 
     For explanation of `busybox_image` and `iproute2_image` parameters see
     "Building a network of nodes" README section.
     """
+    # pylint: disable=too-many-arguments
     node_container = NodeContainer(
         docker_client=docker_client,
         name=name,
         timeout=timeout,
         image=busybox_image,
     )
     node_tap = NodeTap(
```

### Comparing `alpy-2.0.0/alpy/pexpect_log.py` & `alpy-3.0.0/alpy/pexpect_log.py`

 * *Files identical despite different names*

### Comparing `alpy-2.0.0/alpy/qemu.py` & `alpy-3.0.0/alpy/qemu.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from qmp import QEMUMonitorProtocol
 
 import alpy.config
 import alpy.utils
 
 QMP_SOCKET_FILENAME = "qmp.sock"
 """Path to unix domain socket for QMP"""
-OVMF_VARS_COPY_FILENAME = "OVMF_VARS.fd"
+OVMF_VARS_COPY_FILENAME = "OVMF_VARS_4M.fd"
 """OVMF variables store filename"""
 
 
 @contextlib.contextmanager
 def run(qemu_args, timeout):
     """QEMU process context manager.
 
@@ -256,15 +256,15 @@
     On entering context this context manager makes a file to store OVMF
     variables in. The path is specified by
     :py:data:`alpy.qemu.OVMF_VARS_COPY_FILENAME`. The file is a copy of
     "/usr/share/OVMF/OVMF_VARS.fd". On exiting the context the file is removed.
 
     See also :py:func:`alpy.qemu.get_uefi_firmware_args`.
     """
-    shutil.copy("/usr/share/OVMF/OVMF_VARS.fd", OVMF_VARS_COPY_FILENAME)
+    shutil.copy("/usr/share/OVMF/OVMF_VARS_4M.fd", OVMF_VARS_COPY_FILENAME)
     try:
         yield
     finally:
         Path(OVMF_VARS_COPY_FILENAME).unlink()
 
 
 def get_uefi_firmware_args():
@@ -296,15 +296,15 @@
     # firmware executable code
     args.append("-drive")
     args.append(
         "if=pflash,"
         "format=raw,"
         "unit=0,"
         "readonly=on,"
-        "file=/usr/share/OVMF/OVMF_CODE.fd"
+        "file=/usr/share/OVMF/OVMF_CODE_4M.fd"
     )
 
     # firmware variable store
     args.append("-drive")
     args.append("if=pflash,format=raw,unit=1,file=" + OVMF_VARS_COPY_FILENAME)
 
     return args
```

### Comparing `alpy-2.0.0/alpy/remote_shell.py` & `alpy-3.0.0/alpy/remote_shell.py`

 * *Files identical despite different names*

### Comparing `alpy-2.0.0/alpy/run.py` & `alpy-3.0.0/alpy/run.py`

 * *Files identical despite different names*

### Comparing `alpy-2.0.0/alpy/utils.py` & `alpy-3.0.0/alpy/utils.py`

 * *Files identical despite different names*

### Comparing `alpy-2.0.0/alpy.egg-info/PKG-INFO` & `alpy-3.0.0/alpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: alpy
-Version: 2.0.0
+Version: 3.0.0
 Summary: Library for testing network virtual appliances using Docker
-Home-page: https://gitlab.com/abogdanenko/alpy
-Author: Alexey Bogdanenko
-Author-email: alexey@bogdanenko.com
+Author-email: Alexey Bogdanenko <alexey@bogdanenko.com>
+Project-URL: Changelog, https://gitlab.com/abogdanenko/alpy/-/blob/main/CHANGELOG.md
+Project-URL: Homepage, https://gitlab.com/abogdanenko/alpy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-License-File: COPYING
+License-File: LICENSE
+Requires-Dist: docker
+Requires-Dist: pexpect
+Requires-Dist: qmp
 
 ####
 Alpy
 ####
 
 *Test network virtual appliance using Docker containers*
```

