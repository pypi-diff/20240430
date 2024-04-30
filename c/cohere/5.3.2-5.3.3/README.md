# Comparing `tmp/cohere-5.3.2.tar.gz` & `tmp/cohere-5.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-5.3.2.tar", max compression
+gzip compressed data, was "cohere-5.3.3.tar", max compression
```

## Comparing `cohere-5.3.2.tar` & `cohere-5.3.3.tar`

### file list

```diff
@@ -1,176 +1,176 @@
--rw-r--r--   0        0        0     1062 2024-04-17 16:48:22.021336 cohere-5.3.2/LICENSE
--rw-r--r--   0        0        0     2359 2024-04-17 16:48:22.021336 cohere-5.3.2/README.md
--rw-r--r--   0        0        0      700 2024-04-17 16:48:22.025336 cohere-5.3.2/pyproject.toml
--rw-r--r--   0        0        0     8012 2024-04-17 16:48:22.025336 cohere-5.3.2/src/cohere/__init__.py
--rw-r--r--   0        0        0   202912 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/base_client.py
--rw-r--r--   0        0        0    19635 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/client.py
--rw-r--r--   0        0        0       22 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/config.py
--rw-r--r--   0        0        0       65 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/connectors/__init__.py
--rw-r--r--   0        0        0    50199 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/connectors/client.py
--rw-r--r--   0        0        0     1006 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/core/api_error.py
--rw-r--r--   0        0        0     2226 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/core/request_options.py
--rw-r--r--   0        0        0     7123 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/core/unchecked_base_model.py
--rw-r--r--   0        0        0      411 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/datasets/__init__.py
--rw-r--r--   0        0        0    34874 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/datasets/client.py
--rw-r--r--   0        0        0      565 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/datasets/types/__init__.py
--rw-r--r--   0        0        0     1002 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/datasets/types/datasets_create_response.py
--rw-r--r--   0        0        0     1398 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/datasets/types/datasets_create_response_dataset_parts.py
--rw-r--r--   0        0        0      959 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/datasets/types/datasets_get_response.py
--rw-r--r--   0        0        0     1057 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/datasets/types/datasets_get_usage_response.py
--rw-r--r--   0        0        0      998 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/datasets/types/datasets_list_response.py
--rw-r--r--   0        0        0      159 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/embed_jobs/__init__.py
--rw-r--r--   0        0        0    31599 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/embed_jobs/client.py
--rw-r--r--   0        0        0      187 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/embed_jobs/types/__init__.py
--rw-r--r--   0        0        0      169 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/embed_jobs/types/create_embed_job_request_truncate.py
--rw-r--r--   0        0        0      159 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/environment.py
--rw-r--r--   0        0        0      617 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/errors/bad_request_error.py
--rw-r--r--   0        0        0      247 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/errors/forbidden_error.py
--rw-r--r--   0        0        0      252 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/errors/internal_server_error.py
--rw-r--r--   0        0        0      246 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/errors/not_found_error.py
--rw-r--r--   0        0        0      290 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/errors/service_unavailable_error.py
--rw-r--r--   0        0        0      253 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      284 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/errors/unauthorized_error.py
--rw-r--r--   0        0        0      953 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/__init__.py
--rw-r--r--   0        0        0    62127 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/client.py
--rw-r--r--   0        0        0      905 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/finetuning/__init__.py
--rw-r--r--   0        0        0     1343 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/finetuning/types/__init__.py
--rw-r--r--   0        0        0     1475 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/finetuning/types/base_model.py
--rw-r--r--   0        0        0      305 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/finetuning/types/base_type.py
--rw-r--r--   0        0        0     1175 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py
--rw-r--r--   0        0        0      140 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/finetuning/types/delete_finetuned_model_response.py
--rw-r--r--   0        0        0     1083 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/finetuning/types/error.py
--rw-r--r--   0        0        0     1400 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/finetuning/types/event.py
--rw-r--r--   0        0        0     2357 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/finetuning/types/finetuned_model.py
--rw-r--r--   0        0        0     1171 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py
--rw-r--r--   0        0        0     1823 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/finetuning/types/hyperparameters.py
--rw-r--r--   0        0        0     1489 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/finetuning/types/list_events_response.py
--rw-r--r--   0        0        0     1532 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py
--rw-r--r--   0        0        0     1463 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py
--rw-r--r--   0        0        0     1577 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/finetuning/types/settings.py
--rw-r--r--   0        0        0      402 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/finetuning/types/status.py
--rw-r--r--   0        0        0      193 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/finetuning/types/strategy.py
--rw-r--r--   0        0        0     1390 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/finetuning/types/training_step_metrics.py
--rw-r--r--   0        0        0     1177 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py
--rw-r--r--   0        0        0      811 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/manually_maintained/cache.py
--rw-r--r--   0        0        0     1948 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/manually_maintained/tokenizers.py
--rw-r--r--   0        0        0       65 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/models/__init__.py
--rw-r--r--   0        0        0    13673 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/models/client.py
--rw-r--r--   0        0        0      730 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/overrides.py
--rw-r--r--   0        0        0        0 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/py.typed
--rw-r--r--   0        0        0    10202 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/__init__.py
--rw-r--r--   0        0        0     1260 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/api_meta.py
--rw-r--r--   0        0        0     1011 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/api_meta_api_version.py
--rw-r--r--   0        0        0     1434 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/api_meta_billed_units.py
--rw-r--r--   0        0        0     1177 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/api_meta_tokens.py
--rw-r--r--   0        0        0      168 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/auth_token_type.py
--rw-r--r--   0        0        0     1929 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_citation.py
--rw-r--r--   0        0        0     1127 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_citation_generation_event.py
--rw-r--r--   0        0        0     1861 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_connector.py
--rw-r--r--   0        0        0     1297 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_data_metrics.py
--rw-r--r--   0        0        0      117 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_document.py
--rw-r--r--   0        0        0     1644 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_message.py
--rw-r--r--   0        0        0      168 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_message_role.py
--rw-r--r--   0        0        0      170 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_request_citation_quality.py
--rw-r--r--   0        0        0     1708 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_request_connectors_search_options.py
--rw-r--r--   0        0        0      189 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_request_prompt_truncation.py
--rw-r--r--   0        0        0     1011 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_request_tool_results_item.py
--rw-r--r--   0        0        0     1180 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_search_queries_generation_event.py
--rw-r--r--   0        0        0     1247 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_search_query.py
--rw-r--r--   0        0        0     1653 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_search_result.py
--rw-r--r--   0        0        0     1055 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_search_result_connector.py
--rw-r--r--   0        0        0     1417 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_search_results_event.py
--rw-r--r--   0        0        0     1861 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_stream_end_event.py
--rw-r--r--   0        0        0      225 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_stream_end_event_finish_reason.py
--rw-r--r--   0        0        0      893 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_stream_event.py
--rw-r--r--   0        0        0      176 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_stream_request_citation_quality.py
--rw-r--r--   0        0        0     1714 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_stream_request_connectors_search_options.py
--rw-r--r--   0        0        0      195 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_stream_request_prompt_truncation.py
--rw-r--r--   0        0        0     1017 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_stream_request_tool_results_item.py
--rw-r--r--   0        0        0     1102 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_stream_start_event.py
--rw-r--r--   0        0        0     1068 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_text_generation_event.py
--rw-r--r--   0        0        0     1040 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/chat_tool_calls_generation_event.py
--rw-r--r--   0        0        0     1004 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/classify_data_metrics.py
--rw-r--r--   0        0        0      971 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/classify_example.py
--rw-r--r--   0        0        0      171 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/classify_request_truncate.py
--rw-r--r--   0        0        0     1137 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/classify_response.py
--rw-r--r--   0        0        0     2560 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/classify_response_classifications_item.py
--rw-r--r--   0        0        0      214 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/classify_response_classifications_item_classification_type.py
--rw-r--r--   0        0        0      971 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/classify_response_classifications_item_labels_value.py
--rw-r--r--   0        0        0      220 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/compatible_endpoint.py
--rw-r--r--   0        0        0     3383 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/connector.py
--rw-r--r--   0        0        0      163 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/connector_auth_status.py
--rw-r--r--   0        0        0     1660 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/connector_o_auth.py
--rw-r--r--   0        0        0     1725 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/create_connector_o_auth.py
--rw-r--r--   0        0        0      960 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/create_connector_response.py
--rw-r--r--   0        0        0     1195 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/create_connector_service_auth.py
--rw-r--r--   0        0        0     1047 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/create_embed_job_response.py
--rw-r--r--   0        0        0     2209 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/dataset.py
--rw-r--r--   0        0        0     1648 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/dataset_part.py
--rw-r--r--   0        0        0      471 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/dataset_type.py
--rw-r--r--   0        0        0      222 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/dataset_validation_status.py
--rw-r--r--   0        0        0      135 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/delete_connector_response.py
--rw-r--r--   0        0        0     1068 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/detokenize_response.py
--rw-r--r--   0        0        0     1416 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/embed_by_type_response.py
--rw-r--r--   0        0        0     2271 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/embed_by_type_response_embeddings.py
--rw-r--r--   0        0        0     1364 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/embed_floats_response.py
--rw-r--r--   0        0        0      211 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/embed_input_type.py
--rw-r--r--   0        0        0     1864 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/embed_job.py
--rw-r--r--   0        0        0      201 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/embed_job_status.py
--rw-r--r--   0        0        0      156 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/embed_job_truncate.py
--rw-r--r--   0        0        0      168 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/embed_request_truncate.py
--rw-r--r--   0        0        0     1057 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/embed_response.py
--rw-r--r--   0        0        0      184 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/embedding_type.py
--rw-r--r--   0        0        0     1735 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/finetune_dataset_metrics.py
--rw-r--r--   0        0        0      222 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/finish_reason.py
--rw-r--r--   0        0        0      185 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/generate_request_return_likelihoods.py
--rw-r--r--   0        0        0      171 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/generate_request_truncate.py
--rw-r--r--   0        0        0     1197 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/generate_stream_end.py
--rw-r--r--   0        0        0     1101 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/generate_stream_end_response.py
--rw-r--r--   0        0        0     1311 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/generate_stream_error.py
--rw-r--r--   0        0        0      897 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/generate_stream_event.py
--rw-r--r--   0        0        0      191 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/generate_stream_request_return_likelihoods.py
--rw-r--r--   0        0        0      177 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/generate_stream_request_truncate.py
--rw-r--r--   0        0        0     1312 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/generate_stream_text.py
--rw-r--r--   0        0        0     1456 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/generate_streamed_response.py
--rw-r--r--   0        0        0     1254 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/generation.py
--rw-r--r--   0        0        0      957 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/get_connector_response.py
--rw-r--r--   0        0        0     2150 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/get_model_response.py
--rw-r--r--   0        0        0     1256 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/label_metric.py
--rw-r--r--   0        0        0     1095 2024-04-17 16:48:22.029336 cohere-5.3.2/src/cohere/types/list_connectors_response.py
--rw-r--r--   0        0        0      993 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/list_embed_job_response.py
--rw-r--r--   0        0        0     1187 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/list_models_response.py
--rw-r--r--   0        0        0     1024 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/metrics.py
--rw-r--r--   0        0        0     2774 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/non_streamed_chat_response.py
--rw-r--r--   0        0        0     1080 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/o_auth_authorize_response.py
--rw-r--r--   0        0        0      974 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/parse_info.py
--rw-r--r--   0        0        0      239 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/rerank_request_documents_item.py
--rw-r--r--   0        0        0     1001 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/rerank_request_documents_item_text.py
--rw-r--r--   0        0        0     1200 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/rerank_response.py
--rw-r--r--   0        0        0     1342 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/rerank_response_results_item.py
--rw-r--r--   0        0        0     1056 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/rerank_response_results_item_document.py
--rw-r--r--   0        0        0     1818 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/reranker_data_metrics.py
--rw-r--r--   0        0        0     1819 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/single_generation.py
--rw-r--r--   0        0        0     1248 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/single_generation_in_stream.py
--rw-r--r--   0        0        0      952 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/single_generation_token_likelihoods_item.py
--rw-r--r--   0        0        0     3157 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/streamed_chat_response.py
--rw-r--r--   0        0        0      179 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/summarize_request_extractiveness.py
--rw-r--r--   0        0        0      170 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/summarize_request_format.py
--rw-r--r--   0        0        0      173 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/summarize_request_length.py
--rw-r--r--   0        0        0     1201 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/summarize_response.py
--rw-r--r--   0        0        0     1127 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/tokenize_response.py
--rw-r--r--   0        0        0     1928 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/tool.py
--rw-r--r--   0        0        0     1221 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/tool_call.py
--rw-r--r--   0        0        0     1331 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/tool_parameter_definitions_value.py
--rw-r--r--   0        0        0      960 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/types/update_connector_response.py
--rw-r--r--   0        0        0    10036 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/utils.py
--rw-r--r--   0        0        0       74 2024-04-17 16:48:22.033336 cohere-5.3.2/src/cohere/version.py
--rw-r--r--   0        0        0     3064 1970-01-01 00:00:00.000000 cohere-5.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-23 13:36:39.911520 cohere-5.3.3/LICENSE
+-rw-r--r--   0        0        0     2359 2024-04-23 13:36:39.911520 cohere-5.3.3/README.md
+-rw-r--r--   0        0        0      698 2024-04-23 13:36:39.919520 cohere-5.3.3/pyproject.toml
+-rw-r--r--   0        0        0     8012 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/__init__.py
+-rw-r--r--   0        0        0   206571 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/base_client.py
+-rw-r--r--   0        0        0    19635 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/client.py
+-rw-r--r--   0        0        0       22 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/config.py
+-rw-r--r--   0        0        0       65 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/connectors/__init__.py
+-rw-r--r--   0        0        0    50199 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/connectors/client.py
+-rw-r--r--   0        0        0     1006 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/core/api_error.py
+-rw-r--r--   0        0        0     2226 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/core/request_options.py
+-rw-r--r--   0        0        0     7123 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/core/unchecked_base_model.py
+-rw-r--r--   0        0        0      411 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/datasets/__init__.py
+-rw-r--r--   0        0        0    35448 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/datasets/client.py
+-rw-r--r--   0        0        0      565 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/datasets/types/__init__.py
+-rw-r--r--   0        0        0     1002 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/datasets/types/datasets_create_response.py
+-rw-r--r--   0        0        0     1398 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/datasets/types/datasets_create_response_dataset_parts.py
+-rw-r--r--   0        0        0      959 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/datasets/types/datasets_get_response.py
+-rw-r--r--   0        0        0     1057 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/datasets/types/datasets_get_usage_response.py
+-rw-r--r--   0        0        0      998 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/datasets/types/datasets_list_response.py
+-rw-r--r--   0        0        0      159 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/embed_jobs/__init__.py
+-rw-r--r--   0        0        0    31599 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/embed_jobs/client.py
+-rw-r--r--   0        0        0      187 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/embed_jobs/types/__init__.py
+-rw-r--r--   0        0        0      169 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/embed_jobs/types/create_embed_job_request_truncate.py
+-rw-r--r--   0        0        0      159 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/environment.py
+-rw-r--r--   0        0        0      617 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/errors/bad_request_error.py
+-rw-r--r--   0        0        0      247 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/errors/forbidden_error.py
+-rw-r--r--   0        0        0      252 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/errors/internal_server_error.py
+-rw-r--r--   0        0        0      246 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/errors/not_found_error.py
+-rw-r--r--   0        0        0      290 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/errors/service_unavailable_error.py
+-rw-r--r--   0        0        0      253 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      284 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      953 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/__init__.py
+-rw-r--r--   0        0        0    62127 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/client.py
+-rw-r--r--   0        0        0      905 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/finetuning/__init__.py
+-rw-r--r--   0        0        0     1343 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/finetuning/types/__init__.py
+-rw-r--r--   0        0        0     1475 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/finetuning/types/base_model.py
+-rw-r--r--   0        0        0      305 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/finetuning/types/base_type.py
+-rw-r--r--   0        0        0     1175 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py
+-rw-r--r--   0        0        0      140 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/finetuning/types/delete_finetuned_model_response.py
+-rw-r--r--   0        0        0     1083 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/finetuning/types/error.py
+-rw-r--r--   0        0        0     1400 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/finetuning/types/event.py
+-rw-r--r--   0        0        0     2357 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/finetuning/types/finetuned_model.py
+-rw-r--r--   0        0        0     1171 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py
+-rw-r--r--   0        0        0     1823 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/finetuning/types/hyperparameters.py
+-rw-r--r--   0        0        0     1489 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/finetuning/types/list_events_response.py
+-rw-r--r--   0        0        0     1532 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py
+-rw-r--r--   0        0        0     1463 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py
+-rw-r--r--   0        0        0     1577 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/finetuning/types/settings.py
+-rw-r--r--   0        0        0      402 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/finetuning/types/status.py
+-rw-r--r--   0        0        0      193 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/finetuning/types/strategy.py
+-rw-r--r--   0        0        0     1390 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/finetuning/types/training_step_metrics.py
+-rw-r--r--   0        0        0     1177 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py
+-rw-r--r--   0        0        0      811 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/manually_maintained/cache.py
+-rw-r--r--   0        0        0     1948 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/manually_maintained/tokenizers.py
+-rw-r--r--   0        0        0       65 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/models/__init__.py
+-rw-r--r--   0        0        0    13673 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/models/client.py
+-rw-r--r--   0        0        0      730 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/overrides.py
+-rw-r--r--   0        0        0        0 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/py.typed
+-rw-r--r--   0        0        0    10202 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/__init__.py
+-rw-r--r--   0        0        0     1260 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/api_meta.py
+-rw-r--r--   0        0        0     1011 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/api_meta_api_version.py
+-rw-r--r--   0        0        0     1434 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/api_meta_billed_units.py
+-rw-r--r--   0        0        0     1177 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/api_meta_tokens.py
+-rw-r--r--   0        0        0      168 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/auth_token_type.py
+-rw-r--r--   0        0        0     1929 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_citation.py
+-rw-r--r--   0        0        0     1127 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_citation_generation_event.py
+-rw-r--r--   0        0        0     1861 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_connector.py
+-rw-r--r--   0        0        0     1297 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_data_metrics.py
+-rw-r--r--   0        0        0      117 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_document.py
+-rw-r--r--   0        0        0     1644 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_message.py
+-rw-r--r--   0        0        0      168 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_message_role.py
+-rw-r--r--   0        0        0      170 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_request_citation_quality.py
+-rw-r--r--   0        0        0     1708 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_request_connectors_search_options.py
+-rw-r--r--   0        0        0      189 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_request_prompt_truncation.py
+-rw-r--r--   0        0        0     1011 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_request_tool_results_item.py
+-rw-r--r--   0        0        0     1180 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_search_queries_generation_event.py
+-rw-r--r--   0        0        0     1247 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_search_query.py
+-rw-r--r--   0        0        0     1653 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_search_result.py
+-rw-r--r--   0        0        0     1055 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_search_result_connector.py
+-rw-r--r--   0        0        0     1417 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_search_results_event.py
+-rw-r--r--   0        0        0     1861 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_stream_end_event.py
+-rw-r--r--   0        0        0      225 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_stream_end_event_finish_reason.py
+-rw-r--r--   0        0        0      893 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_stream_event.py
+-rw-r--r--   0        0        0      176 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_stream_request_citation_quality.py
+-rw-r--r--   0        0        0     1714 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_stream_request_connectors_search_options.py
+-rw-r--r--   0        0        0      195 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_stream_request_prompt_truncation.py
+-rw-r--r--   0        0        0     1017 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_stream_request_tool_results_item.py
+-rw-r--r--   0        0        0     1102 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_stream_start_event.py
+-rw-r--r--   0        0        0     1068 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_text_generation_event.py
+-rw-r--r--   0        0        0     1040 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/chat_tool_calls_generation_event.py
+-rw-r--r--   0        0        0     1004 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/classify_data_metrics.py
+-rw-r--r--   0        0        0      971 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/classify_example.py
+-rw-r--r--   0        0        0      171 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/classify_request_truncate.py
+-rw-r--r--   0        0        0     1137 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/classify_response.py
+-rw-r--r--   0        0        0     2560 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/classify_response_classifications_item.py
+-rw-r--r--   0        0        0      214 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/classify_response_classifications_item_classification_type.py
+-rw-r--r--   0        0        0      971 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/classify_response_classifications_item_labels_value.py
+-rw-r--r--   0        0        0      220 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/compatible_endpoint.py
+-rw-r--r--   0        0        0     3383 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/connector.py
+-rw-r--r--   0        0        0      163 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/connector_auth_status.py
+-rw-r--r--   0        0        0     1660 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/connector_o_auth.py
+-rw-r--r--   0        0        0     1725 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/create_connector_o_auth.py
+-rw-r--r--   0        0        0      960 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/create_connector_response.py
+-rw-r--r--   0        0        0     1195 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/create_connector_service_auth.py
+-rw-r--r--   0        0        0     1047 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/create_embed_job_response.py
+-rw-r--r--   0        0        0     2209 2024-04-23 13:36:39.919520 cohere-5.3.3/src/cohere/types/dataset.py
+-rw-r--r--   0        0        0     1648 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/dataset_part.py
+-rw-r--r--   0        0        0      471 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/dataset_type.py
+-rw-r--r--   0        0        0      222 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/dataset_validation_status.py
+-rw-r--r--   0        0        0      135 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/delete_connector_response.py
+-rw-r--r--   0        0        0     1068 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/detokenize_response.py
+-rw-r--r--   0        0        0     1416 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/embed_by_type_response.py
+-rw-r--r--   0        0        0     2271 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/embed_by_type_response_embeddings.py
+-rw-r--r--   0        0        0     1364 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/embed_floats_response.py
+-rw-r--r--   0        0        0      211 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/embed_input_type.py
+-rw-r--r--   0        0        0     1864 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/embed_job.py
+-rw-r--r--   0        0        0      201 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/embed_job_status.py
+-rw-r--r--   0        0        0      156 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/embed_job_truncate.py
+-rw-r--r--   0        0        0      168 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/embed_request_truncate.py
+-rw-r--r--   0        0        0     1057 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/embed_response.py
+-rw-r--r--   0        0        0      184 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/embedding_type.py
+-rw-r--r--   0        0        0     1735 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/finetune_dataset_metrics.py
+-rw-r--r--   0        0        0      222 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/finish_reason.py
+-rw-r--r--   0        0        0      185 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/generate_request_return_likelihoods.py
+-rw-r--r--   0        0        0      171 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/generate_request_truncate.py
+-rw-r--r--   0        0        0     1197 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/generate_stream_end.py
+-rw-r--r--   0        0        0     1101 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/generate_stream_end_response.py
+-rw-r--r--   0        0        0     1311 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/generate_stream_error.py
+-rw-r--r--   0        0        0      897 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/generate_stream_event.py
+-rw-r--r--   0        0        0      191 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/generate_stream_request_return_likelihoods.py
+-rw-r--r--   0        0        0      177 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/generate_stream_request_truncate.py
+-rw-r--r--   0        0        0     1312 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/generate_stream_text.py
+-rw-r--r--   0        0        0     1456 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/generate_streamed_response.py
+-rw-r--r--   0        0        0     1254 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/generation.py
+-rw-r--r--   0        0        0      957 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/get_connector_response.py
+-rw-r--r--   0        0        0     2150 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/get_model_response.py
+-rw-r--r--   0        0        0     1256 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/label_metric.py
+-rw-r--r--   0        0        0     1095 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/list_connectors_response.py
+-rw-r--r--   0        0        0      993 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/list_embed_job_response.py
+-rw-r--r--   0        0        0     1187 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/list_models_response.py
+-rw-r--r--   0        0        0     1024 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/metrics.py
+-rw-r--r--   0        0        0     2953 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/non_streamed_chat_response.py
+-rw-r--r--   0        0        0     1080 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/o_auth_authorize_response.py
+-rw-r--r--   0        0        0      974 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/parse_info.py
+-rw-r--r--   0        0        0      239 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/rerank_request_documents_item.py
+-rw-r--r--   0        0        0     1001 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/rerank_request_documents_item_text.py
+-rw-r--r--   0        0        0     1200 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/rerank_response.py
+-rw-r--r--   0        0        0     1909 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/rerank_response_results_item.py
+-rw-r--r--   0        0        0     1136 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/rerank_response_results_item_document.py
+-rw-r--r--   0        0        0     1818 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/reranker_data_metrics.py
+-rw-r--r--   0        0        0     1819 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/single_generation.py
+-rw-r--r--   0        0        0     1248 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/single_generation_in_stream.py
+-rw-r--r--   0        0        0      952 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/single_generation_token_likelihoods_item.py
+-rw-r--r--   0        0        0     3157 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/streamed_chat_response.py
+-rw-r--r--   0        0        0      179 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/summarize_request_extractiveness.py
+-rw-r--r--   0        0        0      170 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/summarize_request_format.py
+-rw-r--r--   0        0        0      173 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/summarize_request_length.py
+-rw-r--r--   0        0        0     1201 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/summarize_response.py
+-rw-r--r--   0        0        0     1127 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/tokenize_response.py
+-rw-r--r--   0        0        0     1928 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/tool.py
+-rw-r--r--   0        0        0     1221 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/tool_call.py
+-rw-r--r--   0        0        0     1331 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/tool_parameter_definitions_value.py
+-rw-r--r--   0        0        0      960 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/types/update_connector_response.py
+-rw-r--r--   0        0        0    10036 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/utils.py
+-rw-r--r--   0        0        0       74 2024-04-23 13:36:39.923520 cohere-5.3.3/src/cohere/version.py
+-rw-r--r--   0        0        0     3060 1970-01-01 00:00:00.000000 cohere-5.3.3/PKG-INFO
```

### Comparing `cohere-5.3.2/LICENSE` & `cohere-5.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/README.md` & `cohere-5.3.3/README.md`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/pyproject.toml` & `cohere-5.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "cohere"
-version = "5.3.2"
+version = "5.3.3"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "cohere", from = "src"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 fastavro = "^1.9.4"
 httpx = ">=0.21.2"
 httpx-sse = "^0.4.0"
 pydantic = ">= 1.9.2"
 requests = "^2.0.0"
-tokenizers = "^0.15.2"
+tokenizers = "^0.19"
 types-requests = "^2.0.0"
 typing_extensions = ">= 4.0.0"
 
 [tool.poetry.dev-dependencies]
 mypy = "^1.8.0"
 pytest = "^7.4.0"
 pytest-asyncio = "^0.23.5"
```

