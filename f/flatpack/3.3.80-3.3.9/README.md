# Comparing `tmp/flatpack-3.3.80.tar.gz` & `tmp/flatpack-3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.3.80.tar", last modified: Mon Apr 29 23:53:00 2024, max compression
+gzip compressed data, was "flatpack-3.3.9.tar", last modified: Sat Apr 20 00:47:10 2024, max compression
```

## Comparing `flatpack-3.3.80.tar` & `flatpack-3.3.9.tar`

### file list

```diff
@@ -1,33 +1,27 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:53:00.847609 flatpack-3.3.80/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.3.80/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     6009 2024-04-29 23:53:00.847261 flatpack-3.3.80/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     5209 2024-04-29 21:40:43.000000 flatpack-3.3.80/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:53:00.843563 flatpack-3.3.80/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      111 2024-04-27 22:37:06.000000 flatpack-3.3.80/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     2836 2024-04-29 23:48:33.000000 flatpack-3.3.80/flatpack/agent_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.3.80/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.3.80/flatpack/datasets.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:53:00.845374 flatpack-3.3.80/flatpack/engines/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.3.80/flatpack/engines/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      796 2024-04-29 23:15:22.000000 flatpack-3.3.80/flatpack/engines/engine_llama_cpp.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      922 2024-04-29 23:48:47.000000 flatpack-3.3.80/flatpack/engines/fast_api_test.py
--rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.3.80/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.3.80/flatpack/load_modules.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    26214 2024-04-29 21:37:50.000000 flatpack-3.3.80/flatpack/main.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:53:00.846315 flatpack-3.3.80/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.3.80/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.3.80/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.3.80/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6876 2024-04-27 20:15:24.000000 flatpack-3.3.80/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.3.80/flatpack/session_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.3.80/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6413 2024-04-27 15:03:11.000000 flatpack-3.3.80/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:53:00.846840 flatpack-3.3.80/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     6009 2024-04-29 23:53:00.000000 flatpack-3.3.80/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      645 2024-04-29 23:53:00.000000 flatpack-3.3.80/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-04-29 23:53:00.000000 flatpack-3.3.80/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-04-29 23:53:00.000000 flatpack-3.3.80/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      297 2024-04-29 23:53:00.000000 flatpack-3.3.80/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-04-29 23:53:00.000000 flatpack-3.3.80/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-04-29 23:53:00.847671 flatpack-3.3.80/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)     1063 2024-04-29 23:52:53.000000 flatpack-3.3.80/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-20 00:47:10.898185 flatpack-3.3.9/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.3.9/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6336 2024-04-20 00:47:10.897865 flatpack-3.3.9/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5647 2024-04-20 00:46:44.000000 flatpack-3.3.9/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-20 00:47:10.895350 flatpack-3.3.9/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      132 2024-01-31 06:56:56.000000 flatpack-3.3.9/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.3.9/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.3.9/flatpack/datasets.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1057 2024-01-31 06:56:56.000000 flatpack-3.3.9/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    26884 2024-04-19 23:45:08.000000 flatpack-3.3.9/flatpack/main.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.3.9/flatpack/models.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-20 00:47:10.897190 flatpack-3.3.9/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.3.9/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.3.9/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.3.9/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6972 2024-04-06 18:22:51.000000 flatpack-3.3.9/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.3.9/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6394 2024-04-19 23:44:50.000000 flatpack-3.3.9/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-20 00:47:10.897511 flatpack-3.3.9/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6336 2024-04-20 00:47:10.000000 flatpack-3.3.9/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      485 2024-04-20 00:47:10.000000 flatpack-3.3.9/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-04-20 00:47:10.000000 flatpack-3.3.9/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-04-20 00:47:10.000000 flatpack-3.3.9/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      232 2024-04-20 00:47:10.000000 flatpack-3.3.9/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-04-20 00:47:10.000000 flatpack-3.3.9/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-04-20 00:47:10.898251 flatpack-3.3.9/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)      964 2024-04-20 00:47:04.000000 flatpack-3.3.9/setup.py
```

### Comparing `flatpack-3.3.80/LICENSE` & `flatpack-3.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.80/PKG-INFO` & `flatpack-3.3.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.3.80
+Version: 3.3.9
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: cryptography==42.0.5
 Requires-Dist: faiss-cpu==1.8.0
-Requires-Dist: fastapi==0.110.2
-Requires-Dist: hnswlib==0.8.0
+Requires-Dist: fastapi==0.110.1
 Requires-Dist: httpx==0.27.0
-Requires-Dist: huggingface-hub==0.22.2
-Requires-Dist: llama-cpp-python==0.2.65
 Requires-Dist: ngrok==1.2.0
 Requires-Dist: nltk==3.8.1
 Requires-Dist: olefile==0.47
-Requires-Dist: psutil==5.9.5
 Requires-Dist: pypdf==4.2.0
 Requires-Dist: requests==2.31.0
-Requires-Dist: sentence-transformers==2.7.0
+Requires-Dist: sentence-transformers==2.6.1
 Requires-Dist: toml==0.10.2
+Requires-Dist: torch==2.2.2
 Requires-Dist: uvicorn==0.29.0
 
 # Flatpack
 
 **NOTE:** Flatpack is currently experimental. Please refrain from using it in production environments.
 
 ## Ready-to-assemble AI
