# Comparing `tmp/v4xyz-0.0.6.tar.gz` & `tmp/v4xyz-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "v4xyz-0.0.6.tar", last modified: Sun May 14 09:54:53 2023, max compression
+gzip compressed data, was "v4xyz-0.1.0.tar", last modified: Tue Apr 30 16:05:18 2024, max compression
```

## Comparing `v4xyz-0.0.6.tar` & `v4xyz-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-14 09:54:53.751529 v4xyz-0.0.6/
--rw-r--r--   0 john      (1000) john      (1000)    11540 2023-05-13 11:27:28.000000 v4xyz-0.0.6/LICENSE
--rw-r--r--   0 john      (1000) john      (1000)     3202 2023-05-14 09:54:53.751529 v4xyz-0.0.6/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     1863 2023-05-14 09:49:41.000000 v4xyz-0.0.6/README.md
--rw-r--r--   0 john      (1000) john      (1000)       74 2023-05-14 09:54:53.751529 v4xyz-0.0.6/setup.cfg
--rw-r--r--   0 john      (1000) john      (1000)     1525 2023-05-14 09:54:51.000000 v4xyz-0.0.6/setup.py
--rw-r--r--   0 john      (1000) john      (1000)     5242 2023-05-13 14:11:35.000000 v4xyz-0.0.6/v4.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-05-14 09:54:53.751529 v4xyz-0.0.6/v4xyz.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)     3202 2023-05-14 09:54:53.000000 v4xyz-0.0.6/v4xyz.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)      218 2023-05-14 09:54:53.000000 v4xyz-0.0.6/v4xyz.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) john      (1000)        1 2023-05-14 09:54:53.000000 v4xyz-0.0.6/v4xyz.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) john      (1000)       32 2023-05-14 09:54:53.000000 v4xyz-0.0.6/v4xyz.egg-info/entry_points.txt
--rw-r--r--   0 john      (1000) john      (1000)       50 2023-05-14 09:54:53.000000 v4xyz-0.0.6/v4xyz.egg-info/requires.txt
--rw-r--r--   0 john      (1000) john      (1000)        3 2023-05-14 09:54:53.000000 v4xyz-0.0.6/v4xyz.egg-info/top_level.txt
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-04-30 16:05:18.299416 v4xyz-0.1.0/
+-rw-r--r--   0 john      (1000) john      (1000)    11540 2024-04-30 15:08:53.000000 v4xyz-0.1.0/LICENSE
+-rw-r--r--   0 john      (1000) john      (1000)     2804 2024-04-30 16:05:18.299416 v4xyz-0.1.0/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     2070 2024-04-30 16:03:52.000000 v4xyz-0.1.0/README.md
+-rw-r--r--   0 john      (1000) john      (1000)       74 2024-04-30 16:05:18.299416 v4xyz-0.1.0/setup.cfg
+-rw-r--r--   0 john      (1000) john      (1000)     1397 2024-04-30 16:01:51.000000 v4xyz-0.1.0/setup.py
+-rw-r--r--   0 john      (1000) john      (1000)     6380 2024-04-30 16:03:19.000000 v4xyz-0.1.0/v4.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2024-04-30 16:05:18.299416 v4xyz-0.1.0/v4xyz.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)     2804 2024-04-30 16:05:18.000000 v4xyz-0.1.0/v4xyz.egg-info/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)      218 2024-04-30 16:05:18.000000 v4xyz-0.1.0/v4xyz.egg-info/SOURCES.txt
+-rw-r--r--   0 john      (1000) john      (1000)        1 2024-04-30 16:05:18.000000 v4xyz-0.1.0/v4xyz.egg-info/dependency_links.txt
+-rw-r--r--   0 john      (1000) john      (1000)       31 2024-04-30 16:05:18.000000 v4xyz-0.1.0/v4xyz.egg-info/entry_points.txt
+-rw-r--r--   0 john      (1000) john      (1000)       50 2024-04-30 16:05:18.000000 v4xyz-0.1.0/v4xyz.egg-info/requires.txt
+-rw-r--r--   0 john      (1000) john      (1000)        3 2024-04-30 16:05:18.000000 v4xyz-0.1.0/v4xyz.egg-info/top_level.txt
```

### Comparing `v4xyz-0.0.6/LICENSE` & `v4xyz-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `v4xyz-0.0.6/setup.py` & `v4xyz-0.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from setuptools import setup
 
-version = "0.0.6"
+version = "0.1.0"
 description = "A command line tool to chat with GPT4 and render markdown response."
 with open("README.md") as fp:
     long_description = fp.read()
 url = "https://github.com/imhuwq/v4xyz"
 author = "imhuwq"
 author_email = "imhuwq@gmail.com"
-with open("LICENSE") as fp:
-    license_text = fp.read()
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Topic :: Communications :: Chat",
     "Topic :: Terminals",
     "Operating System :: POSIX :: Linux",
@@ -20,15 +18,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: Apache Software License",
 ]
 
 setup(name="v4xyz",
-      version=version,  # the package version, it may be different from the release version
+      version=version,
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url=url,
       author=author,
       author_email=author_email,
       license="Apache License 2.0",
```

