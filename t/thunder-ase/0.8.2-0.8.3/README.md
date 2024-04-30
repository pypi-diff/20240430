# Comparing `tmp/thunder_ase-0.8.2.tar.gz` & `tmp/thunder_ase-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunder_ase-0.8.2.tar", last modified: Tue Apr 16 11:34:11 2024, max compression
+gzip compressed data, was "thunder_ase-0.8.3.tar", last modified: Tue Apr 30 07:09:21 2024, max compression
```

## Comparing `thunder_ase-0.8.2.tar` & `thunder_ase-0.8.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:34:11.506564 thunder_ase-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)     8687 2024-04-16 11:34:11.506564 thunder_ase-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8343 2024-04-16 11:34:06.000000 thunder_ase-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-16 11:34:06.000000 thunder_ase-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 11:34:11.506564 thunder_ase-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 11:34:06.000000 thunder_ase-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:34:11.502565 thunder_ase-0.8.2/thunder_ase/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:34:06.000000 thunder_ase-0.8.2/thunder_ase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33664 2024-04-16 11:34:06.000000 thunder_ase-0.8.2/thunder_ase/fireball.py
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-16 11:34:06.000000 thunder_ase-0.8.2/thunder_ase/optimize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:34:11.506564 thunder_ase-0.8.2/thunder_ase/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-16 11:34:06.000000 thunder_ase-0.8.2/thunder_ase/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-04-16 11:34:06.000000 thunder_ase-0.8.2/thunder_ase/utils/basis_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-04-16 11:34:06.000000 thunder_ase-0.8.2/thunder_ase/utils/mwfn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-16 11:34:06.000000 thunder_ase-0.8.2/thunder_ase/utils/shell_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:34:11.506564 thunder_ase-0.8.2/thunder_ase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8687 2024-04-16 11:34:11.000000 thunder_ase-0.8.2/thunder_ase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-16 11:34:11.000000 thunder_ase-0.8.2/thunder_ase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:34:11.000000 thunder_ase-0.8.2/thunder_ase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 11:34:11.000000 thunder_ase-0.8.2/thunder_ase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 11:34:11.000000 thunder_ase-0.8.2/thunder_ase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:21.555753 thunder_ase-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     8687 2024-04-30 07:09:21.555753 thunder_ase-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8343 2024-04-30 07:09:17.000000 thunder_ase-0.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-30 07:09:17.000000 thunder_ase-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 07:09:21.555753 thunder_ase-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 07:09:17.000000 thunder_ase-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:21.555753 thunder_ase-0.8.3/thunder_ase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:17.000000 thunder_ase-0.8.3/thunder_ase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33671 2024-04-30 07:09:17.000000 thunder_ase-0.8.3/thunder_ase/fireball.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-30 07:09:17.000000 thunder_ase-0.8.3/thunder_ase/optimize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:21.555753 thunder_ase-0.8.3/thunder_ase/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-30 07:09:17.000000 thunder_ase-0.8.3/thunder_ase/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-04-30 07:09:17.000000 thunder_ase-0.8.3/thunder_ase/utils/basis_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-04-30 07:09:17.000000 thunder_ase-0.8.3/thunder_ase/utils/mwfn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-30 07:09:17.000000 thunder_ase-0.8.3/thunder_ase/utils/shell_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:21.555753 thunder_ase-0.8.3/thunder_ase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8687 2024-04-30 07:09:21.000000 thunder_ase-0.8.3/thunder_ase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-30 07:09:21.000000 thunder_ase-0.8.3/thunder_ase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 07:09:21.000000 thunder_ase-0.8.3/thunder_ase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 07:09:21.000000 thunder_ase-0.8.3/thunder_ase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 07:09:21.000000 thunder_ase-0.8.3/thunder_ase.egg-info/top_level.txt
```

### Comparing `thunder_ase-0.8.2/PKG-INFO` & `thunder_ase-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thunder-ase
-Version: 0.8.2
+Version: 0.8.3
 Summary: ASE calculator interface for FIREBALL code
 Author-email: PJ Ren <openrpj@gmail.com>
 Project-URL: Homepage, https://github.com/thunder-dft/thunder-ase
 Project-URL: Bug Tracker, https://github.com/thunder-dft/thunder-ase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `thunder_ase-0.8.2/README.md` & `thunder_ase-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `thunder_ase-0.8.2/pyproject.toml` & `thunder_ase-0.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "thunder-ase"
