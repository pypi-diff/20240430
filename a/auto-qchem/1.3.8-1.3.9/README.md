# Comparing `tmp/auto-qchem-1.3.8.tar.gz` & `tmp/auto-qchem-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/auto-qchem-1.3.8.tar", last modified: Wed Apr 10 23:29:16 2024, max compression
+gzip compressed data, was "dist/auto-qchem-1.3.9.tar", last modified: Mon Apr 29 23:27:20 2024, max compression
```

## Comparing `auto-qchem-1.3.8.tar` & `auto-qchem-1.3.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-10 23:29:16.000000 auto-qchem-1.3.8/
--rw-r--r--   0 mac        (501) staff       (20)    35149 2022-10-06 20:25:51.000000 auto-qchem-1.3.8/LICENSE.md
--rw-r--r--   0 mac        (501) staff       (20)      306 2024-04-10 23:29:16.000000 auto-qchem-1.3.8/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1452 2024-04-10 21:52:33.000000 auto-qchem-1.3.8/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-10 23:29:16.000000 auto-qchem-1.3.8/auto_qchem.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      306 2024-04-10 23:29:16.000000 auto-qchem-1.3.8/auto_qchem.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      593 2024-04-10 23:29:16.000000 auto-qchem-1.3.8/auto_qchem.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-10 23:29:16.000000 auto-qchem-1.3.8/auto_qchem.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      221 2024-04-10 23:29:16.000000 auto-qchem-1.3.8/auto_qchem.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       10 2024-04-10 23:29:16.000000 auto-qchem-1.3.8/auto_qchem.egg-info/top_level.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-10 23:29:16.000000 auto-qchem-1.3.8/autoqchem/
--rw-r--r--   0 mac        (501) staff       (20)        0 2024-04-10 21:52:33.000000 auto-qchem-1.3.8/autoqchem/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    24645 2024-04-10 21:52:33.000000 auto-qchem-1.3.8/autoqchem/db_functions.py
--rw-r--r--   0 mac        (501) staff       (20)     2587 2022-10-06 20:25:51.000000 auto-qchem-1.3.8/autoqchem/descriptor_functions.py
--rw-r--r--   0 mac        (501) staff       (20)      981 2022-10-06 20:25:51.000000 auto-qchem-1.3.8/autoqchem/draw_utils.py
--rw-r--r--   0 mac        (501) staff       (20)     6445 2024-04-10 21:52:33.000000 auto-qchem-1.3.8/autoqchem/gaussian_input_generator.py
--rw-r--r--   0 mac        (501) staff       (20)    19324 2024-04-10 21:52:33.000000 auto-qchem-1.3.8/autoqchem/gaussian_log_extractor.py
--rw-r--r--   0 mac        (501) staff       (20)     5232 2024-04-10 21:52:33.000000 auto-qchem-1.3.8/autoqchem/helper_classes.py
--rw-r--r--   0 mac        (501) staff       (20)     5162 2024-04-10 23:28:41.000000 auto-qchem-1.3.8/autoqchem/helper_functions.py
--rw-r--r--   0 mac        (501) staff       (20)     2700 2024-04-10 21:52:33.000000 auto-qchem-1.3.8/autoqchem/molecule.py
--rw-r--r--   0 mac        (501) staff       (20)     2274 2023-05-30 22:08:50.000000 auto-qchem-1.3.8/autoqchem/openbabel_utils.py
--rw-r--r--   0 mac        (501) staff       (20)    11508 2024-04-10 21:52:33.000000 auto-qchem-1.3.8/autoqchem/rdkit_utils.py
--rw-r--r--   0 mac        (501) staff       (20)    28641 2024-04-10 22:09:20.000000 auto-qchem-1.3.8/autoqchem/sge_manager.py
--rw-r--r--   0 mac        (501) staff       (20)    26054 2024-04-10 21:52:33.000000 auto-qchem-1.3.8/autoqchem/slurm_manager.py
--rw-r--r--   0 mac        (501) staff       (20)     1374 2023-08-18 17:24:25.000000 auto-qchem-1.3.8/autoqchem/test.py
--rw-r--r--   0 mac        (501) staff       (20)      211 2024-04-10 21:52:33.000000 auto-qchem-1.3.8/config.yml
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-10 23:29:16.000000 auto-qchem-1.3.8/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     1089 2024-04-10 23:28:51.000000 auto-qchem-1.3.8/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-29 23:27:20.000000 auto-qchem-1.3.9/
+-rw-r--r--   0 mac        (501) staff       (20)    35149 2022-10-06 20:25:51.000000 auto-qchem-1.3.9/LICENSE.md
+-rw-r--r--   0 mac        (501) staff       (20)      306 2024-04-29 23:27:20.000000 auto-qchem-1.3.9/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1452 2024-04-29 23:26:01.000000 auto-qchem-1.3.9/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-29 23:27:20.000000 auto-qchem-1.3.9/auto_qchem.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      306 2024-04-29 23:27:19.000000 auto-qchem-1.3.9/auto_qchem.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      593 2024-04-29 23:27:19.000000 auto-qchem-1.3.9/auto_qchem.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-29 23:27:19.000000 auto-qchem-1.3.9/auto_qchem.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      221 2024-04-29 23:27:19.000000 auto-qchem-1.3.9/auto_qchem.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       10 2024-04-29 23:27:19.000000 auto-qchem-1.3.9/auto_qchem.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-29 23:27:20.000000 auto-qchem-1.3.9/autoqchem/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2024-04-29 23:26:01.000000 auto-qchem-1.3.9/autoqchem/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)    24645 2024-04-29 23:26:01.000000 auto-qchem-1.3.9/autoqchem/db_functions.py
+-rw-r--r--   0 mac        (501) staff       (20)     2587 2022-10-06 20:25:51.000000 auto-qchem-1.3.9/autoqchem/descriptor_functions.py
+-rw-r--r--   0 mac        (501) staff       (20)      981 2022-10-06 20:25:51.000000 auto-qchem-1.3.9/autoqchem/draw_utils.py
+-rw-r--r--   0 mac        (501) staff       (20)     6445 2024-04-29 23:26:01.000000 auto-qchem-1.3.9/autoqchem/gaussian_input_generator.py
+-rw-r--r--   0 mac        (501) staff       (20)    19324 2024-04-29 23:26:01.000000 auto-qchem-1.3.9/autoqchem/gaussian_log_extractor.py
+-rw-r--r--   0 mac        (501) staff       (20)     5232 2024-04-29 23:26:01.000000 auto-qchem-1.3.9/autoqchem/helper_classes.py
+-rw-r--r--   0 mac        (501) staff       (20)     5162 2024-04-29 23:26:01.000000 auto-qchem-1.3.9/autoqchem/helper_functions.py
+-rw-r--r--   0 mac        (501) staff       (20)     2700 2024-04-29 23:26:01.000000 auto-qchem-1.3.9/autoqchem/molecule.py
+-rw-r--r--   0 mac        (501) staff       (20)     2274 2023-05-30 22:08:50.000000 auto-qchem-1.3.9/autoqchem/openbabel_utils.py
+-rw-r--r--   0 mac        (501) staff       (20)    11508 2024-04-29 23:26:01.000000 auto-qchem-1.3.9/autoqchem/rdkit_utils.py
+-rw-r--r--   0 mac        (501) staff       (20)    28621 2024-04-29 23:26:26.000000 auto-qchem-1.3.9/autoqchem/sge_manager.py
+-rw-r--r--   0 mac        (501) staff       (20)    26054 2024-04-29 23:26:01.000000 auto-qchem-1.3.9/autoqchem/slurm_manager.py
+-rw-r--r--   0 mac        (501) staff       (20)     1374 2023-08-18 17:24:25.000000 auto-qchem-1.3.9/autoqchem/test.py
+-rw-r--r--   0 mac        (501) staff       (20)      211 2024-04-29 23:26:01.000000 auto-qchem-1.3.9/config.yml
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-29 23:27:20.000000 auto-qchem-1.3.9/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     1089 2024-04-29 23:27:09.000000 auto-qchem-1.3.9/setup.py
```

### Comparing `auto-qchem-1.3.8/LICENSE.md` & `auto-qchem-1.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.8/README.md` & `auto-qchem-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.8/auto_qchem.egg-info/SOURCES.txt` & `auto-qchem-1.3.9/auto_qchem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.8/autoqchem/db_functions.py` & `auto-qchem-1.3.9/autoqchem/db_functions.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.8/autoqchem/descriptor_functions.py` & `auto-qchem-1.3.9/autoqchem/descriptor_functions.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.8/autoqchem/draw_utils.py` & `auto-qchem-1.3.9/autoqchem/draw_utils.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.8/autoqchem/gaussian_input_generator.py` & `auto-qchem-1.3.9/autoqchem/gaussian_input_generator.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.8/autoqchem/gaussian_log_extractor.py` & `auto-qchem-1.3.9/autoqchem/gaussian_log_extractor.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.8/autoqchem/helper_classes.py` & `auto-qchem-1.3.9/autoqchem/helper_classes.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.8/autoqchem/helper_functions.py` & `auto-qchem-1.3.9/autoqchem/helper_functions.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.8/autoqchem/molecule.py` & `auto-qchem-1.3.9/autoqchem/molecule.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.8/autoqchem/openbabel_utils.py` & `auto-qchem-1.3.9/autoqchem/openbabel_utils.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.8/autoqchem/rdkit_utils.py` & `auto-qchem-1.3.9/autoqchem/rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.8/autoqchem/sge_manager.py` & `auto-qchem-1.3.9/autoqchem/sge_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -600,24 +600,24 @@
         output += f"# echo job info to joblog\n" \
                   f"echo 'Job {base_name} started on:   ' `hostname -s`\n" \
                   f"echo 'Job {base_name} started on:   ' `date `\n\n"
 
         output += f"# set job environment and GAUSS_SCRDIR variable\n" \
                   f". /u/local/Modules/default/init/modules.sh\n" \
                   f"module load gaussian/g16_sse4\n" \
