# Comparing `tmp/tekrsa_api_wrap-1.3.2.tar.gz` & `tmp/tekrsa_api_wrap-1.3.3.tar.gz`

## Comparing `tekrsa_api_wrap-1.3.2.tar` & `tekrsa_api_wrap-1.3.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.2/.markdownlint.yaml
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.2/GitHubRepoPublicReleaseApproval.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.2/src/rsa_api/__init__.py
--rw-r--r--   0        0        0    93191 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.2/src/rsa_api/rsa_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.2/tests/__init__.py
--rw-r--r--   0        0        0    21886 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.2/tests/test_rsa_api.py
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.2/.gitignore
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.2/LICENSE.md
--rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.2/README.md
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.2/pyproject.toml
--rw-r--r--   0        0        0    12496 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.3/.markdownlint.yaml
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.3/GitHubRepoPublicReleaseApproval.md
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.3/ex.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.3/src/rsa_api/__init__.py
+-rw-r--r--   0        0        0    93633 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.3/src/rsa_api/rsa_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.3/tests/__init__.py
+-rw-r--r--   0        0        0    21886 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.3/tests/test_rsa_api.py
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.3/.gitignore
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.3/LICENSE.md
+-rw-r--r--   0        0        0     8928 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.3/README.md
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0    12770 2020-02-02 00:00:00.000000 tekrsa_api_wrap-1.3.3/PKG-INFO
```

### Comparing `tekrsa_api_wrap-1.3.2/.pre-commit-config.yaml` & `tekrsa_api_wrap-1.3.3/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 default_language_version:
   python: python3.8
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.5.0
     hooks:
       - id: check-ast
         types: [file, python]
       - id: check-case-conflict
       - id: check-docstring-first
         types: [file, python]
       - id: check-merge-conflict
       - id: debug-statements
         types: [file, python]
       - id: detect-private-key
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.15.2
     hooks:
       - id: pyupgrade
-        args: ["--py3-plus"]
+        args: ["--py38-plus"]
   - repo: https://github.com/pycqa/isort
-    rev: 5.12.0
+    rev: 5.13.2
     hooks:
       - id: isort
         name: isort (python)
         types: [file, python]
         args: ["--profile", "black", "--filter-files", "--gitignore"]
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 24.4.2
     hooks:
       - id: black
         types: [file, python]
   - repo: https://github.com/igorshubovych/markdownlint-cli
-    rev: v0.33.0
+    rev: v0.40.0
     hooks:
       - id: markdownlint
         types: [file, markdown]
-        exclude: GitHubRepoPublicReleaseApproval.md|LICENSE.md
+        exclude: GitHubRepoPublicReleaseApproval.md
```

### Comparing `tekrsa_api_wrap-1.3.2/GitHubRepoPublicReleaseApproval.md` & `tekrsa_api_wrap-1.3.3/GitHubRepoPublicReleaseApproval.md`

 * *Files identical despite different names*

### Comparing `tekrsa_api_wrap-1.3.2/src/rsa_api/rsa_api.py` & `tekrsa_api_wrap-1.3.3/src/rsa_api/rsa_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 """
 Written for Tektronix RSA API for Linux v1.0.0014
 Refer to the RSA API Programming Reference Manual for details
 on any functions implemented from this module.
 """
+
+import logging
 import tempfile
 from ctypes import *
 from enum import Enum
 from os.path import abspath, join
 from time import sleep
 from typing import Any, Tuple, Union
 
 import numpy as np
 
+logger = logging.getLogger(__name__)
 # GLOBAL CONSTANTS
 
-_MAX_NUM_DEVICES = 10  # Max num. of devices that could be found
-_MAX_SERIAL_STRLEN = 8  # Bytes allocated for serial number string
-_MAX_DEVTYPE_STRLEN = 8  # Bytes allocated for device type string
-_FPGA_VERSION_STRLEN = 6  # Bytes allocated for FPGA version number string
-_FW_VERSION_STRLEN = 6  # Bytes allocated for FW version number string
-_HW_VERSION_STRLEN = 4  # Bytes allocated for HW version number string
-_NOMENCLATURE_STRLEN = 8  # Bytes allocated for device nomenclature string
-_API_VERSION_STRLEN = 8  # Bytes allocated for API version number string
+_DEVSRCH_MAX_NUM_DEVICES = 20  # Max num. of devices that could be found
+_DEVSRCH_SERIAL_MAX_STRLEN = 100  # Char array size allocated for serial number string
+_DEVSRCH_TYPE_MAX_STRLEN = 20  # Char array size allocated for device type string
+_DEVINFO_MAX_STRLEN = 100  # Char array max size to allocate for DEVICE_Get* functions
 _FREQ_REF_USER_SETTING_STRLEN = (
     200  # Max. characters in frequency reference user setting string
 )
-_DEVINFO_MAX_STRLEN = 19  # Datetime substring length in user setting string
 
 # ENUMERATION TUPLES
 
 _DEV_EVENT = ("OVERRANGE", "TRIGGER", "1PPS")
 _FREQ_REF_SOURCE = ("INTERNAL", "EXTREF", "GNSS", "USER")
 _IQS_OUT_DEST = ("CLIENT", "FILE_TIQ", "FILE_SIQ", "FILE_SIQ_SPLIT")
 _IQS_OUT_DTYPE = ("SINGLE", "INT32", "INT16", "SINGLE_SCALE_INT32")
