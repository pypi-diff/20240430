# Comparing `tmp/inventree_supplier_panel-0.3.0.tar.gz` & `tmp/inventree_supplier_panel-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inventree_supplier_panel-0.3.0.tar", last modified: Mon Apr 22 15:53:51 2024, max compression
+gzip compressed data, was "inventree_supplier_panel-0.3.1.tar", last modified: Tue Apr 30 18:02:14 2024, max compression
```

## Comparing `inventree_supplier_panel-0.3.0.tar` & `inventree_supplier_panel-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:53:51.872874 inventree_supplier_panel-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-22 15:53:40.000000 inventree_supplier_panel-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-22 15:53:40.000000 inventree_supplier_panel-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-04-22 15:53:51.872874 inventree_supplier_panel-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-04-22 15:53:40.000000 inventree_supplier_panel-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:53:51.872874 inventree_supplier_panel-0.3.0/inventree_supplier_panel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:53:40.000000 inventree_supplier_panel-0.3.0/inventree_supplier_panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-22 15:53:40.000000 inventree_supplier_panel-0.3.0/inventree_supplier_panel/meta_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    28573 2024-04-22 15:53:40.000000 inventree_supplier_panel-0.3.0/inventree_supplier_panel/supplier_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:53:51.868874 inventree_supplier_panel-0.3.0/inventree_supplier_panel/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:53:51.872874 inventree_supplier_panel-0.3.0/inventree_supplier_panel/templates/supplier_panel/
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-22 15:53:40.000000 inventree_supplier_panel-0.3.0/inventree_supplier_panel/templates/supplier_panel/add_supplierpart.html
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-22 15:53:40.000000 inventree_supplier_panel-0.3.0/inventree_supplier_panel/templates/supplier_panel/digikey.html
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-22 15:53:40.000000 inventree_supplier_panel-0.3.0/inventree_supplier_panel/templates/supplier_panel/mouser.html
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-22 15:53:40.000000 inventree_supplier_panel-0.3.0/inventree_supplier_panel/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:53:51.872874 inventree_supplier_panel-0.3.0/inventree_supplier_panel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-04-22 15:53:51.000000 inventree_supplier_panel-0.3.0/inventree_supplier_panel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-22 15:53:51.000000 inventree_supplier_panel-0.3.0/inventree_supplier_panel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 15:53:51.000000 inventree_supplier_panel-0.3.0/inventree_supplier_panel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-22 15:53:51.000000 inventree_supplier_panel-0.3.0/inventree_supplier_panel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-22 15:53:51.000000 inventree_supplier_panel-0.3.0/inventree_supplier_panel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 15:53:51.872874 inventree_supplier_panel-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-22 15:53:40.000000 inventree_supplier_panel-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:02:14.858384 inventree_supplier_panel-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-30 18:02:02.000000 inventree_supplier_panel-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-30 18:02:02.000000 inventree_supplier_panel-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-04-30 18:02:14.858384 inventree_supplier_panel-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-30 18:02:02.000000 inventree_supplier_panel-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:02:14.854384 inventree_supplier_panel-0.3.1/inventree_supplier_panel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:02:02.000000 inventree_supplier_panel-0.3.1/inventree_supplier_panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-30 18:02:02.000000 inventree_supplier_panel-0.3.1/inventree_supplier_panel/meta_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28603 2024-04-30 18:02:02.000000 inventree_supplier_panel-0.3.1/inventree_supplier_panel/supplier_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:02:14.854384 inventree_supplier_panel-0.3.1/inventree_supplier_panel/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:02:14.858384 inventree_supplier_panel-0.3.1/inventree_supplier_panel/templates/supplier_panel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-30 18:02:02.000000 inventree_supplier_panel-0.3.1/inventree_supplier_panel/templates/supplier_panel/add_supplierpart.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-30 18:02:02.000000 inventree_supplier_panel-0.3.1/inventree_supplier_panel/templates/supplier_panel/digikey.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-30 18:02:02.000000 inventree_supplier_panel-0.3.1/inventree_supplier_panel/templates/supplier_panel/mouser.html
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 18:02:02.000000 inventree_supplier_panel-0.3.1/inventree_supplier_panel/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:02:14.858384 inventree_supplier_panel-0.3.1/inventree_supplier_panel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-04-30 18:02:14.000000 inventree_supplier_panel-0.3.1/inventree_supplier_panel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-30 18:02:14.000000 inventree_supplier_panel-0.3.1/inventree_supplier_panel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:02:14.000000 inventree_supplier_panel-0.3.1/inventree_supplier_panel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-30 18:02:14.000000 inventree_supplier_panel-0.3.1/inventree_supplier_panel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 18:02:14.000000 inventree_supplier_panel-0.3.1/inventree_supplier_panel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 18:02:14.858384 inventree_supplier_panel-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-30 18:02:02.000000 inventree_supplier_panel-0.3.1/setup.py
```

### Comparing `inventree_supplier_panel-0.3.0/LICENSE` & `inventree_supplier_panel-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inventree_supplier_panel-0.3.0/PKG-INFO` & `inventree_supplier_panel-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-supplier-panel
-Version: 0.3.0
+Version: 0.3.1
 Summary: Syncronize a PO with a supplier online store
 Home-page: https://github.com/SergeoLacruz/inventree-supplier-panel
 Author: Michael Buchmann
 Author-email: michael@buchmann.ruhr
 License: MIT
 Keywords: inventree supplier inventory store purchase order
 Requires-Python: >=3.6
