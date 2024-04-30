# Comparing `tmp/elevenlabs-1.2.0.tar.gz` & `tmp/elevenlabs-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabs-1.2.0.tar", max compression
+gzip compressed data, was "elevenlabs-1.2.1.tar", max compression
```

## Comparing `elevenlabs-1.2.0.tar` & `elevenlabs-1.2.1.tar`

### file list

```diff
@@ -1,132 +1,132 @@
--rw-r--r--   0        0        0     1067 2024-04-26 14:24:09.383905 elevenlabs-1.2.0/LICENSE
--rw-r--r--   0        0        0     9366 2024-04-26 14:24:09.383905 elevenlabs-1.2.0/README.md
--rw-r--r--   0        0        0      658 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5583 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/__init__.py
--rw-r--r--   0        0        0       65 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/audio_native/__init__.py
--rw-r--r--   0        0        0    13857 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/audio_native/client.py
--rw-r--r--   0        0        0     8308 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/base_client.py
--rw-r--r--   0        0        0       65 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/chapters/__init__.py
--rw-r--r--   0        0        0    36655 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/chapters/client.py
--rw-r--r--   0        0        0    20882 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/client.py
--rw-r--r--   0        0        0     1006 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/api_error.py
--rw-r--r--   0        0        0     1683 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/request_options.py
--rw-r--r--   0        0        0     7123 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/core/unchecked_base_model.py
--rw-r--r--   0        0        0       65 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/dubbing/__init__.py
--rw-r--r--   0        0        0    29465 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/dubbing/client.py
--rw-r--r--   0        0        0      164 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/environment.py
--rw-r--r--   0        0        0      170 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/history/__init__.py
--rw-r--r--   0        0        0    29717 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/history/client.py
--rw-r--r--   0        0        0       65 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/models/__init__.py
--rw-r--r--   0        0        0     5255 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/models/client.py
--rw-r--r--   0        0        0     2715 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/play.py
--rw-r--r--   0        0        0       65 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/projects/__init__.py
--rw-r--r--   0        0        0    64289 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/projects/client.py
--rw-r--r--   0        0        0      303 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/pronunciation_dictionary/__init__.py
--rw-r--r--   0        0        0    38937 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/pronunciation_dictionary/client.py
--rw-r--r--   0        0        0      344 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/pronunciation_dictionary/types/__init__.py
--rw-r--r--   0        0        0     1192 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/pronunciation_dictionary/types/pronunciation_dictionary_rule.py
--rw-r--r--   0        0        0        0 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/py.typed
--rw-r--r--   0        0        0     5093 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/realtime_tts.py
--rw-r--r--   0        0        0       65 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/samples/__init__.py
--rw-r--r--   0        0        0    11479 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/samples/client.py
--rw-r--r--   0        0        0       65 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/speech_to_speech/__init__.py
--rw-r--r--   0        0        0    29158 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/speech_to_speech/client.py
--rw-r--r--   0        0        0       65 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/text_to_speech/__init__.py
--rw-r--r--   0        0        0    24639 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/text_to_speech/client.py
--rw-r--r--   0        0        0     7085 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/__init__.py
--rw-r--r--   0        0        0      188 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/accent.py
--rw-r--r--   0        0        0      977 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/add_project_response_model.py
--rw-r--r--   0        0        0     1057 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py
--rw-r--r--   0        0        0      955 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/add_pronunciation_dictionary_rules_response_model.py
--rw-r--r--   0        0        0      918 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/add_voice_response_model.py
--rw-r--r--   0        0        0      158 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/age.py
--rw-r--r--   0        0        0      979 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/audio_native_create_project_response_model.py
--rw-r--r--   0        0        0      130 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/audio_native_get_embed_code_response_model.py
--rw-r--r--   0        0        0     1568 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/audio_output.py
--rw-r--r--   0        0        0      177 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/category.py
--rw-r--r--   0        0        0     1195 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/chapter_response.py
--rw-r--r--   0        0        0     1010 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/chapter_snapshot_response.py
--rw-r--r--   0        0        0     1018 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/chapter_snapshots_response.py
--rw-r--r--   0        0        0      161 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/chapter_state.py
--rw-r--r--   0        0        0     1028 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/chapter_statistics_response.py
--rw-r--r--   0        0        0      146 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/currency.py
--rw-r--r--   0        0        0      949 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/do_dubbing_response.py
--rw-r--r--   0        0        0     1006 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/dubbing_metadata_response.py
--rw-r--r--   0        0        0      211 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/extended_subscription_response_model_billing_period.py
--rw-r--r--   0        0        0     1081 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/feedback_item.py
--rw-r--r--   0        0        0     1836 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/fine_tuning_response.py
--rw-r--r--   0        0        0      220 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/finetuning_state.py
--rw-r--r--   0        0        0      148 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/gender.py
--rw-r--r--   0        0        0     2290 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/generation_config.py
--rw-r--r--   0        0        0      987 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/get_chapters_response.py
--rw-r--r--   0        0        0     1071 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/get_library_voices_response.py
--rw-r--r--   0        0        0      987 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/get_projects_response.py
--rw-r--r--   0        0        0     1159 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/get_pronunciation_dictionaries_metadata_response_model.py
--rw-r--r--   0        0        0     1067 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py
--rw-r--r--   0        0        0     1072 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/get_speech_history_response.py
--rw-r--r--   0        0        0      952 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/get_voices_response.py
--rw-r--r--   0        0        0      101 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/history.py
--rw-r--r--   0        0        0      991 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/history_item.py
--rw-r--r--   0        0        0     1009 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/http_validation_error.py
--rw-r--r--   0        0        0      947 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/invoice.py
--rw-r--r--   0        0        0      930 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/language_response.py
--rw-r--r--   0        0        0     1764 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/library_voice_response.py
--rw-r--r--   0        0        0     1010 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/manual_verification_file_response.py
--rw-r--r--   0        0        0     1085 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/manual_verification_response.py
--rw-r--r--   0        0        0     1670 2024-04-26 14:24:09.387905 elevenlabs-1.2.0/src/elevenlabs/types/model.py
--rw-r--r--   0        0        0     2215 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/normalized_alignment.py
--rw-r--r--   0        0        0      173 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/optimize_streaming_latency.py
--rw-r--r--   0        0        0      405 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/output_format.py
--rw-r--r--   0        0        0     1277 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/project_extended_response_model.py
--rw-r--r--   0        0        0     1258 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/project_response.py
--rw-r--r--   0        0        0      990 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/project_snapshot_response.py
--rw-r--r--   0        0        0     1018 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/project_snapshots_response.py
--rw-r--r--   0        0        0      161 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/project_state.py
--rw-r--r--   0        0        0      965 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/pronunciation_dictionary_alias_rule_request_model.py
--rw-r--r--   0        0        0      987 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/pronunciation_dictionary_phoneme_rule_request_model.py
--rw-r--r--   0        0        0      973 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/pronunciation_dictionary_version_locator.py
--rw-r--r--   0        0        0     1488 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/realtime_voice_settings.py
--rw-r--r--   0        0        0     1006 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/recording_response.py
--rw-r--r--   0        0        0      958 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/remove_pronunciation_dictionary_rules_response_model.py
--rw-r--r--   0        0        0      217 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/review_status.py
--rw-r--r--   0        0        0     2361 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/send_text.py
--rw-r--r--   0        0        0      144 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/source.py
--rw-r--r--   0        0        0     1864 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/speech_history_item_response.py
--rw-r--r--   0        0        0      223 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/speech_history_item_response_model_voice_category.py
--rw-r--r--   0        0        0     1078 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/sso_provider_db_model.py
--rw-r--r--   0        0        0      170 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/sso_provider_db_model_provider_type.py
--rw-r--r--   0        0        0     1878 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/subscription.py
--rw-r--r--   0        0        0     1610 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/subscription_response.py
--rw-r--r--   0        0        0      197 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/subscription_response_model_billing_period.py
--rw-r--r--   0        0        0      253 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/subscription_status.py
--rw-r--r--   0        0        0     1140 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/user.py
--rw-r--r--   0        0        0     1028 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     1119 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/verification_attempt_response.py
--rw-r--r--   0        0        0     2088 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/voice.py
--rw-r--r--   0        0        0      945 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/voice_generation_parameter_option_response.py
--rw-r--r--   0        0        0     1324 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/voice_generation_parameter_response.py
--rw-r--r--   0        0        0      213 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/voice_response_model_safety_control.py
--rw-r--r--   0        0        0     1101 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/voice_sample.py
--rw-r--r--   0        0        0     1082 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/voice_settings.py
--rw-r--r--   0        0        0     2484 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/voice_sharing_response.py
--rw-r--r--   0        0        0      193 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/voice_sharing_state.py
--rw-r--r--   0        0        0     1244 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/types/voice_verification_response.py
--rw-r--r--   0        0        0       65 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/user/__init__.py
--rw-r--r--   0        0        0     9597 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/user/client.py
--rw-r--r--   0        0        0       78 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/version.py
--rw-r--r--   0        0        0       65 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/voice_generation/__init__.py
--rw-r--r--   0        0        0    21042 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/voice_generation/client.py
--rw-r--r--   0        0        0       65 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/voices/__init__.py
--rw-r--r--   0        0        0    62413 2024-04-26 14:24:09.391905 elevenlabs-1.2.0/src/elevenlabs/voices/client.py
--rw-r--r--   0        0        0     9958 1970-01-01 00:00:00.000000 elevenlabs-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-30 13:13:46.459825 elevenlabs-1.2.1/LICENSE
+-rw-r--r--   0        0        0     9366 2024-04-30 13:13:46.459825 elevenlabs-1.2.1/README.md
+-rw-r--r--   0        0        0      658 2024-04-30 13:13:46.459825 elevenlabs-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5583 2024-04-30 13:13:46.459825 elevenlabs-1.2.1/src/elevenlabs/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-30 13:13:46.459825 elevenlabs-1.2.1/src/elevenlabs/audio_native/__init__.py
+-rw-r--r--   0        0        0    13857 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/audio_native/client.py
+-rw-r--r--   0        0        0     8308 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/base_client.py
+-rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/chapters/__init__.py
+-rw-r--r--   0        0        0    36655 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/chapters/client.py
+-rw-r--r--   0        0        0    20882 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/client.py
+-rw-r--r--   0        0        0     1006 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/api_error.py
+-rw-r--r--   0        0        0     1683 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/request_options.py
+-rw-r--r--   0        0        0     7123 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/core/unchecked_base_model.py
+-rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/dubbing/__init__.py
+-rw-r--r--   0        0        0    29465 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/dubbing/client.py
+-rw-r--r--   0        0        0      164 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/environment.py
+-rw-r--r--   0        0        0      170 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/history/__init__.py
+-rw-r--r--   0        0        0    29717 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/history/client.py
+-rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/models/__init__.py
+-rw-r--r--   0        0        0     5255 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/models/client.py
+-rw-r--r--   0        0        0     2715 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/play.py
+-rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/projects/__init__.py
+-rw-r--r--   0        0        0    64710 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/projects/client.py
+-rw-r--r--   0        0        0      303 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/pronunciation_dictionary/__init__.py
+-rw-r--r--   0        0        0    38937 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/pronunciation_dictionary/client.py
+-rw-r--r--   0        0        0      344 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/pronunciation_dictionary/types/__init__.py
+-rw-r--r--   0        0        0     1192 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/pronunciation_dictionary/types/pronunciation_dictionary_rule.py
+-rw-r--r--   0        0        0        0 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/py.typed
+-rw-r--r--   0        0        0     5093 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/realtime_tts.py
+-rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/samples/__init__.py
+-rw-r--r--   0        0        0    11479 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/samples/client.py
+-rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/speech_to_speech/__init__.py
+-rw-r--r--   0        0        0    29158 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/speech_to_speech/client.py
+-rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/text_to_speech/__init__.py
+-rw-r--r--   0        0        0    24639 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/text_to_speech/client.py
+-rw-r--r--   0        0        0     7085 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/__init__.py
+-rw-r--r--   0        0        0      188 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/accent.py
+-rw-r--r--   0        0        0      977 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/add_project_response_model.py
+-rw-r--r--   0        0        0     1057 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py
+-rw-r--r--   0        0        0      955 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/add_pronunciation_dictionary_rules_response_model.py
+-rw-r--r--   0        0        0      918 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/add_voice_response_model.py
+-rw-r--r--   0        0        0      158 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/age.py
+-rw-r--r--   0        0        0      979 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/audio_native_create_project_response_model.py
+-rw-r--r--   0        0        0      130 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/audio_native_get_embed_code_response_model.py
+-rw-r--r--   0        0        0     1568 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/audio_output.py
+-rw-r--r--   0        0        0      177 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/category.py
+-rw-r--r--   0        0        0     1195 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/chapter_response.py
+-rw-r--r--   0        0        0     1010 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/chapter_snapshot_response.py
+-rw-r--r--   0        0        0     1018 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/chapter_snapshots_response.py
+-rw-r--r--   0        0        0      161 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/chapter_state.py
+-rw-r--r--   0        0        0     1028 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/chapter_statistics_response.py
+-rw-r--r--   0        0        0      146 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/currency.py
+-rw-r--r--   0        0        0      949 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/do_dubbing_response.py
+-rw-r--r--   0        0        0     1006 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/dubbing_metadata_response.py
+-rw-r--r--   0        0        0      211 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/extended_subscription_response_model_billing_period.py
+-rw-r--r--   0        0        0     1081 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/feedback_item.py
+-rw-r--r--   0        0        0     1836 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/fine_tuning_response.py
+-rw-r--r--   0        0        0      220 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/finetuning_state.py
+-rw-r--r--   0        0        0      148 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/gender.py
+-rw-r--r--   0        0        0     2290 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/generation_config.py
+-rw-r--r--   0        0        0      987 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/get_chapters_response.py
+-rw-r--r--   0        0        0     1071 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/get_library_voices_response.py
+-rw-r--r--   0        0        0      987 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/get_projects_response.py
+-rw-r--r--   0        0        0     1159 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/get_pronunciation_dictionaries_metadata_response_model.py
+-rw-r--r--   0        0        0     1067 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py
+-rw-r--r--   0        0        0     1072 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/get_speech_history_response.py
+-rw-r--r--   0        0        0      952 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/get_voices_response.py
+-rw-r--r--   0        0        0      101 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/history.py
+-rw-r--r--   0        0        0      991 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/history_item.py
+-rw-r--r--   0        0        0     1009 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/http_validation_error.py
+-rw-r--r--   0        0        0      947 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/invoice.py
+-rw-r--r--   0        0        0      930 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/language_response.py
+-rw-r--r--   0        0        0     1764 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/library_voice_response.py
+-rw-r--r--   0        0        0     1010 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/manual_verification_file_response.py
+-rw-r--r--   0        0        0     1085 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/manual_verification_response.py
+-rw-r--r--   0        0        0     1670 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/model.py
+-rw-r--r--   0        0        0     2215 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/normalized_alignment.py
+-rw-r--r--   0        0        0      173 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/optimize_streaming_latency.py
+-rw-r--r--   0        0        0      405 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/output_format.py
+-rw-r--r--   0        0        0     1277 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/project_extended_response_model.py
+-rw-r--r--   0        0        0     1258 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/project_response.py
+-rw-r--r--   0        0        0      990 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/project_snapshot_response.py
+-rw-r--r--   0        0        0     1018 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/project_snapshots_response.py
+-rw-r--r--   0        0        0      161 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/project_state.py
+-rw-r--r--   0        0        0      965 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/pronunciation_dictionary_alias_rule_request_model.py
+-rw-r--r--   0        0        0      987 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/pronunciation_dictionary_phoneme_rule_request_model.py
+-rw-r--r--   0        0        0      973 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/pronunciation_dictionary_version_locator.py
+-rw-r--r--   0        0        0     1488 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/realtime_voice_settings.py
+-rw-r--r--   0        0        0     1006 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/recording_response.py
+-rw-r--r--   0        0        0      958 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/remove_pronunciation_dictionary_rules_response_model.py
+-rw-r--r--   0        0        0      217 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/review_status.py
+-rw-r--r--   0        0        0     2361 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/send_text.py
+-rw-r--r--   0        0        0      144 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/source.py
+-rw-r--r--   0        0        0     1864 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/speech_history_item_response.py
+-rw-r--r--   0        0        0      223 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/speech_history_item_response_model_voice_category.py
+-rw-r--r--   0        0        0     1078 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/sso_provider_db_model.py
+-rw-r--r--   0        0        0      170 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/sso_provider_db_model_provider_type.py
+-rw-r--r--   0        0        0     1878 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/subscription.py
+-rw-r--r--   0        0        0     1610 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/subscription_response.py
+-rw-r--r--   0        0        0      197 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/subscription_response_model_billing_period.py
+-rw-r--r--   0        0        0      253 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/subscription_status.py
+-rw-r--r--   0        0        0     1140 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/user.py
+-rw-r--r--   0        0        0     1028 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     1119 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/verification_attempt_response.py
+-rw-r--r--   0        0        0     2088 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/voice.py
+-rw-r--r--   0        0        0      945 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/voice_generation_parameter_option_response.py
+-rw-r--r--   0        0        0     1324 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/voice_generation_parameter_response.py
+-rw-r--r--   0        0        0      213 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/voice_response_model_safety_control.py
+-rw-r--r--   0        0        0     1101 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/voice_sample.py
+-rw-r--r--   0        0        0     1082 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/voice_settings.py
+-rw-r--r--   0        0        0     2484 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/voice_sharing_response.py
+-rw-r--r--   0        0        0      193 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/voice_sharing_state.py
+-rw-r--r--   0        0        0     1244 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/types/voice_verification_response.py
+-rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/user/__init__.py
+-rw-r--r--   0        0        0     9597 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/user/client.py
+-rw-r--r--   0        0        0       78 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/version.py
+-rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/voice_generation/__init__.py
+-rw-r--r--   0        0        0    21042 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/voice_generation/client.py
+-rw-r--r--   0        0        0       65 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/voices/__init__.py
+-rw-r--r--   0        0        0    62413 2024-04-30 13:13:46.463825 elevenlabs-1.2.1/src/elevenlabs/voices/client.py
+-rw-r--r--   0        0        0     9958 1970-01-01 00:00:00.000000 elevenlabs-1.2.1/PKG-INFO
```

### Comparing `elevenlabs-1.2.0/LICENSE` & `elevenlabs-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/README.md` & `elevenlabs-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/pyproject.toml` & `elevenlabs-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elevenlabs"
-version = "v1.2.0"
+version = "v1.2.1"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "elevenlabs", from = "src"}
 ]
