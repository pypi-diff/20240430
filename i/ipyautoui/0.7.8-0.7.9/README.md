# Comparing `tmp/ipyautoui-0.7.8.tar.gz` & `tmp/ipyautoui-0.7.9.tar.gz`

## Comparing `ipyautoui-0.7.8.tar` & `ipyautoui-0.7.9.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/_dev_maplocal_params.py
--rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/_utils.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/_utils_debounce.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/_version.py
--rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/autoanyof.py
--rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/autobox.py
--rw-r--r--   0        0        0    32690 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/autodisplay.py
--rw-r--r--   0        0        0    14267 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/autodisplay_renderers.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/autoform.py
--rw-r--r--   0        0        0    42812 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/automapschema.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/automapschema.yaml
--rw-r--r--   0        0        0    19437 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/autoobject.py
--rw-r--r--   0        0        0    11476 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/autoui.py
--rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/autovjsf.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/basemodel.py
--rw-r--r--   0        0        0     6231 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/constants.py
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/env.py
--rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/mydocstring_display.py
--rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/nullable.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/vjsf.vue
--rw-r--r--   0        0        0     8036 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/watch_validate.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/__init__.py
--rw-r--r--   0        0        0    43828 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/autogrid.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/boolean_toggle.py
--rw-r--r--   0        0        0    13259 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/buttonbars.py
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/combobox_mapped.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/date_string.py
--rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/decision_branch.py
--rw-r--r--   0        0        0    27408 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/editgrid.py
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/filechooser.py
--rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/filesindir.py
--rw-r--r--   0        0        0    10822 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/fileupload.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/halo_decorator.py
--rw-r--r--   0        0        0    22826 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/iterable.py
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/loadproject.py
--rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/markdown_widget.py
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/modelrun.py
--rw-r--r--   0        0        0     7740 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/multi_toggle_buttons.py
--rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/multiselect_search.py
--rw-r--r--   0        0        0     7605 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/outputlogging.py
--rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/selectandclick.py
--rw-r--r--   0        0        0     9400 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/selectdir.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/showhide.py
--rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/showopenurl.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/title_description.py
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/urlimagelink.py
--rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/custom/widgetcaller_error.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/__init__.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/array_examples.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/array_object_dataframe.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/complex_serialization.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/core_ipywidgets.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/editable_datagrid.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/editable_datagrid_with_nullable.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/multiindex_editable_grid.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/nested.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/nested_editable_datagrid.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/null_and_required.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/override_ipywidgets.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/pydantic_validation.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/pydantic_validation_error.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/pydantic_validation_list.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/recursive_array.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/recursive_object.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/root_array.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/root_array_enum.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/root_enum.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/root_simple.py
--rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/src/ipyautoui/demo_schemas/ruleset.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/.gitignore
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/README.md
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/pyproject.toml
--rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 ipyautoui-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/_dev_maplocal_params.py
+-rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/_utils.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/_utils_debounce.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/_version.py
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/autoanyof.py
+-rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/autobox.py
+-rw-r--r--   0        0        0    32690 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/autodisplay.py
+-rw-r--r--   0        0        0    14267 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/autodisplay_renderers.py
+-rw-r--r--   0        0        0     9416 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/autoform.py
+-rw-r--r--   0        0        0    42812 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/automapschema.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/automapschema.yaml
+-rw-r--r--   0        0        0    19644 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/autoobject.py
+-rw-r--r--   0        0        0    11258 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/autoui.py
+-rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/autovjsf.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/basemodel.py
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/constants.py
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/env.py
+-rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/mydocstring_display.py
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/nullable.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/vjsf.vue
+-rw-r--r--   0        0        0     8036 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/watch_validate.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/__init__.py
+-rw-r--r--   0        0        0    43828 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/autogrid.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/boolean_toggle.py
+-rw-r--r--   0        0        0    13259 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/buttonbars.py
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/combobox_mapped.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/date_string.py
+-rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/decision_branch.py
+-rw-r--r--   0        0        0    27408 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/editgrid.py
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/filechooser.py
+-rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/filesindir.py
+-rw-r--r--   0        0        0    10822 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/fileupload.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/halo_decorator.py
+-rw-r--r--   0        0        0    22826 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/iterable.py
+-rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/loadproject.py
+-rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/markdown_widget.py
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/modelrun.py
+-rw-r--r--   0        0        0     7740 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/multi_toggle_buttons.py
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/multiselect_search.py
+-rw-r--r--   0        0        0     7605 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/outputlogging.py
+-rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/selectandclick.py
+-rw-r--r--   0        0        0     9400 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/selectdir.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/showhide.py
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/showopenurl.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/title_description.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/urlimagelink.py
+-rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/custom/widgetcaller_error.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/__init__.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/array_examples.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/array_object_dataframe.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/complex_serialization.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/core_ipywidgets.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/editable_datagrid.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/editable_datagrid_with_nullable.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/multiindex_editable_grid.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/nested.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/nested_editable_datagrid.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/null_and_required.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/override_ipywidgets.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/pydantic_validation.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/pydantic_validation_error.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/pydantic_validation_list.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/recursive_array.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/recursive_object.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/root_array.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/root_array_enum.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/root_enum.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/root_simple.py
+-rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/src/ipyautoui/demo_schemas/ruleset.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/.gitignore
+-rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/README.md
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 ipyautoui-0.7.9/PKG-INFO
```

### Comparing `ipyautoui-0.7.8/src/ipyautoui/__init__.py` & `ipyautoui-0.7.9/src/ipyautoui/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/_dev_maplocal_params.py` & `ipyautoui-0.7.9/src/ipyautoui/_dev_maplocal_params.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/_utils.py` & `ipyautoui-0.7.9/src/ipyautoui/_utils.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/_utils_debounce.py` & `ipyautoui-0.7.9/src/ipyautoui/_utils_debounce.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/autoanyof.py` & `ipyautoui-0.7.9/src/ipyautoui/autoanyof.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/autobox.py` & `ipyautoui-0.7.9/src/ipyautoui/autobox.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/autodisplay.py` & `ipyautoui-0.7.9/src/ipyautoui/autodisplay.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/autodisplay_renderers.py` & `ipyautoui-0.7.9/src/ipyautoui/autodisplay_renderers.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/autoform.py` & `ipyautoui-0.7.9/src/ipyautoui/autoform.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,29 @@
-# +
-
 """layout attributes of a form box
 """
 # %run _dev_maplocal_params.py
 # +
 import ipywidgets as w
 import traitlets as tr
 import typing as ty
 
 from IPython.display import display, clear_output