@@ -22,17 +22,18 @@
 The data will be created in your supplier account. Each time you transfer your PO
 a new data set cart will be created. So make sure that you delete them from time to time in
 the supplier WEB interface.
 The plugin also helps to create supplierparts based on the supplier part number..
 Actually the plugin supports two suppliers: Mouser and Digikey.
 
 ## Installation
+The plugin is on pypi. You can install it by just calling:
 
 ```
-pip install git+https://github.com/SergeoLacruz/inventree-supplier-panel
+pip install inventree-supplier-panel
 ```
 
 ## Configuration
 
 ### Mouser Supplier ID
 Place here the primary key of the supplier Mouser in your system. You can select from a list of
 your suppliers. If this is not set the panel will not be displayed and a error is raised.
@@ -44,15 +45,15 @@
 ### Mouser API key
 Place here your Mouser key for manipulating shopping carts. You find it in your Mouser account.
 
 ### Digikey ID and Digikey Secret
 This is the client ID and the client secret that has been generated in the Digkey API admin WEB portal.
 Copy it from there to the InvenTree settings.
 
-### Digikey token and Digikey refrech token
+### Digikey token and Digikey refresh token
 These fields are filled automatically. The Digikey API requires two tokens with different life times.
 Please refer to the Digikey section for more information.
 
 ### Proxy CON
 Protocol to proxy server e.g. https
 
 ### Proxy URL
@@ -175,15 +176,15 @@
 are stored in the plugin setting area. Do not change them manually.
 
 Each time you transfer a PO the refresh token is called independently from the
 tokens live time. This also refreshes the refresh token. So you are save when
 you use the plugin ate least once in 90 days. In case the token gets bad you need to
 create a fresh set using the token button again.
 
-If you are confused now read the documentation on the Digikey WEB page for more details. 
+If you are confused now read the documentation on the Digikey WEB page for more details.
 
 #### MyLists
 Digikey does not have such a simple shopping cart API. The plugin uses the MyLists API.
 It creates a list on the WEB shop that can easily be transferred to a shopping
 cart. When creating a list a list name has to be provided. The plugin creates a name
 based on the PO name and adding a -xx that counts upwards each time you push the button.
 The reason is that each name is allowed only once. Even when the list is deleted, the
```

### Comparing `inventree_supplier_panel-0.3.0/README.md` & `inventree_supplier_panel-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 The data will be created in your supplier account. Each time you transfer your PO
 a new data set cart will be created. So make sure that you delete them from time to time in
 the supplier WEB interface.
 The plugin also helps to create supplierparts based on the supplier part number..
 Actually the plugin supports two suppliers: Mouser and Digikey.
 
 ## Installation
+The plugin is on pypi. You can install it by just calling:
 
 ```
-pip install git+https://github.com/SergeoLacruz/inventree-supplier-panel
+pip install inventree-supplier-panel
 ```
 
 ## Configuration
 
 ### Mouser Supplier ID
 Place here the primary key of the supplier Mouser in your system. You can select from a list of
 your suppliers. If this is not set the panel will not be displayed and a error is raised.