### Comparing `v4xyz-0.0.6/v4.py` & `v4xyz-0.1.0/v4.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,21 +10,39 @@
 from rich.markdown import Markdown
 
 HOME_DIR = os.path.expanduser("~")
 CONFIG_PATH = os.path.join(HOME_DIR, ".v4xyz", "config.json")
 CONFIG_TEMPLATE = """
 {
   "openai_secret": "",
+  "openai_model": "gpt-4-turbo",
   "http_proxy": "",
-  "https_proxy": ""
+  "https_proxy": "",
 }
 """.strip()
 OPENAI_SECRET = None
+OPENAI_MODEL = "gpt-4-turbo"
 HISTORY_PATH = os.path.join(HOME_DIR, ".v4xyz", "chat_history.txt")
 
+Prices = {
+    "gpt-4-turbo-2024-04-09": {
+        "input": 0.01 / 1000,
+        "output": 0.03 / 1000,
+
+    },
+    "gpt-4-turbo": {
+        "input": 0.01 / 1000,
+        "output": 0.03 / 1000,
+    },
+    "gpt-4": {
+        "input": 0.03 / 1000,
+        "output": 0.06 / 1000,
+    }
+}
+
 
 class Cmd(click.Command):
     def format_help(self, ctx, formatter):
         art = text2art("This is the Way", "Small Slant")
         click.echo(art)
         super().format_help(ctx, formatter)
 
@@ -35,40 +53,46 @@
         with open(CONFIG_PATH, "w") as fp:
             fp.write(CONFIG_TEMPLATE)
     click.edit(filename=CONFIG_PATH)
 
 
 def load_config():
     global OPENAI_SECRET
+    global OPENAI_MODEL
 
     if not os.path.exists(CONFIG_PATH):
         click.echo("config file not found, try `v4 -e` first to set your config file.")
         exit(1)
 
     with open(CONFIG_PATH) as fp:
         config = json.load(fp)
 
     if config["http_proxy"]:
         os.environ["http_proxy"] = config["http_proxy"]
     if config["https_proxy"]:
         os.environ["https_proxy"] = config["https_proxy"]
+    if config["openai_model"]:
+        OPENAI_MODEL = config["openai_model"]
 
     OPENAI_SECRET = config["openai_secret"]
     if not OPENAI_SECRET:
         click.echo("openai_secret is not set in config file, try `v4 -e` to edit your config file")
         exit(1)
 
     openai.api_key = OPENAI_SECRET
 
 
 def count_token(content: str):
     return len(content) // 4
 
 
