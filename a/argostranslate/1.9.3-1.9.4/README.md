# Comparing `tmp/argostranslate-1.9.3.tar.gz` & `tmp/argostranslate-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argostranslate-1.9.3.tar", last modified: Sun Mar 17 12:31:57 2024, max compression
+gzip compressed data, was "argostranslate-1.9.4.tar", last modified: Mon Apr 29 17:54:08 2024, max compression
```

## Comparing `argostranslate-1.9.3.tar` & `argostranslate-1.9.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-03-17 12:31:57.626131 argostranslate-1.9.3/
--rw-rw-r--   0 pj        (1000) pj        (1000)     1085 2023-06-02 23:17:46.000000 argostranslate-1.9.3/LICENSE
--rw-r--r--   0 pj        (1000) pj        (1000)     9916 2024-03-17 12:31:57.622131 argostranslate-1.9.3/PKG-INFO
--rw-rw-r--   0 pj        (1000) pj        (1000)     8977 2024-03-13 15:02:28.000000 argostranslate-1.9.3/README.md
-drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-03-17 12:31:57.622131 argostranslate-1.9.3/argostranslate/
--rw-rw-r--   0 pj        (1000) pj        (1000)        0 2023-06-02 23:17:46.000000 argostranslate-1.9.3/argostranslate/__init__.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     4324 2024-03-13 15:02:19.000000 argostranslate-1.9.3/argostranslate/apis.py
--rw-rw-r--   0 pj        (1000) pj        (1000)    14371 2024-03-13 15:02:19.000000 argostranslate-1.9.3/argostranslate/apply_bpe.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     4313 2024-03-13 15:02:19.000000 argostranslate-1.9.3/argostranslate/argospm.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     2147 2024-03-13 15:02:19.000000 argostranslate-1.9.3/argostranslate/cli.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     2240 2023-06-02 23:17:46.000000 argostranslate-1.9.3/argostranslate/fewshot.py
--rw-rw-r--   0 pj        (1000) pj        (1000)      298 2023-06-02 23:17:46.000000 argostranslate-1.9.3/argostranslate/models.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     2269 2024-03-13 15:02:19.000000 argostranslate-1.9.3/argostranslate/networking.py
--rw-rw-r--   0 pj        (1000) pj        (1000)    13220 2024-03-13 15:02:19.000000 argostranslate-1.9.3/argostranslate/package.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     3287 2024-03-13 15:02:19.000000 argostranslate-1.9.3/argostranslate/sbd.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     3119 2024-03-13 15:02:19.000000 argostranslate-1.9.3/argostranslate/settings.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     6544 2024-03-13 15:02:19.000000 argostranslate-1.9.3/argostranslate/tags.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     2268 2024-03-13 15:02:19.000000 argostranslate-1.9.3/argostranslate/tokenizer.py
--rw-rw-r--   0 pj        (1000) pj        (1000)    23803 2024-03-13 15:02:19.000000 argostranslate-1.9.3/argostranslate/translate.py
--rw-rw-r--   0 pj        (1000) pj        (1000)      487 2024-03-13 15:02:19.000000 argostranslate-1.9.3/argostranslate/utils.py
-drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-03-17 12:31:57.622131 argostranslate-1.9.3/argostranslate.egg-info/
--rw-r--r--   0 pj        (1000) pj        (1000)     9916 2024-03-17 12:31:57.000000 argostranslate-1.9.3/argostranslate.egg-info/PKG-INFO
--rw-rw-r--   0 pj        (1000) pj        (1000)      695 2024-03-17 12:31:57.000000 argostranslate-1.9.3/argostranslate.egg-info/SOURCES.txt
--rw-rw-r--   0 pj        (1000) pj        (1000)        1 2024-03-17 12:31:57.000000 argostranslate-1.9.3/argostranslate.egg-info/dependency_links.txt
--rw-rw-r--   0 pj        (1000) pj        (1000)       85 2024-03-17 12:31:57.000000 argostranslate-1.9.3/argostranslate.egg-info/requires.txt
--rw-rw-r--   0 pj        (1000) pj        (1000)       21 2024-03-17 12:31:57.000000 argostranslate-1.9.3/argostranslate.egg-info/top_level.txt
-drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-03-17 12:31:57.622131 argostranslate-1.9.3/bin/
--rwxrwxr-x   0 pj        (1000) pj        (1000)       69 2023-06-02 23:17:46.000000 argostranslate-1.9.3/bin/argos-translate
--rw-rw-r--   0 pj        (1000) pj        (1000)       74 2023-06-02 23:17:47.000000 argostranslate-1.9.3/bin/argospm
--rw-rw-r--   0 pj        (1000) pj        (1000)       38 2024-03-17 12:31:57.626131 argostranslate-1.9.3/setup.cfg
--rw-rw-r--   0 pj        (1000) pj        (1000)     1224 2024-03-17 12:31:15.000000 argostranslate-1.9.3/setup.py
-drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-03-17 12:31:57.622131 argostranslate-1.9.3/tests/
--rw-rw-r--   0 pj        (1000) pj        (1000)        0 2024-03-13 15:02:19.000000 argostranslate-1.9.3/tests/__init__.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     2489 2024-03-13 15:02:19.000000 argostranslate-1.9.3/tests/test_package.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     4581 2024-03-13 15:02:19.000000 argostranslate-1.9.3/tests/test_translate.py
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-04-29 17:54:08.991991 argostranslate-1.9.4/
+-rw-rw-r--   0 pj        (1000) pj        (1000)     1085 2023-06-02 23:17:46.000000 argostranslate-1.9.4/LICENSE
+-rw-rw-r--   0 pj        (1000) pj        (1000)     9840 2024-04-29 17:54:08.991991 argostranslate-1.9.4/PKG-INFO
+-rw-rw-r--   0 pj        (1000) pj        (1000)     9024 2024-04-29 17:52:23.000000 argostranslate-1.9.4/README.md
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-04-29 17:54:08.991991 argostranslate-1.9.4/argostranslate/
+-rw-rw-r--   0 pj        (1000) pj        (1000)        0 2023-06-02 23:17:46.000000 argostranslate-1.9.4/argostranslate/__init__.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     4324 2024-03-13 15:02:19.000000 argostranslate-1.9.4/argostranslate/apis.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)    14371 2024-03-13 15:02:19.000000 argostranslate-1.9.4/argostranslate/apply_bpe.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     4313 2024-03-13 15:02:19.000000 argostranslate-1.9.4/argostranslate/argospm.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     2147 2024-03-13 15:02:19.000000 argostranslate-1.9.4/argostranslate/cli.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     2240 2023-06-02 23:17:46.000000 argostranslate-1.9.4/argostranslate/fewshot.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)      298 2023-06-02 23:17:46.000000 argostranslate-1.9.4/argostranslate/models.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     2269 2024-03-13 15:02:19.000000 argostranslate-1.9.4/argostranslate/networking.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)    13220 2024-03-13 15:02:19.000000 argostranslate-1.9.4/argostranslate/package.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     3287 2024-04-29 17:52:19.000000 argostranslate-1.9.4/argostranslate/sbd.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     3119 2024-03-13 15:02:19.000000 argostranslate-1.9.4/argostranslate/settings.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     6544 2024-03-13 15:02:19.000000 argostranslate-1.9.4/argostranslate/tags.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     2268 2024-03-13 15:02:19.000000 argostranslate-1.9.4/argostranslate/tokenizer.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)    23803 2024-04-29 17:52:19.000000 argostranslate-1.9.4/argostranslate/translate.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)      487 2024-03-13 15:02:19.000000 argostranslate-1.9.4/argostranslate/utils.py
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-04-29 17:54:08.991991 argostranslate-1.9.4/argostranslate.egg-info/
+-rw-r--r--   0 pj        (1000) pj        (1000)     9840 2024-04-29 17:54:08.000000 argostranslate-1.9.4/argostranslate.egg-info/PKG-INFO
+-rw-rw-r--   0 pj        (1000) pj        (1000)      695 2024-04-29 17:54:08.000000 argostranslate-1.9.4/argostranslate.egg-info/SOURCES.txt
+-rw-rw-r--   0 pj        (1000) pj        (1000)        1 2024-04-29 17:54:08.000000 argostranslate-1.9.4/argostranslate.egg-info/dependency_links.txt
+-rw-rw-r--   0 pj        (1000) pj        (1000)       84 2024-04-29 17:54:08.000000 argostranslate-1.9.4/argostranslate.egg-info/requires.txt
+-rw-rw-r--   0 pj        (1000) pj        (1000)       21 2024-04-29 17:54:08.000000 argostranslate-1.9.4/argostranslate.egg-info/top_level.txt
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-04-29 17:54:08.991991 argostranslate-1.9.4/bin/
+-rwxrwxr-x   0 pj        (1000) pj        (1000)       69 2023-06-02 23:17:46.000000 argostranslate-1.9.4/bin/argos-translate
+-rw-rw-r--   0 pj        (1000) pj        (1000)       74 2023-06-02 23:17:47.000000 argostranslate-1.9.4/bin/argospm
+-rw-rw-r--   0 pj        (1000) pj        (1000)       38 2024-04-29 17:54:08.991991 argostranslate-1.9.4/setup.cfg
+-rw-rw-r--   0 pj        (1000) pj        (1000)     1224 2024-04-29 17:52:38.000000 argostranslate-1.9.4/setup.py
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-04-29 17:54:08.991991 argostranslate-1.9.4/tests/
+-rw-rw-r--   0 pj        (1000) pj        (1000)        0 2024-03-13 15:02:19.000000 argostranslate-1.9.4/tests/__init__.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     2489 2024-03-13 15:02:19.000000 argostranslate-1.9.4/tests/test_package.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     4581 2024-03-13 15:02:19.000000 argostranslate-1.9.4/tests/test_translate.py
```

### Comparing `argostranslate-1.9.3/LICENSE` & `argostranslate-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.3/PKG-INFO` & `argostranslate-1.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 Metadata-Version: 2.1
 Name: argostranslate
