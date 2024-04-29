# Comparing `tmp/hnt_nf_jira_library-0.4.4.tar.gz` & `tmp/hnt_nf_jira_library-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_nf_jira_library-0.4.4.tar", last modified: Fri Apr 26 14:02:25 2024, max compression
+gzip compressed data, was "hnt_nf_jira_library-0.4.5.tar", last modified: Mon Apr 29 23:06:34 2024, max compression
```

## Comparing `hnt_nf_jira_library-0.4.4.tar` & `hnt_nf_jira_library-0.4.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 14:02:25.533250 hnt_nf_jira_library-0.4.4/
--rw-rw-rw-   0        0        0      286 2024-04-26 14:02:25.533250 hnt_nf_jira_library-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.4.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 14:02:25.530208 hnt_nf_jira_library-0.4.4/hnt_nf_jira_library.egg-info/
--rw-rw-rw-   0        0        0      286 2024-04-26 14:02:25.000000 hnt_nf_jira_library-0.4.4/hnt_nf_jira_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1035 2024-04-26 14:02:25.000000 hnt_nf_jira_library-0.4.4/hnt_nf_jira_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 14:02:25.000000 hnt_nf_jira_library-0.4.4/hnt_nf_jira_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-26 14:02:25.000000 hnt_nf_jira_library-0.4.4/hnt_nf_jira_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-26 14:02:25.000000 hnt_nf_jira_library-0.4.4/hnt_nf_jira_library.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-26 14:02:25.399125 hnt_nf_jira_library-0.4.4/nf_jira/
--rw-rw-rw-   0        0        0       41 2024-04-26 13:46:42.000000 hnt_nf_jira_library-0.4.4/nf_jira/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 14:02:25.507256 hnt_nf_jira_library-0.4.4/nf_jira/entities/
--rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/anexo.py
--rw-rw-rw-   0        0        0      131 2024-04-19 19:08:56.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/chave_acesso.py
-drwxrwxrwx   0        0        0        0 2024-04-26 14:02:25.528023 hnt_nf_jira_library-0.4.4/nf_jira/entities/classes/
--rw-rw-rw-   0        0        0     4893 2024-04-19 19:08:56.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/classes/form_jira.py
--rw-rw-rw-   0        0        0     3669 2024-04-26 13:46:42.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/classes/helper.py
--rw-rw-rw-   0        0        0     2019 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/classes/issue_fields.py
--rw-rw-rw-   0        0        0     7637 2024-04-26 13:56:41.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/classes/issue_jira.py
--rw-rw-rw-   0        0        0      774 2024-04-25 17:39:49.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/classes/n8n_domain.py
--rw-rw-rw-   0        0        0     3477 2024-04-26 13:46:42.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/constants.py
--rw-rw-rw-   0        0        0      331 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/dados_basicos_fatura.py
--rw-rw-rw-   0        0        0      145 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/dados_basicos_miro.py
--rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/dados_nfe.py
--rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/detalhe.py
--rw-rw-rw-   0        0        0      234 2024-04-19 19:08:56.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/fatura.py
--rw-rw-rw-   0        0        0      140 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/item.py
--rw-rw-rw-   0        0        0      224 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/itens_fatura.py
--rw-rw-rw-   0        0        0       97 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/jira_info.py
--rw-rw-rw-   0        0        0      448 2024-04-19 19:08:56.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/miro.py
--rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/nfe_sefaz.py
--rw-rw-rw-   0        0        0      360 2024-04-26 13:46:42.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/nota_pedido.py
--rw-rw-rw-   0        0        0      169 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/pagamento.py
--rw-rw-rw-   0        0        0       92 2024-04-13 16:16:55.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/referencia_pedido.py
--rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/sintese_itens.py
--rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.4.4/nf_jira/entities/sintese_miro.py
--rw-rw-rw-   0        0        0    14975 2024-04-26 13:46:42.000000 hnt_nf_jira_library-0.4.4/nf_jira/wrapper_nf_jira.py
--rw-rw-rw-   0        0        0       42 2024-04-26 14:02:25.533250 hnt_nf_jira_library-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0      510 2024-04-26 14:02:08.000000 hnt_nf_jira_library-0.4.4/setup.py
+drwxr-xr-x   0 ipepe      (501) staff       (20)        0 2024-04-29 23:06:34.309058 hnt_nf_jira_library-0.4.5/
+-rw-r--r--   0 ipepe      (501) staff       (20)      276 2024-04-29 23:06:34.308059 hnt_nf_jira_library-0.4.5/PKG-INFO
+-rw-r--r--   0 ipepe      (501) staff       (20)      381 2024-02-29 14:45:46.000000 hnt_nf_jira_library-0.4.5/README.md
+drwxr-xr-x   0 ipepe      (501) staff       (20)        0 2024-04-29 23:06:34.307236 hnt_nf_jira_library-0.4.5/hnt_nf_jira_library.egg-info/
+-rw-r--r--   0 ipepe      (501) staff       (20)      276 2024-04-29 23:06:33.000000 hnt_nf_jira_library-0.4.5/hnt_nf_jira_library.egg-info/PKG-INFO
+-rw-r--r--   0 ipepe      (501) staff       (20)     1035 2024-04-29 23:06:33.000000 hnt_nf_jira_library-0.4.5/hnt_nf_jira_library.egg-info/SOURCES.txt
+-rw-r--r--   0 ipepe      (501) staff       (20)        1 2024-04-29 23:06:33.000000 hnt_nf_jira_library-0.4.5/hnt_nf_jira_library.egg-info/dependency_links.txt
+-rw-r--r--   0 ipepe      (501) staff       (20)       55 2024-04-29 23:06:33.000000 hnt_nf_jira_library-0.4.5/hnt_nf_jira_library.egg-info/requires.txt
+-rw-r--r--   0 ipepe      (501) staff       (20)        8 2024-04-29 23:06:33.000000 hnt_nf_jira_library-0.4.5/hnt_nf_jira_library.egg-info/top_level.txt
+drwxr-xr-x   0 ipepe      (501) staff       (20)        0 2024-04-29 23:06:34.282087 hnt_nf_jira_library-0.4.5/nf_jira/
+-rw-r--r--   0 ipepe      (501) staff       (20)       41 2024-04-26 20:24:37.000000 hnt_nf_jira_library-0.4.5/nf_jira/__init__.py
+drwxr-xr-x   0 ipepe      (501) staff       (20)        0 2024-04-29 23:06:34.303245 hnt_nf_jira_library-0.4.5/nf_jira/entities/
+-rw-r--r--   0 ipepe      (501) staff       (20)       88 2024-04-19 08:27:42.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/anexo.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      126 2024-04-25 16:53:19.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/chave_acesso.py
+drwxr-xr-x   0 ipepe      (501) staff       (20)        0 2024-04-29 23:06:34.306489 hnt_nf_jira_library-0.4.5/nf_jira/entities/classes/
+-rw-r--r--   0 ipepe      (501) staff       (20)     4741 2024-04-25 16:53:19.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/classes/form_jira.py
+-rw-r--r--   0 ipepe      (501) staff       (20)     3583 2024-04-29 23:05:03.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/classes/helper.py
+-rw-r--r--   0 ipepe      (501) staff       (20)     1961 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/classes/issue_fields.py
+-rw-r--r--   0 ipepe      (501) staff       (20)     7448 2024-04-29 23:05:03.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/classes/issue_jira.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      747 2024-04-25 16:53:19.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/classes/n8n_domain.py
+-rw-r--r--   0 ipepe      (501) staff       (20)     3499 2024-04-29 23:05:03.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/constants.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      385 2024-04-29 23:05:03.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/dados_basicos_fatura.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      145 2024-04-29 23:05:03.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/dados_basicos_miro.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      191 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/dados_nfe.py
+-rw-r--r--   0 ipepe      (501) staff       (20)       73 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/detalhe.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      682 2024-04-29 23:05:03.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/fatura.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      225 2024-04-29 23:05:03.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/item.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      278 2024-04-29 23:05:03.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/itens_fatura.py
+-rw-r--r--   0 ipepe      (501) staff       (20)       93 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/jira_info.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      508 2024-04-29 23:05:03.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/miro.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      122 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/nfe_sefaz.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      864 2024-04-29 23:05:03.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/nota_pedido.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      162 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/pagamento.py
+-rw-r--r--   0 ipepe      (501) staff       (20)       89 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/referencia_pedido.py
+-rw-r--r--   0 ipepe      (501) staff       (20)      165 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/sintese_itens.py
+-rw-r--r--   0 ipepe      (501) staff       (20)       75 2024-04-19 08:27:45.000000 hnt_nf_jira_library-0.4.5/nf_jira/entities/sintese_miro.py
+-rw-r--r--   0 ipepe      (501) staff       (20)    15785 2024-04-29 23:05:03.000000 hnt_nf_jira_library-0.4.5/nf_jira/wrapper_nf_jira.py
+-rw-r--r--   0 ipepe      (501) staff       (20)       38 2024-04-29 23:06:34.309128 hnt_nf_jira_library-0.4.5/setup.cfg
+-rw-r--r--   0 ipepe      (501) staff       (20)      493 2024-04-29 23:05:27.000000 hnt_nf_jira_library-0.4.5/setup.py
```

### Comparing `hnt_nf_jira_library-0.4.4/hnt_nf_jira_library.egg-info/SOURCES.txt` & `hnt_nf_jira_library-0.4.5/hnt_nf_jira_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.4/nf_jira/entities/classes/form_jira.py` & `hnt_nf_jira_library-0.4.5/nf_jira/entities/classes/form_jira.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-import requests
-from ..constants import *
-from .helper import JsonHelper
-# from ...wrapper_nf_jira import wrapper_jira
-
-class FormJira:
-# class FormJira(wrapper_jira):
-
-    def __init__(self) -> None:
-        pass
-
-    def get_form_fields(self, issue_key, form_template, debug=False):
-
-        form_data = self._get_form_data(issue_key, form_template)
-        form_fields = self._get_form_fields_data(form_data)
-
-        JsonHelper().save_json(f"FormFields_{issue_key}_{form_template}", form_fields) if debug else None
-
-        return form_fields
-    
-    def get_form_id(self, issue_key, form_template):
-
-        forms_from_issue = self._get_forms_from_issue(issue_key)
-        form_id = self._get_form_id_data(forms_from_issue, form_template)
-
-        return form_id
-    
-    def get_form_jira_keys(self, issue_key, form_template):
-        
-        form_data = self._get_form_data(issue_key, form_template)
-        form_keys = self._get_form_jira_keys(form_data)
-
-        return form_keys
-
-    def _get_form_data(self, issue_key, form_template):
-
-        forms_from_issue = self._get_forms_from_issue(issue_key)
-        form_id = self._get_form_id_data(forms_from_issue, form_template)
-        form_data = self._get_form(form_id, issue_key)
-
-        return form_data
-
-    def _get_forms_from_issue(self, issue_key):
-
-        try:
-            request = requests.get(
-                f"{API_FORM_URL}/{CLOUD_ID}/issue/{issue_key}/form",
-                headers=API_ATLASSIAN_HEADERS,
-                auth=JIRA_AUTH,
-            )
-            request.raise_for_status()
-            data = request.json()
-            
-            return data
-        except requests.exceptions.HTTPError as e:
-            raise Exception(f"Erro ao receber formulario da issue:\n{e}")
-        
-    def _get_form_id_data(self, data, form_template):
-        
-        for form in data:
-            if form.get("formTemplate")['id'] == form_template:
-                form_id = form.get("id")
-
-        return form_id
-    
-    def _get_form(self, form_id, issue_key):
-
-        try:
-            request = requests.get(
-                f"{API_FORM_URL}/{CLOUD_ID}/issue/{issue_key}/form/{form_id}",
-                headers=API_ATLASSIAN_HEADERS,
-                auth=JIRA_AUTH,
-            )
-            request.raise_for_status()
-            data = request.json()
-
-            return data
-        except requests.exceptions.HTTPError as e:
-            raise Exception(f"Erro ao capturar formulario:\n{e}")
-        
-    def _get_form_fields_data(self, data):
-
-        fields_json = {}
-
-        fields_values = data.get('state')['answers']
-        fields_root = data.get('design')['questions']
-        
-        for root in fields_root:
-
-            field_name = fields_root[root].get('questionKey')
-            if fields_values.get(root) is not None:
-                # field_index = list(fields_values.get(root).keys())[0]
-                if "choices" in list(fields_values.get(root).keys()):
-                    field_value = fields_values.get(root)['choices']
-                else:
-                    field_index = list(fields_values.get(root).keys())[0]
-                    field_value = fields_values.get(root)[field_index]
-            else: 
-                field_value = None
-
-            fields_json[field_name] = field_value
-
-        return fields_json
-    
-    def _get_form_jira_keys(self, data):
-        field_keys = {}
-        fields_root = data.get('design')['questions']
-
-        for root in fields_root:
-
-            field_name = fields_root[root].get('questionKey')
-            jira_key = fields_root[root].get('jiraField')
-            field_keys[field_name] = jira_key
-
-        return field_keys
-
-    def update_jira_form(self, issue, data):
-
-        answers_schema = {
-            "1":"cod_nota_pedido",
-            "4":"cod_fatura",
-            "5":"status_liberacao",
-            "6":"data_liberacao",
-            "7":"cod_miro"
-        }
-
-        answers_json = {}
-
-        for answer in answers_schema:
-            answer_label = answers_schema[answer]
-            if answer_label in data:
-                answers_json[answer] = {"text": data[answer_label]}
-
-        answers = { "answers" : answers_json }
-
-        self._save_form_answers(answers, issue["issue_id"], issue["form_id"])
-
-        pass
-    
-    def _save_form_answers(self, answers, issue_id, form_id):
-
-        try:
-            requests.put(
-                f"{API_FORM_URL}/{CLOUD_ID}/issue/{issue_id}/form/{form_id}",
-                headers = API_ATLASSIAN_HEADERS,
-                auth = JIRA_AUTH,
-                json = answers,
-            )
-
-            pass
-
-        except requests.exceptions.HTTPError as e:
+import requests
+from ..constants import *
+from .helper import JsonHelper
+# from ...wrapper_nf_jira import wrapper_jira
+
+class FormJira:
+# class FormJira(wrapper_jira):
+
+    def __init__(self) -> None:
+        pass
+
+    def get_form_fields(self, issue_key, form_template, debug=False):
+
+        form_data = self._get_form_data(issue_key, form_template)
+        form_fields = self._get_form_fields_data(form_data)
+
+        JsonHelper().save_json(f"FormFields_{issue_key}_{form_template}", form_fields) if debug else None
+
+        return form_fields
+    
+    def get_form_id(self, issue_key, form_template):
+
+        forms_from_issue = self._get_forms_from_issue(issue_key)
+        form_id = self._get_form_id_data(forms_from_issue, form_template)
+
+        return form_id
+    
+    def get_form_jira_keys(self, issue_key, form_template):
+        
+        form_data = self._get_form_data(issue_key, form_template)
+        form_keys = self._get_form_jira_keys(form_data)
+
+        return form_keys
+
+    def _get_form_data(self, issue_key, form_template):
+
+        forms_from_issue = self._get_forms_from_issue(issue_key)
+        form_id = self._get_form_id_data(forms_from_issue, form_template)
+        form_data = self._get_form(form_id, issue_key)
+
+        return form_data
+
+    def _get_forms_from_issue(self, issue_key):
+
+        try:
+            request = requests.get(
+                f"{API_FORM_URL}/{CLOUD_ID}/issue/{issue_key}/form",
+                headers=API_ATLASSIAN_HEADERS,
+                auth=JIRA_AUTH,
+            )
+            request.raise_for_status()
+            data = request.json()
+            
+            return data
+        except requests.exceptions.HTTPError as e:
+            raise Exception(f"Erro ao receber formulario da issue:\n{e}")
+        
+    def _get_form_id_data(self, data, form_template):
+        
+        for form in data:
+            if form.get("formTemplate")['id'] == form_template:
+                form_id = form.get("id")
+
+        return form_id
+    
+    def _get_form(self, form_id, issue_key):
+
+        try:
+            request = requests.get(
+                f"{API_FORM_URL}/{CLOUD_ID}/issue/{issue_key}/form/{form_id}",
+                headers=API_ATLASSIAN_HEADERS,
+                auth=JIRA_AUTH,
+            )
+            request.raise_for_status()
+            data = request.json()
+
+            return data
+        except requests.exceptions.HTTPError as e:
+            raise Exception(f"Erro ao capturar formulario:\n{e}")
+        
+    def _get_form_fields_data(self, data):
+
+        fields_json = {}
+
+        fields_values = data.get('state')['answers']
+        fields_root = data.get('design')['questions']
+        
+        for root in fields_root:
+
+            field_name = fields_root[root].get('questionKey')
+            if fields_values.get(root) is not None:
+                # field_index = list(fields_values.get(root).keys())[0]
+                if "choices" in list(fields_values.get(root).keys()):
+                    field_value = fields_values.get(root)['choices']
+                else:
+                    field_index = list(fields_values.get(root).keys())[0]
+                    field_value = fields_values.get(root)[field_index]
+            else: 
+                field_value = None
+
+            fields_json[field_name] = field_value
+
+        return fields_json
+    
+    def _get_form_jira_keys(self, data):
+        field_keys = {}
+        fields_root = data.get('design')['questions']
+
+        for root in fields_root:
+
+            field_name = fields_root[root].get('questionKey')
+            jira_key = fields_root[root].get('jiraField')
+            field_keys[field_name] = jira_key
+
+        return field_keys
+
+    def update_jira_form(self, issue, data):
+
+        answers_schema = {
+            "1":"cod_nota_pedido",
+            "4":"cod_fatura",
+            "5":"status_liberacao",
+            "6":"data_liberacao",
+            "7":"cod_miro"
+        }
+
+        answers_json = {}
+
+        for answer in answers_schema:
+            answer_label = answers_schema[answer]
+            if answer_label in data:
+                answers_json[answer] = {"text": data[answer_label]}
+
+        answers = { "answers" : answers_json }
+
+        self._save_form_answers(answers, issue["issue_id"], issue["form_id"])
+
+        pass
+    
+    def _save_form_answers(self, answers, issue_id, form_id):
+
+        try:
+            requests.put(
+                f"{API_FORM_URL}/{CLOUD_ID}/issue/{issue_id}/form/{form_id}",
+                headers = API_ATLASSIAN_HEADERS,
+                auth = JIRA_AUTH,
+                json = answers,
+            )
+
+            pass
+
+        except requests.exceptions.HTTPError as e:
             raise Exception(f"Erro ao receber anexo Jira:\n{e}")
