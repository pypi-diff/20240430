# Comparing `tmp/alita_sdk-0.1.0.tar.gz` & `tmp/alita_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alita_sdk-0.1.0.tar", last modified: Wed Apr 24 11:06:08 2024, max compression
+gzip compressed data, was "alita_sdk-0.1.1.tar", last modified: Tue Apr 30 17:56:01 2024, max compression
```

## Comparing `alita_sdk-0.1.0.tar` & `alita_sdk-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:06:08.879981 alita_sdk-0.1.0/
--rw-r--r--   0 arozumenko   (501) staff       (20)    11357 2024-03-08 11:24:37.000000 alita_sdk-0.1.0/LICENSE
--rw-r--r--   0 arozumenko   (501) staff       (20)     3939 2024-04-24 11:06:08.879762 alita_sdk-0.1.0/PKG-INFO
--rw-r--r--   0 arozumenko   (501) staff       (20)     3200 2024-03-10 12:01:09.000000 alita_sdk-0.1.0/README.md
--rw-r--r--   0 arozumenko   (501) staff       (20)      705 2024-04-23 06:09:40.000000 alita_sdk-0.1.0/pyproject.toml
--rw-r--r--   0 arozumenko   (501) staff       (20)      111 2024-04-24 11:05:21.000000 alita_sdk-0.1.0/requirements.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)       38 2024-04-24 11:06:08.880028 alita_sdk-0.1.0/setup.cfg
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:06:08.872859 alita_sdk-0.1.0/src/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:38.000000 alita_sdk-0.1.0/src/__init__.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:06:08.872964 alita_sdk-0.1.0/src/alita_sdk/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:50.000000 alita_sdk-0.1.0/src/alita_sdk/__init__.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:06:08.875017 alita_sdk-0.1.0/src/alita_sdk/agents/
--rw-r--r--   0 arozumenko   (501) staff       (20)     2412 2024-03-18 10:31:52.000000 alita_sdk-0.1.0/src/alita_sdk/agents/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     3030 2024-03-26 19:45:28.000000 alita_sdk-0.1.0/src/alita_sdk/agents/alita_openai.py
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-10 11:28:03.000000 alita_sdk-0.1.0/src/alita_sdk/agents/base_actions.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     2566 2024-04-03 10:33:12.000000 alita_sdk-0.1.0/src/alita_sdk/agents/mixedAgentParser.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     2283 2024-03-18 10:31:02.000000 alita_sdk-0.1.0/src/alita_sdk/agents/mixedAgentRenderes.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     1231 2024-03-13 15:14:36.000000 alita_sdk-0.1.0/src/alita_sdk/agents/utils.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:06:08.875266 alita_sdk-0.1.0/src/alita_sdk/clients/
--rw-r--r--   0 arozumenko   (501) staff       (20)       31 2024-03-09 15:53:40.000000 alita_sdk-0.1.0/src/alita_sdk/clients/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)    17120 2024-04-23 06:28:54.000000 alita_sdk-0.1.0/src/alita_sdk/clients/client.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:06:08.875955 alita_sdk-0.1.0/src/alita_sdk/llms/
--rw-r--r--   0 arozumenko   (501) staff       (20)       33 2024-03-09 14:45:23.000000 alita_sdk-0.1.0/src/alita_sdk/llms/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     8317 2024-03-26 15:53:02.000000 alita_sdk-0.1.0/src/alita_sdk/llms/alita.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:06:08.876981 alita_sdk-0.1.0/src/alita_sdk/toolkits/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-04-12 11:47:05.000000 alita_sdk-0.1.0/src/alita_sdk/toolkits/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     1985 2024-04-12 12:00:03.000000 alita_sdk-0.1.0/src/alita_sdk/toolkits/datasource.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      734 2024-04-12 11:47:16.000000 alita_sdk-0.1.0/src/alita_sdk/toolkits/prompt.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:06:08.878581 alita_sdk-0.1.0/src/alita_sdk/tools/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-11 07:45:42.000000 alita_sdk-0.1.0/src/alita_sdk/tools/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      743 2024-04-12 14:28:55.000000 alita_sdk-0.1.0/src/alita_sdk/tools/datasource.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      281 2024-04-12 14:28:45.000000 alita_sdk-0.1.0/src/alita_sdk/tools/prompt.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:06:08.879172 alita_sdk-0.1.0/src/alita_sdk/utils/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:37.000000 alita_sdk-0.1.0/src/alita_sdk/utils/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)    10148 2024-04-04 04:14:44.000000 alita_sdk-0.1.0/src/alita_sdk/utils/streamlit.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:06:08.879484 alita_sdk-0.1.0/src/alita_sdk.egg-info/
--rw-r--r--   0 arozumenko   (501) staff       (20)     3939 2024-04-24 11:06:08.000000 alita_sdk-0.1.0/src/alita_sdk.egg-info/PKG-INFO
--rw-r--r--   0 arozumenko   (501) staff       (20)      887 2024-04-24 11:06:08.000000 alita_sdk-0.1.0/src/alita_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)        1 2024-04-24 11:06:08.000000 alita_sdk-0.1.0/src/alita_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)      112 2024-04-24 11:06:08.000000 alita_sdk-0.1.0/src/alita_sdk.egg-info/requires.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)       19 2024-04-24 11:06:08.000000 alita_sdk-0.1.0/src/alita_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-30 17:56:01.313858 alita_sdk-0.1.1/
+-rw-r--r--   0 arozumenko   (501) staff       (20)    11357 2024-03-08 11:24:37.000000 alita_sdk-0.1.1/LICENSE
+-rw-r--r--   0 arozumenko   (501) staff       (20)     4063 2024-04-30 17:56:01.313598 alita_sdk-0.1.1/PKG-INFO
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3200 2024-03-10 12:01:09.000000 alita_sdk-0.1.1/README.md
+-rw-r--r--   0 arozumenko   (501) staff       (20)      705 2024-04-30 17:55:53.000000 alita_sdk-0.1.1/pyproject.toml
+-rw-r--r--   0 arozumenko   (501) staff       (20)      175 2024-04-30 17:55:06.000000 alita_sdk-0.1.1/requirements.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)       38 2024-04-30 17:56:01.313909 alita_sdk-0.1.1/setup.cfg
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-30 17:56:01.280529 alita_sdk-0.1.1/src/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:38.000000 alita_sdk-0.1.1/src/__init__.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-30 17:56:01.280633 alita_sdk-0.1.1/src/alita_sdk/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:50.000000 alita_sdk-0.1.1/src/alita_sdk/__init__.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-30 17:56:01.282655 alita_sdk-0.1.1/src/alita_sdk/agents/
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2412 2024-03-18 10:31:52.000000 alita_sdk-0.1.1/src/alita_sdk/agents/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3122 2024-04-30 17:52:10.000000 alita_sdk-0.1.1/src/alita_sdk/agents/alita_openai.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-10 11:28:03.000000 alita_sdk-0.1.1/src/alita_sdk/agents/base_actions.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3095 2024-04-30 17:52:10.000000 alita_sdk-0.1.1/src/alita_sdk/agents/mixedAgentParser.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2283 2024-03-18 10:31:02.000000 alita_sdk-0.1.1/src/alita_sdk/agents/mixedAgentRenderes.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     1169 2024-04-30 17:52:10.000000 alita_sdk-0.1.1/src/alita_sdk/agents/utils.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-30 17:56:01.285219 alita_sdk-0.1.1/src/alita_sdk/clients/
+-rw-r--r--   0 arozumenko   (501) staff       (20)       31 2024-03-09 15:53:40.000000 alita_sdk-0.1.1/src/alita_sdk/clients/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)    17899 2024-04-30 17:52:10.000000 alita_sdk-0.1.1/src/alita_sdk/clients/client.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-30 17:56:01.291137 alita_sdk-0.1.1/src/alita_sdk/llms/
+-rw-r--r--   0 arozumenko   (501) staff       (20)       33 2024-03-09 14:45:23.000000 alita_sdk-0.1.1/src/alita_sdk/llms/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     8383 2024-04-30 17:52:10.000000 alita_sdk-0.1.1/src/alita_sdk/llms/alita.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-30 17:56:01.291669 alita_sdk-0.1.1/src/alita_sdk/toolkits/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-04-12 11:47:05.000000 alita_sdk-0.1.1/src/alita_sdk/toolkits/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     1985 2024-04-12 12:00:03.000000 alita_sdk-0.1.1/src/alita_sdk/toolkits/datasource.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      734 2024-04-12 11:47:16.000000 alita_sdk-0.1.1/src/alita_sdk/toolkits/prompt.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-30 17:56:01.294979 alita_sdk-0.1.1/src/alita_sdk/tools/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-11 07:45:42.000000 alita_sdk-0.1.1/src/alita_sdk/tools/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      743 2024-04-12 14:28:55.000000 alita_sdk-0.1.1/src/alita_sdk/tools/datasource.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      281 2024-04-12 14:28:45.000000 alita_sdk-0.1.1/src/alita_sdk/tools/prompt.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-30 17:56:01.299229 alita_sdk-0.1.1/src/alita_sdk/utils/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:37.000000 alita_sdk-0.1.1/src/alita_sdk/utils/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)    10148 2024-04-04 04:14:44.000000 alita_sdk-0.1.1/src/alita_sdk/utils/streamlit.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-04-30 17:56:01.313208 alita_sdk-0.1.1/src/alita_sdk.egg-info/
+-rw-r--r--   0 arozumenko   (501) staff       (20)     4063 2024-04-30 17:56:01.000000 alita_sdk-0.1.1/src/alita_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 arozumenko   (501) staff       (20)      887 2024-04-30 17:56:01.000000 alita_sdk-0.1.1/src/alita_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)        1 2024-04-30 17:56:01.000000 alita_sdk-0.1.1/src/alita_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)      176 2024-04-30 17:56:01.000000 alita_sdk-0.1.1/src/alita_sdk.egg-info/requires.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)       19 2024-04-30 17:56:01.000000 alita_sdk-0.1.1/src/alita_sdk.egg-info/top_level.txt
```

### Comparing `alita_sdk-0.1.0/LICENSE` & `alita_sdk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.0/PKG-INFO` & `alita_sdk-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: alita_sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: SDK for building langchain agents using resouces from Alita
 Author-email: Artem Rozumenko <support@analysta.ai>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/alita-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: langchain_core==0.1.30
