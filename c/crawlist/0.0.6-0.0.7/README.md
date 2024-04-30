# Comparing `tmp/crawlist-0.0.6.tar.gz` & `tmp/crawlist-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlist-0.0.6.tar", last modified: Fri Apr 19 06:17:32 2024, max compression
+gzip compressed data, was "crawlist-0.0.7.tar", last modified: Tue Apr 30 06:32:40 2024, max compression
```

## Comparing `crawlist-0.0.6.tar` & `crawlist-0.0.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:17:32.332104 crawlist-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-19 06:17:28.000000 crawlist-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 06:17:28.000000 crawlist-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-19 06:17:32.332104 crawlist-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-19 06:17:28.000000 crawlist-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:17:32.328104 crawlist-0.0.6/crawlist/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:17:32.332104 crawlist-0.0.6/crawlist/analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:17:32.332104 crawlist-0.0.6/crawlist/analyzers/pager/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/pager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/pager/dynamic_pager.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/pager/pager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/pager/static_pager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/valid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:17:32.332104 crawlist-0.0.6/crawlist/processings/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/processings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/processings/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/processings/script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:17:32.332104 crawlist-0.0.6/crawlist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-19 06:17:32.000000 crawlist-0.0.6/crawlist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-19 06:17:32.000000 crawlist-0.0.6/crawlist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 06:17:32.000000 crawlist-0.0.6/crawlist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-19 06:17:32.000000 crawlist-0.0.6/crawlist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 06:17:32.000000 crawlist-0.0.6/crawlist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 06:17:32.332104 crawlist-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-19 06:17:28.000000 crawlist-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:32:40.811454 crawlist-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-30 06:32:36.000000 crawlist-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 06:32:36.000000 crawlist-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-30 06:32:40.811454 crawlist-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-30 06:32:36.000000 crawlist-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:32:40.807454 crawlist-0.0.7/crawlist/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:32:40.811454 crawlist-0.0.7/crawlist/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:32:40.811454 crawlist-0.0.7/crawlist/analyzers/pager/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/pager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/pager/dynamic_pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/pager/pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/pager/static_pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/analyzers/valid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:32:40.811454 crawlist-0.0.7/crawlist/processings/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/processings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/processings/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-30 06:32:36.000000 crawlist-0.0.7/crawlist/processings/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:32:40.811454 crawlist-0.0.7/crawlist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-30 06:32:40.000000 crawlist-0.0.7/crawlist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-30 06:32:40.000000 crawlist-0.0.7/crawlist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:32:40.000000 crawlist-0.0.7/crawlist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 06:32:40.000000 crawlist-0.0.7/crawlist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 06:32:40.000000 crawlist-0.0.7/crawlist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 06:32:40.811454 crawlist-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-30 06:32:36.000000 crawlist-0.0.7/setup.py
```

### Comparing `crawlist-0.0.6/LICENSE` & `crawlist-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.6/PKG-INFO` & `crawlist-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlist
-Version: 0.0.6
+Version: 0.0.7
 Summary: A universal solution for web crawling lists
 Home-page: https://github.com/WwwwwyDev/crawlist
 Author: WwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -106,11 +106,11 @@
     # After completion, you need to close the webdriver, otherwise it will occupy your memory resources
     pager.webdriver.quit()
 
 ```
 
 ## Documenting
 If you are interested and would like to see more detailed documentation, please click on the picture below.\
- <a href="https://wwydev.gitbook.io/crawlist/"><img src="https://s2.loli.net/2024/04/12/5gOBimSY4oklGys.png" alt="crawlist" style="width:220px; height:100px" ></a>
+ <a href="https://wwydev.gitbook.io/crawlist/"><img src="https://s2.loli.net/2024/04/12/5gOBimSY4oklGys.png" alt="crawlist" style="width:287px; height:123px" ></a>
 
 ## Contributing
 Please submit pull requests to the develop branch
```

