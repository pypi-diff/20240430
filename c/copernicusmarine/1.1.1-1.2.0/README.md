# Comparing `tmp/copernicusmarine-1.1.1.tar.gz` & `tmp/copernicusmarine-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copernicusmarine-1.1.1.tar", max compression
+gzip compressed data, was "copernicusmarine-1.2.0.tar", max compression
```

## Comparing `copernicusmarine-1.1.1.tar` & `copernicusmarine-1.2.0.tar`

### file list

```diff
@@ -1,52 +1,51 @@
--rw-r--r--   0        0        0    13827 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/LICENSE.txt
--rw-r--r--   0        0        0    29145 2024-04-18 14:17:59.870855 copernicusmarine-1.1.1/README.md
--rw-r--r--   0        0        0      972 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/__init__.py
--rw-r--r--   0        0        0     1070 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/aioretry/LICENSE
--rw-r--r--   0        0        0      225 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/aioretry/__init__.py
--rw-r--r--   0        0        0     4152 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/aioretry/retry.py
--rw-r--r--   0        0        0       10 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/catalogue_parser/__init__.py
--rw-r--r--   0        0        0    28918 2024-04-17 11:09:20.414412 copernicusmarine-1.1.1/copernicusmarine/catalogue_parser/catalogue_parser.py
--rw-r--r--   0        0        0    11545 2024-04-18 14:17:59.870855 copernicusmarine-1.1.1/copernicusmarine/catalogue_parser/request_structure.py
--rw-r--r--   0        0        0       10 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/command_line_interface/__init__.py
--rw-r--r--   0        0        0      868 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/command_line_interface/copernicus_marine.py
--rw-r--r--   0        0        0     1766 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/command_line_interface/exception_handler.py
--rw-r--r--   0        0        0     3784 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/command_line_interface/group_describe.py
--rw-r--r--   0        0        0     9616 2024-04-18 14:17:59.870855 copernicusmarine-1.1.1/copernicusmarine/command_line_interface/group_get.py
--rw-r--r--   0        0        0     3033 2024-04-17 11:09:20.414412 copernicusmarine-1.1.1/copernicusmarine/command_line_interface/group_login.py
--rw-r--r--   0        0        0    12730 2024-04-17 11:09:20.418412 copernicusmarine-1.1.1/copernicusmarine/command_line_interface/group_subset.py
--rw-r--r--   0        0        0     2339 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/command_line_interface/utils.py
--rw-r--r--   0        0        0    13437 2024-04-17 11:09:20.418412 copernicusmarine-1.1.1/copernicusmarine/core_functions/credentials_utils.py
--rw-r--r--   0        0        0     4455 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/core_functions/custom_zarr_store.py
--rw-r--r--   0        0        0     2806 2024-04-02 15:26:12.686202 copernicusmarine-1.1.1/copernicusmarine/core_functions/deprecated.py
--rw-r--r--   0        0        0     2385 2024-04-02 15:26:12.686202 copernicusmarine-1.1.1/copernicusmarine/core_functions/deprecated_options.py
--rw-r--r--   0        0        0     2132 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/core_functions/describe.py
--rw-r--r--   0        0        0     1233 2024-04-17 11:09:20.418412 copernicusmarine-1.1.1/copernicusmarine/core_functions/environment_variables.py
--rw-r--r--   0        0        0      603 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/core_functions/exceptions.py
--rw-r--r--   0        0        0     7622 2024-04-18 14:17:59.870855 copernicusmarine-1.1.1/copernicusmarine/core_functions/get.py
--rw-r--r--   0        0        0     1606 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/core_functions/login.py
--rw-r--r--   0        0        0      460 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/core_functions/models.py
--rw-r--r--   0        0        0    19332 2024-04-18 13:58:11.735885 copernicusmarine-1.1.1/copernicusmarine/core_functions/services_utils.py
--rw-r--r--   0        0        0     2132 2024-04-17 11:09:20.418412 copernicusmarine-1.1.1/copernicusmarine/core_functions/sessions.py
--rw-r--r--   0        0        0     9735 2024-04-04 15:26:42.410893 copernicusmarine-1.1.1/copernicusmarine/core_functions/subset.py
--rw-r--r--   0        0        0     5614 2024-04-17 11:09:20.418412 copernicusmarine-1.1.1/copernicusmarine/core_functions/utils.py
--rw-r--r--   0        0        0     2683 2024-04-17 11:09:20.418412 copernicusmarine-1.1.1/copernicusmarine/core_functions/versions_verifier.py
--rw-r--r--   0        0        0     2484 2024-04-03 07:33:56.619712 copernicusmarine-1.1.1/copernicusmarine/download_functions/common_download.py
--rw-r--r--   0        0        0     8009 2024-04-03 07:33:56.619712 copernicusmarine-1.1.1/copernicusmarine/download_functions/download_arco_series.py
--rw-r--r--   0        0        0     1706 2024-03-28 15:56:56.847755 copernicusmarine-1.1.1/copernicusmarine/download_functions/download_get.py
--rw-r--r--   0        0        0    15349 2024-04-18 14:17:59.870855 copernicusmarine-1.1.1/copernicusmarine/download_functions/download_original_files.py
--rw-r--r--   0        0        0      918 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/download_functions/subset_parameters.py
--rw-r--r--   0        0        0    18583 2024-04-18 13:58:11.735885 copernicusmarine-1.1.1/copernicusmarine/download_functions/subset_xarray.py
--rw-r--r--   0        0        0     5567 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/download_functions/utils.py
--rw-r--r--   0        0        0      863 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/logging_conf.json
--rw-r--r--   0        0        0     1961 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/python_interface/describe.py
--rw-r--r--   0        0        0      447 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/python_interface/exception_handler.py
--rw-r--r--   0        0        0     5817 2024-04-18 14:17:59.870855 copernicusmarine-1.1.1/copernicusmarine/python_interface/get.py
--rw-r--r--   0        0        0     3545 2024-04-04 15:26:42.410893 copernicusmarine-1.1.1/copernicusmarine/python_interface/load_utils.py
--rw-r--r--   0        0        0      731 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/python_interface/login.py
--rw-r--r--   0        0        0     6469 2024-04-04 15:26:42.410893 copernicusmarine-1.1.1/copernicusmarine/python_interface/open_dataset.py
--rw-r--r--   0        0        0     6150 2024-04-04 15:26:42.410893 copernicusmarine-1.1.1/copernicusmarine/python_interface/read_dataframe.py
--rw-r--r--   0        0        0     6620 2024-04-03 07:33:56.619712 copernicusmarine-1.1.1/copernicusmarine/python_interface/subset.py
--rw-r--r--   0        0        0      348 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/python_interface/utils.py
--rw-r--r--   0        0        0      901 2024-04-18 14:17:59.870855 copernicusmarine-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    30966 1970-01-01 00:00:00.000000 copernicusmarine-1.1.1/setup.py
--rw-r--r--   0        0        0    30167 1970-01-01 00:00:00.000000 copernicusmarine-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    13827 2024-04-25 14:08:43.428008 copernicusmarine-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0    31604 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/README.md
+-rw-r--r--   0        0        0      972 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/__init__.py
+-rw-r--r--   0        0        0     1070 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/aioretry/LICENSE
+-rw-r--r--   0        0        0      225 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/aioretry/__init__.py
+-rw-r--r--   0        0        0     4152 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/aioretry/retry.py
+-rw-r--r--   0        0        0       10 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/catalogue_parser/__init__.py
+-rw-r--r--   0        0        0    32561 2024-04-26 11:29:37.955962 copernicusmarine-1.2.0/copernicusmarine/catalogue_parser/catalogue_parser.py
+-rw-r--r--   0        0        0    11593 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/catalogue_parser/request_structure.py
+-rw-r--r--   0        0        0       10 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/command_line_interface/__init__.py
+-rw-r--r--   0        0        0      868 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/command_line_interface/copernicus_marine.py
+-rw-r--r--   0        0        0     1766 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/command_line_interface/exception_handler.py
+-rw-r--r--   0        0        0     4043 2024-04-26 11:29:37.955962 copernicusmarine-1.2.0/copernicusmarine/command_line_interface/group_describe.py
+-rw-r--r--   0        0        0     9849 2024-04-29 15:45:50.086401 copernicusmarine-1.2.0/copernicusmarine/command_line_interface/group_get.py
+-rw-r--r--   0        0        0     3033 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/command_line_interface/group_login.py
+-rw-r--r--   0        0        0    12730 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/command_line_interface/group_subset.py
+-rw-r--r--   0        0        0     2339 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/command_line_interface/utils.py
+-rw-r--r--   0        0        0    13437 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/core_functions/credentials_utils.py
+-rw-r--r--   0        0        0     4455 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/core_functions/custom_zarr_store.py
+-rw-r--r--   0        0        0     2806 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/core_functions/deprecated.py
+-rw-r--r--   0        0        0     2385 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/core_functions/deprecated_options.py
+-rw-r--r--   0        0        0     2174 2024-04-26 11:29:37.955962 copernicusmarine-1.2.0/copernicusmarine/core_functions/describe.py
+-rw-r--r--   0        0        0     1233 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/core_functions/environment_variables.py
+-rw-r--r--   0        0        0      603 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/core_functions/exceptions.py
+-rw-r--r--   0        0        0     8123 2024-04-26 11:40:58.688916 copernicusmarine-1.2.0/copernicusmarine/core_functions/get.py
+-rw-r--r--   0        0        0     1606 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/core_functions/login.py
+-rw-r--r--   0        0        0      460 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/core_functions/models.py
+-rw-r--r--   0        0        0    19873 2024-04-26 11:29:37.955962 copernicusmarine-1.2.0/copernicusmarine/core_functions/services_utils.py
+-rw-r--r--   0        0        0     2132 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/core_functions/sessions.py
+-rw-r--r--   0        0        0     9735 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/core_functions/subset.py
+-rw-r--r--   0        0        0     5941 2024-04-26 12:57:34.844935 copernicusmarine-1.2.0/copernicusmarine/core_functions/utils.py
+-rw-r--r--   0        0        0     2683 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/core_functions/versions_verifier.py
+-rw-r--r--   0        0        0     2484 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/download_functions/common_download.py
+-rw-r--r--   0        0        0     8027 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/download_functions/download_arco_series.py
+-rw-r--r--   0        0        0     1706 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/download_functions/download_get.py
+-rw-r--r--   0        0        0    21043 2024-04-26 11:29:37.955962 copernicusmarine-1.2.0/copernicusmarine/download_functions/download_original_files.py
+-rw-r--r--   0        0        0      918 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/download_functions/subset_parameters.py
+-rw-r--r--   0        0        0    19923 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/download_functions/subset_xarray.py
+-rw-r--r--   0        0        0     5634 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/download_functions/utils.py
+-rw-r--r--   0        0        0      863 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/logging_conf.json
+-rw-r--r--   0        0        0     2143 2024-04-26 11:29:37.955962 copernicusmarine-1.2.0/copernicusmarine/python_interface/describe.py
+-rw-r--r--   0        0        0      447 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/python_interface/exception_handler.py
+-rw-r--r--   0        0        0     5817 2024-04-26 11:01:14.733988 copernicusmarine-1.2.0/copernicusmarine/python_interface/get.py
+-rw-r--r--   0        0        0     3545 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/python_interface/load_utils.py
+-rw-r--r--   0        0        0     1464 2024-04-29 15:37:26.070685 copernicusmarine-1.2.0/copernicusmarine/python_interface/login.py
+-rw-r--r--   0        0        0     6469 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/python_interface/open_dataset.py
+-rw-r--r--   0        0        0     6150 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/python_interface/read_dataframe.py
+-rw-r--r--   0        0        0     6620 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/python_interface/subset.py
+-rw-r--r--   0        0        0      348 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/python_interface/utils.py
+-rw-r--r--   0        0        0      901 2024-04-30 12:32:31.692464 copernicusmarine-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    32677 1970-01-01 00:00:00.000000 copernicusmarine-1.2.0/PKG-INFO
```

### Comparing `copernicusmarine-1.1.1/LICENSE.txt` & `copernicusmarine-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/README.md` & `copernicusmarine-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 And to **upgrade the package** to the newest available version, run:
 ```bash
 python -m pip install copernicusmarine --upgrade
 ```
 
 ## User Guide
