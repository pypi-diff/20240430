# Comparing `tmp/django_json_model_field-0.0.1rc9.tar.gz` & `tmp/django_json_model_field-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_json_model_field-0.0.1rc9.tar", max compression
+gzip compressed data, was "django_json_model_field-1.0.0rc1.tar", max compression
```

## Comparing `django_json_model_field-0.0.1rc9.tar` & `django_json_model_field-1.0.0rc1.tar`

### file list

```diff
@@ -1,19 +1,23 @@
--rw-r--r--   0        0        0        0 2023-04-12 20:21:14.525602 django_json_model_field-0.0.1rc9/django_json_model_field/__init__.py
--rw-r--r--   0        0        0      164 2023-04-13 13:40:27.243250 django_json_model_field-0.0.1rc9/django_json_model_field/apps.py
--rw-r--r--   0        0        0        0 2022-05-23 10:04:59.000000 django_json_model_field-0.0.1rc9/django_json_model_field/db/__init__.py
--rw-r--r--   0        0        0      201 2023-04-12 20:20:36.134890 django_json_model_field-0.0.1rc9/django_json_model_field/db/models/__init__.py
--rw-r--r--   0        0        0    11557 2023-04-13 14:20:30.127417 django_json_model_field-0.0.1rc9/django_json_model_field/db/models/base_json_model_field.py
--rw-r--r--   0        0        0     4789 2023-04-12 20:20:36.135545 django_json_model_field-0.0.1rc9/django_json_model_field/db/models/conditional_json_model_attribute.py
--rw-r--r--   0        0        0    10910 2023-04-12 20:20:36.135837 django_json_model_field-0.0.1rc9/django_json_model_field/db/models/conditional_json_model_field.py
--rw-r--r--   0        0        0    14982 2023-04-13 15:34:27.467409 django_json_model_field-0.0.1rc9/django_json_model_field/db/models/json_model.py
--rw-r--r--   0        0        0     2250 2023-04-12 20:20:36.136519 django_json_model_field-0.0.1rc9/django_json_model_field/db/models/json_model_field.py
--rw-r--r--   0        0        0     9866 2023-04-13 14:29:29.094715 django_json_model_field-0.0.1rc9/django_json_model_field/db/models/json_model_options.py
--rw-r--r--   0        0        0      222 2023-04-12 20:20:40.690115 django_json_model_field-0.0.1rc9/django_json_model_field/forms/__init__.py
--rw-r--r--   0        0        0     7724 2023-04-12 20:20:40.690564 django_json_model_field-0.0.1rc9/django_json_model_field/forms/nested_form_field.py
--rw-r--r--   0        0        0    12215 2023-04-12 20:20:40.690980 django_json_model_field-0.0.1rc9/django_json_model_field/forms/nested_model_form_field.py
--rw-r--r--   0        0        0     2859 2023-04-12 20:20:40.691240 django_json_model_field-0.0.1rc9/django_json_model_field/forms/widgets.py
--rw-r--r--   0        0        0      134 2023-04-12 20:20:45.778809 django_json_model_field-0.0.1rc9/django_json_model_field/templates/django_json_model_field/forms/widgets/nested_form_input.html
--rw-r--r--   0        0        0      188 2022-05-23 10:04:59.000000 django_json_model_field-0.0.1rc9/django_json_model_field/util.py
--rw-r--r--   0        0        0      405 2023-04-13 16:40:50.671476 django_json_model_field-0.0.1rc9/pyproject.toml
--rw-r--r--   0        0        0      875 2023-04-13 16:43:39.972858 django_json_model_field-0.0.1rc9/setup.py
--rw-r--r--   0        0        0      422 2023-04-13 16:43:39.973202 django_json_model_field-0.0.1rc9/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-01 15:25:08.358958 django_json_model_field-1.0.0rc1/django_json_model_field/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:25:08.359243 django_json_model_field-1.0.0rc1/django_json_model_field/db/__init__.py
+-rw-r--r--   0        0        0      255 2024-04-01 15:25:08.359667 django_json_model_field-1.0.0rc1/django_json_model_field/db/models/__init__.py
+-rw-r--r--   0        0        0    12092 2024-04-01 15:51:22.009260 django_json_model_field-1.0.0rc1/django_json_model_field/db/models/base_json_model_field.py
+-rw-r--r--   0        0        0     4789 2024-04-01 15:25:08.360648 django_json_model_field-1.0.0rc1/django_json_model_field/db/models/conditional_json_model_attribute.py
+-rw-r--r--   0        0        0    10910 2024-04-01 15:25:08.361145 django_json_model_field-1.0.0rc1/django_json_model_field/db/models/conditional_json_model_field.py
+-rw-r--r--   0        0        0    14044 2024-04-30 15:06:55.170974 django_json_model_field-1.0.0rc1/django_json_model_field/db/models/json_model.py
+-rw-r--r--   0        0        0     4537 2024-04-01 15:25:08.362172 django_json_model_field-1.0.0rc1/django_json_model_field/db/models/json_model_dict_field.py
+-rw-r--r--   0        0        0     2251 2024-04-11 14:51:07.873731 django_json_model_field-1.0.0rc1/django_json_model_field/db/models/json_model_field.py
+-rw-r--r--   0        0        0     9694 2024-04-30 15:04:45.400312 django_json_model_field-1.0.0rc1/django_json_model_field/db/models/json_model_options.py
+-rw-r--r--   0        0        0      222 2024-04-01 15:25:08.363449 django_json_model_field-1.0.0rc1/django_json_model_field/forms/__init__.py
+-rw-r--r--   0        0        0     7724 2024-04-01 15:25:08.363925 django_json_model_field-1.0.0rc1/django_json_model_field/forms/nested_form_field.py
+-rw-r--r--   0        0        0    12215 2024-04-01 15:25:08.364417 django_json_model_field-1.0.0rc1/django_json_model_field/forms/nested_model_form_field.py
+-rw-r--r--   0        0        0     2859 2024-04-01 15:25:08.364801 django_json_model_field-1.0.0rc1/django_json_model_field/forms/widgets.py
+-rw-r--r--   0        0        0      232 2024-04-01 15:25:08.365168 django_json_model_field-1.0.0rc1/django_json_model_field/serialization/__init__.py
+-rw-r--r--   0        0        0       72 2024-04-01 15:25:08.365533 django_json_model_field-1.0.0rc1/django_json_model_field/serialization/constants.py
+-rw-r--r--   0        0        0      968 2024-04-01 15:25:08.365930 django_json_model_field-1.0.0rc1/django_json_model_field/serialization/json_model_decoder.py
+-rw-r--r--   0        0        0     3333 2024-04-03 21:40:50.701902 django_json_model_field-1.0.0rc1/django_json_model_field/serialization/json_model_encoder.py
+-rw-r--r--   0        0        0      646 2024-04-01 15:25:08.366684 django_json_model_field-1.0.0rc1/django_json_model_field/serialization/types.py
+-rw-r--r--   0        0        0      134 2024-04-01 15:25:08.367066 django_json_model_field-1.0.0rc1/django_json_model_field/templates/django_json_model_field/forms/widgets/nested_form_input.html
+-rw-r--r--   0        0        0      188 2024-04-01 15:25:08.367431 django_json_model_field-1.0.0rc1/django_json_model_field/util.py
+-rw-r--r--   0        0        0      793 2024-04-30 15:17:25.758382 django_json_model_field-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      372 1970-01-01 00:00:00.000000 django_json_model_field-1.0.0rc1/PKG-INFO
```

### Comparing `django_json_model_field-0.0.1rc9/django_json_model_field/db/models/base_json_model_field.py` & `django_json_model_field-1.0.0rc1/django_json_model_field/db/models/base_json_model_field.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
+
 from abc import ABCMeta, abstractmethod
