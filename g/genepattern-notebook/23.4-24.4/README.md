# Comparing `tmp/genepattern-notebook-23.4.tar.gz` & `tmp/genepattern-notebook-24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genepattern-notebook-23.4.tar", last modified: Tue Apr 18 15:52:54 2023, max compression
+gzip compressed data, was "genepattern-notebook-24.4.tar", last modified: Tue Apr 30 16:28:46 2024, max compression
```

## Comparing `genepattern-notebook-23.4.tar` & `genepattern-notebook-24.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-04-18 15:52:54.492458 genepattern-notebook-23.4/
--rw-r--r--   0 tmtabor    (501) staff       (20)     1562 2022-01-03 20:10:07.000000 genepattern-notebook-23.4/LICENSE.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)       67 2022-01-03 20:10:07.000000 genepattern-notebook-23.4/MANIFEST.in
--rw-r--r--   0 tmtabor    (501) staff       (20)     7983 2023-04-18 15:52:54.492571 genepattern-notebook-23.4/PKG-INFO
--rw-r--r--   0 tmtabor    (501) staff       (20)     7019 2022-04-20 16:34:45.000000 genepattern-notebook-23.4/README.md
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-04-18 15:52:54.490228 genepattern-notebook-23.4/genepattern/
--rw-r--r--   0 tmtabor    (501) staff       (20)      534 2023-04-17 17:48:15.000000 genepattern-notebook-23.4/genepattern/__init__.py
--rw-r--r--   0 tmtabor    (501) staff       (20)     7752 2023-04-17 17:43:14.000000 genepattern-notebook-23.4/genepattern/authwidget.py
--rw-r--r--   0 tmtabor    (501) staff       (20)      859 2022-09-12 21:39:43.000000 genepattern-notebook-23.4/genepattern/display.py
--rw-r--r--   0 tmtabor    (501) staff       (20)    13696 2022-10-27 20:54:28.000000 genepattern-notebook-23.4/genepattern/jobwidget.py
--rw-r--r--   0 tmtabor    (501) staff       (20)     3294 2022-04-25 16:13:37.000000 genepattern-notebook-23.4/genepattern/sessions.py
--rw-r--r--   0 tmtabor    (501) staff       (20)     5103 2022-04-20 16:34:37.000000 genepattern-notebook-23.4/genepattern/shim.py
--rw-r--r--   0 tmtabor    (501) staff       (20)    15956 2022-09-22 21:16:50.000000 genepattern-notebook-23.4/genepattern/taskwidget.py
--rw-r--r--   0 tmtabor    (501) staff       (20)     9476 2022-10-27 20:20:12.000000 genepattern-notebook-23.4/genepattern/utils.py
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-04-18 15:52:54.491763 genepattern-notebook-23.4/genepattern_notebook.egg-info/
--rw-r--r--   0 tmtabor    (501) staff       (20)     7983 2023-04-18 15:52:53.000000 genepattern-notebook-23.4/genepattern_notebook.egg-info/PKG-INFO
--rw-r--r--   0 tmtabor    (501) staff       (20)      485 2023-04-18 15:52:54.000000 genepattern-notebook-23.4/genepattern_notebook.egg-info/SOURCES.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)        1 2023-04-18 15:52:53.000000 genepattern-notebook-23.4/genepattern_notebook.egg-info/dependency_links.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)       81 2023-04-18 15:52:54.000000 genepattern-notebook-23.4/genepattern_notebook.egg-info/requires.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)       12 2023-04-18 15:52:54.000000 genepattern-notebook-23.4/genepattern_notebook.egg-info/top_level.txt
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-04-18 15:52:54.491998 genepattern-notebook-23.4/nbtools/
--rw-r--r--   0 tmtabor    (501) staff       (20)       29 2022-04-20 16:34:37.000000 genepattern-notebook-23.4/nbtools/genepattern.json
--rw-r--r--   0 tmtabor    (501) staff       (20)       79 2023-04-18 15:52:54.492970 genepattern-notebook-23.4/setup.cfg
--rwxr-xr-x   0 tmtabor    (501) staff       (20)     1556 2023-04-17 19:06:30.000000 genepattern-notebook-23.4/setup.py
+drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2024-04-30 16:28:46.988620 genepattern-notebook-24.4/
+-rw-r--r--   0 tmtabor    (501) staff       (20)     1562 2022-01-03 20:10:07.000000 genepattern-notebook-24.4/LICENSE.txt
+-rw-r--r--   0 tmtabor    (501) staff       (20)       67 2022-01-03 20:10:07.000000 genepattern-notebook-24.4/MANIFEST.in
+-rw-r--r--   0 tmtabor    (501) staff       (20)     7984 2024-04-30 16:28:46.988754 genepattern-notebook-24.4/PKG-INFO
+-rw-r--r--   0 tmtabor    (501) staff       (20)     7019 2023-06-22 20:48:00.000000 genepattern-notebook-24.4/README.md
+drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2024-04-30 16:28:46.986363 genepattern-notebook-24.4/genepattern/
+-rw-r--r--   0 tmtabor    (501) staff       (20)      534 2024-04-30 16:28:04.000000 genepattern-notebook-24.4/genepattern/__init__.py
+-rw-r--r--   0 tmtabor    (501) staff       (20)     8516 2024-01-25 20:55:49.000000 genepattern-notebook-24.4/genepattern/authwidget.py
+-rw-r--r--   0 tmtabor    (501) staff       (20)      859 2023-06-22 20:48:00.000000 genepattern-notebook-24.4/genepattern/display.py
+-rw-r--r--   0 tmtabor    (501) staff       (20)    13974 2024-02-07 18:08:15.000000 genepattern-notebook-24.4/genepattern/jobwidget.py
+-rw-r--r--   0 tmtabor    (501) staff       (20)     3294 2023-06-22 20:48:00.000000 genepattern-notebook-24.4/genepattern/sessions.py
+-rw-r--r--   0 tmtabor    (501) staff       (20)     5103 2023-06-22 20:48:00.000000 genepattern-notebook-24.4/genepattern/shim.py
+-rw-r--r--   0 tmtabor    (501) staff       (20)    16103 2024-03-13 16:39:37.000000 genepattern-notebook-24.4/genepattern/taskwidget.py
+-rw-r--r--   0 tmtabor    (501) staff       (20)     9476 2023-06-22 20:48:00.000000 genepattern-notebook-24.4/genepattern/utils.py
+drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2024-04-30 16:28:46.987792 genepattern-notebook-24.4/genepattern_notebook.egg-info/
+-rw-r--r--   0 tmtabor    (501) staff       (20)     7984 2024-04-30 16:28:46.000000 genepattern-notebook-24.4/genepattern_notebook.egg-info/PKG-INFO
+-rw-r--r--   0 tmtabor    (501) staff       (20)      485 2024-04-30 16:28:46.000000 genepattern-notebook-24.4/genepattern_notebook.egg-info/SOURCES.txt
+-rw-r--r--   0 tmtabor    (501) staff       (20)        1 2024-04-30 16:28:46.000000 genepattern-notebook-24.4/genepattern_notebook.egg-info/dependency_links.txt
+-rw-r--r--   0 tmtabor    (501) staff       (20)       81 2024-04-30 16:28:46.000000 genepattern-notebook-24.4/genepattern_notebook.egg-info/requires.txt
+-rw-r--r--   0 tmtabor    (501) staff       (20)       12 2024-04-30 16:28:46.000000 genepattern-notebook-24.4/genepattern_notebook.egg-info/top_level.txt
+drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2024-04-30 16:28:46.988050 genepattern-notebook-24.4/nbtools/
+-rw-r--r--   0 tmtabor    (501) staff       (20)       29 2023-06-22 20:48:00.000000 genepattern-notebook-24.4/nbtools/genepattern.json
+-rw-r--r--   0 tmtabor    (501) staff       (20)       79 2024-04-30 16:28:46.989207 genepattern-notebook-24.4/setup.cfg
+-rwxr-xr-x   0 tmtabor    (501) staff       (20)     1557 2024-04-30 16:27:50.000000 genepattern-notebook-24.4/setup.py
```

### Comparing `genepattern-notebook-23.4/LICENSE.txt` & `genepattern-notebook-24.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genepattern-notebook-23.4/PKG-INFO` & `genepattern-notebook-24.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: genepattern-notebook
-Version: 23.4
+Version: 24.4
 Summary: GenePattern Notebook extension for JupyterLab
 Home-page: https://github.com/genepattern/genepattern-notebook