@@ -48,82 +46,93 @@
 _TRIGGER_MODE = ("freerun", "triggered")
 _TRIGGER_SOURCE = ("External", "IFPowerLevel")
 _TRIGGER_TRANSITION = ("LH", "HL", "Either")
 
 # CUSTOM DATA STRUCTURES
 
 
+class _DeviceInfo(Structure):
+    _fields_ = [
+        ("nomenclature", c_char * _DEVINFO_MAX_STRLEN),
+        ("serialNum", c_char * _DEVINFO_MAX_STRLEN),
+        ("apiVersion", c_char * _DEVINFO_MAX_STRLEN),
+        ("fwVersion", c_char * _DEVINFO_MAX_STRLEN),
+        ("fpgaVersion", c_char * _DEVINFO_MAX_STRLEN),
+        ("hwVersion", c_char * _DEVINFO_MAX_STRLEN),
+    ]
+
+
 class _FreqRefUserInfo(Structure):
     _fields_ = [
         ("isvalid", c_bool),
         ("dacValue", c_uint32),
         ("datetime", c_char * _DEVINFO_MAX_STRLEN),
-        (
-            "temperature",
-            c_double,
-        ),  # Documentation indicates this field exists. Testing indicates otherwise.
+        ("temperature", c_double),
     ]
 
 
 class _SpectrumLimits(Structure):
     _fields_ = [
         ("maxSpan", c_double),
         ("minSpan", c_double),
         ("maxRBW", c_double),
         ("minRBW", c_double),
         ("maxVBW", c_double),
         ("minVBW", c_double),
         ("maxTraceLength", c_int),  # Incorrectly documented as a double
-        ("minTraceLength", c_int),
-    ]  # Incorrectly documented as a double
+        ("minTraceLength", c_int),  # Incorrectly documented as a double
+    ]
 
 
 class _SpectrumSettings(Structure):
     _fields_ = [
         ("span", c_double),
         ("rbw", c_double),
         ("enableVBW", c_bool),
         ("vbw", c_double),
-        ("traceLength", c_int),
-        ("window", c_int),
-        ("verticalUnit", c_int),
+        ("traceLength", c_int),  # Must be an odd number
+        ("window", c_int),  # Really a SpectrumWindows enum value
+        ("verticalUnit", c_int),  # Really a SpectrumVerticalUnits enum value
         ("actualStartFreq", c_double),
         ("actualStopFreq", c_double),
         ("actualFreqStepSize", c_double),
         ("actualRBW", c_double),
         ("actualVBW", c_double),
         ("actualNumIQSamples", c_int),
     ]
 
 
 class _SpectrumTraceInfo(Structure):
-    _fields_ = [("timestamp", c_int64), ("acqDataStatus", c_uint16)]
+    _fields_ = [
+        ("timestamp", c_uint64),
+        ("acqDataStatus", c_uint16),
+    ]
 
 
 class _IQBlkAcqInfo(Structure):
     _fields_ = [
         ("sample0Timestamp", c_uint64),
         ("triggerSampleIndex", c_uint64),
         ("triggerTimestamp", c_uint64),
         ("acqStatus", c_uint32),
     ]
 
 
-class _IQStreamFileInfo(Structure):
+class _IQStreamFileInfo(Structure):  # "IQSTRMFILEINFO" in RSA_API.h
     _fields_ = [
         ("numberSamples", c_uint64),
         ("sample0Timestamp", c_uint64),
         ("triggerSampleIndex", c_uint64),
         ("triggerTimestamp", c_uint64),
         ("acqStatus", c_uint32),
-        ("filenames", c_wchar_p),
+        ("filenames", POINTER(c_wchar_p)),
     ]
 
 
-class _IQStreamIQInfo(Structure):
+class _IQStreamIQInfo(Structure):  # "IQSTRMIQINFO" in RSA_API.h
     _fields_ = [
         ("timestamp", c_uint64),
         ("triggerCount", c_int),
         ("triggerIndices", POINTER(c_int)),
         ("scaleFactor", c_double),
         ("acqStatus", c_uint32),
     ]
@@ -131,15 +140,15 @@
 
 # ERROR HANDLING
 
 
 class RSAError(Exception):
     def __init__(self, err_txt=""):
         self.err_txt = err_txt
-        err = "RSA Error: {}".format(self.err_txt)
+        err = f"RSA Error: {self.err_txt}"
         super().__init__(err)
 
 
 class RSA:
     def __init__(self, so_dir: str = "/drivers/"):
         """Load the RSA USB Driver"""
         # Param. 'so_dir' is the directory containing libRSA_API.so and
@@ -156,27 +165,31 @@
 
         # Connection
         errorNotConnected = 101
         errorIncompatibleFirmware = 102
         errorBootLoaderNotRunning = 103
         errorTooManyBootLoadersConnected = 104
         errorRebootFailure = 105
