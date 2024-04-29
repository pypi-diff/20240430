# Comparing `tmp/specsy-0.2.0.tar.gz` & `tmp/specsy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specsy-0.2.0.tar", last modified: Mon Apr 29 22:11:14 2024, max compression
+gzip compressed data, was "specsy-0.2.1.tar", last modified: Mon Apr 29 22:37:07 2024, max compression
```

## Comparing `specsy-0.2.0.tar` & `specsy-0.2.1.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:11:14.839356 specsy-0.2.0/
--rw-rw-r--   0 vital     (1000) vital     (1000)       17 2024-04-29 21:50:58.000000 specsy-0.2.0/MANIFEST.in
--rw-r--r--   0 vital     (1000) vital     (1000)     1883 2024-04-29 22:11:14.839356 specsy-0.2.0/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)      866 2024-04-29 21:50:58.000000 specsy-0.2.0/README.rst
--rw-rw-r--   0 vital     (1000) vital     (1000)     1221 2024-04-29 21:50:58.000000 specsy-0.2.0/pyproject.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)      431 2024-04-29 22:11:14.839356 specsy-0.2.0/setup.cfg
--rw-rw-r--   0 vital     (1000) vital     (1000)     1324 2024-04-29 21:50:58.000000 specsy-0.2.0/setup.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:11:14.835355 specsy-0.2.0/src/
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:11:14.835355 specsy-0.2.0/src/specsy/
--rw-rw-r--   0 vital     (1000) vital     (1000)      878 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)      759 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/core.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:11:14.835355 specsy-0.2.0/src/specsy/inference/
--rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/inference/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    16792 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/inference/emission.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:11:14.835355 specsy-0.2.0/src/specsy/innate/
--rw-rw-r--   0 vital     (1000) vital     (1000)       90 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/innate/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4246 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/innate/interpol_pytensor.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     3795 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/innate/main.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    12905 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/io.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:11:14.839356 specsy-0.2.0/src/specsy/models/
--rw-rw-r--   0 vital     (1000) vital     (1000)      243 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/models/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    16099 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/models/chemistry.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     5282 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/models/chemistry_inference.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    17176 2024-04-29 21:57:45.000000 specsy-0.2.0/src/specsy/models/emissivity.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    22583 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/models/extinction.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/models/fluxes_line.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     8332 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/models/nebular_continuum.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:11:14.839356 specsy-0.2.0/src/specsy/operations/
--rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/operations/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    10732 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/operations/interpolation.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/operations/pytensors.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4631 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/operations/tensors.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     1329 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/operations/tests.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    16155 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/plots.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:11:14.839356 specsy-0.2.0/src/specsy/resources/
--rw-rw-r--   0 vital     (1000) vital     (1000)      419 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/resources/Benjamin1999_OpticalDepthFunctionCoefficients.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    21375 2024-04-29 21:50:58.000000 specsy-0.2.0/src/specsy/resources/HI_t3_elec.ascii
--rw-rw-r--   0 vital     (1000) vital     (1000)    44530 2024-04-29 21:50:59.000000 specsy-0.2.0/src/specsy/resources/HeII_t4_elec.ascii
--rw-rw-r--   0 vital     (1000) vital     (1000)   326042 2024-04-29 21:50:59.000000 specsy-0.2.0/src/specsy/resources/HeI_t5_elec.ascii
--rw-rw-r--   0 vital     (1000) vital     (1000)      451 2024-04-29 21:50:59.000000 specsy-0.2.0/src/specsy/resources/gordon_2003_LMC2_supershell.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      476 2024-04-29 21:50:59.000000 specsy-0.2.0/src/specsy/resources/gordon_2003_LMC_average.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      483 2024-04-29 21:50:59.000000 specsy-0.2.0/src/specsy/resources/gordon_2003_SMC_bar.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)     2887 2024-04-29 21:50:59.000000 specsy-0.2.0/src/specsy/tools.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    10339 2024-04-29 21:50:59.000000 specsy-0.2.0/src/specsy/treatement.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:11:14.839356 specsy-0.2.0/src/specsy/workflow/
--rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:59.000000 specsy-0.2.0/src/specsy/workflow/__init__.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:11:14.835355 specsy-0.2.0/src/specsy.egg-info/
--rw-r--r--   0 vital     (1000) vital     (1000)     1883 2024-04-29 22:11:14.000000 specsy-0.2.0/src/specsy.egg-info/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)     1287 2024-04-29 22:11:14.000000 specsy-0.2.0/src/specsy.egg-info/SOURCES.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-04-29 22:11:14.000000 specsy-0.2.0/src/specsy.egg-info/dependency_links.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      270 2024-04-29 22:11:14.000000 specsy-0.2.0/src/specsy.egg-info/requires.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        7 2024-04-29 22:11:14.000000 specsy-0.2.0/src/specsy.egg-info/top_level.txt
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:37:07.851678 specsy-0.2.1/
+-rw-rw-r--   0 vital     (1000) vital     (1000)       17 2024-04-29 21:50:58.000000 specsy-0.2.1/MANIFEST.in
+-rw-r--r--   0 vital     (1000) vital     (1000)     1883 2024-04-29 22:37:07.851678 specsy-0.2.1/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)      866 2024-04-29 21:50:58.000000 specsy-0.2.1/README.rst
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1221 2024-04-29 22:34:09.000000 specsy-0.2.1/pyproject.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)      431 2024-04-29 22:37:07.851678 specsy-0.2.1/setup.cfg
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1535 2024-04-29 22:29:38.000000 specsy-0.2.1/setup.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:37:07.847678 specsy-0.2.1/src/
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:37:07.847678 specsy-0.2.1/src/specsy/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      878 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     5802 2024-04-29 22:34:09.000000 specsy-0.2.1/src/specsy/config.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)      759 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/core.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:37:07.847678 specsy-0.2.1/src/specsy/inference/
+-rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/inference/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    16792 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/inference/emission.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:37:07.847678 specsy-0.2.1/src/specsy/innate/
+-rw-rw-r--   0 vital     (1000) vital     (1000)       90 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/innate/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4246 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/innate/interpol_pytensor.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     3795 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/innate/main.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    12905 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/io.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:37:07.851678 specsy-0.2.1/src/specsy/models/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      243 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/models/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    16099 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/models/chemistry.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     5282 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/models/chemistry_inference.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17176 2024-04-29 21:57:45.000000 specsy-0.2.1/src/specsy/models/emissivity.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    22583 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/models/extinction.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/models/fluxes_line.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     8332 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/models/nebular_continuum.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:37:07.851678 specsy-0.2.1/src/specsy/operations/
+-rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/operations/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    10732 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/operations/interpolation.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/operations/pytensors.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4631 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/operations/tensors.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1329 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/operations/tests.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    16155 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/plots.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:37:07.851678 specsy-0.2.1/src/specsy/resources/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      419 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/resources/Benjamin1999_OpticalDepthFunctionCoefficients.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    21375 2024-04-29 21:50:58.000000 specsy-0.2.1/src/specsy/resources/HI_t3_elec.ascii
+-rw-rw-r--   0 vital     (1000) vital     (1000)    44530 2024-04-29 21:50:59.000000 specsy-0.2.1/src/specsy/resources/HeII_t4_elec.ascii
+-rw-rw-r--   0 vital     (1000) vital     (1000)   326042 2024-04-29 21:50:59.000000 specsy-0.2.1/src/specsy/resources/HeI_t5_elec.ascii
+-rw-rw-r--   0 vital     (1000) vital     (1000)      451 2024-04-29 21:50:59.000000 specsy-0.2.1/src/specsy/resources/gordon_2003_LMC2_supershell.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      476 2024-04-29 21:50:59.000000 specsy-0.2.1/src/specsy/resources/gordon_2003_LMC_average.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      483 2024-04-29 21:50:59.000000 specsy-0.2.1/src/specsy/resources/gordon_2003_SMC_bar.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2887 2024-04-29 21:50:59.000000 specsy-0.2.1/src/specsy/tools.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    10339 2024-04-29 21:50:59.000000 specsy-0.2.1/src/specsy/treatement.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:37:07.851678 specsy-0.2.1/src/specsy/workflow/
+-rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:59.000000 specsy-0.2.1/src/specsy/workflow/__init__.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:37:07.847678 specsy-0.2.1/src/specsy.egg-info/
+-rw-r--r--   0 vital     (1000) vital     (1000)     1883 2024-04-29 22:37:07.000000 specsy-0.2.1/src/specsy.egg-info/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1310 2024-04-29 22:37:07.000000 specsy-0.2.1/src/specsy.egg-info/SOURCES.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-04-29 22:37:07.000000 specsy-0.2.1/src/specsy.egg-info/dependency_links.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      270 2024-04-29 22:37:07.000000 specsy-0.2.1/src/specsy.egg-info/requires.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        7 2024-04-29 22:37:07.000000 specsy-0.2.1/src/specsy.egg-info/top_level.txt
```

### Comparing `specsy-0.2.0/PKG-INFO` & `specsy-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specsy
-Version: 0.2.0
+Version: 0.2.1
 Summary: Model fitting package for the chemical analysis of astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/specsy
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `specsy-0.2.0/README.rst` & `specsy-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/pyproject.toml` & `specsy-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "specsy"
-version = "0.2.0"
+version = "0.2.1"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {file = "COPYING"}
 authors = [{name = "Vital Fernández", email = "vgf@umich.edu"}]
 description = "Model fitting package for the chemical analysis of astronomical spectra"
 
 dependencies = ["arviz~=0.18",
```

