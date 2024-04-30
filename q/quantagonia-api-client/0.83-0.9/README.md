# Comparing `tmp/quantagonia_api_client-0.83-py3-none-any.whl.zip` & `tmp/quantagonia_api_client-0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,52 +1,24 @@
-Zip file size: 66231 bytes, number of entries: 50
--rw-rw-r--  2.0 unx     2259 b- defN 24-Apr-30 17:28 quantagonia/__init__.py
--rw-rw-r--  2.0 unx      885 b- defN 24-Apr-30 17:28 quantagonia/enums.py
--rw-rw-r--  2.0 unx     7907 b- defN 24-Apr-30 17:28 quantagonia/parameters.py
--rw-rw-r--  2.0 unx      476 b- defN 24-Apr-30 17:28 quantagonia/runner.py
--rw-rw-r--  2.0 unx     3442 b- defN 24-Apr-30 17:28 quantagonia/runner_factory.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-30 17:28 quantagonia/cloud/__init__.py
--rw-rw-r--  2.0 unx    23883 b- defN 24-Apr-30 17:28 quantagonia/cloud/cloud_runner.py
--rw-rw-r--  2.0 unx      961 b- defN 24-Apr-30 17:28 quantagonia/cloud/solver_log.py
--rw-rw-r--  2.0 unx      499 b- defN 24-Apr-30 17:28 quantagonia/cloud/specs_enums.py
--rw-rw-r--  2.0 unx    10885 b- defN 24-Apr-30 17:28 quantagonia/cloud/specs_https_client.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-30 17:28 quantagonia/cloud/dto/__init__.py
--rw-rw-r--  2.0 unx      214 b- defN 24-Apr-30 17:28 quantagonia/cloud/dto/encoder.py
--rw-rw-r--  2.0 unx      462 b- defN 24-Apr-30 17:28 quantagonia/cloud/dto/job.py
--rw-rw-r--  2.0 unx      199 b- defN 24-Apr-30 17:28 quantagonia/cloud/dto/presigned_s3.py
--rw-rw-r--  2.0 unx       50 b- defN 24-Apr-30 17:28 quantagonia/errors/__init__.py
--rw-rw-r--  2.0 unx      160 b- defN 24-Apr-30 17:28 quantagonia/errors/errors.py
--rw-rw-r--  2.0 unx     2438 b- defN 24-Apr-30 17:28 quantagonia/examples/async_qubo.py
--rw-rw-r--  2.0 unx     1906 b- defN 24-Apr-30 17:28 quantagonia/examples/import_dwave_bqm.py
--rw-rw-r--  2.0 unx      620 b- defN 24-Apr-30 17:28 quantagonia/examples/import_pyqubo.py
--rw-rw-r--  2.0 unx     1821 b- defN 24-Apr-30 17:28 quantagonia/examples/import_qiskit_qubo.py
--rw-rw-r--  2.0 unx     1343 b- defN 24-Apr-30 17:28 quantagonia/examples/model_mip.py
--rw-rw-r--  2.0 unx     1376 b- defN 24-Apr-30 17:28 quantagonia/examples/model_qubo.py
--rw-rw-r--  2.0 unx      927 b- defN 24-Apr-30 17:28 quantagonia/examples/solve_ip_as_qubo.py
--rw-rw-r--  2.0 unx      893 b- defN 24-Apr-30 17:28 quantagonia/examples/submit_batched.py
--rw-rw-r--  2.0 unx      644 b- defN 24-Apr-30 17:28 quantagonia/examples/submit_mps.py
--rw-rw-r--  2.0 unx      654 b- defN 24-Apr-30 17:28 quantagonia/examples/submit_qubo.py
--rw-rw-r--  2.0 unx      987 b- defN 24-Apr-30 17:28 quantagonia/examples/submit_qubo_monitored.py
--rw-rw-r--  2.0 unx     1633 b- defN 24-Apr-30 17:28 quantagonia/examples/data/example.mps
--rw-rw-r--  2.0 unx      371 b- defN 24-Apr-30 17:28 quantagonia/examples/data/example.qubo
--rw-rw-r--  2.0 unx    62922 b- defN 24-Apr-30 17:28 quantagonia/examples/data/example_monitor.qubo
--rw-rw-r--  2.0 unx      133 b- defN 24-Apr-30 17:28 quantagonia/examples/data/garbage.mps
--rw-rw-r--  2.0 unx      134 b- defN 24-Apr-30 17:28 quantagonia/examples/data/ip_as_qubo.lp
--rw-rw-r--  2.0 unx       50 b- defN 24-Apr-30 17:28 quantagonia/parser/__init__.py
--rw-rw-r--  2.0 unx     9698 b- defN 24-Apr-30 17:28 quantagonia/parser/log_parser.py
--rw-rw-r--  2.0 unx     1384 b- defN 24-Apr-30 17:28 quantagonia/parser/solution_parser.py
--rw-rw-r--  2.0 unx      314 b- defN 24-Apr-30 17:28 quantagonia/pulp/__init__.py
--rw-rw-r--  2.0 unx     5616 b- defN 24-Apr-30 17:28 quantagonia/pulp/hybrid_solver_api.py
--rw-rw-r--  2.0 unx     1634 b- defN 24-Apr-30 17:28 quantagonia/pulp/qpulp_adapter.py
--rw-rw-r--  2.0 unx      197 b- defN 24-Apr-30 17:28 quantagonia/qubo/__init__.py
--rw-rw-r--  2.0 unx     3100 b- defN 24-Apr-30 17:28 quantagonia/qubo/expression.py
--rw-rw-r--  2.0 unx    19201 b- defN 24-Apr-30 17:28 quantagonia/qubo/model.py
--rw-rw-r--  2.0 unx     6649 b- defN 24-Apr-30 17:28 quantagonia/qubo/overloads.py
--rw-rw-r--  2.0 unx     3070 b- defN 24-Apr-30 17:28 quantagonia/qubo/term.py
--rw-rw-r--  2.0 unx     2352 b- defN 24-Apr-30 17:28 quantagonia/qubo/variable.py
--rwxrwxr-x  2.0 unx    21167 b- defN 24-Apr-30 17:28 quantagonia_api_client-0.83.data/scripts/hybridsolver
--rw-rw-r--  2.0 unx     1460 b- defN 24-Apr-30 17:28 quantagonia_api_client-0.83.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3389 b- defN 24-Apr-30 17:28 quantagonia_api_client-0.83.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-30 17:28 quantagonia_api_client-0.83.dist-info/WHEEL
--rw-rw-r--  2.0 unx       12 b- defN 24-Apr-30 17:28 quantagonia_api_client-0.83.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4490 b- defN 24-Apr-30 17:28 quantagonia_api_client-0.83.dist-info/RECORD
-50 files, 214959 bytes uncompressed, 58965 bytes compressed:  72.6%
+Zip file size: 15540 bytes, number of entries: 22
+-rw-r--r--  2.0 unx        0 b- defN 22-Aug-04 14:14 quantagonia/__init__.py
+-rw-r--r--  2.0 unx      247 b- defN 22-Aug-04 14:14 quantagonia/enums.py
+-rw-r--r--  2.0 unx     8149 b- defN 22-Aug-08 16:42 quantagonia/qubo.py
+-rw-r--r--  2.0 unx      263 b- defN 22-Aug-08 16:42 quantagonia/runner.py
+-rw-r--r--  2.0 unx     1036 b- defN 22-Aug-05 05:36 quantagonia/runner_factory.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Aug-04 14:14 quantagonia/cloud/__init__.py
+-rw-r--r--  2.0 unx     5850 b- defN 22-Aug-08 16:42 quantagonia/cloud/cloud_runner.py
+-rw-r--r--  2.0 unx      948 b- defN 22-Aug-08 16:42 quantagonia/cloud/solver_log.py
+-rw-r--r--  2.0 unx     1918 b- defN 22-Aug-04 14:14 quantagonia/cloud/spec_builder.py
+-rw-r--r--  2.0 unx      318 b- defN 22-Aug-04 14:14 quantagonia/cloud/specs_enums.py
+-rw-r--r--  2.0 unx     3070 b- defN 22-Aug-08 16:42 quantagonia/cloud/specs_https_client.py
+-rw-r--r--  2.0 unx      513 b- defN 22-Aug-04 14:14 quantagonia/cloud/default_specs/cook_GPU.json
+-rw-r--r--  2.0 unx      402 b- defN 22-Aug-04 14:14 quantagonia/cloud/default_specs/fvsdp.json
+-rw-r--r--  2.0 unx      524 b- defN 22-Aug-04 14:14 quantagonia/cloud/default_specs/metropolis_CPU.json
+-rw-r--r--  2.0 unx      314 b- defN 22-Aug-04 14:14 quantagonia/pulp/__init__.py
+-rw-r--r--  2.0 unx     7558 b- defN 22-Aug-04 14:14 quantagonia/pulp/hybrid_solver_api.py
+-rw-r--r--  2.0 unx      521 b- defN 22-Aug-04 14:14 quantagonia/pulp/qpulp_adapter.py
+-rw-r--r--  2.0 unx     1460 b- defN 22-Aug-08 16:42 quantagonia_api_client-0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1545 b- defN 22-Aug-08 16:42 quantagonia_api_client-0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Aug-08 16:42 quantagonia_api_client-0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 22-Aug-08 16:42 quantagonia_api_client-0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1950 b- defN 22-Aug-08 16:42 quantagonia_api_client-0.9.dist-info/RECORD
+22 files, 36690 bytes uncompressed, 12308 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -1,14 +1,14 @@
 Filename: quantagonia/__init__.py
 Comment: 
 
 Filename: quantagonia/enums.py
 Comment: 
 
-Filename: quantagonia/parameters.py
+Filename: quantagonia/qubo.py
 Comment: 
 
 Filename: quantagonia/runner.py
 Comment: 
 
 Filename: quantagonia/runner_factory.py
 Comment: 
@@ -18,134 +18,50 @@
 
 Filename: quantagonia/cloud/cloud_runner.py
 Comment: 
 
 Filename: quantagonia/cloud/solver_log.py
 Comment: 
 
