# Comparing `tmp/django_aux-0.0.82.tar.gz` & `tmp/django-aux-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_aux-0.0.82.tar", last modified: Tue Apr 30 16:18:01 2024, max compression
+gzip compressed data, was "django-aux-0.0.9.tar", last modified: Wed Jul  6 13:38:58 2022, max compression
```

## Comparing `django_aux-0.0.82.tar` & `django-aux-0.0.9.tar`

### file list

```diff
@@ -1,70 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 16:18:01.731932 django_aux-0.0.82/
--rw-rw-rw-   0        0        0     1090 2022-07-05 14:54:23.000000 django_aux-0.0.82/LICENSE
--rw-rw-rw-   0        0        0      143 2022-07-05 21:15:46.000000 django_aux-0.0.82/MANIFEST.in
--rw-rw-rw-   0        0        0     2753 2024-04-30 16:18:01.730929 django_aux-0.0.82/PKG-INFO
--rw-rw-rw-   0        0        0      112 2022-07-05 14:54:23.000000 django_aux-0.0.82/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 16:18:01.680927 django_aux-0.0.82/django_aux/
--rw-rw-rw-   0        0        0        0 2022-07-04 12:21:58.000000 django_aux-0.0.82/django_aux/__init__.py
--rw-rw-rw-   0        0        0       66 2022-07-04 12:21:58.000000 django_aux-0.0.82/django_aux/admin.py
--rw-rw-rw-   0        0        0      157 2022-07-04 12:21:58.000000 django_aux-0.0.82/django_aux/apps.py
--rw-rw-rw-   0        0        0    28535 2024-04-30 16:08:02.000000 django_aux-0.0.82/django_aux/columns.py
--rw-rw-rw-   0        0        0      389 2022-07-06 13:07:44.000000 django_aux-0.0.82/django_aux/decorators.py
--rw-rw-rw-   0        0        0     1552 2022-09-01 02:47:31.000000 django_aux-0.0.82/django_aux/factory.py
--rw-rw-rw-   0        0        0     3904 2022-09-13 12:43:13.000000 django_aux-0.0.82/django_aux/filters.py
--rw-rw-rw-   0        0        0     1434 2023-01-20 18:49:39.000000 django_aux-0.0.82/django_aux/forms.py
--rw-rw-rw-   0        0        0      862 2022-08-26 02:14:36.000000 django_aux-0.0.82/django_aux/middleware.py
--rw-rw-rw-   0        0        0     3914 2023-01-27 14:47:42.000000 django_aux-0.0.82/django_aux/models.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:18:01.658419 django_aux-0.0.82/django_aux/static/
-drwxrwxrwx   0        0        0        0 2024-04-30 16:18:01.689930 django_aux-0.0.82/django_aux/static/css/
--rw-rw-rw-   0        0        0     2647 2022-07-04 12:21:58.000000 django_aux-0.0.82/django_aux/static/css/main.css
-drwxrwxrwx   0        0        0        0 2024-04-30 16:18:01.693930 django_aux-0.0.82/django_aux/static/js/
--rw-rw-rw-   0        0        0     1739 2022-07-26 11:25:34.000000 django_aux-0.0.82/django_aux/static/js/save_set_collapse_status.js
--rw-rw-rw-   0        0        0     1130 2022-07-26 11:23:45.000000 django_aux-0.0.82/django_aux/static/js/save_set_scroll_pos.js
--rw-rw-rw-   0        0        0       13 2023-01-21 18:59:16.000000 django_aux-0.0.82/django_aux/static/js/show_hide_remove_btn.js
-drwxrwxrwx   0        0        0        0 2024-04-30 16:18:01.659421 django_aux-0.0.82/django_aux/templates/
-drwxrwxrwx   0        0        0        0 2024-04-30 16:18:01.705928 django_aux-0.0.82/django_aux/templates/django_aux/
--rw-rw-rw-   0        0        0     9486 2022-12-27 18:33:09.000000 django_aux-0.0.82/django_aux/templates/django_aux/base.html
--rw-rw-rw-   0        0        0      906 2022-12-31 11:46:39.000000 django_aux-0.0.82/django_aux/templates/django_aux/checkbox-table.html
--rw-rw-rw-   0        0        0     1126 2022-12-31 11:46:42.000000 django_aux-0.0.82/django_aux/templates/django_aux/dash-filter.html
--rw-rw-rw-   0        0        0      937 2023-01-03 18:06:33.000000 django_aux-0.0.82/django_aux/templates/django_aux/delete.html
--rw-rw-rw-   0        0        0     2368 2023-01-03 20:28:05.000000 django_aux-0.0.82/django_aux/templates/django_aux/form-table.html
--rw-rw-rw-   0        0        0     2293 2023-01-21 18:57:29.000000 django_aux-0.0.82/django_aux/templates/django_aux/inline-formset.html
--rw-rw-rw-   0        0        0      546 2023-01-27 16:09:55.000000 django_aux-0.0.82/django_aux/templates/django_aux/login.html
--rw-rw-rw-   0        0        0      326 2023-01-27 16:10:37.000000 django_aux-0.0.82/django_aux/templates/django_aux/logout.html
--rw-rw-rw-   0        0        0     3145 2022-12-31 11:46:56.000000 django_aux-0.0.82/django_aux/templates/django_aux/standard-plotly.html
--rw-rw-rw-   0        0        0     2849 2023-01-07 15:57:40.000000 django_aux-0.0.82/django_aux/templates/django_aux/standard.html
--rw-rw-rw-   0        0        0      303 2022-08-07 17:31:57.000000 django_aux-0.0.82/django_aux/urls.py
--rw-rw-rw-   0        0        0     4944 2024-04-30 16:01:12.000000 django_aux-0.0.82/django_aux/utils.py
--rw-rw-rw-   0        0        0    27257 2023-11-12 14:20:43.000000 django_aux-0.0.82/django_aux/views.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:18:01.729928 django_aux-0.0.82/django_aux.egg-info/
--rw-rw-rw-   0        0        0     2753 2024-04-30 16:18:01.000000 django_aux-0.0.82/django_aux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1657 2024-04-30 16:18:01.000000 django_aux-0.0.82/django_aux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 16:18:01.000000 django_aux-0.0.82/django_aux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      228 2024-04-30 16:18:01.000000 django_aux-0.0.82/django_aux.egg-info/requires.txt
--rw-rw-rw-   0        0        0       49 2024-04-30 16:18:01.000000 django_aux-0.0.82/django_aux.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-30 16:18:01.711931 django_aux-0.0.82/django_aux_geo/
--rw-rw-rw-   0        0        0        0 2022-07-04 12:21:58.000000 django_aux-0.0.82/django_aux_geo/__init__.py
--rw-rw-rw-   0        0        0      164 2022-09-16 16:32:11.000000 django_aux-0.0.82/django_aux_geo/apps.py
--rw-rw-rw-   0        0        0      825 2023-12-15 18:18:19.000000 django_aux-0.0.82/django_aux_geo/filters.py
--rw-rw-rw-   0        0        0     5534 2023-12-15 18:06:15.000000 django_aux-0.0.82/django_aux_geo/models.py
--rw-rw-rw-   0        0        0      397 2023-12-15 18:20:05.000000 django_aux-0.0.82/django_aux_geo/tables.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:18:01.716930 django_aux-0.0.82/django_aux_timeperiods/
--rw-rw-rw-   0        0        0        0 2022-07-04 12:21:58.000000 django_aux-0.0.82/django_aux_timeperiods/__init__.py
--rw-rw-rw-   0        0        0       66 2022-07-04 12:21:58.000000 django_aux-0.0.82/django_aux_timeperiods/admin.py
--rw-rw-rw-   0        0        0      179 2022-09-16 15:30:26.000000 django_aux-0.0.82/django_aux_timeperiods/apps.py
--rw-rw-rw-   0        0        0     9126 2023-03-03 13:47:33.000000 django_aux-0.0.82/django_aux_timeperiods/models.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:18:01.661422 django_aux-0.0.82/docs/
-drwxrwxrwx   0        0        0        0 2024-04-30 16:18:01.723929 django_aux-0.0.82/docs/source/
--rw-rw-rw-   0        0        0       39 2022-08-28 17:51:16.000000 django_aux-0.0.82/docs/source/conf.py
--rw-rw-rw-   0        0        0      198 2022-08-28 17:45:17.000000 django_aux-0.0.82/docs/source/django_aux.migrations.rst
--rw-rw-rw-   0        0        0     1964 2022-08-28 17:45:17.000000 django_aux-0.0.82/docs/source/django_aux.rst
--rw-rw-rw-   0        0        0      427 2022-08-28 17:45:17.000000 django_aux-0.0.82/docs/source/django_aux.templatetags.rst
--rw-rw-rw-   0        0        0       84 2022-08-28 17:45:17.000000 django_aux-0.0.82/docs/source/modules.rst
--rw-rw-rw-   0        0        0      110 2022-08-28 17:45:17.000000 django_aux-0.0.82/docs/source/setup.rst
--rw-rw-rw-   0        0        0     1517 2024-04-30 15:42:24.000000 django_aux-0.0.82/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-30 16:18:01.732930 django_aux-0.0.82/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-30 16:18:01.727931 django_aux-0.0.82/tests/
--rw-rw-rw-   0        0        0     9194 2023-01-22 13:55:18.000000 django_aux-0.0.82/tests/test_daux.py
--rw-rw-rw-   0        0        0      378 2022-10-08 17:40:33.000000 django_aux-0.0.82/tests/test_daux_geo.py
--rw-rw-rw-   0        0        0     5229 2022-11-27 18:54:06.000000 django_aux-0.0.82/tests/test_daux_timeperiods.py
--rw-rw-rw-   0        0        0     1975 2022-10-07 18:35:22.000000 django_aux-0.0.82/tests/test_settings.py
+drwxrwxrwx   0        0        0        0 2022-07-06 13:38:58.748368 django-aux-0.0.9/
+-rw-rw-rw-   0        0        0     1090 2022-07-05 14:54:23.000000 django-aux-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      143 2022-07-05 21:15:46.000000 django-aux-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1101 2022-07-06 13:38:58.748368 django-aux-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      112 2022-07-05 14:54:23.000000 django-aux-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-07-06 13:38:58.723368 django-aux-0.0.9/django_aux/
+-rw-rw-rw-   0        0        0        0 2022-07-04 12:21:58.000000 django-aux-0.0.9/django_aux/__init__.py
+-rw-rw-rw-   0        0        0       66 2022-07-04 12:21:58.000000 django-aux-0.0.9/django_aux/admin.py
+-rw-rw-rw-   0        0        0      157 2022-07-04 12:21:58.000000 django-aux-0.0.9/django_aux/apps.py
+-rw-rw-rw-   0        0        0     7360 2022-07-06 12:31:42.000000 django-aux-0.0.9/django_aux/columns.py
+-rw-rw-rw-   0        0        0      389 2022-07-06 13:07:44.000000 django-aux-0.0.9/django_aux/decorators.py
+-rw-rw-rw-   0        0        0     4365 2022-07-06 12:30:45.000000 django-aux-0.0.9/django_aux/filters.py
+drwxrwxrwx   0        0        0        0 2022-07-06 13:38:58.742367 django-aux-0.0.9/django_aux/migrations/
+-rw-rw-rw-   0        0        0        0 2022-07-04 12:21:58.000000 django-aux-0.0.9/django_aux/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2371 2022-07-06 13:33:21.000000 django-aux-0.0.9/django_aux/models.py
+drwxrwxrwx   0        0        0        0 2022-07-06 13:38:58.743368 django-aux-0.0.9/django_aux/static/
+-rw-rw-rw-   0        0        0     2647 2022-07-04 12:21:58.000000 django-aux-0.0.9/django_aux/static/main.css
+drwxrwxrwx   0        0        0        0 2022-07-06 13:38:58.706367 django-aux-0.0.9/django_aux/templates/
+drwxrwxrwx   0        0        0        0 2022-07-06 13:38:58.745367 django-aux-0.0.9/django_aux/templates/django_aux/
+-rw-rw-rw-   0        0        0     7346 2022-07-05 21:35:24.000000 django-aux-0.0.9/django_aux/templates/django_aux/base.html
+-rw-rw-rw-   0        0        0     2082 2022-07-05 22:03:29.000000 django-aux-0.0.9/django_aux/templates/django_aux/standard.html
+drwxrwxrwx   0        0        0        0 2022-07-06 13:38:58.747367 django-aux-0.0.9/django_aux/templatetags/
+-rw-rw-rw-   0        0        0        0 2022-07-04 12:21:58.000000 django-aux-0.0.9/django_aux/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      645 2022-07-04 12:21:58.000000 django-aux-0.0.9/django_aux/templatetags/aux_tags.py
+-rw-rw-rw-   0        0        0       63 2022-07-04 12:21:58.000000 django-aux-0.0.9/django_aux/tests.py
+-rw-rw-rw-   0        0        0       56 2022-07-05 21:41:23.000000 django-aux-0.0.9/django_aux/urls.py
+-rw-rw-rw-   0        0        0    13049 2022-07-06 13:38:15.000000 django-aux-0.0.9/django_aux/views.py
+drwxrwxrwx   0        0        0        0 2022-07-06 13:38:58.741367 django-aux-0.0.9/django_aux.egg-info/
+-rw-rw-rw-   0        0        0     1101 2022-07-06 13:38:58.000000 django-aux-0.0.9/django_aux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      664 2022-07-06 13:38:58.000000 django-aux-0.0.9/django_aux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-07-06 13:38:58.000000 django-aux-0.0.9/django_aux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2022-07-06 13:38:58.000000 django-aux-0.0.9/django_aux.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2022-07-06 13:38:58.000000 django-aux-0.0.9/django_aux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2022-07-05 14:54:23.000000 django-aux-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1196 2022-07-06 13:38:58.749368 django-aux-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0       41 2022-07-05 14:54:23.000000 django-aux-0.0.9/setup.py
```

### Comparing `django_aux-0.0.82/LICENSE` & `django-aux-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django_aux-0.0.82/django_aux/filters.py` & `django-aux-0.0.9/django_aux/filters.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,67 +25,87 @@
             'extra': lambda f: {
                 'widget': forms.CheckboxSelectMultiple,
                 'choices': ((True, 'Yes'), (False, 'No'))
             },
         },
     }
 
