# Comparing `tmp/mhi-cosim-1.1.3.tar.gz` & `tmp/mhi_cosim-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mhi-cosim-1.1.3.tar", last modified: Thu Oct 26 19:42:49 2023, max compression
+gzip compressed data, was "mhi_cosim-1.2.0.tar", last modified: Tue Apr 30 18:20:06 2024, max compression
```

## Comparing `mhi-cosim-1.1.3.tar` & `mhi_cosim-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-10-26 19:42:49.274803 mhi-cosim-1.1.3/
--rw-rw-rw-   0        0        0     1731 2023-08-04 14:43:25.000000 mhi-cosim-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     1118 2023-10-26 19:42:49.274803 mhi-cosim-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-08-04 14:43:25.000000 mhi-cosim-1.1.3/README.rst
--rw-rw-rw-   0        0        0       42 2023-10-26 19:42:49.274803 mhi-cosim-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1899 2023-10-26 17:09:08.000000 mhi-cosim-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-26 19:42:49.231046 mhi-cosim-1.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-10-26 19:42:49.243054 mhi-cosim-1.1.3/src/ext/
-drwxrwxrwx   0        0        0        0 2023-10-26 19:42:49.243054 mhi-cosim-1.1.3/src/ext/EmtCoSim/
--rw-rw-rw-   0        0        0    85974 2023-08-04 14:43:25.000000 mhi-cosim-1.1.3/src/ext/EmtCoSim/EmtCoSim.c
--rw-rw-rw-   0        0        0    10092 2023-08-04 14:43:25.000000 mhi-cosim-1.1.3/src/ext/cosim.c
-drwxrwxrwx   0        0        0        0 2023-10-26 19:42:49.231046 mhi-cosim-1.1.3/src/mhi/
-drwxrwxrwx   0        0        0        0 2023-10-26 19:42:49.243054 mhi-cosim-1.1.3/src/mhi/cosim/
--rw-rw-rw-   0        0        0     7481 2023-10-26 19:39:32.000000 mhi-cosim-1.1.3/src/mhi/cosim/__init__.py
--rw-rw-rw-   0        0        0      186 2023-08-04 14:43:25.000000 mhi-cosim-1.1.3/src/mhi/cosim/__main__.py
-drwxrwxrwx   0        0        0        0 2023-10-26 19:42:49.271799 mhi-cosim-1.1.3/src/mhi_cosim.egg-info/
--rw-rw-rw-   0        0        0     1118 2023-10-26 19:42:48.000000 mhi-cosim-1.1.3/src/mhi_cosim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-10-26 19:42:49.000000 mhi-cosim-1.1.3/src/mhi_cosim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-26 19:42:48.000000 mhi-cosim-1.1.3/src/mhi_cosim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-10-26 19:42:48.000000 mhi-cosim-1.1.3/src/mhi_cosim.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-10-26 19:42:49.274803 mhi-cosim-1.1.3/tests/
--rw-rw-rw-   0        0        0     2000 2023-08-04 14:43:25.000000 mhi-cosim-1.1.3/tests/test_cosim_compliance.py
--rw-rw-rw-   0        0        0      856 2023-10-26 17:09:08.000000 mhi-cosim-1.1.3/tests/test_cosim_version.py
--rw-rw-rw-   0        0        0     1474 2023-08-04 14:43:25.000000 mhi-cosim-1.1.3/tests/test_help.py
+drwxrwxrwx   0        0        0        0 2024-04-30 18:20:06.323952 mhi_cosim-1.2.0/
+-rw-rw-rw-   0        0        0     1731 2024-04-30 16:57:44.000000 mhi_cosim-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1231 2024-04-30 18:20:06.323952 mhi_cosim-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-04-24 16:09:11.000000 mhi_cosim-1.2.0/README.rst
+-rw-rw-rw-   0        0        0       42 2024-04-30 18:20:06.323952 mhi_cosim-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     2575 2024-04-30 18:18:19.000000 mhi_cosim-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 18:20:06.267612 mhi_cosim-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-30 18:20:06.276620 mhi_cosim-1.2.0/src/ext/
+drwxrwxrwx   0        0        0        0 2024-04-30 18:20:06.276620 mhi_cosim-1.2.0/src/ext/EmtCoSim/
+-rw-rw-rw-   0        0        0    90908 2024-04-30 16:38:33.000000 mhi_cosim-1.2.0/src/ext/EmtCoSim/EmtCoSim.c
+-rw-rw-rw-   0        0        0    10092 2023-08-04 14:43:25.000000 mhi_cosim-1.2.0/src/ext/cosim.c
+drwxrwxrwx   0        0        0        0 2024-04-30 18:20:06.267612 mhi_cosim-1.2.0/src/mhi/
+drwxrwxrwx   0        0        0        0 2024-04-30 18:20:06.292256 mhi_cosim-1.2.0/src/mhi/cosim/
+-rw-rw-rw-   0        0        0     8675 2024-04-30 17:12:40.000000 mhi_cosim-1.2.0/src/mhi/cosim/__init__.py
+-rw-rw-rw-   0        0        0      975 2024-04-24 19:08:49.000000 mhi_cosim-1.2.0/src/mhi/cosim/__main__.py
+-rw-rw-rw-   0        0        0    28755 2024-04-30 18:18:43.000000 mhi_cosim-1.2.0/src/mhi/cosim/mhi-cosim.chm
+drwxrwxrwx   0        0        0        0 2024-04-30 18:20:06.323952 mhi_cosim-1.2.0/src/mhi_cosim.egg-info/
+-rw-rw-rw-   0        0        0     1231 2024-04-30 18:20:05.000000 mhi_cosim-1.2.0/src/mhi_cosim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2024-04-30 18:20:06.000000 mhi_cosim-1.2.0/src/mhi_cosim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 18:20:05.000000 mhi_cosim-1.2.0/src/mhi_cosim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-30 18:20:05.000000 mhi_cosim-1.2.0/src/mhi_cosim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 18:20:06.314448 mhi_cosim-1.2.0/tests/
+-rw-rw-rw-   0        0        0     2220 2024-04-24 16:09:11.000000 mhi_cosim-1.2.0/tests/test_cosim_compliance.py
+-rw-rw-rw-   0        0        0      856 2023-10-26 17:09:08.000000 mhi_cosim-1.2.0/tests/test_cosim_version.py
+-rw-rw-rw-   0        0        0     1474 2023-08-04 14:43:25.000000 mhi_cosim-1.2.0/tests/test_help.py
```

### Comparing `mhi-cosim-1.1.3/LICENSE` & `mhi_cosim-1.2.0/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The Clear BSD License
 
-Copyright 2021 Manitoba Hydro International Ltd.
+Copyright 2024 Manitoba Hydro International Ltd.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted (subject to the limitations in the disclaimer
 below) provided that the following conditions are met:
 
      * Redistributions of source code must retain the above copyright notice,
```

### Comparing `mhi-cosim-1.1.3/PKG-INFO` & `mhi_cosim-1.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mhi-cosim
-Version: 1.1.3
+Version: 1.2.0
 Summary: MHI Cosimulation Module
 Home-page: https://www.pscad.com/webhelp-v5-al/index.html
 Author: Manitoba Hydro International Ltd.
 Author-email: pscad@mhi.ca
 License: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -24,7 +24,13 @@
 
 ====================
 Cosimulation Library
 ====================
 
 The EMTDC Python Cosimulation Library is designed to allow control
 simulation of a portion of a power system from a Python script.
+
+=============
+Documentation
+=============
+
+Use `py -m mhi.cosim help` to access the module documentation.
```

### Comparing `mhi-cosim-1.1.3/setup.py` & `mhi_cosim-1.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,37 @@
 import re, codecs
 from setuptools import setup, Extension
 
 def get_version(version_file):
+    """
+    Construct the version string without using
+        from mhi.pscad import VERSION
+    since the import will fail if the module is not installed,
+    which it won't be since we are trying to build it. (Catch-22)
+    """
+
     with codecs.open(version_file, 'r') as fp:
         contents = fp.read()