-Filename: quantagonia/cloud/specs_enums.py
-Comment: 
-
-Filename: quantagonia/cloud/specs_https_client.py
-Comment: 
-
-Filename: quantagonia/cloud/dto/__init__.py
-Comment: 
-
-Filename: quantagonia/cloud/dto/encoder.py
-Comment: 
-
-Filename: quantagonia/cloud/dto/job.py
-Comment: 
-
-Filename: quantagonia/cloud/dto/presigned_s3.py
-Comment: 
-
-Filename: quantagonia/errors/__init__.py
-Comment: 
-
-Filename: quantagonia/errors/errors.py
-Comment: 
-
-Filename: quantagonia/examples/async_qubo.py
-Comment: 
-
-Filename: quantagonia/examples/import_dwave_bqm.py
-Comment: 
-
-Filename: quantagonia/examples/import_pyqubo.py
-Comment: 
-
-Filename: quantagonia/examples/import_qiskit_qubo.py
-Comment: 
-
-Filename: quantagonia/examples/model_mip.py
-Comment: 
-
-Filename: quantagonia/examples/model_qubo.py
-Comment: 
-
-Filename: quantagonia/examples/solve_ip_as_qubo.py
+Filename: quantagonia/cloud/spec_builder.py
 Comment: 
 
-Filename: quantagonia/examples/submit_batched.py
-Comment: 
-
-Filename: quantagonia/examples/submit_mps.py
-Comment: 
-
-Filename: quantagonia/examples/submit_qubo.py
-Comment: 
-
-Filename: quantagonia/examples/submit_qubo_monitored.py
-Comment: 
-
-Filename: quantagonia/examples/data/example.mps
-Comment: 
-
-Filename: quantagonia/examples/data/example.qubo
-Comment: 
-
-Filename: quantagonia/examples/data/example_monitor.qubo
-Comment: 
-
-Filename: quantagonia/examples/data/garbage.mps
+Filename: quantagonia/cloud/specs_enums.py
 Comment: 
 
-Filename: quantagonia/examples/data/ip_as_qubo.lp
+Filename: quantagonia/cloud/specs_https_client.py
 Comment: 
 
-Filename: quantagonia/parser/__init__.py
+Filename: quantagonia/cloud/default_specs/cook_GPU.json
 Comment: 
 
-Filename: quantagonia/parser/log_parser.py
+Filename: quantagonia/cloud/default_specs/fvsdp.json
 Comment: 
 
-Filename: quantagonia/parser/solution_parser.py
+Filename: quantagonia/cloud/default_specs/metropolis_CPU.json
 Comment: 
 
 Filename: quantagonia/pulp/__init__.py
 Comment: 
 
 Filename: quantagonia/pulp/hybrid_solver_api.py
 Comment: 
 
 Filename: quantagonia/pulp/qpulp_adapter.py
 Comment: 
 
-Filename: quantagonia/qubo/__init__.py
-Comment: 
-
-Filename: quantagonia/qubo/expression.py
-Comment: 
-
-Filename: quantagonia/qubo/model.py
-Comment: 
-
-Filename: quantagonia/qubo/overloads.py
-Comment: 
-
-Filename: quantagonia/qubo/term.py
-Comment: 
-
-Filename: quantagonia/qubo/variable.py
-Comment: 
-
-Filename: quantagonia_api_client-0.83.data/scripts/hybridsolver
-Comment: 
-
-Filename: quantagonia_api_client-0.83.dist-info/LICENSE
+Filename: quantagonia_api_client-0.9.dist-info/LICENSE
 Comment: 
 
-Filename: quantagonia_api_client-0.83.dist-info/METADATA
+Filename: quantagonia_api_client-0.9.dist-info/METADATA
 Comment: 
 
-Filename: quantagonia_api_client-0.83.dist-info/WHEEL
+Filename: quantagonia_api_client-0.9.dist-info/WHEEL
 Comment: 
 
-Filename: quantagonia_api_client-0.83.dist-info/top_level.txt
+Filename: quantagonia_api_client-0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: quantagonia_api_client-0.83.dist-info/RECORD
+Filename: quantagonia_api_client-0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## quantagonia/__init__.py

```diff
@@ -1,142 +0,0 @@
-00000000: 696d 706f 7274 2069 6d70 6f72 746c 6962  import importlib
-00000010: 2e6d 6574 6164 6174 610a 696d 706f 7274  .metadata.import
-00000020: 2072 6571 7565 7374 730a 696d 706f 7274   requests.import
-00000030: 2077 6172 6e69 6e67 730a 696d 706f 7274   warnings.import
-00000040: 206f 730a 0a23 2073 6574 7570 2077 6172   os..# setup war
-00000050: 6e69 6e67 730a 6465 6620 6375 7374 6f6d  nings.def custom
-00000060: 5f66 6f72 6d61 7477 6172 6e69 6e67 286d  _formatwarning(m
-00000070: 7367 2c20 2a61 7267 732c 202a 2a6b 7761  sg, *args, **kwa
-00000080: 7267 7329 3a0a 2020 2020 2320 6967 6e6f  rgs):.    # igno
-00000090: 7265 2065 7665 7279 7468 696e 6720 6578  re everything ex
-000000a0: 6365 7074 2074 6865 206d 6573 7361 6765  cept the message
-000000b0: 0a20 2020 2072 6574 7572 6e20 7374 7228  .    return str(
-000000c0: 6d73 6729 202b 2027 5c6e 270a 7761 726e  msg) + '\n'.warn
-000000d0: 696e 6773 2e66 6f72 6d61 7477 6172 6e69  ings.formatwarni
-000000e0: 6e67 203d 2063 7573 746f 6d5f 666f 726d  ng = custom_form
-000000f0: 6174 7761 726e 696e 670a 0a64 6566 2076  atwarning..def v
-00000100: 6572 7369 6f6e 5f63 6f6d 7061 7469 626c  ersion_compatibl
-00000110: 6528 293a 0a20 2020 2022 2222 4368 6563  e():.    """Chec
-00000120: 6b20 6966 2069 6e73 7461 6c6c 6564 2063  k if installed c
-00000130: 6c69 656e 7420 7665 7273 696f 6e20 6973  lient version is
-00000140: 2063 6f6d 7061 7469 626c 6520 746f 2073   compatible to s
-00000150: 6572 7665 722e 2222 220a 2020 2020 7472  erver.""".    tr
-00000160: 793a 0a20 2020 2020 2020 2023 2071 7565  y:.        # que
-00000170: 7279 206c 6174 6573 7420 7665 7273 696f  ry latest versio
-00000180: 6e20 6672 6f6d 2070 7970 690a 2020 2020  n from pypi.    
-00000190: 2020 2020 7061 636b 6167 653d 2271 7561      package="qua
-000001a0: 6e74 6167 6f6e 6961 2d61 7069 2d63 6c69  ntagonia-api-cli
-000001b0: 656e 7422 0a20 2020 2020 2020 2072 6573  ent".        res
-000001c0: 706f 6e73 6520 3d20 7265 7175 6573 7473  ponse = requests
-000001d0: 2e67 6574 2866 2268 7474 7073 3a2f 2f61  .get(f"https://a
-000001e0: 7069 2e71 7561 6e74 6167 6f6e 6961 2e63  pi.quantagonia.c
-000001f0: 6f6d 2f63 6865 636b 636c 6965 6e74 7665  om/checkclientve
-00000200: 7273 696f 6e22 2c0a 2020 2020 2020 2020  rsion",.        
-00000210: 2020 2020 7469 6d65 6f75 743d 312c 2070      timeout=1, p
-00000220: 6172 616d 733d 7b0a 2020 2020 2020 2020  arams={.        
-00000230: 2020 2020 2020 2020 2276 6572 7369 6f6e          "version
-00000240: 2220 3a20 7374 7228 5f5f 7665 7273 696f  " : str(__versio
-00000250: 6e5f 5f29 2c0a 2020 2020 2020 2020 2020  n__),.          
-00000260: 2020 2020 2020 226c 616e 6775 6167 6522        "language"
-00000270: 203a 2022 5059 5448 4f4e 220a 2020 2020   : "PYTHON".    
-00000280: 2020 2020 2020 2020 7d29 0a0a 2020 2020          })..    
-00000290: 2020 2020 6973 5f6c 6174 6573 7420 3d20      is_latest = 
-000002a0: 626f 6f6c 2872 6573 706f 6e73 652e 6a73  bool(response.js
-000002b0: 6f6e 2829 5b22 6973 5f6c 6174 6573 7422  on()["is_latest"
-000002c0: 5d29 0a20 2020 2020 2020 2069 735f 7375  ]).        is_su
-000002d0: 7070 6f72 7465 6420 3d20 626f 6f6c 2872  pported = bool(r
-000002e0: 6573 706f 6e73 652e 6a73 6f6e 2829 5b22  esponse.json()["
-000002f0: 6973 5f73 7570 706f 7274 6564 225d 290a  is_supported"]).
-00000300: 0a20 2020 2020 2020 206c 6174 6573 745f  .        latest_
-00000310: 7665 7273 696f 6e20 3d20 7265 7370 6f6e  version = respon
-00000320: 7365 2e6a 736f 6e28 295b 226c 6174 6573  se.json()["lates
-00000330: 7422 5d0a 2020 2020 2020 2020 6272 6561  t"].        brea
-00000340: 6b69 6e67 5f76 6572 7369 6f6e 203d 2072  king_version = r
-00000350: 6573 706f 6e73 652e 6a73 6f6e 2829 5b22  esponse.json()["
-00000360: 6c61 7465 7374 5f62 7265 616b 696e 6722  latest_breaking"
-00000370: 5d0a 0a0a 2020 2020 2020 2020 2320 7468  ]...        # th
-00000380: 726f 7720 6572 726f 7220 6966 2069 6e73  row error if ins
-00000390: 7461 6c6c 6564 2076 6572 7369 6f6e 206e  talled version n
-000003a0: 6f74 2063 6f6d 7061 7469 626c 650a 2020  ot compatible.  
-000003b0: 2020 2020 2020 6966 206e 6f74 2069 735f        if not is_
-000003c0: 7375 7070 6f72 7465 643a 0a20 2020 2020  supported:.     
-000003d0: 2020 2020 2020 206d 7367 203d 2066 2249         msg = f"I
-000003e0: 6e73 7461 6c6c 6564 2076 6572 7369 6f6e  nstalled version
-000003f0: 207b 5f5f 7665 7273 696f 6e5f 5f7d 206f   {__version__} o
-00000400: 6620 7175 616e 7461 676f 6e69 612d 6170  f quantagonia-ap
-00000410: 692d 636c 6965 6e74 2069 7320 6e6f 7420  i-client is not 
-00000420: 636f 6d70 6174 6962 6c65 2064 7565 2074  compatible due t
-00000430: 6f20 6272 6561 6b69 6e67 2063 6861 6e67  o breaking chang
-00000440: 6573 2069 6e20 7665 7273 696f 6e20 7b62  es in version {b
-00000450: 7265 616b 696e 675f 7665 7273 696f 6e7d  reaking_version}
-00000460: 2e20 220a 2020 2020 2020 2020 2020 2020  . ".            
-00000470: 6d73 6720 2b3d 2066 2250 6c65 6173 6520  msg += f"Please 
-00000480: 7570 6461 7465 2074 6f20 7468 6520 6c61  update to the la
-00000490: 7465 7374 2076 6572 7369 6f6e 207b 6c61  test version {la
-000004a0: 7465 7374 5f76 6572 7369 6f6e 7d2e 220a  test_version}.".
-000004b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000004c0: 7572 6e20 4661 6c73 652c 206d 7367 0a0a  urn False, msg..
-000004d0: 2020 2020 2020 2020 2320 7072 696e 7420          # print 
-000004e0: 7761 726e 696e 6720 6966 2075 7064 6174  warning if updat
-000004f0: 6520 6176 6169 6c61 626c 650a 2020 2020  e available.    
-00000500: 2020 2020 656c 6966 206e 6f74 2069 735f      elif not is_
-00000510: 6c61 7465 7374 3a0a 2020 2020 2020 2020  latest:.        
-00000520: 2020 2020 6d73 6720 3d20 6622 5741 524e      msg = f"WARN
-00000530: 494e 473a 2022 0a20 2020 2020 2020 2020  ING: ".         
-00000540: 2020 206d 7367 202b 3d20 6622 496e 7374     msg += f"Inst
-00000550: 616c 6c65 6420 7665 7273 696f 6e20 7b5f  alled version {_
-00000560: 5f76 6572 7369 6f6e 5f5f 7d20 6f66 2071  _version__} of q
-00000570: 7561 6e74 6167 6f6e 6961 2d61 7069 2d63  uantagonia-api-c
-00000580: 6c69 656e 7420 6973 206f 7574 6461 7465  lient is outdate
-00000590: 642e 2022 0a20 2020 2020 2020 2020 2020  d. ".           
-000005a0: 206d 7367 202b 3d20 6622 436f 6e73 6964   msg += f"Consid
-000005b0: 6572 2075 7064 6174 696e 6720 746f 2074  er updating to t
-000005c0: 6865 206c 6174 6573 7420 7665 7273 696f  he latest versio
-000005d0: 6e20 7b6c 6174 6573 745f 7665 7273 696f  n {latest_versio
-000005e0: 6e7d 2e22 0a0a 2020 2020 2020 2020 2020  n}."..          
-000005f0: 2020 7265 7475 726e 2054 7275 652c 206d    return True, m
-00000600: 7367 0a20 2020 2020 2020 2023 206e 6f20  sg.        # no 
-00000610: 7761 726e 696e 672c 2069 6620 6c61 7465  warning, if late
-00000620: 7374 2076 6572 7369 6f6e 0a20 2020 2020  st version.     
-00000630: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00000640: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00000650: 2c20 2222 0a0a 2020 2020 6578 6365 7074  , ""..    except
-00000660: 3a0a 2020 2020 2020 2020 2320 6361 7463  :.        # catc
-00000670: 6820 616c 6c2c 2074 6865 2063 6865 636b  h all, the check
-00000680: 2066 6f72 2075 7064 6174 6573 2073 686f   for updates sho
-00000690: 756c 6420 6e65 7665 7220 6661 696c 0a20  uld never fail. 
-000006a0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-000006b0: 7565 2c20 2255 6e61 626c 6520 746f 2063  ue, "Unable to c
-000006c0: 6f6c 6c65 6374 206c 6174 6573 7420 7665  ollect latest ve
-000006d0: 7273 696f 6e20 696e 666f 726d 6174 696f  rsion informatio
-000006e0: 6e2c 2073 6b69 7070 696e 6720 6368 6563  n, skipping chec
-000006f0: 6b2e 220a 0a74 7279 3a0a 2020 2020 2320  k."..try:.    # 
-00000700: 736b 6970 2076 6572 7369 6f6e 2063 6865  skip version che
-00000710: 636b 2066 6f72 2064 6576 656c 6f70 6d65  ck for developme
-00000720: 6e74 0a20 2020 2069 6620 2253 4b49 505f  nt.    if "SKIP_
-00000730: 5645 5253 494f 4e5f 4348 4543 4b22 206e  VERSION_CHECK" n
-00000740: 6f74 2069 6e20 6f73 2e65 6e76 6972 6f6e  ot in os.environ
-00000750: 206f 7220 6f73 2e65 6e76 6972 6f6e 5b22   or os.environ["
-00000760: 534b 4950 5f56 4552 5349 4f4e 5f43 4845  SKIP_VERSION_CHE
-00000770: 434b 225d 2021 3d20 2231 223a 0a0a 2020  CK"] != "1":..  
-00000780: 2020 2020 2020 5f5f 7665 7273 696f 6e5f        __version_
-00000790: 5f20 3d20 696d 706f 7274 6c69 622e 6d65  _ = importlib.me
-000007a0: 7461 6461 7461 2e76 6572 7369 6f6e 2822  tadata.version("
-000007b0: 7175 616e 7461 676f 6e69 612d 6170 692d  quantagonia-api-
-000007c0: 636c 6965 6e74 2229 0a20 2020 2020 2020  client").       
-000007d0: 2073 7570 706f 7274 6564 2c20 6d73 6720   supported, msg 
-000007e0: 3d20 7665 7273 696f 6e5f 636f 6d70 6174  = version_compat
-000007f0: 6962 6c65 2829 0a20 2020 2020 2020 2069  ible().        i
-00000800: 6620 6e6f 7420 7375 7070 6f72 7465 643a  f not supported:
-00000810: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00000820: 7365 2049 6d70 6f72 7445 7272 6f72 286d  se ImportError(m
-00000830: 7367 290a 2020 2020 2020 2020 656c 6966  sg).        elif
-00000840: 206d 7367 2021 3d20 2222 3a0a 2020 2020   msg != "":.    
-00000850: 2020 2020 2020 2020 2320 7072 696e 7420          # print 
-00000860: 7761 726e 696e 670a 2020 2020 2020 2020  warning.        
-00000870: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
-00000880: 6e28 6d73 6729 0a0a 6578 6365 7074 3a0a  n(msg)..except:.
-00000890: 2020 2020 5f5f 7665 7273 696f 6e5f 5f20      __version__ 
-000008a0: 3d20 2264 6576 220a 2020 2020 2320 646f  = "dev".    # do
-000008b0: 6e27 7420 6368 6563 6b20 666f 7220 7570  n't check for up
-000008c0: 6461 7465 7320 696e 2074 6869 7320 6361  dates in this ca
-000008d0: 7365 0a                                  se.
```