-class FilterSetBase(FilterSet):
+class BaseFilterSet(FilterSet):
     ''' A BaseFilter class that initializes a crispy form helper 
     with submit and clear filter buttons '''
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.form.helper = FormHelper()
-        self.form.helper.disable_csrf = True
         self.form.helper.add_input(
             Submit('submit', 'Apply Filter')
         )
         self.form.helper.add_input(
             Submit('clear_filter', 'Clear Filter', css_class='btn-warning')
         )
 
 
+
 class PlotSettingsFilterMixin(FilterSet):
     ''' The purpose of this filter is to add in a standard form for plot
     settings to a normal model filter'''
 
     def filter_queryset(self, queryset):
         qdict = self.form.cleaned_data.copy()
-        for key in ['x', 'y', 'plot_type', 'color', 'aggregate_by', 'N_min', 'y_min', 'y_max']:
+        for key in ['x', 'y', 'plot_type', 'color', 'aggregate_by', 'N_min']:
             if key in qdict.keys():
                 qdict.pop(key)
         for name, value in qdict.items():
             if value in ['', None, []]:
                 continue
             queryset = self.filters[name].filter(queryset, value)
             assert isinstance(queryset, models.QuerySet), \
                 "Expected '%s.%s' to return a QuerySet, but got a %s instead." \
                 % (type(self).__name__, name, type(queryset).__name__)
         return queryset
 
     def __init__(self, *args, choices=None, **kwargs):
         super().__init__(*args, **kwargs)
