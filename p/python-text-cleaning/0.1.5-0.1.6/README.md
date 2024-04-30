# Comparing `tmp/python_text_cleaning-0.1.5.tar.gz` & `tmp/python_text_cleaning-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_text_cleaning-0.1.5.tar", max compression
+gzip compressed data, was "python_text_cleaning-0.1.6.tar", max compression
```

## Comparing `python_text_cleaning-0.1.5.tar` & `python_text_cleaning-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/LICENSE
--rw-r--r--   0        0        0      759 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/README.md
--rw-r--r--   0        0        0      765 2024-04-29 14:38:56.519110 python_text_cleaning-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       73 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/python_text_cleaning/__init__.py
--rw-r--r--   0        0        0     3889 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/python_text_cleaning/asr_text_cleaning.py
--rw-r--r--   0        0        0      281 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/__init__.py
--rw-r--r--   0        0        0      872 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/cyrillic_character_maps.py
--rw-r--r--   0        0        0      954 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/german_text_cleaners.py
--rw-r--r--   0        0        0     2111 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/latin_character_maps.py
--rw-r--r--   0        0        0     2182 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/misc_language_text_cleaners.py
--rw-r--r--   0        0        0      219 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/not_str_translatable_maps.py
--rw-r--r--   0        0        0     3305 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/text_cleaning.py
--rw-r--r--   0        0        0     1346 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/todo.md
--rw-r--r--   0        0        0     1352 1970-01-01 00:00:00.000000 python_text_cleaning-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-30 09:27:20.046862 python_text_cleaning-0.1.6/LICENSE
+-rw-r--r--   0        0        0      759 2024-04-30 09:27:20.046862 python_text_cleaning-0.1.6/README.md
+-rw-r--r--   0        0        0      765 2024-04-30 09:27:31.211032 python_text_cleaning-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       73 2024-04-30 09:27:20.046862 python_text_cleaning-0.1.6/python_text_cleaning/__init__.py
+-rw-r--r--   0        0        0     3883 2024-04-30 09:27:20.046862 python_text_cleaning-0.1.6/python_text_cleaning/asr_text_cleaning.py
+-rw-r--r--   0        0        0      281 2024-04-30 09:27:20.046862 python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/__init__.py
+-rw-r--r--   0        0        0      872 2024-04-30 09:27:20.046862 python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/cyrillic_character_maps.py
+-rw-r--r--   0        0        0      954 2024-04-30 09:27:20.050862 python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/german_text_cleaners.py
+-rw-r--r--   0        0        0     2111 2024-04-30 09:27:20.050862 python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/latin_character_maps.py
+-rw-r--r--   0        0        0     2182 2024-04-30 09:27:20.050862 python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/misc_language_text_cleaners.py
+-rw-r--r--   0        0        0      219 2024-04-30 09:27:20.050862 python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/not_str_translatable_maps.py
+-rw-r--r--   0        0        0     3305 2024-04-30 09:27:20.050862 python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/text_cleaning.py
+-rw-r--r--   0        0        0     1346 2024-04-30 09:27:20.050862 python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/todo.md
+-rw-r--r--   0        0        0     1352 1970-01-01 00:00:00.000000 python_text_cleaning-0.1.6/PKG-INFO
```

### Comparing `python_text_cleaning-0.1.5/LICENSE` & `python_text_cleaning-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.5/README.md` & `python_text_cleaning-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.5/pyproject.toml` & `python_text_cleaning-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-text-cleaning"
-version = "0.1.5"
+version = "0.1.6"
 description = "mostly mapping characters"
 authors = ["Tilo Himmelsbach <dertilo@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/dertilo/python-text-cleaning"
 
 packages = [{ include = "python_text_cleaning" }]
```

### Comparing `python_text_cleaning-0.1.5/python_text_cleaning/asr_text_cleaning.py` & `python_text_cleaning-0.1.6/python_text_cleaning/asr_text_cleaning.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 class VocabCasingAwareTextCleaner(TextCleaner):
     casing: str | dict | Casing
     text_cleaner_name: str
     letter_vocab: Letters
 
     @property
     def name(self) -> NeStr:
-        return f"{self.casing.value.name}-{self.text_cleaner_name}"
+        return f"{self.casing.name}-{self.text_cleaner_name}"
 
     def __post_init__(self) -> None:
         if isinstance(self.casing, str):
             self.casing = Casing(self.casing)
         elif isinstance(
             self.casing,
             dict,
```

### Comparing `python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/cyrillic_character_maps.py` & `python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/cyrillic_character_maps.py`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/german_text_cleaners.py` & `python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/german_text_cleaners.py`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/latin_character_maps.py` & `python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/latin_character_maps.py`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/misc_language_text_cleaners.py` & `python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/misc_language_text_cleaners.py`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/text_cleaning.py` & `python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/text_cleaning.py`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/todo.md` & `python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/todo.md`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.5/PKG-INFO` & `python_text_cleaning-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-text-cleaning
-Version: 0.1.5
+Version: 0.1.6
 Summary: mostly mapping characters
 Home-page: https://github.com/dertilo/python-text-cleaning
 Author: Tilo Himmelsbach
 Author-email: dertilo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

