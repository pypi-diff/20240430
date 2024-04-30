# Comparing `tmp/python_tgpt-0.6.6.tar.gz` & `tmp/python_tgpt-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_tgpt-0.6.6.tar", last modified: Wed Apr 24 16:45:06 2024, max compression
+gzip compressed data, was "python_tgpt-0.6.7.tar", last modified: Tue Apr 30 16:15:32 2024, max compression
```

## Comparing `python_tgpt-0.6.6.tar` & `python_tgpt-0.6.7.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.301255 python_tgpt-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21914 2024-04-24 16:45:06.301255 python_tgpt-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19001 2024-04-24 16:45:06.000000 python_tgpt-0.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 16:45:06.301255 python_tgpt-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.289255 python_tgpt-0.6.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.289255 python_tgpt-0.6.6/src/pytgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.289255 python_tgpt-0.6.6/src/pytgpt/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/api/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17394 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/api/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.289255 python_tgpt-0.6.6/src/pytgpt/auto/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/auto/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7999 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/auto/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.289255 python_tgpt-0.6.6/src/pytgpt/blackboxai/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/blackboxai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/blackboxai/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    84784 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.289255 python_tgpt-0.6.6/src/pytgpt/gemini/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/gemini/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/gpt4all/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/gpt4all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/gpt4all/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/gpt4free/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/gpt4free/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/gpt4free/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/gpt4free/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/groq/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/groq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/groq/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/imager/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/imager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/imager/imager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/koboldai/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/koboldai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/koboldai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/leo/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/leo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/leo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/llama2/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/llama2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/llama2/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/openai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/opengpt/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/opengpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/opengpt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/perplexity/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/perplexity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/perplexity/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/phind/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/phind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/phind/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/poe/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/poe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/poe/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    33863 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.297255 python_tgpt-0.6.6/src/pytgpt/webchatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/webchatgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/webchatgpt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.297255 python_tgpt-0.6.6/src/pytgpt/yepchat/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/yepchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/yepchat/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.301255 python_tgpt-0.6.6/src/python_tgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21914 2024-04-24 16:45:06.000000 python_tgpt-0.6.6/src/python_tgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-24 16:45:06.000000 python_tgpt-0.6.6/src/python_tgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:45:06.000000 python_tgpt-0.6.6/src/python_tgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 16:45:06.000000 python_tgpt-0.6.6/src/python_tgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-24 16:45:06.000000 python_tgpt-0.6.6/src/python_tgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 16:45:06.000000 python_tgpt-0.6.6/src/python_tgpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.301255 python_tgpt-0.6.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_blackboxai.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_imager.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_koboldai.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_leo.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_opengpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_phind.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_webchatgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.647299 python_tgpt-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21898 2024-04-30 16:15:32.647299 python_tgpt-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18985 2024-04-30 16:15:32.000000 python_tgpt-0.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 16:15:32.647299 python_tgpt-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.631299 python_tgpt-0.6.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.635299 python_tgpt-0.6.7/src/pytgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.635299 python_tgpt-0.6.7/src/pytgpt/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/api/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17394 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/api/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.635299 python_tgpt-0.6.7/src/pytgpt/auto/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/auto/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7999 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/auto/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.635299 python_tgpt-0.6.7/src/pytgpt/blackboxai/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/blackboxai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/blackboxai/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84784 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.635299 python_tgpt-0.6.7/src/pytgpt/gemini/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/gemini/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.635299 python_tgpt-0.6.7/src/pytgpt/gpt4all/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/gpt4all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/gpt4all/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.639299 python_tgpt-0.6.7/src/pytgpt/gpt4free/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/gpt4free/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/gpt4free/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/gpt4free/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.639299 python_tgpt-0.6.7/src/pytgpt/groq/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/groq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/groq/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.639299 python_tgpt-0.6.7/src/pytgpt/imager/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/imager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/imager/imager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.639299 python_tgpt-0.6.7/src/pytgpt/koboldai/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/koboldai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/koboldai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.639299 python_tgpt-0.6.7/src/pytgpt/leo/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/leo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/leo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.639299 python_tgpt-0.6.7/src/pytgpt/llama2/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/llama2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/llama2/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.639299 python_tgpt-0.6.7/src/pytgpt/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/openai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.639299 python_tgpt-0.6.7/src/pytgpt/opengpt/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/opengpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/opengpt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.639299 python_tgpt-0.6.7/src/pytgpt/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/perplexity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/perplexity/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.639299 python_tgpt-0.6.7/src/pytgpt/phind/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/phind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/phind/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.639299 python_tgpt-0.6.7/src/pytgpt/poe/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/poe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/poe/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33871 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.643299 python_tgpt-0.6.7/src/pytgpt/webchatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/webchatgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/webchatgpt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.643299 python_tgpt-0.6.7/src/pytgpt/yepchat/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/yepchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/src/pytgpt/yepchat/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.647299 python_tgpt-0.6.7/src/python_tgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21898 2024-04-30 16:15:32.000000 python_tgpt-0.6.7/src/python_tgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-30 16:15:32.000000 python_tgpt-0.6.7/src/python_tgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:15:32.000000 python_tgpt-0.6.7/src/python_tgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-30 16:15:32.000000 python_tgpt-0.6.7/src/python_tgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-30 16:15:32.000000 python_tgpt-0.6.7/src/python_tgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 16:15:32.000000 python_tgpt-0.6.7/src/python_tgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:15:32.647299 python_tgpt-0.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/tests/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/tests/test_blackboxai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/tests/test_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/tests/test_gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/tests/test_gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/tests/test_groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/tests/test_imager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/tests/test_koboldai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/tests/test_leo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/tests/test_llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/tests/test_opengpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/tests/test_perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/tests/test_phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/tests/test_poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-30 16:15:01.000000 python_tgpt-0.6.7/tests/test_webchatgpt.py
```

### Comparing `python_tgpt-0.6.6/LICENSE` & `python_tgpt-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/PKG-INFO` & `python_tgpt-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tgpt
-Version: 0.6.6
+Version: 0.6.7
 Summary: Interact with AI without API key
 Home-page: https://github.com/Simatwa/python-tgpt
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
@@ -72,15 +72,15 @@
 <p align="center">
 <!--
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 -->
 <a href="https://github.com/Simatwa/python-tgpt/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/python-tgpt"/></a>
 <a href="https://pypi.org/project/python-tgpt"><img alt="PyPi" src="https://img.shields.io/pypi/v/python-tgpt?color=green"/></a>
