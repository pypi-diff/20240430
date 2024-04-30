# Comparing `tmp/riscv_config-3.9.1.tar.gz` & `tmp/riscv_config-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/riscv_config-3.9.1.tar", last modified: Thu Jun 22 04:01:23 2023, max compression
+gzip compressed data, was "dist/riscv_config-3.9.2.tar", last modified: Mon Jul 31 12:42:53 2023, max compression
```

## Comparing `riscv_config-3.9.1.tar` & `riscv_config-3.9.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:01:23.000000 riscv_config-3.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-22 04:01:00.000000 riscv_config-3.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-22 04:01:23.000000 riscv_config-3.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-22 04:01:00.000000 riscv_config-3.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:01:23.000000 riscv_config-3.9.1/riscv_config/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    97275 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/isa_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/schemaValidator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:01:23.000000 riscv_config-3.9.1/riscv_config/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/schemas/schema_custom.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    60390 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/schemas/schema_debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   551237 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/schemas/schema_isa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/schemas/schema_platform.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36995 2023-06-22 04:01:00.000000 riscv_config-3.9.1/riscv_config/warl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:01:23.000000 riscv_config-3.9.1/riscv_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-22 04:01:23.000000 riscv_config-3.9.1/riscv_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-22 04:01:23.000000 riscv_config-3.9.1/riscv_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 04:01:23.000000 riscv_config-3.9.1/riscv_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-22 04:01:23.000000 riscv_config-3.9.1/riscv_config.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-22 04:01:23.000000 riscv_config-3.9.1/riscv_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 04:01:23.000000 riscv_config-3.9.1/riscv_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-22 04:01:23.000000 riscv_config-3.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-22 04:01:00.000000 riscv_config-3.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:42:53.000000 riscv_config-3.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-31 12:42:26.000000 riscv_config-3.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-31 12:42:53.000000 riscv_config-3.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-31 12:42:26.000000 riscv_config-3.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:42:53.000000 riscv_config-3.9.2/riscv_config/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-31 12:42:26.000000 riscv_config-3.9.2/riscv_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97727 2023-07-31 12:42:26.000000 riscv_config-3.9.2/riscv_config/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-31 12:42:26.000000 riscv_config-3.9.2/riscv_config/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-31 12:42:26.000000 riscv_config-3.9.2/riscv_config/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-31 12:42:26.000000 riscv_config-3.9.2/riscv_config/isa_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-31 12:42:26.000000 riscv_config-3.9.2/riscv_config/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17592 2023-07-31 12:42:26.000000 riscv_config-3.9.2/riscv_config/schemaValidator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:42:53.000000 riscv_config-3.9.2/riscv_config/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-31 12:42:26.000000 riscv_config-3.9.2/riscv_config/schemas/schema_custom.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    60390 2023-07-31 12:42:26.000000 riscv_config-3.9.2/riscv_config/schemas/schema_debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   551374 2023-07-31 12:42:26.000000 riscv_config-3.9.2/riscv_config/schemas/schema_isa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-31 12:42:26.000000 riscv_config-3.9.2/riscv_config/schemas/schema_platform.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-31 12:42:26.000000 riscv_config-3.9.2/riscv_config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36995 2023-07-31 12:42:26.000000 riscv_config-3.9.2/riscv_config/warl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:42:53.000000 riscv_config-3.9.2/riscv_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-31 12:42:52.000000 riscv_config-3.9.2/riscv_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-31 12:42:53.000000 riscv_config-3.9.2/riscv_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 12:42:52.000000 riscv_config-3.9.2/riscv_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-31 12:42:52.000000 riscv_config-3.9.2/riscv_config.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-31 12:42:52.000000 riscv_config-3.9.2/riscv_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 12:42:52.000000 riscv_config-3.9.2/riscv_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-31 12:42:53.000000 riscv_config-3.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-31 12:42:26.000000 riscv_config-3.9.2/setup.py
```

### Comparing `riscv_config-3.9.1/PKG-INFO` & `riscv_config-3.9.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: riscv_config
-Version: 3.9.1
+Version: 3.9.2
 Summary: RISC-V Configuration Validator
 Home-page: https://github.com/riscv/riscv-config
 Author: InCore Semiconductors Pvt. Ltd.
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: RISCV-Config
         ==============
```

### Comparing `riscv_config-3.9.1/riscv_config/checker.py` & `riscv_config-3.9.2/riscv_config/checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,42 +40,42 @@
             if (x in extension_list):
                 extension_enc[25 - int(ord(x) - ord('A'))] = "1"
     extensions = int("".join(extension_enc), 2)
     ext_b=format(extensions, '#0{}b'.format(xlen+2))
     mxl='10'if xlen==64 else '01'
     ext_b = ext_b[:2] + str(mxl) + ext_b[4:]
     return int(ext_b, 2)
- 
+
 def resetsu():
     '''Function to set defaults to reset val of mstatus based on the xlen and S, U extensions'''
     global inp_yaml
     global extension_list
     if 64 in inp_yaml['supported_xlen'] and 'S' not in extension_list and 'U' in extension_list:
       return 8589934592
     elif 64 in inp_yaml['supported_xlen'] and 'U' in extension_list and 'S' in extension_list:
       return 42949672960
-    else:	
+    else:
       return 0
 def reset_vsstatus():
     '''Function to set defaults to reset val of mstatus based on the xlen and S, U extensions'''
     global inp_yaml
     global extension_list
     if 64 in inp_yaml['supported_xlen'] and 'U' in extension_list:
       return 8589934592
-    else:	
+    else:
       return 0
 
 def uset():
     '''Function to set defaults based on presence of 'U' extension.'''
     global extension_list
     if 'U' in extension_list:
         return {'implemented': True}
     else:
         return {'implemented': False}
-   
+
 def hset():
     '''Function to set defaults based on presence of 'U' extension.'''
     global extension_list
     if 'H' in extension_list:
         return {'implemented': True}
     else:
         return {'implemented': False}
@@ -84,23 +84,42 @@
 def sset():
     '''Function to set defaults based on presence of 'S' extension.'''
     global extension_list
     if 'S' in extension_list:
         return {'implemented': True}
     else:
         return {'implemented': False}
-        
+
 def fsset():
-    '''Function to set defaults based on presence of 'F' extension.'''
+    '''Function to set defaults based on presence of 'F' or 'S' extension.'''
     global extension_list
     if 'F' in extension_list or 'S' in extension_list:
         return {'implemented': True}
     else:
         return {'implemented': False}
