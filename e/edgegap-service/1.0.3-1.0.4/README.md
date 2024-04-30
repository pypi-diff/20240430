# Comparing `tmp/edgegap_service-1.0.3.tar.gz` & `tmp/edgegap_service-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_service-1.0.3.tar", max compression
+gzip compressed data, was "edgegap_service-1.0.4.tar", max compression
```

## Comparing `edgegap_service-1.0.3.tar` & `edgegap_service-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1993 2024-04-29 18:44:21.838079 edgegap_service-1.0.3/LICENSE
--rw-r--r--   0        0        0     2188 2024-04-29 18:44:21.838508 edgegap_service-1.0.3/README.md
--rw-r--r--   0        0        0       17 2024-04-29 18:44:21.838719 edgegap_service-1.0.3/edgegap_service/BUILD
--rw-r--r--   0        0        0      164 2024-04-29 18:44:21.838942 edgegap_service-1.0.3/edgegap_service/__init__.py
--rw-r--r--   0        0        0     2662 2024-04-29 18:44:21.839143 edgegap_service-1.0.3/edgegap_service/_configuration.py
--rw-r--r--   0        0        0      733 2024-04-29 18:44:21.839287 edgegap_service-1.0.3/edgegap_service/_documentation.py
--rw-r--r--   0        0        0      714 2024-04-29 18:44:21.839491 edgegap_service-1.0.3/edgegap_service/_environment.py
--rw-r--r--   0        0        0     2208 2024-04-29 18:44:21.839668 edgegap_service-1.0.3/edgegap_service/_logging.py
--rw-r--r--   0        0        0     2318 2024-04-29 18:44:21.839844 edgegap_service-1.0.3/edgegap_service/_scheduling.py
--rw-r--r--   0        0        0     7671 2024-04-29 18:45:11.326263 edgegap_service-1.0.3/edgegap_service/_service.py
--rw-r--r--   0        0        0      739 2024-04-29 18:44:21.840414 edgegap_service-1.0.3/edgegap_service/_templating.py
--rw-r--r--   0        0        0       17 2024-04-29 18:44:21.840524 edgegap_service-1.0.3/edgegap_service/health/BUILD
--rw-r--r--   0        0        0      101 2024-04-29 18:44:21.841176 edgegap_service-1.0.3/edgegap_service/health/__init__.py
--rw-r--r--   0        0        0     1478 2024-04-29 18:44:21.841466 edgegap_service-1.0.3/edgegap_service/health/_health.py
--rw-r--r--   0        0        0      394 2024-04-29 18:44:21.841701 edgegap_service-1.0.3/edgegap_service/health/_model.py
--rw-r--r--   0        0        0       17 2024-04-29 18:44:21.841786 edgegap_service-1.0.3/edgegap_service/health/checks/BUILD
--rw-r--r--   0        0        0      234 2024-04-29 18:44:21.842102 edgegap_service-1.0.3/edgegap_service/health/checks/__init__.py
--rw-r--r--   0        0        0      594 2024-04-29 18:44:21.842322 edgegap_service-1.0.3/edgegap_service/health/checks/_consul.py
--rw-r--r--   0        0        0      740 2024-04-29 18:44:21.842578 edgegap_service-1.0.3/edgegap_service/health/checks/_database.py
--rw-r--r--   0        0        0      590 2024-04-29 18:44:21.842920 edgegap_service-1.0.3/edgegap_service/health/checks/_interface.py
--rw-r--r--   0        0        0      329 2024-04-29 18:44:21.843236 edgegap_service-1.0.3/edgegap_service/health/checks/_model.py
--rw-r--r--   0        0        0     1880 2024-04-29 18:44:21.843536 edgegap_service-1.0.3/edgegap_service/static/html/index.html
--rw-r--r--   0        0        0     4286 2024-04-29 18:44:21.843888 edgegap_service-1.0.3/edgegap_service/static/images/favicon.ico
--rw-r--r--   0        0        0      739 2024-04-29 18:45:35.096052 edgegap_service-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 edgegap_service-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-04-29 18:47:19.869190 edgegap_service-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2188 2024-04-29 18:47:19.869506 edgegap_service-1.0.4/README.md
+-rw-r--r--   0        0        0       17 2024-04-29 18:47:19.869596 edgegap_service-1.0.4/edgegap_service/BUILD
+-rw-r--r--   0        0        0      164 2024-04-29 18:47:19.869784 edgegap_service-1.0.4/edgegap_service/__init__.py
+-rw-r--r--   0        0        0     2653 2024-04-29 18:47:31.945126 edgegap_service-1.0.4/edgegap_service/_configuration.py
+-rw-r--r--   0        0        0      733 2024-04-29 18:47:19.870173 edgegap_service-1.0.4/edgegap_service/_documentation.py
+-rw-r--r--   0        0        0      714 2024-04-29 18:47:19.870454 edgegap_service-1.0.4/edgegap_service/_environment.py
+-rw-r--r--   0        0        0     2208 2024-04-29 18:47:19.870592 edgegap_service-1.0.4/edgegap_service/_logging.py
+-rw-r--r--   0        0        0     2318 2024-04-29 18:47:19.870754 edgegap_service-1.0.4/edgegap_service/_scheduling.py
+-rw-r--r--   0        0        0     7671 2024-04-29 18:47:19.871049 edgegap_service-1.0.4/edgegap_service/_service.py
+-rw-r--r--   0        0        0      739 2024-04-29 18:47:19.871339 edgegap_service-1.0.4/edgegap_service/_templating.py
+-rw-r--r--   0        0        0       17 2024-04-29 18:47:19.871427 edgegap_service-1.0.4/edgegap_service/health/BUILD
+-rw-r--r--   0        0        0      101 2024-04-29 18:47:19.871707 edgegap_service-1.0.4/edgegap_service/health/__init__.py
+-rw-r--r--   0        0        0     1478 2024-04-29 18:47:19.871964 edgegap_service-1.0.4/edgegap_service/health/_health.py
+-rw-r--r--   0        0        0      394 2024-04-29 18:47:19.872227 edgegap_service-1.0.4/edgegap_service/health/_model.py
+-rw-r--r--   0        0        0       17 2024-04-29 18:47:19.872300 edgegap_service-1.0.4/edgegap_service/health/checks/BUILD
+-rw-r--r--   0        0        0      234 2024-04-29 18:47:19.872608 edgegap_service-1.0.4/edgegap_service/health/checks/__init__.py
+-rw-r--r--   0        0        0      594 2024-04-29 18:47:19.872771 edgegap_service-1.0.4/edgegap_service/health/checks/_consul.py
+-rw-r--r--   0        0        0      740 2024-04-29 18:47:19.872959 edgegap_service-1.0.4/edgegap_service/health/checks/_database.py
+-rw-r--r--   0        0        0      590 2024-04-29 18:47:19.873415 edgegap_service-1.0.4/edgegap_service/health/checks/_interface.py
+-rw-r--r--   0        0        0      329 2024-04-29 18:47:19.873589 edgegap_service-1.0.4/edgegap_service/health/checks/_model.py
+-rw-r--r--   0        0        0     1880 2024-04-29 18:47:19.873818 edgegap_service-1.0.4/edgegap_service/static/html/index.html
+-rw-r--r--   0        0        0     4286 2024-04-29 18:47:19.874268 edgegap_service-1.0.4/edgegap_service/static/images/favicon.ico
+-rw-r--r--   0        0        0      739 2024-04-29 18:47:44.300047 edgegap_service-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 edgegap_service-1.0.4/PKG-INFO
```

### Comparing `edgegap_service-1.0.3/LICENSE` & `edgegap_service-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.3/README.md` & `edgegap_service-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.3/edgegap_service/_configuration.py` & `edgegap_service-1.0.4/edgegap_service/_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     depend: Optional[Callable] = Field(default=None, description="The Base Depend Attribute for DB Session")
     port: int = Field(default=8000, description="The Port of the Service")
     host: str = Field(default="0.0.0.0", description="The Host of the Service")
     workers: int = Field(default=1, description="Numbers of Workers, (if you use the scheduler, keep to 1)")
     timeout: int = Field(default=300, description="Default Timeout for Connection")
     worker_class: str = Field(default="uvicorn.workers.UvicornWorker", description="The worker class for ASGI")
     scheduler: Scheduler | None = Field(default=None, description="A Scheduler to start at boot")
