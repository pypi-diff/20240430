# Comparing `tmp/embyclient-4.8.5.0.tar.gz` & `tmp/embyclient-4.8.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embyclient-4.8.5.0.tar", last modified: Sun Apr 21 16:05:17 2024, max compression
+gzip compressed data, was "embyclient-4.8.6.0.tar", last modified: Tue Apr 30 00:16:11 2024, max compression
```

## Comparing `embyclient-4.8.5.0.tar` & `embyclient-4.8.6.0.tar`

### file list

```diff
@@ -1,337 +1,337 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:05:17.885747 embyclient-4.8.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-21 16:05:17.881747 embyclient-4.8.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:05:17.825748 embyclient-4.8.5.0/embyclient/
--rw-r--r--   0 runner    (1001) docker     (127)    28759 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24584 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:05:17.881747 embyclient-4.8.5.0/embyclient/models/
--rw-r--r--   0 runner    (1001) docker     (127)    22941 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/access_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/actions_postback_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/activity_log_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/album_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/all_theme_media_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/api_available_recording_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    23808 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/api_base_items_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/api_configuration_page_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/api_epg_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/api_listing_provider_type_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/api_name_id_description_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/api_on_playback_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/api_set_channel_disabled.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/api_set_channel_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/api_set_channel_sort_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/api_tag_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    11105 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/artist_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/attributes_simple_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/attributes_value_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/authenticate_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/authenticate_user_by_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/authentication_authentication_result.py
--rw-r--r--   0 runner    (1001) docker     (127)   126488 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/base_item_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/base_item_person.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/bit_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/book_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/branding_branding_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/channel_management_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/chapter_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/client_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/codec_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/codec_directions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/codec_kinds.py
--rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/codec_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/codec_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/collections_collection_creation_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/color_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/common_editor_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7820 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/common_interfaces_i_codec_device_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/common_interfaces_i_codec_device_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/common_plugins_i_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/conditions_property_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/conditions_property_condition_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    14728 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/configuration_tone_mapping_tone_map_options_visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/connect_connect_authentication_exchange_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/connect_user_link_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/connect_user_link_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/container_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/create_user_by_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/day_of_week.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/default_directory_browser_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13068 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/device_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/devices_content_upload_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/devices_device_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/devices_device_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/devices_local_file_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/direct_play_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/display_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/dlna_profile_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    10689 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/dlna_profiles_device_identification.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/dlna_profiles_device_profile_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    37624 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/dlna_profiles_dlna_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/dlna_profiles_header_match_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/dlna_profiles_http_header_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/dlna_profiles_protocol_info_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/drawing_image_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/dynamic_day_of_week.py
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/edit_object_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/editors_editor_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/editors_editor_button_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    13141 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/editors_editor_root.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/encoding_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/enums_ui_command_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/enums_ui_view_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/extended_video_sub_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/extended_video_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/external_id_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/external_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/feature_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/feature_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/forgot_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/forgot_password_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/forgot_password_pin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/forgot_password_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/game_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/general_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/generic_edit_i_edit_object_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/get_directory_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/globalization_country_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/globalization_culture_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/globalization_localizaton_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/image_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/image_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/image_provider_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/image_saving_convention.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/image_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/installation_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/io_file_system_entry_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/io_file_system_entry_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/item_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/item_file_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/item_file_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/item_lookup_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    10833 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/level_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/library_add_media_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/library_add_virtual_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/library_delete_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/library_item_link_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/library_library_option_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/library_library_options_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/library_library_type_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/library_media_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/library_media_update_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    60338 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/library_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/library_post_updated_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/library_remove_media_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/library_remove_virtual_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/library_rename_virtual_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/library_sub_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/library_update_library_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/library_update_media_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/library_user_copy_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/live_stream_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/live_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/live_tv_channel_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/live_tv_guide_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/live_tv_keep_until.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/live_tv_keyword_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/live_tv_keyword_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    18555 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/live_tv_listings_provider_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/live_tv_live_tv_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/live_tv_recording_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    25872 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/live_tv_series_timer_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    37492 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/live_tv_series_timer_info_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)    24849 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/live_tv_timer_info_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/live_tv_timer_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    16394 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/live_tv_tuner_host_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/location_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/log_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/logging_log_severity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/marker_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/mb_backup_api_all_backups_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/mb_backup_api_data_restore_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/mb_backup_api_restore_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/mb_backup_api_user_restore_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/mb_backup_backup_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/media_encoding_codec_parameter_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/media_path_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/media_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    39926 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/media_source_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/media_source_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    58923 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/media_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/media_stream_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/media_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/metadata_editor_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/metadata_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/metadata_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/metadata_refresh_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    11057 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/movie_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/music_video_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/name_id_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/name_long_id_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/name_value_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/net_end_point_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/net_sockets_address_family.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/notification_category_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/notification_type_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/operating_system.py
--rw-r--r--   0 runner    (1001) docker     (127)    20362 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/package_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/package_target_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/package_version_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    11611 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/package_version_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/parental_rating.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/path_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/persistence_intro_debug_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/person_lookup_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/person_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/pin_redeem_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/play_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/play_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/play_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/playback_error_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    19970 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/playback_info_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/playback_info_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    25054 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/playback_progress_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    24718 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/playback_start_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13720 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/playback_stop_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    12504 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/player_state_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/playlists_add_to_playlist_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/playlists_playlist_creation_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/playstate_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/playstate_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/plugins_configuration_page_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/plugins_plugin_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/process_run_metrics_process_metric_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/process_run_metrics_process_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/profile_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/profile_condition_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/profile_condition_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/profile_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/profile_level_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/progress_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/provider_id_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/proxy_header_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/public_system_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/query_result_activity_log_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/query_result_api_epg_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/query_result_base_item_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/query_result_channel_management_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/query_result_devices_device_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/query_result_live_tv_series_timer_info_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/query_result_live_tv_timer_info_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/query_result_log_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/query_result_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/query_result_sync_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/query_result_sync_job_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/query_result_user_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/query_result_user_library_official_rating_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/query_result_user_library_tag_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/query_result_virtual_folder_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/queue_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/rating_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/recommendation_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/recommendation_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    10630 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/remote_image_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/remote_image_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/remote_search_query_album_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/remote_search_query_artist_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/remote_search_query_book_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/remote_search_query_game_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/remote_search_query_item_lookup_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/remote_search_query_movie_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/remote_search_query_music_video_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/remote_search_query_person_lookup_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/remote_search_query_series_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/remote_search_query_trailer_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    15283 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/remote_search_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    12937 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/remote_subtitle_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/repeat_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/resolution_with_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/response_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/roku_metadata_api_thumbnail_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/roku_metadata_api_thumbnail_set_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/run_ui_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/secondary_frameworks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/segment_skip_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/series_display_order.py
--rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/series_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    66420 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/server_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    23279 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/session_session_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/session_user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13666 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/song_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/sort_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/subtitle_delivery_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/subtitle_location_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/subtitle_playback_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/subtitle_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/subtitles_subtitle_download_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/sync_category.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/sync_data_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/sync_data_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/sync_dialog_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    22445 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/sync_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/sync_job_creation_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/sync_job_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/sync_job_item_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/sync_job_option.py
--rw-r--r--   0 runner    (1001) docker     (127)    13292 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/sync_job_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/sync_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/sync_profile_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/sync_quality_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/sync_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/synced_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/synced_item_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/system_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    34832 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/system_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/task_completion_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/task_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/task_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/task_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/task_trigger_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/theme_media_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/trailer_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/transcode_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/transcode_seek_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    29815 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/transcoding_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    19145 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/transcoding_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/transcoding_vp_step_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/transcoding_vp_step_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/transport_stream_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/tuple_double_double.py
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/type_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/ui_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/ui_tab_page_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/ui_view_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/unrated_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/update_user_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/user_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/user_action_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    19873 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/user_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    18187 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/user_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/user_item_data_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/user_item_share_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/user_library_add_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/user_library_leave_shared_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/user_library_official_rating_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/user_library_remove_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/user_library_tag_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/user_library_update_user_item_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    13833 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/user_notification_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    45913 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/user_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/validate_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/video3_d_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    22765 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/video_codec_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/video_media_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/virtual_folder_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/models/wake_on_lan_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    12794 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/embyclient/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:05:17.881747 embyclient-4.8.5.0/embyclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-21 16:05:17.000000 embyclient-4.8.5.0/embyclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-04-21 16:05:17.000000 embyclient-4.8.5.0/embyclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 16:05:17.000000 embyclient-4.8.5.0/embyclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-21 16:05:17.000000 embyclient-4.8.5.0/embyclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-21 16:05:17.000000 embyclient-4.8.5.0/embyclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 16:05:17.885747 embyclient-4.8.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-21 16:05:11.000000 embyclient-4.8.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:16:11.480389 embyclient-4.8.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-30 00:16:11.480389 embyclient-4.8.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:16:11.428389 embyclient-4.8.6.0/embyclient/
+-rw-r--r--   0 runner    (1001) docker     (127)    28759 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24584 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:16:11.480389 embyclient-4.8.6.0/embyclient/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    22941 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/access_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/actions_postback_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/activity_log_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/album_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/all_theme_media_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/api_available_recording_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23808 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/api_base_items_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/api_configuration_page_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/api_epg_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/api_listing_provider_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/api_name_id_description_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/api_on_playback_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/api_set_channel_disabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/api_set_channel_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/api_set_channel_sort_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/api_tag_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11105 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/artist_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/attributes_simple_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/attributes_value_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/authenticate_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/authenticate_user_by_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/authentication_authentication_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)   126488 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/base_item_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/base_item_person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/bit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/book_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/branding_branding_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/channel_management_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/chapter_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/client_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/codec_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/codec_directions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/codec_kinds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/codec_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/codec_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/collections_collection_creation_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/color_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/common_editor_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7820 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/common_interfaces_i_codec_device_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/common_interfaces_i_codec_device_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/common_plugins_i_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/conditions_property_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/conditions_property_condition_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14728 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/configuration_tone_mapping_tone_map_options_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/connect_connect_authentication_exchange_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/connect_user_link_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/connect_user_link_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/container_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/create_user_by_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/day_of_week.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/default_directory_browser_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13068 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/device_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/devices_content_upload_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/devices_device_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/devices_device_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/devices_local_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/direct_play_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/display_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/dlna_profile_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10689 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/dlna_profiles_device_identification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/dlna_profiles_device_profile_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37624 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/dlna_profiles_dlna_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/dlna_profiles_header_match_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/dlna_profiles_http_header_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/dlna_profiles_protocol_info_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/drawing_image_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/dynamic_day_of_week.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/edit_object_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/editors_editor_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/editors_editor_button_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13141 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/editors_editor_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/encoding_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/enums_ui_command_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/enums_ui_view_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/extended_video_sub_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/extended_video_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/external_id_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/external_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/feature_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/forgot_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/forgot_password_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/forgot_password_pin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/forgot_password_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/game_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/general_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/generic_edit_i_edit_object_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/get_directory_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/globalization_country_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/globalization_culture_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/globalization_localizaton_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/image_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/image_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/image_provider_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/image_saving_convention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/image_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/installation_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/io_file_system_entry_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/io_file_system_entry_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/item_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/item_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/item_file_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/item_lookup_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10833 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/level_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/library_add_media_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/library_add_virtual_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/library_delete_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/library_item_link_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/library_library_option_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/library_library_options_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/library_library_type_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/library_media_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/library_media_update_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60338 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/library_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/library_post_updated_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/library_remove_media_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/library_remove_virtual_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/library_rename_virtual_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/library_sub_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/library_update_library_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/library_update_media_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/library_user_copy_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/live_stream_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/live_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/live_tv_channel_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/live_tv_guide_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/live_tv_keep_until.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/live_tv_keyword_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/live_tv_keyword_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18555 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/live_tv_listings_provider_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/live_tv_live_tv_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/live_tv_recording_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25872 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/live_tv_series_timer_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37492 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/live_tv_series_timer_info_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24849 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/live_tv_timer_info_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/live_tv_timer_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16394 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/live_tv_tuner_host_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/location_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/log_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/logging_log_severity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/marker_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/mb_backup_api_all_backups_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/mb_backup_api_data_restore_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/mb_backup_api_restore_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/mb_backup_api_user_restore_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/mb_backup_backup_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/media_encoding_codec_parameter_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/media_path_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/media_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39926 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/media_source_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/media_source_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58923 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/media_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/media_stream_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/media_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/metadata_editor_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/metadata_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/metadata_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/metadata_refresh_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11057 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/movie_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/music_video_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/name_id_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/name_long_id_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/name_value_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/net_end_point_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/net_sockets_address_family.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/notification_category_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/notification_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20362 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/package_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/package_target_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/package_version_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11611 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/package_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/parental_rating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/path_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/persistence_intro_debug_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/person_lookup_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/person_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/pin_redeem_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/play_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/play_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/play_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/playback_error_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19970 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/playback_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/playback_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25054 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/playback_progress_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24718 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/playback_start_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13720 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/playback_stop_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12504 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/player_state_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/playlists_add_to_playlist_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/playlists_playlist_creation_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/playstate_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/playstate_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/plugins_configuration_page_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/plugins_plugin_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/process_run_metrics_process_metric_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/process_run_metrics_process_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/profile_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/profile_condition_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/profile_condition_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/profile_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/profile_level_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/progress_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/provider_id_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/proxy_header_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/public_system_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/query_result_activity_log_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/query_result_api_epg_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/query_result_base_item_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/query_result_channel_management_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/query_result_devices_device_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/query_result_live_tv_series_timer_info_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/query_result_live_tv_timer_info_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/query_result_log_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/query_result_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/query_result_sync_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/query_result_sync_job_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/query_result_user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/query_result_user_library_official_rating_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/query_result_user_library_tag_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/query_result_virtual_folder_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/queue_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/rating_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/recommendation_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/recommendation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10630 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/remote_image_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/remote_image_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/remote_search_query_album_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/remote_search_query_artist_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/remote_search_query_book_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/remote_search_query_game_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/remote_search_query_item_lookup_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/remote_search_query_movie_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/remote_search_query_music_video_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/remote_search_query_person_lookup_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/remote_search_query_series_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/remote_search_query_trailer_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15283 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/remote_search_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12937 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/remote_subtitle_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/repeat_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/resolution_with_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/response_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/roku_metadata_api_thumbnail_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/roku_metadata_api_thumbnail_set_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/run_ui_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/secondary_frameworks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/segment_skip_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/series_display_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/series_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66579 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/server_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23279 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/session_session_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/session_user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13666 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/song_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/sort_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/subtitle_delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/subtitle_location_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/subtitle_playback_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/subtitle_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/subtitles_subtitle_download_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/sync_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/sync_data_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/sync_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/sync_dialog_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22445 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/sync_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/sync_job_creation_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/sync_job_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/sync_job_item_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/sync_job_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13292 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/sync_job_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/sync_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/sync_profile_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/sync_quality_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/sync_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/synced_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/synced_item_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/system_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34832 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/system_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/task_completion_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/task_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/task_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/task_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/task_trigger_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/theme_media_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/trailer_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/transcode_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/transcode_seek_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29815 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/transcoding_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19145 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/transcoding_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/transcoding_vp_step_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/transcoding_vp_step_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/transport_stream_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/tuple_double_double.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/type_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/ui_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/ui_tab_page_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/ui_view_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/unrated_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/update_user_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/user_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/user_action_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19873 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/user_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18187 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/user_item_data_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/user_item_share_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/user_library_add_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/user_library_leave_shared_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/user_library_official_rating_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/user_library_remove_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/user_library_tag_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/user_library_update_user_item_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13833 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/user_notification_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45913 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/user_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/validate_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/video3_d_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22765 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/video_codec_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/video_media_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/virtual_folder_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/models/wake_on_lan_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12794 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/embyclient/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:16:11.480389 embyclient-4.8.6.0/embyclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-30 00:16:11.000000 embyclient-4.8.6.0/embyclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-04-30 00:16:11.000000 embyclient-4.8.6.0/embyclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 00:16:11.000000 embyclient-4.8.6.0/embyclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 00:16:11.000000 embyclient-4.8.6.0/embyclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 00:16:11.000000 embyclient-4.8.6.0/embyclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 00:16:11.480389 embyclient-4.8.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-30 00:15:59.000000 embyclient-4.8.6.0/setup.py
```

### Comparing `embyclient-4.8.5.0/PKG-INFO` & `embyclient-4.8.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embyclient
-Version: 4.8.5.0
+Version: 4.8.6.0
 Summary: A Python client for Emby Media Server's API
 Home-page: https://emby.media
 Keywords: Emby,Rest,API,client,media,server,JSON
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Multimedia
```

### Comparing `embyclient-4.8.5.0/README.md` & `embyclient-4.8.6.0/README.md`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/__init__.py` & `embyclient-4.8.6.0/embyclient/__init__.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/api_client.py` & `embyclient-4.8.6.0/embyclient/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = '/4.8.5.0/python'
+        self.user_agent = '/4.8.6.0/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `embyclient-4.8.5.0/embyclient/configuration.py` & `embyclient-4.8.6.0/embyclient/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,10 +234,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 4.8.5.0\n"\
-               "SDK Package Version: 4.8.5.0".\
+               "Version of the API: 4.8.6.0\n"\
+               "SDK Package Version: 4.8.6.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `embyclient-4.8.5.0/embyclient/models/__init__.py` & `embyclient-4.8.6.0/embyclient/models/__init__.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/access_schedule.py` & `embyclient-4.8.6.0/embyclient/models/access_schedule.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/actions_postback_action.py` & `embyclient-4.8.6.0/embyclient/models/actions_postback_action.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/activity_log_entry.py` & `embyclient-4.8.6.0/embyclient/models/activity_log_entry.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/album_info.py` & `embyclient-4.8.6.0/embyclient/models/album_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/all_theme_media_result.py` & `embyclient-4.8.6.0/embyclient/models/all_theme_media_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/api_available_recording_options.py` & `embyclient-4.8.6.0/embyclient/models/api_available_recording_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/api_base_items_request.py` & `embyclient-4.8.6.0/embyclient/models/api_base_items_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/api_configuration_page_info.py` & `embyclient-4.8.6.0/embyclient/models/api_configuration_page_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/api_epg_row.py` & `embyclient-4.8.6.0/embyclient/models/api_epg_row.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/api_listing_provider_type_info.py` & `embyclient-4.8.6.0/embyclient/models/api_listing_provider_type_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/api_name_id_description_pair.py` & `embyclient-4.8.6.0/embyclient/models/api_name_id_description_pair.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/api_on_playback_progress.py` & `embyclient-4.8.6.0/embyclient/models/api_on_playback_progress.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/api_set_channel_disabled.py` & `embyclient-4.8.6.0/embyclient/models/api_set_channel_disabled.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/api_set_channel_mapping.py` & `embyclient-4.8.6.0/embyclient/models/api_set_channel_mapping.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/api_set_channel_sort_index.py` & `embyclient-4.8.6.0/embyclient/models/api_set_channel_sort_index.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/api_tag_item.py` & `embyclient-4.8.6.0/embyclient/models/api_tag_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/artist_info.py` & `embyclient-4.8.6.0/embyclient/models/artist_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/attributes_simple_condition.py` & `embyclient-4.8.6.0/embyclient/models/attributes_simple_condition.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/attributes_value_condition.py` & `embyclient-4.8.6.0/embyclient/models/attributes_value_condition.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/authenticate_user.py` & `embyclient-4.8.6.0/embyclient/models/authenticate_user.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/authenticate_user_by_name.py` & `embyclient-4.8.6.0/embyclient/models/authenticate_user_by_name.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/authentication_authentication_result.py` & `embyclient-4.8.6.0/embyclient/models/authentication_authentication_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/base_item_dto.py` & `embyclient-4.8.6.0/embyclient/models/base_item_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/base_item_person.py` & `embyclient-4.8.6.0/embyclient/models/base_item_person.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/bit_rate.py` & `embyclient-4.8.6.0/embyclient/models/bit_rate.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/book_info.py` & `embyclient-4.8.6.0/embyclient/models/book_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/branding_branding_options.py` & `embyclient-4.8.6.0/embyclient/models/branding_branding_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/channel_management_info.py` & `embyclient-4.8.6.0/embyclient/models/channel_management_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/chapter_info.py` & `embyclient-4.8.6.0/embyclient/models/chapter_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/client_capabilities.py` & `embyclient-4.8.6.0/embyclient/models/client_capabilities.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/codec_configuration.py` & `embyclient-4.8.6.0/embyclient/models/codec_configuration.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/codec_directions.py` & `embyclient-4.8.6.0/embyclient/models/codec_directions.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/codec_kinds.py` & `embyclient-4.8.6.0/embyclient/models/codec_kinds.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/codec_profile.py` & `embyclient-4.8.6.0/embyclient/models/codec_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/codec_type.py` & `embyclient-4.8.6.0/embyclient/models/codec_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/collections_collection_creation_result.py` & `embyclient-4.8.6.0/embyclient/models/collections_collection_creation_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/color_formats.py` & `embyclient-4.8.6.0/embyclient/models/color_formats.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/common_editor_types.py` & `embyclient-4.8.6.0/embyclient/models/common_editor_types.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/common_interfaces_i_codec_device_capabilities.py` & `embyclient-4.8.6.0/embyclient/models/common_interfaces_i_codec_device_capabilities.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/common_interfaces_i_codec_device_info.py` & `embyclient-4.8.6.0/embyclient/models/common_interfaces_i_codec_device_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/common_plugins_i_plugin.py` & `embyclient-4.8.6.0/embyclient/models/common_plugins_i_plugin.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/conditions_property_condition.py` & `embyclient-4.8.6.0/embyclient/models/conditions_property_condition.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/conditions_property_condition_type.py` & `embyclient-4.8.6.0/embyclient/models/conditions_property_condition_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/configuration_tone_mapping_tone_map_options_visibility.py` & `embyclient-4.8.6.0/embyclient/models/configuration_tone_mapping_tone_map_options_visibility.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/connect_connect_authentication_exchange_result.py` & `embyclient-4.8.6.0/embyclient/models/connect_connect_authentication_exchange_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/connect_user_link_result.py` & `embyclient-4.8.6.0/embyclient/models/connect_user_link_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/connect_user_link_type.py` & `embyclient-4.8.6.0/embyclient/models/connect_user_link_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/container_profile.py` & `embyclient-4.8.6.0/embyclient/models/container_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/create_user_by_name.py` & `embyclient-4.8.6.0/embyclient/models/create_user_by_name.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/day_of_week.py` & `embyclient-4.8.6.0/embyclient/models/day_of_week.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/default_directory_browser_info.py` & `embyclient-4.8.6.0/embyclient/models/default_directory_browser_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/device_profile.py` & `embyclient-4.8.6.0/embyclient/models/device_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/devices_content_upload_history.py` & `embyclient-4.8.6.0/embyclient/models/devices_content_upload_history.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/devices_device_info.py` & `embyclient-4.8.6.0/embyclient/models/devices_device_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/devices_device_options.py` & `embyclient-4.8.6.0/embyclient/models/devices_device_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/devices_local_file_info.py` & `embyclient-4.8.6.0/embyclient/models/devices_local_file_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/direct_play_profile.py` & `embyclient-4.8.6.0/embyclient/models/direct_play_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/display_preferences.py` & `embyclient-4.8.6.0/embyclient/models/display_preferences.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/dlna_profile_type.py` & `embyclient-4.8.6.0/embyclient/models/dlna_profile_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/dlna_profiles_device_identification.py` & `embyclient-4.8.6.0/embyclient/models/dlna_profiles_device_identification.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/dlna_profiles_device_profile_type.py` & `embyclient-4.8.6.0/embyclient/models/dlna_profiles_device_profile_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/dlna_profiles_dlna_profile.py` & `embyclient-4.8.6.0/embyclient/models/dlna_profiles_dlna_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/dlna_profiles_header_match_type.py` & `embyclient-4.8.6.0/embyclient/models/dlna_profiles_header_match_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/dlna_profiles_http_header_info.py` & `embyclient-4.8.6.0/embyclient/models/dlna_profiles_http_header_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/dlna_profiles_protocol_info_detection.py` & `embyclient-4.8.6.0/embyclient/models/dlna_profiles_protocol_info_detection.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/drawing_image_orientation.py` & `embyclient-4.8.6.0/embyclient/models/drawing_image_orientation.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/dynamic_day_of_week.py` & `embyclient-4.8.6.0/embyclient/models/dynamic_day_of_week.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/edit_object_container.py` & `embyclient-4.8.6.0/embyclient/models/edit_object_container.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/editors_editor_base.py` & `embyclient-4.8.6.0/embyclient/models/editors_editor_base.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/editors_editor_button_item.py` & `embyclient-4.8.6.0/embyclient/models/editors_editor_button_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/editors_editor_root.py` & `embyclient-4.8.6.0/embyclient/models/editors_editor_root.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/encoding_context.py` & `embyclient-4.8.6.0/embyclient/models/encoding_context.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/enums_ui_command_type.py` & `embyclient-4.8.6.0/embyclient/models/enums_ui_command_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/enums_ui_view_type.py` & `embyclient-4.8.6.0/embyclient/models/enums_ui_view_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/extended_video_sub_types.py` & `embyclient-4.8.6.0/embyclient/models/extended_video_sub_types.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/extended_video_types.py` & `embyclient-4.8.6.0/embyclient/models/extended_video_types.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/external_id_info.py` & `embyclient-4.8.6.0/embyclient/models/external_id_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/external_url.py` & `embyclient-4.8.6.0/embyclient/models/external_url.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/feature_info.py` & `embyclient-4.8.6.0/embyclient/models/feature_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/feature_type.py` & `embyclient-4.8.6.0/embyclient/models/feature_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/forgot_password.py` & `embyclient-4.8.6.0/embyclient/models/forgot_password.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/forgot_password_action.py` & `embyclient-4.8.6.0/embyclient/models/forgot_password_action.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/forgot_password_pin.py` & `embyclient-4.8.6.0/embyclient/models/forgot_password_pin.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/forgot_password_result.py` & `embyclient-4.8.6.0/embyclient/models/forgot_password_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/game_info.py` & `embyclient-4.8.6.0/embyclient/models/game_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/general_command.py` & `embyclient-4.8.6.0/embyclient/models/general_command.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/generic_edit_i_edit_object_container.py` & `embyclient-4.8.6.0/embyclient/models/generic_edit_i_edit_object_container.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/get_directory_contents.py` & `embyclient-4.8.6.0/embyclient/models/get_directory_contents.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/globalization_country_info.py` & `embyclient-4.8.6.0/embyclient/models/globalization_country_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/globalization_culture_dto.py` & `embyclient-4.8.6.0/embyclient/models/globalization_culture_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/globalization_localizaton_option.py` & `embyclient-4.8.6.0/embyclient/models/globalization_localizaton_option.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/image_info.py` & `embyclient-4.8.6.0/embyclient/models/image_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/image_option.py` & `embyclient-4.8.6.0/embyclient/models/image_option.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/image_provider_info.py` & `embyclient-4.8.6.0/embyclient/models/image_provider_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/image_saving_convention.py` & `embyclient-4.8.6.0/embyclient/models/image_saving_convention.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/image_type.py` & `embyclient-4.8.6.0/embyclient/models/image_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/installation_info.py` & `embyclient-4.8.6.0/embyclient/models/installation_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/io_file_system_entry_info.py` & `embyclient-4.8.6.0/embyclient/models/io_file_system_entry_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/io_file_system_entry_type.py` & `embyclient-4.8.6.0/embyclient/models/io_file_system_entry_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/item_counts.py` & `embyclient-4.8.6.0/embyclient/models/item_counts.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/item_file_info.py` & `embyclient-4.8.6.0/embyclient/models/item_file_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/item_file_type.py` & `embyclient-4.8.6.0/embyclient/models/item_file_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/item_lookup_info.py` & `embyclient-4.8.6.0/embyclient/models/item_lookup_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/level_information.py` & `embyclient-4.8.6.0/embyclient/models/level_information.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/library_add_media_path.py` & `embyclient-4.8.6.0/embyclient/models/library_add_media_path.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/library_add_virtual_folder.py` & `embyclient-4.8.6.0/embyclient/models/library_add_virtual_folder.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/library_delete_info.py` & `embyclient-4.8.6.0/embyclient/models/library_delete_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/library_item_link_type.py` & `embyclient-4.8.6.0/embyclient/models/library_item_link_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/library_library_option_info.py` & `embyclient-4.8.6.0/embyclient/models/library_library_option_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/library_library_options_result.py` & `embyclient-4.8.6.0/embyclient/models/library_library_options_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/library_library_type_options.py` & `embyclient-4.8.6.0/embyclient/models/library_library_type_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/library_media_folder.py` & `embyclient-4.8.6.0/embyclient/models/library_media_folder.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/library_media_update_info.py` & `embyclient-4.8.6.0/embyclient/models/library_media_update_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/library_options.py` & `embyclient-4.8.6.0/embyclient/models/library_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/library_post_updated_media.py` & `embyclient-4.8.6.0/embyclient/models/library_post_updated_media.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/library_remove_media_path.py` & `embyclient-4.8.6.0/embyclient/models/library_remove_media_path.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/library_remove_virtual_folder.py` & `embyclient-4.8.6.0/embyclient/models/library_remove_virtual_folder.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/library_rename_virtual_folder.py` & `embyclient-4.8.6.0/embyclient/models/library_rename_virtual_folder.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/library_sub_folder.py` & `embyclient-4.8.6.0/embyclient/models/library_sub_folder.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/library_update_library_options.py` & `embyclient-4.8.6.0/embyclient/models/library_update_library_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/library_update_media_path.py` & `embyclient-4.8.6.0/embyclient/models/library_update_media_path.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/library_user_copy_options.py` & `embyclient-4.8.6.0/embyclient/models/library_user_copy_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/live_stream_request.py` & `embyclient-4.8.6.0/embyclient/models/live_stream_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/live_stream_response.py` & `embyclient-4.8.6.0/embyclient/models/live_stream_response.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/live_tv_channel_type.py` & `embyclient-4.8.6.0/embyclient/models/live_tv_channel_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/live_tv_guide_info.py` & `embyclient-4.8.6.0/embyclient/models/live_tv_guide_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/live_tv_keep_until.py` & `embyclient-4.8.6.0/embyclient/models/live_tv_keep_until.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/live_tv_keyword_info.py` & `embyclient-4.8.6.0/embyclient/models/live_tv_keyword_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/live_tv_keyword_type.py` & `embyclient-4.8.6.0/embyclient/models/live_tv_keyword_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/live_tv_listings_provider_info.py` & `embyclient-4.8.6.0/embyclient/models/live_tv_listings_provider_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/live_tv_live_tv_info.py` & `embyclient-4.8.6.0/embyclient/models/live_tv_live_tv_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/live_tv_recording_status.py` & `embyclient-4.8.6.0/embyclient/models/live_tv_recording_status.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/live_tv_series_timer_info.py` & `embyclient-4.8.6.0/embyclient/models/live_tv_series_timer_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/live_tv_series_timer_info_dto.py` & `embyclient-4.8.6.0/embyclient/models/live_tv_series_timer_info_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/live_tv_timer_info_dto.py` & `embyclient-4.8.6.0/embyclient/models/live_tv_timer_info_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/live_tv_timer_type.py` & `embyclient-4.8.6.0/embyclient/models/live_tv_timer_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/live_tv_tuner_host_info.py` & `embyclient-4.8.6.0/embyclient/models/live_tv_tuner_host_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/location_type.py` & `embyclient-4.8.6.0/embyclient/models/location_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/log_file.py` & `embyclient-4.8.6.0/embyclient/models/log_file.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/logging_log_severity.py` & `embyclient-4.8.6.0/embyclient/models/logging_log_severity.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/marker_type.py` & `embyclient-4.8.6.0/embyclient/models/marker_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/mb_backup_api_all_backups_info.py` & `embyclient-4.8.6.0/embyclient/models/mb_backup_api_all_backups_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/mb_backup_api_data_restore_options.py` & `embyclient-4.8.6.0/embyclient/models/mb_backup_api_data_restore_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/mb_backup_api_restore_options.py` & `embyclient-4.8.6.0/embyclient/models/mb_backup_api_restore_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/mb_backup_api_user_restore_info.py` & `embyclient-4.8.6.0/embyclient/models/mb_backup_api_user_restore_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/mb_backup_backup_info.py` & `embyclient-4.8.6.0/embyclient/models/mb_backup_backup_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/media_encoding_codec_parameter_context.py` & `embyclient-4.8.6.0/embyclient/models/media_encoding_codec_parameter_context.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/media_path_info.py` & `embyclient-4.8.6.0/embyclient/models/media_path_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/media_protocol.py` & `embyclient-4.8.6.0/embyclient/models/media_protocol.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/media_source_info.py` & `embyclient-4.8.6.0/embyclient/models/media_source_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/media_source_type.py` & `embyclient-4.8.6.0/embyclient/models/media_source_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/media_stream.py` & `embyclient-4.8.6.0/embyclient/models/media_stream.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/media_stream_type.py` & `embyclient-4.8.6.0/embyclient/models/media_stream_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/media_url.py` & `embyclient-4.8.6.0/embyclient/models/media_url.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/metadata_editor_info.py` & `embyclient-4.8.6.0/embyclient/models/metadata_editor_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/metadata_features.py` & `embyclient-4.8.6.0/embyclient/models/metadata_features.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/metadata_fields.py` & `embyclient-4.8.6.0/embyclient/models/metadata_fields.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/metadata_refresh_mode.py` & `embyclient-4.8.6.0/embyclient/models/metadata_refresh_mode.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/movie_info.py` & `embyclient-4.8.6.0/embyclient/models/movie_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/music_video_info.py` & `embyclient-4.8.6.0/embyclient/models/music_video_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/name_id_pair.py` & `embyclient-4.8.6.0/embyclient/models/name_id_pair.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/name_long_id_pair.py` & `embyclient-4.8.6.0/embyclient/models/name_long_id_pair.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/name_value_pair.py` & `embyclient-4.8.6.0/embyclient/models/name_value_pair.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/net_end_point_info.py` & `embyclient-4.8.6.0/embyclient/models/net_end_point_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/net_sockets_address_family.py` & `embyclient-4.8.6.0/embyclient/models/net_sockets_address_family.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/notification_category_info.py` & `embyclient-4.8.6.0/embyclient/models/notification_category_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/notification_type_info.py` & `embyclient-4.8.6.0/embyclient/models/notification_type_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/operating_system.py` & `embyclient-4.8.6.0/embyclient/models/operating_system.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/package_info.py` & `embyclient-4.8.6.0/embyclient/models/package_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/package_target_system.py` & `embyclient-4.8.6.0/embyclient/models/package_target_system.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/package_version_class.py` & `embyclient-4.8.6.0/embyclient/models/package_version_class.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/package_version_info.py` & `embyclient-4.8.6.0/embyclient/models/package_version_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/parental_rating.py` & `embyclient-4.8.6.0/embyclient/models/parental_rating.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/path_substitution.py` & `embyclient-4.8.6.0/embyclient/models/path_substitution.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/persistence_intro_debug_info.py` & `embyclient-4.8.6.0/embyclient/models/persistence_intro_debug_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/person_lookup_info.py` & `embyclient-4.8.6.0/embyclient/models/person_lookup_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/person_type.py` & `embyclient-4.8.6.0/embyclient/models/person_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/pin_redeem_result.py` & `embyclient-4.8.6.0/embyclient/models/pin_redeem_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/play_command.py` & `embyclient-4.8.6.0/embyclient/models/play_command.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/play_method.py` & `embyclient-4.8.6.0/embyclient/models/play_method.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/play_request.py` & `embyclient-4.8.6.0/embyclient/models/play_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/playback_error_code.py` & `embyclient-4.8.6.0/embyclient/models/playback_error_code.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/playback_info_request.py` & `embyclient-4.8.6.0/embyclient/models/playback_info_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/playback_info_response.py` & `embyclient-4.8.6.0/embyclient/models/playback_info_response.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/playback_progress_info.py` & `embyclient-4.8.6.0/embyclient/models/playback_progress_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/playback_start_info.py` & `embyclient-4.8.6.0/embyclient/models/playback_start_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/playback_stop_info.py` & `embyclient-4.8.6.0/embyclient/models/playback_stop_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/player_state_info.py` & `embyclient-4.8.6.0/embyclient/models/player_state_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/playlists_add_to_playlist_result.py` & `embyclient-4.8.6.0/embyclient/models/playlists_add_to_playlist_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/playlists_playlist_creation_result.py` & `embyclient-4.8.6.0/embyclient/models/playlists_playlist_creation_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/playstate_command.py` & `embyclient-4.8.6.0/embyclient/models/playstate_command.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/playstate_request.py` & `embyclient-4.8.6.0/embyclient/models/playstate_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/plugins_configuration_page_type.py` & `embyclient-4.8.6.0/embyclient/models/plugins_configuration_page_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/plugins_plugin_info.py` & `embyclient-4.8.6.0/embyclient/models/plugins_plugin_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/process_run_metrics_process_metric_point.py` & `embyclient-4.8.6.0/embyclient/models/process_run_metrics_process_metric_point.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/process_run_metrics_process_statistics.py` & `embyclient-4.8.6.0/embyclient/models/process_run_metrics_process_statistics.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/profile_condition.py` & `embyclient-4.8.6.0/embyclient/models/profile_condition.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/profile_condition_type.py` & `embyclient-4.8.6.0/embyclient/models/profile_condition_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/profile_condition_value.py` & `embyclient-4.8.6.0/embyclient/models/profile_condition_value.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/profile_information.py` & `embyclient-4.8.6.0/embyclient/models/profile_information.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/profile_level_information.py` & `embyclient-4.8.6.0/embyclient/models/profile_level_information.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/progress_event.py` & `embyclient-4.8.6.0/embyclient/models/progress_event.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/provider_id_dictionary.py` & `embyclient-4.8.6.0/embyclient/models/provider_id_dictionary.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/proxy_header_mode.py` & `embyclient-4.8.6.0/embyclient/models/proxy_header_mode.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/public_system_info.py` & `embyclient-4.8.6.0/embyclient/models/public_system_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/query_result_activity_log_entry.py` & `embyclient-4.8.6.0/embyclient/models/query_result_activity_log_entry.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/query_result_api_epg_row.py` & `embyclient-4.8.6.0/embyclient/models/query_result_api_epg_row.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/query_result_base_item_dto.py` & `embyclient-4.8.6.0/embyclient/models/query_result_base_item_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/query_result_channel_management_info.py` & `embyclient-4.8.6.0/embyclient/models/query_result_channel_management_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/query_result_devices_device_info.py` & `embyclient-4.8.6.0/embyclient/models/query_result_devices_device_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/query_result_live_tv_series_timer_info_dto.py` & `embyclient-4.8.6.0/embyclient/models/query_result_live_tv_series_timer_info_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/query_result_live_tv_timer_info_dto.py` & `embyclient-4.8.6.0/embyclient/models/query_result_live_tv_timer_info_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/query_result_log_file.py` & `embyclient-4.8.6.0/embyclient/models/query_result_log_file.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/query_result_string.py` & `embyclient-4.8.6.0/embyclient/models/query_result_string.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/query_result_sync_job.py` & `embyclient-4.8.6.0/embyclient/models/query_result_sync_job.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/query_result_sync_job_item.py` & `embyclient-4.8.6.0/embyclient/models/query_result_sync_job_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/query_result_user_dto.py` & `embyclient-4.8.6.0/embyclient/models/query_result_user_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/query_result_user_library_official_rating_item.py` & `embyclient-4.8.6.0/embyclient/models/query_result_user_library_official_rating_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/query_result_user_library_tag_item.py` & `embyclient-4.8.6.0/embyclient/models/query_result_user_library_tag_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/query_result_virtual_folder_info.py` & `embyclient-4.8.6.0/embyclient/models/query_result_virtual_folder_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/queue_item.py` & `embyclient-4.8.6.0/embyclient/models/queue_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/rating_type.py` & `embyclient-4.8.6.0/embyclient/models/rating_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/recommendation_dto.py` & `embyclient-4.8.6.0/embyclient/models/recommendation_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/recommendation_type.py` & `embyclient-4.8.6.0/embyclient/models/recommendation_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/remote_image_info.py` & `embyclient-4.8.6.0/embyclient/models/remote_image_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/remote_image_result.py` & `embyclient-4.8.6.0/embyclient/models/remote_image_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/remote_search_query_album_info.py` & `embyclient-4.8.6.0/embyclient/models/remote_search_query_album_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/remote_search_query_artist_info.py` & `embyclient-4.8.6.0/embyclient/models/remote_search_query_artist_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/remote_search_query_book_info.py` & `embyclient-4.8.6.0/embyclient/models/remote_search_query_book_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/remote_search_query_game_info.py` & `embyclient-4.8.6.0/embyclient/models/remote_search_query_game_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/remote_search_query_item_lookup_info.py` & `embyclient-4.8.6.0/embyclient/models/remote_search_query_item_lookup_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/remote_search_query_movie_info.py` & `embyclient-4.8.6.0/embyclient/models/remote_search_query_movie_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/remote_search_query_music_video_info.py` & `embyclient-4.8.6.0/embyclient/models/remote_search_query_music_video_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/remote_search_query_person_lookup_info.py` & `embyclient-4.8.6.0/embyclient/models/remote_search_query_person_lookup_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/remote_search_query_series_info.py` & `embyclient-4.8.6.0/embyclient/models/remote_search_query_series_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/remote_search_query_trailer_info.py` & `embyclient-4.8.6.0/embyclient/models/remote_search_query_trailer_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/remote_search_result.py` & `embyclient-4.8.6.0/embyclient/models/remote_search_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/remote_subtitle_info.py` & `embyclient-4.8.6.0/embyclient/models/remote_subtitle_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/repeat_mode.py` & `embyclient-4.8.6.0/embyclient/models/repeat_mode.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/resolution.py` & `embyclient-4.8.6.0/embyclient/models/resolution.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/resolution_with_rate.py` & `embyclient-4.8.6.0/embyclient/models/resolution_with_rate.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/response_profile.py` & `embyclient-4.8.6.0/embyclient/models/response_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/roku_metadata_api_thumbnail_info.py` & `embyclient-4.8.6.0/embyclient/models/roku_metadata_api_thumbnail_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/roku_metadata_api_thumbnail_set_info.py` & `embyclient-4.8.6.0/embyclient/models/roku_metadata_api_thumbnail_set_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/run_ui_command.py` & `embyclient-4.8.6.0/embyclient/models/run_ui_command.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/secondary_frameworks.py` & `embyclient-4.8.6.0/embyclient/models/secondary_frameworks.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/segment_skip_mode.py` & `embyclient-4.8.6.0/embyclient/models/segment_skip_mode.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/series_display_order.py` & `embyclient-4.8.6.0/embyclient/models/series_display_order.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/series_info.py` & `embyclient-4.8.6.0/embyclient/models/series_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/server_configuration.py` & `embyclient-4.8.6.0/embyclient/models/server_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         'log_all_query_times': 'bool',
         'enable_case_sensitive_item_ids': 'bool',
         'metadata_path': 'str',
         'metadata_network_path': 'str',
         'preferred_metadata_language': 'str',
         'metadata_country_code': 'str',
         'sort_remove_words': 'list[str]',
-        'library_monitor_delay': 'int',
+        'library_monitor_delay_seconds': 'int',
         'enable_dashboard_response_caching': 'bool',
         'dashboard_source_path': 'str',
         'image_saving_convention': 'ImageSavingConvention',
         'enable_automatic_restart': 'bool',
         'server_name': 'str',
         'preferred_detected_remote_address_family': 'NetSocketsAddressFamily',
         'wan_ddns': 'str',
@@ -102,15 +102,15 @@
         'log_all_query_times': 'LogAllQueryTimes',
         'enable_case_sensitive_item_ids': 'EnableCaseSensitiveItemIds',
         'metadata_path': 'MetadataPath',
         'metadata_network_path': 'MetadataNetworkPath',
         'preferred_metadata_language': 'PreferredMetadataLanguage',
         'metadata_country_code': 'MetadataCountryCode',
         'sort_remove_words': 'SortRemoveWords',
-        'library_monitor_delay': 'LibraryMonitorDelay',
+        'library_monitor_delay_seconds': 'LibraryMonitorDelaySeconds',
         'enable_dashboard_response_caching': 'EnableDashboardResponseCaching',
         'dashboard_source_path': 'DashboardSourcePath',
         'image_saving_convention': 'ImageSavingConvention',
         'enable_automatic_restart': 'EnableAutomaticRestart',
         'server_name': 'ServerName',
         'preferred_detected_remote_address_family': 'PreferredDetectedRemoteAddressFamily',
         'wan_ddns': 'WanDdns',
@@ -149,15 +149,15 @@
         'enable_auto_update': 'EnableAutoUpdate',
         'log_file_retention_days': 'LogFileRetentionDays',
         'run_at_startup': 'RunAtStartup',
         'is_startup_wizard_completed': 'IsStartupWizardCompleted',
         'cache_path': 'CachePath'
     }
 
-    def __init__(self, enable_u_pn_p=None, public_port=None, public_https_port=None, http_server_port_number=None, https_port_number=None, enable_https=None, certificate_path=None, certificate_password=None, is_port_authorized=None, auto_run_web_app=None, enable_remote_access=None, log_all_query_times=None, enable_case_sensitive_item_ids=None, metadata_path=None, metadata_network_path=None, preferred_metadata_language=None, metadata_country_code=None, sort_remove_words=None, library_monitor_delay=None, enable_dashboard_response_caching=None, dashboard_source_path=None, image_saving_convention=None, enable_automatic_restart=None, server_name=None, preferred_detected_remote_address_family=None, wan_ddns=None, ui_culture=None, remote_client_bitrate_limit=None, local_network_subnets=None, local_network_addresses=None, enable_external_content_in_suggestions=None, require_https=None, is_behind_proxy=None, remote_ip_filter=None, is_remote_ip_filter_blacklist=None, image_extraction_timeout_ms=None, path_substitutions=None, uninstalled_plugins=None, collapse_video_folders=None, enable_original_track_titles=None, vacuum_database_on_startup=None, simultaneous_stream_limit=None, database_cache_size_mb=None, enable_sq_lite_mmio=None, playlists_upgraded_to_m3_u=None, image_extractor_upgraded1=None, enable_people_letter_sub_folders=None, optimize_database_on_shutdown=None, database_analysis_limit=None, disable_async_io=None, migrated_to_user_item_shares6=None, migrated_library_options_to_db=None, allow_legacy_local_network_password=None, enable_saved_metadata_for_people=None, tv_channels_refreshed=None, proxy_header_mode=None, enable_debug_level_logging=None, revert_debug_logging=None, enable_auto_update=None, log_file_retention_days=None, run_at_startup=None, is_startup_wizard_completed=None, cache_path=None):  # noqa: E501
+    def __init__(self, enable_u_pn_p=None, public_port=None, public_https_port=None, http_server_port_number=None, https_port_number=None, enable_https=None, certificate_path=None, certificate_password=None, is_port_authorized=None, auto_run_web_app=None, enable_remote_access=None, log_all_query_times=None, enable_case_sensitive_item_ids=None, metadata_path=None, metadata_network_path=None, preferred_metadata_language=None, metadata_country_code=None, sort_remove_words=None, library_monitor_delay_seconds=None, enable_dashboard_response_caching=None, dashboard_source_path=None, image_saving_convention=None, enable_automatic_restart=None, server_name=None, preferred_detected_remote_address_family=None, wan_ddns=None, ui_culture=None, remote_client_bitrate_limit=None, local_network_subnets=None, local_network_addresses=None, enable_external_content_in_suggestions=None, require_https=None, is_behind_proxy=None, remote_ip_filter=None, is_remote_ip_filter_blacklist=None, image_extraction_timeout_ms=None, path_substitutions=None, uninstalled_plugins=None, collapse_video_folders=None, enable_original_track_titles=None, vacuum_database_on_startup=None, simultaneous_stream_limit=None, database_cache_size_mb=None, enable_sq_lite_mmio=None, playlists_upgraded_to_m3_u=None, image_extractor_upgraded1=None, enable_people_letter_sub_folders=None, optimize_database_on_shutdown=None, database_analysis_limit=None, disable_async_io=None, migrated_to_user_item_shares6=None, migrated_library_options_to_db=None, allow_legacy_local_network_password=None, enable_saved_metadata_for_people=None, tv_channels_refreshed=None, proxy_header_mode=None, enable_debug_level_logging=None, revert_debug_logging=None, enable_auto_update=None, log_file_retention_days=None, run_at_startup=None, is_startup_wizard_completed=None, cache_path=None):  # noqa: E501
         """ServerConfiguration - a model defined in Swagger"""  # noqa: E501
         self._enable_u_pn_p = None
         self._public_port = None
         self._public_https_port = None
         self._http_server_port_number = None
         self._https_port_number = None
         self._enable_https = None
@@ -169,15 +169,15 @@
         self._log_all_query_times = None
         self._enable_case_sensitive_item_ids = None
         self._metadata_path = None
         self._metadata_network_path = None
         self._preferred_metadata_language = None
         self._metadata_country_code = None
         self._sort_remove_words = None
-        self._library_monitor_delay = None
+        self._library_monitor_delay_seconds = None
         self._enable_dashboard_response_caching = None
         self._dashboard_source_path = None
         self._image_saving_convention = None
         self._enable_automatic_restart = None
         self._server_name = None
         self._preferred_detected_remote_address_family = None
         self._wan_ddns = None
@@ -251,16 +251,16 @@
             self.metadata_network_path = metadata_network_path
         if preferred_metadata_language is not None:
             self.preferred_metadata_language = preferred_metadata_language
         if metadata_country_code is not None:
             self.metadata_country_code = metadata_country_code
         if sort_remove_words is not None:
             self.sort_remove_words = sort_remove_words
-        if library_monitor_delay is not None:
-            self.library_monitor_delay = library_monitor_delay
+        if library_monitor_delay_seconds is not None:
+            self.library_monitor_delay_seconds = library_monitor_delay_seconds
         if enable_dashboard_response_caching is not None:
             self.enable_dashboard_response_caching = enable_dashboard_response_caching
         if dashboard_source_path is not None:
             self.dashboard_source_path = dashboard_source_path
         if image_saving_convention is not None:
             self.image_saving_convention = image_saving_convention
         if enable_automatic_restart is not None:
@@ -747,35 +747,35 @@
         :param sort_remove_words: The sort_remove_words of this ServerConfiguration.  # noqa: E501
         :type: list[str]
         """
 
         self._sort_remove_words = sort_remove_words
 
     @property
-    def library_monitor_delay(self):
-        """Gets the library_monitor_delay of this ServerConfiguration.  # noqa: E501
+    def library_monitor_delay_seconds(self):
+        """Gets the library_monitor_delay_seconds of this ServerConfiguration.  # noqa: E501
 
         The delay in seconds that we will wait after a file system change to try and discover what has been added/removed Some delay is necessary with some items because their creation is not atomic.  It involves the creation of several different directories and files.  # noqa: E501
 
-        :return: The library_monitor_delay of this ServerConfiguration.  # noqa: E501
+        :return: The library_monitor_delay_seconds of this ServerConfiguration.  # noqa: E501
         :rtype: int
         """
-        return self._library_monitor_delay
+        return self._library_monitor_delay_seconds
 
-    @library_monitor_delay.setter
-    def library_monitor_delay(self, library_monitor_delay):
-        """Sets the library_monitor_delay of this ServerConfiguration.
+    @library_monitor_delay_seconds.setter
+    def library_monitor_delay_seconds(self, library_monitor_delay_seconds):
+        """Sets the library_monitor_delay_seconds of this ServerConfiguration.
 
         The delay in seconds that we will wait after a file system change to try and discover what has been added/removed Some delay is necessary with some items because their creation is not atomic.  It involves the creation of several different directories and files.  # noqa: E501
 
-        :param library_monitor_delay: The library_monitor_delay of this ServerConfiguration.  # noqa: E501
+        :param library_monitor_delay_seconds: The library_monitor_delay_seconds of this ServerConfiguration.  # noqa: E501
         :type: int
         """
 
-        self._library_monitor_delay = library_monitor_delay
+        self._library_monitor_delay_seconds = library_monitor_delay_seconds
 
     @property
     def enable_dashboard_response_caching(self):
         """Gets the enable_dashboard_response_caching of this ServerConfiguration.  # noqa: E501
 
         A value indicating whether \\[enable dashboard response caching\\]. Allows potential contributors without visual studio to modify production dashboard code and test changes.  # noqa: E501
```

