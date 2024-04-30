# Comparing `tmp/fab_react_toolkit-0.4.3.tar.gz` & `tmp/fab_react_toolkit-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fab_react_toolkit-0.4.3.tar", last modified: Wed Apr 17 07:24:10 2024, max compression
+gzip compressed data, was "fab_react_toolkit-0.4.4.tar", last modified: Tue Apr 30 12:11:48 2024, max compression
```

## Comparing `fab_react_toolkit-0.4.3.tar` & `fab_react_toolkit-0.4.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:24:10.297059 fab_react_toolkit-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-17 07:24:02.000000 fab_react_toolkit-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-17 07:24:10.297059 fab_react_toolkit-0.4.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:24:10.293059 fab_react_toolkit-0.4.3/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:24:10.293059 fab_react_toolkit-0.4.3/example/app/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-17 07:24:02.000000 fab_react_toolkit-0.4.3/example/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-17 07:24:02.000000 fab_react_toolkit-0.4.3/example/app/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-17 07:24:02.000000 fab_react_toolkit-0.4.3/example/app/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-17 07:24:02.000000 fab_react_toolkit-0.4.3/example/app/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-17 07:24:02.000000 fab_react_toolkit-0.4.3/example/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 07:24:02.000000 fab_react_toolkit-0.4.3/example/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-17 07:24:02.000000 fab_react_toolkit-0.4.3/example/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:24:10.297059 fab_react_toolkit-0.4.3/fab_react_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-17 07:24:02.000000 fab_react_toolkit-0.4.3/fab_react_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:24:10.297059 fab_react_toolkit-0.4.3/fab_react_toolkit/api/
--rw-r--r--   0 runner    (1001) docker     (127)    21837 2024-04-17 07:24:02.000000 fab_react_toolkit-0.4.3/fab_react_toolkit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-17 07:24:02.000000 fab_react_toolkit-0.4.3/fab_react_toolkit/api/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-17 07:24:02.000000 fab_react_toolkit-0.4.3/fab_react_toolkit/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-17 07:24:02.000000 fab_react_toolkit-0.4.3/fab_react_toolkit/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29186 2024-04-17 07:24:02.000000 fab_react_toolkit-0.4.3/fab_react_toolkit/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-04-17 07:24:02.000000 fab_react_toolkit-0.4.3/fab_react_toolkit/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-17 07:24:02.000000 fab_react_toolkit-0.4.3/fab_react_toolkit/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-17 07:24:02.000000 fab_react_toolkit-0.4.3/fab_react_toolkit/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:24:10.297059 fab_react_toolkit-0.4.3/fab_react_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-17 07:24:10.000000 fab_react_toolkit-0.4.3/fab_react_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-17 07:24:10.000000 fab_react_toolkit-0.4.3/fab_react_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:24:10.000000 fab_react_toolkit-0.4.3/fab_react_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 07:24:10.000000 fab_react_toolkit-0.4.3/fab_react_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 07:24:10.000000 fab_react_toolkit-0.4.3/fab_react_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-17 07:24:02.000000 fab_react_toolkit-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-17 07:24:02.000000 fab_react_toolkit-0.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 07:24:10.297059 fab_react_toolkit-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:11:48.153905 fab_react_toolkit-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 12:11:38.000000 fab_react_toolkit-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-30 12:11:48.153905 fab_react_toolkit-0.4.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:11:48.149905 fab_react_toolkit-0.4.4/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:11:48.149905 fab_react_toolkit-0.4.4/example/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-30 12:11:38.000000 fab_react_toolkit-0.4.4/example/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-30 12:11:38.000000 fab_react_toolkit-0.4.4/example/app/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-30 12:11:38.000000 fab_react_toolkit-0.4.4/example/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-30 12:11:38.000000 fab_react_toolkit-0.4.4/example/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-30 12:11:38.000000 fab_react_toolkit-0.4.4/example/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 12:11:38.000000 fab_react_toolkit-0.4.4/example/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-30 12:11:38.000000 fab_react_toolkit-0.4.4/example/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:11:48.149905 fab_react_toolkit-0.4.4/fab_react_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-30 12:11:38.000000 fab_react_toolkit-0.4.4/fab_react_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:11:48.153905 fab_react_toolkit-0.4.4/fab_react_toolkit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    21837 2024-04-30 12:11:38.000000 fab_react_toolkit-0.4.4/fab_react_toolkit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-30 12:11:38.000000 fab_react_toolkit-0.4.4/fab_react_toolkit/api/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-30 12:11:38.000000 fab_react_toolkit-0.4.4/fab_react_toolkit/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-30 12:11:38.000000 fab_react_toolkit-0.4.4/fab_react_toolkit/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20785 2024-04-30 12:11:38.000000 fab_react_toolkit-0.4.4/fab_react_toolkit/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-04-30 12:11:38.000000 fab_react_toolkit-0.4.4/fab_react_toolkit/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-30 12:11:38.000000 fab_react_toolkit-0.4.4/fab_react_toolkit/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-30 12:11:38.000000 fab_react_toolkit-0.4.4/fab_react_toolkit/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:11:48.153905 fab_react_toolkit-0.4.4/fab_react_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-30 12:11:48.000000 fab_react_toolkit-0.4.4/fab_react_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-30 12:11:48.000000 fab_react_toolkit-0.4.4/fab_react_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 12:11:48.000000 fab_react_toolkit-0.4.4/fab_react_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 12:11:48.000000 fab_react_toolkit-0.4.4/fab_react_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 12:11:48.000000 fab_react_toolkit-0.4.4/fab_react_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-30 12:11:38.000000 fab_react_toolkit-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-30 12:11:38.000000 fab_react_toolkit-0.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 12:11:48.153905 fab_react_toolkit-0.4.4/setup.cfg
```

### Comparing `fab_react_toolkit-0.4.3/LICENSE` & `fab_react_toolkit-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.3/PKG-INFO` & `fab_react_toolkit-0.4.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.4.3
+Version: 0.4.4
 Summary: A small example package
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fab_react_toolkit-0.4.3/example/app/__init__.py` & `fab_react_toolkit-0.4.4/example/app/__init__.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.3/example/app/apis.py` & `fab_react_toolkit-0.4.4/example/app/apis.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.3/example/app/config.py` & `fab_react_toolkit-0.4.4/example/app/config.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.3/example/app/models.py` & `fab_react_toolkit-0.4.4/example/app/models.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.3/example/run.py` & `fab_react_toolkit-0.4.4/example/run.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.3/fab_react_toolkit/__init__.py` & `fab_react_toolkit-0.4.4/fab_react_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.3/fab_react_toolkit/api/__init__.py` & `fab_react_toolkit-0.4.4/fab_react_toolkit/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.3/fab_react_toolkit/api/convert.py` & `fab_react_toolkit-0.4.4/fab_react_toolkit/api/convert.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.3/fab_react_toolkit/api/utils.py` & `fab_react_toolkit-0.4.4/fab_react_toolkit/api/utils.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.3/fab_react_toolkit/apis.py` & `fab_react_toolkit-0.4.4/fab_react_toolkit/apis.py`

 * *Files 20% similar despite different names*

```diff
@@ -145,208 +145,14 @@
 
         role_ids = [role.id for role in user.roles]
         permissions = [x for x in set([v for k, v in sm.get_user_permissions(user)]) if sm.has_access("can_get", x)]
         user_data['permissions'] = permissions
 
         return user_data
 