-from ipyautoui.constants import BUTTON_WIDTH_MIN
+from ipyautoui.nullable import Nullable
+from ipyautoui.constants import KWARGS_SHOWNULL, KWARGS_SHOWRAW, SHOWNULL_ICON_SHOW, SHOWNULL_ICON_HIDE
 from ipyautoui.custom.buttonbars import SaveButtonBar
 from ipyautoui.custom.title_description import TitleDescription
 from ipyautoui._utils import display_python_string, show_hide_widget
-from ipyautoui.nullable import Nullable
 
 def make_bold(s: str) -> str:
     return f"<big><b>{s}</b></big>"
 
 
 # -
-
-SHOWNULL_ICON_SHOW = "plus"
-SHOWNULL_ICON_HIDE = "minus"
-KWARGS_SHOWNULL = dict(
-            icon=SHOWNULL_ICON_SHOW,
-            layout=w.Layout(width=BUTTON_WIDTH_MIN, display=""),
-            tooltip="show null form fields",
-            style={"font_weight": "bold"})
-KWARGS_SHOWRAW = dict(icon="code",
-            layout=w.Layout(width=BUTTON_WIDTH_MIN, display="None"),
-            tooltip="show raw data",
-            style={"font_weight": "bold"},
-        )
-
-
 class ShowNull(tr.HasTraits):
-    display_bn_shownull = tr.Bool(default_value=True)
+    display_bn_shownull = tr.Bool(default_value=True)        
 
     @tr.observe("display_bn_shownull")
     def _observe_display_bn_shownull(self, change):
         show_hide_widget(self.bn_shownull, self.display_bn_shownull)
     
     def _init_bn_shownull(self):
         self.bn_shownull = w.ToggleButton(**KWARGS_SHOWNULL)
@@ -59,28 +42,21 @@
             self._init_bn_shownull()
         return self._bn_shownull
     
     @bn_shownull.setter
     def bn_shownull(self, value):
         self._bn_shownull = value
 