@@ -31,15 +32,15 @@
 ### Mouser API key
 Place here your Mouser key for manipulating shopping carts. You find it in your Mouser account.
 
 ### Digikey ID and Digikey Secret
 This is the client ID and the client secret that has been generated in the Digkey API admin WEB portal.
 Copy it from there to the InvenTree settings.
 
-### Digikey token and Digikey refrech token
+### Digikey token and Digikey refresh token
 These fields are filled automatically. The Digikey API requires two tokens with different life times.
 Please refer to the Digikey section for more information.
 
 ### Proxy CON
 Protocol to proxy server e.g. https
 
 ### Proxy URL
@@ -162,15 +163,15 @@
 are stored in the plugin setting area. Do not change them manually.
 
 Each time you transfer a PO the refresh token is called independently from the
 tokens live time. This also refreshes the refresh token. So you are save when
 you use the plugin ate least once in 90 days. In case the token gets bad you need to
 create a fresh set using the token button again.
 
-If you are confused now read the documentation on the Digikey WEB page for more details. 
+If you are confused now read the documentation on the Digikey WEB page for more details.
 
 #### MyLists
 Digikey does not have such a simple shopping cart API. The plugin uses the MyLists API.
 It creates a list on the WEB shop that can easily be transferred to a shopping
 cart. When creating a list a list name has to be provided. The plugin creates a name
 based on the PO name and adding a -xx that counts upwards each time you push the button.
 The reason is that each name is allowed only once. Even when the list is deleted, the
```

### Comparing `inventree_supplier_panel-0.3.0/inventree_supplier_panel/meta_access.py` & `inventree_supplier_panel-0.3.1/inventree_supplier_panel/meta_access.py`

 * *Files identical despite different names*

### Comparing `inventree_supplier_panel-0.3.0/inventree_supplier_panel/supplier_panel.py` & `inventree_supplier_panel-0.3.1/inventree_supplier_panel/supplier_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,16 @@
         if isinstance(view, PartDetail):
             has_permission = (check_user_role(view.request.user, 'part', 'change')
                               or check_user_role(view.request.user, 'part', 'delete')
                               or check_user_role(view.request.user, 'part', 'add'))
             show_panel = False
             for s in self.registered_suppliers:
                 show_panel = show_panel or self.registered_suppliers[s]['is_registered']
-            if has_permission and show_panel:
+            part = view.get_object()
+            if has_permission and show_panel and part.purchaseable:
                 panels.append({
                     'title': 'Automatic Supplier parts',
                     'icon': 'fa-user',
                     'content_template': 'supplier_panel/add_supplierpart.html',
                 })
         return panels
 
@@ -505,25 +506,24 @@
         token['status_code'] = response.status_code
         token['message'] = 'success'
         token['acces_token'] = response_data['access_token']
         token['refresh_token'] = response_data['refresh_token']
         return (token)
 
 # --------------------------- receive_authcode --------------------------------
-# The redirect_uri is just a string that has to be there. The content is
-# ignored by Digikey
 
     def receive_authcode(self, request):
         auth_code = request.GET.get('code')
         url = 'https://api.digikey.com/v1/oauth2/token'
+        redirect_uri = InvenTreeSetting.get_setting('INVENTREE_BASE_URL') + '/' + self.base_url + 'digikeytoken/'
         url_data = {
             'code': auth_code,
             'client_id': self.get_setting('DIGIKEY_CLIENT_ID'),
             'client_secret': self.get_setting('DIGIKEY_CLIENT_SECRET'),
-            'redirect_uri': 'https://192.168.1.40:8123/plugin/suppliercart/digikeytoken/',
+            'redirect_uri': redirect_uri,
             'grant_type': 'authorization_code'
         }
         header = {}
         response = self.post_request(url_data, url, headers=header)
         if response.status_code == 200:
             print('\033[32mAccess Token get SUCCESS\033[0m')
             response_data = response.json()
```

### Comparing `inventree_supplier_panel-0.3.0/inventree_supplier_panel/templates/supplier_panel/add_supplierpart.html` & `inventree_supplier_panel-0.3.1/inventree_supplier_panel/templates/supplier_panel/add_supplierpart.html`

 * *Files 6% similar despite different names*

```diff
@@ -27,27 +27,27 @@
 {% endif %}
 
 <table class='table table-condensed'>
 <form>
 <tbody>
     <tr>
         <td> Select Supplier </td>
