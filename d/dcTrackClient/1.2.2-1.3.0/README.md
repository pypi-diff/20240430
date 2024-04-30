# Comparing `tmp/dctrackclient-1.2.2.tar.gz` & `tmp/dctrackclient-1.3.0.tar.gz`

## Comparing `dctrackclient-1.2.2.tar` & `dctrackclient-1.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    44315 2020-02-02 00:00:00.000000 dctrackclient-1.2.2/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 dctrackclient-1.2.2/.gitignore
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 dctrackclient-1.2.2/pyproject.toml
--rw-r--r--   0        0        0    45979 2020-02-02 00:00:00.000000 dctrackclient-1.2.2/../README.md
--rw-r--r--   0        0        0    46669 2020-02-02 00:00:00.000000 dctrackclient-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    46773 2020-02-02 00:00:00.000000 dctrackclient-1.3.0/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 dctrackclient-1.3.0/.gitignore
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 dctrackclient-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    48348 2020-02-02 00:00:00.000000 dctrackclient-1.3.0/../README.md
+-rw-r--r--   0        0        0    49038 2020-02-02 00:00:00.000000 dctrackclient-1.3.0/PKG-INFO
```

### Comparing `dctrackclient-1.2.2/src/dcTrackClient/__init__.py` & `dctrackclient-1.3.0/src/dcTrackClient/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 
 
 class Client:
-    """Sunbird dcTrack API client version 1.2.2 in Python"""
+    """Sunbird dcTrack API client version 1.3.0 in Python"""
 
     def __init__(self, baseUrl: str, username: str = '', password: str = '', apiToken: str = '', httpProxy: str = '', httpsProxy: str = ''):
         """Provide either a username and password, or an API token to access the dcTrack database with Python."""
         self.__BASE_URL = baseUrl
         self.__USERNAME = username
         self.__PASSWORD = password
         self.__APITOKEN = apiToken
@@ -117,17 +117,17 @@
         """Update an existing Connector. Returns JSON entity containing Connector information that was passed in from the Request payload."""
         return self.__request('PUT', '/api/v2/settings/connectors/' + str(connectorId) + '?', payload)
 
     def removeConnector(self, payload: dict):
         """Delete one or more Connector records."""
         return self.__request('POST', '/api/v2/settings/connectors/delete?', payload)
 
-    def searchConnectors(self, pageNumber: int, pageSize: int, usedCount: bool, payload: dict):
-        """Retrieve a List of Connectors. Returns JSON entity containing Connector information that was passed in from the Request payload. Please note, Compatible Connectors are not returned by this API, but can be returned when querying a single Connector using the /api/v2/settings/connectors/{connectorId} API."""
-        return self.__request('POST', '/api/v2/settings/connectors/quicksearch?pageNumber=' + str(pageNumber) + '&pageSize=' + str(pageSize) + '&usedCount=' + str(usedCount) + '&', payload)
+    def searchConnectors(self, pageNumber: int, pageSize: int, payload: dict):
+        """Search for Connectors using criteria JSON object. Search criteria can be any of the fields applicable to Connector, including custom fields. Specify the fields to be included in the response. This API supports pagination. Returns a list of Connectors with the specified information."""
+        return self.__request('POST', '/api/v2/quicksearch/connectors?pageNumber=' + str(pageNumber) + '&pageSize=' + str(pageSize) + '&', payload)
 
     def deleteConnectorImage(self, connectorId: int):
         """Delete a Connector Image using the Connector ID."""
         return self.__request('DELETE', '/api/v2/settings/connectors/' + str(connectorId) + '/images?')
 
     def getDataPorts(self, itemId: int):
         """Use the REST API to retrieve details from all data ports on an item. If the operation was successful, a status code 200 is displayed, and the body contains the item's data port details. If the operation failed, an error code is returned."""