### Comparing `embyclient-4.8.5.0/embyclient/models/session_session_info.py` & `embyclient-4.8.6.0/embyclient/models/session_session_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/session_user_info.py` & `embyclient-4.8.6.0/embyclient/models/session_user_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/song_info.py` & `embyclient-4.8.6.0/embyclient/models/song_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/sort_order.py` & `embyclient-4.8.6.0/embyclient/models/sort_order.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/subtitle_delivery_method.py` & `embyclient-4.8.6.0/embyclient/models/subtitle_delivery_method.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/subtitle_location_type.py` & `embyclient-4.8.6.0/embyclient/models/subtitle_location_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/subtitle_playback_mode.py` & `embyclient-4.8.6.0/embyclient/models/subtitle_playback_mode.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/subtitle_profile.py` & `embyclient-4.8.6.0/embyclient/models/subtitle_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/subtitles_subtitle_download_result.py` & `embyclient-4.8.6.0/embyclient/models/subtitles_subtitle_download_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/sync_category.py` & `embyclient-4.8.6.0/embyclient/models/sync_category.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/sync_data_request.py` & `embyclient-4.8.6.0/embyclient/models/sync_data_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/sync_data_response.py` & `embyclient-4.8.6.0/embyclient/models/sync_data_response.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/sync_dialog_options.py` & `embyclient-4.8.6.0/embyclient/models/sync_dialog_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/sync_job.py` & `embyclient-4.8.6.0/embyclient/models/sync_job.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/sync_job_creation_result.py` & `embyclient-4.8.6.0/embyclient/models/sync_job_creation_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/sync_job_item.py` & `embyclient-4.8.6.0/embyclient/models/sync_job_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/sync_job_item_status.py` & `embyclient-4.8.6.0/embyclient/models/sync_job_item_status.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/sync_job_option.py` & `embyclient-4.8.6.0/embyclient/models/sync_job_option.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/sync_job_request.py` & `embyclient-4.8.6.0/embyclient/models/sync_job_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/sync_job_status.py` & `embyclient-4.8.6.0/embyclient/models/sync_job_status.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/sync_profile_option.py` & `embyclient-4.8.6.0/embyclient/models/sync_profile_option.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/sync_quality_option.py` & `embyclient-4.8.6.0/embyclient/models/sync_quality_option.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/sync_target.py` & `embyclient-4.8.6.0/embyclient/models/sync_target.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/synced_item.py` & `embyclient-4.8.6.0/embyclient/models/synced_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/synced_item_progress.py` & `embyclient-4.8.6.0/embyclient/models/synced_item_progress.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/system_event.py` & `embyclient-4.8.6.0/embyclient/models/system_event.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/system_info.py` & `embyclient-4.8.6.0/embyclient/models/system_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/task_completion_status.py` & `embyclient-4.8.6.0/embyclient/models/task_completion_status.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/task_info.py` & `embyclient-4.8.6.0/embyclient/models/task_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/task_result.py` & `embyclient-4.8.6.0/embyclient/models/task_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/task_state.py` & `embyclient-4.8.6.0/embyclient/models/task_state.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/task_trigger_info.py` & `embyclient-4.8.6.0/embyclient/models/task_trigger_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/theme_media_result.py` & `embyclient-4.8.6.0/embyclient/models/theme_media_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/trailer_info.py` & `embyclient-4.8.6.0/embyclient/models/trailer_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/transcode_reason.py` & `embyclient-4.8.6.0/embyclient/models/transcode_reason.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/transcode_seek_info.py` & `embyclient-4.8.6.0/embyclient/models/transcode_seek_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/transcoding_info.py` & `embyclient-4.8.6.0/embyclient/models/transcoding_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/transcoding_profile.py` & `embyclient-4.8.6.0/embyclient/models/transcoding_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/transcoding_vp_step_info.py` & `embyclient-4.8.6.0/embyclient/models/transcoding_vp_step_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/transcoding_vp_step_types.py` & `embyclient-4.8.6.0/embyclient/models/transcoding_vp_step_types.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/transport_stream_timestamp.py` & `embyclient-4.8.6.0/embyclient/models/transport_stream_timestamp.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/tuple_double_double.py` & `embyclient-4.8.6.0/embyclient/models/tuple_double_double.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/type_options.py` & `embyclient-4.8.6.0/embyclient/models/type_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/ui_command.py` & `embyclient-4.8.6.0/embyclient/models/ui_command.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/ui_tab_page_info.py` & `embyclient-4.8.6.0/embyclient/models/ui_tab_page_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/ui_view_info.py` & `embyclient-4.8.6.0/embyclient/models/ui_view_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/unrated_item.py` & `embyclient-4.8.6.0/embyclient/models/unrated_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/update_user_password.py` & `embyclient-4.8.6.0/embyclient/models/update_user_password.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/user_action.py` & `embyclient-4.8.6.0/embyclient/models/user_action.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/user_action_type.py` & `embyclient-4.8.6.0/embyclient/models/user_action_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/user_configuration.py` & `embyclient-4.8.6.0/embyclient/models/user_configuration.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/user_dto.py` & `embyclient-4.8.6.0/embyclient/models/user_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/user_item_data_dto.py` & `embyclient-4.8.6.0/embyclient/models/user_item_data_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/user_item_share_level.py` & `embyclient-4.8.6.0/embyclient/models/user_item_share_level.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/user_library_add_tags.py` & `embyclient-4.8.6.0/embyclient/models/user_library_add_tags.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/user_library_leave_shared_items.py` & `embyclient-4.8.6.0/embyclient/models/user_library_leave_shared_items.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/user_library_official_rating_item.py` & `embyclient-4.8.6.0/embyclient/models/user_library_official_rating_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/user_library_remove_tags.py` & `embyclient-4.8.6.0/embyclient/models/user_library_remove_tags.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/user_library_tag_item.py` & `embyclient-4.8.6.0/embyclient/models/user_library_tag_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/user_library_update_user_item_access.py` & `embyclient-4.8.6.0/embyclient/models/user_library_update_user_item_access.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/user_notification_info.py` & `embyclient-4.8.6.0/embyclient/models/user_notification_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/user_policy.py` & `embyclient-4.8.6.0/embyclient/models/user_policy.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/validate_path.py` & `embyclient-4.8.6.0/embyclient/models/validate_path.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/version.py` & `embyclient-4.8.6.0/embyclient/models/version.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/video3_d_format.py` & `embyclient-4.8.6.0/embyclient/models/video3_d_format.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/video_codec_base.py` & `embyclient-4.8.6.0/embyclient/models/video_codec_base.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/video_media_types.py` & `embyclient-4.8.6.0/embyclient/models/video_media_types.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/virtual_folder_info.py` & `embyclient-4.8.6.0/embyclient/models/virtual_folder_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/models/wake_on_lan_info.py` & `embyclient-4.8.6.0/embyclient/models/wake_on_lan_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient/rest.py` & `embyclient-4.8.6.0/embyclient/rest.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/embyclient.egg-info/PKG-INFO` & `embyclient-4.8.6.0/embyclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embyclient
-Version: 4.8.5.0
+Version: 4.8.6.0
 Summary: A Python client for Emby Media Server's API
 Home-page: https://emby.media
 Keywords: Emby,Rest,API,client,media,server,JSON
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Multimedia
```

### Comparing `embyclient-4.8.5.0/embyclient.egg-info/SOURCES.txt` & `embyclient-4.8.6.0/embyclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.5.0/setup.py` & `embyclient-4.8.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
-VERSION = "4.8.5.0"
+VERSION = "4.8.6.0"
 REQUIRES = ["urllib3 >= 1.15", "six >= 1.10", "certifi", "python-dateutil"]
 
 
 classifiers = [
     'Intended Audience :: Developers',  # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'Topic :: Multimedia :: Video',
```