-<a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
+<a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml"><img alt="Python Package flow" src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml/badge.svg?branch=master"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="https://pepy.tech/project/tgpt2"><img src="https://static.pepy.tech/personalized-badge/tgpt2?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" alt="Downloads"></a>
 <a href="https://pepy.tech/project/python-tgpt"><img src="https://static.pepy.tech/personalized-badge/python-tgpt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" alt="Downloads"></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases/latest"><img src="https://img.shields.io/github/downloads/Simatwa/python-tgpt/total?label=Asset%20Downloads&color=success" alt="Downloads"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/v/release/Simatwa/python-tgpt?color=success&label=Release&logo=github" alt="Latest release"></img></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.6 Summary: Interact with
+Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.7 Summary: Interact with
 AI without API key Home-page: https://github.com/Simatwa/python-tgpt Author:
 Smartwa Author-email: simatwacaleb@proton.me Maintainer: Smartwa License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/python-tgpt Project-URL:
 Source Code, https://github.com/Simatwa/python-tgpt Project-URL: Issue Tracker,
 https://github.com/Simatwa/python-tgpt/issues Project-URL: Download, https://
 github.com/Simatwa/python-tgpt/releases Project-URL: Documentation, https://
```

### Comparing `python_tgpt-0.6.6/README.md` & `python_tgpt-0.6.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 <p align="center">
 <!--
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 -->
 <a href="https://github.com/Simatwa/python-tgpt/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/python-tgpt"/></a>
 <a href="https://pypi.org/project/python-tgpt"><img alt="PyPi" src="https://img.shields.io/pypi/v/python-tgpt?color=green"/></a>
