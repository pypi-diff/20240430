# Comparing `tmp/opentldr-0.4.1.tar.gz` & `tmp/opentldr-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentldr-0.4.1.tar", last modified: Wed Apr  3 03:57:46 2024, max compression
+gzip compressed data, was "opentldr-0.4.2.tar", last modified: Tue Apr 30 16:58:23 2024, max compression
```

## Comparing `opentldr-0.4.1.tar` & `opentldr-0.4.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:57:46.098998 opentldr-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 03:57:41.000000 opentldr-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 03:57:41.000000 opentldr-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-04-03 03:57:46.098998 opentldr-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-04-03 03:57:41.000000 opentldr-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-03 03:57:41.000000 opentldr-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 03:57:46.098998 opentldr-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:57:46.094998 opentldr-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:57:46.098998 opentldr-0.4.1/src/opentldr/
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-03 03:57:41.000000 opentldr-0.4.1/src/opentldr/AbstractDataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-03 03:57:41.000000 opentldr-0.4.1/src/opentldr/DataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-03 03:57:41.000000 opentldr-0.4.1/src/opentldr/DataRepoJson.py
--rw-r--r--   0 runner    (1001) docker     (127)    25936 2024-04-03 03:57:41.000000 opentldr-0.4.1/src/opentldr/Domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    29794 2024-04-03 03:57:41.000000 opentldr-0.4.1/src/opentldr/KnowledgeGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-03 03:57:41.000000 opentldr-0.4.1/src/opentldr/S3DataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-04-03 03:57:41.000000 opentldr-0.4.1/src/opentldr/TextFileDataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-03 03:57:41.000000 opentldr-0.4.1/src/opentldr/Workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-03 03:57:41.000000 opentldr-0.4.1/src/opentldr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-03 03:57:41.000000 opentldr-0.4.1/src/opentldr/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:57:46.098998 opentldr-0.4.1/src/opentldr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-04-03 03:57:46.000000 opentldr-0.4.1/src/opentldr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-03 03:57:46.000000 opentldr-0.4.1/src/opentldr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 03:57:46.000000 opentldr-0.4.1/src/opentldr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-03 03:57:46.000000 opentldr-0.4.1/src/opentldr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 03:57:46.000000 opentldr-0.4.1/src/opentldr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:57:46.098998 opentldr-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 03:57:41.000000 opentldr-0.4.1/tests/test_contentrepo.py
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 03:57:41.000000 opentldr-0.4.1/tests/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-03 03:57:41.000000 opentldr-0.4.1/tests/test_knowledgegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 03:57:41.000000 opentldr-0.4.1/tests/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:58:23.434674 opentldr-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 16:58:18.000000 opentldr-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:58:18.000000 opentldr-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-04-30 16:58:23.434674 opentldr-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-04-30 16:58:18.000000 opentldr-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-30 16:58:18.000000 opentldr-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 16:58:23.434674 opentldr-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:58:23.430674 opentldr-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:58:23.434674 opentldr-0.4.2/src/opentldr/
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-30 16:58:18.000000 opentldr-0.4.2/src/opentldr/AbstractDataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-30 16:58:18.000000 opentldr-0.4.2/src/opentldr/DataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-30 16:58:18.000000 opentldr-0.4.2/src/opentldr/DataRepoJson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28123 2024-04-30 16:58:18.000000 opentldr-0.4.2/src/opentldr/Domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-30 16:58:18.000000 opentldr-0.4.2/src/opentldr/FileSystemDataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30752 2024-04-30 16:58:18.000000 opentldr-0.4.2/src/opentldr/KnowledgeGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-30 16:58:18.000000 opentldr-0.4.2/src/opentldr/S3DataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-30 16:58:18.000000 opentldr-0.4.2/src/opentldr/Workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-30 16:58:18.000000 opentldr-0.4.2/src/opentldr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-30 16:58:18.000000 opentldr-0.4.2/src/opentldr/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:58:23.434674 opentldr-0.4.2/src/opentldr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-04-30 16:58:23.000000 opentldr-0.4.2/src/opentldr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-30 16:58:23.000000 opentldr-0.4.2/src/opentldr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:58:23.000000 opentldr-0.4.2/src/opentldr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-30 16:58:23.000000 opentldr-0.4.2/src/opentldr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 16:58:23.000000 opentldr-0.4.2/src/opentldr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:58:23.434674 opentldr-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-30 16:58:18.000000 opentldr-0.4.2/tests/test_contentrepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-30 16:58:18.000000 opentldr-0.4.2/tests/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-30 16:58:18.000000 opentldr-0.4.2/tests/test_knowledgegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-30 16:58:18.000000 opentldr-0.4.2/tests/test_workflow.py
```

### Comparing `opentldr-0.4.1/LICENSE` & `opentldr-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opentldr-0.4.1/PKG-INFO` & `opentldr-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentldr
-Version: 0.4.1
+Version: 0.4.2
 Summary: An open framework for creation of a Tailored Daily Report.
 Author-email: Chris Argenta <cargenta@rockfishresearch.com>
 Project-URL: Source, https://github.com/RockfishResearch/OpenTLDR-Core.git
 Project-URL: Issues, https://github.com/RockfishResearch/OpenTLDR-Core/issues
 Project-URL: Documentation, http://www.opentldr.org/docs
 Project-URL: Homepage, http://www.opentldr.org
 Classifier: Programming Language :: Python :: 3