-def load_history(max_token: int = 4096):
+def load_history(num_history:int, max_token: int = 4096):
+    if num_history == 0:
+        return [], 0, 0
+    
     histories = []
     if not os.path.exists(HISTORY_PATH):
         return [], 0, 0
 
     with open(HISTORY_PATH, "r") as fp:
         block_data = ""
         block_role = None
@@ -85,14 +109,16 @@
                     histories.append({"role": last_block_role, "content": last_block_data})
             else:
                 block_data += line
 
         if block_data and block_role == "assistant":
             histories.append({"role": block_role, "content": block_data})
 
+    histories = histories[-num_history:]
+
     total_token = 0
     histories_reverse, histories = histories[::-1], []
     for history in histories_reverse:
         # 1 token ~= 4 chars in English
         # https://help.openai.com/en/articles/4936856-what-are-tokens-and-how-to-count-them
         len_content_token = count_token(history["content"])
         if total_token + len_content_token > max_token:
@@ -101,34 +127,35 @@
         histories.insert(0, history)
         total_token += len_content_token
 
     num_dropped = len(histories_reverse) - len(histories)
     return histories, total_token, num_dropped
 
 
-def ask_gpt4(inputs: str):
-    histories, histories_token, num_dropped = load_history()
+def ask_openai(inputs: str, history: int):
+    histories, histories_token, num_dropped = load_history(history)
 
     system_prompt = "You are a helpful assistant always replay in markdown format."
     system_prompt += "You should answer as brief as possible."
 
     sys_prompt_token = count_token(system_prompt)
     input_token = count_token(inputs)
     total_token = histories_token + sys_prompt_token + input_token
 
     messages = [{"role": "system", "content": system_prompt}, ]
     messages.extend(histories)
     messages.append({"role": "user", "content": inputs})
 
+    print(f"[bold blue  ]Model   : {OPENAI_MODEL}[/]")
     print(f"[bold red   ]Question: {inputs}[/]")
     print(f"[bold yellow]Context : {len(histories)} histories, {num_dropped} dropped, {total_token} tokens[/]")
     print("-" * 10)
     print("")
 
-    rsp = openai.ChatCompletion.create(model="gpt-4", messages=messages, stream=True)
+    rsp = openai.ChatCompletion.create(model=OPENAI_MODEL, messages=messages, stream=True)
     answer = ""
     md = Markdown(answer)
     with Live(md, refresh_per_second=10) as live:
         for chunk in rsp:
             delta = chunk["choices"][0]["delta"]
             answer += delta.get("content", "")
             md = Markdown(answer)
@@ -140,33 +167,43 @@
     with open(HISTORY_PATH, "a") as fp:
         fp.write(f"Answer\t{datetime.now()}\n{answer}\n")
 
     print("")
     print("-" * 10)
     print(f"[bold yellow]Received: {count_token(answer)} tokens[/]")
 
+    price = Prices[OPENAI_MODEL]
+    input_cost = input_token * price["input"]
+    output_cost = count_token(answer) * price["output"]
+    print(f"[bold blue  ]Cost   : {input_cost + output_cost:.6f}$, input {input_cost:.6f}$, output {output_cost:.6f}$[/]")
+
 
 @click.command(cls=Cmd)
 @click.option("-e", "--edit", is_flag=True, help="Edit the config file")
+@click.option("-h", "--history", type=int, default=0, help="Ask with last n histories")
 @click.argument("inputs", nargs=1, required=False)  # required must be False, otherwise we cant get into edit mode
-def v4(edit, inputs):
+def v4(edit, history, inputs):
     if edit is True:
         return edit_config()
+    
+    if history < 0:
+        click.echo("history must be positive")
+        exit(2)
 
     if inputs is None:
         click.echo(v4.get_help(click.Context(v4)))
         exit(1)
 
     load_config()
     inputs = inputs.strip()
     if not inputs:
         return
 
     inputs = inputs.capitalize()
-    return ask_gpt4(inputs)
+    return ask_openai(inputs, history)
 
 
 def main():
     v4()
 
 
 if __name__ == "__main__":
```