-Requires-Dist: langchain==0.1.11
-Requires-Dist: tiktoken==0.6.0
+Requires-Dist: langchain_core~=0.1.30
+Requires-Dist: langchain~=0.1.12
+Requires-Dist: tiktoken~=0.6.0
 Requires-Dist: openai==1.13.3
-Requires-Dist: python-dotenv==1.0.1
-Requires-Dist: alita_tools==0.0.9
+Requires-Dist: python-dotenv~=1.0.1
+Requires-Dist: alita_tools>=0.0.10
+Requires-Dist: jinja2~=3.1.3
+Requires-Dist: pillow~=10.2.0
+Requires-Dist: requests~=2.31.0
+Requires-Dist: pydantic~=1.10.9
 
 Alita SDK
 =========
 
 Alita SDK, built on top of Langchain, enables the creation of intelligent agents within the Alita Platform using project-specific prompts and data sources. This SDK is designed for developers looking to integrate advanced AI capabilities into their projects with ease.
 
 Prerequisites
```

### Comparing `alita_sdk-0.1.0/README.md` & `alita_sdk-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.0/pyproject.toml` & `alita_sdk-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alita_sdk"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Artem Rozumenko", email="support@analysta.ai" },
 ]
 description = "SDK for building langchain agents using resouces from Alita"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `alita_sdk-0.1.0/src/alita_sdk/agents/__init__.py` & `alita_sdk-0.1.1/src/alita_sdk/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.0/src/alita_sdk/agents/alita_openai.py` & `alita_sdk-0.1.1/src/alita_sdk/agents/alita_openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,19 @@
             dumpd(self), input, name=config.get("run_name")
         )
         messages = []
         if input.get("intermediate_steps"):
             messages = format_to_messages(input["intermediate_steps"])
         print(input)
         try:
-            mgs = self.chat_history + input["chat_history"][:-1] + messages + [input["chat_history"][-1]]
+            mgs = self.chat_history + input["chat_history"][:-1] + messages
+            try:
+                mgs.append(input["chat_history"][-1])
+            except IndexError:
+                ...
             callback_manager.on_llm_start(dumpd(self), [message["content"] for message in mgs])
             run = self._create_thread_and_run(mgs)
             response = self._get_response(run)
         except BaseException as e:
             run_manager.on_chain_error(e, metadata=format_exc())
             raise e
         else:
```