@@ -17,16 +17,17 @@
 License-File: LICENSE
 Requires-Dist: python-dotenv>=1.0.0
 Requires-Dist: neo4j>=5.15.0
 Requires-Dist: neomodel>=5.2.1
 Requires-Dist: papermill>=2.5.0
 Requires-Dist: boto3>=1.34.55
 
-# OpenTLDR
+# OpenTLDR-Core
 An Open Framework for Generating an Tailored Daily Report
+This repository contains the OpenTLDR package. You can 'pip install opentldr' to get the contents of this repository as a python package in your virtaul env.
 
 ![overview image](resources/opentldr.png)
 
 ## Introduction to OpenTLDR
 
 OpenTLDR is an open source framework written in Python to implement the process of creating a Tailored Daily Report from a series of news-like articles. This repository contains the Core classes used as a library by OpenTLDR implementations, like the example notebooks you canf ind in the OpenTLDR-Example repo on GitHub.
```

### Comparing `opentldr-0.4.1/README.md` & `opentldr-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# OpenTLDR
+# OpenTLDR-Core
 An Open Framework for Generating an Tailored Daily Report
+This repository contains the OpenTLDR package. You can 'pip install opentldr' to get the contents of this repository as a python package in your virtaul env.
 
 ![overview image](resources/opentldr.png)
 
 ## Introduction to OpenTLDR
 
 OpenTLDR is an open source framework written in Python to implement the process of creating a Tailored Daily Report from a series of news-like articles. This repository contains the Core classes used as a library by OpenTLDR implementations, like the example notebooks you canf ind in the OpenTLDR-Example repo on GitHub.
```

### Comparing `opentldr-0.4.1/pyproject.toml` & `opentldr-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "opentldr"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="Chris Argenta", email="cargenta@rockfishresearch.com" },
 ]
 description = "An open framework for creation of a Tailored Daily Report."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `opentldr-0.4.1/src/opentldr/AbstractDataRepo.py` & `opentldr-0.4.2/src/opentldr/AbstractDataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.4.1/src/opentldr/DataRepo.py` & `opentldr-0.4.2/src/opentldr/DataRepo.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from dotenv import load_dotenv
 load_dotenv()
 
 from .KnowledgeGraph import KnowledgeGraph
 
 from .AbstractDataRepo import AbstractDataRepo
-from .TextFileDataRepo import TextFileDataRepo
+from .FileSystemDataRepo import FileSystemDataRepo
 from .S3DataRepo import S3DataRepo
 
 from .log import log
 
 class DataRepo(AbstractDataRepo):
     '''
     Factory class to setup any type of DataRepo from the configuration inputs.
@@ -56,15 +56,15 @@
                 aws_access_key_id=self._configOrEnv("aws_access_key_id",config)
                 aws_secret_access_key=self._configOrEnv("aws_secret_access_key",config)
                 prefix=self._configOrEnv("prefix",config)
                 self.repo= S3DataRepo(kg,bucket_name=bucket_name, aws_access_key_id=aws_access_key_id, 
                                       aws_secret_access_key=aws_secret_access_key, prefix=prefix)
             case "files":
                 ingest_path=self._configOrEnv("path",config)
-                self.repo= TextFileDataRepo(kg,ingest_path=ingest_path)
+                self.repo= FileSystemDataRepo(kg,ingest_path=ingest_path)
             case _:
                 message:str = "Invalid 'type' config ('{type}').".format(type=type)
                 log.error(message)
                 raise NotImplementedError(message)
 
     def importData(self) -> list[str]:
         if self.repo is None:
```