-from typing import Any, Optional, TYPE_CHECKING, Type, Union
+from typing import Any, TYPE_CHECKING, Type
 
 from django.core import checks
 from django.core.exceptions import ValidationError
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models import Field, JSONField, Model
 
 if TYPE_CHECKING:
@@ -26,32 +28,32 @@
             **kwargs,
         )
 
         # don't use super().formfield because the form field doesn't need the same things as the base JSONField
         return Field.formfield(self, **kwargs)
 
     @abstractmethod
-    def get_json_model_class(self, host: Union[Model, dict]) -> Optional[Type["JSONModel"]]:
+    def get_json_model_class(self, host: Model | dict) -> Type[JSONModel] | None:
         """
         Returns the `JSONModel` class to be used to represent the field data
         """
 
         raise NotImplementedError()
 
     def from_db_value(self, value, expression, connection):
         # overridden method from Field and JSONField used to convert the DB's JSON (string) value to a dict, and then
         # from the dict to an instance of the JSONModel defined for the field
-        data: Optional[dict] = super().from_db_value(value, expression, connection)
+        data: dict | None = super().from_db_value(value, expression, connection)
 
         return self.from_db_data_dict(data, connection)
 
-    def from_db_data_dict(self, data: Optional[dict], connection: BaseDatabaseWrapper) -> Optional["JSONModel"]:
+    def from_db_data_dict(self, data: dict | None, connection: BaseDatabaseWrapper) -> JSONModel | None:
         host_data = self.get_json_model_host_data(data)
         json_model = self.get_json_model_class(host=host_data)
