# Comparing `tmp/promptflow_vectordb-0.2.8-py3-none-any.whl.zip` & `tmp/promptflow_vectordb-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,141 +1,142 @@
-Zip file size: 109524 bytes, number of entries: 139
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-09 01:08 promptflow_vectordb/__init__.py
--rw-rw-rw-  2.0 fat       18 b- defN 24-Apr-09 01:08 promptflow_vectordb/_version.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-09 01:08 promptflow_vectordb/connections/__init__.py
--rw-rw-rw-  2.0 fat      255 b- defN 24-Apr-09 01:09 promptflow_vectordb/connections/pinecone.py
--rw-rw-rw-  2.0 fat      251 b- defN 24-Apr-09 01:09 promptflow_vectordb/connections/qdrant.py
--rw-rw-rw-  2.0 fat      255 b- defN 24-Apr-09 01:09 promptflow_vectordb/connections/weaviate.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/__init__.py
--rw-rw-rw-  2.0 fat     7570 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/embeddingstore_core.py
--rw-rw-rw-  2.0 fat      847 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/contracts/__init__.py
--rw-rw-rw-  2.0 fat     6006 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/contracts/config.py
--rw-rw-rw-  2.0 fat      514 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/contracts/constants.py
--rw-rw-rw-  2.0 fat      398 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/contracts/entities.py
--rw-rw-rw-  2.0 fat     3492 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/contracts/exceptions.py
--rw-rw-rw-  2.0 fat     1458 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/contracts/identifier_converter.py
--rw-rw-rw-  2.0 fat      536 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/contracts/secret.py
--rw-rw-rw-  2.0 fat     1693 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/contracts/telemetry.py
--rw-rw-rw-  2.0 fat     1370 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/contracts/types.py
--rw-rw-rw-  2.0 fat      109 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/embeddings/__init__.py
--rw-rw-rw-  2.0 fat     1215 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/embeddings/aoai_embedding.py
--rw-rw-rw-  2.0 fat      690 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/embeddings/customized_embedding.py
--rw-rw-rw-  2.0 fat      165 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/embeddings/embedding.py
--rw-rw-rw-  2.0 fat     1554 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/embeddings/embedding_factory.py
--rw-rw-rw-  2.0 fat      467 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/embeddings/empty_embedding.py
--rw-rw-rw-  2.0 fat      784 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/embeddings/openai_embedding.py
--rw-rw-rw-  2.0 fat       97 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/engine/__init__.py
--rw-rw-rw-  2.0 fat     1504 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/engine/engine.py
--rw-rw-rw-  2.0 fat     1950 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/engine/engine_factory.py
--rw-rw-rw-  2.0 fat     4207 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/engine/langchain_engine.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/logging/__init__.py
--rw-rw-rw-  2.0 fat     5505 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/logging/handlers.py
--rw-rw-rw-  2.0 fat     5224 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/logging/loggers.py
--rw-rw-rw-  2.0 fat     4370 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/logging/utils.py
--rw-rw-rw-  2.0 fat      124 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/remote_client/__init__.py
--rw-rw-rw-  2.0 fat     1560 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/remote_client/aml_data_store_client.py
--rw-rw-rw-  2.0 fat     4682 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/remote_client/azure_blob_client.py
--rw-rw-rw-  2.0 fat     2936 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/remote_client/github_client.py
--rw-rw-rw-  2.0 fat     3344 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/remote_client/http_client.py
--rw-rw-rw-  2.0 fat      661 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/remote_client/remote_client.py
--rw-rw-rw-  2.0 fat     2799 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/remote_client/remote_client_factory.py
--rw-rw-rw-  2.0 fat       94 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/store/__init__.py
--rw-rw-rw-  2.0 fat     1610 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/store/in_memory_store.py
--rw-rw-rw-  2.0 fat     5351 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/store/local_based_store.py
--rw-rw-rw-  2.0 fat     4852 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/store/remote_based_store.py
--rw-rw-rw-  2.0 fat     1239 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/store/store.py
--rw-rw-rw-  2.0 fat     1323 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/store/store_factory.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/utils/__init__.py
--rw-rw-rw-  2.0 fat     7724 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/utils/aml_helpers.py
--rw-rw-rw-  2.0 fat     1794 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/utils/azure_helpers.py
--rw-rw-rw-  2.0 fat     1560 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/utils/common_utils.py
--rw-rw-rw-  2.0 fat      853 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/utils/global_instance_manager.py
--rw-rw-rw-  2.0 fat      663 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/utils/index_factory.py
--rw-rw-rw-  2.0 fat     3284 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/utils/path_utils.py
--rw-rw-rw-  2.0 fat     1397 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/utils/retry_utils.py
--rw-rw-rw-  2.0 fat     2319 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/utils/secret_manager.py
--rw-rw-rw-  2.0 fat      472 b- defN 24-Apr-09 01:09 promptflow_vectordb/core/utils/singleton_meta.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-09 01:08 promptflow_vectordb/service/__init__.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/client/__init__.py
--rw-rw-rw-  2.0 fat     4003 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/client/embeddingstore_client.py
--rw-rw-rw-  2.0 fat       93 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/client/agent/__init__.py
--rw-rw-rw-  2.0 fat      473 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/client/agent/agent.py
--rw-rw-rw-  2.0 fat     2014 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/client/agent/agent_factory.py
--rw-rw-rw-  2.0 fat     3093 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/client/agent/cog_search_client.py
--rw-rw-rw-  2.0 fat      762 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/client/agent/file_based_agent.py
--rw-rw-rw-  2.0 fat     4747 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/client/agent/milvus_client.py
--rw-rw-rw-  2.0 fat     4552 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/client/agent/pinecone_client.py
--rw-rw-rw-  2.0 fat     2518 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/client/agent/qdrant_client.py
--rw-rw-rw-  2.0 fat     3135 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/client/agent/rest_based_agent.py
--rw-rw-rw-  2.0 fat     2655 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/client/agent/weaviate_client.py
--rw-rw-rw-  2.0 fat      367 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/contracts/__init__.py
--rw-rw-rw-  2.0 fat     4333 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/contracts/config.py
--rw-rw-rw-  2.0 fat      665 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/contracts/constants.py
--rw-rw-rw-  2.0 fat      370 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/contracts/errors.py
--rw-rw-rw-  2.0 fat     2990 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/contracts/request_obj.py
--rw-rw-rw-  2.0 fat      779 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/contracts/telemetry.py
--rw-rw-rw-  2.0 fat      330 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/contracts/types.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/server/__init__.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/server/rest/__init__.py
--rw-rw-rw-  2.0 fat     7170 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/server/rest/app.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/server/utils/__init__.py
--rw-rw-rw-  2.0 fat     7892 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/server/utils/store_request_manager.py
--rw-rw-rw-  2.0 fat     1123 b- defN 24-Apr-09 01:09 promptflow_vectordb/service/server/utils/sys_utils.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/__init__.py
--rw-rw-rw-  2.0 fat     5158 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/common_index_lookup.py
--rw-rw-rw-  2.0 fat     1005 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/faiss_index_lookup.py
--rw-rw-rw-  2.0 fat      852 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/tools_manager.py
--rw-rw-rw-  2.0 fat     3993 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/vector_db_lookup.py
--rw-rw-rw-  2.0 fat     1198 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/vector_index_lookup.py
--rw-rw-rw-  2.0 fat      101 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/adapter/__init__.py
--rw-rw-rw-  2.0 fat      309 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/adapter/adapter.py
--rw-rw-rw-  2.0 fat     1609 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/adapter/adapter_factory.py
--rw-rw-rw-  2.0 fat     4658 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/adapter/connection_based_adapter.py
--rw-rw-rw-  2.0 fat      975 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/adapter/local_faiss_adapter.py
--rw-rw-rw-  2.0 fat    12674 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/adapter/ml_index_adapter.py
--rw-rw-rw-  2.0 fat      974 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/adapter/remote_store_faiss_adapter.py
--rw-rw-rw-  2.0 fat      143 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/__init__.py
--rw-rw-rw-  2.0 fat      537 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/connection_handler.py
--rw-rw-rw-  2.0 fat     1169 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/connection_handler_factory.py
--rw-rw-rw-  2.0 fat      635 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/env_connection_handler.py
--rw-rw-rw-  2.0 fat     1188 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/keyvault_connection_hander.py
--rw-rw-rw-  2.0 fat     2515 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/workspace_connection_handler.py
--rw-rw-rw-  2.0 fat       51 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/common_index_lookup_extensions/__init__.py
--rw-rw-rw-  2.0 fat     6209 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/common_index_lookup_extensions/acs.py
--rw-rw-rw-  2.0 fat     2417 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/common_index_lookup_extensions/utils.py
--rw-rw-rw-  2.0 fat      656 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/common_index_lookup_utils/__init__.py
--rw-rw-rw-  2.0 fat     4040 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/common_index_lookup_utils/acs.py
--rw-rw-rw-  2.0 fat     1007 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/common_index_lookup_utils/constants.py
--rw-rw-rw-  2.0 fat     6088 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/common_index_lookup_utils/embeddings.py
--rw-rw-rw-  2.0 fat     1819 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/common_index_lookup_utils/index_types.py
--rw-rw-rw-  2.0 fat      478 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/common_index_lookup_utils/indices.py
--rw-rw-rw-  2.0 fat     1840 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/common_index_lookup_utils/logger.py
--rw-rw-rw-  2.0 fat    13580 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/common_index_lookup_utils/mapping.py
--rw-rw-rw-  2.0 fat     2005 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/common_index_lookup_utils/mlindex_client.py
--rw-rw-rw-  2.0 fat     1937 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/common_index_lookup_utils/pinecone.py
--rw-rw-rw-  2.0 fat     1814 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/common_index_lookup_utils/query_types.py
--rw-rw-rw-  2.0 fat     2184 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/common_index_lookup_utils/utils.py
--rw-rw-rw-  2.0 fat       89 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/contracts/__init__.py
--rw-rw-rw-  2.0 fat     5050 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/contracts/config.py
--rw-rw-rw-  2.0 fat      230 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/contracts/constants.py
--rw-rw-rw-  2.0 fat     1512 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/contracts/ml_index_yaml_config.py
--rw-rw-rw-  2.0 fat      899 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/contracts/telemetry.py
--rw-rw-rw-  2.0 fat      942 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/contracts/types.py
--rw-rw-rw-  2.0 fat      322 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/contracts/ui_config.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/utils/__init__.py
--rw-rw-rw-  2.0 fat     1539 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/utils/logging.py
--rw-rw-rw-  2.0 fat     3616 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/utils/pf_exception_helpers.py
--rw-rw-rw-  2.0 fat     3372 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/utils/pf_runtime_utils.py
--rw-rw-rw-  2.0 fat      946 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/utils/profiling.py
--rw-rw-rw-  2.0 fat     1944 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/utils/store_core_provider.py
--rw-rw-rw-  2.0 fat     2549 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/utils/workspace_connection_manager.py
--rw-rw-rw-  2.0 fat      889 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/utils/yaml_parser.py
--rw-rw-rw-  2.0 fat    12054 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/yamls/azure/common_index_lookup.yaml
--rw-rw-rw-  2.0 fat      457 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/yamls/azure/vector_index_lookup.yaml
--rw-rw-rw-  2.0 fat      443 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/yamls/shared/faiss_index_lookup.yaml
--rw-rw-rw-  2.0 fat     1507 b- defN 24-Apr-09 01:09 promptflow_vectordb/tool/yamls/shared/vector_db_lookup.yaml
--rw-rw-rw-  2.0 fat     3019 b- defN 24-Apr-09 01:14 promptflow_vectordb-0.2.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-09 01:14 promptflow_vectordb-0.2.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      200 b- defN 24-Apr-09 01:14 promptflow_vectordb-0.2.8.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       20 b- defN 24-Apr-09 01:14 promptflow_vectordb-0.2.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat    15037 b- defN 24-Apr-09 01:14 promptflow_vectordb-0.2.8.dist-info/RECORD
-139 files, 299755 bytes uncompressed, 84418 bytes compressed:  71.8%
+Zip file size: 112321 bytes, number of entries: 140
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-11 22:45 promptflow_vectordb/__init__.py
+-rw-rw-rw-  2.0 fat       18 b- defN 24-Apr-11 22:45 promptflow_vectordb/_version.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-11 22:45 promptflow_vectordb/connections/__init__.py
+-rw-rw-rw-  2.0 fat      255 b- defN 24-Apr-11 22:45 promptflow_vectordb/connections/pinecone.py
+-rw-rw-rw-  2.0 fat      251 b- defN 24-Apr-11 22:45 promptflow_vectordb/connections/qdrant.py
+-rw-rw-rw-  2.0 fat      255 b- defN 24-Apr-11 22:45 promptflow_vectordb/connections/weaviate.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/__init__.py
+-rw-rw-rw-  2.0 fat     7570 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/embeddingstore_core.py
+-rw-rw-rw-  2.0 fat      847 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/contracts/__init__.py
+-rw-rw-rw-  2.0 fat     6006 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/contracts/config.py
+-rw-rw-rw-  2.0 fat      514 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/contracts/constants.py
+-rw-rw-rw-  2.0 fat      619 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/contracts/entities.py
+-rw-rw-rw-  2.0 fat     3492 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/contracts/exceptions.py
+-rw-rw-rw-  2.0 fat     1458 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/contracts/identifier_converter.py
+-rw-rw-rw-  2.0 fat      536 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/contracts/secret.py
+-rw-rw-rw-  2.0 fat     1693 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/contracts/telemetry.py
+-rw-rw-rw-  2.0 fat     1370 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/contracts/types.py
+-rw-rw-rw-  2.0 fat      109 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/embeddings/__init__.py
+-rw-rw-rw-  2.0 fat     1215 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/embeddings/aoai_embedding.py
+-rw-rw-rw-  2.0 fat      690 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/embeddings/customized_embedding.py
+-rw-rw-rw-  2.0 fat      165 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/embeddings/embedding.py
+-rw-rw-rw-  2.0 fat     1554 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/embeddings/embedding_factory.py
+-rw-rw-rw-  2.0 fat      467 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/embeddings/empty_embedding.py
+-rw-rw-rw-  2.0 fat      784 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/embeddings/openai_embedding.py
+-rw-rw-rw-  2.0 fat       97 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/engine/__init__.py
+-rw-rw-rw-  2.0 fat     1504 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/engine/engine.py
+-rw-rw-rw-  2.0 fat     1950 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/engine/engine_factory.py
+-rw-rw-rw-  2.0 fat     4207 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/engine/langchain_engine.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/logging/__init__.py
+-rw-rw-rw-  2.0 fat     5505 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/logging/handlers.py
+-rw-rw-rw-  2.0 fat     5224 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/logging/loggers.py
+-rw-rw-rw-  2.0 fat     4370 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/logging/utils.py
+-rw-rw-rw-  2.0 fat      124 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/remote_client/__init__.py
+-rw-rw-rw-  2.0 fat     1560 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/remote_client/aml_data_store_client.py
+-rw-rw-rw-  2.0 fat     4682 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/remote_client/azure_blob_client.py
+-rw-rw-rw-  2.0 fat     2936 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/remote_client/github_client.py
+-rw-rw-rw-  2.0 fat     3344 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/remote_client/http_client.py
+-rw-rw-rw-  2.0 fat      661 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/remote_client/remote_client.py
+-rw-rw-rw-  2.0 fat     2799 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/remote_client/remote_client_factory.py
+-rw-rw-rw-  2.0 fat       94 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/store/__init__.py
+-rw-rw-rw-  2.0 fat     1610 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/store/in_memory_store.py
+-rw-rw-rw-  2.0 fat     5351 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/store/local_based_store.py
+-rw-rw-rw-  2.0 fat     4852 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/store/remote_based_store.py
+-rw-rw-rw-  2.0 fat     1239 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/store/store.py
+-rw-rw-rw-  2.0 fat     1323 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/store/store_factory.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/utils/__init__.py
+-rw-rw-rw-  2.0 fat     7724 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/utils/aml_helpers.py
+-rw-rw-rw-  2.0 fat     1794 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/utils/azure_helpers.py
+-rw-rw-rw-  2.0 fat     1560 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/utils/common_utils.py
+-rw-rw-rw-  2.0 fat      853 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/utils/global_instance_manager.py
+-rw-rw-rw-  2.0 fat      663 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/utils/index_factory.py
+-rw-rw-rw-  2.0 fat     3284 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/utils/path_utils.py
+-rw-rw-rw-  2.0 fat     1397 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/utils/retry_utils.py
+-rw-rw-rw-  2.0 fat     2319 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/utils/secret_manager.py
+-rw-rw-rw-  2.0 fat      472 b- defN 24-Apr-11 22:45 promptflow_vectordb/core/utils/singleton_meta.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/client/__init__.py
+-rw-rw-rw-  2.0 fat     4003 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/client/embeddingstore_client.py
+-rw-rw-rw-  2.0 fat       93 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/client/agent/__init__.py
+-rw-rw-rw-  2.0 fat      473 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/client/agent/agent.py
+-rw-rw-rw-  2.0 fat     2014 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/client/agent/agent_factory.py
+-rw-rw-rw-  2.0 fat     3093 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/client/agent/cog_search_client.py
+-rw-rw-rw-  2.0 fat      762 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/client/agent/file_based_agent.py
+-rw-rw-rw-  2.0 fat     4747 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/client/agent/milvus_client.py
+-rw-rw-rw-  2.0 fat     4552 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/client/agent/pinecone_client.py
+-rw-rw-rw-  2.0 fat     2518 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/client/agent/qdrant_client.py
+-rw-rw-rw-  2.0 fat     3135 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/client/agent/rest_based_agent.py
+-rw-rw-rw-  2.0 fat     2655 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/client/agent/weaviate_client.py
+-rw-rw-rw-  2.0 fat      367 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/contracts/__init__.py
+-rw-rw-rw-  2.0 fat     4333 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/contracts/config.py
+-rw-rw-rw-  2.0 fat      665 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/contracts/constants.py
+-rw-rw-rw-  2.0 fat      370 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/contracts/errors.py
+-rw-rw-rw-  2.0 fat     2990 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/contracts/request_obj.py
+-rw-rw-rw-  2.0 fat      779 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/contracts/telemetry.py
+-rw-rw-rw-  2.0 fat      330 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/contracts/types.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/server/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/server/rest/__init__.py
+-rw-rw-rw-  2.0 fat     7170 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/server/rest/app.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/server/utils/__init__.py
+-rw-rw-rw-  2.0 fat     7892 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/server/utils/store_request_manager.py
+-rw-rw-rw-  2.0 fat     1123 b- defN 24-Apr-11 22:45 promptflow_vectordb/service/server/utils/sys_utils.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/__init__.py
+-rw-rw-rw-  2.0 fat     5313 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/common_index_lookup.py
+-rw-rw-rw-  2.0 fat     1005 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/faiss_index_lookup.py
+-rw-rw-rw-  2.0 fat      852 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/tools_manager.py
+-rw-rw-rw-  2.0 fat     3993 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/vector_db_lookup.py
+-rw-rw-rw-  2.0 fat     1198 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/vector_index_lookup.py
+-rw-rw-rw-  2.0 fat      101 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/adapter/__init__.py
+-rw-rw-rw-  2.0 fat      309 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/adapter/adapter.py
+-rw-rw-rw-  2.0 fat     1609 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/adapter/adapter_factory.py
+-rw-rw-rw-  2.0 fat     4658 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/adapter/connection_based_adapter.py
+-rw-rw-rw-  2.0 fat      975 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/adapter/local_faiss_adapter.py
+-rw-rw-rw-  2.0 fat    12674 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/adapter/ml_index_adapter.py
+-rw-rw-rw-  2.0 fat      974 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/adapter/remote_store_faiss_adapter.py
+-rw-rw-rw-  2.0 fat      143 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/__init__.py
+-rw-rw-rw-  2.0 fat      537 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/connection_handler.py
+-rw-rw-rw-  2.0 fat     1169 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/connection_handler_factory.py
+-rw-rw-rw-  2.0 fat      635 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/env_connection_handler.py
+-rw-rw-rw-  2.0 fat     1188 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/keyvault_connection_hander.py
+-rw-rw-rw-  2.0 fat     2515 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/workspace_connection_handler.py
+-rw-rw-rw-  2.0 fat       51 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/common_index_lookup_extensions/__init__.py
+-rw-rw-rw-  2.0 fat     6309 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/common_index_lookup_extensions/acs.py
+-rw-rw-rw-  2.0 fat     3581 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/common_index_lookup_extensions/utils.py
+-rw-rw-rw-  2.0 fat      838 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/common_index_lookup_utils/__init__.py
+-rw-rw-rw-  2.0 fat     3298 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/common_index_lookup_utils/acs.py
+-rw-rw-rw-  2.0 fat     1077 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/common_index_lookup_utils/constants.py
+-rw-rw-rw-  2.0 fat     6088 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/common_index_lookup_utils/embeddings.py
+-rw-rw-rw-  2.0 fat     2426 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/common_index_lookup_utils/index_types.py
+-rw-rw-rw-  2.0 fat      478 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/common_index_lookup_utils/indices.py
+-rw-rw-rw-  2.0 fat     1840 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/common_index_lookup_utils/logger.py
+-rw-rw-rw-  2.0 fat    15945 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/common_index_lookup_utils/mapping.py
+-rw-rw-rw-  2.0 fat     2005 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/common_index_lookup_utils/mlindex_client.py
+-rw-rw-rw-  2.0 fat     3977 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/common_index_lookup_utils/mongodb.py
+-rw-rw-rw-  2.0 fat     1937 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/common_index_lookup_utils/pinecone.py
+-rw-rw-rw-  2.0 fat     1814 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/common_index_lookup_utils/query_types.py
+-rw-rw-rw-  2.0 fat     2184 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/common_index_lookup_utils/utils.py
+-rw-rw-rw-  2.0 fat       89 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/contracts/__init__.py
+-rw-rw-rw-  2.0 fat     5050 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/contracts/config.py
+-rw-rw-rw-  2.0 fat      230 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/contracts/constants.py
+-rw-rw-rw-  2.0 fat     1512 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/contracts/ml_index_yaml_config.py
+-rw-rw-rw-  2.0 fat      899 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/contracts/telemetry.py
+-rw-rw-rw-  2.0 fat      942 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/contracts/types.py
+-rw-rw-rw-  2.0 fat      322 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/contracts/ui_config.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/utils/__init__.py
+-rw-rw-rw-  2.0 fat     1539 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/utils/logging.py
+-rw-rw-rw-  2.0 fat     3616 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/utils/pf_exception_helpers.py
+-rw-rw-rw-  2.0 fat     3372 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/utils/pf_runtime_utils.py
+-rw-rw-rw-  2.0 fat      946 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/utils/profiling.py
+-rw-rw-rw-  2.0 fat     1944 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/utils/store_core_provider.py
+-rw-rw-rw-  2.0 fat     2549 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/utils/workspace_connection_manager.py
+-rw-rw-rw-  2.0 fat      889 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/utils/yaml_parser.py
+-rw-rw-rw-  2.0 fat    17182 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/yamls/azure/common_index_lookup.yaml
+-rw-rw-rw-  2.0 fat      457 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/yamls/azure/vector_index_lookup.yaml
+-rw-rw-rw-  2.0 fat      443 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/yamls/shared/faiss_index_lookup.yaml
+-rw-rw-rw-  2.0 fat     1507 b- defN 24-Apr-11 22:45 promptflow_vectordb/tool/yamls/shared/vector_db_lookup.yaml
+-rw-rw-rw-  2.0 fat     3514 b- defN 24-Apr-11 22:50 promptflow_vectordb-0.2.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-11 22:50 promptflow_vectordb-0.2.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      200 b- defN 24-Apr-11 22:50 promptflow_vectordb-0.2.9.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       20 b- defN 24-Apr-11 22:50 promptflow_vectordb-0.2.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat    15155 b- defN 24-Apr-11 22:50 promptflow_vectordb-0.2.9.dist-info/RECORD
+140 files, 313595 bytes uncompressed, 87017 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -330,14 +330,17 @@
 
 Filename: promptflow_vectordb/tool/common_index_lookup_utils/mapping.py
 Comment: 
 
 Filename: promptflow_vectordb/tool/common_index_lookup_utils/mlindex_client.py
 Comment: 
 
