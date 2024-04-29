# Comparing `tmp/pyllsm5dtools-1.0.4.tar.gz` & `tmp/pyllsm5dtools-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllsm5dtools-1.0.4.tar", last modified: Fri Apr 19 06:32:15 2024, max compression
+gzip compressed data, was "pyllsm5dtools-1.0.5.tar", last modified: Mon Apr 29 22:29:58 2024, max compression
```

## Comparing `pyllsm5dtools-1.0.4.tar` & `pyllsm5dtools-1.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-19 06:32:15.899747 pyllsm5dtools-1.0.4/
--rw-rw-r--   0 matt      (1000) matt      (1000)      819 2024-03-05 21:34:03.000000 pyllsm5dtools-1.0.4/LICENSE.txt
--rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-04-19 06:32:15.899747 pyllsm5dtools-1.0.4/PKG-INFO
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-19 06:32:15.899747 pyllsm5dtools-1.0.4/PyLLSM5DTools/
--rw-rw-r--   0 matt      (1000) matt      (1000)     3463 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_FSC_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2885 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_MIP_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3130 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_crop_dataset.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6463 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_decon_data_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5031 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2640 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6542 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_matlab_stitching_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     8046 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3179 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_psf_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3055 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3219 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_resample_dataset.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3313 2024-04-19 06:26:42.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_tiffToZarr_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2062 2024-04-19 06:26:42.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2688 2024-04-19 06:26:42.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_zarrToTiff_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      957 2024-04-19 06:26:42.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     8944 2024-04-05 00:37:52.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/generatePythonWrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1122 2024-03-27 21:30:52.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/generate_config_file.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-19 06:32:15.899747 pyllsm5dtools-1.0.4/PyLLSM5DTools.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-04-19 06:32:15.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      879 2024-04-19 06:32:15.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-04-19 06:32:15.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       14 2024-04-19 06:32:15.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)     1206 2024-03-27 20:42:06.000000 pyllsm5dtools-1.0.4/README.md
--rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-04-19 06:32:15.899747 pyllsm5dtools-1.0.4/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)     3638 2024-04-19 06:30:57.000000 pyllsm5dtools-1.0.4/setup.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-29 22:29:58.066394 pyllsm5dtools-1.0.5/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      819 2024-03-05 21:34:03.000000 pyllsm5dtools-1.0.5/LICENSE.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-04-29 22:29:58.066394 pyllsm5dtools-1.0.5/PKG-INFO
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-29 22:29:58.062394 pyllsm5dtools-1.0.5/PyLLSM5DTools/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3463 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_FSC_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2885 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_MIP_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3130 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_crop_dataset.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6463 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_decon_data_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5031 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2640 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6472 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_matlab_stitching_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     8046 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3179 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_psf_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3055 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3219 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_resample_dataset.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3313 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_tiffToZarr_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2062 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2688 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_zarrToTiff_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      957 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     8944 2024-04-05 00:37:52.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/generatePythonWrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1122 2024-03-27 21:30:52.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/generate_config_file.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-29 22:29:58.066394 pyllsm5dtools-1.0.5/PyLLSM5DTools.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-04-29 22:29:58.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)      879 2024-04-29 22:29:58.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-04-29 22:29:58.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       14 2024-04-29 22:29:58.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools.egg-info/top_level.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1206 2024-03-27 20:42:06.000000 pyllsm5dtools-1.0.5/README.md
+-rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-04-29 22:29:58.066394 pyllsm5dtools-1.0.5/setup.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3638 2024-04-29 22:28:38.000000 pyllsm5dtools-1.0.5/setup.py
```

### Comparing `pyllsm5dtools-1.0.4/LICENSE.txt` & `pyllsm5dtools-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_FSC_analysis_wrapper.py` & `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_FSC_analysis_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_MIP_wrapper.py` & `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_MIP_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_crop_dataset.py` & `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_crop_dataset.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_decon_data_wrapper.py` & `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_decon_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py` & `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py` & `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_matlab_stitching_wrapper.py` & `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_matlab_stitching_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         "IOScan": [kwargs.get("IOScan", False), "logical"],
         "zarrFile": [kwargs.get("zarrFile", False), "logical"],
         "largeZarr": [kwargs.get("largeZarr", False), "logical"],
         "poolSize": [kwargs.get("poolSize", []), "numericScalar"],
         "batchSize": [kwargs.get("batchSize", [500,500,500]), "numericArr"],
         "blockSize": [kwargs.get("blockSize", [500,500,500]), "numericArr"],
         "shardSize": [kwargs.get("shardSize", []), "numericArr"],
-        "zarrSubSize": [kwargs.get("zarrSubSize", []), "numericArr"],
         "resampleType": [kwargs.get("resampleType", "xy_isotropic"), "char"],
         "resample": [kwargs.get("resample", []), "numericArr"],
         "InputBbox": [kwargs.get("InputBbox", []), "numericArr"],
         "tileOutBbox": [kwargs.get("tileOutBbox", []), "numericArr"],
         "TileOffset": [kwargs.get("TileOffset", 0), "numericScalar"],
         "Resolution": [kwargs.get("Resolution", [0.108,0.5]), "numericArr"],
         "resultDir": [kwargs.get("resultDir", "matlab_stitch"), "char"],
```

### Comparing `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py` & `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_psf_analysis_wrapper.py` & `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_psf_analysis_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py` & `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_resample_dataset.py` & `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_resample_dataset.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_tiffToZarr_wrapper.py` & `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_tiffToZarr_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py` & `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_zarrToTiff_wrapper.py` & `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_zarrToTiff_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.4/PyLLSM5DTools/__init__.py` & `pyllsm5dtools-1.0.5/PyLLSM5DTools/__init__.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.4/PyLLSM5DTools/generatePythonWrapper.py` & `pyllsm5dtools-1.0.5/PyLLSM5DTools/generatePythonWrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.4/PyLLSM5DTools/generate_config_file.py` & `pyllsm5dtools-1.0.5/PyLLSM5DTools/generate_config_file.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.4/PyLLSM5DTools.egg-info/SOURCES.txt` & `pyllsm5dtools-1.0.5/PyLLSM5DTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.4/README.md` & `pyllsm5dtools-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.4/setup.py` & `pyllsm5dtools-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
 matlab_runtime_url = ("https://ssd.mathworks.com/supportfiles/downloads/R2023a/Release/6/deployment_files"
                       "/installer/complete/glnxa64/MATLAB_Runtime_R2023a_Update_6_glnxa64.zip")
 name = 'PyLLSM5DTools'
-version = '1.0.4'
+version = '1.0.5'
 
 
 class CustomInstall(install):
     def download_and_extract_matlab_runtime(self, install_dir):
         llsm5dtools_url = "https://github.com/abcucberkeley/LLSM5DTools/archive/refs/heads/main.zip"
         llsm5dtools_github_dir = os.path.join(install_dir, "LLSM5DTools-main")
         llsm5dtools_dir = os.path.join(install_dir, "LLSM5DTools")
```

