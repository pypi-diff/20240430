# Comparing `tmp/mysqlx-connector-python-8.3.0.tar.gz` & `tmp/mysqlx-connector-python-8.4.0.tar.gz`

## Comparing `mysqlx-connector-python-8.3.0.tar` & `mysqlx-connector-python-8.4.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 pb2user   (7161) common   (31415)        0 2023-12-18 21:14:21.000000 mysqlx-connector-python-8.3.0/
-drwxr-xr-x   0 pb2user   (7161) common   (31415)        0 2023-12-18 21:14:21.000000 mysqlx-connector-python-8.3.0/mysqlx/
--rw-r--r--   0 pb2user   (7161) common   (31415)     3570 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/__init__.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     5655 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/authentication.py
--rw-r--r--   0 pb2user   (7161) common   (31415)    27612 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/charsets.py
--rw-r--r--   0 pb2user   (7161) common   (31415)   122137 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/connection.py
--rw-r--r--   0 pb2user   (7161) common   (31415)    15220 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/constants.py
--rw-r--r--   0 pb2user   (7161) common   (31415)    26500 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/crud.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     4070 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/dbdoc.py
--rw-r--r--   0 pb2user   (7161) common   (31415)    69343 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/errorcode.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     8875 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/errors.py
--rw-r--r--   0 pb2user   (7161) common   (31415)    49911 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/expr.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     7803 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/helpers.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     1490 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/logger.py
--rw-r--r--   0 pb2user   (7161) common   (31415)    42492 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/protocol.py
--rw-r--r--   0 pb2user   (7161) common   (31415)    33193 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/result.py
--rw-r--r--   0 pb2user   (7161) common   (31415)    50019 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/statement.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     2575 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/types.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     4663 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/utils.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     1945 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/version.py
-drwxr-xr-x   0 pb2user   (7161) common   (31415)        0 2023-12-18 21:14:21.000000 mysqlx-connector-python-8.3.0/mysqlx/locales/
--rw-r--r--   0 pb2user   (7161) common   (31415)     2819 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/locales/__init__.py
-drwxr-xr-x   0 pb2user   (7161) common   (31415)        0 2023-12-18 21:14:21.000000 mysqlx-connector-python-8.3.0/mysqlx/locales/eng/
--rw-r--r--   0 pb2user   (7161) common   (31415)     1444 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/locales/eng/__init__.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     7475 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/locales/eng/client_error.py
-drwxr-xr-x   0 pb2user   (7161) common   (31415)        0 2023-12-18 21:14:21.000000 mysqlx-connector-python-8.3.0/mysqlx/protobuf/
--rw-r--r--   0 pb2user   (7161) common   (31415)    21354 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/protobuf/__init__.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     3690 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_connection_pb2.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     9745 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_crud_pb2.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     3391 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_cursor_pb2.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     4591 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_datatypes_pb2.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     3651 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_expect_pb2.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     5364 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_expr_pb2.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     5267 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_notice_pb2.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     4761 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_pb2.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     3991 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_prepare_pb2.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     4454 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_resultset_pb2.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     3131 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_session_pb2.py
--rw-r--r--   0 pb2user   (7161) common   (31415)     2852 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_sql_pb2.py
--rw-r--r--   0 pb2user   (7161) common   (31415)        0 2023-12-18 21:13:02.000000 mysqlx-connector-python-8.3.0/mysqlx/py.typed
-drwxr-xr-x   0 pb2user   (7161) common   (31415)        0 2023-12-18 21:14:21.000000 mysqlx-connector-python-8.3.0/mysqlx_connector_python-8.3.0-py3.8.egg-info/
--rw-r--r--   0 pb2user   (7161) common   (31415)     1592 2023-12-18 21:14:21.000000 mysqlx-connector-python-8.3.0/mysqlx_connector_python-8.3.0-py3.8.egg-info/PKG-INFO
--rw-r--r--   0 pb2user   (7161) common   (31415)        1 2023-12-18 21:14:21.000000 mysqlx-connector-python-8.3.0/mysqlx_connector_python-8.3.0-py3.8.egg-info/dependency_links.txt
--rw-r--r--   0 pb2user   (7161) common   (31415)      125 2023-12-18 21:14:21.000000 mysqlx-connector-python-8.3.0/mysqlx_connector_python-8.3.0-py3.8.egg-info/requires.txt
--rw-r--r--   0 pb2user   (7161) common   (31415)        7 2023-12-18 21:14:21.000000 mysqlx-connector-python-8.3.0/mysqlx_connector_python-8.3.0-py3.8.egg-info/top_level.txt
--rw-r--r--   0 pb2user   (7161) common   (31415)     3577 2023-12-18 21:14:21.000000 mysqlx-connector-python-8.3.0/mysqlx_connector_python-8.3.0-py3.8.egg-info/SOURCES.txt
--rw-r--r--   0 pb2user   (7161) common   (31415)      643 2023-12-18 21:14:21.000000 mysqlx-connector-python-8.3.0/README.txt
--rw-r--r--   0 pb2user   (7161) common   (31415)   199941 2023-12-18 21:14:21.000000 mysqlx-connector-python-8.3.0/LICENSE.txt
--rw-r--r--   0 pb2user   (7161) common   (31415)     4041 2023-12-18 21:14:21.000000 mysqlx-connector-python-8.3.0/README.rst
--rw-r--r--   0 pb2user   (7161) common   (31415)    20409 2023-12-18 21:14:21.000000 mysqlx-connector-python-8.3.0/CONTRIBUTING.rst
--rw-r--r--   0 pb2user   (7161) common   (31415)      101 2023-12-18 21:14:21.000000 mysqlx-connector-python-8.3.0/INFO_SRC
--rw-r--r--   0 pb2user   (7161) common   (31415)       93 2023-12-18 21:14:21.000000 mysqlx-connector-python-8.3.0/INFO_BIN
-drwxr-xr-x   0 pb2user   (7161) common   (31415)        0 2023-12-18 21:14:21.000000 mysqlx-connector-python-8.3.0/docs/
+drwxr-xr-x   0 pb2user   (7161) common   (31415)        0 2024-03-15 06:21:01.000000 mysqlx-connector-python-8.4.0/
+drwxr-xr-x   0 pb2user   (7161) common   (31415)        0 2024-03-15 06:21:01.000000 mysqlx-connector-python-8.4.0/mysqlx/
+-rw-r--r--   0 pb2user   (7161) common   (31415)    50066 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/statement.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     8922 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/errors.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)   122564 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/connection.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)    11892 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/constants.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     1971 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/version.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)        0 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/py.typed
+-rw-r--r--   0 pb2user   (7161) common   (31415)     9155 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/tls_ciphers.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     7859 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/helpers.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     1537 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/logger.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     4096 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/dbdoc.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)    33240 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/result.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)    42539 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/protocol.py
+drwxr-xr-x   0 pb2user   (7161) common   (31415)        0 2024-03-15 06:21:01.000000 mysqlx-connector-python-8.4.0/mysqlx/locales/
+drwxr-xr-x   0 pb2user   (7161) common   (31415)        0 2024-03-15 06:21:01.000000 mysqlx-connector-python-8.4.0/mysqlx/locales/eng/
+-rw-r--r--   0 pb2user   (7161) common   (31415)     7501 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/locales/eng/client_error.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     1470 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/locales/eng/__init__.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     2845 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/locales/__init__.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)    27638 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/charsets.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)    69369 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/errorcode.py
+drwxr-xr-x   0 pb2user   (7161) common   (31415)        0 2024-03-15 06:21:01.000000 mysqlx-connector-python-8.4.0/mysqlx/protobuf/
+-rw-r--r--   0 pb2user   (7161) common   (31415)     4638 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_datatypes_pb2.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     4808 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_pb2.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     4501 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_resultset_pb2.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     3438 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_cursor_pb2.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     5411 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_expr_pb2.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     4038 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_prepare_pb2.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     3178 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_session_pb2.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     9792 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_crud_pb2.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     3737 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_connection_pb2.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     2899 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_sql_pb2.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     5314 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_notice_pb2.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     3698 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_expect_pb2.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)    21401 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/protobuf/__init__.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)    26547 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/crud.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     6243 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/utils.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     5702 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/authentication.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)    49939 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/expr.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     3617 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/__init__.py
+-rw-r--r--   0 pb2user   (7161) common   (31415)     4022 2024-03-15 06:11:29.000000 mysqlx-connector-python-8.4.0/mysqlx/types.py
+drwxr-xr-x   0 pb2user   (7161) common   (31415)        0 2024-03-15 06:21:01.000000 mysqlx-connector-python-8.4.0/docs/
+drwxr-xr-x   0 pb2user   (7161) common   (31415)        0 2024-03-15 06:21:01.000000 mysqlx-connector-python-8.4.0/mysqlx_connector_python-8.4.0-py3.8.egg-info/
+-rw-r--r--   0 pb2user   (7161) common   (31415)      125 2024-03-15 06:21:01.000000 mysqlx-connector-python-8.4.0/mysqlx_connector_python-8.4.0-py3.8.egg-info/requires.txt
+-rw-r--r--   0 pb2user   (7161) common   (31415)        7 2024-03-15 06:21:01.000000 mysqlx-connector-python-8.4.0/mysqlx_connector_python-8.4.0-py3.8.egg-info/top_level.txt
+-rw-r--r--   0 pb2user   (7161) common   (31415)        1 2024-03-15 06:21:01.000000 mysqlx-connector-python-8.4.0/mysqlx_connector_python-8.4.0-py3.8.egg-info/dependency_links.txt
+-rw-r--r--   0 pb2user   (7161) common   (31415)     1592 2024-03-15 06:21:01.000000 mysqlx-connector-python-8.4.0/mysqlx_connector_python-8.4.0-py3.8.egg-info/PKG-INFO
+-rw-r--r--   0 pb2user   (7161) common   (31415)     3631 2024-03-15 06:21:01.000000 mysqlx-connector-python-8.4.0/mysqlx_connector_python-8.4.0-py3.8.egg-info/SOURCES.txt
+-rw-r--r--   0 pb2user   (7161) common   (31415)   201537 2024-03-15 06:21:01.000000 mysqlx-connector-python-8.4.0/LICENSE.txt
+-rw-r--r--   0 pb2user   (7161) common   (31415)    20409 2024-03-15 06:21:01.000000 mysqlx-connector-python-8.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 pb2user   (7161) common   (31415)      101 2024-03-15 06:21:01.000000 mysqlx-connector-python-8.4.0/INFO_SRC
+-rw-r--r--   0 pb2user   (7161) common   (31415)      867 2024-03-15 06:21:01.000000 mysqlx-connector-python-8.4.0/README.txt
+-rw-r--r--   0 pb2user   (7161) common   (31415)     4179 2024-03-15 06:21:01.000000 mysqlx-connector-python-8.4.0/README.rst
+-rw-r--r--   0 pb2user   (7161) common   (31415)       89 2024-03-15 06:21:01.000000 mysqlx-connector-python-8.4.0/INFO_BIN
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/__init__.py` & `mysqlx-connector-python-8.4.0/mysqlx/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2016, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2016, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/authentication.py` & `mysqlx-connector-python-8.4.0/mysqlx/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2016, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2016, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/charsets.py` & `mysqlx-connector-python-8.4.0/mysqlx/charsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2013, 2023, Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2013, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/connection.py` & `mysqlx-connector-python-8.4.0/mysqlx/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2016, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2016, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
@@ -35,16 +35,14 @@
 from types import TracebackType
 
 try:
     import ssl
 
     SSL_AVAILABLE = True
     TLS_VERSIONS = {
-        "TLSv1": ssl.PROTOCOL_TLSv1,
-        "TLSv1.1": ssl.PROTOCOL_TLSv1_1,
         "TLSv1.2": ssl.PROTOCOL_TLSv1_2,
     }
     # TLSv1.3 included in PROTOCOL_TLS, but PROTOCOL_TLS is not included on 3.4
     TLS_VERSIONS["TLSv1.3"] = (
         ssl.PROTOCOL_TLS
         if hasattr(ssl, "PROTOCOL_TLS")
         else ssl.PROTOCOL_SSLv23  # Alias of PROTOCOL_TLS
@@ -61,15 +59,14 @@
 import queue
 import random
 import re
 import socket
 import sys
 import threading
 import uuid
-import warnings
 
 from typing import Any, Callable, Dict, List, Mapping, Optional, Tuple, Type, Union
 
 try:
     import dns.exception
     import dns.resolver
 except ImportError:
@@ -81,15 +78,14 @@
 from functools import wraps
 from json.decoder import JSONDecodeError
 from urllib.parse import parse_qsl, unquote, urlparse
 
 from .authentication import MySQL41AuthPlugin, PlainAuthPlugin, Sha256MemoryAuthPlugin
 from .constants import (
     COMPRESSION_ALGORITHMS,
-    DEPRECATED_TLS_VERSIONS,
     OPENSSL_CS_NAMES,
     SUPPORTED_TLS_VERSIONS,
     TLS_CIPHER_SUITES,
     Auth,
     Compression,
     SSLMode,
 )
@@ -122,28 +118,33 @@
     UpdateStatement,
     quote_identifier,
 )
 from .types import ColumnType, MessageType, ResultBaseType, StatementType
 
 sys.path.append("..")
 
