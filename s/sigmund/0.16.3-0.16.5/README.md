# Comparing `tmp/sigmund-0.16.3.tar.gz` & `tmp/sigmund-0.16.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmund-0.16.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sigmund-0.16.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sigmund-0.16.3.tar` & `sigmund-0.16.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    35147 2024-04-25 18:33:14.190341 sigmund-0.16.3/COPYING
--rw-r--r--   0        0        0     1017 2024-04-25 18:33:14.190341 sigmund-0.16.3/pyproject.toml
--rw-r--r--   0        0        0     3037 2024-04-25 18:33:14.190341 sigmund-0.16.3/readme.md
--rw-r--r--   0        0        0      101 2024-04-25 18:33:14.190341 sigmund-0.16.3/sigmund/__init__.py
--rw-r--r--   0        0        0     2746 2024-04-25 18:33:14.190341 sigmund-0.16.3/sigmund/attachments.py
--rw-r--r--   0        0        0     9770 2024-04-25 18:33:14.190341 sigmund-0.16.3/sigmund/config.py
--rw-r--r--   0        0        0        0 2024-04-25 18:33:14.190341 sigmund-0.16.3/sigmund/database/__init__.py
--rw-r--r--   0        0        0     1030 2024-04-25 18:33:14.190341 sigmund-0.16.3/sigmund/database/encryption.py
--rw-r--r--   0        0        0    14378 2024-04-25 18:33:14.190341 sigmund-0.16.3/sigmund/database/manager.py
--rw-r--r--   0        0        0     3213 2024-04-25 18:33:14.190341 sigmund-0.16.3/sigmund/database/models.py
--rw-r--r--   0        0        0     6331 2024-04-25 18:33:14.190341 sigmund-0.16.3/sigmund/documentation.py
--rw-r--r--   0        0        0      389 2024-04-25 18:33:14.190341 sigmund-0.16.3/sigmund/forms.py
--rw-r--r--   0        0        0     2547 2024-04-25 18:33:14.190341 sigmund-0.16.3/sigmund/library.py
--rw-r--r--   0        0        0    10115 2024-04-25 18:33:14.190341 sigmund-0.16.3/sigmund/messages.py
--rw-r--r--   0        0        0     1252 2024-04-25 18:33:14.194341 sigmund-0.16.3/sigmund/model/__init__.py
--rw-r--r--   0        0        0     5297 2024-04-25 18:33:14.194341 sigmund-0.16.3/sigmund/model/_anthropic_model.py
--rw-r--r--   0        0        0     4605 2024-04-25 18:33:14.194341 sigmund-0.16.3/sigmund/model/_base_model.py
--rw-r--r--   0        0        0      379 2024-04-25 18:33:14.194341 sigmund-0.16.3/sigmund/model/_dummy_model.py
--rw-r--r--   0        0        0     2700 2024-04-25 18:33:14.194341 sigmund-0.16.3/sigmund/model/_mistral_model.py
--rw-r--r--   0        0        0     3373 2024-04-25 18:33:14.194341 sigmund-0.16.3/sigmund/model/_openai_model.py
--rw-r--r--   0        0        0     2141 2024-04-25 18:33:14.194341 sigmund-0.16.3/sigmund/prompt.py
--rw-r--r--   0        0        0      160 2024-04-25 18:33:14.194341 sigmund-0.16.3/sigmund/routes/__init__.py
--rw-r--r--   0        0        0     7298 2024-04-25 18:33:14.194341 sigmund-0.16.3/sigmund/routes/api.py
--rw-r--r--   0        0        0     5775 2024-04-25 18:33:14.194341 sigmund-0.16.3/sigmund/routes/app.py
--rw-r--r--   0        0        0     3606 2024-04-25 18:33:14.194341 sigmund-0.16.3/sigmund/routes/google_login.py
--rw-r--r--   0        0        0     7732 2024-04-25 18:33:14.194341 sigmund-0.16.3/sigmund/routes/subscribe.py
--rw-r--r--   0        0        0     1494 2024-04-25 18:33:14.194341 sigmund-0.16.3/sigmund/server.py
--rw-r--r--   0        0        0     9354 2024-04-25 18:33:14.194341 sigmund-0.16.3/sigmund/sigmund.py
--rw-r--r--   0        0        0     4270 2024-04-25 18:33:14.194341 sigmund-0.16.3/sigmund/static/about.md
--rw-r--r--   0        0        0  4708018 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/static/background.png
--rw-r--r--   0        0        0      386 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/static/favicon.svg
--rw-r--r--   0        0        0     1433 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/static/login.md
--rw-r--r--   0        0        0     4976 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/static/pygments.css
--rw-r--r--   0        0        0   708136 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/static/sofa-with-sigmund.png
--rw-r--r--   0        0        0   684883 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/static/sofa.png
--rw-r--r--   0        0        0     3428 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/static/terms.md
--rw-r--r--   0        0        0     1359 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/templates/chat.html
--rw-r--r--   0        0        0      242 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/templates/footer.html
--rw-r--r--   0        0        0      574 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/templates/head.html
--rw-r--r--   0        0        0      244 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/templates/header.html
--rw-r--r--   0        0        0      329 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/templates/info-page.html
--rw-r--r--   0        0        0     3739 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/templates/login.html
--rw-r--r--   0        0        0    10786 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/templates/main.js
--rw-r--r--   0        0        0    12359 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/templates/menu.html
--rw-r--r--   0        0        0       80 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/templates/sign-out.html
--rw-r--r--   0        0        0     6353 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/templates/stylesheet.css.jinja
--rw-r--r--   0        0        0      531 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/templates/subscribe-error.html
--rw-r--r--   0        0        0     1555 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/templates/subscribe-now.html
--rw-r--r--   0        0        0      515 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/templates/subscribe-success.html
--rw-r--r--   0        0        0      265 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/tools/__init__.py
--rw-r--r--   0        0        0     2231 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/tools/_base_tool.py
--rw-r--r--   0        0        0     2920 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/tools/_download.py
--rw-r--r--   0        0        0     2085 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/tools/_execute_code.py
--rw-r--r--   0        0        0     1846 2024-04-25 18:33:14.202341 sigmund-0.16.3/sigmund/tools/_read_attachment.py
--rw-r--r--   0        0        0     2076 2024-04-25 18:33:14.206341 sigmund-0.16.3/sigmund/tools/_search_documentation.py
--rw-r--r--   0        0        0     1275 2024-04-25 18:33:14.206341 sigmund-0.16.3/sigmund/tools/_search_google_scholar.py
--rw-r--r--   0        0        0     4358 2024-04-25 18:33:14.206341 sigmund-0.16.3/sigmund/utils.py
--rw-r--r--   0        0        0     4228 1970-01-01 00:00:00.000000 sigmund-0.16.3/PKG-INFO
+-rw-r--r--   0        0        0    35147 2024-04-30 15:05:06.434642 sigmund-0.16.5/COPYING
+-rw-r--r--   0        0        0     1017 2024-04-30 15:05:06.434642 sigmund-0.16.5/pyproject.toml
+-rw-r--r--   0        0        0     3037 2024-04-30 15:05:06.434642 sigmund-0.16.5/readme.md
+-rw-r--r--   0        0        0      101 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/__init__.py
+-rw-r--r--   0        0        0     2746 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/attachments.py
+-rw-r--r--   0        0        0     9770 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/config.py
+-rw-r--r--   0        0        0        0 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/database/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/database/encryption.py
+-rw-r--r--   0        0        0    14378 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/database/manager.py
+-rw-r--r--   0        0        0     3213 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/database/models.py
+-rw-r--r--   0        0        0     6331 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/documentation.py
+-rw-r--r--   0        0        0      389 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/forms.py
+-rw-r--r--   0        0        0     2547 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/library.py
+-rw-r--r--   0        0        0    10115 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/messages.py
+-rw-r--r--   0        0        0     1252 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/model/__init__.py
+-rw-r--r--   0        0        0     5297 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/model/_anthropic_model.py
+-rw-r--r--   0        0        0     4756 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/model/_base_model.py
+-rw-r--r--   0        0        0      379 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/model/_dummy_model.py
+-rw-r--r--   0        0        0     2700 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/model/_mistral_model.py
+-rw-r--r--   0        0        0     3428 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/model/_openai_model.py
+-rw-r--r--   0        0        0     2141 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/prompt.py
+-rw-r--r--   0        0        0      160 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/routes/__init__.py
+-rw-r--r--   0        0        0     7298 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/routes/api.py
+-rw-r--r--   0        0        0     5775 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/routes/app.py
+-rw-r--r--   0        0        0     3769 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/routes/google_login.py
+-rw-r--r--   0        0        0     7732 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/routes/subscribe.py
+-rw-r--r--   0        0        0     1494 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/server.py
+-rw-r--r--   0        0        0     9354 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/sigmund.py
+-rw-r--r--   0        0        0     4471 2024-04-30 15:05:06.434642 sigmund-0.16.5/sigmund/static/about.md
+-rw-r--r--   0        0        0  4708018 2024-04-30 15:05:06.442642 sigmund-0.16.5/sigmund/static/background.png
+-rw-r--r--   0        0        0      386 2024-04-30 15:05:06.442642 sigmund-0.16.5/sigmund/static/favicon.svg
+-rw-r--r--   0        0        0     1433 2024-04-30 15:05:06.442642 sigmund-0.16.5/sigmund/static/login.md
+-rw-r--r--   0        0        0     4976 2024-04-30 15:05:06.442642 sigmund-0.16.5/sigmund/static/pygments.css
+-rw-r--r--   0        0        0   708136 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/static/sofa-with-sigmund.png
+-rw-r--r--   0        0        0   684883 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/static/sofa.png
+-rw-r--r--   0        0        0     3428 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/static/terms.md
+-rw-r--r--   0        0        0     1359 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/chat.html
+-rw-r--r--   0        0        0      242 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/footer.html
+-rw-r--r--   0        0        0      574 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/head.html
+-rw-r--r--   0        0        0      244 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/header.html
+-rw-r--r--   0        0        0      329 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/info-page.html
+-rw-r--r--   0        0        0     3739 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/login.html
+-rw-r--r--   0        0        0    10786 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/main.js
+-rw-r--r--   0        0        0    12359 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/menu.html
+-rw-r--r--   0        0        0       80 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/sign-out.html
+-rw-r--r--   0        0        0     6380 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/stylesheet.css.jinja
+-rw-r--r--   0        0        0      531 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/subscribe-error.html
+-rw-r--r--   0        0        0     1555 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/subscribe-now.html
+-rw-r--r--   0        0        0      515 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/templates/subscribe-success.html
+-rw-r--r--   0        0        0      265 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/tools/__init__.py
+-rw-r--r--   0        0        0     2231 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/tools/_base_tool.py
+-rw-r--r--   0        0        0     2920 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/tools/_download.py
+-rw-r--r--   0        0        0     2085 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/tools/_execute_code.py
+-rw-r--r--   0        0        0     1846 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/tools/_read_attachment.py
+-rw-r--r--   0        0        0     2076 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/tools/_search_documentation.py
+-rw-r--r--   0        0        0     1275 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/tools/_search_google_scholar.py
+-rw-r--r--   0        0        0     4358 2024-04-30 15:05:06.446642 sigmund-0.16.5/sigmund/utils.py
+-rw-r--r--   0        0        0     4228 1970-01-01 00:00:00.000000 sigmund-0.16.5/PKG-INFO
```

### Comparing `sigmund-0.16.3/COPYING` & `sigmund-0.16.5/COPYING`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/pyproject.toml` & `sigmund-0.16.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/readme.md` & `sigmund-0.16.5/readme.md`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/attachments.py` & `sigmund-0.16.5/sigmund/attachments.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/config.py` & `sigmund-0.16.5/sigmund/config.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/database/encryption.py` & `sigmund-0.16.5/sigmund/database/encryption.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/database/manager.py` & `sigmund-0.16.5/sigmund/database/manager.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/database/models.py` & `sigmund-0.16.5/sigmund/database/models.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/documentation.py` & `sigmund-0.16.5/sigmund/documentation.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/library.py` & `sigmund-0.16.5/sigmund/library.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/messages.py` & `sigmund-0.16.5/sigmund/messages.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/model/__init__.py` & `sigmund-0.16.5/sigmund/model/__init__.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/model/_anthropic_model.py` & `sigmund-0.16.5/sigmund/model/_anthropic_model.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/model/_base_model.py` & `sigmund-0.16.5/sigmund/model/_base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,12 +106,16 @@
         if not use_async:
             logger.info('predicting multiple without async')
             return [self.get_response(self.invoke(prompt))
                                               for prompt in prompts]
             
         async def wrap_gather():
             tasks = [self.async_invoke(prompt) for prompt in prompts]
