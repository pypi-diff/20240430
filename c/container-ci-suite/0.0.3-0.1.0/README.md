# Comparing `tmp/container-ci-suite-0.0.3.tar.gz` & `tmp/container_ci_suite-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "container-ci-suite-0.0.3.tar", last modified: Wed Aug  3 15:24:26 2022, max compression
+gzip compressed data, was "container_ci_suite-0.1.0.tar", last modified: Tue Apr 30 13:34:13 2024, max compression
```

## Comparing `container-ci-suite-0.0.3.tar` & `container_ci_suite-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 15:24:26.438980 container-ci-suite-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-08-03 15:24:12.000000 container-ci-suite-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4185 2022-08-03 15:24:26.438980 container-ci-suite-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3536 2022-08-03 15:24:12.000000 container-ci-suite-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 15:24:26.438980 container-ci-suite-0.0.3/container_ci_suite/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-03 15:24:12.000000 container-ci-suite-0.0.3/container_ci_suite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18241 2022-08-03 15:24:12.000000 container-ci-suite-0.0.3/container_ci_suite/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-08-03 15:24:12.000000 container-ci-suite-0.0.3/container_ci_suite/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2402 2022-08-03 15:24:12.000000 container-ci-suite-0.0.3/container_ci_suite/container.py
--rw-r--r--   0 runner    (1001) docker     (121)     3573 2022-08-03 15:24:12.000000 container-ci-suite-0.0.3/container_ci_suite/git.py
--rw-r--r--   0 runner    (1001) docker     (121)     4441 2022-08-03 15:24:12.000000 container-ci-suite-0.0.3/container_ci_suite/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 15:24:26.438980 container-ci-suite-0.0.3/container_ci_suite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4185 2022-08-03 15:24:26.000000 container-ci-suite-0.0.3/container_ci_suite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-08-03 15:24:26.000000 container-ci-suite-0.0.3/container_ci_suite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-03 15:24:26.000000 container-ci-suite-0.0.3/container_ci_suite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-08-03 15:24:26.000000 container-ci-suite-0.0.3/container_ci_suite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-03 15:24:26.000000 container-ci-suite-0.0.3/container_ci_suite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-03 15:24:26.438980 container-ci-suite-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2437 2022-08-03 15:24:12.000000 container-ci-suite-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:34:13.533852 container_ci_suite-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-30 13:34:10.000000 container_ci_suite-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-30 13:34:13.533852 container_ci_suite-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-30 13:34:10.000000 container_ci_suite-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:34:13.529852 container_ci_suite-0.1.0/container_ci_suite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:34:10.000000 container_ci_suite-0.1.0/container_ci_suite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19674 2024-04-30 13:34:10.000000 container_ci_suite-0.1.0/container_ci_suite/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-30 13:34:10.000000 container_ci_suite-0.1.0/container_ci_suite/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-30 13:34:10.000000 container_ci_suite-0.1.0/container_ci_suite/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-30 13:34:10.000000 container_ci_suite-0.1.0/container_ci_suite/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16199 2024-04-30 13:34:10.000000 container_ci_suite-0.1.0/container_ci_suite/helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-30 13:34:10.000000 container_ci_suite-0.1.0/container_ci_suite/imagestreams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-30 13:34:10.000000 container_ci_suite-0.1.0/container_ci_suite/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26373 2024-04-30 13:34:10.000000 container_ci_suite-0.1.0/container_ci_suite/openshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8495 2024-04-30 13:34:10.000000 container_ci_suite-0.1.0/container_ci_suite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:34:13.533852 container_ci_suite-0.1.0/container_ci_suite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-30 13:34:13.000000 container_ci_suite-0.1.0/container_ci_suite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-30 13:34:13.000000 container_ci_suite-0.1.0/container_ci_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:34:13.000000 container_ci_suite-0.1.0/container_ci_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-30 13:34:13.000000 container_ci_suite-0.1.0/container_ci_suite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-30 13:34:13.000000 container_ci_suite-0.1.0/container_ci_suite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:34:13.533852 container_ci_suite-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-30 13:34:10.000000 container_ci_suite-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:34:13.529852 container_ci_suite-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-30 13:34:10.000000 container_ci_suite-0.1.0/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-30 13:34:10.000000 container_ci_suite-0.1.0/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-30 13:34:10.000000 container_ci_suite-0.1.0/tests/test_openshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-30 13:34:10.000000 container_ci_suite-0.1.0/tests/test_utils.py
```

### Comparing `container-ci-suite-0.0.3/LICENSE` & `container_ci_suite-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `container-ci-suite-0.0.3/container_ci_suite/api.py` & `container_ci_suite-0.1.0/container_ci_suite/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 from typing import List
 from os import getenv
 from pathlib import Path
 from tempfile import mkdtemp, mktemp
 
 from container_ci_suite.container import DockerCLIWrapper
+from container_ci_suite.helm import HelmChartsAPI
 from container_ci_suite.utils import (
     run_command,
     get_file_content,
     get_mount_ca_file,
     get_full_ca_file_path,
     get_os_environment,
     get_mount_options_from_s2i_args,
@@ -305,15 +306,15 @@
         except subprocess.CalledProcessError:
             logger.error(
                 f"'npm --version' does not work inside the image {self.image_name}."
             )
             return False
 
         # TODO
-        # Add {self.iamge_name}-testapp as soon as function `s2i_create_df` is ready.
+        # Add {self.image_name}-testapp as soon as function `s2i_create_df` is ready.
         DockerCLIWrapper.run_docker_command(
             f"run -d {get_mount_ca_file()} --rm --cidfile={self.cid_file} {self.image_name}"
         )
         if not self.wait_for_cid():
             logger.error("Container did not create cidfile.")
             return False
 
@@ -365,16 +366,28 @@
     #
     #     # Check only lines which starts with VERSIONS
     #     latest_version=$(grep '^VERSIONS' Makefile | rev | cut -d ' ' -f 1 | rev )
     #     test_lib_dir=$(dirname "$(readlink -f "$0")")
     #     python3 "${test_lib_dir}/check_imagestreams.py" "$latest_version"
     #
 
-    def doc_content_old(self):
-        pass
+    def doc_content_old(self, strings: List) -> bool:
+        logger.info("Testing documentation in the container image")
+        files_to_check = ["help.1"]
+        for f in files_to_check:
+            doc_content = DockerCLIWrapper.docker_run_command(f'--rm {self.image_name} /bin/bash -c cat {f}')
+            for term in strings:
+                # test = re.search(f"{term}", doc_content)
+                logger.info(f"ERROR: File /{f} does not contain '{term}'.")
+                return False
+            for term in ["TH", "PP", "SH"]:
+                if term not in doc_content:
+                    logger.info(f"ERROR: help.1 is probably not in troff or groff format, since {term} is missing")
+                    return False
+        return True
 
     #         # ct_doc_content_old [strings]
     #         # --------------------
     #         # Looks for occurence of stirngs in the documentation files and checks
     #         # the format of the files. Files examined: help.1
     #         # Argument: strings - strings expected to appear in the documentation
     #         # Uses: $IMAGE_NAME - name of the image being tested
@@ -444,7 +457,22 @@
                 new_env = env_format.replace('VALUE', value)
                 find_env = re.findall(rf"{new_env}", filter_envs)
                 if not find_env:
                     logger.error(f"Value {value} is missing from variable {var_name}")
                     logger.error(filtered_envs)
                     return False
         return True
+
+    def test_helm_chart(self, path: str,  package_name: str, version: str, test_check_string: str):
+        hc = HelmChartsAPI(path=path, package_name=package_name, version=version)
+        if not hc.helm_package():
+            return False
+        hc.helm_installation()
+        hc.test_helm_chart(test_check_string)
+
+    def test_helm_chart_imagestreams(self, path: str, package_name: str, version: str, registry: str) -> bool:
+        hc = HelmChartsAPI(path=path, package_name=package_name, version=version)
+        if not hc.helm_package():
+            return False
+        hc.helm_installation()
+        hc.check_imagestreams(version, registry)
+        return True
```