-        
+
+def fset():
+    '''Function to set defaults based on presence of 'F' extension.'''
+    global extension_list
+    if 'F' in extension_list:
+        return {'implemented': True}
+    else:
+        return {'implemented': False}
+
+def fregset():
+    '''Function to set defaults based on presence of 'F' extension.'''
+    global inp_yaml
+    global extension_list
+    temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}}
+    if 'F' in extension_list:
+      if 32 in inp_yaml['supported_xlen']:
+        temp['rv32']['accessible'] = True
+      if 64 in inp_yaml['supported_xlen']:
+        temp['rv64']['accessible'] = True
+    return temp
 
 def uregset():
     '''Function to set defaults based on presence of 'U' extension.'''
     global inp_yaml
     global extension_list
     temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}}
     if 'U' in extension_list:
@@ -115,24 +134,24 @@
     global inp_yaml
     global extension_list
     temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}}
     if 'U' in extension_list:
       if 32 in inp_yaml['supported_xlen']:
         temp['rv32']['accessible'] = True
     return temp
-  
+
 def hregseth():
     '''Function to set defaults based on presence of 'H' extension.'''
     global inp_yaml
     global extension_list
     temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}}
     if 'H' in extension_list:
       if 32 in inp_yaml['supported_xlen']:
         temp['rv32']['accessible'] = True
-    return temp      
+    return temp
 def sregset():
     '''Function to set defaults based on presence of 'S' extension.'''
     global inp_yaml
     global extension_list
     temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}}
     if 'S' in extension_list:
       if 32 in inp_yaml['supported_xlen']:
@@ -160,15 +179,15 @@
     temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}}
     if 'H' in extension_list:
       if 32 in inp_yaml['supported_xlen']:
         temp['rv32']['accessible'] = True
       if 64 in inp_yaml['supported_xlen']:
         temp['rv64']['accessible'] = True
     return temp
-    
+
 def sregseth():
     '''Function to set defaults based on presence of 'S' extension.'''
     global inp_yaml
     global extension_list
     temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}}
     if 'S' in extension_list:
       if 32 in inp_yaml['supported_xlen']:
@@ -268,81 +287,83 @@
     global inp_yaml
     temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}}
     if 32 in inp_yaml['supported_xlen']:
         temp['rv32']['accessible'] = True
     if 64 in inp_yaml['supported_xlen']:
         temp['rv64']['accessible'] = True
     return temp
-    
+
 def pmpregset():
     global inp_yaml
-    temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}} 
-    return temp    
+    temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}}
+    return temp
 
 def pmpregseth():
     global inp_yaml
     temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}}
     return temp
-    
+
 def counterhset():
     global inp_yaml
     temp = {'rv32': {'accessible': False}, 'rv64': {'accessible': False}}
     if 32 in inp_yaml['supported_xlen']:
         temp['rv32']['accessible'] = True
     return temp
 
 def add_debug_setters(schema_yaml):
     '''Function to set the default setters for various fields in the debug schema'''
     regsetter = lambda doc: regset()
-    
+
     tselectregsetter = lambda doc: pmpregset()
     schema_yaml['dcsr']['default_setter'] = regsetter
     schema_yaml['tselect']['default_setter'] = tselectregsetter
     schema_yaml['tinfo']['default_setter'] = tselectregsetter
     schema_yaml['hcontext']['default_setter'] = tselectregsetter
     schema_yaml['tdata1']['default_setter'] = tselectregsetter
     schema_yaml['tdata2']['default_setter'] = tselectregsetter
     schema_yaml['tdata3']['default_setter'] = tselectregsetter
     schema_yaml['tcontrol']['default_setter'] = tselectregsetter
     schema_yaml['scontext']['default_setter'] = tselectregsetter
     return schema_yaml
-    
+
 def add_reset_setters(schema_yaml):
     '''Function to set the default setters for extension  subfields in the misa'''
     global inp_yaml
     global extensions
     xlen=inp_yaml['supported_xlen'][0]
     rvxlen='rv'+str(xlen)
     extensions=hex(int(format(reset(), '#0{}b'.format(xlen+2))[(xlen-24):(xlen+2)], 2))
     schema_yaml['misa']['schema'][rvxlen]['schema']['extensions']['schema']['type']['default']['warl']['legal'][0]=schema_yaml['misa']['schema'][rvxlen]['schema']['extensions']['schema']['type']['default']['warl']['legal'][0].replace('0x3FFFFFFF', extensions)
     return schema_yaml
-    
+
 def add_fflags_type_setters(schema_yaml):
     global inp_yaml
     global extension_list
     xlen=inp_yaml['supported_xlen'][0]
     rvxlen='rv'+str(xlen)
     if 'F' not in extension_list:
         schema_yaml['fcsr']['schema'][rvxlen]['schema']['frm']['schema']['type']['default'] = {'ro_constant': 0}
         schema_yaml['fcsr']['schema'][rvxlen]['schema']['fflags']['schema']['type']['default'] = {'ro_constant': 0}
     return schema_yaml
-    
+
 def add_def_setters(schema_yaml):
     '''Function to set the default setters for various fields in the schema'''
     regsetter = lambda doc: regset()
     resetsetter=lambda doc: reset()
     reset_susetter=lambda doc: resetsu()
     reset_vsssetter=lambda doc: reset_vsstatus()
     pmpregsetter = lambda doc: pmpregset()
     counthsetter = lambda doc: counterhset()
     pmpreghsetter = lambda doc: pmpregseth()
     uregsetter = lambda doc: uregset()
+    fregsetter = lambda doc: fregset()
     ureghsetter = lambda doc: uregseth()
     ssetter = lambda doc: sset()
     fssetter = lambda doc: fsset()
+    fsetter = lambda doc: fset()
     sregsetter = lambda doc: sregset()
     nregsetter = lambda doc: nregset()
     hregsetter = lambda doc: hregset()
     hreghsetter = lambda doc: hregseth()
     sregsetterh = lambda doc: sregseth()
     nusetter = lambda doc: nuset()
     usetter = lambda doc: uset()
@@ -448,15 +469,15 @@
         'default_setter'] = ssetter
     schema_yaml['stvec']['schema']['rv64']['schema']['base'][
         'default_setter'] = ssetter
     schema_yaml['stvec']['schema']['rv32']['schema']['mode'][
         'default_setter'] = ssetter
     schema_yaml['stvec']['schema']['rv64']['schema']['mode'][
         'default_setter'] = ssetter