-    startup_functions: list[Callable] | None = Field(default=None, description="All function will be called on startup")
+    startup_functions: list[Callable] = Field(default=[], description="All function will be called on startup")
     env_config: EnvironmentConfiguration = Field(
         default=SettingsFactory.from_settings(EnvironmentConfiguration),
         description="The Configuration coming from the Environment Variables"
     )
     log_config: LoggingConfiguration = Field(
         default=LoggingConfiguration(),
         description="The Configuration for the Logging, will be passed as DictConfig to Python logging system"
```

### Comparing `edgegap_service-1.0.3/edgegap_service/_documentation.py` & `edgegap_service-1.0.4/edgegap_service/_documentation.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.3/edgegap_service/_environment.py` & `edgegap_service-1.0.4/edgegap_service/_environment.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.3/edgegap_service/_logging.py` & `edgegap_service-1.0.4/edgegap_service/_logging.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.3/edgegap_service/_scheduling.py` & `edgegap_service-1.0.4/edgegap_service/_scheduling.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.3/edgegap_service/_service.py` & `edgegap_service-1.0.4/edgegap_service/_service.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.3/edgegap_service/_templating.py` & `edgegap_service-1.0.4/edgegap_service/_templating.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.3/edgegap_service/health/_health.py` & `edgegap_service-1.0.4/edgegap_service/health/_health.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.3/edgegap_service/health/checks/_consul.py` & `edgegap_service-1.0.4/edgegap_service/health/checks/_consul.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.3/edgegap_service/health/checks/_database.py` & `edgegap_service-1.0.4/edgegap_service/health/checks/_database.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.3/edgegap_service/health/checks/_interface.py` & `edgegap_service-1.0.4/edgegap_service/health/checks/_interface.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.3/edgegap_service/static/html/index.html` & `edgegap_service-1.0.4/edgegap_service/static/html/index.html`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.3/edgegap_service/static/images/favicon.ico` & `edgegap_service-1.0.4/edgegap_service/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.0.3/pyproject.toml` & `edgegap_service-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-service"
-version = "1.0.3"
+version = "1.0.4"
 description = "The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 include = ["static/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `edgegap_service-1.0.3/PKG-INFO` & `edgegap_service-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-service
-Version: 1.0.3
+Version: 1.0.4
 Summary: The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

