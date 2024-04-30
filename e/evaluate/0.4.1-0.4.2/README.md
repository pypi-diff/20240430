# Comparing `tmp/evaluate-0.4.1.tar.gz` & `tmp/evaluate-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evaluate-0.4.1.tar", last modified: Fri Oct 13 15:54:40 2023, max compression
+gzip compressed data, was "evaluate-0.4.2.tar", last modified: Tue Apr 30 09:44:11 2024, max compression
```

## Comparing `evaluate-0.4.1.tar` & `evaluate-0.4.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 15:54:40.633221 evaluate-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-10-13 15:54:35.000000 evaluate-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2023-10-13 15:54:40.633221 evaluate-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2023-10-13 15:54:35.000000 evaluate-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      407 2023-10-13 15:54:40.637222 evaluate-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2023-10-13 15:54:35.000000 evaluate-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 15:54:40.629222 evaluate-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 15:54:40.633221 evaluate-0.4.1/src/evaluate/
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 15:54:40.633221 evaluate-0.4.1/src/evaluate/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/commands/evaluate_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 15:54:40.633221 evaluate-0.4.1/src/evaluate/evaluation_suite/
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/evaluation_suite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 15:54:40.633221 evaluate-0.4.1/src/evaluate/evaluator/
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/evaluator/audio_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/evaluator/automatic_speech_recognition.py
--rw-r--r--   0 runner    (1001) docker     (127)    22881 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/evaluator/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/evaluator/image_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     9566 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/evaluator/question_answering.py
--rw-r--r--   0 runner    (1001) docker     (127)     9676 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/evaluator/text2text_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6676 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/evaluator/text_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/evaluator/text_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11546 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/evaluator/token_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/evaluator/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)    35228 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/loading.py
--rw-r--r--   0 runner    (1001) docker     (127)    46290 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/saving.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 15:54:40.633221 evaluate-0.4.1/src/evaluate/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22602 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/utils/gradio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6698 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     9293 2023-10-13 15:54:35.000000 evaluate-0.4.1/src/evaluate/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 15:54:40.633221 evaluate-0.4.1/src/evaluate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2023-10-13 15:54:40.000000 evaluate-0.4.1/src/evaluate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2023-10-13 15:54:40.000000 evaluate-0.4.1/src/evaluate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-13 15:54:40.000000 evaluate-0.4.1/src/evaluate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-10-13 15:54:40.000000 evaluate-0.4.1/src/evaluate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-13 15:54:40.000000 evaluate-0.4.1/src/evaluate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2023-10-13 15:54:40.000000 evaluate-0.4.1/src/evaluate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-13 15:54:40.000000 evaluate-0.4.1/src/evaluate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:44:11.161282 evaluate-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-30 09:44:04.000000 evaluate-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-30 09:44:11.161282 evaluate-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-04-30 09:44:04.000000 evaluate-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-30 09:44:11.161282 evaluate-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-04-30 09:44:04.000000 evaluate-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:44:11.153282 evaluate-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:44:11.157282 evaluate-0.4.2/src/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:44:11.157282 evaluate-0.4.2/src/evaluate/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/commands/evaluate_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:44:11.157282 evaluate-0.4.2/src/evaluate/evaluation_suite/
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/evaluation_suite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:44:11.161282 evaluate-0.4.2/src/evaluate/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/evaluator/audio_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/evaluator/automatic_speech_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22881 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/evaluator/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/evaluator/image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/evaluator/question_answering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/evaluator/text2text_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6676 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/evaluator/text_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/evaluator/text_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/evaluator/token_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/evaluator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35219 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46417 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/saving.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:44:11.161282 evaluate-0.4.2/src/evaluate/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22602 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/utils/gradio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-04-30 09:44:04.000000 evaluate-0.4.2/src/evaluate/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:44:11.157282 evaluate-0.4.2/src/evaluate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-30 09:44:11.000000 evaluate-0.4.2/src/evaluate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-30 09:44:11.000000 evaluate-0.4.2/src/evaluate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:44:11.000000 evaluate-0.4.2/src/evaluate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-30 09:44:11.000000 evaluate-0.4.2/src/evaluate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:44:11.000000 evaluate-0.4.2/src/evaluate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-30 09:44:11.000000 evaluate-0.4.2/src/evaluate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 09:44:11.000000 evaluate-0.4.2/src/evaluate.egg-info/top_level.txt
```

### Comparing `evaluate-0.4.1/LICENSE` & `evaluate-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/PKG-INFO` & `evaluate-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evaluate
-Version: 0.4.1
+Version: 0.4.2
 Summary: HuggingFace community-driven open-source library of evaluation
 Home-page: https://github.com/huggingface/evaluate
 Author: HuggingFace Inc.
 Author-email: leandro@huggingface.co
 License: Apache 2.0
 Download-URL: https://github.com/huggingface/evaluate/tags
 Keywords: metrics machine learning evaluate evaluation