-        
+
     schema_yaml['sepc']['default_setter'] = sregsetter
     schema_yaml['stval']['default_setter'] = sregsetter
     schema_yaml['scause']['default_setter'] = sregsetter
     schema_yaml['scause']['schema']['rv32']['schema']['interrupt'][
         'default_setter'] = ssetter
     schema_yaml['scause']['schema']['rv64']['schema']['interrupt'][
         'default_setter'] = ssetter
@@ -474,15 +495,15 @@
     schema_yaml['satp']['schema']['rv64']['schema']['asid'][
         'default_setter'] = ssetter
     schema_yaml['satp']['schema']['rv32']['schema']['mode'][
         'default_setter'] = ssetter
     schema_yaml['satp']['schema']['rv64']['schema']['mode'][
         'default_setter'] = ssetter
     schema_yaml['sscratch']['default_setter'] = sregsetter
-    
+
     schema_yaml['ustatus']['default_setter'] = nregsetter
     schema_yaml['ustatus']['schema']['rv32']['schema']['uie'][
         'default_setter'] = nusetter
     schema_yaml['ustatus']['schema']['rv64']['schema']['uie'][
         'default_setter'] = nusetter
     schema_yaml['ustatus']['schema']['rv32']['schema']['upie'][
         'default_setter'] = nusetter
@@ -534,28 +555,28 @@
     schema_yaml['ucause']['schema']['rv32']['schema']['exception_code'][
         'default_setter'] = nusetter
     schema_yaml['ucause']['schema']['rv64']['schema']['exception_code'][
         'default_setter'] = nusetter
     schema_yaml['uscratch']['default_setter'] = nregsetter
 
     schema_yaml['fcsr']['schema']['rv32']['schema']['frm'][
-        'default_setter'] = usetter
+        'default_setter'] = fsetter
     schema_yaml['fcsr']['schema']['rv64']['schema']['frm'][
-        'default_setter'] = usetter
+        'default_setter'] = fsetter
     schema_yaml['fcsr']['schema']['rv32']['schema']['fflags'][
-        'default_setter'] = usetter
+        'default_setter'] = fsetter
     schema_yaml['fcsr']['schema']['rv64']['schema']['fflags'][
-        'default_setter'] = usetter
+        'default_setter'] = fsetter
 
     schema_yaml['misa']['default_setter'] = regsetter
     schema_yaml['misa']['schema']['reset-val']['default_setter'] = resetsetter
     schema_yaml['mstatus']['default_setter'] = regsetter
     schema_yaml['mstatus']['schema']['reset-val']['default_setter']=reset_susetter
     schema_yaml['vsstatus']['schema']['reset-val']['default_setter']=reset_vsssetter
-    schema_yaml['mstatush']['default_setter'] = counthsetter   
+    schema_yaml['mstatush']['default_setter'] = counthsetter
     schema_yaml['mvendorid']['default_setter'] = regsetter
     schema_yaml['mimpid']['default_setter'] = regsetter
     schema_yaml['marchid']['default_setter'] = regsetter
     schema_yaml['mhartid']['default_setter'] = regsetter
     schema_yaml['mtvec']['default_setter'] = regsetter
     schema_yaml['mip']['default_setter'] = regsetter
     schema_yaml['mie']['default_setter'] = regsetter
@@ -814,17 +835,17 @@
 
     schema_yaml['mstatus']['schema']['rv32']['schema']['mprv'][
         'default_setter'] = ssetter
     schema_yaml['mstatus']['schema']['rv64']['schema']['mprv'][
         'default_setter'] = ssetter
     schema_yaml['mstatus']['schema']['rv64']['schema']['uxl'][
         'default_setter'] = usetter
-    schema_yaml['fflags']['default_setter'] = uregsetter
-    schema_yaml['frm']['default_setter'] = uregsetter
-    schema_yaml['fcsr']['default_setter'] = uregsetter
+    schema_yaml['fflags']['default_setter'] = fregsetter
+    schema_yaml['frm']['default_setter'] = fregsetter
+    schema_yaml['fcsr']['default_setter'] = fregsetter
     schema_yaml['time']['default_setter'] = uregsetter
     schema_yaml['timeh']['default_setter'] = ureghsetter
     schema_yaml['cycle']['default_setter'] = uregsetter
     schema_yaml['cycleh']['default_setter'] = ureghsetter
     schema_yaml['instret']['default_setter'] = uregsetter
     schema_yaml['instreth']['default_setter'] = ureghsetter
 
@@ -943,15 +964,15 @@
         'default_setter'] = ssetter
     schema_yaml['mie']['schema']['rv64']['schema']['vseie'][
         'default_setter'] = ssetter
     schema_yaml['mie']['schema']['rv32']['schema']['sgeie'][
         'default_setter'] = hsetter
     schema_yaml['mie']['schema']['rv64']['schema']['sgeie'][
         'default_setter'] = hsetter
-                
+
     schema_yaml['mstatus']['schema']['rv32']['schema']['tw'][
         'default_setter'] = twsetter
     schema_yaml['mstatus']['schema']['rv64']['schema']['tw'][
         'default_setter'] = twsetter
     schema_yaml['mstatush']['schema']['rv32']['schema']['gva'][
         'default_setter'] = hsetter
     schema_yaml['mstatus']['schema']['rv64']['schema']['gva'][
@@ -960,15 +981,15 @@
         'default_setter'] = hsetter
     schema_yaml['mstatus']['schema']['rv64']['schema']['mpv'][
         'default_setter'] = hsetter
     schema_yaml['medeleg']['default_setter'] = delegsetter
     schema_yaml['mideleg']['default_setter'] = delegsetter
     schema_yaml['sedeleg']['default_setter'] = nregsetter
     schema_yaml['sideleg']['default_setter'] = nregsetter
-    
+
     schema_yaml['hstatus']['schema']['rv32']['schema']['gva'][
         'default_setter'] = hsetter
     schema_yaml['hstatus']['schema']['rv64']['schema']['gva'][
         'default_setter'] = hsetter
     schema_yaml['hstatus']['schema']['rv32']['schema']['spv'][
         'default_setter'] = hsetter
     schema_yaml['hstatus']['schema']['rv64']['schema']['spv'][
@@ -977,39 +998,39 @@
         'default_setter'] = hsetter
     schema_yaml['hstatus']['schema']['rv64']['schema']['spvp'][
         'default_setter'] = hsetter
     schema_yaml['hstatus']['schema']['rv32']['schema']['hu'][
         'default_setter'] = hsetter
     schema_yaml['hstatus']['schema']['rv64']['schema']['hu'][
         'default_setter'] = hsetter
