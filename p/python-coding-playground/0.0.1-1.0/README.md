# Comparing `tmp/python_coding_playground-0.0.1.tar.gz` & `tmp/python_coding_playground-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_coding_playground-0.0.1.tar", last modified: Tue Apr 30 17:01:15 2024, max compression
+gzip compressed data, was "python_coding_playground-1.0.tar", last modified: Tue Apr 30 16:37:31 2024, max compression
```

## Comparing `python_coding_playground-0.0.1.tar` & `python_coding_playground-1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 17:01:15.230117 python_coding_playground-0.0.1/
--rw-rw-rw-   0        0        0      249 2024-04-30 17:01:15.228123 python_coding_playground-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-30 17:01:15.226128 python_coding_playground-0.0.1/python_coding_playground.egg-info/
--rw-rw-rw-   0        0        0      249 2024-04-30 17:01:15.000000 python_coding_playground-0.0.1/python_coding_playground.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-04-30 17:01:15.000000 python_coding_playground-0.0.1/python_coding_playground.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 17:01:15.000000 python_coding_playground-0.0.1/python_coding_playground.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 17:01:15.000000 python_coding_playground-0.0.1/python_coding_playground.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 17:01:15.230117 python_coding_playground-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1759 2024-04-30 17:01:04.000000 python_coding_playground-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:37:31.752009 python_coding_playground-1.0/
+-rw-rw-rw-   0        0        0      247 2024-04-30 16:37:31.750012 python_coding_playground-1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 16:37:31.730452 python_coding_playground-1.0/python_coding_playground.egg-info/
+-rw-rw-rw-   0        0        0      247 2024-04-30 16:37:31.000000 python_coding_playground-1.0/python_coding_playground.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2024-04-30 16:37:31.000000 python_coding_playground-1.0/python_coding_playground.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 16:37:31.000000 python_coding_playground-1.0/python_coding_playground.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 16:37:31.000000 python_coding_playground-1.0/python_coding_playground.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 16:37:31.752009 python_coding_playground-1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2051 2024-04-30 16:34:51.000000 python_coding_playground-1.0/setup.py
```

### Comparing `python_coding_playground-0.0.1/setup.py` & `python_coding_playground-1.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # Define setup parameters for each package
 setup_params = [
     {
         "name": "cipher_decipher",
         "version": "1.0",
         "packages": find_packages(),
         "author": ["koushik katakam"],
-        "description": "A Spy's Whisper: Encryption & Decryption Of Messages Using Python"
+        "description": "A Spy's Whisper: Encryption & Decryption Of Messages Using Python",
+        "long_description": open(r'C:\Users\koush\Downloads\Demo\cipherdecipher_module\cipher-and-decipher\cipherdecipher.md', encoding='utf-8').read()
     },
     {
         "name": "lc_programs",
         "version": "1.0",
         "packages": find_packages(),
         "author": ["Adarsh Reddy"],
         "description": "lc_programs"
@@ -29,15 +30,16 @@
         "author": ["G.Sai Jyothi"]
     },
     {
         "name": "sdkm",
         "version": "1.0",
         "packages": find_packages(),
         "author": ["Bhargav Naik"],
-        "description": 'sdkm'
+        "description": 'sdkm',
+        "long_description": open(r'C:\Users\koush\Downloads\Demo\Python-Snake_Game-main\Snake-game\ReadMe.md', encoding='utf-8').read()
     },
     {
         "name": "String_methods",
         "version": "1.0",
         "packages": find_packages(),
         "author": ["Meghana"]
     }
@@ -54,11 +56,11 @@
 # Merge setup parameters for all packages
 merged_setup_params = {}
 for params in setup_params:
     name = params.pop("name")  # Remove 'name' to avoid conflicts
     merged_setup_params[name] = params
 
 # Call setup() function with combined author name, name, and version
-setup(name="python_coding_playground",version="0.0.1",author=combined_author, **merged_setup_params)
+setup(name="python_coding_playground", version="1.0 ",author=combined_author, **merged_setup_params)
```