### Comparing `cohere-5.3.2/src/cohere/__init__.py` & `cohere-5.3.3/src/cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/base_client.py` & `cohere-5.3.3/src/cohere/base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,18 @@
 from .errors.internal_server_error import InternalServerError
 from .errors.too_many_requests_error import TooManyRequestsError
 from .finetuning.client import AsyncFinetuningClient, FinetuningClient
 from .models.client import AsyncModelsClient, ModelsClient
 from .types.chat_connector import ChatConnector
 from .types.chat_document import ChatDocument
 from .types.chat_message import ChatMessage
+from .types.chat_request_citation_quality import ChatRequestCitationQuality
 from .types.chat_request_prompt_truncation import ChatRequestPromptTruncation
 from .types.chat_request_tool_results_item import ChatRequestToolResultsItem
+from .types.chat_stream_request_citation_quality import ChatStreamRequestCitationQuality
 from .types.chat_stream_request_prompt_truncation import ChatStreamRequestPromptTruncation
 from .types.chat_stream_request_tool_results_item import ChatStreamRequestToolResultsItem
 from .types.classify_example import ClassifyExample
 from .types.classify_request_truncate import ClassifyRequestTruncate
 from .types.classify_response import ClassifyResponse
 from .types.detokenize_response import DetokenizeResponse
 from .types.embed_input_type import EmbedInputType
