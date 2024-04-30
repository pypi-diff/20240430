# Comparing `tmp/opperai-0.3.4.tar.gz` & `tmp/opperai-0.4.0.tar.gz`

## Comparing `opperai-0.3.4.tar` & `opperai-0.4.0.tar`

### file list

```diff
@@ -1,84 +1,85 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 opperai-0.3.4/pytest.ini
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.3.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/__init__.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/_client.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/_http_clients.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/functions/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/functions/_async_functions.py
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/functions/_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/functions/decorator/__init__.py
--rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/functions/decorator/_decorator.py
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/functions/decorator/_schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/indexes/__init__.py
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/indexes/_async_indexes.py
--rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/indexes/_indexes.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/spans/__init__.py
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/spans/_async_spans.py
--rw-r--r--   0        0        0     4876 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/spans/_decorator.py
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/spans/_spans.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/types/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/types/exceptions.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/types/indexes.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/types/spans.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/types/validators.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/utils/__init__.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/conftest.py
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/test_async_functions.py
--rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/test_async_indexes.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/test_async_spans.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/test_decorator.py
--rw-r--r--   0        0        0     8184 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/test_functions.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/test_indexes.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/test_spans.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/test_trace_decorator.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/test_types.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml
--rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_id.yaml
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_path.yaml
--rw-r--r--   0        0        0     9714 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml
--rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_spans/test_save_feedback.yaml
--rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml
--rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml
--rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml
--rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml
--rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_get.yaml
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml
--rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml
--rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_upload_file.yaml
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 opperai-0.3.4/.gitignore
--rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 opperai-0.3.4/LICENSE
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 opperai-0.3.4/README.md
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 opperai-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 opperai-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 opperai-0.4.0/pytest.ini
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.4.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/__init__.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/_client.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/_http_clients.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/functions/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/functions/_async_functions.py
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/functions/_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/functions/decorator/__init__.py
+-rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/functions/decorator/_decorator.py
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/functions/decorator/_schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/indexes/__init__.py
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/indexes/_async_indexes.py
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/indexes/_indexes.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/spans/__init__.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/spans/_async_spans.py
+-rw-r--r--   0        0        0     4876 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/spans/_decorator.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/spans/_spans.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/types/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/types/exceptions.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/types/indexes.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/types/spans.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/types/validators.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 opperai-0.4.0/src/opperai/utils/__init__.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/test_async_functions.py
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/test_async_indexes.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/test_async_spans.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/test_decorator.py
+-rw-r--r--   0        0        0     8184 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/test_functions.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/test_indexes.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/test_spans.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/test_trace_decorator.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/test_types.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml
+-rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_id.yaml
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_path.yaml
+-rw-r--r--   0        0        0     9714 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml
+-rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_spans/test_save_feedback.yaml
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml
+-rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml
+-rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml
+-rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml
+-rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml
+-rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_get.yaml
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml
+-rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml
+-rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_upload_file.yaml
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 opperai-0.4.0/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 opperai-0.4.0/.gitignore
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 opperai-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 opperai-0.4.0/README.md
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 opperai-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 opperai-0.4.0/PKG-INFO
```

### Comparing `opperai-0.3.4/.github/workflows/publish.yml` & `opperai-0.4.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/src/opperai/_client.py` & `opperai-0.4.0/src/opperai/_client.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/src/opperai/_http_clients.py` & `opperai-0.4.0/src/opperai/_http_clients.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/src/opperai/functions/_async_functions.py` & `opperai-0.4.0/src/opperai/functions/_async_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/src/opperai/functions/_functions.py` & `opperai-0.4.0/src/opperai/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/src/opperai/functions/decorator/_decorator.py` & `opperai-0.4.0/src/opperai/functions/decorator/_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/src/opperai/functions/decorator/_schemas.py` & `opperai-0.4.0/src/opperai/functions/decorator/_schemas.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/src/opperai/indexes/_async_indexes.py` & `opperai-0.4.0/src/opperai/indexes/_async_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/src/opperai/indexes/_indexes.py` & `opperai-0.4.0/src/opperai/indexes/_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/src/opperai/spans/_async_spans.py` & `opperai-0.4.0/src/opperai/spans/_async_spans.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
+from typing import Any, Dict
 from uuid import UUID
 
 from opperai._http_clients import _async_http_client