### Comparing `alita_sdk-0.1.0/src/alita_sdk/agents/mixedAgentParser.py` & `alita_sdk-0.1.1/src/alita_sdk/agents/mixedAgentParser.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from langchain_core.agents import AgentAction, AgentFinish
 from langchain_core.exceptions import OutputParserException
 
 from langchain.agents.agent import AgentOutputParser
 
 from .utils import unpack_json
 
-
 FORMAT_INSTRUCTIONS = """Respond only with JSON format as described below
 {
     "thoughts": {
         "text": "message to a user in crisp and clear business language",
         "plan": "short bulleted, list that conveys long-term plan",
         "criticism": "constructive self-criticism",
     },
@@ -23,62 +22,74 @@
     }
 }
 
 You must answer with only JSON and it could be parsed by Python json.loads
 """
 
 
+class UnexpectedResponseError(Exception):
+    pass
+
+
 class MixedAgentOutputParser(AgentOutputParser):
     """ Parser for JSON Style Communication Agent """
 
     def get_format_instructions(self) -> str:
         return FORMAT_INSTRUCTIONS
 
     def parse(self, text: str) -> Union[AgentAction, AgentFinish]:
         try:
             response = unpack_json(text)
         except json.decoder.JSONDecodeError:
             text.replace("\n", "\\n")
             response = unpack_json(text)
-        action = response.get("tool", {"name": None}).get("name")
-        tool_input = response.get("tool", {"args": {}}).get("args")
-        plan = response.get("thoughts", {"plan": []}).get("plan")
+        if not isinstance(response, dict):
+            raise UnexpectedResponseError(f'Could not parse response: {response}')
+        tool: dict | str = response.get("tool", {})
+        if isinstance(tool, dict):
+            action: str | None = tool.get("name")
+            tool_input: dict = tool.get("args", {})
+        elif isinstance(tool, str):
+            action: str | None = tool
+            tool_input: dict = response.get("args", {})
+        else:
+            raise UnexpectedResponseError(f'Unexpected response {response}')
+        thoughts = response.get("thoughts", {})
+        if not isinstance(thoughts, dict):
+            raise UnexpectedResponseError(f'Unexpected response {response}')
+        plan: list | str = thoughts.get("plan", [])
         if isinstance(plan, list):
