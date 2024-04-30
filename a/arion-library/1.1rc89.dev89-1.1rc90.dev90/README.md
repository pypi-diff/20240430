# Comparing `tmp/arion_library-1.1rc89.dev89.tar.gz` & `tmp/arion_library-1.1rc90.dev90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arion_library-1.1rc89.dev89.tar", last modified: Fri Apr 19 13:50:27 2024, max compression
+gzip compressed data, was "arion_library-1.1rc90.dev90.tar", last modified: Tue Apr 30 11:03:59 2024, max compression
```

## Comparing `arion_library-1.1rc89.dev89.tar` & `arion_library-1.1rc90.dev90.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.913797 arion_library-1.1rc89.dev89/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-19 13:50:27.913797 arion_library-1.1rc89.dev89/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.909797 arion_library-1.1rc89.dev89/arion_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-19 13:50:27.000000 arion_library-1.1rc89.dev89/arion_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-19 13:50:27.000000 arion_library-1.1rc89.dev89/arion_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:50:27.000000 arion_library-1.1rc89.dev89/arion_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-19 13:50:27.000000 arion_library-1.1rc89.dev89/arion_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 13:50:27.000000 arion_library-1.1rc89.dev89/arion_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.909797 arion_library-1.1rc89.dev89/processors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.909797 arion_library-1.1rc89.dev89/processors/Cegid_Web_Services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/Cegid_Web_Services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.909797 arion_library-1.1rc89.dev89/processors/Cegid_Web_Services/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/Cegid_Web_Services/lib/Convert_Soap_Rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/Cegid_Web_Services/lib/Handle_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/Cegid_Web_Services/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.909797 arion_library-1.1rc89.dev89/processors/Cegid_Web_Services/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/Cegid_Web_Services/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/Cegid_Web_Services/tests/test_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.909797 arion_library-1.1rc89.dev89/processors/FTP_connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/FTP_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.909797 arion_library-1.1rc89.dev89/processors/FTP_connector/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/FTP_connector/lib/FTPconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/FTP_connector/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.909797 arion_library-1.1rc89.dev89/processors/FTP_connector/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/FTP_connector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/FTP_connector/tests/test_ftp_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.909797 arion_library-1.1rc89.dev89/processors/OracleConnector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/OracleConnector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.909797 arion_library-1.1rc89.dev89/processors/OracleConnector/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/OracleConnector/lib/OracleDatabase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/OracleConnector/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.909797 arion_library-1.1rc89.dev89/processors/OracleConnector/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/OracleConnector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/OracleConnector/tests/test_oracle_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.909797 arion_library-1.1rc89.dev89/processors/SFTP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/SFTP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.913797 arion_library-1.1rc89.dev89/processors/SFTP/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/SFTP/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/SFTP/lib/sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.913797 arion_library-1.1rc89.dev89/processors/SFTP/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/SFTP/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/SFTP/tests/test_sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.913797 arion_library-1.1rc89.dev89/processors/Shopify_connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/Shopify_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.913797 arion_library-1.1rc89.dev89/processors/Shopify_connector/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/Shopify_connector/lib/ShopifyConnector.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/Shopify_connector/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6890 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/Shopify_connector/lib/shopifyConnect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.913797 arion_library-1.1rc89.dev89/processors/Shopify_connector/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/Shopify_connector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/Shopify_connector/tests/test_shopify_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.913797 arion_library-1.1rc89.dev89/processors/TableStorage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/TableStorage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.913797 arion_library-1.1rc89.dev89/processors/TableStorage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/TableStorage/lib/TableStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/TableStorage/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.913797 arion_library-1.1rc89.dev89/processors/TableStorage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/TableStorage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/TableStorage/tests/test_table_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.913797 arion_library-1.1rc89.dev89/processors/azure_blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/azure_blob_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.913797 arion_library-1.1rc89.dev89/processors/azure_blob_storage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/azure_blob_storage/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3101 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/azure_blob_storage/lib/azureBlobStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/azure_blob_storage/lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.913797 arion_library-1.1rc89.dev89/processors/azure_blob_storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/azure_blob_storage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/azure_blob_storage/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/azure_blob_storage/tests/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.913797 arion_library-1.1rc89.dev89/processors/msserversql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/msserversql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.913797 arion_library-1.1rc89.dev89/processors/msserversql/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/msserversql/lib/MsServerSQL.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/msserversql/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:50:27.913797 arion_library-1.1rc89.dev89/processors/msserversql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/msserversql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-19 13:49:38.000000 arion_library-1.1rc89.dev89/processors/msserversql/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:50:27.913797 arion_library-1.1rc89.dev89/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-19 13:50:26.000000 arion_library-1.1rc89.dev89/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.347254 arion_library-1.1rc90.dev90/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-30 11:03:59.347254 arion_library-1.1rc90.dev90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.343254 arion_library-1.1rc90.dev90/arion_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-30 11:03:59.000000 arion_library-1.1rc90.dev90/arion_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-30 11:03:59.000000 arion_library-1.1rc90.dev90/arion_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 11:03:59.000000 arion_library-1.1rc90.dev90/arion_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-30 11:03:59.000000 arion_library-1.1rc90.dev90/arion_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 11:03:59.000000 arion_library-1.1rc90.dev90/arion_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.343254 arion_library-1.1rc90.dev90/processors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.343254 arion_library-1.1rc90.dev90/processors/Cegid_Web_Services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/Cegid_Web_Services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.343254 arion_library-1.1rc90.dev90/processors/Cegid_Web_Services/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/Cegid_Web_Services/lib/Convert_Soap_Rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/Cegid_Web_Services/lib/Handle_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/Cegid_Web_Services/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.343254 arion_library-1.1rc90.dev90/processors/Cegid_Web_Services/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/Cegid_Web_Services/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/Cegid_Web_Services/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/Cegid_Web_Services/tests/test_methods_handle_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.343254 arion_library-1.1rc90.dev90/processors/FTP_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/FTP_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.343254 arion_library-1.1rc90.dev90/processors/FTP_connector/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/FTP_connector/lib/FTPconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/FTP_connector/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.343254 arion_library-1.1rc90.dev90/processors/FTP_connector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/FTP_connector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/FTP_connector/tests/test_ftp_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.343254 arion_library-1.1rc90.dev90/processors/OracleConnector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/OracleConnector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.343254 arion_library-1.1rc90.dev90/processors/OracleConnector/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/OracleConnector/lib/OracleDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/OracleConnector/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.343254 arion_library-1.1rc90.dev90/processors/OracleConnector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/OracleConnector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/OracleConnector/tests/test_oracle_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.343254 arion_library-1.1rc90.dev90/processors/SFTP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/SFTP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.343254 arion_library-1.1rc90.dev90/processors/SFTP/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/SFTP/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/SFTP/lib/sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.343254 arion_library-1.1rc90.dev90/processors/SFTP/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/SFTP/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/SFTP/tests/test_sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.343254 arion_library-1.1rc90.dev90/processors/Shopify_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/Shopify_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.347254 arion_library-1.1rc90.dev90/processors/Shopify_connector/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/Shopify_connector/lib/ShopifyConnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/Shopify_connector/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6890 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/Shopify_connector/lib/shopifyConnect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.347254 arion_library-1.1rc90.dev90/processors/Shopify_connector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/Shopify_connector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/Shopify_connector/tests/test_shopify_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.347254 arion_library-1.1rc90.dev90/processors/TableStorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/TableStorage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.347254 arion_library-1.1rc90.dev90/processors/TableStorage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/TableStorage/lib/TableStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/TableStorage/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.347254 arion_library-1.1rc90.dev90/processors/TableStorage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/TableStorage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/TableStorage/tests/test_table_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.347254 arion_library-1.1rc90.dev90/processors/azure_blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/azure_blob_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.347254 arion_library-1.1rc90.dev90/processors/azure_blob_storage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/azure_blob_storage/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3101 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/azure_blob_storage/lib/azureBlobStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/azure_blob_storage/lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.347254 arion_library-1.1rc90.dev90/processors/azure_blob_storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/azure_blob_storage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/azure_blob_storage/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/azure_blob_storage/tests/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.347254 arion_library-1.1rc90.dev90/processors/msserversql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/msserversql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.347254 arion_library-1.1rc90.dev90/processors/msserversql/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/msserversql/lib/MsServerSQL.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/msserversql/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:59.347254 arion_library-1.1rc90.dev90/processors/msserversql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/msserversql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-30 11:03:07.000000 arion_library-1.1rc90.dev90/processors/msserversql/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 11:03:59.347254 arion_library-1.1rc90.dev90/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-30 11:03:57.000000 arion_library-1.1rc90.dev90/setup.py
```

### Comparing `arion_library-1.1rc89.dev89/arion_library.egg-info/SOURCES.txt` & `arion_library-1.1rc90.dev90/arion_library.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 processors/__init__.py
 processors/Cegid_Web_Services/__init__.py
 processors/Cegid_Web_Services/lib/Convert_Soap_Rest.py
 processors/Cegid_Web_Services/lib/Handle_error_response.py
 processors/Cegid_Web_Services/lib/__init__.py
 processors/Cegid_Web_Services/tests/__init__.py
 processors/Cegid_Web_Services/tests/test_methods.py