### Comparing `container-ci-suite-0.0.3/container_ci_suite/constants.py` & `container_ci_suite-0.1.0/container_ci_suite/constants.py`

 * *Files identical despite different names*

### Comparing `container-ci-suite-0.0.3/container_ci_suite/container.py` & `container_ci_suite-0.1.0/container_ci_suite/container.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # MIT License
 #
 # Copyright (c) 2018-2019 Red Hat, Inc.
+import time
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -28,31 +29,31 @@
     def run_docker_command(
         cmd, return_output: bool = True, ignore_error: bool = False, shell: bool = True
     ):
         """
         Run docker command:
         """
         return run_command(
-            f"docker {cmd}",
+            f"podman {cmd}",
             return_output=return_output,
             ignore_error=ignore_error,
             shell=shell,
         )
 
     @staticmethod
     def docker_image_exists(image_name: str) -> bool:
         """
         Check if docker image exists or not
+        :param image_name: image to check
+        :return True: In case if image is present
+                False: In case if image is not present
         """
         output = DockerCLIWrapper.run_docker_command(
-            f"images {image_name}", ignore_error=True
-        )
-        if image_name in output:
-            return True
-        return False
+            f"images -q {image_name}", ignore_error=True, return_output=True)
+        return True if output != "" else False
 
     @staticmethod
     def docker_inspect(field: str, src_image: str) -> str:
         return DockerCLIWrapper.run_docker_command(
             f"docker inspect -f '{field}' {src_image}"
         )
 
