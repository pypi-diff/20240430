# Comparing `tmp/docindex-0.5.0.tar.gz` & `tmp/docindex-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docindex-0.5.0.tar", last modified: Mon Apr 22 09:50:16 2024, max compression
+gzip compressed data, was "docindex-0.6.0.tar", last modified: Tue Apr 30 17:14:37 2024, max compression
```

## Comparing `docindex-0.5.0.tar` & `docindex-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:50:16.402399 docindex-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-22 09:50:12.000000 docindex-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-04-22 09:50:16.402399 docindex-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-22 09:50:12.000000 docindex-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-22 09:50:12.000000 docindex-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-22 09:50:16.402399 docindex-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:50:16.398399 docindex-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:50:16.398399 docindex-0.5.0/src/_google/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:50:12.000000 docindex-0.5.0/src/_google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-22 09:50:12.000000 docindex-0.5.0/src/_google/create_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-22 09:50:12.000000 docindex-0.5.0/src/_google/delete_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-22 09:50:12.000000 docindex-0.5.0/src/_google/doc_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-04-22 09:50:12.000000 docindex-0.5.0/src/_google/docindex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:50:16.398399 docindex-0.5.0/src/_openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:50:12.000000 docindex-0.5.0/src/_openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-22 09:50:12.000000 docindex-0.5.0/src/_openai/create_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-22 09:50:12.000000 docindex-0.5.0/src/_openai/delete_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-22 09:50:12.000000 docindex-0.5.0/src/_openai/doc_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-22 09:50:12.000000 docindex-0.5.0/src/_openai/doc_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-22 09:50:12.000000 docindex-0.5.0/src/_openai/docindex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:50:16.402399 docindex-0.5.0/src/docindex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-04-22 09:50:16.000000 docindex-0.5.0/src/docindex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-22 09:50:16.000000 docindex-0.5.0/src/docindex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:50:16.000000 docindex-0.5.0/src/docindex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-22 09:50:16.000000 docindex-0.5.0/src/docindex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 09:50:16.000000 docindex-0.5.0/src/docindex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:50:16.402399 docindex-0.5.0/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:50:12.000000 docindex-0.5.0/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-22 09:50:12.000000 docindex-0.5.0/src/tests/googleindex_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-22 09:50:12.000000 docindex-0.5.0/src/tests/openaiindex_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:37.072249 docindex-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-30 17:14:33.000000 docindex-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-30 17:14:37.072249 docindex-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-04-30 17:14:33.000000 docindex-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-30 17:14:33.000000 docindex-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-30 17:14:37.072249 docindex-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:37.068249 docindex-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:37.068249 docindex-0.6.0/src/_cohere/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_cohere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_cohere/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_cohere/create_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_cohere/delete_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_cohere/doc_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_cohere/doc_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_cohere/index_documents.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:37.068249 docindex-0.6.0/src/_google/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_google/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_google/create_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_google/delete_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_google/doc_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_google/index_documents.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:37.072249 docindex-0.6.0/src/_openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_openai/create_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_openai/delete_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_openai/doc_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_openai/doc_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_openai/index_documents.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:37.072249 docindex-0.6.0/src/docindex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-30 17:14:37.000000 docindex-0.6.0/src/docindex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-30 17:14:37.000000 docindex-0.6.0/src/docindex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 17:14:37.000000 docindex-0.6.0/src/docindex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-30 17:14:37.000000 docindex-0.6.0/src/docindex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 17:14:37.000000 docindex-0.6.0/src/docindex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:37.072249 docindex-0.6.0/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:33.000000 docindex-0.6.0/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-30 17:14:33.000000 docindex-0.6.0/src/tests/cohereindex_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-30 17:14:33.000000 docindex-0.6.0/src/tests/googleindex_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-30 17:14:33.000000 docindex-0.6.0/src/tests/openaiindex_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:37.072249 docindex-0.6.0/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:33.000000 docindex-0.6.0/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-30 17:14:33.000000 docindex-0.6.0/src/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-30 17:14:33.000000 docindex-0.6.0/src/utils/response_model.py
```

### Comparing `docindex-0.5.0/LICENSE` & `docindex-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docindex-0.5.0/PKG-INFO` & `docindex-0.6.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: docindex
-Version: 0.5.0
-Summary: A package for fast indexing of multiple documents and their metadata on Pinecone.
+Version: 0.6.0
+Summary: A package for fast persistent storage of multiple document embeddings and their metadata into Pinecone for production-level RAG.
 Home-page: https://github.com/KevKibe/docindex
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,118 +15,131 @@
 Requires-Dist: unstructured==0.12.6
 Requires-Dist: langchain-community==0.0.31
 Requires-Dist: langchain==0.1.14
 Requires-Dist: langchain-openai==0.1.1
 Requires-Dist: langchain-google-genai==1.0.1
 Requires-Dist: langchain-pinecone==0.1.0
 Requires-Dist: google.generativeai==0.4.1
+Requires-Dist: python-dotenv==1.0.1
+Requires-Dist: python-docx==1.1.0
+Requires-Dist: markdown==3.6
+Requires-Dist: langchain-core==0.1.46
+Requires-Dist: langchain-cohere==0.1.4
 
-<h1 align="center">DocIndex: Fast Persistent Document Embeddings Storage for RAG</h1>
+<h1 align="center">DocIndex: Fast Persistent Document Embeddings Storage for Production-Level RAG</h1>
 <p align="center">
 
   <a href="https://github.com/KevKibe/docindex/commits/">
     <img src="https://img.shields.io/github/last-commit/KevKibe/docindex?" alt="Last commit">
   </a>
   <a href="https://github.com/KevKibe/docindex/blob/master/LICENSE">
     <img src="https://img.shields.io/github/license/KevKibe/docindex?" alt="License">
   </a>
 <br>
 
 ![Diagram](diagram.png)
 
- *Efficiently store multiple document embeddings and their metadata, whether they're offline or online, in a persistent Pinecone Vector Database optimized for Retrieval Augmented Generation (RAG) applications fast*
+ *Efficiently store multiple document embeddings and their metadata, whether they're offline or online, in a persistent Pinecone Vector Database optimized for production-level Retrieval Augmented Generation (RAG) applications fast*
 ## Features
 
 - ⚡️ **Rapid Indexing**: Quickly index multiple documents along with their metadata, including source, page details, and content, into Pinecone DB.<br>
 - 📚 **Document Flexibility**: Index documents from your local storage or online sources with ease.<br>
-- 📂 **Format Support**: Seamlessly handle various document formats, including PDF, docx(in-development), etc.<br>
-- 🔁 **Embedding Services Integration**: Enjoy support for multiple embedding services such as OpenAI Embeddings, Google Generative AI Embeddings and more in development.<br>
+- 📂 **Format Support**: Store various document formats, including PDF, docx(in-development), etc.<br>
+- 🔁 **LLM Providers Integration**: Enjoy support for multiple LLM providers such as OpenAI, Google Generative AI, Cohere and more in development.<br>
 - 🛠️ **Configurable Vectorstore**: Configure a vectorstore directly from the index to facilitate RAG pipelines effortlessly.