+        errorGNSSNotInstalled = 106
+        errorGNSSNotEnabled = 107
 
         # POST
         errorPOSTFailureFPGALoad = 201
         errorPOSTFailureHiPower = 202
         errorPOSTFailureI2C = 203
         errorPOSTFailureGPIF = 204
         errorPOSTFailureUsbSpeed = 205
         errorPOSTDiagFailure = 206
+        errorPOSTFailure3P3VSense = 207
+        errorPOSTLinkFailure = 208
 
         # General Msmt
         errorBufferAllocFailed = 301
         errorParameter = 302
-        errorDataNotReady = 304
+        errorDataNotReady = 303
 
         # Spectrum
         errorParameterTraceLength = 1101
         errorMeasurementNotEnabled = 1102
         errorSpanIsLessThanRBW = 1103
         errorFrequencyOutOfRange = 1104
 
@@ -187,19 +200,22 @@
         errorStreamADCToDiskThreadFailure = 1204
         errorStreamedFileInvalidHeader = 1205
         errorStreamedFileOpenFailure = 1206
         errorStreamingOperationNotSupported = 1207
         errorStreamingFastForwardTimeInvalid = 1208
         errorStreamingInvalidParameters = 1209
         errorStreamingEOF = 1210
+        errorStreamingIfReadTimeout = 1211
+        errorStreamingIfNotEnabled = 1212
 
         # IQ streaming
         errorIQStreamInvalidFileDataType = 1301
         errorIQStreamFileOpenFailed = 1302
         errorIQStreamBandwidthOutOfRange = 1303
+        errorIQStreamingNotEnabled = 1304
 
         # -----------------
         # Internal errors
         # -----------------
         errorTimeout = 3001
         errorTransfer = 3002
         errorFileOpen = 3003
@@ -209,20 +225,22 @@
         errorChangeToRunMode = 3007
         errorDSPLError = 3008
         errorLOLockFailure = 3009
         errorExternalReferenceNotEnabled = 3010
         errorLogFailure = 3011
         errorRegisterIO = 3012
         errorFileRead = 3013
+        errorConsumerNotActive = 3014
 
         errorDisconnectedDeviceRemoved = 3101
         errorDisconnectedDeviceNodeChangedAndRemoved = 3102
         errorDisconnectedTimeoutWaitingForADcData = 3103
         errorDisconnectedIOBeginTransfer = 3104
         errorOperationNotSupportedInSimMode = 3015
+        errorDisconnectedIOFinishTransfer = 3016
 
         errorFPGAConfigureFailure = 3201
         errorCalCWNormFailure = 3202
         errorSystemAppDataDirectory = 3203
         errorFileCreateMRU = 3204
         errorDeleteUnsuitableCachePath = 3205
         errorUnableToSetFilePermissions = 3206
@@ -244,15 +262,15 @@
         errorEraseCalConfig = 3305
         errorCalConfigFileSize = 3306
         errorInvalidCalibConstantFileFormat = 3307
         errorMismatchCalibConstantsSize = 3308
         errorCalConfigInvalid = 3309
 
         # flash
-        errorFlashFileSystemUnexpectedSize = (3401,)
+        errorFlashFileSystemUnexpectedSize = 3401
         errorFlashFileSystemNotMounted = 3402
         errorFlashFileSystemOutOfRange = 3403
         errorFlashFileSystemIndexNotFound = 3404
         errorFlashFileSystemReadErrorCRC = 3405
         errorFlashFileSystemReadFileMissing = 3406
         errorFlashFileSystemCreateCacheIndex = 3407
         errorFlashFileSystemCreateCachedDataFile = 3408
@@ -265,17 +283,24 @@
         errorFlashFileSystemImportFileError = 3415
         errorFlashFileSystemFileNotFoundError = 3416
         errorFlashFileSystemReadBufferTooSmall = 3417
         errorFlashWriteFailure = 3418
         errorFlashReadFailure = 3419
         errorFlashFileSystemBadArgument = 3420
         errorFlashFileSystemCreateFile = 3421
+        errorARchiveDirectoryNotFound = 3422
+        errorArchiveDirectoryNotWriteable = 3423
+        errorArchiveWriteFile = 3424
+        errorArchiveGenerateFilename = 3425
+        errorArchiveBoost = 3426
+        errorArchiveStd = 3427
+        errorArchiveGeneric = 3428
 
         # Aux monitoring
-        errorMonitoringNotSupported = (3501,)
+        errorMonitoringNotSupported = 3501
         errorAuxDataNotAvailable = 3502
 
         # battery
         errorBatteryCommFailure = 3601
         errorBatteryChargerCommFailure = 3602
         errorBatteryNotPresent = 3603
 
@@ -291,14 +316,28 @@
 
         # alignment
         error112MHzAlignmentSignalLevelTooLow = 3901
         error10MHzAlignmentSignalLevelTooLow = 3902
         errorInvalidCalConstant = 3903
         errorNormalizationCacheInvalid = 3904
         errorInvalidAlignmentCache = 3905