@@ -12,20 +12,19 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: tensorflow
 Provides-Extra: tensorflow_gpu
 Provides-Extra: torch
 Provides-Extra: dev
 Provides-Extra: tests
 Provides-Extra: quality
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: evaluate Version: 0.4.1 Summary: HuggingFace
+Metadata-Version: 2.1 Name: evaluate Version: 0.4.2 Summary: HuggingFace
 community-driven open-source library of evaluation Home-page: https://
 github.com/huggingface/evaluate Author: HuggingFace Inc. Author-email:
 leandro@huggingface.co License: Apache 2.0 Download-URL: https://github.com/
 huggingface/evaluate/tags Keywords: metrics machine learning evaluate
 evaluation Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown Provides-Extra: tensorflow Provides-
-Extra: tensorflow_gpu Provides-Extra: torch Provides-Extra: dev Provides-Extra:
-tests Provides-Extra: quality Provides-Extra: docs Provides-Extra: template
-Provides-Extra: evaluator License-File: LICENSE
+:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.8.0 Description-Content-Type: text/markdown Provides-
+Extra: tensorflow Provides-Extra: tensorflow_gpu Provides-Extra: torch
+Provides-Extra: dev Provides-Extra: tests Provides-Extra: quality Provides-
+Extra: docs Provides-Extra: template Provides-Extra: evaluator License-File:
+LICENSE
 
     [https://huggingface.co/datasets/evaluate/media/resolve/main/evaluate-
                                   banner.png]
      _[_B_u_i_l_d_]_[_G_i_t_H_u_b_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_]_[_C_o_n_t_r_i_b_u_t_o_r_ _C_o_v_e_n_a_n_t_]
 ð¤ Evaluate is a library that makes evaluating and comparing models and
 reporting their performance easier and more standardized. It currently
 contains: - **implementations of dozens of popular metrics**: the existing
```

### Comparing `evaluate-0.4.1/README.md` & `evaluate-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/__init__.py` & `evaluate-0.4.2/src/evaluate/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Lint as: python3
 # pylint: enable=line-too-long
 # pylint: disable=g-import-not-at-top,g-bad-import-order,wrong-import-position
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 from packaging import version
 
 
 SCRIPTS_VERSION = "main" if version.parse(__version__).is_devrelease else __version__
 
 del version
```

### Comparing `evaluate-0.4.1/src/evaluate/commands/evaluate_cli.py` & `evaluate-0.4.2/src/evaluate/commands/evaluate_cli.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/config.py` & `evaluate-0.4.2/src/evaluate/config.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/evaluation_suite/__init__.py` & `evaluate-0.4.2/src/evaluate/evaluation_suite/__init__.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/evaluator/__init__.py` & `evaluate-0.4.2/src/evaluate/evaluator/__init__.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/evaluator/audio_classification.py` & `evaluate-0.4.2/src/evaluate/evaluator/audio_classification.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/evaluator/automatic_speech_recognition.py` & `evaluate-0.4.2/src/evaluate/evaluator/automatic_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/evaluator/base.py` & `evaluate-0.4.2/src/evaluate/evaluator/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
             n_resamples=n_resamples,
             random_state=random_state,
         )
 
         # TODO: To clarify why `wer` and `cer` return float
         # even though metric.compute contract says that it
         # returns Optional[dict].
