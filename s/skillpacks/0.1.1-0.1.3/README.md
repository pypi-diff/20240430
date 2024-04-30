# Comparing `tmp/skillpacks-0.1.1.tar.gz` & `tmp/skillpacks-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skillpacks-0.1.1.tar", max compression
+gzip compressed data, was "skillpacks-0.1.3.tar", max compression
```

## Comparing `skillpacks-0.1.1.tar` & `skillpacks-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    11357 2024-01-08 19:16:31.383824 skillpacks-0.1.1/LICENSE
--rw-r--r--   0        0        0     3005 2024-04-28 03:31:24.379154 skillpacks-0.1.1/README.md
--rw-r--r--   0        0        0      560 2024-04-28 03:51:38.507438 skillpacks-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       39 2024-04-28 03:26:42.529534 skillpacks-0.1.1/skillpacks/__init__.py
--rw-r--r--   0        0        0       23 2024-04-28 03:37:56.034277 skillpacks-0.1.1/skillpacks/auth/default.py
--rw-r--r--   0        0        0     2546 2024-04-28 03:37:56.034595 skillpacks-0.1.1/skillpacks/auth/key.py
--rw-r--r--   0        0        0     2112 2024-04-28 03:37:56.034886 skillpacks-0.1.1/skillpacks/auth/provider.py
--rw-r--r--   0        0        0      735 2024-04-28 03:37:56.035160 skillpacks-0.1.1/skillpacks/auth/transport.py
--rw-r--r--   0        0        0    10512 2024-04-28 03:47:25.205588 skillpacks-0.1.1/skillpacks/base.py
--rw-r--r--   0        0        0     1927 2024-04-27 22:14:09.985610 skillpacks-0.1.1/skillpacks/db/conn.py
--rw-r--r--   0        0        0     1698 2024-04-28 03:45:30.335728 skillpacks-0.1.1/skillpacks/db/models.py
--rw-r--r--   0        0        0       74 2024-04-27 19:34:23.040044 skillpacks-0.1.1/skillpacks/env.py
--rw-r--r--   0        0        0        0 2024-02-21 19:35:35.693257 skillpacks-0.1.1/skillpacks/explore.py
--rw-r--r--   0        0        0       87 2024-02-22 23:30:11.834067 skillpacks-0.1.1/skillpacks/history/__init__.py
--rw-r--r--   0        0        0      855 2024-04-26 18:04:27.667449 skillpacks-0.1.1/skillpacks/history/base.py
--rw-r--r--   0        0        0      280 2024-04-26 18:04:50.655262 skillpacks-0.1.1/skillpacks/model/base.py
--rw-r--r--   0        0        0        0 2024-04-26 17:43:23.657039 skillpacks-0.1.1/skillpacks/model/qwenvl.py
--rw-r--r--   0        0        0      779 2024-02-22 00:28:00.918717 skillpacks-0.1.1/skillpacks/models/v1alpha/__init__.py
--rw-r--r--   0        0        0       60 2024-02-22 04:16:18.237373 skillpacks-0.1.1/skillpacks/select/__init__.py
--rw-r--r--   0        0        0     2075 2024-02-22 04:23:43.275020 skillpacks-0.1.1/skillpacks/select/base.py
--rw-r--r--   0        0        0       36 2024-02-22 23:57:15.420929 skillpacks-0.1.1/skillpacks/select/gpt4v/__init__.py
--rw-r--r--   0        0        0     4448 2024-04-26 18:05:05.435366 skillpacks-0.1.1/skillpacks/select/gpt4v/instruct.py
--rw-r--r--   0        0        0      838 2024-02-22 04:46:48.024589 skillpacks-0.1.1/skillpacks/select/gpt4v/oai.py
--rw-r--r--   0        0        0     2387 2024-04-26 18:05:20.328047 skillpacks-0.1.1/skillpacks/select/gpt4v/selector.py
--rw-r--r--   0        0        0     2890 2024-04-26 18:05:28.464384 skillpacks-0.1.1/skillpacks/select/qwenvl/instruct.py
--rw-r--r--   0        0        0     2765 2024-04-26 18:05:35.975702 skillpacks-0.1.1/skillpacks/select/qwenvl/selector.py
--rw-r--r--   0        0        0      230 2024-02-22 04:46:17.754077 skillpacks-0.1.1/skillpacks/select/util.py
--rw-r--r--   0        0        0     1631 2024-04-28 03:41:45.950151 skillpacks-0.1.1/skillpacks/server/models.py
--rw-r--r--   0        0        0     2081 2024-04-28 03:50:44.091111 skillpacks-0.1.1/skillpacks/server/routes/action.py
--rw-r--r--   0        0        0     2606 2024-04-28 03:48:26.634175 skillpacks-0.1.1/skillpacks/server/routes/episode.py
--rw-r--r--   0        0        0     2672 2024-04-26 18:05:48.381201 skillpacks-0.1.1/skillpacks/task_old.py
--rw-r--r--   0        0        0     3616 1970-01-01 00:00:00.000000 skillpacks-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-08 19:16:31.383824 skillpacks-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3025 2024-04-29 03:02:23.181667 skillpacks-0.1.3/README.md
+-rw-r--r--   0        0        0      600 2024-04-29 21:24:17.210973 skillpacks-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       39 2024-04-28 03:26:42.529534 skillpacks-0.1.3/skillpacks/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-28 03:37:56.034277 skillpacks-0.1.3/skillpacks/auth/default.py
+-rw-r--r--   0        0        0     2546 2024-04-28 03:37:56.034595 skillpacks-0.1.3/skillpacks/auth/key.py
+-rw-r--r--   0        0        0     2112 2024-04-28 03:37:56.034886 skillpacks-0.1.3/skillpacks/auth/provider.py
+-rw-r--r--   0        0        0      735 2024-04-28 03:37:56.035160 skillpacks-0.1.3/skillpacks/auth/transport.py
+-rw-r--r--   0        0        0    11392 2024-04-29 21:23:19.876063 skillpacks-0.1.3/skillpacks/base.py
+-rw-r--r--   0        0        0     1927 2024-04-27 22:14:09.985610 skillpacks-0.1.3/skillpacks/db/conn.py
+-rw-r--r--   0        0        0     1604 2024-04-29 21:22:55.291710 skillpacks-0.1.3/skillpacks/db/models.py
+-rw-r--r--   0        0        0       74 2024-04-27 19:34:23.040044 skillpacks-0.1.3/skillpacks/env.py
+-rw-r--r--   0        0        0        0 2024-02-21 19:35:35.693257 skillpacks-0.1.3/skillpacks/explore.py
+-rw-r--r--   0        0        0       87 2024-02-22 23:30:11.834067 skillpacks-0.1.3/skillpacks/history/__init__.py
+-rw-r--r--   0        0        0      855 2024-04-26 18:04:27.667449 skillpacks-0.1.3/skillpacks/history/base.py
+-rw-r--r--   0        0        0      280 2024-04-26 18:04:50.655262 skillpacks-0.1.3/skillpacks/model/base.py
+-rw-r--r--   0        0        0        0 2024-04-26 17:43:23.657039 skillpacks-0.1.3/skillpacks/model/qwenvl.py
+-rw-r--r--   0        0        0      779 2024-02-22 00:28:00.918717 skillpacks-0.1.3/skillpacks/models/v1alpha/__init__.py
+-rw-r--r--   0        0        0       60 2024-02-22 04:16:18.237373 skillpacks-0.1.3/skillpacks/select/__init__.py
+-rw-r--r--   0        0        0     2076 2024-04-29 21:22:30.272421 skillpacks-0.1.3/skillpacks/select/base.py
+-rw-r--r--   0        0        0       36 2024-02-22 23:57:15.420929 skillpacks-0.1.3/skillpacks/select/gpt4v/__init__.py
+-rw-r--r--   0        0        0     4448 2024-04-26 18:05:05.435366 skillpacks-0.1.3/skillpacks/select/gpt4v/instruct.py
+-rw-r--r--   0        0        0      838 2024-02-22 04:46:48.024589 skillpacks-0.1.3/skillpacks/select/gpt4v/oai.py
+-rw-r--r--   0        0        0     2387 2024-04-26 18:05:20.328047 skillpacks-0.1.3/skillpacks/select/gpt4v/selector.py
+-rw-r--r--   0        0        0     2890 2024-04-26 18:05:28.464384 skillpacks-0.1.3/skillpacks/select/qwenvl/instruct.py
+-rw-r--r--   0        0        0     2765 2024-04-26 18:05:35.975702 skillpacks-0.1.3/skillpacks/select/qwenvl/selector.py
+-rw-r--r--   0        0        0      230 2024-02-22 04:46:17.754077 skillpacks-0.1.3/skillpacks/select/util.py
+-rw-r--r--   0        0        0     1756 2024-04-29 21:19:18.545481 skillpacks-0.1.3/skillpacks/server/models.py
+-rw-r--r--   0        0        0     2077 2024-04-29 21:15:22.895837 skillpacks-0.1.3/skillpacks/server/routes/action.py
+-rw-r--r--   0        0        0     2602 2024-04-29 21:15:30.688255 skillpacks-0.1.3/skillpacks/server/routes/episode.py
+-rw-r--r--   0        0        0     2669 2024-04-29 21:23:35.336627 skillpacks-0.1.3/skillpacks/task_old.py
+-rw-r--r--   0        0        0     3594 1970-01-01 00:00:00.000000 skillpacks-0.1.3/PKG-INFO
```

### Comparing `skillpacks-0.1.1/LICENSE` & `skillpacks-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.1/README.md` & `skillpacks-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -78,16 +78,16 @@
 
 Mark actions as approved
 
 ```python
 # approve one
 episode.approve_one(event.id)
 
-# approve all actions before the event
-episode.approve_previous(event.id)
+# approve the event and all actions prior to it
+episode.approve_prior(event.id)
 
 # approve all
 episode.approve_all()
 ```
 
 Get all approved actions in an episode
 
