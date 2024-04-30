# Comparing `tmp/superu-0.0.6.tar.gz` & `tmp/superu-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superu-0.0.6.tar", last modified: Wed Apr 10 14:22:38 2024, max compression
+gzip compressed data, was "superu-0.0.7.tar", last modified: Mon Apr 29 13:24:15 2024, max compression
```

## Comparing `superu-0.0.6.tar` & `superu-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 14:22:38.213631 superu-0.0.6/
--rw-rw-rw-   0        0        0     1084 2024-04-09 12:12:26.000000 superu-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     4165 2024-04-10 14:22:38.213631 superu-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3472 2024-04-10 12:32:15.000000 superu-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 14:22:38.222713 superu-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1250 2024-04-10 14:22:34.000000 superu-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 14:22:38.155578 superu-0.0.6/superu/
--rw-rw-rw-   0        0        0      425 2024-04-10 14:21:54.000000 superu-0.0.6/superu/__init__.py
--rw-rw-rw-   0        0        0     1030 2024-04-09 11:04:22.000000 superu-0.0.6/superu/datetime_util.py
--rw-rw-rw-   0        0        0     1299 2024-04-06 10:19:57.000000 superu-0.0.6/superu/download_models.py
--rw-rw-rw-   0        0        0     1933 2024-04-10 14:21:45.000000 superu-0.0.6/superu/serializer.py
--rw-rw-rw-   0        0        0     1131 2024-04-10 14:21:22.000000 superu-0.0.6/superu/superU.py
--rw-rw-rw-   0        0        0     2260 2024-04-10 14:21:29.000000 superu-0.0.6/superu/superUClient.py
--rw-rw-rw-   0        0        0     3061 2024-04-06 07:39:35.000000 superu-0.0.6/superu/superU_Intent_Classification.py
--rw-rw-rw-   0        0        0     4211 2024-04-10 14:21:19.000000 superu-0.0.6/superu/superU_LLM_Analytics.py
--rw-rw-rw-   0        0        0     4402 2024-04-09 10:37:00.000000 superu-0.0.6/superu/superU_User_Persona.py
-drwxrwxrwx   0        0        0        0 2024-04-10 14:22:38.213631 superu-0.0.6/superu.egg-info/
--rw-rw-rw-   0        0        0     4165 2024-04-10 14:22:37.000000 superu-0.0.6/superu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2024-04-10 14:22:37.000000 superu-0.0.6/superu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 14:22:37.000000 superu-0.0.6/superu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2024-04-10 14:22:37.000000 superu-0.0.6/superu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-10 14:22:37.000000 superu-0.0.6/superu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 13:24:15.308460 superu-0.0.7/
+-rw-rw-rw-   0        0        0     1084 2024-04-09 12:12:26.000000 superu-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     5105 2024-04-29 13:24:15.307452 superu-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4392 2024-04-29 13:22:09.000000 superu-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 13:24:15.308460 superu-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1238 2024-04-29 13:14:32.000000 superu-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 13:24:15.296398 superu-0.0.7/superu/
+-rw-rw-rw-   0        0        0      425 2024-04-10 14:21:54.000000 superu-0.0.7/superu/__init__.py
+-rw-rw-rw-   0        0        0     1030 2024-04-09 11:04:22.000000 superu-0.0.7/superu/datetime_util.py
+-rw-rw-rw-   0        0        0     1299 2024-04-06 10:19:57.000000 superu-0.0.7/superu/download_models.py
+-rw-rw-rw-   0        0        0     1933 2024-04-10 14:21:45.000000 superu-0.0.7/superu/serializer.py
+-rw-rw-rw-   0        0        0     1431 2024-04-29 13:16:27.000000 superu-0.0.7/superu/superU.py
+-rw-rw-rw-   0        0        0     2260 2024-04-10 14:21:29.000000 superu-0.0.7/superu/superUClient.py
+-rw-rw-rw-   0        0        0     3061 2024-04-06 07:39:35.000000 superu-0.0.7/superu/superU_Intent_Classification.py
+-rw-rw-rw-   0        0        0     4211 2024-04-10 14:21:19.000000 superu-0.0.7/superu/superU_LLM_Analytics.py
+-rw-rw-rw-   0        0        0     9263 2024-04-29 13:15:43.000000 superu-0.0.7/superu/superU_User_Persona.py
+drwxrwxrwx   0        0        0        0 2024-04-29 13:24:15.305954 superu-0.0.7/superu.egg-info/
+-rw-rw-rw-   0        0        0     5105 2024-04-29 13:24:15.000000 superu-0.0.7/superu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2024-04-29 13:24:15.000000 superu-0.0.7/superu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 13:24:15.000000 superu-0.0.7/superu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2024-04-29 13:24:15.000000 superu-0.0.7/superu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-29 13:24:15.000000 superu-0.0.7/superu.egg-info/top_level.txt
```

### Comparing `superu-0.0.6/LICENSE` & `superu-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `superu-0.0.6/PKG-INFO` & `superu-0.0.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superu
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package that helps optimize your chatbot response
 Author: SuperU
 Author-email: <adi@superu.ai>
 Keywords: python,chatbot,ecommerce,tag generation,semantic search,openai
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,31 @@
 - Language: {English, Hindi, Mandarin}
 
 
 ## User Persona
 
 This functionality is designed to identify the persona of a user based on their conversations or statements. By analyzing the text, it extracts and identifies key aspects of a user's persona, such as age, gender, profession, hobbies, relationship status, and city.
 
+### Requirements for building user persona with open source LLaMA3
+To inference LLaMA3 on CPU it is necessary to have completed the setup of Ollama.
+1. Ensure you have installed docker on your desktop. You can install it from https://docs.docker.com/engine/install/
+2. Run the below command on your terminal to clone the ollma image on your docker container
+```bash
+docker pull ollama/ollama
+```
+3. Run the docker container using the below command
+```bash
+docker run -d -v ollama:/root/.ollama -p 11434:11434 --name ollama ollama/ollama
+```
+4. Go to Exec/Terminal in docker and run the command to install the LLaMA3 model
+```bash
+ollama run llama3
+```
+5. Once you have completed the above steps, you can successfully build user persona using open source LLaMA3 via Ollama
+
 ### Key data points considered
 - Age
 - Gender
 - City
 - Profession
 - Relationship Status
 - Interests
@@ -72,51 +89,54 @@
 
 ```bash
 pip install superu
 ```
 
 ### Example Usage
 ```python