-<a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
+<a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml"><img alt="Python Package flow" src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml/badge.svg?branch=master"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="https://pepy.tech/project/tgpt2"><img src="https://static.pepy.tech/personalized-badge/tgpt2?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" alt="Downloads"></a>
 <a href="https://pepy.tech/project/python-tgpt"><img src="https://static.pepy.tech/personalized-badge/python-tgpt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" alt="Downloads"></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases/latest"><img src="https://img.shields.io/github/downloads/Simatwa/python-tgpt/total?label=Asset%20Downloads&color=success" alt="Downloads"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/v/release/Simatwa/python-tgpt?color=success&label=Release&logo=github" alt="Latest release"></img></a>
```

### Comparing `python_tgpt-0.6.6/setup.py` & `python_tgpt-0.6.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="python-tgpt",
-    version="0.6.6",
+    version="0.6.7",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Interact with AI without API key",
     packages=find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `python_tgpt-0.6.6/src/pytgpt/__init__.py` & `python_tgpt-0.6.7/src/pytgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/api/__init__.py` & `python_tgpt-0.6.7/src/pytgpt/api/__init__.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/api/utils.py` & `python_tgpt-0.6.7/src/pytgpt/api/utils.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/api/v1.py` & `python_tgpt-0.6.7/src/pytgpt/api/v1.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/auto/main.py` & `python_tgpt-0.6.7/src/pytgpt/auto/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/base.py` & `python_tgpt-0.6.7/src/pytgpt/base.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/blackboxai/main.py` & `python_tgpt-0.6.7/src/pytgpt/blackboxai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/console.py` & `python_tgpt-0.6.7/src/pytgpt/console.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/gemini/main.py` & `python_tgpt-0.6.7/src/pytgpt/gemini/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/gpt4all/main.py` & `python_tgpt-0.6.7/src/pytgpt/gpt4all/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/gpt4free/main.py` & `python_tgpt-0.6.7/src/pytgpt/gpt4free/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,17 @@
         self.provider = provider
         self.chat_completion = chat_completion
         self.ignore_working = ignore_working
         self.auth = auth
         self.proxy = None if not proxies else list(proxies.values())[0]
         self.__chat_class = g4f.ChatCompletion if chat_completion else g4f.Completion
 
+    def __str__(self):
+        return f"GPTFREE(provider={self.provider})"
+
     def ask(
         self,
         prompt: str,
         stream: bool = False,
         raw: bool = False,
         optimizer: str = None,
         conversationally: bool = False,
```

### Comparing `python_tgpt-0.6.6/src/pytgpt/gpt4free/utils.py` & `python_tgpt-0.6.7/src/pytgpt/gpt4free/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         self,
     ):
         self.__create_empty_file()
         threads = []
         # Create a progress bar
         total = len(self.working_providers)
         with Progress() as progress:
-            self.__log(20, f"Testing {total} providers : {self.working_providers}")
+            self.__log(20, f"Testing {total} providers : {', '.join(self.working_providers)}")
             task = progress.add_task(
                 f"[cyan]Testing...[{self.test_at_once}]",
                 total=total,
                 visible=self.quiet == False,
             )
             while not progress.finished:
                 for count, provider in enumerate(self.working_providers, start=1):