@@ -70,63 +67,60 @@
 
 ## License
 
 This project is released under [Apache-2.0](https://github.com/romlingroup/flatpack-ai/blob/main/LICENSE).
 
 ## install_requires
 
-**DISCLAIMER:** This information is only a technical reference, not an endorsement or legal advice. Before using any software for commercial purposes, perform compatibility checks and seek legal advice. You are responsible for ensuring compliance with licensing requirements.
+**DISCLAIMER:** The license compatibility information provided herein serves solely as a technical reference. It does not imply endorsement or legal advice. Users are encouraged to perform compatibility checks and consult with legal experts before commercially utilising any software. The user is responsible for ensuring compliance with applicable licensing requirements.
 
-Check out the [JLA - Compatibility Checker](https://joinup.ec.europa.eu/collection/eupl/solution/joinup-licensing-assistant/jla-compatibility-checker) (European Commission 2023).
+BSD 2-Clause "Simplified" (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original BSD-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/BSD-2-Clause/Apache-2.0)).
+
+BSD-3-Clause (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original BSD-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/BSD-3-Clause/Apache-2.0)).
+
+MIT (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original MIT-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/MIT/Apache-2.0)).
+
+*Check out the [JLA - Compatibility Checker](https://joinup.ec.europa.eu/collection/eupl/solution/joinup-licensing-assistant/jla-compatibility-checker) (European Commission 2023).*
 
 - **[beautifulsoup4](https://pypi.org/project/beautifulsoup4/)**\
   MIT License (MIT License) ([LICENSE](https://pypi.org/project/beautifulsoup4/))
 
 - **[cryptography](https://pypi.org/project/cryptography/)**\
   Apache Software License, BSD License (Apache-2.0 OR BSD-3-Clause) ([LICENSE](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE))
 
 - **[faiss-cpu](https://pypi.org/project/faiss-cpu/)**\
   MIT License (MIT License) ([LICENSE](https://github.com/kyamagu/faiss-wheels/blob/main/LICENSE))
 
 - **[fastapi](https://pypi.org/project/fastapi/)**\
   MIT License ([LICENSE](https://github.com/tiangolo/fastapi/blob/master/LICENSE))
 
-- **[hnswlib](https://pypi.org/project/hnswlib/)**\
-  Apache-2.0 license ([LICENSE](https://github.com/nmslib/hnswlib/blob/master/LICENSE))
-
 - **[httpx](https://pypi.org/project/httpx/)**\
   BSD License ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
 
-- **[huggingface-hub](https://pypi.org/project/huggingface-hub/)**\
-  Apache Software License (Apache) ([LICENSE](https://github.com/huggingface/huggingface_hub/blob/main/LICENSE))
-
-- **[llama-cpp-python](https://pypi.org/project/llama-cpp-python/)**\
-  MIT ([LICENSE](https://github.com/abetlen/llama-cpp-python/blob/main/LICENSE.md))
-
 - **[ngrok](https://pypi.org/project/ngrok/)**\
   MIT License (MIT OR Apache-2.0) ([LICENSE](https://github.com/ngrok/ngrok-python/blob/main/LICENSE-APACHE))
 
 - **[nltk](https://pypi.org/project/nltk/)**\
   Apache Software License (Apache License, Version 2.0) ([LICENSE](https://github.com/nltk/nltk/blob/develop/LICENSE.txt))
 
 - **[olefile](https://pypi.org/project/olefile/)**\
   BSD License (BSD) ([LICENSE](https://github.com/decalage2/olefile/blob/master/LICENSE.txt))
 
-- **[psutil](https://pypi.org/project/psutil/)**\
-  BSD License (BSD-3-Clause) ([LICENSE](https://github.com/giampaolo/psutil/blob/master/LICENSE))
-
 - **[pypdf](https://pypi.org/project/pypdf/)**\
   BSD License ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE))
 
 - **[requests](https://pypi.org/project/requests/)**\
   Apache Software License (Apache 2.0) ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
 
 - **[sentence-transformers](https://pypi.org/project/sentence-transformers/)**\
   Apache Software License (Apache License 2.0) ([LICENSE](https://github.com/UKPLab/sentence-transformers/blob/master/LICENSE))
 
 - **[toml](https://pypi.org/project/toml/)**\
   MIT License (MIT) ([LICENSE](https://github.com/uiri/toml/blob/master/LICENSE))
 
+- **[torch](https://pypi.org/project/torch/)**\
+  BSD License (BSD-3) ([LICENSE](https://github.com/pytorch/pytorch/blob/main/LICENSE))
+
 - **[uvicorn](https://pypi.org/project/uvicorn/)**\
   BSD License ([LICENSE](https://github.com/encode/uvicorn/blob/master/LICENSE.md))
 
-Last updated: 2024-04-27
+Last updated: 2024-04-20
```

### Comparing `flatpack-3.3.80/README.md` & `flatpack-3.3.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -43,63 +43,60 @@
 
 ## License
 
 This project is released under [Apache-2.0](https://github.com/romlingroup/flatpack-ai/blob/main/LICENSE).
 
 ## install_requires
 
-**DISCLAIMER:** This information is only a technical reference, not an endorsement or legal advice. Before using any software for commercial purposes, perform compatibility checks and seek legal advice. You are responsible for ensuring compliance with licensing requirements.
+**DISCLAIMER:** The license compatibility information provided herein serves solely as a technical reference. It does not imply endorsement or legal advice. Users are encouraged to perform compatibility checks and consult with legal experts before commercially utilising any software. The user is responsible for ensuring compliance with applicable licensing requirements.
 
-Check out the [JLA - Compatibility Checker](https://joinup.ec.europa.eu/collection/eupl/solution/joinup-licensing-assistant/jla-compatibility-checker) (European Commission 2023).
+BSD 2-Clause "Simplified" (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original BSD-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/BSD-2-Clause/Apache-2.0)).
+
+BSD-3-Clause (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original BSD-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/BSD-3-Clause/Apache-2.0)).
+
+MIT (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original MIT-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/MIT/Apache-2.0)).
+
+*Check out the [JLA - Compatibility Checker](https://joinup.ec.europa.eu/collection/eupl/solution/joinup-licensing-assistant/jla-compatibility-checker) (European Commission 2023).*
 
 - **[beautifulsoup4](https://pypi.org/project/beautifulsoup4/)**\
   MIT License (MIT License) ([LICENSE](https://pypi.org/project/beautifulsoup4/))
 
 - **[cryptography](https://pypi.org/project/cryptography/)**\
   Apache Software License, BSD License (Apache-2.0 OR BSD-3-Clause) ([LICENSE](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE))
 
 - **[faiss-cpu](https://pypi.org/project/faiss-cpu/)**\
   MIT License (MIT License) ([LICENSE](https://github.com/kyamagu/faiss-wheels/blob/main/LICENSE))
 
 - **[fastapi](https://pypi.org/project/fastapi/)**\
   MIT License ([LICENSE](https://github.com/tiangolo/fastapi/blob/master/LICENSE))
 
-- **[hnswlib](https://pypi.org/project/hnswlib/)**\
-  Apache-2.0 license ([LICENSE](https://github.com/nmslib/hnswlib/blob/master/LICENSE))
-
 - **[httpx](https://pypi.org/project/httpx/)**\
   BSD License ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
 
-- **[huggingface-hub](https://pypi.org/project/huggingface-hub/)**\
-  Apache Software License (Apache) ([LICENSE](https://github.com/huggingface/huggingface_hub/blob/main/LICENSE))
-
-- **[llama-cpp-python](https://pypi.org/project/llama-cpp-python/)**\
-  MIT ([LICENSE](https://github.com/abetlen/llama-cpp-python/blob/main/LICENSE.md))
-
 - **[ngrok](https://pypi.org/project/ngrok/)**\
   MIT License (MIT OR Apache-2.0) ([LICENSE](https://github.com/ngrok/ngrok-python/blob/main/LICENSE-APACHE))
 
 - **[nltk](https://pypi.org/project/nltk/)**\
   Apache Software License (Apache License, Version 2.0) ([LICENSE](https://github.com/nltk/nltk/blob/develop/LICENSE.txt))
 
 - **[olefile](https://pypi.org/project/olefile/)**\
   BSD License (BSD) ([LICENSE](https://github.com/decalage2/olefile/blob/master/LICENSE.txt))
 
-- **[psutil](https://pypi.org/project/psutil/)**\
-  BSD License (BSD-3-Clause) ([LICENSE](https://github.com/giampaolo/psutil/blob/master/LICENSE))
-
 - **[pypdf](https://pypi.org/project/pypdf/)**\
   BSD License ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE))
 
 - **[requests](https://pypi.org/project/requests/)**\
   Apache Software License (Apache 2.0) ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
 
 - **[sentence-transformers](https://pypi.org/project/sentence-transformers/)**\
   Apache Software License (Apache License 2.0) ([LICENSE](https://github.com/UKPLab/sentence-transformers/blob/master/LICENSE))
 
 - **[toml](https://pypi.org/project/toml/)**\
   MIT License (MIT) ([LICENSE](https://github.com/uiri/toml/blob/master/LICENSE))
 
+- **[torch](https://pypi.org/project/torch/)**\
+  BSD License (BSD-3) ([LICENSE](https://github.com/pytorch/pytorch/blob/main/LICENSE))
+
 - **[uvicorn](https://pypi.org/project/uvicorn/)**\
   BSD License ([LICENSE](https://github.com/encode/uvicorn/blob/master/LICENSE.md))
 
-Last updated: 2024-04-27
+Last updated: 2024-04-20
```

### Comparing `flatpack-3.3.80/flatpack/datasets.py` & `flatpack-3.3.9/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.80/flatpack/instructions.py` & `flatpack-3.3.9/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.80/flatpack/main.py` & `flatpack-3.3.9/flatpack/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,99 +4,149 @@
 import httpx
 import ngrok
 import os
 import re
 import requests
 import select
 import shlex
-import signal
+import stat
+import subprocess
 import sys
 import toml
 import uvicorn
 
-from .agent_manager import AgentManager
 from cryptography.fernet import Fernet
 from fastapi import FastAPI
-from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import JSONResponse
-from importlib.metadata import version
+from fastapi.middleware.cors import CORSMiddleware
 from .parsers import parse_toml_to_venv_script
 from pathlib import Path
 from sentence_transformers import SentenceTransformer
-from .session_manager import SessionManager
 from typing import List, Optional
 from .vector_manager import VectorManager
 
 CONFIG_FILE_PATH = os.path.join(os.path.expanduser("~"), ".fpk_config.toml")
-KEY_FILE_PATH = os.path.join(os.path.expanduser("~"), ".fpk_encryption_key")
+LOGGING_BATCH_SIZE = 10
 GITHUB_REPO_URL = "https://api.github.com/repos/romlingroup/flatpack"
 BASE_URL = "https://raw.githubusercontent.com/romlingroup/flatpack/main/warehouse"
-VERSION = version("flatpack")
+LOGGING_ENDPOINT = "https://fpk.ai/api/index.php"
+
+log_queue = []
 
 config = {
     "api_key": None
 }
 
+vm = VectorManager()
+
+
+def safe_cleanup():
+    try:
+        files_to_delete = ["flatpack.sh", "device.sh"]
+        current_directory = Path.cwd()
+
+        for filename in files_to_delete:
+            file_path = current_directory / filename
+
+            if file_path.exists():
+                file_path.unlink()
+                print(f"Deleted {filename}.")
+    except Exception as e:
+        print(f"Exception during safe_cleanup: {e}")
+
+
+atexit.register(safe_cleanup)
+
+
+class SessionManager:
+    def __enter__(self):
+        self.session = httpx.Client()
+        return self.session
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.session.close()
+
+
+def fpk_get_encryption_key():
+    key = os.environ.get("FPK_ENCRYPTION_KEY")
+    if key is not None:
+        return key.encode()
+    return None
+
+
+def fpk_encrypt_data(data, key):
+    fernet = Fernet(key)
+    if isinstance(data, str):
+        data = data.encode()
+    return fernet.encrypt(data)
+
+
+def fpk_decrypt_data(data, key):
+    fernet = Fernet(key)
+    if isinstance(data, str):
+        data = data.encode()
+    decrypted = fernet.decrypt(data)
+    return decrypted.decode()
+
+
+def fpk_set_secure_file_permissions(file_path):
+    os.chmod(file_path, stat.S_IRUSR | stat.S_IWUSR)
+
 
 class FPKEncryptionKeyError(Exception):
     """Custom exception for missing encryption key."""
     pass
 
 
-def fpk_build(directory: str):
-    """Build a model using a building script from the last unboxed flatpack."""
-    cache_file_path = Path('last_flatpack.cache')
-    print(f"Looking for cached flatpack in {cache_file_path}.")
+def fpk_set_api_key(api_key: str):
+    encryption_key = fpk_get_encryption_key()
+    if not encryption_key:
+        raise FPKEncryptionKeyError("❌ Encryption key not set.")
+    encrypted_api_key = fpk_encrypt_data(api_key, encryption_key)
+    config["api_key"] = encrypted_api_key.decode()
 
-    if directory and fpk_valid_directory_name(directory):
-        print(f"Using provided directory: {directory}")
-        last_unboxed_flatpack = directory
-    elif cache_file_path.exists():
-        print(f"Found cached flatpack in {cache_file_path}.")
-        last_unboxed_flatpack = cache_file_path.read_text().strip()
-        if not fpk_valid_directory_name(last_unboxed_flatpack):
-            print(f"❌ Invalid directory name from cache: '{last_unboxed_flatpack}'.")
-            return
-    else:
-        print("❌ No cached flatpack found, and no valid directory provided.")
-        return
+    with open(CONFIG_FILE_PATH, "w") as config_file:
+        toml.dump(config, config_file)
+    fpk_set_secure_file_permissions(CONFIG_FILE_PATH)
 
-    building_script_path = Path(last_unboxed_flatpack) / 'build' / 'build.sh'
-    if not building_script_path.exists():
-        print(f"❌ Building script not found in {last_unboxed_flatpack}.")
-        return
 
-    safe_script_path = shlex.quote(str(building_script_path))
+def fpk_get_api_key() -> Optional[str]:
+    encryption_key = fpk_get_encryption_key()
+    if not encryption_key or not os.path.exists(CONFIG_FILE_PATH):
+        return None
 
-    result = os.system(f"bash -u {safe_script_path}")
-    if result != 0:
-        print("❌ An error occurred while executing the build script.")
-    else:
-        print("✅ Build script executed successfully.")
+    with open(CONFIG_FILE_PATH, "r") as config_file:
+        loaded_config = toml.load(config_file)
+        encrypted_api_key_str = loaded_config.get("api_key")
+        if encrypted_api_key_str:
+            encrypted_api_key_bytes = encrypted_api_key_str.encode()
+            return fpk_decrypt_data(encrypted_api_key_bytes, encryption_key)
+        else:
+            return None
 
 
 def fpk_cache_last_flatpack(directory_name: str):
     """Cache the last unboxed flatpack's directory name to a file within the corresponding build directory."""
+    # The directory where the flatpack is unboxed, which includes the build directory
     flatpack_dir = Path.cwd()
-    flatpack_dir.mkdir(parents=True, exist_ok=True)
+    flatpack_dir.mkdir(parents=True, exist_ok=True)  # Ensure the directory exists
 
+    # The cache file that contains the name of the last unboxed flatpack
     cache_file_path = flatpack_dir / 'last_flatpack.cache'
     with open(cache_file_path, 'w') as f:
         f.write(directory_name)
 
 
-def fpk_check_ngrok_auth():
-    """Check if the NGROK_AUTHTOKEN environment variable is set."""
-    ngrok_auth_token = os.environ.get('NGROK_AUTHTOKEN')
-    if not ngrok_auth_token:
-        print("❌ Error: NGROK_AUTHTOKEN is not set. Please set it using:")
-        print("export NGROK_AUTHTOKEN='your_ngrok_auth_token'")
-        sys.exit(1)
-    else:
-        print("NGROK_AUTHTOKEN is set.")
+def fpk_get_last_flatpack(directory_name: str) -> Optional[str]:
+    """Retrieve the last unboxed flatpack's directory name from the cache file within the correct build directory."""
+    flatpack_dir = Path.cwd()
+    cache_file_path = flatpack_dir / 'last_flatpack.cache'
+    if cache_file_path.exists():
+        return cache_file_path.read_text().strip()
+    return None
 
 
 def fpk_colorize(text, color):
     """Colorize a given text with the specified color.
 
     Args:
         text (str): The text to be colorized.
@@ -115,20 +165,14 @@
         "red": "\033[91m",
         "white": "\033[97m",
         "yellow": "\033[93m"
     }
     return colors[color] + text + colors["default"]
 
 
-def fpk_decrypt_data(encrypted_data: str, key: bytes) -> str:
-    """Decrypt data using the provided key."""
-    fernet = Fernet(key)
-    return fernet.decrypt(encrypted_data.encode()).decode()
-
-
 def fpk_display_disclaimer(directory_name: str):
     """Display a disclaimer message with details about a specific flatpack.
 
     Args:
         directory_name (str): Name of the flatpack directory.
     """
     disclaimer_template = """
@@ -163,20 +207,14 @@
 https://fpk.ai/w/{}
 """.format(directory_name)
 
     please_note_colored = fpk_colorize(please_note_content, "yellow")
     print(disclaimer_template.format(please_note=please_note_colored))
 
 
-def fpk_encrypt_data(data: str, key: bytes) -> str:
-    """Encrypt data using the provided key."""
-    fernet = Fernet(key)
-    return fernet.encrypt(data.encode()).decode()
-
-
 def fpk_fetch_flatpack_toml_from_dir(directory_name: str, session: httpx.Client) -> Optional[str]:
     """Fetch the flatpack TOML configuration from a specific directory.
 
     Args:
         directory_name (str): Name of the flatpack directory.
         session (httpx.Client): HTTP client session for making requests.
 
@@ -225,54 +263,80 @@
     for root, _, files in os.walk(directory_path):
         for file in files:
             if any(file.endswith(fmt) for fmt in model_file_formats):
                 model_files.append(os.path.join(root, file))
     return model_files
 
 
-def fpk_get_api_key() -> Optional[str]:
-    """Retrieve and decrypt the API key from the configuration file."""
-    if not os.path.exists(CONFIG_FILE_PATH):
-        return None
+def fpk_unbox(directory_name: str, session, verbose: bool = False, local: bool = False):
+    # Define the directory where the flatpack will be unboxed, which includes the build directory
+    flatpack_dir = Path.cwd() / directory_name
+    flatpack_dir.mkdir(parents=True, exist_ok=True)  # Ensure the directory exists
+    build_dir = flatpack_dir / "build"
+    build_dir.mkdir(parents=True, exist_ok=True)  # Explicitly ensure that build_dir exists
 
-    try:
-        with open(CONFIG_FILE_PATH, 'r') as config_file:
-            loaded_config = toml.load(config_file)
-        encrypted_api_key = loaded_config.get('api_key')
-
-        if encrypted_api_key:
-            encryption_key = fpk_get_or_create_encryption_key()
-            return fpk_decrypt_data(encrypted_api_key, encryption_key)
-    except Exception as e:
-        print(f"Error decrypting API key: {e}")
+    # Define the path for the temporary flatpack TOML file
+    temp_toml_path = build_dir / 'temp_flatpack.toml'
 
-    return None
+    # Handle local directory unboxing
+    if local:
+        local_directory_path = flatpack_dir  # Use flatpack_dir directly since it already points to the correct location
+        # Assuming flatpack.toml is required in the directory
+        toml_path = local_directory_path / 'flatpack.toml'
+        if not toml_path.exists():
+            print(f"❌ flatpack.toml not found in the specified directory: '{directory_name}'.")
+            return
+        toml_content = toml_path.read_text()
+    else:
+        # Existing GitHub fetch logic
+        if not fpk_valid_directory_name(directory_name):
+            print(f"❌ Invalid directory name: '{directory_name}'.")
+            return
 
+        toml_content = fpk_fetch_flatpack_toml_from_dir(directory_name, session)
+        if not toml_content:
+            print(f"❌ Error: Failed to fetch TOML content for '{directory_name}'.")
+            return
 
-def fpk_get_last_flatpack(directory_name: str) -> Optional[str]:
-    """Retrieve the last unboxed flatpack's directory name from the cache file within the correct build directory."""
-    flatpack_dir = Path.cwd()
-    cache_file_path = flatpack_dir / 'last_flatpack.cache'
-    if cache_file_path.exists():
-        return cache_file_path.read_text().strip()
-    return None
+    # Write the TOML content to the temporary file
+    temp_toml_path.write_text(toml_content)
 
+    # Generate the bash script content from the TOML file
+    bash_script_content = parse_toml_to_venv_script(str(temp_toml_path), '3.11.8', directory_name)
+
+    # Save the bash script in the build directory
+    bash_script_path = build_dir / 'flatpack.sh'
+    bash_script_path.write_text(bash_script_content)
+
+    # Remove the temporary TOML file after it's no longer needed
+    temp_toml_path.unlink()
+
+    print(f"📦 Unboxing {directory_name}...")
+
+    # Execute the bash script
+    command = ["bash", str(bash_script_path)]
 
-def fpk_get_or_create_encryption_key() -> bytes:
-    """Retrieve or generate and save an encryption key."""
     try:
-        with open(KEY_FILE_PATH, "rb") as key_file:
-            key = key_file.read()
-    except FileNotFoundError:
-        print("No encryption key found. Generating a new key for persistent use.")
-        key = Fernet.generate_key()
-        with open(KEY_FILE_PATH, "wb") as key_file:
-            key_file.write(key)
-        os.chmod(KEY_FILE_PATH, 0o600)
-    return key
+        if verbose:
+            process = subprocess.Popen(command)
+            process.wait()
+        else:
+            process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+            stdout, stderr = process.communicate()
+            if process.returncode != 0:
+                print("❌ Error: Failed to execute the bash script.")
+                if verbose:
+                    print("Standard Output:", stdout.decode())
+                    print("Standard Error:", stderr.decode())
+
+        if process.returncode == 0:
+            fpk_cache_last_flatpack(directory_name)
+            print(f"🎉 All done!")
+    except subprocess.SubprocessError as e:
+        print(f"❌ An error occurred: {e}")
 
 
 def fpk_is_raspberry_pi():
     """Check if we're running on a Raspberry Pi."""
     try:
         with open('/proc/cpuinfo', 'r') as f:
             for line in f:
@@ -292,102 +356,138 @@
     Returns:
     - str: A newline-separated string of directory names.
     """
     dirs = fpk_fetch_github_dirs(session)
     return "\n".join(dirs)
 
 
-def fpk_safe_cleanup():
-    """Safely clean up temporary files."""
-    try:
-        files_to_delete = ["flatpack.sh"]
-        current_directory = Path.cwd()
+def fpk_log_to_api(message: str, session: httpx.Client, api_key: Optional[str] = None,
+                   model_name: str = "YOUR_MODEL_NAME"):
+    """Log a message to the API.
 
-        for filename in files_to_delete:
-            file_path = current_directory / filename
+    Args:
+        message (str): The log message.
+        session (httpx.Client): HTTP client session for making requests.
+        api_key (Optional[str]): The API key for authentication. Defaults to the global API_KEY.
+        model_name (str): Name of the model associated with the log. Defaults to "YOUR_MODEL_NAME".
+    """
+    if not api_key:
+        api_key = config["api_key"]
+        if not api_key:
+            print("❌ API key not set.")
+            return
 
-            if file_path.exists():
-                file_path.unlink()
-                print(f"Deleted {filename}.")
-    except Exception as e:
-        print(f"Exception during safe_cleanup: {e}")
+    headers = {
+        "Content-Type": "application/json"
+    }
+    params = {
+        "endpoint": "log-message",
+        "api_key": api_key
+    }
+    data = {
+        "model_name": model_name,
+        "log_message": message
+    }
 
+    try:
+        response = session.post(LOGGING_ENDPOINT, params=params, json=data, headers=headers, timeout=10)
+    except httpx.RequestError as e:
+        print(f"Failed to send request: {e}")
 
-def fpk_set_api_key(api_key: str):
-    """Set the API key in the configuration file."""
-    global config
 
-    """Set and encrypt the API key."""
-    encryption_key = fpk_get_or_create_encryption_key()
-    encrypted_api_key = fpk_encrypt_data(api_key, encryption_key)
-    config = {'api_key': encrypted_api_key}
+def fpk_process_output(output, session, last_unboxed_flatpack):
+    """Process output and log it."""
+    # Get the API key for logging
+    api_key = fpk_get_api_key()
 
-    with open(CONFIG_FILE_PATH, "w") as config_file:
-        toml.dump(config, config_file)
-    os.chmod(CONFIG_FILE_PATH, 0o600)
-    print("API key set successfully!")
+    # Regular expression pattern to match ANSI escape codes
+    ansi_escape = re.compile(r'\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])')
 
-    try:
-        test_key = fpk_get_api_key()
-        if test_key == api_key:
-            print("Verification successful: API key can be decrypted correctly.")
-        else:
-            print("Verification failed: Decrypted key does not match the original.")
-    except Exception as e:
-        print(f"Error during API key verification: {e}")
+    # Iterate over each line in the output
+    for line in output.splitlines():
+        # Remove any leading or trailing whitespace
+        line = line.strip()
 
+        # Remove ANSI escape codes from the line
+        line = ansi_escape.sub('', line)
 
-def fpk_set_secure_file_permissions(file_path):
-    """Set secure file permissions for the specified file."""
-    os.chmod(file_path, stat.S_IRUSR | stat.S_IWUSR)
+        # If the line isn't empty, process it
+        if line:
+            # Display the line with a prefix
+            print(f"(*) {line}", flush=True)
 
+            # If we have an API key, log the line to the API
+            if api_key:
+                fpk_log_to_api(line, session, api_key=api_key, model_name=last_unboxed_flatpack)
 
-def fpk_unbox(directory_name: str, session, verbose: bool = False, local: bool = False):
-    """Unbox a flatpack from GitHub or a local directory."""
-    flatpack_dir = Path.cwd() / directory_name
-    flatpack_dir.mkdir(parents=True, exist_ok=True)
-    build_dir = flatpack_dir / "build"
-    build_dir.mkdir(parents=True, exist_ok=True)
 
-    temp_toml_path = build_dir / 'temp_flatpack.toml'
+def fpk_build(directory: str, session: httpx.Client = None):
+    """Build a model using a building script from the last unboxed flatpack."""
+    cache_file_path = Path('last_flatpack.cache')
+    print(f"Looking for cached flatpack in {cache_file_path}.")
 
-    if local:
-        local_directory_path = flatpack_dir
-        toml_path = local_directory_path / 'flatpack.toml'
-        if not toml_path.exists():
-            print(f"❌ flatpack.toml not found in the specified directory: '{directory_name}'.")
+    if directory and fpk_valid_directory_name(directory):
+        print(f"Using provided directory: {directory}")
+        last_unboxed_flatpack = directory
+    elif cache_file_path.exists():
+        print(f"Found cached flatpack in {cache_file_path}.")
+        last_unboxed_flatpack = cache_file_path.read_text().strip()
+        if not fpk_valid_directory_name(last_unboxed_flatpack):
+            print(f"❌ Invalid directory name from cache: '{last_unboxed_flatpack}'.")
             return
-        toml_content = toml_path.read_text()
     else:
-        if not fpk_valid_directory_name(directory_name):
-            print(f"❌ Invalid directory name: '{directory_name}'.")
-            return
-
-        toml_content = fpk_fetch_flatpack_toml_from_dir(directory_name, session)
-        if not toml_content:
-            print(f"❌ Error: Failed to fetch TOML content for '{directory_name}'.")
-            return
-
-    temp_toml_path.write_text(toml_content)
+        print("❌ No cached flatpack found, and no valid directory provided.")
+        return
 
-    bash_script_content = parse_toml_to_venv_script(str(temp_toml_path), '3.11.8', directory_name)
-    bash_script_path = build_dir / 'flatpack.sh'
-    bash_script_path.write_text(bash_script_content)
+    building_script_path = Path(last_unboxed_flatpack) / 'build' / 'build.sh'
+    if not building_script_path.exists():
+        print(f"❌ Building script not found in {last_unboxed_flatpack}.")
+        return
 
-    temp_toml_path.unlink()
+    env = dict(os.environ, PYTHONUNBUFFERED="1")
+    safe_script_path = shlex.quote(str(building_script_path))
 
-    print(f"📦 Unboxing {directory_name}...")
-    command = f"bash {bash_script_path}"
-    result = os.system(command)
+    try:
+        proc = subprocess.Popen(["bash", "-u", safe_script_path], stdin=subprocess.PIPE,
+                                stdout=subprocess.PIPE, stderr=subprocess.PIPE, bufsize=1, universal_newlines=True,
+                                env=env)
+
+        outputs = [proc.stdout, proc.stderr]
+
+        while True:
+            retcode = proc.poll()
+            if retcode is not None:  # Subprocess has exited
+                break
+
+            rlist, _, _ = select.select(outputs, [], [], 0.1)
+            for r in rlist:
+                line = r.readline()
+                if line:
+                    fpk_process_output(line, session, last_unboxed_flatpack)
+
+                    if not line.endswith('\n'):
+                        try:
+                            user_input = input()
+                            print(user_input, file=proc.stdin)
+                        except EOFError:
+                            # Handle end-of-file condition (e.g., if input redirection is closed)
+                            break
 
-    if result != 0:
-        print("❌ Error: Failed to execute the bash script.")
-    else:
-        fpk_cache_last_flatpack(directory_name)
-        print(f"🎉 All done!")
+    except subprocess.SubprocessError as e:
+        print(f"❌ An error occurred while executing the subprocess: {e}")
+    except KeyboardInterrupt:
+        proc.terminate()
+        try:
+            proc.wait(timeout=5)  # Wait up to 5 seconds for proc to terminate
+        except subprocess.TimeoutExpired:
+            proc.kill()  # Forcefully kill if not terminated after timeout
+    finally:
+        # Ensure that the proc.wait() is in the finally block to guarantee it executes.
+        if proc and proc.poll() is None:  # Check if proc is still running
+            proc.wait()
 
 
 def fpk_valid_directory_name(name: str) -> bool:
     """
     Validate that the directory name contains only alphanumeric characters, dashes, and underscores.
 
     Args:
@@ -395,16 +495,14 @@
 
     Returns:
         bool: True if the name is valid, False otherwise.
     """
     return re.match(r'^[\w-]+$', name) is not None
 
 
-atexit.register(fpk_safe_cleanup)
-
 app = FastAPI()
 
 app.add_middleware(
     CORSMiddleware,
     allow_origins=["*"],
     allow_credentials=True,
     allow_methods=["*"],
@@ -418,289 +516,195 @@
 
 
 @app.get("/test")
 async def test_endpoint():
     return JSONResponse(content={"message": "Hello, World!"})
 
 
-def setup_arg_parser():
-    # Create the top-level parser
-    parser = argparse.ArgumentParser(description='Flatpack command line interface')
-    subparsers = parser.add_subparsers(dest='command', help='Available commands')
-
-    # General commands
-    parser_list = subparsers.add_parser('list', help='List available flatpack directories.')
-    parser_list.set_defaults(func=lambda args, session: fpk_cli_handle_list(args, session))
-
-    parser_find = subparsers.add_parser('find', help='Find model files in the current directory.')
-    parser_find.set_defaults(func=lambda args, session: fpk_cli_handle_find(args, session))
-
-    parser_help = subparsers.add_parser('help', help='Display help for commands.')
-    parser_help.set_defaults(func=fpk_cli_handle_help)
-
-    parser_version = subparsers.add_parser('version', help='Display the version of flatpack.')
-    parser_version.set_defaults(func=fpk_cli_handle_version)
-
-    # API Key management
-    parser_api_key = subparsers.add_parser('api-key', help='API key management commands')
-    api_key_subparsers = parser_api_key.add_subparsers(dest='api_key_command')
-
-    # Set API key
-    parser_set_api = api_key_subparsers.add_parser('set', help='Set the API key')
-    parser_set_api.add_argument('api_key', type=str, help='API key to set')
-    parser_set_api.set_defaults(func=lambda args, session: fpk_cli_handle_set_api_key(args, session))
-
-    # Get API key
-    parser_get_api = api_key_subparsers.add_parser('get', help='Get the current API key')
-    parser_get_api.set_defaults(func=lambda args, session: fpk_cli_handle_get_api_key(args, session))
-
-    # Unbox commands
-    parser_unbox = subparsers.add_parser('unbox', help='Unbox a flatpack from GitHub or a local directory.')
-    parser_unbox.add_argument('input', nargs='?', default=None, help='The name of the flatpack to unbox.')
-    parser_unbox.add_argument('--local', action='store_true', help='Unbox from a local directory instead of GitHub.')
-    parser_unbox.add_argument('--verbose', action='store_true', help='Display detailed outputs for debugging.')
-    parser_unbox.set_defaults(func=lambda args, session: fpk_cli_handle_unbox(args, session))
-
-    # Build commands
-    parser_build = subparsers.add_parser('build',
-                                         help='Build a model using the building script from the last unboxed flatpack.')
-    parser_build.add_argument('directory', nargs='?', default=None, help='The directory of the flatpack to build.')
-    parser_build.add_argument('--verbose', action='store_true', help='Display detailed outputs for debugging.')
-    parser_build.set_defaults(func=lambda args, session: fpk_cli_handle_build(args, session))
-
-    # Run server
-    parser_run = subparsers.add_parser('run', help='Run the FastAPI server.')
-    parser_run.set_defaults(func=lambda args, session: fpk_cli_handle_run(args, session))
-
-    # Vector database management
-    parser_vector = subparsers.add_parser('vector', help='Vector database management')
-    vector_subparsers = parser_vector.add_subparsers(dest='vector_command')
-
-    parser_add_text = vector_subparsers.add_parser('add-texts',
-                                                   help='Add new texts to generate embeddings and store them.')
-    parser_add_text.add_argument('texts', nargs='+', help='Texts to add.')
-    parser_add_text.add_argument('--data-dir', type=str, default='.',
-                                 help='Directory path for storing the vector database and metadata files.')
-    parser_add_text.set_defaults(func=lambda args, session: fpk_cli_handle_vector_commands(args, session))
-
-    parser_search_text = vector_subparsers.add_parser('search-text',
-                                                      help='Search for texts similar to the given query.')
-    parser_search_text.add_argument('query', help='Text query to search for.')
-    parser_search_text.add_argument('--data-dir', type=str, default='.',
-                                    help='Directory path for storing the vector database and metadata files.')
-    parser_search_text.set_defaults(func=lambda args, session: fpk_cli_handle_vector_commands(args, session))
-
-    parser_add_pdf = vector_subparsers.add_parser('add-pdf', help='Add text from a PDF file to the vector database.')
-    parser_add_pdf.add_argument('pdf_path', help='Path to the PDF file to add.')
-    parser_add_pdf.add_argument('--data-dir', type=str, default='.',
-                                help='Directory path for storing the vector database and metadata files.')
-    parser_add_pdf.set_defaults(func=lambda args, session: fpk_cli_handle_vector_commands(args, session))
-
-    parser_add_url = vector_subparsers.add_parser('add-url', help='Add text from a URL to the vector database.')
-    parser_add_url.add_argument('url', help='URL to add.')
-    parser_add_url.add_argument('--data-dir', type=str, default='.',
-                                help='Directory path for storing the vector database and metadata files.')
-    parser_add_url.set_defaults(func=lambda args, session: fpk_cli_handle_vector_commands(args, session))
-
-    parser_add_wikipedia_page = vector_subparsers.add_parser('add-wikipedia',
-                                                             help='Add text from a Wikipedia page to the vector database.')
-    parser_add_wikipedia_page.add_argument('page_title', help='The title of the Wikipedia page to add.')
-    parser_add_wikipedia_page.add_argument('--data-dir', type=str, default='.',
-                                           help='Directory path for storing the vector database and metadata files.')
-    parser_add_wikipedia_page.set_defaults(func=lambda args, session: fpk_cli_handle_vector_commands(args, session))
-
-    # Add commands for agents
-    parser_agents = subparsers.add_parser('agents', help='Manage agents')
-    agent_subparsers = parser_agents.add_subparsers(dest='agent_command', help='Available agent commands')
-
-    # Add command to spawn an agent
-    parser_spawn = agent_subparsers.add_parser('spawn', help='Spawn a new agent with a script')
-    parser_spawn.add_argument('script_path', type=str, help='Path to the script to execute')
-    parser_spawn.set_defaults(func=fpk_cli_handle_spawn_agent)
-
-    # Add command to list active agents
-    parser_list = agent_subparsers.add_parser('list', help='List active agents')
-    parser_list.set_defaults(func=fpk_cli_handle_list_agents)
-
-    # Add command to terminate an agent
-    parser_terminate = agent_subparsers.add_parser('terminate', help='Terminate an active agent')
-    parser_terminate.add_argument('pid', type=int, help='Process ID of the agent to terminate')
-    parser_terminate.set_defaults(func=fpk_cli_handle_terminate_agent)
-
-    return parser
-
-
-def fpk_cli_handle_add_pdf(pdf_path, vm):
-    if not os.path.exists(pdf_path):
-        print(f"❌ PDF file does not exist: '{pdf_path}'.")
-        return
-    vm.add_pdf(pdf_path)
-    print(f"✅ Added text from PDF: '{pdf_path}' to the vector database.")
-
-
-def fpk_cli_handle_add_url(url, vm):
-    try:
-        response = requests.head(url, allow_redirects=True, timeout=5)
-        if response.status_code >= 200 and response.status_code < 400:
-            vm.add_url(url)
-            print(f"✅ Added text from URL: '{url}' to the vector database.")
-        else:
-            print(f"❌ URL is not accessible: '{url}'. HTTP Status Code: {response.status_code}")
-    except requests.RequestException as e:
-        print(f"❌ Failed to access URL: '{url}'. Error: {e}")
-
-
-def fpk_cli_handle_build(args, session):
-    directory_name = args.directory
-    fpk_build(directory_name)
-
-
-def fpk_cli_handle_find(args, session):
-    print(fpk_find_models())
-
-
-def fpk_cli_handle_get_api_key(args, session):
-    print("Retrieving API key...")
-    print(fpk_get_api_key())
-
-
-def fpk_cli_handle_help(args, session):
-    parser = setup_arg_parser()
-    parser.print_help()
-
-
-def fpk_cli_handle_list(args, session):
-    print(fpk_list_directories(session))
-
-
-def fpk_cli_handle_list_agents(args, session):
-    """List active agents."""
-    agent_manager = AgentManager()
-    agent_manager.list_agents()
-
-
-def fpk_cli_handle_run(args, session):
-    fpk_check_ngrok_auth()
-    try:
-        port = 8000
-        listener = ngrok.forward(port, authtoken_from_env=True)
-        print(f"Ingress established at {listener.url()}")
-        uvicorn.run(app, host="0.0.0.0", port=port)
-    except KeyboardInterrupt:
-        print("❌ FastAPI server has been stopped.")
-    except Exception as e:
-        print(f"❌ An unexpected error occurred during server run: {e}")
-    finally:
-        ngrok.disconnect(listener.url())
-
-
-def fpk_cli_handle_set_api_key(args, session):
-    print(f"Setting API key: {args.api_key}")
-    global config
-    api_key = args.api_key
-
-    """Set and encrypt the API key."""
-    encryption_key = fpk_get_or_create_encryption_key()
-    encrypted_api_key = fpk_encrypt_data(api_key, encryption_key)
-    config = {'api_key': encrypted_api_key}
-
-    with open(CONFIG_FILE_PATH, "w") as config_file:
-        toml.dump(config, config_file)
-    os.chmod(CONFIG_FILE_PATH, 0o600)
-    print("API key set successfully!")
-
-    try:
-        test_key = fpk_get_api_key()
-        if test_key == api_key:
-            print("Verification successful: API key can be decrypted correctly.")
-        else:
-            print("Verification failed: Decrypted key does not match the original.")
-    except Exception as e:
-        print(f"Error during API key verification: {e}")
-
-
-def fpk_cli_handle_spawn_agent(args, session):
-    """Spawn a new agent with a script."""
-    agent_manager = AgentManager()
-    pid = agent_manager.spawn_agent(args.script_path)
-    print(f"Agent spawned with PID: {pid}")
-
-
-def fpk_cli_handle_terminate_agent(args, session):
-    """Terminate an active agent."""
-    agent_manager = AgentManager()
-    agent_manager.terminate_agent(args.pid)
-
-
-def fpk_cli_handle_unbox(args, session):
-    if not args.input:
-        print("❌ Please specify a flatpack for the unbox command.")
-        return
-
-    directory_name = args.input
-    if not args.local and directory_name not in fpk_fetch_github_dirs(session):
-        print(f"❌ The flatpack '{directory_name}' does not exist.")
-        return
-
-    if args.local:
-        local_directory_path = Path(directory_name)
-        if not local_directory_path.exists() or not local_directory_path.is_dir():
-            print(f"❌ Local directory does not exist: '{directory_name}'.")
-            return
-        toml_path = local_directory_path / 'flatpack.toml'
-        if not toml_path.exists():
-            print(f"❌ flatpack.toml not found in the specified directory: '{directory_name}'.")
-            return
-
-    print("Verbose mode:", args.verbose)
-    print(f"✅ Directory name resolved to: '{directory_name}'")
-    fpk_unbox(directory_name, session, verbose=args.verbose, local=args.local)
-
-
-def fpk_cli_handle_version(args, session):
-    print(VERSION)
-
-
-def fpk_cli_handle_vector_commands(args, session):
-    print("Handling vector commands...")
-
-    vm = VectorManager(model_name='all-MiniLM-L6-v2', directory=getattr(args, 'data_dir', '.'))
-
-    if args.vector_command == 'add-texts':
-        vm.add_texts(args.texts)
-        print(f"Added {len(args.texts)} texts to the database.")
-    elif args.vector_command == 'search-text':
-        results = vm.search_vectors(args.query)
-        if results:
-            print("Search results:")
-            for result in results:
-                print(f"{result['id']}: {result['text']}\n")
-        else:
-            print("No results found.")
-    elif args.vector_command == 'add-pdf':
-        fpk_cli_handle_add_pdf(args.pdf_path, vm)
-    elif args.vector_command == 'add-url':
-        fpk_cli_handle_add_url(args.url, vm)
-    elif args.vector_command == 'add-wikipedia':
-        vm.add_wikipedia_page(args.page_title)
-        print(f"✅ Added text from Wikipedia page: '{args.page_title}' to the vector database.")
-
-
 def main():
-    """Main entry point for the flatpack command line interface."""
     try:
         with SessionManager() as session:
-            parser = setup_arg_parser()
+            parser = argparse.ArgumentParser(description='flatpack command line interface')
+            subparsers = parser.add_subparsers(dest='command', help='Available commands')
+
+            # Adding subparsers for each command
+            subparsers.add_parser('list', help='List available flatpack directories.')
+            subparsers.add_parser('find', help='Find model files in the current directory.')
+            subparsers.add_parser('help', help='Display help for commands.')
+            subparsers.add_parser('get-api-key', help='Get the current API key.')
+
+            # Adjusting the subparser setup for the 'unbox' command
+            parser_unbox = subparsers.add_parser('unbox', help='Unbox a flatpack from GitHub or a local directory.')
+            parser_unbox.add_argument('input', nargs='?', default=None, help='The name of the flatpack to unbox.')
+            parser_unbox.add_argument('--local', action='store_true',
+                                      help='Unbox from a local directory instead of GitHub.')
+            parser.add_argument('--verbose', action='store_true', help='Display detailed outputs for debugging.')
+
+            subparsers.add_parser('run', help='Run the FastAPI server.')
+            subparsers.add_parser('set-api-key', help='Set the API key.')
+
+            # Adjusting the subparser setup for the 'build' command
+            parser_build = subparsers.add_parser('build',
+                                                 help='Build a model using the building script from the last unboxed flatpack.')
+            parser_build.add_argument('directory', nargs='?', default=None,
+                                      help='The directory of the flatpack to build.')
+
+            subparsers.add_parser('version', help='Display the version of flatpack.')
+
+            # Adding subparsers for 'add-text' and 'search-text' commands specifically because they need additional arguments
+            parser_add_text = subparsers.add_parser('vector-add-texts',
+                                                    help='Add new texts to generate embeddings and store them.')
+            parser_add_text.add_argument('texts', nargs='+', help='Texts to add.')
+
+            parser_search_text = subparsers.add_parser('vector-search-text',
+                                                       help='Search for texts similar to the given query.')
+            parser_search_text.add_argument('query', help='Text query to search for.')
+
+            parser_add_pdf = subparsers.add_parser('vector-add-pdf',
+                                                   help='Add text from a PDF file to the vector database.')
+            parser_add_pdf.add_argument('pdf_path', help='Path to the PDF file to add.')
+
+            parser_add_url = subparsers.add_parser('vector-add-url', help='Add text from a URL to the vector database.')
+            parser_add_url.add_argument('url', help='URL to add.')
+
+            parser_add_wikipedia_page = subparsers.add_parser('vector-add-wikipedia-page',
+                                                              help='Add text from a Wikipedia page to the vector database.')
+            parser_add_wikipedia_page.add_argument('page_title', help='The title of the Wikipedia page to add.')
+
             args = parser.parse_args()
 
-            if hasattr(args, 'func'):
-                args.func(args, session)
+            fpk_get_api_key()
+
+            if args.command == 'vector-add-texts':
+                vm.add_texts(args.texts)
+                print(f"Added {len(args.texts)} texts to the database.")
+            elif args.command == 'vector-search':
+                if not vm.is_index_ready():
+                    print("Vector index is not ready. Skipping search.")
+                    return
+
+                try:
+                    results = vm.search_vectors(args.query)
+                    if results:
+                        print("Search results:")
+                        for result in results:
+                            id = result["id"]
+                            distance = result["distance"]
+                            text = result["text"]
+                            print(f"({distance}) {id}: {text}\n")
+                    else:
+                        print("No results found.")
+                except ValueError as e:
+                    print(f"Error: {e}")
+                except Exception as e:
+                    print(f"❌ An unexpected error occurred.")
+            elif args.command == 'vector-add-pdf':
+                pdf_path = args.pdf_path
+                if not os.path.exists(pdf_path):
+                    print(f"❌ PDF file does not exist: '{pdf_path}'.")
+                    return
+                vm.add_pdf(pdf_path)
+                print(f"✅ Added text from PDF: '{pdf_path}' to the vector database.")
+            elif args.command == 'vector-add-url':
+                url = args.url
+                try:
+                    response = requests.head(url, allow_redirects=True, timeout=5)
+                    if response.status_code >= 200 and response.status_code < 400:
+                        vm.add_url(url)
+                        print(f"✅ Added text from URL: '{url}' to the vector database.")
+                    else:
+                        print(f"❌ URL is not accessible: '{url}'. HTTP Status Code: {response.status_code}")
+                except requests.RequestException as e:
+                    print(f"❌ Failed to access URL: '{url}'. Error: {e}")
+            elif args.command == 'vector-add-wikipedia-page':
+                page_title = args.page_title
+                vm.add_wikipedia_page(page_title)
+                print(f"✅ Added text from Wikipedia page: '{page_title}' to the vector database.")
+            elif args.command == "find":
+                print(fpk_find_models())
+            elif args.command == "help":
+                print("[HELP]")
+            elif args.command == "get-api-key":
+                print(fpk_get_api_key())
+            elif args.command == "unbox":
+
+                if not args.input:
+                    print("❌ Please specify a flatpack for the unbox command.")
+                    return
+
+                directory_name = args.input
+
+                if not args.local:
+                    # If not unboxing from a local directory, check if the flatpack exists in GitHub directories
+                    existing_dirs = fpk_fetch_github_dirs(session)
+                    if directory_name not in existing_dirs:
+                        print(f"❌ The flatpack '{directory_name}' does not exist.")
+                        return
+
+                    # Display disclaimer and proceed with unboxing
+                    fpk_display_disclaimer(directory_name)
+
+                    while True:
+                        user_response = input().strip().upper()
+                        if user_response == "YES":
+                            break
+                        elif user_response == "NO":
+                            print("❌ Unboxing aborted by user.")
+                            return
+                        else:
+                            print("❌ Invalid input. Please type 'YES' to accept or 'NO' to decline.")
+
+                if args.local:
+                    # For local unboxing, directly proceed without GitHub check
+                    local_directory_path = Path(directory_name)
+                    if not local_directory_path.exists() or not local_directory_path.is_dir():
+                        print(f"❌ Local directory does not exist: '{directory_name}'.")
+                        return
+                    toml_path = local_directory_path / 'flatpack.toml'
+                    if not toml_path.exists():
+                        print(f"❌ flatpack.toml not found in the specified directory: '{directory_name}'.")
+                        return
+
+                print("Verbose mode:", args.verbose)
+
+                print(f"✅ Directory name resolved to: '{directory_name}'")
+                fpk_unbox(directory_name, session, verbose=args.verbose, local=args.local)
+
+            elif args.command == "list":
+                print(fpk_list_directories(session))
+            elif args.command == "run":
+
+                try:
+                    port = 8000
+                    listener = ngrok.forward(port, authtoken_from_env=True)
+                    print(f"Ingress established at {listener.url()}")
+                    uvicorn.run(app, host="0.0.0.0", port=port)
+
+                except Exception as e:
+                    print(f"❌ An unexpected error occurred: {e}")
+                except KeyboardInterrupt:
+                    print("❌ FastAPI server has been stopped.")
+                except Exception as e:
+                    print(f"❌ An unexpected error occurred: {e}")
+                finally:
+                    print("Finalizing...")
+                    ngrok.disconnect(listener.url())
+
+            elif args.command == "set-api-key":
+                if args.api_key:
+                    fpk_set_api_key(args.api_key)
+                    print("API key set successfully!")
+            elif args.command == "build":
+                if args.directory:
+                    fpk_build(args.directory, session)
+            elif args.command == "version":
+                print("[VERSION]")
             else:
                 parser.print_help()
 
     except Exception as e:
         print(f"❌ An unexpected error occurred: {e}")
-        sys.exit(1)
+    sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `flatpack-3.3.80/flatpack/modules/lstm.py` & `flatpack-3.3.9/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.80/flatpack/modules/rnn.py` & `flatpack-3.3.9/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.80/flatpack/parsers.py` & `flatpack-3.3.9/flatpack/parsers.py`

 * *Files 7% similar despite different names*

```diff
@@ -79,60 +79,63 @@
     echo "Installing required Unix packages..."
     sudo apt update
     sudo apt install -y {' '.join(package_list_unix)}
 fi
         """.strip()
         script.append(apt_install)
 
+    # Setup venv environment
     venv_setup = f"""
 handle_error() {{
     echo "😟 Oops! Something went wrong."
     exit 1
 }}
 
-if [[ $IS_COLAB -ne 0 ]]; then
-    apt install python3.10-venv
-fi  
+if [[ $IS_COLAB -eq 0 ]]; then
     
-echo "🐍 Checking for Python"
-PYTHON_CMD=python
+    echo "🐍 Checking for Python"
+    
+    PYTHON_CMD=python
 
-echo "Python command to be used: $PYTHON_CMD"
+    echo "Python command to be used: $PYTHON_CMD"
 
-echo "🦄 Creating the virtual environment at {env_name}/{build_prefix}"
-    
-if ! $PYTHON_CMD -m venv "{env_name}/{build_prefix}"; then
-    echo "❌ Failed to create the virtual environment using $PYTHON_CMD"
-    handle_error
-else
-    echo "✅ Successfully created the virtual environment"
-fi
+    echo "🦄 Creating the virtual environment at {env_name}/{build_prefix}"
     
-# Ensuring the VENV_PYTHON path does not begin with a dot and is correctly formed
-export VENV_PYTHON="{env_name}/{build_prefix}/bin/python"
-if [[ -f "$VENV_PYTHON" ]]; then
-    echo "✅ VENV_PYTHON is set correctly to $VENV_PYTHON"
-    echo "🐍 Checking Python version in the virtual environment..."
-    $VENV_PYTHON --version
-else
-    echo "❌ VENV_PYTHON is set to $VENV_PYTHON, but this file does not exist"
-    handle_error
-fi
+    if ! $PYTHON_CMD -m venv "{env_name}/{build_prefix}"; then
+        echo "❌ Failed to create the virtual environment using $PYTHON_CMD"
+        handle_error
+    else
+        echo "✅ Successfully created the virtual environment"
+    fi
     
-# Ensure pip is installed within the virtual environment
-if [ ! -x "$VENV_PYTHON -m pip" ]; then
-    echo "Installing pip within the virtual environment..."
-    $VENV_PYTHON -m ensurepip
+    # Ensuring the VENV_PYTHON path does not begin with a dot and is correctly formed
+    export VENV_PYTHON="{env_name}/{build_prefix}/bin/python"
+    if [[ -f "$VENV_PYTHON" ]]; then
+        echo "✅ VENV_PYTHON is set correctly to $VENV_PYTHON"
+        echo "🐍 Checking Python version in the virtual environment..."
+        $VENV_PYTHON --version
+    else
+        echo "❌ VENV_PYTHON is set to $VENV_PYTHON, but this file does not exist"
+        handle_error
+    fi
 fi
-    
-# Set VENV_PIP variable to the path of pip within the virtual environment
-export VENV_PIP="$VENV_PYTHON -m pip"
-    """
+    """.strip()
     script.append(venv_setup)
 
+    # Additional logic for determining VENV_PIP
+    script.append(f"""
+OS=$(uname)
+if [[ "$OS" = "Darwin" ]] || [[ "$OS" = "Linux" ]] || [[ -d "/content" ]]; then
+    export VENV_PIP="$(dirname $VENV_PYTHON)/pip"
+else
+    echo "⚠️  Virtual environment's pip could not be determined."
+    exit 1
+fi
+    """.strip())
+
     # Create other directories within the build directory as per the TOML configuration
     directories_map = config.get("directories")
     if directories_map:
         for directory_path in directories_map.values():
             formatted_path = directory_path.lstrip('/').replace("home/content/", "")
             script.append(f"mkdir -p {model_name}/{build_prefix}/{formatted_path}")
```

### Comparing `flatpack-3.3.80/flatpack/vector_manager.py` & `flatpack-3.3.9/flatpack/vector_manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,170 +1,167 @@
-import datetime
+import faiss
 import hashlib
-import hnswlib
 import json
 import logging
 import nltk
 import numpy as np
 import os
 import re
 import requests
 
 from bs4 import BeautifulSoup
-from contextlib import redirect_stdout
 from nltk.tokenize import sent_tokenize
 from pypdf import PdfReader
 from sentence_transformers import SentenceTransformer
 from typing import List
 from urllib.parse import urlparse
 
-# Configure logging
-logging.basicConfig(level=logging.CRITICAL, format='%(asctime)s - %(levelname)s - %(message)s')
+logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
 
-with redirect_stdout(open(os.devnull, "w")):
-    nltk.download('punkt', quiet=True)
+nltk.download('punkt')
 
 VECTOR_DIMENSION = 384
-INDEX_FILE = "hnsw_index.bin"
+INDEX_FILE = "vector.index"
 METADATA_FILE = "metadata.json"
 SENTENCE_CHUNK_SIZE = 5
 
 
 class VectorManager:
-    def __init__(self, model_name='all-MiniLM-L6-v2', directory='./data'):
-        self.directory = directory
-        self.index_file = os.path.join(self.directory, INDEX_FILE)
-        self.metadata_file = os.path.join(self.directory, METADATA_FILE)
-
+    def __init__(self, model_name='all-MiniLM-L6-v2'):
         self.model = SentenceTransformer(model_name)
-        self.index = hnswlib.Index(space='l2', dim=VECTOR_DIMENSION)
+        self.index = self._initialize_index()
         self.metadata, self.hash_set = self._load_metadata()
-        self._initialize_index()
 
     def _initialize_index(self):
-        if os.path.exists(self.index_file):
-            self.index.load_index(self.index_file, max_elements=0)
-        else:
-            self.index.init_index(max_elements=10000, ef_construction=200, M=16)
+        index = faiss.IndexFlatL2(VECTOR_DIMENSION)
+        if os.path.exists(INDEX_FILE):
+            index = faiss.read_index(INDEX_FILE)
+        return index
 
     def is_index_ready(self):
-        return self.index.get_current_count() > 0
+        return self.index.ntotal > 0
 
     def _load_metadata(self):
-        if os.path.exists(self.metadata_file):
-            with open(self.metadata_file, 'r') as file:
-                metadata = [json.loads(line) for line in file]
-            hash_set = {entry['hash'] for entry in metadata}
-            return metadata, hash_set
-        return [], set()
+        if not os.path.exists(METADATA_FILE):
+            return [], set()
+        with open(METADATA_FILE, 'r') as file:
+            metadata = [json.loads(line) for line in file]
+        hash_set = {entry['hash'] for entry in metadata}
+        return metadata, hash_set
 
     def _save_metadata(self):
-        with open(self.metadata_file, 'w') as file:
+        with open(METADATA_FILE, 'w') as file:
             for entry in self.metadata:
                 json.dump(entry, file)
                 file.write('\n')
-        self.index.save_index(self.index_file)
+        faiss.write_index(self.index, INDEX_FILE)
 
     def _generate_positive_hash(self, text):
         hash_object = hashlib.sha256(text.encode())
         return int(hash_object.hexdigest()[:16], 16)
 
-    def add_texts(self, texts, source_reference):
+    def add_texts(self, texts):
         embeddings = []
-        ids = []
         new_entries = []
         for text in texts:
             text_hash = self._generate_positive_hash(text)
             if text_hash not in self.hash_set:
-                embedding = self.model.encode([text])[0]
-                embeddings.append(embedding)
-                ids.append(text_hash)
+                embeddings.append(self.model.encode([text])[0])
                 self.hash_set.add(text_hash)
-                now = datetime.datetime.now()
-                date_added = now.strftime("%Y-%m-%d %H:%M:%S")
-                new_entries.append({
-                    "hash": text_hash,
-                    "source": source_reference,
-                    "date": date_added,
-                    "text": text
-                })
+                new_entries.append({"hash": text_hash, "text": text})
         if embeddings:
-            embeddings = np.array(embeddings)
-            self.index.add_items(embeddings, ids)
+            self.index.add(np.array(embeddings))
             self.metadata.extend(new_entries)
             self._save_metadata()
 
     def search_vectors(self, query_text: str, top_k=5):
+        if not hasattr(self, 'index') or self.index is None:
+            raise ValueError("Vector index is not available.")
+
         query_embedding = self.model.encode([query_text])[0]
-        labels, distances = self.index.knn_query(query_embedding, k=top_k)
+        query_np = np.array(query_embedding, dtype=np.float32).reshape(1, -1)
+        extended_top_k = min(top_k * 3, len(self.metadata))
+        distances, indices = self.index.search(query_np, extended_top_k)
+
+        ranked_results = sorted(zip(distances[0], indices[0]), key=lambda x: x[0])
+
         results = []
-        for label, distance in zip(labels[0], distances[0]):
-            entry = next((item for item in self.metadata if item['hash'] == label), None)
-            if entry:
-                results.append({
-                    "id": entry['hash'],
-                    "distance": distance,
-                    "source": entry['source'],
-                    "date": entry['date'],
-                    "text": entry['text']
-                })
+        seen_hashes = set()
+        for distance, idx in ranked_results:
+            if idx < len(self.metadata):
+                metadata_entry = self.metadata[idx]
+                text_hash = metadata_entry["hash"]
+                text = metadata_entry["text"]
+                if text_hash not in seen_hashes:
+                    results.append({"id": text_hash, "distance": distance, "text": text})
+                    seen_hashes.add(text_hash)
+                if len(results) == top_k:
+                    break
         return results
 
-    def _process_text_and_add(self, text, source_reference):
+    def _process_text_and_add(self, text):
         if not isinstance(text, str):
             logging.error(f"_process_text_and_add expected a string but got {type(text)}. Value: {text}")
-            return
+            return  # Exit early if not a string
         sentences = sent_tokenize(text)
         for i in range(0, len(sentences), SENTENCE_CHUNK_SIZE):
             chunk_text = " ".join(sentences[i:i + SENTENCE_CHUNK_SIZE]).strip()
-            self.add_texts([chunk_text], source_reference)
+            self.add_texts([chunk_text])
 
     def add_pdf(self, pdf_path: str):
         with open(pdf_path, 'rb') as file:
             pdf = PdfReader(file)
             all_text = " ".join(page.extract_text() or "" for page in pdf.pages)
-        self._process_text_and_add(all_text, pdf_path)
+        self._process_text_and_add(all_text)
 
     def add_url(self, url: str):
         logging.info(f"Fetching URL: {url}")
         response = requests.get(url)
         if response.status_code == 200:
             logging.debug("URL fetched successfully.")
             soup = BeautifulSoup(response.content, 'html.parser')
             text = soup.get_text(separator=' ', strip=True)
             logging.debug("Extracted text from HTML.")
-            self._process_text_and_add(text, url)
+            logging.debug("Starting to clean text.")
+            cleaned_text = self.clean_text(text)
+            logging.debug("Cleaned text obtained.")
+            self._process_text_and_add(cleaned_text)
             logging.info("Text added successfully.")
         else:
             logging.error(f"Failed to fetch {url}: Status code {response.status_code}")
 
     def get_wikipedia_text(self, page_title):
+        """
+        Fetches the plain text content of a Wikipedia page given its title using the Wikipedia API.
+        """
         logging.info(f"Fetching Wikipedia page for: {page_title}")
         base_url = "https://en.wikipedia.org/w/api.php"
         params = {
             "action": "query",
             "titles": page_title,
             "prop": "extracts",
             "explaintext": 1,
             "exsectionformat": "plain",
             "redirects": 1,
             "format": "json"
         }
 
         response = requests.get(base_url, params=params)
-        response.raise_for_status()
+        response.raise_for_status()  # Raises HTTPError, if one occurred during the request
 
         data = response.json()
         page = next(iter(data["query"]["pages"].values()))
         return page.get("extract", "")
 
     def add_wikipedia_page(self, page_title):
         try:
             text = self.get_wikipedia_text(page_title)
             if text:
                 logging.debug("Starting to process and add Wikipedia text.")
-                self._process_text_and_add(text, f"wikipedia:{page_title}")
+                # Debug log to check the type and content of text
+                logging.debug(f"Type of text: {type(text)}, Content: {text[:100]}")
+                self._process_text_and_add(text)
                 logging.info("Wikipedia text added successfully.")
             else:
                 logging.error(f"No text found for Wikipedia page: {page_title}")
         except requests.HTTPError as e:
             logging.error(f"Failed to fetch Wikipedia page: {page_title}. HTTPError: {e}")
```

### Comparing `flatpack-3.3.80/flatpack.egg-info/PKG-INFO` & `flatpack-3.3.9/flatpack.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.3.80
+Version: 3.3.9
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: cryptography==42.0.5
 Requires-Dist: faiss-cpu==1.8.0
-Requires-Dist: fastapi==0.110.2
-Requires-Dist: hnswlib==0.8.0
+Requires-Dist: fastapi==0.110.1
 Requires-Dist: httpx==0.27.0
-Requires-Dist: huggingface-hub==0.22.2
-Requires-Dist: llama-cpp-python==0.2.65
 Requires-Dist: ngrok==1.2.0
 Requires-Dist: nltk==3.8.1
 Requires-Dist: olefile==0.47
-Requires-Dist: psutil==5.9.5
 Requires-Dist: pypdf==4.2.0
 Requires-Dist: requests==2.31.0
-Requires-Dist: sentence-transformers==2.7.0
+Requires-Dist: sentence-transformers==2.6.1
 Requires-Dist: toml==0.10.2
+Requires-Dist: torch==2.2.2
 Requires-Dist: uvicorn==0.29.0
 
 # Flatpack
 
 **NOTE:** Flatpack is currently experimental. Please refrain from using it in production environments.
 
 ## Ready-to-assemble AI
@@ -70,63 +67,60 @@
 
 ## License
 
 This project is released under [Apache-2.0](https://github.com/romlingroup/flatpack-ai/blob/main/LICENSE).
 
 ## install_requires
 
-**DISCLAIMER:** This information is only a technical reference, not an endorsement or legal advice. Before using any software for commercial purposes, perform compatibility checks and seek legal advice. You are responsible for ensuring compliance with licensing requirements.
+**DISCLAIMER:** The license compatibility information provided herein serves solely as a technical reference. It does not imply endorsement or legal advice. Users are encouraged to perform compatibility checks and consult with legal experts before commercially utilising any software. The user is responsible for ensuring compliance with applicable licensing requirements.
 
-Check out the [JLA - Compatibility Checker](https://joinup.ec.europa.eu/collection/eupl/solution/joinup-licensing-assistant/jla-compatibility-checker) (European Commission 2023).
+BSD 2-Clause "Simplified" (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original BSD-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/BSD-2-Clause/Apache-2.0)).
+
+BSD-3-Clause (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original BSD-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/BSD-3-Clause/Apache-2.0)).
+
+MIT (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original MIT-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/MIT/Apache-2.0)).
+
+*Check out the [JLA - Compatibility Checker](https://joinup.ec.europa.eu/collection/eupl/solution/joinup-licensing-assistant/jla-compatibility-checker) (European Commission 2023).*
 
 - **[beautifulsoup4](https://pypi.org/project/beautifulsoup4/)**\
   MIT License (MIT License) ([LICENSE](https://pypi.org/project/beautifulsoup4/))
 
 - **[cryptography](https://pypi.org/project/cryptography/)**\
   Apache Software License, BSD License (Apache-2.0 OR BSD-3-Clause) ([LICENSE](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE))
 
 - **[faiss-cpu](https://pypi.org/project/faiss-cpu/)**\
   MIT License (MIT License) ([LICENSE](https://github.com/kyamagu/faiss-wheels/blob/main/LICENSE))
 
 - **[fastapi](https://pypi.org/project/fastapi/)**\
   MIT License ([LICENSE](https://github.com/tiangolo/fastapi/blob/master/LICENSE))
 
-- **[hnswlib](https://pypi.org/project/hnswlib/)**\
-  Apache-2.0 license ([LICENSE](https://github.com/nmslib/hnswlib/blob/master/LICENSE))
-
 - **[httpx](https://pypi.org/project/httpx/)**\
   BSD License ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
 
-- **[huggingface-hub](https://pypi.org/project/huggingface-hub/)**\
-  Apache Software License (Apache) ([LICENSE](https://github.com/huggingface/huggingface_hub/blob/main/LICENSE))
-
-- **[llama-cpp-python](https://pypi.org/project/llama-cpp-python/)**\
-  MIT ([LICENSE](https://github.com/abetlen/llama-cpp-python/blob/main/LICENSE.md))
-
 - **[ngrok](https://pypi.org/project/ngrok/)**\
   MIT License (MIT OR Apache-2.0) ([LICENSE](https://github.com/ngrok/ngrok-python/blob/main/LICENSE-APACHE))
 
 - **[nltk](https://pypi.org/project/nltk/)**\
   Apache Software License (Apache License, Version 2.0) ([LICENSE](https://github.com/nltk/nltk/blob/develop/LICENSE.txt))
 
 - **[olefile](https://pypi.org/project/olefile/)**\
   BSD License (BSD) ([LICENSE](https://github.com/decalage2/olefile/blob/master/LICENSE.txt))
 
-- **[psutil](https://pypi.org/project/psutil/)**\
-  BSD License (BSD-3-Clause) ([LICENSE](https://github.com/giampaolo/psutil/blob/master/LICENSE))
-
 - **[pypdf](https://pypi.org/project/pypdf/)**\
   BSD License ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE))
 
 - **[requests](https://pypi.org/project/requests/)**\
   Apache Software License (Apache 2.0) ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
 
 - **[sentence-transformers](https://pypi.org/project/sentence-transformers/)**\
   Apache Software License (Apache License 2.0) ([LICENSE](https://github.com/UKPLab/sentence-transformers/blob/master/LICENSE))
 
 - **[toml](https://pypi.org/project/toml/)**\
   MIT License (MIT) ([LICENSE](https://github.com/uiri/toml/blob/master/LICENSE))
 
+- **[torch](https://pypi.org/project/torch/)**\
+  BSD License (BSD-3) ([LICENSE](https://github.com/pytorch/pytorch/blob/main/LICENSE))
+
 - **[uvicorn](https://pypi.org/project/uvicorn/)**\
   BSD License ([LICENSE](https://github.com/encode/uvicorn/blob/master/LICENSE.md))
 
-Last updated: 2024-04-27
+Last updated: 2024-04-20
```

### Comparing `flatpack-3.3.80/setup.py` & `flatpack-3.3.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.3.80",
+    version="3.3.9",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "cryptography==42.0.5",
         "faiss-cpu==1.8.0",
-        "fastapi==0.110.2",
-        "hnswlib==0.8.0",
+        "fastapi==0.110.1",
         "httpx==0.27.0",
-        "huggingface-hub==0.22.2",
-        "llama-cpp-python==0.2.65",
         "ngrok==1.2.0",
         "nltk==3.8.1",
         "olefile==0.47",
-        "psutil==5.9.5",
         "pypdf==4.2.0",
         "requests==2.31.0",
-        "sentence-transformers==2.7.0",
+        "sentence-transformers==2.6.1",
         "toml==0.10.2",
+        "torch==2.2.2",
         "uvicorn==0.29.0"
     ],
     author="Romlin Group AB",
     author_email="hello@romlin.com",
     description="Ready-to-assemble AI",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