-For more comprehensive details on how to use the `copernicusmarine` Toolbox, please refer to our [Help Center](https://help.marine.copernicus.eu/en/collections/9054839-copernicus-marine-toolbox-guide). It ensures a smooth migration for existing users of legacy services such as MOTU, OPeNDAP or FTP.
+For more comprehensive details on how to use the `copernicusmarine` Toolbox, please refer to our [Help Center](https://help.marine.copernicus.eu/en/collections/9080063-copernicus-marine-toolbox). It ensures a smooth migration for existing users of legacy services such as MOTU, OPeNDAP or FTP.
 
 ### General configuration
 
 #### Cache Usage
 Cachier library is used for caching part of the requests (as result of `describe` or `login`). By default, the cache will be located in the home folder. If you need to change the location of the cache, you can set the environment variable `COPERNICUSMARINE_CACHE_DIRECTORY` to point to the desired directory:
 - on **UNIX** platforms: `export COPERNICUSMARINE_CACHE_DIRECTORY=<PATH>`
 - on **Windows** platforms: `set COPERNICUSMARINE_CACHE_DIRECTORY=<PATH>`
@@ -82,14 +82,20 @@
 #### Proxy
 
 To use proxies, as describe in the [aiohttp documentation](https://docs.aiohttp.org/en/stable/client_advanced.html#proxy-support) you can use two options:
 
 - set the `HTTPS_PROXY` variable. For eg: `HTTPS_PROXY="http://user:pass@some.proxy.com"`. It should work even with `COPERNICUSMARINE_TRUST_ENV=False`.
 - use a `.netrc` file but be aware that having a line: "default login anonymous password user@site" is incompatible with S3 connection required by the toolbox. Also note that if you have `COPERNICUSMARINE_TRUST_ENV=True` (the default value) then if `NETRC` environment variable is set with a specified location, the `.netrc` file will be read from the specified location there rather than from `~/.netrc`.
 
+#### Number of concurrent requests
+
+The toolbox makes many requests to STAC to be able to parse the full marine data store STAC catalog. For that, it uses asynchronous calls. It can be problematic to do too many requests at the same time. To limit the number of requests at the same time you can use: `COPERNICUSMARINE_MAX_CONCURRENT_REQUESTS`. The default value is `15` and minimum value is `1`.
+
+Note, that this concerns only the catalog parsing step so the describe command and the start of the get and subset command. It does not apply when downloading files or listing files from the get command or when requesting the data chunks for the subset command.
+
 ## Command Line Interface (CLI)
 
 ### The `--help` option
 To discover commands and their available options, consider appending `--help` on any command line.
 
 Example:
 ```bash
@@ -307,30 +313,58 @@
 s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB - 2023-11-12T23:47:13Z
 s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB - 2023-11-12T23:47:13Z
 
 Total size of the download: 26.59 MB
 Do you want to proceed with download? [Y/n]:
 ```
 
+#### Notes about the file list option
+
 Option `--file-list` allows to specify a list of files for more advanced files selection.
 The file can contain complete absolute paths for each target file (default behavior) or only a partial path defined by the user, as shown below.
 
+By default, the get functionality lists all the files on the bucket to be able to select the requested ones. This create some overhead when there are a lot of files for a specific dataset. For example, a dataset with more than 100 000 files would create an overhead of around two minutes. The file list option will directly download the files and avoid the listings if all the files listed are found.
+
+Careful, a path can easily be mispelled or wrongly queried. The toolbox will display a warning if the file is not found on the bucket and try to find the file by listing all the files on the bucket.
+
+Example of `file_list.txt` with paths that would be directly downloaded without the listing overhead:
+
+```txt
+# correct paths
+> s3://mdl-native-01/native/INSITU_GLO_PHYBGCWAV_DISCRETE_MYNRT_013_030/cmems_obs-ins_glo_phybgcwav_mynrt_na_irr_202311/history/BO/AR_PR_BO_58JM.nc
+> INSITU_GLO_PHYBGCWAV_DISCRETE_MYNRT_013_030/cmems_obs-ins_glo_phybgcwav_mynrt_na_irr_202311/history/BO/AR_PR_BO_58JM.nc
+> cmems_obs-ins_glo_phybgcwav_mynrt_na_irr_202311/history/BO/AR_PR_BO_58JM.nc
+> history/BO/AR_PR_BO_58JM.nc
+> index_history.txt
+
+# incorrect paths
+# version is missing
+> INSITU_GLO_PHYBGCWAV_DISCRETE_MYNRT_013_030/cmems_obs-ins_glo_phybgcwav_mynrt_na_irr/history/BO/AR_PR_BO_58JM.nc
+# only the file name and not the path to the file
+> AR_PR_BO_58JM.nc
+# not the same dataset
+> another_dataset/history/BO/AR_PR_BO_58JM.nc
+```
+
 Example of `file_list.txt` with absolute paths:
+
 ```txt
 s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210101_20210131_R20230101_RE01.nc
 s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210201_20210228_R20230101_RE01.nc
 s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210301_20210331_R20230101_RE01.nc
 ```
 
 Example of `file_list.txt` with partial paths matching the absolute paths (equivalent to previous example):
+
 ```txt
 CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc
 CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc
 CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc
 ```
+
 > **_NOTE:_** This option is compatible with the file generated by the `--create-file-list` option if you generated a ".txt" file.
 
 Then the following command:
 ```bash
 copernicusmarine get -i cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --file-list file_list.txt
 ```
 Returns:
@@ -369,17 +403,19 @@
 s3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_platform.txt - 209.27 kB - 2024-04-03T08:33:37Z
 
 Total size of the download: 2.52 MB
 Do you want to proceed with download? [Y/n]:
 ```
 
 ### Shared options
+
 Both `subset` and `get` commands provide these options:
 
 #### Option `--overwrite-output-data`
+
 When specified, the existing files will be overwritten.
 Otherwise, if the files already exist on destination, new ones with a unique index will be created once the download has been accepted (or once `--force-download` is provided).
 
 #### Option `--create-template`
 Option to create a file in your current directory containing request parameters. If specified, no other action will be performed.
 It will create the following files depending on the feature:
 - `subset`
@@ -459,18 +495,24 @@
 You can use the `--dataset-part` option to fecth a specific part for the chosen dataset version.
 
 #### Option `--log-level`
 Set the details printed to console by the command (based on standard logging library).
 Available values are: `[DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]`
 
 ## Python package (API)
-The `copernicusmarine` exposes a Python interface to allow you to [call commands as functions](https://marine.copernicus.eu/python-interface).
+The `copernicusmarine` exposes a Python interface to allow you to [call commands as functions](https://help.marine.copernicus.eu/en/collections/9054839-main-functionalities).
 
 ## Documentation
-A detailed standalone API documentation is under construction and will come at a later stage. For the moment, see the [Help Center](https://help.marine.copernicus.eu/en/collections/9054839-copernicus-marine-toolbox-guide).
+A detailed standalone API documentation is under construction and will come at a later stage. For the moment, see the [Help Center](https://help.marine.copernicus.eu/en/collections/9080063-copernicus-marine-toolbox).
+
+## Version management
+We are using semantic versioning X.Y.Z → for example 1.0.2
+- Z is bumped on minor non-breaking changes.
+- Y is bumped on breaking changes.
+- X is bumped on demand to highlight a new significant feature or for communication purposes (new Copernicus Marine Service release for example).
 
 ## Contribution
 We welcome contributions from the community to enhance this package. If you find any issues or have suggestions for improvements, please check out our [Report Template](https://help.marine.copernicus.eu/en/articles/8218546-reporting-an-issue-or-feature-request).
 
 ## Future improvements & Roadmap
 To keep up to date with the most recent and planned advancements, including revisions, corrections, and feature requests generated from users' feedback, please refer to our [Roadmap](https://help.marine.copernicus.eu/en/articles/8218641-next-milestones-and-roadmap).
```

#### html2text {}

```diff
@@ -25,16 +25,16 @@
 copernicusmarine/copernicusmarine --version ``` ### Pip Otherwise, if you
 already have an environment (safer to clone it), the package can be installed
 using the `pip` command: ```bash python -m pip install copernicusmarine ``` And
 to **upgrade the package** to the newest available version, run: ```bash python
 -m pip install copernicusmarine --upgrade ``` ## User Guide For more
 comprehensive details on how to use the `copernicusmarine` Toolbox, please
 refer to our [Help Center](https://help.marine.copernicus.eu/en/collections/
-9054839-copernicus-marine-toolbox-guide). It ensures a smooth migration for
-existing users of legacy services such as MOTU, OPeNDAP or FTP. ### General
+9080063-copernicus-marine-toolbox). It ensures a smooth migration for existing
+users of legacy services such as MOTU, OPeNDAP or FTP. ### General
 configuration #### Cache Usage Cachier library is used for caching part of the
 requests (as result of `describe` or `login`). By default, the cache will be
 located in the home folder. If you need to change the location of the cache,
 you can set the environment variable `COPERNICUSMARINE_CACHE_DIRECTORY` to
 point to the desired directory: - on **UNIX** platforms: `export
 COPERNICUSMARINE_CACHE_DIRECTORY=` - on **Windows** platforms: `set
 COPERNICUSMARINE_CACHE_DIRECTORY=` ### Network configuration #### Disable SSL A
@@ -57,32 +57,40 @@
 options: - set the `HTTPS_PROXY` variable. For eg: `HTTPS_PROXY="http://user:
 pass@some.proxy.com"`. It should work even with
 `COPERNICUSMARINE_TRUST_ENV=False`. - use a `.netrc` file but be aware that
 having a line: "default login anonymous password user@site" is incompatible
 with S3 connection required by the toolbox. Also note that if you have
 `COPERNICUSMARINE_TRUST_ENV=True` (the default value) then if `NETRC`
 environment variable is set with a specified location, the `.netrc` file will
-be read from the specified location there rather than from `~/.netrc`. ##
-Command Line Interface (CLI) ### The `--help` option To discover commands and
-their available options, consider appending `--help` on any command line.
-Example: ```bash copernicusmarine --help ``` Returns: ```bash Usage:
-copernicusmarine [OPTIONS] COMMAND [ARGS]... Options: -V, --version Show the
-version and exit. -h, --help Show this message and exit. Commands: describe
-Print Copernicus Marine catalog as JSON. get Download originally produced data
-files. login Create a configuration file with your Copernicus Marine
-credentials. subset Download subsets of datasets as NetCDF files or Zarr
-stores. ``` ### Command `describe` Retrieve metadata information about all
-products/datasets and display as JSON output: ```bash copernicusmarine describe
---include-datasets ``` The JSON output can also be saved as follows: ```bash
-copernicusmarine describe --include-datasets >
-all_datasets_copernicusmarine.json ``` ### Command `login` Create a single
-configuration file `.copernicusmarine-credentials` allowing to access all
-Copernicus Marine Data Store data services. By default, the file is saved in
-user's home directory. Example: ```bash > copernicusmarine login username :
-johndoe password : INFO - Configuration files stored in /Users/
+be read from the specified location there rather than from `~/.netrc`. ####
+Number of concurrent requests The toolbox makes many requests to STAC to be
+able to parse the full marine data store STAC catalog. For that, it uses
+asynchronous calls. It can be problematic to do too many requests at the same
+time. To limit the number of requests at the same time you can use:
+`COPERNICUSMARINE_MAX_CONCURRENT_REQUESTS`. The default value is `15` and
+minimum value is `1`. Note, that this concerns only the catalog parsing step so
+the describe command and the start of the get and subset command. It does not
+apply when downloading files or listing files from the get command or when
+requesting the data chunks for the subset command. ## Command Line Interface
+(CLI) ### The `--help` option To discover commands and their available options,
+consider appending `--help` on any command line. Example: ```bash
+copernicusmarine --help ``` Returns: ```bash Usage: copernicusmarine [OPTIONS]
+COMMAND [ARGS]... Options: -V, --version Show the version and exit. -h, --help
+Show this message and exit. Commands: describe Print Copernicus Marine catalog
+as JSON. get Download originally produced data files. login Create a
+configuration file with your Copernicus Marine credentials. subset Download
+subsets of datasets as NetCDF files or Zarr stores. ``` ### Command `describe`
+Retrieve metadata information about all products/datasets and display as JSON
+output: ```bash copernicusmarine describe --include-datasets ``` The JSON
+output can also be saved as follows: ```bash copernicusmarine describe --
+include-datasets > all_datasets_copernicusmarine.json ``` ### Command `login`
+Create a single configuration file `.copernicusmarine-credentials` allowing to
+access all Copernicus Marine Data Store data services. By default, the file is
+saved in user's home directory. Example: ```bash > copernicusmarine login
+username : johndoe password : INFO - Configuration files stored in /Users/
 foo/.copernicusmarine ``` If `.copernicusmarine-credentials` already exists,
 the user is asked for confirmation to overwrite (`--overwrite`/`--overwrite-
 configuration-file`). You can use the `--skip-if-user-logged-in` option to skip
 the configuration file overwrite if the user is already logged in. #### Access
 points migration and evolution If you still have a configuration for legacy
 services (e.g. `~/motuclient/motuclient-python.ini`, `~/.netrc` or `~/_netrc`)
 in your home directory, it will automatically be taken into account with
@@ -254,19 +262,39 @@
 2023-11-12T23:47:13Z s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
 cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/
 CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB -
 2023-11-12T23:47:13Z s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
 cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/
 CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB -
 2023-11-12T23:47:13Z Total size of the download: 26.59 MB Do you want to
-proceed with download? [Y/n]: ``` Option `--file-list` allows to specify a list
-of files for more advanced files selection. The file can contain complete
-absolute paths for each target file (default behavior) or only a partial path
-defined by the user, as shown below. Example of `file_list.txt` with absolute
-paths: ```txt s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
+proceed with download? [Y/n]: ``` #### Notes about the file list option Option
+`--file-list` allows to specify a list of files for more advanced files
+selection. The file can contain complete absolute paths for each target file
+(default behavior) or only a partial path defined by the user, as shown below.
+By default, the get functionality lists all the files on the bucket to be able
+to select the requested ones. This create some overhead when there are a lot of
+files for a specific dataset. For example, a dataset with more than 100 000
+files would create an overhead of around two minutes. The file list option will
+directly download the files and avoid the listings if all the files listed are
+found. Careful, a path can easily be mispelled or wrongly queried. The toolbox
+will display a warning if the file is not found on the bucket and try to find
+the file by listing all the files on the bucket. Example of `file_list.txt`
+with paths that would be directly downloaded without the listing overhead:
+```txt # correct paths > s3://mdl-native-01/native/
+INSITU_GLO_PHYBGCWAV_DISCRETE_MYNRT_013_030/cmems_obs-
+ins_glo_phybgcwav_mynrt_na_irr_202311/history/BO/AR_PR_BO_58JM.nc >
+INSITU_GLO_PHYBGCWAV_DISCRETE_MYNRT_013_030/cmems_obs-
+ins_glo_phybgcwav_mynrt_na_irr_202311/history/BO/AR_PR_BO_58JM.nc > cmems_obs-
+ins_glo_phybgcwav_mynrt_na_irr_202311/history/BO/AR_PR_BO_58JM.nc > history/BO/
+AR_PR_BO_58JM.nc > index_history.txt # incorrect paths # version is missing >
+INSITU_GLO_PHYBGCWAV_DISCRETE_MYNRT_013_030/cmems_obs-
+ins_glo_phybgcwav_mynrt_na_irr/history/BO/AR_PR_BO_58JM.nc # only the file name
+and not the path to the file > AR_PR_BO_58JM.nc # not the same dataset >
+another_dataset/history/BO/AR_PR_BO_58JM.nc ``` Example of `file_list.txt` with
+absolute paths: ```txt s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
 cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/
 CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210101_20210131_R20230101_RE01.nc s3://mdl-
 native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-
 3D_P1M-m_202012/2021/
 CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210201_20210228_R20230101_RE01.nc s3://mdl-
 native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-
 3D_P1M-m_202012/2021/
@@ -362,28 +390,33 @@
 useful to keep an operational chain working when an evolution impact the chosen
 dataset. #### Option `--dataset-part` You can use the `--dataset-part` option
 to fecth a specific part for the chosen dataset version. #### Option `--log-
 level` Set the details printed to console by the command (based on standard
 logging library). Available values are: `
 [DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]` ## Python package (API) The
 `copernicusmarine` exposes a Python interface to allow you to [call commands as
-functions](https://marine.copernicus.eu/python-interface). ## Documentation A
-detailed standalone API documentation is under construction and will come at a
-later stage. For the moment, see the [Help Center](https://
-help.marine.copernicus.eu/en/collections/9054839-copernicus-marine-toolbox-
-guide). ## Contribution We welcome contributions from the community to enhance
-this package. If you find any issues or have suggestions for improvements,
-please check out our [Report Template](https://help.marine.copernicus.eu/en/
-articles/8218546-reporting-an-issue-or-feature-request). ## Future improvements
-& Roadmap To keep up to date with the most recent and planned advancements,
-including revisions, corrections, and feature requests generated from users'
-feedback, please refer to our [Roadmap](https://help.marine.copernicus.eu/en/
-articles/8218641-next-milestones-and-roadmap). ## Join the community Get in
-touch! - Create your [Copernicus Marine Account](https://
-data.marine.copernicus.eu/register?redirect=%2Fproducts) - [Log in](https://
-data.marine.copernicus.eu/login?redirect=%2Fproducts) and chat with us (bottom
-right corner of [Copernicus Marine Service](https://marine.copernicus.eu/)) -
-Join our [training workshops](https://marine.copernicus.eu/services/user-
-learning-services) - Network y/our [Copernicus Stories](https://twitter.com/
-cmems_eu) - Watch [our videos](https://www.youtube.com/channel/
-UC71ceOVy7WtVC7F04BKoEew) ## Licence Licensed under the [EUPL](https://
-joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12)
+functions](https://help.marine.copernicus.eu/en/collections/9054839-main-
+functionalities). ## Documentation A detailed standalone API documentation is
+under construction and will come at a later stage. For the moment, see the
+[Help Center](https://help.marine.copernicus.eu/en/collections/9080063-
+copernicus-marine-toolbox). ## Version management We are using semantic
+versioning X.Y.Z â for example 1.0.2 - Z is bumped on minor non-breaking
+changes. - Y is bumped on breaking changes. - X is bumped on demand to
+highlight a new significant feature or for communication purposes (new
+Copernicus Marine Service release for example). ## Contribution We welcome
+contributions from the community to enhance this package. If you find any
+issues or have suggestions for improvements, please check out our [Report
+Template](https://help.marine.copernicus.eu/en/articles/8218546-reporting-an-
+issue-or-feature-request). ## Future improvements & Roadmap To keep up to date
+with the most recent and planned advancements, including revisions,
+corrections, and feature requests generated from users' feedback, please refer
+to our [Roadmap](https://help.marine.copernicus.eu/en/articles/8218641-next-
+milestones-and-roadmap). ## Join the community Get in touch! - Create your
+[Copernicus Marine Account](https://data.marine.copernicus.eu/
+register?redirect=%2Fproducts) - [Log in](https://data.marine.copernicus.eu/
+login?redirect=%2Fproducts) and chat with us (bottom right corner of
+[Copernicus Marine Service](https://marine.copernicus.eu/)) - Join our
+[training workshops](https://marine.copernicus.eu/services/user-learning-
+services) - Network y/our [Copernicus Stories](https://twitter.com/cmems_eu) -
+Watch [our videos](https://www.youtube.com/channel/UC71ceOVy7WtVC7F04BKoEew) ##
+Licence Licensed under the [EUPL](https://joinup.ec.europa.eu/collection/eupl/
+eupl-text-eupl-12)
```

### Comparing `copernicusmarine-1.1.1/copernicusmarine/__init__.py` & `copernicusmarine-1.2.0/copernicusmarine/__init__.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/aioretry/LICENSE` & `copernicusmarine-1.2.0/copernicusmarine/aioretry/LICENSE`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/aioretry/retry.py` & `copernicusmarine-1.2.0/copernicusmarine/aioretry/retry.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/catalogue_parser/catalogue_parser.py` & `copernicusmarine-1.2.0/copernicusmarine/catalogue_parser/catalogue_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,14 +176,15 @@
 
 
 @dataclass
 class CopernicusMarineVersionPart:
     name: str
     services: list[CopernicusMarineService]
     retired_date: Optional[str]
+    released_date: Optional[str]
 
     def get_service_by_service_type(
         self, service_type: CopernicusMarineDatasetServiceType
     ):
         return next(
             service
             for service in self.services
@@ -193,26 +194,53 @@
 
 @dataclass
 class CopernicusMarineDatasetVersion:
     label: str
     parts: list[CopernicusMarineVersionPart]
 
     def get_part(
-        self, force_part: Optional[str] = None
+        self, force_part: Optional[str]
     ) -> CopernicusMarineVersionPart:
         wanted_part = force_part or PART_DEFAULT
         for part in self.parts:
             if part.name == wanted_part:
                 return part
             elif not force_part:
-                # TODO: If a dataset version has a non default part,
-                # then return the first one for the moment
                 return part
         raise dataset_version_part_not_found_exception(self)
 
+    def sort_parts(self) -> tuple[Optional[str], Optional[str]]:
+        not_released_parts = {
+            part.name
+            for part in self.parts
+            if part.released_date
+            and datetime_parser(part.released_date) > datetime_parser("now")
+        }
+        will_be_retired_parts = {
+            part.name: datetime_parser(part.retired_date).timestamp()
+            for part in self.parts
+            if part.retired_date
+        }
+        max_retired_timestamp = 0
+        if will_be_retired_parts:
+            max_retired_timestamp = max(will_be_retired_parts.values()) + 1
+        self.parts = sorted(
+            self.parts,
+            key=lambda x: (
+                x.name in not_released_parts,
+                max_retired_timestamp
+                - will_be_retired_parts.get(x.name, max_retired_timestamp),
+                -(x.name == PART_DEFAULT),
+                -(x.name == "latest"),  # for INSITU datasets
+                -(x.name == "bathy"),  # for STATIC datasets
+                x.name,
+            ),
+        )
+        return self.parts[0].released_date, self.parts[0].retired_date
+
 
 class DatasetVersionPartNotFound(Exception):
     ...
 
 
 class DatasetVersionNotFound(Exception):
     ...
@@ -244,19 +272,47 @@
         sorted_versions = sorted(versions, key=lambda x: x.label)
         if sorted_versions:
             return sorted_versions[-1]
         if default_version:
             return default_version
         raise dataset_version_not_found_exception(self)
 
-    def get_latest_version(self) -> Optional[CopernicusMarineDatasetVersion]:
-        try:
-            return self.get_latest_version_or_raise()
-        except DatasetVersionNotFound:
-            return None
+    def get_version(
+        self, force_version: Optional[str]
+    ) -> CopernicusMarineDatasetVersion:
+        wanted_version = force_version or VERSION_DEFAULT
+        for version in self.versions:
+            if version.label == wanted_version:
+                return version
+            elif not force_version:
+                return version
+        raise dataset_version_not_found_exception(self)
+
+    def sort_versions(self) -> None:
+        not_released_versions: set[str] = set()
+        retired_dates = {}
+        for version in self.versions:
+            released_date, retired_date = version.sort_parts()
+            if released_date and datetime_parser(
+                released_date
+            ) > datetime_parser("now"):
+                not_released_versions.add(version.label)
+            if retired_date:
+                retired_dates[version.label] = retired_date
+
+        self.versions = sorted(
+            self.versions,
+            key=lambda x: (
+                -(x.label in not_released_versions),
+                retired_dates.get(x.label, "9999-12-31"),
+                -(x.label == VERSION_DEFAULT),
+                x.label,
+            ),
+            reverse=True,
+        )
 
 
 def dataset_version_part_not_found_exception(
     version: CopernicusMarineDatasetVersion,
 ) -> DatasetVersionPartNotFound:
     return DatasetVersionPartNotFound(
         f"No part found for version {version.label}"
@@ -318,19 +374,21 @@
     production_center: str
     keywords: dict[str, str]
 
 
 @dataclass
 class ProductDatasetFromMarineDataStore(ProductDatasetParser):
     def to_copernicus_marine_dataset(self) -> CopernicusMarineProductDataset:
-        return CopernicusMarineProductDataset(
+        dataset = CopernicusMarineProductDataset(
             dataset_id=self.dataset_id,
             dataset_name=self.dataset_name,
             versions=self.versions,
         )
+        dataset.sort_versions()
+        return dataset
 
 
 @dataclass
 class ProductFromMarineDataStore(ProductParser):
     datasets: list[ProductDatasetFromMarineDataStore]
 
     def to_copernicus_marine_product(self) -> CopernicusMarineProduct:
@@ -354,14 +412,39 @@
 @dataclass
 class CopernicusMarineCatalogue:
     products: list[CopernicusMarineProduct]
 
     def filter(self, tokens: list[str]):
         return filter_catalogue_with_strings(self, tokens)
 
+    def filter_only_official_versions_and_parts(self):
+        products_to_remove = []
+        for product in self.products:
+            datasets_to_remove = []
+            for dataset in product.datasets:
+                latest_version = dataset.versions[0]
+                parts_to_remove = []
+                for part in latest_version.parts:
+                    if part.released_date and datetime_parser(
+                        part.released_date
+                    ) > datetime_parser("now"):
+                        parts_to_remove.append(part)
+                for part_to_remove in parts_to_remove:
+                    latest_version.parts.remove(part_to_remove)
+                if not latest_version.parts:
+                    datasets_to_remove.append(dataset)
+                else:
+                    dataset.versions = [latest_version]
+            for dataset_to_remove in datasets_to_remove:
+                product.datasets.remove(dataset_to_remove)
+            if not product.datasets:
+                products_to_remove.append(product)
+        for product_to_remove in products_to_remove:
+            self.products.remove(product_to_remove)
+
 
 class CatalogParserConnection:
     def __init__(self, proxy: Optional[str] = None) -> None:
         self.proxy = proxy
         self.session = get_configured_aiohttp_session()
         self.proxy = get_https_proxy()
         self.__max_retries = 5
@@ -438,28 +521,29 @@
             datacube.id
         )[1],
     )
     for dataset_version, datacubes in datacubes_by_version:  # type: ignore
         parts = _get_parts(datacubes)
 
         if parts:
-            copernicus_marine_dataset_versions.append(
-                CopernicusMarineDatasetVersion(
-                    label=dataset_version, parts=parts
-                )
+            version = CopernicusMarineDatasetVersion(
+                label=dataset_version,
+                parts=parts,
             )
+            copernicus_marine_dataset_versions.append(version)
+
     return copernicus_marine_dataset_versions
 
 
 def _get_parts(
     datacubes: List[pystac.Item],
 ) -> List[CopernicusMarineVersionPart]:
     parts: List[CopernicusMarineVersionPart] = []
-
     for datacube in datacubes:
+        released_date = datacube.properties.get("admp_released_date")
         retired_date = datacube.properties.get("admp_retired_date")
         if retired_date and datetime_parser(retired_date) < datetime_parser(
             "now"
         ):
             continue
 
         services = _get_services(datacube)
@@ -467,14 +551,15 @@
 
         if services:
             parts.append(
                 CopernicusMarineVersionPart(
                     name=part,
                     services=_get_services(datacube),
                     retired_date=retired_date,
+                    released_date=released_date,
                 )
             )
 
     if parts:
         return parts
     return []
 
@@ -773,15 +858,21 @@
     try:
         catalog = _parse_catalogue(
             ignore_cache=no_metadata_cache,
             _versions=package_version("copernicusmarine"),
             disable_progress_bar=disable_progress_bar,
             staging=staging,
         )
-    except ValueError:
+    except ValueError as e:
+        logger.debug(f"Error while parsing catalogue: {e}")
+        logger.debug(
+            "Now retrying without cache. If the problem with "
+            "the cache persists, try running "
+            "copernicusmarine describe --overwrite-metadata-cache"
+        )
         catalog = _parse_catalogue(
             ignore_cache=True,
             _versions=package_version("copernicusmarine"),
             disable_progress_bar=disable_progress_bar,
             staging=staging,
         )
     logger.debug("Catalogue parsed")
```

### Comparing `copernicusmarine-1.1.1/copernicusmarine/catalogue_parser/request_structure.py` & `copernicusmarine-1.2.0/copernicusmarine/catalogue_parser/request_structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,14 +210,15 @@
     force_service: Optional[str] = None
     filter: Optional[str] = None
     regex: Optional[str] = None
     file_list: Optional[pathlib.Path] = None
     sync: bool = False
     sync_delete: bool = False
     index_parts: bool = False
+    direct_download: Optional[list[str]] = None
 
     def update(self, new_dict: dict):
         """Method to update values in GetRequest object.
         Skips "None" values
         """
         for key, value in new_dict.items():
             if value is None:
```

### Comparing `copernicusmarine-1.1.1/copernicusmarine/command_line_interface/copernicus_marine.py` & `copernicusmarine-1.2.0/copernicusmarine/command_line_interface/copernicus_marine.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/command_line_interface/exception_handler.py` & `copernicusmarine-1.2.0/copernicusmarine/command_line_interface/exception_handler.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/command_line_interface/group_describe.py` & `copernicusmarine-1.2.0/copernicusmarine/command_line_interface/group_describe.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,14 +62,21 @@
     "--include-keywords",
     type=bool,
     is_flag=True,
     default=False,
     help="Include product keyword details in output.",
 )
 @click.option(
+    "--include-all-versions",
+    type=bool,
+    is_flag=True,
+    default=False,
+    help="Whether to include all versions of each item. Defaults to False.",
+)
+@click.option(
     "--contains",
     "-c",
     type=str,
     multiple=True,
     help="Filter catalogue output. Returns products with attributes "
     "matching a string token.",
 )
@@ -109,14 +116,15 @@
     hidden=True,
 )
 @log_exception_and_exit
 def describe(
     include_description: bool,
     include_datasets: bool,
     include_keywords: bool,
+    include_all_versions: bool,
     contains: list[str],
     overwrite_metadata_cache: bool,
     no_metadata_cache: bool,
     disable_progress_bar: bool,
     log_level: str,
     staging: bool,
 ) -> None:
@@ -129,14 +137,15 @@
     if logger.isEnabledFor(logging.DEBUG):
         logger.debug("DEBUG mode activated")
 
     json_dump = describe_function(
         include_description=include_description,
         include_datasets=include_datasets,
         include_keywords=include_keywords,
+        include_all_versions=include_all_versions,
         contains=contains,
         overwrite_metadata_cache=overwrite_metadata_cache,
         no_metadata_cache=no_metadata_cache,
         disable_progress_bar=disable_progress_bar,
         staging=staging,
     )
     blank_logger.info(json_dump)
```

### Comparing `copernicusmarine-1.1.1/copernicusmarine/command_line_interface/group_get.py` & `copernicusmarine-1.2.0/copernicusmarine/command_line_interface/group_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,16 +193,19 @@
     "the files to download.",
 )
 @click.option(
     "--file-list",
     type=pathlib.Path,
     default=None,
     help="A path to a text file that list filenames line by line. "
-    "Filenames must match the absolute paths of "
-    "the files to download.",
+    "Directly download multiple files "
+    "using a list of path from a '.txt' file. "
+    "The files to download have to be from the dataset specified with --dataset-id."
+    "If some files are not found, the toolbox will list all the files "
+    "on the remote server and try to match them.",
 )
 @click.option(
     "--create-file-list",
     type=str,
     default=None,
     help="Option to only create a file containing "
     "the names of the targeted files instead of downloading them. "
@@ -215,14 +218,15 @@
 @click.option(
     "--download-file-list",
     type=bool,
     is_flag=True,
     cls=DeprecatedClickOption,
     deprecated=["--download-file-list"],
     preferred="--create-file-list",
+    hidden=True,
 )
 @click.option(
     "--sync",
     cls=MutuallyExclusiveOption,
     is_flag=True,
     default=False,
     help="Option to synchronize the local directory with "
```

### Comparing `copernicusmarine-1.1.1/copernicusmarine/command_line_interface/group_login.py` & `copernicusmarine-1.2.0/copernicusmarine/command_line_interface/group_login.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/command_line_interface/group_subset.py` & `copernicusmarine-1.2.0/copernicusmarine/command_line_interface/group_subset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/command_line_interface/utils.py` & `copernicusmarine-1.2.0/copernicusmarine/command_line_interface/utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/core_functions/credentials_utils.py` & `copernicusmarine-1.2.0/copernicusmarine/core_functions/credentials_utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/core_functions/custom_zarr_store.py` & `copernicusmarine-1.2.0/copernicusmarine/core_functions/custom_zarr_store.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/core_functions/deprecated.py` & `copernicusmarine-1.2.0/copernicusmarine/core_functions/deprecated.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/core_functions/deprecated_options.py` & `copernicusmarine-1.2.0/copernicusmarine/core_functions/deprecated_options.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/core_functions/describe.py` & `copernicusmarine-1.2.0/copernicusmarine/core_functions/describe.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 logger = logging.getLogger("copernicus_marine_root_logger")
 
 
 def describe_function(
     include_description: bool,
     include_datasets: bool,
     include_keywords: bool,
+    include_all_versions: bool,
     contains: list[str],
     overwrite_metadata_cache: bool,
     no_metadata_cache: bool,
     disable_progress_bar: bool,
     staging: bool,
 ) -> str:
     VersionVerifier.check_version_describe(staging)
@@ -40,15 +41,17 @@
         create_cache_directory()
 
     base_catalogue: CopernicusMarineCatalogue = parse_catalogue(
         no_metadata_cache=no_metadata_cache,
         disable_progress_bar=disable_progress_bar,
         staging=staging,
     )
-    # TODO: the typing of catalogue_dict is wrong, it can be a CopernicusMarineCatalogue
+    if not include_all_versions:
+        base_catalogue.filter_only_official_versions_and_parts()
+
     catalogue_dict = (
         filter_catalogue_with_strings(base_catalogue, contains)
         if contains
         else base_catalogue.__dict__
     )
 
     def default_filter(obj):
```

### Comparing `copernicusmarine-1.1.1/copernicusmarine/core_functions/environment_variables.py` & `copernicusmarine-1.2.0/copernicusmarine/core_functions/environment_variables.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/core_functions/exceptions.py` & `copernicusmarine-1.2.0/copernicusmarine/core_functions/exceptions.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/core_functions/get.py` & `copernicusmarine-1.2.0/copernicusmarine/core_functions/get.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import logging
+import os
 import pathlib
 from typing import List, Optional
 
 from copernicusmarine.catalogue_parser.catalogue_parser import parse_catalogue
 from copernicusmarine.catalogue_parser.request_structure import (
     GetRequest,
-    file_list_to_regex,
     filter_to_regex,
     get_request_from_file,
     overload_regex_with_additionnal_filter,
 )
 from copernicusmarine.core_functions.credentials_utils import (
     get_and_check_username_password,
 )
@@ -100,19 +100,14 @@
         get_request.force_download = force_download
     if overwrite_output_data:
         get_request.overwrite_output_data = overwrite_output_data
     if force_service:
         get_request.force_service = force_service
     if filter:
         get_request.regex = filter_to_regex(filter)
-    if file_list_path:
-        file_list_regex = file_list_to_regex(file_list_path)
-        get_request.regex = overload_regex_with_additionnal_filter(
-            file_list_regex, get_request.regex
-        )
     if regex:
         get_request.regex = overload_regex_with_additionnal_filter(
             regex, get_request.regex
         )
     if sync or sync_delete:
         get_request.sync = True
         if not get_request.force_dataset_version:
@@ -131,14 +126,18 @@
     if download_file_list and not create_file_list:
         create_file_list = "files_to_download.txt"
     if create_file_list is not None:
         assert create_file_list.endswith(".txt") or create_file_list.endswith(
             ".csv"
         ), "Download file list must be a .txt or .csv file. "
         f"Got '{create_file_list}' instead."
+    if file_list_path:
+        direct_download_files = get_direct_download_files(file_list_path)
+        if direct_download_files:
+            get_request.direct_download = direct_download_files
 
     return _run_get_request(
         username=username,
         password=password,
         get_request=get_request,
         create_file_list=create_file_list,
         credentials_file=credentials_file,
@@ -160,14 +159,15 @@
 ) -> List[pathlib.Path]:
     username, password = get_and_check_username_password(
         username,
         password,
         credentials_file,
         no_metadata_cache=no_metadata_cache,
     )
+
     catalogue = parse_catalogue(
         no_metadata_cache=no_metadata_cache,
         disable_progress_bar=disable_progress_bar,
         staging=staging,
     )
     retrieval_service: RetrievalService = get_retrieval_service(
         catalogue,
@@ -225,7 +225,23 @@
                 "no_metadata_cache": False,
                 "log_level": "INFO",
             },
             output_file,
             indent=4,
         )
     logger.info(f"Template created at: {filename}")
+
+
+def get_direct_download_files(
+    file_list_path: Optional[pathlib.Path],
+) -> Optional[list[str]]:
+    if file_list_path:
+        if not os.path.exists(file_list_path):
+            raise FileNotFoundError(
+                f"File {file_list_path} does not exist."
+                " Please provide a valid path to a .txt file."
+            )
+        with open(file_list_path) as f:
+            direct_download_files = [line.strip() for line in f.readlines()]
+        return direct_download_files
+    else:
+        return None
```

### Comparing `copernicusmarine-1.1.1/copernicusmarine/core_functions/login.py` & `copernicusmarine-1.2.0/copernicusmarine/core_functions/login.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/core_functions/services_utils.py` & `copernicusmarine-1.2.0/copernicusmarine/core_functions/services_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,22 @@
     CopernicusMarineCatalogue,
     CopernicusMarineDatasetServiceType,
     CopernicusMarineDatasetVersion,
     CopernicusMarineProductDataset,
     CopernicusMarineService,
     CopernicusMarineServiceFormat,
     CopernicusMarineVersionPart,
-    dataset_version_not_found_exception,
 )
 from copernicusmarine.catalogue_parser.request_structure import (
     DatasetTimeAndGeographicalSubset,
 )
 from copernicusmarine.core_functions import sessions
 from copernicusmarine.core_functions.utils import (
     FormatNotSupported,
+    datetime_parser,
     next_or_raise_exception,
 )
 from copernicusmarine.download_functions.subset_xarray import (
     get_size_of_coordinate_subset,
 )
 
 logger = logging.getLogger("copernicus_marine_root_logger")
@@ -396,26 +396,16 @@
     dataset_sync: bool,
 ) -> RetrievalService:
     if force_dataset_version_label:
         logger.info(
             "You forced selection of dataset version "
             + f'"{force_dataset_version_label}"'
         )