-from opperai.types.spans import Span, SpanFeedback
 from opperai.types.exceptions import APIError
+from opperai.types.spans import Span, SpanMetric
 from opperai.utils import DateTimeEncoder
-from typing import Dict, Any
 
 
 class AsyncSpans:
     def __init__(self, http_client: _async_http_client):
         self.http_client = http_client
 
     async def create(self, span: Span, **kwargs) -> Span:
@@ -64,21 +64,21 @@
         if response.status_code != 200:
             raise APIError(
                 f"Failed to save examples for span {uuid} with status {response.status_code}"
             )
 
         return response.json()
 
-    async def save_feedback(
-        self, uuid: str, feedback: SpanFeedback, **kwargs
+    async def save_metric(
+        self, uuid: str, metric: SpanMetric, **kwargs
     ) -> Dict[str, Any]:
         response = await self.http_client.do_request(
             "POST",
-            f"/v1/spans/{uuid}/feedbacks",
-            json=feedback.model_dump(exclude_unset=True),
+            f"/v1/spans/{uuid}/metrics",
+            json=metric.model_dump(exclude_unset=True),
         )
         if response.status_code != 200:
             raise APIError(
-                f"Failed to add feedback for span {uuid} with status {response.status_code}"
+                f"Failed to add metric for span {uuid} with status {response.status_code}"
             )
 
         return response.json()
```

### Comparing `opperai-0.3.4/src/opperai/spans/_decorator.py` & `opperai-0.4.0/src/opperai/spans/_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/src/opperai/types/__init__.py` & `opperai-0.4.0/src/opperai/types/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ruff: noqa: F401
 from typing import Any, Dict, List, Optional, Union
 from uuid import UUID
-from .spans import SpanFeedback
 
 from pydantic import BaseModel, ConfigDict, Field
 
+from .spans import SpanMetric
 from .validators import validate_id_xor_path
 
 
 class Message(BaseModel):
     role: str
     content: str
```

### Comparing `opperai-0.3.4/src/opperai/types/indexes.py` & `opperai-0.4.0/src/opperai/types/indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/src/opperai/types/spans.py` & `opperai-0.4.0/src/opperai/types/spans.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,11 +16,11 @@
     end_time: Optional[datetime] = None
     error: Optional[str] = None
     meta: Optional[dict] = None
     evaluations: Optional[dict] = None
     score: Optional[int] = None
 
 
-class SpanFeedback(BaseModel):
+class SpanMetric(BaseModel):
     dimension: Optional[str] = None
     score: Optional[float] = Field(None, ge=0, le=1)
     comment: Optional[str] = None
```

### Comparing `opperai-0.3.4/src/opperai/types/validators.py` & `opperai-0.4.0/src/opperai/types/validators.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/src/opperai/utils/__init__.py` & `opperai-0.4.0/src/opperai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/conftest.py` & `opperai-0.4.0/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import re
-import vcr
+
 import pytest
+import vcr
 from opperai import AsyncClient, Client
 
 
 @pytest.fixture(scope="module")
 def aclient() -> AsyncClient:
     yield AsyncClient()
 
@@ -30,17 +31,14 @@
     file_name = os.path.splitext(os.path.basename(module_file))[0]
 
     cassette_name = f"{file_name}/{test_name}.yaml"
 
     my_vcr = vcr.VCR(
         cassette_library_dir="tests/fixtures/vcr_cassettes",
         path_transformer=vcr.VCR.ensure_suffix(".yaml"),
-        filter_headers=[
-            "x-opper-api-key",
-            "host",
-        ],
+        filter_headers=["x-opper-api-key", "host", "accept-encoding", "user-agent"],
     )
     my_vcr.register_matcher("uri_matcher", uri_matcher)
     my_vcr.match_on = ["method", "body", "headers", "uri_matcher"]
 
     with my_vcr.use_cassette(cassette_name):
         yield
```

### Comparing `opperai-0.3.4/tests/test_async_functions.py` & `opperai-0.4.0/tests/test_async_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/test_async_indexes.py` & `opperai-0.4.0/tests/test_async_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/test_async_spans.py` & `opperai-0.4.0/tests/test_async_spans.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from contextlib import asynccontextmanager
 from datetime import datetime
+
 import pytest
-from opperai.types.spans import Span, SpanFeedback
 from opperai import AsyncClient
-from contextlib import asynccontextmanager
+from opperai.types.spans import Span, SpanMetric
 
 
 @asynccontextmanager
 async def span(desc: Span, _client: AsyncClient):
     _span = await _client.spans.create(desc)
     try:
         yield _span
@@ -58,21 +59,21 @@
     )
 
     assert await aclient.spans.delete(child_span.uuid)
     assert await aclient.spans.delete(root_span.uuid)
 
 
 @pytest.mark.asyncio(scope="module")