```

### Comparing `elevenlabs-1.2.0/src/elevenlabs/__init__.py` & `elevenlabs-1.2.1/src/elevenlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/audio_native/client.py` & `elevenlabs-1.2.1/src/elevenlabs/audio_native/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/base_client.py` & `elevenlabs-1.2.1/src/elevenlabs/base_client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/chapters/client.py` & `elevenlabs-1.2.1/src/elevenlabs/chapters/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/client.py` & `elevenlabs-1.2.1/src/elevenlabs/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/core/__init__.py` & `elevenlabs-1.2.1/src/elevenlabs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/core/client_wrapper.py` & `elevenlabs-1.2.1/src/elevenlabs/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "elevenlabs",
-            "X-Fern-SDK-Version": "v1.2.0",
+            "X-Fern-SDK-Version": "v1.2.1",
         }
         if self._api_key is not None:
             headers["xi-api-key"] = self._api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `elevenlabs-1.2.0/src/elevenlabs/core/datetime_utils.py` & `elevenlabs-1.2.1/src/elevenlabs/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/core/file.py` & `elevenlabs-1.2.1/src/elevenlabs/core/file.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/core/http_client.py` & `elevenlabs-1.2.1/src/elevenlabs/core/http_client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/core/jsonable_encoder.py` & `elevenlabs-1.2.1/src/elevenlabs/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/core/request_options.py` & `elevenlabs-1.2.1/src/elevenlabs/core/request_options.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/core/unchecked_base_model.py` & `elevenlabs-1.2.1/src/elevenlabs/core/unchecked_base_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/dubbing/client.py` & `elevenlabs-1.2.1/src/elevenlabs/dubbing/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/history/client.py` & `elevenlabs-1.2.1/src/elevenlabs/history/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/models/client.py` & `elevenlabs-1.2.1/src/elevenlabs/models/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/play.py` & `elevenlabs-1.2.1/src/elevenlabs/play.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/projects/client.py` & `elevenlabs-1.2.1/src/elevenlabs/projects/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,15 +435,15 @@
     def stream_audio(
         self,
         project_id: str,
         project_snapshot_id: str,
         *,
         convert_to_mpeg: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> None:
+    ) -> typing.Iterator[bytes]:
         """
         Stream the audio from a project snapshot.
 
         Parameters:
             - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
 
             - project_snapshot_id: str. The project_snapshot_id of the project snapshot. You can query GET /v1/projects/{project_id}/snapshots to list all available snapshots for a project.
@@ -454,22 +454,23 @@
         ---
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
         client.projects.stream_audio(
-            project_id="project_id",
-            project_snapshot_id="project_snapshot_id",
+            project_id="string",
+            project_snapshot_id="string",
+            convert_to_mpeg=True,
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if convert_to_mpeg is not OMIT:
             _request["convert_to_mpeg"] = convert_to_mpeg
-        _response = self._client_wrapper.httpx_client.request(
+        with self._client_wrapper.httpx_client.stream(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/projects/{jsonable_encoder(project_id)}/snapshots/{jsonable_encoder(project_snapshot_id)}/stream",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
@@ -489,26 +490,29 @@
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 422:
-            raise UnprocessableEntityError(
-                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+        ) as _response:
+            if 200 <= _response.status_code < 300:
+                for _chunk in _response.iter_bytes():
+                    yield _chunk
+                return
+            _response.read()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+                )
+            try:
+                _response_json = _response.json()
+            except JSONDecodeError:
+                raise ApiError(status_code=_response.status_code, body=_response.text)
+            raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def stream_archive(
         self, project_id: str, project_snapshot_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> None:
         """
         Streams archive with project audio.
 
@@ -1054,15 +1058,15 @@
     async def stream_audio(
         self,
         project_id: str,
         project_snapshot_id: str,
         *,
         convert_to_mpeg: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> None:
+    ) -> typing.AsyncIterator[bytes]:
         """
         Stream the audio from a project snapshot.
 
         Parameters:
             - project_id: str. The project_id of the project, you can query GET https://api.elevenlabs.io/v1/projects to list all available projects.
 
             - project_snapshot_id: str. The project_snapshot_id of the project snapshot. You can query GET /v1/projects/{project_id}/snapshots to list all available snapshots for a project.
@@ -1073,22 +1077,23 @@
         ---
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
         await client.projects.stream_audio(
-            project_id="project_id",
-            project_snapshot_id="project_snapshot_id",
+            project_id="string",
+            project_snapshot_id="string",
+            convert_to_mpeg=True,
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if convert_to_mpeg is not OMIT:
             _request["convert_to_mpeg"] = convert_to_mpeg
-        _response = await self._client_wrapper.httpx_client.request(
+        async with self._client_wrapper.httpx_client.stream(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/projects/{jsonable_encoder(project_id)}/snapshots/{jsonable_encoder(project_snapshot_id)}/stream",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
@@ -1108,26 +1113,29 @@
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 422:
-            raise UnprocessableEntityError(
-                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+        ) as _response:
+            if 200 <= _response.status_code < 300:
+                async for _chunk in _response.aiter_bytes():
+                    yield _chunk
+                return
+            await _response.aread()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+                )
+            try:
+                _response_json = _response.json()
+            except JSONDecodeError:
+                raise ApiError(status_code=_response.status_code, body=_response.text)
+            raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def stream_archive(
         self, project_id: str, project_snapshot_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> None:
         """
         Streams archive with project audio.
```

