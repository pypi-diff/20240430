# Comparing `tmp/langchain_google_alloydb_pg-0.2.0-py3-none-any.whl.zip` & `tmp/langchain_google_alloydb_pg-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 29228 bytes, number of entries: 13
--rw-r--r--  2.0 unx     1019 b- defN 24-Mar-27 17:38 langchain_google_alloydb_pg/__init__.py
--rw-r--r--  2.0 unx     4945 b- defN 24-Mar-27 17:38 langchain_google_alloydb_pg/alloydb_chat_message_history.py
--rw-r--r--  2.0 unx    14071 b- defN 24-Mar-27 17:38 langchain_google_alloydb_pg/alloydb_engine.py
--rw-r--r--  2.0 unx    16820 b- defN 24-Mar-27 17:38 langchain_google_alloydb_pg/alloydb_loader.py
--rw-r--r--  2.0 unx    29599 b- defN 24-Mar-27 17:38 langchain_google_alloydb_pg/alloydb_vectorstore.py
--rw-r--r--  2.0 unx     2580 b- defN 24-Mar-27 17:38 langchain_google_alloydb_pg/indexes.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Mar-27 17:38 langchain_google_alloydb_pg/py.typed
--rw-r--r--  2.0 unx      597 b- defN 24-Mar-27 17:38 langchain_google_alloydb_pg/version.py
--rw-rw-r--  2.0 unx    11358 b- defN 24-Mar-27 17:40 langchain_google_alloydb_pg-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    18760 b- defN 24-Mar-27 17:40 langchain_google_alloydb_pg-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-27 17:40 langchain_google_alloydb_pg-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-27 17:40 langchain_google_alloydb_pg-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1293 b- defN 24-Mar-27 17:40 langchain_google_alloydb_pg-0.2.0.dist-info/RECORD
-13 files, 101162 bytes uncompressed, 27000 bytes compressed:  73.3%
+Zip file size: 29371 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     1019 b- defN 24-Apr-30 20:14 langchain_google_alloydb_pg/__init__.py
+-rw-r--r--  2.0 unx     4945 b- defN 24-Apr-30 20:14 langchain_google_alloydb_pg/alloydb_chat_message_history.py
+-rw-r--r--  2.0 unx    13800 b- defN 24-Apr-30 20:14 langchain_google_alloydb_pg/alloydb_engine.py
+-rw-r--r--  2.0 unx    16820 b- defN 24-Apr-30 20:14 langchain_google_alloydb_pg/alloydb_loader.py
+-rw-r--r--  2.0 unx    29532 b- defN 24-Apr-30 20:14 langchain_google_alloydb_pg/alloydb_vectorstore.py
+-rw-r--r--  2.0 unx     2580 b- defN 24-Apr-30 20:14 langchain_google_alloydb_pg/indexes.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-30 20:14 langchain_google_alloydb_pg/py.typed
+-rw-r--r--  2.0 unx      597 b- defN 24-Apr-30 20:14 langchain_google_alloydb_pg/version.py
+-rw-rw-r--  2.0 unx    11358 b- defN 24-Apr-30 20:16 langchain_google_alloydb_pg-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    20244 b- defN 24-Apr-30 20:16 langchain_google_alloydb_pg-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-30 20:16 langchain_google_alloydb_pg-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-30 20:16 langchain_google_alloydb_pg-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1293 b- defN 24-Apr-30 20:16 langchain_google_alloydb_pg-0.2.1.dist-info/RECORD
+13 files, 102308 bytes uncompressed, 27143 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: langchain_google_alloydb_pg/py.typed
 Comment: 
 
 Filename: langchain_google_alloydb_pg/version.py
 Comment: 
 
