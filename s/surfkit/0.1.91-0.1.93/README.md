# Comparing `tmp/surfkit-0.1.91.tar.gz` & `tmp/surfkit-0.1.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surfkit-0.1.91.tar", max compression
+gzip compressed data, was "surfkit-0.1.93.tar", max compression
```

## Comparing `surfkit-0.1.91.tar` & `surfkit-0.1.93.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1069 2024-04-09 16:39:37.152115 surfkit-0.1.91/LICENSE
--rw-r--r--   0        0        0      270 2024-04-03 02:13:16.594885 surfkit-0.1.91/README.md
--rw-r--r--   0        0        0      717 2024-04-26 03:20:55.729795 surfkit-0.1.91/pyproject.toml
--rw-r--r--   0        0        0     1725 2024-04-25 22:12:14.558746 surfkit-0.1.91/surfkit/agent.py
--rw-r--r--   0        0        0      602 2024-04-09 16:39:37.166082 surfkit-0.1.91/surfkit/cli/init.py
--rw-r--r--   0        0        0     6668 2024-04-25 17:18:51.486625 surfkit-0.1.91/surfkit/cli/main.py
--rw-r--r--   0        0        0    10733 2024-04-16 17:55:09.920080 surfkit-0.1.91/surfkit/cli/templates/agent.py
--rw-r--r--   0        0        0        0 2024-04-09 16:39:37.166494 surfkit-0.1.91/surfkit/cli/templates/device.py
--rw-r--r--   0        0        0     2053 2024-04-17 19:36:14.985684 surfkit-0.1.91/surfkit/config.py
--rw-r--r--   0        0        0     2007 2024-04-17 19:23:41.286231 surfkit-0.1.91/surfkit/db/conn.py
--rw-r--r--   0        0        0      982 2024-04-17 16:29:32.098357 surfkit-0.1.91/surfkit/db/models.py
--rw-r--r--   0        0        0      238 2024-04-17 19:35:04.174976 surfkit-0.1.91/surfkit/env.py
--rw-r--r--   0        0        0      993 2024-04-03 16:40:15.124046 surfkit-0.1.91/surfkit/hub.py
--rw-r--r--   0        0        0     9138 2024-04-25 22:16:23.555559 surfkit-0.1.91/surfkit/llm.py
--rw-r--r--   0        0        0     2413 2024-04-17 16:28:56.465927 surfkit-0.1.91/surfkit/models.py
--rw-r--r--   0        0        0     3034 2024-04-25 17:18:59.281584 surfkit-0.1.91/surfkit/runtime/agent/base.py
--rw-r--r--   0        0        0     7381 2024-04-25 17:19:06.360421 surfkit-0.1.91/surfkit/runtime/agent/docker.py
--rw-r--r--   0        0        0    27130 2024-04-25 17:19:11.347240 surfkit-0.1.91/surfkit/runtime/agent/kube.py
--rw-r--r--   0        0        0      910 2024-04-19 03:20:06.559203 surfkit-0.1.91/surfkit/runtime/agent/load.py
--rw-r--r--   0        0        0     1425 2024-04-11 22:52:18.482166 surfkit-0.1.91/surfkit/runtime/container/base.py
--rw-r--r--   0        0        0     5983 2024-04-16 16:34:59.842004 surfkit-0.1.91/surfkit/runtime/container/docker.py
--rw-r--r--   0        0        0    16077 2024-04-11 22:50:31.352813 surfkit-0.1.91/surfkit/runtime/container/kube.py
--rw-r--r--   0        0        0     1028 2024-04-11 16:49:49.850218 surfkit-0.1.91/surfkit/runtime/container/load.py
--rw-r--r--   0        0        0      402 2024-04-11 18:32:09.170609 surfkit-0.1.91/surfkit/runtime/vm/base.py
--rw-r--r--   0        0        0     9920 2024-04-17 20:04:44.519945 surfkit-0.1.91/surfkit/types.py
--rw-r--r--   0        0        0      793 2024-04-25 20:53:50.784539 surfkit-0.1.91/surfkit/util.py
--rw-r--r--   0        0        0     1262 1970-01-01 00:00:00.000000 surfkit-0.1.91/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-09 16:39:37.152115 surfkit-0.1.93/LICENSE
+-rw-r--r--   0        0        0      270 2024-04-03 02:13:16.594885 surfkit-0.1.93/README.md
+-rw-r--r--   0        0        0      734 2024-04-29 20:30:25.198562 surfkit-0.1.93/pyproject.toml
+-rw-r--r--   0        0        0     1725 2024-04-25 22:12:14.558746 surfkit-0.1.93/surfkit/agent.py
+-rw-r--r--   0        0        0     7728 2024-04-29 20:07:35.622937 surfkit-0.1.93/surfkit/cli/main.py
+-rw-r--r--   0        0        0      926 2024-04-29 19:57:18.519637 surfkit-0.1.93/surfkit/cli/new.py
+-rw-r--r--   0        0        0    13462 2024-04-29 19:56:21.528849 surfkit-0.1.93/surfkit/cli/templates/agent.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:39:37.166494 surfkit-0.1.93/surfkit/cli/templates/device.py
+-rw-r--r--   0        0        0      866 2024-04-29 19:58:42.750756 surfkit-0.1.93/surfkit/cli/util.py
+-rw-r--r--   0        0        0     2053 2024-04-17 19:36:14.985684 surfkit-0.1.93/surfkit/config.py
+-rw-r--r--   0        0        0     2007 2024-04-17 19:23:41.286231 surfkit-0.1.93/surfkit/db/conn.py
+-rw-r--r--   0        0        0      982 2024-04-17 16:29:32.098357 surfkit-0.1.93/surfkit/db/models.py
+-rw-r--r--   0        0        0      238 2024-04-17 19:35:04.174976 surfkit-0.1.93/surfkit/env.py
+-rw-r--r--   0        0        0      993 2024-04-03 16:40:15.124046 surfkit-0.1.93/surfkit/hub.py
+-rw-r--r--   0        0        0     9144 2024-04-26 03:39:53.635637 surfkit-0.1.93/surfkit/llm.py
+-rw-r--r--   0        0        0     2649 2024-04-26 03:40:29.954908 surfkit-0.1.93/surfkit/models.py
+-rw-r--r--   0        0        0     3034 2024-04-25 17:18:59.281584 surfkit-0.1.93/surfkit/runtime/agent/base.py
+-rw-r--r--   0        0        0     7381 2024-04-25 17:19:06.360421 surfkit-0.1.93/surfkit/runtime/agent/docker.py
+-rw-r--r--   0        0        0    27130 2024-04-25 17:19:11.347240 surfkit-0.1.93/surfkit/runtime/agent/kube.py
+-rw-r--r--   0        0        0      910 2024-04-19 03:20:06.559203 surfkit-0.1.93/surfkit/runtime/agent/load.py
+-rw-r--r--   0        0        0     1425 2024-04-11 22:52:18.482166 surfkit-0.1.93/surfkit/runtime/container/base.py
+-rw-r--r--   0        0        0     5983 2024-04-16 16:34:59.842004 surfkit-0.1.93/surfkit/runtime/container/docker.py
+-rw-r--r--   0        0        0    16077 2024-04-11 22:50:31.352813 surfkit-0.1.93/surfkit/runtime/container/kube.py
+-rw-r--r--   0        0        0     1028 2024-04-11 16:49:49.850218 surfkit-0.1.93/surfkit/runtime/container/load.py
+-rw-r--r--   0        0        0      402 2024-04-11 18:32:09.170609 surfkit-0.1.93/surfkit/runtime/vm/base.py
+-rw-r--r--   0        0        0     9920 2024-04-17 20:04:44.519945 surfkit-0.1.93/surfkit/types.py
+-rw-r--r--   0        0        0      793 2024-04-25 20:53:50.784539 surfkit-0.1.93/surfkit/util.py
+-rw-r--r--   0        0        0     1301 1970-01-01 00:00:00.000000 surfkit-0.1.93/PKG-INFO
```

### Comparing `surfkit-0.1.91/LICENSE` & `surfkit-0.1.93/LICENSE`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.91/pyproject.toml` & `surfkit-0.1.93/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "surfkit"
-version = "0.1.91"
+version = "0.1.93"
 description = "A toolkit to build GUI surfing AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -17,14 +17,15 @@
 toolfuse = "^0.1.15"
 kubernetes = "^29.0.0"
 devicebay = "^0.1.11"
 litellm = "^1.35.8"
 agentdesk = "^0.2.65"
 tiktoken = "^0.6.0"
 taskara = "^0.1.42"
+rich = "^13.7.1"
 
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.29.4"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `surfkit-0.1.91/surfkit/agent.py` & `surfkit-0.1.93/surfkit/agent.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.91/surfkit/cli/main.py` & `surfkit-0.1.93/surfkit/cli/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import yaml
 
 import typer
 import webbrowser
 from namesgenerator import get_random_name
 import requests
 
