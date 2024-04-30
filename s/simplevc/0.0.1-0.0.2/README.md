# Comparing `tmp/simplevc-0.0.1.tar.gz` & `tmp/simplevc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simplevc-0.0.1.tar", last modified: Sat Dec 19 00:10:24 2020, max compression
+gzip compressed data, was "simplevc-0.0.2.tar", last modified: Tue Apr 30 02:35:32 2024, max compression
```

## Comparing `simplevc-0.0.1.tar` & `simplevc-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kl945    (1362302) pug-kl945 (1361122)        0 2020-12-19 00:10:24.474296 simplevc-0.0.1/
--rw-r--r--   0 kl945    (1362302) pug-kl945 (1361122)     7148 2020-12-19 00:10:24.472296 simplevc-0.0.1/PKG-INFO
--rw-r--r--   0 kl945    (1362302) pug-kl945 (1361122)     5312 2020-12-18 23:48:59.000000 simplevc-0.0.1/README.md
--rw-r--r--   0 kl945    (1362302) pug-kl945 (1361122)       38 2020-12-19 00:10:24.474296 simplevc-0.0.1/setup.cfg
--rw-r--r--   0 kl945    (1362302) pug-kl945 (1361122)      700 2020-12-19 00:02:46.000000 simplevc-0.0.1/setup.py
-drwxr-xr-x   0 kl945    (1362302) pug-kl945 (1361122)        0 2020-12-19 00:10:24.470296 simplevc-0.0.1/simplevc/
--rw-r--r--   0 kl945    (1362302) pug-kl945 (1361122)       23 2020-12-17 01:50:44.000000 simplevc-0.0.1/simplevc/__init__.py
--rw-r--r--   0 kl945    (1362302) pug-kl945 (1361122)    15163 2020-12-18 20:16:09.000000 simplevc-0.0.1/simplevc/simplevc.py
-drwxr-xr-x   0 kl945    (1362302) pug-kl945 (1361122)        0 2020-12-19 00:10:24.471296 simplevc-0.0.1/simplevc.egg-info/
--rw-r--r--   0 kl945    (1362302) pug-kl945 (1361122)     7148 2020-12-19 00:10:24.000000 simplevc-0.0.1/simplevc.egg-info/PKG-INFO
--rw-r--r--   0 kl945    (1362302) pug-kl945 (1361122)      188 2020-12-19 00:10:24.000000 simplevc-0.0.1/simplevc.egg-info/SOURCES.txt
--rw-r--r--   0 kl945    (1362302) pug-kl945 (1361122)        1 2020-12-19 00:10:24.000000 simplevc-0.0.1/simplevc.egg-info/dependency_links.txt
--rw-r--r--   0 kl945    (1362302) pug-kl945 (1361122)        9 2020-12-19 00:10:24.000000 simplevc-0.0.1/simplevc.egg-info/top_level.txt
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-04-30 02:35:32.024893 simplevc-0.0.2/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5744 2024-04-30 02:35:32.024893 simplevc-0.0.2/PKG-INFO
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5268 2024-04-30 02:34:53.000000 simplevc-0.0.2/README.md
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)       38 2024-04-30 02:35:32.024893 simplevc-0.0.2/setup.cfg
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      700 2024-04-30 02:33:21.000000 simplevc-0.0.2/setup.py
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-04-30 02:35:32.022893 simplevc-0.0.2/simplevc/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)       23 2024-04-30 02:11:58.000000 simplevc-0.0.2/simplevc/__init__.py
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)    15327 2024-04-30 02:24:11.000000 simplevc-0.0.2/simplevc/simplevc.py
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-04-30 02:35:32.022893 simplevc-0.0.2/simplevc.egg-info/
+-rw-r--r--   0 kl945     (5298) hy299_0001 (80905)     5744 2024-04-30 02:35:31.000000 simplevc-0.0.2/simplevc.egg-info/PKG-INFO
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      188 2024-04-30 02:35:31.000000 simplevc-0.0.2/simplevc.egg-info/SOURCES.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)        1 2024-04-30 02:35:31.000000 simplevc-0.0.2/simplevc.egg-info/dependency_links.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)        9 2024-04-30 02:35:31.000000 simplevc-0.0.2/simplevc.egg-info/top_level.txt
```

### Comparing `simplevc-0.0.1/PKG-INFO` & `simplevc-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,179 +1,178 @@
 Metadata-Version: 2.1
 Name: simplevc
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple Python version control package
 Home-page: https://github.com/aldenleung/simplevc/
 Author: Alden Leung
 Author-email: alden.leung@gmail.com