@@ -61,7 +62,27 @@
         return DockerCLIWrapper.run_docker_command(f"run {cmd}")
 
     @staticmethod
     def docker_get_user_id(src_image, user):
         return DockerCLIWrapper.docker_run_command(
             f"--rm {src_image} bash -c 'id -u {user} 2>/dev/null"
         )
+
+    @staticmethod
+    def docker_pull_image(image_name: str, loops: int = 10) -> bool:
+        """
+        Function checks if image_name is present in system.
+        In case it isn't, try to pull it for specific count of loops
+        Default is 10.
+        """
+        if DockerCLIWrapper.docker_image_exists(image_name=image_name):
+            print("Pulled image already exists.")
+            return True
+        for loop in range(loops):
+            ret_val = DockerCLIWrapper.run_docker_command(
+                cmd=f"pull {image_name}"
+            )
+            if ret_val == 0:
+                return True
+            print(f"Pulling of image {image_name} failed. Let's wait {loop*5} seconds and try again.")
+            time.sleep(loop*5)
+        return False
```

### Comparing `container-ci-suite-0.0.3/container_ci_suite/git.py` & `container_ci_suite-0.1.0/container_ci_suite/git.py`

 * *Files identical despite different names*

### Comparing `container-ci-suite-0.0.3/container_ci_suite/utils.py` & `container_ci_suite-0.1.0/container_ci_suite/imagestreams.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/bin/env python3
+
 # MIT License
 #
 # Copyright (c) 2018-2019 Red Hat, Inc.
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
@@ -16,122 +18,91 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+import json
 import os
-import logging
-import subprocess
-import re
 
-from typing import List
 from pathlib import Path
+from typing import Dict, List, Any
 
-from container_ci_suite.constants import CA_FILE_PATH
+IMAGESTREAMS_DIR: str = "imagestreams"
 
-logger = logging.getLogger(__name__)
 
+class ImageStreamChecker(object):
+    version: str = ""
 