+        errorLockExtRefAfterAlignment = 3906
+
+        # Triggering
+        errorTriggerSystem = 4000
+
+        # VNA
+        errorVNAUnsupportedConfiguration = 4100
+
+        # MFC
+        errorMFCHWNotPresent = 4200
+        errorMFCWriteCalFile = 4201
+        errorMFCReadCalFile = 4202
+        errorMFCFileFormatError = 4203
+        errorMFCFlashCorruptDataError = 4204
 
         # acq status
         errorADCOverrange = 9000  # must not change the location of these error codes without coordinating with MFG TEST
         errorOscUnlock = 9001
 
         errorNotSupported = 9901
 
@@ -526,25 +565,27 @@
                 was created.
         """
         i_usstr = c_char_p(i_usstr.encode("utf-8"))
         o_fui = _FreqRefUserInfo()
         self.err_check(
             self.rsa.CONFIG_DecodeFreqRefUserSettingString(i_usstr, byref(o_fui))
         )
-        # Temperature result in o_fui is always 0.0 due to broken RSA API
-        # Therefore, it must be retrieved directly from i_usstr.
-        # Strip checksum so temperature can be parsed (checksum has variable digits)
-        i_usstr = i_usstr.value.decode("utf-8").split("*", 1)[0]
-        temperature = float(i_usstr[-5:])
+        try:
+            logger.debug(f"FreqRefUserInfo.isvalid {o_fui.isvalid}")
+            logger.debug(f"FreqRefUserInfo.dacValue {o_fui.dacValue}")
+            logger.debug(f"FreqRefUserInfo.datetime: {o_fui.datetime}")
+            logger.debug(f"FreqRefUserInfo.temperature: {o_fui.temperature}")
+        except Exception as ex:
+            logger.debug(f"unable to print decoded values: {ex}")
 
         fui = {
             "isvalid": o_fui.isvalid,
             "dacValue": o_fui.dacValue,
             "datetime": o_fui.datetime.decode("utf-8"),
-            "temperature": temperature,
+            "temperature": o_fui.temperature,
         }
         return fui
 
     def CONFIG_SetExternalRefEnable(self, ext_ref_en: bool) -> None:
         """
         Enable or disable the external reference.
 
@@ -572,16 +613,17 @@
         Raises
         ------
         RSAError
             If the input string does not match one of the valid settings.
         """
         src = RSA.check_string(src)
         if src in _FREQ_REF_SOURCE:
-            if src == "GNSS" and self.DEVICE_GetNomenclature() in ["RSA306", "RSA306B"]:
-                raise RSAError("RSA 300 series device does not support GNSS reference.")
+            device_name = self.DEVICE_GetNomenclature()
+            if src == "GNSS" and device_name in ["RSA306", "RSA306B"]:
+                raise RSAError(f"{device_name} device does not support GNSS reference.")
             else:
                 value = c_int(_FREQ_REF_SOURCE.index(src))
                 self.err_check(self.rsa.CONFIG_SetFrequencyReferenceSource(value))
         else:
             raise RSAError("Input does not match a valid setting.")
 
     def CONFIG_GetFreqRefUserSetting(self) -> str:
@@ -775,80 +817,80 @@
         Retrieve the FPGA version number.
 
         Returns
         -------
         string
             The FPGA version number.
         """
-        fpga_version = (c_char * _FPGA_VERSION_STRLEN)()
+        fpga_version = (c_char * _DEVINFO_MAX_STRLEN)()
         self.err_check(self.rsa.DEVICE_GetFPGAVersion(byref(fpga_version)))
         return fpga_version.value.decode("utf-8")
 
     def DEVICE_GetFWVersion(self) -> str:
         """
         Retrieve the firmware version number.
 
         Returns
         -------
         string
             The firmware version number.
         """
-        fw_version = (c_char * _FW_VERSION_STRLEN)()
+        fw_version = (c_char * _DEVINFO_MAX_STRLEN)()
         self.err_check(self.rsa.DEVICE_GetFWVersion(byref(fw_version)))
         return fw_version.value.decode("utf-8")
 
     def DEVICE_GetHWVersion(self) -> str:
         """
         Retrieve the hardware version number.
 
         Returns
         -------
         string
             The hardware version number.
         """
-        hw_version = (c_char * _HW_VERSION_STRLEN)()
+        hw_version = (c_char * _DEVINFO_MAX_STRLEN)()
         self.err_check(self.rsa.DEVICE_GetHWVersion(byref(hw_version)))
         return hw_version.value.decode("utf-8")
 
     def DEVICE_GetNomenclature(self) -> str:
         """
         Retrieve the name of the device.
 
         Returns
         -------
         string
             Name of the device.
         """
-        nomenclature = (c_char * _NOMENCLATURE_STRLEN)()
+        nomenclature = (c_char * _DEVINFO_MAX_STRLEN)()
         self.err_check(self.rsa.DEVICE_GetNomenclature(byref(nomenclature)))
         return nomenclature.value.decode("utf-8")
 
     def DEVICE_GetSerialNumber(self) -> str:
         """
         Retrieve the serial number of the device.
 
         Returns
         -------
         string
             Serial number of the device.
         """