-License: UNKNOWN
-Description: # simplevc - A simple Python version control package
-        
-        
-        A simple library built for version control, backward compatibility and command line scripts on non-standard functions. 
-        
-        Version control is an important practice in writing program. However, due to the large variations across experiments, sometimes researchers may need to build new customized pipelines to handle data generated under various conditions. As data can be generated in multiple batches with many tiny modifications among them, researchers need to update the pipeline rapidly. As time is tight, it could be very challenging to keep everything under standard version control. 
-        
-        This package provides several utilities to make life easier for the researchers when building the pipelines:
-        
-        1. Easy version-control and backward compatibility - One should be able to repeat the analysis and generate the same result, even on an older version of the pipeline.
-        
-        2. Compatibility between python functions and command line scripts - the pipeline can be called as a python function, or in a bash script.
-        
-        3. Reusable in the future - The pipelines can be quickly modified and reused in future analysis.
-        
-        4. Fast to build and easy to learn - Minimize the time to build the pipeline.
-        
-        Here we build this simple version-control library that fulfills the above requirements. Researchers do not need to make drastic changes in the codes, but only:
-        
-        1. Register the module the the version-control system.
-        
-        2. Add version number to the function name.
-        
-        3. Add a decorator to the function.
-        
-        
-        The ideas behind this simple version control system:
-        
-        * There is NO guarantee that the input, output nor behavior of any two versions of the same function remain the same. 
-        
-        * All the old-version functions should be kept for backward compatibility. They should not be modified (Create a new one with newer version number instead).
-        
-        * There is no restriction on the function arguments, except the argument name `version` is reserved for version control.
-        
-        * This is a simple and fast but NOT a standard version control system. It only serves as a utility for development. 
-        
-        ## Installation
-        
-        ```sh
-        pip install simplevc
-        ```
-        
-        ## Usage
-        
-        ### Example module registered for version control
-        
-        ```python
-        
-        ### example/pm.py ###
-        
-        # Suppose you want to set simple version control in pm.py
-        
-        # These three lines are required to register this module with version control
-        import sys
-        import simplevc
-        simplevc.register(sys.modules[__name__])
-        
-        # Definition of some_method with version 20200601
-        @vc
-        def _some_method_20200601(a, b, c):
-        	"""
-        	This is the docstring for method _some_method_20200601
-        	"""
-        	print("Call from _some_method_20200601", a, b, c)
-        
-        # Definition of some_method with version 20200721
-        @vc
-        def _some_method_20200721(a, b, c, d):
-        	"""
-        	This is the docstring for method _some_method_20200721
-        	"""
-        	print("Call from _some_method_20200721", a, b, c, d)
-        
-        @vc
-        def _other_method_20200801(a, b, c, d):
-        	"""
-        	This is the docstring for method _other_method_20200801
-        	"""
-        	# If a method needs to call another method in this module, it is recommended to run the exact version, or the backward compatibility may break.
-        	_some_method_20200721(a, b, c, d)
-        
-        @vt(description="File copy method", helps=dict(srcfile="Input source file", dstfile="Output source file"))
-        @vc
-        def _copy_file_20200701(srcfile:str, dstfile:str):
-        	"""
-        	This is the docstring for method _copy_file_20200701
-        
-        	Copy srcfile to dstfile.
-        	"""
-        	import shutil
-        	shutil.copyfile(srcfile, dstfile)
-        
-        # You can still keep your non version control methods
-        def non_version_control_method():
-        	print("This method is not version controlled.")
-        
-        
-        # This is required if you want this module runnable from shell
-        if __name__ == "__main__":
-        	main()
-        
-        ```
-        
-        ### Using the example module
-        
-        ```python
-        ### In your python console ###
-        
-        from example import pm
-        
-        # Set the pipe methods version to 20200801. By default, date of importing the module is used as the version.  
-        pm.set_version("20200801") 
-        
-        # The exposed methods are _other_method_20200801 and _some_method_20200721
-        # The hidden method is _some_method_20200601
-        
-        # To call the method in the package,
-        pm.some_method("A", "B", "C", "D") # some_method of version 20200721 is selected (we are now using version pre-defined 20200801)
-        # Call from _some_method_20200721 A B C D
-        
-        pm.some_method("A", "B", "C")  # This is an error, because _some_method_20200701 accepts 4 parameters
-        # Error
-        
-        # some_method of version 20200601 is selected
-        pm.some_method("A", "B", "C", version="20200615") # As of version 20200615, only _some_method_20200601 is defined
-        # Call from _some_method_20200601 A B C
-        
-        ```
-        
-        ### Running a function from shell or python
-        
-        ```shell
-        ### Running from shell ###
-        
-        # Running the module, you can find out a list of available methods that can be run from shell. 
-        
-        python example/pm.py
-        
-        #usage: pm.py [-h] {copy_file} ...
-        #
-        #version-20201201
-        #
-        #positional arguments:
-        #  {copy_file}
-        #    copy_file  version-20200701
-        #	
-        #optional arguments:
-        #  -h, --help   show this help message and exit
-        
-        
-        # Running the method copy_file in shell
-        
-        python pm.py copy_file --srcfile my_src_file --dstfile my_dst_file 
-        # The file my_src_file will be copied to my_dst_file
-        
-        ```
-        
-        ```python
-        ### Running from python ###
-        
-        # Running copy_file in python
-        
-        from example import pm
-        pm.copy_file(my_src_file, my_dst_file)
-        ```
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
+
+# simplevc - A simple Python version control package
+
+
+A simple library built for version control, backward compatibility and command line scripts on non-standard functions. 
+
+Version control is an important practice in writing program. However, due to the large variations across experiments, sometimes researchers may need to build new customized pipelines to handle data generated under various conditions. As data can be generated in multiple batches with many tiny modifications among them, researchers need to update the pipeline rapidly. As time is tight, it could be very challenging to keep everything under standard version control. 
+
+This package provides several utilities to make life easier for the researchers when building the pipelines:
+
+1. Easy version-control and backward compatibility - One should be able to repeat the analysis and generate the same result, even on an older version of the pipeline.
+
+2. Compatibility between python functions and command line scripts - the pipeline can be called as a python function, or in a bash script.
+
+3. Reusable in the future - The pipelines can be quickly modified and reused in future analysis.
+
+4. Fast to build and easy to learn - Minimize the time to build the pipeline.
+
+Here we build this simple version-control library that fulfills the above requirements. Researchers do not need to make drastic changes in the codes, but only:
+
+1. Register the module the the version-control system.
+
+2. Add version number to the function name.
+
+3. Add a decorator to the function.
+
+
+The ideas behind this simple version control system:
+
+* There is NO guarantee that the input, output nor behavior of any two versions of the same function remain the same. 
+
+* All the old-version functions should be kept for backward compatibility. They should not be modified (Create a new one with newer version number instead).
+
+* There is no restriction on the function arguments, except the argument name `version` is reserved for version control.
+
+* This is a simple and fast but NOT a standard version control system. 
+
+## Installation
+
+```sh
+pip install simplevc
+```
+
+## Usage
+
+### Example module registered for version control
+
+```python
+
+### example/pm.py ###
+
+# Suppose you want to set simple version control in pm.py
+
+# These three lines are required to register this module with version control
+import sys
+import simplevc
+simplevc.register(sys.modules[__name__])
+
+# Definition of some_method with version 20200601
+@vc
+def _some_method_20200601(a, b, c):
+	"""
+	This is the docstring for method _some_method_20200601
+	"""
+	print("Call from _some_method_20200601", a, b, c)
+
+# Definition of some_method with version 20200721
+@vc
+def _some_method_20200721(a, b, c, d):
+	"""
+	This is the docstring for method _some_method_20200721
+	"""
+	print("Call from _some_method_20200721", a, b, c, d)
+
+@vc
+def _other_method_20200801(a, b, c, d):
+	"""
+	This is the docstring for method _other_method_20200801
+	"""
+	# If a method needs to call another method in this module, it is recommended to run the exact version, or the backward compatibility may break.
+	_some_method_20200721(a, b, c, d)
+
+@vt(description="File copy method", helps=dict(srcfile="Input source file", dstfile="Output source file"))
+@vc
+def _copy_file_20200701(srcfile:str, dstfile:str):
+	"""
+	This is the docstring for method _copy_file_20200701
+
+	Copy srcfile to dstfile.
+	"""
+	import shutil
+	shutil.copyfile(srcfile, dstfile)
+
+# You can still keep your non version control methods
+def non_version_control_method():
+	print("This method is not version controlled.")
+
+
+# This is required if you want this module runnable from shell
+if __name__ == "__main__":
+	main()
+
+```
+
+### Using the example module
+
+```python
+### In your python console ###
+
+from example import pm
+
+# Set the pipe methods version to 20200801. By default, date of importing the module is used as the version.  
+pm.set_version("20200801") 
+
+# The exposed methods are _other_method_20200801 and _some_method_20200721
+# The hidden method is _some_method_20200601
+
+# To call the method in the package,
+pm.some_method("A", "B", "C", "D") # some_method of version 20200721 is selected (we are now using version pre-defined 20200801)
+# Call from _some_method_20200721 A B C D
+
+pm.some_method("A", "B", "C")  # This is an error, because _some_method_20200701 accepts 4 parameters
+# Error
+
+# some_method of version 20200601 is selected
+pm.some_method("A", "B", "C", version="20200615") # As of version 20200615, only _some_method_20200601 is defined
+# Call from _some_method_20200601 A B C
+
+```
+
+### Running a function from shell or python
+
+```shell
+### Running from shell ###
+
+# Running the module, you can find out a list of available methods that can be run from shell. 
+
+python example/pm.py
+
+#usage: pm.py [-h] {copy_file} ...
+#
+#version-20201201
+#
+#positional arguments:
+#  {copy_file}
+#    copy_file  version-20200701
+#	
+#optional arguments:
+#  -h, --help   show this help message and exit
+
+
+# Running the method copy_file in shell
+
+python pm.py copy_file --srcfile my_src_file --dstfile my_dst_file 
+# The file my_src_file will be copied to my_dst_file
+
+```
+
+```python
+### Running from python ###
+
+# Running copy_file in python
+
+from example import pm
+pm.copy_file(my_src_file, my_dst_file)
+```
```

### Comparing `simplevc-0.0.1/README.md` & `simplevc-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 * There is NO guarantee that the input, output nor behavior of any two versions of the same function remain the same. 
 
 * All the old-version functions should be kept for backward compatibility. They should not be modified (Create a new one with newer version number instead).
 
 * There is no restriction on the function arguments, except the argument name `version` is reserved for version control.
 