-        self.form.fields['x'] = forms.ChoiceField(choices=choices.get('X_CHOICES'))
-        self.form.fields['y'] = forms.ChoiceField(choices=choices.get('Y_CHOICES'))
-        self.form.fields['plot_type'] = forms.ChoiceField(choices=choices.get('PLOT_TYPE_CHOICES'))
-        self.form.fields['color'] = forms.ChoiceField(choices=choices.get('COLOR_CHOICES'), required=False)
-        self.form.fields['aggregate_by'] = forms.ChoiceField(choices=choices.get('AGG_CHOICES'), required=False)
-        self.form.fields['N_min'] = forms.IntegerField(initial=0, required=False, label='Sample Size Min')
-        self.form.fields['y_min'] = forms.FloatField(required=False, label='Y Min Value')
-        self.form.fields['y_max'] = forms.FloatField(required=False, label='Y Max Value')
+        if choices == None:
+            choices = dict(
+                X_CHOICES=(('quarter', 'Quarter'), ('month', 'Month'),
+                           ('week', 'Week'), ('day', 'Day')),
+                Y_CHOICES=[],
+                COLOR_CHOICES=[],
+                PLOT_TYPE_CHOICES=(
+                    ('barg', 'Bar-Grouped'), ('bars', 'Bar-Stacked'),
+                    ('line', 'Line'), ('scatter', 'Scatter'),
+                    ('box', 'Box'), ('violin', 'Violin'),
+                ),
+                AGG_CHOICES=(
+                    (None, '--------'),
+                    ('quarter', 'Quarter'), ('month',
+                                             'Month'), ('week', 'Week'), ('day', 'Day')
+                )
+            )
+        self.form.fields['x'] = forms.ChoiceField(
+            choices=choices.get('X_CHOICES'))
+        self.form.fields['y'] = forms.ChoiceField(
+            choices=choices.get('Y_CHOICES'))
+        self.form.fields['plot_type'] = forms.ChoiceField(
+            choices=choices.get('PLOT_TYPE_CHOICES'))
+        self.form.fields['color'] = forms.ChoiceField(
+            choices=choices.get('COLOR_CHOICES'), required=False)
+        self.form.fields['aggregate_by'] = forms.ChoiceField(
+            choices=choices.get('AGG_CHOICES'), required=False)
+        self.form.fields['N_min'] = forms.IntegerField(
+            initial=0, required=False, label='Sample Size Min')
         self.extra_layout = Layout(
             Fieldset('Plot Settings',
                 Row(
                     Div('aggregate_by', css_class='ml-2 col-flex'),
                     Div('x', css_class='ml-2 col-flex'),
                     Div('y', css_class='ml-2 col-flex'),
                     Div('color', css_class='ml-2 col-flex'),
                     Div('plot_type', css_class='ml-2 col-flex'),
-                    Div('N_min', css_class='ml-2 col-flex',style='width:125px'),
-                    Div('y_min', css_class='ml-2 col-flex',style='width:125px'),
-                    Div('y_max', css_class='ml-2 col-flex',style='width:125px'),
+                    Div('N_min', css_class='ml-2 col-flex',
+                        style='width:175px'),
                 ),
             ),
         )