@@ -106,15 +106,15 @@
 
 Get all approved actions for a tool
 
 ```python
 actions = ActionEvent.find(tool=desktop.ref(), approved=True)
 ```
 
-Tune a model on the actions
+Tune a model on the actions (In progress)
 
 ```python
 from skillpacks.model import InternVLChat
 from skillpacks.runtime import KubernetesRuntime
 
 runtime = KubernetesRuntime()
 model = InternVLChat(runtime=runtime)
```

#### html2text {}

```diff
@@ -17,21 +17,22 @@
 are {desktop.json_schema()} please return your selection as
 {V1Action.model_json_schema()} """ thread.post(role="user", msg=msg) response =
 router.chat(thread, expect=V1Action) v1action = response.parsed action =
 desktop.find_action(name=v1action.name) result = desktop.use(action,
 **v1action.parameters) ``` Record the action in the episode ```python event =
 episode.record( prompt=response.prompt_id, action=v1action, tool=desktop.ref(),
 result=result, ) ``` Mark actions as approved ```python # approve one
-episode.approve_one(event.id) # approve all actions before the event
-episode.approve_previous(event.id) # approve all episode.approve_all() ``` Get
-all approved actions in an episode ```python episode = Episode.find(id="123")
-[0] actions = episode.approved_actions() ``` Get all approved actions in a
+episode.approve_one(event.id) # approve the event and all actions prior to it
+episode.approve_prior(event.id) # approve all episode.approve_all() ``` Get all
+approved actions in an episode ```python episode = Episode.find(id="123")[0]
+actions = episode.approved_actions() ``` Get all approved actions in a
 namespace ```python from skillpacks import ActionEvent actions =
 ActionEvent.find(namespace="foo", approved=True) ``` Get all approved actions
 for a tool ```python actions = ActionEvent.find(tool=desktop.ref(),
-approved=True) ``` Tune a model on the actions ```python from skillpacks.model
-import InternVLChat from skillpacks.runtime import KubernetesRuntime runtime =
-KubernetesRuntime() model = InternVLChat(runtime=runtime) result = model.train
-(actions=actions, follow=True, publish=True) ``` ## Backends Thread and prompt
-storage can be backed by: - Sqlite - Postgresql Sqlite will be used by default.
-To use postgres simply configure the env vars: ```sh DB_TYPE=postgres
-DB_NAME=skills DB_HOST=localhost DB_USER=postgres DB_PASS=abc123 ```
+approved=True) ``` Tune a model on the actions (In progress) ```python from
+skillpacks.model import InternVLChat from skillpacks.runtime import
+KubernetesRuntime runtime = KubernetesRuntime() model = InternVLChat
+(runtime=runtime) result = model.train(actions=actions, follow=True,
+publish=True) ``` ## Backends Thread and prompt storage can be backed by: -
+Sqlite - Postgresql Sqlite will be used by default. To use postgres simply
+configure the env vars: ```sh DB_TYPE=postgres DB_NAME=skills DB_HOST=localhost
+DB_USER=postgres DB_PASS=abc123 ```
```