-        if json_model is None:
+        if json_model is None or data is None or data in self.empty_values:
             return None
 
         has_input = data is not None
         data = data or {}
         converted_data = {
             field.name: self._convert_field(connection, field, data.get(field.name))
             for field in json_model._meta.fields
@@ -59,30 +61,42 @@
         return json_model(_has_input=has_input, **converted_data, _skip_clean=True) if json_model else None
 
     def _convert_field(self, connection, field: Field, value: Any):
         """
         Uses the field's db converters to restore the value to its Python/Django representation
         """
 
+        from django_json_model_field.db.models import JSONModel
+
+        # TODO: all the DB conversion logic needs to get cleaned up and have unit test coverage - there are too many
+        #       edge cases and potential for bugs to not have tests for this
+        if isinstance(value, JSONModel):
+            return value
+
+        if isinstance(field, BaseJSONModelField):
+            if isinstance(value, str):
+                return field.from_db_value(value, None, connection)
+            return field.from_db_data_dict(value, connection)
+
         # See code comments in _get_db_prep_value_from_model for why this is necessary
         converters = field.get_db_converters(connection)
         for converter in converters:
             value = converter(value=value, expression=None, connection=connection)
 
         return value
 
     def save_form_data(self, instance: Model, data: dict):
         json_model_class = self.get_json_model_class(instance)
         value = json_model_class(**data) if json_model_class else None
         setattr(instance, self.name, value)
 
-    def get_json_model_host_data(self, data: Optional[dict]) -> dict:
+    def get_json_model_host_data(self, data: dict | None) -> dict:
         return {}
 
-    def clean(self, value: Optional[Union[dict, "JSONModel"]], model_instance: Optional[Model]):
+    def clean(self, value: dict | JSONModel | None, model_instance: Model | None):
         """
         Convert the value's type and run validation. Validation errors
         from to_python() and validate() are propagated. Return the correct
         value if no error is raised.
         """
         value = self.to_python(value, model_instance)
         try:
@@ -92,16 +106,15 @@
             # nested validation errors from attempting to validate the JSONModel instance, and allows form fields
             # derived from this field to hide the messaging from this validation error in favor of showing the
             # validation errors on the individual fields for the JSONModel.
             raise ValidationError("The model contains validation errors", code="model_validation")
         self.run_validators(value)
         return value
 
-    def to_python(self, value: Optional[Union[dict, "JSONModel"]], model_instance: Model = None) -> Optional[
-        "JSONModel"]:
+    def to_python(self, value: dict | JSONModel | None, model_instance: Model = None) -> JSONModel | None:
         from django_json_model_field.db.models import JSONModel
 
         # note: signature is overridden from the base Field signature to include the model instance. This is possible
         #       since the `clean` method is also overridden to pass its model_instance argument along.
 
         # the value must either already be a JSONModel instance, or a dict that can then be converted to JSONModel
         # instance so that the field validation for that model can be checked before saving
@@ -117,15 +130,15 @@
                 return None
 
             # _skip_clean=True because it will be validated elsewhere
             return json_model_class(_skip_clean=True, **value)
 
         return None
 
-    def validate(self, value: Optional["JSONModel"], model_instance: Optional[Model]):
+    def validate(self, value: JSONModel | None, model_instance: Model | None):
         if value is not None:
             value.full_clean()
 
         # the JSONField superclass validates whether the value is valid JSON, so it needs the data in dict form
         super().validate(self.get_prep_value(value) if value else None, model_instance)
 
     def get_prep_value(self, value):
@@ -181,15 +194,15 @@
         #
         # Note that this is uses get_db_prep_value as opposed to get_prep_value that is used in
         # _get_prep_value_from_model - get_db_prep_value is used to convert values to representations suitable to be
         # stored in a specific type of database column (e.g. DurationField uses an integer when the DB does not have a
         # specialized "duration" type column). While this is not strictly necessary for a JSONModel since the values are
         # being serialized to JSON, using get_db_prep_value will ensure that the representations of values stored in the
         # JSON are interchangeable with those that use the same Django field type on a field for an actual DB column.
-        # This will make querying the data more straightforward outside of Django, such as when querying a database
+        # This will make querying the data more straightforward outside Django, such as when querying a database
         # directly for debugging or maintenance, or when the data is synchronized to another DB provider for a data
         # warehouse or processed through an ETL.
         return {
             field.name: field.get_db_prep_value(field.value_from_object(instance), connection)
             for field in instance._meta.fields
         }
```

### Comparing `django_json_model_field-0.0.1rc9/django_json_model_field/db/models/conditional_json_model_attribute.py` & `django_json_model_field-1.0.0rc1/django_json_model_field/db/models/conditional_json_model_attribute.py`

 * *Files identical despite different names*

### Comparing `django_json_model_field-0.0.1rc9/django_json_model_field/db/models/conditional_json_model_field.py` & `django_json_model_field-1.0.0rc1/django_json_model_field/db/models/conditional_json_model_field.py`

 * *Files identical despite different names*

### Comparing `django_json_model_field-0.0.1rc9/django_json_model_field/db/models/json_model.py` & `django_json_model_field-1.0.0rc1/django_json_model_field/db/models/json_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-from __future__ import annotations
-
 import copy
-import inspect
 from itertools import chain
-from typing import Any
+from typing import Any, Protocol, runtime_checkable
 
-from django.apps import apps
-from django.core import checks
 from django.core.exceptions import FieldDoesNotExist, FieldError
-from django.db.models import DateField, Field, Model
-from django.db.models.base import ModelBase
+from django.db.models import Model
+from django.db.models.base import ModelBase, ModelState
 
 from .json_model_options import JSONModelOptions
 
 
-def _has_contribute_to_class(value):
-    # Only call contribute_to_class() if it's bound.
-    return not inspect.isclass(value) and hasattr(value, "contribute_to_class")
+@runtime_checkable
+class ContributesToClass(Protocol):
+
+    def contribute_to_class(self, cls: type, name: str, private_only: bool = False):
+        ...
 
 
 class JSONModelBase(type):
     """
     Metaclass for all JSON Models.
 
     Adapted from Django's ModelBase class.
@@ -57,42 +54,27 @@
             new_attrs["__classcell__"] = classcell
         attr_meta = attrs.pop("Meta", None)
         # Pass all attrs without a (Django-specific) contribute_to_class()
         # method to type.__new__() so that they're properly initialized
         # (i.e. __set_name__()).
         contributable_attrs = {}
         for obj_name, obj in list(attrs.items()):
-            if _has_contribute_to_class(obj):
+            if isinstance(obj, ContributesToClass):
                 contributable_attrs[obj_name] = obj
             else:
                 new_attrs[obj_name] = obj
         new_class = super_new(mcs, name, bases, new_attrs, **kwargs)
 
         abstract = getattr(attr_meta, "abstract", False)
         meta = attr_meta or getattr(new_class, "Meta", None)
         base_meta = getattr(new_class, "_meta", None)
 
-        app_label = None
-
-        # Look for an application configuration to attach the model to.
-        app_config = apps.get_containing_app_config(module)
-
-        if getattr(meta, 'app_label', None) is None:
-            if app_config is None:
-                if not abstract:
-                    raise RuntimeError(
-                        "Model class %s.%s doesn't declare an explicit "
-                        "app_label and isn't in an application in "
-                        "INSTALLED_APPS." % (module, name)
-                    )
-
-            else:
-                app_label = app_config.label
+        # skipping ModelBase logic related to app_label since it's not used (Django uses it for its model registry)
 
-        new_class.add_to_class("_meta", JSONModelOptions(meta, app_label))
+        new_class.add_to_class("_meta", JSONModelOptions(meta))
         if not abstract and base_meta and not base_meta.abstract:
             # Non-abstract child classes inherit some attributes from their
             # non-abstract parent (unless an ABC comes before it in the
             # method resolution order).
             if not hasattr(meta, "ordering"):
                 new_class._meta.ordering = base_meta.ordering
 
@@ -218,14 +200,16 @@
 
         Arguments:
             _has_input - for internal use - allows the initializer to distinguish between being invoked with no data
                          (effectively an uninitialized instance), and being invoked with an empty data mapping
             _skip_clean - for internal use - when True, skips validation if input is provided. Used when initializing
                           objects from DB JSON data to prevent malformed data from breaking object loading.
         """
+        
+        self._state = ModelState()
 
         if _has_input is None:
             _has_input = bool(data)
 
         if not _has_input:
             self._init_field_defaults()
             return
@@ -245,46 +229,34 @@
         replaced; if it is not replaced, it will raise an error if anything attempts to access the field's value.
 
         Parameters
         ----------
         initial
         """
 
-        # Iterate through the list of fields rather than data keys so that the field's default value is set if there is
-        # no initial value
+        # Iterate through the list of fields rather than data keys so that a None value is set for any missing fields
         for field in self._meta.fields:
-            value = self._get_initial_value(field=field, initial=initial)
+            value = initial[field.name] if field.name in initial else field.get_default()
             setattr(self, field.name, value)
 
-    @classmethod
-    def _get_initial_value(cls, field: Field, initial: dict[str, Any]) -> Any:
-        if field.name not in initial:
-            return field.get_default()
-
-        initial_value = initial[field.name]
-        if initial_value is None or initial_value in field.empty_values:
-            return None
-
-        return field.to_python(initial_value)
-
     def _init_field_defaults(self) -> None:
         for field in self._meta.fields:
             if field.has_default():
                 setattr(self, field.name, field.get_default())
 
     def _ensure_fields_initialized(self, data: dict = None) -> None:
         """
         Similar to `_init_fields`, ensures all fields have a value set to prevent errors when attempting to use their
         field accessor. Unlike _init_fields, only sets a None value if no value has been defined yet.
         """
 
         for field in self._meta.fields:
             try:
                 getattr(self, field.name)
-            except FieldDoesNotExist:
+            except (FieldDoesNotExist, KeyError):
                 # field value has not been set yet, still using DeferredAttribute
                 setattr(self, field.name, data.get(field.name) if data else None)
 
     ##############################
     # adaptations of Model methods
     ##############################
 
@@ -304,26 +276,14 @@
 
         # adapted from Model._check_fields - only local fields need to be checked, no other types of fields are
         # supported
 
         errors = []
         for field in cls._meta.local_fields:
             errors.extend(field.check(**kwargs))
-            if isinstance(field, DateField):
-                errors.extend(cls._check_date_field(field))
-        return errors
-
-    @classmethod
-    def _check_date_field(cls, field: DateField):
-        errors = []
-        if field.auto_now_add:
-            errors.append(
-                checks.Critical("DateFields defined on a JSONModel cannot use auto_now_add=True", obj=field)
-            )
-
         return errors
 
     ###############################################################################################################
     # passthrough methods - these can be used as-is from Django's Model class directly rather than copy/pasting the
     # code
     ###############################################################################################################
 
@@ -334,14 +294,20 @@
     def clean_fields(self, exclude=None):
         return Model.clean_fields(self, exclude)
 
     def _get_FIELD_display(self, field):
         # used by fields that allow "choices"
         return Model._get_FIELD_display(self, field)
 
+    def get_constraints(self):
+        return Model.get_constraints(self)
+
+    def validate_constraints(self, exclude=None):
+        return Model.validate_constraints(self, exclude)
+
     def clean(self):
         """
         Hook for doing any extra model-wide validation after clean() has been
         called on every field by self.clean_fields. Any ValidationError raised
         by this method will not be associated with a particular field; it will
         have a special-case association with the field defined by NON_FIELD_ERRORS.
         """
@@ -351,7 +317,13 @@
     # placeholder methods - these are methods used by Django Models that pertain to functionality not needed or not
     #                       supported by JSONModel. They are provided as noops so to allow JSONModel classes to be used
     #                       interchangeably with Django Model classes for ModelForms and ModelAdmin.
     ###################################################################################################################
 
     def validate_unique(self, exclude=None):
         pass
+
+    def refresh_from_db(self, using=None, fields=None):
+        pass
+
+    def clone(self):
+        return self.__class__(**{field.name: getattr(self, field.name) for field in self._meta.fields})
```

### Comparing `django_json_model_field-0.0.1rc9/django_json_model_field/db/models/json_model_field.py` & `django_json_model_field-1.0.0rc1/django_json_model_field/db/models/json_model_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .base_json_model_field import BaseJSONModelField
 
 if TYPE_CHECKING:
     from .json_model import JSONModel
 
 
 class JSONModelField(BaseJSONModelField):
+
     def __init__(
         self,
         json_model: Optional[Type["JSONModel"]],
         verbose_name: str = None,
         name: str = None,
         null: bool = True,
         blank: bool = True,
```

### Comparing `django_json_model_field-0.0.1rc9/django_json_model_field/db/models/json_model_options.py` & `django_json_model_field-1.0.0rc1/django_json_model_field/db/models/json_model_options.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from __future__ import annotations
-
 import inspect
 from collections import OrderedDict
 from typing import TYPE_CHECKING, Type
 
 from django.core.exceptions import FieldDoesNotExist
+from django.db.models import Field
 from django.db.models.options import Options as ModelOptions
 from django.utils.datastructures import ImmutableList
 from django.utils.functional import cached_property
 from django.utils.translation import override
 
 if TYPE_CHECKING:
     from .json_model import JSONModel
@@ -38,55 +37,48 @@
 
     Adapted from Django's Options class (imported in this module as ModelOptions for easier disambiguation)
     """
 
     FORWARD_PROPERTIES = {"fields", "concrete_fields", "local_concrete_fields", "_forward_fields_map"}
     REVERSE_PROPERTIES = {"related_objects", "fields_map", "_relation_tree"}
 
-    model: Type[JSONModel]
+    model: Type["JSONModel"]
 
     # not supported
     proxy = False
     proxy_for_model = None
 
-    def __init__(self, meta, app_label: str):
+    def __init__(self, meta):
         self._get_fields_cache = {}
         self.local_fields = []
         self.private_fields = []
         self.model_name = None
         self.verbose_name = None
         self.verbose_name_plural = None
         self.object_name = None
         self.meta = meta
         self.parents = OrderedDict()
         self.concrete_model = None
         self.ordering = []
         self._ordering_clash = False
         self.abstract = False
-        self.app_label = app_label
 
         ##########################################################################################################
         # attributes used for compatibility with Model; values are only used for conditional checks an enumeration
         ##########################################################################################################
 
+        self.app_label = None
+        self.constraints = []
         self.db_table = "n/a"
         self.required_db_features: tuple = ()
         self.local_many_to_many: list = []
         self.many_to_many: list = []
         self.proxy = None
         self._relation_tree = ()
 
-    @property
-    def label(self):
-        return '%s.%s' % (self.app_label, self.object_name)
-
-    @property
-    def label_lower(self):
-        return '%s.%s' % (self.app_label, self.model_name)
-
     def get_field(self, field_name):
         """
         Return a field instance given the name of a forward or reverse field.
         """
 
         # Adapted from Options.get_field to omit checks for related fields, which are not supported
 
@@ -153,15 +145,15 @@
     @property
     def verbose_name_raw(self):
         """Return the untranslated verbose name."""
         with override(None):
             return str(self.verbose_name)
 
     @cached_property
-    def fields(self):
+    def fields(self) -> list[Field]:
         """
         Return a list of all forward fields on the model and its parents,
         excluding ManyToManyFields.
 
         Private API intended only to be used by Django itself; get_fields()
         combined with filtering of field properties is the public API for
         obtaining this field list.
```

### Comparing `django_json_model_field-0.0.1rc9/django_json_model_field/forms/nested_form_field.py` & `django_json_model_field-1.0.0rc1/django_json_model_field/forms/nested_form_field.py`

 * *Files identical despite different names*

### Comparing `django_json_model_field-0.0.1rc9/django_json_model_field/forms/nested_model_form_field.py` & `django_json_model_field-1.0.0rc1/django_json_model_field/forms/nested_model_form_field.py`

 * *Files identical despite different names*

### Comparing `django_json_model_field-0.0.1rc9/django_json_model_field/forms/widgets.py` & `django_json_model_field-1.0.0rc1/django_json_model_field/forms/widgets.py`

 * *Files identical despite different names*