-        dataset_version: CopernicusMarineDatasetVersion = (
-            next_or_raise_exception(
-                filter(
-                    lambda version: version.label
-                    == force_dataset_version_label,
-                    dataset.versions,
-                ),
-                dataset_version_not_found_exception(dataset),
-            )
-        )
-    else:
-        dataset_version = dataset.get_latest_version_or_raise()
+    dataset_version = dataset.get_version(force_dataset_version_label)
+    if not force_dataset_version_label:
         logger.info(
             "Dataset version was not specified, the latest "
             f'one was selected: "{dataset_version.label}"'
         )
     return _get_retrieval_service_from_dataset_version(
         dataset_id=dataset.dataset_id,
         dataset_version=dataset_version,
@@ -456,24 +446,28 @@
             "with the dataset-part option"
         )
     if force_dataset_part_label:
         logger.info(
             f"You forced selection of dataset part "
             f'"{force_dataset_part_label}"'
         )
-    dataset_part = dataset_version.get_part(
-        force_part=force_dataset_part_label
-    )
+    dataset_part = dataset_version.get_part(force_dataset_part_label)
     if not force_dataset_part_label:
         logger.info(
             "Dataset part was not specified, the first "
             f'one was selected: "{dataset_part.name}"'
         )
     if dataset_part.retired_date:
-        warning_dataset_will_be_deprecated(
+        _warning_dataset_will_be_deprecated(
+            dataset_id, dataset_version, dataset_part
+        )
+    if dataset_part.released_date and datetime_parser(
+        dataset_part.released_date
+    ) > datetime_parser("now"):
+        _warning_dataset_not_yet_released(
             dataset_id, dataset_version, dataset_part
         )
 
     if force_service_type:
         logger.info(
             f"You forced selection of service: "
             f"{force_service_type.service_name.value}"
@@ -520,15 +514,15 @@
     return None
 
 
 class ServiceNotAvailable(Exception):
     ...
 
 
-def warning_dataset_will_be_deprecated(
+def _warning_dataset_will_be_deprecated(
     dataset_id: str,
     dataset_version: CopernicusMarineDatasetVersion,
     dataset_part: CopernicusMarineVersionPart,
 ):
     logger.warn(
         f"""The dataset {dataset_id}"""
         f"""{f", version '{dataset_version.label}'"
@@ -537,14 +531,32 @@
               if dataset_part.name != 'default' else '')}"""
         f"""{"," if dataset_version.label != 'default' else ""}"""
         f""" will be retired on the {dataset_part.retired_date}."""
         """ After this date, it will no longer be available on the toolbox."""
     )
 
 
+def _warning_dataset_not_yet_released(
+    dataset_id: str,
+    dataset_version: CopernicusMarineDatasetVersion,
+    dataset_part: CopernicusMarineVersionPart,
+):
+    logger.warn(
+        f"""The dataset {dataset_id}"""
+        f"""{f", version '{dataset_version.label}'"
+             if dataset_version.label != 'default' else ''}"""
+        f"""{(f"and part '{dataset_part.name}'"
+              if dataset_part.name != 'default' else '')}"""
+        f"""{"," if dataset_version.label != 'default' else ""}"""
+        f""" is not yet released officially."""
+        f""" It will be available by default  on the toolbox on the"""
+        f""" {dataset_part.released_date}."""
+    )
+
+
 def _service_not_available_error(
     dataset_version_part: CopernicusMarineVersionPart,
     command_type: CommandType,
 ) -> ServiceNotAvailable:
     dataset_available_service_types = [
         service.service_type.short_name.value
         for service in dataset_version_part.services
```

### Comparing `copernicusmarine-1.1.1/copernicusmarine/core_functions/sessions.py` & `copernicusmarine-1.2.0/copernicusmarine/core_functions/sessions.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/core_functions/subset.py` & `copernicusmarine-1.2.0/copernicusmarine/core_functions/subset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/core_functions/utils.py` & `copernicusmarine-1.2.0/copernicusmarine/core_functions/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import logging
 import os
 import pathlib
 import re
-from datetime import datetime
+from datetime import datetime, timezone
 from importlib.metadata import version
 from typing import (
     Any,
     Awaitable,
     Callable,
     Coroutine,
     Iterable,
@@ -15,14 +15,16 @@
     List,
     Optional,
     Tuple,
     TypeVar,
     Union,
 )
 
+import cftime
+import numpy
 import xarray
 from requests import PreparedRequest
 
 from copernicusmarine.core_functions.environment_variables import (
     COPERNICUSMARINE_CACHE_DIRECTORY,
 )
 
@@ -134,14 +136,25 @@
         try:
             return datetime.strptime(string, format)
         except ValueError:
             pass
     raise WrongDatetimeFormat(string)
 
 
+def convert_datetime64_to_netcdf_timestamp(
+    datetime_value: numpy.datetime64,
+    cftime_unit: str,
+) -> int:
+    nanosecond = 1e-9
+    date = datetime.fromtimestamp(
+        datetime_value.astype(int) * nanosecond, tz=timezone.utc
+    )
+    return cftime.date2num(date, cftime_unit)
+
+
 def add_copernicusmarine_version_in_dataset_attributes(
     dataset: xarray.Dataset,
 ) -> xarray.Dataset:
     dataset.attrs["copernicusmarine_version"] = version("copernicusmarine")
     return dataset
```

### Comparing `copernicusmarine-1.1.1/copernicusmarine/core_functions/versions_verifier.py` & `copernicusmarine-1.2.0/copernicusmarine/core_functions/versions_verifier.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/download_functions/common_download.py` & `copernicusmarine-1.2.0/copernicusmarine/download_functions/common_download.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/download_functions/download_arco_series.py` & `copernicusmarine-1.2.0/copernicusmarine/download_functions/download_arco_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     if "depth" in preferred_chunks:
         preferred_chunks["elevation"] = preferred_chunks["depth"]
     elif "elevation" in preferred_chunks:
         preferred_chunks["depth"] = preferred_chunks["elevation"]
 
     return dataset.chunk(
-        _filter_dimensions(preferred_chunks, dataset.dims.keys())
+        _filter_dimensions(preferred_chunks, dataset.sizes.keys())
     )
 
 
 def _filter_dimensions(
     rechunks: dict[str, int], dimensions: Iterable[Hashable]
 ) -> dict[str, int]:
     return {k: v for k, v in rechunks.items() if k in dimensions}
@@ -205,15 +205,17 @@
     variables: Optional[list[str]],
     geographical_parameters: GeographicalParameters,
     temporal_parameters: TemporalParameters,
     depth_parameters: DepthParameters,
     chunks=Optional[Literal["auto"]],
 ) -> xarray.Dataset:
     dataset = sessions.open_zarr(
-        dataset_url, chunks=chunks, copernicus_marine_username=username
+        dataset_url,
+        chunks=chunks,
+        copernicus_marine_username=username,
     )
     dataset = subset(
         dataset=dataset,
         variables=variables,
         geographical_parameters=geographical_parameters,
         temporal_parameters=temporal_parameters,
         depth_parameters=depth_parameters,
```

### Comparing `copernicusmarine-1.1.1/copernicusmarine/download_functions/download_get.py` & `copernicusmarine-1.2.0/copernicusmarine/download_functions/download_get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/download_functions/download_original_files.py` & `copernicusmarine-1.2.0/copernicusmarine/download_functions/download_original_files.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,23 +2,28 @@
 import logging
 import os
 import pathlib
 import re
 from itertools import chain
 from multiprocessing.pool import ThreadPool
 from pathlib import Path
-from typing import List, Optional, Tuple
+from typing import Callable, List, Optional, Tuple
 
 import boto3
 import botocore
+import botocore.config
 import click
+from botocore.client import ClientError
 from numpy import append, arange
 from tqdm import tqdm
 
-from copernicusmarine.catalogue_parser.request_structure import GetRequest
+from copernicusmarine.catalogue_parser.request_structure import (
+    GetRequest,
+    overload_regex_with_additionnal_filter,
+)
 from copernicusmarine.core_functions.utils import (
     FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE,
     construct_query_params_for_marine_data_store_monitoring,
     construct_url_with_query_params,
     flatten,
     get_unique_filename,
     parse_access_dataset_url,
@@ -30,34 +35,79 @@
 def download_original_files(
     username: str,
     password: str,
     get_request: GetRequest,
     disable_progress_bar: bool,
     create_file_list: Optional[str],
 ) -> list[pathlib.Path]:
-    result = _download_header(
-        str(get_request.dataset_url),
-        get_request.regex,
-        username,
-        password,
-        get_request.sync,
-        create_file_list,
-        pathlib.Path(get_request.output_directory),
-        only_list_root_path=get_request.index_parts,
-        overwrite=get_request.overwrite_output_data,
+    files_not_found: list[str] = []
+    filenames_in_sync_ignored: list[str] = []
+    total_size: float = 0.0
+    sizes: list[float] = []
+    last_modified_datetimes: list[datetime.datetime] = []
+    filenames_in: list[str] = []
+    if get_request.direct_download:
+        (
+            locator,
+            filenames_in,
+            sizes,
+            last_modified_datetimes,
+            total_size,
+            filenames_in_sync_ignored,
+            files_not_found,
+        ) = _download_header_for_direct_download(
+            get_request.direct_download,
+            str(get_request.dataset_url),
+            get_request.sync,
+            pathlib.Path(get_request.output_directory),
+            username,
+        )
+    if not get_request.direct_download or files_not_found or get_request.regex:
+        if files_not_found:
+            files_not_found_regex = "|".join(
+                [
+                    re.escape(file_not_found)
+                    for file_not_found in files_not_found
+                ]
+            )
+            get_request.regex = overload_regex_with_additionnal_filter(
+                files_not_found_regex, get_request.regex
+            )
+        result = _download_header(
+            str(get_request.dataset_url),
+            get_request.regex,
+            username,
+            password,
+            get_request.sync,
+            create_file_list,
+            pathlib.Path(get_request.output_directory),
+            only_list_root_path=get_request.index_parts,
+            overwrite=get_request.overwrite_output_data,
+        )
+        if result:
+            (
+                locator,
+                filenames_in_listing,
+                sizes_listing,
+                last_modified_datetimes_listing,
+                total_size_listing,
+                filenames_in_sync_ignored_listing,
+            ) = result
+            filenames_in.extend(filenames_in_listing)
+            filenames_in_sync_ignored.extend(filenames_in_sync_ignored_listing)
+            total_size += total_size_listing
+            sizes.extend(sizes_listing)
+            last_modified_datetimes.extend(last_modified_datetimes_listing)
+        elif not get_request.direct_download or len(files_not_found) == len(
+            get_request.direct_download
+        ):
+            return []
+    message = _create_information_message_before_download(
+        filenames_in, sizes, last_modified_datetimes, total_size
     )
-    if result is None:
-        return []
-    (
-        message,
-        locator,
-        filenames_in,
-        total_size,
-        filenames_in_sync_ignored,
-    ) = result
     filenames_out = create_filenames_out(
         filenames_in=filenames_in,
         output_directory=pathlib.Path(get_request.output_directory),
         no_directories=get_request.no_directories,
         overwrite=(
             get_request.overwrite_output_data
             if not get_request.sync
@@ -184,83 +234,155 @@
     username: str,
     _password: str,
     sync: bool,
     create_file_list: Optional[str],
     directory_out: pathlib.Path,
     only_list_root_path: bool = False,
     overwrite: bool = False,
-) -> Optional[Tuple[str, Tuple[str, str], list[str], float, list[str]]]:
+) -> Optional[
+    Tuple[
+        Tuple[str, str],
+        list[str],
+        List[float],
+        List[datetime.datetime],
+        float,
+        list[str],
+    ]
+]:
     (endpoint_url, bucket, path) = parse_access_dataset_url(
         data_path, only_dataset_root_path=only_list_root_path
     )
 
-    filenames, sizes, total_size = [], [], 0.0
+    filenames: list[str] = []
+    sizes: list[float] = []
+    total_size = 0.0
+    last_modified_datetimes: list[datetime.datetime] = []
+    etags: list[str] = []
     raw_filenames = _list_files_on_marine_data_lake_s3(
         username, endpoint_url, bucket, path, not only_list_root_path
     )
-    filename_filtered = []
     filenames_without_sync = []
     for filename, size, last_modified_datetime, etag in raw_filenames:
         if not regex or re.search(regex, filename):
             filenames_without_sync.append(filename)
             if not sync or _check_needs_to_be_synced(
                 filename, size, last_modified_datetime, directory_out
             ):
                 filenames.append(filename)
                 sizes.append(float(size))
-                total_size += float(size)
-                filename_filtered.append(
-                    (filename, size, last_modified_datetime, etag)
-                )
-
+                last_modified_datetimes.append(last_modified_datetime)
+                etags.append(etag)
+    total_size = sum(sizes)
     if create_file_list and create_file_list.endswith(".txt"):
         download_filename = get_unique_filename(
             directory_out / create_file_list, overwrite
         )
         logger.info(f"The file list is written at {download_filename}")
         with open(download_filename, "w") as file_out:
-            for filename, _, _, _ in filename_filtered:
+            for filename in filenames:
                 file_out.write(f"{filename}\n")
         return None
     elif create_file_list and create_file_list.endswith(".csv"):
         download_filename = get_unique_filename(
             directory_out / create_file_list, overwrite
         )
         logger.info(f"The file list is written at {download_filename}")
         with open(download_filename, "w") as file_out:
             file_out.write("filename,size,last_modified_datetime,etag\n")
             for (
                 filename,
-                size,
+                size_file,
                 last_modified_datetime,
                 etag,
-            ) in filename_filtered:
+            ) in zip(filenames, sizes, last_modified_datetimes, etags):
                 file_out.write(
-                    f"{filename},{size},{last_modified_datetime},{etag}\n"
+                    f"{filename},{size_file},{last_modified_datetime},{etag}\n"
                 )
         return None
+    locator = (endpoint_url, bucket)
+    return (
+        locator,
+        filenames,
+        sizes,
+        last_modified_datetimes,
+        total_size,
+        filenames_without_sync,
+    )
 
-    message = "You requested the download of the following files:\n"
-    for filename, size, last_modified_datetime, _ in filename_filtered[:20]:
-        message += str(filename)
-        datetime_iso = re.sub(
-            r"\+00:00$",
-            "Z",
-            last_modified_datetime.astimezone(datetime.timezone.utc).isoformat(
-                timespec="seconds"
-            ),
+
+def _download_header_for_direct_download(
+    files_to_download: list[str],
+    dataset_url: str,
+    sync: bool,
+    directory_out: pathlib.Path,
+    username: str,
+) -> Tuple[
+    Tuple[str, str],
+    List[str],
+    List[float],
+    List[datetime.datetime],
+    float,
+    list[str],
+    list[str],
+]:
+    (endpoint_url, bucket, path) = parse_access_dataset_url(dataset_url)
+    splitted_path = path.split("/")
+    root_folder = splitted_path[0]
+    product_id = splitted_path[1]
+    dataset_id_with_tag = splitted_path[2]
+
+    sizes = []
+    last_modified_datetimes = []
+    filenames_in = []
+    filenames_without_sync = []
+    filenames_not_found = []
+    for file_to_download in files_to_download:
+        file_path = file_to_download.split(f"{dataset_id_with_tag}/")[-1]
+        if not file_path:
+            logger.warning(
+                f"{file_to_download} does not seem to be valid. Skipping."
+            )
+            filenames_not_found.append(file_path)
+            continue
+        full_path = (
+            f"s3://{bucket}/{root_folder}/{product_id}/"
+            f"{dataset_id_with_tag}/{file_path}"
         )
-        message += f" - {format_file_size(float(size))} - {datetime_iso}\n"
-    if len(filenames) > 20:
-        message += f"Printed 20 out of {len(filenames)} files\n"
-    message += (
-        f"\nTotal size of the download: {format_file_size(total_size)}\n\n"
+        size_and_last_modified = _get_file_size_and_last_modified(
+            endpoint_url, bucket, full_path, username
+        )
+        if size_and_last_modified:
+            size, last_modified = size_and_last_modified
+            if not sync or _check_needs_to_be_synced(
+                full_path, size, last_modified, directory_out
+            ):
+                filenames_in.append(full_path)
+                sizes.append(float(size))
+                last_modified_datetimes.append(last_modified)
+            else:
+                filenames_without_sync.append(full_path)
+        else:
+            filenames_not_found.append(full_path)
+    if not filenames_in:
+        logger.warning(
+            "No files found to download for direct download. "
+            "Please check the files to download. "
+            "We will try to list the files available for download "
+            "and compare them with the requested files."
+        )
+    total_size = sum([size for size in sizes])
+    return (
+        (endpoint_url, bucket),
+        filenames_in,
+        sizes,
+        last_modified_datetimes,
+        total_size,
+        filenames_without_sync,
+        filenames_not_found,
     )
-    locator = (endpoint_url, bucket)
-    return (message, locator, filenames, total_size, filenames_without_sync)
 
 
 def _check_needs_to_be_synced(
     filename: str,
     size: int,
     last_modified_datetime: datetime.datetime,
     directory_out: pathlib.Path,
@@ -275,51 +397,83 @@
         else:
             last_created_datetime_out = datetime.datetime.fromtimestamp(
                 file_stats.st_ctime, tz=datetime.timezone.utc
             )
             return last_modified_datetime > last_created_datetime_out
 
 
+def _create_information_message_before_download(
+    filenames: list[str],
+    sizes: list[float],
+    last_modified_datetimes: list[datetime.datetime],
+    total_size: float,
+) -> str:
+    message = "You requested the download of the following files:\n"
+    for filename, size, last_modified_datetime in zip(
+        filenames[:20], sizes[:20], last_modified_datetimes[:20]
+    ):
+        message += str(filename)
+        datetime_iso = re.sub(
+            r"\+00:00$",
+            "Z",
+            last_modified_datetime.astimezone(datetime.timezone.utc).isoformat(
+                timespec="seconds"
+            ),
+        )
+        message += f" - {format_file_size(float(size))} - {datetime_iso}\n"
+    if len(filenames) > 20:
+        message += f"Printed 20 out of {len(filenames)} files\n"
+    message += (
+        f"\nTotal size of the download: {format_file_size(total_size)}\n\n"
+    )
+    return message
+
+
 def _local_path_from_s3_url(
     s3_url: str, local_directory: pathlib.Path
 ) -> pathlib.Path:
     return local_directory / pathlib.Path("/".join(s3_url.split("/")[4:]))
 
 
-def _list_files_on_marine_data_lake_s3(
-    username: str,
-    endpoint_url: str,
-    bucket: str,
-    prefix: str,
-    recursive: bool,
-) -> list[tuple[str, int, datetime.datetime, str]]:
+def _create_custom_query_function(username: str) -> Callable:
     def _add_custom_query_param(params, context, **kwargs):
         """
         Add custom query params for MDS's Monitoring
         """
         params["url"] = construct_url_with_query_params(
             params["url"],
             construct_query_params_for_marine_data_store_monitoring(username),
         )
 
+    return _add_custom_query_param
+
+
+def _list_files_on_marine_data_lake_s3(
+    username: str,
+    endpoint_url: str,
+    bucket: str,
+    prefix: str,
+    recursive: bool,
+) -> list[tuple[str, int, datetime.datetime, str]]:
+
     s3_session = boto3.Session()
     s3_client = s3_session.client(
         "s3",
         config=botocore.config.Config(
             # Configures to use subdomain/virtual calling format.
             s3={"addressing_style": "virtual"},
             signature_version=botocore.UNSIGNED,
         ),
         endpoint_url=endpoint_url,
     )
 
     # Register the botocore event handler for adding custom query params
     # to S3 LIST requests
     s3_client.meta.events.register(
-        "before-call.s3.ListObjects", _add_custom_query_param
+        "before-call.s3.ListObjects", _create_custom_query_function(username)
     )
 
     paginator = s3_client.get_paginator("list_objects")
     page_iterator = paginator.paginate(
         Bucket=bucket,
         Prefix=prefix,
         Delimiter="/" if not recursive else "",
@@ -338,36 +492,60 @@
                 s3_object["LastModified"],
                 s3_object["ETag"],
             )
         )
     return files_already_found
 
 
+def _get_file_size_and_last_modified(
+    endpoint_url: str, bucket: str, file_in: str, username: str
+) -> Optional[Tuple[int, datetime.datetime]]:
+    s3_session = boto3.Session()
+    s3_client = s3_session.client(
+        "s3",
+        config=botocore.config.Config(
+            s3={"addressing_style": "virtual"},
+            signature_version=botocore.UNSIGNED,
+        ),
+        endpoint_url=endpoint_url,
+    )
+
+    s3_client.meta.events.register(
+        "before-call.s3.HeadObject", _create_custom_query_function(username)
+    )
+
+    try:
+        s3_object = s3_client.head_object(
+            Bucket=bucket,
+            Key=file_in.replace(f"s3://{bucket}/", ""),
+        )
+        return s3_object["ContentLength"], s3_object["LastModified"]
+    except ClientError as e:
+        if "404" in str(e):
+            logger.warning(
+                f"File {file_in} not found on the server. Skipping."
+            )
+            return None
+        else:
+            raise e
+
+
 def _download_files(
     tuple_original_files_filename: Tuple[
         str, str, str, list[str], list[pathlib.Path]
     ],
 ) -> list[pathlib.Path]:
     (
         username,
         endpoint_url,
         bucket,
         filenames_in,
         filenames_out,
     ) = tuple_original_files_filename
 
-    def _add_custom_query_param(params, context, **kwargs):
-        """
-        Add custom query params for MDS's Monitoring
-        """
-        params["url"] = construct_url_with_query_params(
-            params["url"],
-            construct_query_params_for_marine_data_store_monitoring(username),
-        )
-
     def _original_files_file_download(
         endpoint_url: str, bucket: str, file_in: str, file_out: pathlib.Path
     ) -> pathlib.Path:
         """
         Download ONE file and return a string of the result
         """
         s3_session = boto3.Session()
@@ -389,18 +567,19 @@
             ),
             endpoint_url=endpoint_url,
         )
 
         # Register the botocore event handler for adding custom query params
         # to S3 HEAD and GET requests
         s3_client.meta.events.register(
-            "before-call.s3.HeadObject", _add_custom_query_param
+            "before-call.s3.HeadObject",
+            _create_custom_query_function(username),
         )
         s3_client.meta.events.register(
-            "before-call.s3.GetObject", _add_custom_query_param
+            "before-call.s3.GetObject", _create_custom_query_function(username)
         )
 
         last_modified_date_epoch = s3_resource.Object(
             bucket, file_in.replace(f"s3://{bucket}/", "")
         ).last_modified.timestamp()
 
         s3_client.download_file(
```

### Comparing `copernicusmarine-1.1.1/copernicusmarine/download_functions/subset_parameters.py` & `copernicusmarine-1.2.0/copernicusmarine/download_functions/subset_parameters.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/download_functions/subset_xarray.py` & `copernicusmarine-1.2.0/copernicusmarine/download_functions/subset_xarray.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 from copernicusmarine.core_functions import sessions
 from copernicusmarine.core_functions.exceptions import (
     CoordinatesOutOfDatasetBounds,
     MinimumLongitudeGreaterThanMaximumLongitude,
     VariableDoesNotExistInTheDataset,
 )
 from copernicusmarine.core_functions.models import SubsetMethod
+from copernicusmarine.core_functions.utils import (
+    convert_datetime64_to_netcdf_timestamp,
+)
 from copernicusmarine.download_functions.subset_parameters import (
     DepthParameters,
     GeographicalParameters,
     LatitudeParameters,
     LongitudeParameters,
     TemporalParameters,
 )
@@ -63,20 +66,20 @@
 def _dataset_custom_sel(
     dataset: xarray.Dataset,
     coord_type: Literal["latitude", "longitude", "depth", "time"],
     coord_selection: Union[float, slice, datetime, None],
     method: Union[str, None] = None,
 ) -> xarray.Dataset:
     for coord_label in COORDINATES_LABEL[coord_type]:
-        if coord_label in dataset.dims:
+        if coord_label in dataset.sizes:
             tmp_dataset = dataset.sel(
                 {coord_label: coord_selection}, method=method
             )
             if tmp_dataset.coords[coord_label].size == 0 or (
-                coord_label not in tmp_dataset.dims
+                coord_label not in tmp_dataset.sizes
             ):
                 target = (
                     coord_selection.start
                     if isinstance(coord_selection, slice)
                     else coord_selection
                 )
                 nearest_neighbor_value = _nearest_neighbor_coordinates(
@@ -97,38 +100,49 @@
 def get_size_of_coordinate_subset(
     dataset: xarray.Dataset,
     coordinate: str,
     minimum: Optional[Union[float, datetime]],
     maximum: Optional[Union[float, datetime]],
 ) -> int:
     for label in COORDINATES_LABEL[coordinate]:
-        if label in dataset.dims:
+        if label in dataset.sizes:
             return (
                 dataset.coords[coordinate]
                 .sel({coordinate: slice(minimum, maximum)}, method=None)
                 .coords[coordinate]
                 .size
             )
     else:
         raise KeyError(
             f"Could not subset on {coordinate}. "
             "Didn't find an equivalent in the dataset."
         )
 
 
-def _update_dataset_attributes(dataset: xarray.Dataset):
+def _update_dataset_attributes(
+    dataset: xarray.Dataset,
+    minimum_longitude_modulus: float,
+):
+    window = (
+        minimum_longitude_modulus + 180
+    )  # compute the degrees needed to move the dataset
     for coord_label in COORDINATES_LABEL["longitude"]:
-        if coord_label in dataset.dims:
+        if coord_label in dataset.sizes:
             attrs = dataset[coord_label].attrs
             if "valid_min" in attrs:
-                attrs["valid_min"] += 180
+                attrs["valid_min"] += window
             if "valid_max" in attrs:
-                attrs["valid_max"] += 180
+                attrs["valid_max"] += window
             dataset = dataset.assign_coords(
-                {coord_label: dataset[coord_label] % 360}
+                {
+                    coord_label: (
+                        (dataset[coord_label] + (180 - window)) % 360
+                    )
+                    - (180 - window)
+                }
             ).sortby(coord_label)
             dataset[coord_label].attrs = attrs
     return dataset
 
 
 def _latitude_subset(
     dataset: xarray.Dataset,
@@ -176,15 +190,17 @@
                     minimum_longitude
                 )
                 maximum_longitude_modulus = longitude_modulus(
                     maximum_longitude
                 )
                 if maximum_longitude_modulus < minimum_longitude_modulus:
                     maximum_longitude_modulus += 360
-                    dataset = _update_dataset_attributes(dataset)
+                    dataset = _update_dataset_attributes(
+                        dataset, minimum_longitude_modulus
+                    )
                 longitude_selection = slice(
                     minimum_longitude_modulus,
                     maximum_longitude_modulus,
                 )
         else:
             longitude_selection = slice(minimum_longitude, maximum_longitude)
 
@@ -215,25 +231,28 @@
 
 
 def _depth_subset(
     dataset: xarray.Dataset,
     depth_parameters: DepthParameters,
 ) -> xarray.Dataset:
     def convert_elevation_to_depth(dataset: xarray.Dataset):
-        if "elevation" in dataset.dims:
+        if "elevation" in dataset.sizes:
             attrs = dataset["elevation"].attrs
             dataset = dataset.reindex(elevation=dataset.elevation[::-1])
             dataset["elevation"] = dataset.elevation * (-1)
             attrs["positive"] = "down"
+            attrs["standard_name"] = "depth"
+            attrs["long_name"] = "Depth"
+            attrs["units"] = "m"
             dataset = dataset.rename({"elevation": "depth"})
             dataset.depth.attrs = attrs
         return dataset
 
     def update_elevation_attributes(dataset: xarray.Dataset):
-        if "elevation" in dataset.dims:
+        if "elevation" in dataset.sizes:
             attrs = dataset["elevation"].attrs
             attrs["positive"] = "up"
             attrs["standard_name"] = "elevation"
             attrs["long_name"] = "Elevation"
             attrs["units"] = "m"
             dataset["elevation"].attrs = attrs
         return dataset
@@ -303,24 +322,32 @@
 
 
 def _update_dataset_coordinate_valid_minmax_attributes(
     dataset: xarray.Dataset,
 ) -> xarray.Dataset:
     for coordinate_label in COORDINATES_LABEL:
         for coordinate_alias in COORDINATES_LABEL[coordinate_label]:
-            if coordinate_alias in dataset.dims:
+            if coordinate_alias in dataset.sizes:
                 coord = dataset[coordinate_alias]
                 attrs = coord.attrs
-
-                if "time" not in coordinate_label:
+                if "time" in coordinate_label:
+                    min_time_dimension = coord.values.min()
+                    max_time_dimension = coord.values.max()
+                    netcdf_unit = coord.encoding["units"]
+                    valid_min = convert_datetime64_to_netcdf_timestamp(
+                        min_time_dimension, netcdf_unit
+                    )
+                    valid_max = convert_datetime64_to_netcdf_timestamp(
+                        max_time_dimension, netcdf_unit
+                    )
+                    attrs["valid_min"] = valid_min
+                    attrs["valid_max"] = valid_max
+                else:
                     attrs["valid_min"] = coord.values.min()
                     attrs["valid_max"] = coord.values.max()
-                else:
-                    attrs["valid_min"] = str(coord.values.min())
-                    attrs["valid_max"] = str(coord.values.max())
 
                 coord.attrs = attrs
 
     return dataset
 
 
 def subset(
@@ -347,24 +374,34 @@
     dataset = _update_dataset_coordinate_valid_minmax_attributes(dataset)
 
     return dataset
 
 
 def longitude_modulus(longitude: float) -> float:
     """
-    Returns the equivalent longitude between -180 and 180
+    Returns the equivalent longitude in [-180, 180[
     """
     # We are using Decimal to avoid issue with rounding
     modulus = float(Decimal(str(longitude + 180)) % 360)
     # Modulus with python return a negative value if the denominator is negative
     # To counteract that, we add 360 if the result is < 0
     modulus = modulus if modulus >= 0 else modulus + 360
     return modulus - 180
 
 
+def longitude_modulus_upper_bound(longitude: float) -> float:
+    """
+    Returns the equivalent longitude in ]-180, 180]
+    """
+    modulus = longitude_modulus(longitude)
+    if modulus == -180:
+        return 180.0
+    return modulus
+
+
 def check_dataset_subset_bounds(
     username: str,
     password: str,
     dataset_url: str,
     service_type: CopernicusMarineDatasetServiceType,
     dataset_subset: DatasetTimeAndGeographicalSubset,
     subset_method: SubsetMethod,
@@ -383,15 +420,15 @@
     else:
         session = sessions.get_configured_request_session()
         session.auth = (username, password)
         store = PydapDataStore.open(dataset_url, session=session, timeout=300)
         dataset = xarray.open_dataset(store)
         dataset_coordinates = dataset.coords
     for coordinate_label in COORDINATES_LABEL["latitude"]:
-        if coordinate_label in dataset.dims:
+        if coordinate_label in dataset.sizes:
             latitudes = dataset_coordinates[coordinate_label].values
             user_minimum_coordinate_value = (
                 dataset_subset.minimum_latitude
                 if dataset_subset.minimum_latitude is not None
                 else latitudes.min()
             )
             user_maximum_coordinate_value = (
@@ -404,34 +441,36 @@
                 user_minimum_coordinate_value=user_minimum_coordinate_value,
                 user_maximum_coordinate_value=user_maximum_coordinate_value,
                 dataset_minimum_coordinate_value=latitudes.min(),
                 dataset_maximum_coordinate_value=latitudes.max(),
                 is_strict=subset_method == "strict",
             )
     for coordinate_label in COORDINATES_LABEL["longitude"]:
-        if coordinate_label in dataset.dims:
+        if coordinate_label in dataset.sizes:
             longitudes = dataset_coordinates[coordinate_label].values
             _check_coordinate_overlap(
                 dimension="longitude",
                 user_minimum_coordinate_value=(
                     longitude_modulus(dataset_subset.minimum_longitude)
                     if dataset_subset.minimum_longitude is not None
                     else longitudes.min()
                 ),
                 user_maximum_coordinate_value=(
-                    longitude_modulus(dataset_subset.maximum_longitude)
+                    longitude_modulus_upper_bound(
+                        dataset_subset.maximum_longitude
+                    )
                     if dataset_subset.maximum_longitude is not None
                     else longitudes.max()
                 ),
                 dataset_minimum_coordinate_value=longitudes.min(),
                 dataset_maximum_coordinate_value=longitudes.max(),
                 is_strict=subset_method == "strict",
             )
     for coordinate_label in COORDINATES_LABEL["time"]:
-        if coordinate_label in dataset.dims:
+        if coordinate_label in dataset.sizes:
             times = dataset_coordinates[coordinate_label].values
             if dataset_valid_date:
                 times_min = dataset_valid_date
             else:
                 times_min = times.min()
             dataset_minimum_coordinate_value = date_to_datetime(times_min)
             dataset_maximum_coordinate_value = date_to_datetime(times.max())
```

### Comparing `copernicusmarine-1.1.1/copernicusmarine/download_functions/utils.py` & `copernicusmarine-1.2.0/copernicusmarine/download_functions/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,20 +61,24 @@
         _get_max_coordinate(dataset, "depth"),
     )
 
     min_time_coordinate = _get_min_coordinate(dataset, "time")
     max_time_coordinate = _get_max_coordinate(dataset, "time")
 
     datetimes = _format_datetimes(
-        Timestamp(min_time_coordinate).to_pydatetime()
-        if min_time_coordinate is not None
-        else None,
-        Timestamp(max_time_coordinate).to_pydatetime()
-        if max_time_coordinate is not None
-        else None,
+        (
+            Timestamp(min_time_coordinate).to_pydatetime()
+            if min_time_coordinate is not None
+            else None
+        ),
+        (
+            Timestamp(max_time_coordinate).to_pydatetime()
+            if max_time_coordinate is not None
+            else None
+        ),
     )
 
     filename = "_".join(
         filter(
             None,
             [dataset_id, variables, longitudes, latitudes, depths, datetimes],
         )
@@ -82,22 +86,22 @@
     filename = filename if len(filename) < 250 else filename[250:]
 
     return filename + get_file_extension(file_format)
 
 
 def _get_min_coordinate(dataset: xarray.Dataset, coordinate: str):
     for coord_label in COORDINATES_LABEL[coordinate]:
-        if coord_label in dataset.dims:
+        if coord_label in dataset.sizes:
             return min(dataset[coord_label].values)
     return None
 
 
 def _get_max_coordinate(dataset: xarray.Dataset, coordinate: str):
     for coord_label in COORDINATES_LABEL[coordinate]:
-        if coord_label in dataset.dims:
+        if coord_label in dataset.sizes:
             return max(dataset[coord_label].values)
     return None
 
 
 def _format_longitudes(
     minimum_longitude: Optional[float], maximum_longitude: Optional[float]
 ) -> str:
@@ -163,15 +167,15 @@
                 f"{maximum_datetime.strftime('%Y-%m-%d')}"
             )
         return formatted_datetime
 
 
 def get_formatted_dataset_size_estimation(dataset: xarray.Dataset) -> str:
     coordinates_size = 1
-    for coordinate in dataset.dims:
+    for coordinate in dataset.sizes:
         coordinates_size *= dataset[coordinate].size
     estimate_size = (
         coordinates_size
         * len(list(dataset.data_vars))
         * dataset[list(dataset.data_vars)[0]].dtype.itemsize
         / 1048e3
     )
```

### Comparing `copernicusmarine-1.1.1/copernicusmarine/logging_conf.json` & `copernicusmarine-1.2.0/copernicusmarine/logging_conf.json`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/python_interface/describe.py` & `copernicusmarine-1.2.0/copernicusmarine/python_interface/describe.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 
 @log_exception_and_exit
 def describe(
     include_description: bool = False,
     include_datasets: bool = False,
     include_keywords: bool = False,
+    include_all_versions: bool = False,
     contains: list[str] = [],
     overwrite_metadata_cache: bool = False,
     no_metadata_cache: bool = False,
     disable_progress_bar: bool = False,
     staging: bool = False,
 ) -> dict[str, Any]:
     """
@@ -24,14 +25,15 @@
     This function fetches metadata information from the Copernicus Marine catalogue
     based on specified parameters and options.
 
     Args:
         include_description (bool, optional): Whether to include description for each item. Defaults to False.
         include_datasets (bool, optional): Whether to include dataset information. Defaults to False.
         include_keywords (bool, optional): Whether to include keywords for each item. Defaults to False.
+        include_all_versions (bool, optional): Whether to include all versions of each item. Defaults to False.
         contains (list[str], optional): List of strings to filter items containing these values. Defaults to [].
         overwrite_metadata_cache (bool, optional): Whether to overwrite the metadata cache. Defaults to False.
         no_metadata_cache (bool, optional): Whether to skip using the metadata cache. Defaults to False.
 
     Returns:
         dict[str, Any]: A dictionary containing the retrieved metadata information.
     """  # noqa
@@ -39,14 +41,15 @@
     if not isinstance(contains, list):
         raise ValueError("contains must be of list type")
 
     catalogue_json = describe_function(
         include_description,
         include_datasets,
         include_keywords,
+        include_all_versions,
         contains,
         overwrite_metadata_cache,
         no_metadata_cache,
         disable_progress_bar,
         staging=staging,
     )
     catalogue = json.loads(catalogue_json)
```

### Comparing `copernicusmarine-1.1.1/copernicusmarine/python_interface/get.py` & `copernicusmarine-1.2.0/copernicusmarine/python_interface/get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/python_interface/load_utils.py` & `copernicusmarine-1.2.0/copernicusmarine/python_interface/load_utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/python_interface/open_dataset.py` & `copernicusmarine-1.2.0/copernicusmarine/python_interface/open_dataset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/python_interface/read_dataframe.py` & `copernicusmarine-1.2.0/copernicusmarine/python_interface/read_dataframe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/copernicusmarine/python_interface/subset.py` & `copernicusmarine-1.2.0/copernicusmarine/python_interface/subset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.1/pyproject.toml` & `copernicusmarine-1.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "copernicusmarine"
-version = "1.1.1"
+version = "1.2.0"
 description = ""
 authors = ["Copernicus Marine User Support <servicedesk.cmems@mercator-ocean.eu>"]
 readme = "README.md"
 packages = [{include = "copernicusmarine"}]
 license = "EUPL-1.2"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 click = ">=8.0.4"
 requests = ">=2.27.1"
-aiohttp = ">=3.8.5"
+aiohttp = ">=3.9.4"
 setuptools = ">=68.2.2"
 cachier = ">=2.2.1"
 xarray = ">=2023.4.0"
 tqdm = ">=4.65.0"
 zarr = ">=2.13.3"
 dask = ">=2022"
 netCDF4 = ">=1.5.4"
```

### Comparing `copernicusmarine-1.1.1/setup.py` & `copernicusmarine-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,559 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: copernicusmarine
+Version: 1.2.0
+Summary: 
+License: EUPL-1.2
+Author: Copernicus Marine User Support
+Author-email: servicedesk.cmems@mercator-ocean.eu
+Requires-Python: >=3.9,<3.13
+Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiohttp (>=3.9.4)
+Requires-Dist: boto3 (>=1.25)
+Requires-Dist: cachier (>=2.2.1)
+Requires-Dist: click (>=8.0.4)
+Requires-Dist: dask (>=2022)
+Requires-Dist: lxml (>=4.9.0)
+Requires-Dist: nest-asyncio (>=1.5.8)
+Requires-Dist: netCDF4 (>=1.5.4)
+Requires-Dist: pystac (>=1.8.3)
+Requires-Dist: requests (>=2.27.1)
+Requires-Dist: semver (>=3.0.2)
+Requires-Dist: setuptools (>=68.2.2)
+Requires-Dist: tqdm (>=4.65.0)
+Requires-Dist: xarray (>=2023.4.0)
+Requires-Dist: zarr (>=2.13.3)
+Description-Content-Type: text/markdown
 
-packages = \
-['copernicusmarine',
- 'copernicusmarine.aioretry',
- 'copernicusmarine.catalogue_parser',
- 'copernicusmarine.command_line_interface',
- 'copernicusmarine.core_functions',
- 'copernicusmarine.download_functions',
- 'copernicusmarine.python_interface']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiohttp>=3.8.5',
- 'boto3>=1.25',
- 'cachier>=2.2.1',
- 'click>=8.0.4',
- 'dask>=2022',
- 'lxml>=4.9.0',
- 'nest-asyncio>=1.5.8',
- 'netCDF4>=1.5.4',
- 'pystac>=1.8.3',
- 'requests>=2.27.1',
- 'semver>=3.0.2',
- 'setuptools>=68.2.2',
- 'tqdm>=4.65.0',
- 'xarray>=2023.4.0',
- 'zarr>=2.13.3']
-
-entry_points = \
-{'console_scripts': ['copernicusmarine = '
-                     'copernicusmarine.command_line_interface.copernicus_marine:command_line_interface']}
-
-setup_kwargs = {
-    'name': 'copernicusmarine',
-    'version': '1.1.1',
-    'description': '',
-    'long_description': '\n<h1 align="center">Copernicus Marine Service Toolbox (CLI & Python)</h1>\n<div align="center">\n  <a href="https://pypi.org/project/copernicusmarine/"><img src="https://img.shields.io/pypi/v/copernicusmarine.svg?style=flat-square" alt="PyPI" /></a>\n  <a href="https://pypi.org/project/copernicusmarine/"><img src="https://img.shields.io/pypi/pyversions/copernicusmarine.svg?style=flat-square" alt="PyPI Supported Versions" /></a>\n  <a href="https://pypi.org/project/copernicusmarine/"><img src="https://img.shields.io/badge/platform-windows | linux | macos-lightgrey?style=flat-square" alt="Supported Platforms" /></a>\n  <a href="https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12"><img src="https://img.shields.io/badge/licence-EUPL-lightblue?style=flat-square" alt="Licence" /></a>\n</div>\n\n![Copernicus Marine Service and Mercator Ocean international logos](https://www.mercator-ocean.eu/wp-content/uploads/2022/05/Cartouche_CMEMS_poisson_MOi.png)\n\n## Features\nThe `copernicusmarine` offers capabilities through both **Command Line Interface (CLI)** and **Python API**:\n- **Metadata Information**: List and retrieve metadata information on all variables, datasets, products, and their associated documentation.\n- **Subset Datasets**: Subset datasets to extract only the parts of interest, in preferred format, such as Analysis-Ready Cloud-Optimized (ARCO) Zarr or NetCDF file format.\n- **Advanced Filters**: Apply simple or advanced filters to get multiple files, in original formats like NetCDF/GeoTIFF, via direct Marine Data Store connections.\n- **No Quotas**: Enjoy no quotas, neither on volume size nor bandwidth.\n\n## Installation\nFor installation, multiple options are available depending on your setup:\n\n### Mamba | Conda\nA `conda` package is available on [Anaconda](https://anaconda.org/conda-forge/copernicusmarine).\n\nYou can install it using `mamba` (or conda) through the `conda-forge` channel with the following command:\n```bash\nmamba install conda-forge::copernicusmarine --yes\n```\n\nTo upgrade the Toolbox with mamba (or conda):\n```bash\nmamba update --name copernicusmarine copernicusmarine --yes\n```\n\n### Docker\nA docker image is also available here: [https://hub.docker.com/r/copernicusmarine/copernicusmarine](https://hub.docker.com/r/copernicusmarine/copernicusmarine)\n\nFirst step is to pull the container image:\n```bash\ndocker pull copernicusmarine/copernicusmarine:latest\n```\n\nThen run it:\n```bash\ndocker run -it --rm copernicusmarine/copernicusmarine --version\n```\n\n### Pip\nOtherwise, if you already have an environment (safer to clone it), the package can be installed using the `pip` command:\n```bash\npython -m pip install copernicusmarine\n```\n\nAnd to **upgrade the package** to the newest available version, run:\n```bash\npython -m pip install copernicusmarine --upgrade\n```\n\n## User Guide\nFor more comprehensive details on how to use the `copernicusmarine` Toolbox, please refer to our [Help Center](https://help.marine.copernicus.eu/en/collections/9054839-copernicus-marine-toolbox-guide). It ensures a smooth migration for existing users of legacy services such as MOTU, OPeNDAP or FTP.\n\n### General configuration\n\n#### Cache Usage\nCachier library is used for caching part of the requests (as result of `describe` or `login`). By default, the cache will be located in the home folder. If you need to change the location of the cache, you can set the environment variable `COPERNICUSMARINE_CACHE_DIRECTORY` to point to the desired directory:\n- on **UNIX** platforms: `export COPERNICUSMARINE_CACHE_DIRECTORY=<PATH>`\n- on **Windows** platforms: `set COPERNICUSMARINE_CACHE_DIRECTORY=<PATH>`\n\n### Network configuration\n\n#### Disable SSL\n\nA global SSL context is used when making HTTP calls using the `copernicusmarine` Toolbox. For some reason, it can lead to unexpected behavior depending on your network configuration. You can set the `COPERNICUSMARINE_DISABLE_SSL_CONTEXT` environment variable to any value to globally disable the usage of SSL in the toolbox:\n\n- on **UNIX** platforms: `export COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True`\n- on **Windows** platforms: `set COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True`\n\n#### Trust Env for python libraries\n\nTo do HTTP calls, the Copernicus Marine Toolbox uses two python libraries: requests and aiohttp. By default, those libraries will have `trust_env` values set to `True`. If you want to deactivate this, you can set `COPERNICUSMARINE_TRUST_ENV=False` (default `True`). This can be useful for example if you don\'t want those libraries to read your `.netrc` file as it has been reported that having a `.netrc` with a line: "default login anonymous password user@site" is incompatible with S3 connection required by the toolbox.\n\n#### Proxy\n\nTo use proxies, as describe in the [aiohttp documentation](https://docs.aiohttp.org/en/stable/client_advanced.html#proxy-support) you can use two options:\n\n- set the `HTTPS_PROXY` variable. For eg: `HTTPS_PROXY="http://user:pass@some.proxy.com"`. It should work even with `COPERNICUSMARINE_TRUST_ENV=False`.\n- use a `.netrc` file but be aware that having a line: "default login anonymous password user@site" is incompatible with S3 connection required by the toolbox. Also note that if you have `COPERNICUSMARINE_TRUST_ENV=True` (the default value) then if `NETRC` environment variable is set with a specified location, the `.netrc` file will be read from the specified location there rather than from `~/.netrc`.\n\n## Command Line Interface (CLI)\n\n### The `--help` option\nTo discover commands and their available options, consider appending `--help` on any command line.\n\nExample:\n```bash\ncopernicusmarine --help\n```\n\nReturns:\n```bash\nUsage: copernicusmarine [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  -V, --version  Show the version and exit.\n  -h, --help     Show this message and exit.\n\nCommands:\n  describe  Print Copernicus Marine catalog as JSON.\n  get       Download originally produced data files.\n  login     Create a configuration file with your Copernicus Marine credentials.\n  subset    Download subsets of datasets as NetCDF files or Zarr stores.\n```\n\n### Command `describe`\nRetrieve metadata information about all products/datasets and display as JSON output:\n```bash\ncopernicusmarine describe --include-datasets\n```\n\nThe JSON output can also be saved as follows:\n```bash\ncopernicusmarine describe --include-datasets > all_datasets_copernicusmarine.json\n```\n\n### Command `login`\nCreate a single configuration file `.copernicusmarine-credentials` allowing to access all Copernicus Marine Data Store data services. By default, the file is saved in user\'s home directory.\n\nExample:\n```bash\n> copernicusmarine login\nusername : johndoe\npassword :\nINFO - Configuration files stored in /Users/foo/.copernicusmarine\n```\n\nIf `.copernicusmarine-credentials` already exists, the user is asked for confirmation to overwrite (`--overwrite`/`--overwrite-configuration-file`).\n\nYou can use the `--skip-if-user-logged-in` option to skip the configuration file overwrite if the user is already logged in.\n\n#### Access points migration and evolution\nIf you still have a configuration for legacy services (e.g. `~/motuclient/motuclient-python.ini`, `~/.netrc` or `~/_netrc`) in your home directory, it will automatically be taken into account with commands `get` and `subset` without the need for running the `login` command.\nIf the configuration files are already available in another directory, when running commands `subset` or `get`, you can use the `--credentials-file` option to point to the files.\n\n### Command `subset`\nRemotely subset a dataset, based on variable names, geographical and temporal parameters.\n\nExample:\n```bash\ncopernicusmarine subset --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1D-m --variable thetao --variable so --start-datetime 2021-01-01 --end-datetime 2021-01-03 --minimum-longitude 0.0 --maximum-longitude 0.1 --minimum-latitude 28.0 --maximum-latitude 28.1\n```\nReturns:\n```bash\nINFO - 2024-04-03T10:18:18Z - <xarray.Dataset> Size: 3kB\nDimensions:    (depth: 50, latitude: 2, longitude: 1, time: 3)\nCoordinates:\n  * depth      (depth) float32 200B 0.5058 1.556 2.668 ... 5.292e+03 5.698e+03\n  * latitude   (latitude) float32 8B 28.0 28.08\n  * longitude  (longitude) float32 4B 0.08333\n  * time       (time) datetime64[ns] 24B 2021-01-01 2021-01-02 2021-01-03\nData variables:\n    thetao     (time, depth, latitude, longitude) float32 1kB dask.array<chunksize=(3, 1, 2, 1), meta=np.ndarray>\n    so         (time, depth, latitude, longitude) float32 1kB dask.array<chunksize=(3, 1, 2, 1), meta=np.ndarray>\nAttributes: (12/20)\n    Conventions:               CF-1.0\n    bulletin_date:             2020-12-01\n    ...                        ...\n    references:                http://marine.copernicus.eu\n    copernicusmarine_version:  1.1.0\nINFO - 2024-04-03T10:18:18Z - Estimated size of the dataset file is 0.002 MB.\n\nDo you want to proceed with download? [Y/n]:\n```\n\nBy default, after the display of the summary of the dataset subset, a download confirmation is asked. To skip this confirmation, use the option `--force-download`.\n\n#### Note about `--subset-method` option\nBy default, the `subset` feature uses the `nearest` method of xarray. By specifying `--subset-method strict`, you can only request dimension strictly inside the dataset, useful for **operational use-case**.\n\n#### Note about longitude range\nOptions `--minimum-longitude` and `--maximum-longitude` work as follows:\n- If the result of the substraction ( `--maximum-longitude` minus `--minimum-longitude` ) is superior or equal to 360, then return the full dataset.\n- If the requested longitude range:\n  - **does not cross** the antemeridian, then return the dataset between range -180 and 180.\n  - **does cross** the antemeridian, then return the dataset between range 0 and 360.\n\nNote that you can request any longitudes you want. A modulus is applied to bring the result between -180° and 360°. For example, if you request [530, 560], the result dataset will be in [170, 200].\n\n\n#### Note about `--netcdf-compression-enabled` and `--netcdf-compression-level` options\nWhen subsetting data, if you decide to write your data as a NetCDF file (which is the default behavior), then you can provide the extra option `--netcdf-compression-enabled`. The downloaded file will be lighter but it will take more time to write it (because of the compression task). If you don\'t provide it, the task will be faster, but the file heavier.\nOtherwise, if you decide to write your data in Zarr format (`.zarr` extension), the original compression used in the Copernicus Marine Data Store will be applied, which means that the download task will be fast **and** the file compressed. In that case, you cannot use the `--netcdf-compression-enabled`.\n\nHere are the default parameters added to xarray in the background when using the option: `{\'zlib\': True, \'complevel\': 1, \'contiguous\': False, \'shuffle\': True}`\n\nIn addition to this option, you can also provide the `--netcdf-compression-level` option and customize the NetCDF compression level between 0 (no compression) and 9 (maximal compression).\n\n#### Note about `--netcdf3-compatible` option\nThe `--netcdf3-compatible` option has been added to allow the downloaded dataset to be compatible with the netCDF3 format. It uses the `format="NETCDF3_CLASSIC"` of the xarray [to_netcdf](https://docs.xarray.dev/en/latest/generated/xarray.Dataset.to_netcdf.html) method.\n\n### Command `get`\nDownload the dataset file(s) as originally produced, based on the datasetID or the path to files.\n\nExample:\n```bash\ncopernicusmarine get --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --service original-files\n```\nReturns:\n```bash\nINFO - 2024-04-03T11:39:18Z - Dataset version was not specified, the latest one was selected: "202211"\nINFO - 2024-04-03T11:39:18Z - Dataset part was not specified, the first one was selected: "default"\nINFO - 2024-04-03T11:39:18Z - Service was not specified, the default one was selected: "original-files"\nINFO - 2024-04-03T11:39:18Z - Downloading using service original-files...\nINFO - 2024-04-03T11:39:19Z - You requested the download of the following files:\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_19930101_19931231_R20221101_RE01.nc - 8.83 MB - 2023-11-12T23:47:13Z\n[... truncated for brevity..]\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20120101_20121231_R20221101_RE01.nc - 8.62 MB - 2023-11-12T23:47:14Z\nPrinted 20 out of 29 files\n\nTotal size of the download: 252.94 MB\nDo you want to proceed with download? [Y/n]:\n```\n\nBy default:\n- After the header displays a summary of the request, a download confirmation is asked. To skip this user\'s action, add option `--force-download`.\n- Files are downloaded to the current directory applying the original folder structure. To avoid this behavior, add `--no-directories` and specify a destination with `-o/--output-directory`.\n\nOption `--show-outputnames` displays the full paths of the output files, if required.\n\nOption `--create-file-list` only creates a file containing the names of the targeted files instead of downloading them. You have to input a file name, e.g. `--create-file-list my_files.txt`. The format needs to be `.txt` or `.csv`:\n\n- If the user inputs a filename that ends in `.txt`, then the file contains only the full s3 path to the targeted files and is compatible with the `--file-list` option.\n\nExample:\n```bash\ncopernicusmarine get --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m --filter "*2021*" --create-file-list selected_files_for_2021.txt\n```\nThe content of `selected_files_for_2021.txt` would be:\n```\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210101_20210131_R20230101_RE01.nc\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210201_20210228_R20230101_RE01.nc\n[... truncated for brevity..]\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211101_20211130_R20230101_RE01.nc\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211201_20211231_R20230101_RE01.nc\n```\n\n- If the user inputs a filename that ends in `.csv` the file contains the following columns, separated by a comma: `filename`, `size` (in Bytes), `last_modified_datetime`, and `etag`. It is **not** compatible "as is" with the `--file-list` option and would need further post-processing from user\'s side.\n\nExample:\n```bash\ncopernicusmarine get --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m --filter "*2021*" --create-file-list selected_files_for_2021.csv\n```\n The content of `selected_files_for_2021.csv` would be:\n```\nfilename,size,last_modified_datetime,etag\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210101_20210131_R20230101_RE01.nc,12295906,2023-11-12 23:47:05.466000+00:00,"e8a7e564f676a08bf601bcdeaebdc563"\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210201_20210228_R20230101_RE01.nc,12436177,2023-11-12 23:47:05.540000+00:00,"d4a22dfb6c7ed85860c4a122c45eb953"\n[... truncated for brevity..]\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211101_20211130_R20230101_RE01.nc,12386940,2023-11-12 23:47:06.358000+00:00,"ea15d1f70fcc7f2ce404184d983530ff"\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211201_20211231_R20230101_RE01.nc,12398208,2023-11-12 23:47:06.456000+00:00,"585f49867aaefa2ce9d6e68dd468b5e1"\n```\nIf specified, no other action will be performed.\n\n\n#### Note about sync option\nOption `--sync` allows to download original files only if not exist and not up to date. The Toolbox checks the destination folder against the source folder. It can be combined with filters. Note that if set with `--overwrite-output-data`, the latter will be ignored.\nThe logic is largely inspired from [s5cmd package sync command](https://github.com/peak/s5cmd#sync).\nOption `--sync-delete` will work as `--sync` with the added fonctionnality that it deletes any local file that has not been found on the remote server. Note that the files found on the server are also filtered. Hence, a file present locally might be deleted even if it is on the server because, for example, the executed `get` command contains a filter that excludes this specific file.\n\nLimitations:\n- `--sync` is not compatible with `--no-directories`.\n- `--sync` only works with `--dataset-version`.\n- `--sync` functionality is not available for datasets with several parts (like INSITU or static datasets for example).\n\n#### Note about filtering options\nOption `--filter` allows to specify a Unix shell-style wildcard pattern (see [fnmatch — Unix filename pattern matching](https://docs.python.org/3/library/fnmatch.html)) and select specific files:\n```bash\ncopernicusmarine get --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --filter "*01yav_200[0-2]*"\n```\nReturns:\n```bash\nINFO - 2024-04-03T11:51:15Z - Dataset version was not specified, the latest one was selected: "202211"\nINFO - 2024-04-03T11:51:15Z - Dataset part was not specified, the first one was selected: "default"\nINFO - 2024-04-03T11:51:15Z - Service was not specified, the default one was selected: "original-files"\nINFO - 2024-04-03T11:51:15Z - Downloading using service original-files...\nINFO - 2024-04-03T11:51:17Z - You requested the download of the following files:\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB\n\nTotal size of the download: 26.59 MB\nDo you want to proceed with download? [Y/n]:\n```\n\nOption `--regex` allows to specify a regular expression for more advanced files selection:\n\n```bash\ncopernicusmarine get -i cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --regex ".*01yav_20(00|01|02).*.nc"\n```\nReturns:\n```bash\nINFO - 2024-04-03T11:52:43Z - Dataset version was not specified, the latest one was selected: "202211"\nINFO - 2024-04-03T11:52:43Z - Dataset part was not specified, the first one was selected: "default"\nINFO - 2024-04-03T11:52:43Z - Service was not specified, the default one was selected: "original-files"\nINFO - 2024-04-03T11:52:43Z - Downloading using service original-files...\nINFO - 2024-04-03T11:52:44Z - You requested the download of the following files:\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB - 2023-11-12T23:47:13Z\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB - 2023-11-12T23:47:13Z\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB - 2023-11-12T23:47:13Z\n\nTotal size of the download: 26.59 MB\nDo you want to proceed with download? [Y/n]:\n```\n\nOption `--file-list` allows to specify a list of files for more advanced files selection.\nThe file can contain complete absolute paths for each target file (default behavior) or only a partial path defined by the user, as shown below.\n\nExample of `file_list.txt` with absolute paths:\n```txt\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210101_20210131_R20230101_RE01.nc\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210201_20210228_R20230101_RE01.nc\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210301_20210331_R20230101_RE01.nc\n```\n\nExample of `file_list.txt` with partial paths matching the absolute paths (equivalent to previous example):\n```txt\nCMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc\nCMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc\nCMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc\n```\n> **_NOTE:_** This option is compatible with the file generated by the `--create-file-list` option if you generated a ".txt" file.\n\nThen the following command:\n```bash\ncopernicusmarine get -i cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --file-list file_list.txt\n```\nReturns:\n```bash\nINFO - 2024-04-03T12:57:44Z - Dataset version was not specified, the latest one was selected: "202211"\nINFO - 2024-04-03T12:57:44Z - Dataset part was not specified, the first one was selected: "default"\nINFO - 2024-04-03T12:57:44Z - Service was not specified, the default one was selected: "original-files"\nINFO - 2024-04-03T12:57:44Z - Downloading using service original-files...\nINFO - 2024-04-03T12:57:45Z - You requested the download of the following files:\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB - 2023-11-12T23:47:13Z\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB - 2023-11-12T23:47:13Z\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB - 2023-11-12T23:47:13Z\n\nTotal size of the download: 26.59 MB\nDo you want to proceed with download? [Y/n]:\n```\n\nAlso, there is a specific command `--index-parts` to retrieve the index files of INSITU datasets (as listed on the [Copernicus Marine File Browser](https://data.marine.copernicus.eu/product/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/files?subdataset=cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311--ext--history&path=INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034%2Fcmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311%2F)).\n> **_NOTE:_** In the future, it is planned to have the index files for those datasets directly available through the `--filter`, `--regex` and/or `--file-list` options. Meanwhile, check this [Help Center article for a working example](https://help.marine.copernicus.eu/en/articles/9133855-how-to-download-insitu-data-using-index-files).\n\n\nThen the following command:\n```\ncopernicusmarine get --dataset-id cmems_obs-ins_blk_phybgcwav_mynrt_na_irr --index-parts\n```\nReturns:\n```\nINFO - 2024-04-03T12:58:40Z - Dataset version was not specified, the latest one was selected: "202311"\nINFO - 2024-04-03T12:58:40Z - Dataset part was not specified, the first one was selected: "history"\nINFO - 2024-04-03T12:58:40Z - You forced selection of service: original-files\nINFO - 2024-04-03T12:58:40Z - Downloading using service original-files...\nINFO - 2024-04-03T12:58:41Z - You requested the download of the following files:\ns3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_history.txt - 333.13 kB - 2024-04-02T08:40:30Z\ns3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_latest.txt - 466.38 kB - 2024-04-03T12:51:52Z\ns3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_monthly.txt - 1.51 MB - 2024-03-05T18:09:43Z\ns3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_platform.txt - 209.27 kB - 2024-04-03T08:33:37Z\n\nTotal size of the download: 2.52 MB\nDo you want to proceed with download? [Y/n]:\n```\n\n### Shared options\nBoth `subset` and `get` commands provide these options:\n\n#### Option `--overwrite-output-data`\nWhen specified, the existing files will be overwritten.\nOtherwise, if the files already exist on destination, new ones with a unique index will be created once the download has been accepted (or once `--force-download` is provided).\n\n#### Option `--create-template`\nOption to create a file in your current directory containing request parameters. If specified, no other action will be performed.\nIt will create the following files depending on the feature:\n- `subset`\nExample:\n```bash\ncopernicusmarine subset --create-template\n```\nReturns:\n```txt\nINFO - 2024-04-04T14:38:09Z - Template created at: subset_template.json\n```\n- `get`\nExample:\n```bash\ncopernicusmarine get --create-template\n```\nReturns:\n```txt\nINFO - 2024-04-04T14:38:09Z - Template created at: get_template.json\n```\n\n#### Option `--request-file`\nThis option allows to specify request parameters but in a provided `.json` file, useful for batch processing.\nYou can try the following templates or use the `--create-template` option to create both `subset` or `get` template request files.\n\n- Template for `subset` data request:\n```json\n{\n    "dataset_id": "cmems_mod_glo_phy-thetao_anfc_0.083deg_P1D-m",\n    "start_datetime": "2022-04-11",\n    "end_datetime": "2023-08-11",\n    "minimum_longitude": -182.79,\n    "maximum_longitude": -179.69,\n    "minimum_latitude": -40,\n    "maximum_latitude": -36,\n    "minimum_depth": 0,\n    "maximum_depth": 0,\n    "variables": ["thetao"],\n    "output_directory": "./data/",\n    "force_download": true\n}\n```\n\nExample:\n```bash\ncopernicusmarine subset --request-file template_subset_data_request.json\n```\n\n- Template for `get` data request:\n```json\n{\n    "dataset_id": "cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m",\n    "filter": "*01yav_200[0-2]*",\n    "force_download": false,\n    "log_level": "INFO",\n    "no_directories": false,\n    "no_metadata_cache": false,\n    "output_directory": "./data/",\n    "overwrite_output_data": false,\n    "overwrite_metadata_cache": false,\n    "show_outputnames": true\n}\n```\n\nExample:\n```bash\ncopernicusmarine get --request-file template_get_data_request.json\n```\n\n#### Option `--credentials-file`\nYou can use the `--credentials-file` option to point to a credentials file. The file can be either `.copernicusmarine-credentials`, `motuclient-python.ini`, `.netrc` or `_netrc`.\n\n#### Option `--dataset-version`\nYou can use the `--dataset-version` option to fetch a specific dataset version. Particularly useful to keep an operational chain working when an evolution impact the chosen dataset.\n\n#### Option `--dataset-part`\nYou can use the `--dataset-part` option to fecth a specific part for the chosen dataset version.\n\n#### Option `--log-level`\nSet the details printed to console by the command (based on standard logging library).\nAvailable values are: `[DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]`\n\n## Python package (API)\nThe `copernicusmarine` exposes a Python interface to allow you to [call commands as functions](https://marine.copernicus.eu/python-interface).\n\n## Documentation\nA detailed standalone API documentation is under construction and will come at a later stage. For the moment, see the [Help Center](https://help.marine.copernicus.eu/en/collections/9054839-copernicus-marine-toolbox-guide).\n\n## Contribution\nWe welcome contributions from the community to enhance this package. If you find any issues or have suggestions for improvements, please check out our [Report Template](https://help.marine.copernicus.eu/en/articles/8218546-reporting-an-issue-or-feature-request).\n\n## Future improvements & Roadmap\nTo keep up to date with the most recent and planned advancements, including revisions, corrections, and feature requests generated from users\' feedback, please refer to our [Roadmap](https://help.marine.copernicus.eu/en/articles/8218641-next-milestones-and-roadmap).\n\n## Join the community\nGet in touch!\n- Create your [Copernicus Marine Account](https://data.marine.copernicus.eu/register?redirect=%2Fproducts)\n- [Log in](https://data.marine.copernicus.eu/login?redirect=%2Fproducts) and chat with us (bottom right corner of [Copernicus Marine Service](https://marine.copernicus.eu/))\n- Join our [training workshops](https://marine.copernicus.eu/services/user-learning-services)\n- Network y/our [Copernicus Stories](https://twitter.com/cmems_eu)\n- Watch [our videos](https://www.youtube.com/channel/UC71ceOVy7WtVC7F04BKoEew)\n## Licence\nLicensed under the [EUPL](https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12)\n',
-    'author': 'Copernicus Marine User Support',
-    'author_email': 'servicedesk.cmems@mercator-ocean.eu',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<3.13',
+
+<h1 align="center">Copernicus Marine Service Toolbox (CLI & Python)</h1>
+<div align="center">
+  <a href="https://pypi.org/project/copernicusmarine/"><img src="https://img.shields.io/pypi/v/copernicusmarine.svg?style=flat-square" alt="PyPI" /></a>
+  <a href="https://pypi.org/project/copernicusmarine/"><img src="https://img.shields.io/pypi/pyversions/copernicusmarine.svg?style=flat-square" alt="PyPI Supported Versions" /></a>
+  <a href="https://pypi.org/project/copernicusmarine/"><img src="https://img.shields.io/badge/platform-windows | linux | macos-lightgrey?style=flat-square" alt="Supported Platforms" /></a>
+  <a href="https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12"><img src="https://img.shields.io/badge/licence-EUPL-lightblue?style=flat-square" alt="Licence" /></a>
+</div>
+
+![Copernicus Marine Service and Mercator Ocean international logos](https://www.mercator-ocean.eu/wp-content/uploads/2022/05/Cartouche_CMEMS_poisson_MOi.png)
+
+## Features
+The `copernicusmarine` offers capabilities through both **Command Line Interface (CLI)** and **Python API**:
+- **Metadata Information**: List and retrieve metadata information on all variables, datasets, products, and their associated documentation.
+- **Subset Datasets**: Subset datasets to extract only the parts of interest, in preferred format, such as Analysis-Ready Cloud-Optimized (ARCO) Zarr or NetCDF file format.
+- **Advanced Filters**: Apply simple or advanced filters to get multiple files, in original formats like NetCDF/GeoTIFF, via direct Marine Data Store connections.
+- **No Quotas**: Enjoy no quotas, neither on volume size nor bandwidth.
+
+## Installation
+For installation, multiple options are available depending on your setup:
+
+### Mamba | Conda
+A `conda` package is available on [Anaconda](https://anaconda.org/conda-forge/copernicusmarine).
+
+You can install it using `mamba` (or conda) through the `conda-forge` channel with the following command:
+```bash
+mamba install conda-forge::copernicusmarine --yes
+```
+
+To upgrade the Toolbox with mamba (or conda):
+```bash
+mamba update --name copernicusmarine copernicusmarine --yes
+```
+
+### Docker
+A docker image is also available here: [https://hub.docker.com/r/copernicusmarine/copernicusmarine](https://hub.docker.com/r/copernicusmarine/copernicusmarine)
+
+First step is to pull the container image:
+```bash
+docker pull copernicusmarine/copernicusmarine:latest
+```
+
+Then run it:
+```bash
+docker run -it --rm copernicusmarine/copernicusmarine --version
+```
+
+### Pip
+Otherwise, if you already have an environment (safer to clone it), the package can be installed using the `pip` command:
+```bash
+python -m pip install copernicusmarine
+```
+
+And to **upgrade the package** to the newest available version, run:
+```bash
+python -m pip install copernicusmarine --upgrade
+```
+
+## User Guide
+For more comprehensive details on how to use the `copernicusmarine` Toolbox, please refer to our [Help Center](https://help.marine.copernicus.eu/en/collections/9080063-copernicus-marine-toolbox). It ensures a smooth migration for existing users of legacy services such as MOTU, OPeNDAP or FTP.
+
+### General configuration
+
+#### Cache Usage
+Cachier library is used for caching part of the requests (as result of `describe` or `login`). By default, the cache will be located in the home folder. If you need to change the location of the cache, you can set the environment variable `COPERNICUSMARINE_CACHE_DIRECTORY` to point to the desired directory:
+- on **UNIX** platforms: `export COPERNICUSMARINE_CACHE_DIRECTORY=<PATH>`
+- on **Windows** platforms: `set COPERNICUSMARINE_CACHE_DIRECTORY=<PATH>`
+
+### Network configuration
+
+#### Disable SSL
+
+A global SSL context is used when making HTTP calls using the `copernicusmarine` Toolbox. For some reason, it can lead to unexpected behavior depending on your network configuration. You can set the `COPERNICUSMARINE_DISABLE_SSL_CONTEXT` environment variable to any value to globally disable the usage of SSL in the toolbox:
+
+- on **UNIX** platforms: `export COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True`
+- on **Windows** platforms: `set COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True`
+
+#### Trust Env for python libraries
+
+To do HTTP calls, the Copernicus Marine Toolbox uses two python libraries: requests and aiohttp. By default, those libraries will have `trust_env` values set to `True`. If you want to deactivate this, you can set `COPERNICUSMARINE_TRUST_ENV=False` (default `True`). This can be useful for example if you don't want those libraries to read your `.netrc` file as it has been reported that having a `.netrc` with a line: "default login anonymous password user@site" is incompatible with S3 connection required by the toolbox.
+
+#### Proxy
+
+To use proxies, as describe in the [aiohttp documentation](https://docs.aiohttp.org/en/stable/client_advanced.html#proxy-support) you can use two options:
+
+- set the `HTTPS_PROXY` variable. For eg: `HTTPS_PROXY="http://user:pass@some.proxy.com"`. It should work even with `COPERNICUSMARINE_TRUST_ENV=False`.
+- use a `.netrc` file but be aware that having a line: "default login anonymous password user@site" is incompatible with S3 connection required by the toolbox. Also note that if you have `COPERNICUSMARINE_TRUST_ENV=True` (the default value) then if `NETRC` environment variable is set with a specified location, the `.netrc` file will be read from the specified location there rather than from `~/.netrc`.
+
+#### Number of concurrent requests
+
+The toolbox makes many requests to STAC to be able to parse the full marine data store STAC catalog. For that, it uses asynchronous calls. It can be problematic to do too many requests at the same time. To limit the number of requests at the same time you can use: `COPERNICUSMARINE_MAX_CONCURRENT_REQUESTS`. The default value is `15` and minimum value is `1`.
+
+Note, that this concerns only the catalog parsing step so the describe command and the start of the get and subset command. It does not apply when downloading files or listing files from the get command or when requesting the data chunks for the subset command.
+
+## Command Line Interface (CLI)
+
+### The `--help` option
+To discover commands and their available options, consider appending `--help` on any command line.
+
+Example:
+```bash
+copernicusmarine --help
+```
+
+Returns:
+```bash
+Usage: copernicusmarine [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  -V, --version  Show the version and exit.
+  -h, --help     Show this message and exit.
+
+Commands:
+  describe  Print Copernicus Marine catalog as JSON.
+  get       Download originally produced data files.
+  login     Create a configuration file with your Copernicus Marine credentials.
+  subset    Download subsets of datasets as NetCDF files or Zarr stores.
+```
+
+### Command `describe`
+Retrieve metadata information about all products/datasets and display as JSON output:
+```bash
+copernicusmarine describe --include-datasets
+```
+
+The JSON output can also be saved as follows:
+```bash
+copernicusmarine describe --include-datasets > all_datasets_copernicusmarine.json
+```
+
+### Command `login`
+Create a single configuration file `.copernicusmarine-credentials` allowing to access all Copernicus Marine Data Store data services. By default, the file is saved in user's home directory.
+
+Example:
+```bash
+> copernicusmarine login
+username : johndoe
+password :
+INFO - Configuration files stored in /Users/foo/.copernicusmarine
+```
+
+If `.copernicusmarine-credentials` already exists, the user is asked for confirmation to overwrite (`--overwrite`/`--overwrite-configuration-file`).
+
+You can use the `--skip-if-user-logged-in` option to skip the configuration file overwrite if the user is already logged in.
+
+#### Access points migration and evolution
+If you still have a configuration for legacy services (e.g. `~/motuclient/motuclient-python.ini`, `~/.netrc` or `~/_netrc`) in your home directory, it will automatically be taken into account with commands `get` and `subset` without the need for running the `login` command.
+If the configuration files are already available in another directory, when running commands `subset` or `get`, you can use the `--credentials-file` option to point to the files.
+
+### Command `subset`
+Remotely subset a dataset, based on variable names, geographical and temporal parameters.
+
+Example:
+```bash
+copernicusmarine subset --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1D-m --variable thetao --variable so --start-datetime 2021-01-01 --end-datetime 2021-01-03 --minimum-longitude 0.0 --maximum-longitude 0.1 --minimum-latitude 28.0 --maximum-latitude 28.1
+```
+Returns:
+```bash
+INFO - 2024-04-03T10:18:18Z - <xarray.Dataset> Size: 3kB
+Dimensions:    (depth: 50, latitude: 2, longitude: 1, time: 3)
+Coordinates:
+  * depth      (depth) float32 200B 0.5058 1.556 2.668 ... 5.292e+03 5.698e+03
+  * latitude   (latitude) float32 8B 28.0 28.08
+  * longitude  (longitude) float32 4B 0.08333
+  * time       (time) datetime64[ns] 24B 2021-01-01 2021-01-02 2021-01-03
+Data variables:
+    thetao     (time, depth, latitude, longitude) float32 1kB dask.array<chunksize=(3, 1, 2, 1), meta=np.ndarray>
+    so         (time, depth, latitude, longitude) float32 1kB dask.array<chunksize=(3, 1, 2, 1), meta=np.ndarray>
+Attributes: (12/20)
+    Conventions:               CF-1.0
+    bulletin_date:             2020-12-01
+    ...                        ...
+    references:                http://marine.copernicus.eu
+    copernicusmarine_version:  1.1.0
+INFO - 2024-04-03T10:18:18Z - Estimated size of the dataset file is 0.002 MB.
+
+Do you want to proceed with download? [Y/n]:
+```
+
+By default, after the display of the summary of the dataset subset, a download confirmation is asked. To skip this confirmation, use the option `--force-download`.
+
+#### Note about `--subset-method` option
+By default, the `subset` feature uses the `nearest` method of xarray. By specifying `--subset-method strict`, you can only request dimension strictly inside the dataset, useful for **operational use-case**.
+
+#### Note about longitude range
+Options `--minimum-longitude` and `--maximum-longitude` work as follows:
+- If the result of the substraction ( `--maximum-longitude` minus `--minimum-longitude` ) is superior or equal to 360, then return the full dataset.
+- If the requested longitude range:
+  - **does not cross** the antemeridian, then return the dataset between range -180 and 180.
+  - **does cross** the antemeridian, then return the dataset between range 0 and 360.
+
+Note that you can request any longitudes you want. A modulus is applied to bring the result between -180° and 360°. For example, if you request [530, 560], the result dataset will be in [170, 200].
+
+
+#### Note about `--netcdf-compression-enabled` and `--netcdf-compression-level` options
+When subsetting data, if you decide to write your data as a NetCDF file (which is the default behavior), then you can provide the extra option `--netcdf-compression-enabled`. The downloaded file will be lighter but it will take more time to write it (because of the compression task). If you don't provide it, the task will be faster, but the file heavier.
+Otherwise, if you decide to write your data in Zarr format (`.zarr` extension), the original compression used in the Copernicus Marine Data Store will be applied, which means that the download task will be fast **and** the file compressed. In that case, you cannot use the `--netcdf-compression-enabled`.
+
+Here are the default parameters added to xarray in the background when using the option: `{'zlib': True, 'complevel': 1, 'contiguous': False, 'shuffle': True}`
+
+In addition to this option, you can also provide the `--netcdf-compression-level` option and customize the NetCDF compression level between 0 (no compression) and 9 (maximal compression).
+
+#### Note about `--netcdf3-compatible` option
+The `--netcdf3-compatible` option has been added to allow the downloaded dataset to be compatible with the netCDF3 format. It uses the `format="NETCDF3_CLASSIC"` of the xarray [to_netcdf](https://docs.xarray.dev/en/latest/generated/xarray.Dataset.to_netcdf.html) method.
+
+### Command `get`
+Download the dataset file(s) as originally produced, based on the datasetID or the path to files.
+
+Example:
+```bash
+copernicusmarine get --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --service original-files
+```
+Returns:
+```bash
+INFO - 2024-04-03T11:39:18Z - Dataset version was not specified, the latest one was selected: "202211"
+INFO - 2024-04-03T11:39:18Z - Dataset part was not specified, the first one was selected: "default"
+INFO - 2024-04-03T11:39:18Z - Service was not specified, the default one was selected: "original-files"
+INFO - 2024-04-03T11:39:18Z - Downloading using service original-files...
+INFO - 2024-04-03T11:39:19Z - You requested the download of the following files:
+s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_19930101_19931231_R20221101_RE01.nc - 8.83 MB - 2023-11-12T23:47:13Z
+[... truncated for brevity..]
+s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20120101_20121231_R20221101_RE01.nc - 8.62 MB - 2023-11-12T23:47:14Z
+Printed 20 out of 29 files
+
+Total size of the download: 252.94 MB
+Do you want to proceed with download? [Y/n]:
+```
+
+By default:
+- After the header displays a summary of the request, a download confirmation is asked. To skip this user's action, add option `--force-download`.
+- Files are downloaded to the current directory applying the original folder structure. To avoid this behavior, add `--no-directories` and specify a destination with `-o/--output-directory`.
+
+Option `--show-outputnames` displays the full paths of the output files, if required.
+
+Option `--create-file-list` only creates a file containing the names of the targeted files instead of downloading them. You have to input a file name, e.g. `--create-file-list my_files.txt`. The format needs to be `.txt` or `.csv`:
+
+- If the user inputs a filename that ends in `.txt`, then the file contains only the full s3 path to the targeted files and is compatible with the `--file-list` option.
+
+Example:
+```bash
+copernicusmarine get --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m --filter "*2021*" --create-file-list selected_files_for_2021.txt
+```
+The content of `selected_files_for_2021.txt` would be:
+```
+s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210101_20210131_R20230101_RE01.nc
+s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210201_20210228_R20230101_RE01.nc
+[... truncated for brevity..]
+s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211101_20211130_R20230101_RE01.nc
+s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211201_20211231_R20230101_RE01.nc
+```
+
+- If the user inputs a filename that ends in `.csv` the file contains the following columns, separated by a comma: `filename`, `size` (in Bytes), `last_modified_datetime`, and `etag`. It is **not** compatible "as is" with the `--file-list` option and would need further post-processing from user's side.
+
+Example:
+```bash
+copernicusmarine get --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m --filter "*2021*" --create-file-list selected_files_for_2021.csv
+```
+ The content of `selected_files_for_2021.csv` would be:
+```
+filename,size,last_modified_datetime,etag
+s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210101_20210131_R20230101_RE01.nc,12295906,2023-11-12 23:47:05.466000+00:00,"e8a7e564f676a08bf601bcdeaebdc563"
+s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210201_20210228_R20230101_RE01.nc,12436177,2023-11-12 23:47:05.540000+00:00,"d4a22dfb6c7ed85860c4a122c45eb953"
+[... truncated for brevity..]
+s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211101_20211130_R20230101_RE01.nc,12386940,2023-11-12 23:47:06.358000+00:00,"ea15d1f70fcc7f2ce404184d983530ff"
+s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211201_20211231_R20230101_RE01.nc,12398208,2023-11-12 23:47:06.456000+00:00,"585f49867aaefa2ce9d6e68dd468b5e1"
+```
+If specified, no other action will be performed.
+
+
+#### Note about sync option
+Option `--sync` allows to download original files only if not exist and not up to date. The Toolbox checks the destination folder against the source folder. It can be combined with filters. Note that if set with `--overwrite-output-data`, the latter will be ignored.
+The logic is largely inspired from [s5cmd package sync command](https://github.com/peak/s5cmd#sync).
+Option `--sync-delete` will work as `--sync` with the added fonctionnality that it deletes any local file that has not been found on the remote server. Note that the files found on the server are also filtered. Hence, a file present locally might be deleted even if it is on the server because, for example, the executed `get` command contains a filter that excludes this specific file.
+
+Limitations:
+- `--sync` is not compatible with `--no-directories`.
+- `--sync` only works with `--dataset-version`.
+- `--sync` functionality is not available for datasets with several parts (like INSITU or static datasets for example).
+
+#### Note about filtering options
+Option `--filter` allows to specify a Unix shell-style wildcard pattern (see [fnmatch — Unix filename pattern matching](https://docs.python.org/3/library/fnmatch.html)) and select specific files:
+```bash
+copernicusmarine get --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --filter "*01yav_200[0-2]*"
+```
+Returns:
+```bash
+INFO - 2024-04-03T11:51:15Z - Dataset version was not specified, the latest one was selected: "202211"
+INFO - 2024-04-03T11:51:15Z - Dataset part was not specified, the first one was selected: "default"
+INFO - 2024-04-03T11:51:15Z - Service was not specified, the default one was selected: "original-files"
+INFO - 2024-04-03T11:51:15Z - Downloading using service original-files...
+INFO - 2024-04-03T11:51:17Z - You requested the download of the following files:
+s3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB
+s3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB
+s3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB
+
+Total size of the download: 26.59 MB
+Do you want to proceed with download? [Y/n]:
+```
+
+Option `--regex` allows to specify a regular expression for more advanced files selection:
+
+```bash
+copernicusmarine get -i cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --regex ".*01yav_20(00|01|02).*.nc"
+```
+Returns:
+```bash
+INFO - 2024-04-03T11:52:43Z - Dataset version was not specified, the latest one was selected: "202211"
+INFO - 2024-04-03T11:52:43Z - Dataset part was not specified, the first one was selected: "default"
+INFO - 2024-04-03T11:52:43Z - Service was not specified, the default one was selected: "original-files"
+INFO - 2024-04-03T11:52:43Z - Downloading using service original-files...
+INFO - 2024-04-03T11:52:44Z - You requested the download of the following files:
+s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB - 2023-11-12T23:47:13Z
+s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB - 2023-11-12T23:47:13Z
+s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB - 2023-11-12T23:47:13Z
+
+Total size of the download: 26.59 MB
+Do you want to proceed with download? [Y/n]:
+```
+
+#### Notes about the file list option
+
+Option `--file-list` allows to specify a list of files for more advanced files selection.
+The file can contain complete absolute paths for each target file (default behavior) or only a partial path defined by the user, as shown below.
+
+By default, the get functionality lists all the files on the bucket to be able to select the requested ones. This create some overhead when there are a lot of files for a specific dataset. For example, a dataset with more than 100 000 files would create an overhead of around two minutes. The file list option will directly download the files and avoid the listings if all the files listed are found.
+
+Careful, a path can easily be mispelled or wrongly queried. The toolbox will display a warning if the file is not found on the bucket and try to find the file by listing all the files on the bucket.
+
+Example of `file_list.txt` with paths that would be directly downloaded without the listing overhead:
+
+```txt
+# correct paths
+> s3://mdl-native-01/native/INSITU_GLO_PHYBGCWAV_DISCRETE_MYNRT_013_030/cmems_obs-ins_glo_phybgcwav_mynrt_na_irr_202311/history/BO/AR_PR_BO_58JM.nc
+> INSITU_GLO_PHYBGCWAV_DISCRETE_MYNRT_013_030/cmems_obs-ins_glo_phybgcwav_mynrt_na_irr_202311/history/BO/AR_PR_BO_58JM.nc
+> cmems_obs-ins_glo_phybgcwav_mynrt_na_irr_202311/history/BO/AR_PR_BO_58JM.nc
+> history/BO/AR_PR_BO_58JM.nc
+> index_history.txt
+
+# incorrect paths
+# version is missing
+> INSITU_GLO_PHYBGCWAV_DISCRETE_MYNRT_013_030/cmems_obs-ins_glo_phybgcwav_mynrt_na_irr/history/BO/AR_PR_BO_58JM.nc
+# only the file name and not the path to the file
+> AR_PR_BO_58JM.nc
+# not the same dataset
+> another_dataset/history/BO/AR_PR_BO_58JM.nc
+```
+
+Example of `file_list.txt` with absolute paths:
+
+```txt
+s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210101_20210131_R20230101_RE01.nc
+s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210201_20210228_R20230101_RE01.nc
+s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210301_20210331_R20230101_RE01.nc
+```
+
+Example of `file_list.txt` with partial paths matching the absolute paths (equivalent to previous example):
+
+```txt
+CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc
+CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc
+CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc
+```
+
+> **_NOTE:_** This option is compatible with the file generated by the `--create-file-list` option if you generated a ".txt" file.
+
+Then the following command:
+```bash
+copernicusmarine get -i cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --file-list file_list.txt
+```
+Returns:
+```bash
+INFO - 2024-04-03T12:57:44Z - Dataset version was not specified, the latest one was selected: "202211"
+INFO - 2024-04-03T12:57:44Z - Dataset part was not specified, the first one was selected: "default"
+INFO - 2024-04-03T12:57:44Z - Service was not specified, the default one was selected: "original-files"
+INFO - 2024-04-03T12:57:44Z - Downloading using service original-files...
+INFO - 2024-04-03T12:57:45Z - You requested the download of the following files:
+s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB - 2023-11-12T23:47:13Z
+s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB - 2023-11-12T23:47:13Z
+s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB - 2023-11-12T23:47:13Z
+
+Total size of the download: 26.59 MB
+Do you want to proceed with download? [Y/n]:
+```
+
+Also, there is a specific command `--index-parts` to retrieve the index files of INSITU datasets (as listed on the [Copernicus Marine File Browser](https://data.marine.copernicus.eu/product/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/files?subdataset=cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311--ext--history&path=INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034%2Fcmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311%2F)).
+> **_NOTE:_** In the future, it is planned to have the index files for those datasets directly available through the `--filter`, `--regex` and/or `--file-list` options. Meanwhile, check this [Help Center article for a working example](https://help.marine.copernicus.eu/en/articles/9133855-how-to-download-insitu-data-using-index-files).
+
+
+Then the following command:
+```
+copernicusmarine get --dataset-id cmems_obs-ins_blk_phybgcwav_mynrt_na_irr --index-parts
+```
+Returns:
+```
+INFO - 2024-04-03T12:58:40Z - Dataset version was not specified, the latest one was selected: "202311"
+INFO - 2024-04-03T12:58:40Z - Dataset part was not specified, the first one was selected: "history"
+INFO - 2024-04-03T12:58:40Z - You forced selection of service: original-files
+INFO - 2024-04-03T12:58:40Z - Downloading using service original-files...
+INFO - 2024-04-03T12:58:41Z - You requested the download of the following files:
+s3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_history.txt - 333.13 kB - 2024-04-02T08:40:30Z
+s3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_latest.txt - 466.38 kB - 2024-04-03T12:51:52Z
+s3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_monthly.txt - 1.51 MB - 2024-03-05T18:09:43Z
+s3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_platform.txt - 209.27 kB - 2024-04-03T08:33:37Z
+
+Total size of the download: 2.52 MB
+Do you want to proceed with download? [Y/n]:
+```
+
+### Shared options
+
+Both `subset` and `get` commands provide these options:
+
+#### Option `--overwrite-output-data`
+
+When specified, the existing files will be overwritten.
+Otherwise, if the files already exist on destination, new ones with a unique index will be created once the download has been accepted (or once `--force-download` is provided).
+
+#### Option `--create-template`
+Option to create a file in your current directory containing request parameters. If specified, no other action will be performed.
+It will create the following files depending on the feature:
+- `subset`
+Example:
+```bash
+copernicusmarine subset --create-template
+```
+Returns:
+```txt
+INFO - 2024-04-04T14:38:09Z - Template created at: subset_template.json
+```
+- `get`
+Example:
+```bash
+copernicusmarine get --create-template
+```
+Returns:
+```txt
+INFO - 2024-04-04T14:38:09Z - Template created at: get_template.json
+```
+
+#### Option `--request-file`
+This option allows to specify request parameters but in a provided `.json` file, useful for batch processing.
+You can try the following templates or use the `--create-template` option to create both `subset` or `get` template request files.
+
+- Template for `subset` data request:
+```json
+{
+    "dataset_id": "cmems_mod_glo_phy-thetao_anfc_0.083deg_P1D-m",
+    "start_datetime": "2022-04-11",
+    "end_datetime": "2023-08-11",
+    "minimum_longitude": -182.79,
+    "maximum_longitude": -179.69,
+    "minimum_latitude": -40,
+    "maximum_latitude": -36,
+    "minimum_depth": 0,
+    "maximum_depth": 0,
+    "variables": ["thetao"],
+    "output_directory": "./data/",
+    "force_download": true
 }
+```
+
+Example:
+```bash
+copernicusmarine subset --request-file template_subset_data_request.json
+```
+
+- Template for `get` data request:
+```json
+{
+    "dataset_id": "cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m",
+    "filter": "*01yav_200[0-2]*",
+    "force_download": false,
+    "log_level": "INFO",
+    "no_directories": false,
+    "no_metadata_cache": false,
+    "output_directory": "./data/",
+    "overwrite_output_data": false,
+    "overwrite_metadata_cache": false,
+    "show_outputnames": true
+}
+```
+
+Example:
+```bash
+copernicusmarine get --request-file template_get_data_request.json
+```
+
+#### Option `--credentials-file`
+You can use the `--credentials-file` option to point to a credentials file. The file can be either `.copernicusmarine-credentials`, `motuclient-python.ini`, `.netrc` or `_netrc`.
+
+#### Option `--dataset-version`
+You can use the `--dataset-version` option to fetch a specific dataset version. Particularly useful to keep an operational chain working when an evolution impact the chosen dataset.
+
+#### Option `--dataset-part`
+You can use the `--dataset-part` option to fecth a specific part for the chosen dataset version.
+
+#### Option `--log-level`
+Set the details printed to console by the command (based on standard logging library).
+Available values are: `[DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]`
+
+## Python package (API)
+The `copernicusmarine` exposes a Python interface to allow you to [call commands as functions](https://help.marine.copernicus.eu/en/collections/9054839-main-functionalities).
+
+## Documentation
+A detailed standalone API documentation is under construction and will come at a later stage. For the moment, see the [Help Center](https://help.marine.copernicus.eu/en/collections/9080063-copernicus-marine-toolbox).
+
+## Version management
+We are using semantic versioning X.Y.Z → for example 1.0.2
+- Z is bumped on minor non-breaking changes.
+- Y is bumped on breaking changes.
+- X is bumped on demand to highlight a new significant feature or for communication purposes (new Copernicus Marine Service release for example).
+
+## Contribution
+We welcome contributions from the community to enhance this package. If you find any issues or have suggestions for improvements, please check out our [Report Template](https://help.marine.copernicus.eu/en/articles/8218546-reporting-an-issue-or-feature-request).
+
+## Future improvements & Roadmap
+To keep up to date with the most recent and planned advancements, including revisions, corrections, and feature requests generated from users' feedback, please refer to our [Roadmap](https://help.marine.copernicus.eu/en/articles/8218641-next-milestones-and-roadmap).
 
+## Join the community
+Get in touch!
+- Create your [Copernicus Marine Account](https://data.marine.copernicus.eu/register?redirect=%2Fproducts)
+- [Log in](https://data.marine.copernicus.eu/login?redirect=%2Fproducts) and chat with us (bottom right corner of [Copernicus Marine Service](https://marine.copernicus.eu/))
+- Join our [training workshops](https://marine.copernicus.eu/services/user-learning-services)
+- Network y/our [Copernicus Stories](https://twitter.com/cmems_eu)
+- Watch [our videos](https://www.youtube.com/channel/UC71ceOVy7WtVC7F04BKoEew)
+## Licence
+Licensed under the [EUPL](https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12)
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,416 +1,437 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['copernicusmarine', 'copernicusmarine.aioretry',
-'copernicusmarine.catalogue_parser', 'copernicusmarine.command_line_interface',
-'copernicusmarine.core_functions', 'copernicusmarine.download_functions',
-'copernicusmarine.python_interface'] package_data = \ {'': ['*']}
-install_requires = \ ['aiohttp>=3.8.5', 'boto3>=1.25', 'cachier>=2.2.1',
-'click>=8.0.4', 'dask>=2022', 'lxml>=4.9.0', 'nest-asyncio>=1.5.8',
-'netCDF4>=1.5.4', 'pystac>=1.8.3', 'requests>=2.27.1', 'semver>=3.0.2',
-'setuptools>=68.2.2', 'tqdm>=4.65.0', 'xarray>=2023.4.0', 'zarr>=2.13.3']
-entry_points = \ {'console_scripts': ['copernicusmarine = '
-'copernicusmarine.command_line_interface.copernicus_marine:
-command_line_interface']} setup_kwargs = { 'name': 'copernicusmarine',
-'version': '1.1.1', 'description': '', 'long_description': '\n
+Metadata-Version: 2.1 Name: copernicusmarine Version: 1.2.0 Summary: License:
+EUPL-1.2 Author: Copernicus Marine User Support Author-email:
+servicedesk.cmems@mercator-ocean.eu Requires-Python: >=3.9,<3.13 Classifier:
+License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Requires-Dist: aiohttp (>=3.9.4) Requires-Dist:
+boto3 (>=1.25) Requires-Dist: cachier (>=2.2.1) Requires-Dist: click (>=8.0.4)
+Requires-Dist: dask (>=2022) Requires-Dist: lxml (>=4.9.0) Requires-Dist: nest-
+asyncio (>=1.5.8) Requires-Dist: netCDF4 (>=1.5.4) Requires-Dist: pystac
+(>=1.8.3) Requires-Dist: requests (>=2.27.1) Requires-Dist: semver (>=3.0.2)
+Requires-Dist: setuptools (>=68.2.2) Requires-Dist: tqdm (>=4.65.0) Requires-
+Dist: xarray (>=2023.4.0) Requires-Dist: zarr (>=2.13.3) Description-Content-
+Type: text/markdown
         ************ CCooppeerrnniiccuuss MMaarriinnee SSeerrvviiccee TToooollbbooxx ((CCLLII && PPyytthhoonn)) ************
-\n
-  \n _[_P_y_P_I_]\n _[_P_y_P_I_ _S_u_p_p_o_r_t_e_d_ _V_e_r_s_i_o_n_s_]\n _[_S_u_p_p_o_r_t_e_d_ _P_l_a_t_f_o_r_m_s_]\n _[_L_i_c_e_n_c_e_]\n
-\n\n![Copernicus Marine Service and Mercator Ocean international logos](https:/
-/www.mercator-ocean.eu/wp-content/uploads/2022/05/
-Cartouche_CMEMS_poisson_MOi.png)\n\n## Features\nThe `copernicusmarine` offers
+         _[_P_y_P_I_]_[_P_y_P_I_ _S_u_p_p_o_r_t_e_d_ _V_e_r_s_i_o_n_s_]_[_S_u_p_p_o_r_t_e_d_ _P_l_a_t_f_o_r_m_s_]_[_L_i_c_e_n_c_e_]
+![Copernicus Marine Service and Mercator Ocean international logos](https://
+www.mercator-ocean.eu/wp-content/uploads/2022/05/
+Cartouche_CMEMS_poisson_MOi.png) ## Features The `copernicusmarine` offers
 capabilities through both **Command Line Interface (CLI)** and **Python API**:
-\n- **Metadata Information**: List and retrieve metadata information on all
-variables, datasets, products, and their associated documentation.\n- **Subset
+- **Metadata Information**: List and retrieve metadata information on all
+variables, datasets, products, and their associated documentation. - **Subset
 Datasets**: Subset datasets to extract only the parts of interest, in preferred
 format, such as Analysis-Ready Cloud-Optimized (ARCO) Zarr or NetCDF file
-format.\n- **Advanced Filters**: Apply simple or advanced filters to get
+format. - **Advanced Filters**: Apply simple or advanced filters to get
 multiple files, in original formats like NetCDF/GeoTIFF, via direct Marine Data
-Store connections.\n- **No Quotas**: Enjoy no quotas, neither on volume size
-nor bandwidth.\n\n## Installation\nFor installation, multiple options are
-available depending on your setup:\n\n### Mamba | Conda\nA `conda` package is
-available on [Anaconda](https://anaconda.org/conda-forge/
-copernicusmarine).\n\nYou can install it using `mamba` (or conda) through the
-`conda-forge` channel with the following command:\n```bash\nmamba install
-conda-forge::copernicusmarine --yes\n```\n\nTo upgrade the Toolbox with mamba
-(or conda):\n```bash\nmamba update --name copernicusmarine copernicusmarine --
-yes\n```\n\n### Docker\nA docker image is also available here: [https://
-hub.docker.com/r/copernicusmarine/copernicusmarine](https://hub.docker.com/r/
-copernicusmarine/copernicusmarine)\n\nFirst step is to pull the container
-image:\n```bash\ndocker pull copernicusmarine/copernicusmarine:
-latest\n```\n\nThen run it:\n```bash\ndocker run -it --rm copernicusmarine/
-copernicusmarine --version\n```\n\n### Pip\nOtherwise, if you already have an
-environment (safer to clone it), the package can be installed using the `pip`
-command:\n```bash\npython -m pip install copernicusmarine\n```\n\nAnd to
-**upgrade the package** to the newest available version, run:\n```bash\npython
--m pip install copernicusmarine --upgrade\n```\n\n## User Guide\nFor more
+Store connections. - **No Quotas**: Enjoy no quotas, neither on volume size nor
+bandwidth. ## Installation For installation, multiple options are available
+depending on your setup: ### Mamba | Conda A `conda` package is available on
+[Anaconda](https://anaconda.org/conda-forge/copernicusmarine). You can install
+it using `mamba` (or conda) through the `conda-forge` channel with the
+following command: ```bash mamba install conda-forge::copernicusmarine --yes
+``` To upgrade the Toolbox with mamba (or conda): ```bash mamba update --name
+copernicusmarine copernicusmarine --yes ``` ### Docker A docker image is also
+available here: [https://hub.docker.com/r/copernicusmarine/copernicusmarine]
+(https://hub.docker.com/r/copernicusmarine/copernicusmarine) First step is to
+pull the container image: ```bash docker pull copernicusmarine/
+copernicusmarine:latest ``` Then run it: ```bash docker run -it --rm
+copernicusmarine/copernicusmarine --version ``` ### Pip Otherwise, if you
+already have an environment (safer to clone it), the package can be installed
+using the `pip` command: ```bash python -m pip install copernicusmarine ``` And
+to **upgrade the package** to the newest available version, run: ```bash python
+-m pip install copernicusmarine --upgrade ``` ## User Guide For more
 comprehensive details on how to use the `copernicusmarine` Toolbox, please
 refer to our [Help Center](https://help.marine.copernicus.eu/en/collections/
-9054839-copernicus-marine-toolbox-guide). It ensures a smooth migration for
-existing users of legacy services such as MOTU, OPeNDAP or FTP.\n\n### General
-configuration\n\n#### Cache Usage\nCachier library is used for caching part of
-the requests (as result of `describe` or `login`). By default, the cache will
-be located in the home folder. If you need to change the location of the cache,
+9080063-copernicus-marine-toolbox). It ensures a smooth migration for existing
+users of legacy services such as MOTU, OPeNDAP or FTP. ### General
+configuration #### Cache Usage Cachier library is used for caching part of the
+requests (as result of `describe` or `login`). By default, the cache will be
+located in the home folder. If you need to change the location of the cache,
 you can set the environment variable `COPERNICUSMARINE_CACHE_DIRECTORY` to
-point to the desired directory:\n- on **UNIX** platforms: `export
-COPERNICUSMARINE_CACHE_DIRECTORY=`\n- on **Windows** platforms: `set
-COPERNICUSMARINE_CACHE_DIRECTORY=`\n\n### Network configuration\n\n#### Disable
-SSL\n\nA global SSL context is used when making HTTP calls using the
-`copernicusmarine` Toolbox. For some reason, it can lead to unexpected behavior
-depending on your network configuration. You can set the
-`COPERNICUSMARINE_DISABLE_SSL_CONTEXT` environment variable to any value to
-globally disable the usage of SSL in the toolbox:\n\n- on **UNIX** platforms:
-`export COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True`\n- on **Windows** platforms:
-`set COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True`\n\n#### Trust Env for python
-libraries\n\nTo do HTTP calls, the Copernicus Marine Toolbox uses two python
-libraries: requests and aiohttp. By default, those libraries will have
-`trust_env` values set to `True`. If you want to deactivate this, you can set
+point to the desired directory: - on **UNIX** platforms: `export
+COPERNICUSMARINE_CACHE_DIRECTORY=` - on **Windows** platforms: `set
+COPERNICUSMARINE_CACHE_DIRECTORY=` ### Network configuration #### Disable SSL A
+global SSL context is used when making HTTP calls using the `copernicusmarine`
+Toolbox. For some reason, it can lead to unexpected behavior depending on your
+network configuration. You can set the `COPERNICUSMARINE_DISABLE_SSL_CONTEXT`
+environment variable to any value to globally disable the usage of SSL in the
+toolbox: - on **UNIX** platforms: `export
+COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True` - on **Windows** platforms: `set
+COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True` #### Trust Env for python libraries
+To do HTTP calls, the Copernicus Marine Toolbox uses two python libraries:
+requests and aiohttp. By default, those libraries will have `trust_env` values
+set to `True`. If you want to deactivate this, you can set
 `COPERNICUSMARINE_TRUST_ENV=False` (default `True`). This can be useful for
-example if you don\'t want those libraries to read your `.netrc` file as it has
+example if you don't want those libraries to read your `.netrc` file as it has
 been reported that having a `.netrc` with a line: "default login anonymous
-password user@site" is incompatible with S3 connection required by the
-toolbox.\n\n#### Proxy\n\nTo use proxies, as describe in the [aiohttp
-documentation](https://docs.aiohttp.org/en/stable/client_advanced.html#proxy-
-support) you can use two options:\n\n- set the `HTTPS_PROXY` variable. For eg:
-`HTTPS_PROXY="http://user:pass@some.proxy.com"`. It should work even with
-`COPERNICUSMARINE_TRUST_ENV=False`.\n- use a `.netrc` file but be aware that
+password user@site" is incompatible with S3 connection required by the toolbox.
+#### Proxy To use proxies, as describe in the [aiohttp documentation](https://
+docs.aiohttp.org/en/stable/client_advanced.html#proxy-support) you can use two
+options: - set the `HTTPS_PROXY` variable. For eg: `HTTPS_PROXY="http://user:
+pass@some.proxy.com"`. It should work even with
+`COPERNICUSMARINE_TRUST_ENV=False`. - use a `.netrc` file but be aware that
 having a line: "default login anonymous password user@site" is incompatible
 with S3 connection required by the toolbox. Also note that if you have
 `COPERNICUSMARINE_TRUST_ENV=True` (the default value) then if `NETRC`
 environment variable is set with a specified location, the `.netrc` file will
-be read from the specified location there rather than from `~/.netrc`.\n\n##
-Command Line Interface (CLI)\n\n### The `--help` option\nTo discover commands
-and their available options, consider appending `--help` on any command
-line.\n\nExample:\n```bash\ncopernicusmarine --help\n```\n\nReturns:
-\n```bash\nUsage: copernicusmarine [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n -
-V, --version Show the version and exit.\n -h, --help Show this message and
-exit.\n\nCommands:\n describe Print Copernicus Marine catalog as JSON.\n get
-Download originally produced data files.\n login Create a configuration file
-with your Copernicus Marine credentials.\n subset Download subsets of datasets
-as NetCDF files or Zarr stores.\n```\n\n### Command `describe`\nRetrieve
-metadata information about all products/datasets and display as JSON output:
-\n```bash\ncopernicusmarine describe --include-datasets\n```\n\nThe JSON output
-can also be saved as follows:\n```bash\ncopernicusmarine describe --include-
-datasets > all_datasets_copernicusmarine.json\n```\n\n### Command
-`login`\nCreate a single configuration file `.copernicusmarine-credentials`
-allowing to access all Copernicus Marine Data Store data services. By default,
-the file is saved in user\'s home directory.\n\nExample:\n```bash\n>
-copernicusmarine login\nusername : johndoe\npassword :\nINFO - Configuration
-files stored in /Users/foo/.copernicusmarine\n```\n\nIf `.copernicusmarine-
-credentials` already exists, the user is asked for confirmation to overwrite
-(`--overwrite`/`--overwrite-configuration-file`).\n\nYou can use the `--skip-
-if-user-logged-in` option to skip the configuration file overwrite if the user
-is already logged in.\n\n#### Access points migration and evolution\nIf you
-still have a configuration for legacy services (e.g. `~/motuclient/motuclient-
-python.ini`, `~/.netrc` or `~/_netrc`) in your home directory, it will
-automatically be taken into account with commands `get` and `subset` without
-the need for running the `login` command.\nIf the configuration files are
-already available in another directory, when running commands `subset` or
-`get`, you can use the `--credentials-file` option to point to the
-files.\n\n### Command `subset`\nRemotely subset a dataset, based on variable
-names, geographical and temporal parameters.\n\nExample:
-\n```bash\ncopernicusmarine subset --dataset-id cmems_mod_ibi_phy_my_0.083deg-
-3D_P1D-m --variable thetao --variable so --start-datetime 2021-01-01 --end-
-datetime 2021-01-03 --minimum-longitude 0.0 --maximum-longitude 0.1 --minimum-
-latitude 28.0 --maximum-latitude 28.1\n```\nReturns:\n```bash\nINFO - 2024-04-
-03T10:18:18Z - Size: 3kB\nDimensions: (depth: 50, latitude: 2, longitude: 1,
-time: 3)\nCoordinates:\n * depth (depth) float32 200B 0.5058 1.556 2.668 ...
-5.292e+03 5.698e+03\n * latitude (latitude) float32 8B 28.0 28.08\n * longitude
-(longitude) float32 4B 0.08333\n * time (time) datetime64[ns] 24B 2021-01-01
-2021-01-02 2021-01-03\nData variables:\n thetao (time, depth, latitude,
-longitude) float32 1kB dask.array
-(3, 1, 2, 1), meta=np.ndarray>\n so (time, depth, latitude, longitude) float32
+be read from the specified location there rather than from `~/.netrc`. ####
+Number of concurrent requests The toolbox makes many requests to STAC to be
+able to parse the full marine data store STAC catalog. For that, it uses
+asynchronous calls. It can be problematic to do too many requests at the same
+time. To limit the number of requests at the same time you can use:
+`COPERNICUSMARINE_MAX_CONCURRENT_REQUESTS`. The default value is `15` and
+minimum value is `1`. Note, that this concerns only the catalog parsing step so
+the describe command and the start of the get and subset command. It does not
+apply when downloading files or listing files from the get command or when
+requesting the data chunks for the subset command. ## Command Line Interface
+(CLI) ### The `--help` option To discover commands and their available options,
+consider appending `--help` on any command line. Example: ```bash
+copernicusmarine --help ``` Returns: ```bash Usage: copernicusmarine [OPTIONS]
+COMMAND [ARGS]... Options: -V, --version Show the version and exit. -h, --help
+Show this message and exit. Commands: describe Print Copernicus Marine catalog
+as JSON. get Download originally produced data files. login Create a
+configuration file with your Copernicus Marine credentials. subset Download
+subsets of datasets as NetCDF files or Zarr stores. ``` ### Command `describe`
+Retrieve metadata information about all products/datasets and display as JSON
+output: ```bash copernicusmarine describe --include-datasets ``` The JSON
+output can also be saved as follows: ```bash copernicusmarine describe --
+include-datasets > all_datasets_copernicusmarine.json ``` ### Command `login`
+Create a single configuration file `.copernicusmarine-credentials` allowing to
+access all Copernicus Marine Data Store data services. By default, the file is
+saved in user's home directory. Example: ```bash > copernicusmarine login
+username : johndoe password : INFO - Configuration files stored in /Users/
+foo/.copernicusmarine ``` If `.copernicusmarine-credentials` already exists,
+the user is asked for confirmation to overwrite (`--overwrite`/`--overwrite-
+configuration-file`). You can use the `--skip-if-user-logged-in` option to skip
+the configuration file overwrite if the user is already logged in. #### Access
+points migration and evolution If you still have a configuration for legacy
+services (e.g. `~/motuclient/motuclient-python.ini`, `~/.netrc` or `~/_netrc`)
+in your home directory, it will automatically be taken into account with
+commands `get` and `subset` without the need for running the `login` command.
+If the configuration files are already available in another directory, when
+running commands `subset` or `get`, you can use the `--credentials-file` option
+to point to the files. ### Command `subset` Remotely subset a dataset, based on
+variable names, geographical and temporal parameters. Example: ```bash
+copernicusmarine subset --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1D-m --
+variable thetao --variable so --start-datetime 2021-01-01 --end-datetime 2021-
+01-03 --minimum-longitude 0.0 --maximum-longitude 0.1 --minimum-latitude 28.0 -
+-maximum-latitude 28.1 ``` Returns: ```bash INFO - 2024-04-03T10:18:18Z - Size:
+3kB Dimensions: (depth: 50, latitude: 2, longitude: 1, time: 3) Coordinates: *
+depth (depth) float32 200B 0.5058 1.556 2.668 ... 5.292e+03 5.698e+03 *
+latitude (latitude) float32 8B 28.0 28.08 * longitude (longitude) float32 4B
+0.08333 * time (time) datetime64[ns] 24B 2021-01-01 2021-01-02 2021-01-03 Data
+variables: thetao (time, depth, latitude, longitude) float32 1kB dask.array
+(3, 1, 2, 1), meta=np.ndarray> so (time, depth, latitude, longitude) float32
 1kB dask.array
-(3, 1, 2, 1), meta=np.ndarray>\nAttributes: (12/20)\n Conventions: CF-1.0\n
-bulletin_date: 2020-12-01\n ... ...\n references: http://marine.copernicus.eu\n
-copernicusmarine_version: 1.1.0\nINFO - 2024-04-03T10:18:18Z - Estimated size
-of the dataset file is 0.002 MB.\n\nDo you want to proceed with download? [Y/
-n]:\n```\n\nBy default, after the display of the summary of the dataset subset,
-a download confirmation is asked. To skip this confirmation, use the option `--
-force-download`.\n\n#### Note about `--subset-method` option\nBy default, the
-`subset` feature uses the `nearest` method of xarray. By specifying `--subset-
-method strict`, you can only request dimension strictly inside the dataset,
-useful for **operational use-case**.\n\n#### Note about longitude
-range\nOptions `--minimum-longitude` and `--maximum-longitude` work as follows:
-\n- If the result of the substraction ( `--maximum-longitude` minus `--minimum-
-longitude` ) is superior or equal to 360, then return the full dataset.\n- If
-the requested longitude range:\n - **does not cross** the antemeridian, then
-return the dataset between range -180 and 180.\n - **does cross** the
-antemeridian, then return the dataset between range 0 and 360.\n\nNote that you
-can request any longitudes you want. A modulus is applied to bring the result
-between -180Â° and 360Â°. For example, if you request [530, 560], the result
-dataset will be in [170, 200].\n\n\n#### Note about `--netcdf-compression-
-enabled` and `--netcdf-compression-level` options\nWhen subsetting data, if you
-decide to write your data as a NetCDF file (which is the default behavior),
-then you can provide the extra option `--netcdf-compression-enabled`. The
-downloaded file will be lighter but it will take more time to write it (because
-of the compression task). If you don\'t provide it, the task will be faster,
-but the file heavier.\nOtherwise, if you decide to write your data in Zarr
-format (`.zarr` extension), the original compression used in the Copernicus
-Marine Data Store will be applied, which means that the download task will be
-fast **and** the file compressed. In that case, you cannot use the `--netcdf-
-compression-enabled`.\n\nHere are the default parameters added to xarray in the
-background when using the option: `{\'zlib\': True, \'complevel\': 1,
-\'contiguous\': False, \'shuffle\': True}`\n\nIn addition to this option, you
-can also provide the `--netcdf-compression-level` option and customize the
-NetCDF compression level between 0 (no compression) and 9 (maximal
-compression).\n\n#### Note about `--netcdf3-compatible` option\nThe `--netcdf3-
-compatible` option has been added to allow the downloaded dataset to be
+(3, 1, 2, 1), meta=np.ndarray> Attributes: (12/20) Conventions: CF-1.0
+bulletin_date: 2020-12-01 ... ... references: http://marine.copernicus.eu
+copernicusmarine_version: 1.1.0 INFO - 2024-04-03T10:18:18Z - Estimated size of
+the dataset file is 0.002 MB. Do you want to proceed with download? [Y/n]: ```
+By default, after the display of the summary of the dataset subset, a download
+confirmation is asked. To skip this confirmation, use the option `--force-
+download`. #### Note about `--subset-method` option By default, the `subset`
+feature uses the `nearest` method of xarray. By specifying `--subset-method
+strict`, you can only request dimension strictly inside the dataset, useful for
+**operational use-case**. #### Note about longitude range Options `--minimum-
+longitude` and `--maximum-longitude` work as follows: - If the result of the
+substraction ( `--maximum-longitude` minus `--minimum-longitude` ) is superior
+or equal to 360, then return the full dataset. - If the requested longitude
+range: - **does not cross** the antemeridian, then return the dataset between
+range -180 and 180. - **does cross** the antemeridian, then return the dataset
+between range 0 and 360. Note that you can request any longitudes you want. A
+modulus is applied to bring the result between -180Â° and 360Â°. For example,
+if you request [530, 560], the result dataset will be in [170, 200]. #### Note
+about `--netcdf-compression-enabled` and `--netcdf-compression-level` options
+When subsetting data, if you decide to write your data as a NetCDF file (which
+is the default behavior), then you can provide the extra option `--netcdf-
+compression-enabled`. The downloaded file will be lighter but it will take more
+time to write it (because of the compression task). If you don't provide it,
+the task will be faster, but the file heavier. Otherwise, if you decide to
+write your data in Zarr format (`.zarr` extension), the original compression
+used in the Copernicus Marine Data Store will be applied, which means that the
+download task will be fast **and** the file compressed. In that case, you
+cannot use the `--netcdf-compression-enabled`. Here are the default parameters
+added to xarray in the background when using the option: `{'zlib': True,
+'complevel': 1, 'contiguous': False, 'shuffle': True}` In addition to this
+option, you can also provide the `--netcdf-compression-level` option and
+customize the NetCDF compression level between 0 (no compression) and 9
+(maximal compression). #### Note about `--netcdf3-compatible` option The `--
+netcdf3-compatible` option has been added to allow the downloaded dataset to be
 compatible with the netCDF3 format. It uses the `format="NETCDF3_CLASSIC"` of
 the xarray [to_netcdf](https://docs.xarray.dev/en/latest/generated/
-xarray.Dataset.to_netcdf.html) method.\n\n### Command `get`\nDownload the
-dataset file(s) as originally produced, based on the datasetID or the path to
-files.\n\nExample:\n```bash\ncopernicusmarine get --dataset-id
-cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --service original-files\n```\nReturns:
-\n```bash\nINFO - 2024-04-03T11:39:18Z - Dataset version was not specified, the
-latest one was selected: "202211"\nINFO - 2024-04-03T11:39:18Z - Dataset part
-was not specified, the first one was selected: "default"\nINFO - 2024-04-03T11:
+xarray.Dataset.to_netcdf.html) method. ### Command `get` Download the dataset
+file(s) as originally produced, based on the datasetID or the path to files.
+Example: ```bash copernicusmarine get --dataset-id
+cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --service original-files ``` Returns:
+```bash INFO - 2024-04-03T11:39:18Z - Dataset version was not specified, the
+latest one was selected: "202211" INFO - 2024-04-03T11:39:18Z - Dataset part
+was not specified, the first one was selected: "default" INFO - 2024-04-03T11:
 39:18Z - Service was not specified, the default one was selected: "original-
-files"\nINFO - 2024-04-03T11:39:18Z - Downloading using service original-
-files...\nINFO - 2024-04-03T11:39:19Z - You requested the download of the
-following files:\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
+files" INFO - 2024-04-03T11:39:18Z - Downloading using service original-
+files... INFO - 2024-04-03T11:39:19Z - You requested the download of the
+following files: s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
 cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/
 CMEMS_v5r1_IBI_PHY_MY_NL_01yav_19930101_19931231_R20221101_RE01.nc - 8.83 MB -
-2023-11-12T23:47:13Z\n[... truncated for brevity..]\ns3://mdl-native-10/native/
+2023-11-12T23:47:13Z [... truncated for brevity..] s3://mdl-native-10/native/
 IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/
 CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20120101_20121231_R20221101_RE01.nc - 8.62 MB -
-2023-11-12T23:47:14Z\nPrinted 20 out of 29 files\n\nTotal size of the download:
-252.94 MB\nDo you want to proceed with download? [Y/n]:\n```\n\nBy default:\n-
-After the header displays a summary of the request, a download confirmation is
-asked. To skip this user\'s action, add option `--force-download`.\n- Files are
+2023-11-12T23:47:14Z Printed 20 out of 29 files Total size of the download:
+252.94 MB Do you want to proceed with download? [Y/n]: ``` By default: - After
+the header displays a summary of the request, a download confirmation is asked.
+To skip this user's action, add option `--force-download`. - Files are
 downloaded to the current directory applying the original folder structure. To
 avoid this behavior, add `--no-directories` and specify a destination with `-o/
---output-directory`.\n\nOption `--show-outputnames` displays the full paths of
-the output files, if required.\n\nOption `--create-file-list` only creates a
-file containing the names of the targeted files instead of downloading them.
-You have to input a file name, e.g. `--create-file-list my_files.txt`. The
-format needs to be `.txt` or `.csv`:\n\n- If the user inputs a filename that
-ends in `.txt`, then the file contains only the full s3 path to the targeted
-files and is compatible with the `--file-list` option.\n\nExample:
-\n```bash\ncopernicusmarine get --dataset-id cmems_mod_ibi_phy_my_0.083deg-
-3D_P1M-m --filter "*2021*" --create-file-list
-selected_files_for_2021.txt\n```\nThe content of `selected_files_for_2021.txt`
-would be:\n```\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
-cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/
-CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210101_20210131_R20230101_RE01.nc\ns3://mdl-
+--output-directory`. Option `--show-outputnames` displays the full paths of the
+output files, if required. Option `--create-file-list` only creates a file
+containing the names of the targeted files instead of downloading them. You
+have to input a file name, e.g. `--create-file-list my_files.txt`. The format
+needs to be `.txt` or `.csv`: - If the user inputs a filename that ends in
+`.txt`, then the file contains only the full s3 path to the targeted files and
+is compatible with the `--file-list` option. Example: ```bash copernicusmarine
+get --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m --filter "*2021*" --
+create-file-list selected_files_for_2021.txt ``` The content of
+`selected_files_for_2021.txt` would be: ``` s3://mdl-native-10/native/
+IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/
+CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210101_20210131_R20230101_RE01.nc s3://mdl-
 native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-
 3D_P1M-m_202012/2021/
-CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210201_20210228_R20230101_RE01.nc\n[...
-truncated for brevity..]\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
+CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210201_20210228_R20230101_RE01.nc [...
+truncated for brevity..] s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
 cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/
-CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211101_20211130_R20230101_RE01.nc\ns3://mdl-
+CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211101_20211130_R20230101_RE01.nc s3://mdl-
 native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-
 3D_P1M-m_202012/2021/
-CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211201_20211231_R20230101_RE01.nc\n```\n\n-
-If the user inputs a filename that ends in `.csv` the file contains the
-following columns, separated by a comma: `filename`, `size` (in Bytes),
+CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211201_20211231_R20230101_RE01.nc ``` - If
+the user inputs a filename that ends in `.csv` the file contains the following
+columns, separated by a comma: `filename`, `size` (in Bytes),
 `last_modified_datetime`, and `etag`. It is **not** compatible "as is" with the
-`--file-list` option and would need further post-processing from user\'s
-side.\n\nExample:\n```bash\ncopernicusmarine get --dataset-id
+`--file-list` option and would need further post-processing from user's side.
+Example: ```bash copernicusmarine get --dataset-id
 cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m --filter "*2021*" --create-file-list
-selected_files_for_2021.csv\n```\n The content of `selected_files_for_2021.csv`
-would be:\n```\nfilename,size,last_modified_datetime,etag\ns3://mdl-native-10/
+selected_files_for_2021.csv ``` The content of `selected_files_for_2021.csv`
+would be: ``` filename,size,last_modified_datetime,etag s3://mdl-native-10/
 native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/
 2021/
 CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210101_20210131_R20230101_RE01.nc,12295906,2023-
-11-12 23:47:05.466000+00:00,"e8a7e564f676a08bf601bcdeaebdc563"\ns3://mdl-
-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-
-3D_P1M-m_202012/2021/
+11-12 23:47:05.466000+00:00,"e8a7e564f676a08bf601bcdeaebdc563" s3://mdl-native-
+10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-
+m_202012/2021/
 CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210201_20210228_R20230101_RE01.nc,12436177,2023-
-11-12 23:47:05.540000+00:00,"d4a22dfb6c7ed85860c4a122c45eb953"\n[... truncated
-for brevity..]\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
+11-12 23:47:05.540000+00:00,"d4a22dfb6c7ed85860c4a122c45eb953" [... truncated
+for brevity..] s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
 cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/
 CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211101_20211130_R20230101_RE01.nc,12386940,2023-
-11-12 23:47:06.358000+00:00,"ea15d1f70fcc7f2ce404184d983530ff"\ns3://mdl-
-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-
-3D_P1M-m_202012/2021/
+11-12 23:47:06.358000+00:00,"ea15d1f70fcc7f2ce404184d983530ff" s3://mdl-native-
+10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-
+m_202012/2021/
 CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211201_20211231_R20230101_RE01.nc,12398208,2023-
-11-12 23:47:06.456000+00:00,"585f49867aaefa2ce9d6e68dd468b5e1"\n```\nIf
-specified, no other action will be performed.\n\n\n#### Note about sync
-option\nOption `--sync` allows to download original files only if not exist and
-not up to date. The Toolbox checks the destination folder against the source
-folder. It can be combined with filters. Note that if set with `--overwrite-
-output-data`, the latter will be ignored.\nThe logic is largely inspired from
-[s5cmd package sync command](https://github.com/peak/s5cmd#sync).\nOption `--
-sync-delete` will work as `--sync` with the added fonctionnality that it
-deletes any local file that has not been found on the remote server. Note that
-the files found on the server are also filtered. Hence, a file present locally
-might be deleted even if it is on the server because, for example, the executed
-`get` command contains a filter that excludes this specific
-file.\n\nLimitations:\n- `--sync` is not compatible with `--no-directories`.\n-
-`--sync` only works with `--dataset-version`.\n- `--sync` functionality is not
-available for datasets with several parts (like INSITU or static datasets for
-example).\n\n#### Note about filtering options\nOption `--filter` allows to
-specify a Unix shell-style wildcard pattern (see [fnmatch â Unix filename
-pattern matching](https://docs.python.org/3/library/fnmatch.html)) and select
-specific files:\n```bash\ncopernicusmarine get --dataset-id
-cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --filter "*01yav_200[0-
-2]*"\n```\nReturns:\n```bash\nINFO - 2024-04-03T11:51:15Z - Dataset version was
-not specified, the latest one was selected: "202211"\nINFO - 2024-04-03T11:51:
-15Z - Dataset part was not specified, the first one was selected:
-"default"\nINFO - 2024-04-03T11:51:15Z - Service was not specified, the default
-one was selected: "original-files"\nINFO - 2024-04-03T11:51:15Z - Downloading
-using service original-files...\nINFO - 2024-04-03T11:51:17Z - You requested
-the download of the following files:\ns3://mdl-native/native/
+11-12 23:47:06.456000+00:00,"585f49867aaefa2ce9d6e68dd468b5e1" ``` If
+specified, no other action will be performed. #### Note about sync option
+Option `--sync` allows to download original files only if not exist and not up
+to date. The Toolbox checks the destination folder against the source folder.
+It can be combined with filters. Note that if set with `--overwrite-output-
+data`, the latter will be ignored. The logic is largely inspired from [s5cmd
+package sync command](https://github.com/peak/s5cmd#sync). Option `--sync-
+delete` will work as `--sync` with the added fonctionnality that it deletes any
+local file that has not been found on the remote server. Note that the files
+found on the server are also filtered. Hence, a file present locally might be
+deleted even if it is on the server because, for example, the executed `get`
+command contains a filter that excludes this specific file. Limitations: - `--
+sync` is not compatible with `--no-directories`. - `--sync` only works with `--
+dataset-version`. - `--sync` functionality is not available for datasets with
+several parts (like INSITU or static datasets for example). #### Note about
+filtering options Option `--filter` allows to specify a Unix shell-style
+wildcard pattern (see [fnmatch â Unix filename pattern matching](https://
+docs.python.org/3/library/fnmatch.html)) and select specific files: ```bash
+copernicusmarine get --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --
+filter "*01yav_200[0-2]*" ``` Returns: ```bash INFO - 2024-04-03T11:51:15Z -
+Dataset version was not specified, the latest one was selected: "202211" INFO -
+2024-04-03T11:51:15Z - Dataset part was not specified, the first one was
+selected: "default" INFO - 2024-04-03T11:51:15Z - Service was not specified,
+the default one was selected: "original-files" INFO - 2024-04-03T11:51:15Z -
+Downloading using service original-files... INFO - 2024-04-03T11:51:17Z - You
+requested the download of the following files: s3://mdl-native/native/
 IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/
-CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93
-MB\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/
-cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/
-CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91
-MB\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/
+CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB
+s3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-
+3D_P1Y-m_202211/
+CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB
+s3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-
+3D_P1Y-m_202211/
+CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB
+Total size of the download: 26.59 MB Do you want to proceed with download? [Y/
+n]: ``` Option `--regex` allows to specify a regular expression for more
+advanced files selection: ```bash copernicusmarine get -
+i cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --regex ".*01yav_20(00|01|02).*.nc"
+``` Returns: ```bash INFO - 2024-04-03T11:52:43Z - Dataset version was not
+specified, the latest one was selected: "202211" INFO - 2024-04-03T11:52:43Z -
+Dataset part was not specified, the first one was selected: "default" INFO -
+2024-04-03T11:52:43Z - Service was not specified, the default one was selected:
+"original-files" INFO - 2024-04-03T11:52:43Z - Downloading using service
+original-files... INFO - 2024-04-03T11:52:44Z - You requested the download of
+the following files: s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
 cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/
-CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75
-MB\n\nTotal size of the download: 26.59 MB\nDo you want to proceed with
-download? [Y/n]:\n```\n\nOption `--regex` allows to specify a regular
-expression for more advanced files selection:\n\n```bash\ncopernicusmarine get
--i cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --regex ".*01yav_20
-(00|01|02).*.nc"\n```\nReturns:\n```bash\nINFO - 2024-04-03T11:52:43Z - Dataset
-version was not specified, the latest one was selected: "202211"\nINFO - 2024-
-04-03T11:52:43Z - Dataset part was not specified, the first one was selected:
-"default"\nINFO - 2024-04-03T11:52:43Z - Service was not specified, the default
-one was selected: "original-files"\nINFO - 2024-04-03T11:52:43Z - Downloading
-using service original-files...\nINFO - 2024-04-03T11:52:44Z - You requested
-the download of the following files:\ns3://mdl-native-10/native/
-IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/
 CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB -
-2023-11-12T23:47:13Z\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
+2023-11-12T23:47:13Z s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
 cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/
 CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB -
-2023-11-12T23:47:13Z\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
+2023-11-12T23:47:13Z s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
 cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/
 CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB -
-2023-11-12T23:47:13Z\n\nTotal size of the download: 26.59 MB\nDo you want to
-proceed with download? [Y/n]:\n```\n\nOption `--file-list` allows to specify a
-list of files for more advanced files selection.\nThe file can contain complete
-absolute paths for each target file (default behavior) or only a partial path
-defined by the user, as shown below.\n\nExample of `file_list.txt` with
-absolute paths:\n```txt\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
+2023-11-12T23:47:13Z Total size of the download: 26.59 MB Do you want to
+proceed with download? [Y/n]: ``` #### Notes about the file list option Option
+`--file-list` allows to specify a list of files for more advanced files
+selection. The file can contain complete absolute paths for each target file
+(default behavior) or only a partial path defined by the user, as shown below.
+By default, the get functionality lists all the files on the bucket to be able
+to select the requested ones. This create some overhead when there are a lot of
+files for a specific dataset. For example, a dataset with more than 100 000
+files would create an overhead of around two minutes. The file list option will
+directly download the files and avoid the listings if all the files listed are
+found. Careful, a path can easily be mispelled or wrongly queried. The toolbox
+will display a warning if the file is not found on the bucket and try to find
+the file by listing all the files on the bucket. Example of `file_list.txt`
+with paths that would be directly downloaded without the listing overhead:
+```txt # correct paths > s3://mdl-native-01/native/
+INSITU_GLO_PHYBGCWAV_DISCRETE_MYNRT_013_030/cmems_obs-
+ins_glo_phybgcwav_mynrt_na_irr_202311/history/BO/AR_PR_BO_58JM.nc >
+INSITU_GLO_PHYBGCWAV_DISCRETE_MYNRT_013_030/cmems_obs-
+ins_glo_phybgcwav_mynrt_na_irr_202311/history/BO/AR_PR_BO_58JM.nc > cmems_obs-
+ins_glo_phybgcwav_mynrt_na_irr_202311/history/BO/AR_PR_BO_58JM.nc > history/BO/
+AR_PR_BO_58JM.nc > index_history.txt # incorrect paths # version is missing >
+INSITU_GLO_PHYBGCWAV_DISCRETE_MYNRT_013_030/cmems_obs-
+ins_glo_phybgcwav_mynrt_na_irr/history/BO/AR_PR_BO_58JM.nc # only the file name
+and not the path to the file > AR_PR_BO_58JM.nc # not the same dataset >
+another_dataset/history/BO/AR_PR_BO_58JM.nc ``` Example of `file_list.txt` with
+absolute paths: ```txt s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
 cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/
-CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210101_20210131_R20230101_RE01.nc\ns3://mdl-
+CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210101_20210131_R20230101_RE01.nc s3://mdl-
 native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-
 3D_P1M-m_202012/2021/
-CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210201_20210228_R20230101_RE01.nc\ns3://mdl-
+CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210201_20210228_R20230101_RE01.nc s3://mdl-
 native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-
 3D_P1M-m_202012/2021/
-CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210301_20210331_R20230101_RE01.nc\n```\n\nExample
+CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210301_20210331_R20230101_RE01.nc ``` Example
 of `file_list.txt` with partial paths matching the absolute paths (equivalent
-to previous example):
-\n```txt\nCMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc\nCMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc\nCMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc\n```\n>
+to previous example): ```txt
+CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc
+CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc
+CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc ``` >
 **_NOTE:_** This option is compatible with the file generated by the `--create-
-file-list` option if you generated a ".txt" file.\n\nThen the following
-command:\n```bash\ncopernicusmarine get -i cmems_mod_ibi_phy_my_0.083deg-
-3D_P1Y-m --file-list file_list.txt\n```\nReturns:\n```bash\nINFO - 2024-04-
-03T12:57:44Z - Dataset version was not specified, the latest one was selected:
-"202211"\nINFO - 2024-04-03T12:57:44Z - Dataset part was not specified, the
-first one was selected: "default"\nINFO - 2024-04-03T12:57:44Z - Service was
-not specified, the default one was selected: "original-files"\nINFO - 2024-04-
-03T12:57:44Z - Downloading using service original-files...\nINFO - 2024-04-
-03T12:57:45Z - You requested the download of the following files:\ns3://mdl-
-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-
-3D_P1Y-m_202211/
+file-list` option if you generated a ".txt" file. Then the following command:
+```bash copernicusmarine get -i cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --file-
+list file_list.txt ``` Returns: ```bash INFO - 2024-04-03T12:57:44Z - Dataset
+version was not specified, the latest one was selected: "202211" INFO - 2024-
+04-03T12:57:44Z - Dataset part was not specified, the first one was selected:
+"default" INFO - 2024-04-03T12:57:44Z - Service was not specified, the default
+one was selected: "original-files" INFO - 2024-04-03T12:57:44Z - Downloading
+using service original-files... INFO - 2024-04-03T12:57:45Z - You requested the
+download of the following files: s3://mdl-native-10/native/
+IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/
 CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB -
-2023-11-12T23:47:13Z\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
+2023-11-12T23:47:13Z s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
 cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/
 CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB -
-2023-11-12T23:47:13Z\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
+2023-11-12T23:47:13Z s3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/
 cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/
 CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB -
-2023-11-12T23:47:13Z\n\nTotal size of the download: 26.59 MB\nDo you want to
-proceed with download? [Y/n]:\n```\n\nAlso, there is a specific command `--
-index-parts` to retrieve the index files of INSITU datasets (as listed on the
+2023-11-12T23:47:13Z Total size of the download: 26.59 MB Do you want to
+proceed with download? [Y/n]: ``` Also, there is a specific command `--index-
+parts` to retrieve the index files of INSITU datasets (as listed on the
 [Copernicus Marine File Browser](https://data.marine.copernicus.eu/product/
 INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/files?subdataset=cmems_obs-
 ins_blk_phybgcwav_mynrt_na_irr_202311--ext--
 history&path=INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034%2Fcmems_obs-
-ins_blk_phybgcwav_mynrt_na_irr_202311%2F)).\n> **_NOTE:_** In the future, it is
+ins_blk_phybgcwav_mynrt_na_irr_202311%2F)). > **_NOTE:_** In the future, it is
 planned to have the index files for those datasets directly available through
 the `--filter`, `--regex` and/or `--file-list` options. Meanwhile, check this
 [Help Center article for a working example](https://help.marine.copernicus.eu/
-en/articles/9133855-how-to-download-insitu-data-using-index-files).\n\n\nThen
-the following command:\n```\ncopernicusmarine get --dataset-id cmems_obs-
-ins_blk_phybgcwav_mynrt_na_irr --index-parts\n```\nReturns:\n```\nINFO - 2024-
-04-03T12:58:40Z - Dataset version was not specified, the latest one was
-selected: "202311"\nINFO - 2024-04-03T12:58:40Z - Dataset part was not
-specified, the first one was selected: "history"\nINFO - 2024-04-03T12:58:40Z -
-You forced selection of service: original-files\nINFO - 2024-04-03T12:58:40Z -
-Downloading using service original-files...\nINFO - 2024-04-03T12:58:41Z - You
-requested the download of the following files:\ns3://mdl-native-08/native/
+en/articles/9133855-how-to-download-insitu-data-using-index-files). Then the
+following command: ``` copernicusmarine get --dataset-id cmems_obs-
+ins_blk_phybgcwav_mynrt_na_irr --index-parts ``` Returns: ``` INFO - 2024-04-
+03T12:58:40Z - Dataset version was not specified, the latest one was selected:
+"202311" INFO - 2024-04-03T12:58:40Z - Dataset part was not specified, the
+first one was selected: "history" INFO - 2024-04-03T12:58:40Z - You forced
+selection of service: original-files INFO - 2024-04-03T12:58:40Z - Downloading
+using service original-files... INFO - 2024-04-03T12:58:41Z - You requested the
+download of the following files: s3://mdl-native-08/native/
 INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-
 ins_blk_phybgcwav_mynrt_na_irr_202311/index_history.txt - 333.13 kB - 2024-04-
-02T08:40:30Z\ns3://mdl-native-08/native/
+02T08:40:30Z s3://mdl-native-08/native/
 INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-
 ins_blk_phybgcwav_mynrt_na_irr_202311/index_latest.txt - 466.38 kB - 2024-04-
-03T12:51:52Z\ns3://mdl-native-08/native/
+03T12:51:52Z s3://mdl-native-08/native/
 INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-
 ins_blk_phybgcwav_mynrt_na_irr_202311/index_monthly.txt - 1.51 MB - 2024-03-
-05T18:09:43Z\ns3://mdl-native-08/native/
+05T18:09:43Z s3://mdl-native-08/native/
 INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-
 ins_blk_phybgcwav_mynrt_na_irr_202311/index_platform.txt - 209.27 kB - 2024-04-
-03T08:33:37Z\n\nTotal size of the download: 2.52 MB\nDo you want to proceed
-with download? [Y/n]:\n```\n\n### Shared options\nBoth `subset` and `get`
-commands provide these options:\n\n#### Option `--overwrite-output-data`\nWhen
-specified, the existing files will be overwritten.\nOtherwise, if the files
-already exist on destination, new ones with a unique index will be created once
-the download has been accepted (or once `--force-download` is
-provided).\n\n#### Option `--create-template`\nOption to create a file in your
-current directory containing request parameters. If specified, no other action
-will be performed.\nIt will create the following files depending on the
-feature:\n- `subset`\nExample:\n```bash\ncopernicusmarine subset --create-
-template\n```\nReturns:\n```txt\nINFO - 2024-04-04T14:38:09Z - Template created
-at: subset_template.json\n```\n- `get`\nExample:\n```bash\ncopernicusmarine get
---create-template\n```\nReturns:\n```txt\nINFO - 2024-04-04T14:38:09Z -
-Template created at: get_template.json\n```\n\n#### Option `--request-
-file`\nThis option allows to specify request parameters but in a provided
-`.json` file, useful for batch processing.\nYou can try the following templates
-or use the `--create-template` option to create both `subset` or `get` template
-request files.\n\n- Template for `subset` data request:\n```json\n{\n
-"dataset_id": "cmems_mod_glo_phy-thetao_anfc_0.083deg_P1D-m",\n
-"start_datetime": "2022-04-11",\n "end_datetime": "2023-08-11",\n
-"minimum_longitude": -182.79,\n "maximum_longitude": -179.69,\n
-"minimum_latitude": -40,\n "maximum_latitude": -36,\n "minimum_depth": 0,\n
-"maximum_depth": 0,\n "variables": ["thetao"],\n "output_directory": "./data/
-",\n "force_download": true\n}\n```\n\nExample:\n```bash\ncopernicusmarine
-subset --request-file template_subset_data_request.json\n```\n\n- Template for
-`get` data request:\n```json\n{\n "dataset_id": "cmems_mod_ibi_phy_my_0.083deg-
-3D_P1Y-m",\n "filter": "*01yav_200[0-2]*",\n "force_download": false,\n
-"log_level": "INFO",\n "no_directories": false,\n "no_metadata_cache": false,\n
-"output_directory": "./data/",\n "overwrite_output_data": false,\n
-"overwrite_metadata_cache": false,\n "show_outputnames":
-true\n}\n```\n\nExample:\n```bash\ncopernicusmarine get --request-file
-template_get_data_request.json\n```\n\n#### Option `--credentials-file`\nYou
+03T08:33:37Z Total size of the download: 2.52 MB Do you want to proceed with
+download? [Y/n]: ``` ### Shared options Both `subset` and `get` commands
+provide these options: #### Option `--overwrite-output-data` When specified,
+the existing files will be overwritten. Otherwise, if the files already exist
+on destination, new ones with a unique index will be created once the download
+has been accepted (or once `--force-download` is provided). #### Option `--
+create-template` Option to create a file in your current directory containing
+request parameters. If specified, no other action will be performed. It will
+create the following files depending on the feature: - `subset` Example:
+```bash copernicusmarine subset --create-template ``` Returns: ```txt INFO -
+2024-04-04T14:38:09Z - Template created at: subset_template.json ``` - `get`
+Example: ```bash copernicusmarine get --create-template ``` Returns: ```txt
+INFO - 2024-04-04T14:38:09Z - Template created at: get_template.json ``` ####
+Option `--request-file` This option allows to specify request parameters but in
+a provided `.json` file, useful for batch processing. You can try the following
+templates or use the `--create-template` option to create both `subset` or
+`get` template request files. - Template for `subset` data request: ```json
+{ "dataset_id": "cmems_mod_glo_phy-thetao_anfc_0.083deg_P1D-m",
+"start_datetime": "2022-04-11", "end_datetime": "2023-08-11",
+"minimum_longitude": -182.79, "maximum_longitude": -179.69, "minimum_latitude":
+-40, "maximum_latitude": -36, "minimum_depth": 0, "maximum_depth": 0,
+"variables": ["thetao"], "output_directory": "./data/", "force_download": true
+} ``` Example: ```bash copernicusmarine subset --request-file
+template_subset_data_request.json ``` - Template for `get` data request:
+```json { "dataset_id": "cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m", "filter":
+"*01yav_200[0-2]*", "force_download": false, "log_level": "INFO",
+"no_directories": false, "no_metadata_cache": false, "output_directory": "./
+data/", "overwrite_output_data": false, "overwrite_metadata_cache": false,
+"show_outputnames": true } ``` Example: ```bash copernicusmarine get --request-
+file template_get_data_request.json ``` #### Option `--credentials-file` You
 can use the `--credentials-file` option to point to a credentials file. The
 file can be either `.copernicusmarine-credentials`, `motuclient-python.ini`,
-`.netrc` or `_netrc`.\n\n#### Option `--dataset-version`\nYou can use the `--
+`.netrc` or `_netrc`. #### Option `--dataset-version` You can use the `--
 dataset-version` option to fetch a specific dataset version. Particularly
 useful to keep an operational chain working when an evolution impact the chosen
-dataset.\n\n#### Option `--dataset-part`\nYou can use the `--dataset-part`
-option to fecth a specific part for the chosen dataset version.\n\n#### Option
-`--log-level`\nSet the details printed to console by the command (based on
-standard logging library).\nAvailable values are: `
-[DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]`\n\n## Python package (API)\nThe
+dataset. #### Option `--dataset-part` You can use the `--dataset-part` option
+to fecth a specific part for the chosen dataset version. #### Option `--log-
+level` Set the details printed to console by the command (based on standard
+logging library). Available values are: `
+[DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]` ## Python package (API) The
 `copernicusmarine` exposes a Python interface to allow you to [call commands as
-functions](https://marine.copernicus.eu/python-interface).\n\n##
-Documentation\nA detailed standalone API documentation is under construction
-and will come at a later stage. For the moment, see the [Help Center](https://
-help.marine.copernicus.eu/en/collections/9054839-copernicus-marine-toolbox-
-guide).\n\n## Contribution\nWe welcome contributions from the community to
-enhance this package. If you find any issues or have suggestions for
-improvements, please check out our [Report Template](https://
-help.marine.copernicus.eu/en/articles/8218546-reporting-an-issue-or-feature-
-request).\n\n## Future improvements & Roadmap\nTo keep up to date with the most
-recent and planned advancements, including revisions, corrections, and feature
-requests generated from users\' feedback, please refer to our [Roadmap](https:/
-/help.marine.copernicus.eu/en/articles/8218641-next-milestones-and-
-roadmap).\n\n## Join the community\nGet in touch!\n- Create your [Copernicus
-Marine Account](https://data.marine.copernicus.eu/
-register?redirect=%2Fproducts)\n- [Log in](https://data.marine.copernicus.eu/
+functions](https://help.marine.copernicus.eu/en/collections/9054839-main-
+functionalities). ## Documentation A detailed standalone API documentation is
+under construction and will come at a later stage. For the moment, see the
+[Help Center](https://help.marine.copernicus.eu/en/collections/9080063-
+copernicus-marine-toolbox). ## Version management We are using semantic
+versioning X.Y.Z â for example 1.0.2 - Z is bumped on minor non-breaking
+changes. - Y is bumped on breaking changes. - X is bumped on demand to
+highlight a new significant feature or for communication purposes (new
+Copernicus Marine Service release for example). ## Contribution We welcome
+contributions from the community to enhance this package. If you find any
+issues or have suggestions for improvements, please check out our [Report
+Template](https://help.marine.copernicus.eu/en/articles/8218546-reporting-an-
+issue-or-feature-request). ## Future improvements & Roadmap To keep up to date
+with the most recent and planned advancements, including revisions,
+corrections, and feature requests generated from users' feedback, please refer
+to our [Roadmap](https://help.marine.copernicus.eu/en/articles/8218641-next-
+milestones-and-roadmap). ## Join the community Get in touch! - Create your
+[Copernicus Marine Account](https://data.marine.copernicus.eu/
+register?redirect=%2Fproducts) - [Log in](https://data.marine.copernicus.eu/
 login?redirect=%2Fproducts) and chat with us (bottom right corner of
-[Copernicus Marine Service](https://marine.copernicus.eu/))\n- Join our
+[Copernicus Marine Service](https://marine.copernicus.eu/)) - Join our
 [training workshops](https://marine.copernicus.eu/services/user-learning-
-services)\n- Network y/our [Copernicus Stories](https://twitter.com/
-cmems_eu)\n- Watch [our videos](https://www.youtube.com/channel/
-UC71ceOVy7WtVC7F04BKoEew)\n## Licence\nLicensed under the [EUPL](https://
-joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12)\n', 'author':
-'Copernicus Marine User Support', 'author_email': 'servicedesk.cmems@mercator-
-ocean.eu', 'maintainer': 'None', 'maintainer_email': 'None', 'url': 'None',
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'entry_points': entry_points, 'python_requires':
-'>=3.9,<3.13', } setup(**setup_kwargs)
+services) - Network y/our [Copernicus Stories](https://twitter.com/cmems_eu) -
+Watch [our videos](https://www.youtube.com/channel/UC71ceOVy7WtVC7F04BKoEew) ##
+Licence Licensed under the [EUPL](https://joinup.ec.europa.eu/collection/eupl/
+eupl-text-eupl-12)
```