### Comparing `skillpacks-0.1.1/pyproject.toml` & `skillpacks-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [tool.poetry]
 name = "skillpacks"
-version = "0.1.1"
+version = "0.1.3"
 description = "Pluggable skills for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^2.6.1"
 sqlalchemy = "^2.0.27"
-agentdesk = "^0.2.7"
-mllm = "^0.1.3"
+mllm = "^0.1.5"
 
 
 [tool.poetry.group.openai.dependencies]
 openai = "^1.12.0"
 
 
 [tool.poetry.group.qwen.dependencies]
 transformers = "^4.38.1"
 frequency-ai = "^0.1.8"
 
+
+[tool.poetry.group.dev.dependencies]
+agentdesk = "^0.2.65"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `skillpacks-0.1.1/skillpacks/auth/key.py` & `skillpacks-0.1.3/skillpacks/auth/key.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.1/skillpacks/auth/provider.py` & `skillpacks-0.1.3/skillpacks/auth/provider.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.1/skillpacks/auth/transport.py` & `skillpacks-0.1.3/skillpacks/auth/transport.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.1/skillpacks/base.py` & `skillpacks-0.1.3/skillpacks/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import time
 from typing import Dict, Any, Optional, List
 import uuid
 import json
 import os
 
 from pydantic import BaseModel
-from mllm import Prompt, PromptModel
+from mllm import Prompt, V1Prompt
 from sqlalchemy import asc
 
 from .db.conn import WithDB
 from .db.models import ActionRecord, EpisodeRecord
 from .server.models import (
     V1ActionEvent,
     V1ToolRef,
@@ -30,57 +30,68 @@
         tool: V1ToolRef,
         result: Optional[Any] = None,
         namespace: str = "default",
         metadata: dict = {},
         approved: bool = False,
         flagged: bool = False,
         owner_id: Optional[str] = None,
+        model: Optional[str] = None,
+        agent_id: Optional[str] = None,
     ) -> None:
         self.id = str(uuid.uuid4())
         self.prompt = prompt
         self.action = action
         self.result = result
         self.tool = tool
         self.namespace = namespace
         self.metadata = metadata
         self.created = time.time()
         self.approved = approved
         self.flagged = flagged
         self.owner_id = owner_id
+        self.model = model
+        self.agent_id = agent_id
 
     def approve(self) -> None:
         self.approved = True
+        self.prompt.approved = True
         self.save()
 
     def to_v1(self) -> V1ActionEvent:
         return V1ActionEvent(
             id=self.id,
-            prompt=self.prompt.to_schema(),
+            prompt=self.prompt.to_v1(),
             action=self.action,
             result=self.result,
             tool=self.tool,
             namespace=self.namespace,
             created=self.created,
+            approved=self.approved,
+            flagged=self.flagged,
+            model=self.model,
+            agent_id=self.agent_id,
         )
 
     @classmethod
     def from_v1(
         cls, v1: V1ActionEvent, owner_id: Optional[str] = None
     ) -> "ActionEvent":
         event = cls.__new__(cls)
         event.id = v1.id
-        event.prompt = Prompt.from_schema(v1.prompt)
+        event.prompt = Prompt.from_v1(v1.prompt)
         event.action = v1.action
         event.result = v1.result
         event.tool = v1.tool
         event.namespace = v1.namespace
         event.created = v1.created
         event.approved = v1.approved
         event.flagged = v1.flagged
         event.owner_id = owner_id
+        event.model = v1.model
+        event.agent_id = v1.agent_id
         return event
 
     def save(self) -> None:
         """Saves the instance to the database."""
         for db in self.get_db():
             record = self.to_record()
             db.merge(record)
@@ -96,14 +107,16 @@
             tool=json.dumps(self.tool.model_dump()),
             namespace=self.namespace,
             metadata_=json.dumps(self.metadata),
             approved=self.approved,
             flagged=self.flagged,
             created=self.created,
             owner_id=self.owner_id,
+            model=self.model,
+            agent_id=self.agent_id,
         )
 
     @classmethod
     def from_record(cls, record: ActionRecord) -> "ActionEvent":
         """Creates an instance from a database record using the __new__ method."""
         event = cls.__new__(cls)
         event.id = record.id
@@ -113,14 +126,16 @@
         event.tool = V1ToolRef.model_validate_json(str(record.tool))
         event.namespace = record.namespace
         event.metadata = json.loads(str(record.metadata_))
         event.created = record.created
         event.approved = record.approved
         event.flagged = record.flagged
         event.owner_id = record.owner_id
+        event.model = record.model
+        event.agent_id = record.agent_id
         return event
 
     @classmethod
     def find(cls, tool: Optional[V1ToolRef] = None, **kwargs) -> List["ActionEvent"]:
         for db in cls.get_db():
             records = (
                 db.query(ActionRecord)
@@ -203,26 +218,32 @@
         self,
         prompt: Prompt | str,
         action: V1Action,
         tool: V1ToolRef,
         result: Optional[Any] = None,
         namespace: str = "default",
         metadata: dict = {},
+        owner_id: Optional[str] = None,
+        model: Optional[str] = None,
+        agent_id: Optional[str] = None,
     ) -> ActionEvent:
         """Records an action to the episode."""
         if isinstance(prompt, str):
             prompt = Prompt.find(prompt_id=prompt)[0]
 
         event = ActionEvent(
             prompt=prompt,
             action=action,
             result=result,
             tool=tool,
             namespace=namespace,
             metadata=metadata,
+            owner_id=owner_id,
+            model=model,
+            agent_id=agent_id,
         )
         self.record_event(event)
 
         return event
 
     def save(self) -> None:
         """Saves the instance to the database."""
@@ -294,31 +315,35 @@
     def approve_one(self, event_id: str) -> None:
         """Approve the given event."""
         events = ActionEvent.find(id=event_id)
         if not events:
             raise ValueError("No event found")
         event = events[0]
         event.approved = True
+        event.prompt.approved = True
         self.save()
 
     def approve_all(self) -> None:
         """Approve all actions in the episode."""
         for event in self.actions:
             event.approved = True
+            event.prompt.approved = True
         self.save()
 
-    def approve_previous(self, event_id: str) -> None:
-        """Approve the given event and all previous actions."""
+    def approve_prior(self, event_id: str) -> None:
+        """Approve the given event and all prior actions."""
         events = ActionEvent.find(id=event_id)
         if not events:
             raise ValueError("No event found")
         event = events[0]
         event.approved = True
+        event.prompt.approved = True
         for i in range(len(self.actions) - 1):
             if self.actions[i].id == event_id:
                 for j in range(i + 1, len(self.actions)):
                     self.actions[j].approved = True
+                    self.actions[j].prompt.approved = True
         self.save()
 
     def approved_actions(self) -> List[ActionEvent]:
         """Returns a list of approved actions."""
         return [action for action in self.actions if action.approved]
```