@@ -128,36 +130,38 @@
         preamble: typing.Optional[str] = OMIT,
         chat_history: typing.Optional[typing.Sequence[ChatMessage]] = OMIT,
         conversation_id: typing.Optional[str] = OMIT,
         prompt_truncation: typing.Optional[ChatStreamRequestPromptTruncation] = OMIT,
         connectors: typing.Optional[typing.Sequence[ChatConnector]] = OMIT,
         search_queries_only: typing.Optional[bool] = OMIT,
         documents: typing.Optional[typing.Sequence[ChatDocument]] = OMIT,
+        citation_quality: typing.Optional[ChatStreamRequestCitationQuality] = OMIT,
         temperature: typing.Optional[float] = OMIT,
         max_tokens: typing.Optional[int] = OMIT,
         max_input_tokens: typing.Optional[int] = OMIT,
         k: typing.Optional[int] = OMIT,
         p: typing.Optional[float] = OMIT,
         seed: typing.Optional[float] = OMIT,
         stop_sequences: typing.Optional[typing.Sequence[str]] = OMIT,
         frequency_penalty: typing.Optional[float] = OMIT,
         presence_penalty: typing.Optional[float] = OMIT,
         raw_prompting: typing.Optional[bool] = OMIT,
+        return_prompt: typing.Optional[bool] = OMIT,
         tools: typing.Optional[typing.Sequence[Tool]] = OMIT,
         tool_results: typing.Optional[typing.Sequence[ChatStreamRequestToolResultsItem]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Iterator[StreamedChatResponse]:
         """
         Generates a text response to a user message.
         To learn how to use Chat with Streaming and RAG follow [this guide](https://docs.cohere.com/docs/cochat-beta#various-ways-of-using-the-chat-endpoint).
 
         Parameters:
             - message: str. Text input for the model to respond to.
 
-            - model: typing.Optional[str]. Defaults to `command-r`.
+            - model: typing.Optional[str]. Defaults to `command-r-plus`.
 
                                            The name of a compatible [Cohere model](https://docs.cohere.com/docs/models) or the ID of a [fine-tuned](https://docs.cohere.com/docs/chat-fine-tuning) model.
 
             - preamble: typing.Optional[str]. When specified, the default Cohere preamble will be replaced with the provided one. Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style, and use the `SYSTEM` role.
 
                                               The `SYSTEM` role is also used for the contents of the optional `chat_history=` parameter. When used with the `chat_history=` parameter it adds content throughout a conversation. Conversely, when used with the `preamble=` parameter it adds content at the start of the conversation only.
 
@@ -203,14 +207,18 @@
 
                                                                          An `id` field (string) can be optionally supplied to identify the document in the citations. This field will not be passed to the model.
 
                                                                          An `_excludes` field (array of strings) can be optionally supplied to omit some key-value pairs from being shown to the model. The omitted fields will still show up in the citation object. The "_excludes" field will not be passed to the model.
 
                                                                          See ['Document Mode'](https://docs.cohere.com/docs/retrieval-augmented-generation-rag#document-mode) in the guide for more information.
 
+            - citation_quality: typing.Optional[ChatStreamRequestCitationQuality]. Defaults to `"accurate"`.
+
+                                                                                   Dictates the approach taken to generating citations as part of the RAG flow by allowing the user to specify whether they want `"accurate"` results or `"fast"` results.
+
             - temperature: typing.Optional[float]. Defaults to `0.3`.
 
                                                    A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations, and higher temperatures mean more random generations.
 
                                                    Randomness can be further maximized by increasing the  value of the `p` parameter.
 
             - max_tokens: typing.Optional[int]. The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
@@ -235,14 +243,16 @@
 
             - presence_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
                                                         Used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
 
             - raw_prompting: typing.Optional[bool]. When enabled, the user's prompt will be sent to the model without any pre-processing.
 
+            - return_prompt: typing.Optional[bool]. The prompt is returned in the `prompt` response field when this is enabled.
+
             - tools: typing.Optional[typing.Sequence[Tool]]. A list of available tools (functions) that the model may suggest invoking before producing a text response.
 
                                                              When `tools` is passed (without `tool_results`), the `text` field in the response will be `""` and the `tool_calls` field in the response will be populated with a list of tool calls that need to be made. If no calls need to be made, the `tool_calls` array will be empty.
 
             - tool_results: typing.Optional[typing.Sequence[ChatStreamRequestToolResultsItem]]. A list of results from invoking tools recommended by the model in the previous chat turn. Results are used to produce a text response and will be referenced in citations. When using `tool_results`, `tools` must be passed as well.
                                                                                                 Each tool_result contains information about how it was invoked, as well as a list of outputs in the form of dictionaries.
 
@@ -303,14 +313,16 @@
             _request["prompt_truncation"] = prompt_truncation
         if connectors is not OMIT:
             _request["connectors"] = connectors
         if search_queries_only is not OMIT:
             _request["search_queries_only"] = search_queries_only
         if documents is not OMIT:
             _request["documents"] = documents
+        if citation_quality is not OMIT:
+            _request["citation_quality"] = citation_quality
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if max_tokens is not OMIT:
             _request["max_tokens"] = max_tokens
         if max_input_tokens is not OMIT:
             _request["max_input_tokens"] = max_input_tokens
         if k is not OMIT:
@@ -323,14 +335,16 @@
             _request["stop_sequences"] = stop_sequences
         if frequency_penalty is not OMIT:
             _request["frequency_penalty"] = frequency_penalty
         if presence_penalty is not OMIT:
             _request["presence_penalty"] = presence_penalty
         if raw_prompting is not OMIT:
             _request["raw_prompting"] = raw_prompting
+        if return_prompt is not OMIT:
+            _request["return_prompt"] = return_prompt
         if tools is not OMIT:
             _request["tools"] = tools
         if tool_results is not OMIT:
             _request["tool_results"] = tool_results
         with self._client_wrapper.httpx_client.stream(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "chat"),
@@ -388,36 +402,38 @@
         preamble: typing.Optional[str] = OMIT,
         chat_history: typing.Optional[typing.Sequence[ChatMessage]] = OMIT,
         conversation_id: typing.Optional[str] = OMIT,
         prompt_truncation: typing.Optional[ChatRequestPromptTruncation] = OMIT,
         connectors: typing.Optional[typing.Sequence[ChatConnector]] = OMIT,
         search_queries_only: typing.Optional[bool] = OMIT,
         documents: typing.Optional[typing.Sequence[ChatDocument]] = OMIT,
+        citation_quality: typing.Optional[ChatRequestCitationQuality] = OMIT,
         temperature: typing.Optional[float] = OMIT,
         max_tokens: typing.Optional[int] = OMIT,
         max_input_tokens: typing.Optional[int] = OMIT,
         k: typing.Optional[int] = OMIT,
         p: typing.Optional[float] = OMIT,
         seed: typing.Optional[float] = OMIT,
         stop_sequences: typing.Optional[typing.Sequence[str]] = OMIT,
         frequency_penalty: typing.Optional[float] = OMIT,
         presence_penalty: typing.Optional[float] = OMIT,
         raw_prompting: typing.Optional[bool] = OMIT,
+        return_prompt: typing.Optional[bool] = OMIT,
         tools: typing.Optional[typing.Sequence[Tool]] = OMIT,
         tool_results: typing.Optional[typing.Sequence[ChatRequestToolResultsItem]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> NonStreamedChatResponse:
         """
         Generates a text response to a user message.
         To learn how to use Chat with Streaming and RAG follow [this guide](https://docs.cohere.com/docs/cochat-beta#various-ways-of-using-the-chat-endpoint).
 
         Parameters:
             - message: str. Text input for the model to respond to.
 
-            - model: typing.Optional[str]. Defaults to `command-r`.
+            - model: typing.Optional[str]. Defaults to `command-r-plus`.
 
                                            The name of a compatible [Cohere model](https://docs.cohere.com/docs/models) or the ID of a [fine-tuned](https://docs.cohere.com/docs/chat-fine-tuning) model.
 
             - preamble: typing.Optional[str]. When specified, the default Cohere preamble will be replaced with the provided one. Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style, and use the `SYSTEM` role.
 
                                               The `SYSTEM` role is also used for the contents of the optional `chat_history=` parameter. When used with the `chat_history=` parameter it adds content throughout a conversation. Conversely, when used with the `preamble=` parameter it adds content at the start of the conversation only.
 
@@ -463,14 +479,18 @@
 
                                                                          An `id` field (string) can be optionally supplied to identify the document in the citations. This field will not be passed to the model.
 
                                                                          An `_excludes` field (array of strings) can be optionally supplied to omit some key-value pairs from being shown to the model. The omitted fields will still show up in the citation object. The "_excludes" field will not be passed to the model.
 
                                                                          See ['Document Mode'](https://docs.cohere.com/docs/retrieval-augmented-generation-rag#document-mode) in the guide for more information.
 
+            - citation_quality: typing.Optional[ChatRequestCitationQuality]. Defaults to `"accurate"`.
+
+                                                                             Dictates the approach taken to generating citations as part of the RAG flow by allowing the user to specify whether they want `"accurate"` results or `"fast"` results.
+
             - temperature: typing.Optional[float]. Defaults to `0.3`.
 
                                                    A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations, and higher temperatures mean more random generations.
 
                                                    Randomness can be further maximized by increasing the  value of the `p` parameter.
 
             - max_tokens: typing.Optional[int]. The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
@@ -495,14 +515,16 @@
 
             - presence_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
                                                         Used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
 
             - raw_prompting: typing.Optional[bool]. When enabled, the user's prompt will be sent to the model without any pre-processing.
 
+            - return_prompt: typing.Optional[bool]. The prompt is returned in the `prompt` response field when this is enabled.
+
             - tools: typing.Optional[typing.Sequence[Tool]]. A list of available tools (functions) that the model may suggest invoking before producing a text response.
 
                                                              When `tools` is passed (without `tool_results`), the `text` field in the response will be `""` and the `tool_calls` field in the response will be populated with a list of tool calls that need to be made. If no calls need to be made, the `tool_calls` array will be empty.
 
             - tool_results: typing.Optional[typing.Sequence[ChatRequestToolResultsItem]]. A list of results from invoking tools recommended by the model in the previous chat turn. Results are used to produce a text response and will be referenced in citations. When using `tool_results`, `tools` must be passed as well.
                                                                                           Each tool_result contains information about how it was invoked, as well as a list of outputs in the form of dictionaries.
 
@@ -563,14 +585,16 @@
             _request["prompt_truncation"] = prompt_truncation
         if connectors is not OMIT:
             _request["connectors"] = connectors
         if search_queries_only is not OMIT:
             _request["search_queries_only"] = search_queries_only
         if documents is not OMIT:
             _request["documents"] = documents
+        if citation_quality is not OMIT:
+            _request["citation_quality"] = citation_quality
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if max_tokens is not OMIT:
             _request["max_tokens"] = max_tokens
         if max_input_tokens is not OMIT:
             _request["max_input_tokens"] = max_input_tokens
         if k is not OMIT:
@@ -583,14 +607,16 @@
             _request["stop_sequences"] = stop_sequences
         if frequency_penalty is not OMIT:
             _request["frequency_penalty"] = frequency_penalty
         if presence_penalty is not OMIT:
             _request["presence_penalty"] = presence_penalty
         if raw_prompting is not OMIT:
             _request["raw_prompting"] = raw_prompting
+        if return_prompt is not OMIT:
+            _request["return_prompt"] = return_prompt
         if tools is not OMIT:
             _request["tools"] = tools
         if tool_results is not OMIT:
             _request["tool_results"] = tool_results
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "chat"),
@@ -1205,30 +1231,30 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def classify(
         self,
         *,
         inputs: typing.Sequence[str],
-        examples: typing.Sequence[ClassifyExample],
+        examples: typing.Optional[typing.Sequence[ClassifyExample]] = OMIT,
         model: typing.Optional[str] = OMIT,
         preset: typing.Optional[str] = OMIT,
         truncate: typing.Optional[ClassifyRequestTruncate] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ClassifyResponse:
         """
         This endpoint makes a prediction about which label fits the specified text inputs best. To make a prediction, Classify uses the provided `examples` of text + label pairs as a reference.
         Note: [Fine-tuned models](https://docs.cohere.com/docs/classify-fine-tuning) trained on classification examples don't require the `examples` parameter to be passed in explicitly.
 
         Parameters:
             - inputs: typing.Sequence[str]. A list of up to 96 texts to be classified. Each one must be a non-empty string.
                                             There is, however, no consistent, universal limit to the length a particular input can be. We perform classification on the first `x` tokens of each input, and `x` varies depending on which underlying model is powering classification. The maximum token length for each model is listed in the "max tokens" column [here](https://docs.cohere.com/docs/models).
                                             Note: by default the `truncate` parameter is set to `END`, so tokens exceeding the limit will be automatically dropped. This behavior can be disabled by setting `truncate` to `NONE`, which will result in validation errors for longer texts.
-            - examples: typing.Sequence[ClassifyExample]. An array of examples to provide context to the model. Each example is a text string and its associated label/class. Each unique label requires at least 2 examples associated with it; the maximum number of examples is 2500, and each example has a maximum length of 512 tokens. The values should be structured as `{text: "...",label: "..."}`.
-                                                          Note: [Fine-tuned Models](https://docs.cohere.com/docs/classify-fine-tuning) trained on classification examples don't require the `examples` parameter to be passed in explicitly.
+            - examples: typing.Optional[typing.Sequence[ClassifyExample]]. An array of examples to provide context to the model. Each example is a text string and its associated label/class. Each unique label requires at least 2 examples associated with it; the maximum number of examples is 2500, and each example has a maximum length of 512 tokens. The values should be structured as `{text: "...",label: "..."}`.
+                                                                           Note: [Fine-tuned Models](https://docs.cohere.com/docs/classify-fine-tuning) trained on classification examples don't require the `examples` parameter to be passed in explicitly.
             - model: typing.Optional[str]. The identifier of the model. Currently available models are `embed-multilingual-v2.0`, `embed-english-light-v2.0`, and `embed-english-v2.0` (default). Smaller "light" models are faster, while larger models will perform better. [Fine-tuned models](https://docs.cohere.com/docs/fine-tuning) can also be supplied with their full ID.
 
             - preset: typing.Optional[str]. The ID of a custom playground preset. You can create presets in the [playground](https://dashboard.cohere.ai/playground/classify?model=large). If you use a preset, all other parameters become optional, and any included parameters will override the preset's parameters.
 
             - truncate: typing.Optional[ClassifyRequestTruncate]. One of `NONE|START|END` to specify how the API will handle inputs longer than the maximum token length.
                                                                   Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
                                                                   If `NONE` is selected, when the input exceeds the maximum input token length an error will be returned.
@@ -1284,15 +1310,17 @@
                     text="Pre-read for tomorrow",
                     label="Not spam",
                 ),
             ],
             preset="my-preset-a58sbd",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"inputs": inputs, "examples": examples}
+        _request: typing.Dict[str, typing.Any] = {"inputs": inputs}
+        if examples is not OMIT:
+            _request["examples"] = examples
         if model is not OMIT:
             _request["model"] = model
         if preset is not OMIT:
             _request["preset"] = preset
         if truncate is not OMIT:
             _request["truncate"] = truncate
         _response = self._client_wrapper.httpx_client.request(
@@ -1639,36 +1667,38 @@
         preamble: typing.Optional[str] = OMIT,
         chat_history: typing.Optional[typing.Sequence[ChatMessage]] = OMIT,
         conversation_id: typing.Optional[str] = OMIT,
         prompt_truncation: typing.Optional[ChatStreamRequestPromptTruncation] = OMIT,
         connectors: typing.Optional[typing.Sequence[ChatConnector]] = OMIT,
         search_queries_only: typing.Optional[bool] = OMIT,
         documents: typing.Optional[typing.Sequence[ChatDocument]] = OMIT,
+        citation_quality: typing.Optional[ChatStreamRequestCitationQuality] = OMIT,
         temperature: typing.Optional[float] = OMIT,
         max_tokens: typing.Optional[int] = OMIT,
         max_input_tokens: typing.Optional[int] = OMIT,
         k: typing.Optional[int] = OMIT,
         p: typing.Optional[float] = OMIT,
         seed: typing.Optional[float] = OMIT,
         stop_sequences: typing.Optional[typing.Sequence[str]] = OMIT,
         frequency_penalty: typing.Optional[float] = OMIT,
         presence_penalty: typing.Optional[float] = OMIT,
         raw_prompting: typing.Optional[bool] = OMIT,
+        return_prompt: typing.Optional[bool] = OMIT,
         tools: typing.Optional[typing.Sequence[Tool]] = OMIT,
         tool_results: typing.Optional[typing.Sequence[ChatStreamRequestToolResultsItem]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.AsyncIterator[StreamedChatResponse]:
         """
         Generates a text response to a user message.
         To learn how to use Chat with Streaming and RAG follow [this guide](https://docs.cohere.com/docs/cochat-beta#various-ways-of-using-the-chat-endpoint).
 
         Parameters:
             - message: str. Text input for the model to respond to.
 
-            - model: typing.Optional[str]. Defaults to `command-r`.
+            - model: typing.Optional[str]. Defaults to `command-r-plus`.
 
                                            The name of a compatible [Cohere model](https://docs.cohere.com/docs/models) or the ID of a [fine-tuned](https://docs.cohere.com/docs/chat-fine-tuning) model.
 
             - preamble: typing.Optional[str]. When specified, the default Cohere preamble will be replaced with the provided one. Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style, and use the `SYSTEM` role.
 
                                               The `SYSTEM` role is also used for the contents of the optional `chat_history=` parameter. When used with the `chat_history=` parameter it adds content throughout a conversation. Conversely, when used with the `preamble=` parameter it adds content at the start of the conversation only.
 
@@ -1714,14 +1744,18 @@
 
                                                                          An `id` field (string) can be optionally supplied to identify the document in the citations. This field will not be passed to the model.
 
                                                                          An `_excludes` field (array of strings) can be optionally supplied to omit some key-value pairs from being shown to the model. The omitted fields will still show up in the citation object. The "_excludes" field will not be passed to the model.
 
                                                                          See ['Document Mode'](https://docs.cohere.com/docs/retrieval-augmented-generation-rag#document-mode) in the guide for more information.
 
+            - citation_quality: typing.Optional[ChatStreamRequestCitationQuality]. Defaults to `"accurate"`.
+
+                                                                                   Dictates the approach taken to generating citations as part of the RAG flow by allowing the user to specify whether they want `"accurate"` results or `"fast"` results.
+
             - temperature: typing.Optional[float]. Defaults to `0.3`.
 
                                                    A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations, and higher temperatures mean more random generations.
 
                                                    Randomness can be further maximized by increasing the  value of the `p` parameter.
 
             - max_tokens: typing.Optional[int]. The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
@@ -1746,14 +1780,16 @@
 
             - presence_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
                                                         Used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
 
             - raw_prompting: typing.Optional[bool]. When enabled, the user's prompt will be sent to the model without any pre-processing.
 
+            - return_prompt: typing.Optional[bool]. The prompt is returned in the `prompt` response field when this is enabled.
+
             - tools: typing.Optional[typing.Sequence[Tool]]. A list of available tools (functions) that the model may suggest invoking before producing a text response.
 
                                                              When `tools` is passed (without `tool_results`), the `text` field in the response will be `""` and the `tool_calls` field in the response will be populated with a list of tool calls that need to be made. If no calls need to be made, the `tool_calls` array will be empty.
 
             - tool_results: typing.Optional[typing.Sequence[ChatStreamRequestToolResultsItem]]. A list of results from invoking tools recommended by the model in the previous chat turn. Results are used to produce a text response and will be referenced in citations. When using `tool_results`, `tools` must be passed as well.
                                                                                                 Each tool_result contains information about how it was invoked, as well as a list of outputs in the form of dictionaries.
 
@@ -1814,14 +1850,16 @@
             _request["prompt_truncation"] = prompt_truncation
         if connectors is not OMIT:
             _request["connectors"] = connectors
         if search_queries_only is not OMIT:
             _request["search_queries_only"] = search_queries_only
         if documents is not OMIT:
             _request["documents"] = documents
+        if citation_quality is not OMIT:
+            _request["citation_quality"] = citation_quality
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if max_tokens is not OMIT:
             _request["max_tokens"] = max_tokens
         if max_input_tokens is not OMIT:
             _request["max_input_tokens"] = max_input_tokens
         if k is not OMIT:
@@ -1834,14 +1872,16 @@
             _request["stop_sequences"] = stop_sequences
         if frequency_penalty is not OMIT:
             _request["frequency_penalty"] = frequency_penalty
         if presence_penalty is not OMIT:
             _request["presence_penalty"] = presence_penalty
         if raw_prompting is not OMIT:
             _request["raw_prompting"] = raw_prompting
+        if return_prompt is not OMIT:
+            _request["return_prompt"] = return_prompt
         if tools is not OMIT:
             _request["tools"] = tools
         if tool_results is not OMIT:
             _request["tool_results"] = tool_results
         async with self._client_wrapper.httpx_client.stream(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "chat"),
@@ -1899,36 +1939,38 @@
         preamble: typing.Optional[str] = OMIT,
         chat_history: typing.Optional[typing.Sequence[ChatMessage]] = OMIT,
         conversation_id: typing.Optional[str] = OMIT,
         prompt_truncation: typing.Optional[ChatRequestPromptTruncation] = OMIT,
         connectors: typing.Optional[typing.Sequence[ChatConnector]] = OMIT,
         search_queries_only: typing.Optional[bool] = OMIT,
         documents: typing.Optional[typing.Sequence[ChatDocument]] = OMIT,
+        citation_quality: typing.Optional[ChatRequestCitationQuality] = OMIT,
         temperature: typing.Optional[float] = OMIT,
         max_tokens: typing.Optional[int] = OMIT,
         max_input_tokens: typing.Optional[int] = OMIT,
         k: typing.Optional[int] = OMIT,
         p: typing.Optional[float] = OMIT,
         seed: typing.Optional[float] = OMIT,
         stop_sequences: typing.Optional[typing.Sequence[str]] = OMIT,
         frequency_penalty: typing.Optional[float] = OMIT,
         presence_penalty: typing.Optional[float] = OMIT,
         raw_prompting: typing.Optional[bool] = OMIT,
+        return_prompt: typing.Optional[bool] = OMIT,
         tools: typing.Optional[typing.Sequence[Tool]] = OMIT,
         tool_results: typing.Optional[typing.Sequence[ChatRequestToolResultsItem]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> NonStreamedChatResponse:
         """
         Generates a text response to a user message.
         To learn how to use Chat with Streaming and RAG follow [this guide](https://docs.cohere.com/docs/cochat-beta#various-ways-of-using-the-chat-endpoint).
 
         Parameters:
             - message: str. Text input for the model to respond to.
 
-            - model: typing.Optional[str]. Defaults to `command-r`.
+            - model: typing.Optional[str]. Defaults to `command-r-plus`.
 
                                            The name of a compatible [Cohere model](https://docs.cohere.com/docs/models) or the ID of a [fine-tuned](https://docs.cohere.com/docs/chat-fine-tuning) model.
 
             - preamble: typing.Optional[str]. When specified, the default Cohere preamble will be replaced with the provided one. Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style, and use the `SYSTEM` role.
 
                                               The `SYSTEM` role is also used for the contents of the optional `chat_history=` parameter. When used with the `chat_history=` parameter it adds content throughout a conversation. Conversely, when used with the `preamble=` parameter it adds content at the start of the conversation only.
 
@@ -1974,14 +2016,18 @@
 
                                                                          An `id` field (string) can be optionally supplied to identify the document in the citations. This field will not be passed to the model.
 
                                                                          An `_excludes` field (array of strings) can be optionally supplied to omit some key-value pairs from being shown to the model. The omitted fields will still show up in the citation object. The "_excludes" field will not be passed to the model.
 
                                                                          See ['Document Mode'](https://docs.cohere.com/docs/retrieval-augmented-generation-rag#document-mode) in the guide for more information.
 
+            - citation_quality: typing.Optional[ChatRequestCitationQuality]. Defaults to `"accurate"`.
+
+                                                                             Dictates the approach taken to generating citations as part of the RAG flow by allowing the user to specify whether they want `"accurate"` results or `"fast"` results.
+
             - temperature: typing.Optional[float]. Defaults to `0.3`.
 
                                                    A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations, and higher temperatures mean more random generations.
 
                                                    Randomness can be further maximized by increasing the  value of the `p` parameter.
 
             - max_tokens: typing.Optional[int]. The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
@@ -2006,14 +2052,16 @@
 
             - presence_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
                                                         Used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
 
             - raw_prompting: typing.Optional[bool]. When enabled, the user's prompt will be sent to the model without any pre-processing.
 
+            - return_prompt: typing.Optional[bool]. The prompt is returned in the `prompt` response field when this is enabled.
+
             - tools: typing.Optional[typing.Sequence[Tool]]. A list of available tools (functions) that the model may suggest invoking before producing a text response.
 
                                                              When `tools` is passed (without `tool_results`), the `text` field in the response will be `""` and the `tool_calls` field in the response will be populated with a list of tool calls that need to be made. If no calls need to be made, the `tool_calls` array will be empty.
 
             - tool_results: typing.Optional[typing.Sequence[ChatRequestToolResultsItem]]. A list of results from invoking tools recommended by the model in the previous chat turn. Results are used to produce a text response and will be referenced in citations. When using `tool_results`, `tools` must be passed as well.
                                                                                           Each tool_result contains information about how it was invoked, as well as a list of outputs in the form of dictionaries.
 
@@ -2074,14 +2122,16 @@
             _request["prompt_truncation"] = prompt_truncation
         if connectors is not OMIT:
             _request["connectors"] = connectors
         if search_queries_only is not OMIT:
             _request["search_queries_only"] = search_queries_only
         if documents is not OMIT:
             _request["documents"] = documents
+        if citation_quality is not OMIT:
+            _request["citation_quality"] = citation_quality
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if max_tokens is not OMIT:
             _request["max_tokens"] = max_tokens
         if max_input_tokens is not OMIT:
             _request["max_input_tokens"] = max_input_tokens
         if k is not OMIT:
@@ -2094,14 +2144,16 @@
             _request["stop_sequences"] = stop_sequences
         if frequency_penalty is not OMIT:
             _request["frequency_penalty"] = frequency_penalty
         if presence_penalty is not OMIT:
             _request["presence_penalty"] = presence_penalty
         if raw_prompting is not OMIT:
             _request["raw_prompting"] = raw_prompting
+        if return_prompt is not OMIT:
+            _request["return_prompt"] = return_prompt
         if tools is not OMIT:
             _request["tools"] = tools
         if tool_results is not OMIT:
             _request["tool_results"] = tool_results
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "chat"),
@@ -2716,30 +2768,30 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def classify(
         self,
         *,
         inputs: typing.Sequence[str],
-        examples: typing.Sequence[ClassifyExample],
+        examples: typing.Optional[typing.Sequence[ClassifyExample]] = OMIT,
         model: typing.Optional[str] = OMIT,
         preset: typing.Optional[str] = OMIT,
         truncate: typing.Optional[ClassifyRequestTruncate] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ClassifyResponse:
         """
         This endpoint makes a prediction about which label fits the specified text inputs best. To make a prediction, Classify uses the provided `examples` of text + label pairs as a reference.
         Note: [Fine-tuned models](https://docs.cohere.com/docs/classify-fine-tuning) trained on classification examples don't require the `examples` parameter to be passed in explicitly.
 
         Parameters:
             - inputs: typing.Sequence[str]. A list of up to 96 texts to be classified. Each one must be a non-empty string.
                                             There is, however, no consistent, universal limit to the length a particular input can be. We perform classification on the first `x` tokens of each input, and `x` varies depending on which underlying model is powering classification. The maximum token length for each model is listed in the "max tokens" column [here](https://docs.cohere.com/docs/models).
                                             Note: by default the `truncate` parameter is set to `END`, so tokens exceeding the limit will be automatically dropped. This behavior can be disabled by setting `truncate` to `NONE`, which will result in validation errors for longer texts.
-            - examples: typing.Sequence[ClassifyExample]. An array of examples to provide context to the model. Each example is a text string and its associated label/class. Each unique label requires at least 2 examples associated with it; the maximum number of examples is 2500, and each example has a maximum length of 512 tokens. The values should be structured as `{text: "...",label: "..."}`.
-                                                          Note: [Fine-tuned Models](https://docs.cohere.com/docs/classify-fine-tuning) trained on classification examples don't require the `examples` parameter to be passed in explicitly.
+            - examples: typing.Optional[typing.Sequence[ClassifyExample]]. An array of examples to provide context to the model. Each example is a text string and its associated label/class. Each unique label requires at least 2 examples associated with it; the maximum number of examples is 2500, and each example has a maximum length of 512 tokens. The values should be structured as `{text: "...",label: "..."}`.
+                                                                           Note: [Fine-tuned Models](https://docs.cohere.com/docs/classify-fine-tuning) trained on classification examples don't require the `examples` parameter to be passed in explicitly.
             - model: typing.Optional[str]. The identifier of the model. Currently available models are `embed-multilingual-v2.0`, `embed-english-light-v2.0`, and `embed-english-v2.0` (default). Smaller "light" models are faster, while larger models will perform better. [Fine-tuned models](https://docs.cohere.com/docs/fine-tuning) can also be supplied with their full ID.
 
             - preset: typing.Optional[str]. The ID of a custom playground preset. You can create presets in the [playground](https://dashboard.cohere.ai/playground/classify?model=large). If you use a preset, all other parameters become optional, and any included parameters will override the preset's parameters.
 
             - truncate: typing.Optional[ClassifyRequestTruncate]. One of `NONE|START|END` to specify how the API will handle inputs longer than the maximum token length.
                                                                   Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
                                                                   If `NONE` is selected, when the input exceeds the maximum input token length an error will be returned.
@@ -2795,15 +2847,17 @@
                     text="Pre-read for tomorrow",
                     label="Not spam",
                 ),
             ],
             preset="my-preset-a58sbd",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"inputs": inputs, "examples": examples}
+        _request: typing.Dict[str, typing.Any] = {"inputs": inputs}
+        if examples is not OMIT:
+            _request["examples"] = examples
         if model is not OMIT:
             _request["model"] = model
         if preset is not OMIT:
             _request["preset"] = preset
         if truncate is not OMIT:
             _request["truncate"] = truncate
         _response = await self._client_wrapper.httpx_client.request(
```

### Comparing `cohere-5.3.2/src/cohere/client.py` & `cohere-5.3.3/src/cohere/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/connectors/client.py` & `cohere-5.3.3/src/cohere/connectors/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/core/__init__.py` & `cohere-5.3.3/src/cohere/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/core/client_wrapper.py` & `cohere-5.3.3/src/cohere/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "cohere",
-            "X-Fern-SDK-Version": "5.3.2",
+            "X-Fern-SDK-Version": "5.3.3",
         }
         if self._client_name is not None:
             headers["X-Client-Name"] = self._client_name
         headers["Authorization"] = f"Bearer {self._get_token()}"
         return headers
 
     def _get_token(self) -> str:
```

### Comparing `cohere-5.3.2/src/cohere/core/datetime_utils.py` & `cohere-5.3.3/src/cohere/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/core/file.py` & `cohere-5.3.3/src/cohere/core/file.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/core/http_client.py` & `cohere-5.3.3/src/cohere/core/http_client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/core/jsonable_encoder.py` & `cohere-5.3.3/src/cohere/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/core/request_options.py` & `cohere-5.3.3/src/cohere/core/request_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/core/unchecked_base_model.py` & `cohere-5.3.3/src/cohere/core/unchecked_base_model.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/datasets/client.py` & `cohere-5.3.3/src/cohere/datasets/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from ..core.datetime_utils import serialize_datetime
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..core.unchecked_base_model import construct_type
 from ..errors.too_many_requests_error import TooManyRequestsError
 from ..types.dataset_type import DatasetType
+from ..types.dataset_validation_status import DatasetValidationStatus
 from .types.datasets_create_response import DatasetsCreateResponse
 from .types.datasets_get_response import DatasetsGetResponse
 from .types.datasets_get_usage_response import DatasetsGetUsageResponse
 from .types.datasets_list_response import DatasetsListResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
@@ -32,14 +33,15 @@
         self,
         *,
         dataset_type: typing.Optional[str] = None,
         before: typing.Optional[dt.datetime] = None,
         after: typing.Optional[dt.datetime] = None,
         limit: typing.Optional[float] = None,
         offset: typing.Optional[float] = None,
+        validation_status: typing.Optional[DatasetValidationStatus] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> DatasetsListResponse:
         """
         List datasets that have been created.
 
         Parameters:
             - dataset_type: typing.Optional[str]. optional filter by dataset type
@@ -48,14 +50,16 @@
 
             - after: typing.Optional[dt.datetime]. optional filter after a date
 
             - limit: typing.Optional[float]. optional limit to number of results
 
             - offset: typing.Optional[float]. optional offset to start of results
 
+            - validation_status: typing.Optional[DatasetValidationStatus]. optional filter by validation status
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
@@ -69,14 +73,15 @@
                 remove_none_from_dict(
                     {
                         "datasetType": dataset_type,
                         "before": serialize_datetime(before) if before is not None else None,
                         "after": serialize_datetime(after) if after is not None else None,
                         "limit": limit,
                         "offset": offset,
+                        "validationStatus": validation_status,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
                             else {}
                         ),
                     }
                 )
@@ -378,14 +383,15 @@
         self,
         *,
         dataset_type: typing.Optional[str] = None,
         before: typing.Optional[dt.datetime] = None,
         after: typing.Optional[dt.datetime] = None,
         limit: typing.Optional[float] = None,
         offset: typing.Optional[float] = None,
+        validation_status: typing.Optional[DatasetValidationStatus] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> DatasetsListResponse:
         """
         List datasets that have been created.
 
         Parameters:
             - dataset_type: typing.Optional[str]. optional filter by dataset type
@@ -394,14 +400,16 @@
 
             - after: typing.Optional[dt.datetime]. optional filter after a date
 
             - limit: typing.Optional[float]. optional limit to number of results
 
             - offset: typing.Optional[float]. optional offset to start of results
 
+            - validation_status: typing.Optional[DatasetValidationStatus]. optional filter by validation status
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
@@ -415,14 +423,15 @@
                 remove_none_from_dict(
                     {
                         "datasetType": dataset_type,
                         "before": serialize_datetime(before) if before is not None else None,
                         "after": serialize_datetime(after) if after is not None else None,
                         "limit": limit,
                         "offset": offset,
+                        "validationStatus": validation_status,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
                             else {}
                         ),
                     }
                 )
```

### Comparing `cohere-5.3.2/src/cohere/datasets/types/__init__.py` & `cohere-5.3.3/src/cohere/datasets/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/datasets/types/datasets_create_response.py` & `cohere-5.3.3/src/cohere/datasets/types/datasets_create_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/datasets/types/datasets_create_response_dataset_parts.py` & `cohere-5.3.3/src/cohere/datasets/types/datasets_create_response_dataset_parts.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/datasets/types/datasets_get_response.py` & `cohere-5.3.3/src/cohere/datasets/types/datasets_get_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/datasets/types/datasets_get_usage_response.py` & `cohere-5.3.3/src/cohere/datasets/types/datasets_get_usage_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/datasets/types/datasets_list_response.py` & `cohere-5.3.3/src/cohere/datasets/types/datasets_list_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/embed_jobs/client.py` & `cohere-5.3.3/src/cohere/embed_jobs/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/errors/__init__.py` & `cohere-5.3.3/src/cohere/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/finetuning/__init__.py` & `cohere-5.3.3/src/cohere/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/finetuning/client.py` & `cohere-5.3.3/src/cohere/finetuning/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/finetuning/finetuning/__init__.py` & `cohere-5.3.3/src/cohere/finetuning/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/finetuning/finetuning/types/__init__.py` & `cohere-5.3.3/src/cohere/finetuning/finetuning/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/finetuning/finetuning/types/base_model.py` & `cohere-5.3.3/src/cohere/finetuning/finetuning/types/base_model.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py` & `cohere-5.3.3/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/finetuning/finetuning/types/error.py` & `cohere-5.3.3/src/cohere/finetuning/finetuning/types/error.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/finetuning/finetuning/types/event.py` & `cohere-5.3.3/src/cohere/finetuning/finetuning/types/event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/finetuning/finetuning/types/finetuned_model.py` & `cohere-5.3.3/src/cohere/finetuning/finetuning/types/finetuned_model.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py` & `cohere-5.3.3/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/finetuning/finetuning/types/hyperparameters.py` & `cohere-5.3.3/src/cohere/finetuning/finetuning/types/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/finetuning/finetuning/types/list_events_response.py` & `cohere-5.3.3/src/cohere/finetuning/finetuning/types/list_events_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py` & `cohere-5.3.3/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py` & `cohere-5.3.3/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/finetuning/finetuning/types/settings.py` & `cohere-5.3.3/src/cohere/finetuning/finetuning/types/settings.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/finetuning/finetuning/types/training_step_metrics.py` & `cohere-5.3.3/src/cohere/finetuning/finetuning/types/training_step_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py` & `cohere-5.3.3/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/manually_maintained/cache.py` & `cohere-5.3.3/src/cohere/manually_maintained/cache.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/manually_maintained/tokenizers.py` & `cohere-5.3.3/src/cohere/manually_maintained/tokenizers.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/models/client.py` & `cohere-5.3.3/src/cohere/models/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/overrides.py` & `cohere-5.3.3/src/cohere/overrides.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/__init__.py` & `cohere-5.3.3/src/cohere/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/api_meta.py` & `cohere-5.3.3/src/cohere/types/api_meta.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/api_meta_api_version.py` & `cohere-5.3.3/src/cohere/types/api_meta_api_version.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/api_meta_billed_units.py` & `cohere-5.3.3/src/cohere/types/api_meta_billed_units.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/api_meta_tokens.py` & `cohere-5.3.3/src/cohere/types/api_meta_tokens.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/chat_citation.py` & `cohere-5.3.3/src/cohere/types/chat_citation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/chat_citation_generation_event.py` & `cohere-5.3.3/src/cohere/types/chat_citation_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/chat_connector.py` & `cohere-5.3.3/src/cohere/types/chat_connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/chat_data_metrics.py` & `cohere-5.3.3/src/cohere/types/chat_data_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/chat_message.py` & `cohere-5.3.3/src/cohere/types/chat_message.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/chat_request_connectors_search_options.py` & `cohere-5.3.3/src/cohere/types/chat_request_connectors_search_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/chat_request_tool_results_item.py` & `cohere-5.3.3/src/cohere/types/chat_request_tool_results_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/chat_search_queries_generation_event.py` & `cohere-5.3.3/src/cohere/types/chat_search_queries_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/chat_search_query.py` & `cohere-5.3.3/src/cohere/types/chat_search_query.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/chat_search_result.py` & `cohere-5.3.3/src/cohere/types/chat_search_result.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/chat_search_result_connector.py` & `cohere-5.3.3/src/cohere/types/chat_search_result_connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/chat_search_results_event.py` & `cohere-5.3.3/src/cohere/types/chat_search_results_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/chat_stream_end_event.py` & `cohere-5.3.3/src/cohere/types/chat_stream_end_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/chat_stream_event.py` & `cohere-5.3.3/src/cohere/types/chat_stream_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/chat_stream_request_connectors_search_options.py` & `cohere-5.3.3/src/cohere/types/chat_stream_request_connectors_search_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/chat_stream_request_tool_results_item.py` & `cohere-5.3.3/src/cohere/types/chat_stream_request_tool_results_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/chat_stream_start_event.py` & `cohere-5.3.3/src/cohere/types/chat_stream_start_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/chat_text_generation_event.py` & `cohere-5.3.3/src/cohere/types/chat_text_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/chat_tool_calls_generation_event.py` & `cohere-5.3.3/src/cohere/types/chat_tool_calls_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/classify_data_metrics.py` & `cohere-5.3.3/src/cohere/types/classify_data_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/classify_example.py` & `cohere-5.3.3/src/cohere/types/classify_example.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/classify_response.py` & `cohere-5.3.3/src/cohere/types/classify_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/classify_response_classifications_item.py` & `cohere-5.3.3/src/cohere/types/classify_response_classifications_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/classify_response_classifications_item_labels_value.py` & `cohere-5.3.3/src/cohere/types/classify_response_classifications_item_labels_value.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/connector.py` & `cohere-5.3.3/src/cohere/types/connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/connector_o_auth.py` & `cohere-5.3.3/src/cohere/types/connector_o_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/create_connector_o_auth.py` & `cohere-5.3.3/src/cohere/types/create_connector_o_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/create_connector_response.py` & `cohere-5.3.3/src/cohere/types/create_connector_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/create_connector_service_auth.py` & `cohere-5.3.3/src/cohere/types/create_connector_service_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/create_embed_job_response.py` & `cohere-5.3.3/src/cohere/types/create_embed_job_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/dataset.py` & `cohere-5.3.3/src/cohere/types/dataset.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/dataset_part.py` & `cohere-5.3.3/src/cohere/types/dataset_part.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/detokenize_response.py` & `cohere-5.3.3/src/cohere/types/detokenize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/embed_by_type_response.py` & `cohere-5.3.3/src/cohere/types/embed_by_type_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/embed_by_type_response_embeddings.py` & `cohere-5.3.3/src/cohere/types/embed_by_type_response_embeddings.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/embed_floats_response.py` & `cohere-5.3.3/src/cohere/types/embed_floats_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/embed_job.py` & `cohere-5.3.3/src/cohere/types/embed_job.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/embed_response.py` & `cohere-5.3.3/src/cohere/types/embed_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/finetune_dataset_metrics.py` & `cohere-5.3.3/src/cohere/types/finetune_dataset_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/generate_stream_end.py` & `cohere-5.3.3/src/cohere/types/generate_stream_end.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/generate_stream_end_response.py` & `cohere-5.3.3/src/cohere/types/generate_stream_end_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/generate_stream_error.py` & `cohere-5.3.3/src/cohere/types/generate_stream_error.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/generate_stream_event.py` & `cohere-5.3.3/src/cohere/types/generate_stream_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/generate_stream_text.py` & `cohere-5.3.3/src/cohere/types/generate_stream_text.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/generate_streamed_response.py` & `cohere-5.3.3/src/cohere/types/generate_streamed_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/generation.py` & `cohere-5.3.3/src/cohere/types/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/get_connector_response.py` & `cohere-5.3.3/src/cohere/types/get_connector_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/get_model_response.py` & `cohere-5.3.3/src/cohere/types/get_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/label_metric.py` & `cohere-5.3.3/src/cohere/types/label_metric.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/list_connectors_response.py` & `cohere-5.3.3/src/cohere/types/list_connectors_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/list_embed_job_response.py` & `cohere-5.3.3/src/cohere/types/list_embed_job_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/list_models_response.py` & `cohere-5.3.3/src/cohere/types/list_models_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/metrics.py` & `cohere-5.3.3/src/cohere/types/metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/non_streamed_chat_response.py` & `cohere-5.3.3/src/cohere/types/non_streamed_chat_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,14 +55,19 @@
     finish_reason: typing.Optional[FinishReason] = None
     tool_calls: typing.Optional[typing.List[ToolCall]] = None
     chat_history: typing.Optional[typing.List[ChatMessage]] = pydantic_v1.Field(default=None)
     """
     A list of previous messages between the user and the model, meant to give the model conversational context for responding to the user's `message`.
     """
 
+    prompt: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The prompt that was used. Only present when `return_prompt` in the request is set to true.
+    """
+
     meta: typing.Optional[ApiMeta] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `cohere-5.3.2/src/cohere/types/o_auth_authorize_response.py` & `cohere-5.3.3/src/cohere/types/o_auth_authorize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/parse_info.py` & `cohere-5.3.3/src/cohere/types/parse_info.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/rerank_request_documents_item_text.py` & `cohere-5.3.3/src/cohere/types/rerank_request_documents_item_text.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/rerank_response.py` & `cohere-5.3.3/src/cohere/types/rerank_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/rerank_response_results_item.py` & `cohere-5.3.3/src/cohere/types/tokenize_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,32 +2,25 @@
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .rerank_response_results_item_document import RerankResponseResultsItemDocument
+from .api_meta import ApiMeta
 
 
-class RerankResponseResultsItem(UncheckedBaseModel):
-    document: typing.Optional[RerankResponseResultsItemDocument] = pydantic_v1.Field(default=None)
+class TokenizeResponse(UncheckedBaseModel):
+    tokens: typing.List[int] = pydantic_v1.Field()
     """
-    The doc object which was ranked
+    An array of tokens, where each token is an integer.
     """
 
-    index: int = pydantic_v1.Field()
-    """
-    The index of the input document
-    """
-
-    relevance_score: float = pydantic_v1.Field()
-    """
-    A relevance score assigned to the ranking
-    """
+    token_strings: typing.List[str]
+    meta: typing.Optional[ApiMeta] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.3.2/src/cohere/types/rerank_response_results_item_document.py` & `cohere-5.3.3/src/cohere/types/rerank_response_results_item_document.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
 class RerankResponseResultsItemDocument(UncheckedBaseModel):
     """
-    The doc object which was ranked
+    If `return_documents` is set as `false` this will return none, if `true` it will return the documents passed in
     """
 
     text: str = pydantic_v1.Field()
     """
     The text of the document to rerank
     """
```

### Comparing `cohere-5.3.2/src/cohere/types/reranker_data_metrics.py` & `cohere-5.3.3/src/cohere/types/reranker_data_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/single_generation.py` & `cohere-5.3.3/src/cohere/types/single_generation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/single_generation_in_stream.py` & `cohere-5.3.3/src/cohere/types/single_generation_in_stream.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/single_generation_token_likelihoods_item.py` & `cohere-5.3.3/src/cohere/types/single_generation_token_likelihoods_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/streamed_chat_response.py` & `cohere-5.3.3/src/cohere/types/streamed_chat_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/summarize_response.py` & `cohere-5.3.3/src/cohere/types/summarize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/tokenize_response.py` & `cohere-5.3.3/src/cohere/types/tool_call.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,25 +2,30 @@
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .api_meta import ApiMeta
 
 
-class TokenizeResponse(UncheckedBaseModel):
-    tokens: typing.List[int] = pydantic_v1.Field()
+class ToolCall(UncheckedBaseModel):
     """
-    An array of tokens, where each token is an integer.
+    Contains the tool calls generated by the model. Use it to invoke your tools.
     """
 
-    token_strings: typing.List[str]
-    meta: typing.Optional[ApiMeta] = None
+    name: str = pydantic_v1.Field()
+    """
+    Name of the tool to call.
+    """
+
+    parameters: typing.Dict[str, typing.Any] = pydantic_v1.Field()
+    """
+    The name and value of the parameters to use when invoking a tool.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `cohere-5.3.2/src/cohere/types/tool.py` & `cohere-5.3.3/src/cohere/types/tool.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/types/tool_call.py` & `cohere-5.3.3/src/cohere/types/tool_parameter_definitions_value.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ToolCall(UncheckedBaseModel):
+class ToolParameterDefinitionsValue(UncheckedBaseModel):
+    description: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    Contains the tool calls generated by the model. Use it to invoke your tools.
+    The description of the parameter.
     """
 
-    name: str = pydantic_v1.Field()
+    type: str = pydantic_v1.Field()
     """
-    Name of the tool to call.
+    The type of the parameter. Must be a valid Python type.
     """
 
-    parameters: typing.Dict[str, typing.Any] = pydantic_v1.Field()
+    required: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
-    The name and value of the parameters to use when invoking a tool.
+    Denotes whether the parameter is always present (required) or not. Defaults to not required.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `cohere-5.3.2/src/cohere/types/update_connector_response.py` & `cohere-5.3.3/src/cohere/types/update_connector_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/src/cohere/utils.py` & `cohere-5.3.3/src/cohere/utils.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.2/PKG-INFO` & `cohere-5.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cohere
-Version: 5.3.2
+Version: 5.3.3
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastavro (>=1.9.4,<2.0.0)
 Requires-Dist: httpx (>=0.21.2)
 Requires-Dist: httpx-sse (>=0.4.0,<0.5.0)
 Requires-Dist: pydantic (>=1.9.2)
 Requires-Dist: requests (>=2.0.0,<3.0.0)
-Requires-Dist: tokenizers (>=0.15.2,<0.16.0)
+Requires-Dist: tokenizers (>=0.19,<0.20)
 Requires-Dist: types-requests (>=2.0.0,<3.0.0)
 Requires-Dist: typing_extensions (>=4.0.0)
 Description-Content-Type: text/markdown
 
 # Cohere Python SDK
 
 ![](banner.png)
```