## quantagonia/enums.py

```diff
@@ -1,36 +1,10 @@
 from enum import Enum
 
 class HybridSolverConnectionType(Enum):
 	CLOUD = 0
 	LOCAL = 1
 
-class PlatformVersionEnum(str, Enum):
-    ONE = "1"
-    TWO = "2"
-
 class HybridSolverServers(Enum):
     PROD = "https://api.quantagonia.com"
     STAGING = "https://staging.quantagonia.com"
-    DEV = "https://dev.quantagonia.com"
-    DEV3 = "https://dev3.quantagonia.com"
-    LOCAL = "https://localhost:8088"
-
-class PriorityEnum(str, Enum):
-    HIGH = "high"
-    LOW = "low"
-    MEDIUM = "medium"
-
-class HybridSolverOptSenses(Enum):
-    """
-    An enumeration class representing the optimization senses for the hybrid solver.
-
-    Attributes:
-        MAXIMIZE: Holds a string representing maximization.
-        MINIMIZE: Holds a string representing minimization.
-    """
-    MAXIMIZE = "MAXIMIZE"
-    MINIMIZE = "MINIMIZE"
-
-class HybridSolverProblemType(str, Enum):
-    MIP = "MIP"
-    QUBO = "QUBO"
+    DEV = "https://dev.quantagonia.com"
```

## quantagonia/runner.py

```diff
@@ -5,17 +5,9 @@
 class Runner(ABC):
 
   @abstractmethod
   def solve(self, problem_file: str, spec: dict, **kwargs):
     pass
 
   @abstractmethod
-  def solveBatched(self, problem_file: list, specs: list, **kwargs):
-    pass
-
-  @abstractmethod
-  async def solveAsync(self, problem_files: str, spec: dict, **kwargs):
-    pass
-
-  @abstractmethod
-  async def solveBatchedAsync(self, problem_files: list, specs: list, **kwargs):
+  def solveAsync(self, problem_file: str, spec: dict, **kwargs):
     pass
```

## quantagonia/runner_factory.py

```diff
@@ -1,91 +1,31 @@
+import os, os.path
+from decimal import InvalidOperation
+from enum import Enum
+from multiprocessing import connection
+from sqlite3 import connect
+
 from quantagonia.enums import HybridSolverServers, HybridSolverConnectionType
 from quantagonia.cloud.cloud_runner import CloudRunner
-from quantagonia.runner import Runner
-from quantagonia.parameters import HybridSolverParameters
-
 
 _local_is_there__ = None
 try:
-    from quantagonia.local.local_runner import LocalRunner
-    _local_is_there__ = True
+	from quantagonia.local.local_runner import LocalRunner
+	_local_is_there__ = True
 except ModuleNotFoundError:
-    _local_is_there__ = False
-
+	_local_is_there__ = False
 
-class RunnerSuppresExitWrapper(Runner):
+class RunnerFactory:
 
-    def __init__(self, runner):
-        self.runner = runner
+	@classmethod
+	def getRunner(cls, connection : HybridSolverConnectionType, api_key : str = None, server : HybridSolverServers = HybridSolverServers.PROD, suppress_output : bool = False):
 
-    def solve(self, problem_file: str, params: HybridSolverParameters = None, **kwargs):
-        try:
-            return self.runner.solve(problem_file, params, **kwargs)
-        except SystemExit as e:
-            raise Exception(e)
-
-    def solveBatched(self, problem_files: list, params: list = [], **kwargs):
-        try:
-            return self.runner.solveBatched(problem_files, params, **kwargs)
-        except SystemExit as e:
-            raise Exception(e)
-
-    async def solveAsync(self, problem_file: str, params: HybridSolverParameters = None, **kwargs):
-        try:
-            return self.runner.solve(problem_file, spec, **kwargs)
-        except SystemExit as e:
-            raise Exception(e)
-
-    async def solveBatchedAsync(self, problem_files: list, params: list = [], **kwargs):
-        try:
-            return self.runner.solve(problem_files, specs, **kwargs)
-        except SystemExit as e:
-            raise Exception(e)
+		if connection == HybridSolverConnectionType.CLOUD:
+			return CloudRunner(api_key, server, suppress_output)
 
+		if connection == HybridSolverConnectionType.LOCAL:
+			if _local_is_there__:
+				return LocalRunner(suppress_output)
+			
+			raise InvalidOperation("LocalRunner not supported in packaged version!")
 
-class RunnerFactory:
-    """
-    Creates a Runner instance based on specifications.
-    The Runner is used to submit problem instances for solving.
-    """
-
-    @classmethod
-    def getRunner(
-            cls,
-            connection : HybridSolverConnectionType,
-            api_key : str = None,
-            server : HybridSolverServers = HybridSolverServers.PROD,
-            suppress_output : bool = False,
-            suppress_exitonfailure : bool = False):
-        """
-        Creates and returns a Runner instance based on the provided connection type and optional parameters.
-
-        Args:
-            connection: A HybridSolverConnectionType enum value representing the type of connection to use.
-            api_key: A string containing the Quantagonia API key. Default is None.
-            server: A HybridSolverServers enum value representing the server to use for cloud connections. Default is HybridSolverServers.PROD.
-            suppress_output: A boolean indicating whether to suppress the output when running a job. Default is False.
-
-        Returns:
-            A Runner instance based on the provided connection type and optional parameters.
-
-        Raises:
-            RuntimeError: If unable to instantiate Quantagonia runner.
-    """
-
-        runner = None
-        if connection == HybridSolverConnectionType.CLOUD:
-            if api_key is None or api_key == "":
-                raise RuntimeError("No API key given.")
-            runner = CloudRunner(api_key, server, suppress_output)
-        elif connection == HybridSolverConnectionType.LOCAL:
-            if _local_is_there__:
-                runner = LocalRunner(suppress_output)
-            else:
-                raise RuntimeError("LocalRunner not supported in packaged version!")
-        else:
-            raise RuntimeError("Unable to instantiate Quantagonia runner.")
-
-        if suppress_exitonfailure:
-            return RunnerSuppresExitWrapper(runner)
-        else:
-            return runner
+		raise InvalidOperation("Unable to instantiate Quantagonia runner.")
```