-from .utils import linux_distribution
+from .tls_ciphers import UNACCEPTABLE_TLS_CIPHERSUITES, UNACCEPTABLE_TLS_VERSIONS
+from .utils import (
+    linux_distribution,
+    warn_ciphersuites_deprecated,
+    warn_tls_version_deprecated,
+)
 from .version import LICENSE, VERSION
 
 DUPLICATED_IN_LIST_ERROR = (
     "The '{list}' list must not contain repeated values, the value "
     "'{value}' is duplicated."
 )
 
 TLS_VERSION_ERROR = (
     "The given tls_version: '{}' is not recognized as a valid "
     "TLS protocol version (should be one of {})."
 )
 
-TLS_VERSION_DEPRECATED_ERROR = (
+TLS_VERSION_UNACCEPTABLE_ERROR = (
     "The given tls_version: '{}' are no longer allowed (should be one of {})."
 )
 
 TLS_VER_NO_SUPPORTED = (
     "No supported TLS protocol version found in the 'tls-versions' list '{}'. "
 )
 
@@ -434,23 +435,19 @@
         try:
             self._socket = context.wrap_socket(self._socket, server_hostname=self._host)
         except ssl.CertificateError as err:
             raise InterfaceError(f"{err}") from err
 
         self._is_ssl = True
 
-        # Raise a deprecation warning if TLSv1 or TLSv1.1 is being used
-        tls_version = self._socket.version()
-        if tls_version in ("TLSv1", "TLSv1.1"):
-            warn_msg = (
-                f"This connection is using {tls_version} which is now "
-                "deprecated and will be removed in a future release of "
-                "MySQL Connector/Python"
-            )
-            warnings.warn(warn_msg, DeprecationWarning)
+        # Raise a deprecation warning if a deprecated TLS cipher or
+        # version is being used.
+        cipher, tls_version, _ = self._socket.cipher()
+        warn_tls_version_deprecated(tls_version)
+        warn_ciphersuites_deprecated(cipher, tls_version)
 
     def is_ssl(self) -> bool:
         """Verifies if SSL is being used.
 
         Returns:
             bool: Returns `True` if SSL is being used.
         """
@@ -1540,14 +1537,15 @@
     Raises:
         :class:`mysqlx.PoolError` on errors.
 
     .. versionadded:: 8.0.13
     """
 
     def __init__(self, name: str, **kwargs: Any) -> None:
+        self.name: Optional[str] = None
         self._set_pool_name(name)
         self._open_sessions: int = 0
         self._connections_openned: List[PooledConnection] = []
         self._available: bool = True
         self._timeout: int = 0
         self._timeout_stamp: datetime = datetime.now()
         self.pool_max_size: int = kwargs.get("max_size", 25)
@@ -3089,35 +3087,34 @@
     if not tls_versions:
         raise InterfaceError(
             "At least one TLS protocol version must be specified in "
             "'tls-versions' list."
         )
 
     use_tls_versions = []
-    deprecated_tls_versions = []
+    unacceptable_tls_versions = []
     not_tls_versions = []
     for tls_ver in tls_versions:
         if tls_ver in SUPPORTED_TLS_VERSIONS:
             use_tls_versions.append(tls_ver)
-        if tls_ver in DEPRECATED_TLS_VERSIONS:
-            deprecated_tls_versions.append(tls_ver)
+        if tls_ver in UNACCEPTABLE_TLS_VERSIONS:
+            unacceptable_tls_versions.append(tls_ver)
         else:
             not_tls_versions.append(tls_ver)
 
     if use_tls_versions:
         if use_tls_versions == ["TLSv1.3"] and not TLS_V1_3_SUPPORTED:
             raise NotSupportedError(
                 TLS_VER_NO_SUPPORTED.format(tls_versions, SUPPORTED_TLS_VERSIONS)
             )
-        use_tls_versions.sort()
         settings["tls-versions"] = use_tls_versions
-    elif deprecated_tls_versions:
+    elif unacceptable_tls_versions:
         raise NotSupportedError(
-            TLS_VERSION_DEPRECATED_ERROR.format(
-                deprecated_tls_versions, SUPPORTED_TLS_VERSIONS
+            TLS_VERSION_UNACCEPTABLE_ERROR.format(
+                unacceptable_tls_versions, SUPPORTED_TLS_VERSIONS
             )
         )
     elif not_tls_versions:
         raise InterfaceError(TLS_VERSION_ERROR.format(tls_ver, SUPPORTED_TLS_VERSIONS))
 
 
 def _validate_tls_ciphersuites(settings: Dict[str, Any]) -> None:
@@ -3202,14 +3199,27 @@
             )
 
     if not translated_names:
         raise InterfaceError(
             "No valid cipher suite found in the 'tls-ciphersuites' list"
         )
 
+    # raise an error when using an unacceptable cipher
+    for cipher_as_ossl in translated_names:
+        for tls_ver in SUPPORTED_TLS_VERSIONS[
+            : SUPPORTED_TLS_VERSIONS.index(newer_tls_ver) + 1
+        ]:
+            if (
+                cipher_as_ossl
+                in UNACCEPTABLE_TLS_CIPHERSUITES.get(tls_ver, {}).values()
+            ):
+                raise NotSupportedError(
+                    f"Cipher {cipher_as_ossl} when used with {tls_ver} is unacceptable."
+                )
+
     settings["tls-ciphersuites"] = translated_names
 
 
 def _get_connection_settings(*args: Any, **kwargs: Any) -> Dict[str, Any]:
     """Parses the connection string and returns a dictionary with the
     connection settings.
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/constants.py` & `mysqlx-connector-python-8.4.0/mysqlx/constants.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2016, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2016, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
@@ -26,14 +26,16 @@
 # along with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin St, Fifth Floor, Boston, MA 02110-1301  USA
 
 """Constants."""
 
 from enum import Enum
 
+from . import tls_ciphers
+
 
 class Auth(Enum):
     """Enum to identify the authentication mechanisms."""
 
     PLAIN = "plain"
     MYSQL41 = "mysql41"
     SHA256_MEMORY = "sha256_memory"
@@ -70,74 +72,19 @@
     "deflate_stream": "deflate_stream",
     "lz4": "lz4_message",
     "lz4_message": "lz4_message",
     "zstd": "zstd_stream",
     "zstd_stream": "zstd_stream",
 }
 