-Filename: langchain_google_alloydb_pg-0.2.0.dist-info/LICENSE
+Filename: langchain_google_alloydb_pg-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: langchain_google_alloydb_pg-0.2.0.dist-info/METADATA
+Filename: langchain_google_alloydb_pg-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: langchain_google_alloydb_pg-0.2.0.dist-info/WHEEL
+Filename: langchain_google_alloydb_pg-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: langchain_google_alloydb_pg-0.2.0.dist-info/top_level.txt
+Filename: langchain_google_alloydb_pg-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: langchain_google_alloydb_pg-0.2.0.dist-info/RECORD
+Filename: langchain_google_alloydb_pg-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langchain_google_alloydb_pg/alloydb_engine.py

```diff
@@ -56,15 +56,15 @@
             principal.
     """
     # refresh credentials if they are not valid
     if not credentials.valid:
         request = google.auth.transport.requests.Request()
         credentials.refresh(request)
     if hasattr(credentials, "_service_account_email"):
-        email = credentials._service_account_email
+        return credentials._service_account_email.replace(".gserviceaccount.com", "")
     # call OAuth2 api to get IAM principal email associated with OAuth2 token
     url = f"https://oauth2.googleapis.com/tokeninfo?access_token={credentials.token}"
     async with aiohttp.ClientSession() as client:
         response = await client.get(url, raise_for_status=True)
         response_json: Dict = await response.json()
         email = response_json.get("email")
     if email is None:
@@ -155,22 +155,14 @@
                 "both should be specified to use basic user/password "
                 "authentication or neither for IAM DB authentication."
             )
 
         if cls._connector is None:
             cls._connector = AsyncConnector(user_agent=USER_AGENT)
 
-        if isinstance(ip_type, str):
-            if ip_type.lower() == "public":
-                ip_type = IPTypes.PUBLIC
-            elif ip_type.lower() == "private":
-                ip_type = IPTypes.PRIVATE
-            else:
-                raise ValueError("ip_type is not one of: public, private.")
-
         # if user and password are given, use basic auth
         if user and password:
             enable_iam_auth = False
             db_user = user
         # otherwise use automatic IAM database authentication
         else:
             # get application default credentials
```

## langchain_google_alloydb_pg/alloydb_vectorstore.py

```diff
@@ -91,24 +91,22 @@
         k: int = 4,
         fetch_k: int = 20,
         lambda_mult: float = 0.5,
         index_query_options: Optional[QueryOptions] = None,
     ):
         """Constructor for AlloyDBVectorStore.
         Args:
-            engine (AlloyDBEngine): AsyncEngine with pool connection to the postgres database. Required.
+            engine (AlloyDBEngine): Connection pool engine for managing connections to AlloyDB database.
             embedding_service (Embeddings): Text embedding model to use.
             table_name (str): Name of the existing table or the table to be created.
-            id_column (str): Column that represents the Document's id. Defaults to "langchain_id".
             content_column (str): Column that represent a Document’s page_content. Defaults to "content".
-            embedding_column (str): Column for embedding vectors.
-                              The embedding is generated from the document value. Defaults to "embedding".
+            embedding_column (str): Column for embedding vectors. The embedding is generated from the document value. Defaults to "embedding".
             metadata_columns (List[str]): Column(s) that represent a document's metadata.
-            ignore_metadata_columns (List[str]): Column(s) to ignore in pre-existing tables for a document’s metadata.
-                                     Can not be used with metadata_columns. Defaults to None.
+            ignore_metadata_columns (List[str]): Column(s) to ignore in pre-existing tables for a document's metadata. Can not be used with metadata_columns. Defaults to None.
+            id_column (str): Column that represents the Document's id. Defaults to "langchain_id".
             metadata_json_column (str): Column to store metadata as JSON. Defaults to "langchain_metadata".
         """
         if metadata_columns and ignore_metadata_columns:
             raise ValueError(
                 "Can not use both metadata_columns and ignore_metadata_columns."
             )
         # Get field type information
@@ -308,15 +306,15 @@
         ids: Optional[List[str]] = None,
         **kwargs: Any,
     ) -> Optional[bool]:
         if not ids:
             return False
 
         id_list = ", ".join([f"'{id}'" for id in ids])
-        query = f"DELETE FROM {self.table_name} WHERE {self.id_column} in ({id_list})"
+        query = f'DELETE FROM "{self.table_name}" WHERE {self.id_column} in ({id_list})'
         await self.engine._aexecute(query)
         return True
 
     def delete(
         self,
         ids: Optional[List[str]] = None,
         **kwargs: Any,
```