-    
+
     schema_yaml['hstatus']['default_setter'] = hregsetter
     schema_yaml['hedeleg']['default_setter'] = hregsetter
     schema_yaml['hideleg']['default_setter'] = hregsetter
     schema_yaml['hie']['default_setter'] = hregsetter
     schema_yaml['hip']['default_setter'] = hregsetter
     schema_yaml['hvip']['default_setter'] = hregsetter
     schema_yaml['hgeip']['default_setter'] = hregsetter
     schema_yaml['hgeie']['default_setter'] = hregsetter
     schema_yaml['htval']['default_setter'] = hregsetter
     schema_yaml['htinst']['default_setter'] = hregsetter
     schema_yaml['hgatp']['default_setter'] = hregsetter
     schema_yaml['htimedelta']['default_setter'] = hregsetter
     schema_yaml['htimedeltah']['default_setter'] = hreghsetter
     schema_yaml['hcounteren']['default_setter'] = hregsetter
-    
+
     schema_yaml['hie']['schema']['rv32']['schema']['sgeie'][
         'default_setter'] = hsetter
     schema_yaml['hie']['schema']['rv64']['schema']['sgeie'][
         'default_setter'] = hsetter
     schema_yaml['hip']['schema']['rv32']['schema']['sgeip'][
         'default_setter'] = hsetter
     schema_yaml['hip']['schema']['rv64']['schema']['sgeip'][
         'default_setter'] = hsetter
-    
+
     schema_yaml['vsstatus']['default_setter'] = sregsetter
     schema_yaml['vsstatus']['schema']['rv32']['schema']['uie'][
         'default_setter'] = nusetter
     schema_yaml['vsstatus']['schema']['rv64']['schema']['uie'][
         'default_setter'] = nusetter
     schema_yaml['vsstatus']['schema']['rv32']['schema']['upie'][
         'default_setter'] = nusetter
@@ -1161,79 +1182,79 @@
             if csrnode['rv32']['accessible']:
                 csrnode['rv32']['fields'] = get_fields(
                     csrnode['rv32'], 32)
             if csrnode['rv64']['accessible']:
                 csrnode['rv64']['fields'] = get_fields(
                     csrnode['rv64'], 64)
     return spec
-        
+
 def check_fields(spec):
-    errors = {} 
+    errors = {}
     for csr, node, in spec.items() :
          fault_node = node
          error=[]
          if csr.startswith('uarch_'):
              continue
          if node['rv32']['accessible']:
                 node['rv32']['fields'] = get_fields(node['rv32'], 32)
          if node['rv64']['accessible']:
                 node['rv64']['fields'] = get_fields(node['rv64'], 64)
          fields = list(set(['rv32', 'rv64', 'description', 'address', 'priv_mode', 'reset-val']) - set(node.keys()) )
          if fields:
             error.append("The fields " + "".join(fields) + " are missing")
          if node['rv32']['accessible']:
-            if any(type(e)==list for e in node['rv32']['fields']): 
+            if any(type(e)==list for e in node['rv32']['fields']):
              sub_fields = node['rv32']['fields'][:-1]
             else:
              sub_fields = node['rv32']['fields']
             if not sub_fields :
-             subfields = list(set(['msb', 'lsb', 'accessible', 'shadow', 'shadow_type', 'fields', 'type']) - set(node['rv32'].keys()) )    
+             subfields = list(set(['msb', 'lsb', 'accessible', 'shadow', 'shadow_type', 'fields', 'type']) - set(node['rv32'].keys()) )
              if subfields:
-                error.append("The subfield " + "".join(subfields) + " are not present")         
+                error.append("The subfield " + "".join(subfields) + " are not present")
             else:
               for x in sub_fields :
                 subfields = list(set(['msb', 'lsb', 'implemented', 'description', 'shadow', 'shadow_type', 'type']) - set(node['rv32'][x].keys()) )
-                if subfields :                   
+                if subfields :
                    error.append("The subfields " + "".join(subfields) + " are not present in " + str(x))
-         if node['rv64']['accessible']:            
-            if any(type(e)==list for e in node['rv64']['fields']): 
+         if node['rv64']['accessible']:
+            if any(type(e)==list for e in node['rv64']['fields']):
              sub_fields = node['rv64']['fields'][:-1]
             else:
              sub_fields = node['rv64']['fields']
             if not sub_fields :
              subfields = list(set(['msb', 'lsb', 'accessible', 'fields', 'shadow', 'shadow_type', 'type']) - set(node['rv64'].keys()))
              if subfields:
                 error.append("The subfield " + "".join(subfields) + " are not present")
             else:
               for x in sub_fields :
                 subfields = list(set(['msb', 'lsb', 'implemented', 'description', 'shadow', 'shadow_type', 'type']) - set(node['rv64'][x].keys()) )
-                if subfields :                   
+                if subfields :
                    error.append("The subfields " + "".join(subfields) + " are not present in " + str(x))
          if bin(node['address'])[2:][::-1][6:8] != '11' and bin(node['address'])[2:][::-1][8:12] != '0001':
              error.append('Address is not in custom csr ranges')
          if (bin(node['address'])[2:][::-1][8:10] == '00' and node['priv_mode'] != 'U' ) or (bin(node['address'])[2:][::-1][8:10] == '01' and node['priv_mode'] != 'S' ) or (bin(node['address'])[2:][::-1][8:10] == '11' and node['priv_mode'] != 'M') :
             error.append('Privilege does not match with the address')
          if error:
             errors[csr] = error
-    return errors 
+    return errors
 def check_shadows(spec, logging = False):
     ''' Check if the shadowed fields are implemented and of the same size as the
     source'''
     errors = {}
     _rvxlen = ['rv32', 'rv64']
     for csr, content in spec.items():
         if logging:
             logger.debug('Checking Shadows for ' + csr)
         error = []
         if isinstance(content, dict) and 'description' in content:
             if 'indexing_reg' in content:
                 continue
             for rvxlen in _rvxlen:
                 if content[rvxlen]['accessible'] and not content[rvxlen]['fields']:
-                    if content[rvxlen]['shadow'] is None: 
+                    if content[rvxlen]['shadow'] is None:
                         continue
                     else:
                         shadow = content[rvxlen]['shadow'].split('.')
                         if len(shadow) > 2:
                             error.append('Shadow field of should only up to 1 dot')
                             continue
                         elif len(shadow) == 2:
@@ -1255,15 +1276,15 @@
                             if not spec[scsr][rvxlen]['accessible']:
                                 error.append('Shadow field ' + scsr + ' not implemented')
                                 continue
                             scsr_size = spec[scsr][rvxlen]['msb'] - spec[scsr][rvxlen]['lsb']
                             csr_size = spec[csr][rvxlen]['msb'] - spec[csr][rvxlen]['lsb']
                             if scsr_size != csr_size :
                                 error.append('Shadow field '+ scsr +\
-                                        'does not match in size') 
+                                        'does not match in size')
                 elif content[rvxlen]['accessible']:
                     for subfield in content[rvxlen]['fields']:
                         if isinstance(subfield ,list):
                             continue
                         if content[rvxlen][subfield]['shadow'] is None:
                            continue
                         elif content[rvxlen][subfield]['implemented']:
@@ -1294,15 +1315,15 @@
                                 scsr_size = spec[scsr][rvxlen][subscsr]['msb'] -\
                                         spec[scsr][rvxlen][subscsr]['lsb']
                                 csr_size = spec[csr][rvxlen][subfield]['msb'] -\
                                         spec[csr][rvxlen][subfield]['lsb']
                                 if scsr_size != csr_size :
                                     error.append('Subfield ' + subfield +'shadowing'+ \
                                             scsr + '.' + subscsr + \
-                                            ' does not match in size') 
+                                            ' does not match in size')
 
         if error:
             errors[csr] = error
     return errors
 
 def check_mhpm(spec, logging = False):
     ''' Check if the mhpmcounters and corresponding mhpmevents are implemented and of the same size as the
@@ -1328,15 +1349,15 @@
                     error.append(csrname + " event reg doesn't have the corresponding mhpmcounter register accessible")
             if content['rv32']['accessible'] :
                 if not spec['mhpmcounter'+str(index)+'h']['rv32']['accessible']:
                     error.append(csrname + " event reg doesn't have the corresponding mhpmcounter 'h' counterpart register accessible")
         if error:
             errors[csrname] = error
     return errors
-   
+
 def check_supervisor(spec, logging=False):
     ''' this function includes several supervisor related checks:
 
     - check if pte_ad_hw_update is True, then satp.mode should be able to take
       one of the possible virtualization modes
     '''
     errors = {}
@@ -1370,28 +1391,28 @@
                 virtualization_possible = True
                 break
 
     if pte_ad_hw_update and not virtualization_possible:
         errors['pte_ad_hw_update'] = ['pte_ad_hw_update should be True only if satp.mode can be \
 set to one of the legal virtualization modes']
     return errors
-        
-    
-     
+
+
+
 def check_pmp(spec, logging = False):
     ''' Check if the pmp csrs are implemented correctly as per spec. The
     following checks are performed:
 
         - the number of accessible pmpaddr csrs must be 0, 16 or 64
         - the number of implemented pmpcfg csrs must be 0, 16 or 64
         - the pmpaddr and pmpcfgs must be implemented implemented from the
           lowest numbered indices and be contiguous
-        - the number of accessible pmpaddr csrs and the implemented pmpcfg csrs 
+        - the number of accessible pmpaddr csrs and the implemented pmpcfg csrs
           must be the same
-        - for each accesible pmpaddr csr the corresponding pmpcfg csr must be 
+        - for each accesible pmpaddr csr the corresponding pmpcfg csr must be
           implemented
         - reset values of the accessible pmpaddr csrs must be coherent with the
           pmp_granularity field.
     '''
     logger.info('Performing Checks on PMP CSRs')
     errors = {}
     isa = 'rv32' if '32' in spec['ISA'] else 'rv64'
@@ -1427,35 +1448,35 @@
 must be 0, 16 or 64. But found {pmpaddr_count}']
     if pmpcfg_count not in [0, 16, 64]:
         errors["PMP-CFG"] = [f'The number of implemented PMP*CGF registers \
 must be 0, 16 or 64. But found {pmpcfg_count}']
     if pmpcfg_count != pmpaddr_count:
         errors["PMP"] = [f' the number of pmpaddr* csrs [{pmpaddr_count}]and \
 pmp*cfg registers [{pmpcfg_count}] do not match']
-        
+
     for csrname, content, in spec.items():
         error = []
         Grain=int(spec['pmp_granularity'])
         if 'pmpaddr' in csrname:
             index = int(re.findall('\d+',csrname.lower())[0])
-            if content['rv64']['accessible'] :                
-                reset_val_addr = (bin(content['reset-val'])[2:].zfill(64))[::-1] 
+            if content['rv64']['accessible'] :
+                reset_val_addr = (bin(content['reset-val'])[2:].zfill(64))[::-1]
                 reset_val_cfg  = (bin(spec['pmpcfg'+str(int(int(index/8)*2))]['reset-val'])[2:].zfill(64))[::-1]
                 if not spec['pmpcfg'+str(int(int(index/8)*2))]['rv64']['accessible']:
                     error.append(csrname + " addr doesn't have the corresponding pmp config register accessible")
                 if not spec['pmpcfg'+str(int(int(index/8)*2))]['rv64']['pmp'+str(index)+'cfg']['implemented'] :
                     error.append(csrname + " addr doesn't have the corresponding pmpcfg" +str(int(index/4)) + "_pmp" + str(index) +"cfg register implemented")
                 if reset_val_cfg[8*(index-(int(index/8)*8)) + 4] == '1' and Grain >=2 :     #NAPOT, Bit A of pmpXcfg is set
                   if '0' in reset_val_addr[0:(Grain-1)] or (reset_val_addr[Grain-1] != '0') :
                     error.append(csrname + 'reset value does not adhere with the pmp granularity')
                 elif Grain >= 1: #TOR
                   if int(content['reset-val']) % (2**Grain) != 0 :
                     error.append(csrname + 'reset value does not adhere with the pmp granularity')
             if content['rv32']['accessible'] :
-                reset_val_addr = (bin(content['reset-val'])[2:].zfill(32))[::-1] 
+                reset_val_addr = (bin(content['reset-val'])[2:].zfill(32))[::-1]
                 reset_val_cfg  = (bin(spec['pmpcfg'+str(int(index/4))]['reset-val'])[2:].zfill(32))[::-1]
                 if not spec['pmpcfg'+str(int(index/4))]['rv32']['accessible']:
                     error.append(csrname + " addr doesn't have the corresponding pmp config register accessible")
                 if not spec['pmpcfg'+str(int(index/4))]['rv32']['pmp'+str(index)+'cfg']['implemented'] :
                     error.append(csrname + " addr doesn't have the corresponding pmpcfg" +str(int(index/4)) + "_pmp" + str(index) +"cfg register implemented")
                 if reset_val_cfg[8*(index-(int(index/4)*4)) + 4] == '1' and Grain >=2 :     #NAPOT, Bit A of pmpXcfg is set
                  if '0' in reset_val_addr[0:(Grain-1)] or (reset_val_addr[Grain-1] != '0') :
@@ -1519,15 +1540,15 @@
         err = []
         warl_inst = warl_class(node['warl'], csrname, node['msb'],node['lsb'], spec)
         err_f = warl_inst.iserr()
         if err_f:
             errors[csrname] = err_f
 
     return errors
-                
+
 def check_reset(spec, logging=False):
     errors = {}
     resetnodes = {}
     xlen = 64 if 64 in spec['supported_xlen'] else 32
     for csrname, csrnode in spec.items():
         if isinstance(csrnode, dict) and 'priv_mode' in csrnode:
             if csrnode[f'rv{xlen}']['accessible']:
@@ -1628,30 +1649,30 @@
                             value_for_indexing_reg = n['index_val']
                             logger.debug(f'--- Checking if index value: {value_for_indexing_reg} is legal for indexing register : {indexing_reg} ')
                             valuenode = {}
                             valuenode['msb'] = spec[indexing_reg][f'rv{xlen}']['msb']
                             valuenode['lsb'] = spec[indexing_reg][f'rv{xlen}']['lsb']
                             valuenode['val'] = value_for_indexing_reg
                             valuenode['type'] = spec[indexing_reg][f'rv{xlen}']['type']
-                            error = check_values_in_type(indexing_reg, valuenode, spec, False) 
+                            error = check_values_in_type(indexing_reg, valuenode, spec, False)
                             if value_for_indexing_reg in index_val_list:
                                 error.append(f'Founding repeating index-val {value_for_indexing_reg} for indexed csr : {csrname}')
                             else:
                                 index_val_list.append(value_for_indexing_reg)
                             if error:
                                 errors[csrname] = error
 
     return errors
 
 def check_triggers(spec, logging):
     error = []
     xlen = 64 if 64 in spec['supported_xlen'] else 32
     indexed_registers = ['tdata1','tinfo','tdata1', 'tdata2', 'tcontrol', 'hcontext', 'scontext']
     ind_prop = {}
-    
+
     for i in indexed_registers:
         ind_prop[i] = {}
         ind_prop[i]['accessible'] = spec[i][f'rv{xlen}']['accessible']
         if ind_prop[i]['accessible']:
             ind_prop[i]['size'] = len(spec[i][f'rv{xlen}']['index_list'])
             ind_prop[i]['index_vals'] = []
             for x in spec[i][f'rv{xlen}']['index_list']:
@@ -1699,15 +1720,15 @@
 
         :return: A tuple with the first entry being the absolute path to normalized isa file
             and the second being the absolute path to the platform spec file.
     '''
 
     if logging:
         logger.info('Input-Debug file')