+Filename: promptflow_vectordb/tool/common_index_lookup_utils/mongodb.py
+Comment: 
+
 Filename: promptflow_vectordb/tool/common_index_lookup_utils/pinecone.py
 Comment: 
 
 Filename: promptflow_vectordb/tool/common_index_lookup_utils/query_types.py
 Comment: 
 
 Filename: promptflow_vectordb/tool/common_index_lookup_utils/utils.py
@@ -396,23 +399,23 @@
 
 Filename: promptflow_vectordb/tool/yamls/shared/faiss_index_lookup.yaml
 Comment: 
 
 Filename: promptflow_vectordb/tool/yamls/shared/vector_db_lookup.yaml
 Comment: 
 
-Filename: promptflow_vectordb-0.2.8.dist-info/METADATA
+Filename: promptflow_vectordb-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: promptflow_vectordb-0.2.8.dist-info/WHEEL
+Filename: promptflow_vectordb-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: promptflow_vectordb-0.2.8.dist-info/entry_points.txt
+Filename: promptflow_vectordb-0.2.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: promptflow_vectordb-0.2.8.dist-info/top_level.txt
+Filename: promptflow_vectordb-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: promptflow_vectordb-0.2.8.dist-info/RECORD
+Filename: promptflow_vectordb-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## promptflow_vectordb/_version.py