## quantagonia/cloud/cloud_runner.py

```diff
@@ -1,490 +1,150 @@
-import sys
+from io import UnsupportedOperation
+import sys, os
 import asyncio
 from time import sleep
-from yaspin import yaspin
-import uuid
-import pathlib
+from enum import Enum
+
 from quantagonia.cloud.solver_log import SolverLog
 from quantagonia.cloud.specs_https_client import SpecsHTTPSClient, JobStatus
 from quantagonia.cloud.specs_enums import *
 from quantagonia.runner import Runner
-from quantagonia.parameters import HybridSolverParameters
-from quantagonia.enums import HybridSolverServers, HybridSolverProblemType
-from quantagonia.parser.log_parser import SolverLogParser
-from quantagonia.parser.solution_parser import SolutionParser
-
+from quantagonia.enums import HybridSolverServers
 
 class CloudRunner(Runner):
-    """
-    Runner subclass that provides functionality for submitting and solving QUBO and MIP instances to the cloud.
-
-    Args:
-        api_key (str): The API key string used to authenticate with the cloud.
-        server (HybridSolverServers): (optional) The 'HybridSolverServers' to use for the hybrid solver service, defaults to the
-            production server. Defaults to 'HybridSolverServers.PROD'.
-        suppress_output (bool): (optional) Boolean indicating whether to suppress logging output from the runner, defaults to False.
-
-    Attributes:
-        https_client: The 'SpecsHTTPSClient' used for making requests to the hybrid solver service.
-    """
-    def __init__(self, api_key: str, server: HybridSolverServers = HybridSolverServers.PROD, suppress_output : bool = False):
+    def __init__(self, api_key: str, server: HybridSolverServers = HybridSolverServers.PROD, suppress_log : bool = False):
         self.https_client = SpecsHTTPSClient(api_key=api_key, target_server=server)
-        self.suppress_output = suppress_output
-        self._error_symbol = "❌"
+        self.suppress_log = suppress_log
 
-    def httpsClient(self):
-        return self.https_client
+    def _solveParseArgs(self, **kwargs):
 
-    def _parseKwargs(self, **kwargs):
+        # default values
+        poll_frequency: float = 1
+        timeout: float = 14400
 
-        poll_frequency = kwargs.get("poll_frequency", 1)
-        timeout = kwargs.get("timeout", 14400)
-        new_incumbent_callback = kwargs.get("new_incumbent_callback", None)
-        submit_callback = kwargs.get("submit_callback", None)
-        job_options = kwargs.get("job_options", {})
-
-        return poll_frequency, timeout, new_incumbent_callback, submit_callback, job_options
-
-    def waitForJob(self, jobid: uuid, poll_frequency: float, timeout: float, solver_logs: list, batch_size : int, new_incumbent_callback = None) -> JobStatus:
-        """
-        Polls the status of a job identified by `jobid` until it reaches a final status or until the timeout is exceeded. The function updates the solver logs and calls the new incumbent callback function if a new incumbent is found in the batch item.
-
-        Args:
-            jobid: A UUID object that identifies the job to poll the status for.
-            poll_frequency: The frequency (as float, in seconds) at which the function should poll for job status.
-            timeout: The maximum amount of time (as float, in seconds) to wait for the job to finish before timing out.
-            solver_logs: A list of `SolverLog` objects to update with the current log of the job.
-            batch_size: The size of the batch for the job as an integer.
-            new_incumbent_callback: (optional) A callback function to call if a new incumbent is found in the batch item. Defaults to None.
-
-        Returns:
-            JobStatus: A `JobStatus` enum value indicating whether the job has finished, terminated, or timed out.
-        """
-        printed_created = False
-        printed_running = False
-        spinner = yaspin()
+        # parse args
+        if "poll_frequency" in kwargs:
+            poll_frequency = kwargs["poll_frequency"]
+        if "poll_frequency" in kwargs:
+            timeout = kwargs["timeout"]
 
-        batch_num_incumbents = [0] * batch_size
+        solver_log = SolverLog() 
 
+        return poll_frequency, timeout, solver_log
+
+    def waitForJob(self, jobid: int, poll_frequency: float, timeout: float, solver_log: SolverLog) -> JobStatus:
+
+        printed_created = False
+        printed_running = False
         for t in range(0,int(timeout/poll_frequency)):
 
             sleep(poll_frequency)
 
-            try:
-                status = self.https_client.checkJob(jobid=jobid)
-            except RuntimeError as runtime_e:
-                sys.exit(f"{self._error_symbol} Unable to check job:\n\n{runtime_e}")
-
-            if printed_running and not self.suppress_output:
-                try:
-                    logs = self.https_client.getCurrentLog(jobid=jobid)
-                except RuntimeError as runtime_e:
-                    sys.exit(f"{self._error_symbol} Unable to get log:\n\n{runtime_e}")
-
-                for ix in range(0, batch_size):
-                    solver_logs[ix].updateLog(logs[ix])
-
-            # stop spinner if necessary: for small problems polling interval might be too long to ever reach JobStatus.running
-            if (status == JobStatus.running or status == JobStatus.finished) and not printed_running and not self.suppress_output:
-                spinner.text = f"Job {jobid} unqueued, processing..."
-                spinner.ok("✔")
-                spinner.stop()
-                solver_logs[0].nextTimeAddNewLine()
-                printed_running = True
+            status = self.https_client.checkJob(jobid=jobid)
+            if not self.suppress_log:
+                solver_log.updateLog(self.https_client.getCurrentLog(jobid=jobid))
 
-            # note: we do not give an error status to the job, but rather do
-            # this on the batch item level (as part of getResults)
             if status == JobStatus.finished:
                 return JobStatus.finished
-            elif status == JobStatus.terminated:
-                return JobStatus.terminated
             elif status == JobStatus.error:
                 return JobStatus.error
             elif status == JobStatus.created:
-                if not self.suppress_output:
+                if not self.suppress_log:
                     if not printed_created:
                         printed_created = True
-                        spinner.text = "Waiting for a free slot in the queue..."
-                        spinner.start()
-                        solver_logs[0].nextTimeAddNewLine()
+                        print("Waiting for a free slot in the queue.", end="", flush=True)
+                        solver_log.nextTimeAddNewLine()
+                    else:
+                        print(".", end="", flush=True)
+
             elif status == JobStatus.running:
-                # check whether we got a new solution in any of the batch items
-                if new_incumbent_callback is not None:
-                    try:
-                        batch_solutions = self.https_client.getCurrentSolution(jobid=jobid)
-                    except RuntimeError as runtime_e:
-                        sys.exit(f"{self._error_symbol}: " + str(runtime_e))
-
-                    for ix in range(0, batch_size):
-                        if int(batch_solutions[ix]["incumbents"]) > batch_num_incumbents[ix]:
-                            new_incumbent_callback(ix, batch_solutions[ix]["objective"], batch_solutions[ix]["solution"])
-                            batch_num_incumbents[ix] = int(batch_solutions[ix]["incumbents"])
+                if not printed_running and not self.suppress_log:
+                    printed_running = True
+                    print(f"\nJob {jobid} unqueued, processing...")
+
+                    solver_log.nextTimeAddNewLine()
 
         return JobStatus.timeout
 
-    async def waitForJobAsync(self, jobid: uuid, poll_frequency: float, timeout: float, solver_logs: list, batch_size : int, new_incumbent_callback = None) -> JobStatus:
-        """
-        Asynchronously polls the status of a job identified by `jobid` until it reaches a final status or until the timeout is exceeded. The function updates the solver logs and calls the new incumbent callback function if a new incumbent is found in the batch item.
-
-        Args:
-            jobid: A UUID that identifies the job to poll the status for.
-            poll_frequency: The frequency (as float, in seconds) at which the function should poll for job status.
-            timeout: The maximum amount of time (as float, in seconds) to wait for the job to finish before timing out.
-            solver_logs: A list of `SolverLog` objects to update with the current log of the job.
-            batch_size: The size of the batch for the job as integer.
-            new_incumbent_callback: (optional) A callback function to call if a new incumbent is found in the batch item. Defaults to None.
-
-        Returns:
-            JobStatus: A `JobStatus` enum value indicating whether the job has finished, terminated, or timed out.
-        """
+    async def waitForJobAsync(self, jobid: int, poll_frequency: float, timeout: float, solver_log: SolverLog) -> JobStatus:
 
         printed_created = False
         printed_running = False
-        spinner = yaspin()
-
-        batch_num_incumbents = [0] * batch_size
-
         for t in range(0,int(timeout/poll_frequency)):
 
             await asyncio.sleep(poll_frequency)
 
-            try:
-                status = await self.https_client.checkJobAsync(jobid=jobid)
-            except RuntimeError as runtime_e:
-                sys.exit(f"{self._error_symbol} Unable to check job:\n\n{runtime_e}")
-
-            if printed_running and not self.suppress_output:
-                try:
-                    logs = await self.https_client.getCurrentLogAsync(jobid=jobid)
-                except RuntimeError as runtime_e:
-                    sys.exit(f"{self._error_symbol}: " + str(runtime_e))
-                for ix in range(0, batch_size):
-                    solver_logs[ix].updateLog(logs[ix])
-
-            # stop spinner if necessary: for small problems polling interval might be too long to ever reach JobStatus.running
-            if (status == JobStatus.running or status == JobStatus.finished) and not printed_running and not self.suppress_output:
-                spinner.text = f"Job {jobid} unqueued, processing..."
-                spinner.ok("✔")
-                spinner.stop()
-                solver_logs[0].nextTimeAddNewLine()
-                printed_running = True
+            status = await self.https_client.checkJobAsync(jobid=jobid)
+            if not self.suppress_log:
+                solver_log.updateLog(await self.https_client.getCurrentLogAsync(jobid=jobid))
 
             if status == JobStatus.finished:
                 return JobStatus.finished
-            elif status == JobStatus.terminated:
-                return JobStatus.terminated
             elif status == JobStatus.error:
                 return JobStatus.error
             elif status == JobStatus.created:
-                if not self.suppress_output:
+                if not self.suppress_log:
                     if not printed_created:
                         printed_created = True
-                        spinner.text = "Waiting for a free slot in the queue..."
-                        spinner.start()
-                        solver_logs[0].nextTimeAddNewLine()
+                        print("Waiting for a free slot in the queue.", end="", flush=True)
+                        solver_log.nextTimeAddNewLine()
+                    else:
+                        print(".", end="", flush=True)
 
             elif status == JobStatus.running:
-                # check whether we got a new solution in any of the batch items
-                if new_incumbent_callback is not None:
-                    try:
-                        batch_solutions = await self.https_client.getCurrentSolutionAsync(jobid=jobid)
-                    except RuntimeError as runtime_e:
-                        sys.exit(f"{self._error_symbol}: " + str(runtime_e))
-
-                    for ix in range(0, batch_size):
-                        if int(batch_solutions[ix]["incumbents"]) > batch_num_incumbents[ix]:
-                            new_incumbent_callback(ix, batch_solutions[ix]["objective"], batch_solutions[ix]["solution"])
-                            batch_num_incumbents[ix] = int(batch_solutions[ix]["incumbents"])
+                if not printed_running and not self.suppress_log:
+                    printed_running = True
+                    print(f"\nJob {jobid} unqueued, processing...")
+
+                    solver_log.nextTimeAddNewLine()
 
         return JobStatus.timeout
 
-    def solve(self, problem_file: str, params: HybridSolverParameters = None, tag : str = "", **kwargs):
-        """
-        Submits a QUBO or MIP instance to the solver.
-
-        Args:
-            problem_file (str): Path to problem file as string.
-            params (HybridSolverParameters): HybridSolverParameter object.
-
-        Keyword arguments:
-            submit_callback: (optional) Custom callback function that is called when a job is submitted. Defaults to None.
-            poll_frequency (float): (optional) The frequency (as float, in seconds) at which the function should poll for job status. Defaults to 1.
-            new_incumbent_callback: (optional) A callback function to call if a new incumbent is found in the batch item. Defaults to None.
-            timeout (float): (optional) The maximum amount of time (as float, in seconds) to wait for the job to finish before timing out. Defaults to 14400.
-
-        Returns:
-            dict: Solver results as dictionary containing the keys 'status', 'solver_log', 'sol_status', 'timing', 'objective', 'bound', 'absolute_gap', 'relative_gap', 'iterations', 'nodes', 'nodes_per_sec', 'best_node', 'best_time', 'num_quantum_solutions', 'solver_mix', and 'solution'.
-        """
-        if params is None:
-            params = HybridSolverParameters()
-
-        res, time_billed = self.solveBatched([problem_file], [params], tag, **kwargs)
-        return res[0], time_billed
-
-
-    ###
-    # kwargs:
-    # - submit_callback(jobid): called when job is submitted, receives jobid as parameter
-    ###
-    def solveBatched(self, problem_files: list, params: list = [], tag : str = "", **kwargs):
-        """
-        Submits a set of QUBO or MIP instances to the cloud for solving.
-
-        Args:
-            problem_files (List[str]): List of paths to problem files as string.
-            params (List[HybridSolverParameters]): List of HybridSolverParameter objects.
-
-        Keyword arguments:
-            submit_callback: (optional) Custom callback function that is called when a job is submitted. Defaults to None.
-            poll_frequency (float): (optional) The frequency (as float, in seconds) at which the function should poll for job status. Defaults to 1.
-            new_incumbent_callback: (optional) A callback function to call if a new incumbent is found in the batch item. Defaults to None.
-            timeout  (float): (optional) The maximum amount of time (as float, in seconds) to wait for the job to finish before timing out. Defaults to 14400.
-
-        Returns:
-            List[Dict[str, Any]]: List of solver results. For each submitted instance it contains a dictionary with the keys 'status', 'solver_log', 'sol_status', 'timing', 'objective', 'bound', 'absolute_gap', 'relative_gap', 'iterations', 'nodes', 'nodes_per_sec', 'best_node', 'best_time', 'num_quantum_solutions', 'solver_mix', and 'solution'.
-        """
-
-        # parse keyword args
-        poll_frequency, timeout, new_incumbent_callback, submit_callback, job_options = self._parseKwargs(**kwargs)
-        # get batch size
-        batch_size = len(problem_files)
-        # prepare solver logs
-        solver_logs = [SolverLog() for ix in range(0, batch_size)]
-
-        # initialize params list if it is not passed
-        if params == []:
-            params = [HybridSolverParameters() for _ in problem_files]
-        specs = build_specs_list(params, problem_files, job_options)
-
-
-        if not self.suppress_output:
-            spinner = yaspin()
-            spinner.start()
-            spinner.text = "Submitting job to the Quantagonia cloud..."
-            spinner.start()
-        try:
-            context = kwargs["context"] if 'context' in kwargs.keys() else ""
-            jobid = self.https_client.submitJob(
-                problem_files=problem_files, specs=specs, tag=tag, context=context)
-            if("submit_callback" in kwargs):
-                kwargs["submit_callback"](jobid)
-        except RuntimeError as runtime_e:
-            if not self.suppress_output:
-                spinner.text = "Cannot submit job"
-                spinner.ok(self._error_symbol)
-                spinner.stop()
-            sys.exit(str(runtime_e))
-        except FileNotFoundError as fnf_e:
-            if not self.suppress_output:
-                spinner.text = "File not found"
-                spinner.ok(self._error_symbol)
-                spinner.stop()
-            sys.exit(str(fnf_e))
-
-        if not self.suppress_output:
-            spinner.text = f"Queued job with jobid: {jobid} for execution in the Quantagonia cloud..."
-            spinner.ok("✔")
-            spinner.stop()
+    def solve(self, problem_file: str, spec: dict, **kwargs):
+        
+        poll_frequency, timeout, solver_log = self._solveParseArgs(**kwargs)
+
+        jobid = self.https_client.submitJob(problem_file=problem_file, spec=spec)
+        if not self.suppress_log:
+            print(f"Queued job with jobid: {jobid} for execution in the Quantagonia cloud...\n")
 
-        status: JobStatus = self.waitForJob(jobid=jobid, poll_frequency=poll_frequency, timeout=timeout,
-            solver_logs=solver_logs, batch_size=batch_size, new_incumbent_callback=new_incumbent_callback)
+        status: JobStatus = self.waitForJob(jobid=jobid, poll_frequency=poll_frequency, timeout=timeout, solver_log=solver_log)
 
         if status is not JobStatus.finished:
             raise Exception(f"Job with jobid {jobid} error. Status of the job: {status}")
         else:
-            if not self.suppress_output:
+            if not self.suppress_log:
                 print(f"Finished processing job {jobid}...")
 
-        try:
-            res, time_billed = self.https_client.getResults(jobid=jobid)
-        except RuntimeError as runtime_e:
-            sys.exit(f"{self._error_symbol}: " + str(runtime_e))
-
-        if not self.suppress_output:
-            for ix in range(0, batch_size):
-                solver_logs[ix].updateLog(res[ix]['solver_log'])
-
-        # parse solver logs and add solution
-        for ix in range(0, batch_size):
-            # parse and add solve stats
-            logparser = SolverLogParser(res[ix]["solver_log"])
-            res[ix].update(logparser.get_solver_summary())
-            # add solution
-            res[ix]["solution"] = SolutionParser.parse(res[ix]["solution_file"])
-            # no need to keep the solution file
-            res[ix].pop("solution_file")
-
-        return res, time_billed
-
-    async def solveAsync(self, problem_file: str, params: HybridSolverParameters = None, tag : str = "", **kwargs):
-        """
-        Asynchonously submits a QUBO or MIP instance to the cloud for solving.
-
-        Args:
-            problem_file (str): Path to problem file as string.
-            spec (dict): A dictionary of solver options and parameters.
-
-        Keyword arguments:
-            submit_callback: (optional) Custom callback function that is called when a job is submitted. Defaults to None.
-            poll_frequency (float): (optional) The frequency (as float, in seconds) at which the function should poll for job status. Defaults to 1.
-            new_incumbent_callback: (optional) A callback function to call if a new incumbent is found in the batch item. Defaults to None.
-            timeout (float): (optional) The maximum amount of time (as float, in seconds) to wait for the job to finish before timing out. Defaults to 14400.
-
-        Returns:
-            dict: Solver results as dictionary containing the keys 'status', 'solver_log', 'sol_status', 'timing', 'objective', 'bound', 'absolute_gap', 'relative_gap', 'iterations', 'nodes', 'nodes_per_sec', 'best_node', 'best_time', 'num_quantum_solutions', 'solver_mix', and 'solution'.
-        """
-        if not params:
-            params = HybridSolverParameters()
-
-        res, time_billed = await self.solveBatchedAsync([problem_file], [params], tag, **kwargs)
-        return res[0], time_billed
-
-    async def solveBatchedAsync(self, problem_files: list, params: list = [], tag : str = "", **kwargs):
-        """
-        Asynchronously submits a set of QUBO or MIP instances to the cloud for solving.
-
-        Args:
-            problem_files (List[str]): List of paths to problem files as string.
-            specs (List[HybridSolverParameters]): List of HybridSolverParameters
-
-        Keyword arguments:
-            submit_callback: (optional) Custom callback function that is called when a job is submitted. Defaults to None.
-            poll_frequency (float): (optional) The frequency (as float, in seconds) at which the function should poll for job status. Defaults to 1.
-            new_incumbent_callback: (optional) A callback function to call if a new incumbent is found in the batch item. Defaults to None.
-            timeout (float): (optional) The maximum amount of time (as float, in seconds) to wait for the job to finish before timing out. Defaults to 14400.
-
-        Returns:
-            List[Dict[str, Any]]: List of solver results. For each submitted instance it contains a dictionary containing the keys 'status', 'solver_log', 'sol_status', 'timing', 'objective', 'bound', 'absolute_gap', 'relative_gap', 'iterations', 'nodes', 'nodes_per_sec', 'best_node', 'best_time', 'num_quantum_solutions', 'solver_mix', and 'solution'.
-        """
-
-        # parse keyword args
-        poll_frequency, timeout, new_incumbent_callback, submit_callback, job_options = self._parseKwargs(**kwargs)
-        # get batch size
-        batch_size = len(problem_files)
-        # prepare solver logs
-        solver_logs = [SolverLog() for ix in range(0, batch_size)]
-
-        # initialize params list if it is not passed
-        if params == []:
-            params = [HybridSolverParameters() for _ in problem_files]
-        specs = build_specs_list(params, problem_files, job_options)
-
-
-        if not self.suppress_output:
-            spinner = yaspin()
-            spinner.start()
-            spinner.text = "Submitting job to the Quantagonia cloud..."
-            spinner.start()
-        try:
-            context = kwargs["context"] if 'context' in kwargs.keys() else ""
-            jobid = await self.https_client.submitJobAsync(
-                problem_files=problem_files, specs=specs, tag=tag, context=context)
-        except RuntimeError as runtime_e:
-            if not self.suppress_output:
-                spinner.text = "Cannot submit job"
-                spinner.ok(self._error_symbol)
-                spinner.stop()
-            sys.exit(str(runtime_e))
-        except FileNotFoundError as fnf_e:
-            if not self.suppress_output:
-                spinner.text = "File not found"
-                spinner.ok(self._error_symbol)
-                spinner.stop()
-            sys.exit(str(fnf_e))
-
-        if not self.suppress_output:
-            spinner.text = f"Queued job with jobid: {jobid} for execution in the Quantagonia cloud..."
-            spinner.ok("✔")
-            spinner.stop()
+        res = self.https_client.getResults(jobid=jobid)
+        if not self.suppress_log:
+            solver_log.updateLog(res['solver_log'])
+
+        return {
+            'solver_log' : res['solver_log'],
+            'solution_file' : res['solution_file']
+        }
+
+    async def solveAsync(self, problem_file: str, spec: dict, **kwargs):
+        
+        poll_frequency, timeout, solver_log = self._solveParseArgs(**kwargs)
+
+        jobid = await self.https_client.submitJobAsync(problem_file=problem_file, spec=spec)
+        if not self.suppress_log:
+            print(f"Queued job with jobid: {jobid} for execution in the Quantagonia cloud...")
 
-        status: JobStatus = await self.waitForJobAsync(jobid=jobid, poll_frequency=poll_frequency, timeout=timeout,
-            solver_logs=solver_logs, batch_size=batch_size, new_incumbent_callback=new_incumbent_callback)
+        status: JobStatus = await self.waitForJobAsync(jobid=jobid, poll_frequency=poll_frequency, timeout=timeout, solver_log=solver_log)
 
         if status is not JobStatus.finished:
             raise Exception(f"Job with jobid {jobid} error. Status of the job: {status}")
         else:
-            if not self.suppress_output:
+            if not self.suppress_log:
                 print(f"Finished processing job {jobid}...")
 
-        try:
-            res, time_billed = self.https_client.getResults(jobid=jobid)
-        except RuntimeError as runtime_e:
-            sys.exit(f"{self._error_symbol}: " + str(runtime_e))
-        if not self.suppress_output:
-            for ix in range(0, batch_size):
-                solver_logs[ix].updateLog(res[ix]['solver_log'])
-
-        for ix in range(0, batch_size):
-            # parse and add solve stats
-            logparser = SolverLogParser(res[ix]["solver_log"])
-            res[ix].update(logparser.get_solver_summary())
-            # add solution
-            res[ix]["solution"] = SolutionParser.parse(res[ix]["solution_file"])
-            # no need to keep the solution file
-            res[ix].pop("solution_file")
-
-        return res, time_billed
-
-
-    def interrupt_job(self, jobid: uuid):
-        """
-        Sends an interrupt signal to stop the execution of the specified job.
-
-        Args:
-            jobid (uuid): The UUID of the job to be interrupted.
-
-        Returns:
-            dict: A dictionary containing the response from the server.
-        """
-        resp = self.https_client.interrupt_job(jobid)
-        return resp
-
-    async def interrupt_job_async(self, jobid:uuid):
-        """
-        Asynchronously sends an interrupt signal to stop the execution of a submitted job.
-
-        Args:
-            jobid (uuid): The UUID of the job to be interrupted.
-
-        Returns:
-            dict: A dictionary containing the response from the server.
-        """
-        resp = await self.https_client.interruptJobAsync(jobid)
-        return resp
-
-
-
-#################################
-# helper functions
-#################################
-
-def build_specs_list(params: list, problem_files: list, job_options: dict):
-    """
-    Build a list of spec dictionaries consisting of solver parameters and the problem type.
-    Here we use the file suffix to determine the problem type.
-    A proper problem type detection is done serverside.
-    """
-
-    specs = []
-    for idx, param in enumerate(params):
-        spec = {
-            "solver_config": param.getd(),
-            "problem_type": get_problem_type_from_filename(problem_files[idx]).value,
-            "processing": job_options
-        }
-        specs.append(spec)
-
-    return specs
-
-def get_problem_type_from_filename(problem_file_name):
-    # remove suffixes
-    problem_file_name = pathlib.Path(problem_file_name)
-    suffixes = problem_file_name.suffixes
-    suffixes.reverse()  # reverse list to check last suffix first
-    for suffix in suffixes:
-        if suffix in [".qubo"]:
-            return HybridSolverProblemType.QUBO
-        elif suffix in [".lp", ".mps"]:
-            return HybridSolverProblemType.MIP
-
-    raise RuntimeError("Could not detect problem type.")
+        res = await self.https_client.getResultsAsync(jobid=jobid)
+        if not self.suppress_log:
+            solver_log.updateLog(res['solver_log'])
+
+        return {
+            'solver_log' : res['solver_log'],
+            'solution_file' : res['solution_file']
+        }
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## quantagonia/cloud/solver_log.py

```diff
@@ -1,24 +1,23 @@
 class SolverLog:
-    
     def __init__(self):
         self.log: str = ""
         self.add_newline = False
 
     def nextTimeAddNewLine(self):
         self.add_newline = True
 
     """
     takes as input the updated log. It will make sure that the old log is contained in the new log, and print the
     difference to the screen
     """
     def updateLog(self, new_log: str, add_newline : bool = False) -> None:
         if new_log == "":
             return
-        
+
         old_log_len = len(self.log)
 
         if self.log != new_log[:old_log_len]:
             print("WARNING: there was some suspicious discrepancy in the solver log received from the server. "
                   "The solver log might not be printed in the order as the solver generated it.")
 
         if len(new_log) != old_log_len and self.add_newline:
```

## quantagonia/cloud/specs_enums.py

```diff
@@ -1,23 +1,14 @@
 from enum import Enum
 
-
 class SpecsEndpoints(str, Enum):
+    submitjob = "/submitjob"
     checkjob = "/checkjob"
-    getcurstatus = "/getcurstatus"
-    getcursolution = "/getcursolution"
     getcurlog = "/getcurlog"
     getresults = "/getresults"
-    getjobs = "/jobs"
-    interruptjob = "/job"
-    job = "/job"
-    s3 = "/s3"
-
 
 class JobStatus(str, Enum):
-    finished = "FINISHED"
-    terminated = "TERMINATED"
-    error = "ERROR"
-    running = "RUNNING"
-    created = "CREATED"
-    timeout = "TIMEOUT"
-    success = "SUCCESS"
+    finished = "Finished"
+    error = "Error"
+    running = "Running"
+    created = "Created"
+    timeout = "Timeout"
```

## quantagonia/cloud/specs_https_client.py

```diff
@@ -1,262 +1,76 @@
 import json
 import os