-            predictions = await asyncio.gather(*tasks)
+            try:
+                predictions = await asyncio.gather(*tasks)
+            except Exception as e:
+                logger.warning(f'failed to gather predictions: {e}')
+                return []
             return [self.get_response(p) for p in predictions]
             
         logger.info('predicting multiple using async')
         return loop.run_until_complete(wrap_gather())
```

### Comparing `sigmund-0.16.3/sigmund/model/_mistral_model.py` & `sigmund-0.16.5/sigmund/model/_mistral_model.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/model/_openai_model.py` & `sigmund-0.16.5/sigmund/model/_openai_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import json
+import logging
 from .. import config
 from . import BaseModel
 
 
+logger = logging.getLogger('sigmund')
+
+
 class OpenAIModel(BaseModel):
 
     def __init__(self, sigmund, model, **kwargs):
         from openai import Client, AsyncClient
         super().__init__(sigmund, **kwargs)
         self._model = model
         if self._tool_choice not in (None, 'auto'):
```

### Comparing `sigmund-0.16.3/sigmund/prompt.py` & `sigmund-0.16.5/sigmund/prompt.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/routes/api.py` & `sigmund-0.16.5/sigmund/routes/api.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/routes/app.py` & `sigmund-0.16.5/sigmund/routes/app.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/routes/google_login.py` & `sigmund-0.16.5/sigmund/routes/google_login.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,20 +40,25 @@
     # Get authorization code Google sent back to you
     code = request.args.get("code")
     # Find out what URL to hit to get tokens that allow you to ask for
     # things on behalf of a user
     google_provider_cfg = get_google_provider_cfg()
     token_endpoint = google_provider_cfg["token_endpoint"]
     # Prepare and send a request to get tokens! Yay tokens!