-version = "0.8.2"
+version = "0.8.3"
 authors = [
   { name="PJ Ren", email="openrpj@gmail.com" },
 ]
 description = "ASE calculator interface for FIREBALL code"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `thunder_ase-0.8.2/thunder_ase/fireball.py` & `thunder_ase-0.8.3/thunder_ase/fireball.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,15 @@
         self.nkpt = fireball_params['nkpt']['default']
         self.kpt_reduced = fireball_params['kpt_reduced']['default']
         self.kpt_gamma = fireball_params['kpt_gamma']['default']
         self._kpoints = None
 
         self.valid_xc = ['blyp', 'lda']
         self.check_kwargs(kwargs)
+        self._kwargs = kwargs
 
     @property
     def atoms(self):
         return self._atoms
 
     @atoms.setter
     def atoms(self, atoms):
@@ -460,35 +461,30 @@
             directory = self.directory
         errorcode = subprocess.call(command,
                                     shell=True,
                                     cwd=directory)
         return errorcode
 
     def read_results(self):
-        # try to read 001.traj first
-        output = self.sname + ".traj"
-        if os.path.isfile(output):
-            atoms = ase.io.read(output)
-            self.results = atoms.arrays
-            return None
+        if self.options_params.get('ipi') == 1:
+            # read 001.traj instead of 001.json
+            output = self.sname + ".traj"
+            if os.path.isfile(output):
+                atoms = ase.io.read(output)
+                self.results = atoms.arrays
+                return None
+        else:
+            output = self.sname + ".json"
+            result = jsonio.read_json(output)
+            if 'charges' in result['fireball'][-1]:
+                shell_charges = result['fireball'][-1]['charges']
+                result['fireball'][-1]['shell_charges'] = shell_charges
+                del (result['fireball'][-1]['charges'])
 
-        output = self.sname + ".json"
-        result = jsonio.read_json(output)
-        if 'charges' in result['fireball'][-1]:
-            shell_charges = result['fireball'][-1]['charges']
-            result['fireball'][-1]['shell_charges'] = shell_charges
-            del (result['fireball'][-1]['charges'])
-
-        self.results = result['fireball'][-1]
-
-        if self.atoms is not None:
-            # update results
-            self.atoms.array.update(self.results)
-            # write current result and atoms to traj
-            self.atoms.write(self.sname+'.traj')
+            self.results = result['fireball'][-1]
 
     def get_charges(self, atoms=None):
         if self.results is None:
             try:
                 self.read_results()
             except AttributeError:
                 return None
@@ -712,51 +708,41 @@
         # write out
         if filename is None:
             filename = self.sname + '.mwfn'
         with open(filename, 'w') as f:
             f.write(content)
 
     def dynamics(self, dyn, **kwargs):
-        assert dyn is not None
-
-        atoms = dyn.atoms
-        dyn.attach(write_current_result, atoms=atoms, sname=self.sname)
-
-        if 'nstepf' not in self.options_params:
-            if 'steps' in kwargs:
-                max_step = kwargs['steps']
-            else:
-                max_step = dyn.max_steps
+        if self.options_params.get('ipi') == 1:
+            atoms = dyn.atoms
+            kwargs.setdefault('steps', self.options_params.get('nstepf', dyn.max_steps))
+            # set FIREBALL nstepf option, unless it will stop after 1 step.
+            self.options_params['nstepf'] = kwargs['steps'] + 1
+            with SocketIOCalculator(self, log=None, unixsocket=self.socket) as calc:
+                atoms.calc = calc
+                dyn.run(**kwargs)
         else:
-            max_step = self.options_params['nstepf']
-        self.options_params['nstepf'] = max_step + 1
-
-        with SocketIOCalculator(self, log=None, unixsocket=self.socket) as calc:
-            atoms.calc = calc
+            print('Warning: Use ipi=1 to implement socket is highly recommended!')
+            print('Warning: Without socket, it reads Fdata every step, which is slow for multi-element systems.')
             dyn.run(**kwargs)
 
     def minimize(self, atoms=None, fmax=0.1, method='MDMin', **kwargs):
         from thunder_ase.optimize import rms_converged
         from importlib import import_module
         opt_module = import_module('thunder_ase.optimize')
         try:
             Optimizer = getattr(opt_module, method)
         except ImportError:
             raise ImportError(method)
 
-        if atoms is None:
-            atoms = self.atoms
-
         atoms.calc = self
-
-        if 'trajectory' not in kwargs:
-            kwargs['trajectory'] = 'minimize.traj'
-        if 'logfile' not in kwargs:
-            kwargs['logfile'] = 'minimize.log'
+        kwargs.setdefault('trajectory', 'minimize.traj')
+        kwargs.setdefault('logfile', 'minimize.log')
         dyn = Optimizer(atoms, **kwargs)
+        dyn.attach(write_current_result, atoms=atoms, sname=self.sname)
         dyn.converged = MethodType(rms_converged, dyn)  # use rms as convergence criteria instead of fmax
         self.dynamics(dyn, fmax=fmax)
 
 
 class MultiFireball:
     name = 'multi_fireball'
```

### Comparing `thunder_ase-0.8.2/thunder_ase/optimize.py` & `thunder_ase-0.8.3/thunder_ase/optimize.py`

 * *Files identical despite different names*

### Comparing `thunder_ase-0.8.2/thunder_ase/utils/__init__.py` & `thunder_ase-0.8.3/thunder_ase/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `thunder_ase-0.8.2/thunder_ase/utils/basis_set.py` & `thunder_ase-0.8.3/thunder_ase/utils/basis_set.py`

 * *Files identical despite different names*

### Comparing `thunder_ase-0.8.2/thunder_ase/utils/mwfn.py` & `thunder_ase-0.8.3/thunder_ase/utils/mwfn.py`

 * *Files identical despite different names*

### Comparing `thunder_ase-0.8.2/thunder_ase/utils/shell_dict.py` & `thunder_ase-0.8.3/thunder_ase/utils/shell_dict.py`

 * *Files identical despite different names*

### Comparing `thunder_ase-0.8.2/thunder_ase.egg-info/PKG-INFO` & `thunder_ase-0.8.3/thunder_ase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thunder-ase
-Version: 0.8.2
+Version: 0.8.3
 Summary: ASE calculator interface for FIREBALL code
 Author-email: PJ Ren <openrpj@gmail.com>
 Project-URL: Homepage, https://github.com/thunder-dft/thunder-ase
 Project-URL: Bug Tracker, https://github.com/thunder-dft/thunder-ase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