-TLS_VERSIONS = ["TLSv1", "TLSv1.1", "TLSv1.2", "TLSv1.3"]
-SUPPORTED_TLS_VERSIONS = ["TLSv1.2", "TLSv1.3"]
-DEPRECATED_TLS_VERSIONS = ["TLSv1", "TLSv1.1"]
-
-# TLS v1.0 cipher suites IANI to OpenSSL name translation
-TLSV1_CIPHER_SUITES = {
-    "TLS_RSA_WITH_NULL_MD5": "NULL-MD5",
-    "TLS_RSA_WITH_NULL_SHA": "NULL-SHA",
-    "TLS_RSA_WITH_RC4_128_MD5": "RC4-MD5",
-    "TLS_RSA_WITH_RC4_128_SHA": "RC4-SHA",
-    "TLS_RSA_WITH_IDEA_CBC_SHA": "IDEA-CBC-SHA",
-    "TLS_RSA_WITH_3DES_EDE_CBC_SHA": "DES-CBC3-SHA",
-    "TLS_DH_DSS_WITH_3DES_EDE_CBC_SHA": "Not implemented.",
-    "TLS_DH_RSA_WITH_3DES_EDE_CBC_SHA": "Not implemented.",
-    "TLS_DHE_DSS_WITH_3DES_EDE_CBC_SHA": "DHE-DSS-DES-CBC3-SHA",
-    "TLS_DHE_RSA_WITH_3DES_EDE_CBC_SHA": "DHE-RSA-DES-CBC3-SHA",
-    "TLS_DH_anon_WITH_RC4_128_MD5": "ADH-RC4-MD5",
-    "TLS_DH_anon_WITH_3DES_EDE_CBC_SHA": "ADH-DES-CBC3-SHA",
-    # AES cipher suites from RFC3268, extending TLS v1.0
-    "TLS_RSA_WITH_AES_128_CBC_SHA": "AES128-SHA",
-    "TLS_RSA_WITH_AES_256_CBC_SHA": "AES256-SHA",
-    "TLS_DH_DSS_WITH_AES_128_CBC_SHA": "DH-DSS-AES128-SHA",
-    "TLS_DH_DSS_WITH_AES_256_CBC_SHA": "DH-DSS-AES256-SHA",
-    "TLS_DH_RSA_WITH_AES_128_CBC_SHA": "DH-RSA-AES128-SHA",
-    "TLS_DH_RSA_WITH_AES_256_CBC_SHA": "DH-RSA-AES256-SHA",
-    "TLS_DHE_DSS_WITH_AES_128_CBC_SHA": "DHE-DSS-AES128-SHA",
-    "TLS_DHE_DSS_WITH_AES_256_CBC_SHA": "DHE-DSS-AES256-SHA",
-    "TLS_DHE_RSA_WITH_AES_128_CBC_SHA": "DHE-RSA-AES128-SHA",
-    "TLS_DHE_RSA_WITH_AES_256_CBC_SHA": "DHE-RSA-AES256-SHA",
-    "TLS_DH_anon_WITH_AES_128_CBC_SHA": "ADH-AES128-SHA",
-    "TLS_DH_anon_WITH_AES_256_CBC_SHA": "ADH-AES256-SHA",
-    # Camellia cipher suites from RFC4132, extending TLS v1.0
-    "TLS_RSA_WITH_CAMELLIA_128_CBC_SHA": "CAMELLIA128-SHA",
-    "TLS_RSA_WITH_CAMELLIA_256_CBC_SHA": "CAMELLIA256-SHA",
-    "TLS_DH_DSS_WITH_CAMELLIA_128_CBC_SHA": "DH-DSS-CAMELLIA128-SHA",
-    "TLS_DH_DSS_WITH_CAMELLIA_256_CBC_SHA": "DH-DSS-CAMELLIA256-SHA",
-    "TLS_DH_RSA_WITH_CAMELLIA_128_CBC_SHA": "DH-RSA-CAMELLIA128-SHA",
-    "TLS_DH_RSA_WITH_CAMELLIA_256_CBC_SHA": "DH-RSA-CAMELLIA256-SHA",
-    "TLS_DHE_DSS_WITH_CAMELLIA_128_CBC_SHA": "DHE-DSS-CAMELLIA128-SHA",
-    "TLS_DHE_DSS_WITH_CAMELLIA_256_CBC_SHA": "DHE-DSS-CAMELLIA256-SHA",
-    "TLS_DHE_RSA_WITH_CAMELLIA_128_CBC_SHA": "DHE-RSA-CAMELLIA128-SHA",
-    "TLS_DHE_RSA_WITH_CAMELLIA_256_CBC_SHA": "DHE-RSA-CAMELLIA256-SHA",
-    "TLS_DH_anon_WITH_CAMELLIA_128_CBC_SHA": "ADH-CAMELLIA128-SHA",
-    "TLS_DH_anon_WITH_CAMELLIA_256_CBC_SHA": "ADH-CAMELLIA256-SHA",
-    # SEED cipher suites from RFC4162, extending TLS v1.0
-    "TLS_RSA_WITH_SEED_CBC_SHA": "SEED-SHA",
-    "TLS_DH_DSS_WITH_SEED_CBC_SHA": "DH-DSS-SEED-SHA",
-    "TLS_DH_RSA_WITH_SEED_CBC_SHA": "DH-RSA-SEED-SHA",
-    "TLS_DHE_DSS_WITH_SEED_CBC_SHA": "DHE-DSS-SEED-SHA",
-    "TLS_DHE_RSA_WITH_SEED_CBC_SHA": "DHE-RSA-SEED-SHA",
-    "TLS_DH_anon_WITH_SEED_CBC_SHA": "ADH-SEED-SHA",
-    # GOST cipher suites from draft-chudov-cryptopro-cptls, extending TLS v1.0
-    "TLS_GOSTR341094_WITH_28147_CNT_IMIT": "GOST94-GOST89-GOST89",
-    "TLS_GOSTR341001_WITH_28147_CNT_IMIT": "GOST2001-GOST89-GOST89",
-    "TLS_GOSTR341094_WITH_NULL_GOSTR3411": "GOST94-NULL-GOST94",
-    "TLS_GOSTR341001_WITH_NULL_GOSTR3411": "GOST2001-NULL-GOST94",
-}
 