```

### Comparing `hnt_nf_jira_library-0.4.4/nf_jira/entities/classes/helper.py` & `hnt_nf_jira_library-0.4.5/nf_jira/entities/classes/helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-import json
-from os import getcwd, makedirs, path
-from ..constants import *
-
-class BaseHelper:
-
-    def __init__(self):
-        pass
-
-class JsonHelper(BaseHelper):
-
-    def save_json(self, filename, json_data):
-
-        path_dir = path.join(getcwd(), 'output/json')
-        if not path.exists(path_dir):
-            makedirs(path_dir)
-
-        with open(f"./output/json/{filename}.json", "w", encoding="utf-8") as json_file:
-            json.dump( json_data, json_file, ensure_ascii=False, indent=4)
-
-class JiraFieldsHelper(BaseHelper):
-
-    def remove_null_fields(self, fields):
-        fields_data_without_nulls = {}
-
-        for key, value in fields.items():
-            if value is not None:
-                fields_data_without_nulls[key] = value
-
-        return fields_data_without_nulls
-    
-    def _rename_fields(self, fields):
-        fields = self._fields
-        new_fields_data = {}
-
-        for key, value in self._jira_fields.items():
-            if value in fields:
-                if "text" in fields[value]:
-                    new_value = fields[value].get("text")
-                elif "date" in fields[value]:
-                    new_value = fields[value].get("date")
-                elif "value" in fields[value]:
-                    new_value = fields[value].get("value")
-                else:
-                    new_value = fields[value]
-
-                new_fields_data[key] = new_value
-
-        return new_fields_data
-    
-class GuiandoHelper(BaseHelper):
-        
-    def __init__(self):
-        self._check_sefaz = lambda form_data: form_data[POSSUI_CHAVE_ACESSO][0] == "1"
-        self._check_document_type = lambda document_type: 'nota_fiscal' if document_type == "2" else 'fatura'
-
-    def include_cod_sap_miro(self, cod_sap, miro):
-        miro['referencia_pedido']['numero_pedido'] = cod_sap
-        return miro
-    
-    ## Validar o Form com base no Sefaz
-    def check_guiando_form(self, form_data):
-        check_sefaz = self._check_sefaz(form_data)
-        if check_sefaz: self._check_sefaz_form(form_data)
-        document_type = self._check_document_type(form_data['document_type'][0])
-        self._check_fiscal_form(form_data) if document_type == 'nota_fiscal' else self._check_fatura_form(form_data)
-        self._check_required_form(form_data)
-        pass
-
-    def _check_sefaz_form(self, form_data):
-        for sefaz_field in SEFAZ_FIELDS:
-            if sefaz_field not in form_data: raise KeyError(f"ERRO - O campo {sefaz_field} não foi enviado.")
-            if form_data[sefaz_field] is None or form_data[sefaz_field] == "" : raise KeyError(f"ERRO - O campo {sefaz_field} está vazio.")
-        pass
-
-    def _check_fiscal_form(self, form_data):
-        if 'nro_nota_fiscal' not in form_data: raise KeyError(f"ERRO - O Campo {'nro_nota_fiscal'} não foi enviado.")
-        if form_data['nro_nota_fiscal'] is None or form_data['nro_nota_fiscal'] == "": raise KeyError(f"ERRO - O Campo {'nro_nota_fiscal'} está vazio.")
-        pass
-
-    def _check_fatura_form(self, form_data):
-        if 'nro_fatura' not in form_data: raise KeyError(f"ERRO - O Campo {'nro_fatura'} não foi enviado.")
-        if form_data['nro_fatura'] is None or form_data['nro_fatura'] == "": raise KeyError(f"ERRO - O Campo {'nro_fatura'} está vazio.")
-        pass
-
-    def _check_required_form(self, form_data):
-        for field in form_data:
-            if field not in OPTIONAL_FIELDS and field not in SEFAZ_FIELDS:
-                if form_data[field] is None or form_data[field] == "":raise KeyError(f"ERRO - O Campo {field} está vazio")
+import json
+from os import getcwd, makedirs, path
+from ..constants import *
+
+class BaseHelper:
+
+    def __init__(self):
+        pass
+
+class JsonHelper(BaseHelper):
+
+    def save_json(self, filename, json_data):
+
+        path_dir = path.join(getcwd(), 'output', 'json')
+        if not path.exists(path_dir):
+            makedirs(path_dir)
+
+        with open(f"./output/json/{filename}.json", "w", encoding="utf-8") as json_file:
+            json.dump( json_data, json_file, ensure_ascii=False, indent=4)
+
+class JiraFieldsHelper(BaseHelper):
+
+    def remove_null_fields(self, fields):
+        fields_data_without_nulls = {}
+
+        for key, value in fields.items():
+            if value is not None:
+                fields_data_without_nulls[key] = value
+
+        return fields_data_without_nulls
+    
+    def _rename_fields(self, fields):
+        fields = self._fields
+        new_fields_data = {}
+
+        for key, value in self._jira_fields.items():
+            if value in fields:
+                if "text" in fields[value]:
+                    new_value = fields[value].get("text")
+                elif "date" in fields[value]:
+                    new_value = fields[value].get("date")
+                elif "value" in fields[value]:
+                    new_value = fields[value].get("value")
+                else:
+                    new_value = fields[value]
+
+                new_fields_data[key] = new_value
+
+        return new_fields_data
+    
+class GuiandoHelper(BaseHelper):
+        
+    def __init__(self):
+        self._check_sefaz = lambda form_data: form_data[POSSUI_CHAVE_ACESSO][0] == "1"
+        self._check_document_type = lambda document_type: 'nota_fiscal' if document_type == "2" else 'fatura'
+
+    def include_cod_sap_miro(self, cod_sap, miro):
+        miro['referencia_pedido']['numero_pedido'] = cod_sap
+        return miro
+    
+    ## Validar o Form com base no Sefaz
+    def check_guiando_form(self, form_data):
+        check_sefaz = self._check_sefaz(form_data)
+        if check_sefaz: self._check_sefaz_form(form_data)
+        document_type = self._check_document_type(form_data['document_type'][0])
+        self._check_fiscal_form(form_data) if document_type == 'nota_fiscal' else self._check_fatura_form(form_data)
+        self._check_required_form(form_data)
+        pass
+
+    def _check_sefaz_form(self, form_data):
+        for sefaz_field in SEFAZ_FIELDS:
+            if sefaz_field not in form_data: raise KeyError(f"ERRO - O campo {sefaz_field} não foi enviado.")
+            if form_data[sefaz_field] is None or form_data[sefaz_field] == "" : raise KeyError(f"ERRO - O campo {sefaz_field} está vazio.")
+        pass
+
+    def _check_fiscal_form(self, form_data):
+        if 'nro_nota_fiscal' not in form_data: raise KeyError(f"ERRO - O Campo {'nro_nota_fiscal'} não foi enviado.")
+        if form_data['nro_nota_fiscal'] is None or form_data['nro_nota_fiscal'] == "": raise KeyError(f"ERRO - O Campo {'nro_nota_fiscal'} está vazio.")
+        pass
+
+    def _check_fatura_form(self, form_data):
+        if 'nro_fatura' not in form_data: raise KeyError(f"ERRO - O Campo {'nro_fatura'} não foi enviado.")
+        if form_data['nro_fatura'] is None or form_data['nro_fatura'] == "": raise KeyError(f"ERRO - O Campo {'nro_fatura'} está vazio.")
+        pass
+
+    def _check_required_form(self, form_data):
+        for field in form_data:
+            if field not in OPTIONAL_FIELDS and field not in SEFAZ_FIELDS:
+                if form_data[field] is None or form_data[field] == "":raise KeyError(f"ERRO - O Campo {field} está vazio")
         pass
