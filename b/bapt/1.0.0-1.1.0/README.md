# Comparing `tmp/bapt-1.0.0.tar.gz` & `tmp/bapt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bapt-1.0.0.tar", last modified: Fri Oct 20 12:32:33 2017, max compression
+gzip compressed data, was "bapt-1.1.0.tar", last modified: Tue Apr 30 09:50:38 2024, max compression
```

## Comparing `bapt-1.0.0.tar` & `bapt-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0 alex      (1000) alex      (1000)        0 2017-10-20 12:32:33.000000 bapt-1.0.0/
--rw-rw-rw-   0 alex      (1000) alex      (1000)      920 2017-10-20 12:32:33.000000 bapt-1.0.0/PKG-INFO
--rw-rw-rw-   0 alex      (1000) alex      (1000)     1694 2017-10-20 11:32:59.000000 bapt-1.0.0/README.md
-drwxrwxrwx   0 alex      (1000) alex      (1000)        0 2017-10-20 12:32:33.000000 bapt-1.0.0/bapt/
--rw-rw-rw-   0 alex      (1000) alex      (1000)     4351 2017-10-20 11:59:01.000000 bapt-1.0.0/bapt/__init__.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)     3826 2017-10-20 11:40:40.000000 bapt-1.0.0/bapt/cli.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)     3954 2017-10-20 12:00:56.000000 bapt-1.0.0/bapt/plotting.py
-drwxrwxrwx   0 alex      (1000) alex      (1000)        0 2017-10-20 12:32:33.000000 bapt-1.0.0/bapt.egg-info/
--rw-rw-rw-   0 alex      (1000) alex      (1000)      920 2017-10-20 12:32:33.000000 bapt-1.0.0/bapt.egg-info/PKG-INFO
--rw-rw-rw-   0 alex      (1000) alex      (1000)      244 2017-10-20 12:32:33.000000 bapt-1.0.0/bapt.egg-info/SOURCES.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)        1 2017-10-20 12:32:33.000000 bapt-1.0.0/bapt.egg-info/dependency_links.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)       40 2017-10-20 12:32:33.000000 bapt-1.0.0/bapt.egg-info/entry_points.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)       11 2017-10-20 12:32:33.000000 bapt-1.0.0/bapt.egg-info/requires.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)        5 2017-10-20 12:32:33.000000 bapt-1.0.0/bapt.egg-info/top_level.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)      108 2017-10-20 12:32:33.000000 bapt-1.0.0/setup.cfg
--rw-rw-rw-   0 alex      (1000) alex      (1000)     1255 2017-10-20 12:32:27.000000 bapt-1.0.0/setup.py
+drwxr-xr-x   0 alexganose   (501) staff       (20)        0 2024-04-30 09:50:38.881173 bapt-1.1.0/
+-rw-r--r--   0 alexganose   (501) staff       (20)     1068 2023-07-31 08:51:49.000000 bapt-1.1.0/LICENSE
+-rw-r--r--   0 alexganose   (501) staff       (20)      895 2024-04-30 09:50:38.881229 bapt-1.1.0/PKG-INFO
+-rw-r--r--   0 alexganose   (501) staff       (20)     2495 2023-07-31 08:51:49.000000 bapt-1.1.0/README.md
+drwxr-xr-x   0 alexganose   (501) staff       (20)        0 2024-04-30 09:50:38.880346 bapt-1.1.0/bapt/
+-rw-r--r--   0 alexganose   (501) staff       (20)     9823 2024-04-30 09:45:23.000000 bapt-1.1.0/bapt/__init__.py
+-rw-r--r--   0 alexganose   (501) staff       (20)     6888 2023-07-31 08:51:49.000000 bapt-1.1.0/bapt/cli.py
+-rw-r--r--   0 alexganose   (501) staff       (20)     4576 2024-04-30 09:45:23.000000 bapt-1.1.0/bapt/plotting.py
+drwxr-xr-x   0 alexganose   (501) staff       (20)        0 2024-04-30 09:50:38.881060 bapt-1.1.0/bapt.egg-info/
+-rw-r--r--   0 alexganose   (501) staff       (20)      895 2024-04-30 09:50:38.000000 bapt-1.1.0/bapt.egg-info/PKG-INFO
+-rw-r--r--   0 alexganose   (501) staff       (20)      252 2024-04-30 09:50:38.000000 bapt-1.1.0/bapt.egg-info/SOURCES.txt
+-rw-r--r--   0 alexganose   (501) staff       (20)        1 2024-04-30 09:50:38.000000 bapt-1.1.0/bapt.egg-info/dependency_links.txt
+-rw-r--r--   0 alexganose   (501) staff       (20)       39 2024-04-30 09:50:38.000000 bapt-1.1.0/bapt.egg-info/entry_points.txt
+-rw-r--r--   0 alexganose   (501) staff       (20)       23 2024-04-30 09:50:38.000000 bapt-1.1.0/bapt.egg-info/requires.txt
+-rw-r--r--   0 alexganose   (501) staff       (20)        5 2024-04-30 09:50:38.000000 bapt-1.1.0/bapt.egg-info/top_level.txt
+-rw-r--r--   0 alexganose   (501) staff       (20)      108 2024-04-30 09:50:38.881423 bapt-1.1.0/setup.cfg
+-rw-r--r--   0 alexganose   (501) staff       (20)     1270 2024-04-30 09:50:04.000000 bapt-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bapt-1.0.0/PKG-INFO` & `bapt-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: bapt
-Version: 1.0.0
+Version: 1.1.0
 Summary: Band alignment plotting tool
 Home-page: https://github.com/utf/bapt
 Author: Alex Ganose
 Author-email: alexganose@googlemail.com
 License: MIT