@@ -161,14 +161,38 @@
         """Use the REST API to create power ports for an existing item. If ports are already defined for the item because it is included in the Item Models Library, you can use the REST API to create additional ports for the item."""
         return self.__request('PUT', '/api/v1/items/' + str(itemId) + '/powerports/' + str(portId) + '?proceedOnWarning=' + str(proceedOnWarning) + '&', payload)
 
     def getCompatibleConnector(self, itemId: int, portId: int, connectorId: int):
         """Use the REST API to determine if a Connector is compatible with a specific Power Port."""
         return self.__request('GET', '/api/v1/items/' + str(itemId) + '/powerports/' + str(portId) + '/connectors/' + str(connectorId) + '/isCompatible?')
 
+    def getBreakers(self, panelItemID: int):
+        """Get a list of all Breakers for a given Panel Item. Returns JSON entity containing an array of all the Breakers for the specified Panel Item."""
+        return self.__request('GET', '/api/v2/dcimoperations/items/' + str(panelItemID) + '/breakers?')
+
+    def getBreaker(self, panelItemID: int, breakerPortId: int):
+        """Get a list of all Breakers for a given Panel Item. Returns JSON entity containing information for a single Panel Item Breaker."""
+        return self.__request('GET', '/api/v2/dcimoperations/items/' + str(panelItemID) + '/breakers/' + str(breakerPortId) + '?')
+
+    def updateBreaker(self, panelItemD: str, beakerPortID: int, payload: dict):
+        """Update a single Breaker for a given Panel Item. Returns JSON entity containing information for the updated Panel Item Breaker. Note: This API performs as a true PUT and not a PATCH. Unlike with a PATCH, you must specify all attributes even if you want to change only one. Attributes that are not included in the Request will be considered as removed."""
+        return self.__request('PUT', '/api/v2/dcimoperations/items/' + str(panelItemD) + '/breakers/' + str(beakerPortID) + '?', payload)
+
+    def createBreaker(self, panelItemId: int, payload: dict):
+        """Create a single Breaker for a given Panel Item. Returns JSON entity containing information for the created Panel Item Breaker. Note: Breaker State is set based on the connection status of the Breaker. If the breaker is connected it will always be set to "Closed", even if "Open" is specified in the Request."""
+        return self.__request('POST', '/api/v2/dcimoperations/items/' + str(panelItemId) + '/breakers?', payload)
+
+    def deleteBreaker(self, panelItemID: int, breakerPortId: int):
+        """Delete a Breaker for a given Panel Item. Returns empty JSON."""
+        return self.__request('DELETE', '/api/v2/dcimoperations/items/' + str(panelItemID) + '/breakers/' + str(breakerPortId) + '?')
+
+    def createBreakersBulk(self, panelItemID: int, payload: dict):
+        """Add/Update/Delete Breakers for a given Panel Item."""
+        return self.__request('POST', '/api/v2/dcimoperations/items/' + str(panelItemID) + '/breakers/bulk?', payload)
+
     def getLocations(self):
         """Returns a list for all Locations."""
         return self.__request('GET', '/api/v1/locations?')
 
     def getLocation(self, locationId: int):
         """Get a single Location. Returns json containing location data for the specified ID."""
         return self.__request('GET', '/api/v1/locations' + str(locationId) + '?')
@@ -189,18 +213,14 @@
         """Search for Locations by user supplied search criteria. Returns a list of Locations with the "selectedColumns" returned in the payload."""
         return self.__request('POST', '/api/v2/quicksearch/locations?pageNumber=' + str(pageNumber) + '&pageSize=' + str(pageSize) + '&', payload)
 
     def getLocationFieldList(self):
         """Returns a list of all Location fields."""
         return self.__request('GET', '/api/v2/quicksearch/locations/locationListFields?')
 