```diff
@@ -1 +1 @@
-VERSION = "0.2.8"
+VERSION = "0.2.9"
```

## promptflow_vectordb/core/contracts/entities.py

```diff
@@ -1,18 +1,27 @@
 from dataclasses import dataclass, asdict
-from typing import List
+from typing import List, Union
 
 
 @dataclass
 class SearchResultEntity:
     text: str = None
     vector: List[float] = None
     score: float = None
     original_entity: dict = None
-    metadata: dict = None
+    metadata: Union[dict, str] = None
+    additional_fields: dict = None
 
     def as_dict(self):
         return asdict(self)
 
     @staticmethod
     def from_dict(dict_object: dict):
         return SearchResultEntity(**dict_object)
+
+
+@dataclass
+class SearchResultDocument:
+    page_content: str = None
+    score: float = None
+    metadata: Union[dict, str] = None
+    additional_fields: dict = None
```

## promptflow_vectordb/tool/common_index_lookup.py

```diff
@@ -45,15 +45,15 @@
 )
 rag_logger = get_lookup_logger(LoggerNames.AzureMLRAG)
 
 
 @lru_cache(maxsize=32)
 def _get_search_func(mlindex_content: str, top_k: int, query_type: str):
     with measure_execution_time(LoggingEvents.SearchFunctionConstruction):
-        mlindex_config = yaml.load(mlindex_content)
+        mlindex_config = YAML().load(mlindex_content)
         index = MLIndex(mlindex_config=mlindex_config)
         search_func = build_search_func(index, top_k, query_type)
 
     with measure_execution_time(LoggingEvents.TelemetryWrapperConstruction):
 
         def telemetry_wrapper(query: str):
             with tracer.start_as_current_span("search") as span:
@@ -64,14 +64,15 @@
 
                 try:
                     loggable_results = [
                         {
                             "document.content": doc.page_content,
                             "document.score": score,
                             "document.metadata": doc.metadata,
+                            "document.additional_fields": doc.additional_fields,
                         }
                         for doc, score in search_result
                     ]
                     span.set_attribute(
                         "retrieval.documents", json.dumps(loggable_results)
                     )
                 except Exception as ex:
@@ -130,14 +131,15 @@
             ) as search_executor:
                 search_results = search_executor.map(search_func, queries)
                 results = [
                     [
                         {
                             "text": doc.page_content,
                             "metadata": doc.metadata,
+                            "additional_fields": doc.additional_fields,
                             "score": score,
                         }
                         for doc, score in search_result
                     ]
                     for search_result in search_results
                 ]
```