-    
+
     foo1 = isa_spec
     foo = debug_spec
     schema = constants.debug_schema
     """
       Read the input-isa foo (yaml file) and validate with schema-isa for feature values
       and constraints
     """
@@ -1717,15 +1738,15 @@
     master_inp_debug_yaml = utils.load_yaml(foo, no_anchors)
 
     # Load input YAML file
     if logging:
         logger.info('Loading input isa file: ' + str(foo1))
     master_inp_yaml = utils.load_yaml(foo1, no_anchors)
     isa_string = master_inp_yaml['hart0']['ISA']
-    
+
     # instantiate validator
     if logging:
         logger.info('Load Schema ' + str(schema))
     master_schema_yaml = utils.load_yaml(schema, no_anchors)
 
     outyaml = copy.deepcopy(master_inp_debug_yaml)
     for x in master_inp_debug_yaml['hart_ids']:
@@ -1818,16 +1839,16 @@
 
     outyaml = copy.deepcopy(master_inp_yaml)
     for x in master_inp_yaml['hart_ids']:
         if logging:
             logger.info('Processing Hart: hart'+str(x))
         inp_yaml = master_inp_yaml['hart'+str(x)]
         schema_yaml = add_def_setters(master_schema_yaml['hart_schema']['schema'])
-        schema_yaml = add_reset_setters(master_schema_yaml['hart_schema']['schema']) 
-        schema_yaml = add_fflags_type_setters(master_schema_yaml['hart_schema']['schema']) 
+        schema_yaml = add_reset_setters(master_schema_yaml['hart_schema']['schema'])
+        schema_yaml = add_fflags_type_setters(master_schema_yaml['hart_schema']['schema'])
         #Extract xlen
         xlen = inp_yaml['supported_xlen']
         validator = schemaValidator(schema_yaml, xlen=xlen, isa_string=inp_yaml['ISA'])
         validator.allow_unknown = False
         validator.purge_readonly = True
         normalized = validator.normalized(inp_yaml, schema_yaml)
 