-* This is a simple and fast but NOT a standard version control system. It only serves as a utility for development. 
+* This is a simple and fast but NOT a standard version control system. 
 
 ## Installation
 
 ```sh
 pip install simplevc
 ```
 
@@ -158,8 +158,8 @@
 ```python
 ### Running from python ###
 
 # Running copy_file in python
 
 from example import pm
 pm.copy_file(my_src_file, my_dst_file)
-```
+```
```

### Comparing `simplevc-0.0.1/setup.py` & `simplevc-0.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as readme_file:
 	readme = readme_file.read()
 
 requirements = []
 
 setup(
 	name="simplevc",
-	version="0.0.1",
+	version="0.0.2",
 	author="Alden Leung",
 	author_email="alden.leung@gmail.com",
 	description="A simple Python version control package",
 	long_description=readme,
 	long_description_content_type="text/markdown",
 	url="https://github.com/aldenleung/simplevc/",
 	packages=find_packages(),
```

### Comparing `simplevc-0.0.1/simplevc/simplevc.py` & `simplevc-0.0.2/simplevc/simplevc.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,15 +297,15 @@
 			display_help = True
 			i += 1
 		else:
 			break
 	if i == len(sys.argv):
 		display_help = True
 	
-	_parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter, description=f"version-{module._version}")
+	_parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter, description=f"version-{module._module_display_version}" if module._module_display_version is not None else "")
 	
 	_subparsers = _parser.add_subparsers(dest='_subparser_name')
 	_return_routines = {} 
 	for func_name, tool_dict in module._tool_dicts.items():
 		version = module._version
 		rversion = _get_last_version(sorted(tool_dict.keys()), version)
 		if rversion is None:
@@ -379,26 +379,26 @@
 			else:
 				getattr(module, _subparser_name)(**vars(args))
 			
 				
 		except argparse.ArgumentError:
 			print("Some errors occur in arguments")
 
-def register(module):
+def register(module, module_display_version=None):
 	'''
 	Register the simple version control system to the target module. 
 	
 	'''
 	global _default_version
 	global _registered_modules
 	
 	setattr(module, "_method_dicts", {})
 	setattr(module, "_tool_dicts", {})
 	set_module_version(module, _default_version)
-	
+	setattr(module, "_module_display_version", module_display_version)
 	
 	def set_version(version):
 		'''
 		Set the module version to use. 
 		
 		:param version: version of format yyyymmdd.
```

### Comparing `simplevc-0.0.1/simplevc.egg-info/PKG-INFO` & `simplevc-0.0.2/simplevc.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,179 +1,178 @@
 Metadata-Version: 2.1
 Name: simplevc
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple Python version control package
 Home-page: https://github.com/aldenleung/simplevc/
 Author: Alden Leung
 Author-email: alden.leung@gmail.com
-License: UNKNOWN
-Description: # simplevc - A simple Python version control package
-        
-        
-        A simple library built for version control, backward compatibility and command line scripts on non-standard functions. 
-        
-        Version control is an important practice in writing program. However, due to the large variations across experiments, sometimes researchers may need to build new customized pipelines to handle data generated under various conditions. As data can be generated in multiple batches with many tiny modifications among them, researchers need to update the pipeline rapidly. As time is tight, it could be very challenging to keep everything under standard version control. 
-        
-        This package provides several utilities to make life easier for the researchers when building the pipelines:
-        
-        1. Easy version-control and backward compatibility - One should be able to repeat the analysis and generate the same result, even on an older version of the pipeline.
-        
-        2. Compatibility between python functions and command line scripts - the pipeline can be called as a python function, or in a bash script.
-        
-        3. Reusable in the future - The pipelines can be quickly modified and reused in future analysis.
-        
-        4. Fast to build and easy to learn - Minimize the time to build the pipeline.
-        
-        Here we build this simple version-control library that fulfills the above requirements. Researchers do not need to make drastic changes in the codes, but only:
-        
-        1. Register the module the the version-control system.
-        
-        2. Add version number to the function name.
-        
-        3. Add a decorator to the function.
-        
-        
-        The ideas behind this simple version control system:
-        
-        * There is NO guarantee that the input, output nor behavior of any two versions of the same function remain the same. 
-        
-        * All the old-version functions should be kept for backward compatibility. They should not be modified (Create a new one with newer version number instead).
-        
-        * There is no restriction on the function arguments, except the argument name `version` is reserved for version control.
-        
-        * This is a simple and fast but NOT a standard version control system. It only serves as a utility for development. 
-        
-        ## Installation
-        
-        ```sh
-        pip install simplevc
-        ```
-        
-        ## Usage
-        
-        ### Example module registered for version control
-        
-        ```python
-        
-        ### example/pm.py ###
-        
-        # Suppose you want to set simple version control in pm.py
-        
-        # These three lines are required to register this module with version control
-        import sys
-        import simplevc
-        simplevc.register(sys.modules[__name__])
-        
-        # Definition of some_method with version 20200601
-        @vc
-        def _some_method_20200601(a, b, c):
-        	"""
-        	This is the docstring for method _some_method_20200601
-        	"""
-        	print("Call from _some_method_20200601", a, b, c)
-        
-        # Definition of some_method with version 20200721
-        @vc
-        def _some_method_20200721(a, b, c, d):
-        	"""
-        	This is the docstring for method _some_method_20200721
-        	"""
-        	print("Call from _some_method_20200721", a, b, c, d)
-        
-        @vc
-        def _other_method_20200801(a, b, c, d):
-        	"""
-        	This is the docstring for method _other_method_20200801
-        	"""
-        	# If a method needs to call another method in this module, it is recommended to run the exact version, or the backward compatibility may break.
-        	_some_method_20200721(a, b, c, d)
-        
-        @vt(description="File copy method", helps=dict(srcfile="Input source file", dstfile="Output source file"))
-        @vc
-        def _copy_file_20200701(srcfile:str, dstfile:str):
-        	"""
-        	This is the docstring for method _copy_file_20200701
-        
-        	Copy srcfile to dstfile.
-        	"""
-        	import shutil
-        	shutil.copyfile(srcfile, dstfile)
-        
-        # You can still keep your non version control methods
-        def non_version_control_method():
-        	print("This method is not version controlled.")
-        
-        
-        # This is required if you want this module runnable from shell
-        if __name__ == "__main__":
-        	main()
-        
-        ```
-        
-        ### Using the example module
-        
-        ```python
-        ### In your python console ###
-        
-        from example import pm
-        
-        # Set the pipe methods version to 20200801. By default, date of importing the module is used as the version.  
-        pm.set_version("20200801") 
-        
-        # The exposed methods are _other_method_20200801 and _some_method_20200721
-        # The hidden method is _some_method_20200601
-        
-        # To call the method in the package,
-        pm.some_method("A", "B", "C", "D") # some_method of version 20200721 is selected (we are now using version pre-defined 20200801)
-        # Call from _some_method_20200721 A B C D
-        
-        pm.some_method("A", "B", "C")  # This is an error, because _some_method_20200701 accepts 4 parameters
-        # Error
-        
-        # some_method of version 20200601 is selected
-        pm.some_method("A", "B", "C", version="20200615") # As of version 20200615, only _some_method_20200601 is defined
-        # Call from _some_method_20200601 A B C
-        
-        ```
-        
-        ### Running a function from shell or python
-        
-        ```shell
-        ### Running from shell ###
-        
-        # Running the module, you can find out a list of available methods that can be run from shell. 
-        
-        python example/pm.py
-        
-        #usage: pm.py [-h] {copy_file} ...
-        #
-        #version-20201201
-        #
-        #positional arguments:
-        #  {copy_file}
-        #    copy_file  version-20200701
-        #	
-        #optional arguments:
-        #  -h, --help   show this help message and exit
-        
-        
-        # Running the method copy_file in shell
-        
-        python pm.py copy_file --srcfile my_src_file --dstfile my_dst_file 
-        # The file my_src_file will be copied to my_dst_file
-        
-        ```
-        
-        ```python
-        ### Running from python ###
-        
-        # Running copy_file in python
-        
-        from example import pm
-        pm.copy_file(my_src_file, my_dst_file)
-        ```
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
+
+# simplevc - A simple Python version control package
+
+
+A simple library built for version control, backward compatibility and command line scripts on non-standard functions. 
+
+Version control is an important practice in writing program. However, due to the large variations across experiments, sometimes researchers may need to build new customized pipelines to handle data generated under various conditions. As data can be generated in multiple batches with many tiny modifications among them, researchers need to update the pipeline rapidly. As time is tight, it could be very challenging to keep everything under standard version control. 
+
+This package provides several utilities to make life easier for the researchers when building the pipelines:
+
+1. Easy version-control and backward compatibility - One should be able to repeat the analysis and generate the same result, even on an older version of the pipeline.
+
+2. Compatibility between python functions and command line scripts - the pipeline can be called as a python function, or in a bash script.
+
+3. Reusable in the future - The pipelines can be quickly modified and reused in future analysis.
+
+4. Fast to build and easy to learn - Minimize the time to build the pipeline.
+
+Here we build this simple version-control library that fulfills the above requirements. Researchers do not need to make drastic changes in the codes, but only:
+
+1. Register the module the the version-control system.
+
+2. Add version number to the function name.
+
+3. Add a decorator to the function.
+
+
+The ideas behind this simple version control system:
+
+* There is NO guarantee that the input, output nor behavior of any two versions of the same function remain the same. 
+
+* All the old-version functions should be kept for backward compatibility. They should not be modified (Create a new one with newer version number instead).
+
+* There is no restriction on the function arguments, except the argument name `version` is reserved for version control.
+
+* This is a simple and fast but NOT a standard version control system. 
+
+## Installation
+
+```sh
+pip install simplevc
+```
+
+## Usage
+
+### Example module registered for version control
+
+```python
+
+### example/pm.py ###
+
+# Suppose you want to set simple version control in pm.py
+
+# These three lines are required to register this module with version control
+import sys
+import simplevc
+simplevc.register(sys.modules[__name__])
+
+# Definition of some_method with version 20200601
+@vc
+def _some_method_20200601(a, b, c):
+	"""
+	This is the docstring for method _some_method_20200601
+	"""
+	print("Call from _some_method_20200601", a, b, c)
+
+# Definition of some_method with version 20200721
+@vc
+def _some_method_20200721(a, b, c, d):
+	"""
+	This is the docstring for method _some_method_20200721
+	"""
+	print("Call from _some_method_20200721", a, b, c, d)
+
+@vc
+def _other_method_20200801(a, b, c, d):
+	"""
+	This is the docstring for method _other_method_20200801
+	"""
+	# If a method needs to call another method in this module, it is recommended to run the exact version, or the backward compatibility may break.
+	_some_method_20200721(a, b, c, d)
+
+@vt(description="File copy method", helps=dict(srcfile="Input source file", dstfile="Output source file"))
+@vc
+def _copy_file_20200701(srcfile:str, dstfile:str):
+	"""
+	This is the docstring for method _copy_file_20200701
+
+	Copy srcfile to dstfile.
+	"""
+	import shutil
+	shutil.copyfile(srcfile, dstfile)
+
+# You can still keep your non version control methods
+def non_version_control_method():
+	print("This method is not version controlled.")
+
+
+# This is required if you want this module runnable from shell
+if __name__ == "__main__":
+	main()
+
+```
+
+### Using the example module
+
+```python
+### In your python console ###
+
+from example import pm
+
+# Set the pipe methods version to 20200801. By default, date of importing the module is used as the version.  
+pm.set_version("20200801") 
+
+# The exposed methods are _other_method_20200801 and _some_method_20200721
+# The hidden method is _some_method_20200601
+
+# To call the method in the package,
+pm.some_method("A", "B", "C", "D") # some_method of version 20200721 is selected (we are now using version pre-defined 20200801)
+# Call from _some_method_20200721 A B C D
+
+pm.some_method("A", "B", "C")  # This is an error, because _some_method_20200701 accepts 4 parameters
+# Error
+
+# some_method of version 20200601 is selected
+pm.some_method("A", "B", "C", version="20200615") # As of version 20200615, only _some_method_20200601 is defined
+# Call from _some_method_20200601 A B C
+
+```
+
+### Running a function from shell or python
+
+```shell
+### Running from shell ###
+
+# Running the module, you can find out a list of available methods that can be run from shell. 
+
+python example/pm.py
+
+#usage: pm.py [-h] {copy_file} ...
+#
+#version-20201201
+#
+#positional arguments:
+#  {copy_file}
+#    copy_file  version-20200701
+#	
+#optional arguments:
+#  -h, --help   show this help message and exit
+
+
+# Running the method copy_file in shell
+
+python pm.py copy_file --srcfile my_src_file --dstfile my_dst_file 
+# The file my_src_file will be copied to my_dst_file
+
+```
+
+```python
+### Running from python ###
+
+# Running copy_file in python
+
+from example import pm
+pm.copy_file(my_src_file, my_dst_file)
+```
```