-# TLS v1.1 cipher suites IANI to OpenSSL name translation
-TLSV1_1_CIPHER_SUITES = TLSV1_CIPHER_SUITES
+SUPPORTED_TLS_VERSIONS = (
+    tls_ciphers.APPROVED_TLS_VERSIONS + tls_ciphers.DEPRECATED_TLS_VERSIONS
+)
+
 
 # TLS v1.2 cipher suites IANI to OpenSSL name translation
 TLSV1_2_CIPHER_SUITES = {
     "TLS_RSA_WITH_NULL_SHA256": "NULL-SHA256",
     "TLS_RSA_WITH_AES_128_CBC_SHA256": "AES128-SHA256",
     "TLS_RSA_WITH_AES_256_CBC_SHA256": "AES256-SHA256",
     "TLS_RSA_WITH_AES_128_GCM_SHA256": "AES128-GCM-SHA256",
@@ -279,19 +226,15 @@
     "TLS_AES_256_GCM_SHA384": "TLS_AES_256_GCM_SHA384",
     "TLS_CHACHA20_POLY1305_SHA256": "TLS_CHACHA20_POLY1305_SHA256",
     "TLS_AES_128_CCM_SHA256": "TLS_AES_128_CCM_SHA256",
     "TLS_AES_128_CCM_8_SHA256": "TLS_AES_128_CCM_8_SHA256",
 }
 
 TLS_CIPHER_SUITES = {
-    "TLSv1": TLSV1_CIPHER_SUITES,
-    "TLSv1.1": TLSV1_1_CIPHER_SUITES,
     "TLSv1.2": TLSV1_2_CIPHER_SUITES,
     "TLSv1.3": TLSV1_3_CIPHER_SUITES,
 }
 
 OPENSSL_CS_NAMES = {
-    "TLSv1": TLSV1_CIPHER_SUITES.values(),
-    "TLSv1.1": TLSV1_1_CIPHER_SUITES.values(),
     "TLSv1.2": TLSV1_2_CIPHER_SUITES.values(),
     "TLSv1.3": TLSV1_3_CIPHER_SUITES.values(),
 }
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/crud.py` & `mysqlx-connector-python-8.4.0/mysqlx/crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2016, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2016, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/dbdoc.py` & `mysqlx-connector-python-8.4.0/mysqlx/dbdoc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2016, 2023, Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2016, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/errorcode.py` & `mysqlx-connector-python-8.4.0/mysqlx/errorcode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2013, 2023, Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2013, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/errors.py` & `mysqlx-connector-python-8.4.0/mysqlx/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2016, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2016, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/expr.py` & `mysqlx-connector-python-8.4.0/mysqlx/expr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2016, 2023, Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2016, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
@@ -969,17 +969,17 @@
 
         msg_expr = Message("Mysqlx.Expr.Expr")
         msg_expr["type"] = mysqlxpb_enum("Mysqlx.Expr.Expr.Type.PLACEHOLDER")
         if place_holder_name in self.placeholder_name_to_position:
             msg_expr["position"] = self.placeholder_name_to_position[place_holder_name]
         else:
             msg_expr["position"] = self.positional_placeholder_count