### Comparing `elevenlabs-1.2.0/src/elevenlabs/pronunciation_dictionary/client.py` & `elevenlabs-1.2.1/src/elevenlabs/pronunciation_dictionary/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/pronunciation_dictionary/types/pronunciation_dictionary_rule.py` & `elevenlabs-1.2.1/src/elevenlabs/pronunciation_dictionary/types/pronunciation_dictionary_rule.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/realtime_tts.py` & `elevenlabs-1.2.1/src/elevenlabs/realtime_tts.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/samples/client.py` & `elevenlabs-1.2.1/src/elevenlabs/samples/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/speech_to_speech/client.py` & `elevenlabs-1.2.1/src/elevenlabs/speech_to_speech/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/text_to_speech/client.py` & `elevenlabs-1.2.1/src/elevenlabs/text_to_speech/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/__init__.py` & `elevenlabs-1.2.1/src/elevenlabs/types/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/add_project_response_model.py` & `elevenlabs-1.2.1/src/elevenlabs/types/add_project_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py` & `elevenlabs-1.2.1/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/add_pronunciation_dictionary_rules_response_model.py` & `elevenlabs-1.2.1/src/elevenlabs/types/add_pronunciation_dictionary_rules_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/add_voice_response_model.py` & `elevenlabs-1.2.1/src/elevenlabs/types/add_voice_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/audio_native_create_project_response_model.py` & `elevenlabs-1.2.1/src/elevenlabs/types/audio_native_create_project_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/audio_output.py` & `elevenlabs-1.2.1/src/elevenlabs/types/audio_output.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/chapter_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/chapter_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/chapter_snapshot_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/chapter_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/chapter_snapshots_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/chapter_snapshots_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/chapter_statistics_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/chapter_statistics_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/do_dubbing_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/do_dubbing_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/dubbing_metadata_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/dubbing_metadata_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/feedback_item.py` & `elevenlabs-1.2.1/src/elevenlabs/types/feedback_item.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/fine_tuning_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/fine_tuning_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/generation_config.py` & `elevenlabs-1.2.1/src/elevenlabs/types/generation_config.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/get_chapters_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/get_chapters_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/get_library_voices_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/get_library_voices_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/get_projects_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/get_projects_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/get_pronunciation_dictionaries_metadata_response_model.py` & `elevenlabs-1.2.1/src/elevenlabs/types/get_pronunciation_dictionaries_metadata_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/get_speech_history_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/get_speech_history_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/get_voices_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/get_voices_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/history_item.py` & `elevenlabs-1.2.1/src/elevenlabs/types/history_item.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/http_validation_error.py` & `elevenlabs-1.2.1/src/elevenlabs/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/invoice.py` & `elevenlabs-1.2.1/src/elevenlabs/types/invoice.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/language_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/language_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/library_voice_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/library_voice_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/manual_verification_file_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/manual_verification_file_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/manual_verification_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/manual_verification_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/model.py` & `elevenlabs-1.2.1/src/elevenlabs/types/model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/normalized_alignment.py` & `elevenlabs-1.2.1/src/elevenlabs/types/normalized_alignment.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/project_extended_response_model.py` & `elevenlabs-1.2.1/src/elevenlabs/types/project_extended_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/project_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/project_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/project_snapshot_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/project_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/project_snapshots_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/project_snapshots_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/pronunciation_dictionary_alias_rule_request_model.py` & `elevenlabs-1.2.1/src/elevenlabs/types/pronunciation_dictionary_alias_rule_request_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/pronunciation_dictionary_phoneme_rule_request_model.py` & `elevenlabs-1.2.1/src/elevenlabs/types/pronunciation_dictionary_phoneme_rule_request_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/pronunciation_dictionary_version_locator.py` & `elevenlabs-1.2.1/src/elevenlabs/types/pronunciation_dictionary_version_locator.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/realtime_voice_settings.py` & `elevenlabs-1.2.1/src/elevenlabs/types/realtime_voice_settings.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/recording_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/recording_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/remove_pronunciation_dictionary_rules_response_model.py` & `elevenlabs-1.2.1/src/elevenlabs/types/remove_pronunciation_dictionary_rules_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/send_text.py` & `elevenlabs-1.2.1/src/elevenlabs/types/send_text.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/speech_history_item_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/speech_history_item_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/sso_provider_db_model.py` & `elevenlabs-1.2.1/src/elevenlabs/types/sso_provider_db_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/subscription.py` & `elevenlabs-1.2.1/src/elevenlabs/types/subscription.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/subscription_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/subscription_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/user.py` & `elevenlabs-1.2.1/src/elevenlabs/types/user.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/validation_error.py` & `elevenlabs-1.2.1/src/elevenlabs/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/verification_attempt_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/verification_attempt_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/voice.py` & `elevenlabs-1.2.1/src/elevenlabs/types/voice.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/voice_generation_parameter_option_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/voice_generation_parameter_option_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/voice_generation_parameter_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/voice_generation_parameter_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/voice_sample.py` & `elevenlabs-1.2.1/src/elevenlabs/types/voice_sample.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/voice_settings.py` & `elevenlabs-1.2.1/src/elevenlabs/types/voice_settings.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/voice_sharing_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/voice_sharing_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/types/voice_verification_response.py` & `elevenlabs-1.2.1/src/elevenlabs/types/voice_verification_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/user/client.py` & `elevenlabs-1.2.1/src/elevenlabs/user/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/voice_generation/client.py` & `elevenlabs-1.2.1/src/elevenlabs/voice_generation/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/src/elevenlabs/voices/client.py` & `elevenlabs-1.2.1/src/elevenlabs/voices/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.2.0/PKG-INFO` & `elevenlabs-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 1.2.0
+Version: 1.2.1
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