### Comparing `skillpacks-0.1.1/skillpacks/db/conn.py` & `skillpacks-0.1.3/skillpacks/db/conn.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.1/skillpacks/db/models.py` & `skillpacks-0.1.3/skillpacks/db/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,37 +4,29 @@
 from sqlalchemy.orm import relationship
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.dialects.postgresql import JSONB  # If using PostgreSQL
 
 Base = declarative_base()
 
 
-# def __init__(
-#     self,
-#     prompt: Prompt,
-#     action: V1Action,
-#     result: Any,
-#     tool: V1ToolRef,
-#     namespace: str = "default",
-#     metadata: dict = {},
-
-
 class ActionRecord(Base):
     __tablename__ = "actions"
 
     id = Column(String, primary_key=True)
     owner_id = Column(String, nullable=True)
     namespace = Column(String, default="default")
     prompt_id = Column(String)
     action = Column(Text)
     result = Column(Text)
     tool = Column(Text)
     metadata_ = Column(Text, default=dict)
     approved = Column(Boolean, default=False)
     flagged = Column(Boolean, default=False)
+    model = Column(String, default=None)
+    agent_id = Column(String, default=None)
     created = Column(Float, default=time.time)
 
     episode_id = Column(String, ForeignKey("episodes.id"), nullable=True)
     episode = relationship("EpisodeRecord", back_populates="actions")
 
 
 class EpisodeRecord(Base):