@@ -1882,15 +1903,15 @@
         :return: A tuple with the first entry being the absolute path to normalized isa file
             and the second being the absolute path to the platform spec file.
     '''
     if logging:
         logger.info('Custom CSR Spec')
 
     foo = custom_spec
-    
+
     # Load input YAML file
     if logging:
         logger.info('Loading input file: ' + str(foo))
     master_custom_yaml = utils.load_yaml(foo, no_anchors)
     schema_yaml = utils.load_yaml(constants.custom_schema, no_anchors)
     validator = schemaValidator(schema_yaml, xlen=[])
     validator.allow_unknown = True
@@ -1919,15 +1940,15 @@
         work_dir, file_name_split[0] + '_checked.' + file_name_split[1])
     cfile = output_filename
     outfile = open(output_filename, 'w')
     if logging:
         logger.info('Dumping out Normalized Checked YAML: ' + output_filename)
     utils.dump_yaml(outyaml, outfile, no_anchors )
     return cfile
-    
+
 def check_platform_specs(platform_spec,
                 work_dir,
                 logging=False,
                 no_anchors=False):
     foo = platform_spec
     schema = constants.platform_schema
     if logging:
@@ -2102,8 +2123,8 @@
             errors = check_triggers(csr_db, logging)
         if errors:
             raise ValidationError("Error in csr definitions", errors)
 
         if logging and not errors:
             logger.info(f'All checks completed for hart{entry}. No errors found.')
 
-    return specs_list
+    return specs_list
```

### Comparing `riscv_config-3.9.1/riscv_config/constants.py` & `riscv_config-3.9.2/riscv_config/constants.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.1/riscv_config/errors.py` & `riscv_config-3.9.2/riscv_config/errors.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.1/riscv_config/isa_validator.py` & `riscv_config-3.9.2/riscv_config/isa_validator.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.1/riscv_config/main.py` & `riscv_config-3.9.2/riscv_config/main.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.1/riscv_config/schemaValidator.py` & `riscv_config-3.9.2/riscv_config/schemaValidator.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     def _check_with_smrnmi_check(self, field, value):
       global extension_list
       if value and 'Smrnmi' not in extension_list:
         self._error(field,
                   "Register cannot be implemented without Smrnmi extension in ISA."
               )
 
-    
+
     def _check_with_satp_modes64(self, field, value):
         pass
 
     def _check_with_isa_xlen(self, field, value):
         global supported_xlen
         global isa_string
         if str(max(supported_xlen)) not in isa_string:
@@ -60,14 +60,23 @@
         if value & (value - 1) != 0:
             self._error(field, "Cache block size should be power of 2")
 
     def _check_with_cannot_be_false_rv64(self, field, value):
         ''' Functions ensures that the field cannot be False in rv64 mode'''
         if rv64 and not value:
             self._error(field, "This field cannot be False")
+    def _check_with_cannot_be_false_rv64f(self, field, value):
+        ''' Functions ensures that the field cannot be False in rv64 mode when F is present'''
+        global extension_list
+        if rv64 and 'F' in extension_list and not value:
+            self._error(field, "This field cannot be False")
+    def _check_with_cannot_be_false_rv32f(self, field, value):
+        ''' Functions ensures that the field cannot be False in rv32 mode when F is present'''
+        if rv32 and 'F' in extension_list and not value:
+            self._error(field, "This field cannot be False")
 
     def _check_with_cannot_be_false_rv32(self, field, value):
         ''' Functions ensures that the field cannot be False in rv32 mode'''
         if rv32 and not value:
             self._error(field, "This field cannot be False")
 
     def _check_with_capture_isa_specifics(self, field, value):
@@ -128,15 +137,15 @@
     def _check_with_max_length(self, field, value):
         '''Function to check whether the given value is less than the maximum value that can be stored(2^xlen-1).'''
         global supported_xlen
         global extensions
         maxv = max(supported_xlen)
         if value > (2**maxv) - 1:
             self._error(field, "Value exceeds max supported length")
-    
+
     def _check_with_max_length32(self, field, value):
         '''Function to check whether the given value is less than the maximum value that can be stored(2^xlen-1).'''
         maxv = 32
         if value > (2**maxv) - 1:
             self._error(field, "Value exceeds max supported length")
 
     def _check_with_xtveccheck(self, field, value):
@@ -186,15 +195,15 @@
             if (mxl[65 - s:66 - s] != '1'):
                 self._error(field, "should not be implemented since S is not present")
 
         elif rv32 and check:
             mxl = format(extensions, '#034b')
             if (mxl[33 - s:34 - s] != '1'):
                 self._error(field, "should not be implemented S is not present")
-    
+
     def _check_with_fs_check(self, field, value):
         f = 5
         s = 18
         check = False
         if 'implemented' in value:
             if value['implemented']:
                 check = True
@@ -207,15 +216,34 @@
             if (mxl[65 - s:66 - s] != '1') and (mxl[65 - f:66 - f] != '1'):
                 self._error(field, "neither S nor F is present")
 
         elif rv32 and check:
             mxl = format(extensions, '#034b')
             if (mxl[33 - s:34 - s] != '1') and (mxl[33 - f:34 - f] != '1'):
                 self._error(field, "neither S nor F is present")
-                
+
+
+    def _check_with_f_check(self, field, value):
+        f = 5
+        check = False
+        if 'implemented' in value:
+            if value['implemented']:
+                check = True
+        if 'accessible' in value:
+            if value['accessible']:
+                check = True
+        if rv64 and check:
+            mxl = format(extensions, '#066b')
+            if (mxl[65 - f:66 - f] != '1'):
+                self._error(field, "should not be implemented since F is not present")
+        elif rv32 and check:
+            mxl = format(extensions, '#034b')
+            if (mxl[33 - f:34 - f] != '1'):
+                self._error(field, "should not be implemented since F is not present")
+
 
     def _check_with_u_check(self, field, value):
         u = 20
         check = False
         if 'implemented' in value:
             if value['implemented']:
                 check = True
@@ -227,26 +255,26 @@
             if (mxl[65 - u:66 - u] != '1'):
                 self._error(field, "should not be implemented since U is not present")
 
         elif rv32 and check:
             mxl = format(extensions, '#034b')
             if (mxl[33 - u:34 - u] != '1'):
                 self._error(field, "should not be implemented since U is not present")
-              
+
     def _check_with_s_debug_check(self, field, value):
         ''' Function ensures that the ro_constant is hardwired to zero when S is present in the ISA string
             Used mainly for debug schema'''
         global extension_list
 
         if 'S' not in extension_list :
           if 'ro_constant' not in value:
               self._error(field, "S is not present to dcsr.v should be ro_constant = 0")
           elif value['ro_constant'] != 0:
                 self._error(field, "S is not present but ro constant is not hardwired to zero")
-                
+
     def _check_with_u_debug_check(self, field, value):
         ''' Function ensures that the ro_constant is hardwired to zero when U is present in the ISA string
             Used mainly for debug schema'''
         global extension_list
 
         if 'U' not in extension_list :
           if value['ro_constant'] != 0:
@@ -268,29 +296,29 @@
             if (mxl[65 - s:66 - s] != '1') and (mxl[65 - u:66 - u] != '1'):
                 self._error(field, "neither S nor U is present")
 
         elif rv32 and check:
             mxl = format(extensions, '#034b')
             if (mxl[33 - s:34 - s] != '1') and (mxl[33 - u:34 - u] != '1'):
                 self._error(field, "neither S nor U is present")
-                
+
     def _check_with_reset_ext(self, field, value):
-        
+
         if rv64:
             mxl = format(extensions, '#066b')
             reset = format(value, '#066b')
             if (mxl[40:66] != reset[40:66] ):
                 self._error(field, "reset value does not match with extensions enabled")
 
         elif rv32 :
             mxl = format(extensions, '#034b')
             reset = format(value, '#034b')
             if (mxl[8:34] != reset[8:34] ):
                 self._error(field, "reset value does not match with extensions enabled")
-                
+
     def _check_with_sn_check(self, field, value):
         s = 18
         n = 13
         check = False
         if 'implemented' in value:
             if value['implemented']:
                 check = True
@@ -409,8 +437,8 @@
             self._error(field,f'[{xlen_str}] Field should be accessible since Zpn is present')
         if not 'Zpn' in extension_list and value[xlen_str]['accessible']:
             self._error(field,f'[{xlen_str}] Field should be accessible only when Zpn is present')
         if not 'Zpn' in extension_list and value[xlen_str]['ov']['implemented']:
             self._error(field, f'[{xlen_str}] Subfield ov should not be implemented since Zpn is not present')
         if 'Zpn' in extension_list and not value[xlen_str]['ov']['implemented']:
             self._error(field, f'[{xlen_str}] Subfield ov should be implemented since Zpn is present in isa')
-            
+
```

### Comparing `riscv_config-3.9.1/riscv_config/schemas/schema_custom.yaml` & `riscv_config-3.9.2/riscv_config/schemas/schema_custom.yaml`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.1/riscv_config/schemas/schema_debug.yaml` & `riscv_config-3.9.2/riscv_config/schemas/schema_debug.yaml`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.1/riscv_config/schemas/schema_isa.yaml` & `riscv_config-3.9.2/riscv_config/schemas/schema_isa.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -6059,27 +6059,27 @@
           type: dict
           schema:
             fields: {type: list, default: []}
             shadow: {type: string, default: fcsr.fflags, nullable: True}
             shadow_type: {type: string, default: rw, nullable: True, allowed: ['rw','ro']}
             msb: {type: integer, default: 4, allowed: [4]}
             lsb: {type: integer, default: 0, allowed: [0]}
-            accessible: {type: boolean, default: true, check_with: [rv32_check]}
-          check_with: u_check
+            accessible: {type: boolean, default: true, check_with: [rv32_check,cannot_be_false_rv32f]}
+          check_with: f_check
           default: {accessible: False}
         rv64:
           type: dict
           schema:
             fields: {type: list, default: []}
             shadow: {type: string, default: fcsr.fflags, nullable: True}
             shadow_type: {type: string, default: rw, nullable: True, allowed: ['rw','ro']}
             msb: {type: integer, default: 4, allowed: [4]}
             lsb: {type: integer, default: 0, allowed: [0]}
-            accessible: {default: true, check_with: [rv64_check]}
-          check_with: u_check
+            accessible: {default: true, check_with: [rv64_check,cannot_be_false_rv64f]}
+          check_with: f_check
           default: {accessible: False}
     frm:
       type: dict
       schema:
         description:
           type: string
           default: 32-bit register to hold Floating-Point Dynamic Rounding Mode.
@@ -6094,27 +6094,27 @@
           type: dict
           schema:
             fields: {type: list, default: []}
             shadow: {type: string, default: fcsr.frm, nullable: True}
             shadow_type: {type: string, default: rw, nullable: True, allowed: ['rw','ro']}
             msb: {type: integer, default: 2, allowed: [2]}
             lsb: {type: integer, default: 0, allowed: [0]}
-            accessible: {type: boolean, default: true, check_with: [rv32_check]}
-          check_with: u_check
+            accessible: {type: boolean, default: true, check_with: [rv32_check,cannot_be_false_rv32f]}
+          check_with: f_check
           default: {accessible: False}
         rv64:
           type: dict
           schema:
             fields: {type: list, default: []}
             shadow: {type: string, default: fcsr.frm, nullable: True}
             shadow_type: {type: string, default: rw, nullable: True, allowed: ['rw','ro']}
             msb: {type: integer, default: 2, allowed: [2]}
             lsb: {type: integer, default: 0, allowed: [0]}
-            accessible: {default: true, check_with: [rv64_check]}
-          check_with: u_check
+            accessible: {default: true, check_with: [rv64_check,cannot_be_false_rv64f]}
+          check_with: f_check
           default: {accessible: False}
     fcsr:
       type: dict
       schema:
         description:
           type: string
           default: 32-bit register to hold Floating-Point Control and Status Register.
@@ -6171,16 +6171,16 @@
                         - fflags[4:0] in [0x0:0x1F]
                       wr_illegal:
                         - Unchanged
               default: {implemented: true}
             accessible:
               type: boolean
               default: true
-              check_with: rv32_check
-          check_with: u_check
+              check_with: [rv32_check, cannot_be_false_rv32f]
+          check_with: f_check
           default: {accessible: False}
         rv64:
           type: dict
           schema:
             fields: {type: list, default: []}
             frm:
               type: dict
@@ -6224,16 +6224,16 @@
                       legal:
                         - fflags[4:0] in [0x0:0x1F]
                       wr_illegal:
                         - Unchanged
               default: {implemented: true}
             accessible:
               default: true
-              check_with: rv64_check
-          check_with: u_check
+              check_with: [rv64_check,cannot_be_false_rv64f]
+          check_with: f_check
           default: {accessible: False}
     cycle:
       type: dict
       schema:
         description: {type: string, default: Captures the number of cycles executed from an arbitrary point in time.}
         priv_mode: {type: string, default: U, allowed: [U]}
         address: {type: integer, default: 0xC00, allowed: [0xC00]}
```

### Comparing `riscv_config-3.9.1/riscv_config/schemas/schema_platform.yaml` & `riscv_config-3.9.2/riscv_config/schemas/schema_platform.yaml`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.1/riscv_config/utils.py` & `riscv_config-3.9.2/riscv_config/utils.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.1/riscv_config/warl.py` & `riscv_config-3.9.2/riscv_config/warl.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.1/riscv_config.egg-info/PKG-INFO` & `riscv_config-3.9.2/riscv_config.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: riscv-config
-Version: 3.9.1
+Version: 3.9.2
 Summary: RISC-V Configuration Validator
 Home-page: https://github.com/riscv/riscv-config
 Author: InCore Semiconductors Pvt. Ltd.
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: RISCV-Config
         ==============
```

### Comparing `riscv_config-3.9.1/riscv_config.egg-info/SOURCES.txt` & `riscv_config-3.9.2/riscv_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `riscv_config-3.9.1/setup.py` & `riscv_config-3.9.2/setup.py`

 * *Files identical despite different names*