-        if type(metric_results) == float:
+        if type(metric_results) is float:
             metric_results = {metric.name: metric_results}
 
         result.update(metric_results)
         result.update(perf_results)
 
         return result
```

### Comparing `evaluate-0.4.1/src/evaluate/evaluator/image_classification.py` & `evaluate-0.4.2/src/evaluate/evaluator/image_classification.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/evaluator/question_answering.py` & `evaluate-0.4.2/src/evaluate/evaluator/question_answering.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/evaluator/text2text_generation.py` & `evaluate-0.4.2/src/evaluate/evaluator/text2text_generation.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/evaluator/text_classification.py` & `evaluate-0.4.2/src/evaluate/evaluator/text_classification.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/evaluator/text_generation.py` & `evaluate-0.4.2/src/evaluate/evaluator/text_generation.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/evaluator/token_classification.py` & `evaluate-0.4.2/src/evaluate/evaluator/token_classification.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/evaluator/utils.py` & `evaluate-0.4.2/src/evaluate/evaluator/utils.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/hub.py` & `evaluate-0.4.2/src/evaluate/hub.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/info.py` & `evaluate-0.4.2/src/evaluate/info.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/inspect.py` & `evaluate-0.4.2/src/evaluate/inspect.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/loading.py` & `evaluate-0.4.2/src/evaluate/loading.py`

 * *Files 0% similar despite different names*

```diff
@@ -737,15 +737,15 @@
     Returns:
         [`evaluate.EvaluationModule`]
 
     Example:
 
         ```py
         >>> from evaluate import load
-        >>> accuracy = evaluate.load("accuracy")
+        >>> accuracy = load("accuracy")
         ```
     """
     download_mode = DownloadMode(download_mode or DownloadMode.REUSE_DATASET_IF_EXISTS)
     evaluation_module = evaluation_module_factory(
         path, module_type=module_type, revision=revision, download_config=download_config, download_mode=download_mode
     )
     evaluation_cls = import_main_class(evaluation_module.module_path)
```

### Comparing `evaluate-0.4.1/src/evaluate/module.py` & `evaluate-0.4.2/src/evaluate/module.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,34 +43,39 @@
 
 class FileFreeLock(BaseFileLock):
     """Thread lock until a file **cannot** be locked"""
 
     def __init__(self, lock_file, *args, **kwargs):
         self.filelock = FileLock(lock_file)
         super().__init__(lock_file, *args, **kwargs)
+        self._lock_file_fd = None
 
     def _acquire(self):
         try:
-            self.filelock.acquire(timeout=0.01, poll_intervall=0.02)  # Try to lock once
+            self.filelock.acquire(timeout=0.01, poll_interval=0.02)  # Try to lock once
         except Timeout:
             # We couldn't acquire the lock, the file is locked!
             self._lock_file_fd = self.filelock.lock_file
         else:
             # We were able to acquire the lock, the file is not yet locked!
             self.filelock.release()
             self._lock_file_fd = None
 
     def _release(self):
         self._lock_file_fd = None
 
+    @property
+    def is_locked(self) -> bool:
+        return self._lock_file_fd is not None
+
 
 # lists - summarize long lists similarly to NumPy
 # arrays/tensors - let the frameworks control formatting
 def summarize_if_long_list(obj):
-    if not type(obj) == list or len(obj) <= 6:
+    if type(obj) is not list or len(obj) <= 6:
         return f"{obj}"
 
     def format_chunk(chunk):
         return ", ".join(repr(x) for x in chunk)
 
     return f"[{format_chunk(obj[:3])}, ..., {format_chunk(obj[-3:])}]"
```

### Comparing `evaluate-0.4.1/src/evaluate/naming.py` & `evaluate-0.4.2/src/evaluate/naming.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/saving.py` & `evaluate-0.4.2/src/evaluate/saving.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/utils/__init__.py` & `evaluate-0.4.2/src/evaluate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/utils/file_utils.py` & `evaluate-0.4.2/src/evaluate/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/utils/gradio.py` & `evaluate-0.4.2/src/evaluate/utils/gradio.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/utils/logging.py` & `evaluate-0.4.2/src/evaluate/utils/logging.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate/visualization.py` & `evaluate-0.4.2/src/evaluate/visualization.py`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate.egg-info/PKG-INFO` & `evaluate-0.4.2/src/evaluate.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evaluate
-Version: 0.4.1
+Version: 0.4.2
 Summary: HuggingFace community-driven open-source library of evaluation
 Home-page: https://github.com/huggingface/evaluate
 Author: HuggingFace Inc.
 Author-email: leandro@huggingface.co
 License: Apache 2.0
 Download-URL: https://github.com/huggingface/evaluate/tags
 Keywords: metrics machine learning evaluate evaluation
@@ -12,20 +12,19 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: tensorflow
 Provides-Extra: tensorflow_gpu
 Provides-Extra: torch
 Provides-Extra: dev
 Provides-Extra: tests
 Provides-Extra: quality
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: evaluate Version: 0.4.1 Summary: HuggingFace
+Metadata-Version: 2.1 Name: evaluate Version: 0.4.2 Summary: HuggingFace
 community-driven open-source library of evaluation Home-page: https://
 github.com/huggingface/evaluate Author: HuggingFace Inc. Author-email:
 leandro@huggingface.co License: Apache 2.0 Download-URL: https://github.com/
 huggingface/evaluate/tags Keywords: metrics machine learning evaluate
 evaluation Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown Provides-Extra: tensorflow Provides-
-Extra: tensorflow_gpu Provides-Extra: torch Provides-Extra: dev Provides-Extra:
-tests Provides-Extra: quality Provides-Extra: docs Provides-Extra: template
-Provides-Extra: evaluator License-File: LICENSE
+:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.8.0 Description-Content-Type: text/markdown Provides-
+Extra: tensorflow Provides-Extra: tensorflow_gpu Provides-Extra: torch
+Provides-Extra: dev Provides-Extra: tests Provides-Extra: quality Provides-
+Extra: docs Provides-Extra: template Provides-Extra: evaluator License-File:
+LICENSE
 
     [https://huggingface.co/datasets/evaluate/media/resolve/main/evaluate-
                                   banner.png]
      _[_B_u_i_l_d_]_[_G_i_t_H_u_b_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_]_[_C_o_n_t_r_i_b_u_t_o_r_ _C_o_v_e_n_a_n_t_]
 ð¤ Evaluate is a library that makes evaluating and comparing models and
 reporting their performance easier and more standardized. It currently
 contains: - **implementations of dozens of popular metrics**: the existing
```

### Comparing `evaluate-0.4.1/src/evaluate.egg-info/SOURCES.txt` & `evaluate-0.4.2/src/evaluate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evaluate-0.4.1/src/evaluate.egg-info/requires.txt` & `evaluate-0.4.2/src/evaluate.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 requests>=2.19.0
 tqdm>=4.62.1
 xxhash
 multiprocess
 fsspec[http]>=2021.05.0
 huggingface-hub>=0.7.0
 packaging
-responses<0.19
 
 [:python_version < "3.8"]
 importlib_metadata
 
 [dev]
 absl-py
 charcut>=1.1.1
@@ -25,15 +24,15 @@
 tensorflow!=2.6.0,!=2.6.1,<=2.10,>=2.3
 torch
 accelerate
 bert_score>=0.3.6
 rouge_score>=0.1.2
 sacrebleu
 sacremoses
-scipy
+scipy>=1.10.0
 seqeval
 scikit-learn
 jiwer
 sentencepiece
 transformers
 mauve-text
 trectools
@@ -83,15 +82,15 @@
 tensorflow!=2.6.0,!=2.6.1,<=2.10,>=2.3
 torch
 accelerate
 bert_score>=0.3.6
 rouge_score>=0.1.2
 sacrebleu
 sacremoses
-scipy
+scipy>=1.10.0
 seqeval
 scikit-learn
 jiwer
 sentencepiece
 transformers
 mauve-text
 trectools
```