```

### Comparing `skillpacks-0.1.1/skillpacks/history/base.py` & `skillpacks-0.1.3/skillpacks/history/base.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.1/skillpacks/models/v1alpha/__init__.py` & `skillpacks-0.1.3/skillpacks/models/v1alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.1/skillpacks/select/base.py` & `skillpacks-0.1.3/skillpacks/select/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC, abstractmethod
 from typing import List
 
-from agent_tools import Action, Observation
+from toolfuse import Action, Observation
 
-from skillpacks.task import Attempt
+from skillpacks.task_old import Attempt
 
 
 class Selector(ABC):
     """Selects actions and observations for a task attempt"""
 
     @abstractmethod
     def select_observations(self, attempt: Attempt) -> List[Observation]:
```

### Comparing `skillpacks-0.1.1/skillpacks/select/gpt4v/instruct.py` & `skillpacks-0.1.3/skillpacks/select/gpt4v/instruct.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.1/skillpacks/select/gpt4v/oai.py` & `skillpacks-0.1.3/skillpacks/select/gpt4v/oai.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.1/skillpacks/select/gpt4v/selector.py` & `skillpacks-0.1.3/skillpacks/select/gpt4v/selector.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.1/skillpacks/select/qwenvl/instruct.py` & `skillpacks-0.1.3/skillpacks/select/qwenvl/instruct.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.1/skillpacks/select/qwenvl/selector.py` & `skillpacks-0.1.3/skillpacks/select/qwenvl/selector.py`

 * *Files identical despite different names*

### Comparing `skillpacks-0.1.1/skillpacks/server/models.py` & `skillpacks-0.1.3/skillpacks/server/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, Dict, Any, List
 
 from pydantic import BaseModel