## promptflow_vectordb/tool/common_index_lookup_extensions/acs.py

```diff
@@ -1,10 +1,12 @@
+from ...core.contracts.entities import SearchResultDocument
+
 import json
 from langchain.docstore.document import Document
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Callable, Dict, List, Optional, Tuple, Union
 
 
 def simple_search_with_score(
         query: str,
         store: "langchain.vectorstores.AzureSearch",
         k: int = 4,
         field_mapping: Dict[str, str] = None,
@@ -38,55 +40,30 @@
     return docs
 
 
 def semantic_search_with_score(
         query: str,
         store: "langchain.vectorstores.AzureSearch",
         k: int = 4,
-        hybrid: bool = False,
         field_mapping: Dict[str, str] = None,
         filters: Optional[str] = None
 ) -> List[Tuple[Document, float]]:
     content_field = (field_mapping or {}).get("content") or "content"
     embedding_field = (field_mapping or {}).get("embedding") or "contentVector"
     metadata_field = (field_mapping or {}).get("metadata") or "meta_json_string"
 
-    if hybrid:
-        from azure.search.documents.models import Vector
-        import numpy as np
-        results = store.client.search(
-            search_text=query,
-            vectors=[
-                Vector(
-                    value=np.array(
-                        store.embedding_function(query), dtype=np.float32
-                    ).tolist(),
-                    k=50,
-                    fields=embedding_field,
-                )
-            ],
-            filter=filters,
-            query_type='semantic',
-            query_language=store.semantic_query_language,
-            semantic_configuration_name=store.semantic_configuration_name,
-            query_caption='extractive',
-            query_answer='extractive',
-            top=k,
-        )
-    else:
-        results = store.client.search(
-            search_text=query,
-            filter=filters,
-            query_type='semantic',
-            query_language=store.semantic_query_language,
-            semantic_configuration_name=store.semantic_configuration_name,
-            query_caption='extractive',
-            query_answer='extractive',
-            top=k,
-        )
+    results = store.client.search(
+        search_text=query,
+        filter=filters,
+        query_type='semantic',
+        semantic_configuration_name=store.semantic_configuration_name,
+        query_caption='extractive',
+        query_answer='extractive',
+        top=k,
+    )
 
     # Get Semantic Answers
     semantic_answers = results.get_answers() or []
     semantic_answers_dict: Dict = {}
     for semantic_answer in semantic_answers:
         semantic_answers_dict[semantic_answer.key] = {
             'text': semantic_answer.text,
@@ -124,14 +101,43 @@
         )
         for result in results
     ]
 
     return docs
 
 
+def with_metadata_unpacker(
+    search_func: Callable[[str], List[Tuple[Document, float]]],
+    metadata_field_name: str
+) -> Callable[[str], List[Tuple[SearchResultDocument, float]]]:
+    def wrapper(query: str) -> List[Tuple[Document, float]]:
+        results = search_func(query)
+        processed_results = []
+        for result, score in results:
+            metadata = result.metadata.pop(metadata_field_name, None)
+            try:
+                metadata = json.loads(metadata)
+            except Exception:
+                pass
+
+            processed_results.append((
+                SearchResultDocument(
+                    page_content=result.page_content,
+                    score=score,
+                    metadata=metadata or result.metadata,
+                    additional_fields=result.metadata
+                ),
+                score
+            ))
+
+        return processed_results
+
+    return wrapper
+
+
 def search_by_vector_with_score(
         vector: List[float],
         store: Union["langchain.vectorstores.AzureSearch", "langchain.vectorstores.FAISS"],
         kind: str,
         k: int = 4,
         field_mapping: Dict[str, str] = None,
         filters: Optional[str] = None
```

## promptflow_vectordb/tool/common_index_lookup_extensions/utils.py

```diff
@@ -1,63 +1,94 @@
-from .acs import simple_search_with_score, semantic_search_with_score
+from .acs import (
+    simple_search_with_score,
+    semantic_search_with_score,
+    with_metadata_unpacker as with_acs_metadata_unpacker
+)
 
 from ..common_index_lookup_utils.constants import QueryTypes
 
+from ...core.contracts.entities import SearchResultDocument
+
 from azureml.rag import MLIndex
 import functools
 from langchain.docstore.document import Document
 from typing import Callable, List, Tuple
 
 
 def build_search_func(index: MLIndex, top_k: int, query_type: str) -> Callable[[str], List[Tuple[Document, float]]]:
     # Override the embeddings section if we're making keyword queries.
     if query_type in {QueryTypes.Simple, QueryTypes.Semantic}:
         index.embeddings_config = {
             'schema_version': '2',
             'kind': 'none'
         }
 
-        # Temporary workaround for `as_langchain_vectorstore` throwing when field_mapping.embedding is None.
-        if 'field_mapping' in index.index_config:
-            index.index_config['field_mapping']['embedding'] = ''
+        index.index_config.get('field_mapping', {})['embedding'] = ''
 
     index_kind = index.index_config.get("kind", "none")
-    store = index.as_langchain_vectorstore()
 
     if index_kind == 'acs':
+        # Copy the MLIndex's metadata field mapping value, and force-set the value in the MLIndex to None.
+        # This will make langchain dump all the fields in the index, and we can manually extract metadata after.
+        metadata_field_name = index.index_config.get('field_mapping', {}).get('metadata', 'meta_json_string')
+        if 'field_mapping' in index.index_config:
+            index.index_config['field_mapping']['metadata'] = '@'
+        store = index.as_langchain_vectorstore()
+
         if query_type == QueryTypes.Simple:
-            return functools.partial(
+            search_func = functools.partial(
                 simple_search_with_score,
                 store=store,
                 k=top_k,
-                field_mapping=index.index_config.get('field_mapping')
+                field_mapping=index.index_config.get('field_mapping'),
             )
 
-        if query_type == QueryTypes.Semantic:
-            return functools.partial(
+        elif query_type == QueryTypes.Semantic:
+            search_func = functools.partial(
                 semantic_search_with_score,
                 store=store,
                 k=top_k,
-                field_mapping=index.index_config.get('field_mapping'),
-                hybrid=False
+                field_mapping=index.index_config.get('field_mapping')
             )
 
-        if query_type == QueryTypes.Vector:
-            # AzureSearch doesn't implement similiarity_search_with_score
-            return functools.partial(store.vector_search_with_score, k=top_k)
+        elif query_type == QueryTypes.Vector:
+            search_func = functools.partial(store.vector_search_with_score, k=top_k)
 
-        if query_type == QueryTypes.VectorSimpleHybrid:
-            return functools.partial(store.hybrid_search_with_score, k=top_k)
+        elif query_type == QueryTypes.VectorSimpleHybrid:
+            search_func = functools.partial(store.hybrid_search_with_score, k=top_k)
 
-        if query_type == QueryTypes.VectorSemanticHybrid:
-            return functools.partial(
-                semantic_search_with_score,
-                store=store,
-                k=top_k,
-                field_mapping=index.index_config.get('field_mapping'),
-                hybrid=True
-            )
+        elif query_type == QueryTypes.VectorSemanticHybrid:
+            search_func = functools.partial(store.semantic_hybrid_search_with_score, k=top_k)
+
+        else:
+            raise ValueError(f'Unsupported query type: {query_type} for index kind {index_kind}.')
+
+        return with_acs_metadata_unpacker(search_func, metadata_field_name)
     else:
         if query_type == QueryTypes.Vector:
-            return functools.partial(store.similarity_search_with_score, k=top_k)
+            return with_type_mapper(
+                functools.partial(index.as_langchain_vectorstore().similarity_search_with_score, k=top_k)
+            )
 
     raise ValueError(f'Unsupported query type: {query_type} for index kind {index_kind}.')
+
+
+def with_type_mapper(
+    search_func: Callable[[str], List[Tuple[Document, float]]]
+) -> Callable[[str], List[Tuple[SearchResultDocument, float]]]:
+    def wrapper(query: str) -> List[Tuple[Document, float]]:
+        results = search_func(query)
+        processed_results = []
+        for result, score in results:
+            processed_results.append((
+                SearchResultDocument(
+                    page_content=result.page_content,
+                    score=score,
+                    metadata=result.metadata,
+                    additional_fields=result.metadata,
+                ),
+                score
+            ))
+
+        return processed_results
+
+    return wrapper
```

## promptflow_vectordb/tool/common_index_lookup_utils/__init__.py

```diff
@@ -5,11 +5,17 @@
 from .embeddings import (  # noqa: F401
     list_available_embedding_types,
     list_embedding_models,
     list_aoai_embedding_deployments,
     list_serverless_embedding_connections)
 from .index_types import list_available_index_types  # noqa: F401
 from .indices import list_registered_mlindices  # noqa: F401
+from .mongodb import (  # noqa: F401
+    list_mongodb_connections,
+    list_mongodb_databases,
+    list_mongodb_collections,
+    list_mongodb_indexes,
+    list_mongodb_index_fields)
 from .pinecone import list_pinecone_connections, list_pinecone_indices  # noqa: F401
 from .query_types import list_available_query_types  # noqa: F401
 
 from .mapping import forward_mapping, reverse_mapping  # noqa: F401
```

## promptflow_vectordb/tool/common_index_lookup_utils/acs.py