### Comparing `opentldr-0.4.1/src/opentldr/DataRepoJson.py` & `opentldr-0.4.2/src/opentldr/DataRepoJson.py`

 * *Files 11% similar despite different names*

```diff
@@ -73,38 +73,15 @@
             ref_edge = ReferenceEdge.from_json(ref_edge_json)
             # TODO: set the to/from uids into neomodel object
             ref_edge.save()
             edge_uids.append(ref_edge.uid)
         log.info("Imported {c} Reference Edges.".format(len(edge_uids)))
 
         return {"ReferenceNodes":node_uids, "ReferenceEdges":edge_uids}
-
-    def exportReferenceData(self):
-        log.info("Exporting Reference Data to JSON File...")
-
-        # Import Reference Nodes
-        node_uids:list[str] = []
-        for ref_node_json in self.data['reference']['nodes']:
-            ref_node = ReferenceNode.from_json(ref_node_json)
-            ref_node.save()
-            node_uids.append(ref_node.uid)
-            node_look_up[ref_node.uid]=ref_node
-        log.info("Imported {c} Reference Nodes.".format(len(node_uids)))
-
-        # Import Reference Edges
-        edge_uids:list[str] = []
-        for ref_edge_json in self.data['reference']['edges']:
-            ref_edge = ReferenceEdge.from_json(ref_edge_json)
-            # TODO: set the to/from uids into neomodel object
-            ref_edge.save()
-            edge_uids.append(ref_edge.uid)
-        log.info("Imported {c} Reference Edges.".format(len(edge_uids)))
-
-        return {"ReferenceNodes":node_uids, "ReferenceEdges":edge_uids}   
-
+    
 
     def importRequestData(self) -> list[str]:
         log.info("Importing Requests from File System...")
 
         path = self.ingest_path
         alt_path = os.path.join(self.ingest_path,"requests")
         if os.path.exists(alt_path) and os.path.isdir(alt_path) and os.access(alt_path,os.R_OK):
```

### Comparing `opentldr-0.4.1/src/opentldr/Domain.py` & `opentldr-0.4.2/src/opentldr/Domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 class OpenTldrMeta():
     '''
     OpenTldrMeta is a mixin class that adds a unique id (uid) and JSON property (metadata)
     to a Node or Edge. This is used in every Edge and Node in OpenTLDR and provides an
     interface for PyDantic for data manipulation and JSON.
     '''
     uid=nm.UniqueIdProperty()
-    metadata=nm.JSONProperty(default="{}")
+    metadata=nm.JSONProperty(default={})
        
     def to_text(self) -> str:
         '''
         to_text() returns a user readable string representing the values in the object.
         '''
         return "uid: {uid}".format(uid=self.uid)
 
@@ -85,15 +85,17 @@
     def to_json(self,kg) -> str:
         data = self.__properties__.copy()
         if "date" in data:
             data["date"]=data["date"].strftime("%m/%d/%Y")
         data["class"]=type(self).__name__
         if "element_id_property" in data:
             data.pop("element_id_property")
-        data.update(self.to_json_connect(kg, data))
+        connection = self.to_json_connect(kg, data)
+        if connection is not None:
+            data.update(connection)
         return json.dumps(data)
 
     def to_json_connect(self, kg, json_dict) -> dict:
         '''
         override to_json_connect to insert edge data into the node.
 
         '''
@@ -115,19 +117,53 @@
     @abstractmethod
     def get_connection_json() -> dict:
         pass
 
     @classmethod
     def from_json(cls, kg, json_string):
         json_dict=json.loads(json_string)
+        if "class" in json_dict:
+            json_dict.pop("class")
+        if "date" in json_dict:
+            json_dict["date"]=inferDateFormat(json_dict["date"])
+        node = cls(**json_dict)
+        node.from_json_connect(kg, json_dict)
+        node.save()
+        return node
+        
+    def to_json(self,kg) -> str:
+        data = self.__properties__.copy()
+        if "date" in data:
+            data["date"]=data["date"].strftime("%m/%d/%Y")
+        data["class"]=type(self).__name__
+        if "element_id_property" in data:
+            data.pop("element_id_property")
+        connection = self.to_json_connect(kg, data)
+        if connection is not None:
+            data.update(connection)
+        return json.dumps(data)
+
+    def to_json_connect(self, kg, json_dict) -> dict:
+        '''
+        override to_json_connect to insert edge data into the node.
+
+        '''
+        pass
+
+    def from_json_connect(self, kg, json_dict):
+        '''
+        override from_json_connect to rebuild edge data from serialized node.
+        '''
+        pass
+
+    @classmethod
+    def from_json(cls, kg, json_string):
+        json_dict=json.loads(json_string)
         if "connection" in json_dict:
             connection=json_dict["connection"]