-    def getSublocationTree(self):
-        """Get the sublocation tree."""
-        return self.__request('GET', '/api/v2/subLocations/tree?')
-
     def getSublocations(self, locationId: int):
         """Get all sub-locations for a given location in the hierarchy. The locationId is the ID of the location to get the sub-locations for."""
         return self.__request('GET', '/api/v2/subLocations/list/' + str(locationId) + '?')
 
     def getSublocationsOfType(self, locationId: int, typeCode: str):
         """Get all sub-locations of given type for a given location in the hierarchy. The locationId is the id of the location you are querying the sub-location types for. The type is one of either 5016 and 5017 for rows and aisles respectively."""
         return self.__request('GET', '/api/v2/subLocations/' + str(locationId) + '/type/' + str(typeCode) + '?')
@@ -289,14 +309,22 @@
         """Get a list of records (options) for use in drop-down lists for dcTrack standard fields by list type. Returns a list of records for a given list type."""
         return self.__request('GET', '/api/v2/dcimoperations/picklists/' + str(listType) + '?')
 
     def updatePicklistOptions(self, listType: str, payload: dict):
         """Update a list of records (options) for use in drop-down lists for dcTrack standard fields by list type. Returns a list of records for a given list type."""
         return self.__request('PUT', '/api/v2/dcimoperations/picklists/' + str(listType) + '?', payload)
 
+    def updateDefaultValue(self, payload: dict):
+        """Update the default value for a picklist field."""
+        return self.__request('PUT', '/api/v2/settings/lists/defaultValue?', payload)
+
+    def getFieldProperties(self, entity: str):
+        """Get the properties for all fields applicable to the Entity."""
+        return self.__request('GET', '/api/v2/settings/lists/fieldProperties?entity=' + str(entity) + '&')
+
     def submitRequest(self, id: int, payload: dict):
         """Create a request."""
         return self.__request('PUT', '/api/v2/dcimoperations/items/' + str(id) + '?', payload)
 
     def deleteRequest(self, requestId: int):
         """Cancel a request. Returns Returns request ID canceled."""
         return self.__request('DELETE', '/api/v2/dcimoperations/requests/' + str(requestId) + '?')
```

### Comparing `dctrackclient-1.2.2/pyproject.toml` & `dctrackclient-1.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "1.2.2"
+version = "1.3.0"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "../README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dctrackclient-1.2.2/../README.md` & `dctrackclient-1.3.0/../README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API clients in Python and JavaScript
 
 ## Installation
 > dcTrackClient can be installed from the package manager of your choice.
 
 ### Python
 ```shell
-pip install dcTrackClient==1.2.2
+pip install dcTrackClient==1.3.0
 ```
 
 ### JavaScript
 ```shell
-npm i dctrackclient@1.2.2
+npm i dctrackclient@1.3.0
 ```
 
 ## Initialize a connection to the dcTrack API
 > Authentication is by using a base URL (the same URL to access the GUI) and a username and password, or a base URL and an API token.
 
 ### Python
 ```py
@@ -201,15 +201,15 @@
 { "itemId": 1234 }
 ```
 
 # Official DcTrack Documentation
 
 Visit this link for the official documentation on request bodies and attrribute names.
 
-https://www.sunbirddcim.com/help/dcTrack/v910/API/en/Default.htm
+https://www.sunbirddcim.com/help/dcTrack/v911/API/en/Default.htm
 
 # Package Documentation
 
 The section below shows all the functions contained within this client along with basic usage.
 
 ## getItem(id)
 > Get item details using the item ID. Returns an Item JSON object.
@@ -430,24 +430,23 @@
 ```
 POST api/v2/settings/connectors/delete payload
 ```
 |Parameter|Type|
 |---|---|
 |payload|object|
 
-## searchConnectors(pageNumber, pageSize, usedCount, payload)
-> Retrieve a List of Connectors. Returns JSON entity containing Connector information that was passed in from the Request payload. Please note, Compatible Connectors are not returned by this API, but can be returned when querying a single Connector using the /api/v2/settings/connectors/{connectorId} API.
+## searchConnectors(pageNumber, pageSize, payload)
+> Search for Connectors using criteria JSON object. Search criteria can be any of the fields applicable to Connector, including custom fields. Specify the fields to be included in the response. This API supports pagination. Returns a list of Connectors with the specified information.
 ```
-POST api/v2/settings/connectors/quicksearch payload
+POST api/v2/quicksearch/connectors payload
 ```
 |Parameter|Type|
 |---|---|
 |pageNumber|number|
 |pageSize|number|