-
+- 🔍 **Initialize a RAG Retriever**: Spin up a RAG retriever using your vectorstore.
+  
 ## Setup
 
 ```python
 pip install docindex
 ```
 
 ## Getting Started
 - Sign up to [Pinecone](https://www.pinecone.io/) and get an API key.
-## Using OpenAI 
-[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1f5DzVjM9n9XWFtErTdWkKUFtszXyqzMI#scrollTo=olWrGV2viIsP)
+### Import Dependencies
+```python
+# Import the appropriate indexer class based on the language model you want to use
+from _openai.doc_index import OpenaiPineconeIndexer  # Using OpenAI
+from _google.doc_index import GooglePineconeIndexer  # Using GoogleGenerativeAI
+from _cohere.doc_index import CoherePineconeIndexer  # Using Cohere
+```
+
+### API Keys and Configuration
 ```python
-from _openai.docindex import OpenaiPineconeIndexer
+# Replace these values with your actual API keys and index name or have them in a variable environment/secret key.
+pinecone_api_key = "your_pinecone_api_key"  # Your Pinecone API key
+index_name = "your_index_name"  # Your Pinecone index name
+
+openai_api_key = "your_openai_api_key"     # Using OpenAI)
+# google_api_key = "your_google_api_key"   # Using GoogleGenerativeAI
+#cohere_api_key = "your_cohere_api_key"    # Using Cohere
 
-# Replace these values with your actual Pinecone API key, index name, OpenAI API key
-pinecone_api_key = "pinecone-api-key"
-index_name = "index-name"               # e.g index-1
-openai_api_key = "openai-api-key"
-batch_limit = 20                        # Batch limit for upserting documents
-chunk_size = 256                        # Optional: size of texts per chunk. 
+# Configure batch limit and chunk size
+batch_limit = "batch-limit" # Maximum batch size for upserting documents -> Optional: Default 32
+chunk_size = "chunk-size"  # Size of texts per chunk -> Optional: Default 256
+```
 
+### List of Documents:
+```python
 # List of URLs of the documents to be indexed. (offline on your computer or online)
 urls = [
  "your-document-1.pdf",
  "your-document-2.md",
  "your-document-3.html",
  "your-document-4.docx",
 ]
+```
+### Index, Store Documents and Initialize VectorStore
+```python
+# Initialize the Pinecone indexer with the desired model
+
+pinecone_indexer = OpenaiPineconeIndexer(index_name, pinecone_api_key, openai_api_key)    # Using OpenAI
+# pinecone_indexer = GooglePineconeIndexer(index_name, pinecone_api_key, google_api_key)  # Using GoogleGenerativeAI
+# pinecone_indexer = CoherePineconeIndexer(index_name, pinecone_api_key, cohere_api_key)  # Using Cohere
 
-# Initialize the Pinecone indexer
-pinecone_indexer = OpenaiPineconeIndexer(index_name, pinecone_api_key, openai_api_key)
 
 # To create a new Index
 pinecone_indexer.create_index()
 
 # Store the document embeddings with the specified URLs and batch limit
 pinecone_indexer.index_documents(urls,batch_limit,chunk_size)
 
 # Initialize the Vectorstore
 vectorstore = pinecone_indexer.initialize_vectorstore(index_name)
 ```
+### Query and Retrieve Information
 ```python
-# To delete the created Index
-pinecone_indexer.delete_index()
+query = "what is the transformers architecture"
+response = pinecone_indexer.retrieve_and_generate(vector_store = vectorstore, query = query)
+response
 ```
 
+### Response
+```bash
+query='what is the transformers architecture' result='The Transformer follows this overall architecture using stacked self-attention and point-wise, fully-connected layers for both the encoder and decoder, shown in the left and right halves of Figure 1, respectively.' page=1 source_documents=[Document(page_content='Figure 1: The Transformer - model architecture.\nThe Transformer follows this overall architecture using stacked self-attention and point-wise, fully\nconnected layers for both the encoder and decoder, shown in the left and right halves of Figure 1,\nrespectively.\n3.1 Encoder and Decoder Stacks\nEncoder: The encoder is composed of a stack of N= 6 identical layers. Each layer has two\nsub-layers. The first is a multi-head self-attention mechanism, and the second is a simple, position-\nwise fully connected feed-forward network. We employ a residual connection [ 11] around each of\nthe two sub-layers, followed by layer normalization [ 1]. That is, the output of each sub-layer is\nLayerNorm( x+ Sublayer( x)), where Sublayer( x)is the function implemented by the sub-layer\nitself. To facilitate these residual connections, all sub-layers in the model, as well as the embedding\nlayers, produce outputs of dimension dmodel = 512 .\nDecoder: The decoder is also composed of a stack of N= 6identical layers. In addition to the two', source=2.0, title='https://arxiv.org/pdf/1706.03762.pdf')]
 
-## Using Google Generative AI  
-[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1C4DyIsWMJWUmNuXEmmUMyshqoAKspFlp?usp=sharing)
-```python
-from _google.docindex import GooglePineconeIndexer
-
-# Replace these values with your actual Pinecone API key, index name, Google API key
-pinecone_api_key = "pinecone-api-key"
-index_name = "index-name"                # e.g index-1
-google_api_key = "google-api-key"
-batch_limit = 20                         # Batch limit for upserting documents
-chunk_size = 256                         # Optional: size of texts per chunk. 
-
-# List of URLs of the documents to be indexed. (offline on your computer or an online)
-urls = [
- "your-document-1.pdf",
- "your-document-2.pdf"
-]
-
-pinecone_indexer = GooglePineconeIndexer(index_name, pinecone_api_key, google_api_key)
-
-# To create a new Index
-pinecone_indexer.create_index()
-
-# Store the document embeddings with the specified URLs and batch limit
-pinecone_indexer.index_documents(urls,batch_limit,chunk_size)
+```
 
-# Initialize the Vectorstore
-vectorstore = pinecone_indexer.initialize_vectorstore(index_name)
+### Query Response Attributes:
+```python
+response.query                 # The query that was submitted
+response.result                # The result of the query, including any retrieved information.
+response.source_documents      # A list of source documents related to the query.
+response.sources               # A list of the sources (page numbers) from the source documents.
+response.titles                # A list of the titles from the source documents.
+response.page_contents         # A list of the page contents from the source documents.
 ```
+
+### Delete Index: 
 ```python
 # To delete the created Index
 pinecone_indexer.delete_index()
 ```
 
-
 ## Using the CLI
 
 - Clone the Repository: Clone or download the application code to your local machine.
 ```bash
 git clone https://github.com/KevKibe/docindex.git
 ```
 
@@ -150,38 +163,40 @@
 ```bash
 cd src
 ```
 - To create an index
 
 ```bash
 # Using OpenAI 
-python -m  _openai.create_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key "your_openai_api_key"
+python -m  _openai.create_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" -
 
-# Using Google Generative AI
-python -m  _google.create_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --google_api_key "your_google_api_key"
 ```
 
 - Run the command to start indexing the documents
 
 ```bash
-# Using OpenAI 
-python -m _openai.doc_index  --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key "your_openai_api_key" --batch_limit 10 --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size 256 
-```
-```bash
-# Using Google Generative AI 
-python -m _google.doc_index  --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --google_api_key "your_google_api_key" --batch_limit 10 --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size 256 
+# Using OpenAI
+
+python -m _openai.index_documents  --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key "your_openai_api_key" --batch_limit "batch-limit" --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-size"
+
+# Using Google Generative AI
+
+python -m _google.index_documents  --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --google_api_key "your_google_api_key" --batch_limit "batch-limit" --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-size"
+
+Using Cohere
+
+python -m _cohere.index_documents   --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --cohere_api_key "your_google_api_key" --batch_limit "batch-limit" --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-size"
+
 ```
 - To delete an index
 
 ```bash
 # Using OpenAI 
-python -m  _openai.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key "your_openai_api_key"
+python -m  _openai.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" 
 
-# Using Google Generative AI
-python -m  _google.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --google_api_key "your_google_api_key"
 ```
 
 ## Contributing 
 🌟 First consider giving it a star at the top right. It means a lot!
 Contributions are welcome and encouraged.
 Before contributing, please take a moment to review our [Contribution Guidelines](https://github.com/KevKibe/docindex/blob/master/DOCS/CONTRIBUTING.md) for important information on how to contribute to this project.
```

#### html2text {}

```diff
@@ -1,97 +1,120 @@
-Metadata-Version: 2.1 Name: docindex Version: 0.5.0 Summary: A package for fast
-indexing of multiple documents and their metadata on Pinecone. Home-page:
-https://github.com/KevKibe/docindex Author: Kevin Kibe Author-email:
-keviinkibe@gmail.com License: MIT Requires-Python: >=3.8 Description-Content-
-Type: text/markdown License-File: LICENSE Requires-Dist: pinecone-client==3.2.2
-Requires-Dist: tiktoken==0.6.0 Requires-Dist: pypdf==4.1.0 Requires-Dist:
-unstructured==0.12.6 Requires-Dist: langchain-community==0.0.31 Requires-Dist:
-langchain==0.1.14 Requires-Dist: langchain-openai==0.1.1 Requires-Dist:
-langchain-google-genai==1.0.1 Requires-Dist: langchain-pinecone==0.1.0
-Requires-Dist: google.generativeai==0.4.1
-  ************ DDooccIInnddeexx:: FFaasstt PPeerrssiisstteenntt DDooccuummeenntt EEmmbbeeddddiinnggss SSttoorraaggee ffoorr RRAAGG ************
+Metadata-Version: 2.1 Name: docindex Version: 0.6.0 Summary: A package for fast
+persistent storage of multiple document embeddings and their metadata into
+Pinecone for production-level RAG. Home-page: https://github.com/KevKibe/
+docindex Author: Kevin Kibe Author-email: keviinkibe@gmail.com License: MIT
+Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: pinecone-client==3.2.2 Requires-Dist: tiktoken==0.6.0
+Requires-Dist: pypdf==4.1.0 Requires-Dist: unstructured==0.12.6 Requires-Dist:
+langchain-community==0.0.31 Requires-Dist: langchain==0.1.14 Requires-Dist:
+langchain-openai==0.1.1 Requires-Dist: langchain-google-genai==1.0.1 Requires-
+Dist: langchain-pinecone==0.1.0 Requires-Dist: google.generativeai==0.4.1
+Requires-Dist: python-dotenv==1.0.1 Requires-Dist: python-docx==1.1.0 Requires-
+Dist: markdown==3.6 Requires-Dist: langchain-core==0.1.46 Requires-Dist:
+langchain-cohere==0.1.4
+ ************ DDooccIInnddeexx:: FFaasstt PPeerrssiisstteenntt DDooccuummeenntt EEmmbbeeddddiinnggss SSttoorraaggee ffoorr PPrroodduuccttiioonn--
+                               LLeevveell RRAAGG ************
                             _[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
   ![Diagram](diagram.png) *Efficiently store multiple document embeddings and
   their metadata, whether they're offline or online, in a persistent Pinecone
-Vector Database optimized for Retrieval Augmented Generation (RAG) applications
-fast* ## Features - â¡ï¸ **Rapid Indexing**: Quickly index multiple documents
- along with their metadata, including source, page details, and content, into
-                                 Pinecone DB.
+Vector Database optimized for production-level Retrieval Augmented Generation
+(RAG) applications fast* ## Features - â¡ï¸ **Rapid Indexing**: Quickly index
+ multiple documents along with their metadata, including source, page details,
+                        and content, into Pinecone DB.
   - ð **Document Flexibility**: Index documents from your local storage or
                            online sources with ease.
-    - ð **Format Support**: Seamlessly handle various document formats,
-                   including PDF, docx(in-development), etc.
-- ð **Embedding Services Integration**: Enjoy support for multiple embedding
-services such as OpenAI Embeddings, Google Generative AI Embeddings and more in
-                                 development.
+- ð **Format Support**: Store various document formats, including PDF, docx
+                            (in-development), etc.
+- ð **LLM Providers Integration**: Enjoy support for multiple LLM providers
+     such as OpenAI, Google Generative AI, Cohere and more in development.
  - ð ï¸ **Configurable Vectorstore**: Configure a vectorstore directly from
-  the index to facilitate RAG pipelines effortlessly. ## Setup ```python pip
-   install docindex ``` ## Getting Started - Sign up to [Pinecone](https://
-   www.pinecone.io/) and get an API key. ## Using OpenAI [![Colab](https://
-          colab.research.google.com/assets/colab-badge.svg)](https://
-                       colab.research.google.com/drive/
-    1f5DzVjM9n9XWFtErTdWkKUFtszXyqzMI#scrollTo=olWrGV2viIsP) ```python from
-_openai.docindex import OpenaiPineconeIndexer # Replace these values with your
-    actual Pinecone API key, index name, OpenAI API key pinecone_api_key =
-  "pinecone-api-key" index_name = "index-name" # e.g index-1 openai_api_key =
-    "openai-api-key" batch_limit = 20 # Batch limit for upserting documents
-  chunk_size = 256 # Optional: size of texts per chunk. # List of URLs of the
- documents to be indexed. (offline on your computer or online) urls = [ "your-
-document-1.pdf", "your-document-2.md", "your-document-3.html", "your-document-
-        4.docx", ] # Initialize the Pinecone indexer pinecone_indexer =
-OpenaiPineconeIndexer(index_name, pinecone_api_key, openai_api_key) # To create
-  a new Index pinecone_indexer.create_index() # Store the document embeddings
-   with the specified URLs and batch limit pinecone_indexer.index_documents
-   (urls,batch_limit,chunk_size) # Initialize the Vectorstore vectorstore =
- pinecone_indexer.initialize_vectorstore(index_name) ``` ```python # To delete
-     the created Index pinecone_indexer.delete_index() ``` ## Using Google
-    Generative AI [![Colab](https://colab.research.google.com/assets/colab-
-             badge.svg)](https://colab.research.google.com/drive/
-1C4DyIsWMJWUmNuXEmmUMyshqoAKspFlp?usp=sharing) ```python from _google.docindex
- import GooglePineconeIndexer # Replace these values with your actual Pinecone
-   API key, index name, Google API key pinecone_api_key = "pinecone-api-key"
-   index_name = "index-name" # e.g index-1 google_api_key = "google-api-key"
-   batch_limit = 20 # Batch limit for upserting documents chunk_size = 256 #
-   Optional: size of texts per chunk. # List of URLs of the documents to be
-   indexed. (offline on your computer or an online) urls = [ "your-document-
-   1.pdf", "your-document-2.pdf" ] pinecone_indexer = GooglePineconeIndexer
-    (index_name, pinecone_api_key, google_api_key) # To create a new Index
-   pinecone_indexer.create_index() # Store the document embeddings with the
-        specified URLs and batch limit pinecone_indexer.index_documents
-   (urls,batch_limit,chunk_size) # Initialize the Vectorstore vectorstore =
- pinecone_indexer.initialize_vectorstore(index_name) ``` ```python # To delete
-the created Index pinecone_indexer.delete_index() ``` ## Using the CLI - Clone
- the Repository: Clone or download the application code to your local machine.
-   ```bash git clone https://github.com/KevKibe/docindex.git ``` - Create a
-  virtual environment for the project and activate it. ```bash # Navigate to
+ the index to facilitate RAG pipelines effortlessly. - ð **Initialize a RAG
+Retriever**: Spin up a RAG retriever using your vectorstore. ## Setup ```python
+ pip install docindex ``` ## Getting Started - Sign up to [Pinecone](https://
+   www.pinecone.io/) and get an API key. ### Import Dependencies ```python #
+ Import the appropriate indexer class based on the language model you want to
+  use from _openai.doc_index import OpenaiPineconeIndexer # Using OpenAI from
+_google.doc_index import GooglePineconeIndexer # Using GoogleGenerativeAI from
+_cohere.doc_index import CoherePineconeIndexer # Using Cohere ``` ### API Keys
+ and Configuration ```python # Replace these values with your actual API keys
+       and index name or have them in a variable environment/secret key.
+pinecone_api_key = "your_pinecone_api_key" # Your Pinecone API key index_name =
+         "your_index_name" # Your Pinecone index name openai_api_key =
+"your_openai_api_key" # Using OpenAI) # google_api_key = "your_google_api_key"
+  # Using GoogleGenerativeAI #cohere_api_key = "your_cohere_api_key" # Using
+  Cohere # Configure batch limit and chunk size batch_limit = "batch-limit" #
+Maximum batch size for upserting documents -> Optional: Default 32 chunk_size =
+"chunk-size" # Size of texts per chunk -> Optional: Default 256 ``` ### List of
+Documents: ```python # List of URLs of the documents to be indexed. (offline on
+your computer or online) urls = [ "your-document-1.pdf", "your-document-2.md",
+    "your-document-3.html", "your-document-4.docx", ] ``` ### Index, Store
+   Documents and Initialize VectorStore ```python # Initialize the Pinecone
+    indexer with the desired model pinecone_indexer = OpenaiPineconeIndexer
+        (index_name, pinecone_api_key, openai_api_key) # Using OpenAI #
+    pinecone_indexer = GooglePineconeIndexer(index_name, pinecone_api_key,
+        google_api_key) # Using GoogleGenerativeAI # pinecone_indexer =
+  CoherePineconeIndexer(index_name, pinecone_api_key, cohere_api_key) # Using
+  Cohere # To create a new Index pinecone_indexer.create_index() # Store the
+          document embeddings with the specified URLs and batch limit
+pinecone_indexer.index_documents(urls,batch_limit,chunk_size) # Initialize the
+ Vectorstore vectorstore = pinecone_indexer.initialize_vectorstore(index_name)
+     ``` ### Query and Retrieve Information ```python query = "what is the
+ transformers architecture" response = pinecone_indexer.retrieve_and_generate
+ (vector_store = vectorstore, query = query) response ``` ### Response ```bash
+ query='what is the transformers architecture' result='The Transformer follows
+ this overall architecture using stacked self-attention and point-wise, fully-
+connected layers for both the encoder and decoder, shown in the left and right
+     halves of Figure 1, respectively.' page=1 source_documents=[Document
+(page_content='Figure 1: The Transformer - model architecture.\nThe Transformer
+follows this overall architecture using stacked self-attention and point-wise,
+fully\nconnected layers for both the encoder and decoder, shown in the left and
+       right halves of Figure 1,\nrespectively.\n3.1 Encoder and Decoder
+ Stacks\nEncoder: The encoder is composed of a stack of N= 6 identical layers.
+   Each layer has two\nsub-layers. The first is a multi-head self-attention
+ mechanism, and the second is a simple, position-\nwise fully connected feed-
+forward network. We employ a residual connection [ 11] around each of\nthe two
+ sub-layers, followed by layer normalization [ 1]. That is, the output of each
+ sub-layer is\nLayerNorm( x+ Sublayer( x)), where Sublayer( x)is the function
+implemented by the sub-layer\nitself. To facilitate these residual connections,
+all sub-layers in the model, as well as the embedding\nlayers, produce outputs
+ of dimension dmodel = 512 .\nDecoder: The decoder is also composed of a stack
+ of N= 6identical layers. In addition to the two', source=2.0, title='https://
+ arxiv.org/pdf/1706.03762.pdf')] ``` ### Query Response Attributes: ```python
+ response.query # The query that was submitted response.result # The result of
+ the query, including any retrieved information. response.source_documents # A
+list of source documents related to the query. response.sources # A list of the
+ sources (page numbers) from the source documents. response.titles # A list of
+ the titles from the source documents. response.page_contents # A list of the
+ page contents from the source documents. ``` ### Delete Index: ```python # To
+delete the created Index pinecone_indexer.delete_index() ``` ## Using the CLI -
+  Clone the Repository: Clone or download the application code to your local
+machine. ```bash git clone https://github.com/KevKibe/docindex.git ``` - Create
+ a virtual environment for the project and activate it. ```bash # Navigate to
 project repository cd docindex # create virtual environment python -m venv venv
      # activate virtual environment source venv/bin/activate ``` - Install
  dependencies by running this command ```bash pip install -r requirements.txt
  ``` - Navigate to src ```bash cd src ``` - To create an index ```bash # Using
            OpenAI python -m _openai.create_index --pinecone_api_key
-    "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key
-          "your_openai_api_key" # Using Google Generative AI python -
-m _google.create_index --pinecone_api_key "your_pinecone_api_key" --index_name
-"your_index_name" --google_api_key "your_google_api_key" ``` - Run the command
+"your_pinecone_api_key" --index_name "your_index_name" - ``` - Run the command
         to start indexing the documents ```bash # Using OpenAI python -
-  m _openai.doc_index --pinecone_api_key "your_pinecone_api_key" --index_name
- "your_index_name" --openai_api_key "your_openai_api_key" --batch_limit 10 --
-   docs "doc-1.pdf" "doc-2.pdf' --chunk_size 256 ``` ```bash # Using Google
-         Generative AI python -m _google.doc_index --pinecone_api_key
-    "your_pinecone_api_key" --index_name "your_index_name" --google_api_key
-   "your_google_api_key" --batch_limit 10 --docs "doc-1.pdf" "doc-2.pdf' --
-    chunk_size 256 ``` - To delete an index ```bash # Using OpenAI python -
+    m _openai.index_documents --pinecone_api_key "your_pinecone_api_key" --
+    index_name "your_index_name" --openai_api_key "your_openai_api_key" --
+ batch_limit "batch-limit" --docs "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-
+    size" # Using Google Generative AI python -m _google.index_documents --
+  pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --
+ google_api_key "your_google_api_key" --batch_limit "batch-limit" --docs "doc-
+      1.pdf" "doc-2.pdf' --chunk_size "chunk-size" Using Cohere python -
+    m _cohere.index_documents --pinecone_api_key "your_pinecone_api_key" --
+    index_name "your_index_name" --cohere_api_key "your_google_api_key" --
+ batch_limit "batch-limit" --docs "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-
+        size" ``` - To delete an index ```bash # Using OpenAI python -
 m _openai.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name
-    "your_index_name" --openai_api_key "your_openai_api_key" # Using Google
-        Generative AI python -m _google.delete_index --pinecone_api_key
-    "your_pinecone_api_key" --index_name "your_index_name" --google_api_key
-"your_google_api_key" ``` ## Contributing ð First consider giving it a star
-  at the top right. It means a lot! Contributions are welcome and encouraged.
-     Before contributing, please take a moment to review our [Contribution
-       Guidelines](https://github.com/KevKibe/docindex/blob/master/DOCS/
-    CONTRIBUTING.md) for important information on how to contribute to this
-project. If you're unsure about anything or need assistance, don't hesitate to
-reach out to us or open an issue to discuss your ideas. We look forward to your
-contributions! ## License This project is licensed under the MIT License - see
-the [LICENSE](https://github.com/KevKibe/docindex/blob/master/LICENSE) file for
-     details. ## Contact For any enquiries, please reach out to me through
-                             keviinkibe@gmail.com
+ "your_index_name" ``` ## Contributing ð First consider giving it a star at
+the top right. It means a lot! Contributions are welcome and encouraged. Before
+  contributing, please take a moment to review our [Contribution Guidelines]
+  (https://github.com/KevKibe/docindex/blob/master/DOCS/CONTRIBUTING.md) for
+ important information on how to contribute to this project. If you're unsure
+about anything or need assistance, don't hesitate to reach out to us or open an
+issue to discuss your ideas. We look forward to your contributions! ## License
+  This project is licensed under the MIT License - see the [LICENSE](https://
+ github.com/KevKibe/docindex/blob/master/LICENSE) file for details. ## Contact
+    For any enquiries, please reach out to me through keviinkibe@gmail.com
```

### Comparing `docindex-0.5.0/README.md` & `docindex-0.6.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,110 +1,118 @@
-<h1 align="center">DocIndex: Fast Persistent Document Embeddings Storage for RAG</h1>
+<h1 align="center">DocIndex: Fast Persistent Document Embeddings Storage for Production-Level RAG</h1>
 <p align="center">
 
   <a href="https://github.com/KevKibe/docindex/commits/">
     <img src="https://img.shields.io/github/last-commit/KevKibe/docindex?" alt="Last commit">
   </a>
   <a href="https://github.com/KevKibe/docindex/blob/master/LICENSE">
     <img src="https://img.shields.io/github/license/KevKibe/docindex?" alt="License">
   </a>
 <br>
 
 ![Diagram](diagram.png)
 
- *Efficiently store multiple document embeddings and their metadata, whether they're offline or online, in a persistent Pinecone Vector Database optimized for Retrieval Augmented Generation (RAG) applications fast*
+ *Efficiently store multiple document embeddings and their metadata, whether they're offline or online, in a persistent Pinecone Vector Database optimized for production-level Retrieval Augmented Generation (RAG) applications fast*
 ## Features
 
 - ⚡️ **Rapid Indexing**: Quickly index multiple documents along with their metadata, including source, page details, and content, into Pinecone DB.<br>
 - 📚 **Document Flexibility**: Index documents from your local storage or online sources with ease.<br>
-- 📂 **Format Support**: Seamlessly handle various document formats, including PDF, docx(in-development), etc.<br>
-- 🔁 **Embedding Services Integration**: Enjoy support for multiple embedding services such as OpenAI Embeddings, Google Generative AI Embeddings and more in development.<br>
+- 📂 **Format Support**: Store various document formats, including PDF, docx(in-development), etc.<br>
+- 🔁 **LLM Providers Integration**: Enjoy support for multiple LLM providers such as OpenAI, Google Generative AI, Cohere and more in development.<br>
 - 🛠️ **Configurable Vectorstore**: Configure a vectorstore directly from the index to facilitate RAG pipelines effortlessly.
-
+- 🔍 **Initialize a RAG Retriever**: Spin up a RAG retriever using your vectorstore.
+  
 ## Setup
 
 ```python
 pip install docindex
 ```
 
 ## Getting Started
 - Sign up to [Pinecone](https://www.pinecone.io/) and get an API key.
-## Using OpenAI 
-[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1f5DzVjM9n9XWFtErTdWkKUFtszXyqzMI#scrollTo=olWrGV2viIsP)
+### Import Dependencies
+```python
+# Import the appropriate indexer class based on the language model you want to use
+from _openai.doc_index import OpenaiPineconeIndexer  # Using OpenAI
+from _google.doc_index import GooglePineconeIndexer  # Using GoogleGenerativeAI
+from _cohere.doc_index import CoherePineconeIndexer  # Using Cohere
+```
+
+### API Keys and Configuration
 ```python
-from _openai.docindex import OpenaiPineconeIndexer
+# Replace these values with your actual API keys and index name or have them in a variable environment/secret key.
+pinecone_api_key = "your_pinecone_api_key"  # Your Pinecone API key
+index_name = "your_index_name"  # Your Pinecone index name
+
+openai_api_key = "your_openai_api_key"     # Using OpenAI)
+# google_api_key = "your_google_api_key"   # Using GoogleGenerativeAI
+#cohere_api_key = "your_cohere_api_key"    # Using Cohere
 
-# Replace these values with your actual Pinecone API key, index name, OpenAI API key
-pinecone_api_key = "pinecone-api-key"
-index_name = "index-name"               # e.g index-1
-openai_api_key = "openai-api-key"
-batch_limit = 20                        # Batch limit for upserting documents
-chunk_size = 256                        # Optional: size of texts per chunk. 
+# Configure batch limit and chunk size
+batch_limit = "batch-limit" # Maximum batch size for upserting documents -> Optional: Default 32
+chunk_size = "chunk-size"  # Size of texts per chunk -> Optional: Default 256
+```
 
+### List of Documents:
+```python
 # List of URLs of the documents to be indexed. (offline on your computer or online)
 urls = [
  "your-document-1.pdf",
  "your-document-2.md",
  "your-document-3.html",
  "your-document-4.docx",
 ]
+```
+### Index, Store Documents and Initialize VectorStore
+```python
+# Initialize the Pinecone indexer with the desired model
+
+pinecone_indexer = OpenaiPineconeIndexer(index_name, pinecone_api_key, openai_api_key)    # Using OpenAI
+# pinecone_indexer = GooglePineconeIndexer(index_name, pinecone_api_key, google_api_key)  # Using GoogleGenerativeAI
+# pinecone_indexer = CoherePineconeIndexer(index_name, pinecone_api_key, cohere_api_key)  # Using Cohere
 
-# Initialize the Pinecone indexer
-pinecone_indexer = OpenaiPineconeIndexer(index_name, pinecone_api_key, openai_api_key)
 
 # To create a new Index
 pinecone_indexer.create_index()
 
 # Store the document embeddings with the specified URLs and batch limit
 pinecone_indexer.index_documents(urls,batch_limit,chunk_size)
 
 # Initialize the Vectorstore
 vectorstore = pinecone_indexer.initialize_vectorstore(index_name)
 ```
+### Query and Retrieve Information
 ```python
-# To delete the created Index
-pinecone_indexer.delete_index()
+query = "what is the transformers architecture"
+response = pinecone_indexer.retrieve_and_generate(vector_store = vectorstore, query = query)
+response
 ```
 
+### Response
+```bash
+query='what is the transformers architecture' result='The Transformer follows this overall architecture using stacked self-attention and point-wise, fully-connected layers for both the encoder and decoder, shown in the left and right halves of Figure 1, respectively.' page=1 source_documents=[Document(page_content='Figure 1: The Transformer - model architecture.\nThe Transformer follows this overall architecture using stacked self-attention and point-wise, fully\nconnected layers for both the encoder and decoder, shown in the left and right halves of Figure 1,\nrespectively.\n3.1 Encoder and Decoder Stacks\nEncoder: The encoder is composed of a stack of N= 6 identical layers. Each layer has two\nsub-layers. The first is a multi-head self-attention mechanism, and the second is a simple, position-\nwise fully connected feed-forward network. We employ a residual connection [ 11] around each of\nthe two sub-layers, followed by layer normalization [ 1]. That is, the output of each sub-layer is\nLayerNorm( x+ Sublayer( x)), where Sublayer( x)is the function implemented by the sub-layer\nitself. To facilitate these residual connections, all sub-layers in the model, as well as the embedding\nlayers, produce outputs of dimension dmodel = 512 .\nDecoder: The decoder is also composed of a stack of N= 6identical layers. In addition to the two', source=2.0, title='https://arxiv.org/pdf/1706.03762.pdf')]
 
-## Using Google Generative AI  
-[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1C4DyIsWMJWUmNuXEmmUMyshqoAKspFlp?usp=sharing)
-```python
-from _google.docindex import GooglePineconeIndexer
-
-# Replace these values with your actual Pinecone API key, index name, Google API key
-pinecone_api_key = "pinecone-api-key"
-index_name = "index-name"                # e.g index-1
-google_api_key = "google-api-key"
-batch_limit = 20                         # Batch limit for upserting documents
-chunk_size = 256                         # Optional: size of texts per chunk. 
-
-# List of URLs of the documents to be indexed. (offline on your computer or an online)
-urls = [
- "your-document-1.pdf",
- "your-document-2.pdf"
-]
-
-pinecone_indexer = GooglePineconeIndexer(index_name, pinecone_api_key, google_api_key)
-
-# To create a new Index
-pinecone_indexer.create_index()
-
-# Store the document embeddings with the specified URLs and batch limit
-pinecone_indexer.index_documents(urls,batch_limit,chunk_size)
+```
 
-# Initialize the Vectorstore
-vectorstore = pinecone_indexer.initialize_vectorstore(index_name)
+### Query Response Attributes:
+```python
+response.query                 # The query that was submitted
+response.result                # The result of the query, including any retrieved information.
+response.source_documents      # A list of source documents related to the query.
+response.sources               # A list of the sources (page numbers) from the source documents.
+response.titles                # A list of the titles from the source documents.
+response.page_contents         # A list of the page contents from the source documents.
 ```
+
+### Delete Index: 
 ```python
 # To delete the created Index
 pinecone_indexer.delete_index()
 ```
 
-
 ## Using the CLI
 
 - Clone the Repository: Clone or download the application code to your local machine.
 ```bash
 git clone https://github.com/KevKibe/docindex.git
 ```
 
@@ -128,38 +136,40 @@
 ```bash
 cd src
 ```
 - To create an index
 
 ```bash
 # Using OpenAI 
-python -m  _openai.create_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key "your_openai_api_key"
+python -m  _openai.create_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" -
 
-# Using Google Generative AI
-python -m  _google.create_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --google_api_key "your_google_api_key"
 ```
 
 - Run the command to start indexing the documents
 
 ```bash
-# Using OpenAI 
-python -m _openai.doc_index  --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key "your_openai_api_key" --batch_limit 10 --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size 256 
-```
-```bash
-# Using Google Generative AI 
-python -m _google.doc_index  --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --google_api_key "your_google_api_key" --batch_limit 10 --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size 256 
+# Using OpenAI
+
+python -m _openai.index_documents  --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key "your_openai_api_key" --batch_limit "batch-limit" --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-size"
+
+# Using Google Generative AI
+
+python -m _google.index_documents  --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --google_api_key "your_google_api_key" --batch_limit "batch-limit" --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-size"
+
+Using Cohere
+
+python -m _cohere.index_documents   --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --cohere_api_key "your_google_api_key" --batch_limit "batch-limit" --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-size"
+
 ```
 - To delete an index
 
 ```bash
 # Using OpenAI 
-python -m  _openai.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key "your_openai_api_key"
+python -m  _openai.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" 
 
-# Using Google Generative AI
-python -m  _google.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --google_api_key "your_google_api_key"
 ```
 
 ## Contributing 
 🌟 First consider giving it a star at the top right. It means a lot!
 Contributions are welcome and encouraged.
 Before contributing, please take a moment to review our [Contribution Guidelines](https://github.com/KevKibe/docindex/blob/master/DOCS/CONTRIBUTING.md) for important information on how to contribute to this project.
```

#### html2text {}

```diff
@@ -1,87 +1,107 @@
-  ************ DDooccIInnddeexx:: FFaasstt PPeerrssiisstteenntt DDooccuummeenntt EEmmbbeeddddiinnggss SSttoorraaggee ffoorr RRAAGG ************
+ ************ DDooccIInnddeexx:: FFaasstt PPeerrssiisstteenntt DDooccuummeenntt EEmmbbeeddddiinnggss SSttoorraaggee ffoorr PPrroodduuccttiioonn--
+                               LLeevveell RRAAGG ************
                             _[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
   ![Diagram](diagram.png) *Efficiently store multiple document embeddings and
   their metadata, whether they're offline or online, in a persistent Pinecone
-Vector Database optimized for Retrieval Augmented Generation (RAG) applications
-fast* ## Features - â¡ï¸ **Rapid Indexing**: Quickly index multiple documents
- along with their metadata, including source, page details, and content, into
-                                 Pinecone DB.
+Vector Database optimized for production-level Retrieval Augmented Generation
+(RAG) applications fast* ## Features - â¡ï¸ **Rapid Indexing**: Quickly index
+ multiple documents along with their metadata, including source, page details,
+                        and content, into Pinecone DB.
   - ð **Document Flexibility**: Index documents from your local storage or
                            online sources with ease.
-    - ð **Format Support**: Seamlessly handle various document formats,
-                   including PDF, docx(in-development), etc.
-- ð **Embedding Services Integration**: Enjoy support for multiple embedding
-services such as OpenAI Embeddings, Google Generative AI Embeddings and more in
-                                 development.
+- ð **Format Support**: Store various document formats, including PDF, docx
+                            (in-development), etc.
+- ð **LLM Providers Integration**: Enjoy support for multiple LLM providers
+     such as OpenAI, Google Generative AI, Cohere and more in development.
  - ð ï¸ **Configurable Vectorstore**: Configure a vectorstore directly from
-  the index to facilitate RAG pipelines effortlessly. ## Setup ```python pip
-   install docindex ``` ## Getting Started - Sign up to [Pinecone](https://
-   www.pinecone.io/) and get an API key. ## Using OpenAI [![Colab](https://
-          colab.research.google.com/assets/colab-badge.svg)](https://
-                       colab.research.google.com/drive/
-    1f5DzVjM9n9XWFtErTdWkKUFtszXyqzMI#scrollTo=olWrGV2viIsP) ```python from
-_openai.docindex import OpenaiPineconeIndexer # Replace these values with your
-    actual Pinecone API key, index name, OpenAI API key pinecone_api_key =
-  "pinecone-api-key" index_name = "index-name" # e.g index-1 openai_api_key =
-    "openai-api-key" batch_limit = 20 # Batch limit for upserting documents
-  chunk_size = 256 # Optional: size of texts per chunk. # List of URLs of the
- documents to be indexed. (offline on your computer or online) urls = [ "your-
-document-1.pdf", "your-document-2.md", "your-document-3.html", "your-document-
-        4.docx", ] # Initialize the Pinecone indexer pinecone_indexer =
-OpenaiPineconeIndexer(index_name, pinecone_api_key, openai_api_key) # To create
-  a new Index pinecone_indexer.create_index() # Store the document embeddings
-   with the specified URLs and batch limit pinecone_indexer.index_documents
-   (urls,batch_limit,chunk_size) # Initialize the Vectorstore vectorstore =
- pinecone_indexer.initialize_vectorstore(index_name) ``` ```python # To delete
-     the created Index pinecone_indexer.delete_index() ``` ## Using Google
-    Generative AI [![Colab](https://colab.research.google.com/assets/colab-
-             badge.svg)](https://colab.research.google.com/drive/
-1C4DyIsWMJWUmNuXEmmUMyshqoAKspFlp?usp=sharing) ```python from _google.docindex
- import GooglePineconeIndexer # Replace these values with your actual Pinecone
-   API key, index name, Google API key pinecone_api_key = "pinecone-api-key"
-   index_name = "index-name" # e.g index-1 google_api_key = "google-api-key"
-   batch_limit = 20 # Batch limit for upserting documents chunk_size = 256 #
-   Optional: size of texts per chunk. # List of URLs of the documents to be
-   indexed. (offline on your computer or an online) urls = [ "your-document-
-   1.pdf", "your-document-2.pdf" ] pinecone_indexer = GooglePineconeIndexer
-    (index_name, pinecone_api_key, google_api_key) # To create a new Index
-   pinecone_indexer.create_index() # Store the document embeddings with the
-        specified URLs and batch limit pinecone_indexer.index_documents
-   (urls,batch_limit,chunk_size) # Initialize the Vectorstore vectorstore =
- pinecone_indexer.initialize_vectorstore(index_name) ``` ```python # To delete
-the created Index pinecone_indexer.delete_index() ``` ## Using the CLI - Clone
- the Repository: Clone or download the application code to your local machine.
-   ```bash git clone https://github.com/KevKibe/docindex.git ``` - Create a
-  virtual environment for the project and activate it. ```bash # Navigate to
+ the index to facilitate RAG pipelines effortlessly. - ð **Initialize a RAG
+Retriever**: Spin up a RAG retriever using your vectorstore. ## Setup ```python
+ pip install docindex ``` ## Getting Started - Sign up to [Pinecone](https://
+   www.pinecone.io/) and get an API key. ### Import Dependencies ```python #
+ Import the appropriate indexer class based on the language model you want to
+  use from _openai.doc_index import OpenaiPineconeIndexer # Using OpenAI from
+_google.doc_index import GooglePineconeIndexer # Using GoogleGenerativeAI from
+_cohere.doc_index import CoherePineconeIndexer # Using Cohere ``` ### API Keys
+ and Configuration ```python # Replace these values with your actual API keys
+       and index name or have them in a variable environment/secret key.
+pinecone_api_key = "your_pinecone_api_key" # Your Pinecone API key index_name =
+         "your_index_name" # Your Pinecone index name openai_api_key =
+"your_openai_api_key" # Using OpenAI) # google_api_key = "your_google_api_key"
+  # Using GoogleGenerativeAI #cohere_api_key = "your_cohere_api_key" # Using
+  Cohere # Configure batch limit and chunk size batch_limit = "batch-limit" #
+Maximum batch size for upserting documents -> Optional: Default 32 chunk_size =
+"chunk-size" # Size of texts per chunk -> Optional: Default 256 ``` ### List of
+Documents: ```python # List of URLs of the documents to be indexed. (offline on
+your computer or online) urls = [ "your-document-1.pdf", "your-document-2.md",
+    "your-document-3.html", "your-document-4.docx", ] ``` ### Index, Store
+   Documents and Initialize VectorStore ```python # Initialize the Pinecone
+    indexer with the desired model pinecone_indexer = OpenaiPineconeIndexer
+        (index_name, pinecone_api_key, openai_api_key) # Using OpenAI #
+    pinecone_indexer = GooglePineconeIndexer(index_name, pinecone_api_key,
+        google_api_key) # Using GoogleGenerativeAI # pinecone_indexer =
+  CoherePineconeIndexer(index_name, pinecone_api_key, cohere_api_key) # Using
+  Cohere # To create a new Index pinecone_indexer.create_index() # Store the
+          document embeddings with the specified URLs and batch limit
+pinecone_indexer.index_documents(urls,batch_limit,chunk_size) # Initialize the
+ Vectorstore vectorstore = pinecone_indexer.initialize_vectorstore(index_name)
+     ``` ### Query and Retrieve Information ```python query = "what is the
+ transformers architecture" response = pinecone_indexer.retrieve_and_generate
+ (vector_store = vectorstore, query = query) response ``` ### Response ```bash
+ query='what is the transformers architecture' result='The Transformer follows
+ this overall architecture using stacked self-attention and point-wise, fully-
+connected layers for both the encoder and decoder, shown in the left and right
+     halves of Figure 1, respectively.' page=1 source_documents=[Document
+(page_content='Figure 1: The Transformer - model architecture.\nThe Transformer
+follows this overall architecture using stacked self-attention and point-wise,
+fully\nconnected layers for both the encoder and decoder, shown in the left and
+       right halves of Figure 1,\nrespectively.\n3.1 Encoder and Decoder
+ Stacks\nEncoder: The encoder is composed of a stack of N= 6 identical layers.
+   Each layer has two\nsub-layers. The first is a multi-head self-attention
+ mechanism, and the second is a simple, position-\nwise fully connected feed-
+forward network. We employ a residual connection [ 11] around each of\nthe two
+ sub-layers, followed by layer normalization [ 1]. That is, the output of each
+ sub-layer is\nLayerNorm( x+ Sublayer( x)), where Sublayer( x)is the function
+implemented by the sub-layer\nitself. To facilitate these residual connections,
+all sub-layers in the model, as well as the embedding\nlayers, produce outputs
+ of dimension dmodel = 512 .\nDecoder: The decoder is also composed of a stack
+ of N= 6identical layers. In addition to the two', source=2.0, title='https://
+ arxiv.org/pdf/1706.03762.pdf')] ``` ### Query Response Attributes: ```python
+ response.query # The query that was submitted response.result # The result of
+ the query, including any retrieved information. response.source_documents # A
+list of source documents related to the query. response.sources # A list of the
+ sources (page numbers) from the source documents. response.titles # A list of
+ the titles from the source documents. response.page_contents # A list of the
+ page contents from the source documents. ``` ### Delete Index: ```python # To
+delete the created Index pinecone_indexer.delete_index() ``` ## Using the CLI -
+  Clone the Repository: Clone or download the application code to your local
+machine. ```bash git clone https://github.com/KevKibe/docindex.git ``` - Create
+ a virtual environment for the project and activate it. ```bash # Navigate to
 project repository cd docindex # create virtual environment python -m venv venv
      # activate virtual environment source venv/bin/activate ``` - Install
  dependencies by running this command ```bash pip install -r requirements.txt
  ``` - Navigate to src ```bash cd src ``` - To create an index ```bash # Using
            OpenAI python -m _openai.create_index --pinecone_api_key
-    "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key
-          "your_openai_api_key" # Using Google Generative AI python -
-m _google.create_index --pinecone_api_key "your_pinecone_api_key" --index_name
-"your_index_name" --google_api_key "your_google_api_key" ``` - Run the command
+"your_pinecone_api_key" --index_name "your_index_name" - ``` - Run the command
         to start indexing the documents ```bash # Using OpenAI python -
-  m _openai.doc_index --pinecone_api_key "your_pinecone_api_key" --index_name
- "your_index_name" --openai_api_key "your_openai_api_key" --batch_limit 10 --
-   docs "doc-1.pdf" "doc-2.pdf' --chunk_size 256 ``` ```bash # Using Google
-         Generative AI python -m _google.doc_index --pinecone_api_key
-    "your_pinecone_api_key" --index_name "your_index_name" --google_api_key
-   "your_google_api_key" --batch_limit 10 --docs "doc-1.pdf" "doc-2.pdf' --
-    chunk_size 256 ``` - To delete an index ```bash # Using OpenAI python -
+    m _openai.index_documents --pinecone_api_key "your_pinecone_api_key" --
+    index_name "your_index_name" --openai_api_key "your_openai_api_key" --
+ batch_limit "batch-limit" --docs "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-
+    size" # Using Google Generative AI python -m _google.index_documents --
+  pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --
+ google_api_key "your_google_api_key" --batch_limit "batch-limit" --docs "doc-
+      1.pdf" "doc-2.pdf' --chunk_size "chunk-size" Using Cohere python -
+    m _cohere.index_documents --pinecone_api_key "your_pinecone_api_key" --
+    index_name "your_index_name" --cohere_api_key "your_google_api_key" --
+ batch_limit "batch-limit" --docs "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-
+        size" ``` - To delete an index ```bash # Using OpenAI python -
 m _openai.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name
-    "your_index_name" --openai_api_key "your_openai_api_key" # Using Google
-        Generative AI python -m _google.delete_index --pinecone_api_key
-    "your_pinecone_api_key" --index_name "your_index_name" --google_api_key
-"your_google_api_key" ``` ## Contributing ð First consider giving it a star
-  at the top right. It means a lot! Contributions are welcome and encouraged.
-     Before contributing, please take a moment to review our [Contribution
-       Guidelines](https://github.com/KevKibe/docindex/blob/master/DOCS/
-    CONTRIBUTING.md) for important information on how to contribute to this
-project. If you're unsure about anything or need assistance, don't hesitate to
-reach out to us or open an issue to discuss your ideas. We look forward to your
-contributions! ## License This project is licensed under the MIT License - see
-the [LICENSE](https://github.com/KevKibe/docindex/blob/master/LICENSE) file for
-     details. ## Contact For any enquiries, please reach out to me through
-                             keviinkibe@gmail.com
+ "your_index_name" ``` ## Contributing ð First consider giving it a star at
+the top right. It means a lot! Contributions are welcome and encouraged. Before
+  contributing, please take a moment to review our [Contribution Guidelines]
+  (https://github.com/KevKibe/docindex/blob/master/DOCS/CONTRIBUTING.md) for
+ important information on how to contribute to this project. If you're unsure
+about anything or need assistance, don't hesitate to reach out to us or open an
+issue to discuss your ideas. We look forward to your contributions! ## License
+  This project is licensed under the MIT License - see the [LICENSE](https://
+ github.com/KevKibe/docindex/blob/master/LICENSE) file for details. ## Contact
+    For any enquiries, please reach out to me through keviinkibe@gmail.com
```

### Comparing `docindex-0.5.0/setup.cfg` & `docindex-0.6.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = docindex
 author = Kevin Kibe
-version = 0.5.0
+version = 0.6.0
 author_email = keviinkibe@gmail.com
-description = A package for fast indexing of multiple documents and their metadata on Pinecone.
+description = A package for fast persistent storage of multiple document embeddings and their metadata into Pinecone for production-level RAG.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/KevKibe/docindex
 license = MIT
 
 [options]
 python_requires = >=3.8
@@ -19,14 +19,19 @@
 	unstructured==0.12.6
 	langchain-community==0.0.31
 	langchain==0.1.14
 	langchain-openai==0.1.1
 	langchain-google-genai==1.0.1
 	langchain-pinecone==0.1.0
 	google.generativeai==0.4.1
+	python-dotenv==1.0.1
+	python-docx==1.1.0
+	markdown==3.6
+	langchain-core==0.1.46
+	langchain-cohere==0.1.4
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
 
 [egg_info]
```

### Comparing `docindex-0.5.0/src/_google/create_index.py` & `docindex-0.6.0/src/_google/create_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .docindex import GooglePineconeIndexer
+from .doc_index import GooglePineconeIndexer
 import argparse
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Creates an Index on Pinecone.")
     parser.add_argument("--pinecone_api_key", type=str, help="Pinecone API key")
     parser.add_argument("--index_name", type=str, help="Name of the Pinecone index")
     parser.add_argument("--google_api_key", type=str, help="Google API key")
```

### Comparing `docindex-0.5.0/src/_google/delete_index.py` & `docindex-0.6.0/src/_google/delete_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .docindex import GooglePineconeIndexer
+from .doc_index import GooglePineconeIndexer
 import argparse
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Deletes an Index on Pinecone.")
     parser.add_argument("--pinecone_api_key", type=str, help="Pinecone API key")
     parser.add_argument("--index_name", type=str, help="Name of the Pinecone index")
     parser.add_argument("--google_api_key", type=str, help="OpenAI API key")
```

### Comparing `docindex-0.5.0/src/_google/doc_index.py` & `docindex-0.6.0/src/_google/index_documents.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from .docindex import GooglePineconeIndexer
+from .doc_index import GooglePineconeIndexer
 import argparse
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Index documents on Pinecone using OpenAI embeddings.")
     parser.add_argument("--pinecone_api_key", type=str, help="Pinecone API key")
     parser.add_argument("--index_name", type=str, help="Name of the Pinecone index")
     parser.add_argument("--google_api_key", type=str, help="OpenAI API key")
-    parser.add_argument("--batch_limit", type=int,  help="Maximum batch size for indexing")
+    parser.add_argument("--batch_limit", default = 32, type=int,  help="Maximum batch size for indexing")
     parser.add_argument("--docs", nargs="+", help="URLs of the documents to be indexed")
-    parser.add_argument("--chunk_size", help="size of texts per chunk")
+    parser.add_argument("--chunk_size", default = 256, help="size of texts per chunk")
     return parser.parse_args()
 
 
 if __name__ == "__main__":
     args = parse_args()
     pinecone_indexer = GooglePineconeIndexer(args.index_name, args.pinecone_api_key, args.google_api_key)
     pinecone_indexer.index_documents(args.docs, args.batch_limit, args.chunk_size)
```

### Comparing `docindex-0.5.0/src/_google/docindex.py` & `docindex-0.6.0/src/_google/doc_index.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,20 +3,26 @@
 from uuid import uuid4
 from langchain_community.document_loaders import PyPDFLoader
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain_google_genai import GoogleGenerativeAIEmbeddings
 import tiktoken
 from typing import List
 from _openai.doc_model import Page
-from langchain_pinecone import PineconeVectorStore 
 import google.generativeai as genai
 from pathlib import Path
 from langchain_community.document_loaders import UnstructuredWordDocumentLoader
 from langchain_community.document_loaders import UnstructuredMarkdownLoader
 from langchain_community.document_loaders import UnstructuredHTMLLoader
+from langchain_pinecone import PineconeVectorStore
+from langchain_core.prompts import PromptTemplate
+from operator import itemgetter
+from langchain_google_genai import ChatGoogleGenerativeAI
+from utils.config import Config
+from utils.response_model import QueryResult
+from langchain.output_parsers import PydanticOutputParser
 
 class GooglePineconeIndexer:
     """
     Class for indexing documents to Pinecone using GoogleGenerativeAIEmbeddings embeddings.
     """
     def __init__(
         self,
@@ -87,39 +93,30 @@
             List[str]: A list of strings, where each string represents a page from the loaded document.
 
         Raises:
             ValueError: If the file type is not supported or recognized.
         """
         pages = []
         file_path = Path(file_url)
-
-        # Determine file type and use the appropriate loader
         file_extension = file_path.suffix
-
-        # Load and split PDF files
         if file_extension == ".pdf":
             loader = PyPDFLoader(file_url)
             pages = loader.load_and_split()
 
-        # Load and split DOCX and DOC files
         elif file_extension in ('.docx', '.doc'):
             loader = UnstructuredWordDocumentLoader(file_url)
             pages = loader.load_and_split()
 
-        # Load and split Markdown files
         elif file_extension == '.md':
             loader = UnstructuredMarkdownLoader(file_url)
             pages = loader.load_and_split()
 
-        # Load and split HTML files
-        elif file_extension == '.html':
             loader = UnstructuredHTMLLoader(file_url)
             pages = loader.load_and_split()
 
-        # Return the list of pages
         return pages
         
     def tiktoken_len(self, text: str) -> int:
         """
         Calculate length of text in tokens.
 
         Parameters:
@@ -189,15 +186,15 @@
                 embeds = embeds['embedding']
                 index = self.pc.Index(self.index_name)  
                 index.upsert(vectors=zip(ids, embeds, metadatas), async_req=True)
                 texts = []
                 metadatas = []
 
 
-    def index_documents(self, urls: List[str], batch_limit: int, chunk_size: int = 256) -> None:
+    def index_documents(self, urls: List[str], batch_limit: int = 32, chunk_size: int = 256) -> None:
         """
         Process a list of URLs and upsert documents to a Pinecone index.
 
         Args:
             urls (List[str]): List of URLs to process.
             batch_limit (int): Batch limit for upserting documents.
             chunks_size(int): size of texts per chunk.
@@ -230,7 +227,35 @@
         index = self.pc.Index(index_name)
         embed = GoogleGenerativeAIEmbeddings(
                 model="models/embedding-001", 
                 google_api_key=self.google_api_key
                 )
         vectorstore = PineconeVectorStore(index, embed, "text")
         return vectorstore
+
+
+    def retrieve_and_generate(self,query: str, vector_store: str, model_name: str = 'gemini-pro', top_k: int =5):
+        """
+        Retrieve documents from the Pinecone index and generate a response.
+        Args:
+            query: The qury from the user
+            index_name: The name of the Pinecone index
+            model_name: The name of the model to use : defaults to 'gemini-pro'
+            top_k: The number of documents to retrieve from the index : defaults to 5
+        """
+        llm = ChatGoogleGenerativeAI(model = Config.default_google_model, google_api_key=self.google_api_key)
+        parser = PydanticOutputParser(pydantic_object=QueryResult)
+        rag_prompt = PromptTemplate(template = Config.template_str, 
+                                    input_variables = ["query", "context"],
+                                    partial_variables={"format_instructions": parser.get_format_instructions()})
+        retriever = vector_store.as_retriever(search_kwargs = {"k": top_k})
+        
+        rag_chain = (
+            {"context": itemgetter("query")| retriever,
+            "query": itemgetter("query"),
+            }
+            | rag_prompt
+            | llm
+            | parser
+        )
+
+        return rag_chain.invoke({"query": query})
```

### Comparing `docindex-0.5.0/src/_openai/create_index.py` & `docindex-0.6.0/src/_openai/create_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .docindex import OpenaiPineconeIndexer
+from .doc_index import OpenaiPineconeIndexer
 import argparse
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Index documents on Pinecone using OpenAI embeddings.")
     parser.add_argument("--pinecone_api_key", type=str, help="Pinecone API key")
     parser.add_argument("--index_name", type=str, help="Name of the Pinecone index")
     parser.add_argument("--openai_api_key", type=str, help="OpenAI API key")
```

### Comparing `docindex-0.5.0/src/_openai/delete_index.py` & `docindex-0.6.0/src/_cohere/create_index.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from .docindex import OpenaiPineconeIndexer
+from .doc_index import CoherePineconeIndexer
 import argparse
 
 def parse_args():
-    parser = argparse.ArgumentParser(description="Index documents on Pinecone using OpenAI embeddings.")
+    parser = argparse.ArgumentParser(description="Creates an Index on Pinecone.")
     parser.add_argument("--pinecone_api_key", type=str, help="Pinecone API key")
     parser.add_argument("--index_name", type=str, help="Name of the Pinecone index")
-    parser.add_argument("--openai_api_key", type=str, help="OpenAI API key")
     return parser.parse_args()
 
 
 if __name__ == "__main__":
     args = parse_args()
-    pinecone_indexer = OpenaiPineconeIndexer(args.index_name, args.pinecone_api_key, args.openai_api_key)
-    pinecone_indexer.delete_index()
+    pinecone_indexer = CoherePineconeIndexer(args.index_name, args.pinecone_api_key)
+    pinecone_indexer.create_index()
```

### Comparing `docindex-0.5.0/src/_openai/doc_index.py` & `docindex-0.6.0/src/_openai/index_documents.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from .docindex import OpenaiPineconeIndexer
+from .doc_index import OpenaiPineconeIndexer
 import argparse
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Index documents on Pinecone using OpenAI embeddings.")
     parser.add_argument("--pinecone_api_key", type=str, help="Pinecone API key")
     parser.add_argument("--index_name", type=str, help="Name of the Pinecone index")
     parser.add_argument("--openai_api_key", type=str, help="OpenAI API key")
-    parser.add_argument("--batch_limit", type=int,  help="Maximum batch size for indexing")
+    parser.add_argument("--batch_limit", default = 20, type=int,  help="Maximum batch size for indexing")
     parser.add_argument("--docs", nargs="+", help="URLs of the documents to be indexed")
-    parser.add_argument("--chunk_size", help="size of texts per chunk")
+    parser.add_argument("--chunk_size", default = 256, help="size of texts per chunk")
     return parser.parse_args()
 
 
 if __name__ == "__main__":
     args = parse_args()
     pinecone_indexer = OpenaiPineconeIndexer(args.index_name, args.pinecone_api_key, args.openai_api_key)
     pinecone_indexer.index_documents(args.docs, args.batch_limit, args.chunk_size)
```

### Comparing `docindex-0.5.0/src/_openai/docindex.py` & `docindex-0.6.0/src/_openai/doc_index.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,19 +3,25 @@
 from uuid import uuid4
 from langchain_community.document_loaders import PyPDFLoader
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain_openai import OpenAIEmbeddings
 import tiktoken
 from typing import List
 from .doc_model import Page
-from langchain_pinecone import PineconeVectorStore 
 from pathlib import Path
 from langchain_community.document_loaders import UnstructuredWordDocumentLoader
 from langchain_community.document_loaders import UnstructuredMarkdownLoader
 from langchain_community.document_loaders import UnstructuredHTMLLoader
+from langchain_pinecone import PineconeVectorStore
+from langchain_core.prompts import PromptTemplate
+from operator import itemgetter
+from langchain_openai import ChatOpenAI
+from utils.config import Config
+from utils.response_model import QueryResult
+from langchain.output_parsers import PydanticOutputParser
 
 class OpenaiPineconeIndexer:
     """
     Class for indexing documents to Pinecone using OpenAI embeddings.
     """
     def __init__(
         self,
@@ -88,38 +94,31 @@
 
         Raises:
             ValueError: If the file type is not supported or recognized.
         """
         pages = []
         file_path = Path(file_url)
 
-        # Determine file type and use the appropriate loader
         file_extension = file_path.suffix
 
-        # Load and split PDF files
         if file_extension == ".pdf":
             loader = PyPDFLoader(file_url)
             pages = loader.load_and_split()
 
-        # Load and split DOCX and DOC files
         elif file_extension in ('.docx', '.doc'):
             loader = UnstructuredWordDocumentLoader(file_url)
             pages = loader.load_and_split()
 
-        # Load and split Markdown files
         elif file_extension == '.md':
             loader = UnstructuredMarkdownLoader(file_url)
             pages = loader.load_and_split()
 
-        # Load and split HTML files
         elif file_extension == '.html':
             loader = UnstructuredHTMLLoader(file_url)
             pages = loader.load_and_split()
-
-        # Return the list of pages
         return pages
     
     
     def tiktoken_len(self, text: str) -> int:
         """
         Calculate length of text in tokens.
 
@@ -227,7 +226,42 @@
         index = self.pc.Index(index_name)
         embed = OpenAIEmbeddings(
                 model = 'text-embedding-ada-002',
                 openai_api_key = self.openai_api_key
                 )
         vectorstore = PineconeVectorStore(index, embed, "text")
         return vectorstore
+    
+
+    def retrieve_and_generate(self,query: str, vector_store: str, model_name: str = 'gpt-3.5-turbo-1106', top_k: int =5):
+        """
+        Retrieve documents from the Pinecone index and generate a response.
+        Args:
+            query: The query from the user
+            index_name: The name of the Pinecone index
+            model_name: The name of the model to use : defaults to 'gpt-3.5-turbo-1106'
+            top_k: The number of documents to retrieve from the index : defaults to 5
+        """
+        llm = ChatOpenAI(model = Config.default_openai_model, openai_api_key = self.openai_api_key)
+        parser = PydanticOutputParser(pydantic_object=QueryResult)
+        rag_prompt = PromptTemplate(template = Config.template_str, 
+                                    input_variables = ["query", "context"],
+                                    partial_variables={"format_instructions": parser.get_format_instructions()})
+        retriever = vector_store.as_retriever(search_kwargs = {"k": top_k})
+        
+        rag_chain = (
+            {"context": itemgetter("query")| retriever,
+            "query": itemgetter("query"),
+            }
+            | rag_prompt
+            | llm
+            | parser
+        )
+
+        return rag_chain.invoke({"query": query})
+
+
+
+
+
+
+
```

### Comparing `docindex-0.5.0/src/docindex.egg-info/PKG-INFO` & `docindex-0.6.0/src/docindex.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: docindex
-Version: 0.5.0
-Summary: A package for fast indexing of multiple documents and their metadata on Pinecone.
+Version: 0.6.0
+Summary: A package for fast persistent storage of multiple document embeddings and their metadata into Pinecone for production-level RAG.
 Home-page: https://github.com/KevKibe/docindex
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,118 +15,131 @@
 Requires-Dist: unstructured==0.12.6
 Requires-Dist: langchain-community==0.0.31
 Requires-Dist: langchain==0.1.14
 Requires-Dist: langchain-openai==0.1.1
 Requires-Dist: langchain-google-genai==1.0.1
 Requires-Dist: langchain-pinecone==0.1.0
 Requires-Dist: google.generativeai==0.4.1
+Requires-Dist: python-dotenv==1.0.1
+Requires-Dist: python-docx==1.1.0
+Requires-Dist: markdown==3.6
+Requires-Dist: langchain-core==0.1.46
+Requires-Dist: langchain-cohere==0.1.4
 
-<h1 align="center">DocIndex: Fast Persistent Document Embeddings Storage for RAG</h1>
+<h1 align="center">DocIndex: Fast Persistent Document Embeddings Storage for Production-Level RAG</h1>
 <p align="center">
 
   <a href="https://github.com/KevKibe/docindex/commits/">
     <img src="https://img.shields.io/github/last-commit/KevKibe/docindex?" alt="Last commit">
   </a>
   <a href="https://github.com/KevKibe/docindex/blob/master/LICENSE">
     <img src="https://img.shields.io/github/license/KevKibe/docindex?" alt="License">
   </a>
 <br>
 
 ![Diagram](diagram.png)
 
- *Efficiently store multiple document embeddings and their metadata, whether they're offline or online, in a persistent Pinecone Vector Database optimized for Retrieval Augmented Generation (RAG) applications fast*
+ *Efficiently store multiple document embeddings and their metadata, whether they're offline or online, in a persistent Pinecone Vector Database optimized for production-level Retrieval Augmented Generation (RAG) applications fast*
 ## Features
 
 - ⚡️ **Rapid Indexing**: Quickly index multiple documents along with their metadata, including source, page details, and content, into Pinecone DB.<br>
 - 📚 **Document Flexibility**: Index documents from your local storage or online sources with ease.<br>
-- 📂 **Format Support**: Seamlessly handle various document formats, including PDF, docx(in-development), etc.<br>
-- 🔁 **Embedding Services Integration**: Enjoy support for multiple embedding services such as OpenAI Embeddings, Google Generative AI Embeddings and more in development.<br>
+- 📂 **Format Support**: Store various document formats, including PDF, docx(in-development), etc.<br>
+- 🔁 **LLM Providers Integration**: Enjoy support for multiple LLM providers such as OpenAI, Google Generative AI, Cohere and more in development.<br>
 - 🛠️ **Configurable Vectorstore**: Configure a vectorstore directly from the index to facilitate RAG pipelines effortlessly.
-
+- 🔍 **Initialize a RAG Retriever**: Spin up a RAG retriever using your vectorstore.
+  
 ## Setup
 
 ```python
 pip install docindex
 ```
 
 ## Getting Started
 - Sign up to [Pinecone](https://www.pinecone.io/) and get an API key.
-## Using OpenAI 
-[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1f5DzVjM9n9XWFtErTdWkKUFtszXyqzMI#scrollTo=olWrGV2viIsP)
+### Import Dependencies
+```python
+# Import the appropriate indexer class based on the language model you want to use
+from _openai.doc_index import OpenaiPineconeIndexer  # Using OpenAI
+from _google.doc_index import GooglePineconeIndexer  # Using GoogleGenerativeAI
+from _cohere.doc_index import CoherePineconeIndexer  # Using Cohere
+```
+
+### API Keys and Configuration
 ```python
-from _openai.docindex import OpenaiPineconeIndexer
+# Replace these values with your actual API keys and index name or have them in a variable environment/secret key.
+pinecone_api_key = "your_pinecone_api_key"  # Your Pinecone API key
+index_name = "your_index_name"  # Your Pinecone index name
+
+openai_api_key = "your_openai_api_key"     # Using OpenAI)
+# google_api_key = "your_google_api_key"   # Using GoogleGenerativeAI
+#cohere_api_key = "your_cohere_api_key"    # Using Cohere
 
-# Replace these values with your actual Pinecone API key, index name, OpenAI API key
-pinecone_api_key = "pinecone-api-key"
-index_name = "index-name"               # e.g index-1
-openai_api_key = "openai-api-key"
-batch_limit = 20                        # Batch limit for upserting documents
-chunk_size = 256                        # Optional: size of texts per chunk. 
+# Configure batch limit and chunk size
+batch_limit = "batch-limit" # Maximum batch size for upserting documents -> Optional: Default 32
+chunk_size = "chunk-size"  # Size of texts per chunk -> Optional: Default 256
+```
 
+### List of Documents:
+```python
 # List of URLs of the documents to be indexed. (offline on your computer or online)
 urls = [
  "your-document-1.pdf",
  "your-document-2.md",
  "your-document-3.html",
  "your-document-4.docx",
 ]
+```
+### Index, Store Documents and Initialize VectorStore
+```python
+# Initialize the Pinecone indexer with the desired model
+
+pinecone_indexer = OpenaiPineconeIndexer(index_name, pinecone_api_key, openai_api_key)    # Using OpenAI
+# pinecone_indexer = GooglePineconeIndexer(index_name, pinecone_api_key, google_api_key)  # Using GoogleGenerativeAI
+# pinecone_indexer = CoherePineconeIndexer(index_name, pinecone_api_key, cohere_api_key)  # Using Cohere
 
-# Initialize the Pinecone indexer
-pinecone_indexer = OpenaiPineconeIndexer(index_name, pinecone_api_key, openai_api_key)
 
 # To create a new Index
 pinecone_indexer.create_index()
 
 # Store the document embeddings with the specified URLs and batch limit
 pinecone_indexer.index_documents(urls,batch_limit,chunk_size)
 
 # Initialize the Vectorstore
 vectorstore = pinecone_indexer.initialize_vectorstore(index_name)
 ```
+### Query and Retrieve Information
 ```python
-# To delete the created Index
-pinecone_indexer.delete_index()
+query = "what is the transformers architecture"
+response = pinecone_indexer.retrieve_and_generate(vector_store = vectorstore, query = query)
+response
 ```
 
+### Response
+```bash
+query='what is the transformers architecture' result='The Transformer follows this overall architecture using stacked self-attention and point-wise, fully-connected layers for both the encoder and decoder, shown in the left and right halves of Figure 1, respectively.' page=1 source_documents=[Document(page_content='Figure 1: The Transformer - model architecture.\nThe Transformer follows this overall architecture using stacked self-attention and point-wise, fully\nconnected layers for both the encoder and decoder, shown in the left and right halves of Figure 1,\nrespectively.\n3.1 Encoder and Decoder Stacks\nEncoder: The encoder is composed of a stack of N= 6 identical layers. Each layer has two\nsub-layers. The first is a multi-head self-attention mechanism, and the second is a simple, position-\nwise fully connected feed-forward network. We employ a residual connection [ 11] around each of\nthe two sub-layers, followed by layer normalization [ 1]. That is, the output of each sub-layer is\nLayerNorm( x+ Sublayer( x)), where Sublayer( x)is the function implemented by the sub-layer\nitself. To facilitate these residual connections, all sub-layers in the model, as well as the embedding\nlayers, produce outputs of dimension dmodel = 512 .\nDecoder: The decoder is also composed of a stack of N= 6identical layers. In addition to the two', source=2.0, title='https://arxiv.org/pdf/1706.03762.pdf')]
 
-## Using Google Generative AI  
-[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1C4DyIsWMJWUmNuXEmmUMyshqoAKspFlp?usp=sharing)
-```python
-from _google.docindex import GooglePineconeIndexer
-
-# Replace these values with your actual Pinecone API key, index name, Google API key
-pinecone_api_key = "pinecone-api-key"
-index_name = "index-name"                # e.g index-1
-google_api_key = "google-api-key"
-batch_limit = 20                         # Batch limit for upserting documents
-chunk_size = 256                         # Optional: size of texts per chunk. 
-
-# List of URLs of the documents to be indexed. (offline on your computer or an online)
-urls = [
- "your-document-1.pdf",
- "your-document-2.pdf"
-]
-
-pinecone_indexer = GooglePineconeIndexer(index_name, pinecone_api_key, google_api_key)
-
-# To create a new Index
-pinecone_indexer.create_index()
-
-# Store the document embeddings with the specified URLs and batch limit
-pinecone_indexer.index_documents(urls,batch_limit,chunk_size)
+```
 
-# Initialize the Vectorstore
-vectorstore = pinecone_indexer.initialize_vectorstore(index_name)
+### Query Response Attributes:
+```python
+response.query                 # The query that was submitted
+response.result                # The result of the query, including any retrieved information.
+response.source_documents      # A list of source documents related to the query.
+response.sources               # A list of the sources (page numbers) from the source documents.
+response.titles                # A list of the titles from the source documents.
+response.page_contents         # A list of the page contents from the source documents.
 ```
+
+### Delete Index: 
 ```python
 # To delete the created Index
 pinecone_indexer.delete_index()
 ```
 
-
 ## Using the CLI
 
 - Clone the Repository: Clone or download the application code to your local machine.
 ```bash
 git clone https://github.com/KevKibe/docindex.git
 ```
 
@@ -150,38 +163,40 @@
 ```bash
 cd src
 ```
 - To create an index
 
 ```bash
 # Using OpenAI 
-python -m  _openai.create_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key "your_openai_api_key"
+python -m  _openai.create_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" -
 
-# Using Google Generative AI
-python -m  _google.create_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --google_api_key "your_google_api_key"
 ```
 
 - Run the command to start indexing the documents
 
 ```bash
-# Using OpenAI 
-python -m _openai.doc_index  --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key "your_openai_api_key" --batch_limit 10 --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size 256 
-```
-```bash
-# Using Google Generative AI 
-python -m _google.doc_index  --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --google_api_key "your_google_api_key" --batch_limit 10 --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size 256 
+# Using OpenAI
+
+python -m _openai.index_documents  --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key "your_openai_api_key" --batch_limit "batch-limit" --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-size"
+
+# Using Google Generative AI
+
+python -m _google.index_documents  --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --google_api_key "your_google_api_key" --batch_limit "batch-limit" --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-size"
+
+Using Cohere
+
+python -m _cohere.index_documents   --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --cohere_api_key "your_google_api_key" --batch_limit "batch-limit" --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-size"
+
 ```
 - To delete an index
 
 ```bash
 # Using OpenAI 
-python -m  _openai.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key "your_openai_api_key"
+python -m  _openai.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" 
 
-# Using Google Generative AI
-python -m  _google.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --google_api_key "your_google_api_key"
 ```
 
 ## Contributing 
 🌟 First consider giving it a star at the top right. It means a lot!
 Contributions are welcome and encouraged.
 Before contributing, please take a moment to review our [Contribution Guidelines](https://github.com/KevKibe/docindex/blob/master/DOCS/CONTRIBUTING.md) for important information on how to contribute to this project.
```

#### html2text {}

```diff
@@ -1,97 +1,120 @@
-Metadata-Version: 2.1 Name: docindex Version: 0.5.0 Summary: A package for fast
-indexing of multiple documents and their metadata on Pinecone. Home-page:
-https://github.com/KevKibe/docindex Author: Kevin Kibe Author-email:
-keviinkibe@gmail.com License: MIT Requires-Python: >=3.8 Description-Content-
-Type: text/markdown License-File: LICENSE Requires-Dist: pinecone-client==3.2.2
-Requires-Dist: tiktoken==0.6.0 Requires-Dist: pypdf==4.1.0 Requires-Dist:
-unstructured==0.12.6 Requires-Dist: langchain-community==0.0.31 Requires-Dist:
-langchain==0.1.14 Requires-Dist: langchain-openai==0.1.1 Requires-Dist:
-langchain-google-genai==1.0.1 Requires-Dist: langchain-pinecone==0.1.0
-Requires-Dist: google.generativeai==0.4.1
-  ************ DDooccIInnddeexx:: FFaasstt PPeerrssiisstteenntt DDooccuummeenntt EEmmbbeeddddiinnggss SSttoorraaggee ffoorr RRAAGG ************
+Metadata-Version: 2.1 Name: docindex Version: 0.6.0 Summary: A package for fast
+persistent storage of multiple document embeddings and their metadata into
+Pinecone for production-level RAG. Home-page: https://github.com/KevKibe/
+docindex Author: Kevin Kibe Author-email: keviinkibe@gmail.com License: MIT
+Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: pinecone-client==3.2.2 Requires-Dist: tiktoken==0.6.0
+Requires-Dist: pypdf==4.1.0 Requires-Dist: unstructured==0.12.6 Requires-Dist:
+langchain-community==0.0.31 Requires-Dist: langchain==0.1.14 Requires-Dist:
+langchain-openai==0.1.1 Requires-Dist: langchain-google-genai==1.0.1 Requires-
+Dist: langchain-pinecone==0.1.0 Requires-Dist: google.generativeai==0.4.1
+Requires-Dist: python-dotenv==1.0.1 Requires-Dist: python-docx==1.1.0 Requires-
+Dist: markdown==3.6 Requires-Dist: langchain-core==0.1.46 Requires-Dist:
+langchain-cohere==0.1.4
+ ************ DDooccIInnddeexx:: FFaasstt PPeerrssiisstteenntt DDooccuummeenntt EEmmbbeeddddiinnggss SSttoorraaggee ffoorr PPrroodduuccttiioonn--
+                               LLeevveell RRAAGG ************
                             _[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
   ![Diagram](diagram.png) *Efficiently store multiple document embeddings and
   their metadata, whether they're offline or online, in a persistent Pinecone
-Vector Database optimized for Retrieval Augmented Generation (RAG) applications
-fast* ## Features - â¡ï¸ **Rapid Indexing**: Quickly index multiple documents
- along with their metadata, including source, page details, and content, into
-                                 Pinecone DB.
+Vector Database optimized for production-level Retrieval Augmented Generation
+(RAG) applications fast* ## Features - â¡ï¸ **Rapid Indexing**: Quickly index
+ multiple documents along with their metadata, including source, page details,
+                        and content, into Pinecone DB.
   - ð **Document Flexibility**: Index documents from your local storage or
                            online sources with ease.
-    - ð **Format Support**: Seamlessly handle various document formats,
-                   including PDF, docx(in-development), etc.
-- ð **Embedding Services Integration**: Enjoy support for multiple embedding
-services such as OpenAI Embeddings, Google Generative AI Embeddings and more in
-                                 development.
+- ð **Format Support**: Store various document formats, including PDF, docx
+                            (in-development), etc.
+- ð **LLM Providers Integration**: Enjoy support for multiple LLM providers
+     such as OpenAI, Google Generative AI, Cohere and more in development.
  - ð ï¸ **Configurable Vectorstore**: Configure a vectorstore directly from
-  the index to facilitate RAG pipelines effortlessly. ## Setup ```python pip
-   install docindex ``` ## Getting Started - Sign up to [Pinecone](https://
-   www.pinecone.io/) and get an API key. ## Using OpenAI [![Colab](https://
-          colab.research.google.com/assets/colab-badge.svg)](https://
-                       colab.research.google.com/drive/
-    1f5DzVjM9n9XWFtErTdWkKUFtszXyqzMI#scrollTo=olWrGV2viIsP) ```python from
-_openai.docindex import OpenaiPineconeIndexer # Replace these values with your
-    actual Pinecone API key, index name, OpenAI API key pinecone_api_key =
-  "pinecone-api-key" index_name = "index-name" # e.g index-1 openai_api_key =
-    "openai-api-key" batch_limit = 20 # Batch limit for upserting documents
-  chunk_size = 256 # Optional: size of texts per chunk. # List of URLs of the
- documents to be indexed. (offline on your computer or online) urls = [ "your-
-document-1.pdf", "your-document-2.md", "your-document-3.html", "your-document-
-        4.docx", ] # Initialize the Pinecone indexer pinecone_indexer =
-OpenaiPineconeIndexer(index_name, pinecone_api_key, openai_api_key) # To create
-  a new Index pinecone_indexer.create_index() # Store the document embeddings
-   with the specified URLs and batch limit pinecone_indexer.index_documents
-   (urls,batch_limit,chunk_size) # Initialize the Vectorstore vectorstore =
- pinecone_indexer.initialize_vectorstore(index_name) ``` ```python # To delete
-     the created Index pinecone_indexer.delete_index() ``` ## Using Google
-    Generative AI [![Colab](https://colab.research.google.com/assets/colab-
-             badge.svg)](https://colab.research.google.com/drive/
-1C4DyIsWMJWUmNuXEmmUMyshqoAKspFlp?usp=sharing) ```python from _google.docindex
- import GooglePineconeIndexer # Replace these values with your actual Pinecone
-   API key, index name, Google API key pinecone_api_key = "pinecone-api-key"
-   index_name = "index-name" # e.g index-1 google_api_key = "google-api-key"
-   batch_limit = 20 # Batch limit for upserting documents chunk_size = 256 #
-   Optional: size of texts per chunk. # List of URLs of the documents to be
-   indexed. (offline on your computer or an online) urls = [ "your-document-
-   1.pdf", "your-document-2.pdf" ] pinecone_indexer = GooglePineconeIndexer
-    (index_name, pinecone_api_key, google_api_key) # To create a new Index
-   pinecone_indexer.create_index() # Store the document embeddings with the
-        specified URLs and batch limit pinecone_indexer.index_documents
-   (urls,batch_limit,chunk_size) # Initialize the Vectorstore vectorstore =
- pinecone_indexer.initialize_vectorstore(index_name) ``` ```python # To delete
-the created Index pinecone_indexer.delete_index() ``` ## Using the CLI - Clone
- the Repository: Clone or download the application code to your local machine.
-   ```bash git clone https://github.com/KevKibe/docindex.git ``` - Create a
-  virtual environment for the project and activate it. ```bash # Navigate to
+ the index to facilitate RAG pipelines effortlessly. - ð **Initialize a RAG
+Retriever**: Spin up a RAG retriever using your vectorstore. ## Setup ```python
+ pip install docindex ``` ## Getting Started - Sign up to [Pinecone](https://
+   www.pinecone.io/) and get an API key. ### Import Dependencies ```python #
+ Import the appropriate indexer class based on the language model you want to
+  use from _openai.doc_index import OpenaiPineconeIndexer # Using OpenAI from
+_google.doc_index import GooglePineconeIndexer # Using GoogleGenerativeAI from
+_cohere.doc_index import CoherePineconeIndexer # Using Cohere ``` ### API Keys
+ and Configuration ```python # Replace these values with your actual API keys
+       and index name or have them in a variable environment/secret key.
+pinecone_api_key = "your_pinecone_api_key" # Your Pinecone API key index_name =
+         "your_index_name" # Your Pinecone index name openai_api_key =
+"your_openai_api_key" # Using OpenAI) # google_api_key = "your_google_api_key"
+  # Using GoogleGenerativeAI #cohere_api_key = "your_cohere_api_key" # Using
+  Cohere # Configure batch limit and chunk size batch_limit = "batch-limit" #
+Maximum batch size for upserting documents -> Optional: Default 32 chunk_size =
+"chunk-size" # Size of texts per chunk -> Optional: Default 256 ``` ### List of
+Documents: ```python # List of URLs of the documents to be indexed. (offline on
+your computer or online) urls = [ "your-document-1.pdf", "your-document-2.md",
+    "your-document-3.html", "your-document-4.docx", ] ``` ### Index, Store
+   Documents and Initialize VectorStore ```python # Initialize the Pinecone
+    indexer with the desired model pinecone_indexer = OpenaiPineconeIndexer
+        (index_name, pinecone_api_key, openai_api_key) # Using OpenAI #
+    pinecone_indexer = GooglePineconeIndexer(index_name, pinecone_api_key,
+        google_api_key) # Using GoogleGenerativeAI # pinecone_indexer =
+  CoherePineconeIndexer(index_name, pinecone_api_key, cohere_api_key) # Using
+  Cohere # To create a new Index pinecone_indexer.create_index() # Store the
+          document embeddings with the specified URLs and batch limit
+pinecone_indexer.index_documents(urls,batch_limit,chunk_size) # Initialize the
+ Vectorstore vectorstore = pinecone_indexer.initialize_vectorstore(index_name)
+     ``` ### Query and Retrieve Information ```python query = "what is the
+ transformers architecture" response = pinecone_indexer.retrieve_and_generate
+ (vector_store = vectorstore, query = query) response ``` ### Response ```bash
+ query='what is the transformers architecture' result='The Transformer follows
+ this overall architecture using stacked self-attention and point-wise, fully-
+connected layers for both the encoder and decoder, shown in the left and right
+     halves of Figure 1, respectively.' page=1 source_documents=[Document
+(page_content='Figure 1: The Transformer - model architecture.\nThe Transformer
+follows this overall architecture using stacked self-attention and point-wise,
+fully\nconnected layers for both the encoder and decoder, shown in the left and
+       right halves of Figure 1,\nrespectively.\n3.1 Encoder and Decoder
+ Stacks\nEncoder: The encoder is composed of a stack of N= 6 identical layers.
+   Each layer has two\nsub-layers. The first is a multi-head self-attention
+ mechanism, and the second is a simple, position-\nwise fully connected feed-
+forward network. We employ a residual connection [ 11] around each of\nthe two
+ sub-layers, followed by layer normalization [ 1]. That is, the output of each
+ sub-layer is\nLayerNorm( x+ Sublayer( x)), where Sublayer( x)is the function
+implemented by the sub-layer\nitself. To facilitate these residual connections,
+all sub-layers in the model, as well as the embedding\nlayers, produce outputs
+ of dimension dmodel = 512 .\nDecoder: The decoder is also composed of a stack
+ of N= 6identical layers. In addition to the two', source=2.0, title='https://
+ arxiv.org/pdf/1706.03762.pdf')] ``` ### Query Response Attributes: ```python
+ response.query # The query that was submitted response.result # The result of
+ the query, including any retrieved information. response.source_documents # A
+list of source documents related to the query. response.sources # A list of the
+ sources (page numbers) from the source documents. response.titles # A list of
+ the titles from the source documents. response.page_contents # A list of the
+ page contents from the source documents. ``` ### Delete Index: ```python # To
+delete the created Index pinecone_indexer.delete_index() ``` ## Using the CLI -
+  Clone the Repository: Clone or download the application code to your local
+machine. ```bash git clone https://github.com/KevKibe/docindex.git ``` - Create
+ a virtual environment for the project and activate it. ```bash # Navigate to
 project repository cd docindex # create virtual environment python -m venv venv
      # activate virtual environment source venv/bin/activate ``` - Install
  dependencies by running this command ```bash pip install -r requirements.txt
  ``` - Navigate to src ```bash cd src ``` - To create an index ```bash # Using
            OpenAI python -m _openai.create_index --pinecone_api_key
-    "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key
-          "your_openai_api_key" # Using Google Generative AI python -
-m _google.create_index --pinecone_api_key "your_pinecone_api_key" --index_name
-"your_index_name" --google_api_key "your_google_api_key" ``` - Run the command
+"your_pinecone_api_key" --index_name "your_index_name" - ``` - Run the command
         to start indexing the documents ```bash # Using OpenAI python -
-  m _openai.doc_index --pinecone_api_key "your_pinecone_api_key" --index_name
- "your_index_name" --openai_api_key "your_openai_api_key" --batch_limit 10 --
-   docs "doc-1.pdf" "doc-2.pdf' --chunk_size 256 ``` ```bash # Using Google
-         Generative AI python -m _google.doc_index --pinecone_api_key
-    "your_pinecone_api_key" --index_name "your_index_name" --google_api_key
-   "your_google_api_key" --batch_limit 10 --docs "doc-1.pdf" "doc-2.pdf' --
-    chunk_size 256 ``` - To delete an index ```bash # Using OpenAI python -
+    m _openai.index_documents --pinecone_api_key "your_pinecone_api_key" --
+    index_name "your_index_name" --openai_api_key "your_openai_api_key" --
+ batch_limit "batch-limit" --docs "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-
+    size" # Using Google Generative AI python -m _google.index_documents --
+  pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --
+ google_api_key "your_google_api_key" --batch_limit "batch-limit" --docs "doc-
+      1.pdf" "doc-2.pdf' --chunk_size "chunk-size" Using Cohere python -
+    m _cohere.index_documents --pinecone_api_key "your_pinecone_api_key" --
+    index_name "your_index_name" --cohere_api_key "your_google_api_key" --
+ batch_limit "batch-limit" --docs "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-
+        size" ``` - To delete an index ```bash # Using OpenAI python -
 m _openai.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name
-    "your_index_name" --openai_api_key "your_openai_api_key" # Using Google
-        Generative AI python -m _google.delete_index --pinecone_api_key
-    "your_pinecone_api_key" --index_name "your_index_name" --google_api_key
-"your_google_api_key" ``` ## Contributing ð First consider giving it a star
-  at the top right. It means a lot! Contributions are welcome and encouraged.
-     Before contributing, please take a moment to review our [Contribution
-       Guidelines](https://github.com/KevKibe/docindex/blob/master/DOCS/
-    CONTRIBUTING.md) for important information on how to contribute to this
-project. If you're unsure about anything or need assistance, don't hesitate to
-reach out to us or open an issue to discuss your ideas. We look forward to your
-contributions! ## License This project is licensed under the MIT License - see
-the [LICENSE](https://github.com/KevKibe/docindex/blob/master/LICENSE) file for
-     details. ## Contact For any enquiries, please reach out to me through
-                             keviinkibe@gmail.com
+ "your_index_name" ``` ## Contributing ð First consider giving it a star at
+the top right. It means a lot! Contributions are welcome and encouraged. Before
+  contributing, please take a moment to review our [Contribution Guidelines]
+  (https://github.com/KevKibe/docindex/blob/master/DOCS/CONTRIBUTING.md) for
+ important information on how to contribute to this project. If you're unsure
+about anything or need assistance, don't hesitate to reach out to us or open an
+issue to discuss your ideas. We look forward to your contributions! ## License
+  This project is licensed under the MIT License - see the [LICENSE](https://
+ github.com/KevKibe/docindex/blob/master/LICENSE) file for details. ## Contact
+    For any enquiries, please reach out to me through keviinkibe@gmail.com
```

### Comparing `docindex-0.5.0/src/docindex.egg-info/SOURCES.txt` & `docindex-0.6.0/src/docindex.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
+src/_cohere/__init__.py
+src/_cohere/config.py
+src/_cohere/create_index.py
+src/_cohere/delete_index.py
+src/_cohere/doc_index.py
+src/_cohere/doc_model.py
+src/_cohere/index_documents.py
 src/_google/__init__.py
+src/_google/config.py
 src/_google/create_index.py
 src/_google/delete_index.py
 src/_google/doc_index.py
-src/_google/docindex.py
+src/_google/index_documents.py
 src/_openai/__init__.py
 src/_openai/create_index.py
 src/_openai/delete_index.py
 src/_openai/doc_index.py
 src/_openai/doc_model.py
-src/_openai/docindex.py
+src/_openai/index_documents.py
 src/docindex.egg-info/PKG-INFO
 src/docindex.egg-info/SOURCES.txt
 src/docindex.egg-info/dependency_links.txt
 src/docindex.egg-info/requires.txt
 src/docindex.egg-info/top_level.txt
 src/tests/__init__.py
+src/tests/cohereindex_test.py
 src/tests/googleindex_test.py
-src/tests/openaiindex_test.py
+src/tests/openaiindex_test.py
+src/utils/__init__.py
+src/utils/config.py
+src/utils/response_model.py
```

### Comparing `docindex-0.5.0/src/tests/googleindex_test.py` & `docindex-0.6.0/src/tests/openaiindex_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import unittest
-from _google.docindex import GooglePineconeIndexer
+from _openai.doc_index import OpenaiPineconeIndexer
 import os 
 from io import StringIO
 from unittest.mock import patch
 import pinecone
 from langchain_pinecone import PineconeVectorStore 
 from dotenv import load_dotenv
 load_dotenv()
-class TestGooglePineconeIndexer(unittest.TestCase):
+
+class TestOpenaiPineconeIndexer(unittest.TestCase):
     """
-    Test case class for the GooglePineconeIndexer.
+    Test case class for the OpenaiPineconeIndexer.
     """
 
     def setUp(self):
         """
         Set up the test case with common attributes.
         """
         self.index_name = "new-index-1"
         self.pinecone_api_key = os.environ.get('PINECONE_API_KEY')
-        self.google_api_key = os.environ.get('GOOGLE_API_KEY')
-        self.indexer = GooglePineconeIndexer(self.index_name, self.pinecone_api_key, self.google_api_key)
-
+        self.openai_api_key = os.environ.get('OPENAI_API_KEY')
+        self.indexer = OpenaiPineconeIndexer(self.index_name, self.pinecone_api_key, self.openai_api_key)
+        return super().setUp()
+    
     @patch('sys.stdout', new_callable=StringIO)
     def test_01_create_index(self, mock_stdout):
         """
         Test creating an index and assert the output.
         """
         self.indexer.create_index()
         printed_output = mock_stdout.getvalue().strip()  
@@ -52,16 +54,26 @@
     def test_03_initialize_vectorstore(self):
         """
         Test initializing the vector store and assert its type.
         """
         vectorstore = self.indexer.initialize_vectorstore(self.index_name)
         self.assertIsInstance(vectorstore, PineconeVectorStore)
 
+    def test_04_retrieve_and_generate(self):
+        """
+        Test initializing the vector store and assert its type.
+        """
+        vectorstore = self.indexer.initialize_vectorstore(self.index_name)
+        response = self.indexer.retrieve_and_generate(query = "give a short summary of the introduction",
+                                                      vector_store = vectorstore
+                                                      )
+        self.assertIsNotNone(response, "The retriever response should not be None.")
+
     @patch('sys.stdout', new_callable=StringIO)
-    def test_04_delete_index(self, mock_stdout):
+    def test_05_delete_index(self, mock_stdout):
         """
         Test deleting an index and assert the output.
         """
         self.indexer.delete_index()
         printed_output = mock_stdout.getvalue().strip()  
         lines = printed_output.split('\n')
         index_deleted_message_0 = lines[0] 
@@ -73,9 +85,9 @@
     def sort_test_methods(cls, testCaseClass, testCaseNames):
         """
         Sort test methods for better readability.
         """
         return sorted(testCaseNames)
 
 if __name__ == "__main__":
-    unittest.TestLoader.sortTestMethodsUsing = TestGooglePineconeIndexer.sort_test_methods
+    unittest.TestLoader.sortTestMethodsUsing = TestOpenaiPineconeIndexer.sort_test_methods
     unittest.main()
```

### Comparing `docindex-0.5.0/src/tests/openaiindex_test.py` & `docindex-0.6.0/src/tests/googleindex_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import unittest
-from _openai.docindex import OpenaiPineconeIndexer
+from _google.doc_index import GooglePineconeIndexer
 import os 
 from io import StringIO
 from unittest.mock import patch
 import pinecone
 from langchain_pinecone import PineconeVectorStore 
 from dotenv import load_dotenv
 load_dotenv()
-class TestOpenaiPineconeIndexer(unittest.TestCase):
+
+
+class TestGooglePineconeIndexer(unittest.TestCase):
     """
-    Test case class for the OpenaiPineconeIndexer.
+    Test case class for the GooglePineconeIndexer.
     """
 
     def setUp(self):
         """
         Set up the test case with common attributes.
         """
         self.index_name = "new-index-1"
         self.pinecone_api_key = os.environ.get('PINECONE_API_KEY')
-        self.openai_api_key = os.environ.get('OPENAI_API_KEY')
-        self.indexer = OpenaiPineconeIndexer(self.index_name, self.pinecone_api_key, self.openai_api_key)
-
+        self.google_api_key = os.environ.get('GOOGLE_API_KEY')
+        self.indexer = GooglePineconeIndexer(self.index_name, self.pinecone_api_key, self.google_api_key)
+        return super().setUp()
+    
     @patch('sys.stdout', new_callable=StringIO)
     def test_01_create_index(self, mock_stdout):
         """
         Test creating an index and assert the output.
         """
         self.indexer.create_index()
         printed_output = mock_stdout.getvalue().strip()  
@@ -52,16 +55,27 @@
     def test_03_initialize_vectorstore(self):
         """
         Test initializing the vector store and assert its type.
         """
         vectorstore = self.indexer.initialize_vectorstore(self.index_name)
         self.assertIsInstance(vectorstore, PineconeVectorStore)
 
+    def test_04_retrieve_and_generate(self):
+        """
+        Test initializing the vector store and assert its type.
+        """
+        vector_store = self.indexer.initialize_vectorstore(self.index_name)
+        response = self.indexer.retrieve_and_generate(query = "give a short summary of the introduction",
+                                                      vector_store= vector_store
+                                                      )
+        print(response)
+        self.assertIsNotNone(response, "The retriever response should not be None.")
+
     @patch('sys.stdout', new_callable=StringIO)
-    def test_04_delete_index(self, mock_stdout):
+    def test_05_delete_index(self, mock_stdout):
         """
         Test deleting an index and assert the output.
         """
         self.indexer.delete_index()
         printed_output = mock_stdout.getvalue().strip()  
         lines = printed_output.split('\n')
         index_deleted_message_0 = lines[0] 
@@ -73,9 +87,9 @@
     def sort_test_methods(cls, testCaseClass, testCaseNames):
         """
         Sort test methods for better readability.
         """
         return sorted(testCaseNames)
 
 if __name__ == "__main__":
-    unittest.TestLoader.sortTestMethodsUsing = TestOpenaiPineconeIndexer.sort_test_methods
+    unittest.TestLoader.sortTestMethodsUsing = TestGooglePineconeIndexer.sort_test_methods
     unittest.main()
```