-            
-            print(connection["start"])
-            print(connection["end"])
 
             from_node=kg.get_by_uid(connection["start"])
             #print("FROM: {type}\t{uid}\t{desc}".format(type=type(from_node),uid=from_node.uid,desc=from_node.to_text()))
             
             to_node=kg.get_by_uid(connection["end"])
             #print("to: {type}\t{uid}\t{desc}".format(type=type(to_node),uid=to_node.uid,desc=to_node.to_text()))
 
@@ -138,15 +174,15 @@
             edge= rel.connect(to_node,json_dict)
             edge.save()
             return edge
         else:
             raise TypeError("OpenTldrEdge requires connection data stored in json.")
 
         
-    def to_json(self) -> str:
+    def to_json(self,kg) -> str:
         data = self.__properties__.copy()
         data["class"]=type(self).__name__
         data["connection"]=self.get_connection_json()
         if "element_id_property" in data:
             data.pop("element_id_property")
         return json.dumps(data)
 
@@ -313,14 +349,17 @@
     '''
     title = nm.StringProperty(required=True)
     date = nm.properties.DateProperty(required=True)
     url = nm.StringProperty(required=True)
 
     is_from = nm.RelationshipTo(Source, 'IS_FROM', model=IsFrom, cardinality=One)
 
+    def get_is_from(self) -> Source:
+        return self.is_from.single()
+
     def to_text(self) -> str:
         return "A {content_type} content titled '{content_title}' from {date}.".format(
             content_type= self.type,
             content_title=self.title,
             date=self.date)
     
     def to_json_connect(self, kg, json_dict) -> dict:
@@ -367,14 +406,19 @@
     (e.g., Content or Requests) that "refers_to" some ReferenceNode information. The text property
     contains the text for the entity identified and they type property expresses what it is.
     The "refers_to" edge can be uncertain (e.g., sematic similarity of text and type consistency). 
     '''
     refers_to=nm.RelationshipTo(ReferenceNode,'REFERS_TO', model = RefersTo, cardinality=ZeroOrMore)  
     mentioned_in = nm.RelationshipTo("CitableNode", 'MENTIONED_IN', model=MentionedIn, cardinality=OneOrMore)
 
+    def get_refers_to(self) -> list[Source]:
+        return self.refers_to
+    
+    def get_mentioned_in(self) -> Source:
+        return self.mentioned_in.single()
 
 
 # Information Request
 
 
 class User(nm.StructuredNode, OpenTldrMeta, OpenTldrNode):
     '''
@@ -408,23 +452,30 @@
     links each request to one User node.
     '''
     title=nm.StringProperty(required=True)
     text = nm.StringProperty(required=True)
 
     requested_by = nm.RelationshipTo(User, 'REQUESTED_BY', model=RequestedBy, cardinality=One)
 
+    def get_requested_by(self) -> User:
+        return self.requested_by.single()
+
     def to_text(self) -> str:
         return "The request titled '{title}'.".format(title=self.title)
 
     def to_json_connect(self, kg, json_dict) -> dict:
         out:dict= {}
+        user:User = self.requested_by.single()
+        log.warn("USER: {}".format(user))
+
         if "user" not in json_dict:
-            out["user"]=self.requested_by.single().name
+            out["user"]=user.name
         if "email" not in json_dict:
-            out["email"]=self.requested_by.single().email
+            out["email"]=user.email
+
         return out
 
     def from_json_connect(self, kg, json_dict):
         # Ensure there is an requested_by relation
         if "user" in json_dict:
             user=kg.get_user_by_name(json_dict["user"])
             if user is None:
@@ -463,14 +514,21 @@
     '''
     Recommendation nodes represent the assertion that a Content node (pointed to by Recommends edge)
     is believed to be relevant to a Request node (pointed to by the RelatesTo edge). The score
     property (float 0.0 - 1.0) indicates how relevant and thus how strong the recommendation.
     '''
     recommends = nm.RelationshipTo(Content, 'RECOMMENDS', model=Recommends, cardinality=One)
     relates_to = nm.RelationshipTo(Request, 'RELATES_TO', model=RelatesTo, cardinality=One)