-    def show_hide_bn_nullable(self):  # work with AutoObject only
-        is_nullable = [True for v in self.di_widgets.values() if isinstance(v, Nullable)]
-        if len(is_nullable) > 0:
-            if self.display_bn_shownull:
-                show_hide_widget(self.bn_shownull, self.display_bn_shownull)
-                # NOTE: don't think should be required but it appeared to be saving the 
-                #       state of the button.layout.display between objects otherwise ... 
-                #       ... not sure... but this seems to fix it
-            else:
-                self.display_bn_shownull = True
+    def show_hide_bn_nullable(self):
+        """Set display of show null button based on if any nullable widgets are found."""
+        if self.check_for_nullables():  # check_for_nullables is defined in AutoObject
+            self.display_bn_shownull = True
         else:
             self.display_bn_shownull = False
-
-
+    
 
 if __name__ == "__main__":
     sn = ShowNull()
     display(sn.bn_shownull)
 
 
 # +
@@ -243,19 +219,14 @@
 
 if __name__ == "__main__":
     ui = AutoObjectFormLayout(show_savebuttonbar=True)  # description="description", 
     display(ui)
 
 
 # +
-
-
-
-
-
 def demo_autoobject_form(title="test", description="a description of the title"):
     """for docs and testing only..."""
     from ipyautoui.custom.buttonbars import SaveButtonBar
     li = [AutoObjectFormLayout, TitleDescription, w.VBox, ShowNull]
     class TestForm(*li):
         def __init__(self, **kwargs):
             self.vbx_error = w.VBox()
```

### Comparing `ipyautoui-0.7.8/src/ipyautoui/automapschema.py` & `ipyautoui-0.7.9/src/ipyautoui/automapschema.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/automapschema.yaml` & `ipyautoui-0.7.9/src/ipyautoui/automapschema.yaml`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/autoobject.py` & `ipyautoui-0.7.9/src/ipyautoui/autoobject.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,31 +17,26 @@
 """AutoObject - create a 
 """
 # %run _dev_maplocal_params.py
 # %load_ext lab_black
 
 import logging
 import pathlib
-import functools
 import ipywidgets as w
-from IPython.display import display
+import pandas as pd  # TODO: pandas is a heavy dep. if only used for pd.isnull... ? 
 import traitlets as tr
-import typing as ty
-import json
+from IPython.display import display
+from jsonref import replace_refs
 import ipyautoui.automapschema as aumap
 from ipyautoui._utils import obj_from_importstr
 from ipyautoui.nullable import Nullable
 from ipyautoui.autobox import AutoBox
 from ipyautoui.autoform import AutoObjectFormLayout
-from jsonref import replace_refs
-from pydantic import BaseModel
 from ipyautoui.watch_validate import WatchValidate
 from ipyautoui.custom.title_description import TitleDescription
-import contextlib
-import pandas as pd  # TODO: pandas is a heavy dep. if only used for pd.isnull... ? 
 
 logger = logging.getLogger(__name__)
 
 
 # -
 def _get_value_trait(obj_with_traits):
     """gets the trait type for a given object (looks for "_value" and
@@ -434,29 +429,37 @@
         return self.di_widgets_value
 
     @property
     def di_widgets_value(self):  # used to set _value
         get_value = lambda v: v._value if "_value" in v.traits() else v.value
         return {k: get_value(v) for k, v in self.di_widgets.items()}
 
+    def check_for_nullables(self) -> bool:
+        """Search through widgets and as soon as a Nullable widget is found, return True.
+        Else, return False."""
+        for v in self.di_widgets.values():
+            if isinstance(v, Nullable):
+                return True
+        return False
+
 
 class AutoObjectForm(AutoObject, AutoObjectFormLayout):
     def __init__(self, **kwargs):
         super().__init__(
             **kwargs,
         )
         self.children = [
             w.HBox([self.bn_shownull, self.savebuttonbar ]),
             self.html_title,
             self.html_description,
             self.vbx_widget,
             self.vbx_showraw,
         ]
         self.show_hide_bn_nullable()
-
+        
     def display_ui(self):  # NOTE: this overwritten this in AutoObjectForm
         self.vbx_widget.layout.display = ""
 
     def display_showraw(self):  # NOTE: this overwritten this in AutoObjectForm
         self.vbx_widget.layout.display = "None"
         return self.json
```