+processors/Cegid_Web_Services/tests/test_methods_handle_errors.py
 processors/FTP_connector/__init__.py
 processors/FTP_connector/lib/FTPconnector.py
 processors/FTP_connector/lib/__init__.py
 processors/FTP_connector/tests/__init__.py
 processors/FTP_connector/tests/test_ftp_connector.py
 processors/OracleConnector/__init__.py
 processors/OracleConnector/lib/OracleDatabase.py
```

### Comparing `arion_library-1.1rc89.dev89/processors/Cegid_Web_Services/lib/Convert_Soap_Rest.py` & `arion_library-1.1rc90.dev90/processors/Cegid_Web_Services/lib/Convert_Soap_Rest.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc89.dev89/processors/Cegid_Web_Services/lib/Handle_error_response.py` & `arion_library-1.1rc90.dev90/processors/Cegid_Web_Services/lib/Handle_error_response.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc89.dev89/processors/Cegid_Web_Services/tests/test_methods.py` & `arion_library-1.1rc90.dev90/processors/Cegid_Web_Services/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc89.dev89/processors/FTP_connector/lib/FTPconnector.py` & `arion_library-1.1rc90.dev90/processors/FTP_connector/lib/FTPconnector.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc89.dev89/processors/OracleConnector/lib/OracleDatabase.py` & `arion_library-1.1rc90.dev90/processors/OracleConnector/lib/OracleDatabase.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc89.dev89/processors/OracleConnector/tests/test_oracle_connector.py` & `arion_library-1.1rc90.dev90/processors/OracleConnector/tests/test_oracle_connector.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc89.dev89/processors/SFTP/lib/sftp.py` & `arion_library-1.1rc90.dev90/processors/SFTP/lib/sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc89.dev89/processors/SFTP/tests/test_sftp.py` & `arion_library-1.1rc90.dev90/processors/SFTP/tests/test_sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc89.dev89/processors/Shopify_connector/lib/ShopifyConnector.py` & `arion_library-1.1rc90.dev90/processors/Shopify_connector/lib/ShopifyConnector.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc89.dev89/processors/Shopify_connector/lib/shopifyConnect.py` & `arion_library-1.1rc90.dev90/processors/Shopify_connector/lib/shopifyConnect.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc89.dev89/processors/TableStorage/lib/TableStorage.py` & `arion_library-1.1rc90.dev90/processors/TableStorage/lib/TableStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc89.dev89/processors/TableStorage/tests/test_table_storage.py` & `arion_library-1.1rc90.dev90/processors/TableStorage/tests/test_table_storage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc89.dev89/processors/azure_blob_storage/lib/azureBlobStorage.py` & `arion_library-1.1rc90.dev90/processors/azure_blob_storage/lib/azureBlobStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc89.dev89/processors/azure_blob_storage/lib/config.py` & `arion_library-1.1rc90.dev90/processors/azure_blob_storage/lib/config.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc89.dev89/processors/azure_blob_storage/tests/test_blob.py` & `arion_library-1.1rc90.dev90/processors/azure_blob_storage/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc89.dev89/processors/azure_blob_storage/tests/test_env.py` & `arion_library-1.1rc90.dev90/processors/azure_blob_storage/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc89.dev89/processors/msserversql/lib/MsServerSQL.py` & `arion_library-1.1rc90.dev90/processors/msserversql/lib/MsServerSQL.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc89.dev89/processors/msserversql/tests/test_methods.py` & `arion_library-1.1rc90.dev90/processors/msserversql/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc89.dev89/setup.py` & `arion_library-1.1rc90.dev90/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='arion_library',  # Replace with your package name
-    version='1.1rc89.dev89',  # Replace with your package version
+    version='1.1rc90.dev90',  # Replace with your package version
     author='Heni Nechi',  # Replace with your name
     author_email='h.nechi@arion-tech.com',  # Replace with your email
     url='https://github.com/Ariontech/ArionLibrary.git',  # Replace with your repository URL
     packages=find_packages(),  # Automatically find all packages
     python_requires='>=3.8',  # Specify Python version requirements
     install_requires=['pyodbc', 'pytest', 'pysftp==0.2.9', 'ShopifyAPI==12.5.0', 'requests==2.31.0', 'azure-core==1.29.6', 'azure-data-tables==12.5.0', 'azure-storage-blob==12.19.1', 'python-dotenv==1.0.1', 'pytest==8.1.1', 'pandas==2.0.3', 'pytest'],
 )
```