-from superu import superU as su
 import openai
+import superu
 
 openai.api_type = ""
 openai.api_key = ""
 openai.azure_endpoint = ""
 openai.api_version = ""
+User_Persona_1 = superu.superU.Build_User_Persona_OpenAI(openai, llm_deploymentname='')
+User_Persona_2 = superu.superU.Build_User_Persona_LLaMA3()
+Intent_Classification_1 = superu.superU.Intent_Classification()
+
+prompt = "What is 1 + 1"
+
+intent = Intent_Classification_1.get_intent(prompt)
+user_persona_openai = User_Persona_1.build([prompt])
+user_persona_llama3 = User_Persona_2.build([prompt])
 
-User_Persona = Build_User_Persona(openai, llm_deploymentname='')
-Intent_Classifier = Intent_Classification()
-LLM_Analysis = LLM_Analytics(public_key="", secret_key="")
-
-# Chatbot Session
-user_question = "What is 1 + 1"
-
-intent = Intent_Classification_1.get_intent(user_question)
-user_persona = User_Persona_1.build([user_question])   # List of users previous inputs
 
 messages = [{"role": "system", "content":"You are a helpful assistant."}]
-message_append = {"role": "user", "content": f"{user_question}"}
-messages.append(message_append)
+message_r = {"role": "user", "content": f"{prompt}"}
+messages.append(message_r)
 response = openai.chat.completions.create(model="", messages=messages)
 