```diff
@@ -1,84 +1,85 @@
 from .utils import CallbackContext, tool_ui_callback
 from promptflow.connections import CognitiveSearchConnection
 from typing import Dict, List
 
 
-@tool_ui_callback
-def list_acs_indices(context: CallbackContext, acs_connection: CognitiveSearchConnection) -> List[Dict[str, str]]:
+def _fetch_acs_indices(context: CallbackContext, acs_connection, acs_index_name=""):
     selected_connection = context.ml_client.connections._operation.get(
         workspace_name=context.workspace_name,
         connection_name=acs_connection,
         **context.ml_client.connections._scope_kwargs)
 
-    url = f'https://management.azure.com{context.arm_id}' +\
-        f'/connections/{selected_connection.name}/listSecrets?api-version=2022-01-01-preview'
-    auth_header = f'Bearer {context.credential.get_token("https://management.azure.com/.default").token}'
-
-    secrets_response = context.http.post(url, headers={'Authorization': auth_header}).json()
-    api_key = secrets_response.get('properties', dict()).get('credentials', dict()).get('key')
+    if selected_connection.properties.auth_type == "ApiKey":
+        # API key auth type
+        url = f'https://management.azure.com{context.arm_id}' +\
+            f'/connections/{selected_connection.name}/listSecrets?api-version=2022-01-01-preview'
+        auth_header = f'Bearer {context.credential.get_token("https://management.azure.com/.default").token}'
+        secrets_response = context.http.post(url, headers={'Authorization': auth_header}).json()
+        api_key = secrets_response.get('properties', dict()).get('credentials', dict()).get('key')
+
+        headers = {'api-key': api_key}
+    else:
+        # AAD auth type
+        auth_token = f'Bearer {context.credential.get_token("https://search.azure.com/.default").token}'
+        headers = {"Authorization": auth_token}
 
     api_version = selected_connection.properties.metadata.get('ApiVersion', '2023-03-15-preview')
-    indexes_response = context.http.get(
-        f'{selected_connection.properties.target}/indexes?api-version={api_version}',
-        headers={'api-key': api_key}).json()
+
+    if acs_index_name:
+        response = context.http.get(
+            f'{selected_connection.properties.target}/indexes/{acs_index_name}?api-version={api_version}',
+            headers=headers,
+        )
+    else:
+        response = context.http.get(
+            f'{selected_connection.properties.target}/indexes?api-version={api_version}',
+            headers=headers,
+        )
+
+    if response.status_code == 403:
+        raise Exception(
+            f"""The auth type of connection {acs_connection} does not match
+            the API Access Control level of its underlying resource.
+            Please check the resource setting."""
+        )
+
+    return response.json()
+
+
+@tool_ui_callback
+def list_acs_indices(context: CallbackContext, acs_connection: CognitiveSearchConnection) -> List[Dict[str, str]]:
+
+    indexes_response = _fetch_acs_indices(context, acs_connection)
 
     return [{
         'value': index.get('name'),
         'display_value': index.get('name')} for index in indexes_response.get('value', [])]
 
 
 @tool_ui_callback
 def list_acs_index_fields(
         context: CallbackContext,
         acs_connection: CognitiveSearchConnection,
         acs_index_name: str,
         field_data_type: str
 ) -> List[Dict[str, str]]:
-    selected_connection = context.ml_client.connections._operation.get(
-        workspace_name=context.workspace_name,
-        connection_name=acs_connection,
-        **context.ml_client.connections._scope_kwargs)
-
-    url = f'https://management.azure.com{context.arm_id}' +\
-        f'/connections/{selected_connection.name}/listSecrets?api-version=2022-01-01-preview'
-    auth_header = f'Bearer {context.credential.get_token("https://management.azure.com/.default").token}'
 
-    secrets_response = context.http.post(url, headers={'Authorization': auth_header}).json()
-    api_key = secrets_response.get('properties', dict()).get('credentials', dict()).get('key')
-
-    api_version = selected_connection.properties.metadata.get('ApiVersion', '2023-03-15-preview')
-    selected_index = context.http.get(
-        f'{selected_connection.properties.target}/indexes/{acs_index_name}?api-version={api_version}',
-        headers={'api-key': api_key}).json()
+    selected_index = _fetch_acs_indices(context, acs_connection, acs_index_name)
 
     return [{
         'value': field.get('name'),
         'display_value': field.get('name')}
         for field in selected_index.get('fields', []) if field.get('type') == field_data_type]
 
 
 @tool_ui_callback
 def list_acs_index_semantic_configurations(
         context: CallbackContext,
         acs_connection: CognitiveSearchConnection,
         acs_index_name: str
 ) -> List[Dict[str, str]]:
-    selected_connection = context.ml_client.connections._operation.get(
-        workspace_name=context.workspace_name,
-        connection_name=acs_connection,
-        **context.ml_client.connections._scope_kwargs)
 
-    url = f'https://management.azure.com{context.arm_id}' +\
-        f'/connections/{selected_connection.name}/listSecrets?api-version=2022-01-01-preview'
-    auth_header = f'Bearer {context.credential.get_token("https://management.azure.com/.default").token}'
-
-    secrets_response = context.http.post(url, headers={'Authorization': auth_header}).json()
-    api_key = secrets_response.get('properties', dict()).get('credentials', dict()).get('key')
-
-    api_version = selected_connection.properties.metadata.get('ApiVersion', '2023-03-15-preview')
-    selected_index = context.http.get(
-        f'{selected_connection.properties.target}/indexes/{acs_index_name}?api-version={api_version}',
-        headers={'api-key': api_key}).json()
+    selected_index = _fetch_acs_indices(context, acs_connection, acs_index_name)
 
     configurations = selected_index.get('semantic', {}).get('configurations', [])
     return [{'value': configuration.get('name')} for configuration in configurations]
```

## promptflow_vectordb/tool/common_index_lookup_utils/constants.py

```diff
@@ -1,12 +1,13 @@
 class IndexTypes(str):
     AzureCognitiveSearch = "Azure AI Search"
     FAISS = "FAISS"
     Pinecone = "Pinecone"
     MLIndexAsset = "Registered Index"
+    AzureCosmosDBforMongoDBvCore = "Azure CosmosDB for MongoDB vCore"
     MLIndexPath = "MLIndex file from path"
 
 
 class EmbeddingTypes(str):
     NoEmbedding = "None"
     AzureOpenAI = "Azure OpenAI"
     OpenAI = "OpenAI"
```

## promptflow_vectordb/tool/common_index_lookup_utils/index_types.py

```diff
@@ -13,23 +13,31 @@
         **context.ml_client.connections._scope_kwargs)
 
     mlindex_client = MLIndexClient(context)
     registered_indices = mlindex_client.list_indices()
 
     workspace_contains_acs_connection = False
     workspace_contains_pinecone_connection = False
+    workspace_contains_cosmosdb_connection = False
 
     for connection in connections:
         if connection.properties.category == "CognitiveSearch":
             workspace_contains_acs_connection = True
-        if connection.properties.category == "CustomKeys" and \
-                'environment' in connection.properties.metadata and 'project_id' in connection.properties.metadata:
-            workspace_contains_pinecone_connection = True
-
-        if workspace_contains_acs_connection and workspace_contains_pinecone_connection:
+        if connection.properties.category == "CustomKeys":
+            if "environment" in connection.properties.metadata and "project_id" in connection.properties.metadata:
+                workspace_contains_pinecone_connection = True
+
+            elif connection.properties.metadata.get("connection_type") == "vectorindex" and \
+                    "index_type" in connection.properties.metadata:
+                if connection.properties.metadata["index_type"] == "azurecosmosdbformongodbvcore":
+                    workspace_contains_cosmosdb_connection = True
+
+        if workspace_contains_acs_connection and \
+                workspace_contains_pinecone_connection and \
+                workspace_contains_cosmosdb_connection:
             break
 
     index_options = []
 
     if len([index for index in registered_indices if index.status == 'Ready']) > 0:
         index_options.append({
             'value': IndexTypes.MLIndexAsset,
@@ -45,12 +53,17 @@
     })
 
     if workspace_contains_pinecone_connection:
         index_options.append({
             'value': IndexTypes.Pinecone,
         })
 
+    if workspace_contains_cosmosdb_connection:
+        index_options.append({
+            'value': IndexTypes.AzureCosmosDBforMongoDBvCore
+        })
+
     index_options.append({
         'value': IndexTypes.MLIndexPath,
     })
 
     return index_options
```

## promptflow_vectordb/tool/common_index_lookup_utils/mapping.py

