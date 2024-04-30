# Comparing `tmp/PrimeBotFramework-1.0.50.tar.gz` & `tmp/primebotframework-1.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-b1su3wrr/PrimeBotFramework-1.0.50.tar", last modified: Thu Apr 11 16:50:05 2024, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-qmvilr51/primebotframework-1.0.53.tar", last modified: Tue Apr 30 16:38:54 2024, max compression
```

## Comparing `PrimeBotFramework-1.0.50.tar` & `primebotframework-1.0.53.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 16:50:05.582051 PrimeBotFramework-1.0.50/
--rw-r--r--   0 root         (0) root         (0)      891 2024-04-11 16:50:05.582051 PrimeBotFramework-1.0.50/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 16:50:05.578051 PrimeBotFramework-1.0.50/PrimeBot/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 16:50:05.578051 PrimeBotFramework-1.0.50/PrimeBot/B2E/
--rw-rw-rw-   0 root         (0) root         (0)     4028 2024-04-11 16:49:57.000000 PrimeBotFramework-1.0.50/PrimeBot/B2E/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 16:50:05.578051 PrimeBotFramework-1.0.50/PrimeBot/Cnab750/
--rw-rw-rw-   0 root         (0) root         (0)    10261 2024-04-11 16:49:57.000000 PrimeBotFramework-1.0.50/PrimeBot/Cnab750/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 16:50:05.578051 PrimeBotFramework-1.0.50/PrimeBot/CpfCnpj/
--rw-rw-rw-   0 root         (0) root         (0)     1963 2024-04-11 16:49:57.000000 PrimeBotFramework-1.0.50/PrimeBot/CpfCnpj/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2024-04-11 16:49:57.000000 PrimeBotFramework-1.0.50/PrimeBot/CpfCnpj/api_codes.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2024-04-11 16:49:57.000000 PrimeBotFramework-1.0.50/PrimeBot/CpfCnpj/model.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 16:50:05.578051 PrimeBotFramework-1.0.50/PrimeBot/D4Sign/
--rw-rw-rw-   0 root         (0) root         (0)     2600 2024-04-11 16:49:57.000000 PrimeBotFramework-1.0.50/PrimeBot/D4Sign/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 16:50:05.578051 PrimeBotFramework-1.0.50/PrimeBot/DeathByCaptcha/
--rw-rw-rw-   0 root         (0) root         (0)     5755 2024-04-11 16:49:57.000000 PrimeBotFramework-1.0.50/PrimeBot/DeathByCaptcha/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 16:50:05.578051 PrimeBotFramework-1.0.50/PrimeBot/Documents/
--rw-rw-rw-   0 root         (0) root         (0)     1098 2024-04-11 16:49:57.000000 PrimeBotFramework-1.0.50/PrimeBot/Documents/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 16:50:05.578051 PrimeBotFramework-1.0.50/PrimeBot/Elastic/
--rw-rw-rw-   0 root         (0) root         (0)     1239 2024-04-11 16:49:57.000000 PrimeBotFramework-1.0.50/PrimeBot/Elastic/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 16:50:05.578051 PrimeBotFramework-1.0.50/PrimeBot/EmailAlert/
--rw-rw-rw-   0 root         (0) root         (0)     3427 2024-04-11 16:49:57.000000 PrimeBotFramework-1.0.50/PrimeBot/EmailAlert/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 16:50:05.578051 PrimeBotFramework-1.0.50/PrimeBot/ExchangeGraph/
--rw-rw-rw-   0 root         (0) root         (0)     8987 2024-04-11 16:49:57.000000 PrimeBotFramework-1.0.50/PrimeBot/ExchangeGraph/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 16:50:05.578051 PrimeBotFramework-1.0.50/PrimeBot/FeriadosBancarios/
--rw-rw-rw-   0 root         (0) root         (0)     1925 2024-04-11 16:49:57.000000 PrimeBotFramework-1.0.50/PrimeBot/FeriadosBancarios/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2024-04-11 16:49:57.000000 PrimeBotFramework-1.0.50/PrimeBot/FeriadosBancarios/model.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 16:50:05.578051 PrimeBotFramework-1.0.50/PrimeBot/IntegracaoSendGrid/
--rw-rw-rw-   0 root         (0) root         (0)     4251 2024-04-11 16:49:57.000000 PrimeBotFramework-1.0.50/PrimeBot/IntegracaoSendGrid/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 16:50:05.578051 PrimeBotFramework-1.0.50/PrimeBot/ListenerECS/
--rw-rw-rw-   0 root         (0) root         (0)     4096 2024-04-11 16:49:57.000000 PrimeBotFramework-1.0.50/PrimeBot/ListenerECS/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 16:50:05.578051 PrimeBotFramework-1.0.50/PrimeBot/Mongo/
--rw-rw-rw-   0 root         (0) root         (0)      465 2024-04-11 16:49:57.000000 PrimeBotFramework-1.0.50/PrimeBot/Mongo/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 16:50:05.578051 PrimeBotFramework-1.0.50/PrimeBot/OracleDB/
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-11 16:49:57.000000 PrimeBotFramework-1.0.50/PrimeBot/OracleDB/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 16:50:05.578051 PrimeBotFramework-1.0.50/PrimeBot/Vault/
--rw-rw-rw-   0 root         (0) root         (0)     2740 2024-04-11 16:49:57.000000 PrimeBotFramework-1.0.50/PrimeBot/Vault/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 16:49:57.000000 PrimeBotFramework-1.0.50/PrimeBot/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 16:50:05.582051 PrimeBotFramework-1.0.50/PrimeBotFramework.egg-info/
--rw-r--r--   0 root         (0) root         (0)      891 2024-04-11 16:50:05.000000 PrimeBotFramework-1.0.50/PrimeBotFramework.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      814 2024-04-11 16:50:05.000000 PrimeBotFramework-1.0.50/PrimeBotFramework.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-11 16:50:05.000000 PrimeBotFramework-1.0.50/PrimeBotFramework.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-11 16:50:05.000000 PrimeBotFramework-1.0.50/PrimeBotFramework.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2024-04-11 16:50:05.000000 PrimeBotFramework-1.0.50/PrimeBotFramework.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-11 16:50:05.582051 PrimeBotFramework-1.0.50/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      928 2024-04-11 16:49:57.000000 PrimeBotFramework-1.0.50/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:38:54.077519 primebotframework-1.0.53/
+-rw-r--r--   0 root         (0) root         (0)      891 2024-04-30 16:38:54.077519 primebotframework-1.0.53/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:38:54.073519 primebotframework-1.0.53/PrimeBot/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:38:54.073519 primebotframework-1.0.53/PrimeBot/B2E/
+-rw-rw-rw-   0 root         (0) root         (0)     4028 2024-04-30 16:38:44.000000 primebotframework-1.0.53/PrimeBot/B2E/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:38:54.073519 primebotframework-1.0.53/PrimeBot/Cnab750/
+-rw-rw-rw-   0 root         (0) root         (0)    10261 2024-04-30 16:38:44.000000 primebotframework-1.0.53/PrimeBot/Cnab750/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:38:54.073519 primebotframework-1.0.53/PrimeBot/CpfCnpj/
+-rw-rw-rw-   0 root         (0) root         (0)     1963 2024-04-30 16:38:44.000000 primebotframework-1.0.53/PrimeBot/CpfCnpj/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2024-04-30 16:38:44.000000 primebotframework-1.0.53/PrimeBot/CpfCnpj/api_codes.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2024-04-30 16:38:44.000000 primebotframework-1.0.53/PrimeBot/CpfCnpj/model.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:38:54.073519 primebotframework-1.0.53/PrimeBot/D4Sign/
+-rw-rw-rw-   0 root         (0) root         (0)     2600 2024-04-30 16:38:44.000000 primebotframework-1.0.53/PrimeBot/D4Sign/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:38:54.073519 primebotframework-1.0.53/PrimeBot/DeathByCaptcha/
+-rw-rw-rw-   0 root         (0) root         (0)     5755 2024-04-30 16:38:44.000000 primebotframework-1.0.53/PrimeBot/DeathByCaptcha/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:38:54.073519 primebotframework-1.0.53/PrimeBot/Documents/
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2024-04-30 16:38:44.000000 primebotframework-1.0.53/PrimeBot/Documents/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:38:54.073519 primebotframework-1.0.53/PrimeBot/Elastic/
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2024-04-30 16:38:44.000000 primebotframework-1.0.53/PrimeBot/Elastic/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:38:54.073519 primebotframework-1.0.53/PrimeBot/EmailAlert/
+-rw-rw-rw-   0 root         (0) root         (0)     3650 2024-04-30 16:38:44.000000 primebotframework-1.0.53/PrimeBot/EmailAlert/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:38:54.073519 primebotframework-1.0.53/PrimeBot/ExchangeGraph/
+-rw-rw-rw-   0 root         (0) root         (0)     8987 2024-04-30 16:38:44.000000 primebotframework-1.0.53/PrimeBot/ExchangeGraph/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:38:54.073519 primebotframework-1.0.53/PrimeBot/FeriadosBancarios/
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2024-04-30 16:38:44.000000 primebotframework-1.0.53/PrimeBot/FeriadosBancarios/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2024-04-30 16:38:44.000000 primebotframework-1.0.53/PrimeBot/FeriadosBancarios/model.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:38:54.073519 primebotframework-1.0.53/PrimeBot/IntegracaoSendGrid/
+-rw-rw-rw-   0 root         (0) root         (0)     4251 2024-04-30 16:38:44.000000 primebotframework-1.0.53/PrimeBot/IntegracaoSendGrid/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:38:54.073519 primebotframework-1.0.53/PrimeBot/ListenerECS/
+-rw-rw-rw-   0 root         (0) root         (0)     4096 2024-04-30 16:38:44.000000 primebotframework-1.0.53/PrimeBot/ListenerECS/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:38:54.073519 primebotframework-1.0.53/PrimeBot/Mongo/
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-04-30 16:38:44.000000 primebotframework-1.0.53/PrimeBot/Mongo/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:38:54.073519 primebotframework-1.0.53/PrimeBot/OracleDB/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-30 16:38:44.000000 primebotframework-1.0.53/PrimeBot/OracleDB/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:38:54.073519 primebotframework-1.0.53/PrimeBot/Vault/
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2024-04-30 16:38:44.000000 primebotframework-1.0.53/PrimeBot/Vault/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 16:38:44.000000 primebotframework-1.0.53/PrimeBot/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:38:54.073519 primebotframework-1.0.53/PrimeBotFramework.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      891 2024-04-30 16:38:54.000000 primebotframework-1.0.53/PrimeBotFramework.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      814 2024-04-30 16:38:54.000000 primebotframework-1.0.53/PrimeBotFramework.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-30 16:38:54.000000 primebotframework-1.0.53/PrimeBotFramework.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-30 16:38:54.000000 primebotframework-1.0.53/PrimeBotFramework.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2024-04-30 16:38:54.000000 primebotframework-1.0.53/PrimeBotFramework.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-30 16:38:54.077519 primebotframework-1.0.53/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      928 2024-04-30 16:38:44.000000 primebotframework-1.0.53/setup.py
```

### Comparing `PrimeBotFramework-1.0.50/PKG-INFO` & `primebotframework-1.0.53/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrimeBotFramework
-Version: 1.0.50
+Version: 1.0.53
 Summary: Um pacote de padronizacao de pacotes a serem utilizados pela Prime
 Home-page: 
 Author: Prime Control
 Author-email: 
 License: MIT
 Keywords: PrimeBotFramework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PrimeBotFramework-1.0.50/PrimeBot/B2E/__init__.py` & `primebotframework-1.0.53/PrimeBot/B2E/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.50/PrimeBot/Cnab750/__init__.py` & `primebotframework-1.0.53/PrimeBot/Cnab750/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.50/PrimeBot/CpfCnpj/__init__.py` & `primebotframework-1.0.53/PrimeBot/CpfCnpj/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.50/PrimeBot/CpfCnpj/api_codes.py` & `primebotframework-1.0.53/PrimeBot/CpfCnpj/api_codes.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.50/PrimeBot/D4Sign/__init__.py` & `primebotframework-1.0.53/PrimeBot/D4Sign/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.50/PrimeBot/DeathByCaptcha/__init__.py` & `primebotframework-1.0.53/PrimeBot/DeathByCaptcha/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.50/PrimeBot/Documents/__init__.py` & `primebotframework-1.0.53/PrimeBot/Documents/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.50/PrimeBot/Elastic/__init__.py` & `primebotframework-1.0.53/PrimeBot/Elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.50/PrimeBot/EmailAlert/__init__.py` & `primebotframework-1.0.53/PrimeBot/EmailAlert/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -53,26 +53,28 @@
             Retorna: 
                 str: Caminho do arquivo mais recente.
         """
         files = glob.glob(path_pasta + '\*')
         item_recente = max(files, key=os.path.getctime)
         return item_recente
     
-    def enviar_alerta_de_erro(self, destinatario: str, nome_projeto: str ,mensagem_erro: str) -> None:
+    def enviar_alerta_de_erro(self, destinatario: str, nome_projeto: str, task: str, keyword:str ,mensagem_erro: str) -> None:
         """
             Dispara um email de alerta de erro, caso um processo seja interrompido antes da conclusão do processo.
 
             Atributos:
+                destinatario (str): Endereço de email que receberá a mensagem.
                 nome_projeto (str): Nome do projeto em que houve a falha.
+                task (str): Nome da task que falhou.
+                keyword (str): Nome da keyword processada no momento da falha.
                 mensagem_erro (str): Mensagem retornada pelo processo detalhando o erro.
-                destinatario (str): Endereço de email que receberá a mensagem.
         """
         data = datetime.datetime.now().strftime('%d/%m/%Y')
         hora = datetime.datetime.now().strftime('%H:%M:%S')
-        mensagem = f'<p>Olá, tudo bem?</p><p>Houve um erro durante a execução do processo: {nome_projeto}, que ocasionou a interrupção do mesmo antes de concluir o processo.</p><p>Data: {data}.</p><p>Hora: {hora}.</p><p>Detalhe retornado do erro: {mensagem_erro}.</p>'
+        mensagem = f'<p>Olá, tudo bem?</p><p>Houve um erro durante a execução do processo: {nome_projeto}, que ocasionou a interrupção do mesmo antes de concluir o processo, segue informações:</p><p>Data: {data};</p><p>Hora: {hora};</p><p>Task: {task};</p><p>Keyword: {keyword};</p><p>Detalhe retornado do erro: {mensagem_erro}.</p>'
         html = self.create_html(mensagem)
         to= destinatario
         email = self.sg.create_message(to, f'Azul RPA Erro no projeto: {nome_projeto}', html)
         # Verifica se existe screenshot
         try:
             archives = os.listdir(self.pasta_screenshots)
             if len(archives) > 0:
```

### Comparing `PrimeBotFramework-1.0.50/PrimeBot/ExchangeGraph/__init__.py` & `primebotframework-1.0.53/PrimeBot/ExchangeGraph/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.50/PrimeBot/FeriadosBancarios/__init__.py` & `primebotframework-1.0.53/PrimeBot/FeriadosBancarios/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.50/PrimeBot/IntegracaoSendGrid/__init__.py` & `primebotframework-1.0.53/PrimeBot/IntegracaoSendGrid/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.50/PrimeBot/ListenerECS/__init__.py` & `primebotframework-1.0.53/PrimeBot/ListenerECS/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.50/PrimeBot/OracleDB/__init__.py` & `primebotframework-1.0.53/PrimeBot/OracleDB/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.50/PrimeBot/Vault/__init__.py` & `primebotframework-1.0.53/PrimeBot/Vault/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.50/PrimeBotFramework.egg-info/PKG-INFO` & `primebotframework-1.0.53/PrimeBotFramework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrimeBotFramework
-Version: 1.0.50
+Version: 1.0.53
 Summary: Um pacote de padronizacao de pacotes a serem utilizados pela Prime
 Home-page: 
 Author: Prime Control
 Author-email: 
 License: MIT
 Keywords: PrimeBotFramework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PrimeBotFramework-1.0.50/PrimeBotFramework.egg-info/SOURCES.txt` & `primebotframework-1.0.53/PrimeBotFramework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.50/setup.py` & `primebotframework-1.0.53/setup.py`

 * *Files identical despite different names*