```

### Comparing `python_tgpt-0.6.6/src/pytgpt/groq/main.py` & `python_tgpt-0.6.7/src/pytgpt/groq/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/imager/imager.py` & `python_tgpt-0.6.7/src/pytgpt/imager/imager.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/koboldai/main.py` & `python_tgpt-0.6.7/src/pytgpt/koboldai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/leo/main.py` & `python_tgpt-0.6.7/src/pytgpt/leo/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/llama2/main.py` & `python_tgpt-0.6.7/src/pytgpt/llama2/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/openai/main.py` & `python_tgpt-0.6.7/src/pytgpt/openai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/opengpt/main.py` & `python_tgpt-0.6.7/src/pytgpt/opengpt/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/perplexity/main.py` & `python_tgpt-0.6.7/src/pytgpt/perplexity/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/phind/main.py` & `python_tgpt-0.6.7/src/pytgpt/phind/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/poe/main.py` & `python_tgpt-0.6.7/src/pytgpt/poe/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/utils.py` & `python_tgpt-0.6.7/src/pytgpt/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
         """
         for key_, value in self.all_acts.items():
             if str(key).lower() in str(key_).lower():
                 return key_
         if raise_not_found:
             raise KeyError(f"Zero awesome prompt found with key - `{key}`")
 
-    def get_acts(self):
+    def get_acts(self) -> dict:
         """Retrieves all awesome-prompts"""
         with open(self.awesome_prompt_path) as fh:
             prompt_dict = json.load(fh)
         return prompt_dict
 
     def update_prompts_from_online(self, override: bool = False):
         """Download awesome-prompts and update existing ones if available
```

### Comparing `python_tgpt-0.6.6/src/pytgpt/webchatgpt/main.py` & `python_tgpt-0.6.7/src/pytgpt/webchatgpt/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/pytgpt/yepchat/main.py` & `python_tgpt-0.6.7/src/pytgpt/yepchat/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/src/python_tgpt.egg-info/PKG-INFO` & `python_tgpt-0.6.7/src/python_tgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tgpt
-Version: 0.6.6
+Version: 0.6.7
 Summary: Interact with AI without API key
 Home-page: https://github.com/Simatwa/python-tgpt
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
@@ -72,15 +72,15 @@
 <p align="center">
 <!--
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 -->
 <a href="https://github.com/Simatwa/python-tgpt/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/python-tgpt"/></a>
 <a href="https://pypi.org/project/python-tgpt"><img alt="PyPi" src="https://img.shields.io/pypi/v/python-tgpt?color=green"/></a>
-<a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
+<a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml"><img alt="Python Package flow" src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml/badge.svg?branch=master"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="https://pepy.tech/project/tgpt2"><img src="https://static.pepy.tech/personalized-badge/tgpt2?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" alt="Downloads"></a>
 <a href="https://pepy.tech/project/python-tgpt"><img src="https://static.pepy.tech/personalized-badge/python-tgpt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" alt="Downloads"></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases/latest"><img src="https://img.shields.io/github/downloads/Simatwa/python-tgpt/total?label=Asset%20Downloads&color=success" alt="Downloads"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/v/release/Simatwa/python-tgpt?color=success&label=Release&logo=github" alt="Latest release"></img></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.6 Summary: Interact with
+Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.7 Summary: Interact with
 AI without API key Home-page: https://github.com/Simatwa/python-tgpt Author:
 Smartwa Author-email: simatwacaleb@proton.me Maintainer: Smartwa License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/python-tgpt Project-URL:
 Source Code, https://github.com/Simatwa/python-tgpt Project-URL: Issue Tracker,
 https://github.com/Simatwa/python-tgpt/issues Project-URL: Download, https://
 github.com/Simatwa/python-tgpt/releases Project-URL: Documentation, https://
```

### Comparing `python_tgpt-0.6.6/src/python_tgpt.egg-info/SOURCES.txt` & `python_tgpt-0.6.7/src/python_tgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/tests/test_api.py` & `python_tgpt-0.6.7/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/tests/test_imager.py` & `python_tgpt-0.6.7/tests/test_imager.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.6/tests/test_utils.py` & `python_tgpt-0.6.7/tests/test_utils.py`

 * *Files identical despite different names*

