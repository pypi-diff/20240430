# Comparing `tmp/EcoStock-0.4.8.tar.gz` & `tmp/EcoStock-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EcoStock-0.4.8.tar", last modified: Tue Apr 30 16:07:44 2024, max compression
+gzip compressed data, was "EcoStock-0.5.tar", last modified: Tue Apr 30 18:15:25 2024, max compression
```

## Comparing `EcoStock-0.4.8.tar` & `EcoStock-0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 16:07:44.126445 EcoStock-0.4.8/
-drwxrwxrwx   0        0        0        0 2024-04-30 16:07:44.118558 EcoStock-0.4.8/EcoStock/
--rw-rw-rw-   0        0        0     1324 2024-04-30 16:07:02.000000 EcoStock-0.4.8/EcoStock/__init__.py
--rw-rw-rw-   0        0        0    37245 2024-04-30 15:46:50.000000 EcoStock-0.4.8/EcoStock/adalo.py
--rw-rw-rw-   0        0        0    10701 2024-04-30 15:37:58.000000 EcoStock-0.4.8/EcoStock/api.py
--rw-rw-rw-   0        0        0    19977 2024-04-30 15:43:00.000000 EcoStock-0.4.8/EcoStock/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:07:44.124989 EcoStock-0.4.8/EcoStock.egg-info/
--rw-rw-rw-   0        0        0     1735 2024-04-30 16:07:44.000000 EcoStock-0.4.8/EcoStock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-04-30 16:07:44.000000 EcoStock-0.4.8/EcoStock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 16:07:44.000000 EcoStock-0.4.8/EcoStock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2024-04-30 16:07:44.000000 EcoStock-0.4.8/EcoStock.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-30 16:07:44.000000 EcoStock-0.4.8/EcoStock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2024-04-29 07:13:36.000000 EcoStock-0.4.8/LICENSE.md
--rw-rw-rw-   0        0        0     1735 2024-04-30 16:07:44.125404 EcoStock-0.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     1121 2024-04-29 08:30:40.000000 EcoStock-0.4.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-30 16:07:44.126445 EcoStock-0.4.8/setup.cfg
--rw-rw-rw-   0        0        0     1075 2024-04-30 16:06:41.000000 EcoStock-0.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 18:15:25.885397 EcoStock-0.5/
+drwxrwxrwx   0        0        0        0 2024-04-30 18:15:25.880181 EcoStock-0.5/EcoStock/
+-rw-rw-rw-   0        0        0     1322 2024-04-30 18:14:54.000000 EcoStock-0.5/EcoStock/__init__.py
+-rw-rw-rw-   0        0        0    38261 2024-04-30 18:09:11.000000 EcoStock-0.5/EcoStock/adalo.py
+-rw-rw-rw-   0        0        0    10398 2024-04-30 18:09:58.000000 EcoStock-0.5/EcoStock/api.py
+-rw-rw-rw-   0        0        0    19977 2024-04-30 16:55:46.000000 EcoStock-0.5/EcoStock/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-30 18:15:25.884461 EcoStock-0.5/EcoStock.egg-info/
+-rw-rw-rw-   0        0        0     1733 2024-04-30 18:15:25.000000 EcoStock-0.5/EcoStock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-04-30 18:15:25.000000 EcoStock-0.5/EcoStock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 18:15:25.000000 EcoStock-0.5/EcoStock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2024-04-30 18:15:25.000000 EcoStock-0.5/EcoStock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-30 18:15:25.000000 EcoStock-0.5/EcoStock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2024-04-29 07:13:36.000000 EcoStock-0.5/LICENSE.md
+-rw-rw-rw-   0        0        0     1733 2024-04-30 18:15:25.885397 EcoStock-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1121 2024-04-29 08:30:40.000000 EcoStock-0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-30 18:15:25.886395 EcoStock-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1073 2024-04-30 18:14:36.000000 EcoStock-0.5/setup.py
```

### Comparing `EcoStock-0.4.8/EcoStock/__init__.py` & `EcoStock-0.5/EcoStock/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """
 Economic-Finance Correlation Package
 
 A Python package for investigating the correlation between economic and financial data.
 """
 