-def get_file_content(filename: Path) -> str:
-    with open(str(filename)) as f:
-        return f.read()
-
-
-def get_full_ca_file_path() -> Path:
-    return Path(CA_FILE_PATH)
-
-
-def get_os_environment(variable: str) -> str:
-    return os.getenv(variable)
-
-
-def get_mount_ca_file() -> str:
-    if get_os_environment("NPM_REGISTRY") and get_full_ca_file_path().exists():
-        return f"-v {CA_FILE_PATH}:{CA_FILE_PATH}:Z"
-    return ""
-
-
-def get_npm_variables():
-    npm_registry = get_os_environment("NPM_REGISTRY")
-    if npm_registry and get_full_ca_file_path().exists():
-        return f"-e NPM_MIRROR={npm_registry} {get_mount_ca_file()}"
-    return ""
-
-
-def get_registry_name(os: str) -> str:
-    return "registry.redhat.io" if os.startswith("rhel") else "docker.io"
-
-
-def get_mount_options_from_s2i_args(s2i_args: str) -> str:
-    # Check if -v parameter is present in s2i_args and add it into docker build command
-    searchObj = re.search(r"(-v \.*\S*)", s2i_args)
-    logger.debug(searchObj)
-    if not searchObj:
-        return ""
-
-    logger.debug(searchObj.group(1))
-    mount_options = searchObj.group()
-
-    logger.info(f"Mount options: {mount_options}")
-    return searchObj.group()
-
-
-def get_env_commands_from_s2i_args(s2i_args: str) -> List:
-    matchObj = re.findall(r"(-e|--env)\s*(\S*)=(\S*)", s2i_args)
-    logger.debug(matchObj)
-    env_content: List = []
-    if matchObj:
-        env_content.extend([f"ENV {x[1]}={x[2]}" for x in matchObj])
-        logger.debug(env_content)
-        return env_content
-    return env_content
-
-
-def get_public_image_name(os: str, base_image_name: str, version: str) -> str:
-    registry = get_registry_name(os)
-    if os == "rhel7":
-        return f"{registry}/rhscl/{base_image_name}-{version}-rhel7"
-    elif os == "rhel8":
-        return f"{registry}/rhel8/{base_image_name}-{version}"
-    else:
-        return f"{registry}/centos/{base_image_name}-{version}-centos7"
-
-
-def run_command(
-    cmd,
-    return_output: bool = True,
-    ignore_error: bool = False,
-    shell: bool = True,
-    **kwargs,
-):
-    """
-    Run provided command on host system using the same user as invoked this code.
-    Raises subprocess.CalledProcessError if it fails.
-    :param cmd: list or str
-    :param return_output: bool, return output of the command
-    :param ignore_error: bool, do not fail in case nonzero return code
-    :param shell: bool, run command in shell
-    :return: None or str
-    """
-    logger.debug("command: %r", cmd)
-    try:
-        if return_output:
-            return subprocess.check_output(
-                cmd,
-                stderr=subprocess.STDOUT,
-                universal_newlines=True,
-                shell=shell,
-                **kwargs,
+    def __init__(self, working_dir: Path = Path(".")):
+        self.results: Dict[Any, Any] = {}
+        self.working_dir = working_dir
+
+    def get_latest_version(self) -> str:
+        latest_version = ""
+        with open(self.working_dir / "Makefile") as f:
+            for line in f:
+                if not line.startswith("VERSIONS ="):
+                    continue
+                versions = line.split("=")[1].strip().split()
+                latest_version = versions[-1]
+        print(f"The latest version is {latest_version}.")
+        return latest_version
+
+    def load_json_file(self, filename: Path) -> Any:
+        with open(str(filename)) as f:
+            data = json.load(f)
+            isinstance(data, Dict)
+            return data
+
+    def check_version(self, json_dict: Dict[Any, Any]) -> List[str]:
+        res = []
+        for tags in json_dict["spec"]["tags"]:
+            print(
+                f"check_version: Compare tags['name']:'{tags['name']}' against version:'{self.version}'"
+            )
+            # The name can be"<stream>" or "<stream>-elX" or "<stream>-ubiX"
+            if tags["name"] == self.version or tags["name"].startswith(
+                self.version + "-"
+            ):
+                res.append(tags)
+        return res
+
+    def check_latest_tag(self, json_dict: Dict[Any, Any]) -> bool:
+        latest_tag_correct: bool = False
+        for tags in json_dict["spec"]["tags"]:
+            if tags["name"] != "latest":
+                continue
+            print(
+                f"check_latest_tag: Compare tags['name']:'{tags['name']}' against version:'{self.version}'"
             )
-        else:
-            return subprocess.check_call(cmd, shell=shell, **kwargs)
-    except subprocess.CalledProcessError as cpe:
-        if ignore_error:
-            if return_output:
-                return cpe.output
-            else:
-                return cpe.returncode
-        else:
-            logger.error(f"failed with code {cpe.returncode} and output:\n{cpe.output}")
-            raise cpe
+            # The latest can link to either "<stream>" or "<stream>-elX" or "<stream>-ubiX"
+            if tags["from"]["name"] == self.version or tags["from"]["name"].startswith(
+                self.version + "-"
+            ):
+                latest_tag_correct = True
+                print("Latest tag found.")
+        return latest_tag_correct
+
+    def check_imagestreams(self, version: str) -> int:
+        self.version = version
+        p = Path(".")
+        json_files = p.glob(f"{IMAGESTREAMS_DIR}/*.json")
+        if not json_files:
+            print(f"No json files present in {IMAGESTREAMS_DIR}.")
+            return 0
+        for f in json_files:
+            if os.environ.get("TARGET") in ("rhel7", "centos7") and "aarch64" in str(f):
+                print("Imagestream aarch64 is not supported on rhel7")
+                continue
+            print(f"Checking file {str(f)}.")
+            json_dict = self.load_json_file(f)
+            if not (self.check_version(json_dict) and self.check_latest_tag(json_dict)):
+                print(
+                    f"The latest version is not present in {str(f)} or in latest tag."
+                )
+                self.results[f] = False
+        if self.results:
+            return 1
+        print("Imagestreams contains the latest version.")
+        return 0
```

### Comparing `container-ci-suite-0.0.3/setup.py` & `container_ci_suite-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 
 setup(
     name="container-ci-suite",
     description='A python3 container CI tool for testing images.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version="0.0.3",
+    version="0.1.0",
     keywords='tool,containers,images,tests',
     packages=find_packages(exclude=["tests"]),
     url="https://github.com/phracek/container-ci-suite",
     license="MIT",
     author="Petr Hracek",
     author_email="phracek@redhat.com",
     install_requires=get_requirements(),
```

