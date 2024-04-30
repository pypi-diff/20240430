# Comparing `tmp/fastapi_simple_auth-0.0.1.tar.gz` & `tmp/fastapi_simple_auth-0.0.2.tar.gz`

## Comparing `fastapi_simple_auth-0.0.1.tar` & `fastapi_simple_auth-0.0.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/.env-example
--rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/alembic.ini
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/app.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/requirements.txt
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/alembic/README
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/alembic/env.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/alembic/script.py.mako
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/alembic/versions/9a3f872373f4_initial.py
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/__init__.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/cron.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/crud.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/db.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/envmail.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/exceptions.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/models.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/pub.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/router.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/schemas.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/session.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/settings.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/startup.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/templates.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/verification.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/cli/__init__.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/cli/simpleauth.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/templates/afterlogin.html
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/templates/base.html
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/templates/login.html
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/templates/profile.html
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/templates/recover.html
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/templates/recover_code.html
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/templates/register.html
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/templates/verify-email.html
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/templates/email/change-email.html
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/templates/email/confirm-email.html
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/templates/email/recover.html
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/views/__init__.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/views/login.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/views/profile.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/views/recover.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/views/settingsjs.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/views/signup.py
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/fastapi_simple_auth/views/verify.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/LICENSE
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/README.md
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/.env-example
+-rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/alembic.ini
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/app.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/requirements.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/alembic/README
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/alembic/env.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/alembic/script.py.mako
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/alembic/versions/9a3f872373f4_initial.py
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/__init__.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/cron.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/crud.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/db.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/envmail.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/exceptions.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/models.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/pub.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/router.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/schemas.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/session.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/settings.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/startup.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/templates.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/verification.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/cli/__init__.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/cli/simpleauth.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/templates/afterlogin.html
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/templates/base.html
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/templates/login.html
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/templates/profile.html
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/templates/recover.html
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/templates/recover_code.html
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/templates/register.html
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/templates/verify-email.html
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/templates/email/change-email.html
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/templates/email/confirm-email.html
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/templates/email/recover.html
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/views/__init__.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/views/login.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/views/profile.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/views/recover.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/views/settingsjs.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/views/signup.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/fastapi_simple_auth/views/verify.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/LICENSE
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/README.md
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.2/PKG-INFO
```

### Comparing `fastapi_simple_auth-0.0.1/.env-example` & `fastapi_simple_auth-0.0.2/.env-example`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/alembic.ini` & `fastapi_simple_auth-0.0.2/alembic.ini`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/alembic/env.py` & `fastapi_simple_auth-0.0.2/alembic/env.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/alembic/script.py.mako` & `fastapi_simple_auth-0.0.2/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/alembic/versions/9a3f872373f4_initial.py` & `fastapi_simple_auth-0.0.2/alembic/versions/9a3f872373f4_initial.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/__init__.py` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from .verification import send_verification_signup
 from .templates import template_env
 from .startup import startup
 from .models import User
 from .pub import logged_in_user
 from . import views
 
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
 # to get a string like this run:
 # openssl rand -hex 32
 SECRET_KEY = "09d25e094faa6ca2556c818166b7a9563b93f7099f6f0f4caa6cf63b88e8d3e7"
 ALGORITHM = "HS256"
 ACCESS_TOKEN_EXPIRE_MINUTES = 30
```

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/cron.py` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/cron.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/crud.py` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/crud.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/envmail.py` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/envmail.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/models.py` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/pub.py` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/pub.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/session.py` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/session.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/settings.py` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     code_lifetime: int = 86400
     code_regenerate: int = 30
     
     mail_transport: str = "stdout"
     mail_host: str = "127.0.0.1"
     mail_port: int = 25
     mail_from: str = "NoReply <noreply@example.com>"
-    mail_user: str = None
-    mail_password: str = None
+    mail_user: str | None = None
+    mail_password: str | None = None
     mail_starttls: bool = False
 
     auth_transport: str = "session"
 
     cron_interval: int = 300
 
     afterlogin_url: str = "/"
```

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/verification.py` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/verification.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/cli/simpleauth.py` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/cli/simpleauth.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/templates/base.html` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/templates/base.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/templates/login.html` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/templates/login.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/templates/profile.html` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/templates/profile.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/templates/recover.html` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/templates/recover.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/templates/recover_code.html` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/templates/recover_code.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/templates/register.html` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/templates/register.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/templates/verify-email.html` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/templates/verify-email.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/views/__init__.py` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/views/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/views/login.py` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/views/login.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/views/profile.py` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/views/profile.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/views/recover.py` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/views/recover.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/views/settingsjs.py` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/views/settingsjs.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/views/signup.py` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/views/signup.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/fastapi_simple_auth/views/verify.py` & `fastapi_simple_auth-0.0.2/fastapi_simple_auth/views/verify.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/.gitignore` & `fastapi_simple_auth-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/LICENSE` & `fastapi_simple_auth-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/README.md` & `fastapi_simple_auth-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/pyproject.toml` & `fastapi_simple_auth-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.1/PKG-INFO` & `fastapi_simple_auth-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fastapi-simple-auth
-Version: 0.0.1
+Version: 0.0.2
 Summary: FastAPI simple authentication
 Project-URL: Documentation, https://github.com/yaroslaff/fastapi-simple-auth#readme
 Project-URL: Issues, https://github.com/yaroslaff/fastapi-simple-auth/issues
 Project-URL: Source, https://github.com/yaroslaff/fastapi-simple-auth
 Author-email: Yaroslav Polyakov <yaroslaff@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