-        serial_num = (c_char * _MAX_SERIAL_STRLEN)()
+        serial_num = (c_char * _DEVSRCH_SERIAL_MAX_STRLEN)()
         self.err_check(self.rsa.DEVICE_GetSerialNumber(byref(serial_num)))
         return serial_num.value.decode("utf-8")
 
     def DEVICE_GetAPIVersion(self) -> str:
         """
         Retrieve the API version number.
 
         Returns
         -------
         string
             The API version number.
         """
-        api_version = (c_char * _API_VERSION_STRLEN)()
+        api_version = (c_char * _DEVINFO_MAX_STRLEN)()
         self.err_check(self.rsa.DEVICE_GetAPIVersion(byref(api_version)))
         return api_version.value.decode("utf-8")
 
     def DEVICE_PrepareForRun(self) -> None:
         """
         Put the system in a known state, ready to stream data.
         """
@@ -860,27 +902,23 @@
 
         Returns
         -------
         dict
             Keys: nomenclature, serialNum, fwVersion, fpgaVersion,
                   hwVersion, apiVersion
         """
-        nomenclature = self.DEVICE_GetNomenclature()
-        serial_num = self.DEVICE_GetSerialNumber()
-        fw_version = self.DEVICE_GetFWVersion()
-        fpga_version = self.DEVICE_GetFPGAVersion()
-        hw_version = self.DEVICE_GetHWVersion()
-        api_version = self.DEVICE_GetAPIVersion()
+        dev_info = _DeviceInfo()
+        self.err_check(self.rsa.DEVICE_GetInfo(byref(dev_info)))
         info = {
-            "nomenclature": nomenclature,
-            "serialNum": serial_num,
-            "fwVersion": fw_version,
-            "fpgaVersion": fpga_version,
-            "hwVersion": hw_version,
-            "apiVersion": api_version,
+            "nomenclature": dev_info.nomenclature.decode("utf-8"),
+            "serialNum": dev_info.serialNum.decode("utf-8"),
+            "apiVersion": dev_info.apiVersion.decode("utf-8"),
+            "fwVersion": dev_info.fwVersion.decode("utf-8"),
+            "fpgaVersion": dev_info.fpgaVersion.decode("utf-8"),
+            "hwVersion": dev_info.hwVersion.decode("utf-8"),
         }
         return info
 
     def DEVICE_GetOverTemperatureStatus(self) -> bool:
         """
         Query device for over-temperature status.
 
@@ -938,17 +976,19 @@
 
         Raises
         ------
         RSAError
             If no devices are found.
         """
         num_found = c_int()
-        dev_ids = (c_int * _MAX_NUM_DEVICES)()
-        dev_serial = ((c_char * _MAX_NUM_DEVICES) * _MAX_SERIAL_STRLEN)()
-        dev_type = ((c_char * _MAX_NUM_DEVICES) * _MAX_DEVTYPE_STRLEN)()
+        dev_ids = (c_int * _DEVSRCH_MAX_NUM_DEVICES)()
+        dev_serial = (
+            (c_char * _DEVSRCH_MAX_NUM_DEVICES) * _DEVSRCH_SERIAL_MAX_STRLEN
+        )()
+        dev_type = ((c_char * _DEVSRCH_MAX_NUM_DEVICES) * _DEVSRCH_TYPE_MAX_STRLEN)()
 
         self.err_check(
             self.rsa.DEVICE_Search(
                 byref(num_found), byref(dev_ids), dev_serial, dev_type
             )
         )
 
@@ -2216,21 +2256,31 @@
             self.DEVICE_PrepareForRun()
 
             # Collect data
             complete = False
 
             self.DEVICE_Run()
             self.IQSTREAM_Start()
+            sleep_time = (duration_msec + 1) / 1000
+            logger.debug(f"Started IQ stream. Sleeping for {sleep_time}")
+            sleep(sleep_time)
+            complete = self.IQSTREAM_GetDiskFileWriteStatus()[0]
+            logger.debug(f"File write complete: {complete}")
             while not complete:
+                logger.debug(f"Sleeping for {sleep_time_sec}")
                 sleep(sleep_time_sec)
                 complete = self.IQSTREAM_GetDiskFileWriteStatus()[0]
+                logger.debug(f"File write complete: {complete}")
+            logger.debug("Stopping stream.")
             self.IQSTREAM_Stop()
 
             # Check acquisition status
             file_info = self.IQSTREAM_GetDiskFileInfo()
+            logger.debug(f"Status: {file_info.acqStatus}")
+            logger.debug(f"Filename: {file_info.filenames.contents.value}")
             iq_status = self.IQSTREAMFileInfo_StatusParser(file_info, not return_status)
 
             self.DEVICE_Stop()
 
             # Read data back in from file
             with open(filename_base + ".siqd", "rb") as f:
                 d = np.frombuffer(f.read(), dtype=np.float32)
@@ -2253,15 +2303,17 @@
         ref_level: Union[float, int],
         bw: Union[float, int],
         duration_msec: int,
         return_status: bool = False,
     ) -> Union[np.ndarray, Tuple[np.ndarray, str]]:
         """
         Retrieve IQ data from device by first writing to a tempfile.
