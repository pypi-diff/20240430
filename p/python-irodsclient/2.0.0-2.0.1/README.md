# Comparing `tmp/python-irodsclient-2.0.0.tar.gz` & `tmp/python-irodsclient-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-irodsclient-2.0.0.tar", last modified: Mon Feb 12 19:56:10 2024, max compression
+gzip compressed data, was "python-irodsclient-2.0.1.tar", last modified: Tue Apr 30 18:35:13 2024, max compression
```

## Comparing `python-irodsclient-2.0.0.tar` & `python-irodsclient-2.0.1.tar`

### file list

```diff
@@ -1,103 +1,104 @@
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-02-12 19:56:10.351770 python-irodsclient-2.0.0/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      595 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/AUTHORS
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    34330 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/CHANGELOG.rst
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     2120 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/LICENSE.txt
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      133 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/MANIFEST.in
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    75520 2024-02-12 19:56:10.351770 python-irodsclient-2.0.0/PKG-INFO
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    60950 2024-02-12 19:53:57.000000 python-irodsclient-2.0.0/README.md
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-02-12 19:56:10.339770 python-irodsclient-2.0.0/irods/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     2156 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/__init__.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3556 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/access.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1427 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/account.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     5444 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/api_number.py
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-02-12 19:56:10.343770 python-irodsclient-2.0.0/irods/auth/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      735 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/auth/__init__.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      334 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/auth/native.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      243 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/auth/pam_password.py
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-02-12 19:56:10.343770 python-irodsclient-2.0.0/irods/client_configuration/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    14798 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/client_configuration/__init__.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      995 2018-02-04 01:59:15.000000 python-irodsclient-2.0.0/irods/client_server_negotiation.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3949 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/collection.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3772 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/column.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    25077 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/connection.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)       79 2016-01-07 14:03:09.000000 python-irodsclient-2.0.0/irods/constants.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     7232 2024-02-12 19:53:57.000000 python-irodsclient-2.0.0/irods/data_object.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    39162 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/exception.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    10116 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/keywords.py
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-02-12 19:56:10.343770 python-irodsclient-2.0.0/irods/manager/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      552 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/manager/__init__.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     5972 2024-02-12 19:53:57.000000 python-irodsclient-2.0.0/irods/manager/access_manager.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     5072 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/manager/collection_manager.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    29013 2024-02-12 19:53:57.000000 python-irodsclient-2.0.0/irods/manager/data_object_manager.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     7119 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/manager/metadata_manager.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     5329 2018-02-04 01:59:15.000000 python-irodsclient-2.0.0/irods/manager/resource_manager.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    13715 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/manager/user_manager.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1593 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/manager/zone_manager.py
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-02-12 19:56:10.343770 python-irodsclient-2.0.0/irods/message/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    38449 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/message/__init__.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1222 2017-04-05 17:18:12.000000 python-irodsclient-2.0.0/irods/message/message.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1167 2017-04-05 17:18:12.000000 python-irodsclient-2.0.0/irods/message/ordered.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3378 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/message/property.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     5592 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/message/quasixml.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     6136 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/meta.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    11436 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/models.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    21944 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/parallel.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     9946 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/password_obfuscation.py
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-02-12 19:56:10.343770 python-irodsclient-2.0.0/irods/path/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3331 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/path/__init__.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     4845 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/pool.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    12244 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/query.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     4866 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/resource.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3127 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/results.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     7443 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/rule.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    14974 2024-02-12 19:53:57.000000 python-irodsclient-2.0.0/irods/session.py
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-02-12 19:56:10.347771 python-irodsclient-2.0.0/irods/test/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      726 2018-02-04 01:59:15.000000 python-irodsclient-2.0.0/irods/test/README.rst
--rw-rw-r--   0 tgr       (1000) tgr       (1000)        0 2014-09-05 15:54:22.000000 python-irodsclient-2.0.0/irods/test/__init__.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    16054 2024-02-12 19:53:57.000000 python-irodsclient-2.0.0/irods/test/access_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    14819 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/admin_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    13309 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/collection_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     5074 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/connection_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    88692 2024-02-12 19:53:57.000000 python-irodsclient-2.0.0/irods/test/data_obj_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1832 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/exception_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     2879 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/extended_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     2660 2018-02-04 01:59:15.000000 python-irodsclient-2.0.0/irods/test/file_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1599 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/force_create.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    12496 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/helpers.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    22120 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/login_auth_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     7198 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/message_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    21699 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/meta_test.py
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-02-12 19:56:10.351770 python-irodsclient-2.0.0/irods/test/modules/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)        0 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/modules/__init__.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1877 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/modules/test_auto_close_of_data_objects__issue_456.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1360 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/modules/test_saving_and_loading_of_settings__issue_471.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    15503 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/pool_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    41588 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/query_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     4667 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/resource_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    14829 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/rule_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1139 2017-09-03 17:28:09.000000 python-irodsclient-2.0.0/irods/test/runner.py
--rwxrwxr-x   0 tgr       (1000) tgr       (1000)     2827 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/setupssl.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      457 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/ssl_test_client.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     2866 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/temp_password_test.py
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-02-12 19:56:10.351770 python-irodsclient-2.0.0/irods/test/test-data/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      168 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/test-data/irods_environment.json
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      169 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/test-data/irods_environment_negative_refresh_field.json
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      126 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/test-data/irods_environment_no_refresh_field.json
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3528 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/test_paths.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    15267 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/ticket_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    26095 2016-01-07 14:03:09.000000 python-irodsclient-2.0.0/irods/test/unicode_sampler.xml
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3920 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/unicode_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    25921 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/user_group_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1932 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/test/zone_test.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3440 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/ticket.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     4002 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/user.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      226 2024-02-12 19:53:57.000000 python-irodsclient-2.0.0/irods/version.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      602 2024-01-21 20:12:39.000000 python-irodsclient-2.0.0/irods/zone.py
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-02-12 19:56:10.351770 python-irodsclient-2.0.0/python_irodsclient.egg-info/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    75520 2024-02-12 19:56:10.000000 python-irodsclient-2.0.0/python_irodsclient.egg-info/PKG-INFO
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     2379 2024-02-12 19:56:10.000000 python-irodsclient-2.0.0/python_irodsclient.egg-info/SOURCES.txt
--rw-rw-r--   0 tgr       (1000) tgr       (1000)        1 2024-02-12 19:56:10.000000 python-irodsclient-2.0.0/python_irodsclient.egg-info/dependency_links.txt
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      110 2024-02-12 19:56:10.000000 python-irodsclient-2.0.0/python_irodsclient.egg-info/requires.txt
--rw-rw-r--   0 tgr       (1000) tgr       (1000)        6 2024-02-12 19:56:10.000000 python-irodsclient-2.0.0/python_irodsclient.egg-info/top_level.txt
--rw-rw-r--   0 tgr       (1000) tgr       (1000)       80 2024-02-12 19:56:10.351770 python-irodsclient-2.0.0/setup.cfg
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     2109 2024-02-12 19:53:57.000000 python-irodsclient-2.0.0/setup.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-04-30 18:35:13.186267 python-irodsclient-2.0.1/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      595 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/AUTHORS
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    36689 2024-04-30 18:35:03.000000 python-irodsclient-2.0.1/CHANGELOG.rst
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     2120 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/LICENSE.txt
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      133 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/MANIFEST.in
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    75972 2024-04-30 18:35:13.190267 python-irodsclient-2.0.1/PKG-INFO
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    61330 2024-04-30 18:20:25.000000 python-irodsclient-2.0.1/README.md
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-04-30 18:35:13.178267 python-irodsclient-2.0.1/irods/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     2156 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/__init__.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3556 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/access.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1427 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/account.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     5475 2024-04-25 18:57:19.000000 python-irodsclient-2.0.1/irods/api_number.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-04-30 18:35:13.178267 python-irodsclient-2.0.1/irods/auth/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      735 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/auth/__init__.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      334 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/auth/native.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      316 2024-04-30 18:20:25.000000 python-irodsclient-2.0.1/irods/auth/pam.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      243 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/auth/pam_password.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-04-30 18:35:13.178267 python-irodsclient-2.0.1/irods/client_configuration/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    14798 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/client_configuration/__init__.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      995 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/client_server_negotiation.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3949 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/collection.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3772 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/column.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    25293 2024-04-25 18:57:19.000000 python-irodsclient-2.0.1/irods/connection.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)       79 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/constants.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     7232 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/data_object.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    39162 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/exception.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    10116 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/keywords.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-04-30 18:35:13.182267 python-irodsclient-2.0.1/irods/manager/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      552 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/manager/__init__.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     5972 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/manager/access_manager.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     5072 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/manager/collection_manager.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    29013 2024-04-30 18:20:25.000000 python-irodsclient-2.0.1/irods/manager/data_object_manager.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     7119 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/manager/metadata_manager.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     5329 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/manager/resource_manager.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    13898 2024-04-25 18:57:19.000000 python-irodsclient-2.0.1/irods/manager/user_manager.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1593 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/manager/zone_manager.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-04-30 18:35:13.182267 python-irodsclient-2.0.1/irods/message/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    38449 2024-04-25 18:57:19.000000 python-irodsclient-2.0.1/irods/message/__init__.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1222 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/message/message.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1167 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/message/ordered.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3378 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/message/property.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     5592 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/message/quasixml.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     6136 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/meta.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    11436 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/models.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    21944 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/parallel.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     9946 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/password_obfuscation.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-04-30 18:35:13.182267 python-irodsclient-2.0.1/irods/path/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3331 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/path/__init__.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     4845 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/pool.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    12244 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/query.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     4866 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/resource.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3127 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/results.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     7443 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/rule.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    14974 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/session.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-04-30 18:35:13.186267 python-irodsclient-2.0.1/irods/test/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      726 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/README.rst
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)        0 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/__init__.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    16054 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/access_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    14819 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/admin_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    13309 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/collection_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     5074 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/connection_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    89116 2024-04-30 18:20:25.000000 python-irodsclient-2.0.1/irods/test/data_obj_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1832 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/exception_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     2879 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/extended_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     2660 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/file_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1599 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/force_create.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    12496 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/helpers.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    22483 2024-04-25 18:57:19.000000 python-irodsclient-2.0.1/irods/test/login_auth_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     7198 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/message_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    21699 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/meta_test.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-04-30 18:35:13.186267 python-irodsclient-2.0.1/irods/test/modules/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)        0 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/modules/__init__.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1877 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/modules/test_auto_close_of_data_objects__issue_456.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1360 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/modules/test_saving_and_loading_of_settings__issue_471.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    15503 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/pool_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    41588 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/query_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     4667 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/resource_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    14829 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/rule_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1139 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/runner.py
+-rwxrwxr-x   0 tgr       (1000) tgr       (1000)     4422 2024-04-25 18:57:19.000000 python-irodsclient-2.0.1/irods/test/setupssl.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      457 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/ssl_test_client.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     2866 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/temp_password_test.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-04-30 18:35:13.186267 python-irodsclient-2.0.1/irods/test/test-data/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      168 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/test-data/irods_environment.json
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      169 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/test-data/irods_environment_negative_refresh_field.json
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      126 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/test-data/irods_environment_no_refresh_field.json
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3528 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/test_paths.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    15267 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/ticket_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    26095 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/unicode_sampler.xml
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3920 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/unicode_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    25921 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/user_group_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1932 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/test/zone_test.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3440 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/ticket.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     4058 2024-04-25 18:57:19.000000 python-irodsclient-2.0.1/irods/user.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      226 2024-04-30 18:35:03.000000 python-irodsclient-2.0.1/irods/version.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      602 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/irods/zone.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2024-04-30 18:35:13.186267 python-irodsclient-2.0.1/python_irodsclient.egg-info/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    75972 2024-04-30 18:35:13.000000 python-irodsclient-2.0.1/python_irodsclient.egg-info/PKG-INFO
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     2397 2024-04-30 18:35:13.000000 python-irodsclient-2.0.1/python_irodsclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)        1 2024-04-30 18:35:13.000000 python-irodsclient-2.0.1/python_irodsclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      110 2024-04-30 18:35:13.000000 python-irodsclient-2.0.1/python_irodsclient.egg-info/requires.txt
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)        6 2024-04-30 18:35:13.000000 python-irodsclient-2.0.1/python_irodsclient.egg-info/top_level.txt
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)       80 2024-04-30 18:35:13.190267 python-irodsclient-2.0.1/setup.cfg
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     2109 2024-02-13 00:03:21.000000 python-irodsclient-2.0.1/setup.py
```

### Comparing `python-irodsclient-2.0.0/AUTHORS` & `python-irodsclient-2.0.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/CHANGELOG.rst` & `python-irodsclient-2.0.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,47 @@
 Changelog
 =========
 