### Comparing `specsy-0.2.0/setup.py` & `specsy-0.2.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,37 +4,39 @@
 from setuptools import setup
 from setuptools import find_packages
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # README
-README = (HERE/"README.rst").read_text()
+README = (HERE / "README.rst").read_text()
 
 # Read lime configuration
 _dir_path = os.path.dirname(os.path.realpath(__file__))
 _setup_cfg = configparser.ConfigParser()
 _setup_cfg.optionxform = str
-_setup_cfg.read(HERE/'setup.cfg')
+_setup_cfg.read(HERE / 'setup.cfg')
 
 # Setup
-setup(
-    name=_setup_cfg['metadata']['name'],
-    version=_setup_cfg['metadata']['version'],
-    author=_setup_cfg['metadata']['author'],
-    author_email=_setup_cfg['metadata']['author_email'],
-    description=_setup_cfg['metadata']['description'],
-    long_description=README,
-    long_description_content_type=_setup_cfg['metadata']['long_description_content_type'],
-    url=_setup_cfg['metadata']['url'],
-    license=_setup_cfg['metadata']['licence'],
-    classifiers=[
-                "License :: OSI Approved :: MIT License",
-                "Programming Language :: Python :: 3",
-                "Programming Language :: Python :: 3.9",
-                ],
-    packages=find_packages('src'),
-    package_dir={'': 'src'},
-    package_data={'':  ['resources/*']},
-    include_package_data=True,
-    install_requires=['numpy', 'matplotlib', 'pandas', 'astropy', 'lime', 'pyneb'],
-    )
+setup(name=_setup_cfg['metadata']['name'],
+      version=_setup_cfg['metadata']['version'],
+      author=_setup_cfg['metadata']['author'],
+      author_email=_setup_cfg['metadata']['author_email'],
+      description=_setup_cfg['metadata']['description'],
+      long_description=README,
+      long_description_content_type=_setup_cfg['metadata']['long_description_content_type'],
+      url=_setup_cfg['metadata']['url'],
+      license=_setup_cfg['metadata']['licence'],
+      classifiers=[
+          "License :: OSI Approved :: MIT License",
+          "Programming Language :: Python :: 3",
+          "Programming Language :: Python :: 3.9",
+      ],
+      packages=find_packages('src'),
+      package_dir={'': 'src'},
+      package_data={'': ['config.toml', 'inference/*', 'innate/*', 'models/*', 'operations/*', 'resources/*', 'workflow/*']},
+      include_package_data=True,
+      install_requires=["arviz", "astropy", "h5netcdf", "jax", "jaxlib", "lime-stable", "lmfit", "matplotlib", "numpy",
+                        "pandas", "pymc", "PyNeb", "pytensor", "scipy", "toml", "xarray"],
+      )
+
+
```

### Comparing `specsy-0.2.0/src/specsy/__init__.py` & `specsy-0.2.1/src/specsy/__init__.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/core.py` & `specsy-0.2.1/src/specsy/core.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/inference/emission.py` & `specsy-0.2.1/src/specsy/inference/emission.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/innate/interpol_pytensor.py` & `specsy-0.2.1/src/specsy/innate/interpol_pytensor.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/innate/main.py` & `specsy-0.2.1/src/specsy/innate/main.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/io.py` & `specsy-0.2.1/src/specsy/io.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/models/chemistry.py` & `specsy-0.2.1/src/specsy/models/chemistry.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/models/chemistry_inference.py` & `specsy-0.2.1/src/specsy/models/chemistry_inference.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/models/emissivity.py` & `specsy-0.2.1/src/specsy/models/emissivity.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/models/extinction.py` & `specsy-0.2.1/src/specsy/models/extinction.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/models/fluxes_line.py` & `specsy-0.2.1/src/specsy/models/fluxes_line.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/models/nebular_continuum.py` & `specsy-0.2.1/src/specsy/models/nebular_continuum.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/operations/interpolation.py` & `specsy-0.2.1/src/specsy/operations/interpolation.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/operations/pytensors.py` & `specsy-0.2.1/src/specsy/operations/pytensors.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/operations/tensors.py` & `specsy-0.2.1/src/specsy/operations/tensors.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/operations/tests.py` & `specsy-0.2.1/src/specsy/operations/tests.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/plots.py` & `specsy-0.2.1/src/specsy/plots.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/resources/HI_t3_elec.ascii` & `specsy-0.2.1/src/specsy/resources/HI_t3_elec.ascii`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/resources/HeII_t4_elec.ascii` & `specsy-0.2.1/src/specsy/resources/HeII_t4_elec.ascii`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/resources/HeI_t5_elec.ascii` & `specsy-0.2.1/src/specsy/resources/HeI_t5_elec.ascii`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/tools.py` & `specsy-0.2.1/src/specsy/tools.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy/treatement.py` & `specsy-0.2.1/src/specsy/treatement.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.0/src/specsy.egg-info/PKG-INFO` & `specsy-0.2.1/src/specsy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specsy
-Version: 0.2.0
+Version: 0.2.1
 Summary: Model fitting package for the chemical analysis of astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/specsy
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `specsy-0.2.0/src/specsy.egg-info/SOURCES.txt` & `specsy-0.2.1/src/specsy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 src/specsy/__init__.py
+src/specsy/config.toml
 src/specsy/core.py
 src/specsy/io.py
 src/specsy/plots.py
 src/specsy/tools.py
 src/specsy/treatement.py
 src/specsy.egg-info/PKG-INFO
 src/specsy.egg-info/SOURCES.txt
```

