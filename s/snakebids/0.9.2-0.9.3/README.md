# Comparing `tmp/snakebids-0.9.2.tar.gz` & `tmp/snakebids-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakebids-0.9.2.tar", max compression
+gzip compressed data, was "snakebids-0.9.3.tar", max compression
```

## Comparing `snakebids-0.9.2.tar` & `snakebids-0.9.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1065 2023-08-22 18:06:43.190023 snakebids-0.9.2/LICENSE
--rw-r--r--   0        0        0     4696 2023-08-22 18:06:43.190023 snakebids-0.9.2/README.md
--rw-r--r--   0        0        0     3502 2023-08-22 18:07:07.370407 snakebids-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      686 2023-08-22 18:07:07.370407 snakebids-0.9.2/snakebids/__init__.py
--rw-r--r--   0        0        0     1939 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/admin.py
--rw-r--r--   0        0        0    11734 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/app.py
--rw-r--r--   0        0        0    12301 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/cli.py
--rw-r--r--   0        0        0      859 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/core/__init__.py
--rw-r--r--   0        0        0     8194 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/core/construct_bids.py
--rw-r--r--   0        0        0    31486 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/core/datasets.py
--rw-r--r--   0        0        0     9326 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/core/filtering.py
--rw-r--r--   0        0        0    28503 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/core/input_generation.py
--rw-r--r--   0        0        0     1623 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/exceptions.py
--rw-r--r--   0        0        0     4219 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/io/console.py
--rw-r--r--   0        0        0     3271 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/io/printing.py
--rw-r--r--   0        0        0     2367 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/plugins/validator.py
--rw-r--r--   0        0        0      340 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/project_template/cookiecutter.json
--rw-r--r--   0        0        0     1226 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/project_template/hooks/post_gen_project.py
--rw-r--r--   0        0        0       68 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/README.md
--rw-r--r--   0        0        0        7 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/docs/.gitignore
--rw-r--r--   0        0        0      634 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/docs/Makefile
--rw-r--r--   0        0        0     1997 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/docs/conf.py
--rw-r--r--   0        0        0     3180 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/docs/getting_started/installation.md
--rw-r--r--   0        0        0      305 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/docs/index.md
--rw-r--r--   0        0        0       96 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/docs/requirements.txt
--rw-r--r--   0        0        0      150 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/docs/usage/app_cli.md
--rw-r--r--   0        0        0      117 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/docs/usage/snakemake_cli.md
--rw-r--r--   0        0        0     1221 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/setup.py
--rw-r--r--   0        0        0     3365 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/{{cookiecutter.__app_name}}/config/snakebids.yml
--rw-r--r--   0        0        0      913 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/{{cookiecutter.__app_name}}/pipeline_description.json
--rwxr-xr-x   0        0        0      532 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/{{cookiecutter.__app_name}}/run.py
--rw-r--r--   0        0        0     1635 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/{{cookiecutter.__app_name}}/workflow/Snakefile
--rw-r--r--   0        0        0        0 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/py.typed
--rw-r--r--   0        0        0       13 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/resources/__init__.py
--rw-r--r--   0        0        0     4339 2023-08-22 18:06:43.194023 snakebids-0.9.2/snakebids/resources/bids_tags.json
--rw-r--r--   0        0        0     4828 2023-08-22 18:06:43.198023 snakebids-0.9.2/snakebids/types.py
--rw-r--r--   0        0        0       70 2023-08-22 18:06:43.198023 snakebids-0.9.2/snakebids/utils/__init__.py
--rw-r--r--   0        0        0     5839 2023-08-22 18:06:43.198023 snakebids-0.9.2/snakebids/utils/output.py
--rw-r--r--   0        0        0      990 2023-08-22 18:06:43.198023 snakebids-0.9.2/snakebids/utils/sb_itertools.py
--rw-r--r--   0        0        0     4947 2023-08-22 18:06:43.198023 snakebids-0.9.2/snakebids/utils/snakemake_io.py
--rw-r--r--   0        0        0       91 2023-08-22 18:06:43.198023 snakebids-0.9.2/snakebids/utils/user_property.py
--rw-r--r--   0        0        0      242 2023-08-22 18:06:43.198023 snakebids-0.9.2/snakebids/utils/user_property.pyi
--rw-r--r--   0        0        0    16203 2023-08-22 18:06:43.198023 snakebids-0.9.2/snakebids/utils/utils.py
--rw-r--r--   0        0        0     6511 1970-01-01 00:00:00.000000 snakebids-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-09-15 15:17:01.891785 snakebids-0.9.3/LICENSE
+-rw-r--r--   0        0        0     4696 2023-09-15 15:17:01.891785 snakebids-0.9.3/README.md
+-rw-r--r--   0        0        0     3502 2023-09-15 15:17:27.868157 snakebids-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      686 2023-09-15 15:17:27.872157 snakebids-0.9.3/snakebids/__init__.py
+-rw-r--r--   0        0        0     1939 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/admin.py
+-rw-r--r--   0        0        0    12011 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/app.py
+-rw-r--r--   0        0        0    12301 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/cli.py
+-rw-r--r--   0        0        0      859 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/core/__init__.py
+-rw-r--r--   0        0        0     8194 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/core/construct_bids.py
+-rw-r--r--   0        0        0    31486 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/core/datasets.py
+-rw-r--r--   0        0        0     9326 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/core/filtering.py
+-rw-r--r--   0        0        0    30555 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/core/input_generation.py
+-rw-r--r--   0        0        0     1623 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/exceptions.py
+-rw-r--r--   0        0        0     4219 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/io/console.py
+-rw-r--r--   0        0        0     3271 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/io/printing.py
+-rw-r--r--   0        0        0     2366 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/plugins/validator.py
+-rw-r--r--   0        0        0      340 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/project_template/cookiecutter.json
+-rw-r--r--   0        0        0     1226 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/project_template/hooks/post_gen_project.py
+-rw-r--r--   0        0        0       68 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/README.md
+-rw-r--r--   0        0        0        7 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/docs/.gitignore
+-rw-r--r--   0        0        0      634 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/docs/Makefile
+-rw-r--r--   0        0        0     1997 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/docs/conf.py
+-rw-r--r--   0        0        0     3180 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/docs/getting_started/installation.md
+-rw-r--r--   0        0        0      305 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/docs/index.md
+-rw-r--r--   0        0        0       96 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/docs/requirements.txt
+-rw-r--r--   0        0        0      150 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/docs/usage/app_cli.md
+-rw-r--r--   0        0        0      117 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/docs/usage/snakemake_cli.md
+-rw-r--r--   0        0        0     1221 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/setup.py
+-rw-r--r--   0        0        0     3365 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/{{cookiecutter.__app_name}}/config/snakebids.yml
+-rw-r--r--   0        0        0      913 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/{{cookiecutter.__app_name}}/pipeline_description.json
+-rwxr-xr-x   0        0        0      532 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/{{cookiecutter.__app_name}}/run.py
+-rw-r--r--   0        0        0     1635 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/{{cookiecutter.__app_name}}/workflow/Snakefile
+-rw-r--r--   0        0        0        0 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/py.typed
+-rw-r--r--   0        0        0       13 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/resources/__init__.py
+-rw-r--r--   0        0        0     4339 2023-09-15 15:17:01.895784 snakebids-0.9.3/snakebids/resources/bids_tags.json
+-rw-r--r--   0        0        0     4828 2023-09-15 15:17:01.899785 snakebids-0.9.3/snakebids/types.py
+-rw-r--r--   0        0        0       70 2023-09-15 15:17:01.899785 snakebids-0.9.3/snakebids/utils/__init__.py
+-rw-r--r--   0        0        0     5839 2023-09-15 15:17:01.899785 snakebids-0.9.3/snakebids/utils/output.py
+-rw-r--r--   0        0        0      990 2023-09-15 15:17:01.899785 snakebids-0.9.3/snakebids/utils/sb_itertools.py
+-rw-r--r--   0        0        0     4947 2023-09-15 15:17:01.899785 snakebids-0.9.3/snakebids/utils/snakemake_io.py
+-rw-r--r--   0        0        0       91 2023-09-15 15:17:01.899785 snakebids-0.9.3/snakebids/utils/user_property.py
+-rw-r--r--   0        0        0      242 2023-09-15 15:17:01.899785 snakebids-0.9.3/snakebids/utils/user_property.pyi
+-rw-r--r--   0        0        0    16298 2023-09-15 15:17:01.899785 snakebids-0.9.3/snakebids/utils/utils.py
+-rw-r--r--   0        0        0     6511 1970-01-01 00:00:00.000000 snakebids-0.9.3/PKG-INFO
```

### Comparing `snakebids-0.9.2/LICENSE` & `snakebids-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/README.md` & `snakebids-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/pyproject.toml` & `snakebids-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakebids"
-version = "0.9.2"
+version = "0.9.3"
 description = "BIDS integration into snakemake workflows"
 readme = "README.md"
 repository = "https://github.com/akhanf/snakebids"
 documentation = "https://snakebids.readthedocs.io/"
 authors = [
     "Ali Khan <alik@robarts.ca>",
     "Peter Van Dyken <pvandyk2@uwo.ca>",
```

### Comparing `snakebids-0.9.2/snakebids/__init__.py` & `snakebids-0.9.3/snakebids/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __submodules__ = ["core"]
 
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 # <AUTOGEN_INIT>
 from snakebids.core import (
     BidsComponent,
     BidsComponentRow,
     BidsDataset,
     BidsDatasetDict,
```

### Comparing `snakebids-0.9.2/snakebids/admin.py` & `snakebids-0.9.3/snakebids/admin.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/app.py` & `snakebids-0.9.3/snakebids/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     create_parser,
     parse_snakebids_args,
 )
 from snakebids.exceptions import ConfigError, RunError
 from snakebids.types import OptionalFilter
 from snakebids.utils.output import write_config_file  # type: ignore
 from snakebids.utils.output import prepare_bidsapp_output, write_output_mode
-from snakebids.utils.utils import to_resolved_path
+from snakebids.utils.utils import DEPRECATION_FLAG, to_resolved_path
 
 logger = logging.Logger(__name__)
 
 
 SNAKEFILE_CHOICES = [
     "Snakefile",
     "snakefile",
@@ -180,14 +180,20 @@
 
         self.config["snakemake_dir"] = self.snakemake_dir
         self.config["snakefile"] = self.snakefile_path
 
         # Update config with pybids settings
         self.config["pybidsdb_dir"] = self.args.pybidsdb_dir
         self.config["pybidsdb_reset"] = self.args.pybidsdb_reset
+        self.config[
+            "pybids_db_dir"
+        ] = f"{DEPRECATION_FLAG}{self.args.pybidsdb_dir}{DEPRECATION_FLAG}"
+        self.config[
+            "pybids_db_reset"
+        ] = f"{DEPRECATION_FLAG}{int(self.args.pybidsdb_reset)}{DEPRECATION_FLAG}"
 
         # First, handle outputs in snakebids_root or results folder
         try:
             # py3.9 has the Path.is_relative() function. But as long as we support py38
             # and lower, this is the easiest way
             self.args.outputdir.resolve().relative_to(self.snakemake_dir / "results")
             relative_to_results = True
```

### Comparing `snakebids-0.9.2/snakebids/cli.py` & `snakebids-0.9.3/snakebids/cli.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/core/__init__.py` & `snakebids-0.9.3/snakebids/core/__init__.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/core/construct_bids.py` & `snakebids-0.9.3/snakebids/core/construct_bids.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/core/datasets.py` & `snakebids-0.9.3/snakebids/core/datasets.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/core/filtering.py` & `snakebids-0.9.3/snakebids/core/filtering.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/core/input_generation.py` & `snakebids-0.9.3/snakebids/core/input_generation.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 import json
 import logging
 import os
 import re
 import sys
+import warnings
 from collections import defaultdict
 from pathlib import Path
 from typing import Any, Generator, Iterable, Mapping, Optional, Sequence, overload
 
 import attrs
 import more_itertools as itx
 from bids import BIDSLayout, BIDSLayoutIndexer
@@ -23,15 +24,20 @@
     ConfigError,
     DuplicateComponentError,
     PybidsError,
     RunError,
 )
 from snakebids.types import InputsConfig, ZipList
 from snakebids.utils.snakemake_io import glob_wildcards
-from snakebids.utils.utils import BidsEntity, BidsParseError, get_first_dir
+from snakebids.utils.utils import (
+    DEPRECATION_FLAG,
+    BidsEntity,
+    BidsParseError,
+    get_first_dir,
+)
 
 _logger = logging.getLogger(__name__)
 
 
 @overload
 def generate_inputs(
     bids_dir: Path | str,
@@ -70,24 +76,24 @@
     ...
 
 
 def generate_inputs(
     bids_dir: Path | str,
     pybids_inputs: InputsConfig,
     pybidsdb_dir: Path | str | None = None,
-    pybidsdb_reset: bool = False,
+    pybidsdb_reset: bool | None = None,
     derivatives: bool | Path | str = False,
     pybids_config: str | None = None,
     limit_to: Iterable[str] | None = None,
     participant_label: Iterable[str] | str | None = None,
     exclude_participant_label: Iterable[str] | str | None = None,
     use_bids_inputs: bool | None = None,
     validate: bool = False,
     pybids_database_dir: Path | str | None = None,
-    pybids_reset_database: bool = False,
+    pybids_reset_database: bool | None = None,
 ) -> BidsDataset | BidsDatasetDict:
     """Dynamically generate snakemake inputs using pybids_inputs
 
     Pybids is used to parse the bids_dir. Custom paths can also be parsed by including
     the custom_paths entry under the pybids_inputs descriptor.
 
     Parameters
@@ -148,15 +154,15 @@
 
     use_bids_inputs
         If False, returns the classic :class:`BidsDatasetDict` instead of
         :class`BidsDataset`. Setting to True is deprecated as of v0.8, as this is now
         the default behaviour
 
     validate
-        If True performs validation of BIDS directory using pybids, otherwise 
+        If True performs validation of BIDS directory using pybids, otherwise
         skips validation.
 
     Returns
     -------
     BidsDataset | BidsDatasetDict
         Object containing organized information about the bids inputs for consumption in
         snakemake. See the documentation of :class:`BidsDataset` for details and
@@ -251,35 +257,26 @@
         })
     """
 
     subject_filter, regex_search = _generate_filters(
         participant_label, exclude_participant_label
     )
 
-    if pybids_database_dir:
-        _logger.warning(
-            "The parameter `pybids_database_dir` in generate_inputs() is deprecated "
-            "and will be removed in the next release. To set the pybids database, use "
-            "the `pybidsdb_dir` parameter instead."
-        )
-    if pybids_reset_database:
-        _logger.warning(
-            "The parameter `pybids_reset_database` in generate_inputs() is deprecated "
-            "and will be removed in the next release. To reset the pybids database, "
-            "use the `pybidsdb_reset` parameter instead."
-        )
+    pybidsdb_dir, pybidsdb_reset = _normalize_database_args(
+        pybidsdb_dir, pybidsdb_reset, pybids_database_dir, pybids_reset_database
+    )
 
     # Generates a BIDSLayout
     layout = (
         _gen_bids_layout(
             bids_dir=bids_dir,
             derivatives=derivatives,
             pybids_config=pybids_config,
-            pybidsdb_dir=pybidsdb_dir or pybids_database_dir,
-            pybidsdb_reset=pybidsdb_reset or pybids_reset_database,
+            pybidsdb_dir=pybidsdb_dir,
+            pybidsdb_reset=pybidsdb_reset,
             validate=validate,
         )
         if not _all_custom_paths(pybids_inputs)
         else None
     )
 
     filters = {"subject": subject_filter} if subject_filter else {}
@@ -308,14 +305,76 @@
         ) from err
 
     if use_bids_inputs:
         return dataset
     return dataset.as_dict
 
 
+def _normalize_database_args(
+    pybidsdb_dir: Path | str | None,
+    pybidsdb_reset: bool | str | None,
+    pybids_database_dir: Path | str | None,
+    pybids_reset_database: str | bool | None,
+) -> tuple[Path | str | None, bool]:
+    """This function exists to help handle deprecation for pybidsdb"""
+    if pybids_database_dir is not None:
+        warnings.warn(
+            "The parameter `pybids_database_dir` in generate_inputs() is deprecated "
+            "and will be removed in the next release. To set the pybids database, use "
+            "the `pybidsdb_dir` parameter instead."
+        )
+    if pybids_reset_database is not None:
+        warnings.warn(
+            "The parameter `pybids_reset_database` in generate_inputs() is deprecated "
+            "and will be removed in the next release. To reset the pybids database, "
+            "use the `pybidsdb_reset` parameter instead."
+        )
+
+    pybidsdb_dir = pybidsdb_dir or pybids_database_dir
+    pybidsdb_reset = (
+        pybidsdb_reset
+        if pybidsdb_reset is not None
+        else pybids_reset_database
+        if pybids_reset_database is not None
+        else False
+    )
+
+    depr_len = len(DEPRECATION_FLAG)
+    if (
+        pybidsdb_dir is not None
+        and str(pybidsdb_dir).startswith(DEPRECATION_FLAG)
+        and str(pybidsdb_dir).endswith(DEPRECATION_FLAG)
+    ):
+        warnings.warn(
+            "The config value `pybids_db_dir` is deprecated and will be removed in a "
+            "future release. To access a CLI-specified pybids database directory, use "
+            '`config.get("pybidsdb_dir")` instead.'
+        )
+        pybidsdb_dir = str(pybidsdb_dir)[depr_len:-depr_len]
+    try:
+        if (
+            isinstance(pybidsdb_reset, str)
+            and pybidsdb_reset.startswith(DEPRECATION_FLAG)
+            and pybidsdb_reset.endswith(DEPRECATION_FLAG)
+        ):
+            pybidsdb_reset = bool(int(pybidsdb_reset[depr_len:-depr_len]))
+            warnings.warn(
+                "The config value `pybids_db_reset` is deprecated and will be removed "
+                "in a future release. To access CLI-specified pybids database reset "
+                'instructions, use `config.get("pybidsdb_reset")` instead.'
+            )
+    except ValueError:
+        raise TypeError("pybidsdb_reset must be a boolean")
+
+    if not isinstance(pybidsdb_reset, bool):
+        raise TypeError("pybidsdb_reset must be a boolean")
+
+    return pybidsdb_dir, pybidsdb_reset
+
+
 def _all_custom_paths(config: InputsConfig):
     """Check that all input components have a custom path"""
     return all(comp.get("custom_path") for comp in config.values())
 
 
 def _gen_bids_layout(
     *,
```

### Comparing `snakebids-0.9.2/snakebids/exceptions.py` & `snakebids-0.9.3/snakebids/exceptions.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/io/console.py` & `snakebids-0.9.3/snakebids/io/console.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/io/printing.py` & `snakebids-0.9.3/snakebids/io/printing.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/plugins/validator.py` & `snakebids-0.9.3/snakebids/plugins/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         validator_config_dict = {"ignoredFiles": ["/participants.tsv"]}
 
         with tempfile.NamedTemporaryFile(mode="w+", suffix=".json") as temp:
             temp.write(json.dumps(validator_config_dict))
             temp.flush()
             try:
                 subprocess.check_call(
-                    ["bids-validator", app.config["bids_dirs"], "-c", temp.name]
+                    ["bids-validator", app.config["bids_dir"], "-c", temp.name]
                 )
 
                 # If successfully bids-validation performed
                 app.config["plugins.validator.success"] = True
             except FileNotFoundError:
                 # If the bids-validator call can't be made
                 app.config["plugins.validator.success"] = False
```

### Comparing `snakebids-0.9.2/snakebids/project_template/hooks/post_gen_project.py` & `snakebids-0.9.3/snakebids/project_template/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/docs/Makefile` & `snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/docs/Makefile`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/docs/conf.py` & `snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/docs/getting_started/installation.md` & `snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/docs/getting_started/installation.md`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/setup.py` & `snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/setup.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/{{cookiecutter.__app_name}}/config/snakebids.yml` & `snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/{{cookiecutter.__app_name}}/config/snakebids.yml`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/{{cookiecutter.__app_name}}/pipeline_description.json` & `snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/{{cookiecutter.__app_name}}/pipeline_description.json`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/{{cookiecutter.__app_name}}/run.py` & `snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/{{cookiecutter.__app_name}}/run.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/project_template/{{cookiecutter.__app_name}}/{{cookiecutter.__app_name}}/workflow/Snakefile` & `snakebids-0.9.3/snakebids/project_template/{{cookiecutter.__app_name}}/{{cookiecutter.__app_name}}/workflow/Snakefile`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/resources/bids_tags.json` & `snakebids-0.9.3/snakebids/resources/bids_tags.json`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/types.py` & `snakebids-0.9.3/snakebids/types.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/utils/output.py` & `snakebids-0.9.3/snakebids/utils/output.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/utils/sb_itertools.py` & `snakebids-0.9.3/snakebids/utils/sb_itertools.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/utils/snakemake_io.py` & `snakebids-0.9.3/snakebids/utils/snakemake_io.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.9.2/snakebids/utils/utils.py` & `snakebids-0.9.3/snakebids/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,18 @@
     after: NotRequired[str]
     leader: NotRequired[bool]
 
 
 BidsTags: TypeAlias = "dict[str, BidsTag]"
 
 
+DEPRECATION_FLAG = "<!DEPRECATED!>"
+"""Sentinel string to mark deprecated config features"""
+
+
 @ft.lru_cache(None)
 def read_bids_tags(bids_json: Path | None = None) -> BidsTags:
     """Read the bids tags we are aware of from a JSON file.
 
     This is used specifically for compatibility with pybids, since some tag keys
     are different from how they appear in the file name, e.g. ``subject`` for
     ``sub``, and ``acquisition`` for ``acq``.
```

### Comparing `snakebids-0.9.2/PKG-INFO` & `snakebids-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakebids
-Version: 0.9.2
+Version: 0.9.3
 Summary: BIDS integration into snakemake workflows
 Home-page: https://github.com/akhanf/snakebids
 License: MIT
 Author: Ali Khan
 Author-email: alik@robarts.ca
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