## langchain_google_alloydb_pg/version.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
```

## Comparing `langchain_google_alloydb_pg-0.2.0.dist-info/LICENSE` & `langchain_google_alloydb_pg-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langchain_google_alloydb_pg-0.2.0.dist-info/RECORD` & `langchain_google_alloydb_pg-0.2.1.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 langchain_google_alloydb_pg/__init__.py,sha256=o-3xTGhj34XtT1B4mNEVaXq5ANdeFLpMvcafTm8-B_c,1019
 langchain_google_alloydb_pg/alloydb_chat_message_history.py,sha256=Uxz6VuQPxqxQp200QEa2epXKVfWEaqhp2MBHxxx8Q6o,4945
-langchain_google_alloydb_pg/alloydb_engine.py,sha256=JRbt9e4MsdcCFWQHCaL3Pc4GMcrwFFO8dbC9pk1wQDs,14071
+langchain_google_alloydb_pg/alloydb_engine.py,sha256=YEhS_X0EmKlozeCXEviPEaGYA4YuHOO04HsqVt7IkEM,13800
 langchain_google_alloydb_pg/alloydb_loader.py,sha256=WC3y-APUG1X2I6xxL7lg1d9ar6RJ7xyDl1ZSNIUVxOI,16820
-langchain_google_alloydb_pg/alloydb_vectorstore.py,sha256=ZzMCrg8DbxmKarF4JwQDZlppv4B82OAHaqw5DtQPWtI,29599
+langchain_google_alloydb_pg/alloydb_vectorstore.py,sha256=5ZVH8diMOOO7YHoJCn7s9wZcXfAHl05QADrCR22J4O0,29532
 langchain_google_alloydb_pg/indexes.py,sha256=UYbXMcZXBvaU7FFa7IjhXvBvCuDdxr0Tq2pgyQrKVtU,2580
 langchain_google_alloydb_pg/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-langchain_google_alloydb_pg/version.py,sha256=c32tFkU7bcWMAeqBrDdHTYBzbZPaJPvhWqbKnyY_LxM,597
-langchain_google_alloydb_pg-0.2.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-langchain_google_alloydb_pg-0.2.0.dist-info/METADATA,sha256=XwweB30nSxks86koosV9wx0nEe6geqmzAJNOXCyMyW0,18760
-langchain_google_alloydb_pg-0.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-langchain_google_alloydb_pg-0.2.0.dist-info/top_level.txt,sha256=oHZAsNgaSCO84iduMcOJROVrOYrW7BeE-c8kvmydZyo,28
-langchain_google_alloydb_pg-0.2.0.dist-info/RECORD,,
+langchain_google_alloydb_pg/version.py,sha256=lal6j0-2qdxqYCLjy1FcTVeiboHQADADWfCBuVKcU3k,597
+langchain_google_alloydb_pg-0.2.1.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+langchain_google_alloydb_pg-0.2.1.dist-info/METADATA,sha256=Rfk_CxChH2WwWMVgL-3u6-5ssUZOLchEpalPNf3QdoA,20244
+langchain_google_alloydb_pg-0.2.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+langchain_google_alloydb_pg-0.2.1.dist-info/top_level.txt,sha256=oHZAsNgaSCO84iduMcOJROVrOYrW7BeE-c8kvmydZyo,28
+langchain_google_alloydb_pg-0.2.1.dist-info/RECORD,,
```