-    @expose('/login', methods=["POST"])
-    @safe
-    def login(self):
-        """Login endpoint for the API, creates a session cookie
-         ---
-         post:
-           description: >-
-             Authenticate and create a session cookie
-           requestBody:
-             required: true
-             content:
-               application/json:
-                 schema:
-                   type: object
-                   properties:
-                     username:
-                       description: The username for authentication
-                       example: user1234
-                       type: string
-                       required: true
-                     password:
-                       description: The password for authentication
-                       example: complex-password
-                       type: string
-                       required: true
-           responses:
-             200:
-               description: Authentication Successful
-             400:
-               $ref: '#/components/responses/400'
-             401:
-               $ref: '#/components/responses/401'
-             500:
-               $ref: '#/components/responses/500'
-         """
-
-        if current_user is not None and current_user.is_authenticated:
-            user_data = self.get_client_user_data(current_user)
-            return self.response(200, **user_data)
-
-        # Read and validate request body
-        if not request.is_json:
-            return self.response_400(message="Request payload is not JSON")
-        username = request.json.get(API_SECURITY_USERNAME_KEY, None)
-        password = request.json.get(API_SECURITY_PASSWORD_KEY, None)
-
-        if not username or not password:
-            return self.response_400(message="Missing required parameter")
-
-        # Authenticate based on method
-        user = None
-        method = self.appbuilder.sm.auth_type
-        if method == AUTH_DB:
-            user = self.appbuilder.sm.auth_user_db(username, password)
-        elif method == AUTH_LDAP:
-            user = self.appbuilder.sm.auth_user_ldap(username, password)
-
-        elif method == AUTH_REMOTE_USER:
-            username = request.environ.get("REMOTE_USER")
-            if username:
-                user = self.appbuilder.sm.auth_user_remote_user(username)
-        else:
-            return self.response_500(
-                message="Method {} not supported".format(method)
-            )
-        if not user:
-            return self.response_401()
-
-        # get client user data
-        user_data = self.get_client_user_data(user)
-        # Set session cookie
-        login_user(user, remember=False)
-        return self.response(200, **user_data)
-
-    @expose('/login/<provider>', methods=["GET"])
-    @safe
-    def init_oauth(self, provider):
-        """OAuth initiation endpoint for the API
-         ---
-          get:
-            description: >-
-              Initiate OAuth login
-            parameters:
-              - in: path
-                name: provider
-                schema:
-                  type: str
-                required: true
-                description: Provider to authenticate against
-
-            responses:
-              302:
-                $ref: '#/components/responses/202'
-              500:
-                $ref: '#/components/responses/500'
-         """
-        if current_user is not None and current_user.is_authenticated:
-            return redirect(self.appbuilder.app.config["REDIRECT_URI"])
-
-        if provider is None:
-            return self.response_400(message="Missing required parameter")
-
-        state = jwt.encode(
-            request.args.to_dict(flat=False),
-            self.appbuilder.app.config["SECRET_KEY"],
-            algorithm="HS256",
-        )
-
-        try:
-            if provider == "twitter":
-                # not works
-                return self.appbuilder.sm.oauth_remotes[provider].authorize_redirect(
-                    redirect_uri=request.base_url + "/callback"
-                )
-            else:
-                return self.appbuilder.sm.oauth_remotes[provider].authorize_redirect(
-                    redirect_uri=request.base_url + "/callback",
-                    state=state.decode("ascii") if isinstance(state, bytes) else state,
-                )
-
-        except Exception as e:
-            print(e)
-            return self.response_500()
-
-    @expose("/login/<provider>/callback")
-    def oauth_callback(self, provider):
-        """OAuth redirect endpoint for the API, creates a session cookie
-           Make sure to add this endpoint as the redirect uri of your provider
-         ---
-          get:
-            description: >-
-              Authenticate and create a session cookie
-            parameters:
-              - in: path
-                name: provider
-                schema:
-                  type: str
-                required: true
-                description: Provider to authenticate against
-
-            responses:
-              302:
-                $ref: '#/components/responses/202'
-              400:
-                $ref: '#/components/responses/400'
-              500:
-                $ref: '#/components/responses/500'
-         """
-        if provider not in self.appbuilder.sm.oauth_remotes:
-            return self.response_400(message="Provider not supported")
-        resp = self.appbuilder.sm.oauth_remotes[provider].authorize_access_token()
-        if resp is None:
-            return self.response_400(message="Request for sign in was denied.")
-
-        # Retrieves specific user info from the provider
-        try:
-            self.appbuilder.sm.set_oauth_session(provider, resp)
-            userinfo = self.appbuilder.sm.oauth_user_info(provider, resp)
-        except Exception as e:
-            user = None
-        else:
-            # User email is not whitelisted
-            if provider in self.appbuilder.sm.oauth_whitelists:
-                whitelist = self.appbuilder.sm.oauth_whitelists[provider]
-                allow = False
-                for email in whitelist:
-                    if "email" in userinfo and re.search(email, userinfo["email"]):
-                        allow = True
-                        break
-                if not allow:
-                    self.response_401()
-            user = self.appbuilder.sm.auth_user_oauth(userinfo)
-        if user is None:
-            self.response_400(message="Invalid login. Please try again.")
-        else:
-            login_user(user)
-            try:
-                # redirect uri could be stored in state, I don't see the point though
-                state = jwt.decode(
-                    request.args["state"],
-                    self.appbuilder.app.config["SECRET_KEY"],
-                    algorithms=["HS256"],
-                )
-            except jwt.InvalidTokenError:
-                raise Exception("State signature is not valid!")
-
-            return redirect(self.appbuilder.app.config["REDIRECT_URI"])
-
-    @expose('/logout', methods=["GET"])
-    @safe
-    def logout(self):
-        """Logs the user out and deletes session cookie"""
-        logout_user()
-        return self.response(200, message="Logout successful")
 
     @expose('/signup', methods=["POST"])
     @safe
     def signup(self):
         """
         This endpoint creates a new user
 
@@ -489,48 +295,14 @@
         item.last_name = lastname
         self.appbuilder.sm.update_user(item)
 
         # get public user data
         user_data = self.get_client_user_data(item)
         return self.response(200, **user_data)
 
-    @expose('/resetpassword', methods=["PUT"])
-    @safe
-    def reset_password(self):
-        """Reset user password endpoint for the API, resets user password
-             ---
-             post:
-               description: >-
-                 Reset user password
-               requestBody:
-                 required: true
-                 content:
-                   application/json:
-                     schema:
-                       type: object
-                       properties:
-                         password:
-                           description: The password to rest
-                           example: complex-password
-                           type: string
-                           required: true
-               responses:
-                 200:
-                   description: Update Successful
-                 400:
-                   $ref: '#/components/responses/400'
-                 401:
-                   $ref: '#/components/responses/401'
-                 500:
-                   $ref: '#/components/responses/500'
-             """
-        password = request.json.get('password', None)
-        self.appbuilder.sm.reset_password(current_user.id, password)
-        return self.response(200, message="Update successful")
-
     # testing endpoint (might be useful in general)
 
     @expose('/authenticate', methods=["GET"])
     @login_required
     @safe
     def authenticate(self):
```

### Comparing `fab_react_toolkit-0.4.3/fab_react_toolkit/filters.py` & `fab_react_toolkit-0.4.4/fab_react_toolkit/filters.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.3/fab_react_toolkit/views.py` & `fab_react_toolkit-0.4.4/fab_react_toolkit/views.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.3/fab_react_toolkit.egg-info/PKG-INFO` & `fab_react_toolkit-0.4.4/fab_react_toolkit.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.4.3
+Version: 0.4.4
 Summary: A small example package
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fab_react_toolkit-0.4.3/fab_react_toolkit.egg-info/SOURCES.txt` & `fab_react_toolkit-0.4.4/fab_react_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.3/pyproject.toml` & `fab_react_toolkit-0.4.4/pyproject.toml`

 * *Files identical despite different names*