### Comparing `crawlist-0.0.6/README.md` & `crawlist-0.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -81,11 +81,11 @@
     # After completion, you need to close the webdriver, otherwise it will occupy your memory resources
     pager.webdriver.quit()
 
 ```
 
 ## Documenting
 If you are interested and would like to see more detailed documentation, please click on the picture below.\
- <a href="https://wwydev.gitbook.io/crawlist/"><img src="https://s2.loli.net/2024/04/12/5gOBimSY4oklGys.png" alt="crawlist" style="width:220px; height:100px" ></a>
+ <a href="https://wwydev.gitbook.io/crawlist/"><img src="https://s2.loli.net/2024/04/12/5gOBimSY4oklGys.png" alt="crawlist" style="width:287px; height:123px" ></a>
 
 ## Contributing
 Please submit pull requests to the develop branch
```

### Comparing `crawlist-0.0.6/crawlist/analyzers/analyzer.py` & `crawlist-0.0.7/crawlist/analyzers/analyzer.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.6/crawlist/analyzers/driver.py` & `crawlist-0.0.7/crawlist/analyzers/driver.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,84 @@
 from selenium import webdriver as wd
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.options import ArgOptions
 from selenium.webdriver.remote.webdriver import WebDriver
 from webdriver_manager.chrome import ChromeDriverManager
-from webdriver_manager.firefox import GeckoDriverManager
 from selenium.webdriver import DesiredCapabilities
 
 
 class BaseDriver(object):
     pass
 
 
-class Browser:
-    """
-    Set of supported locator strategies.
-    """
-
-    Chrome = "chrome"
-    Firefox = "firefox"
-
-
 class Driver(BaseDriver):
 
     def get_driver(self) -> WebDriver:
         raise NotImplementedError
 
     def __call__(self) -> WebDriver:
         return self.get_driver()
 
 
 class DefaultDriver(Driver):
-    def __init__(self, isDebug: bool = False):
-        self.isDebug = isDebug
+    def __init__(self, is_debug: bool = False, is_eager: bool = False):
+        self.is_debug = is_debug
+        self.is_eager = is_eager
 
     def get_driver(self) -> WebDriver:
         option = wd.ChromeOptions()
         add_default_chrome_options(option)
-        if not self.isDebug:
+        if not self.is_debug:
             option.add_argument("--headless")
+        if not self.is_eager:
+            option.page_load_strategy = 'eager'
         option.add_experimental_option('excludeSwitches', ['enable-automation'])
         webdriver = wd.Chrome(service=Service(ChromeDriverManager().install()), options=option)
+        webdriver.execute_cdp_cmd("Page.addScriptToEvaluateOnNewDocument", {
+            "source": """
+                Object.defineProperty(navigator, 'webdriver', {
+                  get: () => false
+                })
+              """
+        })
         webdriver.implicitly_wait(10)
         return webdriver
 
 
 class DefaultRemoteDriver(Driver):
-    def __init__(self, webdriver_url: str):
+    def __init__(self, webdriver_url: str, is_eager: bool = False):
         self.webdriver_url = webdriver_url
+        self.is_eager = is_eager
 
     def get_driver(self) -> WebDriver:
         option = wd.ChromeOptions()
         add_default_chrome_options(option)
+        option.add_argument("--headless")
+        if not self.is_eager:
+            option.page_load_strategy = 'eager'
         option.set_capability('cloud:options', DesiredCapabilities.CHROME)
         option.add_experimental_option('excludeSwitches', ['enable-automation'])
         webdriver = wd.Remote(command_executor=self.webdriver_url, options=option)
+        webdriver.execute_cdp_cmd("Page.addScriptToEvaluateOnNewDocument", {
+            "source": """
+                Object.defineProperty(navigator, 'webdriver', {
+                  get: () => false
+                })
+              """
+        })
         webdriver.implicitly_wait(10)
         return webdriver
 
 
 def add_default_chrome_options(option: ArgOptions):
     arguments = [
         "no-sandbox",
         "--disable-extensions",
         '--disable-gpu',
         'User-Agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77 Safari/537.36"',
         "window-size=1920x3000",
         "start-maximized",
-        'cache-control="max-age=0"'
+        'cache-control="max-age=0"',
+        "disable-blink-features=AutomationControlled"
     ]
     for argument in arguments:
         option.add_argument(argument)
-    option.page_load_strategy = 'eager'
```

### Comparing `crawlist-0.0.6/crawlist/analyzers/pager/dynamic_pager.py` & `crawlist-0.0.7/crawlist/analyzers/pager/dynamic_pager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import parsel
+from selenium.webdriver import ActionChains, Keys
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.remote.webdriver import WebDriver
 
 from crawlist.analyzers.pager.pager import Pager
 from crawlist.analyzers.driver import Driver, DefaultDriver
 from crawlist.analyzers.valid import Valid
 from crawlist.analyzers.selector import WebElementSelector
 from crawlist.annotation import check
 
 
 class DynamicPager(Pager):
     @check