```diff
@@ -26,14 +26,20 @@
     acs_metadata_field: str = None,
     semantic_configuration: str = None,
     faiss_index_path: str = None,
     pinecone_index_connection: str = None,
     pinecone_index_name: str = None,
     pinecone_content_field: str = None,
     pinecone_metadata_field: str = None,
+    mongodb_connection: str = None,
+    mongodb_database: str = None,
+    mongodb_collection: str = None,
+    mongodb_index_name: str = None,
+    mongodb_content_field: str = None,
+    mongodb_embedding_field: str = None,
     embedding_type: str = None,
     aoai_embedding_connection: str = None,
     oai_embedding_connection: str = None,
     embedding_model: str = None,
     embedding_deployment: str = None,
     serverless_embedding_connection: str = None
 ) -> str:
@@ -63,30 +69,40 @@
                     yaml.dump(mlindex_config, stream)
                     mlindex_content = stream.getvalue()
         except Exception as e:
             raise ValueError(f'Failed to process mlindex content with exception: { e }')
 
         return mlindex_content
 
-    elif index_type in {IndexTypes.AzureCognitiveSearch , IndexTypes.FAISS, IndexTypes.Pinecone}:
+    elif index_type in {
+            IndexTypes.AzureCognitiveSearch,
+            IndexTypes.AzureCosmosDBforMongoDBvCore,
+            IndexTypes.FAISS,
+            IndexTypes.Pinecone}:
         mlindex_config = {
             'index': _get_index_config(
                 context,
                 index_type,
                 acs_index_connection,
                 acs_index_name,
                 acs_content_field,
                 acs_embedding_field,
                 acs_metadata_field,
                 semantic_configuration,
                 faiss_index_path,
                 pinecone_index_connection,
                 pinecone_index_name,
                 pinecone_content_field,
-                pinecone_metadata_field),
+                pinecone_metadata_field,
+                mongodb_connection,
+                mongodb_database,
+                mongodb_collection,
+                mongodb_index_name,
+                mongodb_content_field,
+                mongodb_embedding_field),
             'embeddings': get_embeddings_config(
                 context,
                 embedding_type,
                 aoai_embedding_connection,
                 oai_embedding_connection,
                 embedding_model,
                 embedding_deployment,
@@ -146,14 +162,30 @@
             "pinecone_content_field": mlindex.index_config.get("field_mapping", {}).get(
                 "content"
             ),
             "pinecone_metadata_field": mlindex.index_config.get(
                 "field_mapping", {}
             ).get("metadata"),
         }
+    elif index_kind == "azure_cosmos_mongo_vcore":
+        mapped_index_args = {
+            "index_type": IndexTypes.AzureCosmosDBforMongoDBvCore,
+            "mongodb_connection": mlindex.index_config.get("connection", {})
+            .get("id", "")
+            .split("/")[-1],
+            "mongodb_database": mlindex.index_config.get("database"),
+            "mongodb_collection": mlindex.index_config.get("collection"),
+            "mongodb_index_name": mlindex.index_config.get("index"),
+            "mongodb_content_field": mlindex.index_config.get("field_mapping", {}).get(
+                "content"
+            ),
+            "mongodb_embedding_field": mlindex.index_config.get("field_mapping", {}).get(
+                "embedding"
+            ),
+        }
     else:
         raise NotImplementedError(f'"{index_kind}" is not a supported index kind.')
 
     embedding_kind = mlindex.embeddings_config.get("kind")
     embedding_api_type = mlindex.embeddings_config.get("api_type")
     if embedding_kind == "none":
         mapped_embedding_args = {
@@ -286,14 +318,20 @@
     acs_metadata_field: str = None,
     semantic_configuration: str = None,
     faiss_index_path: str = None,
     pinecone_index_connection: str = None,
     pinecone_index_name: str = None,
     pinecone_content_field: str = None,
     pinecone_metadata_field: str = None,
+    mongodb_connection: str = None,
+    mongodb_database: str = None,
+    mongodb_collection: str = None,
+    mongodb_index_name: str = None,
+    mongodb_content_field: str = None,
+    mongodb_embeddings_field: str = None
 ) -> Dict[str, Any]:
     if index_type == IndexTypes.AzureCognitiveSearch:
         selected_connection = context.ml_client.connections._operation.get(
             workspace_name=context.workspace_name,
             connection_name=acs_index_connection,
             **context.ml_client.connections._scope_kwargs,
         )
@@ -343,14 +381,37 @@
             "index": pinecone_index_name,
             "field_mapping": {
                 "content": pinecone_content_field,
                 "metadata": pinecone_metadata_field,
             },
         }
 
+    if index_type == IndexTypes.AzureCosmosDBforMongoDBvCore:
+        selected_connection = context.ml_client.connections._operation.get(
+            workspace_name=context.workspace_name,
+            connection_name=mongodb_connection,
+            **context.ml_client.connections._scope_kwargs,
+        )
+
+        return {
+            "kind": "azure_cosmos_mongo_vcore",
+            "connection": {
+                "id": selected_connection.id,
+            },
+            "connection_type": "workspace_connection",
+            "engine": "pymongo-sdk",
+            "database": mongodb_database,
+            "collection": mongodb_collection,
+            "index": mongodb_index_name,
+            "field_mapping": {
+                "content": mongodb_content_field,
+                "embedding": mongodb_embeddings_field,
+            },
+        }
+
     raise ValueError(f"Unexpected index type: {index_type}")
 
 
 def _get_embedding_model(
     context: CallbackContext, selected_connection, deployment_name: str
 ) -> str:
     deployment_url = (
```

## promptflow_vectordb/tool/yamls/azure/common_index_lookup.yaml

```diff
@@ -73,14 +73,44 @@
           optional: true
           reference: ${inputs.pinecone_content_field}
         - name: pinecone_metadata_field
           type:
           - string
           optional: true
           reference: ${inputs.pinecone_metadata_field}
+        - name: mongodb_connection
+          type:
+          - string
+          optional: true
+          reference: ${inputs.mongodb_connection}
+        - name: mongodb_database
+          type:
+          - string
+          optional: true
+          reference: ${inputs.mongodb_database}
+        - name: mongodb_collection
+          type:
+          - string
+          optional: true
+          reference: ${inputs.mongodb_collection}
+        - name: mongodb_index_name
+          type:
+          - string
+          optional: true
+          reference: ${inputs.mongodb_index_name}
+        - name: mongodb_content_field
+          type:
+          - string
+          optional: true
+          reference: ${inputs.mongodb_content_field}
+        - name: mongodb_embedding_field
+          type:
+          - string
+          optional: true
+          reference: ${inputs.mongodb_embedding_field}
         - name: embedding_type
           type:
           - string
           optional: true
           reference: ${inputs.embedding_type}
         - name: aoai_embedding_connection
           type:
@@ -326,21 +356,163 @@
     pinecone_metadata_field:
       input_type: uionly_hidden
       type:
       - string
       enabled_by: index_type
       enabled_by_value:
       - Pinecone
+    mongodb_connection:
+      input_type: uionly_hidden
+      type:
+      - string
+      enabled_by: index_type
+      enabled_by_value:
+      - Azure CosmosDB for MongoDB vCore
+      dynamic_list:
+        func_path: promptflow_vectordb.tool.common_index_lookup_utils.list_mongodb_connections
+      allow_manual_entry: false
+      is_multi_select: false
+    mongodb_database:
+      input_type: uionly_hidden
+      type:
+      - string
+      enabled_by: index_type
+      enabled_by_value:
+      - Azure CosmosDB for MongoDB vCore
+      dynamic_list:
+        func_path: promptflow_vectordb.tool.common_index_lookup_utils.list_mongodb_databases
+        func_kwargs:
+        - name: mongodb_connection
+          type:
+          - string
+          optional: false
+          reference: ${inputs.mongodb_connection}
+      allow_manual_entry: false
+      is_multi_select: false
+    mongodb_collection:
+      input_type: uionly_hidden
+      type:
+      - string
+      enabled_by: index_type
+      enabled_by_value:
+      - Azure CosmosDB for MongoDB vCore
+      dynamic_list:
+        func_path: promptflow_vectordb.tool.common_index_lookup_utils.list_mongodb_collections
+        func_kwargs:
+        - name: mongodb_connection
+          type:
+          - string
+          optional: false
+          reference: ${inputs.mongodb_connection}
+        - name: mongodb_database
+          type:
+          - string
+          optional: false
+          reference: ${inputs.mongodb_database}
+      allow_manual_entry: false
+      is_multi_select: false
+    mongodb_index_name:
+      input_type: uionly_hidden
+      type:
+      - string
+      enabled_by: index_type
+      enabled_by_value:
+      - Azure CosmosDB for MongoDB vCore
+      dynamic_list:
+        func_path: promptflow_vectordb.tool.common_index_lookup_utils.list_mongodb_indexes
+        func_kwargs:
+        - name: mongodb_connection
+          type:
+          - string
+          optional: false
+          reference: ${inputs.mongodb_connection}
+        - name: mongodb_database
+          type:
+          - string
+          optional: false
+          reference: ${inputs.mongodb_database}
+        - name: mongodb_collection
+          type:
+          - string
+          optional: false
+          reference: ${inputs.mongodb_collection}
+      allow_manual_entry: false
+      is_multi_select: false
+    mongodb_content_field:
+      input_type: uionly_hidden
+      type:
+      - string
+      enabled_by: index_type
+      enabled_by_value:
+      - Azure CosmosDB for MongoDB vCore
+      dynamic_list:
+        func_path: promptflow_vectordb.tool.common_index_lookup_utils.list_mongodb_index_fields
+        func_kwargs:
+        - name: mongodb_connection
+          type:
+          - string
+          optional: false
+          reference: ${inputs.mongodb_connection}
+        - name: mongodb_database
+          type:
+          - string
+          optional: false
+          reference: ${inputs.mongodb_database}
+        - name: mongodb_collection
+          type:
+          - string
+          optional: false
+          reference: ${inputs.mongodb_collection}
+        - name: field_data_type
+          type:
+          - string
+          optional: false
+          default: string
+      allow_manual_entry: false
+      is_multi_select: false
+    mongodb_embedding_field:
+      input_type: uionly_hidden
+      type:
+      - string
+      enabled_by: index_type
+      enabled_by_value:
+      - Azure CosmosDB for MongoDB vCore
+      dynamic_list:
+        func_path: promptflow_vectordb.tool.common_index_lookup_utils.list_mongodb_index_fields
+        func_kwargs:
+        - name: mongodb_connection
+          type:
+          - string
+          optional: false
+          reference: ${inputs.mongodb_connection}
+        - name: mongodb_database
+          type:
+          - string
+          optional: false
+          reference: ${inputs.mongodb_database}
+        - name: mongodb_collection
+          type:
+          - string
+          optional: false
+          reference: ${inputs.mongodb_collection}
+        - name: field_data_type
+          type:
+          - string
+          optional: false
+          default: ARRAY(float)
+      allow_manual_entry: false
+      is_multi_select: false
     embedding_type:
       input_type: uionly_hidden
       type:
       - string
       enabled_by: index_type
       enabled_by_value:
       - Azure AI Search
+      - Azure CosmosDB for MongoDB vCore
       - FAISS
       - Pinecone
       dynamic_list:
         func_path: promptflow_vectordb.tool.common_index_lookup_utils.list_available_embedding_types
         func_kwargs:
         - name: index_type
           type:
```