-# Format data to build analysis
 data = {
     "input_messages": messages,                                         # Required - Input Messages 
     "output_messages": response.choices[0].message.content,      # Required - the output from the model
     "metadata": {"user": "test-user", "context": "openai testing"},     # Optional - to give some metadata to the conversation
     "model": response.model,                                     # Required - Name of the model
-    "user_id": "",                                                      # Optional - if not given a user_id will be generated
+    "user_id": "pip package test",                                                      # Optional - if not given a user_id will be generated
     "usage": response.usage.model_dump(),                        # Optional - usage details to track the model usage and costs
-    "name": ""                                                          # Optional - to name the given conversation 
+    "name": "test"                                                          # Optional - to name the given conversation 
 }
 
-LLM_Analysis.analyse(data)
+service_client = superu.superU.LLM_Analytics(public_key="", secret_key="")
+
+service_client.analyse(data)
+
 print("Intent: ", intent)
-print("User  Details: ", user_persona)
+print("User Details OpenAI: ", user_persona_openai)
+print("User Details LLaMA3: ", user_persona_llama3)
 
 ```
 
 
 ## Contributing
 
 We welcome contributions to this project! If you have suggestions for improvements or bug fixes, feel free to open an issue or submit a pull request.
```

### Comparing `superu-0.0.6/README.md` & `superu-0.0.7/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -19,14 +19,31 @@
 - Language: {English, Hindi, Mandarin}
 
 
 ## User Persona
 
 This functionality is designed to identify the persona of a user based on their conversations or statements. By analyzing the text, it extracts and identifies key aspects of a user's persona, such as age, gender, profession, hobbies, relationship status, and city.
 
+### Requirements for building user persona with open source LLaMA3
+To inference LLaMA3 on CPU it is necessary to have completed the setup of Ollama.
+1. Ensure you have installed docker on your desktop. You can install it from https://docs.docker.com/engine/install/
+2. Run the below command on your terminal to clone the ollma image on your docker container
+```bash
+docker pull ollama/ollama
+```
+3. Run the docker container using the below command
+```bash
+docker run -d -v ollama:/root/.ollama -p 11434:11434 --name ollama ollama/ollama
+```
+4. Go to Exec/Terminal in docker and run the command to install the LLaMA3 model
+```bash
+ollama run llama3
+```
+5. Once you have completed the above steps, you can successfully build user persona using open source LLaMA3 via Ollama
+
 ### Key data points considered
 - Age
 - Gender
 - City
 - Profession
 - Relationship Status
 - Interests
@@ -55,51 +72,54 @@
 
 ```bash
 pip install superu
 ```
 
 ### Example Usage
 ```python
-from superu import superU as su
 import openai
+import superu
 
 openai.api_type = ""
 openai.api_key = ""
 openai.azure_endpoint = ""
 openai.api_version = ""
+User_Persona_1 = superu.superU.Build_User_Persona_OpenAI(openai, llm_deploymentname='')
+User_Persona_2 = superu.superU.Build_User_Persona_LLaMA3()
+Intent_Classification_1 = superu.superU.Intent_Classification()
+
+prompt = "What is 1 + 1"
+
+intent = Intent_Classification_1.get_intent(prompt)
+user_persona_openai = User_Persona_1.build([prompt])
+user_persona_llama3 = User_Persona_2.build([prompt])
 
-User_Persona = Build_User_Persona(openai, llm_deploymentname='')
-Intent_Classifier = Intent_Classification()
-LLM_Analysis = LLM_Analytics(public_key="", secret_key="")
-
-# Chatbot Session
-user_question = "What is 1 + 1"
-
-intent = Intent_Classification_1.get_intent(user_question)
-user_persona = User_Persona_1.build([user_question])   # List of users previous inputs
 
 messages = [{"role": "system", "content":"You are a helpful assistant."}]
-message_append = {"role": "user", "content": f"{user_question}"}
-messages.append(message_append)
+message_r = {"role": "user", "content": f"{prompt}"}
+messages.append(message_r)
 response = openai.chat.completions.create(model="", messages=messages)
 
-# Format data to build analysis
 data = {
     "input_messages": messages,                                         # Required - Input Messages 
     "output_messages": response.choices[0].message.content,      # Required - the output from the model
     "metadata": {"user": "test-user", "context": "openai testing"},     # Optional - to give some metadata to the conversation
     "model": response.model,                                     # Required - Name of the model
-    "user_id": "",                                                      # Optional - if not given a user_id will be generated
+    "user_id": "pip package test",                                                      # Optional - if not given a user_id will be generated
     "usage": response.usage.model_dump(),                        # Optional - usage details to track the model usage and costs
-    "name": ""                                                          # Optional - to name the given conversation 
+    "name": "test"                                                          # Optional - to name the given conversation 
 }
 
-LLM_Analysis.analyse(data)
+service_client = superu.superU.LLM_Analytics(public_key="", secret_key="")
+
+service_client.analyse(data)
+
 print("Intent: ", intent)
-print("User  Details: ", user_persona)
+print("User Details OpenAI: ", user_persona_openai)
+print("User Details LLaMA3: ", user_persona_llama3)
 
 ```
 
 
 ## Contributing
 
 We welcome contributions to this project! If you have suggestions for improvements or bug fixes, feel free to open an issue or submit a pull request.