```

### Comparing `django_aux-0.0.82/django_aux/models.py` & `django-aux-0.0.9/django_aux/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,31 @@
 from django.db import models
 from django.core.exceptions import ValidationError
 from django.db.models import Q
-from simple_history.models import HistoricalRecords
-import pandas as pd
 
-class ModelBase(models.Model):
-    class Meta:
-        abstract = True
-    history = HistoricalRecords(related_name='log', inherit=True)
-
-    @classmethod
-    def get_field_names(cls):
-        ''' Return a list of the db field names for objects of this class '''
-        return [f.name for f in cls._meta.get_fields()]
-
-
-class CheckRangeMixin:
-    '''
-        This model mixin adds cleaning functionality to a model that will ensure the value of a ending attr 
-        is greater than the value of a start attr. Default will not let them be equal but can be overwritten
-    '''
-    start_attr = '' # Name of the attr that starts the range (must be overwritten)
-    end_attr = '' # Name of the attr that ends the range (must be overwritten)
-    allow_zero_diff = False
-    clean_during_save = True
-
-    def check_range(self):
-        start = self.cleaned_data.get(f'{self.start_attr}')
-        end = self.cleaned_data.get(f'{self.end_attr}')
-        if self.allow_zero_diff:
-            valid = end >= start
-        else:
-            valid = end > start        
-        if not valid:
-            raise ValidationError(f'{self.end_attr} must be larger than {self.start_attr}')
-
-    def clean(self):
-        cd = super().clean()
-        self.check_range()
-        return cd
-
-    def save(self, *args, **kwargs):
-        if self.clean_during_save:
-            self.clean()
-        super().save(*args,**kwargs)
-
-
-class CheckOverlapMixin(CheckRangeMixin):
+class CheckOverlapMixin:
     ''' 
         This mixin adds cleaning functionality to a model that will not allow a range overlap defined by two attributes.
         default behavior is to include the boundaries, but can be overwritten
     '''
     start_attr = '' # Name of the attr that starts the range (must be overwritten)
     end_attr = '' # Name of the attr that ends the range (must be overwritten)
     extra_filter_attrs = [] # Additional filter attrs to apply before checking for overlap
     include_end_boundary = True
     include_start_boundary = True
     clean_during_save = True
 