-Download-URL: https://github.com/genepattern/genepattern-notebook/archive/23.4.tar.gz
+Download-URL: https://github.com/genepattern/genepattern-notebook/archive/24.04.tar.gz
 Author: Thorin Tabor
 Author-email: tmtabor@cloud.ucsd.edu
 License: BSD
 Keywords: genepattern,genomics,bioinformatics,ipython,jupyter
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `genepattern-notebook-23.4/README.md` & `genepattern-notebook-24.4/README.md`

 * *Files identical despite different names*

### Comparing `genepattern-notebook-23.4/genepattern/__init__.py` & `genepattern-notebook-24.4/genepattern/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,11 +2,11 @@
 from .taskwidget import GPTaskWidget, reproduce_job, load_task
 from .jobwidget import GPJobWidget
 from .sessions import session, get_session, register_session
 from .display import display
 from nbtools import UIBuilder as GPUIBuilder, UIOutput as GPUIOutput, build_ui, open
 
 __author__ = 'Thorin Tabor'
-__copyright__ = 'Copyright 2014-2023, Regents of the University of California & Broad Institute'
-__version__ = '23.04'
+__copyright__ = 'Copyright 2014-2024, Regents of the University of California & Broad Institute'
+__version__ = '24.04'
 __status__ = 'Production'
 __license__ = 'BSD-3-Clause'
