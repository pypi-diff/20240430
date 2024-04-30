# Comparing `tmp/outlines-0.0.9.tar.gz` & `tmp/outlines-0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outlines-0.0.9.tar", last modified: Sun Oct 22 19:58:13 2023, max compression
+gzip compressed data, was "/home/remi/projects/normal/outlines-name/dist/.tmp-ukq6qskn/outlines-0.1.dev0.tar", last modified: Wed Mar 22 12:56:36 2023, max compression
```

## Comparing `outlines-0.0.9.tar` & `outlines-0.1.dev0.tar`

### file list

```diff
@@ -1,110 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:13.649498 outlines-0.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:13.633498 outlines-0.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:13.637498 outlines-0.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2023-10-22 19:58:01.000000 outlines-0.0.9/.github/workflows/build_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)      781 2023-10-22 19:58:01.000000 outlines-0.0.9/.github/workflows/publish_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2023-10-22 19:58:01.000000 outlines-0.0.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2023-10-22 19:58:01.000000 outlines-0.0.9/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-22 19:58:01.000000 outlines-0.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-10-22 19:58:01.000000 outlines-0.0.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-10-22 19:58:01.000000 outlines-0.0.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-22 19:58:01.000000 outlines-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14573 2023-10-22 19:58:13.649498 outlines-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12974 2023-10-22 19:58:01.000000 outlines-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:13.637498 outlines-0.0.9/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-10-22 19:58:01.000000 outlines-0.0.9/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2023-10-22 19:58:01.000000 outlines-0.0.9/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:13.637498 outlines-0.0.9/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:13.637498 outlines-0.0.9/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   372647 2023-10-22 19:58:01.000000 outlines-0.0.9/docs/source/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-10-22 19:58:01.000000 outlines-0.0.9/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2023-10-22 19:58:01.000000 outlines-0.0.9/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2023-10-22 19:58:01.000000 outlines-0.0.9/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-10-22 19:58:01.000000 outlines-0.0.9/docs/source/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:13.637498 outlines-0.0.9/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-10-22 19:58:01.000000 outlines-0.0.9/docs/source/reference/batching.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2023-10-22 19:58:01.000000 outlines-0.0.9/docs/source/reference/controlled_generation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2023-10-22 19:58:01.000000 outlines-0.0.9/docs/source/reference/multimodel.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2023-10-22 19:58:01.000000 outlines-0.0.9/docs/source/reference/prompting.rst
--rw-r--r--   0 runner    (1001) docker     (127)      370 2023-10-22 19:58:01.000000 outlines-0.0.9/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:13.641498 outlines-0.0.9/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2023-10-22 19:58:01.000000 outlines-0.0.9/examples/babyagi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8064 2023-10-22 19:58:01.000000 outlines-0.0.9/examples/dating_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2023-10-22 19:58:01.000000 outlines-0.0.9/examples/math_generate_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2023-10-22 19:58:01.000000 outlines-0.0.9/examples/meta_prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2023-10-22 19:58:01.000000 outlines-0.0.9/examples/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-10-22 19:58:01.000000 outlines-0.0.9/examples/pick_odd_one_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2023-10-22 19:58:01.000000 outlines-0.0.9/examples/react.py
--rw-r--r--   0 runner    (1001) docker     (127)    33052 2023-10-22 19:58:01.000000 outlines-0.0.9/examples/sampling.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2023-10-22 19:58:01.000000 outlines-0.0.9/examples/self_consistency.py
--rw-r--r--   0 runner    (1001) docker     (127)    20104 2023-10-22 19:58:01.000000 outlines-0.0.9/examples/simulation_based_inference.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:13.641498 outlines-0.0.9/outlines/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-22 19:58:13.000000 outlines-0.0.9/outlines/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9746 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/caching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:13.641498 outlines-0.0.9/outlines/models/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/models/hf_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14504 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/models/hf_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/models/image_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/models/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/models/routers.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/models/text_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/models/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/models/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:13.645498 outlines-0.0.9/outlines/text/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22669 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/text/fsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/text/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:13.645498 outlines-0.0.9/outlines/text/generate/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/text/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/text/generate/continuation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14251 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/text/generate/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/text/generate/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     8222 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/text/generate/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     9517 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/text/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/text/masks.py
--rw-r--r--   0 runner    (1001) docker     (127)    30668 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/text/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9415 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/text/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:13.645498 outlines-0.0.9/outlines/vectors/
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/vectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2023-10-22 19:58:01.000000 outlines-0.0.9/outlines/vectors/retrieval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:13.641498 outlines-0.0.9/outlines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14573 2023-10-22 19:58:13.000000 outlines-0.0.9/outlines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2023-10-22 19:58:13.000000 outlines-0.0.9/outlines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-22 19:58:13.000000 outlines-0.0.9/outlines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-10-22 19:58:13.000000 outlines-0.0.9/outlines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-22 19:58:13.000000 outlines-0.0.9/outlines.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2023-10-22 19:58:01.000000 outlines-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-10-22 19:58:01.000000 outlines-0.0.9/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2023-10-22 19:58:13.649498 outlines-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:13.645498 outlines-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:13.645498 outlines-0.0.9/tests/models/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/models/test_hf_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/models/test_hf_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/models/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/models/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/test_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:13.645498 outlines-0.0.9/tests/text/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:13.645498 outlines-0.0.9/tests/text/generate/
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/text/generate/test_continuation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9070 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/text/generate/test_integration_transfomers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/text/generate/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/text/generate/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    12049 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/text/generate/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11180 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/text/partial_python.lark
--rw-r--r--   0 runner    (1001) docker     (127)    17055 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/text/test_fsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/text/test_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    16796 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/text/test_json_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/text/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6121 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/text/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/text/test_prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 19:58:13.649498 outlines-0.0.9/tests/vectors/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/vectors/test_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2023-10-22 19:58:01.000000 outlines-0.0.9/tests/vectors/test_vectors.py
+drwxr-xr-x   0 remi      (1000) remi      (1000)        0 2023-03-22 12:56:36.521021 outlines-0.1.dev0/
+-rw-r--r--   0 remi      (1000) remi      (1000)      654 2023-03-22 12:56:36.521021 outlines-0.1.dev0/PKG-INFO
+drwxr-xr-x   0 remi      (1000) remi      (1000)        0 2023-03-22 12:56:36.517687 outlines-0.1.dev0/outlines/
+-rw-r--r--   0 remi      (1000) remi      (1000)        0 2023-03-22 12:55:44.000000 outlines-0.1.dev0/outlines/__init__.py
+-rw-r--r--   0 remi      (1000) remi      (1000)      168 2023-03-22 12:56:36.000000 outlines-0.1.dev0/outlines/_version.py
+drwxr-xr-x   0 remi      (1000) remi      (1000)        0 2023-03-22 12:56:36.517687 outlines-0.1.dev0/outlines.egg-info/
+-rw-r--r--   0 remi      (1000) remi      (1000)      654 2023-03-22 12:56:36.000000 outlines-0.1.dev0/outlines.egg-info/PKG-INFO
+-rw-r--r--   0 remi      (1000) remi      (1000)      184 2023-03-22 12:56:36.000000 outlines-0.1.dev0/outlines.egg-info/SOURCES.txt
+-rw-r--r--   0 remi      (1000) remi      (1000)        1 2023-03-22 12:56:36.000000 outlines-0.1.dev0/outlines.egg-info/dependency_links.txt
+-rw-r--r--   0 remi      (1000) remi      (1000)        9 2023-03-22 12:56:36.000000 outlines-0.1.dev0/outlines.egg-info/top_level.txt
+-rw-r--r--   0 remi      (1000) remi      (1000)      888 2023-03-22 12:55:32.000000 outlines-0.1.dev0/pyproject.toml
+-rw-r--r--   0 remi      (1000) remi      (1000)       38 2023-03-22 12:56:36.521021 outlines-0.1.dev0/setup.cfg
```