+    def clean(self):
+        super().clean()
+        self.check_overlap()
+
+    def save(self, *args, **kwargs):
+        if self.clean_during_save:
+            self.clean()
+        super().save(*args,**kwargs)
 
     def check_overlap(self):
         # Overlapping ranges will always meet BOTH of the following conditions
         # 1.) existing end date is >= new start date
         # 2.) existing start date is <= new end date
         fkwargs= {} # initialize filter kwargs
         #  Get the look ups based on boundary cond settings
@@ -81,17 +45,8 @@
         #No other objects should have met that criteria
         if bad_count > 0:
             msg = f'{self.__class__.__name__} cannot overlap another instance'
             if self.extra_filter_attrs != []:
                 msg = msg + f' with the same {self.extra_filter_attrs}'
             raise ValidationError(
                 msg
-            )
-
-    def clean(self):
-        super().clean()
-        self.check_overlap()
-
-    def save(self, *args, **kwargs):
-        if self.clean_during_save:
-            self.clean()
-        super().save(*args,**kwargs)
+            )
```

### Comparing `django_aux-0.0.82/django_aux/static/css/main.css` & `django-aux-0.0.9/django_aux/static/main.css`

 * *Files identical despite different names*

### Comparing `django_aux-0.0.82/django_aux/templates/django_aux/base.html` & `django-aux-0.0.9/django_aux/templates/django_aux/base.html`

 * *Files 19% similar despite different names*

```diff
@@ -7,23 +7,23 @@
     {% bootstrap_javascript jquery='full' %}
     {% block extrahead %}  {% endblock %}     {# Embeds Extra Resources #}
     <!-- Required meta tags -->
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
     <!-- Bootstrap CSS -->
     <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">
-    <link rel="stylesheet" type="text/css" href="{% static 'example/main.css' %}">
+    <link rel="stylesheet" type="text/css" href="{% static 'django_aux/main.css' %}">
     <title>{% block title %} {% endblock %}</title>
   </head>
 
   <body>
     <div class="container-fluid">
       <nav class="navbar navbar-expand-lg navbar-dark bg-steel fixed-top">
         <a class="navbar-brand" href="{% url 'home' %}">
-          <img src="#"  width="60" class="img-fluid" alt="PUT LOGO HERE">
+          <img src="{% static 'project/logo.jpg' %}"  width="60" class="img-fluid" alt="PUT LOGO HERE">
         </a>
         <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarToggle" aria-controls="navbarToggle" aria-expanded="false" aria-label="Toggle navigation">
           <span class="navbar-toggler-icon"></span>
         </button>
         <div class="collapse navbar-collapse" id="navbarToggle">
           <div class="navbar-nav mr-auto">
             <a class="nav-item nav-link" href="#">Home</a>
@@ -133,60 +133,17 @@
     </script>
     <script>
         // The purose of this script is to retreive the x and y scroll position of a given pathname
         // and scroll the window to it
         function setScroll() {
             var key = window.location.pathname + '_yscroll' // Build the unique key for yscroll
             y = window.sessionStorage.getItem(key) // store in session variables
+            console.log(y, '!!!')
             var key = window.location.pathname + '_xscroll' // Build the unique key for xscroll
             x = window.sessionStorage.getItem(key)
-            setTimeout(function () {
-                window.scrollTo(x, y);
-            }, 200);
+            window.scrollTo(x, y)
         }
         $(document).ready(setScroll)
     </script>
-    <script language="JavaScript">
-        // The purose of this script is to record the class names of each collapsable divs after they are clicked
-        // and store it in sessionStorage
-        function savecollapsestatus(element) {
-            var key = window.location.pathname + '_collapse_states' // build the key from the window path name
-            var dict = window.sessionStorage.getItem(key) // pull the existing dict from sessionStorage 
-            // if that dict did not exist create it, otherwise JSON parse it
-            if (dict == null) {
-                dict = {}
-            } else {
-                dict = JSON.parse(dict)
-            }
-            //  Work out the new classname 
-            var prevclassname = element.className
-            if (prevclassname.includes('show')) {
-                newclassname = prevclassname.replace(' show', '')
-            } else {
-                newclassname = prevclassname + ' show'
-            }
-            dict[element.id] = newclassname // Store the new class name in the dict
-            window.sessionStorage.setItem(key, JSON.stringify(dict)) // Set the new dict in session storage using the key built previously
-        }
-    </script>
-    <script language="JavaScript">
-        // The purose of this script is to resotore the state of collapasable divs upon document loading 
-        function setdivclass() {
-            var key = window.location.pathname + '_collapse_states' // build the key from the path
-            var dict = window.sessionStorage.getItem(key) // pull the existing dict from sessionStorage 
-            // if that dict did not exist create it, otherwise JSON parse it
-            if (dict == null) {
-                dict = {}
-            } else {
-                dict = JSON.parse(dict)
-            }
-            // loop the sub-dictionaries setting the classnames (show or no show)
-            for (var id in dict) {
-                var classname = dict[id];
-                document.getElementById(id).className = classname
-            }
-        }
-        $(document).ready(setdivclass)
-    </script>
     {% block extra_javascript %}{% endblock %}
   </body>
 </html>
```

### Comparing `django_aux-0.0.82/django_aux/templates/django_aux/standard-plotly.html` & `django-aux-0.0.9/django_aux/templates/django_aux/standard.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,34 @@
 {% extends extend_str %}
 {% load crispy_forms_tags %}
 {% load render_table from django_tables2 %}
 {% load querystring from django_tables2 %}
-{% load static %}
 
 {% block content %}
-
-{% if header %}<h1 class="text-center"> {{ header }} </h1>
+{% if header %}<h1> {{ header }} </h1>
 <hr>{% endif %}
-{% if sub_header %}<h2 class="text-center"> {{ sub_header }} </h2>
+{% if sub_header %}<h2> {{ sub_header }} </h2>
 <hr>{% endif %}
 
 {% if form%}
-<h3 class="text-center"> {{ form_header }} </h3>
+<h3> {{ form_header }} </h3>
 {% crispy form %}
 {% endif %}
 {% if filter %}
-<h3 class="text-center"> {{ filter_header }} </h3>
+<h3> {{ filter_header }} </h3>
 <h4> Filter Results </h4>
-<form action="" method="get" enctype="multipart/form-data">
+<form action="" method="get" enctype="multipart/form-data">{% csrf_token %}
     {% crispy filter.form %}
 </form>
 {% endif %}
 {% if agg_table %}
-<h4 class="text-center">{{ agg_table_header }}</h4>
+<h4>{{ agg_table_header }}</h4>
 {% render_table agg_table %}
 {% endif %}
 
-{% if fig %}
-    {{ fig|safe }}
-{% endif %}
-{% if not plot_df.empty %}
-<a class="btn btn-info" data-toggle="collapse" data-target="#pdf" role="button" aria-expanded="true"
-    aria-controls="fe_df">
-    Plot Data Frame
-</a>
-<div class="collapse" id="pdf">
-    <div class="table table-striped table-sm">
-        {{ plot_df.to_html|safe }}
-    </div>
-</div>
-{% endif %}
-
-
 <div class="row">
     {% if export %}
     <button type="button" class="btn">
         <a href="{% querystring '_export'='xlsx' %}">Export Excel (1000 Row Limit)</a>
     </button>
     {% endif %}
     {% if export_csv %}
@@ -71,31 +53,18 @@
     <h5 class='ml-4'><a href="{{ furl2 }}"> {{ furl2_text }} </a></h5>
     {% endif %}
     {% if furl3 %}
     <h5 class='ml-4'><a href="{{ furl3 }}"> {{ furl3_text }} </a></h5>
     {% endif %}
 </div>
 
-{% if submit_buttons %}
-<div class="row">
-    <div id="form_card1" class="card-panel col s12">
-        <form action="output">{% csrf_token %}
-            {% for sb in submit_buttons %}
-            <button class="btn btn-primary" name="{{ sb.name }}" type="submit"> {{ sb.desc }} </button>
-            {% endfor %}
-            {% render_table table %}
-        </form>
-    </div>
-</div>
-{% else %}
 {% if table %}
 <h4>{{ table_header }}</h4>
 {% render_table table %}
 {% endif %}
-{% endif %}
 
 {% if plot1 %}
 <div style="width:1200px;height:100">
     {{ plot1|safe }}
 </div>
 {% endif %}
 
@@ -103,16 +72,8 @@
 <hr>{% endif %}
 {% if object.as_html %}
 {% if show_as_html %}
 {{ object.as_html }}
 {% endif %}
 {% endif %}
 
-{% endblock content %}
-
-
-
-{% block extra_javascript %}
-    {% for ejs in extra_js %}
-        <script src="{% static ejs %}"></script>
-    {% endfor %}
-{% endblock %}
+{% endblock content %}
```

#### html2text {}

```diff
@@ -1,48 +1,40 @@
 {% extends extend_str %} {% load crispy_forms_tags %} {% load render_table from
-django_tables2 %} {% load querystring from django_tables2 %} {% load static %}
-{% block content %} {% if header %}
+django_tables2 %} {% load querystring from django_tables2 %} {% block content
+%} {% if header %}
 ************ {{{{ hheeaaddeerr }}}} ************
 ===============================================================================
 {% endif %} {% if sub_header %}
 ********** {{{{ ssuubb__hheeaaddeerr }}}} **********
 ===============================================================================
 {% endif %} {% if form%}
 ******** {{{{ ffoorrmm__hheeaaddeerr }}}} ********
 {% crispy form %} {% endif %} {% if filter %}
 ******** {{{{ ffiilltteerr__hheeaaddeerr }}}} ********
 ****** FFiilltteerr RReessuullttss ******