```

### Comparing `superu-0.0.6/setup.py` & `superu-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'A package that helps optimize your chatbot response'
 # LONG_DESCRIPTION = 'A package that allows to build simple streams of video, audio and camera data.'
 
 # Setting up
 setup(
     name="superu",
     version=VERSION,
     author="SuperU",
     author_email="<adi@superu.ai>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['sentence_transformers==2.2.2', 'pandas==2.1.1', 'openai==1.16.2', 'torch', 'regex==2023.12.25', 'langchain'],
+    install_requires=['sentence_transformers', 'pandas', 'openai', 'torch', 'regex==2023.12.25', 'langchain', 'ollama'],
     keywords=['python', 'chatbot', 'ecommerce', 'tag generation', 'semantic search', 'openai'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `superu-0.0.6/superu/datetime_util.py` & `superu-0.0.7/superu/datetime_util.py`

 * *Files identical despite different names*

### Comparing `superu-0.0.6/superu/download_models.py` & `superu-0.0.7/superu/download_models.py`

 * *Files identical despite different names*

### Comparing `superu-0.0.6/superu/serializer.py` & `superu-0.0.7/superu/serializer.py`

 * *Files identical despite different names*

### Comparing `superu-0.0.6/superu/superU.py` & `superu-0.0.7/superu/superU.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from superu.download_models import FileDownloader
-from superu.superU_User_Persona import User_Persona
+from superu.superU_User_Persona import User_Persona_OpenAI, User_Persona_LLaMA3
 from superu.superU_Intent_Classification import Intent_Classifier
 from superu.superU_LLM_Analytics import llm_analytics
 
-class Build_User_Persona:
+class Build_User_Persona_OpenAI:
     def __init__(self, openai, llm_deploymentname):
-        self.user_persona = User_Persona(openai, llm_deploymentname)
+        self.user_persona = User_Persona_OpenAI(openai, llm_deploymentname)
         
     def build(self, conversations):
         persona = self.user_persona.analyze_conversation(conversations)
         return persona
+    
+class Build_User_Persona_LLaMA3:
+    def __init__(self):
+        self.user_persona = User_Persona_LLaMA3()
         
+    def build(self, conversations):
+        persona = self.user_persona.analyze_conversation(conversations)
+        return persona        
 
     
 class Intent_Classification:
     def __init__(self):
         self.files = FileDownloader()
         self.files.download_files()
         self.intent_classifier = Intent_Classifier()
```

### Comparing `superu-0.0.6/superu/superUClient.py` & `superu-0.0.7/superu/superUClient.py`

 * *Files identical despite different names*

### Comparing `superu-0.0.6/superu/superU_Intent_Classification.py` & `superu-0.0.7/superu/superU_Intent_Classification.py`

 * *Files identical despite different names*

### Comparing `superu-0.0.6/superu/superU_LLM_Analytics.py` & `superu-0.0.7/superu/superU_LLM_Analytics.py`

 * *Files identical despite different names*

### Comparing `superu-0.0.6/superu.egg-info/PKG-INFO` & `superu-0.0.7/superu.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superu
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package that helps optimize your chatbot response
 Author: SuperU
 Author-email: <adi@superu.ai>
 Keywords: python,chatbot,ecommerce,tag generation,semantic search,openai
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,31 @@
 - Language: {English, Hindi, Mandarin}
 
 
 ## User Persona
 
 This functionality is designed to identify the persona of a user based on their conversations or statements. By analyzing the text, it extracts and identifies key aspects of a user's persona, such as age, gender, profession, hobbies, relationship status, and city.
 
+### Requirements for building user persona with open source LLaMA3
+To inference LLaMA3 on CPU it is necessary to have completed the setup of Ollama.
+1. Ensure you have installed docker on your desktop. You can install it from https://docs.docker.com/engine/install/
+2. Run the below command on your terminal to clone the ollma image on your docker container
+```bash
+docker pull ollama/ollama
+```
+3. Run the docker container using the below command
+```bash
+docker run -d -v ollama:/root/.ollama -p 11434:11434 --name ollama ollama/ollama
+```
+4. Go to Exec/Terminal in docker and run the command to install the LLaMA3 model
+```bash
+ollama run llama3
+```
+5. Once you have completed the above steps, you can successfully build user persona using open source LLaMA3 via Ollama
+
 ### Key data points considered
 - Age
 - Gender
 - City
 - Profession
 - Relationship Status
 - Interests
@@ -72,51 +89,54 @@
 
 ```bash
 pip install superu
 ```
 
 ### Example Usage
 ```python
-from superu import superU as su
 import openai
+import superu
 
 openai.api_type = ""
 openai.api_key = ""
 openai.azure_endpoint = ""
 openai.api_version = ""
+User_Persona_1 = superu.superU.Build_User_Persona_OpenAI(openai, llm_deploymentname='')
+User_Persona_2 = superu.superU.Build_User_Persona_LLaMA3()
+Intent_Classification_1 = superu.superU.Intent_Classification()
+
+prompt = "What is 1 + 1"
+
+intent = Intent_Classification_1.get_intent(prompt)
+user_persona_openai = User_Persona_1.build([prompt])
+user_persona_llama3 = User_Persona_2.build([prompt])
 
-User_Persona = Build_User_Persona(openai, llm_deploymentname='')
-Intent_Classifier = Intent_Classification()
-LLM_Analysis = LLM_Analytics(public_key="", secret_key="")
-
-# Chatbot Session
-user_question = "What is 1 + 1"
-
-intent = Intent_Classification_1.get_intent(user_question)
-user_persona = User_Persona_1.build([user_question])   # List of users previous inputs
 
 messages = [{"role": "system", "content":"You are a helpful assistant."}]
-message_append = {"role": "user", "content": f"{user_question}"}
-messages.append(message_append)
+message_r = {"role": "user", "content": f"{prompt}"}
+messages.append(message_r)
 response = openai.chat.completions.create(model="", messages=messages)
 
-# Format data to build analysis
 data = {
     "input_messages": messages,                                         # Required - Input Messages 
     "output_messages": response.choices[0].message.content,      # Required - the output from the model
     "metadata": {"user": "test-user", "context": "openai testing"},     # Optional - to give some metadata to the conversation
     "model": response.model,                                     # Required - Name of the model
-    "user_id": "",                                                      # Optional - if not given a user_id will be generated
+    "user_id": "pip package test",                                                      # Optional - if not given a user_id will be generated
     "usage": response.usage.model_dump(),                        # Optional - usage details to track the model usage and costs
-    "name": ""                                                          # Optional - to name the given conversation 
+    "name": "test"                                                          # Optional - to name the given conversation 
 }
 
-LLM_Analysis.analyse(data)
+service_client = superu.superU.LLM_Analytics(public_key="", secret_key="")
+
+service_client.analyse(data)
+
 print("Intent: ", intent)
-print("User  Details: ", user_persona)
+print("User Details OpenAI: ", user_persona_openai)
+print("User Details LLaMA3: ", user_persona_llama3)
 
 ```
 
 
 ## Contributing
 
 We welcome contributions to this project! If you have suggestions for improvements or bug fixes, feel free to open an issue or submit a pull request.
```

