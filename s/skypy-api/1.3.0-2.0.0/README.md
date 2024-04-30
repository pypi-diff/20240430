# Comparing `tmp/skypy-api-1.3.0.tar.gz` & `tmp/skypy-api-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypy-api-1.3.0.tar", last modified: Sat Jun 25 13:51:39 2022, max compression
+gzip compressed data, was "skypy-api-2.0.0.tar", last modified: Tue Apr 30 20:12:43 2024, max compression
```

## Comparing `skypy-api-1.3.0.tar` & `skypy-api-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 13:51:39.743511 skypy-api-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-06-25 13:51:26.000000 skypy-api-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-06-25 13:51:39.743511 skypy-api-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-06-25 13:51:26.000000 skypy-api-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-25 13:51:39.743511 skypy-api-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-06-25 13:51:26.000000 skypy-api-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 13:51:39.743511 skypy-api-1.3.0/skypy/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-06-25 13:51:26.000000 skypy-api-1.3.0/skypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6494 2022-06-25 13:51:26.000000 skypy-api-1.3.0/skypy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 13:51:39.743511 skypy-api-1.3.0/skypy_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-06-25 13:51:39.000000 skypy-api-1.3.0/skypy_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-06-25 13:51:39.000000 skypy-api-1.3.0/skypy_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-25 13:51:39.000000 skypy-api-1.3.0/skypy_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-25 13:51:39.000000 skypy-api-1.3.0/skypy_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-25 13:51:39.000000 skypy-api-1.3.0/skypy_api.egg-info/top_level.txt
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-30 20:12:43.195075 skypy-api-2.0.0/
+-rw-r--r--   0 david     (1000) david     (1000)     2251 2024-04-30 19:28:37.000000 skypy-api-2.0.0/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)      841 2024-04-30 20:12:43.195075 skypy-api-2.0.0/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      456 2024-04-30 19:28:37.000000 skypy-api-2.0.0/README.md
+-rw-r--r--   0 david     (1000) david     (1000)       38 2024-04-30 20:12:43.195075 skypy-api-2.0.0/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)      658 2024-04-30 19:28:37.000000 skypy-api-2.0.0/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-30 20:12:43.195075 skypy-api-2.0.0/skypy/
+-rw-r--r--   0 david     (1000) david     (1000)       30 2024-04-30 19:28:37.000000 skypy-api-2.0.0/skypy/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     9506 2024-04-30 19:28:37.000000 skypy-api-2.0.0/skypy/main.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-30 20:12:43.195075 skypy-api-2.0.0/skypy_api.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      841 2024-04-30 20:12:43.000000 skypy-api-2.0.0/skypy_api.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      222 2024-04-30 20:12:43.000000 skypy-api-2.0.0/skypy_api.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2024-04-30 20:12:43.000000 skypy-api-2.0.0/skypy_api.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)       14 2024-04-30 20:12:43.000000 skypy-api-2.0.0/skypy_api.egg-info/requires.txt
+-rw-r--r--   0 david     (1000) david     (1000)        6 2024-04-30 20:12:43.000000 skypy-api-2.0.0/skypy_api.egg-info/top_level.txt
```

### Comparing `skypy-api-1.3.0/PKG-INFO` & `skypy-api-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: skypy-api
-Version: 1.3.0
+Version: 2.0.0
 Summary: Framework to connect to the Hypixel Skyblock API
 Home-page: https://github.com/FuchsCrafter/skypy
 Author: FuchsCrafter
 License: GPL2
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # skypy
@@ -18,7 +19,9 @@
 
 You can find the documentation in the [GitHub wiki](https://github.com/FuchsCrafter/skypy/wiki).
 
 Find the work-in-progress example page [Here](https://fuchscrafter.github.io/skypy/examples/).
 
 ***
 *skypy-api is maintained by [FuchsCrafter](https://github.com/FuchsCrafter)*
+
+
```

### Comparing `skypy-api-1.3.0/setup.py` & `skypy-api-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="skypy-api",
     url="https://github.com/FuchsCrafter/skypy",
-    version="1.3.0",
+    version="2.0.0",
     author="FuchsCrafter",
     license="GPL2",
     description="Framework to connect to the Hypixel Skyblock API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `skypy-api-1.3.0/skypy/main.py` & `skypy-api-2.0.0/skypy/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,168 +1,209 @@
 # skypy(skypy-api) by FuchsCrafter - https://github.com/FuchsCrafter/skypy
 # Also check out skypy-webui - https://github.com/FuchsCrafter/skypy-webui
 
 import requests
 import json
 
 class skypy:
-  """ The main class for the module. Uses an api key that you can find by running /apinew on mc.hypixel.net """
-  def __init__(self, key="NO_KEY"):
-    global apikey
-    if key == "NO_KEY":
-      returns = False
-    else:
-      apikey = str(key)
-      r = requests.get("https://api.hypixel.net/key?key="+ key)
-      returns = json.loads(r.text)
-      returns = returns["success"]
-
-    if not returns and key != "NO_KEY":
-      print("Invalid API Key! Please note that you cant use some modules now!")
-
-  def getNews(self):
-    """**Requires Authentication**\nGets the latest SkyBlock news. """
-    r = requests.get("https://api.hypixel.net/skyblock/news?key=" + apikey)
-    returns = json.loads(r.text)
-    if not returns["success"]:
-      print("Failed! Make sure that you api key is correct!")
-    else:
-      return returns["items"]
-
-  def getItem(self, itemname):
-    """ Gets a specific item and its childs (e.g. NPC sell price, category, name, etc.)"""
-    r = requests.get("https://api.hypixel.net/resources/skyblock/items")
-    r = json.loads(r.text)["items"]
-    try:
-      for element in r:
-        if element["id"] == itemname:
-          return element
-    except:
-      return
-
-  def getAllItems(self):
-    """ Gets all Items and returns them in a disctionary."""
-    r = requests.get("https://api.hypixel.net/resources/skyblock/items")
-    r = json.loads(r.text)["items"]
-    returns = {}
-    for element in r:
-      returns[element["id"]] = element
-    return returns
-
-  def getCurrentBingo(self):
-    return json.loads(requests.get("https://api.hypixel.net/resources/skyblock/bingo").text)["goals"]
-
-
-
-
-
-  class bazaar:
-    """ The bazaar class was made to get bazaar values from certain items. """
-    def __init__(self):
-      pass
-
-    def fetchAllProducts(self):
-      """ Fetches all products and returns them as a JSON string. """
-      return json.loads(requests.get("https://api.hypixel.net/skyblock/bazaar").text)["products"]
-
-
-    def fetchProduct(self, itemname, quickmode=False):
-      """ Fetches a specific product and returns his data as a JSON string. Use Quick Mode for shorter but cleaner returns. Returns False if the product is not found. """
-      r = requests.get("https://api.hypixel.net/skyblock/bazaar")
-      bazaarProducts = json.loads(r.text)
-      bazaarProducts = bazaarProducts["products"]
-      try:
-        if not quickmode:
-          return bazaarProducts[itemname]
+    """ The main class for the module. Uses an api key"""
+    def __init__(self, key:str, blockKeyTest:bool=False) -> None:
+        global apikey
+        assert key != ""
+        apikey = str(key)
+        if not blockKeyTest:
+            r = requests.get("https://api.hypixel.net/v2/skyblock/news?key="+ key)
+            returns = json.loads(r.text)
+            returns = returns["success"]
+            if not returns:
+                print("Invalid API Key! Please note that you cant use some modules now!")
+
+
+    def getNews(self) -> list:
+        """(Requires Authentication) Gets the latest SkyBlock news. """
+        r = requests.get("https://api.hypixel.net/v2/skyblock/news?key=" + apikey)
+        returns = json.loads(r.text)
+        if not returns["success"]:
+            print("Failed! Make sure that you api key is correct!")
         else:
-          _ = bazaarProducts[itemname]
-          return _["quick_status"]
-      except:
-        return False
-  class auction:
-    """ The auction class is there to get auction informations. It requires the Hypixel api key (log into mc.hypixel.net and type /api in chat)."""
-    def __init__(self):
-      pass
-
-    def getAuctionByPlayer(self, uuid):
-      """ Gets the auction by a player uuid. """
-      r = requests.get("https://api.hypixel.net/skyblock/auction?key=" + apikey + "&player=" + uuid)
-      returns = json.loads(r.text)
-      if not returns["success"]:
-        print("Failed! Make sure, that you api key and the uuid is correct!")
-      else:
-        return json.loads(returns["auctions"])
-
-    def getAuctionByPlayerName(self, player):
-      """ Uses the Mojang API to get the uuid of a player. """
-      r = requests.get("https://api.mojang.com/users/profiles/minecraft/" + player)
-      returns = json.loads(r.text)
-      try:
-        playeruuid = returns["id"]
-        return self.getAuctionByPlayer(playeruuid)
-      except:
-        print("Invalid Playername!")
-
-    def getAuction(self, auctionid):
-      """ Gets an auction by its ID. """
-      r = requests.get("https://api.hypixel.net/skyblock/auction?key=" + apikey + "&uuid=" + auctionid)
-      returns = json.loads(r.text)
-      if not returns["success"]:
-        print("Failed! Make sure, that you api key and the auction-id is correct!")
-      else:
-        return json.loads(returns["auctions"])
-   
-    def getAuctions(self):
-      """ Gets all active auctions. You dont need an API key for this. """
-      r = requests.get("https://api.hypixel.net/skyblock/auctions")
-      returns = json.loads(r.text)
-      return json.loads(returns["auctions"])
-
-    def getEndedAuctions(self):
-      """ Gets the latest ended auctions. It works also without any authorization."""
-      r = requests.get("https://api.hypixel.net/skyblock/auctions_ended")
-      returns = json.loads(r.text)
-      return json.loads(returns["auctions"])
-  class politics:
-    """ The politics class is there to get the current election results or the current mayor. """
-    def __init__(self):
-      pass
-    def getCurrentMayor(self, quickmode=False):
-      """ Gets the current mayor an his perks. """
-      r = requests.get("https://api.hypixel.net/resources/skyblock/election")
-      returns = json.loads(r.text)
-
-      if quickmode:
-        returns = returns["mayor"]
-        name = returns["name"]
-        mkey = returns["key"]
-        _ = {"name": name,"key": mkey}
-        return _
-      else:
-        return returns["mayor"]
-
-    def getCurrentElection(self, quickmode=False, full=True):
-      """ Gets the current election results. Using Quickmode only gets the canidates list with all the child data."""
-      r = requests.get("https://api.hypixel.net/resources/skyblock/election")
-      returns = json.loads(r.text)
-      if not quickmode:
-        return returns["current"]
-      else:
-        _ = returns["current"]["candidates"]
+            return returns["items"]
+
+    def getItem(self, itemname:str) -> dict:
+        """ Gets a specific item and its childs (e.g. NPC sell price, category, name, etc.)"""
+        r = requests.get("https://api.hypixel.net/v2/resources/skyblock/items")
+        r = json.loads(r.text)["items"]
+        try:
+            for element in r:
+                if element["id"] == itemname:
+                    return element
+        except:
+            return
+
+    def getAllItems(self) -> dict:
+        """ Gets all Items and returns them in a disctionary."""
+        r = requests.get("https://api.hypixel.net/v2/resources/skyblock/items")
+        r = json.loads(r.text)["items"]
         returns = {}
-        for element in _:
-          if full:
-            returns[element["name"]] = {"name": element["name"],"key": element["key"], "votes": element["votes"], "perks": element["perks"]}
-          else:
-            returns[element["name"]] = {"name": element["name"],"key": element["key"], "votes": element["votes"]}
+        for element in r:
+            returns[element["id"]] = element
         return returns
 
-    def getElectionResults(self):
-      """ Gets only the election votes. """
-      r = requests.get("https://api.hypixel.net/resources/skyblock/election")
-      returns = json.loads(r.text)
-      _ = returns["current"]["candidates"]
-      returns = {}
-      for element in _:
-        returns[element["name"]] = element["votes"]
-      return returns
-
+    def getCurrentBingo(self):
+        return json.loads(requests.get("https://api.hypixel.net/v2/resources/skyblock/bingo").text)
+    
+
+    class bazaar:
+        """ The bazaar class was made to get bazaar values from certain items. """
+        def __init__(self):
+            pass
+
+        def fetchAllProducts(self) -> dict:
+            """ Fetches all products and returns them as a JSON string. """
+            return json.loads(requests.get("https://api.hypixel.net/v2/skyblock/bazaar").text)["products"]
+
+
+        def fetchProduct(self, itemname, quickmode=False) -> dict:
+            """ Fetches a specific product and returns his data as a JSON string. Use Quick Mode for shorter but cleaner returns. Returns False if the product is not found. """
+            r = requests.get("https://api.hypixel.net/v2/skyblock/bazaar")
+            bazaarProducts = json.loads(r.text)
+            bazaarProducts = bazaarProducts["products"]
+            try:
+                if not quickmode:
+                    return bazaarProducts[itemname]
+                else:
+                    _ = bazaarProducts[itemname]
+                    return _["quick_status"]
+            except:
+                return False
+            
+    class auction:
+        """ The auction class is there to get auction informations. It requires the Hypixel api key (log into mc.hypixel.net and type /api in chat)."""
+        def __init__(self):
+            pass
+
+        def getAuctionByPlayer(self, uuid:str) -> list:
+            """ Gets the auction by a player uuid. """
+            r = requests.get("https://api.hypixel.net/v2/skyblock/auction?key=" + apikey + "&player=" + uuid)
+            returns = json.loads(r.text)
+            if not returns["success"]:
+                print("Failed! Make sure, that you api key and the uuid is correct!")
+            else:
+                return returns["auctions"]
+
+        def getAuctionByPlayerName(self, player:str) -> list: 
+            """ Uses the Mojang API to get the uuid of a player. """
+            r = requests.get("https://api.mojang.com/users/profiles/minecraft/" + player) # TODO: Create dedicated function for this
+            returns = json.loads(r.text)
+            try:
+                playeruuid = returns["id"]
+            except:
+                print("Invalid Playername!")
+            else: 
+                return self.getAuctionByPlayer(playeruuid)
+        
+        def getAuctionsByPlayer(self, uuid:str) -> list:
+            """Alias function for getAuctionByPlayer"""
+            return self.getAuctionByPlayer(uuid=uuid)
+            
+        def getAuctionsByPlayerName(self, player:str) -> list:
+            """Alias function for getAuctionByPlayerName"""
+            return self.getAuctionByPlayerName(player=player)
+
+        def getAuction(self, auctionid:str) -> dict:
+            """ Gets an auction by its ID. """
+            r = requests.get("https://api.hypixel.net/v2/skyblock/auction?key=" + apikey + "&uuid=" + auctionid)
+            returns = json.loads(r.text)
+            if not returns["success"]:
+                print("Failed to get auction! Make sure that you api-key and the auction's ID are both correct!")
+                # raise ValueError(f"Incorrect auction ID: {auctionid}") # TODO: Check for error (if it is the invalid API key or the invalid auction id)
+            else:
+                return returns["auctions"][0]
+
+        def getAuctions(self, page:int=0) -> list:
+            """ Gets all active auctions.. """
+            r = requests.get("https://api.hypixel.net/v2/skyblock/auctions?page=" + str(page))
+            returns = json.loads(r.text)
+            return returns["auctions"]
+        
+        def getAuctionsMetadata() -> dict[str: int]: 
+            """ Gets general info about all auctions """
+            r = requests.get("https://api.hypixel.net/v2/skyblock/auctions")
+            returns = json.loads(r.text)
+            out = { "totalPages": returns["totalPages"], "totalAuctions": returns["totalAuctions"], "lastUpdated": returns["lastUpdated"]}
+            return out
+
+        def getEndedAuctions(self) -> list:
+            """ Gets the latest ended auctions. It works also without any authorization."""
+            r = requests.get("https://api.hypixel.net/v2/skyblock/auctions_ended")
+            returns = json.loads(r.text)
+            return returns["auctions"]
+        
+        
+    class mayor:
+        """ The mayor class is there to get the current election results or the current mayor."""
+        def __init__(self):
+            r = requests.get("https://api.hypixel.net/v2/resources/skyblock/election")
+            returns = json.loads(r.text)
+            self.currentElectionCache = returns
+            pass
+
+        def updateElectionCache(self) -> None:
+            r = requests.get("https://api.hypixel.net/v2/resources/skyblock/election")
+            returns = json.loads(r.text)
+            self.currentElectionCache = returns
+
+        def getCurrentMayor(self, quickmode:bool=False):
+            """ Gets the current mayor an his perks. """
+            currentMayor = self.currentElectionCache["mayor"]
+            if quickmode:
+                return {"name": currentMayor["name"],"key": currentMayor["key"]}
+            else:
+                return currentMayor
+
+        def getCurrentElection(self, quickmode:bool=False, full:bool=True, updateCache:bool=False) -> dict: #TODO: Remaining rewrite, testing
+            """ Gets the current election results.
+            
+            Use the updateCache parameter to update the election cache, or call 
+            the updateElectionCache method of the mayor class to do so."""
+            if updateCache:
+                self.updateElectionCache()
+            else:
+                returns = self.currentElectionCache
+            if "current" in returns:
+                if not quickmode:
+                    return returns["current"]
+                else:
+                    _ = returns["current"]["candidates"]
+                    returns = {}
+                    for element in _:
+                        if full:
+                            returns[element["name"]] = {"name": element["name"],"key": element["key"], "votes": element["votes"], "perks": element["perks"]}
+                        else:
+                            returns[element["name"]] = {"name": element["name"],"key": element["key"], "votes": element["votes"]}
+                    return returns
+            else:
+                return False
+
+        def getElectionResults(self, updateCache):  #TODO: Remaining rewrite, testing
+            """ Gets only the election votes.
+
+            Use the updateCache parameter to update the election cache, or call 
+            the updateElectionCache method of the mayor class to do so."""
+            if updateCache:
+                self.updateElectionCache()
+            else:
+                returns = self.currentElectionCache
+            if "current" in returns:
+                _ = returns["current"]["candidates"]
+                returns = {}
+                for element in _:
+                    returns[element["name"]] = element["votes"]
+                return returns
+            else:
+                return False
+    class politics(mayor):
+        """# Attention: Class was renamed!
+            This class was renamed to 'mayor', but remains as a synonym of 'mayor'. 
+            
+            Please do not use it when writing new code!
+        """
+        pass
```

### Comparing `skypy-api-1.3.0/skypy_api.egg-info/PKG-INFO` & `skypy-api-2.0.0/skypy_api.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: skypy-api
-Version: 1.3.0
+Version: 2.0.0
 Summary: Framework to connect to the Hypixel Skyblock API
 Home-page: https://github.com/FuchsCrafter/skypy
 Author: FuchsCrafter
 License: GPL2
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # skypy
@@ -18,7 +19,9 @@
 
 You can find the documentation in the [GitHub wiki](https://github.com/FuchsCrafter/skypy/wiki).
 
 Find the work-in-progress example page [Here](https://fuchscrafter.github.io/skypy/examples/).
 
 ***
 *skypy-api is maintained by [FuchsCrafter](https://github.com/FuchsCrafter)*
+
+
```