-|usedCount|boolean|
 |payload|object|
 
 ## deleteConnectorImage(connectorId)
 > Delete a Connector Image using the Connector ID.
 ```
 DELETE api/v2/settings/connectors/{connectorId}/images
 ```
@@ -543,14 +542,74 @@
 ```
 |Parameter|Type|
 |---|---|
 |itemId|number|
 |portId|number|
 |connectorId|number|
 
+## getBreakers(panelItemID)
+> Get a list of all Breakers for a given Panel Item. Returns JSON entity containing an array of all the Breakers for the specified Panel Item.
+```
+GET api/v2/dcimoperations/items/{panelItemID}/breakers
+```
+|Parameter|Type|
+|---|---|
+|panelItemID|number|
+
+## getBreaker(panelItemID, breakerPortId)
+> Get a list of all Breakers for a given Panel Item. Returns JSON entity containing information for a single Panel Item Breaker.
+```
+GET api/v2/dcimoperations/items/{panelItemID}/breakers/{breakerPortId}
+```
+|Parameter|Type|
+|---|---|
+|panelItemID|number|
+|breakerPortId|number|
+
+## updateBreaker(panelItemD, beakerPortID, payload)
+> Update a single Breaker for a given Panel Item. Returns JSON entity containing information for the updated Panel Item Breaker. Note: This API performs as a true PUT and not a PATCH. Unlike with a PATCH, you must specify all attributes even if you want to change only one. Attributes that are not included in the Request will be considered as removed.
+```
+PUT api/v2/dcimoperations/items/{panelItemD}/breakers/{beakerPortID} payload
+```
+|Parameter|Type|
+|---|---|
+|panelItemD|string|
+|beakerPortID|number|
+|payload|object|
+
+## createBreaker(panelItemId, payload)
+> Create a single Breaker for a given Panel Item. Returns JSON entity containing information for the created Panel Item Breaker. Note: Breaker State is set based on the connection status of the Breaker. If the breaker is connected it will always be set to "Closed", even if "Open" is specified in the Request.
+```
+POST api/v2/dcimoperations/items/{panelItemId}/breakers payload
+```
+|Parameter|Type|
+|---|---|
+|panelItemId|number|
+|payload|object|
+
+## deleteBreaker(panelItemID, breakerPortId)
+> Delete a Breaker for a given Panel Item. Returns empty JSON.
+```
+DELETE api/v2/dcimoperations/items/{panelItemID}/breakers/{breakerPortId}
+```
+|Parameter|Type|
+|---|---|
+|panelItemID|number|
+|breakerPortId|number|
+
+## createBreakersBulk(panelItemID, payload)
+> Add/Update/Delete Breakers for a given Panel Item.
+```
+POST api/v2/dcimoperations/items/{panelItemID}/breakers/bulk payload
+```
+|Parameter|Type|
+|---|---|
+|panelItemID|number|
+|payload|object|
+
 ## getLocations()
 > Returns a list for all Locations.
 ```
 GET api/v1/locations
 ```
 *No parameters.*
 
@@ -607,21 +666,14 @@
 ## getLocationFieldList()
 > Returns a list of all Location fields.
 ```
 GET api/v2/quicksearch/locations/locationListFields
 ```
 *No parameters.*
 
-## getSublocationTree()
-> Get the sublocation tree.
-```
-GET api/v2/subLocations/tree
-```
-*No parameters.*
-
 ## getSublocations(locationId)
 > Get all sub-locations for a given location in the hierarchy. The locationId is the ID of the location to get the sub-locations for.
 ```
 GET api/v2/subLocations/list/{locationId}
 ```
 |Parameter|Type|
 |---|---|
@@ -833,14 +885,32 @@
 PUT api/v2/dcimoperations/picklists/{listType} payload
 ```
 |Parameter|Type|
 |---|---|
 |listType|string|
 |payload|object|
 