-{% crispy filter.form %}
+{% csrf_token %} {% crispy filter.form %}
 {% endif %} {% if agg_table %}
 ****** {{{{ aagggg__ttaabbllee__hheeaaddeerr }}}} ******
-{% render_table agg_table %} {% endif %} {% if fig %} {{ fig|safe }} {% endif
-%} {% if not plot_df.empty %} Plot Data Frame
-{{ plot_df.to_html|safe }}
-{% endif %}
+{% render_table agg_table %} {% endif %}
 {% if export %} _E_x_p_o_r_t_ _E_x_c_e_l_ _(_1_0_0_0_ _R_o_w_ _L_i_m_i_t_) {% endif %} {% if export_csv %}
 _E_x_p_o_r_t_ _C_S_V {% endif %} {% if url1 %}
 **** _{{_{{_ _uu_rr_ll_11____tt_ee_xx_tt_ _}}_}} ****
 {% endif %} {% if url2 %}
 **** _{{_{{_ _uu_rr_ll_22____tt_ee_xx_tt_ _}}_}} ****
 {% endif %} {% if url3 %}
 **** _{{_{{_ _uu_rr_ll_33____tt_ee_xx_tt_ _}}_}} ****
 {% endif %} {% if furl1 %}
 **** _{{_{{_ _ff_uu_rr_ll_11____tt_ee_xx_tt_ _}}_}} ****
 {% endif %} {% if furl2 %}
 **** _{{_{{_ _ff_uu_rr_ll_22____tt_ee_xx_tt_ _}}_}} ****
 {% endif %} {% if furl3 %}
 **** _{{_{{_ _ff_uu_rr_ll_33____tt_ee_xx_tt_ _}}_}} ****
 {% endif %}
-{% if submit_buttons %}
-{% csrf_token %} {% for sb in submit_buttons %} {{ sb.desc }} {% endfor %} {%
-render_table table %}
-{% else %} {% if table %}
+{% if table %}
 ****** {{{{ ttaabbllee__hheeaaddeerr }}}} ******
-{% render_table table %} {% endif %} {% endif %} {% if plot1 %}
+{% render_table table %} {% endif %} {% if plot1 %}
 {{ plot1|safe }}
 {% endif %} {% if detail_header %}
 ********** {{{{ ddeettaaiill__hheeaaddeerr }}}} **********
 ===============================================================================
 {% endif %} {% if object.as_html %} {% if show_as_html %} {{ object.as_html }}
-{% endif %} {% endif %} {% endblock content %} {% block extra_javascript %} {%
-for ejs in extra_js %}
-{% endfor %} {% endblock %}
+{% endif %} {% endif %} {% endblock content %}
```