```

### Comparing `genepattern-notebook-23.4/genepattern/authwidget.py` & `genepattern-notebook-24.4/genepattern/authwidget.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import gp
 from IPython.display import display
 from urllib.error import HTTPError
-from nbtools import UIBuilder, ToolManager, NBTool, EventManager
+from nbtools import UIBuilder, ToolManager, NBTool, EventManager, DataManager, Data
 from .sessions import session
 from .shim import login, system_message
+from .jobwidget import GPJobWidget
 from .taskwidget import TaskTool
 from .utils import GENEPATTERN_LOGO, GENEPATTERN_SERVERS, server_name, session_color
 
 
 REGISTER_EVENT = """
     const target = event.target;
     const widget = target.closest('.nbtools') || target;
@@ -106,14 +107,15 @@
             # Call the superclass constructor with the spec
             UIBuilder.__init__(self, self.login, **kwargs)
 
     def prepare_session(self):
         """Prepare a valid session by registering the session and modules"""
         self.register_session()     # Register the session with the SessionList
         self.register_modules()     # Register the modules with the ToolManager
+        self.register_jobs()        # Add recent jobs to the data panel
         self.system_message()       # Display the system message
         self.trigger_login()        # Trigger login callbacks of job and task widgets
 
     def login(self, server, username, password):
         """Login to the GenePattern server"""
         # Assign login values to session
         self.session.url = server
@@ -173,14 +175,28 @@
         else: message = system_message(self.session)
         self.info = message
 
     def trigger_login(self):
         """Dispatch a login event after authentication"""
         EventManager.instance().dispatch("gp.login", self.session)
 
+    def register_jobs(self):
+        data_list = []
+        for job in self.session.get_recent_jobs():
+            origin = server_name(self.session.url)
+            group = f"{job.job_number}. {job.task_name}"
+
+            # Register a custom data group widget (GPJobWidget) with the manager
+            DataManager.instance().group_widget(origin=origin, group=group, widget=GPJobWidget(job))
+
+            # Add data entries for all output files
+            for file in job.get_output_files():
+                data_list.append(Data(origin=origin, group=group, uri=file.get_url()))
+        DataManager.instance().register_all(data_list)
+
 
 class AuthenticationTool(NBTool):
     """Tool wrapper for the authentication widget"""
     origin = '+'
     id = 'authentication'
     name = 'GenePattern Login'
     description = 'Log into a GenePattern server'
```

### Comparing `genepattern-notebook-23.4/genepattern/display.py` & `genepattern-notebook-24.4/genepattern/display.py`

 * *Files identical despite different names*

### Comparing `genepattern-notebook-23.4/genepattern/jobwidget.py` & `genepattern-notebook-24.4/genepattern/jobwidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,20 +57,24 @@
                 self.job.get_info()
             except HTTPError:  # Handle HTTP errors contacting the server
                 self.name = 'Error Loading Job'
                 self.error = f'Error loading job #{self.job.job_number}'
                 return
 
             # Add the job information to the widget
-            self.name = f'Job #{self.job.job_number}'
+            self.name = f'{self.job.job_number}. {self.job.task_name}'
+            self.origin = server_name(self.job.server_data.url)
             self.status = self.status_text()
             self.description = self.submitted_text()
             self.files = self.files_list()
             self.visualization = self.visualizer()
 
+            # Register any output files
+            self.register_data()
+
             # Send notification if completed
             self.handle_notification()
 
             # Update the menu items
             self.attach_terminate()
             self.extra_file_menu_items = {
                 'Send to Code': {
@@ -233,20 +237,23 @@
         cancel_button = Button(description='Cancel')
         cancel_button.on_click(lambda b: self.toggle_job_sharing())
 
         # Save sharing permissions functionality
         def save_permissions(button):
             save_perms = []
             for g in group_widgets:
+                # Special case for public jobs
+                group_name = '*' if g.description == 'All Users' else g.description
+
                 if g.value == 'Read & Write':
-                    save_perms.append({'id': g.description, 'read': True, 'write': True})
+                    save_perms.append({'id': group_name, 'read': True, 'write': True})
                 elif g.value == 'Read':
-                    save_perms.append({'id': g.description, 'read': True, 'write': False})
+                    save_perms.append({'id': group_name, 'read': True, 'write': False})
                 else:
-                    save_perms.append({'id': g.description, 'read': False, 'write': False})
+                    save_perms.append({'id': group_name, 'read': False, 'write': False})
             # Save the permissions, using the shim if necessary
             if hasattr(self.job, 'set_permissions'):
                 self.job.set_permissions(save_perms)
             else:
                 set_permissions(self.job, save_perms)
             self.toggle_job_sharing()
```

### Comparing `genepattern-notebook-23.4/genepattern/sessions.py` & `genepattern-notebook-24.4/genepattern/sessions.py`

 * *Files identical despite different names*

### Comparing `genepattern-notebook-23.4/genepattern/shim.py` & `genepattern-notebook-24.4/genepattern/shim.py`

 * *Files identical despite different names*

### Comparing `genepattern-notebook-23.4/genepattern/taskwidget.py` & `genepattern-notebook-24.4/genepattern/taskwidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import inspect
 import json
 import os
+from decimal import Decimal
 from urllib.request import Request, urlopen
 from urllib.error import HTTPError
 from gp import GPTask
 from IPython.display import display
 from ipywidgets import Output
 from .jobwidget import GPJobWidget
 from nbtools import NBTool, UIBuilder, UIOutput, python_safe, EventManager
@@ -27,14 +28,15 @@
         name_map = {}  # Map of Python-safe parameter names to GP parameter names
 
         # Function for submitting a new GenePattern job based on the task form
         def submit_job(**kwargs):
             spec = task.make_job_spec()
             for name, value in kwargs.items():
                 if value is None: value = ''    # Handle the case of blank optional parameters
+                if isinstance(value, float): value = Decimal(str(value)).__format__('f')  # Handle scientific notation
                 spec.set_parameter(name_map[name], value)
             job = task.server_data.run_job(spec, wait_until_done=False)
             display(GPJobWidget(job, logo='none', color=session_color(self.task.server_data.url, secondary_color=True)))
 
         # Function for adding a parameter with a safe name
         def add_param(param_list, p):
             safe_name = python_safe(p.name)
```

### Comparing `genepattern-notebook-23.4/genepattern/utils.py` & `genepattern-notebook-24.4/genepattern/utils.py`

 * *Files identical despite different names*

### Comparing `genepattern-notebook-23.4/genepattern_notebook.egg-info/PKG-INFO` & `genepattern-notebook-24.4/genepattern_notebook.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: genepattern-notebook
-Version: 23.4
+Version: 24.4
 Summary: GenePattern Notebook extension for JupyterLab
 Home-page: https://github.com/genepattern/genepattern-notebook
-Download-URL: https://github.com/genepattern/genepattern-notebook/archive/23.4.tar.gz
+Download-URL: https://github.com/genepattern/genepattern-notebook/archive/24.04.tar.gz
 Author: Thorin Tabor
 Author-email: tmtabor@cloud.ucsd.edu
 License: BSD
 Keywords: genepattern,genomics,bioinformatics,ipython,jupyter
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `genepattern-notebook-23.4/setup.py` & `genepattern-notebook-24.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 
-__version__ = '23.4'
+__version__ = '24.04'
 
 
 with open('README.md') as f:
     long_description = f.read()
 
 
 setup(name='genepattern-notebook',
```