+## updateDefaultValue(payload)
+> Update the default value for a picklist field.
+```
+PUT api/v2/settings/lists/defaultValue payload
+```
+|Parameter|Type|
+|---|---|
+|payload|object|
+
+## getFieldProperties(entity)
+> Get the properties for all fields applicable to the Entity.
+```
+GET api/v2/settings/lists/fieldProperties
+```
+|Parameter|Type|
+|---|---|
+|entity|string|
+
 ## submitRequest(id, payload)
 > Create a request.
 ```
 PUT api/v2/dcimoperations/items/{id} payload
 ```
 |Parameter|Type|
 |---|---|
```

### Comparing `dctrackclient-1.2.2/PKG-INFO` & `dctrackclient-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dcTrackClient
-Version: 1.2.2
+Version: 1.3.0
 Summary: Sunbird dcTrack API client in Python
 Project-URL: Homepage, https://github.com/nicfv/dcTrackClient/
 Project-URL: Bug Tracker, https://github.com/nicfv/dcTrackClient/pulls
 Author-email: Nicolas Ventura <ventura@lbl.gov>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -20,20 +20,20 @@
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API clients in Python and JavaScript
 
 ## Installation
 > dcTrackClient can be installed from the package manager of your choice.
 
 ### Python
 ```shell
-pip install dcTrackClient==1.2.2
+pip install dcTrackClient==1.3.0
 ```
 
 ### JavaScript
 ```shell
-npm i dctrackclient@1.2.2
+npm i dctrackclient@1.3.0
 ```
 
 ## Initialize a connection to the dcTrack API
 > Authentication is by using a base URL (the same URL to access the GUI) and a username and password, or a base URL and an API token.
 
 ### Python
 ```py
@@ -219,15 +219,15 @@
 { "itemId": 1234 }
 ```
 
 # Official DcTrack Documentation
 
 Visit this link for the official documentation on request bodies and attrribute names.
 
-https://www.sunbirddcim.com/help/dcTrack/v910/API/en/Default.htm
+https://www.sunbirddcim.com/help/dcTrack/v911/API/en/Default.htm
 
 # Package Documentation
 
 The section below shows all the functions contained within this client along with basic usage.
 
 ## getItem(id)
 > Get item details using the item ID. Returns an Item JSON object.
@@ -448,24 +448,23 @@
 ```
 POST api/v2/settings/connectors/delete payload
 ```
 |Parameter|Type|
 |---|---|
 |payload|object|
 
-## searchConnectors(pageNumber, pageSize, usedCount, payload)
-> Retrieve a List of Connectors. Returns JSON entity containing Connector information that was passed in from the Request payload. Please note, Compatible Connectors are not returned by this API, but can be returned when querying a single Connector using the /api/v2/settings/connectors/{connectorId} API.
+## searchConnectors(pageNumber, pageSize, payload)
+> Search for Connectors using criteria JSON object. Search criteria can be any of the fields applicable to Connector, including custom fields. Specify the fields to be included in the response. This API supports pagination. Returns a list of Connectors with the specified information.
 ```
-POST api/v2/settings/connectors/quicksearch payload
+POST api/v2/quicksearch/connectors payload
 ```
 |Parameter|Type|
 |---|---|
 |pageNumber|number|
 |pageSize|number|
-|usedCount|boolean|
 |payload|object|
 
 ## deleteConnectorImage(connectorId)
 > Delete a Connector Image using the Connector ID.
 ```
 DELETE api/v2/settings/connectors/{connectorId}/images
 ```