-import urllib
 import uuid
 import requests
-import copy
-from typing import Tuple
 
-from requests.packages.urllib3.util import Retry
-from requests.adapters import HTTPAdapter
-
-from quantagonia.cloud.dto.encoder import DtoJSONEncoder
-from quantagonia.cloud.dto.job import JobDto
-from quantagonia.cloud.dto.presigned_s3 import PresignedS3
 from quantagonia.cloud.specs_enums import *
 from quantagonia.enums import HybridSolverServers
-from quantagonia.errors import SolverError
-
 
 class SpecsHTTPSClient():
     """ client class for qqvm server """
-    def __init__(self, api_key: str, target_server: HybridSolverServers = HybridSolverServers.PROD,
-        custom_headers = {}) -> None:
+    def __init__(self, api_key: str, target_server: HybridSolverServers = HybridSolverServers.PROD) -> None:
         """ """
         self.api_key = api_key
         self.server = target_server.value
-        self.custom_headers = custom_headers
 
-        self.retry = Retry(total=5, backoff_factor=1, allowed_methods=frozenset(['GET', 'POST', 'PUT', 'DELETE']))
-        self.session = requests.Session()
-        self.session.mount('http://', HTTPAdapter(max_retries=self.retry))
-        self.session.mount('https://', HTTPAdapter(max_retries=self.retry))
-
-    def _submitJob(self, problem_files: list, specs: list, tag : str = "", context : str = "") -> uuid:
-
-        # build a single JSON array with specs
-        spec_arr = {}
-        for ix in range(0, len(specs)):
-            spec_arr[str(ix)] = specs[ix]
-
-        files = [("files", (os.path.basename(prob), open(prob, "rb"))) for prob in problem_files]
-
-        job = JobDto()
-        data = json.dumps(job, cls=DtoJSONEncoder)
-        response = self.session.post(self.server + SpecsEndpoints.job,
-            data=data,
-            headers={"X-api-key": self.api_key, 'Content-type': "application/json",
-            **self.custom_headers})
+    def _submitJob(self, problem_file: str, spec: dict) -> uuid:
+        with open(problem_file, 'rb') as file:
+            files = {'file': (os.path.basename(problem_file), file, 'text/plain')}
+            response = requests.post(self.server + SpecsEndpoints.submitjob, files=files, params={"spec" : json.dumps(spec)}, headers={"X-api-key" : self.api_key})
+
         if not response.ok:
-            error_report = response.json()
-            raise RuntimeError(error_report)
-        jobId = response.json()['jobId']
-        problems = []
-        spec_files = []
-        for ind, prob in enumerate(problem_files):
-            try:
-                filename = prob.parts[len(prob.parts)-1]
-            except AttributeError as e:
-                filename = prob.split("/")[len(prob.split("/")) - 1]
-
-            file_key = jobId + "/" + str(ind) + "/" + filename
-            problems.append(file_key)
-            ps3_problem_file = PresignedS3(jobId=jobId, contentType="application/octet-stream",
-                key=file_key)
-            data_for_s3 = json.dumps(ps3_problem_file, cls=DtoJSONEncoder)
-            response = self.session.post(self.server + SpecsEndpoints.s3, data=data_for_s3,
-                headers={"X-api-key": self.api_key, 'Content-type': "application/json",
-                **self.custom_headers})
-            if not response.ok:
-                raise RuntimeError("Unable to get an S3 presigned URL")
-            presigned_url = response.json()['url']
-            author = response.json()['metaAuthor']
-            version = response.json()['metaVersion']
-
-            # uploading files as binaries as they could be zipped
-            with open(prob, 'rb') as problem_file:
-                problem_bytes = problem_file.read()
-
-            headers = {"X-amz-meta-author": author,
-                       "X-amz-meta-version": version,
-                       'Content-type': "application/octet-stream"}
-            response = self.session.put(presigned_url, data=problem_bytes, headers=headers)
-            if not response.ok:
-                error_report = response.json()
-                raise RuntimeError(error_report)
-            spec = spec_arr[str(ind)]
-            spec_key = jobId + "/" + str(ind) + "/spec.json"
-            spec_files.append(spec_key)
-            ps3_specs_file = PresignedS3(jobId=jobId, contentType="text/plain", key=spec_key)
-            spec_for_s3 = json.dumps(ps3_specs_file, cls=DtoJSONEncoder)
-            response = self.session.post(self.server + SpecsEndpoints.s3, data=spec_for_s3,
-                headers={"X-api-key": self.api_key, 'Content-type': "application/json",
-                **self.custom_headers})
-            spec_str = json.dumps(spec)
-            presigned_url = response.json()['url']
-            author = response.json()['metaAuthor']
-            version = response.json()['metaVersion']
-            headers = {"X-amz-meta-author": author,
-                        "X-amz-meta-version": version,
-                        'Content-type': "text/plain"}
-            response = self.session.put(presigned_url, data=spec_str, headers=headers)
-            if not response.ok:
-                error_report = response.json()
-                raise RuntimeError(error_report)
-
-        start_job = JobDto(jobId=jobId, problemFiles=problems, specFiles=spec_files, tag=tag, context=context)
-        start_job_data = json.dumps(start_job, cls=DtoJSONEncoder)
-        started_job = self.session.post(self.server + SpecsEndpoints.job, data=start_job_data,
-            headers={"X-api-key": self.api_key, 'Content-type': "application/json",
-            **self.custom_headers})
-        if not started_job.ok:
-            error_report = started_job.json()
-            raise RuntimeError(error_report)
-        returned_job_id = started_job.json()['jobId']
-        return returned_job_id
-
-    def _replaceFileContentFromUrl(self, e, key):
-        e[key] = self._getFileContentFromUrl(e[key])
-            
-    def _getFileContentFromUrl(self, e):
-        if type(e) is dict and "error" in e:
-            return "Error: " + e["error"]
-        elif type(e) is dict and "url" in e:
-            if e["url"] == "":
-                return ""
-            response = self.session.get(e["url"])
-            if response.status_code == 200:
-                return response.text
-            else:
-                return ""
-        else:
-            return e
+            raise RuntimeError(f"Request error. status: {response.status_code}, text: {response.text}")
+        return response.json()['jobid']
 
     def _checkJob(self, jobid: uuid) -> str:
         params = {'jobid': str(jobid)}
-        response = self.session.get(self.server + SpecsEndpoints.checkjob, params=params,
-            headers={"X-api-key": self.api_key, **self.custom_headers})
-        if response.ok:
-            return response.json()['status']
-        elif response.status_code > 499:
-            log = self._getCurrentLog(jobid)
-            error_report = response.json()
-            error_report["details"] = log[0]
-            raise SolverError(error_report)
-        elif response.status_code < 499:
-            error_report = response.json()
-            raise RuntimeError(error_report)
-
-    def _getCurrentStatus(self, jobid: uuid) -> str:
-        params = {'jobid': str(jobid)}
-        response = self.session.get(self.server + SpecsEndpoints.getcurstatus, params=params,
-            headers={"X-api-key" : self.api_key, **self.custom_headers})
-
-        return json.loads(response.text)
-
-    def _getCurrentSolution(self, jobid: uuid) -> str:
-        params = {'jobid': str(jobid)}
-        response = self.session.get(self.server + SpecsEndpoints.getcursolution, params=params,
-            headers={"X-api-key" : self.api_key, **self.custom_headers})
-
-        array = json.loads(response.text)
-        for e in array:
-            self._replaceFileContentFromUrl(e, "solution")
-        return array
-
-    def _getCurrentLog(self, jobid: uuid) -> str:
-        params = {'jobid': str(jobid)}
-        response = self.session.get(self.server + SpecsEndpoints.getcurlog, params=params,
-            headers={"X-api-key" : self.api_key, **self.custom_headers})
+        response = requests.get(self.server + SpecsEndpoints.checkjob, params=params, headers={"X-api-key" : self.api_key})
+        
         if not response.ok:
-            error_report = response.json()
-            raise RuntimeError(error_report)
-        return [self._getFileContentFromUrl(e) for e in json.loads(response.text)]
+            raise RuntimeError(f"Request error. status: {response.status_code}, text: {response.text}")
+        return response.json()['status']
 
-    def _getResults(self, jobid: uuid) -> Tuple[dict, int]:
+    def _getCurrentLog(self, jobid: uuid) -> str:
         params = {'jobid': str(jobid)}
-        response = self.session.get(self.server + SpecsEndpoints.getresults, params=params,
-            headers={"X-api-key" : self.api_key, **self.custom_headers})
-
-        if not response.ok:
-            error_report = response.json()
-            raise RuntimeError(error_report)
-    
-        result = json.loads(response.text)
-        array = copy.deepcopy(result["result"])
-
-        for e in array:
-            self._replaceFileContentFromUrl(e, "solution_file")
-            self._replaceFileContentFromUrl(e, "solver_log")
-
-        return array, int(result["time_billed"])
-    
-    def _getJobs(self, n : int) -> dict:
-        params = {'n': str(n)}
-        response = self.session.get(self.server + SpecsEndpoints.getjobs, params=params,
-            headers={"X-api-key" : self.api_key, **self.custom_headers})
+        response = requests.get(self.server + SpecsEndpoints.getcurlog, params=params, headers={"X-api-key" : self.api_key})
 
         if not response.ok:
-            error_report = response.json()
-            raise RuntimeError(error_report)
-
-        return json.loads(response.text)
+            raise RuntimeError(f"Request error. status: {response.status_code}, text: {response.text}")
+        return response.text
 
-    def _interruptJob(self, jobid: uuid):
-        response = self.session.delete(self.server + SpecsEndpoints.interruptjob + "/" + str(jobid),
-            headers={"X-api-key": self.api_key, **self.custom_headers})
+    def _getResults(self, jobid: uuid) -> dict:
+        params = {'jobid': str(jobid)}
+        response = requests.get(self.server + SpecsEndpoints.getresults, params=params, headers={"X-api-key" : self.api_key})
         
         if not response.ok:
-            error_report = response.json()
-            raise RuntimeError(error_report)
-
-        return True
+            raise RuntimeError(f"Request error. status: {response.status_code}, text: {response.text}")
+        return {
+            "solver_log" : response.json()['solver_log'],
+            "solution_file" : response.json()['solution_file']
+        }
 
     ### blocking interface
-    def submitJob(self, problem_files: list, specs: list, tag : str = "", context : str = "") -> uuid:
-        return self._submitJob(problem_files, specs, tag = tag, context = context)
+    def submitJob(self, problem_file: str, spec: dict) -> uuid:
+        return self._submitJob(problem_file, spec)
 
     def checkJob(self, jobid: uuid) -> str:
         return self._checkJob(jobid)
 
-    def getCurrentStatus(self, jobid: uuid) -> str:
-        return self._getCurrentStatus(jobid)
-
-    def getCurrentSolution(self, jobid: uuid) -> str:
-        return self._getCurrentSolution(jobid)
-
     def getCurrentLog(self, jobid: uuid) -> str:
         return self._getCurrentLog(jobid)
 
-    def getResults(self, jobid: uuid) -> Tuple[dict, int]:
+    def getResults(self, jobid: uuid) -> dict:
         return self._getResults(jobid)
-    
-    def getJobs(self, n : int) -> dict:
-        return self._getJobs(n)
-
-    def interruptJob(self, jobid: uuid) -> dict:
-        return self._interruptJob(jobid)
 
     ### non-blocking interface
-    async def submitJobAsync(self, problem_files: list, specs: list, tag : str = "", context : str = "") -> uuid:
-        return self._submitJob(problem_files, specs, tag = tag, context = context)
+    async def submitJobAsync(self, problem_file: str, spec: dict) -> uuid:
+        return self._submitJob(problem_file, spec)
 
     async def checkJobAsync(self, jobid: uuid) -> str:
         return self._checkJob(jobid)
 
-    async def getCurrentStatusAsync(self, jobid: uuid) -> str:
-        return self._getCurrentStatus(jobid)
-
-    async def getCurrentSolutionAsync(self, jobid: uuid) -> str:
-        return self._getCurrentSolution(jobid)
-
     async def getCurrentLogAsync(self, jobid: uuid) -> str:
         return self._getCurrentLog(jobid)
 
-    async def getResultsAsync(self, jobid: uuid) -> Tuple[dict, int]:
-        return self._getResults(jobid)
-    
-    async def getJobsAsync(self) -> dict:
-        return self._getJobs()
-
-    async def interruptJobAsync(self, jobid: uuid) -> dict:
-        return self._interrupt_job(jobid)
+    async def getResultsAsync(self, jobid: uuid) -> dict:
+        return self._getResults(jobid)
```

## quantagonia/pulp/hybrid_solver_api.py

```diff
@@ -1,71 +1,102 @@
 import sys, os, os.path
 from pulp.apis import LpSolver_CMD, subprocess, PulpSolverError, constants
 from enum import Enum
 import warnings
 
 from quantagonia.runner import Runner