-    token_url, headers, body = client.prepare_token_request(
-        token_endpoint,
-        authorization_response=request.url.replace('http:', 'https:'),
-        redirect_url=request.base_url.replace('http:', 'https:'),
-        code=code
-    )
+    try:
+        token_url, headers, body = client.prepare_token_request(
+            token_endpoint,
+            authorization_response=request.url.replace('http:', 'https:'),
+            redirect_url=request.base_url.replace('http:', 'https:'),
+            code=code
+        )
+    except Exception as e:
+        logger.warning(f'failed to prepare token request: {e}')
+        return redirect('/')
+        
     token_response = requests.post(
         token_url,
         headers=headers,
         data=body,
         auth=(config.google_client_id, config.google_client_secret),
     )
     # Parse the tokens!
@@ -79,8 +84,8 @@
                      iterations=100000,
                      backend=default_backend())
     session['encryption_key'] = base64.urlsafe_b64encode(
         kdf.derive(unique_id.encode()))
     user = User(f'{username} (google)')
     login_user(user)
     logger.info(f'initializing encryption key')    
-    return redirect('/')
+    return redirect('/')
```

### Comparing `sigmund-0.16.3/sigmund/routes/subscribe.py` & `sigmund-0.16.5/sigmund/routes/subscribe.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/server.py` & `sigmund-0.16.5/sigmund/server.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/sigmund.py` & `sigmund-0.16.5/sigmund/sigmund.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/static/about.md` & `sigmund-0.16.5/sigmund/static/about.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Sigmund is a powerful, privacy-focused AI assistant (or chatbot). It is a web app that built on state-of-the-art large language models (LLMs).
+Sigmund is a powerful, privacy-focused AI assistant (or chatbot). It is a web app that is built on state-of-the-art large language models (LLMs).
 
 
 [TOC]
 
 
 ## Sigmund is an OpenSesame expert
 
 If OpenSesame-expert mode is enabled (in the menu), Sigmund searches for relevant sections in the documentation of [OpenSesame](https://osdoc.cogsci.nl/), a program for developing psychology and cognitive-neuroscience experiments. Sigmund also receives a set of fixed instructions designed to enhance its general knowledge of OpenSesame. Sigmund subsequently uses this information to answer questions, and to provide links to relevant pages from the documentation. This technique, which is a variation of so-called Retrieval-Augmented Generation, allows Sigmund to answer questions about OpenSesame much better than other chatbots.
 
 Sigmund is especially good at generating code for (Python) inline_script or inline_javascript items. Try it!
 
-<blockquote>
+<blockquote style="white-space:pre-wrap;">
 I want to create a stimulus display in OpenSesame, using a canvas in a Python inline script. It's a bit complex, so please read carefully! There should be:
 
 - A central fixation dot.
 - Six shapes in a circular arrangement around the central dot.
 - One of these shapes, randomly selected, should be a square. The other shapes should be circles.
 - One of these shapes, again randomly selected, should be green. The other shapes should be red.
 - Inside each shape there should be a line segment that is tilted 45 degrees clockwise or counterclockwise.
@@ -36,14 +36,16 @@
 
 Sigmund can search Google Scholar for scientific literature. Try it!
 
 > Do your pupils constrict when you think of something bright, such as a sunny beach? Please base your answer on scientific literature.
 
 Limitation: Sigmund reads abstracts, titles, author lists, etc. but does not spontaneously reads complete articles. To have Sigmund read complete articles, you can either encourage Sigmund to download the article (see below) or upload the article as an attachment yourself.
 
+Limitation: Google Scholar occasionally blocks searches from autonomous agents such as Sigmund, which results in an error message. When this happens, try again later.
+
 
 ### Execute Python and R code
 
 Sigmund can not only write Python and R code, but also execute it. Try it!
 
 > Can you write a Python function that returns the number of words in a sentence? Please also write some test cases and execute them to make sure that the function is correct.
```

### Comparing `sigmund-0.16.3/sigmund/static/background.png` & `sigmund-0.16.5/sigmund/static/background.png`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/static/login.md` & `sigmund-0.16.5/sigmund/static/login.md`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/static/pygments.css` & `sigmund-0.16.5/sigmund/static/pygments.css`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/static/sofa-with-sigmund.png` & `sigmund-0.16.5/sigmund/static/sofa-with-sigmund.png`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/static/sofa.png` & `sigmund-0.16.5/sigmund/static/sofa.png`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/static/terms.md` & `sigmund-0.16.5/sigmund/static/terms.md`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/templates/chat.html` & `sigmund-0.16.5/sigmund/templates/chat.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/templates/head.html` & `sigmund-0.16.5/sigmund/templates/head.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/templates/login.html` & `sigmund-0.16.5/sigmund/templates/login.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/templates/main.js` & `sigmund-0.16.5/sigmund/templates/main.js`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/templates/menu.html` & `sigmund-0.16.5/sigmund/templates/menu.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/templates/stylesheet.css.jinja` & `sigmund-0.16.5/sigmund/templates/stylesheet.css.jinja`

 * *Files 0% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 
 #page-notification a {
     color: #fff;
 }
 
 .message-user {
     color: #00796b;
+    white-space: pre-wrap;
 }
 
 .message-loading {
     color: gray;
 }
 
 .message-loading,