-            self.placeholder_name_to_position[
-                place_holder_name
-            ] = self.positional_placeholder_count
+            self.placeholder_name_to_position[place_holder_name] = (
+                self.positional_placeholder_count
+            )
             self.positional_placeholder_count += 1
         return msg_expr
 
     def cast(self) -> MessageType:
         """cast ::= CAST LPAREN expr AS cast_data_type RPAREN"""
         operator = Message("Mysqlx.Expr.Operator", name="cast")
         self.consume_token(TokenType.LPAREN)
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/helpers.py` & `mysqlx-connector-python-8.4.0/mysqlx/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2017, 2023, Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2017, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
@@ -32,15 +32,15 @@
 import decimal
 import functools
 import inspect
 import warnings
 
 from typing import Any, Callable, List, Optional, Union
 
-from .constants import TLS_CIPHER_SUITES, TLS_VERSIONS
+from .constants import SUPPORTED_TLS_VERSIONS, TLS_CIPHER_SUITES
 from .errors import InterfaceError
 from .types import EscapeTypes, StrOrBytes
 
 BYTE_TYPES = (bytearray, bytes)
 NUMERIC_TYPES = (int, float, decimal.Decimal)
 
 
@@ -203,16 +203,16 @@
         List[str]: List of translated names.
     """
     translated_names = []
 
     cipher_suites = {}  # TLS_CIPHER_SUITES[TLS_version]
 
     # Find the previews TLS versions of the given on TLS_version
-    for index in range(TLS_VERSIONS.index(tls_version) + 1):
-        cipher_suites.update(TLS_CIPHER_SUITES[TLS_VERSIONS[index]])
+    for index in range(SUPPORTED_TLS_VERSIONS.index(tls_version) + 1):
+        cipher_suites.update(TLS_CIPHER_SUITES[SUPPORTED_TLS_VERSIONS[index]])
 
     for name in cipher_suites_names:
         if "-" in name:
             translated_names.append(name)
         elif name in cipher_suites:
             translated_names.append(cipher_suites[name])
         else:
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/logger.py` & `mysqlx-connector-python-8.4.0/mysqlx/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2022, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2022, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/protocol.py` & `mysqlx-connector-python-8.4.0/mysqlx/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2016, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2016, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/result.py` & `mysqlx-connector-python-8.4.0/mysqlx/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2016, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2016, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/statement.py` & `mysqlx-connector-python-8.4.0/mysqlx/statement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2016, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2016, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/utils.py` & `mysqlx-connector-python-8.4.0/mysqlx/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2009, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2009, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
@@ -27,17 +27,20 @@
 # 51 Franklin St, Fifth Floor, Boston, MA 02110-1301  USA
 
 """Utilities."""
 
 import os
 import subprocess
 import sys
+import warnings
 
 from typing import Dict, Optional, Tuple
 
+from .tls_ciphers import DEPRECATED_TLS_CIPHERSUITES, DEPRECATED_TLS_VERSIONS
+
 
 def _parse_os_release() -> Dict[str, str]:
     """Parse the contents of /etc/os-release file.
 
     Returns:
         A dictionary containing release information.
     """
@@ -130,7 +133,46 @@
         return (
             distro.get("name", ""),
             distro.get("version_id", ""),
             distro.get("version_codename", ""),
         )
 
     return ("", "", "")
+
+
+def warn_ciphersuites_deprecated(cipher_as_ossl: str, tls_version: str) -> None:
+    """Emits a warning if a deprecated cipher is being utilized.
+
+    Args:
+        cipher: Must be ingested as OpenSSL name.
+        tls_versions: TLS version to check the cipher against.
+
+    Raises:
+        DeprecationWarning: If the cipher is flagged as deprecated
+                            according to the OSSA cipher list.
+    """
+    if cipher_as_ossl in DEPRECATED_TLS_CIPHERSUITES.get(tls_version, {}).values():
+        warn_msg = (
+            f"This connection is using TLS cipher {cipher_as_ossl} which is now "
+            "deprecated and will be removed in a future release of "
+            "MySQL Connector/Python."
+        )
+        warnings.warn(warn_msg, DeprecationWarning)
+
+
+def warn_tls_version_deprecated(tls_version: str) -> None:
+    """Emits a warning if a deprecated TLS version is being utilized.
+
+    Args:
+        tls_versions: TLS version to check.
+
+    Raises:
+        DeprecationWarning: If the TLS version is flagged as deprecated
+                            according to the OSSA cipher list.
+    """
+    if tls_version in DEPRECATED_TLS_VERSIONS:
+        warn_msg = (
+            f"This connection is using TLS version {tls_version} which is now "
+            "deprecated and will be removed in a future release of "
+            "MySQL Connector/Python."
+        )
+        warnings.warn(warn_msg, DeprecationWarning)
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/version.py` & `mysqlx-connector-python-8.4.0/mysqlx/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2012, 2023, Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2012, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
@@ -28,15 +28,15 @@
 
 """MySQL Connector/Python version information
 
 The file version.py gets installed and is available after installation
 as mysqlx.version.
 """
 
-VERSION = (8, 3, 0, "", 1)
+VERSION = (8, 4, 0, "", 1)
 
 # pylint: disable=consider-using-f-string
 if VERSION[3] and VERSION[4]:
     VERSION_TEXT = "{0}.{1}.{2}{3}{4}".format(*VERSION)
 else:
     VERSION_TEXT = "{0}.{1}.{2}".format(*VERSION[0:3])
 # pylint: enable=consider-using-f-string
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/locales/__init__.py` & `mysqlx-connector-python-8.4.0/mysqlx/locales/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2012, 2023, Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2012, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/locales/eng/__init__.py` & `mysqlx-connector-python-8.4.0/mysqlx/locales/eng/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2012, 2023, Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2012, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/locales/eng/client_error.py` & `mysqlx-connector-python-8.4.0/mysqlx/locales/eng/client_error.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2013, 2023, Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2013, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/protobuf/__init__.py` & `mysqlx-connector-python-8.4.0/mysqlx/protobuf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2017, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2017, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_connection_pb2.py` & `mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_connection_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2017, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2017, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_crud_pb2.py` & `mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_crud_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2017, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2017, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_cursor_pb2.py` & `mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_cursor_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2017, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2017, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_datatypes_pb2.py` & `mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_datatypes_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2017, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2017, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_expect_pb2.py` & `mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_expect_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2017, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2017, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_expr_pb2.py` & `mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_expr_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2017, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2017, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_notice_pb2.py` & `mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_notice_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2017, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2017, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_pb2.py` & `mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2017, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2017, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_prepare_pb2.py` & `mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_prepare_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2017, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2017, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_resultset_pb2.py` & `mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_resultset_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2017, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2017, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_session_pb2.py` & `mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_session_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2017, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2017, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx/protobuf/mysqlx_sql_pb2.py` & `mysqlx-connector-python-8.4.0/mysqlx/protobuf/mysqlx_sql_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2017, 2023, Oracle and/or its affiliates.
+# Copyright (c) 2017, 2024, Oracle and/or its affiliates.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License, version 2.0, as
 # published by the Free Software Foundation.
 #
-# This program is also distributed with certain software (including
+# This program is designed to work with certain software (including
 # but not limited to OpenSSL) that is licensed under separate terms,
 # as designated in a particular file or component or in included license
-# documentation.  The authors of MySQL hereby grant you an
+# documentation. The authors of MySQL hereby grant you an
 # additional permission to link the program and your derivative works
-# with the separately licensed software that they have included with
-# MySQL.
+# with the separately licensed software that they have either included with
+# the program or referenced in the documentation.
 #
 # Without limiting anything contained in the foregoing, this file,
 # which is part of MySQL Connector/Python, is also subject to the
 # Universal FOSS Exception, version 1.0, a copy of which can be found at
 # http://oss.oracle.com/licenses/universal-foss-exception.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx_connector_python-8.3.0-py3.8.egg-info/PKG-INFO` & `mysqlx-connector-python-8.4.0/mysqlx_connector_python-8.4.0-py3.8.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx-connector-python
-Version: 8.3.0
+Version: 8.4.0
 Summary: XDevAPI MySQL driver written in Python
 Home-page: http://dev.mysql.com/doc/connector-python/en/index.html
 Author: Oracle and/or its affiliates
 Author-email: 
 License: GNU GPLv2 (with FOSS License Exception)
 Download-URL: http://dev.mysql.com/downloads/connector/python/
 Description:
```

### Comparing `mysqlx-connector-python-8.3.0/mysqlx_connector_python-8.3.0-py3.8.egg-info/SOURCES.txt` & `mysqlx-connector-python-8.4.0/mysqlx_connector_python-8.4.0-py3.8.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 lib/mysqlx/expr.py
 lib/mysqlx/helpers.py
 lib/mysqlx/logger.py
 lib/mysqlx/protocol.py
 lib/mysqlx/py.typed
 lib/mysqlx/result.py
 lib/mysqlx/statement.py
+lib/mysqlx/tls_ciphers.py
 lib/mysqlx/types.py
 lib/mysqlx/utils.py
 lib/mysqlx/version.py
 lib/mysqlx/locales/__init__.py
 lib/mysqlx/locales/eng/__init__.py
 lib/mysqlx/locales/eng/client_error.py
 lib/mysqlx/protobuf/__init__.py
@@ -86,14 +87,15 @@
 tests/data/ssl/tests_client_cert.pem
 tests/data/ssl/tests_client_key.pem
 tests/data/ssl/tests_expired_server_cert.pem
 tests/data/ssl/tests_expired_server_key.pem
 tests/data/ssl/tests_server_cert.pem
 tests/data/ssl/tests_server_key.pem
 tests/qa/__init__.py
+tests/qa/test_qa_ciphers.py
 tests/qa/test_qa_mysqlx_api_result.py
 tests/qa/test_qa_mysqlx_api_transaction.py
 tests/qa/test_qa_mysqlx_collection_replace_remove_one.py
 tests/qa/test_qa_mysqlx_conn_ipv6.py
 tests/qa/test_qa_mysqlx_crud_collection_add.py
 tests/qa/test_qa_mysqlx_crud_collection_find.py
 tests/qa/test_qa_mysqlx_crud_collection_index.py
```

### Comparing `mysqlx-connector-python-8.3.0/LICENSE.txt` & `mysqlx-connector-python-8.4.0/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Licensing Information User Manual
 
-MySQL Connector/Python 8.3.0 Community
+MySQL Connector/Python 8.4.0 Community
      __________________________________________________________________
 
 Introduction
 
    This License Information User Manual contains Oracle's product license
    and other licensing information, including licensing information for
    third-party software which may be included in this distribution of
-   MySQL Connector/Python 8.3.0 Community.
+   MySQL Connector/Python 8.4.0 Community.
 
-   Last updated: November 2023
+   Last updated: March 2024
 
 Licensing Information
 
-   This release of MySQL Connector/Python 8.3.0 Community is brought to
+   This release of MySQL Connector/Python 8.4.0 Community is brought to
    you by the MySQL team at Oracle. This software is released under
    version 2 of the GNU General Public License (GPLv2), as set forth
    below, with the following additional permissions:
 
-   This distribution of MySQL Connector/Python 8.3.0 Community is
-   distributed with certain software (including but not limited to
-   OpenSSL) that is licensed under separate terms, as designated in a
-   particular file or component or in the license documentation. Without
-   limiting your rights under the GPLv2, the authors of MySQL hereby grant
-   you an additional permission to link the program and your derivative
-   works with the separately licensed software that they have included
-   with the program.
+   This distribution of MySQL Connector/Python 8.4.0 Community is designed
+   to work with certain software (including but not limited to OpenSSL)
+   that is licensed under separate terms, as designated in a particular
+   file or component or in the license documentation. Without limiting
+   your rights under the GPLv2, the authors of MySQL hereby grant you an
+   additional permission to link the program and your derivative works
+   with the separately licensed software that they have either included
+   with the program or referenced in the documentation.
 
    Without limiting the foregoing grant of rights under the GPLv2 and
    additional permission as to separately licensed software, this
    Connector is also subject to the Universal FOSS Exception, version 1.0,
    a copy of which is reproduced below and can also be found along with
    its FAQ at http://oss.oracle.com/licenses/universal-foss-exception.
 
-   Copyright (c) 2012, 2023, Oracle and/or its affiliates.
+   Copyright (c) 2012, 2024, Oracle and/or its affiliates.
 
 Election of GPLv2
 
    For the avoidance of doubt, except that if any license choice other
    than GPL or LGPL is available it will apply instead, Oracle elects to
    use only the General Public License version 2 (GPLv2) at this time for
    any software where a choice of GPL license versions is made available
@@ -638,14 +638,43 @@
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 Code generated by the Protocol Buffer compiler is owned by the owner
 of the input file used when generating it.  This code is not
 standalone and requires a support library to be linked with it.  This
 support library is itself covered by the above license.
 
+4th party - abseil-cpp
+----------------------
+
+=== Header in source files:
+// Copyright 2017 The Abseil Authors.
+//
+// Licensed under the Apache License, Version 2.0 (the "License");
+// you may not use this file except in compliance with the License.
+// You may obtain a copy of the License at
+//
+//      https://www.apache.org/licenses/LICENSE-2.0
+//
+// Unless required by applicable law or agreed to in writing, software
+// distributed under the License is distributed on an "AS IS" BASIS,
+// WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+// See the License for the specific language governing permissions and
+// limitations under the License.
+//
+// This header file contains C++11 versions of standard <utility> header
+// abstractions available within C++14 and C++17, and are designed to be
+// drop-in replacement for code compliant with C++14 and C++17.
+
+                                 Apache License
+                           Version 2.0, January 2004
+                        https://www.apache.org/licenses/
+
+A copy of the Apache License v2.0, January 2004 license can be found
+in the 'Standard Licenses' section.
+
    ======================================================================
    ======================================================================
 
 GSSAPI
 
 Copyright (c) 2014, The Python GSSAPI Team
 
@@ -2110,14 +2139,21 @@
 'Standard Licenses' section.
 
    ======================================================================
    ======================================================================
 
 OpenTelemetry C++
 
+You may be receiving a copy of the opentelemetry-cpp library with
+this MySQL product. The terms of the Oracle license do NOT apply
+to the opentelemetry-cpp library; it is licensed under the following
+license, separately from the Oracle programs you receive.
+If you do not wish to install this program, you may delete its files
+but the Oracle program might not operate properly or at all without it.
+
 // Copyright The OpenTelemetry Authors
 // SPDX-License-Identifier: Apache-2.0
 
 LICENSE:
                         Apache License
                   Version 2.0, January 2004
                http://www.apache.org/licenses/
```

### Comparing `mysqlx-connector-python-8.3.0/README.rst` & `mysqlx-connector-python-8.4.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -8,24 +8,38 @@
 .. image:: https://img.shields.io/pypi/l/mysql-connector-python.svg
    :target: https://pypi.org/project/mysql-connector-python/
 
 MySQL Connector/Python enables Python programs to access MySQL databases, using an API that is compliant with the `Python Database API Specification v2.0 (PEP 249) <https://www.python.org/dev/peps/pep-0249/>`_. It also contains an implementation of the `X DevAPI <https://dev.mysql.com/doc/x-devapi-userguide/en>`_, an Application Programming Interface for working with the `MySQL Document Store <https://dev.mysql.com/doc/refman/8.0/en/document-store.html>`_.
 
 Installation
 ------------
-
 The recommended way to install Connector/Python is via `pip <https://pip.pypa.io/>`_.
 
 Make sure you have a recent `pip <https://pip.pypa.io/>`_ version installed on your system. If your system already has ``pip`` installed, you might need to update it. Or you can use the `standalone pip installer <https://pip.pypa.io/en/latest/installing/#installing-with-get-pip-py>`_.
 
++++++++
+Classic
++++++++
+
 .. code-block:: bash
 
     shell> pip install mysql-connector-python
 
-Please refer to the `installation tutorial <https://dev.mysql.com/doc/dev/connector-python/8.0/installation.html>`_ for installation alternatives.
+
++++++++
+XDevAPI
++++++++
+
+.. code-block:: bash
+
+    shell> pip install mysqlx-connector-python
+
+
+Please refer to the `installation tutorial <https://dev.mysql.com/doc/dev/connector-python/8.0/installation.html>`_ for installation alternatives of the X DevAPI.
+
 
 Getting Started
 ---------------
 
 Using the MySQL classic protocol:
 
 .. code:: python
```

### Comparing `mysqlx-connector-python-8.3.0/CONTRIBUTING.rst` & `mysqlx-connector-python-8.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