-async def test_save_feedback(aclient: AsyncClient, vcr_cassette):
+async def test_save_metric(aclient: AsyncClient, vcr_cassette):
     async with span(
         Span(
             uuid="bcf1b3b4-0b3b-4b3b-8b3b-0b3b4b3b4133",
             project="project",
             name="name",
             input="input",
             start_time=datetime(2021, 1, 1, 0, 0, 0, 0),
         ),
         aclient,
     ) as _span:
-        await aclient.spans.save_feedback(
-            _span.uuid, SpanFeedback(dimension="dim", score=0.5, comment="comment")
+        await aclient.spans.save_metric(
+            _span.uuid, SpanMetric(dimension="dim", score=0.5, comment="comment")
         )
```

### Comparing `opperai-0.3.4/tests/test_decorator.py` & `opperai-0.4.0/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/test_functions.py` & `opperai-0.4.0/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/test_indexes.py` & `opperai-0.4.0/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/test_spans.py` & `opperai-0.4.0/tests/test_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/test_trace_decorator.py` & `opperai-0.4.0/tests/test_trace_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/test_types.py` & `opperai-0.4.0/tests/test_types.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
+from opperai.types import SpanMetric, validate_id_xor_path
 from pydantic import ValidationError
-from opperai.types import validate_id_xor_path, SpanFeedback
 
 
 def test_id_xor_path():
     @validate_id_xor_path
     def test_function(id=None, path=None):
         return id, path
 
@@ -19,14 +19,14 @@
         test_function()
 
     with pytest.raises(ValueError):
         test_function(id=1, path="test", other="other")
 
 
 def test_feedback_score_in_range():
-    assert SpanFeedback(score=0.5).score == 0.5
-    assert SpanFeedback(score=0).score == 0
-    assert SpanFeedback(score=1).score == 1
+    assert SpanMetric(score=0.5).score == 0.5
+    assert SpanMetric(score=0).score == 0
+    assert SpanMetric(score=1).score == 1
     with pytest.raises(ValidationError):
-        SpanFeedback(score=1.1)
+        SpanMetric(score=1.1)
     with pytest.raises(ValidationError):
-        SpanFeedback(score=-0.1)
+        SpanMetric(score=-0.1)
```

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_id.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_path.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_spans/test_save_feedback.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_async_spans/test_save_feedback.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_get.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_get.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_upload_file.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_indexes/test_upload_file.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml` & `opperai-0.4.0/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/LICENSE` & `opperai-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opperai-0.3.4/README.md` & `opperai-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -115,9 +115,10 @@
 ```
 
 ## Configuration
 
 ### Environment variable
 
 The `OPPER_API_KEY` environment variable is read by the SDK if no `api_key` is provided to the `Client` object. 
+`OPPER_PROJECT` is attached to traces and can be used for filtering in the Opper UI.
 
 When using the `fn` decorator the SDK client is automatically initialized with the `OPPER_API_KEY` environment variable.
```

### Comparing `opperai-0.3.4/pyproject.toml` & `opperai-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "opperai"
-version = "0.3.4"
+version = "0.4.0"
 description = "Opper Python client"
 authors = [
   {name = "Opper", email = "opper@opper.ai"},
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `opperai-0.3.4/PKG-INFO` & `opperai-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: opperai
-Version: 0.3.4
+Version: 0.4.0
 Summary: Opper Python client
 Project-URL: Homepage, https://opper.ai
 Project-URL: Documentation, https://docs.opper.ai
 Project-URL: Platform, https://platform.opper.ai
 Author-email: Opper <opper@opper.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -138,9 +138,10 @@
 ```
 
 ## Configuration
 
 ### Environment variable
 
 The `OPPER_API_KEY` environment variable is read by the SDK if no `api_key` is provided to the `Client` object. 
+`OPPER_PROJECT` is attached to traces and can be used for filtering in the Opper UI.
 
 When using the `fn` decorator the SDK client is automatically initialized with the `OPPER_API_KEY` environment variable.
```