-Version: 1.9.3
+Version: 1.9.4
 Summary: Open-source neural machine translation library based on OpenNMT's CTranslate2
 Home-page: https://www.argosopentech.com
 Author: Argos Open Technologies, LLC
 Author-email: admin@argosopentech.com
+License: UNKNOWN
 Project-URL: Website, https://www.argosopentech.com
 Project-URL: Documentation, https://argos-translate.readthedocs.io/en/latest/
 Project-URL: GitHub, https://github.com/argosopentech/argos-translate
 Project-URL: Forum, https://community.libretranslate.com/c/argos-translate/5
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ctranslate2==3.20.0
-Requires-Dist: sentencepiece==0.1.99
-Requires-Dist: stanza==1.1.1
-Requires-Dist: packaging
-Requires-Dist: sacremoses==0.0.53
 
 # Argos Translate
 [Demo](https://libretranslate.com) | [Website](https://www.argosopentech.com) | [Docs](https://argos-translate.readthedocs.io) |  [Forum](https://community.libretranslate.com/c/argos-translate/5) | [GitHub](https://github.com/argosopentech/argos-translate) | [PyPI](https://pypi.org/project/argostranslate/)
 
 **Open-source offline translation library written in Python**
 
 Argos Translate uses [OpenNMT](https://opennmt.net/) for translations and can be used as either a Python library, command-line, or GUI application. Argos Translate supports installing language model packages which are zip archives with a ".argosmodel" extension containing the data needed for translation. [LibreTranslate](https://libretranslate.com) is an API and web-app built on top of Argos Translate.
@@ -200,16 +197,17 @@
 [I am also available for hire](https://www.argosopentech.com/about/) to do support, consulting, or custom software development.
 
 ## Donate
 If you find this software useful donations are appreciated.
 - [GitHub Sponsor](https://github.com/sponsors/argosopentech)
 - [PayPal](https://www.paypal.com/biz/fund?id=MCCFG437JP9PJ)
 - Bitcoin: 16UJrmSEGojFPaqjTGpuSMNhNRSsnspFJT
-- BCH: bitcoincash:qzvpxe8y5kq45kahqkyv3p88sjrhlymj2v6xdrj3cv
 - Ethereum: argosopentech.eth
+- Litecoin: MCwu7RRWeCRJdsv2bXGj2nnL1xYxDBvwW5
+- BCH: bitcoincash:qzvpxe8y5kq45kahqkyv3p88sjrhlymj2v6xdrj3cv
 
 Paid supporters receive priority support.
 
 #### Hosting affiliate links
 You can help support Argos Translate financially by purchasing hosting through these referral links:
 - [Vast.ai](http://vast.ai/?ref=24817) - Cheap GPU rentals
 - [DigitalOcean](https://m.do.co/c/a1af57be6e3f) - Best all around hosting
@@ -220,7 +218,9 @@
 A beta version of Argos Translate 2 is available to install from source from the [v2 branch on GitHub](https://github.com/argosopentech/argos-translate/tree/v2). Argos Translate 2 has a [multilingual model architecture](https://community.libretranslate.com/t/multilingual-translation-with-ctranslate2-and-pre-trained-fairseq-models/178/), more extensive unit testing, and a more experimental orientation.
 
 ## Contributing
 Contributions are welcome! Bug reports, pull requests, documentation writing, and feature ideas are all appreciated.
 
 ## License
 Argos Translate is dual licensed under either the [MIT License](https://github.com/argosopentech/argos-translate/blob/master/LICENSE) or [Creative Commons CC0](https://creativecommons.org/share-your-work/public-domain/cc0/).
+
+
```

### Comparing `argostranslate-1.9.3/README.md` & `argostranslate-1.9.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -177,16 +177,17 @@
 [I am also available for hire](https://www.argosopentech.com/about/) to do support, consulting, or custom software development.
 
 ## Donate
 If you find this software useful donations are appreciated.
 - [GitHub Sponsor](https://github.com/sponsors/argosopentech)
 - [PayPal](https://www.paypal.com/biz/fund?id=MCCFG437JP9PJ)
 - Bitcoin: 16UJrmSEGojFPaqjTGpuSMNhNRSsnspFJT
-- BCH: bitcoincash:qzvpxe8y5kq45kahqkyv3p88sjrhlymj2v6xdrj3cv
 - Ethereum: argosopentech.eth
+- Litecoin: MCwu7RRWeCRJdsv2bXGj2nnL1xYxDBvwW5
+- BCH: bitcoincash:qzvpxe8y5kq45kahqkyv3p88sjrhlymj2v6xdrj3cv
 
 Paid supporters receive priority support.
 
 #### Hosting affiliate links
 You can help support Argos Translate financially by purchasing hosting through these referral links:
 - [Vast.ai](http://vast.ai/?ref=24817) - Cheap GPU rentals
 - [DigitalOcean](https://m.do.co/c/a1af57be6e3f) - Best all around hosting
```

### Comparing `argostranslate-1.9.3/argostranslate/apis.py` & `argostranslate-1.9.4/argostranslate/apis.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.3/argostranslate/apply_bpe.py` & `argostranslate-1.9.4/argostranslate/apply_bpe.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.3/argostranslate/argospm.py` & `argostranslate-1.9.4/argostranslate/argospm.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.3/argostranslate/cli.py` & `argostranslate-1.9.4/argostranslate/cli.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.3/argostranslate/fewshot.py` & `argostranslate-1.9.4/argostranslate/fewshot.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.3/argostranslate/networking.py` & `argostranslate-1.9.4/argostranslate/networking.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.3/argostranslate/package.py` & `argostranslate-1.9.4/argostranslate/package.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.3/argostranslate/sbd.py` & `argostranslate-1.9.4/argostranslate/sbd.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.3/argostranslate/settings.py` & `argostranslate-1.9.4/argostranslate/settings.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.3/argostranslate/tags.py` & `argostranslate-1.9.4/argostranslate/tags.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.3/argostranslate/tokenizer.py` & `argostranslate-1.9.4/argostranslate/tokenizer.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.3/argostranslate/translate.py` & `argostranslate-1.9.4/argostranslate/translate.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.3/argostranslate.egg-info/PKG-INFO` & `argostranslate-1.9.4/argostranslate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 Metadata-Version: 2.1
 Name: argostranslate
-Version: 1.9.3
+Version: 1.9.4
 Summary: Open-source neural machine translation library based on OpenNMT's CTranslate2
 Home-page: https://www.argosopentech.com
 Author: Argos Open Technologies, LLC
 Author-email: admin@argosopentech.com
+License: UNKNOWN
 Project-URL: Website, https://www.argosopentech.com
 Project-URL: Documentation, https://argos-translate.readthedocs.io/en/latest/
 Project-URL: GitHub, https://github.com/argosopentech/argos-translate
 Project-URL: Forum, https://community.libretranslate.com/c/argos-translate/5
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ctranslate2==3.20.0
-Requires-Dist: sentencepiece==0.1.99
-Requires-Dist: stanza==1.1.1
-Requires-Dist: packaging
-Requires-Dist: sacremoses==0.0.53
 
 # Argos Translate
 [Demo](https://libretranslate.com) | [Website](https://www.argosopentech.com) | [Docs](https://argos-translate.readthedocs.io) |  [Forum](https://community.libretranslate.com/c/argos-translate/5) | [GitHub](https://github.com/argosopentech/argos-translate) | [PyPI](https://pypi.org/project/argostranslate/)
 
 **Open-source offline translation library written in Python**
 
 Argos Translate uses [OpenNMT](https://opennmt.net/) for translations and can be used as either a Python library, command-line, or GUI application. Argos Translate supports installing language model packages which are zip archives with a ".argosmodel" extension containing the data needed for translation. [LibreTranslate](https://libretranslate.com) is an API and web-app built on top of Argos Translate.
@@ -200,16 +197,17 @@
 [I am also available for hire](https://www.argosopentech.com/about/) to do support, consulting, or custom software development.
 
 ## Donate
 If you find this software useful donations are appreciated.
 - [GitHub Sponsor](https://github.com/sponsors/argosopentech)
 - [PayPal](https://www.paypal.com/biz/fund?id=MCCFG437JP9PJ)
 - Bitcoin: 16UJrmSEGojFPaqjTGpuSMNhNRSsnspFJT
-- BCH: bitcoincash:qzvpxe8y5kq45kahqkyv3p88sjrhlymj2v6xdrj3cv
 - Ethereum: argosopentech.eth
+- Litecoin: MCwu7RRWeCRJdsv2bXGj2nnL1xYxDBvwW5
+- BCH: bitcoincash:qzvpxe8y5kq45kahqkyv3p88sjrhlymj2v6xdrj3cv
 
 Paid supporters receive priority support.
 
 #### Hosting affiliate links
 You can help support Argos Translate financially by purchasing hosting through these referral links:
 - [Vast.ai](http://vast.ai/?ref=24817) - Cheap GPU rentals
 - [DigitalOcean](https://m.do.co/c/a1af57be6e3f) - Best all around hosting
@@ -220,7 +218,9 @@
 A beta version of Argos Translate 2 is available to install from source from the [v2 branch on GitHub](https://github.com/argosopentech/argos-translate/tree/v2). Argos Translate 2 has a [multilingual model architecture](https://community.libretranslate.com/t/multilingual-translation-with-ctranslate2-and-pre-trained-fairseq-models/178/), more extensive unit testing, and a more experimental orientation.
 
 ## Contributing
 Contributions are welcome! Bug reports, pull requests, documentation writing, and feature ideas are all appreciated.
 
 ## License
 Argos Translate is dual licensed under either the [MIT License](https://github.com/argosopentech/argos-translate/blob/master/LICENSE) or [Creative Commons CC0](https://creativecommons.org/share-your-work/public-domain/cc0/).
+
+
```

### Comparing `argostranslate-1.9.3/argostranslate.egg-info/SOURCES.txt` & `argostranslate-1.9.4/argostranslate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.3/setup.py` & `argostranslate-1.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     required_packages = f.read().splitlines()
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="argostranslate",
-    version="1.9.3",
+    version="1.9.4",
     description="Open-source neural machine translation library based on OpenNMT's CTranslate2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Argos Open Technologies, LLC",
     author_email="admin@argosopentech.com",
     url="https://www.argosopentech.com",
     project_urls={
```

### Comparing `argostranslate-1.9.3/tests/test_package.py` & `argostranslate-1.9.4/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.3/tests/test_translate.py` & `argostranslate-1.9.4/tests/test_translate.py`

 * *Files identical despite different names*