### Comparing `ipyautoui-0.7.8/src/ipyautoui/autoui.py` & `ipyautoui-0.7.9/src/ipyautoui/autoui.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,45 +27,33 @@
         from ipyautoui.constants import DISPLAY_AUTOUI_SCHEMA_EXAMPLE
         DISPLAY_AUTOUI_SCHEMA_EXAMPLE()
 """
 # %run _dev_maplocal_params.py
 # %load_ext lab_black
 
 import pathlib
-from IPython.display import display
-from pydantic import BaseModel, ValidationError
 import json
+import logging
+import functools
 import traitlets as tr
 import typing as ty
-from ipyautoui.autoform import AutoObjectFormLayout, ShowRaw
-from ipyautoui.custom import SaveButtonBar  # removing makes circular import error
-import json
-import logging
-from ipyautoui.automapschema import map_widget, widgetcaller, _init_model_schema
 import ipywidgets as w
-from pydantic import BaseModel
-from ipyautoui.automapschema import pydantic_validate
-from IPython.display import clear_output
-from ipyautoui.automapschema import (
-    map_widget,
-    widgetcaller,
-    _init_model_schema,
-    get_widgets_map,
-    get_containers_map,
-)
+from pydantic import BaseModel, ValidationError
+from IPython.display import display
+
+from ipyautoui.custom import SaveButtonBar  # removing makes circular import error
 from ipyautoui.autobox import AutoBox
-from ipyautoui.autoform import TitleDescription, WrapSaveButtonBar, ShowRaw, ShowNull
+from ipyautoui.autoform import AutoObjectFormLayout, TitleDescription, WrapSaveButtonBar, ShowRaw, ShowNull
 from ipyautoui.custom.editgrid import EditGrid
+from ipyautoui.automapschema import get_widgets_map, get_containers_map, map_widget, widgetcaller, _init_model_schema, pydantic_validate
+
 logger = logging.getLogger(__name__)
 
 
 # +
-import functools
-
-
 def wrapped_partial(func, *args, **kwargs):
     # http://louistiao.me/posts/adding-__name__-and-__doc__-attributes-to-functoolspartial-objects/
     partial_func = functools.partial(func, *args, **kwargs)
     functools.update_wrapper(partial_func, func)
     return partial_func
 
 
@@ -213,17 +201,14 @@
     def create_autodisplay_map(
         cls, schema: ty.Union[ty.Type[BaseModel], dict], ext=".json", **kwargs
     ):
         AutoRenderer = cls.create_autoui_renderer(schema, **kwargs)
         return {ext: AutoRenderer}
 
 
-
-
-
 def get_autoui(schema: ty.Union[ty.Type[BaseModel], dict], **kwargs):
     model, schema = _init_model_schema(schema)
     schema = {**schema, **kwargs}
     try:
         # assumes the root object is a container so reduces the search space
         caller = map_widget(
             schema, widgets_map=get_containers_map(), fail_on_error=True
@@ -254,14 +239,15 @@
                         self.savebuttonbar,
                         w.HBox([self.bn_showraw, self.bn_shownull, self.html_title]),
                         self.html_description,
                         self.vbx_error,
                         self.vbx_widget,
                         self.vbx_showraw,
                     ]
+                    self.show_hide_bn_nullable()
 
         if model is not None:
             return wrapped_partial(
                 AutoUi.from_pydantic_model, model
             )  # TODO: this is inefficient as the top-level mapping is called twice.
         else:
             return wrapped_partial(AutoUi.from_jsonschema, schema)
```

### Comparing `ipyautoui-0.7.8/src/ipyautoui/autovjsf.py` & `ipyautoui-0.7.9/src/ipyautoui/autovjsf.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/basemodel.py` & `ipyautoui-0.7.9/src/ipyautoui/basemodel.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/constants.py` & `ipyautoui-0.7.9/src/ipyautoui/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,14 +134,27 @@
 DELETE_BUTTON_KWARGS = frozenmap(
     icon="trash-alt",
     button_style="danger",
     tooltip="delete",
     layout={"width": BUTTON_WIDTH_MIN},
 )
 
+SHOWNULL_ICON_SHOW = "plus"
+SHOWNULL_ICON_HIDE = "minus"
+KWARGS_SHOWNULL = frozenmap(
+            icon=SHOWNULL_ICON_SHOW,
+            layout=dict(width=BUTTON_WIDTH_MIN, display=""),
+            tooltip="show null form fields",
+            style={"font_weight": "bold"})
+KWARGS_SHOWRAW = frozenmap(icon="code",
+            layout=dict(width=BUTTON_WIDTH_MIN, display="None"),
+            tooltip="show raw data",
+            style={"font_weight": "bold"},
+        )
+
 
 KWARGS_DATAGRID_DEFAULT = frozenmap(
     header_renderer=TextRenderer(
         vertical_alignment="top",
         horizontal_alignment="center",
     )
 )
```

### Comparing `ipyautoui-0.7.8/src/ipyautoui/demo.py` & `ipyautoui-0.7.9/src/ipyautoui/demo.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/env.py` & `ipyautoui-0.7.9/src/ipyautoui/env.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/mydocstring_display.py` & `ipyautoui-0.7.9/src/ipyautoui/mydocstring_display.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/nullable.py` & `ipyautoui-0.7.9/src/ipyautoui/nullable.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/vjsf.vue` & `ipyautoui-0.7.9/src/ipyautoui/vjsf.vue`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/watch_validate.py` & `ipyautoui-0.7.9/src/ipyautoui/watch_validate.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/autogrid.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/autogrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/boolean_toggle.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/boolean_toggle.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/buttonbars.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/buttonbars.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/combobox_mapped.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/combobox_mapped.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/date_string.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/date_string.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/decision_branch.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/decision_branch.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/editgrid.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/editgrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/filechooser.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/filechooser.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/filesindir.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/filesindir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/fileupload.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/fileupload.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/halo_decorator.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/halo_decorator.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/iterable.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/iterable.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/loadproject.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/loadproject.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/markdown_widget.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/markdown_widget.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/modelrun.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/modelrun.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/multi_toggle_buttons.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/multi_toggle_buttons.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/multiselect_search.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/multiselect_search.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/outputlogging.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/outputlogging.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/selectandclick.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/selectandclick.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/selectdir.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/selectdir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/showhide.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/showhide.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/showopenurl.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/showopenurl.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/title_description.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/title_description.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/urlimagelink.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/urlimagelink.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/custom/widgetcaller_error.py` & `ipyautoui-0.7.9/src/ipyautoui/custom/widgetcaller_error.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/demo_schemas/__init__.py` & `ipyautoui-0.7.9/src/ipyautoui/demo_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/demo_schemas/array_examples.py` & `ipyautoui-0.7.9/src/ipyautoui/demo_schemas/array_examples.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/demo_schemas/array_object_dataframe.py` & `ipyautoui-0.7.9/src/ipyautoui/demo_schemas/array_object_dataframe.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/demo_schemas/complex_serialization.py` & `ipyautoui-0.7.9/src/ipyautoui/demo_schemas/complex_serialization.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/demo_schemas/core_ipywidgets.py` & `ipyautoui-0.7.9/src/ipyautoui/demo_schemas/core_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/demo_schemas/editable_datagrid.py` & `ipyautoui-0.7.9/src/ipyautoui/demo_schemas/editable_datagrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/demo_schemas/editable_datagrid_with_nullable.py` & `ipyautoui-0.7.9/src/ipyautoui/demo_schemas/editable_datagrid_with_nullable.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/demo_schemas/multiindex_editable_grid.py` & `ipyautoui-0.7.9/src/ipyautoui/demo_schemas/multiindex_editable_grid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/demo_schemas/nested.py` & `ipyautoui-0.7.9/src/ipyautoui/demo_schemas/nested.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/demo_schemas/nested_editable_datagrid.py` & `ipyautoui-0.7.9/src/ipyautoui/demo_schemas/nested_editable_datagrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/demo_schemas/null_and_required.py` & `ipyautoui-0.7.9/src/ipyautoui/demo_schemas/null_and_required.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py` & `ipyautoui-0.7.9/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/demo_schemas/override_ipywidgets.py` & `ipyautoui-0.7.9/src/ipyautoui/demo_schemas/override_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/demo_schemas/root_array_enum.py` & `ipyautoui-0.7.9/src/ipyautoui/demo_schemas/root_array_enum.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/demo_schemas/root_enum.py` & `ipyautoui-0.7.9/src/ipyautoui/demo_schemas/root_enum.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/src/ipyautoui/demo_schemas/ruleset.py` & `ipyautoui-0.7.9/src/ipyautoui/demo_schemas/ruleset.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/.gitignore` & `ipyautoui-0.7.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/README.md` & `ipyautoui-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/pyproject.toml` & `ipyautoui-0.7.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.7.8/PKG-INFO` & `ipyautoui-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyautoui
-Version: 0.7.8
+Version: 0.7.9
 Summary: wrapper that sits on top of ipywidgets and other ipy widget libraries to template / automate the creation of widget forms. Uses pydantic to create defined data-container and serialisation to JSON. Includes example patterns for adding new custom widgets.
 Project-URL: Homepage, https://github.com/maxfordham/ipyautoui
 Author-email: John Gunstone <gunstone.john@gmail.com>
 Keywords: ipyautoui
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