+v2.0.1 (2024-04-30)
+-------------------
+- [#543] Fix issue with parallel downloads to a directory [Raoul Schram]
+- [#521] clearer documentation and errors regarding pam/pam_password [Daniel Moore]
+- [#518] preserve login_<auth-type> internally generated exceptions [Daniel Moore]
+- [#522][#523] allow '=' and ';' in PAM passwords [Daniel Moore]
+- [#519] force verify mode to CERT_NONE if irods verify setting is explicitly none [Daniel Moore]
+- [#526] can now opt out of strong primes to speed up SSL & PAM tests [Daniel Moore]
+- [#3] make sure tempfile.mktemp imported where needed for tests [Daniel Moore]
+- [#3] tweak compatibility to iRODS 4.3.2 [Daniel Moore]
+- [#539] iRODS 4.3.2 rmgroup adaptation [Daniel Moore]
+
+v2.0.0 (2024-02-12)
+-------------------
+- [#3] version bump for 2.0.0 [Terrell Russell]
+- [#3] update project description [Terrell Russell]
+- [#495] append modes seek to end on data_object.open(...) [Daniel Moore]
+- [#510] update README to reflect removal of session.permissions [Terrell Russell]
+- [#510] change permissions to acls [Daniel Moore]
+- [#504] modify replicate/trim code snippet and description [Daniel Moore]
+- [#459] respect the default_resource setting for replication [Daniel Moore]
+- [#484,#509] Update version mentioned in README for Quota [Terrell Russell]
+- [#503] swap readme from .rst to markdown [Terrell Russell]
+- [#484] change to proper RST marker "::" in quotas section [Daniel Moore]
+- [#485][#430][#494] document new legacy_auth.pam.* settings [Daniel Moore]
+- [#501] context manager to temporarily alter settings [Daniel Moore]
+- [#430][#494][#498] client auth "plugins" / pam_password compatibility / TTL fix [Daniel Moore]
+- [#485] allow detection of config without actually loading it. [Daniel Moore]
+- [#462][#399] Default the dataSize to 0 and prefer DATA_SIZE_KW over seek [Daniel Moore]
+- [#497] suppress fatal errors when loading configuration [Daniel Moore]
+- [#485][#489] document available settings and override environment variables [Daniel Moore]
+- [#489] allow environment variable overrides of individual settings during autoload [Daniel Moore]
+- [#485] writeable_properties including xml parser [Daniel Moore]
+- [#484] Add quotas to README [Daniel Moore]
+- [#474][#479] Allow querying, setting, and removing quotas [Daniel Moore]
+- [#483] make PRC version available as tuple [Daniel Moore]
+
 v1.1.9 (2023-10-13)
 -------------------
 - [#471][#472] allow save, load, and autoload of configuration [Daniel Moore]
 - [#456] auto-close data objects that go out of scope [Daniel Moore]
 - [#455] remove ticket check [Daniel Moore]
 - [#452] implement client redirection to resource server [Daniel Moore]
 - [#455] introduce low level ticket api changes [Daniel Moore]
```

### Comparing `python-irodsclient-2.0.0/LICENSE.txt` & `python-irodsclient-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/PKG-INFO` & `python-irodsclient-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-irodsclient
-Version: 2.0.0
+Version: 2.0.1
 Summary: A python API for iRODS
 Home-page: https://github.com/irods/python-irodsclient
 Author: iRODS Consortium
 Author-email: support@irods.org
 License: BSD
 Description: Python iRODS Client (PRC)
         =========================
@@ -165,14 +165,23 @@
         ```
         
         Note that the `irods_` prefix is unnecessary when providing
         the `encryption_*` and `ssl_*` options
         directly to the constructor as keyword arguments, even though it is
         required when they are placed in the environment file.
         
+        PAM logins
+        ----------
+        
+        Starting with v2.0.0, the python iRODS client is able to authenticate under PAM using the same file-based client environment as the
+        iCommands.
+        
+        Caveat for iRODS 4.3+: when upgrading from 4.2, the "irods_authentication_scheme" setting must be changed from "pam" to "pam_password" in
+        `~/.irods/irods_environment.json` for all file-based client environments.
+        
         Maintaining a connection
         ------------------------
         
         The default library timeout for a connection to an iRODS Server is 120
         seconds.
         
         This can be overridden by changing the session `connection_timeout` immediately after creation of the
```

### Comparing `python-irodsclient-2.0.0/README.md` & `python-irodsclient-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,23 @@
 ```
 
 Note that the `irods_` prefix is unnecessary when providing
 the `encryption_*` and `ssl_*` options
 directly to the constructor as keyword arguments, even though it is
 required when they are placed in the environment file.
 
+PAM logins
+----------
+
+Starting with v2.0.0, the python iRODS client is able to authenticate under PAM using the same file-based client environment as the
+iCommands.
+
+Caveat for iRODS 4.3+: when upgrading from 4.2, the "irods_authentication_scheme" setting must be changed from "pam" to "pam_password" in
+`~/.irods/irods_environment.json` for all file-based client environments.
+
 Maintaining a connection
 ------------------------
 
 The default library timeout for a connection to an iRODS Server is 120
 seconds.
 
 This can be overridden by changing the session `connection_timeout` immediately after creation of the
```

### Comparing `python-irodsclient-2.0.0/irods/__init__.py` & `python-irodsclient-2.0.1/irods/__init__.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/access.py` & `python-irodsclient-2.0.1/irods/access.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/account.py` & `python-irodsclient-2.0.1/irods/account.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/api_number.py` & `python-irodsclient-2.0.1/irods/api_number.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,9 +175,11 @@
 
     # 1100 - 1200 - SSL API calls
     "SSL_START_AN": 1100,
     "SSL_END_AN": 1101,
     "GET_RESOURCE_INFO_FOR_OPERATION_AN": 10220,
     "ATOMIC_APPLY_METADATA_OPERATIONS_APN": 20002,
     "GET_FILE_DESCRIPTOR_INFO_APN": 20000,
-    "REPLICA_CLOSE_APN": 20004
+    "REPLICA_CLOSE_APN": 20004,
+
+    "AUTH_PLUG_REQ_AN": 1201
 }
```

### Comparing `python-irodsclient-2.0.0/irods/auth/__init__.py` & `python-irodsclient-2.0.1/irods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/client_configuration/__init__.py` & `python-irodsclient-2.0.1/irods/client_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/client_server_negotiation.py` & `python-irodsclient-2.0.1/irods/client_server_negotiation.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/collection.py` & `python-irodsclient-2.0.1/irods/collection.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/column.py` & `python-irodsclient-2.0.1/irods/column.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/connection.py` & `python-irodsclient-2.0.1/irods/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,14 @@
     OpenedDataObjRequest, FileSeekResponse, StringStringMap, VersionResponse,
     PluginAuthMessage, ClientServerNegotiation, Error, GetTempPasswordOut)
 from irods.exception import (get_exception_by_code, NetworkException, nominal_code)
 import irods.exception as ex
 from irods.message import (PamAuthRequest, PamAuthRequestOut)
 
 
-
-ALLOW_PAM_LONG_TOKENS = True      # True to fix [#279]
 # Message to be logged when the connection
 # destructor is called. Used in a unit test
 DESTRUCTOR_MSG = "connection __del__() called"
 
 from irods import (
     MAX_PASSWORD_LENGTH, RESPONSE_LEN,
     AUTH_SCHEME_KEY, AUTH_USER_KEY, AUTH_PWD_KEY, AUTH_TTL_KEY,
@@ -61,39 +59,42 @@
         self.socket = None
         self.account = account
         self._client_signature = None
         self._server_version = self._connect()
         self._disconnected = False
 
         scheme = self.account._original_authentication_scheme
-        auth_type = ''
+
+        # These variables are just useful diagnostics.  The login_XYZ() methods should fail by
+        # raising exceptions if they encounter authentication errors.
+        auth_module = auth_type = ''
 
         if self.server_version >= (4,3,0):
+            auth_module = None
             # use client side "plugin" module: irods.auth.<scheme>
             irods.auth.load_plugins(subset=[scheme])
             auth_module = getattr(irods.auth, scheme, None)
             if auth_module:
                 auth_module.login(self)
                 auth_type = auth_module.__name__
         else:
             # use legacy (iRODS pre-4.3 style) authentication
             auth_type = scheme
-            try:
-                if scheme == NATIVE_AUTH_SCHEME:
-                    self._login_native()
-                elif scheme == GSI_AUTH_SCHEME:
-                    self.client_ctx = None
-                    self._login_gsi()
-                elif scheme == PAM_AUTH_SCHEME:
-                    self._login_pam()
-            except:
+            if scheme == NATIVE_AUTH_SCHEME:
+                self._login_native()
+            elif scheme == GSI_AUTH_SCHEME:
+                self.client_ctx = None
+                self._login_gsi()
+            elif scheme == PAM_AUTH_SCHEME:
+                self._login_pam()
+            else:
                 auth_type = None
 
         if not auth_type:
-            msg = "Authentication failed: scheme = {scheme!r}, auth_type = {auth_type!r}".format(**locals())
+            msg = "Authentication failed: scheme = {scheme!r}, auth_type = {auth_type!r}, auth_module = {auth_module!r}, ".format(**locals())
             raise ValueError(msg)
 
         self.create_time = datetime.datetime.now()
         self.last_used_time = self.create_time
 
     @property
     def server_version(self):
@@ -177,22 +178,22 @@
                 return True
         except AttributeError:
             return False
         return False
 
     @staticmethod
     def make_ssl_context(irods_account):
-        check_hostname = getattr(irods_account,'ssl_verify_server','hostname')
+        verify_server = getattr(irods_account,'ssl_verify_server','hostname')
         CAfile = getattr(irods_account,'ssl_ca_certificate_file',None)
         CApath = getattr(irods_account,'ssl_ca_certificate_path',None)
-        verify = ssl.CERT_NONE if (None is CAfile is CApath) else ssl.CERT_REQUIRED
+        verify = ssl.CERT_NONE if ((None is CAfile is CApath) or verify_server == 'none') else ssl.CERT_REQUIRED
         # See https://stackoverflow.com/questions/30461969/disable-default-certificate-verification-in-python-2-7-9/49040695#49040695
         ctx = ssl.create_default_context(ssl.Purpose.SERVER_AUTH, cafile=CAfile, capath=CApath)
         # Note: check_hostname must be assigned prior to verify_mode property or Python library complains!
-        ctx.check_hostname = (check_hostname.startswith('host') and verify != ssl.CERT_NONE)
+        ctx.check_hostname = (verify_server == 'hostname' and verify != ssl.CERT_NONE)
         ctx.verify_mode = verify
         return ctx
 
     def ssl_startup(self):
         # Get encryption settings from client environment
         host = self.account.host
         algo = self.account.encryption_algorithm
@@ -462,23 +463,21 @@
         time_to_live_in_hours = 0
         # For certain characters in the pam password, if they need escaping with '\' then do so.
         new_pam_password = PAM_PW_ESC_PATTERN.sub(lambda m: '\\'+m.group(1), self.account.password)
         if not inline_password:
             # Login using PAM password from .irodsA
             try:
                 self._login_native()
-            except (ex.CAT_PASSWORD_EXPIRED, ex.CAT_INVALID_USER, ex.CAT_INVALID_AUTHENTICATION):
+            except (ex.CAT_PASSWORD_EXPIRED, ex.CAT_INVALID_USER, ex.CAT_INVALID_AUTHENTICATION) as exc:
                 time_to_live_in_hours = cfg.legacy_auth.pam.time_to_live_in_hours
                 if cfg.legacy_auth.pam.password_for_auto_renew:
                     new_pam_password = cfg.legacy_auth.pam.password_for_auto_renew
                     # Fall through and retry the native login later, after creating a new PAM password
                 else:
-                    message = ('Time To Live has expired for the PAM password, and no new password is given in ' +
-                               'legacy_auth.pam.password_for_auto_renew.  Please run iinit.')
-                    raise RuntimeError(message)
+                    raise exc
             else:
                 # Login succeeded, so we're within the time-to-live and can return without error.
                 return
 
         # Generate a new PAM password.
         ctx_user = '%s=%s' % (AUTH_USER_KEY, self.account.client_user)
         ctx_pwd = '%s=%s' % (AUTH_PWD_KEY, new_pam_password)
@@ -486,39 +485,41 @@
 
         ctx = ";".join([ctx_user, ctx_pwd, ctx_ttl])
 
         if type(self.socket) is socket.socket:
             if getattr(self,'DISALLOWING_PAM_PLAINTEXT',True):
                 raise PlainTextPAMPasswordError
 
-        Pam_Long_Tokens = (ALLOW_PAM_LONG_TOKENS and (len(ctx) >= MAX_NAME_LEN))
+        # In general authentication API, a ';' and '=' in the password would be misinterpreted due to those
+        # characters' special meaning in the context string parameter.
+        use_dedicated_pam_api = len(ctx) >= MAX_NAME_LEN or \
+                                {';','='}.intersection(set(new_pam_password))
 
-        if Pam_Long_Tokens:
+        if use_dedicated_pam_api:
             message_body = PamAuthRequest( pamUser = self.account.client_user,
                                            pamPassword = new_pam_password,
                                            timeToLive = time_to_live_in_hours)
         else:
             message_body = PluginAuthMessage( auth_scheme_ = PAM_AUTH_SCHEME,  context_ = ctx)
 
         auth_req = iRODSMessage(
             msg_type='RODS_API_REQ',
             msg=message_body,
-            int_info=(725 if Pam_Long_Tokens else 1201)
+            int_info=api_number['PAM_AUTH_REQUEST_AN' if use_dedicated_pam_api else 'AUTH_PLUG_REQ_AN']
         )
 
         self.send(auth_req)
         # Getting the new password
         try:
             output_message = self.recv()
         except irods.exception.PAM_AUTH_PASSWORD_INVALID_TTL as exc:
             # TODO (#480): In Python3 will be able to do: 'raise RuntimeError(...) from exc' for more succinct error messages
             raise RuntimeError('Client-configured TTL is outside server parameters (password min and max times)')
 
-        Pam_Response_Class = (PamAuthRequestOut if Pam_Long_Tokens
-                         else AuthPluginOut)
+        Pam_Response_Class = (PamAuthRequestOut if use_dedicated_pam_api else AuthPluginOut)
 
         auth_out = output_message.get_main_message( Pam_Response_Class )
 
         self.disconnect()
         self._connect()
 
         if hasattr(self.account,'store_pw'):
```

### Comparing `python-irodsclient-2.0.0/irods/data_object.py` & `python-irodsclient-2.0.1/irods/data_object.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/exception.py` & `python-irodsclient-2.0.1/irods/exception.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/keywords.py` & `python-irodsclient-2.0.1/irods/keywords.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/manager/__init__.py` & `python-irodsclient-2.0.1/irods/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/manager/access_manager.py` & `python-irodsclient-2.0.1/irods/manager/access_manager.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/manager/collection_manager.py` & `python-irodsclient-2.0.1/irods/manager/collection_manager.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/manager/data_object_manager.py` & `python-irodsclient-2.0.1/irods/manager/data_object_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             raise ex.OVERWRITE_WITHOUT_FORCE_FLAG
 
         data_open_returned_values_ = {}
         with open(local_file, 'wb') as f:
             with self.open(obj, 'r', returned_values = data_open_returned_values_, **options) as o:
                 if self.should_parallelize_transfer (num_threads, o, open_options = options.items()):
                     f.close()
-                    if not self.parallel_get( (obj,o), local_path, num_threads = num_threads,
+                    if not self.parallel_get( (obj,o), local_file, num_threads = num_threads,
                                               target_resource_name = options.get(kw.RESC_NAME_KW,''),
                                               data_open_returned_values = data_open_returned_values_):
                         raise RuntimeError("parallel get failed")
                 else:
                     for chunk in chunks(o, self.READ_BUFFER_SIZE):
                         f.write(chunk)
```

### Comparing `python-irodsclient-2.0.0/irods/manager/metadata_manager.py` & `python-irodsclient-2.0.1/irods/manager/metadata_manager.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/manager/resource_manager.py` & `python-irodsclient-2.0.1/irods/manager/resource_manager.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/manager/user_manager.py` & `python-irodsclient-2.0.1/irods/manager/user_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,18 +85,20 @@
                                int_info=api_number['GENERAL_ADMIN_AN'])
         with self.sess.pool.get_connection() as conn:
             conn.send(request)
             response = conn.recv()
         logger.debug(response.int_info)
         return self.get(user_name, user_zone)
 
-    def remove(self, user_name, user_zone=""):
+    def remove(self, user_name, user_zone="", _object = None):
+        if _object is None:
+            _object = self.get(user_name, user_zone)
         message_body = GeneralAdminRequest(
             "rm",
-            "user",
+            "user" if (_object.type != "rodsgroup" or self.sess.server_version < (4, 3, 2)) else "group",
             user_name,
             user_zone
         )
         request = iRODSMessage("RODS_API_REQ", msg=message_body,
                                int_info=api_number['GENERAL_ADMIN_AN'])
         with self.sess.pool.get_connection() as conn:
             conn.send(request)
```

### Comparing `python-irodsclient-2.0.0/irods/manager/zone_manager.py` & `python-irodsclient-2.0.1/irods/manager/zone_manager.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/message/__init__.py` & `python-irodsclient-2.0.1/irods/message/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
     if isinstance(server_version, _TUPLE_LIKE_TYPES):
         _thrlocal.irods_server_version = tuple(server_version)  #  A default server version for Quasi-XML parsing is set (from the environment) and
     return _XML_parsers[current_XML_parser()]                   #  applies to all threads in which ET() has not been called to update the value.
 
 
 logger = logging.getLogger(__name__)
 
-IRODS_VERSION = (4, 3, 1, 'd')
+IRODS_VERSION = (4, 3, 2, 'd')
 
 try:
     # Python 2
     UNICODE = unicode
 except NameError:
     # Python 3
     UNICODE = str
```

### Comparing `python-irodsclient-2.0.0/irods/message/message.py` & `python-irodsclient-2.0.1/irods/message/message.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/message/ordered.py` & `python-irodsclient-2.0.1/irods/message/ordered.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/message/property.py` & `python-irodsclient-2.0.1/irods/message/property.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/message/quasixml.py` & `python-irodsclient-2.0.1/irods/message/quasixml.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/meta.py` & `python-irodsclient-2.0.1/irods/meta.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/models.py` & `python-irodsclient-2.0.1/irods/models.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/parallel.py` & `python-irodsclient-2.0.1/irods/parallel.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/password_obfuscation.py` & `python-irodsclient-2.0.1/irods/password_obfuscation.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/path/__init__.py` & `python-irodsclient-2.0.1/irods/path/__init__.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/pool.py` & `python-irodsclient-2.0.1/irods/pool.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/query.py` & `python-irodsclient-2.0.1/irods/query.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/resource.py` & `python-irodsclient-2.0.1/irods/resource.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/results.py` & `python-irodsclient-2.0.1/irods/results.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/rule.py` & `python-irodsclient-2.0.1/irods/rule.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/session.py` & `python-irodsclient-2.0.1/irods/session.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/README.rst` & `python-irodsclient-2.0.1/irods/test/README.rst`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/access_test.py` & `python-irodsclient-2.0.1/irods/test/access_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/admin_test.py` & `python-irodsclient-2.0.1/irods/test/admin_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/collection_test.py` & `python-irodsclient-2.0.1/irods/test/collection_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/connection_test.py` & `python-irodsclient-2.0.1/irods/test/connection_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/data_obj_test.py` & `python-irodsclient-2.0.1/irods/test/data_obj_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 import irods.test.modules as test_modules
 import irods.keywords as kw
 import irods.client_configuration as config
 from irods.manager import data_object_manager
 from irods.message import RErrorStack
 from irods.message import ( ET, XML_Parser_Type, default_XML_parser, current_XML_parser )
 from datetime import datetime
-from tempfile import NamedTemporaryFile, gettempdir
+from tempfile import NamedTemporaryFile, gettempdir, mktemp
 from irods.test.helpers import (unique_name, my_function_name)
 from irods.ticket import Ticket
 import irods.parallel
 from irods.manager.data_object_manager import Server_Checksum_Warning
 
 RODSUSER = 'nonadmin'
 
@@ -1300,28 +1300,36 @@
         os.remove(test_file)
 
         # remove ufs resources
         for resource in ufs_resources:
             resource.remove()
 
 
-    def test_obj_put_get(self):
+    def test_obj_put_get_small(self):
+        # Test put/get with 16M binary file that will be transferred with a single thread.
+        self._check_obj_put_get(1024 * 1024 * 16)
+
+    def test_obj_put_get_large(self):
+        # Test put/get with binary file that is large enough to trigger parallel transfers.
+        self._check_obj_put_get(data_object_manager.MAXIMUM_SINGLE_THREADED_TRANSFER_SIZE + 1)
+        
+    def _check_obj_put_get(self, file_size):
         # Can't do one step open/create with older servers
         if self.sess.server_version <= (4, 1, 4):
             self.skipTest('For iRODS 4.1.5 and newer')
 
         # test vars
         test_dir = '/tmp'
         filename = 'obj_put_get_test_file'
         test_file = os.path.join(test_dir, filename)
         collection = self.coll.path
 
-        # make random 16M binary file
+        # make random binary file
         with open(test_file, 'wb') as f:
-            f.write(os.urandom(1024 * 1024 * 16))
+            f.write(os.urandom(file_size))
 
         # compute file checksum
         digest = self.sha256_checksum(test_file)
 
         # put file in test collection
         self.sess.data_objects.put(test_file, collection + '/')
```

### Comparing `python-irodsclient-2.0.0/irods/test/exception_test.py` & `python-irodsclient-2.0.1/irods/test/exception_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/extended_test.py` & `python-irodsclient-2.0.1/irods/test/extended_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/file_test.py` & `python-irodsclient-2.0.1/irods/test/file_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/force_create.py` & `python-irodsclient-2.0.1/irods/test/force_create.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/helpers.py` & `python-irodsclient-2.0.1/irods/test/helpers.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/login_auth_test.py` & `python-irodsclient-2.0.1/irods/test/login_auth_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from irods.access import iRODSAccess
 import irods.exception as ex
 import contextlib
 import socket
 from re import compile as regex
 import gc
 import six
+from irods.test.setupssl import create_ssl_dir
 
 #
 # Allow override to specify the PAM password in effect for the test rodsuser.
 #
 TEST_PAM_PW_OVERRIDE = os.environ.get('PYTHON_IRODSCLIENT_TEST_PAM_PW_OVERRIDE','')
 TEST_PAM_PW = TEST_PAM_PW_OVERRIDE or 'test123'
 
@@ -53,42 +54,39 @@
     with open(fname,'w') as out:
         json.dump(j, out, indent=4)
 
 def env_dir_fullpath(authtype):  return os.path.join( os.environ['HOME'] , '.irods.' + authtype)
 def json_env_fullpath(authtype):  return os.path.join( env_dir_fullpath(authtype), 'irods_environment.json')
 def secrets_fullpath(authtype):   return os.path.join( env_dir_fullpath(authtype), '.irodsA')
 
-SERVER_ENV_PATH = os.path.expanduser('~irods/.irods/irods_environment.json')
+RODSADMIN_ENV_PATH = os.path.expanduser('~/.irods/irods_environment.json')
 
 SERVER_ENV_SSL_SETTINGS = {
     "irods_ssl_certificate_chain_file": "/etc/irods/ssl/irods.crt",
     "irods_ssl_certificate_key_file": "/etc/irods/ssl/irods.key",
     "irods_ssl_dh_params_file": "/etc/irods/ssl/dhparams.pem",
     "irods_ssl_ca_certificate_file": "/etc/irods/ssl/irods.crt",
     "irods_ssl_verify_server": "cert"
 }
 
-def update_service_account_for_SSL():
-    json_file_update( SERVER_ENV_PATH, **SERVER_ENV_SSL_SETTINGS )
-
 CLIENT_OPTIONS_FOR_SSL = {
     "irods_client_server_policy": "CS_NEG_REQUIRE",
     "irods_client_server_negotiation": "request_server_negotiation",
     "irods_ssl_ca_certificate_file": "/etc/irods/ssl/irods.crt",
     "irods_ssl_verify_server": "cert",
     "irods_encryption_key_size": 16,
     "irods_encryption_salt_size": 8,
     "irods_encryption_num_hash_rounds": 16,
     "irods_encryption_algorithm": "AES-256-CBC"
 }
 
 
-def client_env_from_server_env(user_name, auth_scheme=""):
+def client_env_keys_from_admin_env(user_name, auth_scheme=""):
     cli_env = {}
-    with open(SERVER_ENV_PATH) as f:
+    with open(RODSADMIN_ENV_PATH) as f:
         srv_env = json.load(f)
         for k in [ "irods_host", "irods_zone_name", "irods_port"  ]:
             cli_env [k] = srv_env[k]
     cli_env["irods_user_name"] = user_name
     if auth_scheme:
         cli_env["irods_authentication_scheme"] = auth_scheme
     return cli_env
@@ -159,15 +157,15 @@
 
     def create_env_dirs(self):
         dirs = {}
         retval = []
         # -- create environment configurations and secrets
         with pam_password_in_plaintext():
             for dirname,lookup in self.user_auth_envs.items():
-                if lookup['AUTH'] == 'pam':
+                if lookup['AUTH'] in ('pam','pam_password'):
                     ses = iRODSSession( host=gethostname(),
                                         user=lookup['USER'],
                                         zone='tempZone',
                                         authentication_scheme=lookup['AUTH'],
                                         password=lookup['PASSWORD'],
                                         port= 1247 )
                     try:
@@ -175,15 +173,15 @@
                     except AttributeError:
                         pam_hashes = []
                     if not pam_hashes: print('Warning ** PAM pw couldnt be generated' ); break
                     scrambled_pw = pw_encode( pam_hashes[0] )
                #elif lookup['AUTH'] == 'XXXXXX': # TODO: insert other authentication schemes here
                 elif lookup['AUTH'] in ('native', '',None):
                     scrambled_pw = pw_encode( lookup['PASSWORD'] )
-                cl_env = client_env_from_server_env(TEST_RODS_USER)
+                cl_env = client_env_keys_from_admin_env(TEST_RODS_USER)
                 if lookup.get('AUTH',None) is not None:     # - specify auth scheme only if given
                     cl_env['irods_authentication_scheme'] = lookup['AUTH']
                 dirbase = os.path.join(os.environ['HOME'],dirname)
                 dirs[dirbase] = { 'secrets':scrambled_pw , 'client_environment':cl_env }
 
         # -- create the environment directories and write into them the configurations just created
         for absdir in dirs.keys():
@@ -195,26 +193,27 @@
             with open(os.path.join(absdir,'.irodsA'),'w') as secrets_file:
                 secrets_file.write(dirs[absdir]['secrets'])
             os.chmod(secrets_file.name,0o600)
 
         retval = dirs.keys()
         return retval
 
+    PAM_SCHEME_STRING = 'pam'
 
     @classmethod
     def setUpClass(cls):
         cls.admin = helpers.make_session()
+        if cls.admin.server_version >= (4,3):
+            cls.PAM_SCHEME_STRING = cls.user_auth_envs['.irods.pam']['AUTH'] = 'pam_password'
 
     @classmethod
     def tearDownClass(cls):
         cls.admin.cleanup()
 
     def setUp(self):
-        if os.environ['HOME'] != '/var/lib/irods':
-            self.skipTest('Must be run as irods')
         super(TestLogins,self).setUp()
 
     def tearDown(self):
         for envdir in getattr(self, 'envdirs', []):
             shutil.rmtree(envdir, ignore_errors=True)
         super(TestLogins,self).tearDown()
 
@@ -240,20 +239,22 @@
             if make_irods_pw:
                 self.admin.users.modify(name,'password',TEST_IRODS_PW)
             yield
         finally:
             self.admin.users.remove( name )
 
     def tst0(self, ssl_opt, auth_opt, env_opt, name = TEST_RODS_USER, make_irods_pw = False):
-
+        _auth_opt = auth_opt
+        if auth_opt in ('pam', 'pam_password'):
+            auth_opt = self.PAM_SCHEME_STRING
         with self._setup_rodsuser_and_optional_pw(name = name, make_irods_pw = make_irods_pw):
             self.envdirs = self.create_env_dirs()
             if not self.envdirs:
                 raise RuntimeError('Could not create one or more client environments')
-            auth_opt_explicit = 'native' if auth_opt=='' else  auth_opt
+            auth_opt_explicit = 'native' if _auth_opt=='' else  _auth_opt
             verbosity=False
             #verbosity='' # -- debug - sanity check by printing out options applied
             out = {'':''}
             if env_opt:
                 with self.setenv('IRODS_ENVIRONMENT_FILE', json_env_fullpath(auth_opt_explicit)) as env_file,\
                      self.setenv('IRODS_AUTHENTICATION_FILE', secrets_fullpath(auth_opt_explicit)):
                     cli_env_extras = {} if not(ssl_opt) else dict( CLIENT_OPTIONS_FOR_SSL )
@@ -278,15 +279,15 @@
                     SSL_cert = CLIENT_OPTIONS_FOR_SSL["irods_ssl_ca_certificate_file"]
                     session_options.update(
                         ssl_context = ssl.create_default_context ( purpose = ssl.Purpose.SERVER_AUTH,
                                                                    capath = None,
                                                                    cadata = None,
                                                                    cafile = SSL_cert),
                         **CLIENT_OPTIONS_FOR_SSL )
-                lookup = self.user_auth_envs ['.irods.'+('native' if not(auth_opt) else auth_opt)]
+                lookup = self.user_auth_envs ['.irods.'+('native' if not(_auth_opt) else _auth_opt)]
                 session = iRODSSession ( host=gethostname(),
                                          user=lookup['USER'],
                                          zone='tempZone',
                                          password=lookup['PASSWORD'],
                                          port= 1247,
                                          **session_options )
                 out = session_options
@@ -504,28 +505,31 @@
         with helpers.make_session() as session:
             if not session.host in ('localhost', socket.gethostname()):
                 self.skipTest('Test must be run co-resident with server')
 
 
     def test_ssl_with_server_verify_set_to_none_281(self):
         env_file = os.path.expanduser('~/.irods/irods_environment.json')
-        with helpers.file_backed_up(env_file):
-            with open(env_file) as env_file_handle:
-                env = json.load( env_file_handle )
-            env.update({ "irods_client_server_negotiation": "request_server_negotiation",
-                         "irods_client_server_policy": "CS_NEG_REQUIRE",
-                         "irods_ssl_ca_certificate_file": "/path/to/some/file.crt",  # does not need to exist
-                         "irods_ssl_verify_server": "none",
-                         "irods_encryption_key_size": 32,
-                         "irods_encryption_salt_size": 8,
-                         "irods_encryption_num_hash_rounds": 16,
-                         "irods_encryption_algorithm": "AES-256-CBC" })
-            with open(env_file,'w') as f:
-                json.dump(env,f)
-            with helpers.make_session() as session:
-                session.collections.get('/{session.zone}/home/{session.username}'.format(**locals()))
-
+        my_ssl_directory = ''
+        try:
+            with helpers.file_backed_up(env_file):
+                with open(env_file) as env_file_handle:
+                    env = json.load( env_file_handle )
+                my_ssl_directory = tempfile.mkdtemp(dir = os.path.expanduser("~"))
+                # Elect for efficiency in DH param generation, eg. when setting up for testing.
+                create_ssl_dir(ssl_dir = my_ssl_directory, use_strong_primes_for_dh_generation = False)
+                settings_to_update = {key:value.replace("/etc/irods/ssl",my_ssl_directory)
+                                  for key,value in env.items() if type(value) is str and value.startswith("/etc/irods/ssl")}
+                settings_to_update["irods_ssl_verify_server"] = "none"
+                env.update( settings_to_update )
+                with open(env_file,'w') as f:
+                    json.dump(env,f)
+                with helpers.make_session() as session:
+                    session.collections.get('/{session.zone}/home/{session.username}'.format(**locals()))
+        finally:
+            if my_ssl_directory:
+                shutil.rmtree(my_ssl_directory)
 
 if __name__ == '__main__':
     # let the tests find the parent irods lib
     sys.path.insert(0, os.path.abspath('../..'))
     unittest.main()
```

### Comparing `python-irodsclient-2.0.0/irods/test/message_test.py` & `python-irodsclient-2.0.1/irods/test/message_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/meta_test.py` & `python-irodsclient-2.0.1/irods/test/meta_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/modules/test_auto_close_of_data_objects__issue_456.py` & `python-irodsclient-2.0.1/irods/test/modules/test_auto_close_of_data_objects__issue_456.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/modules/test_saving_and_loading_of_settings__issue_471.py` & `python-irodsclient-2.0.1/irods/test/modules/test_saving_and_loading_of_settings__issue_471.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/pool_test.py` & `python-irodsclient-2.0.1/irods/test/pool_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/query_test.py` & `python-irodsclient-2.0.1/irods/test/query_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/resource_test.py` & `python-irodsclient-2.0.1/irods/test/resource_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/rule_test.py` & `python-irodsclient-2.0.1/irods/test/rule_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/runner.py` & `python-irodsclient-2.0.1/irods/test/runner.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/temp_password_test.py` & `python-irodsclient-2.0.1/irods/test/temp_password_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/test_paths.py` & `python-irodsclient-2.0.1/irods/test/test_paths.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/ticket_test.py` & `python-irodsclient-2.0.1/irods/test/ticket_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/unicode_sampler.xml` & `python-irodsclient-2.0.1/irods/test/unicode_sampler.xml`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/unicode_test.py` & `python-irodsclient-2.0.1/irods/test/unicode_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/user_group_test.py` & `python-irodsclient-2.0.1/irods/test/user_group_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/test/zone_test.py` & `python-irodsclient-2.0.1/irods/test/zone_test.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/ticket.py` & `python-irodsclient-2.0.1/irods/ticket.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/irods/user.py` & `python-irodsclient-2.0.1/irods/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,22 +61,24 @@
     def modify(self, *args, **kwargs):
         self.manager.modify(self.name, *args, **kwargs)
 
     def __repr__(self):
         return "<iRODSUser {id} {name} {type} {zone}>".format(**vars(self))
 
     def remove(self):
-        self.manager.remove(self.name, self.zone)
+        self.manager.remove(self.name, self.zone, _object = self)
 
     def temp_password(self):
         return self.manager.temp_password_for_user(self.name)
 
 
 class iRODSGroup(object):
 
+    type = "rodsgroup"
+
     def remove_quota(self, resource = 'total'):
         self.set_quota(amount = 0, resource = resource)
 
     def set_quota(self, amount, resource = 'total'):
         self.manager.set_quota(self.name, amount, resource = resource)
 
     def __init__(self, manager, result=None):
@@ -86,15 +88,15 @@
             self.name = result[Group.name]
         self._meta = None
 
     def __repr__(self):
         return "<iRODSGroup {id} {name}>".format(**vars(self))
 
     def remove(self):
-        self.manager.remove(self.name)
+        self.manager.remove(self.name, _object = self)
 
     @property
     def members(self):
         return self.manager.getmembers(self.name)
 
     @property
     def metadata(self):
```

### Comparing `python-irodsclient-2.0.0/irods/zone.py` & `python-irodsclient-2.0.1/irods/zone.py`

 * *Files identical despite different names*

### Comparing `python-irodsclient-2.0.0/python_irodsclient.egg-info/PKG-INFO` & `python-irodsclient-2.0.1/python_irodsclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-irodsclient
-Version: 2.0.0
+Version: 2.0.1
 Summary: A python API for iRODS
 Home-page: https://github.com/irods/python-irodsclient
 Author: iRODS Consortium
 Author-email: support@irods.org
 License: BSD
 Description: Python iRODS Client (PRC)
         =========================
@@ -165,14 +165,23 @@
         ```
         
         Note that the `irods_` prefix is unnecessary when providing
         the `encryption_*` and `ssl_*` options
         directly to the constructor as keyword arguments, even though it is
         required when they are placed in the environment file.
         
+        PAM logins
+        ----------
+        
+        Starting with v2.0.0, the python iRODS client is able to authenticate under PAM using the same file-based client environment as the
+        iCommands.
+        
+        Caveat for iRODS 4.3+: when upgrading from 4.2, the "irods_authentication_scheme" setting must be changed from "pam" to "pam_password" in
+        `~/.irods/irods_environment.json` for all file-based client environments.
+        
         Maintaining a connection
         ------------------------
         
         The default library timeout for a connection to an iRODS Server is 120
         seconds.
         
         This can be overridden by changing the session `connection_timeout` immediately after creation of the
```

### Comparing `python-irodsclient-2.0.0/python_irodsclient.egg-info/SOURCES.txt` & `python-irodsclient-2.0.1/python_irodsclient.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 irods/session.py
 irods/ticket.py
 irods/user.py
 irods/version.py
 irods/zone.py
 irods/auth/__init__.py
 irods/auth/native.py
+irods/auth/pam.py
 irods/auth/pam_password.py
 irods/client_configuration/__init__.py
 irods/manager/__init__.py
 irods/manager/access_manager.py
 irods/manager/collection_manager.py
 irods/manager/data_object_manager.py
 irods/manager/metadata_manager.py
```

### Comparing `python-irodsclient-2.0.0/setup.py` & `python-irodsclient-2.0.1/setup.py`

 * *Files identical despite different names*