+
+    def get_recommends(self) -> Content:
+        return self.recommends.single()
+    
+    def get_relates_to(self) -> Request:
+        return self.relates_to.single()
+
     def to_text(self) -> str:
         return "The {content_type} '{content_title}' has {score} relevance to the request '{request}'.".format(
             content_title=self.recommends.single().text,
             content_type= self.recommends.single().type,
             request= self.relates_to.single().title,
             score=self.score_to_text())
 
@@ -496,14 +554,19 @@
     of the Content node connect with the "summaries" edge. The "focus_on" edge connects to the
     Recommendation that may inform how this summary is tailored.
     '''
     text = nm.StringProperty(required=True)
     summarizes = nm.RelationshipTo(Content, 'SUMMARIZES', model=Summarizes, cardinality=One)
     focus_on = nm.RelationshipTo(Recommendation, 'FOCUS_ON', model=FocusOn, cardinality=ZeroOrOne)
 
+    def get_summarizes(self) -> Content:
+        return self.summarizes.single()
+    
+    def get_focus_on(self) -> Recommendation:
+        return self.focus_on.single()
 
 
 # Workflow Products | TLDR
 
 
 class Includes(nm.StructuredRel, OpenTldrMeta, OpenTldrEdge):
     '''
@@ -530,14 +593,20 @@
     to the original Content (from both the Recommendation and Summary).
     '''
     link = nm.StringProperty(required=False)
 
     includes = nm.RelationshipTo(Summary, 'INCLUDES', model=Includes, cardinality=One)
     based_on = nm.RelationshipTo(Recommendation, 'BASED_ON', model=BasedOn, cardinality=One)
 
+    def get_includes(self) -> Summary:
+        return self.includes.single()
+    
+    def get_based_on(self) -> Recommendation:
+        return self.based_on.single()
+
     def to_text(self) -> str:
         return "The entry '{entry}' summarizes {content_type} '{content_title}' and {score} relevance to the request '{request}'.".format(
             entry=self.includes.single().summarizes.single().title,
             content_title=self.includes.single().summarizes.single().title,
             content_type= self.includes.single().summarizes.single().type,
             request= self.based_on.single().relates_to.single().title,
             score=self.based_on.single().score_to_text())
@@ -566,14 +635,20 @@
     by "Entries" edges.
     '''
     date = nm.DateProperty(required=True)
 
     contains = nm.RelationshipTo(TldrEntry, 'CONTAINS', model=Contains, cardinality=ZeroOrMore)
     response_to = nm.RelationshipTo(Request, 'RESPONSE_TO', model=ResponseTo, cardinality=One)
 
+    def get_contains(self) -> list[TldrEntry]:
+        return self.contains
+
+    def get_response_to(self) -> Request:
+        return self.response_to.single()
+
     def to_text(self) -> str:
         out:str = "The TLDR for request '{request}' on date {date} includes: ".format(
             request= self.response_to.single().title,
             date=self.date)
         for tldr_entry in self.includes:
             out += "\t{text}\n".format(text=tldr_entry.to_text())
         return out