-Description: 
-        Get yourself some nice band alignment diagrams
-        
 Keywords: chemistry dft band alignment ionisation potential electron
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
+License-File: LICENSE
+
+
+Get yourself some nice band alignment diagrams
```

### Comparing `bapt-1.0.0/README.md` & `bapt-1.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -30,33 +30,60 @@
 A more advanced plot, generated using the `examples/gradients.yaml` config
 file, allows for additional effects:
 
     bapt --filename examples/gradients.yaml
 
 <img src="https://raw.githubusercontent.com/utf/bapt/master/examples/gradients.png" height="350">
 
+In the alternative case of the relative alignment of bands, without vacuum alignment,
+one can specify the band gap values `--band-gap` alongside the valence band offsets `--vbo`,
+or equivalently the conduction band offsets `--cbo`:
+
+    bapt -n ZnO,MOF-5,COF-1M --band-gap 1.774,1.366,1.6 --cbo 0.247,-0.4
+
+<img src="https://raw.githubusercontent.com/utf/bapt/master/examples/offset.png" height="300">
+
+The band offset approach can also be controlled through a yaml config file. For an example,
+see `examples/offset.yml`.
+
 
 Requirements
 ------------
 
-Bapt is currently compatible with Python 2.7 and Python 3.4. Matplotlib is required 
+Bapt is currently compatible with Python 2.7 and Python 3.4. Matplotlib is required
 for plotting and PyYAML is needed for config files.
 
 Bapt uses Pip and setuptools for installation. You *probably* already
 have this; if not, your GNU/Linux package manager will be able to oblige
 with a package named something like ``python-setuptools``. On Max OSX
 the Python distributed with [Homebrew](<http://brew.sh>) includes
 setuptools and Pip.
 
 
 Installation
 ------------
 
-First clone the this repository, then, from the directory containing this README::
+Bapt is available on PyPI making installation easy:
+
+    pip install --user bapt
+
+Or:
+
+    pip3 install --user bapt
+
+To install the python 3 version.
+
+
+Contributors
+------------
+
+`bapt` was developed by Alex Ganose.
+
+Other contributions are provided by:
 
-    pip3 install --user .
+* Seán Kavanagh through the research groups of David Scanlon at University College London and Aron Walsh at Imperial College London.
 
 
 License
 -------
 
 Bapt is made available under the MIT License.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bapt-1.0.0/bapt/plotting.py` & `bapt-1.1.0/bapt/plotting.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 cb_colours = [(247/255., 148/255., 51/255.), (251/255., 216/255., 181/255.)]
 vb_colours = [(23/255., 71/255., 158/255.), (174/255., 198/255., 242/255.)]
 cb_cmap = LinearSegmentedColormap.from_list('cb', cb_colours, N=200)
 vb_cmap = LinearSegmentedColormap.from_list('vb', vb_colours, N=200)
 
-default_fonts = ['Whitney Book Extended', 'Helvetica', 'Arial', 'Whitney Book'
+default_fonts = ['Whitney Pro', 'Helvetica', 'Arial', 'Whitney Book'
                  'Liberation Sans', 'Andale Sans']
 _ticklabelsize = 15
 _labelsize = 18
 _ticksize = 5
 _linewidth = 1.
 
 
@@ -55,24 +55,39 @@
     ax.set_title(ax.get_title(), size=20)
     for axis in ['top', 'bottom', 'left', 'right']:
         ax.spines[axis].set_linewidth(_linewidth)
 
     ax.set_xlabel(ax.get_xlabel(), size=_labelsize)
     ax.set_ylabel(ax.get_ylabel(), size=_labelsize)
 
-    fonts = default_fonts if fonts is None else fonts + default_fonts
+    fonts = default_fonts if fonts is None or fonts == [None] else fonts + default_fonts
 
     rc('font', **{'family': 'sans-serif', 'sans-serif': fonts})
     rc('text', usetex=False)
     rc('pdf', fonttype=42)
     rc('mathtext', fontset='stixsans')
     rc('legend', handlelength=2)
     return plt
 
 
+def cbar(ax, left, top, face_colour, bar_width=3, bottom=0,
+         show_edge=True, edge_colour='k', edge_zorder=5):
+    X = [[.6, .6], [.7, .7]]
+    right = left + bar_width
+    patch = Rectangle((left, top), bar_width, bottom-top, fill=True,
+                           clip_on=False, facecolor=face_colour,
+                          )
+    ax.add_patch(patch)
+
+    if show_edge:
+        border = Rectangle((left, top), bar_width, bottom-top, fill=False,
+                           lw=_linewidth, edgecolor=edge_colour, clip_on=False,
+                           zorder=edge_zorder)
+        ax.add_patch(border)
+
 def gbar(ax, left, top, bar_width=3, bottom=0, gradient=vb_cmap,
          show_edge=True, edge_colour='k', edge_zorder=5):
     X = [[.6, .6], [.7, .7]]
     right = left + bar_width
     ax.imshow(X, interpolation='bicubic', cmap=gradient,
               extent=(left, right, bottom, top), alpha=1)
```

### Comparing `bapt-1.0.0/bapt.egg-info/PKG-INFO` & `bapt-1.1.0/bapt.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: bapt
-Version: 1.0.0
+Version: 1.1.0
 Summary: Band alignment plotting tool
 Home-page: https://github.com/utf/bapt
 Author: Alex Ganose
 Author-email: alexganose@googlemail.com
 License: MIT
-Description: 
-        Get yourself some nice band alignment diagrams
-        
 Keywords: chemistry dft band alignment ionisation potential electron
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
+License-File: LICENSE
+
+
+Get yourself some nice band alignment diagrams
```

### Comparing `bapt-1.0.0/setup.py` & `bapt-1.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from os.path import abspath, dirname
 from setuptools import setup, find_packages
 
 project_dir = abspath(dirname(__file__))
 
 setup(
     name='bapt',
-    version='1.0.0',
+    version='1.1.0',
     description='Band alignment plotting tool',
     long_description="""
 Get yourself some nice band alignment diagrams
 """,
     url="https://github.com/utf/bapt",
     author="Alex Ganose",
     author_email="alexganose@googlemail.com",
@@ -30,10 +30,10 @@
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Topic :: Scientific/Engineering :: Chemistry',
         'Topic :: Scientific/Engineering :: Physics'
         ],
     keywords='chemistry dft band alignment ionisation potential electron',
     packages=find_packages(),
-    install_requires=['matplotlib'],
+    install_requires=['matplotlib', 'PyYAML>=5.1'],
     entry_points={'console_scripts': ['bapt = bapt.cli:main']}
 )
```