-        <td> 
+        <td>
 	    <select id="supplier">
 		{% for supplier,data in plugin.registered_suppliers.items %}
                 {% if data.is_registered == True %}
 		   <option value="{{ data.pk }}"> {{ data.name }} </option>
                 {% endif %}
 		{% endfor %}
 	    </select>
         </td>
     </tr>
     <tr>
         <td> Exact supplier part number from suppliers WEB page</td>
-        <td> 
+        <td>
             <input id="sku" type="text" value="">
         </td>
     </tr>
 </tbody>
 <tfoot>
     <tr>
 	<td>
```

### Comparing `inventree_supplier_panel-0.3.0/inventree_supplier_panel/templates/supplier_panel/digikey.html` & `inventree_supplier_panel-0.3.1/inventree_supplier_panel/templates/supplier_panel/digikey.html`

 * *Files identical despite different names*

### Comparing `inventree_supplier_panel-0.3.0/inventree_supplier_panel/templates/supplier_panel/mouser.html` & `inventree_supplier_panel-0.3.1/inventree_supplier_panel/templates/supplier_panel/mouser.html`

 * *Files identical despite different names*

### Comparing `inventree_supplier_panel-0.3.0/inventree_supplier_panel.egg-info/PKG-INFO` & `inventree_supplier_panel-0.3.1/inventree_supplier_panel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-supplier-panel
-Version: 0.3.0
+Version: 0.3.1
 Summary: Syncronize a PO with a supplier online store
 Home-page: https://github.com/SergeoLacruz/inventree-supplier-panel
 Author: Michael Buchmann
 Author-email: michael@buchmann.ruhr
 License: MIT
 Keywords: inventree supplier inventory store purchase order
 Requires-Python: >=3.6
@@ -22,17 +22,18 @@
 The data will be created in your supplier account. Each time you transfer your PO
 a new data set cart will be created. So make sure that you delete them from time to time in
 the supplier WEB interface.
 The plugin also helps to create supplierparts based on the supplier part number..
 Actually the plugin supports two suppliers: Mouser and Digikey.
 
 ## Installation
+The plugin is on pypi. You can install it by just calling:
 
 ```
-pip install git+https://github.com/SergeoLacruz/inventree-supplier-panel
+pip install inventree-supplier-panel
 ```
 
 ## Configuration
 
 ### Mouser Supplier ID
 Place here the primary key of the supplier Mouser in your system. You can select from a list of
 your suppliers. If this is not set the panel will not be displayed and a error is raised.
@@ -44,15 +45,15 @@
 ### Mouser API key
 Place here your Mouser key for manipulating shopping carts. You find it in your Mouser account.
 
 ### Digikey ID and Digikey Secret
 This is the client ID and the client secret that has been generated in the Digkey API admin WEB portal.
 Copy it from there to the InvenTree settings.
 
-### Digikey token and Digikey refrech token
+### Digikey token and Digikey refresh token
 These fields are filled automatically. The Digikey API requires two tokens with different life times.
 Please refer to the Digikey section for more information.
 
 ### Proxy CON
 Protocol to proxy server e.g. https
 
 ### Proxy URL
@@ -175,15 +176,15 @@
 are stored in the plugin setting area. Do not change them manually.
 
 Each time you transfer a PO the refresh token is called independently from the
 tokens live time. This also refreshes the refresh token. So you are save when
 you use the plugin ate least once in 90 days. In case the token gets bad you need to
 create a fresh set using the token button again.
 
-If you are confused now read the documentation on the Digikey WEB page for more details. 
+If you are confused now read the documentation on the Digikey WEB page for more details.
 
 #### MyLists
 Digikey does not have such a simple shopping cart API. The plugin uses the MyLists API.
 It creates a list on the WEB shop that can easily be transferred to a shopping
 cart. When creating a list a list name has to be provided. The plugin creates a name
 based on the PO name and adding a -xx that counts upwards each time you push the button.
 The reason is that each name is allowed only once. Even when the list is deleted, the
```

### Comparing `inventree_supplier_panel-0.3.0/inventree_supplier_panel.egg-info/SOURCES.txt` & `inventree_supplier_panel-0.3.1/inventree_supplier_panel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inventree_supplier_panel-0.3.0/setup.py` & `inventree_supplier_panel-0.3.1/setup.py`

 * *Files identical despite different names*