-__version__ = "0.4.8"
+__version__ = "0.5"
 
 from .api import app
 from .adalo import (
     temporary_file,
     candlestick, 
     bollinger_bands,
     correlation,
```

### Comparing `EcoStock-0.4.8/EcoStock/adalo.py` & `EcoStock-0.5/EcoStock/adalo.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,14 +59,18 @@
         # Add grid and legend
         ax.grid(True)
         ax.legend()
 
         # Auto format date labels
         fig.autofmt_xdate()
 
+        # Check if 'static' directory exists, if not, create it
+        if not os.path.exists('static'):
+            os.makedirs('static')
+
         # Use the temporary_file context manager to create a temporary file
         with temporary_file(suffix='.png', dir='static') as filename:
             # Save the plot directly to the temporary file
             fig.savefig(filename)
 
             # Construct the image URL
             image_url = f"https://ecofin-496487b9809a.herokuapp.com/images/{os.path.basename(filename)}"
@@ -197,14 +201,18 @@
         if formatter is not None:
             ax2.yaxis.set_major_formatter(formatter)
 
         fig.legend(loc="upper left", bbox_to_anchor=(0,1), bbox_transform=ax1.transAxes)
         plt.title(f'Correlation between {ticker} Price and {econ_label}: {correlation:.2f}')
         fig.tight_layout()
 
+        # Check if 'static' directory exists, if not, create it
+        if not os.path.exists('static'):
+            os.makedirs('static')
+
         # Use the temporary_file context manager to create a temporary file
         with temporary_file(suffix='.png', dir='static') as filename:
             # Save the plot directly to the temporary file
             fig.savefig(filename)
 
             # Construct the image URL
             image_url = f"https://ecofin-496487b9809a.herokuapp.com/images/{os.path.basename(filename)}"
@@ -345,14 +353,18 @@
         formatter = mdates.AutoDateFormatter(locator)
         ax.xaxis.set_major_locator(locator)
         ax.xaxis.set_major_formatter(formatter)
 
         # Auto format date labels
         fig.autofmt_xdate()
 
+        # Check if 'static' directory exists, if not, create it
+        if not os.path.exists('static'):
+            os.makedirs('static')
+
         # Use the temporary_file context manager to create a temporary file
         with temporary_file(suffix='.png', dir='static') as filename:
             # Save the plot directly to the temporary file
             fig.savefig(filename)
 
             # Construct the image URL
             image_url = f"https://ecofin-496487b9809a.herokuapp.com/images/{os.path.basename(filename)}"
@@ -460,14 +472,18 @@
 
             formatter = mticker.FuncFormatter(lambda x, pos: human_format(x))
         else:
             formatter = None
 
         if formatter is not None:
             ax.yaxis.set_major_formatter(formatter)
+        
+        # Check if 'static' directory exists, if not, create it
+        if not os.path.exists('static'):
+            os.makedirs('static')
 
         with temporary_file(suffix='.png', dir='static') as filename:
             fig.savefig(filename)
             image_url = f"https://ecofin-496487b9809a.herokuapp.com/images/{os.path.basename(filename)}"
             return {"image_url": image_url}
 
     except Exception as e:
@@ -606,14 +622,18 @@
         # Add grid and legend with smaller font size
         ax.grid(True)
         ax.legend(fontsize='x-small')
 
         # Auto format date labels
         fig.autofmt_xdate()
 
+        # Check if 'static' directory exists, if not, create it
+        if not os.path.exists('static'):
+            os.makedirs('static')
+
         # Use the temporary_file context manager to create a temporary file
         with temporary_file(suffix='.png', dir='static') as filename:
             # Save the plot directly to the temporary file
             fig.savefig(filename)
 
             # Construct the image URL
             image_url = f"https://ecofin-496487b9809a.herokuapp.com/images/{os.path.basename(filename)}"
@@ -741,14 +761,18 @@
         ax[2].set_ylabel('MACD')
         ax[2].legend(fontsize='x-small')
         ax[2].grid(True)
         
         fig.autofmt_xdate()
         fig.tight_layout()
 
+        # Check if 'static' directory exists, if not, create it
+        if not os.path.exists('static'):
+            os.makedirs('static')
+
         # Use the temporary_file context manager to create a temporary file
         with temporary_file(suffix='.png', dir='static') as filename:
             # Save the plot directly to the temporary file
             fig.savefig(filename)
 
             # Construct the image URL
             image_url = f"https://ecofin-496487b9809a.herokuapp.com/images/{os.path.basename(filename)}"
@@ -901,14 +925,18 @@
         plt.title('Portfolio Cumulative Returns')
         plt.xlabel('Date')
         plt.ylabel('Cumulative Return (%)')
 
         # Auto format date labels
         fig.autofmt_xdate()
 
+        # Check if 'static' directory exists, if not, create it
+        if not os.path.exists('static'):
+            os.makedirs('static')
+
         # Use the temporary_file context manager to create a temporary file
         with temporary_file(suffix='.png', dir='static') as filename:
             # Save the plot directly to the temporary file
             fig.savefig(filename)
 
             # Construct the image URL
             image_url = f"https://ecofin-496487b9809a.herokuapp.com/images/{os.path.basename(filename)}"
```

### Comparing `EcoStock-0.4.8/EcoStock/api.py` & `EcoStock-0.5/EcoStock/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,12 @@
 from fastapi import FastAPI, HTTPException,Response
-from fastapi.staticfiles import StaticFiles
 import base64
 import argparse
 import uvicorn
-from EcoStock.functions import (
-    get_stock_data,
-    moving_avg_stock_data,
-    get_world_bank_data
-)
 from EcoStock.adalo import (
-    temporary_file,
     candlestick, 
     bollinger_bands,
     correlation, 
     indicator_for_countries, 
     stock_correlation, 
     get_news,
     stock_prediction,
@@ -25,17 +18,14 @@
     stock_correlation_json,
     stock_prediction_json,
     portfolio_return_json
     )
 
 app = FastAPI()
 
-# Mount the 'static' directory at the path '/images'
-app.mount("/images", StaticFiles(directory="static"), name="static")
-
 @app.get("/")
 async def read_root():
     return {"results": {
     "message": "Welcome to EcoStock API!"
   }}
 
 @app.get("/candlestick_json/{ticker}/{start_date}/{end_date}")
```

### Comparing `EcoStock-0.4.8/EcoStock/functions.py` & `EcoStock-0.5/EcoStock/functions.py`

 * *Files identical despite different names*

### Comparing `EcoStock-0.4.8/EcoStock.egg-info/PKG-INFO` & `EcoStock-0.5/EcoStock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 0.4.8
+Version: 0.5
 Summary: A Python package for investigating the correlation between economic and financial data.
 Home-page: https://github.com/Tonij10/fastapi-project
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo and Francesco Caldo
 Author-email: antoniopaparo@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EcoStock-0.4.8/LICENSE.md` & `EcoStock-0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `EcoStock-0.4.8/PKG-INFO` & `EcoStock-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 0.4.8
+Version: 0.5
 Summary: A Python package for investigating the correlation between economic and financial data.
 Home-page: https://github.com/Tonij10/fastapi-project
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo and Francesco Caldo
 Author-email: antoniopaparo@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EcoStock-0.4.8/README.md` & `EcoStock-0.5/README.md`

 * *Files identical despite different names*

### Comparing `EcoStock-0.4.8/setup.py` & `EcoStock-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='EcoStock',
-    version='0.4.8',
+    version='0.5',
     author="Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo and Francesco Caldo",
     author_email="antoniopaparo@outlook.com",
     description='A Python package for investigating the correlation between economic and financial data.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Tonij10/fastapi-project",
     packages=find_packages(),
```