-    def __init__(self, webdriver: Driver = None, interval: float = 0.1) -> None:
+    def __init__(self, webdriver: Driver | WebDriver = None, interval: float = 0.1) -> None:
         """
         :param webdriver: WebDriver object for selenium
         :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         if not webdriver:
             self.webdriver = DefaultDriver()()
         else:
-            self.webdriver = webdriver()
+            if isinstance(webdriver, WebDriver):
+                self.webdriver = webdriver
+            else:
+                self.webdriver = webdriver()
         super().__init__(interval=interval)
 
     def click_safety(self, button: WebElement) -> None:
         """
         Attempt to click the button multiple times
         :param button: Button elements
         """
@@ -44,15 +48,15 @@
             self.webdriver.quit()
         except:
             pass
 
 
 class DynamicRedirectPager(DynamicPager):
     @check
-    def __init__(self, uri: str, uri_split: str, webdriver: Driver = None, start: int = 1, offset: int = 1,
+    def __init__(self, uri: str, uri_split: str, webdriver: Driver | WebDriver = None, start: int = 1, offset: int = 1,
                  interval: float = 0.1) -> None:
         """
         Based on dynamic web page analyzer (redirect page flipping)
         :param uri: First page link
         :param uri_split: Link pagination (using% v proxy) Example: https://www.boc.cn/sourcedb/whpj/index_%v.html
         :param webdriver: WebDriver object for selenium
         :param start: Start page
@@ -79,15 +83,15 @@
     def html(self) -> str:
         self.webdriver.get(self.current_uri)
         return self.webdriver.page_source
 
 
 class DynamicListRedirectPager(DynamicPager):
     @check
-    def __init__(self, uris: list, webdriver: Driver = None, interval: float = 0.1) -> None:
+    def __init__(self, uris: list, webdriver: Driver | WebDriver = None, interval: float = 0.1) -> None:
         """
         Based on dynamic web page analyzer (redirect page flipping)
         :param uris: A list containing multiple uris, executed in order downwards
         :param webdriver: WebDriver object for selenium
         :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         for uri in uris:
@@ -112,15 +116,15 @@
         uri = self.uris[self.index]
         self.webdriver.get(uri)
         return self.webdriver.page_source
 
 
 class DynamicScrollPager(DynamicPager):
     @check
-    def __init__(self, uri: str, webdriver: Driver = None, interval: float = 1) -> None:
+    def __init__(self, uri: str, webdriver: Driver | WebDriver = None, interval: float = 1) -> None:
         """
         Based on dynamic web page analyzer (scrolling and flipping)
         :param uri: webpage link, which is a scrolling page
         :param webdriver: WebDriver object for selenium
         :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         assert Valid.is_valid_url(uri)