-from mllm import PromptModel
+from mllm import V1Prompt
 
 
 class V1ToolRef(BaseModel):
     """A reference to a tool or device"""
 
     module: str
     name: str
@@ -27,41 +27,45 @@
     action: V1Action
 
 
 class V1ActionEvent(BaseModel):
     """An action that has occurred"""
 
     id: str
-    prompt: PromptModel
+    prompt: V1Prompt
     action: V1Action
     result: Any
     tool: V1ToolRef
     namespace: str
     approved: bool = False
     flagged: bool = False
+    model: Optional[str] = None
+    agent_id: Optional[str] = None
     created: float
 
 
 class V1ActionEvents(BaseModel):
     """A list of action events"""
 
     events: List[V1ActionEvent] = []
 
 
 class V1CreateActionEvent(BaseModel):
     """An action that has occurred"""
 
-    prompt: PromptModel
+    prompt: V1Prompt
     action: V1Action
     result: Any
     tool: V1ToolRef
     namespace: str
     metadata: dict = {}
     approved: bool = False
     flagged: bool = False
+    model: Optional[str] = None
+    agent_id: Optional[str] = None
 
 
 class V1Episode(BaseModel):
     """An agent episode"""
 
     actions: List[V1ActionEvent] = []
     tags: List[str] = []