```

### Comparing `hnt_nf_jira_library-0.4.4/nf_jira/entities/classes/issue_fields.py` & `hnt_nf_jira_library-0.4.5/nf_jira/entities/classes/issue_fields.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from .helper import JsonHelper, JiraFieldsHelper
-from ..constants import *
-
-class IssueFields:
-
-    def get_fields_by_form_and_jira(self, form_jira_keys, form_fields, jira_fields, debug=False):
-
-        
-        fields = self._generate_fields(form_jira_keys)
-        fields_from_jira_keys = self._get_issue_fields_data_from_jira_keys(form_jira_keys, jira_fields)
-        JiraFieldsHelper().remove_null_fields(fields_from_jira_keys)
-        JiraFieldsHelper().remove_null_fields(form_fields)
-
-        self._append_jira_fields(fields_from_jira_keys, fields)
-        self._append_form_fields(form_fields, fields)
-
-        JsonHelper().save_json(f'Fields_From_Keys_{ISSUE_KEY}',fields) if debug else None
-        return fields
-
-    def _get_issue_fields_data_from_jira_keys(self, form_jira_keys, jira_fields):
-
-        jira_fields_from_keys = {}
-
-        for field_key in form_jira_keys:
-
-            jira_key = form_jira_keys[field_key]
-    
-            if jira_key is not None:
-                field_value = jira_fields[jira_key]
-                if 'value' in field_value:
-                    field_value = field_value['value']
-            else:
-                field_value = None
-
-            jira_fields_from_keys[field_key] = field_value if field_value else None
-
-        return jira_fields_from_keys
-    
-    def _append_jira_fields(self, jira_fields_from_keys, fields):
-
-        for jira_field in jira_fields_from_keys:
-            fields[jira_field] = jira_fields_from_keys[jira_field]  if jira_fields_from_keys[jira_field] is not None else fields[jira_field]
-
-        pass
-
-    def _append_form_fields(self, form_fields, fields):
-
-        for form_field in form_fields:
-            fields[form_field] = form_fields[form_field] if form_fields[form_field] is not None else fields[form_field]
-
-        pass
-
-    def _generate_fields(self, fields_keys):
-
-        fields = {}
-        for key in fields_keys:
-            fields[key] = None
-
+from .helper import JsonHelper, JiraFieldsHelper
+from ..constants import *
+
+class IssueFields:
+
+    def get_fields_by_form_and_jira(self, form_jira_keys, form_fields, jira_fields, debug=False):
+
+        
+        fields = self._generate_fields(form_jira_keys)
+        fields_from_jira_keys = self._get_issue_fields_data_from_jira_keys(form_jira_keys, jira_fields)
+        JiraFieldsHelper().remove_null_fields(fields_from_jira_keys)
+        JiraFieldsHelper().remove_null_fields(form_fields)
+
+        self._append_jira_fields(fields_from_jira_keys, fields)
+        self._append_form_fields(form_fields, fields)
+
+        JsonHelper().save_json(f'Fields_From_Keys_{ISSUE_KEY}',fields) if debug else None
+        return fields
+
+    def _get_issue_fields_data_from_jira_keys(self, form_jira_keys, jira_fields):
+
+        jira_fields_from_keys = {}
+
+        for field_key in form_jira_keys:
+
+            jira_key = form_jira_keys[field_key]
+    
+            if jira_key is not None:
+                field_value = jira_fields[jira_key]
+                if 'value' in field_value:
+                    field_value = field_value['value']
+            else:
+                field_value = None
+
+            jira_fields_from_keys[field_key] = field_value if field_value else None
+
+        return jira_fields_from_keys
+    
+    def _append_jira_fields(self, jira_fields_from_keys, fields):
+
+        for jira_field in jira_fields_from_keys:
+            fields[jira_field] = jira_fields_from_keys[jira_field]  if jira_fields_from_keys[jira_field] is not None else fields[jira_field]
+
+        pass
+
+    def _append_form_fields(self, form_fields, fields):
+
+        for form_field in form_fields:
+            fields[form_field] = form_fields[form_field] if form_fields[form_field] is not None else fields[form_field]
+
+        pass
+
+    def _generate_fields(self, fields_keys):
+
+        fields = {}
+        for key in fields_keys:
+            fields[key] = None
+
         return fields