-        Performs device configuration before capturing.
+        Tunes device parameters before recording: center frequency,
+        reference level, and IQ bandwidth. Does not adjust preamp
+        or attenuation settings for RSA500/600 devices.
 
         Parameters
         ----------
         cf : float or int
             Center frequency value in Hz.
         ref_level : float or int
             Reference level value in dBm.
@@ -2278,70 +2330,24 @@
         -------
         iq_data : np.ndarray of np.complex64 values
             IQ data, with each element in the form (I + j*Q)
         iq_status : str (optional)
             The status code for the IQ capture, as defined in
             the documentation for IQSTREAMFileInfo_StatusParser().
         """
-        # Configuration parameters
-        dest = _IQS_OUT_DEST[3]  # Split SIQ format
-        dtype = _IQS_OUT_DTYPE[0]  # 32-bit single precision floating point
-        suffix_ctl = -2  # No file suffix
-        filename = "tempIQ"
-        sleep_time_sec = 0.05  # Loop sleep time checking if acquisition complete
-
-        # Ensure device is stopped before proceeding
-        self.DEVICE_Stop()
-
-        # Create temp directory and configure/collect data
-        with tempfile.TemporaryDirectory() as tmp_dir:
-            filename_base = tmp_dir + "/" + filename
-
-            # Configure device
-            self.CONFIG_SetCenterFreq(cf)
-            self.CONFIG_SetReferenceLevel(ref_level)
-            self.IQSTREAM_SetAcqBandwidth(bw)
-            self.IQSTREAM_SetOutputConfiguration(dest, dtype)
-            self.IQSTREAM_SetDiskFilenameBase(filename_base)
-            self.IQSTREAM_SetDiskFilenameSuffix(suffix_ctl)
-            self.IQSTREAM_SetDiskFileLength(duration_msec)
-            self.IQSTREAM_ClearAcqStatus()
-            self.DEVICE_PrepareForRun()
-
-            # Collect data
-            complete = False
-
-            self.DEVICE_Run()
-            self.IQSTREAM_Start()
-            while not complete:
-                sleep(sleep_time_sec)
-                complete = self.IQSTREAM_GetDiskFileWriteStatus()[0]
-            self.IQSTREAM_Stop()
-
-            # Check acquisition status
-            file_info = self.IQSTREAM_GetDiskFileInfo()
-            iq_status = self.IQSTREAMFileInfo_StatusParser(file_info, not return_status)
-
-            self.DEVICE_Stop()
-
-            # Read data back in from file
-            with open(filename_base + ".siqd", "rb") as f:
-                d = np.frombuffer(f.read(), dtype=np.float32)
-
-        # Deinterleave I and Q
-        i = d[0:-1:2]
-        q = np.append(d[1:-1:2], d[-1])
-        # Re-interleave as numpy complex64)
-        iq_data = i + 1j * q
-        assert iq_data.dtype == np.complex64
+        logger.warning(
+            "IQSTREAM_Tempfile is not recommended! Use IQSTREAM_Tempfile_NoConfig instead."
+        )
+        # Configure the device: tune frequency and
+        self.CONFIG_SetCenterFreq(cf)
+        self.CONFIG_SetReferenceLevel(ref_level)
+        self.IQSTREAM_SetAcqBandwidth(bw)
 
-        if return_status:
-            return iq_data, iq_status
-        else:
-            return iq_data
+        # Retrieve IQ data (and, optionally, status message)
+        return self.IQSTREAM_Tempfile_NoConfig(duration_msec, return_status)
 
     @staticmethod
     def IQSTREAMFileInfo_StatusParser(
         iq_stream_info: _IQStreamFileInfo, exit: bool = True
     ) -> Union[None, str]:
         """
         Parse an _IQStreamFileInfo struct to get the acquisition status.