@@ -561,14 +560,74 @@
 ```
 |Parameter|Type|
 |---|---|
 |itemId|number|
 |portId|number|
 |connectorId|number|
 
+## getBreakers(panelItemID)
+> Get a list of all Breakers for a given Panel Item. Returns JSON entity containing an array of all the Breakers for the specified Panel Item.
+```
+GET api/v2/dcimoperations/items/{panelItemID}/breakers
+```
+|Parameter|Type|
+|---|---|
+|panelItemID|number|
+
+## getBreaker(panelItemID, breakerPortId)
+> Get a list of all Breakers for a given Panel Item. Returns JSON entity containing information for a single Panel Item Breaker.
+```
+GET api/v2/dcimoperations/items/{panelItemID}/breakers/{breakerPortId}
+```
+|Parameter|Type|
+|---|---|
+|panelItemID|number|
+|breakerPortId|number|
+
+## updateBreaker(panelItemD, beakerPortID, payload)
+> Update a single Breaker for a given Panel Item. Returns JSON entity containing information for the updated Panel Item Breaker. Note: This API performs as a true PUT and not a PATCH. Unlike with a PATCH, you must specify all attributes even if you want to change only one. Attributes that are not included in the Request will be considered as removed.
+```
+PUT api/v2/dcimoperations/items/{panelItemD}/breakers/{beakerPortID} payload
+```
+|Parameter|Type|
+|---|---|
+|panelItemD|string|
+|beakerPortID|number|
+|payload|object|
+
+## createBreaker(panelItemId, payload)
+> Create a single Breaker for a given Panel Item. Returns JSON entity containing information for the created Panel Item Breaker. Note: Breaker State is set based on the connection status of the Breaker. If the breaker is connected it will always be set to "Closed", even if "Open" is specified in the Request.
+```
+POST api/v2/dcimoperations/items/{panelItemId}/breakers payload
+```
+|Parameter|Type|
+|---|---|
+|panelItemId|number|
+|payload|object|
+
+## deleteBreaker(panelItemID, breakerPortId)
+> Delete a Breaker for a given Panel Item. Returns empty JSON.
+```
+DELETE api/v2/dcimoperations/items/{panelItemID}/breakers/{breakerPortId}
+```
+|Parameter|Type|
+|---|---|
+|panelItemID|number|
+|breakerPortId|number|
+
+## createBreakersBulk(panelItemID, payload)
+> Add/Update/Delete Breakers for a given Panel Item.
+```
+POST api/v2/dcimoperations/items/{panelItemID}/breakers/bulk payload
+```
+|Parameter|Type|
+|---|---|
+|panelItemID|number|
+|payload|object|
+
 ## getLocations()
 > Returns a list for all Locations.
 ```
 GET api/v1/locations
 ```
 *No parameters.*
 
@@ -625,21 +684,14 @@
 ## getLocationFieldList()
 > Returns a list of all Location fields.
 ```
 GET api/v2/quicksearch/locations/locationListFields
 ```
 *No parameters.*
 
-## getSublocationTree()
-> Get the sublocation tree.
-```
-GET api/v2/subLocations/tree
-```
-*No parameters.*
-
 ## getSublocations(locationId)
 > Get all sub-locations for a given location in the hierarchy. The locationId is the ID of the location to get the sub-locations for.
 ```
 GET api/v2/subLocations/list/{locationId}
 ```
 |Parameter|Type|
 |---|---|
@@ -851,14 +903,32 @@
 PUT api/v2/dcimoperations/picklists/{listType} payload
 ```
 |Parameter|Type|
 |---|---|
 |listType|string|
 |payload|object|
 
+## updateDefaultValue(payload)
+> Update the default value for a picklist field.
+```
+PUT api/v2/settings/lists/defaultValue payload
+```
+|Parameter|Type|
+|---|---|
+|payload|object|
+
+## getFieldProperties(entity)
+> Get the properties for all fields applicable to the Entity.
+```
+GET api/v2/settings/lists/fieldProperties
+```
+|Parameter|Type|
+|---|---|
+|entity|string|
+
 ## submitRequest(id, payload)
 > Create a request.
 ```
 PUT api/v2/dcimoperations/items/{id} payload
 ```
 |Parameter|Type|
 |---|---|
```