-
 art = """
  _______                ___  __  __  __  __   
 |     __|.--.--..----..'  _||  |/  ||__||  |_ 
 |__     ||  |  ||   _||   _||     < |  ||   _|
 |_______||_____||__|  |__|  |__|\__||__||____|
 """
 
@@ -167,15 +166,47 @@
     resp = requests.post(url, json=agent_type.model_dump(), headers=headers)
     resp.raise_for_status()
     typer.echo(f"Agent published!")
 
 
 @app.command(help="Create a new agent repo")
 def new():
-    raise NotImplementedError()
+    from rich.prompt import Prompt
+    from .new import new_agent
+    from .util import get_git_global_user_config
+
+    name = Prompt.ask("Enter agent name")
+    if not name.isalnum() or len(name) > 50:
+        typer.echo(
+            "Invalid agent name. Must be alphanumeric and less than 50 characters."
+        )
+
+    name = Prompt.ask("Enter agent name")
+    if not name.isalnum() or len(name) > 50:
+        typer.echo(
+            "Invalid agent name. Must be alphanumeric and less than 50 characters."
+        )
+        raise typer.Exit()
+
+    description = Prompt.ask("Describe the agent")
+    git_user_ref = Prompt.ask(
+        "Enter git user reference", default=get_git_global_user_config()
+    )
+    image_repo = Prompt.ask("Enter docker image repo")
+    icon_url = Prompt.ask(
+        "Enter icon url",
+        default="https://upload.wikimedia.org/wikipedia/commons/a/a5/Tsunami_by_hokusai_19th_century.jpg",
+    )
+    new_agent(
+        name=name,
+        description=description,
+        git_user_ref=git_user_ref,
+        img_repo=image_repo,
+        icon_url=icon_url,
+    )
 
 
 @app.command(help="Use an agent to solve a task")
 def solve(
     description: str,
     agent_name: str,
     max_steps: int = 20,
```

### Comparing `surfkit-0.1.91/surfkit/cli/templates/agent.py` & `surfkit-0.1.93/surfkit/cli/templates/agent.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,205 +1,190 @@
+import os
+
 from surfkit.types import AgentType
 
 
-def generate_dockerfile(package_name: str) -> str:
-    return f"""
-# Use an official Python runtime as a parent image
-FROM python:3.10
+def generate_dockerfile(package_name: str) -> None:
+    out = f"""
+FROM thehale/python-poetry:1.8.2-py3.10-slim
 
-# Set the working directory in the container to /app
+COPY . /app
 WORKDIR /app
 
-# Copy the current directory contents into the container at /app
-COPY requirements.txt .
-
-# Install system dependencies
-RUN apt-get update && apt-get install -y \
-    build-essential \
-    software-properties-common \
-    python3-dev \
-    git \
-    ntp \
-    rm -rf /var/lib/apt/lists/*  # Clean up to reduce image size
-
-# Upgrade pip
-RUN pip install --upgrade pip
-RUN pip install -r requirements.txt
-
-# Surfkit
-RUN pip install surfkit
+RUN apt-get update && apt-get install -y openssh-client ntp
+RUN poetry install
 
-COPY . .
+EXPOSE 9090
 
 # Run the application
 CMD ["uvicorn", "{package_name}.server:app", "--host=0.0.0.0", "--port=9090", "--log-level", "debug"]
 """
+    with open(f"Dockerfile", "w") as f:
+        f.write(out)
 
 
-def generate_server(agent_name: str) -> str:
-    return f"""
-from fastapi import FastAPI, BackgroundTasks
-from fastapi.middleware.cors import CORSMiddleware
+def generate_server(agent_name: str) -> None:
+    out = f"""
 import os
-from contextlib import asynccontextmanager
 
-from tenacity import retry, stop_after_attempt, wait_fixed
-from taskara.models import SolveTaskModel
+from taskara.server.models import SolveTaskModel, TaskModel, TasksModel
 from taskara.task import Task
-from taskara.models import TaskModel, TasksModel
 from surfkit.hub import Hub
 from surfkit.llm import LLMProvider
-from agentdesk import Desktop
-
-from .agent import {agent_name}
+from fastapi import FastAPI, BackgroundTasks
+from fastapi.middleware.cors import CORSMiddleware
+from contextlib import asynccontextmanager
 
-HUB_SERVER = os.environ.get("SURF_HUB_SERVER", "https://surf.agentlabs.xyz")
-HUB_API_KEY = os.environ.get("HUB_API_KEY")
-if not HUB_API_KEY:
-    raise Exception("$HUB_API_KEY not set")
-AGENTD_ADDR = os.environ.get("AGENTD_ADDR")
-if not AGENTD_ADDR:
-    raise Exception("$AGENTD_ADDR not set")
-AGENTD_PRIVATE_SSH_KEY = os.environ.get("AGENTD_PRIVATE_SSH_KEY")
-if not AGENTD_PRIVATE_SSH_KEY:
-    raise Exception("$AGENTD_PRIVATE_SSH_KEY not set")
+from .agent import Agent
+from .util import get_remote_task
 
 
 # Get the LLM provider from env
 llm_provider = LLMProvider.from_env()
 
 
 @asynccontextmanager
 async def lifespan(app: FastAPI):
+    # Initialize the agent type before the server comes live
+    Agent.init()
     yield
 
 
-app = FastAPI(lifespan=lifespan)
+app = FastAPI(lifespan=lifespan)  # type: ignore
 
 app.add_middleware(
     CORSMiddleware,
     allow_origins=["*"],
     allow_credentials=True,
     allow_methods=["*"],
     allow_headers=["*"],
 )
 
 
 @app.get("/")
 async def root():
-    return {"message": "Agent in the shell"}
+    return {{"message": "Agent in the shell"}}
 
 
 @app.get("/health")
 async def health():
-    return {"status": "ok"}
+    return {{"status": "ok"}}
 
 
 @app.post("/v1/tasks")
-async def create_task(background_tasks: BackgroundTasks, task: SolveTaskModel):
-    print(f"solving task: \n{{task.model_dump()}}")
+async def solve_task(background_tasks: BackgroundTasks, task_model: SolveTaskModel):
+    print(f"solving task: \n{{task_model.model_dump()}}")
     try:
         # TODO: we need to find a way to do this earlier but get status back
         llm_provider.check_model()
     except Exception as e:
         print(f"Cannot connect to LLM providers: {{e}} -- did you provide a valid key?")
-        return {
+        return {{
             "status": "failed",
-            "message": f'failed to conect to LLM providers -- did you provide a valid key?',
-        }
+            "message": f"failed to conect to LLM providers: {{e}} -- did you provide a valid key?",
+        }}
 
-    background_tasks.add_task(_create_task, task)
+    background_tasks.add_task(_solve_task, task_model)
     print("created background task...")
 
 
-def _create_task(task: SolveTaskModel):
-    hub = Hub(HUB_SERVER)
-    user_info = hub.get_user_info(HUB_API_KEY)
-    print("got user info: ", user_info.__dict__)
-
-    print("syncing to remote task: ", task.task.id, HUB_SERVER)
-    rtask = get_remote_task(
-        id=task.task.id,
-        owner_id=user_info.email,
-    )
-    print("got remote task: ", rtask.__dict__)
+def _solve_task(task_model: SolveTaskModel):
+    task = Task.from_schema(task_model.task, owner_id="local")
+    if task.remote:
+        print("connecting to remote task...")
+        HUB_SERVER = os.environ.get("SURF_HUB_SERVER", "https://surf.agentlabs.xyz")
+        HUB_API_KEY = os.environ.get("HUB_API_KEY")
+        if not HUB_API_KEY:
+            raise Exception("$HUB_API_KEY not set")
+
+        hub = Hub(HUB_SERVER)
+        user_info = hub.get_user_info(HUB_API_KEY)
+        print("got user info: ", user_info.__dict__)
+
+        task = get_remote_task(
+            id=task.id,
+            owner_id=user_info.email,  # type: ignore
+            server=task.remote,
+        )
+        print("got remote task: ", task.__dict__)
 
     print("Saving remote tasks status to running...")
-    rtask.status = "in progress"
-    rtask.save()
-
-    rtask.post_message("assistant", f"Starting task '{{rtask.description}}'")
-    print("creating threads...")
-
-    rtask.create_thread("debug")
-    rtask.post_message("assistant", f"I'll post debug messages here", thread="debug")
+    task.status = "in progress"
+    task.save()
 
-    rtask.create_thread("prompt")
-    rtask.post_message(
-        "assistant", f"I'll post all llm prompts that take place here", thread="prompt"
-    )
-    print("created work thread 'debug' and 'prompt'")
-
-    print("creating desktop...")
-    desktop: SemanticDesktop = SemanticDesktop(
-        task=rtask,
-        agentd_url=AGENTD_ADDR,
-        requires_proxy=True,
-        proxy_port=7000,
-        private_ssh_key=AGENTD_PRIVATE_SSH_KEY,
-    )
-    print("created desktop: ", desktop.__dict__)
+    if task_model.device:
+        print(f"connecting to device {{task_model.device.name}}...")
+        device = None
+        for Device in Agent.supported_devices():
+            if Device.name() == task_model.device.name:
+                print("found device: ", task_model.device.model_dump())
+                print("model config: ", task_model.device.config)
+                config = Device.connect_config_type()(**task_model.device.config)
+                device = Device.connect(config=config)
+
+        if not device:
+            raise ValueError(
+                f"Device {{task_model.device.name}} provided in solve task, but not supported by agent"
+            )
+
+        print("connected to device: ", device.__dict__)
+    else:
+        raise ValueError("No device provided")
+
+    print("starting agent...")
+    if task_model.agent:
+        config = Agent.config_type()(**task_model.agent.config.model_dump())
+        agent = Agent.from_config(config=config)
+    else:
+        agent = Agent.default()
 
     try:
-        fin_task = agent.solve_task(rtask, desktop, task.max_steps, task.site)
+        fin_task = agent.solve_task(task=task, device=device, max_steps=task.max_steps)
     except Exception as e:
         print("error running agent: ", e)
-        rtask.status = "failed"
-        rtask.error = str(e)
-        rtask.save()
-        rtask.post_message(
-            "assistant", f"Failed to run task '{{rtask.description}}': {{e}}"
-        )
+        task.status = "failed"
+        task.error = str(e)
+        task.save()
+        task.post_message("assistant", f"Failed to run task '{{task.description}}': {{e}}")
         raise e
     if fin_task:
         fin_task.save()
 
-@retry(stop=stop_after_attempt(10), wait=wait_fixed(10))
-def get_remote_task(id: str, owner_id: str) -> Task:
-    print("connecting to remote task: ", id, HUB_SERVER, HUB_API_KEY)
-    try:
-        tasks = Task.find(
-            id=id,
-            remote=HUB_SERVER,
-            owner_id=owner_id,
-        )
-        if not tasks:
-            raise Exception(f"Task {{id}} not found")
-        print("got remote task: ", tasks[0].__dict__)
-        return tasks[0]
-    except Exception as e:
-        print("error getting remote task: ", e)
-        raise e
+
+@app.get("/v1/tasks", response_model=TasksModel)
+async def get_tasks():
+    tasks = Task.find()
+    return TasksModel(tasks=[task.to_schema() for task in tasks])
+
+
+@app.get("/v1/tasks/{{id}}", response_model=TaskModel)
+async def get_task(id: str):
+    tasks = Task.find(id=id)
+    if not tasks:
+        raise Exception(f"Task {{id}} not found")
+    return tasks[0].to_schema()
 
 """
+    with open(f"{agent_name.lower()}/server.py", "w") as f:
+        f.write(out)
 
 
-def generate_main() -> str:
-    return f"""
+def generate_main(agent_name: str) -> None:
+    out = f"""
 import argparse
 import logging
 import yaml
 
 from rich.console import Console
 from agentdesk.device import Desktop, ProvisionConfig
 from agentdesk.vm.gce import GCEProvider
 from agentdesk.vm.ec2 import EC2Provider
 from agentdesk.vm.qemu import QemuProvider
 from taskara import Task
-from taskara.models import SolveTaskModel
+from taskara.server.models import SolveTaskModel
 from surfkit.types import AgentType
 from surfkit.models import AgentTypeModel
 from surfkit.runtime.agent.load import (
     load_agent_runtime,
     AgentRuntimeConfig,
     DockerConnectConfig,
     KubeConnectConfig,
@@ -301,29 +286,30 @@
 task = Task(description=args.task, owner_id="local", parameters=parameters)
 
 with open(args.agent_type) as f:
     agent_data = yaml.safe_load(f)
     agent_schema = AgentTypeModel(**agent_data)
 agent_type = AgentType.from_schema(agent_schema)
 
+# TODO: dynamically supply and provision devices
 console.print("Creating device...", style="green")
 print("\nprovider data: ", provider.to_data())
 config = ProvisionConfig(provider=provider.to_data())
-device: Desktop = Desktop.ensure("gpt4v-demo1", config=config)
+device: Desktop = Desktop.ensure("gpt4v-demo", config=config)
 
 # View the desktop, we'll run in the background so it doesn't block
 device.view(background=True)
 
 if args.agent_runtime == "docker":
     print("using docker runtime...")
     dconf = DockerConnectConfig()
     conf = AgentRuntimeConfig(provider="docker", docker_config=dconf)
 elif args.agent_runtime == "kube":
     print("using kube runtime...")
-    kconf = KubeConnectConfig()
+    kconf = KubeConnectConfig(namespace=args.namespace)
     conf = AgentRuntimeConfig(provider="kube", kube_config=kconf)
 else:
     raise ValueError("Unknown agent runtime")
 
 runtime = load_agent_runtime(conf)
 
 print("\ndevice schema: ", device.to_schema())
@@ -333,97 +319,211 @@
 agent.proxy(DEFAULT_PROXY_PORT)
 console.print(f"Proxying agent to port {{DEFAULT_PROXY_PORT}}", style="green")
 
 task_model = SolveTaskModel(
     task=task.to_schema(), device=device.to_schema(), max_steps=args.max_steps
 )
 agent.solve_task(task_model, follow_logs=True)
+
 """
+    with open(f"{agent_name.lower()}/__main__.py", "w") as f:
+        f.write(out)
 
 
-def generate_agent(agent_name: str) -> str:
-    return f"""
-from typing import List, Tuple, Optional
+def generate_agent(agent_name: str) -> None:
+    out = f"""
+from typing import List, Tuple, Type
 import json
 import time
 import logging
+from typing import Final
+from copy import deepcopy
+import traceback
+import os
 
+from tenacity import (
+    retry,
+    stop_after_attempt,
+    before_sleep_log,
+)
+from devicebay import Device
+from agentdesk.device import Desktop
 from rich.console import Console
 from rich.json import JSON
-
 from surfkit.llm import LLMProvider
+from pydantic import BaseModel
+from modelscope.pipelines import pipeline
+from MobileAgent.icon_localization import load_model
+from modelscope.utils.constant import Tasks
 from surfkit.agent import TaskAgent
 from taskara import Task
+from threadmem import RoleThread
+
+from .instruct import (
+    system_prompt,
+    action_prompt,
+    ActionSelection,
+    reflection_prompt,
+    EndReflection,
+)
+from .util import remove_user_image_urls, clean_llm_json, ensure_download
+from .tool import SemanticDesktop
 
 logger: Final = logging.getLogger(__name__)
 logging.basicConfig(level=logging.INFO)
 
 console = Console(force_terminal=True)
 
 llm_provider = LLMProvider.from_env()
 
+
+class {agent_name}Config(BaseModel):
+    pass
+
+
 class {agent_name}(TaskAgent):
+    \"""A desktop agent that uses GPT-4V augmented with OCR and Grounding Dino to solve tasks\"""
 
     def solve_task(
         self,
         task: Task,
-        desktop: Desktop,
-        max_steps: int = 10,
-        site: Optional[str] = None,
+        device: Device,
+        max_steps: int = 30,
     ) -> Task:
         \"""Solve a task
 
         Args:
-            task (Task): Task to solve
-            desktop (Desktop): An AgentDesk desktop instance.
-            max_steps (int, optional): Max steps to try and solve. Defaults to 5.
-            site (str, optional): Site to open. Defaults to None.
+            task (Task): Task to solve.
+            device (Desktop): Device to perform the task on.
+            max_steps (int, optional): Max steps to try and solve. Defaults to 30.
 
         Returns:
             Task: The task
         \"""
 
+        task.post_message("assistant", f"Starting task '{{task.description}}'")
         # > ENTER YOUR TASK LOGIC HERE <
 
-"""
+        
+    @classmethod
+    def supported_devices(cls) -> List[Type[Device]]:
+        \"""Devices this agent supports
+
+        Returns:
+            List[Type[Device]]: A list of supported devices
+        \"""
+        return [Desktop]
+
+    @classmethod
+    def config_type(cls) -> Type[{agent_name}Config]:
+        \"""Type of config
+
+        Returns:
+            Type[DinoConfig]: Config type
+        \"""
+        return {agent_name}Config
+
+    @classmethod
+    def from_config(cls, config: {agent_name}Config) -> "{agent_name}":
+        \"""Create an agent from a config
 
+        Args:
+            config (DinoConfig): Agent config
+
+        Returns:
+            {agent_name}: The agent
+        \"""
+        return {agent_name}()
 
-def generate_ci() -> str:
-    return ""
+    @classmethod
+    def default(cls) -> "{agent_name}":
+        \"""Create a default agent
+
+        Returns:
+            {agent_name}: The agent
+        \"""
+        return {agent_name}()
 
+    @classmethod
+    def init(cls) -> None:
+        \"""Initialize the agent class\"""
+        # <INITIALIZE AGENT HERE>
+        return
 
-def generate_requirements() -> str:
-    return """
-agentdesk
-rich
-google-cloud-compute
-google-cloud-container
-google-cloud-storage
-boto3
-boto3-stubs
-mypy-boto3-ec2
-fastapi[all]
-pydantic
-uvicorn
-tenacity
-surfkit
+
+Agent = {agent_name}
 """
+    with open(f"{agent_name.lower()}/agent.py", "w") as f:
+        f.write(out)
+
+
+def generate_dir(agent_name: str) -> None:
+    os.mkdir(agent_name.lower())
 
 
-# def generate_agentfile(name: str, description: str) -> str:
+def generate_pyproject(agent_name: str, description, git_user_ref: str) -> None:
+    out = f"""
+[tool.poetry]
+name = "{agent_name}"
+version = "0.1.0"
+description = "AI agent for {description}"
+authors = ["{git_user_ref}"]
+license = "MIT"
+readme = "README.md"
+packages = [{{include = "{agent_name}"}}]
+
+[tool.poetry.dependencies]
+python = "^3.10"
+sqlalchemy = "^2.0.27"
+pydantic = "^2.6.3"
+requests = "^2.31.0"
+surfkit - "^0.1.92"
+fastapi = {{version = "^0.109", extras = ["all"]}}
+
+
+[tool.poetry.group.dev.dependencies]
+flake8 = "^7.0.0"
+black = "^24.2.0"
+pytest = "^8.0.2"
+ipykernel = "^6.29.3"
+pytest-env = "^1.1.3"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+"""
+    with open(f"{agent_name.lower()}/pyproject.toml", "w") as f:
+        f.write(out)
+
 
-#     return f"""
-# version: v1
-# name: "{name}"
-# description: "{description}"
-# supported_runtimes:
-#   - "gke"
-# llm_providers:
-#   preference:
-#     - "gpt-4-vision-preview"
-#     - "anthropic/claude-3-opus-20240229"
-# public: True
-# icon: https://storage.googleapis.com/guisurfer-assets/surf_dino2.webp
-# min_cpu: 1
-# min_mem: 1Gi
-# min_gpu: 0
-# """
+def generate_agentfile(
+    name: str, description: str, image_repo: str, icon_url: str
+) -> None:
+
+    out = f"""
+api_version: v1alpha
+kind: TaskAgent
+name: "{name}"
+description: "{description}"
+image: "{image_repo}:latest"
+versions:
+  latest: "{image_repo}:latest"
+runtimes:
+  - type: "agent"
+    preference:
+      - "docker"
+      - "kube"
+llm_providers:
+  preference:
+    - "gpt-4-turbo"
+    - "anthropic/claude-3-opus-20240229"
+public: True
+icon: {icon_url}
+resource_requests:
+  cpu: "1"
+  memory: "2Gi"
+resource_limits:
+  cpu: "2"
+  memory: "4Gi"
+"""
+    with open(f"{name.lower()}/agent.yaml", "w") as f:
+        f.write(out)
```

### Comparing `surfkit-0.1.91/surfkit/config.py` & `surfkit-0.1.93/surfkit/config.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.91/surfkit/db/conn.py` & `surfkit-0.1.93/surfkit/db/conn.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.91/surfkit/db/models.py` & `surfkit-0.1.93/surfkit/db/models.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.91/surfkit/hub.py` & `surfkit-0.1.93/surfkit/hub.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.91/surfkit/llm.py` & `surfkit-0.1.93/surfkit/llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         self,
         thread: RoleThread,
         model: Optional[str] = None,
         task: Optional[Task] = None,
         namespace: str = "default",
         response_schema: Optional[Type[T]] = None,
         retries: int = 3,
-    ) -> ChatResponse:
+    ) -> ChatResponse[T]:
         """Chat with a language model
 
         Args:
             thread (RoleThread): A role thread
             model (Optional[str], optional): Model to use. Defaults to None.
             task (Optional[Task], optional): Optional task to log into. Defaults to None.
             namespace (Optional[str], optional): Namespace to log into. Defaults to "default".
@@ -164,15 +164,15 @@
         @retry(stop=stop_after_attempt(retries))
         def call_llm(
             thread: RoleThread,
             model: str,
             task: Optional[Task] = None,
             namespace: str = "default",
             response_schema: Optional[Type[T]] = None,
-        ) -> ChatResponse:
+        ) -> ChatResponse[T]:
             start = time.time()
             response = self.router.completion(model, thread.to_openai())
 
             if not isinstance(response, ModelResponse):
                 raise Exception(f"Unexpected response type: {type(response)}")
 
             end = time.time()
```

### Comparing `surfkit-0.1.91/surfkit/models.py` & `surfkit-0.1.93/surfkit/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,27 @@
-from typing import List, Optional, Dict
+from typing import List, Optional, Dict, Any
 
 from pydantic import BaseModel
 
 
+class Action(BaseModel):
+    """An action"""
+
+    name: str
+    parameters: Dict[str, Any]
+
+
+class ActionSelection(BaseModel):
+    """An action selection from the model"""
+
+    observation: str
+    reason: str
+    action: Action
+
+
 class EnvVarOptModel(BaseModel):
     name: str
     description: Optional[str] = None
     required: bool = False
     default: Optional[str] = None
     secret: bool = False
     options: List[str] = []
```

### Comparing `surfkit-0.1.91/surfkit/runtime/agent/base.py` & `surfkit-0.1.93/surfkit/runtime/agent/base.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.91/surfkit/runtime/agent/docker.py` & `surfkit-0.1.93/surfkit/runtime/agent/docker.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.91/surfkit/runtime/agent/kube.py` & `surfkit-0.1.93/surfkit/runtime/agent/kube.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.91/surfkit/runtime/agent/load.py` & `surfkit-0.1.93/surfkit/runtime/agent/load.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.91/surfkit/runtime/container/base.py` & `surfkit-0.1.93/surfkit/runtime/container/base.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.91/surfkit/runtime/container/docker.py` & `surfkit-0.1.93/surfkit/runtime/container/docker.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.91/surfkit/runtime/container/kube.py` & `surfkit-0.1.93/surfkit/runtime/container/kube.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.91/surfkit/runtime/container/load.py` & `surfkit-0.1.93/surfkit/runtime/container/load.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.91/surfkit/types.py` & `surfkit-0.1.93/surfkit/types.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.91/surfkit/util.py` & `surfkit-0.1.93/surfkit/util.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.91/PKG-INFO` & `surfkit-0.1.93/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surfkit
-Version: 0.1.91
+Version: 0.1.93
 Summary: A toolkit to build GUI surfing AI agents
 License: MIT
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,15 @@
 Requires-Dist: devicebay (>=0.1.11,<0.2.0)
 Requires-Dist: docker (>=7.0.0,<8.0.0)
 Requires-Dist: kubernetes (>=29.0.0,<30.0.0)
 Requires-Dist: litellm (>=1.35.8,<2.0.0)
 Requires-Dist: namesgenerator (>=0.3,<0.4)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: rootpath (>=0.1.1,<0.2.0)
 Requires-Dist: taskara (>=0.1.42,<0.2.0)
 Requires-Dist: threadmem (>=0.2.11,<0.3.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: toolfuse (>=0.1.15,<0.2.0)
 Description-Content-Type: text/markdown
```