```

### Comparing `skillpacks-0.1.1/skillpacks/server/routes/action.py` & `skillpacks-0.1.3/skillpacks/server/routes/action.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 @router.post("/v1/actions", response_model=V1ActionEvent)
 async def create_action_event(
     current_user: Annotated[V1UserProfile, Depends(get_current_user)],
     data: V1CreateActionEvent,
 ):
     event = ActionEvent(
-        prompt=Prompt.from_schema(data.prompt),
+        prompt=Prompt.from_v1(data.prompt),
         action=data.action,
         tool=data.tool,
         result=data.result,
         namespace=data.namespace,
         metadata=data.metadata,
         approved=data.approved,
         flagged=data.flagged,
```

### Comparing `skillpacks-0.1.1/skillpacks/server/routes/episode.py` & `skillpacks-0.1.3/skillpacks/server/routes/episode.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 ):
     episodes = Episode.find(id=id, owner_id=current_user.email)
     if not episodes:
         raise HTTPException(status_code=404, detail="Episode not found")
     episode = episodes[0]
 
     event = ActionEvent(
-        prompt=Prompt.from_schema(data.prompt),
+        prompt=Prompt.from_v1(data.prompt),
         action=data.action,
         tool=data.tool,
         result=data.result,
         namespace=data.namespace,
         metadata=data.metadata,
         approved=data.approved,
         flagged=data.flagged,
```

### Comparing `skillpacks-0.1.1/skillpacks/task_old.py` & `skillpacks-0.1.3/skillpacks/task_old.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # type: ignore
 from typing import List, Optional, Any
 from enum import Enum
 from dataclasses import dataclass
 import uuid
 
-from agent_tools import Tool
+from toolfuse import Tool
 
 from skillpacks.models.v1alpha import (
     V1ActionEvent,
     V1Attempt,
     V1AcceptedSolution,
     V1StateAction,
     V1Task,
```

### Comparing `skillpacks-0.1.1/PKG-INFO` & `skillpacks-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: skillpacks
-Version: 0.1.1
+Version: 0.1.3
 Summary: Pluggable skills for AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: agentdesk (>=0.2.7,<0.3.0)
-Requires-Dist: mllm (>=0.1.3,<0.2.0)
+Requires-Dist: mllm (>=0.1.5,<0.2.0)
 Requires-Dist: pydantic (>=2.6.1,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.27,<3.0.0)
 Description-Content-Type: text/markdown
 
 <!-- PROJECT LOGO -->
 <br />
 <p align="center">
@@ -96,16 +95,16 @@
 
 Mark actions as approved
 
 ```python
 # approve one
 episode.approve_one(event.id)
 
-# approve all actions before the event
-episode.approve_previous(event.id)
+# approve the event and all actions prior to it
+episode.approve_prior(event.id)
 
 # approve all
 episode.approve_all()
 ```
 
 Get all approved actions in an episode
 
@@ -124,15 +123,15 @@
 
 Get all approved actions for a tool
 
 ```python
 actions = ActionEvent.find(tool=desktop.ref(), approved=True)
 ```
 
-Tune a model on the actions
+Tune a model on the actions (In progress)
 
 ```python
 from skillpacks.model import InternVLChat
 from skillpacks.runtime import KubernetesRuntime
 
 runtime = KubernetesRuntime()
 model = InternVLChat(runtime=runtime)
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: skillpacks Version: 0.1.1 Summary: Pluggable skills
+Metadata-Version: 2.1 Name: skillpacks Version: 0.1.3 Summary: Pluggable skills
 for AI agents License: Apache 2.0 Author: Patrick Barker Author-email:
 patrickbarkerco@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
 Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: agentdesk (>=0.2.7,<0.3.0) Requires-
-Dist: mllm (>=0.1.3,<0.2.0) Requires-Dist: pydantic (>=2.6.1,<3.0.0) Requires-
-Dist: sqlalchemy (>=2.0.27,<3.0.0) Description-Content-Type: text/markdown
+Language :: Python :: 3.11 Requires-Dist: mllm (>=0.1.5,<0.2.0) Requires-Dist:
+pydantic (>=2.6.1,<3.0.0) Requires-Dist: sqlalchemy (>=2.0.27,<3.0.0)
+Description-Content-Type: text/markdown
                            ************ SSkkiillllPPaacckkss ************
                       Pluggable skillsets for AI agents
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
                   _V_i_e_w_ _D_e_m_o Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 Skillpacks provide a means of fine tuning agents on tools, and the ability to
 hotswap learned skills at inference time. Teach a model how to use a
@@ -24,21 +24,22 @@
 are {desktop.json_schema()} please return your selection as
 {V1Action.model_json_schema()} """ thread.post(role="user", msg=msg) response =
 router.chat(thread, expect=V1Action) v1action = response.parsed action =
 desktop.find_action(name=v1action.name) result = desktop.use(action,
 **v1action.parameters) ``` Record the action in the episode ```python event =
 episode.record( prompt=response.prompt_id, action=v1action, tool=desktop.ref(),
 result=result, ) ``` Mark actions as approved ```python # approve one
-episode.approve_one(event.id) # approve all actions before the event
-episode.approve_previous(event.id) # approve all episode.approve_all() ``` Get
-all approved actions in an episode ```python episode = Episode.find(id="123")
-[0] actions = episode.approved_actions() ``` Get all approved actions in a
+episode.approve_one(event.id) # approve the event and all actions prior to it
+episode.approve_prior(event.id) # approve all episode.approve_all() ``` Get all
+approved actions in an episode ```python episode = Episode.find(id="123")[0]
+actions = episode.approved_actions() ``` Get all approved actions in a
 namespace ```python from skillpacks import ActionEvent actions =
 ActionEvent.find(namespace="foo", approved=True) ``` Get all approved actions
 for a tool ```python actions = ActionEvent.find(tool=desktop.ref(),
-approved=True) ``` Tune a model on the actions ```python from skillpacks.model
-import InternVLChat from skillpacks.runtime import KubernetesRuntime runtime =
-KubernetesRuntime() model = InternVLChat(runtime=runtime) result = model.train
-(actions=actions, follow=True, publish=True) ``` ## Backends Thread and prompt
-storage can be backed by: - Sqlite - Postgresql Sqlite will be used by default.
-To use postgres simply configure the env vars: ```sh DB_TYPE=postgres
-DB_NAME=skills DB_HOST=localhost DB_USER=postgres DB_PASS=abc123 ```
+approved=True) ``` Tune a model on the actions (In progress) ```python from
+skillpacks.model import InternVLChat from skillpacks.runtime import
+KubernetesRuntime runtime = KubernetesRuntime() model = InternVLChat
+(runtime=runtime) result = model.train(actions=actions, follow=True,
+publish=True) ``` ## Backends Thread and prompt storage can be backed by: -
+Sqlite - Postgresql Sqlite will be used by default. To use postgres simply
+configure the env vars: ```sh DB_TYPE=postgres DB_NAME=skills DB_HOST=localhost
+DB_USER=postgres DB_PASS=abc123 ```
```