+                  f"# another compiled version: gaussian/16_avx\n" \
                   f"export GAUSS_SCRDIR=$TMPDIR\n\n"
 
         output += f"# echo current module used to joblog\n" \
                   f"module li\n" \
                   f'echo "GAUSS_SCRDIR=$GAUSS_SCRDIR"\n' \
-                  f"# another compiled version: $g16root/16_avx/g16\n" \
-                  f"echo '/usr/bin/time -v $g16root/16_sse4/g16 < {base_name}.gjf > {base_name}.log'\n\n" \
+                  f"echo '/usr/bin/time -v $g16root/g16 < {base_name}.gjf > {base_name}.log'\n\n" \
                   f"cd {self.remote_dir}\n" \
                   f"# run command\n" \
-                  f"/usr/bin/time -v $g16root/16_sse4/g16 < {base_name}.gjf > {base_name}.log\n\n" 
+                  f"/usr/bin/time -v $g16root/g16 < {base_name}.gjf > {base_name}.log\n\n" 
 
         output += f"# echo job info to joblog\n" \
                   f"echo 'Job $JOB_ID ended on:   '' `hostname -s`\n" \
                   f"echo 'Job $JOB_ID ended on:   ' `date `"
 
         sh_file_path = f"{directory}/{base_name}.sh"
         with open(sh_file_path, "w") as f:
```

### Comparing `auto-qchem-1.3.8/autoqchem/slurm_manager.py` & `auto-qchem-1.3.9/autoqchem/slurm_manager.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.8/autoqchem/test.py` & `auto-qchem-1.3.9/autoqchem/test.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.8/setup.py` & `auto-qchem-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='auto-qchem',
-    version='1.3.8',
+    version='1.3.9',
     packages=['autoqchem'],
     data_files=['config.yml'],
     url='https://github.com/doyle-lab-ucla/auto-qchem',
     license='GPL',
     author='Andrzej Zuranski, Benjamin Shields, Jason Wang, Winston Gee',
     description='auto-qchem',
     long_description='automated dft calculation management software',
```