## Comparing `promptflow_vectordb-0.2.8.dist-info/METADATA` & `promptflow_vectordb-0.2.9.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: promptflow_vectordb
-Version: 0.2.8
+Version: 0.2.9
 Summary: Prompt flow tools for accessing popular vector databases
 Author: Microsoft Corporation
 Author-email: aethercn@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Description-Content-Type: text/markdown
 Requires-Dist: azure.ai.ml >=1.5.0
 Requires-Dist: azure.identity >=1.12.0
-Requires-Dist: azureml.rag[azure,cognitive_search,faiss,pinecone] >=0.2.28
-Requires-Dist: langchain <0.2,>=0.0.123
+Requires-Dist: azureml.rag[azure,azure_cosmos_mongo_vcore,cognitive_search,faiss,pinecone] >=0.2.28
+Requires-Dist: pymongo-schema
+Requires-Dist: langchain <0.2,>=0.1
 Requires-Dist: numpy >=1.24.1
 Requires-Dist: requests >=2.28.1
 Requires-Dist: requests-cache ~=1.1.1
 Requires-Dist: ruamel.yaml <1.0.0,>=0.17.10
 Provides-Extra: azure
 Provides-Extra: hugging_face
 Requires-Dist: azureml.rag[hugging_face] >=0.2.28 ; extra == 'hugging_face'
 
 # Introduction
 
 To store and search over unstructured data, a widely adopted approach is embedding data into vectors, stored and indexed in vector databases. The promptflow-vectordb SDK is designed for PromptFlow, provides essential tools for vector similarity search within popular vector databases, including  FAISS, Qdrant, Azure Congnitive Search, and more.
 
+## 0.2.9
+- Fix compatibility issue with langchain 0.1 that broke Azure AI Search semantic searches.
+- Refactor metadata retrieval in `Index Lookup`. Metadata fields that are specifically requested are now present in the `metadata` property of a retrieval result, and all other retrieved fields have been moved to `additional_fields`, instead of being discarded.
+- Add support for bring-your-own `Azure CosmosDB for MongoDB vCore` index.
+
 ## 0.2.8
 - Add support for langchain 0.1
 - Remove preview tag from `Index Lookup`.
 - Replace `FAISS Index Lookup`, `Vector Index Lookup` and `Vector DB Lookup` internals with `Index Lookup` internals.
 - Use azureml.rag logger and promptflow.tool logger in `Index Lookup`.
 
 ## 0.2.7
```

## Comparing `promptflow_vectordb-0.2.8.dist-info/RECORD` & `promptflow_vectordb-0.2.9.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 promptflow_vectordb/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-promptflow_vectordb/_version.py,sha256=isVN5u10HK02j7X1XC40jDSuadZQ8-Gv_Ax0AMxwHkw,18
+promptflow_vectordb/_version.py,sha256=xcHqQCfqvl5HQQt-xKKyKY65g0JwSXvtJ6TusOLm7no,18
 promptflow_vectordb/connections/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 promptflow_vectordb/connections/pinecone.py,sha256=YwFvw1QaFtx3CGSOTwCK5Tm9SsamGKqYqetJslE5qvk,255
 promptflow_vectordb/connections/qdrant.py,sha256=SFAG6l66RcIle5YB0SHTDrbVAU_6a5PFJ525i0rwrm8,251
 promptflow_vectordb/connections/weaviate.py,sha256=Pi1GeyduGy4WdWhQShZmtBV5jXqJ7kE1e9GR6zlMDsw,255
 promptflow_vectordb/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 promptflow_vectordb/core/embeddingstore_core.py,sha256=wJvGBmf8R4jrexb0sg2typehDDqKpYOSzNylsP-p1tM,7570
 promptflow_vectordb/core/contracts/__init__.py,sha256=eFCBv6fY_BBu8mNEPtD99RQtSzSiKhDGHmxy0H-5NSw,847
 promptflow_vectordb/core/contracts/config.py,sha256=hdxaEe9OF9YKwI8ObRlu5vvv0dGiQnMroKLEq6__Uck,6006
 promptflow_vectordb/core/contracts/constants.py,sha256=yy-vde1oGkQXbT790IqOldIxal-2O2C5CMRtVjZ8Tlw,514
-promptflow_vectordb/core/contracts/entities.py,sha256=IbmvqFxnGvGKevoyYvLzUEcwopfK_OZtPEBIRJ-sbdU,398
+promptflow_vectordb/core/contracts/entities.py,sha256=k06GGIlY0Kefz5ZFwl5wgQDlr0Wgq-3FtkVOetyquZQ,619
 promptflow_vectordb/core/contracts/exceptions.py,sha256=bRTVyW9kqNfbH3GxqFR8jZanyjlP9GbhQEHwlEfCPLA,3492
 promptflow_vectordb/core/contracts/identifier_converter.py,sha256=MiU0J2SFPd3s_cbQEosrc3xD-4_p9qljA8LgUyBshDg,1458
 promptflow_vectordb/core/contracts/secret.py,sha256=GvtJfdbQHa81ViEtl1qtq0Ol8o-5kxF1V9YJrAm07nQ,536
 promptflow_vectordb/core/contracts/telemetry.py,sha256=ZEMd9onRTOWoNwqHzt5EFOhnkq133x2yXckBI_qmTa0,1693
 promptflow_vectordb/core/contracts/types.py,sha256=IctfLPZp85_G3JaHfN8VOCa9s_t3Q8954iAG83qZYFY,1370
 promptflow_vectordb/core/embeddings/__init__.py,sha256=8AK2jZrxAyM13J9K1lfhEjRTi8uEelSkQiMuw9vo71A,109
 promptflow_vectordb/core/embeddings/aoai_embedding.py,sha256=4vqtMDHPlNT4qp6q_T3d3GJ-zmt7nc_IE4PZ3JXlycg,1215
@@ -76,15 +76,15 @@
 promptflow_vectordb/service/server/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 promptflow_vectordb/service/server/rest/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 promptflow_vectordb/service/server/rest/app.py,sha256=cNm_gec3eQ97SQjKXTAklTsfnAgSt_qHfrB1W8bFttM,7170
 promptflow_vectordb/service/server/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 promptflow_vectordb/service/server/utils/store_request_manager.py,sha256=PkwL4jwDrNHZu3q2bjA-RUev6cRa9CHQ7KZttZuiRMs,7892
 promptflow_vectordb/service/server/utils/sys_utils.py,sha256=xnBWoydnVQsvg92SiifMpaid5TelpLZm4aTVfAXvrPo,1123
 promptflow_vectordb/tool/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-promptflow_vectordb/tool/common_index_lookup.py,sha256=HuUq1Fh5UAjyPhntpqLvv4D8vZreKVWdRU9DzPXqmsI,5158
+promptflow_vectordb/tool/common_index_lookup.py,sha256=VaxnDdZxF43vxevHbmKG-7kBNtRYjUUvBxWia7xoPZ0,5313
 promptflow_vectordb/tool/faiss_index_lookup.py,sha256=1ToAYaqJZrUDXkZP-UsRp6FeIrttjmYUWeYezfl5Qyo,1005
 promptflow_vectordb/tool/tools_manager.py,sha256=wHtbtQo53fT9HAMBHtp8zIrEgBw-BCZ1Ogl9Ks1RsZQ,852
 promptflow_vectordb/tool/vector_db_lookup.py,sha256=SegqcYrZXWWup_xT8IywTqoniMgGer8OgxgUIrqdL74,3993
 promptflow_vectordb/tool/vector_index_lookup.py,sha256=XSxpjH4RDCsq1bL5L-tl_DVdLhoJD5OV1vwoK-dTNs8,1198
 promptflow_vectordb/tool/adapter/__init__.py,sha256=MFWKX1_d679pLONjxH-hf59HKN8JbOrNfzhMMDOSLqw,101
 promptflow_vectordb/tool/adapter/adapter.py,sha256=RhRZqaJK6OrEngJqYjPTpaqIgPvI9faEkDQUH-1BT_M,309
 promptflow_vectordb/tool/adapter/adapter_factory.py,sha256=VgjbUI0L0OZLTwuQOzSDQtDq0fVl8Muh7f1FUxzOKdA,1609