```

### Comparing `tekrsa_api_wrap-1.3.2/tests/test_rsa_api.py` & `tekrsa_api_wrap-1.3.3/tests/test_rsa_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This is a test for the entire API Wrapper.
 It requires a compatible RSA device to be connected.
 """
+
 import unittest
 from os import environ, mkdir
 from os.path import isdir
 from time import sleep
 
 import numpy as np
 
@@ -553,13 +554,13 @@
     #     self.rsa.SPECTRUM_SetSettings(
     #         span, rbw, enableVBW, vbw, traceLength, window, verticalUnit
     #     )
     #     spectrum, outTracePoints = self.rsa.SPECTRUM_Acquire(
     #         trace="Trace1", trace_points=traceLength
     #     )
     #     self.assertEqual(len(spectrum), traceLength)
-    #     self.assertIsInstance(spectrum, np.ndarray)s
+    #     self.assertIsInstance(spectrum, np.ndarray)
     #     self.assertRaises(TypeError, self.rsa.SPECTRUM_Acquire, trace=1)
 
     #     traceInfo = self.rsa.SPECTRUM_GetTraceInfo()
     #     self.assertIsInstance(traceInfo, dict)
     #     self.assertEqual(len(traceInfo), 2)
```

### Comparing `tekrsa_api_wrap-1.3.2/.gitignore` & `tekrsa_api_wrap-1.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tekrsa_api_wrap-1.3.2/LICENSE.md` & `tekrsa_api_wrap-1.3.3/LICENSE.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,34 @@
-SOFTWARE DISCLAIMER / RELEASE
+# SOFTWARE DISCLAIMER / RELEASE
 
-This software was developed by employees of the National Telecommunications and Information Administration (NTIA), an agency of the Federal Government and is provided to you as a public service.  Pursuant to Title 15 United States Code Section 105, works of NTIA employees are not subject to copyright protection within the United States.
+This software was developed by employees of the National Telecommunications and Information
+Administration (NTIA), an agency of the Federal Government and is provided to you
+as a public service.  Pursuant to Title 15 United States Code Section 105, works
+of NTIA employees are not subject to copyright protection within the United States.
+
+The software is provided by NTIA “AS IS.”  NTIA MAKES NO WARRANTY OF ANY KIND, EXPRESS,
+IMPLIED OR STATUTORY, INCLUDING, WITHOUT LIMITATION, THE IMPLIED WARRANTY OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE, NON-INFRINGEMENT AND DATA ACCURACY. NTIA does
+not warrant or make any representations regarding the use of the software or the
+results thereof, including but not limited to the correctness, accuracy, reliability
+or usefulness of the software.
+
+To the extent that NTIA holds rights in countries other than the United States,
+you are hereby granted the non-exclusive irrevocable and unconditional right to
+print, publish, prepare derivative works and distribute the NTIA software, in any
+medium, or authorize others to do so on your behalf, on a royalty-free basis throughout
+the World.
+
+You may improve, modify, and create derivative works of the software or any portion
+of the software, and you may copy and distribute such modifications or works. Modified
+works should carry a notice stating that you changed the software and should note
+the date and nature of any such change.
+
+You are solely responsible for determining the appropriateness of using and distributing
+the software and you assume all risks associated with its use, including but not
+limited to the risks and costs of program errors, compliance with applicable laws,
+damage to or loss of data, programs or equipment, and the unavailability or interruption
+of operation. This software is not intended to be used in any situation where a failure
+could cause risk of injury or damage to property.
 
-The software is provided by NTIA “AS IS.”  NTIA MAKES NO WARRANTY OF ANY KIND, EXPRESS, IMPLIED OR STATUTORY, INCLUDING, WITHOUT LIMITATION, THE IMPLIED WARRANTY OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, NON-INFRINGEMENT AND DATA ACCURACY. NTIA does not warrant or make any representations regarding the use of the software or the results thereof, including but not limited to the correctness, accuracy, reliability or usefulness of the software.
-
-To the extent that NTIA holds rights in countries other than the United States, you are hereby granted the non-exclusive irrevocable and unconditional right to print, publish, prepare derivative works and distribute the NTIA software, in any medium, or authorize others to do so on your behalf, on a royalty-free basis throughout the World.
-
-You may improve, modify, and create derivative works of the software or any portion of the software, and you may copy and distribute such modifications or works. Modified works should carry a notice stating that you changed the software and should note the date and nature of any such change.
-
-You are solely responsible for determining the appropriateness of using and distributing the software and you assume all risks associated with its use, including but not limited to the risks and costs of program errors, compliance with applicable laws, damage to or loss of data, programs or equipment, and the unavailability or interruption of operation. This software is not intended to be used in any situation where a failure could cause risk of injury or damage to property.
-
-Please provide appropriate acknowledgments of NTIA’s creation of the software in any copies or derivative works of this software.
+Please provide appropriate acknowledgments of NTIA’s creation of the software in
+any copies or derivative works of this software.
```

### Comparing `tekrsa_api_wrap-1.3.2/README.md` & `tekrsa_api_wrap-1.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
 
 TEKTRONIX and TEK are registered trademarks of Tektronix, Inc.
 
 Microsoft and Windows are trademarks of the Microsoft group of companies.
 
 ## Contact
 
-For technical questions, contact Anthony Romaniello, aromaniello@ntia.gov
+For technical questions, contact Anthony Romaniello, <aromaniello@ntia.gov>
 
 ## Disclaimer
 
 Certain commercial equipment, instruments, or materials are identified in this project
 were used for the convenience of the developers. In no case does such identification
 imply recommendation or endorsement by the National Telecommunications and Information
 Administration, nor does it imply that the material or equipment identified is necessarily
```

### Comparing `tekrsa_api_wrap-1.3.2/pyproject.toml` & `tekrsa_api_wrap-1.3.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     "Natural Language :: English",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 
 dependencies = [
     "numpy>=1.22",
 ]
 
 [project.optional-dependencies]
```

### Comparing `tekrsa_api_wrap-1.3.2/PKG-INFO` & `tekrsa_api_wrap-1.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,66 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tekrsa-api-wrap
-Version: 1.3.2
+Version: 1.3.3
 Summary: NTIA/ITS Python wrapper for the Tektronix RSA API for Linux
 Project-URL: Repository, https://github.com/NTIA/tekrsa-api-wrap
 Project-URL: Bug Tracker, https://github.com/NTIA/tekrsa-api-wrap/issues
 Project-URL: NTIA GitHub, https://github.com/NTIA
 Project-URL: ITS Website, https://its.ntia.gov
 Project-URL: Tektronix Website, https://www.tek.com/en
 Author: The Institute for Telecommunication Sciences
 Maintainer-email: Anthony Romaniello <aromaniello@ntia.gov>
-License: SOFTWARE DISCLAIMER / RELEASE
+License: # SOFTWARE DISCLAIMER / RELEASE
         
-        This software was developed by employees of the National Telecommunications and Information Administration (NTIA), an agency of the Federal Government and is provided to you as a public service.  Pursuant to Title 15 United States Code Section 105, works of NTIA employees are not subject to copyright protection within the United States.
+        This software was developed by employees of the National Telecommunications and Information
+        Administration (NTIA), an agency of the Federal Government and is provided to you
+        as a public service.  Pursuant to Title 15 United States Code Section 105, works
+        of NTIA employees are not subject to copyright protection within the United States.
         
-        The software is provided by NTIA “AS IS.”  NTIA MAKES NO WARRANTY OF ANY KIND, EXPRESS, IMPLIED OR STATUTORY, INCLUDING, WITHOUT LIMITATION, THE IMPLIED WARRANTY OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, NON-INFRINGEMENT AND DATA ACCURACY. NTIA does not warrant or make any representations regarding the use of the software or the results thereof, including but not limited to the correctness, accuracy, reliability or usefulness of the software.
+        The software is provided by NTIA “AS IS.”  NTIA MAKES NO WARRANTY OF ANY KIND, EXPRESS,
+        IMPLIED OR STATUTORY, INCLUDING, WITHOUT LIMITATION, THE IMPLIED WARRANTY OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE, NON-INFRINGEMENT AND DATA ACCURACY. NTIA does
+        not warrant or make any representations regarding the use of the software or the
+        results thereof, including but not limited to the correctness, accuracy, reliability
+        or usefulness of the software.
         
-        To the extent that NTIA holds rights in countries other than the United States, you are hereby granted the non-exclusive irrevocable and unconditional right to print, publish, prepare derivative works and distribute the NTIA software, in any medium, or authorize others to do so on your behalf, on a royalty-free basis throughout the World.
+        To the extent that NTIA holds rights in countries other than the United States,
+        you are hereby granted the non-exclusive irrevocable and unconditional right to
+        print, publish, prepare derivative works and distribute the NTIA software, in any
+        medium, or authorize others to do so on your behalf, on a royalty-free basis throughout
+        the World.
         
-        You may improve, modify, and create derivative works of the software or any portion of the software, and you may copy and distribute such modifications or works. Modified works should carry a notice stating that you changed the software and should note the date and nature of any such change.
+        You may improve, modify, and create derivative works of the software or any portion
+        of the software, and you may copy and distribute such modifications or works. Modified
+        works should carry a notice stating that you changed the software and should note
+        the date and nature of any such change.
         
-        You are solely responsible for determining the appropriateness of using and distributing the software and you assume all risks associated with its use, including but not limited to the risks and costs of program errors, compliance with applicable laws, damage to or loss of data, programs or equipment, and the unavailability or interruption of operation. This software is not intended to be used in any situation where a failure could cause risk of injury or damage to property.
+        You are solely responsible for determining the appropriateness of using and distributing
+        the software and you assume all risks associated with its use, including but not
+        limited to the risks and costs of program errors, compliance with applicable laws,
+        damage to or loss of data, programs or equipment, and the unavailability or interruption
+        of operation. This software is not intended to be used in any situation where a failure
+        could cause risk of injury or damage to property.
         
-        Please provide appropriate acknowledgments of NTIA’s creation of the software in any copies or derivative works of this software.
+        Please provide appropriate acknowledgments of NTIA’s creation of the software in
+        any copies or derivative works of this software.
 License-File: LICENSE.md
 Keywords: API,Linux,RF,RSA,SCOS,SDR,Tektronix,analyzer,radio,spectrum,wrapper
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: numpy>=1.22
 Provides-Extra: dev
 Requires-Dist: hatchling<2.0,>=1.6.0; extra == 'dev'
 Requires-Dist: pre-commit>=2.20.0; extra == 'dev'
 Requires-Dist: twine<5.0,>=4.0.1; extra == 'dev'
 Description-Content-Type: text/markdown
@@ -242,15 +265,15 @@
 
 TEKTRONIX and TEK are registered trademarks of Tektronix, Inc.
 
 Microsoft and Windows are trademarks of the Microsoft group of companies.
 
 ## Contact
 
-For technical questions, contact Anthony Romaniello, aromaniello@ntia.gov
+For technical questions, contact Anthony Romaniello, <aromaniello@ntia.gov>
 
 ## Disclaimer
 
 Certain commercial equipment, instruments, or materials are identified in this project
 were used for the convenience of the developers. In no case does such identification
 imply recommendation or endorsement by the National Telecommunications and Information
 Administration, nor does it imply that the material or equipment identified is necessarily
```