-    match = re.search(r"^VERSION = '([^']+)'", contents, re.M)
-    if match:
-        return match.group(1)
-    raise RuntimeError("Unable to find version string")
+
+    match = re.search(r"^_VERSION = \((\d+), (\d+), (\d+)\)$", contents, re.M)
+    if match is None:
+        raise RuntimeError("Unable to find _VERSION")
+    version = ".".join(match.groups())
+
+    match = re.search(r"^_TYPE = '([abcf]\d)'$", contents, re.M)
+    if match is None:
+        raise RuntimeError("Unable to find _TYPE")
+    version_type = match.group(1).lower()
+
+    if version_type != 'f0':
+        if version_type[0] == 'f':
+            version_type = 'p' + version_type[1]
+        version += version_type
+
+    return version
 
 version = get_version(r'src/mhi/cosim/__init__.py')
 
 cosim = Extension('_cosim',
                   sources=['src/ext/cosim.c',
                            'src/ext/EmtCoSim/EmtCoSim.c',
                            ],
@@ -27,14 +47,15 @@
       description='MHI Cosimulation Module',
       long_description=long_description,
       long_description_content_type="text/x-rst",
       ext_modules=[cosim],
       ext_package='mhi.cosim',
       package_dir={'': 'src'},
       packages=['mhi.cosim'],
+      package_data={'mhi.cosim': ['*.chm']},
       requires=['wheel'],
       python_requires='>=3.6',
       author='Manitoba Hydro International Ltd.',
       author_email='pscad@mhi.ca',
       url='https://www.pscad.com/webhelp-v5-al/index.html',
       license="BSD License",
```

### Comparing `mhi-cosim-1.1.3/src/ext/EmtCoSim/EmtCoSim.c` & `mhi_cosim-1.2.0/src/ext/EmtCoSim/EmtCoSim.c`

 * *Files 26% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 #include "EmtCoSim.h"
 
 /* Dependencies */
 #include <Windows.h>          /* Used For System Calls                          */
 #include <stdint.h>           /* Used For accessing specific byte count values  */
 #include <assert.h>           /* Debugging asserts                              */
 #include <stdio.h>            /* Used for file reading                          */
+#include <float.h>            /* Used for max double                            */
 
 #ifndef POSIX
 #define strcmpi  _strcmpi           /* For POSIX Compatibility */
 #define strnicmp _strnicmp
 #endif
 
 /*==============================================================================*/
@@ -83,200 +84,205 @@
 /* Maintains the life of an arbitrary sized data buffer                         */
 /*==============================================================================*/
 
 struct EmtdcCosimulation_Buffer_S;
 typedef struct EmtdcCosimulation_Buffer_S Buffer;
 
 /*==============================================================================*/
+/* Initialization Data                                                          */
+/*------------------------------------------------------------------------------*/
+/* The data for initializing the co-simulation                                  */
+/*==============================================================================*/
+
+struct EmtdcCosimulation_InitData_S;
+typedef struct EmtdcCosimulation_InitData_S InitData;
+
+/*==============================================================================*/
 /* Singletons                                                                   */
 /*------------------------------------------------------------------------------*/
 /* These can, and should be only accessible to the local file.                  */
 /*==============================================================================*/
 
-HashTable *      pEmtdcCosimulation_ChannelManager = NULL;
-char             sEmtdcCosimulation_HostName[256];
-int              iEmtdcCosimulation_Port = -1;
-unsigned short   iEmtdcCosimulation_ClientId = 0;
+static HashTable *      pEmtdcCosimulation_ChannelManager = NULL;
+static char             sEmtdcCosimulation_HostName[256];
+static int              iEmtdcCosimulation_Port = -1;
+static unsigned short   iEmtdcCosimulation_ClientId = 0;
+static double           dEmtdcCosimulation_Time = 0.0;
+static double           dEmtdcCosimulation_Step = 0.0;
 
 /*==============================================================================*/
 /* EmtdcCosimulation_Channel                                                    */
 /*------------------------------------------------------------------------------*/
 /* The manager for a specific channel of information traveling between this     */
 /* Client and another client, the channel should be globally unique across the  */
 /* entire system                                                                */
 /*==============================================================================*/
 
 /*===================================================================*/
 /* Constructor / Destructor                                          */
 /*===================================================================*/
-EmtdcCosimulation_Channel * EmtdcCosimulation_Channel_Create(unsigned short client_id, unsigned int channel_id, int recv_size, int send_size);
-void           EmtdcCosimulation_Channel_Delete(EmtdcCosimulation_Channel* _this);
+static EmtdcCosimulation_Channel * EmtdcCosimulation_Channel_Create(unsigned short client_id, unsigned int channel_id, int recv_size, int send_size);
+static void           EmtdcCosimulation_Channel_Delete(EmtdcCosimulation_Channel* _this);
 
 /*-------------------------------------------------------------------*/
 /* Member Functions                                                  */
 /*-------------------------------------------------------------------*/
-double       EmtdcCosimulation_Channel_GetValue        (EmtdcCosimulation_Channel* _this, double time, int index);
-void         EmtdcCosimulation_Channel_SetValue        (EmtdcCosimulation_Channel* _this, double val, int index);
-void         EmtdcCosimulation_Channel_Send            (EmtdcCosimulation_Channel* _this, double time);
-unsigned int EmtdcCosimulation_Channel_GetChannelId    (EmtdcCosimulation_Channel* _this);
-int          EmtdcCosimulation_Channel_GetSendSize     (EmtdcCosimulation_Channel* _this);
-int          EmtdcCosimulation_Channel_GetRecvSize     (EmtdcCosimulation_Channel* _this);
+static double       EmtdcCosimulation_Channel_GetValue        (EmtdcCosimulation_Channel* _this, double time, int index);
+static void         EmtdcCosimulation_Channel_SetValue        (EmtdcCosimulation_Channel* _this, double val, int index);
+static void         EmtdcCosimulation_Channel_Send            (EmtdcCosimulation_Channel* _this, double time);
+static unsigned int EmtdcCosimulation_Channel_GetChannelId    (EmtdcCosimulation_Channel* _this);
+static int          EmtdcCosimulation_Channel_GetSendSize     (EmtdcCosimulation_Channel* _this);
+static int          EmtdcCosimulation_Channel_GetRecvSize     (EmtdcCosimulation_Channel* _this);
 
 /*==============================================================================*/
 /* ChannelImpl                                                                  */
 /*------------------------------------------------------------------------------*/
 /* This is the internal representation of the Channel, The                      */
 /* EmtdcCosimulation_Channel is a thin wrapper for this structure               */
 /*==============================================================================*/
 
 /*-------------------------------------------------------------------*/
 /* Shared Members                                                    */
 /*-------------------------------------------------------------------*/
-Buffer *     pEmtdcCosimulation_Channel_Impl_Buffer = NULL;
-int          iEmtdcCosimulation_Channel_Impl_Master = 0;
+static Buffer *     pEmtdcCosimulation_Channel_Impl_Buffer = NULL;
+static int          iEmtdcCosimulation_Channel_Impl_Master = 0;
 
 /*-------------------------------------------------------------------*/
 /* Shared Functions                                                  */
 /*-------------------------------------------------------------------*/
-unsigned int   EmtdcCosimulation_Channel_Impl_GetNextChannelMessage(unsigned short client_id);
+static unsigned int   EmtdcCosimulation_Channel_Impl_GetNextChannelMessage(unsigned short client_id);
 
 /*===================================================================*/
 /* Constructor / Destructor                                          */
 /*===================================================================*/
-ChannelImpl * EmtdcCosimulation_Channel_Impl_Create(unsigned short client_id, unsigned int channel_id, int recv_size, int send_size);
-void          EmtdcCosimulation_Channel_Impl_Delete(ChannelImpl* _this);
+static ChannelImpl * EmtdcCosimulation_Channel_Impl_Create(unsigned short client_id, unsigned int channel_id, int recv_size, int send_size);
+static void          EmtdcCosimulation_Channel_Impl_Delete(ChannelImpl* _this);
 
 /*-------------------------------------------------------------------*/
 /* Member Functions                                                  */
 /*-------------------------------------------------------------------*/
-double         EmtdcCosimulation_Channel_Impl_GetValue        (ChannelImpl* _this, double time, int i);
-void           EmtdcCosimulation_Channel_Impl_SetValue        (ChannelImpl* _this, double d, int i);
-void           EmtdcCosimulation_Channel_Impl_Send            (ChannelImpl* _this, double time);
-void           EmtdcCosimulation_Channel_Impl_Parse           (ChannelImpl* _this, void * ptr, int size);
-char *         EmtdcCosimulation_Channel_Impl_SetValueBufferI (ChannelImpl* _this, char* ptr, unsigned int val);
-char *         EmtdcCosimulation_Channel_Impl_SetValueBufferD (ChannelImpl* _this, char* ptr, double val);
+static double         EmtdcCosimulation_Channel_Impl_GetValue        (ChannelImpl* _this, double time, int i);
+static void           EmtdcCosimulation_Channel_Impl_SetValue        (ChannelImpl* _this, double d, int i);
+static void           EmtdcCosimulation_Channel_Impl_Send            (ChannelImpl* _this, double time);
+static void           EmtdcCosimulation_Channel_Impl_Parse           (ChannelImpl* _this, void * ptr, int size);
+static char *         EmtdcCosimulation_Channel_Impl_SetValueBufferI (ChannelImpl* _this, char* ptr, unsigned int val);
+static char *         EmtdcCosimulation_Channel_Impl_SetValueBufferD (ChannelImpl* _this, char* ptr, double val);
+static void           EmtdcCosimulation_Channel_Impl_Send_Final      (ChannelImpl* _this);
 
 /*-------------------------------------------------------------------*/
 /* Structure                                                         */
 /*-------------------------------------------------------------------*/
 struct EmtdcCosimulation_Channel_Impl_S
    {
    unsigned short    iClientId;           /* The Client ID of the foreign Client that this channel is connected to */
    unsigned int      iChannelId;          /* A System wide unique value used to identify this information channel  */
    int               iRecvSize;           /* The size of the data being received                                   */
    int               iSendSize;           /* The size of the data being sent                                       */
    unsigned short    iMessageSize;        /* A cache of the complete message size                                  */
 
+   Message *         pLastMessage;
    Message *         pSendMessage;        /* The message being constructed to send                                 */
    Message *         pRecvMessage;        /* The currently received message (list)                                 */
    Message *         pRecvMessageBuffer;  /* A backlog, of allocated messages that can be overwritten              */
-
-   /* Functions */
-   double   (*GetValue)        (ChannelImpl* _this, double time, int i);
-   void     (*SetValue)        (ChannelImpl* _this, double d, int i);
-   void     (*Send)            (ChannelImpl* _this, double time);
-   void     (*Parse)           (ChannelImpl* _this, void * ptr, int size);
-   char*    (*SetValueBufferI) (ChannelImpl* _this, char* ptr, unsigned int val);
-   char*    (*SetValueBufferD) (ChannelImpl* _this, char* ptr, double val);  
    };
 
 /*==============================================================================*/
 /* Primitive Marshalling                                                        */
 /*------------------------------------------------------------------------------*/
 /* The following function are created to perform Bit-wise Marshalling           */
 /* on primitive types to pass information quickly and robustly over             */
 /* an unknown connection                                                        */
 /*==============================================================================*/
 
 /*-------------------------------------------------------------------*/
 /* EmtdcCosimulation_Marshal_int32()                                 */
 /*-------------------------------------------------------------------*/
-int32_t  EmtdcCosimulation_Marshal_int32  (int32_t value)
+static int32_t  EmtdcCosimulation_Marshal_int32  (int32_t value)
    {
    unsigned char bytes[sizeof(int32_t)];
    int i;
    for(i=0; i<sizeof(int32_t); i++)
       bytes[i]=(unsigned char)(value>>(8*(sizeof(int32_t)-i-1)));
    return *((int32_t*)bytes);
    }
 
 /*-------------------------------------------------------------------*/
 /* EmtdcCosimulation_Marshal_int64()                                 */
 /*-------------------------------------------------------------------*/
-int64_t  EmtdcCosimulation_Marshal_int64  (int64_t value)
+static int64_t  EmtdcCosimulation_Marshal_int64  (int64_t value)
    {
    unsigned char bytes[sizeof(int64_t)];
    int i;
    for(i=0; i<sizeof(int64_t); i++)
       bytes[i]=(unsigned char)(value>>(8*(sizeof(int64_t)-i-1)));
    return *((int64_t*)bytes);
    }
 
 /*-------------------------------------------------------------------*/
 /* EmtdcCosimulation_Marshal_double()                                */
 /*-------------------------------------------------------------------*/
-double EmtdcCosimulation_Marshal_double(double value)
+static double EmtdcCosimulation_Marshal_double(double value)
    {
-   uint64_t a;  
+   uint64_t a;
    a = EmtdcCosimulation_Marshal_int64(*((uint64_t*)(&value)));
    return *((double*)(&a));
    }
 
 /*-------------------------------------------------------------------*/
 /* EmtdcCosimulation_Extract_int32()                                 */
 /*-------------------------------------------------------------------*/
-void * EmtdcCosimulation_Extract_int32(void * ptr, uint32_t * value)
+static void * EmtdcCosimulation_Extract_int32(void * ptr, uint32_t * value)
    {
    (*value) = EmtdcCosimulation_Marshal_int32(*(uint32_t*)(ptr));
    return (char*)ptr + sizeof(uint32_t);
    }
 
 /*-------------------------------------------------------------------*/
 /* EmtdcCosimulation_Extract_double()                                */
 /*-------------------------------------------------------------------*/
-void * EmtdcCosimulation_Extract_double(void * ptr, double  * value)
+static void * EmtdcCosimulation_Extract_double(void * ptr, double  * value)
    {
    (*value) = EmtdcCosimulation_Marshal_double(*(double*)(ptr));
    return (char*)ptr + sizeof(double);
    }
 
 /*-------------------------------------------------------------------*/
 /* EmtdcCosimulation_Insert_Int32()                                  */
 /*-------------------------------------------------------------------*/
-void * EmtdcCosimulation_Insert_int32(void * ptr, int32_t value)
+static void * EmtdcCosimulation_Insert_int32(void * ptr, int32_t value)
    {
    *((int32_t*)(ptr)) = EmtdcCosimulation_Marshal_int32(value);
    return (char*)ptr + sizeof(int32_t);
    }
 
 /*-------------------------------------------------------------------*/
 /* EmtdcCosimulation_Insert_String()                                 */
 /*-------------------------------------------------------------------*/
-void * EmtdcCosimulation_Insert_string(void * ptr, char * value)
+static void * EmtdcCosimulation_Insert_string(void * ptr, char * value)
    {
    int len;
    len = (int)strlen(value);
    memcpy(ptr, value, len + 1);
    return (char*)ptr + len + 1;
    }
 
 /*-------------------------------------------------------------------*/
 /* EmtdcCosimulation_string_trim()                                   */
 /*-------------------------------------------------------------------*/
-char* EmtdcCosimulation_string_trim(char * str)
+static char* EmtdcCosimulation_string_trim(char * str)
    {
    char *end;
 
    /* Trim leading space  */
    /**/
    while (isspace(*str))
       str++;
 
    /* If empty string */
-   if (*str == 0)  
+   if (*str == 0)
       return str;
 
    /* Trim trailing space */
    /**/
    end = str + strlen(str) - 1;
    while (end > str && isspace(*end))
       end--;
@@ -301,78 +307,77 @@
 /*-------------------------------------------------------------------*/
 typedef int (_cdecl * CommunicationFabric_Init_Func)(int argc, char * args[]);
 typedef int (_cdecl * CommunicationFabric_Com_Func)(unsigned short to, void * buffer, unsigned short size, unsigned short flag);
 
 /*-------------------------------------------------------------------*/
 /* Variables                                                         */
 /*-------------------------------------------------------------------*/
-HMODULE hComFabLibrary = NULL;         /* Handle to Library */
-
-CommunicationFabric_Init_Func   _CommunicationFabric_Initialize   = NULL;  /* Function Pointer to the Communication Fabric Initialize  function */
-CommunicationFabric_Init_Func   _CommunicationFabric_Finalize     = NULL;  /* Function Pointer to the Communication Fabric Finalize    function */
-CommunicationFabric_Com_Func    _CommunicationFabric_Send_Client  = NULL;  /* Function Pointer to the Communication Fabric send_client function */
-CommunicationFabric_Com_Func    _CommunicationFabric_Recv_Client  = NULL;  /* Function Pointer to the Communication Fabric recv_client function */
-CommunicationFabric_Com_Func    _CommunicationFabric_Peek_Client  = NULL;  /* Function Pointer to the Communication Fabric peek_client function */
-CommunicationFabric_Com_Func    _CommunicationFabric_Send_Server  = NULL;  /* Function Pointer to the Communication Fabric send_server function */
-CommunicationFabric_Com_Func    _CommunicationFabric_Recv_Server  = NULL;  /* Function Pointer to the Communication Fabric recv_server function */
-CommunicationFabric_Com_Func    _CommunicationFabric_Peek_Server  = NULL;  /* Function Pointer to the Communication Fabric peek_server function */
+static HMODULE hComFabLibrary = NULL;         /* Handle to Library */
+static CommunicationFabric_Init_Func   _CommunicationFabric_Initialize   = NULL;  /* Function Pointer to the Communication Fabric Initialize  function */
+static CommunicationFabric_Init_Func   _CommunicationFabric_Finalize     = NULL;  /* Function Pointer to the Communication Fabric Finalize    function */
+static CommunicationFabric_Com_Func    _CommunicationFabric_Send_Client  = NULL;  /* Function Pointer to the Communication Fabric send_client function */
+static CommunicationFabric_Com_Func    _CommunicationFabric_Recv_Client  = NULL;  /* Function Pointer to the Communication Fabric recv_client function */
+static CommunicationFabric_Com_Func    _CommunicationFabric_Peek_Client  = NULL;  /* Function Pointer to the Communication Fabric peek_client function */
+static CommunicationFabric_Com_Func    _CommunicationFabric_Send_Server  = NULL;  /* Function Pointer to the Communication Fabric send_server function */
+static CommunicationFabric_Com_Func    _CommunicationFabric_Recv_Server  = NULL;  /* Function Pointer to the Communication Fabric recv_server function */
+static CommunicationFabric_Com_Func    _CommunicationFabric_Peek_Server  = NULL;  /* Function Pointer to the Communication Fabric peek_server function */
 
 /*-------------------------------------------------------------------*/
 /* Functions                                                         */
 /*-------------------------------------------------------------------*/
 
 /* Loads the Communication Fabric and finds the required Function pointers */
-int CommunicationFabric_Load(const char * location);
-int CommunicationFabric_Unload();
+static int CommunicationFabric_Load(const char * location);
+static int CommunicationFabric_Unload();
 
 /* Call into the Communication Fabric */
-int CommunicationFabric_Initialize(int argc, char * args[]);
-int CommunicationFabric_Finalize(int argc, char * args[]);
-int CommunicationFabric_Send_Client(unsigned short to, void * buffer, unsigned short size, unsigned short flag);
-int CommunicationFabric_Recv_Client(unsigned short to, void * buffer, unsigned short size, unsigned short flag);
-int CommunicationFabric_Peek_Client(unsigned short to, void * buffer, unsigned short size, unsigned short flag);
-int CommunicationFabric_Send_Server(unsigned short to, void * buffer, unsigned short size, unsigned short flag);
-int CommunicationFabric_Recv_Server(unsigned short to, void * buffer, unsigned short size, unsigned short flag);
-int CommunicationFabric_Peek_Server(unsigned short to, void * buffer, unsigned short size, unsigned short flag);
+static int CommunicationFabric_Initialize(int argc, char * args[]);
+static int CommunicationFabric_Finalize(int argc, char * args[]);
+static int CommunicationFabric_Send_Client(unsigned short to, void * buffer, unsigned short size, unsigned short flag);
+static int CommunicationFabric_Recv_Client(unsigned short to, void * buffer, unsigned short size, unsigned short flag);
+static int CommunicationFabric_Peek_Client(unsigned short to, void * buffer, unsigned short size, unsigned short flag);
+static int CommunicationFabric_Send_Server(unsigned short to, void * buffer, unsigned short size, unsigned short flag);
+static int CommunicationFabric_Recv_Server(unsigned short to, void * buffer, unsigned short size, unsigned short flag);
+static int CommunicationFabric_Peek_Server(unsigned short to, void * buffer, unsigned short size, unsigned short flag);
 
 /*==============================================================================*/
 /* HashTable                                                                    */
 /*------------------------------------------------------------------------------*/
 /* This is a fast hash-table used to quickly retrieve objects by a hash         */
 /* identifier                                                                   */
 /*==============================================================================*/
 
 /*-------------------------------------------------------------------*/
 /* Constants                                                         */
 /*-------------------------------------------------------------------*/
 
-const int  iEmtdcCosimulation_HashTable_StartSize        = 32;
-const int  iEmtdcCosimulation_HashTable_StartCapacity    = 16;
-const int  iEmtdcCosimulation_HashTable_HashMulti        = 7;
-const int  iEmtdcCosimulation_HashTable_EmptyDivisor     = 4;
-const int  iEmtdcCosimulation_HashTable_EmptyMin         = 10;
+static const int  iEmtdcCosimulation_HashTable_StartSize        = 32;
+static const int  iEmtdcCosimulation_HashTable_StartCapacity    = 16;
+static const int  iEmtdcCosimulation_HashTable_HashMulti        = 7;
+static const int  iEmtdcCosimulation_HashTable_EmptyDivisor     = 4;
+static const int  iEmtdcCosimulation_HashTable_EmptyMin         = 10;
 
 /*===================================================================*/
 /* Constructor / Destructor                                          */
 /*===================================================================*/
-HashTable * EmtdcCosimulation_HashTable_Create(double fill_cap);
-void EmtdcCosimulation_HashTable_Delete(HashTable * _this);
+static HashTable * EmtdcCosimulation_HashTable_Create(double fill_cap);
+static void EmtdcCosimulation_HashTable_Delete(HashTable * _this);
 
 /*-------------------------------------------------------------------*/
 /* Member Functions                                                  */
 /*-------------------------------------------------------------------*/
-void*  EmtdcCosimulation_HashTable_Fetch(HashTable * _this, int key);
-int    EmtdcCosimulation_HashTable_Append(HashTable * _this, void* object, int key);
-int    EmtdcCosimulation_HashTable_Remove(HashTable * _this, int key);
-int    EmtdcCosimulation_HashTable_GetCount(HashTable * _this);
-int    EmtdcCosimulation_HashTable_GetKey(HashTable * _this, int index) ;
-void*  EmtdcCosimulation_HashTable_Get(HashTable * _this, int index);
-void   EmtdcCosimulation_HashTable_EnsureCapacity(HashTable * _this, int size);
-int    EmtdcCosimulation_HashTable_Hash(HashTable * _this, int val, int is_new, HashTableEntry* entries, int size);
-void   EmtdcCosimulation_HashTable_Rebuild(HashTable * _this, int capacity);
+static void*  EmtdcCosimulation_HashTable_Fetch(HashTable * _this, int key);
+static int    EmtdcCosimulation_HashTable_Append(HashTable * _this, void* object, int key);
+static int    EmtdcCosimulation_HashTable_Remove(HashTable * _this, int key);
+static int    EmtdcCosimulation_HashTable_GetCount(HashTable * _this);
+static int    EmtdcCosimulation_HashTable_GetKey(HashTable * _this, int index) ;
+static void*  EmtdcCosimulation_HashTable_Get(HashTable * _this, int index);
+static void   EmtdcCosimulation_HashTable_EnsureCapacity(HashTable * _this, int size);
+static int    EmtdcCosimulation_HashTable_Hash(HashTable * _this, int val, int is_new, HashTableEntry* entries, int size);
+static void   EmtdcCosimulation_HashTable_Rebuild(HashTable * _this, int capacity);
 
 /*-------------------------------------------------------------------*/
 /* Sub Structure                                                     */
 /*-------------------------------------------------------------------*/
 struct EmtdcCosimulation_HashTable_Entry_S
    {
    int iKey;
@@ -388,41 +393,30 @@
    HashTableObject*     aObjects;      /* List of Pointers to the stored objects                  */
    int                  iCapacity;     /* The Capacity of the Key and Object lists                */
    int                  iCount;        /* The count of the objects (and keys) that fill the list  */
    HashTableEntry*      aHash;         /* Hash Entries                                            */
    int                  iHashSize;     /* Size of Hash Entries                                    */
    double               dFull;         /* Fill Size                                               */
    int                  iRemoveCount;  /* Removed Count                                           */
-
-   /* Functions */
-   void* (*Fetch)          (HashTable * _this, int key);
-   int   (*Append)         (HashTable * _this, void* object, int key);
-   int   (*Remove)         (HashTable * _this, int key);
-   int   (*GetCount)       (HashTable * _this);
-   int   (*GetKey)         (HashTable * _this, int index) ;
-   void* (*Get)            (HashTable * _this, int index);
-   void  (*EnsureCapacity) (HashTable * _this, int size);
-   int   (*Hash)           (HashTable * _this, int val, int is_new, HashTableEntry* entries, int size);
-   void  (*Rebuild)        (HashTable * _this, int capacity);      
    };
 
 /*==============================================================================*/
 /* Message                                                                      */
 /*------------------------------------------------------------------------------*/
 /* Maintains the information sent in a single transmission of co-simulation.    */
 /* the valid-time and values are stored and can be queries                      */
 /*                                                                              */
 /* This is a node in a linked list of received messages                         */
 /*==============================================================================*/
 
 /*===================================================================*/
 /* Constructor / Destructor                                          */
 /*===================================================================*/
-Message * EmtdcCosimulation_Message_Create(int size);
-void EmtdcCosimulation_Message_Delete(Message * _this);
+static Message * EmtdcCosimulation_Message_Create(int size);
+static void EmtdcCosimulation_Message_Delete(Message * _this);
 
 /*-------------------------------------------------------------------*/
 /* Structure                                                         */
 /*-------------------------------------------------------------------*/
 struct  EmtdcCosimulation_Message_S
    {
    double         dValidTime;    /* The time that this message is valid until */
@@ -435,21 +429,21 @@
 /*------------------------------------------------------------------------------*/
 /* Maintains the life of an arbitrary sized data buffer                         */
 /*==============================================================================*/
 
 /*===================================================================*/
 /* Constructor / Destructor                                          */
 /*===================================================================*/
-Buffer* EmtdcCosimulation_Buffer_Create();
-void  EmtdcCosimulation_Buffer_Delete(Buffer *_this);
+static Buffer* EmtdcCosimulation_Buffer_Create();
+static void  EmtdcCosimulation_Buffer_Delete(Buffer *_this);
 
 /*-------------------------------------------------------------------*/
 /* Member Functions                                                  */
 /*-------------------------------------------------------------------*/
-void * EmtdcCosimulation_Buffer_GetBuffer(Buffer * _this, int size);
+static void * EmtdcCosimulation_Buffer_GetBuffer(Buffer * _this, int size);
 
 /*-------------------------------------------------------------------*/
 /* Structure                                                         */
 /*-------------------------------------------------------------------*/
 struct EmtdcCosimulation_Buffer_S
    {
    int iSize;
@@ -464,109 +458,109 @@
 /* Client and another client, the channel should be globally unique across the                                 */
 /* entire system                                                                                               */
 /*=============================================================================================================*/
 
 /*=============================================================================================================*/
 /* Constructor                                                                                                 */
 /*=============================================================================================================*/
-EmtdcCosimulation_Channel * EmtdcCosimulation_Channel_Create(unsigned short client_id, unsigned int channel_id, int recv_size, int send_size)
+static EmtdcCosimulation_Channel * EmtdcCosimulation_Channel_Create(unsigned short client_id, unsigned int channel_id, int recv_size, int send_size)
    {
    EmtdcCosimulation_Channel * _this;
-   
+
    _this = malloc(sizeof(EmtdcCosimulation_Channel));
    _this->pReserved = EmtdcCosimulation_Channel_Impl_Create(client_id, channel_id, recv_size, send_size);
    _this->GetValue = &EmtdcCosimulation_Channel_GetValue;
    _this->SetValue = &EmtdcCosimulation_Channel_SetValue;
    _this->Send = &EmtdcCosimulation_Channel_Send;
    _this->GetChannelId = &EmtdcCosimulation_Channel_GetChannelId;
    _this->GetSendSize = &EmtdcCosimulation_Channel_GetSendSize;
    _this->GetRecvSize = &EmtdcCosimulation_Channel_GetRecvSize;
    return _this;
    }
 
 /*=============================================================================================================*/
 /* Destructor                                                                                                  */
 /*=============================================================================================================*/
-void           EmtdcCosimulation_Channel_Delete(EmtdcCosimulation_Channel* _this)
+static void EmtdcCosimulation_Channel_Delete(EmtdcCosimulation_Channel* _this)
    {
    if (_this == NULL)
       return;
 
    EmtdcCosimulation_Channel_Impl_Delete((ChannelImpl*)_this->pReserved);
    free(_this);
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_Channel_GetValue()                                                                        */
 /*-------------------------------------------------------------------------------------------------------------*/
-double       EmtdcCosimulation_Channel_GetValue(EmtdcCosimulation_Channel* _this, double time, int index)
+static double EmtdcCosimulation_Channel_GetValue(EmtdcCosimulation_Channel* _this, double time, int index)
    {
    ChannelImpl * impl;
 
    impl = (ChannelImpl*)_this->pReserved;
-   return impl->GetValue(impl, time, index);
+   return EmtdcCosimulation_Channel_Impl_GetValue(impl, time, index);
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_Channel_SetValue()                                                                        */
 /*-------------------------------------------------------------------------------------------------------------*/
-void         EmtdcCosimulation_Channel_SetValue        (EmtdcCosimulation_Channel* _this, double val, int index)
+static void EmtdcCosimulation_Channel_SetValue        (EmtdcCosimulation_Channel* _this, double val, int index)
    {
    ChannelImpl * impl;
 
    impl = (ChannelImpl*)_this->pReserved;
-   impl->SetValue(impl, val, index);
+   EmtdcCosimulation_Channel_Impl_SetValue(impl, val, index);
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_Channel_Send()                                                                            */
 /*-------------------------------------------------------------------------------------------------------------*/
-void         EmtdcCosimulation_Channel_Send(EmtdcCosimulation_Channel* _this, double time)
+static void EmtdcCosimulation_Channel_Send(EmtdcCosimulation_Channel* _this, double time)
    {
    ChannelImpl * impl;
 
    impl = (ChannelImpl*)_this->pReserved;
-   impl->Send(impl, time);
+   EmtdcCosimulation_Channel_Impl_Send(impl, time);
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_Channel_GetChannelId()                                                                    */
 /*-------------------------------------------------------------------------------------------------------------*/
-unsigned int EmtdcCosimulation_Channel_GetChannelId(EmtdcCosimulation_Channel* _this)
+static unsigned int EmtdcCosimulation_Channel_GetChannelId(EmtdcCosimulation_Channel* _this)
    {
    ChannelImpl * impl;
-   
+
    impl = (ChannelImpl*)_this->pReserved;
    return impl->iChannelId;
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_Channel_GetSendSize()                                                                     */
 /*-------------------------------------------------------------------------------------------------------------*/
-int          EmtdcCosimulation_Channel_GetSendSize(EmtdcCosimulation_Channel* _this)
+static int EmtdcCosimulation_Channel_GetSendSize(EmtdcCosimulation_Channel* _this)
    {
    ChannelImpl * impl;
-   
+
    impl = (ChannelImpl*)_this->pReserved;
    return impl->iSendSize;
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_Channel_GetRecvSize()                                                                     */
 /*-------------------------------------------------------------------------------------------------------------*/
-int          EmtdcCosimulation_Channel_GetRecvSize(EmtdcCosimulation_Channel* _this)
+static int EmtdcCosimulation_Channel_GetRecvSize(EmtdcCosimulation_Channel* _this)
    {
    ChannelImpl * impl = (ChannelImpl*)_this->pReserved;
    return impl->iRecvSize;
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_Channel_Impl_GetNextChannelMessage()                                                      */
 /*-------------------------------------------------------------------------------------------------------------*/
-unsigned int   EmtdcCosimulation_Channel_Impl_GetNextChannelMessage(unsigned short client_id)
+static unsigned int EmtdcCosimulation_Channel_Impl_GetNextChannelMessage(unsigned short client_id)
    {
    int size;
    void * buffer;
    int channel_id;
    EmtdcCosimulation_Channel * ch;
 
    /* Wait for the next message from the client */
@@ -581,32 +575,32 @@
          {
          /* Extract the channel ID the message is intended for. */
          /**/
          EmtdcCosimulation_Extract_int32(buffer, &channel_id);
 
          /* Multiplex the message to the correct channel and parse the message for processing */
          /**/
-         ch = (EmtdcCosimulation_Channel*)pEmtdcCosimulation_ChannelManager->Fetch(pEmtdcCosimulation_ChannelManager, channel_id);
+         ch = (EmtdcCosimulation_Channel*)EmtdcCosimulation_HashTable_Fetch(pEmtdcCosimulation_ChannelManager, channel_id);
          if (ch != NULL)
-            ((ChannelImpl *)ch->pReserved)->Parse(((ChannelImpl *)ch->pReserved), buffer, size);
+            EmtdcCosimulation_Channel_Impl_Parse(((ChannelImpl *)ch->pReserved), buffer, size);
          return channel_id;
          }
       }
 
    /* No Data Received.                                                       */
    /* This should be impossible as both a blocking Peek and Receive are used  */
    /**/
-   assert(0); 
+   assert(0);
    return -1;
    }
 
 /*=============================================================================================================*/
 /* Constructor                                                                                                 */
 /*=============================================================================================================*/
-ChannelImpl * EmtdcCosimulation_Channel_Impl_Create(unsigned short client_id, unsigned int channel_id, int recv_size, int send_size)
+static ChannelImpl * EmtdcCosimulation_Channel_Impl_Create(unsigned short client_id, unsigned int channel_id, int recv_size, int send_size)
    {
    ChannelImpl * _this;
 
    /* Allocate memory */
    /**/
    _this = (ChannelImpl*)malloc(sizeof(ChannelImpl));
 
@@ -614,52 +608,47 @@
    /**/
    _this->iClientId = client_id;
    _this->iChannelId = channel_id;
    _this->iRecvSize = recv_size;
    _this->iSendSize = send_size;
    _this->pRecvMessageBuffer = EmtdcCosimulation_Message_Create(recv_size);
    _this->pSendMessage = EmtdcCosimulation_Message_Create(send_size);
+   _this->pLastMessage = EmtdcCosimulation_Message_Create(send_size);
    _this->pRecvMessage = NULL;
    _this->iMessageSize = (unsigned short)(sizeof(int) + sizeof(double) + sizeof(double)*send_size);
 
-   /* Set the function of the structure */
-   /**/
-   _this->GetValue          = &EmtdcCosimulation_Channel_Impl_GetValue;
-   _this->SetValue          = &EmtdcCosimulation_Channel_Impl_SetValue;
-   _this->Send              = &EmtdcCosimulation_Channel_Impl_Send;
-   _this->Parse             = &EmtdcCosimulation_Channel_Impl_Parse;
-   _this->SetValueBufferI   = &EmtdcCosimulation_Channel_Impl_SetValueBufferI;
-   _this->SetValueBufferD   = &EmtdcCosimulation_Channel_Impl_SetValueBufferD;
-
    /* Increment the counter of the number of structure in existence. */
    /* if this is the first allocation, allocate a shared buffer for  */
    /* all channels to use when sending or receiving                  */
    /**/
    if (iEmtdcCosimulation_Channel_Impl_Master == 0)
       pEmtdcCosimulation_Channel_Impl_Buffer = EmtdcCosimulation_Buffer_Create();
    iEmtdcCosimulation_Channel_Impl_Master++;
 
    return _this;
    }
 
 /*=============================================================================================================*/
 /* Destructor                                                                                                  */
 /*=============================================================================================================*/
-void           EmtdcCosimulation_Channel_Impl_Delete(ChannelImpl* _this)
+static void EmtdcCosimulation_Channel_Impl_Delete(ChannelImpl* _this)
    {
    /* Ensure that the parameter is not null */
    /**/
    if (_this == NULL)
       return;
-   
+
    /* Deallocate the cached messages */
    /**/
    if (_this->pSendMessage != NULL)
       EmtdcCosimulation_Message_Delete(_this->pSendMessage);
 
+   if (_this->pLastMessage != NULL)
+      EmtdcCosimulation_Message_Delete(_this->pLastMessage);
+
    if (_this->pRecvMessage != NULL)
       EmtdcCosimulation_Message_Delete(_this->pRecvMessage);
 
    if (_this->pRecvMessage != NULL)
       EmtdcCosimulation_Message_Delete(_this->pRecvMessageBuffer);
 
    /* decrement the counter for the number of structures in existence.   */
@@ -675,15 +664,15 @@
    /**/
    free(_this);
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_Channel_Impl_GetValue()                                                                   */
 /*-------------------------------------------------------------------------------------------------------------*/
-double         EmtdcCosimulation_Channel_Impl_GetValue(ChannelImpl* _this, double time, int i)
+static double EmtdcCosimulation_Channel_Impl_GetValue(ChannelImpl* _this, double time, int i)
    {
    Message * prev_msg;
    Message * recv_msg;
 
    if ( i >= _this->iRecvSize )
       return 0.0; /* Bad data */
 
@@ -717,64 +706,65 @@
       /* Retrieve messages until we get the time we are looking for */
       /**/
       while (EmtdcCosimulation_Channel_Impl_GetNextChannelMessage(_this->iClientId) != _this->iChannelId);
       }
 
    /* should not have been able to get here; */
    /**/
-   return 0.0;  
+   return 0.0;
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_Channel_Impl_SetValue()                                                                   */
 /*-------------------------------------------------------------------------------------------------------------*/
-void           EmtdcCosimulation_Channel_Impl_SetValue(ChannelImpl* _this, double d, int i)
+static void EmtdcCosimulation_Channel_Impl_SetValue(ChannelImpl* _this, double d, int i)
    {
    if ( i < _this->iSendSize )
       _this->pSendMessage->pData[i] = d;
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_Channel_Impl_Send()                                                                       */
 /*-------------------------------------------------------------------------------------------------------------*/
-void           EmtdcCosimulation_Channel_Impl_Send(ChannelImpl* _this, double time)
+static void EmtdcCosimulation_Channel_Impl_Send(ChannelImpl* _this, double time)
    {
    void * buffer;
    char * ptr;
    int i;
    int n;
 
    /* Get a buffer ready to send */
    /**/
    buffer = pEmtdcCosimulation_Channel_Impl_Buffer->GetBuffer(pEmtdcCosimulation_Channel_Impl_Buffer, _this->iMessageSize);
    ptr = (char*)buffer;
 
    /* Set the channel id and the valid time as the header value */
    /**/
-   ptr = _this->SetValueBufferI(_this, ptr, _this->iChannelId);
-   ptr = _this->SetValueBufferD(_this, ptr, time);
+   ptr = EmtdcCosimulation_Channel_Impl_SetValueBufferI(_this, ptr, _this->iChannelId);
+   ptr = EmtdcCosimulation_Channel_Impl_SetValueBufferD(_this, ptr, time);
 
    /* Set each of the values into the buffer */
    /**/
    n = _this->iSendSize;
    for ( i = 0 ; i < n; i++)
       {
-      ptr = _this->SetValueBufferD(_this, ptr, _this->pSendMessage->pData[i]);
+      ptr = EmtdcCosimulation_Channel_Impl_SetValueBufferD(_this, ptr, _this->pSendMessage->pData[i]);
+      _this->pLastMessage->pData[i] = _this->pSendMessage->pData[i];
       _this->pSendMessage->pData[i] = 0;
       }
 
    /* Send the buffer to the specified client */
    /**/
    CommunicationFabric_Send_Client(_this->iClientId, buffer, _this->iMessageSize, 0);
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_Channel_Impl_Parse()                                                                      */
 /*-------------------------------------------------------------------------------------------------------------*/
-void           EmtdcCosimulation_Channel_Impl_Parse(ChannelImpl* _this, void * _ptr, int size)
+static void EmtdcCosimulation_Channel_Impl_Parse(ChannelImpl* _this, void * _ptr, int size)
    {
    int channel_id;
    int message_size;
    void * ptr;
    int i;
    int n;
    Message * last;
@@ -816,95 +806,142 @@
          /**/
          last = _this->pRecvMessage;
          while (last->pNextMessage != NULL)
             last = last->pNextMessage;
 
          last->pNextMessage = _this->pRecvMessageBuffer;
          _this->pRecvMessageBuffer = _this->pRecvMessageBuffer->pNextMessage;
-         _this->pRecvMessage->pNextMessage = NULL;
+         last->pNextMessage->pNextMessage = NULL;
          }
       }
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_Channel_Impl_SetValueBufferI()                                                            */
 /*-------------------------------------------------------------------------------------------------------------*/
-char *         EmtdcCosimulation_Channel_Impl_SetValueBufferI(ChannelImpl* _this, char* ptr, unsigned int val)
+static char * EmtdcCosimulation_Channel_Impl_SetValueBufferI(ChannelImpl* _this, char* ptr, unsigned int val)
    {
    *((unsigned int*)ptr) = EmtdcCosimulation_Marshal_int32(val);
    return ptr + sizeof(unsigned int);
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_Channel_Impl_SetValueBufferD()                                                            */
 /*-------------------------------------------------------------------------------------------------------------*/
-char *         EmtdcCosimulation_Channel_Impl_SetValueBufferD(ChannelImpl* _this, char* ptr, double val)
+static char * EmtdcCosimulation_Channel_Impl_SetValueBufferD(ChannelImpl* _this, char* ptr, double val)
    {
    *((double*)ptr) = EmtdcCosimulation_Marshal_double(val);
    return ptr + sizeof(double);
    }
 
+/*-------------------------------------------------------------------------------------------------------------*/
+/* EmtdcCosimulation_Channel_Impl_Send_Final()                                                            */
+/*-------------------------------------------------------------------------------------------------------------*/
+static void  EmtdcCosimulation_Channel_Impl_Send_Final(ChannelImpl* _this)
+   {
+   void* buffer;
+   char* ptr;
+   int i;
+   int n;
+
+   /* Get a buffer ready to send */
+   /**/
+   buffer = pEmtdcCosimulation_Channel_Impl_Buffer->GetBuffer(pEmtdcCosimulation_Channel_Impl_Buffer, _this->iMessageSize);
+   ptr = (char*)buffer;
+
+   /* Set the channel id and the valid time as the header value                        */
+   /* As this is the final send the time will be set to the maximum double value       */
+   /* this indicates an unlimited amount of time. This value is valid from the last    */
+   /* message sent until the simulation is complete.                                   */
+   /**/
+   ptr = EmtdcCosimulation_Channel_Impl_SetValueBufferI(_this, ptr, _this->iChannelId);
+   ptr = EmtdcCosimulation_Channel_Impl_SetValueBufferD(_this, ptr, DBL_MAX);
+
+   /* Set each of the values into the buffer */
+   /**/
+   n = _this->iSendSize;
+   for (i = 0; i < n; i++)
+      ptr = EmtdcCosimulation_Channel_Impl_SetValueBufferD(_this, ptr, _this->pLastMessage->pData[i]);
+
+   /* Send the buffer to the specified client */
+   /**/
+   CommunicationFabric_Send_Client(_this->iClientId, buffer, _this->iMessageSize, 0);
+   }
+
+/*-------------------------------------------------------------------*/
+/* Structure                                                         */
+/*-------------------------------------------------------------------*/
+struct EmtdcCosimulation_InitData_S
+   {
+   const char* sFabricLocation;
+   const char* sHostName;
+   int iPort;
+   int iClientId;
+   double dTime;
+   double dStep;
+   };
+
 /*=============================================================================================================*/
-/* InitializeCosimulation                                                                                      */
+/* EmtdcCosimulation_InitializeCosimulationImpl                                                                */
 /*-------------------------------------------------------------------------------------------------------------*/
-/* Call this function to start the Co-Simulation Process. Only call this                                       */
-/* function once per process. This version of the function accepts the                                         */
-/* host-name and the port directly                                                                             */
+/* IMplementation of initialization this should only be called once                                            */
 /*=============================================================================================================*/
-void   EmtdcCosimulation_InitializeCosimulation(const char * fabric_location, const char * hostname, int port, int client_id)
+static void EmtdcCosimulation_InitializeCosimulationImpl(InitData* data)
    {
    char s_port[10];
    char s_id[10];
-   char * exe_path;
-   char * cmp_name;
+   char* exe_path;
+   char* cmp_name;
    const int iargs = 9;
-   char * args[9];
+   char* args[9];
    int peek_size;
-   void * _buffer;
-   void * send_buffer;
+   void* _buffer;
+   void* send_buffer;
    int com_size;
    int header;
    int channel_count;
    int message_size;
    int i;
    int n;
    int client_id2;
    int channel_id;
    int send_size;
    int recv_size;
    int pid;
    unsigned long cmp_name_size;
-   EmtdcCosimulation_Channel * new_channel;
-   Buffer * buffer;
+   EmtdcCosimulation_Channel* new_channel;
+   Buffer* buffer;
    HMODULE hModule;
 
    /* Load the communication fabric */
    /**/
-   if (CommunicationFabric_Load(fabric_location) == 0)
+   if (CommunicationFabric_Load(data->sFabricLocation) == 0)
       return;
 
    /* If this has already been initialized do not initialize again */
    /**/
    if (pEmtdcCosimulation_ChannelManager != NULL)
       return;
 
    /* Copy the parameters to be used during the finalization process */
    /**/
-   iEmtdcCosimulation_ClientId = client_id;
-   iEmtdcCosimulation_Port = port;
-   strcpy_s(sEmtdcCosimulation_HostName, 256, hostname);
+   iEmtdcCosimulation_ClientId = data->iClientId;
+   iEmtdcCosimulation_Port = data->iPort;
+   strcpy_s(sEmtdcCosimulation_HostName, 256, data->sHostName);
+   dEmtdcCosimulation_Time = data->dTime;
+   dEmtdcCosimulation_Step = data->dStep;
 
    /* Convert the integers to strings to pass in as arguments */
    /**/
    _itoa_s(iEmtdcCosimulation_Port, s_port, 10, 10);
    _itoa_s(iEmtdcCosimulation_ClientId, s_id, 10, 10);
 
    /* Get the executable path */
    /**/
-   exe_path = malloc(sizeof(char)*MAX_PATH);
+   exe_path = malloc(sizeof(char) * MAX_PATH);
    hModule = GetModuleHandle(NULL);
    GetModuleFileNameA(hModule, exe_path, MAX_PATH);
 
    /* Construct the arguments */
    /**/
    args[0] = exe_path;
    args[1] = "/API";
@@ -916,35 +953,35 @@
    args[7] = "/ID";
    args[8] = s_id;
 
    /* Initialize the Communication Fabric                               */
    /* (When this process returns all connection will be established)    */
    /**/
    CommunicationFabric_Initialize(iargs, args);
-  
+
    /* Construct a new Channel manager to process the channels */
    /**/
    pEmtdcCosimulation_ChannelManager = EmtdcCosimulation_HashTable_Create(0.75);
-  
+
    /* Check Message Size of the incoming Channel Map from the master (PSCAD) */
    /**/
-   peek_size = CommunicationFabric_Peek_Server(0, NULL, 0, 0);  
+   peek_size = CommunicationFabric_Peek_Server(0, NULL, 0, 0);
 
    /* Allocate a buffer large enough for the Map */
    /**/
    buffer = EmtdcCosimulation_Buffer_Create();
    _buffer = buffer->GetBuffer(buffer, peek_size);
 
    /* Receive the Map from the master (PSCAD) */
    /**/
    com_size = CommunicationFabric_Recv_Server(0, _buffer, peek_size, 0);
 
    /* Ensure the message is large enough to contain the meta-data on the map itself */
    /**/
-   assert(com_size >= (sizeof(int) + sizeof(int)));   
+   assert(com_size >= (sizeof(int) + sizeof(int)));
    if (com_size >= (sizeof(int) + sizeof(int)))
       {
       /* Extract the header to ensure the communication is transmitting correctly  */
       /* and extract the count of channel contains in the message                  */
       /**/
       _buffer = EmtdcCosimulation_Extract_int32(_buffer, &header);
       _buffer = EmtdcCosimulation_Extract_int32(_buffer, &channel_count);
@@ -969,31 +1006,31 @@
             _buffer = EmtdcCosimulation_Extract_int32(_buffer, &client_id2);
             _buffer = EmtdcCosimulation_Extract_int32(_buffer, &channel_id);
             _buffer = EmtdcCosimulation_Extract_int32(_buffer, &send_size);
             _buffer = EmtdcCosimulation_Extract_int32(_buffer, &recv_size);
 
             /* Construct a new Channel */
             /**/
-            new_channel = EmtdcCosimulation_Channel_Create(client_id2, channel_id, recv_size/sizeof(double), send_size/sizeof(double));
+            new_channel = EmtdcCosimulation_Channel_Create(client_id2, channel_id, recv_size / sizeof(double), send_size / sizeof(double));
 
             /* Add the Channel to the Hash-Table Manager of the Channels */
             /**/
-            pEmtdcCosimulation_ChannelManager->Append(pEmtdcCosimulation_ChannelManager, new_channel, channel_id);
+            EmtdcCosimulation_HashTable_Append(pEmtdcCosimulation_ChannelManager, new_channel, channel_id);
             }
          }
       }
 
 
    /* Send identification information back to the master */
    /**/
    cmp_name_size = MAX_COMPUTERNAME_LENGTH + 1;
-   cmp_name = malloc(sizeof(char)*cmp_name_size);
+   cmp_name = malloc(sizeof(char) * cmp_name_size);
    GetComputerNameA(cmp_name, &cmp_name_size);
    pid = GetCurrentProcessId();
-   send_size = (int)(sizeof(int) + sizeof(char)*strlen(cmp_name) + 1);
+   send_size = (int)(sizeof(int) + sizeof(char) * strlen(cmp_name) + 1);
 
    send_buffer = buffer->GetBuffer(buffer, send_size);
    _buffer = EmtdcCosimulation_Insert_int32(send_buffer, pid);
    _buffer = EmtdcCosimulation_Insert_string(_buffer, cmp_name);
 
    CommunicationFabric_Send_Server(0, send_buffer, (unsigned short)send_size, 0);
 
@@ -1003,70 +1040,103 @@
    free(exe_path);
    }
 
 /*=============================================================================================================*/
 /* InitializeCosimulation                                                                                      */
 /*-------------------------------------------------------------------------------------------------------------*/
 /* Call this function to start the Co-Simulation Process. Only call this                                       */
+/* function once per process. This version of the function accepts the                                         */
+/* host-name and the port directly                                                                             */
+/*=============================================================================================================*/
+void   EmtdcCosimulation_InitializeCosimulation(const char* fabric_location, const char* hostname, int port, int client_id)
+   {
+   InitData data;
+   data.sFabricLocation = fabric_location;
+   data.sHostName = hostname;
+   data.iPort = port;
+   data.iClientId = client_id;
+   data.dTime = 0;
+   data.dStep = 0;
+   EmtdcCosimulation_InitializeCosimulationImpl(&data);
+   }
+
+/*=============================================================================================================*/
+/* InitializeCosimulation                                                                                      */
+/*-------------------------------------------------------------------------------------------------------------*/
+/* Call this function to start the Co-Simulation Process. Only call this                                       */
 /* function once per process. This version of the function accepts the accepts                                 */
 /* the host and port as a configuration file.                                                                  */
 /*=============================================================================================================*/
 void  EmtdcCosimulation_InitializeCosimulationCfg(const char * cfg_path)
    {
-
    const char * TAG_CLIENT;
    const char * TAG_VERSION;
    const char * TAG_ADDRESS;
    const char * TAG_PORT;
    const char * TAG_COMFAB_x86;
    const char * TAG_COMFAB_x64;
+   const char * TAG_TIME;
+   const char * TAG_STEP;
 
    int MAX_LINE_LENGTH;
    int MAX_IPADDRESS_LENGTH;
    int TAG_SIZE_CLIENT;
    int TAG_SIZE_VERSION;
    int TAG_SIZE_ADDRESS;
    int TAG_SIZE_PORT;
    int TAG_SIZE_COMFAB_x86;
    int TAG_SIZE_COMFAB_x64;
+   int TAG_SIZE_TIME;
+   int TAG_SIZE_STEP;
 
    FILE *   file;
    char*    _line;
    int      version;
    int      client_id;
    char *   ipaddress;
    char *   comfab_x86;
    char *   comfab_x64;
    int      port;
+   double   time;
+   double   step;
+
+   InitData data;
+   memset(&data, 0, sizeof(InitData));
 
    /* Initialize Memory required to read the file */
    /**/
    MAX_LINE_LENGTH = 1024;
    MAX_IPADDRESS_LENGTH = 256;
 
    file = NULL;
    _line = NULL;
    version = 0;
    ipaddress = NULL;
    port = 0;
    client_id = -1;
+   time = 0.0;
+   step = 0.0;
 
    TAG_CLIENT = "Client:";
    TAG_VERSION = "Version:";
    TAG_ADDRESS = "Address:";
    TAG_PORT    = "Port:";
    TAG_COMFAB_x86 = "ComFabx86:";
    TAG_COMFAB_x64 = "ComFabx64:";
+   TAG_TIME = "Time:";
+   TAG_STEP = "Step:";
 
    TAG_SIZE_CLIENT = (int)strlen(TAG_CLIENT);
    TAG_SIZE_VERSION = (int)strlen(TAG_VERSION);
    TAG_SIZE_ADDRESS = (int)strlen(TAG_ADDRESS);
    TAG_SIZE_PORT = (int)strlen(TAG_PORT);
    TAG_SIZE_COMFAB_x86 = (int)strlen(TAG_COMFAB_x86);
    TAG_SIZE_COMFAB_x64 = (int)strlen(TAG_COMFAB_x64);
+   TAG_SIZE_TIME = (int)strlen(TAG_TIME);
+   TAG_SIZE_STEP = (int)strlen(TAG_STEP);
 
    _line = (char*)malloc(sizeof(char) * MAX_LINE_LENGTH);
    ipaddress = (char*)malloc(sizeof(char) * MAX_IPADDRESS_LENGTH);
    comfab_x86 = (char*)malloc(sizeof(char) * MAX_PATH);
    comfab_x64 = (char*)malloc(sizeof(char) * MAX_PATH);
 
    memset(ipaddress, 0, sizeof(char) * MAX_IPADDRESS_LENGTH);
@@ -1118,14 +1188,24 @@
                {
                strcpy_s(comfab_x86, MAX_PATH, _line + TAG_SIZE_COMFAB_x86);
                }
             else if (strnicmp(TAG_COMFAB_x64, _line, TAG_SIZE_COMFAB_x64) == 0)
                {
                strcpy_s(comfab_x64, MAX_PATH, _line + TAG_SIZE_COMFAB_x64);
                }
+            else if (strnicmp(TAG_TIME, _line, TAG_SIZE_TIME) == 0)
+               {
+               if (sscanf_s(_line + TAG_SIZE_TIME, "%lf", &time) != 1)
+                  time = 0.0;
+               }
+            else if (strnicmp(TAG_STEP, _line, TAG_SIZE_STEP) == 0)
+               {
+               if (sscanf_s(_line + TAG_SIZE_STEP, "%lf", &step) != 1)
+                  step = 0.0;
+               }
             }
          }
       }
 
    /* Close and free required memory, and resources */
    /**/
    fclose(file);
@@ -1133,17 +1213,23 @@
    _line = NULL;
 
    /* Perform normal initialization */
    /**/
    if (port > 0 && client_id > 0 && ipaddress[0] != '\0' && comfab_x86[0] != '\0' && comfab_x64[0] != '\0')
       {
       if (sizeof(char*) == 4)
-         EmtdcCosimulation_InitializeCosimulation(EmtdcCosimulation_string_trim(comfab_x86), ipaddress, port, client_id);
+         data.sFabricLocation = EmtdcCosimulation_string_trim(comfab_x86);
       else if (sizeof(char*) == 8)
-         EmtdcCosimulation_InitializeCosimulation(EmtdcCosimulation_string_trim(comfab_x64), ipaddress, port, client_id);
+         data.sFabricLocation = EmtdcCosimulation_string_trim(comfab_x64);
+      data.sHostName = ipaddress;
+      data.iClientId = client_id;
+      data.iPort = port;
+      data.dTime = time;
+      data.dStep = step;
+      EmtdcCosimulation_InitializeCosimulationImpl(&data);
       }
 
    free(ipaddress);
    free(comfab_x86);
    free(comfab_x64);
    ipaddress = NULL;
    }
@@ -1152,41 +1238,70 @@
 /* FindChannel()                                                                                               */
 /*-------------------------------------------------------------------------------------------------------------*/
 /* Get the channel with the channel_id specified (if it exists)                                                */
 /*=============================================================================================================*/
 EmtdcCosimulation_Channel *   EmtdcCosimulation_FindChannel(unsigned int channel_id)
    {
    if (pEmtdcCosimulation_ChannelManager != NULL)
-      return (EmtdcCosimulation_Channel*)pEmtdcCosimulation_ChannelManager->Fetch(pEmtdcCosimulation_ChannelManager, channel_id);
+      return (EmtdcCosimulation_Channel*)EmtdcCosimulation_HashTable_Fetch(pEmtdcCosimulation_ChannelManager, channel_id);
    return NULL;
    }
 
 /*=============================================================================================================*/
 /* FinalizeCosimulation                                                                                        */
 /*-------------------------------------------------------------------------------------------------------------*/
 /* Call this function to end the Co-Simulation process                                                         */
 /*=============================================================================================================*/
-void             EmtdcCosimulation_FinalizeCosimulation()
+void  EmtdcCosimulation_FinalizeCosimulation()
    {
    char s_port[10];
    char s_id[10];
    const int iargs = 9;
    char * args[9];
    char*  exe_path;
    HMODULE hModule;
    int message;
-   int i;
-   int n;
+   int i, n;
+   EmtdcCosimulation_Channel* channel;
+   ChannelImpl* channel_imp;
 
    /* If the Co-Simulation has not been initialized then */
    /* it cannot be finalized                             */
    /**/
    if (pEmtdcCosimulation_ChannelManager == NULL)
       return;
 
+   /* Resend the last message with unlimited expiration date. This will ensure */
+   /* that the simulation will not stall if the timings are slightly off       */
+   /**/
+   n = EmtdcCosimulation_HashTable_GetCount(pEmtdcCosimulation_ChannelManager);
+   for (i = 0; i < n; i++)
+      {
+      channel = EmtdcCosimulation_HashTable_Get(pEmtdcCosimulation_ChannelManager, i);
+      if (channel != NULL && EmtdcCosimulation_Channel_GetSendSize(channel) > 0)
+         {
+         channel_imp = (ChannelImpl*)channel->pReserved;
+         if (channel_imp != NULL)
+            EmtdcCosimulation_Channel_Impl_Send_Final(channel_imp);
+         }
+      }
+
+   /* Receive all data until the end of the simulation to ensure the buffer is emptied */
+   /**/
+   if (dEmtdcCosimulation_Time > 0)
+      {
+      n = EmtdcCosimulation_HashTable_GetCount(pEmtdcCosimulation_ChannelManager);
+      for (i = 0; i < n; i++)
+         {
+         channel = EmtdcCosimulation_HashTable_Get(pEmtdcCosimulation_ChannelManager, i);
+         if (channel != NULL && EmtdcCosimulation_Channel_GetRecvSize(channel) > 0)
+            EmtdcCosimulation_Channel_GetValue(channel, dEmtdcCosimulation_Time, 0);
+         }
+      }
+
    /* Send a complete message */
    /**/
    message = 0xFFFF;
    CommunicationFabric_Send_Server(0, &message, sizeof(int), 0);
 
    /* Reconstruct the argument list */
    /**/
@@ -1211,17 +1326,17 @@
 
    /* Finalize the communication fabric, this will disconnect and shut down all communication */
    /**/
    CommunicationFabric_Finalize(iargs, args);
 
    /* Delete and reset the channel manager */
    /**/
-   n = pEmtdcCosimulation_ChannelManager->GetCount(pEmtdcCosimulation_ChannelManager);
+   n = EmtdcCosimulation_HashTable_GetCount(pEmtdcCosimulation_ChannelManager);
    for (i = 0; i < n; i++)
-      EmtdcCosimulation_Channel_Delete((EmtdcCosimulation_Channel*)pEmtdcCosimulation_ChannelManager->Get(pEmtdcCosimulation_ChannelManager, i));
+      EmtdcCosimulation_Channel_Delete((EmtdcCosimulation_Channel*)EmtdcCosimulation_HashTable_Get(pEmtdcCosimulation_ChannelManager, i));
 
    EmtdcCosimulation_HashTable_Delete(pEmtdcCosimulation_ChannelManager);
    pEmtdcCosimulation_ChannelManager = NULL;
 
    /* Clean up and remove the communication fabric */
    CommunicationFabric_Unload();
 
@@ -1233,15 +1348,15 @@
 /*-------------------------------------------------------------------------------------------------------------*/
 /* This namespace contains the calls into the Communication Fabric DLL.                                        */
 /*-------------------------------------------------------------------------------------------------------------*/
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* Load()                                                                                                      */
 /*-------------------------------------------------------------------------------------------------------------*/
-int CommunicationFabric_Load(const char * location)
+static int CommunicationFabric_Load(const char * location)
    {
    hComFabLibrary = LoadLibraryA(location);
    if ( hComFabLibrary != NULL )
       {
       _CommunicationFabric_Initialize  = (CommunicationFabric_Init_Func)GetProcAddress(hComFabLibrary,"Communication_Initialize");
 	   _CommunicationFabric_Finalize    = (CommunicationFabric_Init_Func)GetProcAddress(hComFabLibrary,"Communication_Finalize");
 	   _CommunicationFabric_Send_Client = (CommunicationFabric_Com_Func)GetProcAddress(hComFabLibrary,"Communication_send_client");
@@ -1259,15 +1374,15 @@
       }
    return 0;
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* CommunicationFabric_Unload()                                                                                */
 /*-------------------------------------------------------------------------------------------------------------*/
-int CommunicationFabric_Unload()
+static int CommunicationFabric_Unload()
    {
    if (hComFabLibrary != NULL)
       {
       /* Reset the Function pointers to NULL */
       /**/
       _CommunicationFabric_Initialize   = NULL;
       _CommunicationFabric_Finalize     = NULL;
@@ -1291,85 +1406,85 @@
 
    return 0;
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* CommunicationFabric_Initialize()                                                                            */
 /*-------------------------------------------------------------------------------------------------------------*/
-int CommunicationFabric_Initialize(int argc, char * args[])
+static int CommunicationFabric_Initialize(int argc, char * args[])
    {
    if ( _CommunicationFabric_Initialize != NULL )
       return _CommunicationFabric_Initialize(argc, args);
    return -10; /* This should not happen */
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* CommunicationFabric_Finalize()                                                                              */
 /*-------------------------------------------------------------------------------------------------------------*/
-int CommunicationFabric_Finalize(int argc, char * args[])
+static int CommunicationFabric_Finalize(int argc, char * args[])
    {
    if ( _CommunicationFabric_Finalize != NULL )
       return _CommunicationFabric_Finalize(argc, args);
    return -10; /* This should not happen */
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* CommunicationFabric_send_client()                                                                           */
 /*-------------------------------------------------------------------------------------------------------------*/
-int CommunicationFabric_Send_Client(unsigned short to, void * buffer, unsigned short size, unsigned short flag)
+static int CommunicationFabric_Send_Client(unsigned short to, void * buffer, unsigned short size, unsigned short flag)
    {
    if ( _CommunicationFabric_Send_Client != NULL )
       return _CommunicationFabric_Send_Client(to, buffer, size, flag);
    return -10; /* This should not happen */
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* CommunicationFabric_recv_client()                                                                           */
 /*-------------------------------------------------------------------------------------------------------------*/
-int CommunicationFabric_Recv_Client(unsigned short to, void * buffer, unsigned short size, unsigned short flag)
+static int CommunicationFabric_Recv_Client(unsigned short to, void * buffer, unsigned short size, unsigned short flag)
    {
    if ( _CommunicationFabric_Recv_Client != NULL )
       return _CommunicationFabric_Recv_Client(to, buffer, size, flag);
    return -10; /* This should not happen */
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* CommunicationFabric_peek_client()                                                                           */
 /*-------------------------------------------------------------------------------------------------------------*/
-int CommunicationFabric_Peek_Client(unsigned short to, void * buffer, unsigned short size, unsigned short flag)
+static int CommunicationFabric_Peek_Client(unsigned short to, void * buffer, unsigned short size, unsigned short flag)
    {
    if ( _CommunicationFabric_Peek_Client != NULL )
       return _CommunicationFabric_Peek_Client(to, buffer, size, flag);
    return -10; /* This should not happen */
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* CommunicationFabric_send_server()                                                                           */
 /*-------------------------------------------------------------------------------------------------------------*/
-int CommunicationFabric_Send_Server(unsigned short to, void * buffer, unsigned short size, unsigned short flag)
+static int CommunicationFabric_Send_Server(unsigned short to, void * buffer, unsigned short size, unsigned short flag)
    {
    if ( _CommunicationFabric_Send_Server != NULL )
       return _CommunicationFabric_Send_Server(to, buffer, size, flag);
    return -10; /* This should not happen */
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* CommunicationFabric_recv_server()                                                                           */
 /*-------------------------------------------------------------------------------------------------------------*/
-int CommunicationFabric_Recv_Server(unsigned short to, void * buffer, unsigned short size, unsigned short flag)
+static int CommunicationFabric_Recv_Server(unsigned short to, void * buffer, unsigned short size, unsigned short flag)
    {
    if ( _CommunicationFabric_Recv_Server != NULL )
       return _CommunicationFabric_Recv_Server(to, buffer, size, flag);
    return -10; /* This should not happen */
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* CommunicationFabric_peek_server()                                                                           */
 /*-------------------------------------------------------------------------------------------------------------*/
-int CommunicationFabric_Peek_Server(unsigned short to, void * buffer, unsigned short size, unsigned short flag)
+static int CommunicationFabric_Peek_Server(unsigned short to, void * buffer, unsigned short size, unsigned short flag)
    {
    if ( _CommunicationFabric_Peek_Server != NULL )
       return _CommunicationFabric_Peek_Server(to, buffer, size, flag);
    return -10; /* This should not happen */
    }
 
 /*=============================================================================================================*/
@@ -1378,15 +1493,15 @@
 /* This is a fast hash-table used to quickly retrieve objects by a hash                                        */
 /* identifier                                                                                                  */
 /*=============================================================================================================*/
 
 /*=============================================================================================================*/
 /* Constructor                                                                                                 */
 /*=============================================================================================================*/
-HashTable * EmtdcCosimulation_HashTable_Create(double fill_cap)
+static HashTable * EmtdcCosimulation_HashTable_Create(double fill_cap)
    {
 
    HashTable * _this;
 
    /* Allocate memory */
    /**/
    _this = (HashTable*)malloc(sizeof(HashTable));
@@ -1401,33 +1516,21 @@
 
    /* Initialize Memory */
    /**/
    memset(_this->aHash     , 0, _this->iHashSize   *  sizeof(HashTableEntry));
    memset(_this->aKeys     , 0, _this->iCapacity   *  sizeof(int));
    memset(_this->aObjects  , 0, _this->iCapacity   *  sizeof(HashTableObject));
 
-   /* Set the functions */
-   /**/
-   _this->Fetch            = &EmtdcCosimulation_HashTable_Fetch;
-   _this->Append           = &EmtdcCosimulation_HashTable_Append;
-   _this->Remove           = &EmtdcCosimulation_HashTable_Remove;
-   _this->GetCount         = &EmtdcCosimulation_HashTable_GetCount;
-   _this->GetKey           = &EmtdcCosimulation_HashTable_GetKey;
-   _this->Get              = &EmtdcCosimulation_HashTable_Get;
-   _this->EnsureCapacity   = &EmtdcCosimulation_HashTable_EnsureCapacity;
-   _this->Hash             = &EmtdcCosimulation_HashTable_Hash;
-   _this->Rebuild          = &EmtdcCosimulation_HashTable_Rebuild;
-
    return _this;
    }
 
 /*=============================================================================================================*/
 /* Destructor                                                                                                  */
 /*=============================================================================================================*/
-void EmtdcCosimulation_HashTable_Delete(HashTable * _this)
+static void EmtdcCosimulation_HashTable_Delete(HashTable * _this)
    {
    /* Ensure the structure exists */
    /**/
    if (_this == NULL)
       return;
 
    /* Deallocate the internal lists and arrays */
@@ -1440,43 +1543,43 @@
    /**/
    free(_this);
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_HashTable_Fetch()                                                                         */
 /*-------------------------------------------------------------------------------------------------------------*/
-void*  EmtdcCosimulation_HashTable_Fetch(HashTable * _this, int key)
+static void*  EmtdcCosimulation_HashTable_Fetch(HashTable * _this, int key)
    {
    int val;
 
    if (0 < key)
       {
-      val = _this->Hash(_this, key, 0, NULL, 0);
+      val = EmtdcCosimulation_HashTable_Hash(_this, key, 0, NULL, 0);
       if (val >= 0 && _this->aHash[val].iKey == key )
          return _this->aObjects[_this->aHash[val].iIndex];
       }
    return NULL;
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_HashTable_Append()                                                                        */
 /*-------------------------------------------------------------------------------------------------------------*/
-int    EmtdcCosimulation_HashTable_Append(HashTable * _this, void* object, int key)
+static int    EmtdcCosimulation_HashTable_Append(HashTable * _this, void* object, int key)
    {
    int val;
 
    if (object != NULL && 0 < key)
       {
-      _this->EnsureCapacity(_this, _this->iCount + 1);
+      EmtdcCosimulation_HashTable_EnsureCapacity(_this, _this->iCount + 1);
 
       /* By design the object map must have a unique key   */
       /* for each object. Ensure that the key is available */
       /* before adding it to the map.                      */
       /**/
-      val = _this->Hash(_this, key, 1, NULL, 0);
+      val = EmtdcCosimulation_HashTable_Hash(_this, key, 1, NULL, 0);
       if (val >= 0 && _this->aHash[val].iKey == 0 || _this->aHash[val].iKey == -1)
          {
          _this->aKeys[_this->iCount] = key;
          _this->aObjects[_this->iCount] = object;
          _this->aHash[val].iIndex = _this->iCount;
          _this->aHash[val].iKey = key;
          _this->iCount++;
@@ -1485,90 +1588,90 @@
       }
    return 0;
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_HashTable_Remove()                                                                        */
 /*-------------------------------------------------------------------------------------------------------------*/
-int    EmtdcCosimulation_HashTable_Remove(HashTable * _this, int key)
+static int    EmtdcCosimulation_HashTable_Remove(HashTable * _this, int key)
    {
    int val;
    int empty_ratio;
    int min_remove;
 
-   val = _this->Hash(_this, key, 0, NULL, 0);
+   val = EmtdcCosimulation_HashTable_Hash(_this, key, 0, NULL, 0);
    if (val >= 0 && _this->aHash[val].iKey == key )
       {
       int index = _this->aHash[val].iIndex;
 
       _this->aObjects[index]   = NULL;
       _this->aKeys[index]      = 0;
       _this->aHash[val].iIndex = -1;
       _this->aHash[val].iKey = -1;
 
       _this->iRemoveCount++;
 
       empty_ratio = _this->iCount/iEmtdcCosimulation_HashTable_EmptyDivisor;
-      min_remove = (empty_ratio > iEmtdcCosimulation_HashTable_EmptyMin) ? empty_ratio : iEmtdcCosimulation_HashTable_EmptyMin; 
+      min_remove = (empty_ratio > iEmtdcCosimulation_HashTable_EmptyMin) ? empty_ratio : iEmtdcCosimulation_HashTable_EmptyMin;
       if ( _this->iRemoveCount >  min_remove)
-         _this->Rebuild(_this, -1);
+         EmtdcCosimulation_HashTable_Rebuild(_this, -1);
       return 1;
       }
    return 0;
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_HashTable_GetCount()                                                                      */
 /*-------------------------------------------------------------------------------------------------------------*/
-int    EmtdcCosimulation_HashTable_GetCount(HashTable * _this)
+static int    EmtdcCosimulation_HashTable_GetCount(HashTable * _this)
    {
    return _this->iCount;
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_HashTable_GetKey()                                                                        */
 /*-------------------------------------------------------------------------------------------------------------*/
-int    EmtdcCosimulation_HashTable_GetKey(HashTable * _this, int index)
+static int    EmtdcCosimulation_HashTable_GetKey(HashTable * _this, int index)
    {
    if (0 <= index && index < _this->iCount)
       return _this->aKeys[index];
-   return -1; 
+   return -1;
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_HashTable_Get()                                                                           */
 /*-------------------------------------------------------------------------------------------------------------*/
-void*  EmtdcCosimulation_HashTable_Get(HashTable * _this, int index)
+static void*  EmtdcCosimulation_HashTable_Get(HashTable * _this, int index)
    {
    if ( 0 <= index && index < _this->iCount )
       return _this->aObjects[index];
    return NULL;
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_HashTable_EnsureCapacity()                                                                */
 /*-------------------------------------------------------------------------------------------------------------*/
-void   EmtdcCosimulation_HashTable_EnsureCapacity(HashTable * _this, int size)
+static void   EmtdcCosimulation_HashTable_EnsureCapacity(HashTable * _this, int size)
    {
    int new_capacity;
 
    if (_this->iCapacity <= size)
       {
       new_capacity = _this->iCapacity * 2;
       while (new_capacity <= size)
          new_capacity *= 2;
 
-      _this->Rebuild(_this, new_capacity);
+      EmtdcCosimulation_HashTable_Rebuild(_this, new_capacity);
       }
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_HashTable_Hash()                                                                          */
 /*-------------------------------------------------------------------------------------------------------------*/
-int    EmtdcCosimulation_HashTable_Hash(HashTable * _this, int key, int is_new, HashTableEntry* entries, int size)
+static int    EmtdcCosimulation_HashTable_Hash(HashTable * _this, int key, int is_new, HashTableEntry* entries, int size)
    {
    unsigned int count;
    unsigned int val;
 
    /* Invalid key */
    /**/
    assert(key > 0);
@@ -1609,15 +1712,15 @@
 
    return val;
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_HashTable_Rebuild()                                                                       */
 /*-------------------------------------------------------------------------------------------------------------*/
-void   EmtdcCosimulation_HashTable_Rebuild(HashTable * _this, int capacity)
+static void   EmtdcCosimulation_HashTable_Rebuild(HashTable * _this, int capacity)
    {
    int new_hashsize;
    int * new_keys;
    HashTableObject * new_objects;
    HashTableEntry* new_entries;
    int index;
    int i;
@@ -1649,15 +1752,15 @@
    n = _this->iCount;
    for ( i = 0; i < n; i++)
       {
       key = _this->aKeys[i];
       o = _this->aObjects[i];
       if ( key > 0 && o != NULL )
          {
-         val = _this->Hash(_this, key, 1, new_entries, new_hashsize);
+         val = EmtdcCosimulation_HashTable_Hash(_this, key, 1, new_entries, new_hashsize);
          if ( val >= 0 )
             {
             new_keys[index] = key;
             new_objects[index] = o;
             new_entries[val].iIndex = index;
             new_entries[val].iKey = key;
             index++;
@@ -1691,16 +1794,16 @@
 /*                                                                                                             */
 /* This is a node in a linked list of received messages                                                        */
 /*=============================================================================================================*/
 
 /*=============================================================================================================*/
 /* Constructor                                                                                                 */
 /*=============================================================================================================*/
-Message * EmtdcCosimulation_Message_Create(int size)
-   { 
+static Message * EmtdcCosimulation_Message_Create(int size)
+   {
    Message * _this;
 
    /* Allocate the structure */
    /**/
    _this = malloc(sizeof(Message));
 
    /* Set the local members */
@@ -1715,15 +1818,15 @@
 
    return _this;
    }
 
 /*=============================================================================================================*/
 /* Destructor                                                                                                  */
 /*=============================================================================================================*/
-void EmtdcCosimulation_Message_Delete(Message * _this)
+static void EmtdcCosimulation_Message_Delete(Message * _this)
    {
    /* Ensure the structure exists */
    /**/
    if (_this == NULL)
       return;
 
    /* Delete the next node in the linked list */
@@ -1745,30 +1848,30 @@
 /*-------------------------------------------------------------------------------------------------------------*/
 /* Maintains the life of an arbitrary sized data buffer                                                        */
 /*=============================================================================================================*/
 
 /*=============================================================================================================*/
 /* Constructor                                                                                                 */
 /*=============================================================================================================*/
-Buffer* EmtdcCosimulation_Buffer_Create()
+static Buffer* EmtdcCosimulation_Buffer_Create()
    {
    Buffer * _this;
    _this = malloc(sizeof(Buffer));
    _this->pBuffer = malloc(32);
    _this->iSize = 32;
 
    _this->GetBuffer = &EmtdcCosimulation_Buffer_GetBuffer;
 
    return _this;
    }
 
 /*=============================================================================================================*/
 /* Destructor                                                                                                  */
 /*=============================================================================================================*/
-void  EmtdcCosimulation_Buffer_Delete(Buffer * _this)
+static void  EmtdcCosimulation_Buffer_Delete(Buffer * _this)
    {
    /* Ensure the structure exists */
    /**/
    if (_this == NULL)
       return;
 
    /* Deallocate the memory buffer */
@@ -1779,15 +1882,15 @@
    /**/
    free(_this);
    }
 
 /*-------------------------------------------------------------------------------------------------------------*/
 /* EmtdcCosimulation_Buffer_GetBuffer()                                                                        */
 /*-------------------------------------------------------------------------------------------------------------*/
-void * EmtdcCosimulation_Buffer_GetBuffer(Buffer * _this, int size)
+static void * EmtdcCosimulation_Buffer_GetBuffer(Buffer * _this, int size)
    {
    /* If the currently allocate buffer is too small reallocate the buffer  */
    /* to be large enough to store the complete data                        */
    /**/
    if ( _this->iSize < size )
       {
       _this->pBuffer = realloc(_this->pBuffer, size);
```

### Comparing `mhi-cosim-1.1.3/src/ext/cosim.c` & `mhi_cosim-1.2.0/src/ext/cosim.c`

 * *Files identical despite different names*

### Comparing `mhi-cosim-1.1.3/src/mhi/cosim/__init__.py` & `mhi_cosim-1.2.0/src/mhi/cosim/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,23 +28,42 @@
            channel.set_values(a, b, c, d)
            channel.send(time)
 
            if time <= run_time:
                x, y, z = channel.get_values(time)
 """
 
-import os, sys
+#===============================================================================
+# Imports
+#===============================================================================
+
+from __future__ import annotations
+import os
+import sys
 from contextlib import contextmanager
-from typing import Tuple, Iterable
+from typing import Dict, Iterable, List, Tuple
 
 # Import the C extension module
-from mhi.cosim._cosim import initialize_cfg, finalize, Error, Channel
+from mhi.cosim._cosim import initialize_cfg, finalize, Error, Channel # pylint: disable=no-name-in-module
 
-VERSION = '1.1.3'
-VERSION_HEX = 0x010103f0
+
+#===============================================================================
+# Version Info
+#===============================================================================
+
+_VERSION = (1, 2, 0)
+
+_TYPE = 'f0'
+VERSION = '.'.join(map(str, _VERSION))
+VERSION_HEX = int.from_bytes((*_VERSION, int(_TYPE, 16)), byteorder='big')
+
+
+#===============================================================================
+# Named Channel
+#===============================================================================
 
 class NamedChannel:
     """
     A communication channel with subchannels identified usings
     names instead of numeric indices.
 
     Parameters:
@@ -101,14 +120,17 @@
                 channel.send(time)
 
                 if time <= run_time:
                     channel.get_values(time)
                     r_speed = channel.r_speed
     """
 
+    _channel: Channel
+    _recv_names: List[str]
+    _send: Dict[str, int]
 
     def __init__(self, channel_id, recv_names, send_names):
 
         if isinstance(recv_names, str):
             recv_names = recv_names.replace(',', ' ').split()
         recv_names = tuple(map(str, recv_names))
 
@@ -167,14 +189,18 @@
         Parameters:
             time (float): time stored values are valid until.
         """
 
         self._channel.send(time)
 
 
+#===============================================================================
+# Cosimulation
+#===============================================================================
+
 class Cosimulation:
     """
     A shim class to support a `with` statement that returns an
     object that manages intialization and finalization of the cosimulation
     library.
     """
 
@@ -206,16 +232,21 @@
                 Alternatively, `send_names` can be a single string with each
                 name separated by whitespace and/or commas, for example
                 ``'x y'`` or ``'x, y'``.
         """
 
         return NamedChannel(channel_id, recv_names, send_names)
 
+
+#===============================================================================
+# Context Manager for cosimulation
+#===============================================================================
+
 @contextmanager
-def cosimulation(config_file) -> Cosimulation:
+def cosimulation(config_file):
     """
     This function returns a context managed object suitable for use in
     a `with` statement.
 
     Parameters:
         config_file: the cosimulation configuration file.
```

### Comparing `mhi-cosim-1.1.3/src/mhi_cosim.egg-info/PKG-INFO` & `mhi_cosim-1.2.0/src/mhi_cosim.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mhi-cosim
-Version: 1.1.3
+Version: 1.2.0
 Summary: MHI Cosimulation Module
 Home-page: https://www.pscad.com/webhelp-v5-al/index.html
 Author: Manitoba Hydro International Ltd.
 Author-email: pscad@mhi.ca
 License: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -24,7 +24,13 @@
 
 ====================
 Cosimulation Library
 ====================
 
 The EMTDC Python Cosimulation Library is designed to allow control
 simulation of a portion of a power system from a Python script.
+
+=============
+Documentation
+=============
+
+Use `py -m mhi.cosim help` to access the module documentation.
```

### Comparing `mhi-cosim-1.1.3/tests/test_cosim_compliance.py` & `mhi_cosim-1.2.0/tests/test_cosim_compliance.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 import ast
 import re
+import sys
 import unittest
 
 from pathlib import Path
+from typing import Tuple
+
+if sys.version_info < (3, 9):
+    raise unittest.SkipTest("ast.parse(type_comment=, feature_version=)"
+                            " requires Python 3.9")
+
 
 class TestCompliance(unittest.TestCase):
 
     @staticmethod
     def module_path() -> Path:
         return Path(__file__).parents[1]
 
-    def python_requires(self) -> tuple[int, int]:
+    def python_requires(self) -> Tuple[int, int]:
 
         major, minor = 3, 0
 
         setup_cfg = self.module_dir / "setup.cfg"
         setup_py = self.module_dir / "setup.py"
         if setup_cfg.is_file():
-            if m := re.search(r"^\s*python_requires\s*=\s*>=\s*3.(\d+)",
-                              setup_cfg.read_text(), re.MULTILINE):
+            m = re.search(r"^\s*python_requires\s*=\s*>=\s*3.(\d+)",
+                          setup_cfg.read_text(), re.MULTILINE)
+            if m:
                 minor = int(m.group(1))
             else:
                 raise ValueError("Unable to find 'python_requires = >= 3.#'"
                                  " in setup.cfg")
         elif setup_py.is_file():
-            if m := re.search(r'''\bpython_requires=['"]>=3\.(\d+)['"]''',
-                              setup_py.read_text()):
+            m = re.search(r'''\bpython_requires=['"]>=3\.(\d+)['"]''',
+                          setup_py.read_text())
+            if m:
                 minor = int(m.group(1))
             else:
                 raise ValueError("""Unable to find 'python_requires=">=3.#"'"""
                                  " in setup.py")
 
         if minor < 4:
             raise ValueError("Python requires must be at least 3.4")
```

### Comparing `mhi-cosim-1.1.3/tests/test_cosim_version.py` & `mhi_cosim-1.2.0/tests/test_cosim_version.py`

 * *Files identical despite different names*

### Comparing `mhi-cosim-1.1.3/tests/test_help.py` & `mhi_cosim-1.2.0/tests/test_help.py`

 * *Files identical despite different names*