```

### Comparing `sigmund-0.16.3/sigmund/templates/subscribe-error.html` & `sigmund-0.16.5/sigmund/templates/subscribe-error.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/templates/subscribe-now.html` & `sigmund-0.16.5/sigmund/templates/subscribe-now.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/templates/subscribe-success.html` & `sigmund-0.16.5/sigmund/templates/subscribe-success.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/tools/_base_tool.py` & `sigmund-0.16.5/sigmund/tools/_base_tool.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/tools/_download.py` & `sigmund-0.16.5/sigmund/tools/_download.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/tools/_execute_code.py` & `sigmund-0.16.5/sigmund/tools/_execute_code.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/tools/_read_attachment.py` & `sigmund-0.16.5/sigmund/tools/_read_attachment.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/tools/_search_documentation.py` & `sigmund-0.16.5/sigmund/tools/_search_documentation.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/tools/_search_google_scholar.py` & `sigmund-0.16.5/sigmund/tools/_search_google_scholar.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/sigmund/utils.py` & `sigmund-0.16.5/sigmund/utils.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.3/PKG-INFO` & `sigmund-0.16.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmund
-Version: 0.16.3
+Version: 0.16.5
 Summary: AI-based chatbot that provides sensible answers based on documentation
 Keywords: ai,chatbot,llm
 Author-email: Sebastiaan Mathôt <s.mathot@cogsci.nl>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: anthropic
 Requires-Dist: cryptography
```