@@ -642,14 +717,16 @@
     Request (i.e., what the user is interested in). This represents a "correct" tailoring pair.
     This also includes a score and text to help identify what was most relevant in the pair.
     '''
     text = nm.StringProperty(required=True)
     key_for_content = nm.RelationshipTo(Content, 'KEY_FOR_CONTENT', model=KeyForContent, cardinality=One)
     key_for_request = nm.RelationshipTo(Request, 'KEY_FOR_REQUEST', model=KeyForRequest, cardinality=One)
     
+    
+
     def to_json_connect(self, kg, json_dict) -> dict:
         out:dict= {}
         if "request" not in json_dict:
             out["request"]=self.key_for_request.single().title
         if "content" not in json_dict:
             out["content"]=self.key_for_content.single().title
         return out
```

### Comparing `opentldr-0.4.1/src/opentldr/KnowledgeGraph.py` & `opentldr-0.4.2/src/opentldr/KnowledgeGraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,37 +118,42 @@
         
         return nm.db.cypher_query(cypher_query, resolve_objects = True)
 
     def connect(self, driver=None):
         '''
         ensures that a connection to Neo4j has been established and is functioning.
         '''
-        if driver==None:
-            driver = GraphDatabase.driver(self.connection, auth=(self.user,self.password))
-        
-        log.info("Testing Neo4j Connectivity...")
-        driver.verify_connectivity()
-        
-        if driver.verify_connectivity:
-            log.info("Successfully connected to Neo4J server for KnowledgeGraph.")
-        else:
-            log.error("Unable to connect to Neo4J for KnowledgeGraph. Check that Neo4j server is running.")
-            return False
-
-        log.info("Testing Neo4j Authentication...")
-        driver.verify_authentication()
-        
-        if driver.verify_authentication:
-            log.info("Successfully logged into Neo4J server for KnowledgeGraph.")
-        else:
-            log.error("Unable to log in to Neo4J for KnowledgeGraph. Check that your user and password are correct.")
-            return False
-        
-        self.driver=driver
-        return True
+        try:
+            if driver==None:
+                driver = GraphDatabase.driver(self.connection, auth=(self.user,self.password))
+            
+            log.info("Testing Neo4j Connectivity...")
+            driver.verify_connectivity()
+            
+            if driver.verify_connectivity:
+                log.info("Successfully connected to Neo4J server for KnowledgeGraph.")
+            else:
+                log.error("Unable to connect to Neo4J for KnowledgeGraph. Check that Neo4j server is running.")
+                return False
+
+            log.info("Testing Neo4j Authentication...")
+            driver.verify_authentication()
+            
+            if driver.verify_authentication:
+                log.info("Successfully logged into Neo4J server for KnowledgeGraph.")
+            else:
+                log.error("Unable to log in to Neo4J for KnowledgeGraph. Check that your user and password are correct.")
+                return False
+            
+            self.driver=driver
+            return True
+        except Exception as e:
+            log.error(e)
+            log.error("There was an issue connecting to Neo4J server, please verify that it is running and configured correctly.")            
+            raise e
     
     def getNeo4jDriver(self):
         '''
         returns the Neo4j driver class being used (usually neo4j.GraphDatabase.driver) so that direct neo4j calls can be
         made or it can be passed into other libraries.
         '''
         if self.driver==None:
@@ -170,15 +175,14 @@
         So, we can use this to determine if an object has been saved or not and respond appropriately.
         '''
         if node.uid is None:
             log.warn("Nodes must be persisted with node.save() before being connected. Forcing this now.")
             return node.save()
         return node
 
-
     def get_all_node_uids_by_tag(self, tag:str ) -> list[str]:
         '''
         returns the list of uids for the tag specified as a string.
         '''
         return self.cypher_query("MATCH (n:{tag}) RETURN n.uid".format(tag=tag))
 
     def get_all_nodes_by_tag(self, tag:str ):
@@ -205,16 +209,16 @@
         results, meta = nm.db.cypher_query(cypher_query, resolve_objects = True)
         
         index=0
         if extract_variable is not None:
             index=meta.index(extract_variable)
         else:
             if len(meta)>1:
-                log.warn("cypher_query is defaulting to return the first element of multiple return values in results.")       
-        
+                log.warn("cypher_query is defaulting to return the first element of multiple return values in results.")      
+
         return [item[index] for item in results]
 
     def cypher_query_one(self,cypher_query,extract_variable=None):
         '''
         performs a query that is intended to LIMIT the return values to one single Neomodel object. This simplifies the processing
         of the query results to consistently only get a single object for the extract_variable, it is undefined which unless you sort them.
         For example: cypher_query_one("MATCH (a)-[b]->(c) RETURN a,b,c","a") returns the FIRST object of result "a".
@@ -497,14 +501,18 @@
     def get_user_by_uid(self,uid:str) -> User:
         user = User.nodes.get_or_none(uid=uid)
         return user
 
     def get_user_by_name(self,name:str) -> User:
         user = User.nodes.get_or_none(name=name)
         return user
+    
+    def get_all_users(self) -> list[User]:
+        users = User.nodes
+        return users
 
 
 # Requests
     
     def add_request(self, title:str, text:str, user:User) -> Request:
         request = Request.nodes.get_or_none(title=title)
         if request is None or request.requested_by.single().uid != user.uid:
@@ -521,22 +529,25 @@
     def get_request(self, name:str) -> Request:
         request = Request.nodes.get_or_none(name=name)
         return request
     
     def get_all_requests(self) -> list[Request]:
         requests = Request.nodes
         return requests
- 
-    def get_requests_by_user(self,user:User) -> list[Request]:
-       return self.cypher_query("""
+    
+    def get_requests_by_user_uid(self,uid:str) -> list[Request]: 
+        return self.cypher_query("""
             MATCH (u:User) WHERE u.uid='{user_id}'
             MATCH (q:Request)
             MATCH (q)-[y:REQUESTED_BY]->(u)
             RETURN q """.format(
-                user_id=user.uid),"q")
+                user_id=uid),"q")
+    
+    def get_requests_by_user(self,user:User) -> list[Request]:
+       return self.get_requests_by_user_uid(user.uid)
     
     def get_request_by_title(self,title:str) -> Request:
        return self.cypher_query_one("""
             MATCH (q:Request) WHERE q.title='{title}'
             RETURN q """.format(title=title),"q")
 
     def get_entities_by_request(self,request:Request) -> list[Entity]:
@@ -660,17 +671,21 @@
     
     def add_entry_to_tldr(self, tldr:Tldr, score:float, recommendation:Recommendation, summary:Summary, content:Content) -> TldrEntry:
         tldr_entry=TldrEntry(link=content.url).save()
         tldr_entry.includes.connect(summary)
         tldr_entry.based_on.connect(recommendation)
         tldr.contains.connect(tldr_entry, {'score': score })
 
-    def get_tldr_by_id(self, uid:str) -> Tldr:
+    def get_tldr_by_uid(self, uid:str) -> Tldr:
         tldr = Tldr.nodes.get_or_none(uid=uid)
         return tldr
+    
+    def get_tldr_entry_by_uid(self, uid:str) -> Tldr:
+        tldr_entry = TldrEntry.nodes.get_or_none(uid=uid)
+        return tldr_entry
 
     def delete_tldr_entry(self, tldr_entry:TldrEntry):
         tldr_entry.delete()
 
     def delete_tldr(self, tldr:Tldr):
         for tldr_entry in tldr.contains.all():
             self.delete_tldr_entry(tldr_entry)
@@ -706,28 +721,34 @@
         return self.cypher_query("""
             MATCH (t:Tldr) WHERE t.uid='{tldr_id}'
             MATCH (e:TldrEntry)
             MATCH (t)-[x:CONTAINS]->(e)
             RETURN e ORDER BY e.score DESC""".format(tldr_id=tldr.uid),"e")                 
 
     def get_tldr_by_request(self,request:Request) -> list[Tldr]:
+        return self.get_tldr_by_request_uid(request.uid)
+    
+    def get_tldr_by_request_uid(self,request_uid:str) -> list[Tldr]:
         return self.cypher_query("""
-            MATCH (q:Request) WHERE q.uid='{request_id}'
+            MATCH (q:Request) WHERE q.uid='{request_uid}'
             MATCH (t:Tldr)
             MATCH (t)-[y:RESPONSE_TO]->(q)
             RETURN t """.format(
-                request_id=request.uid),"t")
-    
-    def get_tldr(self,request:Request, date:datetime.date) -> Tldr:
+                request_uid=request_uid),"t")
+
+    def get_tldr_by_uid_and_date(self,request_uid:str, date:datetime.date) -> Tldr:
         return self.cypher_query_one("""
-            MATCH (q:Request) WHERE q.uid='{request_id}'
+            MATCH (q:Request) WHERE q.uid='{request_uid}'
             MATCH (t:Tldr) where t.date='{date}'
             MATCH (t)-[y:RESPONSE_TO]->(q)
             RETURN t """.format( date=date,
-                request_id=request.uid),"t")
+                request_uid=request_uid),"t")
+    
+    def get_tldr(self,request:Request, date:datetime.date) -> Tldr:
+        return self.get_tldr_by_uid_and_date(request.uid, date)
 
 
 ## EvalKey Nodes - rubric for evaluation metrics
 
     def add_evalkey(self, content:Content, request:Request, score:float, text:str) -> EvalKey:
         key = EvalKey(text=text, score=score).save()
         key.key_for_content.connect(content)
```

### Comparing `opentldr-0.4.1/src/opentldr/S3DataRepo.py` & `opentldr-0.4.2/src/opentldr/S3DataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.4.1/src/opentldr/TextFileDataRepo.py` & `opentldr-0.4.2/src/opentldr/FileSystemDataRepo.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .KnowledgeGraph import KnowledgeGraph
 from .log import log
 
 import os
 import json
 
 
-class TextFileDataRepo(AbstractDataRepo):
+class FileSystemDataRepo(AbstractDataRepo):
     '''
     Reads all the text files in the provided directory path. Creates a Source node for the directory and parses the text files.
     This extracts lines with property definitions (e.g., "date: 05/14/1960 08:00PM") and puts the rest into the text body.
     Creates a Content node, for each file and adds it to the knowledge graph.
     '''
     ingest_path:str = "."
     files:list[str] = []
```

### Comparing `opentldr-0.4.1/src/opentldr/Workflow.py` & `opentldr-0.4.2/src/opentldr/Workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,21 +118,26 @@
             os.makedirs(path)
             log.info("Created output directory: "+path)
 
     def execute_notebook(self, notebook:str, variables:dict, output_path:str) -> float:
         '''
         execute_notebook runs a single notebook file in PaperMill returns the run time in seconds
         '''
-        out_notebook:str = os.path.join(output_path,notebook.replace('/',"_"))
-        log.debug("Now executing notebook '{notebook}' with params '{params}' and output '{output}'.".format(notebook=notebook,params=variables,output=output_path))
+        try:
+            out_notebook:str = os.path.join(output_path,notebook.replace('/',"_"))
+            log.debug("Now executing notebook '{notebook}' with params '{params}' and output '{output}'.".format(notebook=notebook,params=variables,output=output_path))
 
-        step_start=perf_counter()
-        pm.execute_notebook(notebook, out_notebook, variables)
-        step_end=perf_counter()
-        return (step_end-step_start)
+            step_start=perf_counter()
+            pm.execute_notebook(notebook, out_notebook, variables)
+            step_end=perf_counter()
+            return (step_end-step_start)
+        
+        except Exception as e:
+            log.error("There was an error executing the notebook ({nb}), please verify the parameters and that the notebook runs successfully on its own.".format(nb=notebook))
+            raise e
 
     def run(self):
         '''
         run the defined workflow files in order in PaperMill
         '''
         output_path=self.workflow["Output"]
         self.ensure_path(output_path)
```

### Comparing `opentldr-0.4.1/src/opentldr.egg-info/PKG-INFO` & `opentldr-0.4.2/src/opentldr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentldr
-Version: 0.4.1
+Version: 0.4.2
 Summary: An open framework for creation of a Tailored Daily Report.
 Author-email: Chris Argenta <cargenta@rockfishresearch.com>
 Project-URL: Source, https://github.com/RockfishResearch/OpenTLDR-Core.git
 Project-URL: Issues, https://github.com/RockfishResearch/OpenTLDR-Core/issues
 Project-URL: Documentation, http://www.opentldr.org/docs
 Project-URL: Homepage, http://www.opentldr.org
 Classifier: Programming Language :: Python :: 3
@@ -17,16 +17,17 @@
 License-File: LICENSE
 Requires-Dist: python-dotenv>=1.0.0
 Requires-Dist: neo4j>=5.15.0
 Requires-Dist: neomodel>=5.2.1
 Requires-Dist: papermill>=2.5.0
 Requires-Dist: boto3>=1.34.55
 
-# OpenTLDR
+# OpenTLDR-Core
 An Open Framework for Generating an Tailored Daily Report
+This repository contains the OpenTLDR package. You can 'pip install opentldr' to get the contents of this repository as a python package in your virtaul env.
 
 ![overview image](resources/opentldr.png)
 
 ## Introduction to OpenTLDR
 
 OpenTLDR is an open source framework written in Python to implement the process of creating a Tailored Daily Report from a series of news-like articles. This repository contains the Core classes used as a library by OpenTLDR implementations, like the example notebooks you canf ind in the OpenTLDR-Example repo on GitHub.
```

### Comparing `opentldr-0.4.1/src/opentldr.egg-info/SOURCES.txt` & `opentldr-0.4.2/src/opentldr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 MANIFEST.in
 README.md
 pyproject.toml
 src/opentldr/AbstractDataRepo.py
 src/opentldr/DataRepo.py
 src/opentldr/DataRepoJson.py
 src/opentldr/Domain.py
+src/opentldr/FileSystemDataRepo.py
 src/opentldr/KnowledgeGraph.py
 src/opentldr/S3DataRepo.py
-src/opentldr/TextFileDataRepo.py
 src/opentldr/Workflow.py
 src/opentldr/__init__.py
 src/opentldr/log.py
 src/opentldr.egg-info/PKG-INFO
 src/opentldr.egg-info/SOURCES.txt
 src/opentldr.egg-info/dependency_links.txt
 src/opentldr.egg-info/requires.txt
```

### Comparing `opentldr-0.4.1/tests/test_knowledgegraph.py` & `opentldr-0.4.2/tests/test_knowledgegraph.py`

 * *Files identical despite different names*