```

### Comparing `hnt_nf_jira_library-0.4.4/nf_jira/entities/classes/issue_jira.py` & `hnt_nf_jira_library-0.4.5/nf_jira/entities/classes/issue_jira.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,220 +1,220 @@
-import json
-from os import getcwd, makedirs, path
-import requests
-from ..constants import *
-from .helper import JsonHelper, JiraFieldsHelper
-
-
-class IssueJira:
-
-    def get_issue(self, issue_key, debug=False):
-        issue = self._get_issue_data(issue_key)
-        JsonHelper().save_json(f'Issue_{issue_key}',issue) if debug else None
-
-        return issue
-    
-    def get_issue_fields_data(self, issue_key, debug=False):
-
-        issue = self._get_issue_data(issue_key)
-        issue_fields = self._get_issue_fields(issue)
-        
-        JsonHelper().save_json(f'Issue_Fields_{issue_key}',issue_fields) if debug else None
-        issue_fields_min = JiraFieldsHelper().remove_null_fields(issue_fields)
-
-        return issue_fields_min
-
-    def _get_issue_data(self, issue_key):
-        try:
-            request = requests.get(
-                f"{API_ISSUE_URL}/issue/{issue_key}",
-                # f"{API_ISSUE_URL}/{CLOUD_ID}/issue/{issue_key}",
-                headers=API_HEADERS,
-                auth=JIRA_AUTH,
-            )
-            request.raise_for_status()
-            data = request.json()
-
-            return data
-        except requests.exceptions.HTTPError as e:
-            raise Exception(f"Erro ao receber dados da issue:\n{e}")
-        
-    def _get_issue_fields(self, issue):
-
-        jira_fields = issue.get('fields')
-        return jira_fields
-    
-
-        
-class AttachmentJira:
-
-    def get_attachment(self, issue, is_pdf=False):
-
-        self._check_issue_attachment(issue)
-        attachments_ids = self._get_attachment_id(issue)
-        attachment = {}
-        for attachment_key in attachments_ids:
-            attachments_from_issue = self._get_attachments_from_issue(attachment_key)
-            if attachments_from_issue:
-                attachment = attachments_from_issue
-
-        
-        return attachment
-        
-    def _check_issue_attachment(self, issue):
-        if issue.get("fields")["attachment"] is None:
-            raise Exception("Could not find attachment")
-        
-    def _get_attachments_from_issue(self, attachment_key):
-        try:
-            request = requests.get(
-                f"{API_ISSUE_URL}/attachment/content/{attachment_key}",
-                headers=API_ATTACHMENT_HEADERS,
-                auth=JIRA_AUTH,
-            )
-            request.raise_for_status()
-            check_pdf = self._check_pdf_attachment_request(request)
-            attachment_data = request.json() if not check_pdf else None
-
-            return attachment_data
-
-        except requests.exceptions.HTTPError as e:
-            raise Exception(f"Erro ao receber anexo Jira:\n{e}")
-        
-    def _check_pdf_attachment_request(self, request):
-        return True if "application/pdf" in request.headers.get("Content-Type", "") else False
-        
-    def _check_pdf_attachment_list(self, attachment):
-        if 'mimeType' in attachment:
-            return True if "application/pdf" in attachment['mimeType'] else False
-        return False
-    
-    def _get_attachment_id(self, issue):
-        attachment_ids = []
-
-        for attachment in issue.get("fields")["attachment"]:
-            attachment_ids.append(attachment["id"])
-
-        return attachment_ids
-    
-    def download_attachments(self, issue_data):
-
-        attachment_list = self._get_attachment_list(issue_data)
-        donwload_list = []
-
-        for attachment in attachment_list:
-            attachment_params = self._get_download_attachment_params(attachment)
-            check_pdf = self._check_pdf_attachment_list(attachment)
-            if check_pdf:
-                donwload_path = self._download_attachment(attachment_params, DEST_PATH) if check_pdf else None
-                download_path_without_filename, filename = os.path.split(donwload_path)
-                donwload_list.append({
-                    "path": download_path_without_filename,
-                    "filename": filename
-                })
-
-        return donwload_list
-
-    def _get_attachment_list(self, issue_data):
-
-        attachment_list = []
-
-        for attachment in issue_data.get("fields")["attachment"]:
-            attachment_list.append(attachment)
-
-        return attachment_list
-
-    def _get_download_attachment_params(self, attachment):
-        attachment_params = {
-            "filename": attachment['filename'],
-            'content': attachment['content']
-        }
-        return attachment_params
-    
-    def _download_attachment(self, attachment_params, dest_path):
-        try:
-            res = requests.get(
-                attachment_params['content'],
-                timeout=10,
-                auth=JIRA_AUTH,
-                allow_redirects=True)
-            res.raise_for_status()
-            if not path.exists(dest_path):
-                makedirs(dest_path)
-            dest_path_filename = path.join(dest_path, attachment_params['filename'])
-            open(dest_path_filename, 'wb').write(res.content)
-            return dest_path_filename
-        
-        except requests.exceptions.HTTPError as e:
-            raise Exception(f"Erro ao baixar anexo Jira:\n{e}")
-    
-class TransitionJira:
-
-    def post_transition(self, transition_id, issue_key):
-
-        self._post_transition(transition_id, issue_key)
-        pass
-
-    def _post_transition(self, transition_id, issue_key):
-
-        payload = json.dumps(
-            {
-                "transition": {"id": transition_id},
-                "update": {"comment": []},
-            }
-        )
-        try:
-            res = requests.post(
-                f"{API_ISSUE_URL}/issue/{issue_key}/transitions",
-                auth=JIRA_AUTH,
-                headers=API_HEADERS,
-                data=payload,
-            )
-            res.raise_for_status()
-            pass
-        except requests.exceptions.HTTPError as e:
-            raise Exception(f"Erro ao alterar transição da issue:\n{e}")    
-        
-class CommentJira:
-
-    def add_comment(self, issue_key, comment):
-
-        self._add_comment(issue_key, comment)
-        pass
-
-    def _add_comment(self, issue_key, message):
-
-        try:
-            payload = json.dumps(
-                {
-                    "body": {
-                        "content": [
-                            {
-                                "content": [
-                                    {
-                                        "type": "emoji",
-                                        "attrs": {
-                                            "shortName": ":robot:",
-                                            "id": "1f916",
-                                            "text": "🤖",
-                                        },
-                                    },
-                                    {"text": f" {message}", "type": "text"},
-                                ],
-                                "type": "paragraph",
-                            }
-                        ],
-                        "type": "doc",
-                        "version": 1,
-                    }
-                }
-            )
-            res = requests.post(
-                f"{API_ISSUE_URL}/issue/{issue_key}/comment",
-                auth=JIRA_AUTH,
-                headers=API_HEADERS,
-                data=payload,
-            )
-            res.raise_for_status()
-        except requests.exceptions.HTTPError as e:
-            raise Exception(f"Erro ao enviar comentario para issue:\n{e}")
+import json
+from os import getcwd, makedirs, path
+import requests
+from ..constants import *
+from .helper import JsonHelper, JiraFieldsHelper
+
+
+class IssueJira:
+
+    def get_issue(self, issue_key, debug=False):
+        issue = self._get_issue_data(issue_key)
+        JsonHelper().save_json(f'Issue_{issue_key}',issue) if debug else None
+
+        return issue
+    
+    def get_issue_fields_data(self, issue_key, debug=False):
+
+        issue = self._get_issue_data(issue_key)
+        issue_fields = self._get_issue_fields(issue)
+        
+        JsonHelper().save_json(f'Issue_Fields_{issue_key}',issue_fields) if debug else None
+        issue_fields_min = JiraFieldsHelper().remove_null_fields(issue_fields)
+
+        return issue_fields_min
+
+    def _get_issue_data(self, issue_key):
+        try:
+            request = requests.get(
+                f"{API_ISSUE_URL}/issue/{issue_key}",
+                # f"{API_ISSUE_URL}/{CLOUD_ID}/issue/{issue_key}",
+                headers=API_HEADERS,
+                auth=JIRA_AUTH,
+            )
+            request.raise_for_status()
+            data = request.json()
+
+            return data
+        except requests.exceptions.HTTPError as e:
+            raise Exception(f"Erro ao receber dados da issue:\n{e}")
+        
+    def _get_issue_fields(self, issue):
+
+        jira_fields = issue.get('fields')
+        return jira_fields
+    
+
+        
+class AttachmentJira:
+
+    def get_attachment(self, issue, is_pdf=False):
+
+        self._check_issue_attachment(issue)
+        attachments_ids = self._get_attachment_id(issue)
+        attachment = {}
+        for attachment_key in attachments_ids:
+            attachments_from_issue = self._get_attachments_from_issue(attachment_key)
+            if attachments_from_issue:
+                attachment = attachments_from_issue
+
+        
+        return attachment
+        
+    def _check_issue_attachment(self, issue):
+        if issue.get("fields")["attachment"] is None:
+            raise Exception("Could not find attachment")
+        
+    def _get_attachments_from_issue(self, attachment_key):
+        try:
+            request = requests.get(
+                f"{API_ISSUE_URL}/attachment/content/{attachment_key}",
+                headers=API_ATTACHMENT_HEADERS,
+                auth=JIRA_AUTH,
+            )
+            request.raise_for_status()
+            check_pdf = self._check_pdf_attachment_request(request)
+            attachment_data = json.loads(request.text.replace('\n','\\n')) if not check_pdf else None
+
+            return attachment_data
+
+        except requests.exceptions.HTTPError as e:
+            raise Exception(f"Erro ao receber anexo Jira:\n{e}")
+        
+    def _check_pdf_attachment_request(self, request):
+        return True if "application/pdf" in request.headers.get("Content-Type", "") else False
+        
+    def _check_pdf_attachment_list(self, attachment):
+        if 'mimeType' in attachment:
+            return True if "application/pdf" in attachment['mimeType'] else False
+        return False
+    
+    def _get_attachment_id(self, issue):
+        attachment_ids = []
+
+        for attachment in issue.get("fields")["attachment"]:
+            attachment_ids.append(attachment["id"])
+
+        return attachment_ids
+    
+    def download_attachments(self, issue_data):
+
+        attachment_list = self._get_attachment_list(issue_data)
+        donwload_list = []
+
+        for attachment in attachment_list:
+            attachment_params = self._get_download_attachment_params(attachment)
+            check_pdf = self._check_pdf_attachment_list(attachment)
+            if check_pdf:
+                donwload_path = self._download_attachment(attachment_params, DEST_PATH) if check_pdf else None
+                download_path_without_filename, filename = os.path.split(donwload_path)
+                donwload_list.append({
+                    "path": download_path_without_filename,
+                    "filename": filename
+                })
+
+        return donwload_list
+
+    def _get_attachment_list(self, issue_data):
+
+        attachment_list = []
+
+        for attachment in issue_data.get("fields")["attachment"]:
+            attachment_list.append(attachment)
+
+        return attachment_list
+
+    def _get_download_attachment_params(self, attachment):
+        attachment_params = {
+            "filename": attachment['filename'],
+            'content': attachment['content']
+        }
+        return attachment_params
+    
+    def _download_attachment(self, attachment_params, dest_path):
+        try:
+            res = requests.get(
+                attachment_params['content'],
+                timeout=10,
+                auth=JIRA_AUTH,
+                allow_redirects=True)
+            res.raise_for_status()
+            if not path.exists(dest_path):
+                makedirs(dest_path)
+            dest_path_filename = path.join(dest_path, attachment_params['filename'])
+            open(dest_path_filename, 'wb').write(res.content)
+            return dest_path_filename
+        
+        except requests.exceptions.HTTPError as e:
+            raise Exception(f"Erro ao baixar anexo Jira:\n{e}")
+    
+class TransitionJira:
+
+    def post_transition(self, transition_id, issue_key):
+
+        self._post_transition(transition_id, issue_key)
+        pass
+
+    def _post_transition(self, transition_id, issue_key):
+
+        payload = json.dumps(
+            {
+                "transition": {"id": transition_id},
+                "update": {"comment": []},
+            }
+        )
+        try:
+            res = requests.post(
+                f"{API_ISSUE_URL}/issue/{issue_key}/transitions",
+                auth=JIRA_AUTH,
+                headers=API_HEADERS,
+                data=payload,
+            )
+            res.raise_for_status()
+            pass
+        except requests.exceptions.HTTPError as e:
+            raise Exception(f"Erro ao alterar transição da issue:\n{e}")    
+        
+class CommentJira:
+
+    def add_comment(self, issue_key, comment):
+
+        self._add_comment(issue_key, comment)
+        pass
+
+    def _add_comment(self, issue_key, message):
+
+        try:
+            payload = json.dumps(
+                {
+                    "body": {
+                        "content": [
+                            {
+                                "content": [
+                                    {
+                                        "type": "emoji",
+                                        "attrs": {
+                                            "shortName": ":robot:",
+                                            "id": "1f916",
+                                            "text": "🤖",
+                                        },
+                                    },
+                                    {"text": f" {message}", "type": "text"},
+                                ],
+                                "type": "paragraph",
+                            }
+                        ],
+                        "type": "doc",
+                        "version": 1,
+                    }
+                }
+            )
+            res = requests.post(
+                f"{API_ISSUE_URL}/issue/{issue_key}/comment",
+                auth=JIRA_AUTH,
+                headers=API_HEADERS,
+                data=payload,
+            )
+            res.raise_for_status()
+        except requests.exceptions.HTTPError as e:
+            raise Exception(f"Erro ao enviar comentario para issue:\n{e}")
```

### Comparing `hnt_nf_jira_library-0.4.4/nf_jira/entities/classes/n8n_domain.py` & `hnt_nf_jira_library-0.4.5/nf_jira/entities/classes/n8n_domain.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import requests
-from ..constants import *
-
-class N8NDomain:
-
-    def get_nf_domain(self, type, cnpj):
-
-        n8n_data = self._get_nf_domain_data(cnpj, type)
-        return n8n_data
-
-    def _get_nf_domain_data(self, cnpj, type):
-
-        try:
-            domain_request = requests.get(
-                f"{API_DOMAIN_N8N_URL}/{'fornecedores' if type == 'fornecedor' else 'centros'}?cnpj={cnpj}",
-                auth=N8N_AUTH,
-            )
-            domain_request.raise_for_status()
-            domain_data = domain_request.json()
-
-            if not domain_data:
-                raise Exception("Could not find domain")
-
-        except Exception as e:
-            raise Exception(f"Erro ao receber {type}:\n{e}")
-
-        return domain_data
+import requests
+from ..constants import *
+
+class N8NDomain:
+
+    def get_nf_domain(self, type, cnpj):
+
+        n8n_data = self._get_nf_domain_data(cnpj, type)
+        return n8n_data
+
+    def _get_nf_domain_data(self, cnpj, type):
+
+        try:
+            domain_request = requests.get(
+                f"{API_DOMAIN_N8N_URL}/{'fornecedores' if type == 'fornecedor' else 'centros'}?cnpj={cnpj}",
+                auth=N8N_AUTH,
+            )
+            domain_request.raise_for_status()
+            domain_data = domain_request.json()
+
+            if not domain_data:
+                raise Exception("Could not find domain")
+
+        except Exception as e:
+            raise Exception(f"Erro ao receber {type}:\n{e}")
+
+        return domain_data
```

### Comparing `hnt_nf_jira_library-0.4.4/nf_jira/entities/constants.py` & `hnt_nf_jira_library-0.4.5/nf_jira/entities/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,112 +1,115 @@
-import os
-
-#PATH
-DEST_PATH = os.path.join(os.getcwd(), "output\pdf")
-
-#Constant N8N
-N8N_AUTH = (os.getenv("N8N_USERNAME"), os.getenv("N8N_PASSWORD"))
-API_DOMAIN_N8N_URL = os.getenv("DOMAIN_URL")
-FORNECEDOR_N8N_DOMAIN = "fornecedor"
-CENTRO_N8N_DOMAIN = "centro"
-
-# Constantes dos ID's de Formulario
-FORM_TEMPLATE_AUTOMACAO = "910a886b-701a-490d-8b02-708b6c2d9881"
-FORM_TEMPLATE_COMPLEMENTO = "720b4c69-9d84-4f08-930e-1d6c22805f71"
-
-# Constants Jira
-JIRA_AUTH = (os.getenv("USER"), os.getenv("ACCESS_TOKEN"))
-API_ISSUE_URL = os.getenv("ISSUE_URL")
-API_FORM_URL = os.getenv("FORM_URL")
-CLOUD_ID = os.getenv("CLOUD_ID")
-
-#Constantes de Validação
-OPTIONAL_FIELDS = [
-    "nro_fatura",
-    "nro_nota_fiscal",
-    "valor_liquido",
-    "juros",
-    "data_leitura_atual",
-    "data_leitura_anterior"
-]
-
-SEFAZ_FIELDS = [
-    "data_autorizacao",
-    "hora_autorizacao",
-    "protocolo_autorizacao",
-    "chave_acesso"
-]
-
-FISCAL_FIELDS = [
-    "InvoiceNumber"
-]
-
-FATURA_FIELDS = [
-    "SupplierInvoiceNumber"
-]
-
-API_HEADERS = {
-                "Accept": "application/json",
-                "Content-Type": "application/json",
-              }
-
-API_ATTACHMENT_HEADERS = {
-                            "Accept": "*/*",
-                         }
-
-API_ATLASSIAN_HEADERS = {
-                            "Accept": "application/json",
-                            "X-ExperimentalApi": "opt-in",
-                        }
-
-#Test Constants
-ISSUE_KEY = "GHN-487"
-TRASITION_PEDIDO_CRIADO = '241'
-TRASITION_REVISAR_ERRO  = '231'
-FORM_COMPLEMENTO_ID = "f1671ecd-fc44-418f-b6e3-88d774a4b0d4"
-FORM_AUTOMACAO_ID = "e6214bb3-eafc-4de8-ad5a-c8b387346c3e"
-STATUS_LIBERADO = "2"
-STATUS_BLOQUEADO = "1"
-
-# # Constantes do Anexo Json
-ID_DO_LOCATÁRIO = "TenantId"
-NOME_DA_INTEGRAÇÃO = "IntegrationName"
-NOME_DO_USUÁRIO = "UserName"
-EMAIL_DO_USUÁRIO = "UserEmail"
-ID_DA_FATURA = "InvoiceId"
-NÚMERO_DA_FATURA_DO_APLICATIVO = "AplicationInvoiceNumber"
-CNPJ_DO_FORNECEDOR = "SupplierCnpj"
-RAZÃO_SOCIAL_DO_FORNECEDOR = "SupplierCorporateName"
-CNPJ_DO_CLIENTE = "ClientCnpj"
-RAZÃO_SOCIAL_DO_CLIENTE = "ClientCorporateName"
-ENDEREÇO_DO_FORNECEDOR = "SupplierAddress"
-ENDEREÇO_DO_CLIENTE = "ClientAddress"
-DATA_DE_VENCIMENTO = "DueDate"
-DATA_DE_EMISSÃO = "DateOfIssue"
-DATA_DE_REFERÊNCIA = "ReferenceDate"
-DATA_DE_REGISTRO = "DateRegister"
-VALOR_TOTAL_DA_FATURA = "TotalInvoiceAmount"
-VALOR_BRUTO_DA_FATURA = "GrossInvoiceValue"
-CÓDIGO_DE_BARRAS = "BarCode"
-NÚMERO_DA_FATURA = "InvoiceNumber"
-CHAVE_DE_ACESSO_DA_FATURA = "InvoiceAccessKey"
-NÚMERO_DA_FATURA_DO_FORNECEDOR = "SupplierInvoiceNumber"
-CÓDIGO_DE_DEBITO_AUTOMÁTICO = "AutomaticDebitCode"
-INFORMAÇÃO_DA_FATURA = "InvoiceInformation"
-OBSERVAÇÃO_DA_FATURA = "InvoiceObservation"
-NOME_DO_FORNECEDOR = "SupplierName"
-NÚMERO_DO_CONTRATO = "ContractNumber"
-ID_DO_CONTRATO = "ContractId"
-STATUS_DO_CONTRATO = "ContractStatus"
-STATUS_DA_FATURA = "InvoiceStatus"
-LOCALIZAÇÃO_DO_CONTRATO = "ContractLocation"
-VERTICAL_DO_FORNECEDOR = "SupplierVertical"
-PROTOCOLO_DE_LANÇAMENTO = "launchProtocol"
-SERVIÇOS_DA_FATURA = "InvoiceServices"
-IMPOSTOS = "Taxes"
-CAMPOS_CUSTOMIZADOS = "CustomFields"
-ALOCAÇÕES_DE_CUSTO = "CostAllocations"
-ARQUIVOS_DA_FATURA = "InvoiceFiles"
-COMPLEMENTO_DE_ÁGUA = "WaterComplement"
-COMPLEMENTO_DE_ENERGIA = "EnergyComplement"
-COMPLEMENTO_DE_GÁS = "GasComplement"
+import os
+
+#PATH
+DEST_PATH = os.path.join(os.getcwd(), "output", "pdf")
+
+#Constant N8N
+N8N_AUTH = (os.getenv("N8N_USERNAME"), os.getenv("N8N_PASSWORD"))
+API_DOMAIN_N8N_URL = os.getenv("DOMAIN_URL")
+FORNECEDOR_N8N_DOMAIN = "fornecedor"
+CENTRO_N8N_DOMAIN = "centro"
+
+# Constantes dos ID's de Formulario
+FORM_TEMPLATE_AUTOMACAO = "910a886b-701a-490d-8b02-708b6c2d9881"
+FORM_TEMPLATE_COMPLEMENTO = "720b4c69-9d84-4f08-930e-1d6c22805f71"
+
+# Constants Jira
+JIRA_AUTH = (os.getenv("USER"), os.getenv("ACCESS_TOKEN"))
+API_ISSUE_URL = os.getenv("ISSUE_URL")
+API_FORM_URL = os.getenv("FORM_URL")
+CLOUD_ID = os.getenv("CLOUD_ID")
+
+#Constantes de Validação
+OPTIONAL_FIELDS = [
+    "nro_fatura",
+    "nro_nota_fiscal",
+    "valor_liquido",
+    "juros",
+    "data_leitura_atual",
+    "data_leitura_anterior"
+]
+
+SEFAZ_FIELDS = [
+    "data_autorizacao",
+    "hora_autorizacao",
+    "protocolo_autorizacao",
+    "chave_acesso"
+]
+
+FISCAL_FIELDS = [
+    "InvoiceNumber"
+]
+
+FATURA_FIELDS = [
+    "SupplierInvoiceNumber"
+]
+
+API_HEADERS = {
+                "Accept": "application/json",
+                "Content-Type": "application/json",
+              }
+
+API_ATTACHMENT_HEADERS = {
+                            "Accept": "*/*",
+                         }
+
+API_ATLASSIAN_HEADERS = {
+                            "Accept": "application/json",
+                            "X-ExperimentalApi": "opt-in",
+                        }
+
+#Test Constants
+ISSUE_KEY = "GHN-487"
+TRASITION_PEDIDO_CRIADO = '241'
+TRASITION_REVISAR_ERRO  = '231'
+FORM_COMPLEMENTO_ID = "f1671ecd-fc44-418f-b6e3-88d774a4b0d4"
+FORM_AUTOMACAO_ID = "e6214bb3-eafc-4de8-ad5a-c8b387346c3e"
+STATUS_LIBERADO = "2"
+STATUS_BLOQUEADO = "1"
+# Jira Form Nota de Pedido
+VALOR_LIQUIDO_DA_FATURA = "valor_liquido"
+JUROS_DA_FATURA = "juro"
+CEM_PORCENTO_DO_VALOR_BRUTO = 100.00
+# # Constantes do Anexo Json
+ID_DO_LOCATÁRIO = "TenantId"
+NOME_DA_INTEGRAÇÃO = "IntegrationName"
+NOME_DO_USUÁRIO = "UserName"
+EMAIL_DO_USUÁRIO = "UserEmail"
+ID_DA_FATURA = "InvoiceId"
+NÚMERO_DA_FATURA_DO_APLICATIVO = "AplicationInvoiceNumber"
+CNPJ_DO_FORNECEDOR = "SupplierCnpj"
+RAZÃO_SOCIAL_DO_FORNECEDOR = "SupplierCorporateName"
+CNPJ_DO_CLIENTE = "ClientCnpj"
+RAZÃO_SOCIAL_DO_CLIENTE = "ClientCorporateName"
+ENDEREÇO_DO_FORNECEDOR = "SupplierAddress"
+ENDEREÇO_DO_CLIENTE = "ClientAddress"
+DATA_DE_VENCIMENTO = "DueDate"
+DATA_DE_EMISSÃO = "DateOfIssue"
+DATA_DE_REFERÊNCIA = "ReferenceDate"
+DATA_DE_REGISTRO = "DateRegister"
+VALOR_TOTAL_DA_FATURA = "TotalInvoiceAmount"
+VALOR_BRUTO_DA_FATURA = "GrossInvoiceValue"
+CÓDIGO_DE_BARRAS = "BarCode"
+NÚMERO_DA_FATURA = "InvoiceNumber"
+CHAVE_DE_ACESSO_DA_FATURA = "InvoiceAccessKey"
+NÚMERO_DA_FATURA_DO_FORNECEDOR = "SupplierInvoiceNumber"
+CÓDIGO_DE_DEBITO_AUTOMÁTICO = "AutomaticDebitCode"
+INFORMAÇÃO_DA_FATURA = "InvoiceInformation"
+OBSERVAÇÃO_DA_FATURA = "InvoiceObservation"
+NOME_DO_FORNECEDOR = "SupplierName"
+NÚMERO_DO_CONTRATO = "ContractNumber"
+ID_DO_CONTRATO = "ContractId"
+STATUS_DO_CONTRATO = "ContractStatus"
+STATUS_DA_FATURA = "InvoiceStatus"
+LOCALIZAÇÃO_DO_CONTRATO = "ContractLocation"
+VERTICAL_DO_FORNECEDOR = "SupplierVertical"
+PROTOCOLO_DE_LANÇAMENTO = "launchProtocol"
+SERVIÇOS_DA_FATURA = "InvoiceServices"
+IMPOSTOS = "Taxes"
+CAMPOS_CUSTOMIZADOS = "CustomFields"
+ALOCAÇÕES_DE_CUSTO = "CostAllocations"
+ARQUIVOS_DA_FATURA = "InvoiceFiles"
+COMPLEMENTO_DE_ÁGUA = "WaterComplement"
+COMPLEMENTO_DE_ENERGIA = "EnergyComplement"
+COMPLEMENTO_DE_GÁS = "GasComplement"
 POSSUI_CHAVE_ACESSO = "possui_chave_acesso"