@@ -136,26 +140,33 @@
                         }
                     },100)
                 '''
 
     def next(self) -> None:
         self.webdriver.execute_script(DynamicScrollPager.js_code)
         self.sleep()
+        actions = ActionChains(self.webdriver)
+        actions.move_by_offset(0, 0).click().perform()
+        self.sleep()
+        for _ in range(5):
+            actions.send_keys(Keys.SPACE).perform()
+            self.sleep()
+        self.sleep()
 
     @property
     def html(self) -> str:
         return self.webdriver.page_source
 
     def pre_load(self, webdriver: WebDriver) -> None:
         webdriver.get(self.uri)
 
 
 class DynamicLineButtonPager(DynamicPager):
     @check
-    def __init__(self, uri: str, button_selector: WebElementSelector, webdriver: Driver = None,
+    def __init__(self, uri: str, button_selector: WebElementSelector, webdriver: Driver | WebDriver = None,
                  interval: float = 1) -> None:
         """
         Based on dynamic web page analyzer (row button page flipping)
         :param uri: webpage link, which is a row button for flipping pages
         :param button.selector: row button selector
         :param webdriver: WebDriver object for selenium
         :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
@@ -179,15 +190,15 @@
 
     def pre_load(self, webdriver: WebDriver) -> None:
         webdriver.get(self.uri)
 
 
 class DynamicNumButtonPager(DynamicPager):
     @check
-    def __init__(self, uri: str, button_selector: WebElementSelector, webdriver: Driver = None, start: int = 1,
+    def __init__(self, uri: str, button_selector: WebElementSelector, webdriver: Driver | WebDriver = None, start: int = 1,
                  offset: int = 1, interval: float = 1) -> None:
         """
         Based on dynamic web page analyzer (digital button flipping)
         :param uri: webpage link, which is a numeric button for flipping pages
         :param button.selector: numeric button selector
         :param webdriver: WebDriver object for selenium
         :param start: Start page
@@ -258,15 +269,15 @@
 
     def pre_load(self, webdriver: WebDriver) -> None:
         webdriver.get(self.uri)
 
 
 class DynamicNextButtonPager(DynamicPager):
     @check
-    def __init__(self, uri: str, button_selector: WebElementSelector, webdriver: Driver = None, start: int = 1,
+    def __init__(self, uri: str, button_selector: WebElementSelector, webdriver: Driver | WebDriver = None, start: int = 1,
                  offset: int = 1, interval: float = 1) -> None:
         """
         Based on dynamic web page analyzer (click the next page button to page)
         :param uri: Web page link, which is a page that can be flipped by clicking the next page button
         :param button.selector: Click on the next page button selector
         :param webdriver: WebDriver object for selenium
         :param start: Start page
```

### Comparing `crawlist-0.0.6/crawlist/analyzers/pager/pager.py` & `crawlist-0.0.7/crawlist/analyzers/pager/pager.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.6/crawlist/analyzers/pager/static_pager.py` & `crawlist-0.0.7/crawlist/analyzers/pager/static_pager.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.6/crawlist/analyzers/request.py` & `crawlist-0.0.7/crawlist/analyzers/request.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.6/crawlist/analyzers/selector.py` & `crawlist-0.0.7/crawlist/analyzers/selector.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.6/crawlist/analyzers/trie.py` & `crawlist-0.0.7/crawlist/analyzers/trie.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.6/crawlist/analyzers/valid.py` & `crawlist-0.0.7/crawlist/analyzers/valid.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.6/crawlist/annotation.py` & `crawlist-0.0.7/crawlist/annotation.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.6/crawlist/processings/action.py` & `crawlist-0.0.7/crawlist/processings/action.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.6/crawlist/processings/script.py` & `crawlist-0.0.7/crawlist/processings/script.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.6/crawlist.egg-info/PKG-INFO` & `crawlist-0.0.7/crawlist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlist
-Version: 0.0.6
+Version: 0.0.7
 Summary: A universal solution for web crawling lists
 Home-page: https://github.com/WwwwwyDev/crawlist
 Author: WwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -106,11 +106,11 @@
     # After completion, you need to close the webdriver, otherwise it will occupy your memory resources
     pager.webdriver.quit()
 
 ```
 
 ## Documenting
 If you are interested and would like to see more detailed documentation, please click on the picture below.\
- <a href="https://wwydev.gitbook.io/crawlist/"><img src="https://s2.loli.net/2024/04/12/5gOBimSY4oklGys.png" alt="crawlist" style="width:220px; height:100px" ></a>
+ <a href="https://wwydev.gitbook.io/crawlist/"><img src="https://s2.loli.net/2024/04/12/5gOBimSY4oklGys.png" alt="crawlist" style="width:287px; height:123px" ></a>
 
 ## Contributing
 Please submit pull requests to the develop branch
```

### Comparing `crawlist-0.0.6/crawlist.egg-info/SOURCES.txt` & `crawlist-0.0.7/crawlist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.6/setup.py` & `crawlist-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'crawlist'
 DESCRIPTION = 'A universal solution for web crawling lists'
 URL = 'https://github.com/WwwwwyDev/crawlist'
 EMAIL = 'wwy20001014@foxmail.com'
 AUTHOR = 'WwyDev'
 REQUIRES_PYTHON = '>=3.10.0'
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 # What packages are required for this module to be executed?
 REQUIRED = [
     'parsel', 'selenium>=4.0.0', 'cssselect', 'lxml', 'requests', 'webdriver-manager'
 ]
 
 # What packages are optional?
 EXTRAS = {
```