@@ -95,25 +95,26 @@
 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/__init__.py,sha256=hB9H4VgXSp1dLuMvy1xLYC1WEHzQanwhkYKpuQJS6BE,143
 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/connection_handler.py,sha256=tiZWVt19J58Azkq9D093EJ4zI26Zz0ranOZRfMkhTEo,537
 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/connection_handler_factory.py,sha256=J-sP5ZqxDq1020kk0t1eiqhoJKovicGJDoxERQBUrxk,1169
 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/env_connection_handler.py,sha256=HXWyQmXfa-pBgZBTcLEH3vIG2FifZEy0b6_oIbYE238,635
 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/keyvault_connection_hander.py,sha256=VPRb1TZa5880ShojzepJRHWr_8mMCV7qWED25jKlqBs,1188
 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/workspace_connection_handler.py,sha256=UO5uLeyPMT7HT8RWwwsDbck9nFNe5KQbsw7XG8yit0Y,2515
 promptflow_vectordb/tool/common_index_lookup_extensions/__init__.py,sha256=xhqpwJ_ZB7Lz959ivjcs74tPcbgA4EbSoLLDnPmmpQs,51
-promptflow_vectordb/tool/common_index_lookup_extensions/acs.py,sha256=hXPlC1DJDZS_5eJh4MS-Jvgt7PPIK_jeM3xEh_jHyw8,6209
-promptflow_vectordb/tool/common_index_lookup_extensions/utils.py,sha256=MJ5GO-pnxB_GVWQfqaVJdLnewA5x_idGtPipq7C8cgA,2417
-promptflow_vectordb/tool/common_index_lookup_utils/__init__.py,sha256=IbjeUTAy8-RXws_6EJfON6iu4us6nX4knubh22XRUBQ,656
-promptflow_vectordb/tool/common_index_lookup_utils/acs.py,sha256=2xPq_okL9L7M249G0OyNz57gqIWE_DhYSHSWuoIZjIQ,4040
-promptflow_vectordb/tool/common_index_lookup_utils/constants.py,sha256=8h4m0HpQ89yb893NMOZaH9bwGmh-rNJ_m6k2Kt8Yw4k,1007
+promptflow_vectordb/tool/common_index_lookup_extensions/acs.py,sha256=eRoWsl7Kielb1oMEevCP1th4xSwvJst7W4VSMjWG-9Q,6309
+promptflow_vectordb/tool/common_index_lookup_extensions/utils.py,sha256=4aENGN8RjpLh8_riKiHYquqSnREE5k4FA9et342hmH4,3581
+promptflow_vectordb/tool/common_index_lookup_utils/__init__.py,sha256=tobxQIbNNj1Uw7LpcE4fdqH-vyn8LodTpJ0D6vxJMtU,838
+promptflow_vectordb/tool/common_index_lookup_utils/acs.py,sha256=cIAUlnBsbgtWtZJoxYc2QSoD_wtuU4ko1eHV1m_TRrs,3298
+promptflow_vectordb/tool/common_index_lookup_utils/constants.py,sha256=F0YBXJHCcp92Ymb0lCdhw9QTSHgXVtvm8uA7NXL_W9U,1077
 promptflow_vectordb/tool/common_index_lookup_utils/embeddings.py,sha256=wjcW5elRF3AfwVyiUCstYVDgWnF1HRRK-wuDfmrosZI,6088
-promptflow_vectordb/tool/common_index_lookup_utils/index_types.py,sha256=IcBuYzA6A0bXlOOAyhdSpmAgUH5ZxBM6smd1JowdKMw,1819
+promptflow_vectordb/tool/common_index_lookup_utils/index_types.py,sha256=ArBboRIy93oUNHk2hwbpgDJKWEneUeHQWryQC-tk61Y,2426
 promptflow_vectordb/tool/common_index_lookup_utils/indices.py,sha256=cQwtBGCTUjDkF8DiuQayw8SpDL9HwiQ3LD2U1Gm6hjA,478
 promptflow_vectordb/tool/common_index_lookup_utils/logger.py,sha256=nhhOLVrp7oiYU-ECfvGTlzw_PdbLH4UkGwgFrTIXsLw,1840
-promptflow_vectordb/tool/common_index_lookup_utils/mapping.py,sha256=wEVgv0QtTgCMA8hOni3LsF5iGZls4SzpI7J3Wzviffw,13580
+promptflow_vectordb/tool/common_index_lookup_utils/mapping.py,sha256=QDHFPbnJL-ULXP_CLKl3OtEM1rF02rqISarUJzGhxd0,15945
 promptflow_vectordb/tool/common_index_lookup_utils/mlindex_client.py,sha256=pO9-S1z8Jq-7rxeW8JnOpkJ9dv_Ya2Zk29PlCaXdjnA,2005
+promptflow_vectordb/tool/common_index_lookup_utils/mongodb.py,sha256=9Beo8PtmU3_3y0S7Vx96xyGAPjdYUrOS1LLvqOsWt8s,3977
 promptflow_vectordb/tool/common_index_lookup_utils/pinecone.py,sha256=0qkcSctepwqwbaR_CRQPYLxZ_WJPLn9mVrRvqG30hvk,1937
 promptflow_vectordb/tool/common_index_lookup_utils/query_types.py,sha256=RodyiPIkup5Yg1NVu6RG4Q3jevytkJz3IEjCk2pFh3w,1814
 promptflow_vectordb/tool/common_index_lookup_utils/utils.py,sha256=en77dbsII8K9THtWysQ-wu2UKCP8Cpd1qb0PVLb45_g,2184
 promptflow_vectordb/tool/contracts/__init__.py,sha256=w2wEJZosUreNBtCotdkW9ZsBQVI-GmbWqpzjQGoeS_U,89
 promptflow_vectordb/tool/contracts/config.py,sha256=1d3wN20-uiMRoZ_xwf428cD9S4-ffS00__3VD7bQ75Q,5050
 promptflow_vectordb/tool/contracts/constants.py,sha256=CjBL2-ra0LzzXQY09wjl5TvDG5C3d99MLkUPXKPlaHA,230
 promptflow_vectordb/tool/contracts/ml_index_yaml_config.py,sha256=W0CJN4ybNT8d5MihSClzxCr6Fe7A06702_NqFF3Ppzs,1512
@@ -124,16 +125,16 @@
 promptflow_vectordb/tool/utils/logging.py,sha256=HGBxmKzEng5TtE9qjWcCezZr4WTRdfGh3lbkybVpqRo,1539
 promptflow_vectordb/tool/utils/pf_exception_helpers.py,sha256=s5GGRV3ic-KhP5LIn5xAetfsiuvCYfFcrpeaxdGB1XA,3616
 promptflow_vectordb/tool/utils/pf_runtime_utils.py,sha256=r9o1Aw5nY0GHEkmRVvwwWOBTknIABqUCe34UFvHxd-c,3372
 promptflow_vectordb/tool/utils/profiling.py,sha256=5DN0tSjChL6MfqN93f75xwBQWL4al1PlWBmWID189hc,946
 promptflow_vectordb/tool/utils/store_core_provider.py,sha256=Iz9k8cxja2cjAGgf6CKBq9F_wh4FfN_vxtVmkZzCDxM,1944
 promptflow_vectordb/tool/utils/workspace_connection_manager.py,sha256=mIYvNUqy5VunR20j0I8g7B2hej1X8q7lkTQIcpix-Wk,2549
 promptflow_vectordb/tool/utils/yaml_parser.py,sha256=Mw76QJV7fOCJmyw6JJkHZO4Fg3rSxWH129JhpAlWFIs,889
-promptflow_vectordb/tool/yamls/azure/common_index_lookup.yaml,sha256=ka_GzQjUjhG6SE_0W02fVpRe-5UMalPpaG3name-FP0,12054
+promptflow_vectordb/tool/yamls/azure/common_index_lookup.yaml,sha256=coDYHTqHaq5QAjEZiy9EKwiQs5RETrWSMHGzGgLstKE,17182
 promptflow_vectordb/tool/yamls/azure/vector_index_lookup.yaml,sha256=Ps4XNBDz17ZNAl4Lg8huFCNnGMfH3Z_0PtfyhFItQT4,457
 promptflow_vectordb/tool/yamls/shared/faiss_index_lookup.yaml,sha256=A3FcLLu0XxQkLywq4A8ijCBo6tqSbdgt6dWwNemWoAg,443
 promptflow_vectordb/tool/yamls/shared/vector_db_lookup.yaml,sha256=grYJamNVbr5pAZePdfXJENPv1UMxnTnWI2gHt_e6phs,1507
-promptflow_vectordb-0.2.8.dist-info/METADATA,sha256=mDR5K6sdypAI7IAWw4oIE_yGBDecVroeVVs_UM4122o,3019
-promptflow_vectordb-0.2.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-promptflow_vectordb-0.2.8.dist-info/entry_points.txt,sha256=U2bURx76LNRyrBkb-gksXN8hbaH1D4sMtrxcu8nzmDI,200
-promptflow_vectordb-0.2.8.dist-info/top_level.txt,sha256=AIbxh30bIFT76vitS0NSe96iRftM0tuVOo_HrZxRedw,20
-promptflow_vectordb-0.2.8.dist-info/RECORD,,
+promptflow_vectordb-0.2.9.dist-info/METADATA,sha256=ivOSAzHu07ZfWTSkVg8GD0MsXx4Omy2B9HL3o9QKaBY,3514
+promptflow_vectordb-0.2.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+promptflow_vectordb-0.2.9.dist-info/entry_points.txt,sha256=U2bURx76LNRyrBkb-gksXN8hbaH1D4sMtrxcu8nzmDI,200
+promptflow_vectordb-0.2.9.dist-info/top_level.txt,sha256=AIbxh30bIFT76vitS0NSe96iRftM0tuVOo_HrZxRedw,20
+promptflow_vectordb-0.2.9.dist-info/RECORD,,
```