```

### Comparing `hnt_nf_jira_library-0.4.4/nf_jira/wrapper_nf_jira.py` & `hnt_nf_jira_library-0.4.5/nf_jira/wrapper_nf_jira.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,338 +1,351 @@
-import json
-import requests
-import os
-import locale
-from os import getcwd, path
-from datetime import datetime
-from pydantic import ValidationError
-
-from .entities.nota_pedido import NotaPedido
-from .entities.miro import Miro
-from .entities.fatura import Fatura
-from .entities.constants import *
-
-from .entities.classes.form_jira    import FormJira
-from .entities.classes.issue_jira   import IssueJira, AttachmentJira, TransitionJira, CommentJira
-from .entities.classes.issue_fields import IssueFields
-from .entities.classes.helper       import JiraFieldsHelper, JsonHelper, GuiandoHelper
-from .entities.classes.n8n_domain   import N8NDomain
-class wrapper_jira:
-
-    def __init__(self, miro_is_active=False ,debug=False):
-        
-        self._test_mode = debug
-        self._miro_is_active  = miro_is_active
-        self._instance_class()
-        locale.setlocale(locale.LC_ALL, ('pt_BR.UTF-8'))
-
-    def _instance_class(self):
-        self.FormJira         = FormJira()
-        self.IssueJira        = IssueJira()
-        self.AttachmentJira   = AttachmentJira()
-        self.TransitionJira   = TransitionJira()
-        self.CommentJira      = CommentJira()
-        self.JiraFieldsHelper = JiraFieldsHelper()
-        self.GuiandoHelper    = GuiandoHelper()
-        self.JsonHelper       = JsonHelper()
-        self.IssueFields      = IssueFields()
-        self.N8NDomain        = N8NDomain()
-
-    def get_document_by_issue(self, issue_key):
-
-        issue_sap_json = {}
-
-        issue = self._get_issue_by_key(issue_key)
-        issue_transition = issue['domain_data']['fornecedor']['transacao']
-
-        if issue_transition == 'ME21N':
-            nota_pedido_factory = self._issue_factory(issue)
-            nota_pedido_model   = NotaPedido(**nota_pedido_factory).model_dump()
-            issue_sap_json["nota_pedido"] = nota_pedido_model
-
-            if self._miro_is_active:
-                miro_factory = self._miro_factory(issue)
-                miro_model = Miro(**miro_factory).model_dump()
-                issue_sap_json["miro"] = miro_model
-
-        elif issue_transition == 'FV60':
-            fatura_factory = self._fatura_factory(issue)
-            fatura_model   = Fatura(**fatura_factory).model_dump()
-            issue_sap_json["fatura"] = fatura_model
-
-        issue_sap_json["jira_info"] = issue["jira_info"]
-
-        if self._test_mode:
-            for json in issue_sap_json:
-                self.JsonHelper.save_json(f'{json}_{issue_key}', issue_sap_json[json])
-            
-        return issue_sap_json
-
-    def _get_issue_by_key(self, issue_key):
-
-        issue_json = self._get_nf_jira(issue_key)
-
-        issue_attachment = issue_json["attachment"]
-        jira_info = issue_json["jira_info"]
-
-        fornecedor_domain = self.N8NDomain.get_nf_domain(FORNECEDOR_N8N_DOMAIN, issue_attachment[CNPJ_DO_FORNECEDOR])
-        centro_domain = self.N8NDomain.get_nf_domain(CENTRO_N8N_DOMAIN, issue_attachment[CNPJ_DO_CLIENTE])
-
-        domain = {
-            "fornecedor"    : fornecedor_domain,
-            "centro" : centro_domain
-        }
-
-
-        issue = {
-            "issue_data": issue_json["issue_data"],
-            "json_data": issue_attachment,
-            "domain_data": domain,
-            "pdf_data": issue_json["pdf_data"],
-            "jira_info": jira_info,
-        }
-
-        if self._test_mode:
-            self.JsonHelper.save_json(f'Issue_data_{issue_key}', issue)
-
-        return issue
-
-    def _issue_factory(self, issue: dict):
-
-        sintese_itens = []
-
-        if not issue['json_data'][ALOCAÇÕES_DE_CUSTO]:
-
-            item = {
-                "centro": issue["domain_data"]["centro"]["centro"],
-                "centro_custo": f"{issue['domain_data']['centro']['centro_custo']}",
-                "cod_imposto": "C6",
-                "valor_bruto": str(issue["json_data"][VALOR_TOTAL_DA_FATURA]),
-            }
-
-            sintese_item = {
-                "categoria_cc": "K",
-                "quantidade": 1,
-                "cod_material": issue["domain_data"]["fornecedor"]["codigo_material"],
-                "item": item,
-            }
-
-            sintese_itens.append(sintese_item)
-
-        else:
-
-            for cost_allocation in issue['json_data'][ALOCAÇÕES_DE_CUSTO]:
-                
-                item = {
-                    "centro": cost_allocation['CustCenterDescription'].split(' - ')[0],
-                    "centro_custo": cost_allocation['Code'],
-                    "cod_imposto": "C6",
-                    "valor_bruto": locale.format_string("%.2f", cost_allocation['CustCenterTotalAmount']),
-                }
-
-                sintese_item = {
-                    "categoria_cc": "K",
-                    "quantidade": 1,
-                    "cod_material": issue["domain_data"]["fornecedor"][
-                        "codigo_material"
-                    ],
-                    "item": item,
-                }
-
-                sintese_itens.append(sintese_item)
-
-        nota_pedido = {
-            "tipo": "ZCOR",
-            "org_compras": issue["domain_data"]["centro"]["org_compras"],
-            "grp_compradores": issue['json_data']['grupo_compradores'][0],
-            "empresa": "HFNT",
-            "cod_fornecedor": issue["domain_data"]["fornecedor"]["codigo_sap"],
-            "sintese_itens": sintese_itens,
-            "anexo": issue['pdf_data'],
-        }
-
-        return nota_pedido
-
-    def _miro_factory(self, issue: dict):
-
-        texto = self._prepare_ref(issue)
-
-        dados_basicos = {
-            "data_da_fatura": datetime.strptime(
-                issue['json_data'][DATA_DE_EMISSÃO], "%Y-%m-%d"
-            ).strftime("%d.%m.%Y"),
-            "referencia": f"{issue['json_data'][CHAVE_DE_ACESSO_DA_FATURA][25:34]}-{issue['json_data'][CHAVE_DE_ACESSO_DA_FATURA][22:25]}",
-            "montante": str(issue['json_data'][VALOR_TOTAL_DA_FATURA]),
-            "texto": texto,
-        }
-
-        detalhe = {"ctg_nf": issue["domain_data"]["fornecedor"]["categoria_nf"]}
-
-        sintese = {"CFOP": issue["domain_data"]["fornecedor"]["cfop"]}
-
-        chave_acesso = {
-            "tp_emissao":f"{issue['json_data'][CHAVE_DE_ACESSO_DA_FATURA][34]}",
-            "numero_aleatorio": f"{issue['json_data'][CHAVE_DE_ACESSO_DA_FATURA][35:43]}",
-            "dig_verif": f"{issue['json_data'][CHAVE_DE_ACESSO_DA_FATURA][43:]}",
-        }
-
-        nfe_sefaz = {
-            "numero_log": issue['json_data']["numero_log"],
-            "data_procmto": datetime.strptime(issue['json_data']["data_procmto"], "%Y-%m-%d").strftime("%d.%m.%Y"),
-            "hora_procmto": issue['json_data']["hora_procmto"],
-        }
-
-        dados_nfe = {"chave_acesso_sefaz": chave_acesso, "nfe_sefaz": nfe_sefaz}
-
-        miro_model = {
-            "dados_basicos": dados_basicos,
-            "detalhe": detalhe,
-            "sintese": sintese,
-            "dados_nfe": dados_nfe,
-        }
-
-        return miro_model
-    
-    def _fatura_factory(self, issue): 
-
-        texto = self._prepare_ref(issue)
-
-        item = {
-            "Cta_razao": issue['domain_data']['fornecedor']['razao'], #Conta Contabil SAP
-            "Montante":  str(issue['json_data'][VALOR_TOTAL_DA_FATURA]),
-            "loc_negocios": issue['domain_data']['centro']['centro'],
-            "atribuicao": datetime.strptime(issue['json_data'][DATA_DE_EMISSÃO], "%Y-%m-%d").strftime("%Y%m%d"),
-            "texto": texto,
-            "centro_custo":  f"{issue['domain_data']['centro']['centro']}210"
-        }
-
-        itens = [item]
-
-        dados_basicos = {
-            "cod_fornecedor": issue['domain_data']['fornecedor']['codigo_sap'], #ID_EXTERNO_SAP
-            "data_fatura": datetime.strptime(issue['json_data'][DATA_DE_EMISSÃO], "%Y-%m-%d").strftime("%d.%m.%Y"),
-            "referencia": issue['json_data'][NÚMERO_DA_FATURA_DO_FORNECEDOR],
-            "montante": str(issue['json_data'][VALOR_TOTAL_DA_FATURA]),
-            "bus_pl_sec_cd": itens[0]["loc_negocios"],
-            "texto": texto,
-            "itens": itens
-        }
-
-        pagamento = {
-            "data_basica": datetime.now().strftime("%d.%m.%Y"),
-            "cond_pgto": "0000" #CONSTANTE 
-        }
-
-        fatura_model = {
-            "dados_basicos": dados_basicos,
-            "pagamento":pagamento,
-        }
-
-        return fatura_model
-
-    def _get_nf_jira(self, issue_id):
-        try:
-
-            issue_data = self.IssueJira.get_issue(issue_id)
-            complement_form = self._get_issue_fields_by_keys( issue_id, FORM_TEMPLATE_COMPLEMENTO )
-            self.GuiandoHelper.check_guiando_form(complement_form)
-            donwload_attachment = self.AttachmentJira.download_attachments(issue_data)
-
-            issue_data["fields"] = self.JiraFieldsHelper.remove_null_fields(issue_data.get("fields"))
-            attachment = self.AttachmentJira.get_attachment(issue_data)
-
-            nf_type_id = complement_form["tipo_conta"]
-
-            if nf_type_id == "ÁGUA":
-                nf_type = COMPLEMENTO_DE_ÁGUA
-
-            elif nf_type_id == "ENERGIA":
-                nf_type = COMPLEMENTO_DE_ENERGIA
-
-            elif nf_type_id == "GÁS":
-                nf_type = COMPLEMENTO_DE_GÁS
-
-            else:
-                if attachment[COMPLEMENTO_DE_ÁGUA] is not None:
-                    nf_type = COMPLEMENTO_DE_ÁGUA
-                elif attachment[COMPLEMENTO_DE_ENERGIA] is not None:
-                    nf_type = COMPLEMENTO_DE_ENERGIA
-                elif attachment[COMPLEMENTO_DE_GÁS] is not None:
-                    nf_type = COMPLEMENTO_DE_GÁS
-
-            attachment[CNPJ_DO_FORNECEDOR] = complement_form['cnpj_fornecedor']
-            attachment[RAZÃO_SOCIAL_DO_FORNECEDOR] = complement_form['razao_social_fornecedor']
-
-            attachment[CNPJ_DO_CLIENTE] = complement_form['cnpj_destinatario']
-            attachment[NÚMERO_DA_FATURA] = complement_form['nro_nota_fiscal']
-            attachment[NÚMERO_DA_FATURA_DO_FORNECEDOR] = complement_form['nro_fatura']
-            attachment[DATA_DE_EMISSÃO] = complement_form['data_emissao']
-            attachment[DATA_DE_VENCIMENTO] = complement_form['data_vencimento']
-            attachment[CHAVE_DE_ACESSO_DA_FATURA] = complement_form['chave_acesso']
-            attachment[DATA_DE_REFERÊNCIA] = complement_form['periodo_referencia']
-            attachment["numero_log"] = complement_form['protocolo_autorizacao']
-            attachment["data_procmto"] = complement_form['data_autorizacao']
-            attachment["hora_procmto"] = complement_form['hora_autorizacao']
-            attachment[nf_type] = {
-                "DataLeituraAnterior" : complement_form['data_leitura_anterior'],
-                "DataLeituraAtual"    : complement_form['data_leitura_atual']
-            }
-            # attachment[nf_type]["DataLeituraAnterior"] = complement_form['data_leitura_anterior']
-            # attachment[nf_type]["DataLeituraAtual"] = complement_form['data_leitura_atual']
-            attachment["grupo_compradores"] = complement_form['grupo_compradores']
-
-            #Validação de Valor Liquido da Fatura
-            if complement_form['valor_liquido'] != "" and complement_form['valor_liquido'] != None:
-                attachment[VALOR_TOTAL_DA_FATURA] = complement_form['valor_liquido']
-            elif complement_form['valor_nota'] != None and complement_form['valor_nota'] != "":
-                attachment[VALOR_TOTAL_DA_FATURA] = complement_form['valor_nota']
-            else:
-                attachment[VALOR_TOTAL_DA_FATURA] = attachment.get(
-                    VALOR_TOTAL_DA_FATURA
-                )
-
-            automation_form_id = self.FormJira.get_form_id(issue_id, FORM_TEMPLATE_AUTOMACAO)
-
-            jira_info = {"issue_id": issue_id, "form_id": automation_form_id}
-
-            nf_jira_json = {
-                "issue_data": issue_data,
-                "attachment": attachment,
-                "jira_info": jira_info,
-                "pdf_data": donwload_attachment
-            }
-
-            return nf_jira_json
-
-        except requests.exceptions.HTTPError as e:
-            raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
-
-        except Exception as e:
-            raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
-
-    def _prepare_ref(self, issue):
-
-        data_ref = datetime.strptime(issue['json_data'][DATA_DE_REFERÊNCIA], "%m/%Y").strftime("%b/%y").upper()
-
-        if issue['json_data'][COMPLEMENTO_DE_ÁGUA] is not None:
-            
-            leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAnterior'] is not None else None
-            leitura_atual = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAtual'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAtual'] is not None else None
-        elif issue['json_data'][COMPLEMENTO_DE_ENERGIA] is not None:
-            leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAnterior'] is not None else None
-            leitura_atual = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAtual'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAtual'] is not None else None
-        elif issue['json_data'][COMPLEMENTO_DE_GÁS] is not None:
-            leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAnterior'] is not None else None
-            leitura_atual = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAtual'], "%Y-%m-%d").strftime("%b/%y").upper()  if issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAtual'] is not None else None
-
-        extra_ref = f"PERIODO: {leitura_anterior} A {leitura_atual}" if leitura_anterior is not None and leitura_atual is not None else None
-
-        return f"REF: {data_ref} {extra_ref}"
-
-    def _get_issue_fields_by_keys(self, issue_key, form_template):
-
-        form_jira_keys = self.FormJira.get_form_jira_keys(issue_key, form_template)
-        form_fields    = self.FormJira.get_form_fields(issue_key, form_template)
-        jira_fields    = self.IssueJira.get_issue_fields_data(issue_key)
-        fields_by_jira_and_form = self.IssueFields.get_fields_by_form_and_jira(form_jira_keys, form_fields, jira_fields)
-
+import json
+import requests
+import os
+import locale
+from os import getcwd, path
+from datetime import datetime
+from pydantic import ValidationError
+
+from .entities.nota_pedido import NotaPedido
+from .entities.miro import Miro
+from .entities.fatura import Fatura
+from .entities.constants import *
+
+from .entities.classes.form_jira    import FormJira
+from .entities.classes.issue_jira   import IssueJira, AttachmentJira, TransitionJira, CommentJira
+from .entities.classes.issue_fields import IssueFields
+from .entities.classes.helper       import JiraFieldsHelper, JsonHelper, GuiandoHelper
+from .entities.classes.n8n_domain   import N8NDomain
+class wrapper_jira:
+
+    def __init__(self, miro_is_active=False ,debug=False):
+        locale.setlocale(locale.LC_ALL, ('pt_BR.UTF-8'))
+        self._test_mode = debug
+        self._miro_is_active  = miro_is_active
+        self._instance_class()
+
+    def _instance_class(self):
+        self.FormJira         = FormJira()
+        self.IssueJira        = IssueJira()
+        self.AttachmentJira   = AttachmentJira()
+        self.TransitionJira   = TransitionJira()
+        self.CommentJira      = CommentJira()
+        self.JiraFieldsHelper = JiraFieldsHelper()
+        self.GuiandoHelper    = GuiandoHelper()
+        self.JsonHelper       = JsonHelper()
+        self.IssueFields      = IssueFields()
+        self.N8NDomain        = N8NDomain()
+
+    def get_document_by_issue(self, issue_key):
+
+        issue_sap_json = {}
+
+        issue = self._get_issue_by_key(issue_key)
+        issue_transition = issue['domain_data']['fornecedor']['transacao']
+
+        if issue_transition == 'ME21N':
+            nota_pedido_factory = self._issue_factory(issue)
+            nota_pedido_model   = NotaPedido(**nota_pedido_factory).model_dump()
+            issue_sap_json["nota_pedido"] = nota_pedido_model
+
+            if self._miro_is_active:
+                miro_factory = self._miro_factory(issue)
+                miro_model = Miro(**miro_factory).model_dump()
+                issue_sap_json["miro"] = miro_model
+
+        elif issue_transition == 'FV60':
+            fatura_factory = self._fatura_factory(issue)
+            fatura_model   = Fatura(**fatura_factory).model_dump()
+            issue_sap_json["fatura"] = fatura_model
+
+        issue_sap_json["jira_info"] = issue["jira_info"]
+
+        if self._test_mode:
+            for json in issue_sap_json:
+                self.JsonHelper.save_json(f'{json}_{issue_key}', issue_sap_json[json])
+            
+        return issue_sap_json
+
+    def _get_issue_by_key(self, issue_key):
+
+        issue_json = self._get_nf_jira(issue_key)
+
+        issue_attachment = issue_json["attachment"]
+        jira_info = issue_json["jira_info"]
+
+        fornecedor_domain = self.N8NDomain.get_nf_domain(FORNECEDOR_N8N_DOMAIN, issue_attachment[CNPJ_DO_FORNECEDOR])
+        centro_domain = self.N8NDomain.get_nf_domain(CENTRO_N8N_DOMAIN, issue_attachment[CNPJ_DO_CLIENTE])
+
+        domain = {
+            "fornecedor"    : fornecedor_domain,
+            "centro" : centro_domain
+        }
+
+        issue = {
+            "issue_data": issue_json["issue_data"],
+            "json_data": issue_attachment,
+            "domain_data": domain,
+            "pdf_data": issue_json["pdf_data"],
+            "jira_info": jira_info,
+        }
+
+        if self._test_mode:
+            self.JsonHelper.save_json(f'Issue_data_{issue_key}', issue)
+
+        return issue
+
+    def _issue_factory(self, issue: dict):
+
+        sintese_itens = []
+
+        if not issue['json_data'][ALOCAÇÕES_DE_CUSTO]:
+
+            item = {
+                "centro": issue["domain_data"]["centro"]["centro"],
+                "centro_custo": f"{issue['domain_data']['centro']['centro_custo']}",
+                "cod_imposto": "C6",
+                "valor_bruto": issue["json_data"][VALOR_TOTAL_DA_FATURA],
+                "percentage": CEM_PORCENTO_DO_VALOR_BRUTO
+            }
+
+            sintese_item = {
+                "categoria_cc": "K",
+                "quantidade": 1,
+                "cod_material": issue["domain_data"]["fornecedor"]["codigo_material"],
+                "item": item,
+            }
+
+            sintese_itens.append(sintese_item)
+
+        else:
+
+            for cost_allocation in issue['json_data'][ALOCAÇÕES_DE_CUSTO]:
+                
+                item = {
+                    "centro": cost_allocation['CustCenterDescription'].split(' - ')[0],
+                    "centro_custo": cost_allocation['Code'],
+                    "cod_imposto": "C6",
+                    "valor_bruto": cost_allocation['CustCenterTotalAmount'],
+                    "percentage": cost_allocation['Percentage']
+                }
+
+                sintese_item = {
+                    "categoria_cc": "K",
+                    "quantidade": 1,
+                    "cod_material": issue["domain_data"]["fornecedor"][
+                        "codigo_material"
+                    ],
+                    "item": item,
+                }
+
+                sintese_itens.append(sintese_item)
+
+        nota_pedido = {
+            "valor_bruto": issue['json_data'][VALOR_TOTAL_DA_FATURA],
+            "valor_liquido": issue["json_data"][VALOR_LIQUIDO_DA_FATURA],
+            "juros": issue["json_data"][JUROS_DA_FATURA],
+            "tipo": "ZCOR",
+            "org_compras": issue["domain_data"]["centro"]["org_compras"],
+            "grp_compradores": issue['json_data']['grupo_compradores'][0],
+            "empresa": "HFNT",
+            "cod_fornecedor": issue["domain_data"]["fornecedor"]["codigo_sap"],
+            "sintese_itens": sintese_itens,
+            "anexo": issue['pdf_data'],
+        }
+
+        return nota_pedido
+
+    def _miro_factory(self, issue: dict):
+
+        texto = self._prepare_ref(issue)
+
+        dados_basicos = {
+            "data_da_fatura": datetime.strptime(
+                issue['json_data'][DATA_DE_EMISSÃO], "%Y-%m-%d"
+            ).strftime("%d.%m.%Y"),
+            "referencia": f"{issue['json_data'][CHAVE_DE_ACESSO_DA_FATURA][25:34]}-{issue['json_data'][CHAVE_DE_ACESSO_DA_FATURA][22:25]}",
+            "montante": issue["json_data"][VALOR_LIQUIDO_DA_FATURA] if issue["json_data"][VALOR_LIQUIDO_DA_FATURA] > 0 else issue['json_data'][VALOR_TOTAL_DA_FATURA],
+            "texto": texto,
+        }
+
+        detalhe = {"ctg_nf": issue["domain_data"]["fornecedor"]["categoria_nf"]}
+
+        sintese = {"CFOP": issue["domain_data"]["fornecedor"]["cfop"]}
+
+        chave_acesso = {
+            "tp_emissao":f"{issue['json_data'][CHAVE_DE_ACESSO_DA_FATURA][34]}",
+            "numero_aleatorio": f"{issue['json_data'][CHAVE_DE_ACESSO_DA_FATURA][35:43]}",
+            "dig_verif": f"{issue['json_data'][CHAVE_DE_ACESSO_DA_FATURA][43:]}",
+        }
+
+        nfe_sefaz = {
+            "numero_log": issue['json_data']["numero_log"],
+            "data_procmto": datetime.strptime(issue['json_data']["data_procmto"], "%Y-%m-%d").strftime("%d.%m.%Y"),
+            "hora_procmto": issue['json_data']["hora_procmto"],
+        }
+
+        dados_nfe = {"chave_acesso_sefaz": chave_acesso, "nfe_sefaz": nfe_sefaz}
+
+        miro_model = {
+            "dados_basicos": dados_basicos,
+            "detalhe": detalhe,
+            "sintese": sintese,
+            "dados_nfe": dados_nfe,
+        }
+
+        return miro_model
+    
+    def _fatura_factory(self, issue): 
+
+        texto = self._prepare_ref(issue)
+        itens = []
+        if not issue['json_data'][ALOCAÇÕES_DE_CUSTO]:
+            itens.append({
+                "cta_razao": issue['domain_data']['fornecedor']['razao'], #Conta Contabil SAP
+                "montante":  issue['json_data'][VALOR_TOTAL_DA_FATURA],
+                "percentage" : CEM_PORCENTO_DO_VALOR_BRUTO,
+                "loc_negocios": issue['domain_data']['centro']['centro'],
+                "atribuicao": datetime.strptime(issue['json_data'][DATA_DE_EMISSÃO], "%Y-%m-%d").strftime("%Y%m%d"),
+                "texto": texto,
+                "centro_custo":  f"{issue['domain_data']['centro']['centro_custo']}",
+            })
+        else:
+            for cost_allocation in issue['json_data'][ALOCAÇÕES_DE_CUSTO]:
+                itens.append({
+                    "cta_razao": issue['domain_data']['fornecedor']['razao'], #Conta Contabil SAP
+                    "montante":  cost_allocation['CustCenterTotalAmount'],
+                    "percentage" : cost_allocation['Percentage'],
+                    "loc_negocios": cost_allocation['CustCenterDescription'].split(' - ')[0],
+                    "atribuicao": datetime.strptime(issue['json_data'][DATA_DE_EMISSÃO], "%Y-%m-%d").strftime("%Y%m%d"),
+                    "texto": texto,
+                    "centro_custo":  cost_allocation['Code']
+                })
+
+        dados_basicos = {
+            "cod_fornecedor": issue['domain_data']['fornecedor']['codigo_sap'], #ID_EXTERNO_SAP
+            "data_fatura": datetime.strptime(issue['json_data'][DATA_DE_EMISSÃO], "%Y-%m-%d").strftime("%d.%m.%Y"),
+            "referencia": issue['json_data'][NÚMERO_DA_FATURA_DO_FORNECEDOR],
+            "montante": issue['json_data'][VALOR_TOTAL_DA_FATURA],
+            "valor_liquido": issue["json_data"][VALOR_LIQUIDO_DA_FATURA],
+            "juros": issue["json_data"][JUROS_DA_FATURA],
+            "bus_pl_sec_cd": itens[0]["loc_negocios"],
+            "texto": texto,
+            "itens": itens
+        }
+
+        pagamento = {
+            "data_basica": datetime.now().strftime("%d.%m.%Y"),
+            "cond_pgto": "0000" #CONSTANTE 
+        }
+
+        fatura_model = {
+            "dados_basicos": dados_basicos,
+            "pagamento":pagamento,
+        }
+
+        return fatura_model
+
+    def _get_nf_jira(self, issue_id):
+        try:
+
+            issue_data = self.IssueJira.get_issue(issue_id)
+            complement_form = self._get_issue_fields_by_keys( issue_id, FORM_TEMPLATE_COMPLEMENTO )
+            self.GuiandoHelper.check_guiando_form(complement_form)
+            donwload_attachment = self.AttachmentJira.download_attachments(issue_data)
+
+            issue_data["fields"] = self.JiraFieldsHelper.remove_null_fields(issue_data.get("fields"))
+            attachment = self.AttachmentJira.get_attachment(issue_data)
+
+            nf_type_id = complement_form["tipo_conta"]
+
+            if nf_type_id == "ÁGUA":
+                nf_type = COMPLEMENTO_DE_ÁGUA
+
+            elif nf_type_id == "ENERGIA":
+                nf_type = COMPLEMENTO_DE_ENERGIA
+
+            elif nf_type_id == "GÁS":
+                nf_type = COMPLEMENTO_DE_GÁS
+
+            else:
+                if attachment[COMPLEMENTO_DE_ÁGUA] is not None:
+                    nf_type = COMPLEMENTO_DE_ÁGUA
+                elif attachment[COMPLEMENTO_DE_ENERGIA] is not None:
+                    nf_type = COMPLEMENTO_DE_ENERGIA
+                elif attachment[COMPLEMENTO_DE_GÁS] is not None:
+                    nf_type = COMPLEMENTO_DE_GÁS
+
+            attachment[CNPJ_DO_FORNECEDOR] = complement_form['cnpj_fornecedor']
+            attachment[RAZÃO_SOCIAL_DO_FORNECEDOR] = complement_form['razao_social_fornecedor']
+
+            attachment[CNPJ_DO_CLIENTE] = complement_form['cnpj_destinatario']
+            attachment[NÚMERO_DA_FATURA] = complement_form['nro_nota_fiscal']
+            attachment[NÚMERO_DA_FATURA_DO_FORNECEDOR] = complement_form['nro_fatura']
+            attachment[DATA_DE_EMISSÃO] = complement_form['data_emissao']
+            attachment[DATA_DE_VENCIMENTO] = complement_form['data_vencimento']
+            attachment[CHAVE_DE_ACESSO_DA_FATURA] = complement_form['chave_acesso']
+            attachment[DATA_DE_REFERÊNCIA] = complement_form['periodo_referencia']
+            attachment["numero_log"] = complement_form['protocolo_autorizacao']
+            attachment["data_procmto"] = complement_form['data_autorizacao']
+            attachment["hora_procmto"] = complement_form['hora_autorizacao']
+            attachment[nf_type] = {
+                "DataLeituraAnterior" : complement_form['data_leitura_anterior'],
+                "DataLeituraAtual"    : complement_form['data_leitura_atual']
+            }
+
+            attachment["grupo_compradores"] = complement_form['grupo_compradores']
+
+            #Init Valor Liquido e Juros
+            attachment[VALOR_LIQUIDO_DA_FATURA] = 0
+            attachment[JUROS_DA_FATURA] = 0
+            if complement_form['valor_liquido'] != "" and complement_form['valor_liquido'] != None:
+                attachment[VALOR_LIQUIDO_DA_FATURA] = float(complement_form['valor_liquido'].replace('.','').replace(',','.'))
+            if complement_form['juros'] != "" and complement_form['juros'] != None:
+                attachment[JUROS_DA_FATURA] = float(complement_form['juros'].replace('.','').replace(',','.'))
+
+            automation_form_id = self.FormJira.get_form_id(issue_id, FORM_TEMPLATE_AUTOMACAO)
+
+            jira_info = {"issue_id": issue_id, "form_id": automation_form_id}
+
+            nf_jira_json = {
+                "issue_data": issue_data,
+                "attachment": attachment,
+                "jira_info": jira_info,
+                "pdf_data": donwload_attachment
+            }
+
+            return nf_jira_json
+
+        except requests.exceptions.HTTPError as e:
+            raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
+
+        except Exception as e:
+            raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
+
+    def _prepare_ref(self, issue):
+
+        data_ref = datetime.strptime(issue['json_data'][DATA_DE_REFERÊNCIA], "%m/%Y").strftime("%b/%y").upper()
+
+        if issue['json_data'][COMPLEMENTO_DE_ÁGUA] is not None:
+            
+            leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAnterior'] is not None else None
+            leitura_atual = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAtual'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAtual'] is not None else None
+        elif issue['json_data'][COMPLEMENTO_DE_ENERGIA] is not None:
+            leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAnterior'] is not None else None
+            leitura_atual = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAtual'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAtual'] is not None else None
+        elif issue['json_data'][COMPLEMENTO_DE_GÁS] is not None:
+            leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAnterior'] is not None else None
+            leitura_atual = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAtual'], "%Y-%m-%d").strftime("%b/%y").upper()  if issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAtual'] is not None else None
+
+        extra_ref = f"PERIODO: {leitura_anterior} A {leitura_atual}" if leitura_anterior is not None and leitura_atual is not None else None
+
+        return f"REF: {data_ref} {extra_ref}"
+
+    def _get_issue_fields_by_keys(self, issue_key, form_template):
+
+        form_jira_keys = self.FormJira.get_form_jira_keys(issue_key, form_template)
+        form_fields    = self.FormJira.get_form_fields(issue_key, form_template)
+        jira_fields    = self.IssueJira.get_issue_fields_data(issue_key)
+        fields_by_jira_and_form = self.IssueFields.get_fields_by_form_and_jira(form_jira_keys, form_fields, jira_fields)
+
         return fields_by_jira_and_form
```