-from quantagonia.parameters import HybridSolverParameters
-from quantagonia.parser.solution_parser import SolutionParser
+from quantagonia.cloud.spec_builder import MIPSpecBuilder
+
+THIS_SCRIPT = os.path.dirname(os.path.realpath(__file__))
+
+def EPSLE(x, y, eps=1e-7): return (x-y) <= eps
+def EPSLT(x, y, eps=1e-7): return (x-y) < -eps
+def EPSGE(x, y, eps=1e-7): return (x-y) >= -eps
+def EPSGT(x, y, eps=1e-7): return (x-y) > eps
+def EPSEQ(x, y, eps=1e-7): return abs(x-y) <= eps
 
 class QQVM_CMD(LpSolver_CMD):
     """The QQVM_CMD solver"""
 
     name = "QQVM_CMD"
 
     def __init__(
-            self,
-            runner : Runner = None,
-            params : dict = None,
-            keepFiles = False,
-            obfuscate: bool = True
+        self,
+        runner : Runner,
+        keepFiles=False,
+        msg=True,
+        options=None,
+        timeLimit=None,
+        mip_abs_gap=None,
+        mip_rel_gap=None,
+        threads=1,
+        obfuscate: bool = True
     ):
         """
-        :param dict params: sets parameters and options for Bolt
+        :param bool msg: if False, no log is shown
+        :param float timeLimit: maximum time for solver (in seconds)
+        :param list options: list of additional options to pass to solver
         :param bool keepFiles: if True, files are saved in the current directory and not deleted after solving
-        :param bool obfuscate: if True, constraints and variable names are obfuscated
+        :param str path_to_qqvm: path to the solver binary
         """
         self.runner = runner
-        self.params = params
-        if self.params is None:
-            self.params = HybridSolverParameters()
+        self.mip_rel_gap=mip_rel_gap
+        self.mip_abs_gap=mip_abs_gap,
+        self.threads=threads
         self.obfuscate = obfuscate
         LpSolver_CMD.__init__(
             self,
             mip=True,
+            msg=msg,
+            timeLimit=timeLimit,
+            options=options,
             path="",
             keepFiles=keepFiles,
         )
 
     def defaultPath(self):
         return self.executableExtension("qqvm")
 
     def available(self):
         """True if the solver is available"""
         return self.executable(self.path)
 
     def actualSolve(self, lp):
         """Solve a well formulated lp problem"""
-
-        if not self.runner:
-            raise PulpSolverError("QQVM runner not set.")
-
         varLP = False # When lp files are written, qqvm-bolt loses the ordering of variables. This results in wrong
         # reading of solutions as the assumed ordering is not present. In order to support varLP=True, one would have to
         # reimplement the readsol method.
 
         if varLP:
             tmpMps, tmpSol, tmpOptions, tmpLog = self.create_tmp_files(
                 lp.name, "lp", "sol", "QQVM", "QQVM_log"
             )
         else:
             tmpMps, tmpSol, tmpOptions, tmpLog = self.create_tmp_files(
                 lp.name, "mps", "sol", "QQVM", "QQVM_log"
             )
 
+        options_file_lines = [
+            "write_solution_style=2",
+        ]
+
+        if self.mip_rel_gap is not None:
+            fl = float(self.mip_rel_gap)
+            if EPSLT(fl, 0.0) or EPSGT(fl, 100.0):
+                raise Exception("relative mip gap needs to be: 0 <= mip_rel_gap <= 100 (in percentages)")
+            options_file_lines.append(f"mip_rel_gap={fl}")
+
+        options_file_lines.append(f"threads={self.threads}")
+        if self.threads > 1:
+            options_file_lines.append("parallel=on")
+        if self.timeLimit is not None:
+            options_file_lines.append("time_limit=%s" % self.timeLimit)
+        if self.mip_abs_gap is not None:
+            options_file_lines.append("mip_abs_gap=%s" % self.mip_abs_gap)
+
         if not varLP:
             if lp.sense == constants.LpMaximize:
                 # we swap the objectives
                 # because it does not handle maximization.
 
                 warnings.warn(
                     "QQVM_CMD solving equivalent minimization form."
@@ -78,81 +109,109 @@
 
         # flag for renaming in writeMPS() should be {0,1}
         rename = 1
         if not self.obfuscate:
             rename = 0
 
         rename_map = {}
-
+        
         if varLP:
             lp.writeLP(filename=tmpMps)  # , mpsSense=constants.LpMinimize)
         else:
             ret_tpl = lp.writeMPS(filename=tmpMps, rename = rename)  # , mpsSense=constants.LpMinimize)
             rename_map = ret_tpl[1]
 
         if lp.isMIP():
             if not self.mip:
                 warnings.warn("QQVM_CMD cannot solve the relaxation of a problem")
 
+        # call Runner to solve the problem (using no special options)
+        spec = MIPSpecBuilder()
+
         ########################################################################
         # actual solve operation (local or cloud)
-        result, _ = self.runner.solve(tmpMps, self.params)
+        result = self.runner.solve(tmpMps, spec.getd(), True)
         ########################################################################
 
         if not varLP:
             if lp.sense == constants.LpMaximize:
                 lp += -lp.objective
 
         # parse solution
         content = result['solver_log'].splitlines()
 
-        sol_status_key = "Solution Status"
-        try:
-            sol_status = next(l for l in content if sol_status_key in l).split()[3]
-        except:
-            raise PulpSolverError("Pulp: Error while executing", self.path)
-
-        has_sol_key = "Best solution found"
-        has_sol = True if len([l for l in content if has_sol_key in l]) >= 1 else False
-
-        # map HybridSolver Status to pulp status
-        if sol_status.lower() == "optimal":  # optimal
+        # LP
+        model_line = [l for l in content if len(l.split()) > 2 and l.split()[:2] == ["Model", "status"]]
+        if len(model_line) > 0:
+            model_status = model_line[0].split()[3]  # Model status: ...
+        else:
+            # ILP
+            model_line = [l for l in content if "Status" in l][0]
+            model_status = model_line.split()[1]
+
+        sol_line = [l for l in content if l[:2] == ["Solution", "status"]]
+        sol_line = sol_line[0] if len(sol_line) > 0 else ["Not solved"]
+        sol_status = sol_line[-1]
+        if model_status.lower() == "optimal":  # optimal
             status, status_sol = (
                 constants.LpStatusOptimal,
                 constants.LpSolutionOptimal,
             )
-        elif sol_status.lower() == "time limit reached" and has_sol:  # feasible
+        elif sol_status.lower() == "feasible":  # feasible
             # Following the PuLP convention
             status, status_sol = (
                 constants.LpStatusOptimal,
                 constants.LpSolutionIntegerFeasible,
             )
-        elif sol_status.lower() == "time limit reached" and not has_sol:  # feasible
-            # Following the PuLP convention
-            status, status_sol = (
-                constants.LpStatusOptimal,
-                constants.LpSolutionNoSolutionFound,
-            )
-        elif sol_status.lower() == "infeasible":  # infeasible
+        elif model_status.lower() == "infeasible":  # infeasible
             status, status_sol = (
                 constants.LpStatusInfeasible,
                 constants.LpSolutionNoSolutionFound,
             )
-        elif sol_status.lower() == "unbounded":  # unbounded
+        elif model_status.lower() == "unbounded":  # unbounded
             status, status_sol = (
                 constants.LpStatusUnbounded,
                 constants.LpSolutionNoSolutionFound,
             )
-        else:
-            raise RuntimeError(f"Uncatched solution status: {sol_status}")
 
-        # remap obfuscated variable names to original variable names
-        for orig_name, obfuscated_name in rename_map.items():
-            result["solution"][orig_name] = result["solution"].pop(obfuscated_name)
+        if status == constants.LpStatusUndefined:
+            raise PulpSolverError("Pulp: Error while executing", self.path)
+
+        values = self.readsol(lp.variables(), result['solution_file'], rename_map)
 
         self.delete_tmp_files(tmpMps, tmpSol, tmpOptions, tmpLog)
         lp.assignStatus(status, status_sol)
 
         if status == constants.LpStatusOptimal:
-            lp.assignVarsVals(result["solution"])
+            lp.assignVarsVals(values)
 
         return status
+
+    @staticmethod
+    def readsol(variables, solution_file, rename_keys = {}):
+        """Read a QQVM solution file"""
+
+        content = solution_file.splitlines()
+
+        values = {}
+        if not len(content):  # if file is empty, update the status_sol
+            return None
+        # extract everything between the line Columns and Rows
+        col_id = [ix for ix in range(0, len(content)) if "Columns" in content[ix]][0]
+        row_id = [ix for ix in range(0, len(content)) if "Row" in content[ix]][0]
+        solution = content[col_id + 1 : row_id]
+
+        for l in solution:
+            var_name, var_val = l.split()
+            values[var_name] = float(var_val)
+
+        # adapt variabel names to obfuscated names
+        if len(rename_keys) > 0:
+            new_values = {}
+
+            for k in rename_keys:
+                new_values[k] = values[rename_keys[k]]
+
+            return new_values
+
+        return values
+
```

## quantagonia/pulp/qpulp_adapter.py

```diff
@@ -1,38 +1,15 @@
 from .hybrid_solver_api import QQVM_CMD
 
 from quantagonia.runner import Runner
 from quantagonia.runner_factory import HybridSolverConnectionType, RunnerFactory
 from quantagonia.enums import HybridSolverServers
-from quantagonia.parameters import HybridSolverParameters
 
 class QPuLPAdapter:
-  """
-  This class provides an adapter for solving MILPs modeled with PuLP.
-  """
 
   @classmethod
-  def getSolver(cls,
-                connection : HybridSolverConnectionType = HybridSolverConnectionType.CLOUD,
-                api_key : str = None,
-                server : HybridSolverServers = HybridSolverServers.PROD,
-                params : HybridSolverParameters = HybridSolverParameters(),
-                keep_files : bool = False):
-    """
-    Returns a solver object for MILP problem instances created with PuLP.
-
-    The solver solves these MILPs with Quantagonias cloud-based HybridSolver.
-
-    Args:
-        connection (optional): Connection type. Defaults to `HybridSolverConnectionType.CLOUD`.
-        api_key (optional): The Quantagonia API key used for the connection. Defaults to None.
-        server (optional): The server used for the connection. It is recommended to use the default value: `HybridSolverServers.PROD`.
-        spec_dict (optional): A solver specifications dictionary. Defaults to None.
-        keep_files (optional): Whether to keep the generated input and output files. Defaults to False.
-
-    Returns:
-        A solver instance.
-    """
+  def getSolver(cls, connection : HybridSolverConnectionType, api_key : str = None, server : HybridSolverServers = HybridSolverServers.PROD):
     runner : Runner = RunnerFactory.getRunner(connection, api_key, server)
-    solver = QQVM_CMD(runner=runner, params=params, keepFiles=keep_files)
+    solver = QQVM_CMD(runner=runner)
 
     return solver
+
```

## Comparing `quantagonia_api_client-0.83.dist-info/LICENSE` & `quantagonia_api_client-0.9.dist-info/LICENSE`

 * *Files identical despite different names*

