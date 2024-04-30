# Comparing `tmp/mailme-api-0.2.0.tar.gz` & `tmp/mailme-api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mailme-api-0.2.0.tar", last modified: Sat Apr 20 16:45:12 2024, max compression
+gzip compressed data, was "dist/mailme-api-0.2.1.tar", last modified: Tue Apr 30 14:56:29 2024, max compression
```

## Comparing `mailme-api-0.2.0.tar` & `mailme-api-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 16:45:12.000000 mailme-api-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     2655 2024-04-20 16:45:07.000000 mailme-api-0.2.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     1214 2024-04-20 16:45:07.000000 mailme-api-0.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-20 16:45:12.000000 mailme-api-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2735 2024-04-20 16:45:12.000000 mailme-api-0.2.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 16:45:12.000000 mailme-api-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 16:45:12.000000 mailme-api-0.2.0/src/mailme_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 16:45:12.000000 mailme-api-0.2.0/src/mailme_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      356 2024-04-20 16:45:12.000000 mailme-api-0.2.0/src/mailme_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-20 16:45:12.000000 mailme-api-0.2.0/src/mailme_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2735 2024-04-20 16:45:12.000000 mailme-api-0.2.0/src/mailme_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-20 16:45:12.000000 mailme-api-0.2.0/src/mailme_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 16:45:09.000000 mailme-api-0.2.0/src/mailme_api.egg-info/not-zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 16:45:12.000000 mailme-api-0.2.0/src/mailme/
--rw-r--r--   0 root         (0) root         (0)     2467 2024-04-20 16:45:07.000000 mailme-api-0.2.0/src/mailme/base.py
--rw-r--r--   0 root         (0) root         (0)     1073 2024-04-20 16:45:07.000000 mailme-api-0.2.0/src/mailme/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 16:45:12.000000 mailme-api-0.2.0/src/mailme/scripts/
--rw-r--r--   0 root         (0) root         (0)     1836 2024-04-20 16:45:07.000000 mailme-api-0.2.0/src/mailme/scripts/sender.py
--rw-r--r--   0 root         (0) root         (0)     1012 2024-04-20 16:45:07.000000 mailme-api-0.2.0/src/mailme/scripts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:56:29.000000 mailme-api-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)     2696 2024-04-30 14:56:23.000000 mailme-api-0.2.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2024-04-30 14:56:23.000000 mailme-api-0.2.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-30 14:56:29.000000 mailme-api-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3116 2024-04-30 14:56:29.000000 mailme-api-0.2.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:56:29.000000 mailme-api-0.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:56:29.000000 mailme-api-0.2.1/src/mailme_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 14:56:28.000000 mailme-api-0.2.1/src/mailme_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      376 2024-04-30 14:56:28.000000 mailme-api-0.2.1/src/mailme_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-30 14:56:28.000000 mailme-api-0.2.1/src/mailme_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3116 2024-04-30 14:56:28.000000 mailme-api-0.2.1/src/mailme_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-30 14:56:28.000000 mailme-api-0.2.1/src/mailme_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 14:56:25.000000 mailme-api-0.2.1/src/mailme_api.egg-info/not-zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:56:29.000000 mailme-api-0.2.1/src/mailme/
+-rw-r--r--   0 root         (0) root         (0)     2467 2024-04-30 14:56:23.000000 mailme-api-0.2.1/src/mailme/base.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-04-30 14:56:23.000000 mailme-api-0.2.1/src/mailme/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:56:29.000000 mailme-api-0.2.1/src/mailme/scripts/
+-rw-r--r--   0 root         (0) root         (0)     1836 2024-04-30 14:56:23.000000 mailme-api-0.2.1/src/mailme/scripts/sender.py
+-rw-r--r--   0 root         (0) root         (0)     1012 2024-04-30 14:56:23.000000 mailme-api-0.2.1/src/mailme/scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2024-04-30 14:56:23.000000 mailme-api-0.2.1/src/mailme/base.pyi
```

### Comparing `mailme-api-0.2.0/setup.py` & `mailme-api-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Mailme API
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Mailme API.
 #
 # Hive Mailme API is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,35 +18,36 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Mailme API. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
 import setuptools
 
 setuptools.setup(
     name="mailme-api",
-    version="0.2.0",
+    version="0.2.1",
     author="Hive Solutions Lda.",
     author_email="development@hive.pt",
     description="Mailme API Client",
     license="Apache License, Version 2.0",
     keywords="mailme api",
     url="http://mailme-api.hive.pt",
     zip_safe=False,
     packages=["mailme", "mailme.scripts"],
     package_dir={"": os.path.normpath("src")},
+    package_data={"mailme": ["*.pyi"]},
     install_requires=["appier"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Topic :: Utilities",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
```

### Comparing `mailme-api-0.2.0/PKG-INFO` & `mailme-api-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mailme-api
-Version: 0.2.0
+Version: 0.2.1
 Summary: Mailme API Client
 Home-page: http://mailme-api.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Mailme API](http://mailme-api.hive.pt)
         
         API Python client for the Mailme service.
         
         ## Configuration
         
-        | Name | Type | Description |
-        | ----- | ----- | ----- |
-        | **MAILME_BASE_URL** | `str` | The base URL for the Mailme API requests (defaults to `https://mailme.bemisc.com/api/`). |
-        | **MAILME_KEY** | `str` |  The secret key to be used to authenticate API requests (defaults to `None`). |
+        | Name                | Type  | Default                          | Description                                             |
+        | ------------------- | ----- | -------------------------------- | ------------------------------------------------------- |
+        | **MAILME_BASE_URL** | `str` | `https://mailme.bemisc.com/api/` | The base URL for the Mailme API requests.               |
+        | **MAILME_KEY**      | `str` | `None`                           | The secret key to be used to authenticate API requests. |
         
         ## Installation
         
         ```bash
         pip install mailme-api
         ```
         
@@ -34,14 +34,15 @@
         ## License
         
         Mailme API is currently licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/).
         
         ## Build Automation
         
         [![Build Status](https://app.travis-ci.com/hivesolutions/mailme-api.svg?branch=master)](https://travis-ci.com/github/hivesolutions/mailme-api)
+        [![Build Status GitHub](https://github.com/hivesolutions/mailme-api/workflows/Main%20Workflow/badge.svg)](https://github.com/hivesolutions/mailme-api/actions)
         [![Coverage Status](https://coveralls.io/repos/hivesolutions/mailme-api/badge.svg?branch=master)](https://coveralls.io/r/hivesolutions/mailme-api?branch=master)
         [![PyPi Status](https://img.shields.io/pypi/v/mailme-api.svg)](https://pypi.python.org/pypi/mailme-api)
         [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://www.apache.org/licenses/)
         
 Keywords: mailme api
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mailme-api-0.2.0/src/mailme_api.egg-info/PKG-INFO` & `mailme-api-0.2.1/src/mailme_api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mailme-api
-Version: 0.2.0
+Version: 0.2.1
 Summary: Mailme API Client
 Home-page: http://mailme-api.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Mailme API](http://mailme-api.hive.pt)
         
         API Python client for the Mailme service.
         
         ## Configuration
         
-        | Name | Type | Description |
-        | ----- | ----- | ----- |
-        | **MAILME_BASE_URL** | `str` | The base URL for the Mailme API requests (defaults to `https://mailme.bemisc.com/api/`). |
-        | **MAILME_KEY** | `str` |  The secret key to be used to authenticate API requests (defaults to `None`). |
+        | Name                | Type  | Default                          | Description                                             |
+        | ------------------- | ----- | -------------------------------- | ------------------------------------------------------- |
+        | **MAILME_BASE_URL** | `str` | `https://mailme.bemisc.com/api/` | The base URL for the Mailme API requests.               |
+        | **MAILME_KEY**      | `str` | `None`                           | The secret key to be used to authenticate API requests. |
         
         ## Installation
         
         ```bash
         pip install mailme-api
         ```
         
@@ -34,14 +34,15 @@
         ## License
         
         Mailme API is currently licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/).
         
         ## Build Automation
         
         [![Build Status](https://app.travis-ci.com/hivesolutions/mailme-api.svg?branch=master)](https://travis-ci.com/github/hivesolutions/mailme-api)
+        [![Build Status GitHub](https://github.com/hivesolutions/mailme-api/workflows/Main%20Workflow/badge.svg)](https://github.com/hivesolutions/mailme-api/actions)
         [![Coverage Status](https://coveralls.io/repos/hivesolutions/mailme-api/badge.svg?branch=master)](https://coveralls.io/r/hivesolutions/mailme-api?branch=master)
         [![PyPi Status](https://img.shields.io/pypi/v/mailme-api.svg)](https://pypi.python.org/pypi/mailme-api)
         [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://www.apache.org/licenses/)
         
 Keywords: mailme api
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mailme-api-0.2.0/src/mailme/base.py` & `mailme-api-0.2.1/src/mailme/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Mailme API
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Mailme API.
 #
 # Hive Mailme API is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,15 +18,15 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Mailme API. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import appier
```

### Comparing `mailme-api-0.2.0/src/mailme/__init__.py` & `mailme-api-0.2.1/src/mailme/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Mailme API
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Mailme API.
 #
 # Hive Mailme API is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -15,15 +15,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # Apache License for more details.
 #
 # You should have received a copy of the Apache License along with
 # Hive Mailme API. If not, see <http://www.apache.org/licenses/>.
 
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import base
```

### Comparing `mailme-api-0.2.0/src/mailme/scripts/sender.py` & `mailme-api-0.2.1/src/mailme/scripts/sender.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Mailme API
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Mailme API.
 #
 # Hive Mailme API is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,15 +18,15 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Mailme API. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import pprint
```

### Comparing `mailme-api-0.2.0/src/mailme/scripts/__init__.py` & `mailme-api-0.2.1/src/mailme/scripts/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Mailme API
-# Copyright (c) 2008-2020 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Mailme API.
 #
 # Hive Mailme API is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -15,15 +15,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # Apache License for more details.
 #
 # You should have received a copy of the Apache License along with
 # Hive Mailme API. If not, see <http://www.apache.org/licenses/>.
 
-__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import sender
```

