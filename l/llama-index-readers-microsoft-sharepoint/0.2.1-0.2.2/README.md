# Comparing `tmp/llama_index_readers_microsoft_sharepoint-0.2.1.tar.gz` & `tmp/llama_index_readers_microsoft_sharepoint-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_microsoft_sharepoint-0.2.1.tar", max compression
+gzip compressed data, was "llama_index_readers_microsoft_sharepoint-0.2.2.tar", max compression
```

## Comparing `llama_index_readers_microsoft_sharepoint-0.2.1.tar` & `llama_index_readers_microsoft_sharepoint-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1782 2024-04-24 20:25:49.929346 llama_index_readers_microsoft_sharepoint-0.2.1/README.md
--rw-r--r--   0        0        0      107 2024-04-24 20:25:49.929346 llama_index_readers_microsoft_sharepoint-0.2.1/llama_index/readers/microsoft_sharepoint/__init__.py
--rw-r--r--   0        0        0    18842 2024-04-24 20:25:49.929346 llama_index_readers_microsoft_sharepoint-0.2.1/llama_index/readers/microsoft_sharepoint/base.py
--rw-r--r--   0        0        0    41139 2024-04-24 20:25:49.929346 llama_index_readers_microsoft_sharepoint-0.2.1/llama_index/readers/microsoft_sharepoint/file_path_info.png
--rw-r--r--   0        0        0     1594 2024-04-24 20:25:49.929346 llama_index_readers_microsoft_sharepoint-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 llama_index_readers_microsoft_sharepoint-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1782 2024-04-30 21:14:32.067069 llama_index_readers_microsoft_sharepoint-0.2.2/README.md
+-rw-r--r--   0        0        0      107 2024-04-30 21:14:32.067069 llama_index_readers_microsoft_sharepoint-0.2.2/llama_index/readers/microsoft_sharepoint/__init__.py
+-rw-r--r--   0        0        0    19700 2024-04-30 21:14:32.071069 llama_index_readers_microsoft_sharepoint-0.2.2/llama_index/readers/microsoft_sharepoint/base.py
+-rw-r--r--   0        0        0    41139 2024-04-30 21:14:32.071069 llama_index_readers_microsoft_sharepoint-0.2.2/llama_index/readers/microsoft_sharepoint/file_path_info.png
+-rw-r--r--   0        0        0     1594 2024-04-30 21:14:32.071069 llama_index_readers_microsoft_sharepoint-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 llama_index_readers_microsoft_sharepoint-0.2.2/PKG-INFO
```

### Comparing `llama_index_readers_microsoft_sharepoint-0.2.1/README.md` & `llama_index_readers_microsoft_sharepoint-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_microsoft_sharepoint-0.2.1/llama_index/readers/microsoft_sharepoint/base.py` & `llama_index_readers_microsoft_sharepoint-0.2.2/llama_index/readers/microsoft_sharepoint/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -417,14 +417,36 @@
         return self._download_files_and_extract_metadata(
             sharepoint_folder_id,
             download_dir,
             os.path.join(sharepoint_site_name, sharepoint_folder_path),
             recursive,
         )
 
+    def _exclude_access_control_metadata(
+        self, documents: List[Document]
+    ) -> List[Document]:
+        """
+        Excludes the access control metadata from the documents for embedding and LLM calls.
+
+        Args:
+            documents (List[Document]): A list of documents.
+
+        Returns:
+            List[Document]: A list of documents with access control metadata excluded.
+        """
+        for doc in documents:
+            access_control_keys = [
+                key for key in doc.metadata if key.startswith("allowed_")
+            ]
+
+            doc.excluded_embed_metadata_keys.extend(access_control_keys)
+            doc.excluded_llm_metadata_keys.extend(access_control_keys)
+
+        return documents
+
     def _load_documents_with_metadata(
         self,
         files_metadata: Dict[str, Any],
         download_dir: str,
         recursive: bool,
     ) -> List[Document]:
         """
@@ -444,15 +466,18 @@
 
         simple_loader = SimpleDirectoryReader(
             download_dir,
             file_extractor=self.file_extractor,
             file_metadata=get_metadata,
             recursive=recursive,
         )
-        return simple_loader.load_data()
+        docs = simple_loader.load_data()
+        if self.attach_permission_metadata:
+            docs = self._exclude_access_control_metadata(docs)
+        return docs
 
     def load_data(
         self,
         sharepoint_site_name: Optional[str] = None,
         sharepoint_folder_path: Optional[str] = None,
         sharepoint_folder_id: Optional[str] = None,
         recursive: bool = True,
```

### Comparing `llama_index_readers_microsoft_sharepoint-0.2.1/llama_index/readers/microsoft_sharepoint/file_path_info.png` & `llama_index_readers_microsoft_sharepoint-0.2.2/llama_index/readers/microsoft_sharepoint/file_path_info.png`

 * *Files identical despite different names*

### Comparing `llama_index_readers_microsoft_sharepoint-0.2.1/pyproject.toml` & `llama_index_readers_microsoft_sharepoint-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 description = "llama-index readers microsoft_sharepoint integration"
 exclude = ["**/BUILD"]
 keywords = ["microsoft 365", "microsoft365", "sharepoint"]
 license = "MIT"
 maintainers = ["arun-soliton"]
 name = "llama-index-readers-microsoft-sharepoint"
 readme = "README.md"
-version = "0.2.1"
+version = "0.2.2"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_readers_microsoft_sharepoint-0.2.1/PKG-INFO` & `llama_index_readers_microsoft_sharepoint-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-microsoft-sharepoint
-Version: 0.2.1
+Version: 0.2.2
 Summary: llama-index readers microsoft_sharepoint integration
 License: MIT
 Keywords: microsoft 365,microsoft365,sharepoint
 Author: Your Name
 Author-email: you@example.com
 Maintainer: arun-soliton
 Requires-Python: >=3.8.1,<4.0
```

