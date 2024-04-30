# Comparing `tmp/aspose-tasks-cloud-22.7.0.tar.gz` & `tmp/aspose_tasks_cloud-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aspose-tasks-cloud-22.7.0.tar", last modified: Fri Jul 29 13:41:57 2022, max compression
+gzip compressed data, was "aspose_tasks_cloud-24.4.0.tar", last modified: Tue Apr 30 10:13:49 2024, max compression
```

## Comparing `aspose-tasks-cloud-22.7.0.tar` & `aspose_tasks_cloud-24.4.0.tar`

### file list

```diff
@@ -1,275 +1,297 @@
-drwxrwxrwx   0        0        0        0 2022-07-29 13:41:57.639025 aspose-tasks-cloud-22.7.0/
--rw-rw-rw-   0        0        0     1075 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/LICENSE
--rw-rw-rw-   0        0        0     7897 2022-07-29 13:41:57.638025 aspose-tasks-cloud-22.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     6817 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/README.md
-drwxrwxrwx   0        0        0        0 2022-07-29 13:41:57.414214 aspose-tasks-cloud-22.7.0/aspose_tasks_cloud.egg-info/
--rw-rw-rw-   0        0        0     7897 2022-07-29 13:41:57.000000 aspose-tasks-cloud-22.7.0/aspose_tasks_cloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12768 2022-07-29 13:41:57.000000 aspose-tasks-cloud-22.7.0/aspose_tasks_cloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-29 13:41:57.000000 aspose-tasks-cloud-22.7.0/aspose_tasks_cloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2022-07-29 13:41:57.000000 aspose-tasks-cloud-22.7.0/aspose_tasks_cloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2022-07-29 13:41:57.000000 aspose-tasks-cloud-22.7.0/aspose_tasks_cloud.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-07-29 13:41:57.418215 aspose-tasks-cloud-22.7.0/asposetaskscloud/
--rw-rw-rw-   0        0        0    18412 2022-07-21 09:17:32.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-29 13:41:57.419215 aspose-tasks-cloud-22.7.0/asposetaskscloud/api/
--rw-rw-rw-   0        0        0      130 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/api/__init__.py
--rw-rw-rw-   0        0        0   505116 2022-07-21 09:17:32.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/api/tasks_api.py
--rw-rw-rw-   0        0        0    27765 2022-07-21 09:24:12.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/api_client.py
--rw-rw-rw-   0        0        0     9702 2022-07-21 09:25:18.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/configuration.py
-drwxrwxrwx   0        0        0        0 2022-07-29 13:41:57.538961 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/
--rw-rw-rw-   0        0        0     9723 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/__init__.py
--rw-rw-rw-   0        0        0     6898 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/aspose_response.py
--rw-rw-rw-   0        0        0     5603 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/assignment_baseline.py
--rw-rw-rw-   0        0        0     6815 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/assignment_item.py
--rw-rw-rw-   0        0        0     4448 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/assignment_item_response.py
--rw-rw-rw-   0        0        0     4324 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/assignment_items.py
--rw-rw-rw-   0        0        0     4294 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/assignment_items_response.py
--rw-rw-rw-   0        0        0     4357 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/assignment_response.py
--rw-rw-rw-   0        0        0     4274 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/assignments_response.py
--rw-rw-rw-   0        0        0     8216 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/baseline.py
--rw-rw-rw-   0        0        0     3884 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/baseline_type.py
--rw-rw-rw-   0        0        0     3596 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/booking_type.py
--rw-rw-rw-   0        0        0     3838 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calculation_mode.py
--rw-rw-rw-   0        0        0     3615 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calculation_type.py
--rw-rw-rw-   0        0        0     9067 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calendar.py
--rw-rw-rw-   0        0        0    18824 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calendar_exception.py
--rw-rw-rw-   0        0        0     3859 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calendar_exception_type.py
--rw-rw-rw-   0        0        0     4529 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calendar_exceptions_response.py
--rw-rw-rw-   0        0        0     5374 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calendar_item.py
--rw-rw-rw-   0        0        0     4400 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calendar_item_response.py
--rw-rw-rw-   0        0        0     4083 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calendar_items.py
--rw-rw-rw-   0        0        0     4232 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calendar_items_response.py
--rw-rw-rw-   0        0        0     4245 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calendar_response.py
--rw-rw-rw-   0        0        0     4492 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calendar_work_weeks_response.py
--rw-rw-rw-   0        0        0     3758 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/confidence_level.py
--rw-rw-rw-   0        0        0     3896 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/constraint_type.py
--rw-rw-rw-   0        0        0     3643 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/cost_accrual_type.py
--rw-rw-rw-   0        0        0     3762 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/custom_field_type.py
--rw-rw-rw-   0        0        0     3639 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/day_of_week.py
--rw-rw-rw-   0        0        0     3688 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/day_type.py
--rw-rw-rw-   0        0        0     5288 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/disc_usage.py
--rw-rw-rw-   0        0        0     4169 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/document_properties.py
--rw-rw-rw-   0        0        0     4411 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/document_properties_response.py
--rw-rw-rw-   0        0        0     4974 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/document_property.py
--rw-rw-rw-   0        0        0     4368 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/document_property_response.py
--rw-rw-rw-   0        0        0     5434 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/duration.py
--rw-rw-rw-   0        0        0     3692 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/earned_value_method_type.py
--rw-rw-rw-   0        0        0     3568 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/element_type.py
--rw-rw-rw-   0        0        0     6420 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/error.py
--rw-rw-rw-   0        0        0     5051 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/error_details.py
--rw-rw-rw-   0        0        0    13623 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/extended_attribute.py
--rw-rw-rw-   0        0        0    27684 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/extended_attribute_definition.py
--rw-rw-rw-   0        0        0     7003 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/extended_attribute_item.py
--rw-rw-rw-   0        0        0     4617 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/extended_attribute_item_response.py
--rw-rw-rw-   0        0        0     4182 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/extended_attribute_items.py
--rw-rw-rw-   0        0        0     4530 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/extended_attribute_items_response.py
--rw-rw-rw-   0        0        0     4593 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/extended_attribute_response.py
--rw-rw-rw-   0        0        0     5276 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/file_version.py
--rw-rw-rw-   0        0        0     4218 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/file_versions.py
--rw-rw-rw-   0        0        0     4226 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/files_list.py
--rw-rw-rw-   0        0        0     5049 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/files_upload_result.py
--rw-rw-rw-   0        0        0     3663 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/imported_project_type.py
--rw-rw-rw-   0        0        0     7637 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/link.py
--rw-rw-rw-   0        0        0     4660 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/link_element.py
--rw-rw-rw-   0        0        0     3762 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/mask_type.py
--rw-rw-rw-   0        0        0     3775 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/month.py
--rw-rw-rw-   0        0        0     3829 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/month_item_type.py
--rw-rw-rw-   0        0        0     3668 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/month_position.py
--rw-rw-rw-   0        0        0     5295 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/object_exist.py
--rw-rw-rw-   0        0        0     3653 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/ordinal_number.py
--rw-rw-rw-   0        0        0     6269 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/outline_code.py
--rw-rw-rw-   0        0        0    18747 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/outline_code_definition.py
--rw-rw-rw-   0        0        0     4838 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/outline_code_item.py
--rw-rw-rw-   0        0        0     4116 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/outline_code_items.py
--rw-rw-rw-   0        0        0     4344 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/outline_code_items_response.py
--rw-rw-rw-   0        0        0     4395 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/outline_code_response.py
--rw-rw-rw-   0        0        0     6922 2022-07-21 09:17:30.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/outline_mask.py
--rw-rw-rw-   0        0        0     9805 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/outline_value.py
--rw-rw-rw-   0        0        0     3705 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/outline_value_type.py
--rw-rw-rw-   0        0        0     4457 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/page_count_response.py
--rw-rw-rw-   0        0        0     3599 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/page_size.py
--rw-rw-rw-   0        0        0     3697 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/presentation_format.py
--rw-rw-rw-   0        0        0     3637 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/probability_distribution_type.py
--rw-rw-rw-   0        0        0     3624 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/project_database_type.py
--rw-rw-rw-   0        0        0     3891 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/project_file_format.py
--rw-rw-rw-   0        0        0     4342 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/project_ids_response.py
--rw-rw-rw-   0        0        0    10272 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/project_info.py
--rw-rw-rw-   0        0        0     4223 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/project_list.py
--rw-rw-rw-   0        0        0     4190 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/project_list_response.py
--rw-rw-rw-   0        0        0     4251 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/project_recalculate_response.py
--rw-rw-rw-   0        0        0     5687 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/project_recalculation_result.py
--rw-rw-rw-   0        0        0     8867 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/project_server_save_options_dto.py
--rw-rw-rw-   0        0        0     3665 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/project_validation_state.py
--rw-rw-rw-   0        0        0     3744 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/rate_format_type.py
--rw-rw-rw-   0        0        0     3680 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/rate_scale_type.py
--rw-rw-rw-   0        0        0     3601 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/rate_type.py
--rw-rw-rw-   0        0        0     3646 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/recurrence_pattern.py
--rw-rw-rw-   0        0        0    28838 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/recurring_info.py
--rw-rw-rw-   0        0        0     4453 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/recurring_info_response.py
--rw-rw-rw-   0        0        0     4133 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/report_type.py
-drwxrwxrwx   0        0        0        0 2022-07-29 13:41:57.614989 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/
--rw-rw-rw-   0        0        0     8548 2022-07-21 09:17:32.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/__init__.py
--rw-rw-rw-   0        0        0     2135 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/copy_file_request.py
--rw-rw-rw-   0        0        0     2043 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/copy_folder_request.py
--rw-rw-rw-   0        0        0     1808 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/create_folder_request.py
--rw-rw-rw-   0        0        0     2724 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/create_new_project_request.py
--rw-rw-rw-   0        0        0     2172 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/delete_assignment_request.py
--rw-rw-rw-   0        0        0     2339 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/delete_calendar_exception_request.py
--rw-rw-rw-   0        0        0     2171 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/delete_calendar_request.py
--rw-rw-rw-   0        0        0     2037 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/delete_extended_attribute_by_index_request.py
--rw-rw-rw-   0        0        0     1892 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/delete_file_request.py
--rw-rw-rw-   0        0        0     1908 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/delete_folder_request.py
--rw-rw-rw-   0        0        0     1995 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/delete_outline_code_by_index_request.py
--rw-rw-rw-   0        0        0     2169 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/delete_resource_request.py
--rw-rw-rw-   0        0        0     2178 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/delete_task_link_request.py
--rw-rw-rw-   0        0        0     2125 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/delete_task_request.py
--rw-rw-rw-   0        0        0     1900 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/download_file_request.py
--rw-rw-rw-   0        0        0     1961 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_assignment_request.py
--rw-rw-rw-   0        0        0     2294 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_assignment_timephased_data_request.py
--rw-rw-rw-   0        0        0     1860 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_assignments_request.py
--rw-rw-rw-   0        0        0     1979 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_calendar_exceptions_request.py
--rw-rw-rw-   0        0        0     1947 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_calendar_request.py
--rw-rw-rw-   0        0        0     1976 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_calendar_work_weeks_request.py
--rw-rw-rw-   0        0        0     1854 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_calendars_request.py
--rw-rw-rw-   0        0        0     1850 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_critical_path_request.py
--rw-rw-rw-   0        0        0     1696 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_disc_usage_request.py
--rw-rw-rw-   0        0        0     1863 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_document_properties_request.py
--rw-rw-rw-   0        0        0     1978 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_document_property_request.py
--rw-rw-rw-   0        0        0     2045 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_extended_attribute_by_index_request.py
--rw-rw-rw-   0        0        0     1883 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_extended_attributes_request.py
--rw-rw-rw-   0        0        0     1798 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_file_versions_request.py
--rw-rw-rw-   0        0        0     1789 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_files_list_request.py
--rw-rw-rw-   0        0        0     2003 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_outline_code_by_index_request.py
--rw-rw-rw-   0        0        0     1867 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_outline_codes_request.py
--rw-rw-rw-   0        0        0     2421 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_page_count_request.py
--rw-rw-rw-   0        0        0     1859 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_project_ids_request.py
--rw-rw-rw-   0        0        0     2346 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_project_list_request.py
--rw-rw-rw-   0        0        0     1932 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_report_pdf_request.py
--rw-rw-rw-   0        0        0     1980 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_resource_assignments_request.py
--rw-rw-rw-   0        0        0     1945 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_resource_request.py
--rw-rw-rw-   0        0        0     2278 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_resource_timephased_data_request.py
--rw-rw-rw-   0        0        0     1854 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_resources_request.py
--rw-rw-rw-   0        0        0     3459 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_risk_analysis_report_request.py
--rw-rw-rw-   0        0        0     1948 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_task_assignments_request.py
--rw-rw-rw-   0        0        0     1865 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_task_document_request.py
--rw-rw-rw-   0        0        0     2246 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_task_document_with_format_request.py
--rw-rw-rw-   0        0        0     1856 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_task_links_request.py
--rw-rw-rw-   0        0        0     1956 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_task_recurring_info_request.py
--rw-rw-rw-   0        0        0     1913 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_task_request.py
--rw-rw-rw-   0        0        0     2246 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_task_timephased_data_request.py
--rw-rw-rw-   0        0        0     1842 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_tasks_request.py
--rw-rw-rw-   0        0        0     1841 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_vba_project_request.py
--rw-rw-rw-   0        0        0     1851 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_wbs_definition_request.py
--rw-rw-rw-   0        0        0     2161 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/move_file_request.py
--rw-rw-rw-   0        0        0     2076 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/move_folder_request.py
--rw-rw-rw-   0        0        0     1904 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/object_exists_request.py
--rw-rw-rw-   0        0        0     2571 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/post_assignment_request.py
--rw-rw-rw-   0        0        0     2338 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/post_calendar_exception_request.py
--rw-rw-rw-   0        0        0     2164 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/post_calendar_request.py
--rw-rw-rw-   0        0        0     2303 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/post_document_property_request.py
--rw-rw-rw-   0        0        0     2479 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/post_resource_request.py
--rw-rw-rw-   0        0        0     2435 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/post_task_document_with_format_request.py
--rw-rw-rw-   0        0        0     2202 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/post_task_link_request.py
--rw-rw-rw-   0        0        0     2519 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/post_task_recurring_info_request.py
--rw-rw-rw-   0        0        0     2432 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/post_task_request.py
--rw-rw-rw-   0        0        0     2063 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/post_tasks_request.py
--rw-rw-rw-   0        0        0     2322 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_assignment_request.py
--rw-rw-rw-   0        0        0     2459 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_calendar_exception_request.py
--rw-rw-rw-   0        0        0     2292 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_calendar_request.py
--rw-rw-rw-   0        0        0     2302 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_document_property_request.py
--rw-rw-rw-   0        0        0     2264 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_extended_attribute_request.py
--rw-rw-rw-   0        0        0     2575 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_import_project_from_db_request.py
--rw-rw-rw-   0        0        0     2406 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_import_project_from_file_request.py
--rw-rw-rw-   0        0        0     2834 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_import_project_from_project_online_request.py
--rw-rw-rw-   0        0        0     2313 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_move_task_request.py
--rw-rw-rw-   0        0        0     2356 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_move_task_to_sibling_request.py
--rw-rw-rw-   0        0        0     2496 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_recalculate_project_request.py
--rw-rw-rw-   0        0        0     2022 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_recalculate_project_resource_fields_request.py
--rw-rw-rw-   0        0        0     2149 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_recalculate_project_uncomplete_work_to_start_after_request.py
--rw-rw-rw-   0        0        0     2374 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_recalculate_project_work_as_complete_request.py
--rw-rw-rw-   0        0        0     2281 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_renumber_wbs_code_request.py
--rw-rw-rw-   0        0        0     2395 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_resource_request.py
--rw-rw-rw-   0        0        0     2309 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_task_link_request.py
--rw-rw-rw-   0        0        0     2193 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_task_recurring_info_request.py
--rw-rw-rw-   0        0        0     2250 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_task_request.py
--rw-rw-rw-   0        0        0     1711 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/storage_exists_request.py
--rw-rw-rw-   0        0        0     2732 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/update_project_request.py
--rw-rw-rw-   0        0        0     2095 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/upload_file_request.py
--rw-rw-rw-   0        0        0    80226 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/resource.py
--rw-rw-rw-   0        0        0    74662 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/resource_assignment.py
--rw-rw-rw-   0        0        0     4149 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/resource_assignments.py
--rw-rw-rw-   0        0        0     6025 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/resource_item.py
--rw-rw-rw-   0        0        0     4404 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/resource_item_response.py
--rw-rw-rw-   0        0        0     4262 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/resource_items.py
--rw-rw-rw-   0        0        0     4232 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/resource_items_response.py
--rw-rw-rw-   0        0        0     4245 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/resource_response.py
--rw-rw-rw-   0        0        0     3572 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/resource_type.py
--rw-rw-rw-   0        0        0     3767 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/rollup_type.py
--rw-rw-rw-   0        0        0     4343 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/storage_exist.py
--rw-rw-rw-   0        0        0     7540 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/storage_file.py
--rw-rw-rw-   0        0        0     3706 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/summary_rows_calculation_type.py
--rw-rw-rw-   0        0        0   118802 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task.py
--rw-rw-rw-   0        0        0     9707 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_baseline.py
--rw-rw-rw-   0        0        0     6191 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_creation_request.py
--rw-rw-rw-   0        0        0     8325 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_item.py
--rw-rw-rw-   0        0        0     4268 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_item_response.py
--rw-rw-rw-   0        0        0     4138 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_items.py
--rw-rw-rw-   0        0        0     4108 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_items_response.py
--rw-rw-rw-   0        0        0     8939 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_link.py
--rw-rw-rw-   0        0        0     4268 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_link_response.py
--rw-rw-rw-   0        0        0     3661 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_link_type.py
--rw-rw-rw-   0        0        0     4241 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_links_response.py
--rw-rw-rw-   0        0        0     4113 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_response.py
--rw-rw-rw-   0        0        0     3613 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_type.py
--rw-rw-rw-   0        0        0     4455 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/time_unit_type.py
--rw-rw-rw-   0        0        0     9019 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/timephased_data.py
--rw-rw-rw-   0        0        0     4200 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/timephased_data_response.py
--rw-rw-rw-   0        0        0     7471 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/timephased_data_type.py
--rw-rw-rw-   0        0        0     3633 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/timescale.py
--rw-rw-rw-   0        0        0     8280 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/value.py
--rw-rw-rw-   0        0        0     5890 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/vba_module.py
--rw-rw-rw-   0        0        0     4970 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/vba_module_attribute.py
--rw-rw-rw-   0        0        0     9544 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/vba_project.py
--rw-rw-rw-   0        0        0     4257 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/vba_project_response.py
--rw-rw-rw-   0        0        0     5080 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/vba_reference.py
--rw-rw-rw-   0        0        0     6981 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/wbs_code_mask.py
--rw-rw-rw-   0        0        0     7677 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/wbs_definition.py
--rw-rw-rw-   0        0        0     4433 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/wbs_definition_response.py
--rw-rw-rw-   0        0        0     3706 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/wbs_sequence.py
--rw-rw-rw-   0        0        0     8230 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/week_day.py
--rw-rw-rw-   0        0        0     3739 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/week_day_type.py
--rw-rw-rw-   0        0        0     3788 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/work_contour_type.py
--rw-rw-rw-   0        0        0     3594 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/work_group_type.py
--rw-rw-rw-   0        0        0     6908 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/work_week.py
--rw-rw-rw-   0        0        0     5417 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/models/working_time.py
--rw-rw-rw-   0        0        0    14865 2022-07-21 09:17:31.000000 aspose-tasks-cloud-22.7.0/asposetaskscloud/rest.py
--rw-rw-rw-   0        0        0       42 2022-07-29 13:41:57.639025 aspose-tasks-cloud-22.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1626 2022-07-29 13:36:53.000000 aspose-tasks-cloud-22.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-29 13:41:57.637026 aspose-tasks-cloud-22.7.0/test/
--rw-rw-rw-   0        0        0     1338 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/__init__.py
--rw-rw-rw-   0        0        0     3340 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/base_test_context.py
--rw-rw-rw-   0        0        0     3232 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_api_coverage.py
--rw-rw-rw-   0        0        0    10588 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_assignments.py
--rw-rw-rw-   0        0        0     8621 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_calendar_exceptions.py
--rw-rw-rw-   0        0        0     4665 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_calendar_work_weeks.py
--rw-rw-rw-   0        0        0     8089 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_calendars.py
--rw-rw-rw-   0        0        0     4954 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_document_properties.py
--rw-rw-rw-   0        0        0     8995 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_extended_attributes.py
--rw-rw-rw-   0        0        0     4695 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_file.py
--rw-rw-rw-   0        0        0     4439 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_folder.py
--rw-rw-rw-   0        0        0     2658 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_get_page_count.py
--rw-rw-rw-   0        0        0     5718 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_import_project.py
--rw-rw-rw-   0        0        0     3347 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_outline_codes.py
--rw-rw-rw-   0        0        0     4935 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_project_online.py
--rw-rw-rw-   0        0        0     2386 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_read_project.py
--rw-rw-rw-   0        0        0     4867 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_recalculation.py
--rw-rw-rw-   0        0        0     5717 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_recurring_info.py
--rw-rw-rw-   0        0        0     3185 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_report.py
--rw-rw-rw-   0        0        0     6715 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_resources.py
--rw-rw-rw-   0        0        0     3118 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_storage.py
--rw-rw-rw-   0        0        0     4237 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_task_document_format.py
--rw-rw-rw-   0        0        0     4392 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_task_links.py
--rw-rw-rw-   0        0        0    10130 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_tasks.py
--rw-rw-rw-   0        0        0    14926 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_tasks_extended_attributes.py
--rw-rw-rw-   0        0        0     3768 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_timephased_data.py
--rw-rw-rw-   0        0        0     2235 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_vba.py
--rw-rw-rw-   0        0        0     2536 2022-07-21 09:04:59.000000 aspose-tasks-cloud-22.7.0/test/test_wbs.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:13:49.345562 aspose_tasks_cloud-24.4.0/
+-rw-rw-rw-   0        0        0     1075 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/LICENSE
+-rw-rw-rw-   0        0        0     8317 2024-04-30 10:13:49.344545 aspose_tasks_cloud-24.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7117 2024-03-30 06:49:20.000000 aspose_tasks_cloud-24.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 10:13:49.343510 aspose_tasks_cloud-24.4.0/aspose_tasks_cloud.egg-info/
+-rw-rw-rw-   0        0        0     8317 2024-04-30 10:13:48.000000 aspose_tasks_cloud-24.4.0/aspose_tasks_cloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13865 2024-04-30 10:13:49.000000 aspose_tasks_cloud-24.4.0/aspose_tasks_cloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 10:13:48.000000 aspose_tasks_cloud-24.4.0/aspose_tasks_cloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-30 10:13:48.000000 aspose_tasks_cloud-24.4.0/aspose_tasks_cloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-30 10:13:48.000000 aspose_tasks_cloud-24.4.0/aspose_tasks_cloud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 10:13:49.034004 aspose_tasks_cloud-24.4.0/asposetaskscloud/
+-rw-rw-rw-   0        0        0    20039 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:13:49.035031 aspose_tasks_cloud-24.4.0/asposetaskscloud/api/
+-rw-rw-rw-   0        0        0      130 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/api/__init__.py
+-rw-rw-rw-   0        0        0   546042 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/api/tasks_api.py
+-rw-rw-rw-   0        0        0    27765 2024-03-30 06:49:49.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/api_client.py
+-rw-rw-rw-   0        0        0     9702 2024-03-30 06:50:08.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/configuration.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:13:49.204624 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/
+-rw-rw-rw-   0        0        0    10625 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/__init__.py
+-rw-rw-rw-   0        0        0     7144 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/aspose_response.py
+-rw-rw-rw-   0        0        0     5603 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/assignment_baseline.py
+-rw-rw-rw-   0        0        0     6815 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/assignment_item.py
+-rw-rw-rw-   0        0        0     4448 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/assignment_item_response.py
+-rw-rw-rw-   0        0        0     4324 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/assignment_items.py
+-rw-rw-rw-   0        0        0     4294 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/assignment_items_response.py
+-rw-rw-rw-   0        0        0     4357 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/assignment_response.py
+-rw-rw-rw-   0        0        0     4274 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/assignments_response.py
+-rw-rw-rw-   0        0        0     4023 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/background_pattern.py
+-rw-rw-rw-   0        0        0     8216 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/baseline.py
+-rw-rw-rw-   0        0        0     3884 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/baseline_type.py
+-rw-rw-rw-   0        0        0     3596 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/booking_type.py
+-rw-rw-rw-   0        0        0     3838 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calculation_mode.py
+-rw-rw-rw-   0        0        0     3615 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calculation_type.py
+-rw-rw-rw-   0        0        0     9067 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calendar.py
+-rw-rw-rw-   0        0        0    18824 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calendar_exception.py
+-rw-rw-rw-   0        0        0     3859 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calendar_exception_type.py
+-rw-rw-rw-   0        0        0     4529 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calendar_exceptions_response.py
+-rw-rw-rw-   0        0        0     5374 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calendar_item.py
+-rw-rw-rw-   0        0        0     4400 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calendar_item_response.py
+-rw-rw-rw-   0        0        0     4083 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calendar_items.py
+-rw-rw-rw-   0        0        0     4232 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calendar_items_response.py
+-rw-rw-rw-   0        0        0     4245 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calendar_response.py
+-rw-rw-rw-   0        0        0     4492 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calendar_work_weeks_response.py
+-rw-rw-rw-   0        0        0     7513 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/colors.py
+-rw-rw-rw-   0        0        0     3758 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/confidence_level.py
+-rw-rw-rw-   0        0        0     3896 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/constraint_type.py
+-rw-rw-rw-   0        0        0     3643 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/cost_accrual_type.py
+-rw-rw-rw-   0        0        0     3762 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/custom_field_type.py
+-rw-rw-rw-   0        0        0     3639 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/day_of_week.py
+-rw-rw-rw-   0        0        0     3688 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/day_type.py
+-rw-rw-rw-   0        0        0     5288 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/disc_usage.py
+-rw-rw-rw-   0        0        0     4169 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/document_properties.py
+-rw-rw-rw-   0        0        0     4411 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/document_properties_response.py
+-rw-rw-rw-   0        0        0     4974 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/document_property.py
+-rw-rw-rw-   0        0        0     4368 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/document_property_response.py
+-rw-rw-rw-   0        0        0     5434 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/duration.py
+-rw-rw-rw-   0        0        0     3692 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/earned_value_method_type.py
+-rw-rw-rw-   0        0        0     3568 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/element_type.py
+-rw-rw-rw-   0        0        0     6420 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/error.py
+-rw-rw-rw-   0        0        0     5051 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/error_details.py
+-rw-rw-rw-   0        0        0    13623 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/extended_attribute.py
+-rw-rw-rw-   0        0        0    27684 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/extended_attribute_definition.py
+-rw-rw-rw-   0        0        0     7003 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/extended_attribute_item.py
+-rw-rw-rw-   0        0        0     4617 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/extended_attribute_item_response.py
+-rw-rw-rw-   0        0        0     4182 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/extended_attribute_items.py
+-rw-rw-rw-   0        0        0     4530 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/extended_attribute_items_response.py
+-rw-rw-rw-   0        0        0     4593 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/extended_attribute_response.py
+-rw-rw-rw-   0        0        0    75652 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/field.py
+-rw-rw-rw-   0        0        0     5276 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/file_version.py
+-rw-rw-rw-   0        0        0     4218 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/file_versions.py
+-rw-rw-rw-   0        0        0     4226 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/files_list.py
+-rw-rw-rw-   0        0        0     5049 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/files_upload_result.py
+-rw-rw-rw-   0        0        0     3663 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/imported_project_type.py
+-rw-rw-rw-   0        0        0     3579 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/item_type.py
+-rw-rw-rw-   0        0        0     7637 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/link.py
+-rw-rw-rw-   0        0        0     4660 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/link_element.py
+-rw-rw-rw-   0        0        0     3762 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/mask_type.py
+-rw-rw-rw-   0        0        0     3775 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/month.py
+-rw-rw-rw-   0        0        0     3829 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/month_item_type.py
+-rw-rw-rw-   0        0        0     3668 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/month_position.py
+-rw-rw-rw-   0        0        0     5295 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/object_exist.py
+-rw-rw-rw-   0        0        0     3653 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/ordinal_number.py
+-rw-rw-rw-   0        0        0     6269 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/outline_code.py
+-rw-rw-rw-   0        0        0    18747 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/outline_code_definition.py
+-rw-rw-rw-   0        0        0     4838 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/outline_code_item.py
+-rw-rw-rw-   0        0        0     4116 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/outline_code_items.py
+-rw-rw-rw-   0        0        0     4344 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/outline_code_items_response.py
+-rw-rw-rw-   0        0        0     4395 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/outline_code_response.py
+-rw-rw-rw-   0        0        0     6922 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/outline_mask.py
+-rw-rw-rw-   0        0        0     9805 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/outline_value.py
+-rw-rw-rw-   0        0        0     3705 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/outline_value_type.py
+-rw-rw-rw-   0        0        0     4457 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/page_count_response.py
+-rw-rw-rw-   0        0        0     3599 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/page_size.py
+-rw-rw-rw-   0        0        0     3697 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/presentation_format.py
+-rw-rw-rw-   0        0        0    15571 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/primavera_task_properties.py
+-rw-rw-rw-   0        0        0     4692 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/primavera_task_properties_response.py
+-rw-rw-rw-   0        0        0     3637 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/probability_distribution_type.py
+-rw-rw-rw-   0        0        0     3624 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/project_database_type.py
+-rw-rw-rw-   0        0        0     3891 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/project_file_format.py
+-rw-rw-rw-   0        0        0     4340 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/project_ids_response.py
+-rw-rw-rw-   0        0        0    10272 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/project_info.py
+-rw-rw-rw-   0        0        0     4223 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/project_list.py
+-rw-rw-rw-   0        0        0     4190 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/project_list_response.py
+-rw-rw-rw-   0        0        0     4251 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/project_recalculate_response.py
+-rw-rw-rw-   0        0        0     5687 2024-03-29 11:15:53.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/project_recalculation_result.py
+-rw-rw-rw-   0        0        0     8867 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/project_server_save_options_dto.py
+-rw-rw-rw-   0        0        0     3665 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/project_validation_state.py
+-rw-rw-rw-   0        0        0     3744 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/rate_format_type.py
+-rw-rw-rw-   0        0        0     3680 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/rate_scale_type.py
+-rw-rw-rw-   0        0        0     3601 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/rate_type.py
+-rw-rw-rw-   0        0        0     3646 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/recurrence_pattern.py
+-rw-rw-rw-   0        0        0    28838 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/recurring_info.py
+-rw-rw-rw-   0        0        0     4453 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/recurring_info_response.py
+-rw-rw-rw-   0        0        0     4133 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/report_type.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:13:49.310273 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/
+-rw-rw-rw-   0        0        0     9273 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/__init__.py
+-rw-rw-rw-   0        0        0     2135 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/copy_file_request.py
+-rw-rw-rw-   0        0        0     2043 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/copy_folder_request.py
+-rw-rw-rw-   0        0        0     1808 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/create_folder_request.py
+-rw-rw-rw-   0        0        0     2724 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/create_new_project_request.py
+-rw-rw-rw-   0        0        0     2182 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/create_table_text_style_request.py
+-rw-rw-rw-   0        0        0     2172 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_assignment_request.py
+-rw-rw-rw-   0        0        0     2339 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_calendar_exception_request.py
+-rw-rw-rw-   0        0        0     2171 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_calendar_request.py
+-rw-rw-rw-   0        0        0     2037 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_extended_attribute_by_index_request.py
+-rw-rw-rw-   0        0        0     1892 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_file_request.py
+-rw-rw-rw-   0        0        0     1908 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_folder_request.py
+-rw-rw-rw-   0        0        0     1995 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_outline_code_by_index_request.py
+-rw-rw-rw-   0        0        0     2169 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_resource_request.py
+-rw-rw-rw-   0        0        0     2236 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_table_text_style_request.py
+-rw-rw-rw-   0        0        0     2178 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_task_link_request.py
+-rw-rw-rw-   0        0        0     2125 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_task_request.py
+-rw-rw-rw-   0        0        0     1900 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/download_file_request.py
+-rw-rw-rw-   0        0        0     1969 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_all_table_text_styles_request.py
+-rw-rw-rw-   0        0        0     1961 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_assignment_request.py
+-rw-rw-rw-   0        0        0     2294 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_assignment_timephased_data_request.py
+-rw-rw-rw-   0        0        0     1860 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_assignments_request.py
+-rw-rw-rw-   0        0        0     1979 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_calendar_exceptions_request.py
+-rw-rw-rw-   0        0        0     1947 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_calendar_request.py
+-rw-rw-rw-   0        0        0     1976 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_calendar_work_weeks_request.py
+-rw-rw-rw-   0        0        0     1854 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_calendars_request.py
+-rw-rw-rw-   0        0        0     1850 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_critical_path_request.py
+-rw-rw-rw-   0        0        0     1696 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_disc_usage_request.py
+-rw-rw-rw-   0        0        0     1863 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_document_properties_request.py
+-rw-rw-rw-   0        0        0     1978 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_document_property_request.py
+-rw-rw-rw-   0        0        0     2045 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_extended_attribute_by_index_request.py
+-rw-rw-rw-   0        0        0     1883 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_extended_attributes_request.py
+-rw-rw-rw-   0        0        0     1798 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_file_versions_request.py
+-rw-rw-rw-   0        0        0     1789 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_files_list_request.py
+-rw-rw-rw-   0        0        0     2003 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_outline_code_by_index_request.py
+-rw-rw-rw-   0        0        0     1867 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_outline_codes_request.py
+-rw-rw-rw-   0        0        0     2421 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_page_count_request.py
+-rw-rw-rw-   0        0        0     2010 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_primavera_task_properties_request.py
+-rw-rw-rw-   0        0        0     1859 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_project_ids_request.py
+-rw-rw-rw-   0        0        0     2346 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_project_list_request.py
+-rw-rw-rw-   0        0        0     1932 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_report_pdf_request.py
+-rw-rw-rw-   0        0        0     1980 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_resource_assignments_request.py
+-rw-rw-rw-   0        0        0     1945 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_resource_request.py
+-rw-rw-rw-   0        0        0     2278 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_resource_timephased_data_request.py
+-rw-rw-rw-   0        0        0     1854 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_resources_request.py
+-rw-rw-rw-   0        0        0     3459 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_risk_analysis_report_request.py
+-rw-rw-rw-   0        0        0     2123 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_table_text_style_request.py
+-rw-rw-rw-   0        0        0     1948 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_task_assignments_request.py
+-rw-rw-rw-   0        0        0     1865 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_task_document_request.py
+-rw-rw-rw-   0        0        0     2246 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_task_document_with_format_request.py
+-rw-rw-rw-   0        0        0     1856 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_task_links_request.py
+-rw-rw-rw-   0        0        0     1956 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_task_recurring_info_request.py
+-rw-rw-rw-   0        0        0     1913 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_task_request.py
+-rw-rw-rw-   0        0        0     2246 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_task_timephased_data_request.py
+-rw-rw-rw-   0        0        0     1842 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_tasks_request.py
+-rw-rw-rw-   0        0        0     1841 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_vba_project_request.py
+-rw-rw-rw-   0        0        0     1842 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_views_request.py
+-rw-rw-rw-   0        0        0     1851 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_wbs_definition_request.py
+-rw-rw-rw-   0        0        0     2161 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/move_file_request.py
+-rw-rw-rw-   0        0        0     2076 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/move_folder_request.py
+-rw-rw-rw-   0        0        0     1904 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/object_exists_request.py
+-rw-rw-rw-   0        0        0     2571 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/post_assignment_request.py
+-rw-rw-rw-   0        0        0     2338 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/post_calendar_exception_request.py
+-rw-rw-rw-   0        0        0     2164 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/post_calendar_request.py
+-rw-rw-rw-   0        0        0     2303 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/post_document_property_request.py
+-rw-rw-rw-   0        0        0     2479 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/post_resource_request.py
+-rw-rw-rw-   0        0        0     2435 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/post_task_document_with_format_request.py
+-rw-rw-rw-   0        0        0     2202 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/post_task_link_request.py
+-rw-rw-rw-   0        0        0     2519 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/post_task_recurring_info_request.py
+-rw-rw-rw-   0        0        0     2432 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/post_task_request.py
+-rw-rw-rw-   0        0        0     2063 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/post_tasks_request.py
+-rw-rw-rw-   0        0        0     2322 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_assignment_request.py
+-rw-rw-rw-   0        0        0     2459 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_calendar_exception_request.py
+-rw-rw-rw-   0        0        0     2292 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_calendar_request.py
+-rw-rw-rw-   0        0        0     2302 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_document_property_request.py
+-rw-rw-rw-   0        0        0     2264 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_extended_attribute_request.py
+-rw-rw-rw-   0        0        0     2575 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_import_project_from_db_request.py
+-rw-rw-rw-   0        0        0     2406 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_import_project_from_file_request.py
+-rw-rw-rw-   0        0        0     2834 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_import_project_from_project_online_request.py
+-rw-rw-rw-   0        0        0     2313 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_move_task_request.py
+-rw-rw-rw-   0        0        0     2356 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_move_task_to_sibling_request.py
+-rw-rw-rw-   0        0        0     2496 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_recalculate_project_request.py
+-rw-rw-rw-   0        0        0     2022 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_recalculate_project_resource_fields_request.py
+-rw-rw-rw-   0        0        0     2149 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_recalculate_project_uncomplete_work_to_start_after_request.py
+-rw-rw-rw-   0        0        0     2374 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_recalculate_project_work_as_complete_request.py
+-rw-rw-rw-   0        0        0     2281 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_renumber_wbs_code_request.py
+-rw-rw-rw-   0        0        0     2395 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_resource_request.py
+-rw-rw-rw-   0        0        0     2309 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_task_link_request.py
+-rw-rw-rw-   0        0        0     2193 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_task_recurring_info_request.py
+-rw-rw-rw-   0        0        0     2250 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_task_request.py
+-rw-rw-rw-   0        0        0     1711 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/storage_exists_request.py
+-rw-rw-rw-   0        0        0     2732 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/update_project_request.py
+-rw-rw-rw-   0        0        0     2201 2024-03-29 11:15:55.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/update_table_text_style_request.py
+-rw-rw-rw-   0        0        0     2095 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/upload_file_request.py
+-rw-rw-rw-   0        0        0    80226 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/resource.py
+-rw-rw-rw-   0        0        0    74662 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/resource_assignment.py
+-rw-rw-rw-   0        0        0     4149 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/resource_assignments.py
+-rw-rw-rw-   0        0        0     6025 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/resource_item.py
+-rw-rw-rw-   0        0        0     4404 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/resource_item_response.py
+-rw-rw-rw-   0        0        0     4262 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/resource_items.py
+-rw-rw-rw-   0        0        0     4232 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/resource_items_response.py
+-rw-rw-rw-   0        0        0     4245 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/resource_response.py
+-rw-rw-rw-   0        0        0     3572 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/resource_type.py
+-rw-rw-rw-   0        0        0     3767 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/rollup_type.py
+-rw-rw-rw-   0        0        0     4343 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/storage_exist.py
+-rw-rw-rw-   0        0        0     7540 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/storage_file.py
+-rw-rw-rw-   0        0        0     3706 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/summary_rows_calculation_type.py
+-rw-rw-rw-   0        0        0     9608 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/table_text_style.py
+-rw-rw-rw-   0        0        0     4520 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/table_text_style_response.py
+-rw-rw-rw-   0        0        0     4349 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/table_text_styles_response.py
+-rw-rw-rw-   0        0        0   118802 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task.py
+-rw-rw-rw-   0        0        0     9707 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_baseline.py
+-rw-rw-rw-   0        0        0     6191 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_creation_request.py
+-rw-rw-rw-   0        0        0     8325 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_item.py
+-rw-rw-rw-   0        0        0     4268 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_item_response.py
+-rw-rw-rw-   0        0        0     4138 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_items.py
+-rw-rw-rw-   0        0        0     4108 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_items_response.py
+-rw-rw-rw-   0        0        0     8939 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_link.py
+-rw-rw-rw-   0        0        0     4268 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_link_response.py
+-rw-rw-rw-   0        0        0     3661 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_link_type.py
+-rw-rw-rw-   0        0        0     4241 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_links_response.py
+-rw-rw-rw-   0        0        0     4113 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_response.py
+-rw-rw-rw-   0        0        0     3613 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_type.py
+-rw-rw-rw-   0        0        0     4400 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/text_item_type.py
+-rw-rw-rw-   0        0        0     4455 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/time_unit_type.py
+-rw-rw-rw-   0        0        0     9019 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/timephased_data.py
+-rw-rw-rw-   0        0        0     4200 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/timephased_data_response.py
+-rw-rw-rw-   0        0        0     7471 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/timephased_data_type.py
+-rw-rw-rw-   0        0        0     3633 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/timescale.py
+-rw-rw-rw-   0        0        0     8280 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/value.py
+-rw-rw-rw-   0        0        0     5890 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/vba_module.py
+-rw-rw-rw-   0        0        0     4970 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/vba_module_attribute.py
+-rw-rw-rw-   0        0        0     9544 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/vba_project.py
+-rw-rw-rw-   0        0        0     4257 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/vba_project_response.py
+-rw-rw-rw-   0        0        0     5080 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/vba_reference.py
+-rw-rw-rw-   0        0        0     7917 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/view.py
+-rw-rw-rw-   0        0        0     3989 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/view_screen.py
+-rw-rw-rw-   0        0        0     4182 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/views_response.py
+-rw-rw-rw-   0        0        0     6981 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/wbs_code_mask.py
+-rw-rw-rw-   0        0        0     7677 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/wbs_definition.py
+-rw-rw-rw-   0        0        0     4433 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/wbs_definition_response.py
+-rw-rw-rw-   0        0        0     3706 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/wbs_sequence.py
+-rw-rw-rw-   0        0        0     8230 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/week_day.py
+-rw-rw-rw-   0        0        0     3739 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/week_day_type.py
+-rw-rw-rw-   0        0        0     3788 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/work_contour_type.py
+-rw-rw-rw-   0        0        0     3594 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/work_group_type.py
+-rw-rw-rw-   0        0        0     6908 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/work_week.py
+-rw-rw-rw-   0        0        0     5417 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/models/working_time.py
+-rw-rw-rw-   0        0        0    14865 2024-03-29 11:15:54.000000 aspose_tasks_cloud-24.4.0/asposetaskscloud/rest.py
+-rw-rw-rw-   0        0        0       42 2024-04-30 10:13:49.345562 aspose_tasks_cloud-24.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1626 2024-03-30 06:50:36.000000 aspose_tasks_cloud-24.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:13:49.342491 aspose_tasks_cloud-24.4.0/test/
+-rw-rw-rw-   0        0        0     1454 2024-03-29 11:21:13.000000 aspose_tasks_cloud-24.4.0/test/__init__.py
+-rw-rw-rw-   0        0        0     3340 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/base_test_context.py
+-rw-rw-rw-   0        0        0     3298 2024-03-29 11:22:33.000000 aspose_tasks_cloud-24.4.0/test/test_api_coverage.py
+-rw-rw-rw-   0        0        0    10588 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_assignments.py
+-rw-rw-rw-   0        0        0     8621 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_calendar_exceptions.py
+-rw-rw-rw-   0        0        0     4665 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_calendar_work_weeks.py
+-rw-rw-rw-   0        0        0     8089 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_calendars.py
+-rw-rw-rw-   0        0        0     4954 2022-11-30 08:09:39.000000 aspose_tasks_cloud-24.4.0/test/test_document_properties.py
+-rw-rw-rw-   0        0        0     8995 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_extended_attributes.py
+-rw-rw-rw-   0        0        0     4695 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_file.py
+-rw-rw-rw-   0        0        0     4439 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_folder.py
+-rw-rw-rw-   0        0        0     2658 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_get_page_count.py
+-rw-rw-rw-   0        0        0     5718 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_import_project.py
+-rw-rw-rw-   0        0        0     3347 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_outline_codes.py
+-rw-rw-rw-   0        0        0     4935 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_project_online.py
+-rw-rw-rw-   0        0        0     2386 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_read_project.py
+-rw-rw-rw-   0        0        0     4867 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_recalculation.py
+-rw-rw-rw-   0        0        0     5717 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_recurring_info.py
+-rw-rw-rw-   0        0        0     3185 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_report.py
+-rw-rw-rw-   0        0        0     6715 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_resources.py
+-rw-rw-rw-   0        0        0     3118 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_storage.py
+-rw-rw-rw-   0        0        0     4237 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_task_document_format.py
+-rw-rw-rw-   0        0        0     4392 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_task_links.py
+-rw-rw-rw-   0        0        0    10130 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_tasks.py
+-rw-rw-rw-   0        0        0    14926 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_tasks_extended_attributes.py
+-rw-rw-rw-   0        0        0     2874 2022-11-30 08:05:13.000000 aspose_tasks_cloud-24.4.0/test/test_tasks_primavera_properties.py
+-rw-rw-rw-   0        0        0     3768 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_timephased_data.py
+-rw-rw-rw-   0        0        0     2235 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_vba.py
+-rw-rw-rw-   0        0        0     6892 2024-03-30 06:46:53.000000 aspose_tasks_cloud-24.4.0/test/test_views.py
+-rw-rw-rw-   0        0        0     2536 2022-07-21 09:04:59.000000 aspose_tasks_cloud-24.4.0/test/test_wbs.py
```

### Comparing `aspose-tasks-cloud-22.7.0/LICENSE` & `aspose_tasks_cloud-24.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/PKG-INFO` & `aspose_tasks_cloud-24.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspose-tasks-cloud
-Version: 22.7.0
+Version: 24.4.0
 Summary: Aspose.Tasks Cloud API Reference
 Home-page: https://github.com/aspose-tasks-cloud/aspose-tasks-cloud-python
 Author: Ivan Andreychikov
 Author-email: ivan.andreychikov@aspose.com
 Keywords: aspose,python,aspose cloud,microsoft project,mpp,primavera,microsoft project server,microsoft project online
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,18 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: urllib3>=1.16
+Requires-Dist: six>=1.10
+Requires-Dist: certifi
+Requires-Dist: python-dateutil
 
 ![](https://img.shields.io/badge/api-v3.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/aspose-tasks-cloud) ![PyPI - Format](https://img.shields.io/pypi/format/aspose-tasks-cloud) ![PyPI - Downloads](https://img.shields.io/pypi/dm/aspose-tasks-cloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aspose-tasks-cloud) [![GitHub license](https://img.shields.io/github/license/aspose-tasks-cloud/aspose-tasks-cloud-python)](https://github.com/aspose-tasks-cloud/aspose-tasks-cloud-php/blob/master/LICENSE) ![GitHub last commit](https://img.shields.io/github/last-commit/Aspose-tasks-Cloud/aspose-tasks-cloud-python)
 
 # Manipulate MS Project Files in Python via Cloud REST API
 
 Aspose.Tasks for Cloud offers the ability to manipulate and convert Microsoft Project MPT, MPP, MPX & Oracle Primavera XER, XML, and PrimaveraP6XML files in Python. [Aspose.Tasks Cloud SDK for Python](https://products.aspose.cloud/tasks/python) wraps the REST API to make it easier for the developers to integrate MS Project Task Management features in their own cloud-based Python applications on Linux, MacOS, Windows or Android.
 
@@ -51,14 +55,22 @@
 ## Read & Write Project Data
 **Microsoft Project** MPP, XML, MPT **Primavera** MPX
 
 ## Save Project Data As
 XER, XLSX, HTML, XML, TXT, TIF, SVG, PNG, JPEG
 
 
+## Enhancements in Version 24.4
+- Added new ability to get views information
+- Possibility to modify table text styles for Gantt Chart views.
+
+## Enhancements in Version 22.12
+- Added new ability to read Primavera-specific task's properties.
+- Provided the ability to read more document properties.
+
 ## Enhancements in Version 20.11
 - Support for the batch creation of tasks (i.e. the ability to create multiple tasks in a single *API* call).
 
 ## Enhancements in Version 20.8
 - Ability to specify the non-default path for Project Server's *PWA* URL.
 - Ability to modify *timephasedData* collection in assignments.
```

### Comparing `aspose-tasks-cloud-22.7.0/README.md` & `aspose_tasks_cloud-24.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,22 @@
 ## Read & Write Project Data
 **Microsoft Project** MPP, XML, MPT **Primavera** MPX
 
 ## Save Project Data As
 XER, XLSX, HTML, XML, TXT, TIF, SVG, PNG, JPEG
 
 
+## Enhancements in Version 24.4
+- Added new ability to get views information
+- Possibility to modify table text styles for Gantt Chart views.
+
+## Enhancements in Version 22.12
+- Added new ability to read Primavera-specific task's properties.
+- Provided the ability to read more document properties.
+
 ## Enhancements in Version 20.11
 - Support for the batch creation of tasks (i.e. the ability to create multiple tasks in a single *API* call).
 
 ## Enhancements in Version 20.8
 - Ability to specify the non-default path for Project Server's *PWA* URL.
 - Ability to modify *timephasedData* collection in assignments.
```

### Comparing `aspose-tasks-cloud-22.7.0/aspose_tasks_cloud.egg-info/PKG-INFO` & `aspose_tasks_cloud-24.4.0/aspose_tasks_cloud.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspose-tasks-cloud
-Version: 22.7.0
+Version: 24.4.0
 Summary: Aspose.Tasks Cloud API Reference
 Home-page: https://github.com/aspose-tasks-cloud/aspose-tasks-cloud-python
 Author: Ivan Andreychikov
 Author-email: ivan.andreychikov@aspose.com
 Keywords: aspose,python,aspose cloud,microsoft project,mpp,primavera,microsoft project server,microsoft project online
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,18 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: urllib3>=1.16
+Requires-Dist: six>=1.10
+Requires-Dist: certifi
+Requires-Dist: python-dateutil
 
 ![](https://img.shields.io/badge/api-v3.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/aspose-tasks-cloud) ![PyPI - Format](https://img.shields.io/pypi/format/aspose-tasks-cloud) ![PyPI - Downloads](https://img.shields.io/pypi/dm/aspose-tasks-cloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aspose-tasks-cloud) [![GitHub license](https://img.shields.io/github/license/aspose-tasks-cloud/aspose-tasks-cloud-python)](https://github.com/aspose-tasks-cloud/aspose-tasks-cloud-php/blob/master/LICENSE) ![GitHub last commit](https://img.shields.io/github/last-commit/Aspose-tasks-Cloud/aspose-tasks-cloud-python)
 
 # Manipulate MS Project Files in Python via Cloud REST API
 
 Aspose.Tasks for Cloud offers the ability to manipulate and convert Microsoft Project MPT, MPP, MPX & Oracle Primavera XER, XML, and PrimaveraP6XML files in Python. [Aspose.Tasks Cloud SDK for Python](https://products.aspose.cloud/tasks/python) wraps the REST API to make it easier for the developers to integrate MS Project Task Management features in their own cloud-based Python applications on Linux, MacOS, Windows or Android.
 
@@ -51,14 +55,22 @@
 ## Read & Write Project Data
 **Microsoft Project** MPP, XML, MPT **Primavera** MPX
 
 ## Save Project Data As
 XER, XLSX, HTML, XML, TXT, TIF, SVG, PNG, JPEG
 
 
+## Enhancements in Version 24.4
+- Added new ability to get views information
+- Possibility to modify table text styles for Gantt Chart views.
+
+## Enhancements in Version 22.12
+- Added new ability to read Primavera-specific task's properties.
+- Provided the ability to read more document properties.
+
 ## Enhancements in Version 20.11
 - Support for the batch creation of tasks (i.e. the ability to create multiple tasks in a single *API* call).
 
 ## Enhancements in Version 20.8
 - Ability to specify the non-default path for Project Server's *PWA* URL.
 - Ability to modify *timephasedData* collection in assignments.
```

### Comparing `aspose-tasks-cloud-22.7.0/aspose_tasks_cloud.egg-info/SOURCES.txt` & `aspose_tasks_cloud-24.4.0/aspose_tasks_cloud.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 asposetaskscloud/models/assignment_baseline.py
 asposetaskscloud/models/assignment_item.py
 asposetaskscloud/models/assignment_item_response.py
 asposetaskscloud/models/assignment_items.py
 asposetaskscloud/models/assignment_items_response.py
 asposetaskscloud/models/assignment_response.py
 asposetaskscloud/models/assignments_response.py
+asposetaskscloud/models/background_pattern.py
 asposetaskscloud/models/baseline.py
 asposetaskscloud/models/baseline_type.py
 asposetaskscloud/models/booking_type.py
 asposetaskscloud/models/calculation_mode.py
 asposetaskscloud/models/calculation_type.py
 asposetaskscloud/models/calendar.py
 asposetaskscloud/models/calendar_exception.py
@@ -32,14 +33,15 @@
 asposetaskscloud/models/calendar_exceptions_response.py
 asposetaskscloud/models/calendar_item.py
 asposetaskscloud/models/calendar_item_response.py
 asposetaskscloud/models/calendar_items.py
 asposetaskscloud/models/calendar_items_response.py
 asposetaskscloud/models/calendar_response.py
 asposetaskscloud/models/calendar_work_weeks_response.py
+asposetaskscloud/models/colors.py
 asposetaskscloud/models/confidence_level.py
 asposetaskscloud/models/constraint_type.py
 asposetaskscloud/models/cost_accrual_type.py
 asposetaskscloud/models/custom_field_type.py
 asposetaskscloud/models/day_of_week.py
 asposetaskscloud/models/day_type.py
 asposetaskscloud/models/disc_usage.py
@@ -55,19 +57,21 @@
 asposetaskscloud/models/extended_attribute.py
 asposetaskscloud/models/extended_attribute_definition.py
 asposetaskscloud/models/extended_attribute_item.py
 asposetaskscloud/models/extended_attribute_item_response.py
 asposetaskscloud/models/extended_attribute_items.py
 asposetaskscloud/models/extended_attribute_items_response.py
 asposetaskscloud/models/extended_attribute_response.py
+asposetaskscloud/models/field.py
 asposetaskscloud/models/file_version.py
 asposetaskscloud/models/file_versions.py
 asposetaskscloud/models/files_list.py
 asposetaskscloud/models/files_upload_result.py
 asposetaskscloud/models/imported_project_type.py
+asposetaskscloud/models/item_type.py
 asposetaskscloud/models/link.py
 asposetaskscloud/models/link_element.py
 asposetaskscloud/models/mask_type.py
 asposetaskscloud/models/month.py
 asposetaskscloud/models/month_item_type.py
 asposetaskscloud/models/month_position.py
 asposetaskscloud/models/object_exist.py
@@ -80,14 +84,16 @@
 asposetaskscloud/models/outline_code_response.py
 asposetaskscloud/models/outline_mask.py
 asposetaskscloud/models/outline_value.py
 asposetaskscloud/models/outline_value_type.py
 asposetaskscloud/models/page_count_response.py
 asposetaskscloud/models/page_size.py
 asposetaskscloud/models/presentation_format.py
+asposetaskscloud/models/primavera_task_properties.py
+asposetaskscloud/models/primavera_task_properties_response.py
 asposetaskscloud/models/probability_distribution_type.py
 asposetaskscloud/models/project_database_type.py
 asposetaskscloud/models/project_file_format.py
 asposetaskscloud/models/project_ids_response.py
 asposetaskscloud/models/project_info.py
 asposetaskscloud/models/project_list.py
 asposetaskscloud/models/project_list_response.py
@@ -111,38 +117,45 @@
 asposetaskscloud/models/resource_items_response.py
 asposetaskscloud/models/resource_response.py
 asposetaskscloud/models/resource_type.py
 asposetaskscloud/models/rollup_type.py
 asposetaskscloud/models/storage_exist.py
 asposetaskscloud/models/storage_file.py
 asposetaskscloud/models/summary_rows_calculation_type.py
+asposetaskscloud/models/table_text_style.py
+asposetaskscloud/models/table_text_style_response.py
+asposetaskscloud/models/table_text_styles_response.py
 asposetaskscloud/models/task.py
 asposetaskscloud/models/task_baseline.py
 asposetaskscloud/models/task_creation_request.py
 asposetaskscloud/models/task_item.py
 asposetaskscloud/models/task_item_response.py
 asposetaskscloud/models/task_items.py
 asposetaskscloud/models/task_items_response.py
 asposetaskscloud/models/task_link.py
 asposetaskscloud/models/task_link_response.py
 asposetaskscloud/models/task_link_type.py
 asposetaskscloud/models/task_links_response.py
 asposetaskscloud/models/task_response.py
 asposetaskscloud/models/task_type.py
+asposetaskscloud/models/text_item_type.py
 asposetaskscloud/models/time_unit_type.py
 asposetaskscloud/models/timephased_data.py
 asposetaskscloud/models/timephased_data_response.py
 asposetaskscloud/models/timephased_data_type.py
 asposetaskscloud/models/timescale.py
 asposetaskscloud/models/value.py
 asposetaskscloud/models/vba_module.py
 asposetaskscloud/models/vba_module_attribute.py
 asposetaskscloud/models/vba_project.py
 asposetaskscloud/models/vba_project_response.py
 asposetaskscloud/models/vba_reference.py
+asposetaskscloud/models/view.py
+asposetaskscloud/models/view_screen.py
+asposetaskscloud/models/views_response.py
 asposetaskscloud/models/wbs_code_mask.py
 asposetaskscloud/models/wbs_definition.py
 asposetaskscloud/models/wbs_definition_response.py
 asposetaskscloud/models/wbs_sequence.py
 asposetaskscloud/models/week_day.py
 asposetaskscloud/models/week_day_type.py
 asposetaskscloud/models/work_contour_type.py
@@ -150,25 +163,28 @@
 asposetaskscloud/models/work_week.py
 asposetaskscloud/models/working_time.py
 asposetaskscloud/models/requests/__init__.py
 asposetaskscloud/models/requests/copy_file_request.py
 asposetaskscloud/models/requests/copy_folder_request.py
 asposetaskscloud/models/requests/create_folder_request.py
 asposetaskscloud/models/requests/create_new_project_request.py
+asposetaskscloud/models/requests/create_table_text_style_request.py
 asposetaskscloud/models/requests/delete_assignment_request.py
 asposetaskscloud/models/requests/delete_calendar_exception_request.py
 asposetaskscloud/models/requests/delete_calendar_request.py
 asposetaskscloud/models/requests/delete_extended_attribute_by_index_request.py
 asposetaskscloud/models/requests/delete_file_request.py
 asposetaskscloud/models/requests/delete_folder_request.py
 asposetaskscloud/models/requests/delete_outline_code_by_index_request.py
 asposetaskscloud/models/requests/delete_resource_request.py
+asposetaskscloud/models/requests/delete_table_text_style_request.py
 asposetaskscloud/models/requests/delete_task_link_request.py
 asposetaskscloud/models/requests/delete_task_request.py
 asposetaskscloud/models/requests/download_file_request.py
+asposetaskscloud/models/requests/get_all_table_text_styles_request.py
 asposetaskscloud/models/requests/get_assignment_request.py
 asposetaskscloud/models/requests/get_assignment_timephased_data_request.py
 asposetaskscloud/models/requests/get_assignments_request.py
 asposetaskscloud/models/requests/get_calendar_exceptions_request.py
 asposetaskscloud/models/requests/get_calendar_request.py
 asposetaskscloud/models/requests/get_calendar_work_weeks_request.py
 asposetaskscloud/models/requests/get_calendars_request.py
@@ -179,31 +195,34 @@
 asposetaskscloud/models/requests/get_extended_attribute_by_index_request.py
 asposetaskscloud/models/requests/get_extended_attributes_request.py
 asposetaskscloud/models/requests/get_file_versions_request.py
 asposetaskscloud/models/requests/get_files_list_request.py
 asposetaskscloud/models/requests/get_outline_code_by_index_request.py
 asposetaskscloud/models/requests/get_outline_codes_request.py
 asposetaskscloud/models/requests/get_page_count_request.py
+asposetaskscloud/models/requests/get_primavera_task_properties_request.py
 asposetaskscloud/models/requests/get_project_ids_request.py
 asposetaskscloud/models/requests/get_project_list_request.py
 asposetaskscloud/models/requests/get_report_pdf_request.py
 asposetaskscloud/models/requests/get_resource_assignments_request.py
 asposetaskscloud/models/requests/get_resource_request.py
 asposetaskscloud/models/requests/get_resource_timephased_data_request.py
 asposetaskscloud/models/requests/get_resources_request.py
 asposetaskscloud/models/requests/get_risk_analysis_report_request.py
+asposetaskscloud/models/requests/get_table_text_style_request.py
 asposetaskscloud/models/requests/get_task_assignments_request.py
 asposetaskscloud/models/requests/get_task_document_request.py
 asposetaskscloud/models/requests/get_task_document_with_format_request.py
 asposetaskscloud/models/requests/get_task_links_request.py
 asposetaskscloud/models/requests/get_task_recurring_info_request.py
 asposetaskscloud/models/requests/get_task_request.py
 asposetaskscloud/models/requests/get_task_timephased_data_request.py
 asposetaskscloud/models/requests/get_tasks_request.py
 asposetaskscloud/models/requests/get_vba_project_request.py
+asposetaskscloud/models/requests/get_views_request.py
 asposetaskscloud/models/requests/get_wbs_definition_request.py
 asposetaskscloud/models/requests/move_file_request.py
 asposetaskscloud/models/requests/move_folder_request.py
 asposetaskscloud/models/requests/object_exists_request.py
 asposetaskscloud/models/requests/post_assignment_request.py
 asposetaskscloud/models/requests/post_calendar_exception_request.py
 asposetaskscloud/models/requests/post_calendar_request.py
@@ -231,14 +250,15 @@
 asposetaskscloud/models/requests/put_renumber_wbs_code_request.py
 asposetaskscloud/models/requests/put_resource_request.py
 asposetaskscloud/models/requests/put_task_link_request.py
 asposetaskscloud/models/requests/put_task_recurring_info_request.py
 asposetaskscloud/models/requests/put_task_request.py
 asposetaskscloud/models/requests/storage_exists_request.py
 asposetaskscloud/models/requests/update_project_request.py
+asposetaskscloud/models/requests/update_table_text_style_request.py
 asposetaskscloud/models/requests/upload_file_request.py
 test/__init__.py
 test/base_test_context.py
 test/test_api_coverage.py
 test/test_assignments.py
 test/test_calendar_exceptions.py
 test/test_calendar_work_weeks.py
@@ -257,10 +277,12 @@
 test/test_report.py
 test/test_resources.py
 test/test_storage.py
 test/test_task_document_format.py
 test/test_task_links.py
 test/test_tasks.py
 test/test_tasks_extended_attributes.py
+test/test_tasks_primavera_properties.py
 test/test_timephased_data.py
 test/test_vba.py
+test/test_views.py
 test/test_wbs.py
```

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/__init__.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 
 # import ApiClient
 from asposetaskscloud.api_client import ApiClient
 from asposetaskscloud.configuration import Configuration
 # import models into sdk package
 from asposetaskscloud.models.aspose_response import AsposeResponse
 from asposetaskscloud.models.assignment_item import AssignmentItem
+from asposetaskscloud.models.background_pattern import BackgroundPattern
 from asposetaskscloud.models.baseline import Baseline
 from asposetaskscloud.models.baseline_type import BaselineType
 from asposetaskscloud.models.booking_type import BookingType
 from asposetaskscloud.models.calculation_mode import CalculationMode
 from asposetaskscloud.models.calculation_type import CalculationType
 from asposetaskscloud.models.calendar import Calendar
 from asposetaskscloud.models.calendar_exception import CalendarException
 from asposetaskscloud.models.calendar_exception_type import CalendarExceptionType
 from asposetaskscloud.models.calendar_item import CalendarItem
+from asposetaskscloud.models.colors import Colors
 from asposetaskscloud.models.confidence_level import ConfidenceLevel
 from asposetaskscloud.models.constraint_type import ConstraintType
 from asposetaskscloud.models.cost_accrual_type import CostAccrualType
 from asposetaskscloud.models.custom_field_type import CustomFieldType
 from asposetaskscloud.models.day_of_week import DayOfWeek
 from asposetaskscloud.models.day_type import DayType
 from asposetaskscloud.models.disc_usage import DiscUsage
@@ -33,18 +35,20 @@
 from asposetaskscloud.models.earned_value_method_type import EarnedValueMethodType
 from asposetaskscloud.models.element_type import ElementType
 from asposetaskscloud.models.error import Error
 from asposetaskscloud.models.error_details import ErrorDetails
 from asposetaskscloud.models.extended_attribute import ExtendedAttribute
 from asposetaskscloud.models.extended_attribute_definition import ExtendedAttributeDefinition
 from asposetaskscloud.models.extended_attribute_item import ExtendedAttributeItem
+from asposetaskscloud.models.field import Field
 from asposetaskscloud.models.file_versions import FileVersions
 from asposetaskscloud.models.files_list import FilesList
 from asposetaskscloud.models.files_upload_result import FilesUploadResult
 from asposetaskscloud.models.imported_project_type import ImportedProjectType
+from asposetaskscloud.models.item_type import ItemType
 from asposetaskscloud.models.link import Link
 from asposetaskscloud.models.link_element import LinkElement
 from asposetaskscloud.models.mask_type import MaskType
 from asposetaskscloud.models.month import Month
 from asposetaskscloud.models.month_item_type import MonthItemType
 from asposetaskscloud.models.month_position import MonthPosition
 from asposetaskscloud.models.object_exist import ObjectExist
@@ -53,14 +57,15 @@
 from asposetaskscloud.models.outline_code_definition import OutlineCodeDefinition
 from asposetaskscloud.models.outline_code_item import OutlineCodeItem
 from asposetaskscloud.models.outline_mask import OutlineMask
 from asposetaskscloud.models.outline_value import OutlineValue
 from asposetaskscloud.models.outline_value_type import OutlineValueType
 from asposetaskscloud.models.page_size import PageSize
 from asposetaskscloud.models.presentation_format import PresentationFormat
+from asposetaskscloud.models.primavera_task_properties import PrimaveraTaskProperties
 from asposetaskscloud.models.probability_distribution_type import ProbabilityDistributionType
 from asposetaskscloud.models.project_database_type import ProjectDatabaseType
 from asposetaskscloud.models.project_file_format import ProjectFileFormat
 from asposetaskscloud.models.project_info import ProjectInfo
 from asposetaskscloud.models.project_recalculation_result import ProjectRecalculationResult
 from asposetaskscloud.models.project_server_save_options_dto import ProjectServerSaveOptionsDTO
 from asposetaskscloud.models.project_validation_state import ProjectValidationState
@@ -74,29 +79,33 @@
 from asposetaskscloud.models.resource_assignment import ResourceAssignment
 from asposetaskscloud.models.resource_item import ResourceItem
 from asposetaskscloud.models.resource_type import ResourceType
 from asposetaskscloud.models.rollup_type import RollupType
 from asposetaskscloud.models.storage_exist import StorageExist
 from asposetaskscloud.models.storage_file import StorageFile
 from asposetaskscloud.models.summary_rows_calculation_type import SummaryRowsCalculationType
+from asposetaskscloud.models.table_text_style import TableTextStyle
 from asposetaskscloud.models.task import Task
 from asposetaskscloud.models.task_creation_request import TaskCreationRequest
 from asposetaskscloud.models.task_item import TaskItem
 from asposetaskscloud.models.task_link import TaskLink
 from asposetaskscloud.models.task_link_type import TaskLinkType
 from asposetaskscloud.models.task_type import TaskType
+from asposetaskscloud.models.text_item_type import TextItemType
 from asposetaskscloud.models.time_unit_type import TimeUnitType
 from asposetaskscloud.models.timephased_data import TimephasedData
 from asposetaskscloud.models.timephased_data_type import TimephasedDataType
 from asposetaskscloud.models.timescale import Timescale
 from asposetaskscloud.models.value import Value
 from asposetaskscloud.models.vba_module import VbaModule
 from asposetaskscloud.models.vba_module_attribute import VbaModuleAttribute
 from asposetaskscloud.models.vba_project import VbaProject
 from asposetaskscloud.models.vba_reference import VbaReference
+from asposetaskscloud.models.view import View
+from asposetaskscloud.models.view_screen import ViewScreen
 from asposetaskscloud.models.wbs_code_mask import WBSCodeMask
 from asposetaskscloud.models.wbs_definition import WBSDefinition
 from asposetaskscloud.models.wbs_sequence import WBSSequence
 from asposetaskscloud.models.week_day import WeekDay
 from asposetaskscloud.models.week_day_type import WeekDayType
 from asposetaskscloud.models.work_contour_type import WorkContourType
 from asposetaskscloud.models.work_group_type import WorkGroupType
@@ -123,33 +132,37 @@
 from asposetaskscloud.models.extended_attribute_items_response import ExtendedAttributeItemsResponse
 from asposetaskscloud.models.extended_attribute_response import ExtendedAttributeResponse
 from asposetaskscloud.models.file_version import FileVersion
 from asposetaskscloud.models.outline_code_items import OutlineCodeItems
 from asposetaskscloud.models.outline_code_items_response import OutlineCodeItemsResponse
 from asposetaskscloud.models.outline_code_response import OutlineCodeResponse
 from asposetaskscloud.models.page_count_response import PageCountResponse
+from asposetaskscloud.models.primavera_task_properties_response import PrimaveraTaskPropertiesResponse
 from asposetaskscloud.models.project_ids_response import ProjectIdsResponse
 from asposetaskscloud.models.project_list import ProjectList
 from asposetaskscloud.models.project_list_response import ProjectListResponse
 from asposetaskscloud.models.project_recalculate_response import ProjectRecalculateResponse
 from asposetaskscloud.models.recurring_info_response import RecurringInfoResponse
 from asposetaskscloud.models.resource_assignments import ResourceAssignments
 from asposetaskscloud.models.resource_item_response import ResourceItemResponse
 from asposetaskscloud.models.resource_items import ResourceItems
 from asposetaskscloud.models.resource_items_response import ResourceItemsResponse
 from asposetaskscloud.models.resource_response import ResourceResponse
+from asposetaskscloud.models.table_text_style_response import TableTextStyleResponse
+from asposetaskscloud.models.table_text_styles_response import TableTextStylesResponse
 from asposetaskscloud.models.task_baseline import TaskBaseline
 from asposetaskscloud.models.task_item_response import TaskItemResponse
 from asposetaskscloud.models.task_items import TaskItems
 from asposetaskscloud.models.task_items_response import TaskItemsResponse
 from asposetaskscloud.models.task_link_response import TaskLinkResponse
 from asposetaskscloud.models.task_links_response import TaskLinksResponse
 from asposetaskscloud.models.task_response import TaskResponse
 from asposetaskscloud.models.timephased_data_response import TimephasedDataResponse
 from asposetaskscloud.models.vba_project_response import VbaProjectResponse
+from asposetaskscloud.models.views_response import ViewsResponse
 from asposetaskscloud.models.wbs_definition_response import WBSDefinitionResponse
 
 from asposetaskscloud.models.requests.copy_file_request import CopyFileRequest
 from asposetaskscloud.models.requests.delete_file_request import DeleteFileRequest
 from asposetaskscloud.models.requests.download_file_request import DownloadFileRequest
 from asposetaskscloud.models.requests.move_file_request import MoveFileRequest
 from asposetaskscloud.models.requests.upload_file_request import UploadFileRequest
@@ -210,14 +223,15 @@
 from asposetaskscloud.models.requests.get_resource_assignments_request import GetResourceAssignmentsRequest
 from asposetaskscloud.models.requests.get_resource_timephased_data_request import GetResourceTimephasedDataRequest
 from asposetaskscloud.models.requests.get_resources_request import GetResourcesRequest
 from asposetaskscloud.models.requests.post_resource_request import PostResourceRequest
 from asposetaskscloud.models.requests.put_resource_request import PutResourceRequest
 from asposetaskscloud.models.requests.get_risk_analysis_report_request import GetRiskAnalysisReportRequest
 from asposetaskscloud.models.requests.delete_task_request import DeleteTaskRequest
+from asposetaskscloud.models.requests.get_primavera_task_properties_request import GetPrimaveraTaskPropertiesRequest
 from asposetaskscloud.models.requests.get_task_request import GetTaskRequest
 from asposetaskscloud.models.requests.get_task_assignments_request import GetTaskAssignmentsRequest
 from asposetaskscloud.models.requests.get_task_recurring_info_request import GetTaskRecurringInfoRequest
 from asposetaskscloud.models.requests.get_task_timephased_data_request import GetTaskTimephasedDataRequest
 from asposetaskscloud.models.requests.get_tasks_request import GetTasksRequest
 from asposetaskscloud.models.requests.post_task_request import PostTaskRequest
 from asposetaskscloud.models.requests.post_task_recurring_info_request import PostTaskRecurringInfoRequest
@@ -227,10 +241,16 @@
 from asposetaskscloud.models.requests.put_task_request import PutTaskRequest
 from asposetaskscloud.models.requests.put_task_recurring_info_request import PutTaskRecurringInfoRequest
 from asposetaskscloud.models.requests.delete_task_link_request import DeleteTaskLinkRequest
 from asposetaskscloud.models.requests.get_task_links_request import GetTaskLinksRequest
 from asposetaskscloud.models.requests.post_task_link_request import PostTaskLinkRequest
 from asposetaskscloud.models.requests.put_task_link_request import PutTaskLinkRequest
 from asposetaskscloud.models.requests.get_vba_project_request import GetVbaProjectRequest
+from asposetaskscloud.models.requests.create_table_text_style_request import CreateTableTextStyleRequest
+from asposetaskscloud.models.requests.delete_table_text_style_request import DeleteTableTextStyleRequest
+from asposetaskscloud.models.requests.get_all_table_text_styles_request import GetAllTableTextStylesRequest
+from asposetaskscloud.models.requests.get_table_text_style_request import GetTableTextStyleRequest
+from asposetaskscloud.models.requests.get_views_request import GetViewsRequest
+from asposetaskscloud.models.requests.update_table_text_style_request import UpdateTableTextStyleRequest
 from asposetaskscloud.models.requests.get_wbs_definition_request import GetWbsDefinitionRequest
 from asposetaskscloud.models.requests.put_renumber_wbs_code_request import PutRenumberWbsCodeRequest
 from asposetaskscloud.models.requests.post_task_document_with_format_request import PostTaskDocumentWithFormatRequest
```

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/api/tasks_api.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/api/tasks_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -8012,14 +8012,129 @@
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def get_primavera_task_properties(self, request, **kwargs):  # noqa: E501
+        """Get primavera properties for a task with the specified Uid.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+
+        :param is_async bool
+        :param name str : The name of the file. (required)
+        :param task_uid int : Uid of task to get primavera properties for. (required)
+        :param folder str : The document folder.
+        :param storage str : The document storage.
+        :return: PrimaveraTaskPropertiesResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        try:
+            if kwargs.get('is_async'):
+                return self.get_primavera_task_properties_with_http_info(request, **kwargs)  # noqa: E501
+            (data) = self.get_primavera_task_properties_with_http_info(request, **kwargs)  # noqa: E501
+            return data
+        except ApiException as e:
+            if e.status == 401:
+                self.__request_token()
+                if kwargs.get('is_async'):
+                    return self.get_primavera_task_properties_with_http_info(request, **kwargs)  # noqa: E501
+            (data) = self.get_primavera_task_properties_with_http_info(request, **kwargs)  # noqa: E501
+            return data
+        
+    def get_primavera_task_properties_with_http_info(self, request, **kwargs):  # noqa: E501
+        """Get primavera properties for a task with the specified Uid.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+
+        :param is_async bool
+        :param request get_primavera_task_properties_request object with parameters
+        :return: PrimaveraTaskPropertiesResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        params = locals()
+        params['is_async'] = ''
+        params['_return_http_data_only'] = False
+        params['_preload_content'] = True
+        params['_request_timeout'] = ''
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_primavera_task_properties" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if request.name is None:
+            raise ValueError("Missing the required parameter `name` when calling `get_primavera_task_properties`")  # noqa: E501
+        # verify the required parameter 'task_uid' is set
+        if request.task_uid is None:
+            raise ValueError("Missing the required parameter `task_uid` when calling `get_primavera_task_properties`")  # noqa: E501
+
+        collection_formats = {}
+        path = '/tasks/{name}/tasks/{taskUid}/primaveraProperties'
+        path_params = {}
+        if request.name is not None:
+            path_params[self.__downcase_first_letter('name')] = request.name  # noqa: E501
+        if request.task_uid is not None:
+            path_params[self.__downcase_first_letter('taskUid')] = request.task_uid  # noqa: E501
+
+        query_params = []
+        if '{' + self.__downcase_first_letter('folder') + '}' in path:
+            path = path.replace('{' + self.__downcase_first_letter('folder' + '}'), request.folder if request.folder is not None else '')
+        else:
+            if request.folder is not None:
+                query_params.append((self.__downcase_first_letter('folder'), request.folder))  # noqa: E501
+        if '{' + self.__downcase_first_letter('storage') + '}' in path:
+            path = path.replace('{' + self.__downcase_first_letter('storage' + '}'), request.storage if request.storage is not None else '')
+        else:
+            if request.storage is not None:
+                query_params.append((self.__downcase_first_letter('storage'), request.storage))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = []
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            path, 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PrimaveraTaskPropertiesResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def get_task(self, request, **kwargs):  # noqa: E501
         """Read project task.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass is_async=True
 
         :param is_async bool
@@ -10110,14 +10225,753 @@
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+
+    def create_table_text_style(self, request, **kwargs):  # noqa: E501
+        """Create table text style in specified view.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+
+        :param is_async bool
+        :param name str : The name of the file. (required)
+        :param view_uid int : Uid of the view. (required)
+        :param table_text_style TableTextStyle : A DTO of TableTextStyle to create (required)
+        :param file_name str : File name to save changes to.
+        :param storage str : The document storage.
+        :param folder str : The document folder.
+        :return: AsposeResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        try:
+            if kwargs.get('is_async'):
+                return self.create_table_text_style_with_http_info(request, **kwargs)  # noqa: E501
+            (data) = self.create_table_text_style_with_http_info(request, **kwargs)  # noqa: E501
+            return data
+        except ApiException as e:
+            if e.status == 401:
+                self.__request_token()
+                if kwargs.get('is_async'):
+                    return self.create_table_text_style_with_http_info(request, **kwargs)  # noqa: E501
+            (data) = self.create_table_text_style_with_http_info(request, **kwargs)  # noqa: E501
+            return data
+        
+    def create_table_text_style_with_http_info(self, request, **kwargs):  # noqa: E501
+        """Create table text style in specified view.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+
+        :param is_async bool
+        :param request create_table_text_style_request object with parameters
+        :return: AsposeResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        params = locals()
+        params['is_async'] = ''
+        params['_return_http_data_only'] = False
+        params['_preload_content'] = True
+        params['_request_timeout'] = ''
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method create_table_text_style" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if request.name is None:
+            raise ValueError("Missing the required parameter `name` when calling `create_table_text_style`")  # noqa: E501
+        # verify the required parameter 'view_uid' is set
+        if request.view_uid is None:
+            raise ValueError("Missing the required parameter `view_uid` when calling `create_table_text_style`")  # noqa: E501
+        # verify the required parameter 'table_text_style' is set
+        if request.table_text_style is None:
+            raise ValueError("Missing the required parameter `table_text_style` when calling `create_table_text_style`")  # noqa: E501
+
+        collection_formats = {}
+        path = '/tasks/{name}/views/{viewUid}/tabletextstyles'
+        path_params = {}
+        if request.name is not None:
+            path_params[self.__downcase_first_letter('name')] = request.name  # noqa: E501
+        if request.view_uid is not None:
+            path_params[self.__downcase_first_letter('viewUid')] = request.view_uid  # noqa: E501
+
+        query_params = []
+        if '{' + self.__downcase_first_letter('fileName') + '}' in path:
+            path = path.replace('{' + self.__downcase_first_letter('fileName' + '}'), request.file_name if request.file_name is not None else '')
+        else:
+            if request.file_name is not None:
+                query_params.append((self.__downcase_first_letter('fileName'), request.file_name))  # noqa: E501
+        if '{' + self.__downcase_first_letter('storage') + '}' in path:
+            path = path.replace('{' + self.__downcase_first_letter('storage' + '}'), request.storage if request.storage is not None else '')
+        else:
+            if request.storage is not None:
+                query_params.append((self.__downcase_first_letter('storage'), request.storage))  # noqa: E501
+        if '{' + self.__downcase_first_letter('folder') + '}' in path:
+            path = path.replace('{' + self.__downcase_first_letter('folder' + '}'), request.folder if request.folder is not None else '')
+        else:
+            if request.folder is not None:
+                query_params.append((self.__downcase_first_letter('folder'), request.folder))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = []
+
+        body_params = None
+        if request.table_text_style is not None:
+            body_params = request.table_text_style
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            path, 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='AsposeResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def delete_table_text_style(self, request, **kwargs):  # noqa: E501
+        """Delete specified table text style from specified view.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+
+        :param is_async bool
+        :param name str : The name of the file. (required)
+        :param view_uid int : Uid of the view. (required)
+        :param row_uid int : Uid of the row. (required)
+        :param field str : Specifies exact field of the row
+        :param file_name str : File name to save changes to.
+        :param storage str : The document storage.
+        :param folder str : The document folder.
+        :return: AsposeResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        try:
+            if kwargs.get('is_async'):
+                return self.delete_table_text_style_with_http_info(request, **kwargs)  # noqa: E501
+            (data) = self.delete_table_text_style_with_http_info(request, **kwargs)  # noqa: E501
+            return data
+        except ApiException as e:
+            if e.status == 401:
+                self.__request_token()
+                if kwargs.get('is_async'):
+                    return self.delete_table_text_style_with_http_info(request, **kwargs)  # noqa: E501
+            (data) = self.delete_table_text_style_with_http_info(request, **kwargs)  # noqa: E501
+            return data
+        
+    def delete_table_text_style_with_http_info(self, request, **kwargs):  # noqa: E501
+        """Delete specified table text style from specified view.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+
+        :param is_async bool
+        :param request delete_table_text_style_request object with parameters
+        :return: AsposeResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        params = locals()
+        params['is_async'] = ''
+        params['_return_http_data_only'] = False
+        params['_preload_content'] = True
+        params['_request_timeout'] = ''
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method delete_table_text_style" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if request.name is None:
+            raise ValueError("Missing the required parameter `name` when calling `delete_table_text_style`")  # noqa: E501
+        # verify the required parameter 'view_uid' is set
+        if request.view_uid is None:
+            raise ValueError("Missing the required parameter `view_uid` when calling `delete_table_text_style`")  # noqa: E501
+        # verify the required parameter 'row_uid' is set
+        if request.row_uid is None:
+            raise ValueError("Missing the required parameter `row_uid` when calling `delete_table_text_style`")  # noqa: E501
+
+        collection_formats = {}
+        path = '/tasks/{name}/views/{viewUid}/tabletextstyles/{rowUid}'
+        path_params = {}
+        if request.name is not None:
+            path_params[self.__downcase_first_letter('name')] = request.name  # noqa: E501
+        if request.view_uid is not None:
+            path_params[self.__downcase_first_letter('viewUid')] = request.view_uid  # noqa: E501
+        if request.row_uid is not None:
+            path_params[self.__downcase_first_letter('rowUid')] = request.row_uid  # noqa: E501
+
+        query_params = []
+        if '{' + self.__downcase_first_letter('field') + '}' in path:
+            path = path.replace('{' + self.__downcase_first_letter('field' + '}'), request.field if request.field is not None else '')
+        else:
+            if request.field is not None:
+                query_params.append((self.__downcase_first_letter('field'), request.field))  # noqa: E501
+        if '{' + self.__downcase_first_letter('fileName') + '}' in path:
+            path = path.replace('{' + self.__downcase_first_letter('fileName' + '}'), request.file_name if request.file_name is not None else '')
+        else:
+            if request.file_name is not None:
+                query_params.append((self.__downcase_first_letter('fileName'), request.file_name))  # noqa: E501
+        if '{' + self.__downcase_first_letter('storage') + '}' in path:
+            path = path.replace('{' + self.__downcase_first_letter('storage' + '}'), request.storage if request.storage is not None else '')
+        else:
+            if request.storage is not None:
+                query_params.append((self.__downcase_first_letter('storage'), request.storage))  # noqa: E501
+        if '{' + self.__downcase_first_letter('folder') + '}' in path:
+            path = path.replace('{' + self.__downcase_first_letter('folder' + '}'), request.folder if request.folder is not None else '')
+        else:
+            if request.folder is not None:
+                query_params.append((self.__downcase_first_letter('folder'), request.folder))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = []
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            path, 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='AsposeResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_all_table_text_styles(self, request, **kwargs):  # noqa: E501
+        """Read all table text styles from specified view.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+
+        :param is_async bool
+        :param name str : The name of the file. (required)
+        :param view_uid int : Uid of the view. (required)
+        :param storage str : The document storage.
+        :param folder str : The document folder.
+        :return: TableTextStylesResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        try:
+            if kwargs.get('is_async'):
+                return self.get_all_table_text_styles_with_http_info(request, **kwargs)  # noqa: E501
+            (data) = self.get_all_table_text_styles_with_http_info(request, **kwargs)  # noqa: E501
+            return data
+        except ApiException as e:
+            if e.status == 401:
+                self.__request_token()
+                if kwargs.get('is_async'):
+                    return self.get_all_table_text_styles_with_http_info(request, **kwargs)  # noqa: E501
+            (data) = self.get_all_table_text_styles_with_http_info(request, **kwargs)  # noqa: E501
+            return data
+        
+    def get_all_table_text_styles_with_http_info(self, request, **kwargs):  # noqa: E501
+        """Read all table text styles from specified view.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+
+        :param is_async bool
+        :param request get_all_table_text_styles_request object with parameters
+        :return: TableTextStylesResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        params = locals()
+        params['is_async'] = ''
+        params['_return_http_data_only'] = False
+        params['_preload_content'] = True
+        params['_request_timeout'] = ''
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_all_table_text_styles" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if request.name is None:
+            raise ValueError("Missing the required parameter `name` when calling `get_all_table_text_styles`")  # noqa: E501
+        # verify the required parameter 'view_uid' is set
+        if request.view_uid is None:
+            raise ValueError("Missing the required parameter `view_uid` when calling `get_all_table_text_styles`")  # noqa: E501
+
+        collection_formats = {}
+        path = '/tasks/{name}/views/{viewUid}/tabletextstyles'
+        path_params = {}
+        if request.name is not None:
+            path_params[self.__downcase_first_letter('name')] = request.name  # noqa: E501
+        if request.view_uid is not None:
+            path_params[self.__downcase_first_letter('viewUid')] = request.view_uid  # noqa: E501
+
+        query_params = []
+        if '{' + self.__downcase_first_letter('storage') + '}' in path:
+            path = path.replace('{' + self.__downcase_first_letter('storage' + '}'), request.storage if request.storage is not None else '')
+        else:
+            if request.storage is not None:
+                query_params.append((self.__downcase_first_letter('storage'), request.storage))  # noqa: E501
+        if '{' + self.__downcase_first_letter('folder') + '}' in path:
+            path = path.replace('{' + self.__downcase_first_letter('folder' + '}'), request.folder if request.folder is not None else '')
+        else:
+            if request.folder is not None:
+                query_params.append((self.__downcase_first_letter('folder'), request.folder))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = []
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            path, 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='TableTextStylesResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_table_text_style(self, request, **kwargs):  # noqa: E501
+        """Read specified table text style from specified view.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+
+        :param is_async bool
+        :param name str : The name of the file. (required)
+        :param view_uid int : Uid of the view. (required)
+        :param row_uid int : Uid of the row. (required)
+        :param field str : Specifies exact field of the row
+        :param storage str : The document storage.
+        :param folder str : The document folder.
+        :return: TableTextStyleResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        try:
+            if kwargs.get('is_async'):
+                return self.get_table_text_style_with_http_info(request, **kwargs)  # noqa: E501
+            (data) = self.get_table_text_style_with_http_info(request, **kwargs)  # noqa: E501
+            return data
+        except ApiException as e:
+            if e.status == 401:
+                self.__request_token()
+                if kwargs.get('is_async'):
+                    return self.get_table_text_style_with_http_info(request, **kwargs)  # noqa: E501
+            (data) = self.get_table_text_style_with_http_info(request, **kwargs)  # noqa: E501
+            return data
+        
+    def get_table_text_style_with_http_info(self, request, **kwargs):  # noqa: E501
+        """Read specified table text style from specified view.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+
+        :param is_async bool
+        :param request get_table_text_style_request object with parameters
+        :return: TableTextStyleResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        params = locals()
+        params['is_async'] = ''
+        params['_return_http_data_only'] = False
+        params['_preload_content'] = True
+        params['_request_timeout'] = ''
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_table_text_style" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if request.name is None:
+            raise ValueError("Missing the required parameter `name` when calling `get_table_text_style`")  # noqa: E501
+        # verify the required parameter 'view_uid' is set
+        if request.view_uid is None:
+            raise ValueError("Missing the required parameter `view_uid` when calling `get_table_text_style`")  # noqa: E501
+        # verify the required parameter 'row_uid' is set
+        if request.row_uid is None:
+            raise ValueError("Missing the required parameter `row_uid` when calling `get_table_text_style`")  # noqa: E501
+
+        collection_formats = {}
+        path = '/tasks/{name}/views/{viewUid}/tabletextstyles/{rowUid}'
+        path_params = {}
+        if request.name is not None:
+            path_params[self.__downcase_first_letter('name')] = request.name  # noqa: E501
+        if request.view_uid is not None:
+            path_params[self.__downcase_first_letter('viewUid')] = request.view_uid  # noqa: E501
+        if request.row_uid is not None:
+            path_params[self.__downcase_first_letter('rowUid')] = request.row_uid  # noqa: E501
+
+        query_params = []
+        if '{' + self.__downcase_first_letter('field') + '}' in path:
+            path = path.replace('{' + self.__downcase_first_letter('field' + '}'), request.field if request.field is not None else '')
+        else:
+            if request.field is not None:
+                query_params.append((self.__downcase_first_letter('field'), request.field))  # noqa: E501
+        if '{' + self.__downcase_first_letter('storage') + '}' in path:
+            path = path.replace('{' + self.__downcase_first_letter('storage' + '}'), request.storage if request.storage is not None else '')
+        else:
+            if request.storage is not None:
+                query_params.append((self.__downcase_first_letter('storage'), request.storage))  # noqa: E501
+        if '{' + self.__downcase_first_letter('folder') + '}' in path:
+            path = path.replace('{' + self.__downcase_first_letter('folder' + '}'), request.folder if request.folder is not None else '')
+        else:
+            if request.folder is not None:
+                query_params.append((self.__downcase_first_letter('folder'), request.folder))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = []
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            path, 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='TableTextStyleResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_views(self, request, **kwargs):  # noqa: E501
+        """Read all project views.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+
+        :param is_async bool
+        :param name str : The name of the file. (required)
+        :param storage str : The document storage.
+        :param folder str : The document folder.
+        :return: ViewsResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        try:
+            if kwargs.get('is_async'):
+                return self.get_views_with_http_info(request, **kwargs)  # noqa: E501
+            (data) = self.get_views_with_http_info(request, **kwargs)  # noqa: E501
+            return data
+        except ApiException as e:
+            if e.status == 401:
+                self.__request_token()
+                if kwargs.get('is_async'):
+                    return self.get_views_with_http_info(request, **kwargs)  # noqa: E501
+            (data) = self.get_views_with_http_info(request, **kwargs)  # noqa: E501
+            return data
+        
+    def get_views_with_http_info(self, request, **kwargs):  # noqa: E501
+        """Read all project views.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+
+        :param is_async bool
+        :param request get_views_request object with parameters
+        :return: ViewsResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        params = locals()
+        params['is_async'] = ''
+        params['_return_http_data_only'] = False
+        params['_preload_content'] = True
+        params['_request_timeout'] = ''
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_views" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if request.name is None:
+            raise ValueError("Missing the required parameter `name` when calling `get_views`")  # noqa: E501
+
+        collection_formats = {}
+        path = '/tasks/{name}/views'
+        path_params = {}
+        if request.name is not None:
+            path_params[self.__downcase_first_letter('name')] = request.name  # noqa: E501
+
+        query_params = []
+        if '{' + self.__downcase_first_letter('storage') + '}' in path:
+            path = path.replace('{' + self.__downcase_first_letter('storage' + '}'), request.storage if request.storage is not None else '')
+        else:
+            if request.storage is not None:
+                query_params.append((self.__downcase_first_letter('storage'), request.storage))  # noqa: E501
+        if '{' + self.__downcase_first_letter('folder') + '}' in path:
+            path = path.replace('{' + self.__downcase_first_letter('folder' + '}'), request.folder if request.folder is not None else '')
+        else:
+            if request.folder is not None:
+                query_params.append((self.__downcase_first_letter('folder'), request.folder))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = []
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            path, 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='ViewsResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def update_table_text_style(self, request, **kwargs):  # noqa: E501
+        """Update table text style in specified view.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+
+        :param is_async bool
+        :param name str : The name of the file. (required)
+        :param view_uid int : Uid of the view. (required)
+        :param table_text_style TableTextStyle : A DTO of TableTextStyle to update (required)
+        :param file_name str : File name to save changes to.
+        :param storage str : The document storage.
+        :param folder str : The document folder.
+        :return: AsposeResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        try:
+            if kwargs.get('is_async'):
+                return self.update_table_text_style_with_http_info(request, **kwargs)  # noqa: E501
+            (data) = self.update_table_text_style_with_http_info(request, **kwargs)  # noqa: E501
+            return data
+        except ApiException as e:
+            if e.status == 401:
+                self.__request_token()
+                if kwargs.get('is_async'):
+                    return self.update_table_text_style_with_http_info(request, **kwargs)  # noqa: E501
+            (data) = self.update_table_text_style_with_http_info(request, **kwargs)  # noqa: E501
+            return data
+        
+    def update_table_text_style_with_http_info(self, request, **kwargs):  # noqa: E501
+        """Update table text style in specified view.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+
+        :param is_async bool
+        :param request update_table_text_style_request object with parameters
+        :return: AsposeResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        params = locals()
+        params['is_async'] = ''
+        params['_return_http_data_only'] = False
+        params['_preload_content'] = True
+        params['_request_timeout'] = ''
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method update_table_text_style" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if request.name is None:
+            raise ValueError("Missing the required parameter `name` when calling `update_table_text_style`")  # noqa: E501
+        # verify the required parameter 'view_uid' is set
+        if request.view_uid is None:
+            raise ValueError("Missing the required parameter `view_uid` when calling `update_table_text_style`")  # noqa: E501
+        # verify the required parameter 'table_text_style' is set
+        if request.table_text_style is None:
+            raise ValueError("Missing the required parameter `table_text_style` when calling `update_table_text_style`")  # noqa: E501
+
+        collection_formats = {}
+        path = '/tasks/{name}/views/{viewUid}/tabletextstyles'
+        path_params = {}
+        if request.name is not None:
+            path_params[self.__downcase_first_letter('name')] = request.name  # noqa: E501
+        if request.view_uid is not None:
+            path_params[self.__downcase_first_letter('viewUid')] = request.view_uid  # noqa: E501
+
+        query_params = []
+        if '{' + self.__downcase_first_letter('fileName') + '}' in path:
+            path = path.replace('{' + self.__downcase_first_letter('fileName' + '}'), request.file_name if request.file_name is not None else '')
+        else:
+            if request.file_name is not None:
+                query_params.append((self.__downcase_first_letter('fileName'), request.file_name))  # noqa: E501
+        if '{' + self.__downcase_first_letter('storage') + '}' in path:
+            path = path.replace('{' + self.__downcase_first_letter('storage' + '}'), request.storage if request.storage is not None else '')
+        else:
+            if request.storage is not None:
+                query_params.append((self.__downcase_first_letter('storage'), request.storage))  # noqa: E501
+        if '{' + self.__downcase_first_letter('folder') + '}' in path:
+            path = path.replace('{' + self.__downcase_first_letter('folder' + '}'), request.folder if request.folder is not None else '')
+        else:
+            if request.folder is not None:
+                query_params.append((self.__downcase_first_letter('folder'), request.folder))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = []
+
+        body_params = None
+        if request.table_text_style is not None:
+            body_params = request.table_text_style
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            path, 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='AsposeResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
 
     def get_wbs_definition(self, request, **kwargs):  # noqa: E501
         """Get a project&#39;s WBS Definition.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass is_async=True
```

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/api_client.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,20 +73,20 @@
                  cookie=None):
         if configuration is None:
             configuration = Configuration()
         self.configuration = configuration
 
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
-        self.default_headers = {'x-aspose-client': 'python sdk', 'x-aspose-version': '22.7'}
+        self.default_headers = {'x-aspose-client': 'python sdk', 'x-aspose-version': '24.4'}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'python sdk 22.7'
+        self.user_agent = 'python sdk 24.4'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/configuration.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,9 +260,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.0\n"\
-               "SDK Package Version: 22.7.0".\
+               "SDK Package Version: 24.4.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/__init__.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 
 # flake8: noqa
 from __future__ import absolute_import
 
 # import models into model package
 from asposetaskscloud.models.aspose_response import AsposeResponse
 from asposetaskscloud.models.assignment_item import AssignmentItem
+from asposetaskscloud.models.background_pattern import BackgroundPattern
 from asposetaskscloud.models.baseline import Baseline
 from asposetaskscloud.models.baseline_type import BaselineType
 from asposetaskscloud.models.booking_type import BookingType
 from asposetaskscloud.models.calculation_mode import CalculationMode
 from asposetaskscloud.models.calculation_type import CalculationType
 from asposetaskscloud.models.calendar import Calendar
 from asposetaskscloud.models.calendar_exception import CalendarException
 from asposetaskscloud.models.calendar_exception_type import CalendarExceptionType
 from asposetaskscloud.models.calendar_item import CalendarItem
+from asposetaskscloud.models.colors import Colors
 from asposetaskscloud.models.confidence_level import ConfidenceLevel
 from asposetaskscloud.models.constraint_type import ConstraintType
 from asposetaskscloud.models.cost_accrual_type import CostAccrualType
 from asposetaskscloud.models.custom_field_type import CustomFieldType
 from asposetaskscloud.models.day_of_week import DayOfWeek
 from asposetaskscloud.models.day_type import DayType
 from asposetaskscloud.models.disc_usage import DiscUsage
@@ -26,18 +28,20 @@
 from asposetaskscloud.models.earned_value_method_type import EarnedValueMethodType
 from asposetaskscloud.models.element_type import ElementType
 from asposetaskscloud.models.error import Error
 from asposetaskscloud.models.error_details import ErrorDetails
 from asposetaskscloud.models.extended_attribute import ExtendedAttribute
 from asposetaskscloud.models.extended_attribute_definition import ExtendedAttributeDefinition
 from asposetaskscloud.models.extended_attribute_item import ExtendedAttributeItem
+from asposetaskscloud.models.field import Field
 from asposetaskscloud.models.file_versions import FileVersions
 from asposetaskscloud.models.files_list import FilesList
 from asposetaskscloud.models.files_upload_result import FilesUploadResult
 from asposetaskscloud.models.imported_project_type import ImportedProjectType
+from asposetaskscloud.models.item_type import ItemType
 from asposetaskscloud.models.link import Link
 from asposetaskscloud.models.link_element import LinkElement
 from asposetaskscloud.models.mask_type import MaskType
 from asposetaskscloud.models.month import Month
 from asposetaskscloud.models.month_item_type import MonthItemType
 from asposetaskscloud.models.month_position import MonthPosition
 from asposetaskscloud.models.object_exist import ObjectExist
@@ -46,14 +50,15 @@
 from asposetaskscloud.models.outline_code_definition import OutlineCodeDefinition
 from asposetaskscloud.models.outline_code_item import OutlineCodeItem
 from asposetaskscloud.models.outline_mask import OutlineMask
 from asposetaskscloud.models.outline_value import OutlineValue
 from asposetaskscloud.models.outline_value_type import OutlineValueType
 from asposetaskscloud.models.page_size import PageSize
 from asposetaskscloud.models.presentation_format import PresentationFormat
+from asposetaskscloud.models.primavera_task_properties import PrimaveraTaskProperties
 from asposetaskscloud.models.probability_distribution_type import ProbabilityDistributionType
 from asposetaskscloud.models.project_database_type import ProjectDatabaseType
 from asposetaskscloud.models.project_file_format import ProjectFileFormat
 from asposetaskscloud.models.project_info import ProjectInfo
 from asposetaskscloud.models.project_recalculation_result import ProjectRecalculationResult
 from asposetaskscloud.models.project_server_save_options_dto import ProjectServerSaveOptionsDTO
 from asposetaskscloud.models.project_validation_state import ProjectValidationState
@@ -67,29 +72,33 @@
 from asposetaskscloud.models.resource_assignment import ResourceAssignment
 from asposetaskscloud.models.resource_item import ResourceItem
 from asposetaskscloud.models.resource_type import ResourceType
 from asposetaskscloud.models.rollup_type import RollupType
 from asposetaskscloud.models.storage_exist import StorageExist
 from asposetaskscloud.models.storage_file import StorageFile
 from asposetaskscloud.models.summary_rows_calculation_type import SummaryRowsCalculationType
+from asposetaskscloud.models.table_text_style import TableTextStyle
 from asposetaskscloud.models.task import Task
 from asposetaskscloud.models.task_creation_request import TaskCreationRequest
 from asposetaskscloud.models.task_item import TaskItem
 from asposetaskscloud.models.task_link import TaskLink
 from asposetaskscloud.models.task_link_type import TaskLinkType
 from asposetaskscloud.models.task_type import TaskType
+from asposetaskscloud.models.text_item_type import TextItemType
 from asposetaskscloud.models.time_unit_type import TimeUnitType
 from asposetaskscloud.models.timephased_data import TimephasedData
 from asposetaskscloud.models.timephased_data_type import TimephasedDataType
 from asposetaskscloud.models.timescale import Timescale
 from asposetaskscloud.models.value import Value
 from asposetaskscloud.models.vba_module import VbaModule
 from asposetaskscloud.models.vba_module_attribute import VbaModuleAttribute
 from asposetaskscloud.models.vba_project import VbaProject
 from asposetaskscloud.models.vba_reference import VbaReference
+from asposetaskscloud.models.view import View
+from asposetaskscloud.models.view_screen import ViewScreen
 from asposetaskscloud.models.wbs_code_mask import WBSCodeMask
 from asposetaskscloud.models.wbs_definition import WBSDefinition
 from asposetaskscloud.models.wbs_sequence import WBSSequence
 from asposetaskscloud.models.week_day import WeekDay
 from asposetaskscloud.models.week_day_type import WeekDayType
 from asposetaskscloud.models.work_contour_type import WorkContourType
 from asposetaskscloud.models.work_group_type import WorkGroupType
@@ -116,27 +125,31 @@
 from asposetaskscloud.models.extended_attribute_items_response import ExtendedAttributeItemsResponse
 from asposetaskscloud.models.extended_attribute_response import ExtendedAttributeResponse
 from asposetaskscloud.models.file_version import FileVersion
 from asposetaskscloud.models.outline_code_items import OutlineCodeItems
 from asposetaskscloud.models.outline_code_items_response import OutlineCodeItemsResponse
 from asposetaskscloud.models.outline_code_response import OutlineCodeResponse
 from asposetaskscloud.models.page_count_response import PageCountResponse
+from asposetaskscloud.models.primavera_task_properties_response import PrimaveraTaskPropertiesResponse
 from asposetaskscloud.models.project_ids_response import ProjectIdsResponse
 from asposetaskscloud.models.project_list import ProjectList
 from asposetaskscloud.models.project_list_response import ProjectListResponse
 from asposetaskscloud.models.project_recalculate_response import ProjectRecalculateResponse
 from asposetaskscloud.models.recurring_info_response import RecurringInfoResponse
 from asposetaskscloud.models.resource_assignments import ResourceAssignments
 from asposetaskscloud.models.resource_item_response import ResourceItemResponse
 from asposetaskscloud.models.resource_items import ResourceItems
 from asposetaskscloud.models.resource_items_response import ResourceItemsResponse
 from asposetaskscloud.models.resource_response import ResourceResponse
+from asposetaskscloud.models.table_text_style_response import TableTextStyleResponse
+from asposetaskscloud.models.table_text_styles_response import TableTextStylesResponse
 from asposetaskscloud.models.task_baseline import TaskBaseline
 from asposetaskscloud.models.task_item_response import TaskItemResponse
 from asposetaskscloud.models.task_items import TaskItems
 from asposetaskscloud.models.task_items_response import TaskItemsResponse
 from asposetaskscloud.models.task_link_response import TaskLinkResponse
 from asposetaskscloud.models.task_links_response import TaskLinksResponse
 from asposetaskscloud.models.task_response import TaskResponse
 from asposetaskscloud.models.timephased_data_response import TimephasedDataResponse
 from asposetaskscloud.models.vba_project_response import VbaProjectResponse
+from asposetaskscloud.models.views_response import ViewsResponse
 from asposetaskscloud.models.wbs_definition_response import WBSDefinitionResponse
```

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/aspose_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/aspose_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,18 @@
         'TaskLinkResponse': 'TaskLinkResponse',
         'ExtendedAttributeResponse': 'ExtendedAttributeResponse',
         'TimephasedDataResponse': 'TimephasedDataResponse',
         'ExtendedAttributeItemsResponse': 'ExtendedAttributeItemsResponse',
         'PageCountResponse': 'PageCountResponse',
         'TaskResponse': 'TaskResponse',
         'RecurringInfoResponse': 'RecurringInfoResponse',
+        'ViewsResponse': 'ViewsResponse',
         'ExtendedAttributeItemResponse': 'ExtendedAttributeItemResponse',
         'AssignmentResponse': 'AssignmentResponse',
+        'PrimaveraTaskPropertiesResponse': 'PrimaveraTaskPropertiesResponse',
         'CalendarItemsResponse': 'CalendarItemsResponse',
         'OutlineCodeItemsResponse': 'OutlineCodeItemsResponse',
         'ResourceResponse': 'ResourceResponse',
         'OutlineCodeResponse': 'OutlineCodeResponse',
         'TaskLinksResponse': 'TaskLinksResponse',
         'AssignmentItemResponse': 'AssignmentItemResponse',
         'WBSDefinitionResponse': 'WBSDefinitionResponse',
@@ -74,14 +76,16 @@
         'CalendarWorkWeeksResponse': 'CalendarWorkWeeksResponse',
         'TaskItemsResponse': 'TaskItemsResponse',
         'VbaProjectResponse': 'VbaProjectResponse',
         'ProjectRecalculateResponse': 'ProjectRecalculateResponse',
         'CalendarResponse': 'CalendarResponse',
         'DocumentPropertyResponse': 'DocumentPropertyResponse',
         'ResourceItemsResponse': 'ResourceItemsResponse',
+        'TableTextStyleResponse': 'TableTextStyleResponse',
+        'TableTextStylesResponse': 'TableTextStylesResponse',
         'AssignmentsResponse': 'AssignmentsResponse',
         'CalendarItemResponse': 'CalendarItemResponse',
         'ResourceItemResponse': 'ResourceItemResponse',
         'DocumentPropertiesResponse': 'DocumentPropertiesResponse',
         'TaskItemResponse': 'TaskItemResponse'
     }
```

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/assignment_baseline.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/assignment_baseline.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/assignment_item.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/assignment_item.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/assignment_item_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/assignment_item_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/assignment_items.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/assignment_items.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/assignment_items_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/assignment_items_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/assignment_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/assignment_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/assignments_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/assignments_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/baseline.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/baseline.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/baseline_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/baseline_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/booking_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/booking_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calculation_mode.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calculation_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calculation_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calculation_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calendar.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calendar.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calendar_exception.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calendar_exception.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calendar_exception_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calendar_exception_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calendar_exceptions_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calendar_exceptions_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calendar_item.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calendar_item.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calendar_item_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calendar_item_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calendar_items.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calendar_items.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calendar_items_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calendar_items_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calendar_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calendar_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/calendar_work_weeks_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/calendar_work_weeks_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/confidence_level.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/confidence_level.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/constraint_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/constraint_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/cost_accrual_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/cost_accrual_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/custom_field_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/custom_field_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/day_of_week.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/day_of_week.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/day_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/day_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/disc_usage.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/disc_usage.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/document_properties.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/document_properties.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/document_properties_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/document_properties_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/document_property.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/document_property.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/document_property_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/document_property_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/duration.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/duration.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/earned_value_method_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/earned_value_method_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/element_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/element_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/error.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/error.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/error_details.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/extended_attribute.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/extended_attribute.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/extended_attribute_definition.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/extended_attribute_definition.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/extended_attribute_item.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/extended_attribute_item.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/extended_attribute_item_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/extended_attribute_item_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/extended_attribute_items.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/extended_attribute_items.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/extended_attribute_items_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/extended_attribute_items_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/extended_attribute_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/extended_attribute_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/file_version.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/file_version.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/file_versions.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/file_versions.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/files_list.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/files_upload_result.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/imported_project_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/imported_project_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/link.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/link.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/link_element.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/link_element.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/mask_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/mask_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/month.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/month.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/month_item_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/month_item_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/month_position.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/month_position.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/object_exist.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/object_exist.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/ordinal_number.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/ordinal_number.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/outline_code.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/outline_code.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/outline_code_definition.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/outline_code_definition.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/outline_code_item.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/outline_code_item.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/outline_code_items.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/outline_code_items.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/outline_code_items_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/outline_code_items_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/outline_code_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/outline_code_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/outline_mask.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/outline_mask.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/outline_value.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/outline_value.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/outline_value_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/outline_value_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/page_count_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/page_count_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/page_size.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/page_size.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/presentation_format.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/presentation_format.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/probability_distribution_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/probability_distribution_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/project_database_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/project_database_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/project_file_format.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/project_file_format.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/project_ids_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/project_ids_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,26 +57,26 @@
         if project_ids is not None:
             self.project_ids = project_ids
 
     @property
     def project_ids(self):
         """Gets the project_ids of this ProjectIdsResponse.  # noqa: E501
 
-        UIds of the projects  # noqa: E501
+        UIds of the project  # noqa: E501
 
         :return: The project_ids of this ProjectIdsResponse.  # noqa: E501
         :rtype: list[str]
         """
         return self._project_ids
 
     @project_ids.setter
     def project_ids(self, project_ids):
         """Sets the project_ids of this ProjectIdsResponse.
 
-        UIds of the projects  # noqa: E501
+        UIds of the project  # noqa: E501
 
         :param project_ids: The project_ids of this ProjectIdsResponse.  # noqa: E501
         :type: list[str]
         """
         self._project_ids = project_ids
     def to_dict(self):
         """Returns the model properties as a dict"""
```

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/project_info.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/project_info.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/project_list.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/project_list.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/project_list_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/project_list_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/project_recalculate_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/project_recalculate_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/project_recalculation_result.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/project_recalculation_result.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/project_server_save_options_dto.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/project_server_save_options_dto.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/project_validation_state.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/project_validation_state.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/rate_format_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/rate_format_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/rate_scale_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/rate_scale_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/rate_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/rate_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/recurrence_pattern.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/recurrence_pattern.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/recurring_info.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/recurring_info.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/recurring_info_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/recurring_info_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/report_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/report_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/__init__.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 from asposetaskscloud.models.requests.get_resource_assignments_request import GetResourceAssignmentsRequest
 from asposetaskscloud.models.requests.get_resource_timephased_data_request import GetResourceTimephasedDataRequest
 from asposetaskscloud.models.requests.get_resources_request import GetResourcesRequest
 from asposetaskscloud.models.requests.post_resource_request import PostResourceRequest
 from asposetaskscloud.models.requests.put_resource_request import PutResourceRequest
 from asposetaskscloud.models.requests.get_risk_analysis_report_request import GetRiskAnalysisReportRequest
 from asposetaskscloud.models.requests.delete_task_request import DeleteTaskRequest
+from asposetaskscloud.models.requests.get_primavera_task_properties_request import GetPrimaveraTaskPropertiesRequest
 from asposetaskscloud.models.requests.get_task_request import GetTaskRequest
 from asposetaskscloud.models.requests.get_task_assignments_request import GetTaskAssignmentsRequest
 from asposetaskscloud.models.requests.get_task_recurring_info_request import GetTaskRecurringInfoRequest
 from asposetaskscloud.models.requests.get_task_timephased_data_request import GetTaskTimephasedDataRequest
 from asposetaskscloud.models.requests.get_tasks_request import GetTasksRequest
 from asposetaskscloud.models.requests.post_task_request import PostTaskRequest
 from asposetaskscloud.models.requests.post_task_recurring_info_request import PostTaskRecurringInfoRequest
@@ -82,10 +83,16 @@
 from asposetaskscloud.models.requests.put_task_request import PutTaskRequest
 from asposetaskscloud.models.requests.put_task_recurring_info_request import PutTaskRecurringInfoRequest
 from asposetaskscloud.models.requests.delete_task_link_request import DeleteTaskLinkRequest
 from asposetaskscloud.models.requests.get_task_links_request import GetTaskLinksRequest
 from asposetaskscloud.models.requests.post_task_link_request import PostTaskLinkRequest
 from asposetaskscloud.models.requests.put_task_link_request import PutTaskLinkRequest
 from asposetaskscloud.models.requests.get_vba_project_request import GetVbaProjectRequest
+from asposetaskscloud.models.requests.create_table_text_style_request import CreateTableTextStyleRequest
+from asposetaskscloud.models.requests.delete_table_text_style_request import DeleteTableTextStyleRequest
+from asposetaskscloud.models.requests.get_all_table_text_styles_request import GetAllTableTextStylesRequest
+from asposetaskscloud.models.requests.get_table_text_style_request import GetTableTextStyleRequest
+from asposetaskscloud.models.requests.get_views_request import GetViewsRequest
+from asposetaskscloud.models.requests.update_table_text_style_request import UpdateTableTextStyleRequest
 from asposetaskscloud.models.requests.get_wbs_definition_request import GetWbsDefinitionRequest
 from asposetaskscloud.models.requests.put_renumber_wbs_code_request import PutRenumberWbsCodeRequest
 from asposetaskscloud.models.requests.post_task_document_with_format_request import PostTaskDocumentWithFormatRequest
```

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/copy_file_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/copy_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/copy_folder_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/copy_folder_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/create_folder_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/create_folder_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/create_new_project_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/create_new_project_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/delete_assignment_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_assignment_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/delete_calendar_exception_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_calendar_exception_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/delete_calendar_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_calendar_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/delete_extended_attribute_by_index_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_extended_attribute_by_index_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/delete_file_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/delete_folder_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_folder_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/delete_outline_code_by_index_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_outline_code_by_index_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/delete_resource_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_resource_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/delete_task_link_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_task_link_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/delete_task_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/delete_task_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/download_file_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/download_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_assignment_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_assignment_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_assignment_timephased_data_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_assignment_timephased_data_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_assignments_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_assignments_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_calendar_exceptions_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_calendar_exceptions_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_calendar_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_calendar_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_calendar_work_weeks_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_calendar_work_weeks_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_calendars_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_calendars_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_critical_path_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_critical_path_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_disc_usage_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_disc_usage_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_document_properties_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_document_properties_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_document_property_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_document_property_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_extended_attribute_by_index_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_extended_attribute_by_index_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_extended_attributes_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_extended_attributes_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_file_versions_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_file_versions_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_files_list_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_files_list_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_outline_code_by_index_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_outline_code_by_index_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_outline_codes_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_outline_codes_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_page_count_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_page_count_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_project_ids_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_project_ids_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_project_list_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_project_list_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_report_pdf_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_report_pdf_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_resource_assignments_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_resource_assignments_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_resource_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_resource_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_resource_timephased_data_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_resource_timephased_data_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_resources_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_resources_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_risk_analysis_report_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_risk_analysis_report_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_task_assignments_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_task_assignments_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_task_document_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_task_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_task_document_with_format_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_task_document_with_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_task_links_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_task_links_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_task_recurring_info_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_task_recurring_info_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_task_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_task_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_task_timephased_data_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_task_timephased_data_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_tasks_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_tasks_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_vba_project_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_vba_project_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/get_wbs_definition_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/get_wbs_definition_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/move_file_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/move_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/move_folder_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/move_folder_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/object_exists_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/object_exists_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/post_assignment_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/post_assignment_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/post_calendar_exception_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/post_calendar_exception_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/post_calendar_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/post_calendar_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/post_document_property_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/post_document_property_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/post_resource_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/post_resource_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/post_task_document_with_format_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/post_task_document_with_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/post_task_link_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/post_task_link_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/post_task_recurring_info_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/post_task_recurring_info_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/post_task_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/post_task_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/post_tasks_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/post_tasks_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_assignment_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_assignment_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_calendar_exception_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_calendar_exception_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_calendar_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_calendar_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_document_property_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_document_property_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_extended_attribute_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_extended_attribute_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_import_project_from_db_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_import_project_from_db_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_import_project_from_file_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_import_project_from_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_import_project_from_project_online_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_import_project_from_project_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_move_task_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_move_task_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_move_task_to_sibling_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_move_task_to_sibling_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_recalculate_project_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_recalculate_project_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_recalculate_project_resource_fields_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_recalculate_project_resource_fields_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_recalculate_project_uncomplete_work_to_start_after_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_recalculate_project_uncomplete_work_to_start_after_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_recalculate_project_work_as_complete_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_recalculate_project_work_as_complete_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_renumber_wbs_code_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_renumber_wbs_code_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_resource_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_resource_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_task_link_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_task_link_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_task_recurring_info_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_task_recurring_info_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/put_task_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/put_task_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/storage_exists_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/storage_exists_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/update_project_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/update_project_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/requests/upload_file_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/requests/upload_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/resource.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/resource.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/resource_assignment.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/resource_assignment.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/resource_assignments.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/resource_assignments.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/resource_item.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/resource_item.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/resource_item_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/resource_item_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/resource_items.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/resource_items.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/resource_items_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/resource_items_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/resource_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/resource_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/resource_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/resource_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/rollup_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/rollup_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/storage_exist.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/storage_exist.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/storage_file.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/summary_rows_calculation_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/summary_rows_calculation_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_baseline.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_baseline.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_creation_request.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_creation_request.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_item.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_item.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_item_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_item_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_items.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_items.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_items_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_items_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_link.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_link.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_link_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_link_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_link_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_link_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_links_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_links_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/task_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/task_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/time_unit_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/time_unit_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/timephased_data.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/timephased_data.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/timephased_data_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/timephased_data_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/timephased_data_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/timephased_data_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/timescale.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/timescale.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/value.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/value.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/vba_module.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/vba_module.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/vba_module_attribute.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/vba_module_attribute.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/vba_project.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/vba_project.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/vba_project_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/vba_project_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/vba_reference.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/vba_reference.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/wbs_code_mask.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/wbs_code_mask.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/wbs_definition.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/wbs_definition.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/wbs_definition_response.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/wbs_definition_response.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/wbs_sequence.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/wbs_sequence.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/week_day.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/week_day.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/week_day_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/week_day_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/work_contour_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/work_contour_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/work_group_type.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/work_group_type.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/work_week.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/work_week.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/models/working_time.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/models/working_time.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/asposetaskscloud/rest.py` & `aspose_tasks_cloud-24.4.0/asposetaskscloud/rest.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/setup.py` & `aspose_tasks_cloud-24.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "aspose-tasks-cloud"
-VERSION = "22.7.0"
+VERSION = "24.4.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `aspose-tasks-cloud-22.7.0/test/__init__.py` & `aspose_tasks_cloud-24.4.0/test/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,10 +17,12 @@
 from test.test_report import TestReport
 from test.test_resources import TestResources
 from test.test_storage import TestStorage
 from test.test_task_document_format import TestTaskDocumentFormat
 from test.test_task_links import TestTaskLinks
 from test.test_tasks import TestTasks
 from test.test_tasks_extended_attributes import TestTasksExtendedAttributes
+from test.test_tasks_primavera_properties import TestTasksPrimaveraProperties
 from test.test_timephased_data import TestTimephasedData
 from test.test_vba import TestVba
+from test.test_views import TestViews
 from test.test_wbs import TestWbs
```

### Comparing `aspose-tasks-cloud-22.7.0/test/base_test_context.py` & `aspose_tasks_cloud-24.4.0/test/base_test_context.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_api_coverage.py` & `aspose_tasks_cloud-24.4.0/test/test_api_coverage.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,16 @@
 
     def test_api_coverage(self):
         arr = [test.TestAssignments, test.TestCalendarExceptions, test.TestCalendarWorkWeeks, test.TestCalendars,
                test.TestDocumentProperties, test.TestExtendedAttributes, test.TestFile, test.TestFolder,
                test.TestGetPageCount, test.TestImportProject, test.TestOutlineCodes, test.TestProjectOnline,
                test.TestReadProject, test.TestRecalculation, test.TestRecurringInfo, test.TestReport,
                test.TestResources, test.TestStorage, test.TestTaskDocumentFormat, test.TestTaskLinks, test.TestTasks,
-               test.TestTasksExtendedAttributes, test.TestTimephasedData, test.TestVba, test.TestWbs]
+               test.TestTasksExtendedAttributes, test.TestTasksPrimaveraProperties, test.TestTimephasedData,
+               test.TestVba, test.TestViews, test.TestWbs]
         test_methods = []
         uncovered_methods = ''
         for ar in arr:
             test_methods += list(filter(lambda x: not (x.startswith('__') and x.endswith('__')) and x != 'test_folder',
                                         ar.__dict__.keys()))
         api_methods = list(filter(lambda x: not (x.startswith('__') and x.endswith('__'))
                                             and not x.endswith('with_http_info')
```

### Comparing `aspose-tasks-cloud-22.7.0/test/test_assignments.py` & `aspose_tasks_cloud-24.4.0/test/test_assignments.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_calendar_exceptions.py` & `aspose_tasks_cloud-24.4.0/test/test_calendar_exceptions.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_calendar_work_weeks.py` & `aspose_tasks_cloud-24.4.0/test/test_calendar_work_weeks.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_calendars.py` & `aspose_tasks_cloud-24.4.0/test/test_calendars.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_document_properties.py` & `aspose_tasks_cloud-24.4.0/test/test_document_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         filename = 'Home_move_plan.mpp'
         self.upload_file(filename)
         request = GetDocumentPropertiesRequest(filename)
         result = self.tasks_api.get_document_properties(request)
         self.assertIsNotNone(result)
         self.assertIsInstance(result, DocumentPropertiesResponse)
         self.assertIsNotNone(result.properties)
-        self.assertEqual(52, len(result.properties.list))
+        self.assertEqual(63, len(result.properties.list))
         self.assertEqual('Title', result.properties.list[0].name)
         self.assertEqual('Home Move', result.properties.list[0].value)
 
     def test_get_document_property(self):
         filename = 'Home_move_plan.mpp'
         self.upload_file(filename)
         request = GetDocumentPropertyRequest(filename, 'Title')
```

### Comparing `aspose-tasks-cloud-22.7.0/test/test_extended_attributes.py` & `aspose_tasks_cloud-24.4.0/test/test_extended_attributes.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_file.py` & `aspose_tasks_cloud-24.4.0/test/test_file.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_folder.py` & `aspose_tasks_cloud-24.4.0/test/test_folder.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_get_page_count.py` & `aspose_tasks_cloud-24.4.0/test/test_get_page_count.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_import_project.py` & `aspose_tasks_cloud-24.4.0/test/test_import_project.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_outline_codes.py` & `aspose_tasks_cloud-24.4.0/test/test_outline_codes.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_project_online.py` & `aspose_tasks_cloud-24.4.0/test/test_project_online.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_read_project.py` & `aspose_tasks_cloud-24.4.0/test/test_read_project.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_recalculation.py` & `aspose_tasks_cloud-24.4.0/test/test_recalculation.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_recurring_info.py` & `aspose_tasks_cloud-24.4.0/test/test_recurring_info.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_report.py` & `aspose_tasks_cloud-24.4.0/test/test_report.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_resources.py` & `aspose_tasks_cloud-24.4.0/test/test_resources.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_storage.py` & `aspose_tasks_cloud-24.4.0/test/test_storage.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_task_document_format.py` & `aspose_tasks_cloud-24.4.0/test/test_task_document_format.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_task_links.py` & `aspose_tasks_cloud-24.4.0/test/test_task_links.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_tasks.py` & `aspose_tasks_cloud-24.4.0/test/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_tasks_extended_attributes.py` & `aspose_tasks_cloud-24.4.0/test/test_tasks_extended_attributes.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_timephased_data.py` & `aspose_tasks_cloud-24.4.0/test/test_timephased_data.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_vba.py` & `aspose_tasks_cloud-24.4.0/test/test_vba.py`

 * *Files identical despite different names*

### Comparing `aspose-tasks-cloud-22.7.0/test/test_wbs.py` & `aspose_tasks_cloud-24.4.0/test/test_wbs.py`

 * *Files identical despite different names*