-            plan = "\n".join(plan)
-        txt = response.get("thoughts", {"text": ""}).get("text")
-        criticism = response.get("thoughts", {"criticism": ""}).get("criticism")
-        log = f"""Step Details:
+            plan: str = "\n".join(plan)
+        txt: str = thoughts.get("text", '')
+        criticism: str = thoughts.get("criticism", '')
+        log: str = f"""Step Details:
 {txt}
 Long Term Plan:
 {plan}
 Criticism:
 {criticism}
 
 Running Tool:
 {action} with param {tool_input}
 """
-        if action:
-            if action == 'complete_task':
-                
-                try:
-                    output = tool_input[list(tool_input.keys())[0]]
-                except AttributeError:
-                    output = tool_input
-                if output.strip() == "final_answer":
-                    output = txt
-                return AgentFinish({"output": output}, log=log)  
+        if action == 'complete_task':
+            try:
+                output: str = tool_input[list(tool_input.keys())[0]]
+            except AttributeError:
+                output: str = tool_input
+            if output.strip() == "final_answer":
+                output = txt
+            return AgentFinish({"output": output}, log=log)
+        elif action:
             return AgentAction(action, tool_input, log)
         elif txt:
             return AgentFinish({"output": txt}, log=log)
         else:
             raise OutputParserException(f"""ERROR: RESPONSE FORMAT IS INCORRECT
 The response may have a great data, format response to the required JSON strcuture. 
 Expected format: {FORMAT_INSTRUCTIONS}
 
 Recieved data: {response}""")
 
     @property
     def _type(self) -> str:
         return "mixed-agent-parser"
-
-
-
```

### Comparing `alita_sdk-0.1.0/src/alita_sdk/agents/mixedAgentRenderes.py` & `alita_sdk-0.1.1/src/alita_sdk/agents/mixedAgentRenderes.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.0/src/alita_sdk/agents/utils.py` & `alita_sdk-0.1.1/src/alita_sdk/agents/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-
 import logging
 import json
 import re
 
 logger = logging.getLogger(__name__)
 
-def unpack_json(json_data, message_key=None):
-    if (isinstance(json_data, str)):
+
+def unpack_json(json_data: str | dict, message_key=None):
+    if isinstance(json_data, str):
         if '```json' in json_data:
             pattern = r'```json(.*)```'
             matches = re.findall(pattern, json_data, re.DOTALL)
             try:
                 text = json_data.replace(f'{matches[0]}', '').replace('```json', '').replace('```', '').strip()
                 res = json.loads(matches[0])
                 if message_key and text:
                     txt = "\n".join([match.value for match in message_key.find(res)])
                     message_key.update(res, txt + text)
                 return res
             except IndexError:
                 logger.error(f"Error in unpacking json: {json_data}")
-                raise ValueError("Wrong type of json_data")        
+                raise ValueError("Wrong type of json_data")
         try:
             return json.loads(json_data)
-        except json.decoder.JSONDecodeError:
+        except json.decoder.JSONDecodeError as e:
             logger.error(f"Error in unpacking json: {json_data}")
-            raise json.decoder.JSONDecodeError(f"Error in unpacking json: {json_data}")
-    elif (isinstance(json_data, dict)):
+            raise e
+    elif isinstance(json_data, dict):
         return json_data
     else:
-        raise ValueError("Wrong type of json_data")
+        raise ValueError("Wrong type of json_data")
```

### Comparing `alita_sdk-0.1.0/src/alita_sdk/clients/client.py` & `alita_sdk-0.1.1/src/alita_sdk/clients/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,28 +8,30 @@
     AIMessage,
     HumanMessage,
     SystemMessage,
     BaseMessage,
     ToolMessage
 )
 from langchain_core.prompts import ChatPromptTemplate
-from langchain.agents import  AgentExecutor
+from langchain.agents import AgentExecutor
 from langchain_core.utils.function_calling import convert_to_openai_function
 
-logger = logging.getLogger(__name__)
 from ..agents import create_mixed_agent
 from ..agents.alita_openai import AlitaAssistantRunnable
 from ..toolkits.prompt import PromptToolkit
 from ..toolkits.datasource import DatasourcesToolkit
 from alita_tools.openapi import AlitaOpenAPIToolkit
 from pydantic import create_model
 
+logger = logging.getLogger(__name__)
+
+
 class Jinja2TemplatedChatMessagesTemplate(ChatPromptTemplate):
-    
-    def _resolve_variables(self, message:BaseMessage, kwargs:Dict) -> BaseMessage:
+
+    def _resolve_variables(self, message: BaseMessage, kwargs: Dict) -> BaseMessage:
         environment = Environment(undefined=DebugUndefined)
         template = environment.from_string(message.content)
         content = template.render(kwargs)
         if isinstance(message, SystemMessage):
             return SystemMessage(content=content)
         elif isinstance(message, AIMessage):
             return AIMessage(content=content)
@@ -54,115 +56,118 @@
         result = []
         for message_template in self.messages:
             if isinstance(message_template, BaseMessage):
                 message = self._resolve_variables(message_template, kwargs)
                 logger.debug(message.content)
                 result.append(message)
         return result
-    
+
 
 class AlitaDataSource:
-    def __init__(self, alita:Any, datasource_id:int, name:str, description: str,
+    def __init__(self, alita: Any, datasource_id: int, name: str, description: str,
                  datasource_settings, datasource_predict_settings):
         self.alita = alita
         self.name = name
         self.description = description
         self.datasource_id = datasource_id
         self.datasource_settings = datasource_settings
         self.datasource_predict_settings = datasource_predict_settings
-    
-    def predict(self, user_input: str, chat_history: Optional[list[BaseMessage]]=[]):
+
+    def predict(self, user_input: str, chat_history: Optional[list] = None):
+        if chat_history is None:
+            chat_history = []
         messages = chat_history + [HumanMessage(content=user_input)]
-        return self.alita.rag(self.datasource_id, messages, 
-                              self.datasource_settings, 
+        return self.alita.rag(self.datasource_id, messages,
+                              self.datasource_settings,
                               self.datasource_predict_settings)
-        
+
     def search(self, query: str):
-        return self.alita.search(self.datasource_id, [HumanMessage(content=query)], 
-                                  self.datasource_settings)
-        
+        return self.alita.search(self.datasource_id, [HumanMessage(content=query)],
+                                 self.datasource_settings)
+
 
 class AlitaPrompt:
-    def __init__(self, alita:Any, prompt: ChatPromptTemplate, name:str, description: str, llm_settings: dict):
+    def __init__(self, alita: Any, prompt: ChatPromptTemplate, name: str, description: str, llm_settings: dict):
         self.alita = alita
         self.prompt = prompt
         self.name = name
         self.llm_settings = llm_settings
         self.description = description
-    
+
     def create_pydantic_model(self):
         fields = {}
         for variable in self.prompt.input_variables:
             fields[variable] = (str, None)
         if "input" not in list(fields.keys()):
             fields["input"] = (str, None)
         return create_model("PromptVariables", **fields)
-        
-    
-    def predict(self, variables: dict={}):
-        input = variables.pop("input", None)
+
+    def predict(self, variables: Optional[dict] = None):
+        if variables is None:
+            variables = {}
+        user_input = variables.pop("input", '')
         alita_vars = []
         for key, value in variables.items():
             alita_vars.append({
                 "name": key,
                 "value": value
             })
-        messages = [SystemMessage(content=self.prompt.messages[0].content), HumanMessage(content=input)]
+        messages = [SystemMessage(content=self.prompt.messages[0].content), HumanMessage(content=user_input)]
         result = []
         for message in self.alita.predict(messages, self.llm_settings, variables=alita_vars):
             result.append(message.content)
         return "\n\n".join(result)
 
 
 class Assistant:
-    def __init__(self, client:Any, prompt:ChatPromptTemplate, tools: list, 
-                 openai_tools: Optional[Dict]=None):
+    def __init__(self, client: Any, prompt: ChatPromptTemplate, tools: list,
+                 openai_tools: Optional[Dict] = None):
         self.prompt = prompt
         self.client = client
         self.tools = tools
         self.openai_tools = openai_tools
-    
+
     def getAgentExecutor(self):
         agent = create_mixed_agent(llm=self.client, tools=self.tools, prompt=self.prompt)
         return AgentExecutor.from_agent_and_tools(agent=agent, tools=self.tools,
-                                                  verbose=True, handle_parsing_errors=True, 
+                                                  verbose=True, handle_parsing_errors=True,
                                                   max_execution_time=None, return_intermediate_steps=True)
-        
+
     def getOpenAIAgentExecutor(self):
         agent = AlitaAssistantRunnable(client=self.client, assistant=self)
         return AgentExecutor.from_agent_and_tools(agent=agent, tools=self.tools,
-                                                  verbose=True, handle_parsing_errors=True, 
+                                                  verbose=True, handle_parsing_errors=True,
                                                   max_execution_time=None,
                                                   return_intermediate_steps=True)
-    
+
     # This one is used only in Alita OpenAI
     def apredict(self, messages: list[BaseMessage]):
         yield from self.client.ainvoke([self.prompt.messages[0]] + messages, functions=self.openai_tools)
-    
+
     def predict(self, messages: list[BaseMessage]):
         response = self.client.invoke([self.prompt.messages[0]] + messages, functions=self.openai_tools)
         return response
-    
+
 
 class AlitaClient:
     def __init__(self, base_url: str, project_id: int, auth_token: str):
-        self.base_url = base_url
+        self.base_url = base_url.rstrip('/')
+        self.api_path = '/api/v1'
         self.project_id = project_id
-        self.auth_token = auth_token        
+        self.auth_token = auth_token
         self.headers = {
             "Authorization": f"Bearer {auth_token}"
         }
-        self.predict_url = f"{self.base_url}/api/v1/prompt_lib/predict/prompt_lib/{self.project_id}"
-        self.prompt_versions = f"{self.base_url}/api/v1/prompt_lib/version/prompt_lib/{self.project_id}"
-        self.prompts = f"{self.base_url}/api/v1/prompt_lib/prompt/prompt_lib/{self.project_id}"
-        self.datasources = f"{self.base_url}/api/v1/datasources/datasource/prompt_lib/{self.project_id}"
-        self.datasources_predict = f"{self.base_url}/api/v1/datasources/predict/prompt_lib/{self.project_id}"
-        self.datasources_search = f"{self.base_url}/api/v1/datasources/search/prompt_lib/{self.project_id}"
-        self.application_versions = f"{self.base_url}/api/v1/applications/version/prompt_lib/{self.project_id}"
-        
+        self.predict_url = f"{self.base_url}{self.api_path}/prompt_lib/predict/prompt_lib/{self.project_id}"
+        self.prompt_versions = f"{self.base_url}{self.api_path}/prompt_lib/version/prompt_lib/{self.project_id}"
+        self.prompts = f"{self.base_url}{self.api_path}/prompt_lib/prompt/prompt_lib/{self.project_id}"
+        self.datasources = f"{self.base_url}{self.api_path}/datasources/datasource/prompt_lib/{self.project_id}"
+        self.datasources_predict = f"{self.base_url}{self.api_path}/datasources/predict/prompt_lib/{self.project_id}"
+        self.datasources_search = f"{self.base_url}{self.api_path}/datasources/search/prompt_lib/{self.project_id}"
+        self.application_versions = f"{self.base_url}{self.api_path}/applications/version/prompt_lib/{self.project_id}"
 
     def prompt(self, prompt_id, prompt_version_id, chat_history=None, return_tool=False):
         url = f"{self.prompt_versions}/{prompt_id}/{prompt_version_id}"
         data = requests.get(url, headers=self.headers).json()
         model_settings = data['model_settings']
         messages = [SystemMessage(content=data['context'])]
         variables = {}
@@ -170,15 +175,15 @@
             for message in data['messages']:
                 if message.get('role') == 'assistant':
                     messages.append(AIMessage(content=message['content']))
                 elif message.get('role') == 'user':
                     messages.append(HumanMessage(content=message['content']))
                 else:
                     messages.append(SystemMessage(content=message['content']))
-        if chat_history and isinstance(chat_history, list[BaseMessage]):
+        if chat_history and isinstance(chat_history, list):
             messages.extend(chat_history)
         input_variables = []
         for variable in data['variables']:
             if variable['value']:
                 variables[variable['name']] = variable['value']
             else:
                 input_variables.append(variable['name'])
@@ -190,16 +195,17 @@
         if not return_tool:
             return template
         else:
             url = f"{self.prompts}/{prompt_id}"
             data = requests.get(url, headers=self.headers).json()
             return AlitaPrompt(self, template, data['name'], data['description'], model_settings)
 
-    
-    def application(self, client: Any, application_id:int, application_version_id:int, tools: Optional[list] = []):
+    def application(self, client: Any, application_id: int, application_version_id: int, tools: Optional[list] = None):
+        if tools is None:
+            tools = []
         url = f"{self.application_versions}/{application_id}/{application_version_id}"
         data = requests.get(url, headers=self.headers).json()
         messages = [SystemMessage(content=data['instructions'])]
         variables = {}
         input_variables = []
         for variable in data['variables']:
             print(variable)
@@ -215,52 +221,64 @@
         if input_variables:
             prompt_type = 'react'
         else:
             prompt_type = 'openai'
         prompts = []
         for tool in data['tools']:
             if tool['type'] == 'prompt':
-                prompts.append([tool['settings']['prompt_id'], tool['settings']['prompt_version_id']])
+                prompts.append([
+                    int(tool['settings']['prompt_id']),
+                    int(tool['settings']['prompt_version_id'])
+                ])
             elif tool['type'] == 'datasource':
-                tools += DatasourcesToolkit.get_toolkit(self, [tool['settings']['datasource_id']], tool['settings']['actions']).get_tools()
+                tools.extend(DatasourcesToolkit.get_toolkit(
+                    self,
+                    datasource_ids=[int(tool['settings']['datasource_id'])],
+                    selected_tools=tool['settings']['selected_tools']
+                ).get_tools())
             elif tool['type'] == 'openapi':
                 headers = {}
                 if tool['settings'].get('authentication'):
-                    if tool['settings']['authentication']['type'] == 'api_key': 
+                    if tool['settings']['authentication']['type'] == 'api_key':
                         auth_type = tool['settings']['authentication']['settings']['auth_type']
                         auth_key = tool["settings"]["authentication"]["settings"]["api_key"]
                         if auth_type.lower() == 'bearer':
                             headers['Authorization'] = f'Bearer {auth_key}'
                         if auth_type.lower() == 'basic':
                             headers['Authorization'] = f'Basic {auth_key}'
                         if auth_type.lower() == 'custom':
-                            headers[tool["settings"]["authentication"]["settings"]["custom_header_name"]] = f'{auth_key}'  
-                tools += AlitaOpenAPIToolkit.get_toolkit(tool['settings']['schema_settings'], headers={}).get_tools()
+                            headers[
+                                tool["settings"]["authentication"]["settings"]["custom_header_name"]] = f'{auth_key}'
+                tools.extend(AlitaOpenAPIToolkit.get_toolkit(
+                    openapi_spec=tool['settings']['schema_settings'],
+                    selected_tools=tool['settings'].get('selected_tools', []),
+                    headers={}
+                ).get_tools())
         if len(prompts) > 0:
-            tools += PromptToolkit.get_toolkit(self, prompts).get_tools() 
+            tools += PromptToolkit.get_toolkit(self, prompts).get_tools()
         if prompt_type == 'openai':
             open_ai_funcs = [convert_to_openai_function(t) for t in tools]
             return Assistant(client, template, tools, open_ai_funcs).getOpenAIAgentExecutor()
         else:
             return Assistant(client, template, tools).getAgentExecutor()
 
-    def datasource(self, datasource_id:int) -> AlitaDataSource:
+    def datasource(self, datasource_id: int) -> AlitaDataSource:
         url = f"{self.datasources}/{datasource_id}"
         data = requests.get(url, headers=self.headers).json()
         datasource_model = data['version_details']['datasource_settings']['chat']['chat_settings_embedding']
         chat_model = data['version_details']['datasource_settings']['chat']['chat_settings_ai']
         return AlitaDataSource(self, datasource_id, data["name"], data["description"],
                                datasource_model, chat_model)
-    
-    def assistant(self, prompt_id: int, prompt_version_id: int, 
-                  tools: list, openai_tools: Optional[Dict]=None, 
+
+    def assistant(self, prompt_id: int, prompt_version_id: int,
+                  tools: list, openai_tools: Optional[Dict] = None,
                   client: Optional[Any] = None):
         prompt = self.prompt(prompt_id=prompt_id, prompt_version_id=prompt_version_id)
         return Assistant(client, prompt, tools, openai_tools)
-    
+
     def _prepare_messages(self, messages: list[BaseMessage]):
         context = ''
         chat_history = []
         if messages[0].type == "system":
             context = messages[0].content
         for message in messages[1:-1]:
             if message.type == 'human':
@@ -276,45 +294,45 @@
             else:
                 chat_history.append({
                     'role': 'assistant',
                     'content': message.content
                 })
         user_input = messages[-1].content
         return context, chat_history, user_input
-    
-    def _prepare_payload(self, messages: list[BaseMessage], model_settings: dict, variables: dict):
+
+    def _prepare_payload(self, messages: list[BaseMessage], model_settings: dict, variables: list[dict]):
         context, chat_history, user_input = self._prepare_messages(messages)
         if not variables:
             variables = []
         return {
             "type": "chat",
             "project_id": self.project_id,
             "context": context,
             "model_settings": model_settings,
             "user_input": user_input,
             "chat_history": chat_history,
             "variables": variables,
             "format_response": True
         }
-        
-    def async_predict(self, messages: list[BaseMessage], model_settings: dict, variables: list[dict]=None):
+
+    def async_predict(self, messages: list[BaseMessage], model_settings: dict, variables: list[dict] = None):
         # TODO: Modify to make it appropriate stream response
         prompt_data = self._prepare_payload(messages, model_settings, variables)
         response = requests.post(self.predict_url, headers=self.headers, json=prompt_data)
         logger.info(response.content)
         response_data = response.json()
         for message in response_data['messages']:
             if message.get('role') == 'user':
                 yield HumanMessage(content=message['content'])
             else:
                 yield AIMessage(content=message['content'])
-    
-    def predict(self, messages: list[BaseMessage], model_settings: dict, variables: list[dict]=None):
+
+    def predict(self, messages: list[BaseMessage], model_settings: dict, variables: list[dict] = None):
         prompt_data = self._prepare_payload(messages, model_settings, variables)
-        
+
         response = requests.post(self.predict_url, headers=self.headers, json=prompt_data)
         if response.status_code != 200:
             logger.error("Error in response of predict: {response.content}")
             raise requests.exceptions.HTTPError(response.content)
         try:
             response_data = response.json()
             response_messages = []
@@ -322,42 +340,47 @@
             for message in response_data['messages']:
                 if message.get('type') == 'user':
                     response_messages.append(HumanMessage(content=message['content']))
                 else:
                     response_messages.append(AIMessage(content=message['content']))
             return response_messages
         except TypeError:
-            logger.error(f"TypeError in response of predict: {response_data}")
+            logger.error(f"TypeError in response of predict: {response.content}")
             raise
-    
-    def rag(self, datasource_id:int, messages:list[BaseMessage], 
-        datasource_settings: dict, datasource_predict_settings: dict):
+
+    def rag(self, datasource_id: int, messages: list[BaseMessage],
+            datasource_settings: dict, datasource_predict_settings: dict):
         context, chat_history, user_input = self._prepare_messages(messages)
         data = {
             "input": user_input,
             "context": '',
             "chat_history": chat_history,
             "chat_settings_ai": datasource_predict_settings,
             "chat_settings_embedding": datasource_settings
         }
         if context:
             data['context'] = context
         headers = self.headers | {"Content-Type": "application/json"}
         response = requests.post(f"{self.datasources_predict}/{datasource_id}", headers=headers, json=data).json()
         return AIMessage(content=response['response'], additional_kwargs={"references": response['references']})
-    
-    def search(self, datasource_id:int, messages:list[BaseMessage], datasource_settings: dict):
+
+    def search(self, datasource_id: int, messages: list[BaseMessage], datasource_settings: dict) -> AIMessage:
         _, _, user_input = self._prepare_messages(messages)
         data = {
             "chat_history": [
                 {
                     "role": "user",
                     "content": user_input
                 }
             ],
             "chat_settings_embedding": datasource_settings,
             "str_content": True
         }
         headers = self.headers | {"Content-Type": "application/json"}
-        response = requests.post(f"{self.datasources_search}/{datasource_id}", headers=headers, json=data).json()
-        content = "\n\n".join([finding["page_content"] for finding in response["findings"]])
-        return AIMessage(content=content, additional_kwargs={"references": response['references']})
+        response = requests.post(f"{self.datasources_search}/{datasource_id}", headers=headers, json=data)
+        if not response.ok:
+            raise Exception(f'Search request failed with code {response.status_code}')
+        resp_data = response.json()
+        # content = "\n\n".join([finding["page_content"] for finding in response["findings"]])
+        content = resp_data["findings"]
+        references = resp_data['references']
+        return AIMessage(content=content, additional_kwargs={"references": references})
```

### Comparing `alita_sdk-0.1.0/src/alita_sdk/llms/alita.py` & `alita_sdk-0.1.1/src/alita_sdk/llms/alita.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,19 @@
 class MaxRetriesExceededError(Exception):
     """Raised when the maximum number of retries is exceeded"""
     
     def __init__(self, message="Maximum number of retries exceeded"):
         self.message = message
         super().__init__(self.message)
 
+
 class AlitaChatModel(BaseChatModel):
+    class Config:
+        allow_population_by_field_name = True
+
     client: Any  #: :meta private:
     encoding: Any  #: :meta private:
     model_name: str = Field(default="gpt-3.5-turbo", alias="model")
     deployment: str = Field(default="https://eye.projectalita.ai", alias="base_url")
     api_token: str = Field(default=None, alias="api_key")
     project_id: int = None
     integration_uid: str = None
```

### Comparing `alita_sdk-0.1.0/src/alita_sdk/toolkits/datasource.py` & `alita_sdk-0.1.1/src/alita_sdk/toolkits/datasource.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.0/src/alita_sdk/toolkits/prompt.py` & `alita_sdk-0.1.1/src/alita_sdk/toolkits/prompt.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.0/src/alita_sdk/tools/datasource.py` & `alita_sdk-0.1.1/src/alita_sdk/tools/datasource.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.0/src/alita_sdk/utils/streamlit.py` & `alita_sdk-0.1.1/src/alita_sdk/utils/streamlit.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.0/src/alita_sdk.egg-info/PKG-INFO` & `alita_sdk-0.1.1/src/alita_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: alita_sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: SDK for building langchain agents using resouces from Alita
 Author-email: Artem Rozumenko <support@analysta.ai>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/alita-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: langchain_core==0.1.30
-Requires-Dist: langchain==0.1.11
-Requires-Dist: tiktoken==0.6.0
+Requires-Dist: langchain_core~=0.1.30
+Requires-Dist: langchain~=0.1.12
+Requires-Dist: tiktoken~=0.6.0
 Requires-Dist: openai==1.13.3
-Requires-Dist: python-dotenv==1.0.1
-Requires-Dist: alita_tools==0.0.9
+Requires-Dist: python-dotenv~=1.0.1
+Requires-Dist: alita_tools>=0.0.10
+Requires-Dist: jinja2~=3.1.3
+Requires-Dist: pillow~=10.2.0
+Requires-Dist: requests~=2.31.0
+Requires-Dist: pydantic~=1.10.9
 
 Alita SDK
 =========
 
 Alita SDK, built on top of Langchain, enables the creation of intelligent agents within the Alita Platform using project-specific prompts and data sources. This SDK is designed for developers looking to integrate advanced AI capabilities into their projects with ease.
 
 Prerequisites
```

### Comparing `alita_sdk-0.1.0/src/alita_sdk.egg-info/SOURCES.txt` & `alita_sdk-0.1.1/src/alita_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

