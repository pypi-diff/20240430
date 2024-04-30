# Comparing `tmp/django_aux-0.0.84.tar.gz` & `tmp/django-aux-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_aux-0.0.84.tar", last modified: Tue Apr 30 21:18:37 2024, max compression
+gzip compressed data, was "django-aux-0.0.9.tar", last modified: Wed Jul  6 13:38:58 2022, max compression
```

## Comparing `django_aux-0.0.84.tar` & `django-aux-0.0.9.tar`

### file list

```diff
@@ -1,97 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 21:18:37.200132 django_aux-0.0.84/
--rw-rw-rw-   0        0        0     1090 2022-07-05 14:54:23.000000 django_aux-0.0.84/LICENSE
--rw-rw-rw-   0        0        0      143 2022-07-05 21:15:46.000000 django_aux-0.0.84/MANIFEST.in
--rw-rw-rw-   0        0        0     1510 2024-04-30 21:18:37.199126 django_aux-0.0.84/PKG-INFO
--rw-rw-rw-   0        0        0      112 2022-07-05 14:54:23.000000 django_aux-0.0.84/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 21:18:37.113604 django_aux-0.0.84/django_aux/
--rw-rw-rw-   0        0        0        0 2022-07-04 12:21:58.000000 django_aux-0.0.84/django_aux/__init__.py
--rw-rw-rw-   0        0        0       66 2022-07-04 12:21:58.000000 django_aux-0.0.84/django_aux/admin.py
--rw-rw-rw-   0        0        0      157 2022-07-04 12:21:58.000000 django_aux-0.0.84/django_aux/apps.py
--rw-rw-rw-   0        0        0    28535 2024-04-30 16:08:02.000000 django_aux-0.0.84/django_aux/columns.py
--rw-rw-rw-   0        0        0      389 2022-07-06 13:07:44.000000 django_aux-0.0.84/django_aux/decorators.py
--rw-rw-rw-   0        0        0     1552 2022-09-01 02:47:31.000000 django_aux-0.0.84/django_aux/factory.py
--rw-rw-rw-   0        0        0     3904 2022-09-13 12:43:13.000000 django_aux-0.0.84/django_aux/filters.py
--rw-rw-rw-   0        0        0     1434 2023-01-20 18:49:39.000000 django_aux-0.0.84/django_aux/forms.py
--rw-rw-rw-   0        0        0      862 2022-08-26 02:14:36.000000 django_aux-0.0.84/django_aux/middleware.py
-drwxrwxrwx   0        0        0        0 2024-04-30 21:18:37.132608 django_aux-0.0.84/django_aux/migrations/
--rw-rw-rw-   0        0        0        0 2022-07-04 12:21:58.000000 django_aux-0.0.84/django_aux/migrations/__init__.py
--rw-rw-rw-   0        0        0     3914 2023-01-27 14:47:42.000000 django_aux-0.0.84/django_aux/models.py
-drwxrwxrwx   0        0        0        0 2024-04-30 21:18:37.088604 django_aux-0.0.84/django_aux/static/
-drwxrwxrwx   0        0        0        0 2024-04-30 21:18:37.133605 django_aux-0.0.84/django_aux/static/css/
--rw-rw-rw-   0        0        0     2647 2022-07-04 12:21:58.000000 django_aux-0.0.84/django_aux/static/css/main.css
-drwxrwxrwx   0        0        0        0 2024-04-30 21:18:37.137605 django_aux-0.0.84/django_aux/static/js/
--rw-rw-rw-   0        0        0     1739 2022-07-26 11:25:34.000000 django_aux-0.0.84/django_aux/static/js/save_set_collapse_status.js
--rw-rw-rw-   0        0        0     1130 2022-07-26 11:23:45.000000 django_aux-0.0.84/django_aux/static/js/save_set_scroll_pos.js
--rw-rw-rw-   0        0        0       13 2023-01-21 18:59:16.000000 django_aux-0.0.84/django_aux/static/js/show_hide_remove_btn.js
-drwxrwxrwx   0        0        0        0 2024-04-30 21:18:37.089606 django_aux-0.0.84/django_aux/templates/
-drwxrwxrwx   0        0        0        0 2024-04-30 21:18:37.150606 django_aux-0.0.84/django_aux/templates/django_aux/
--rw-rw-rw-   0        0        0     9486 2022-12-27 18:33:09.000000 django_aux-0.0.84/django_aux/templates/django_aux/base.html
--rw-rw-rw-   0        0        0      906 2022-12-31 11:46:39.000000 django_aux-0.0.84/django_aux/templates/django_aux/checkbox-table.html
--rw-rw-rw-   0        0        0     1126 2022-12-31 11:46:42.000000 django_aux-0.0.84/django_aux/templates/django_aux/dash-filter.html
--rw-rw-rw-   0        0        0      937 2023-01-03 18:06:33.000000 django_aux-0.0.84/django_aux/templates/django_aux/delete.html
--rw-rw-rw-   0        0        0     2368 2023-01-03 20:28:05.000000 django_aux-0.0.84/django_aux/templates/django_aux/form-table.html
--rw-rw-rw-   0        0        0     2293 2023-01-21 18:57:29.000000 django_aux-0.0.84/django_aux/templates/django_aux/inline-formset.html
--rw-rw-rw-   0        0        0      546 2023-01-27 16:09:55.000000 django_aux-0.0.84/django_aux/templates/django_aux/login.html
--rw-rw-rw-   0        0        0      326 2023-01-27 16:10:37.000000 django_aux-0.0.84/django_aux/templates/django_aux/logout.html
--rw-rw-rw-   0        0        0     3145 2022-12-31 11:46:56.000000 django_aux-0.0.84/django_aux/templates/django_aux/standard-plotly.html
--rw-rw-rw-   0        0        0     2849 2023-01-07 15:57:40.000000 django_aux-0.0.84/django_aux/templates/django_aux/standard.html
-drwxrwxrwx   0        0        0        0 2024-04-30 21:18:37.152606 django_aux-0.0.84/django_aux/templatetags/
--rw-rw-rw-   0        0        0        0 2022-07-04 12:21:58.000000 django_aux-0.0.84/django_aux/templatetags/__init__.py
--rw-rw-rw-   0        0        0      996 2023-01-03 17:43:59.000000 django_aux-0.0.84/django_aux/templatetags/aux_tags.py
--rw-rw-rw-   0        0        0      303 2022-08-07 17:31:57.000000 django_aux-0.0.84/django_aux/urls.py
--rw-rw-rw-   0        0        0     4905 2024-04-30 21:18:07.000000 django_aux-0.0.84/django_aux/utils.py
--rw-rw-rw-   0        0        0    27257 2023-11-12 14:20:43.000000 django_aux-0.0.84/django_aux/views.py
-drwxrwxrwx   0        0        0        0 2024-04-30 21:18:37.198128 django_aux-0.0.84/django_aux.egg-info/
--rw-rw-rw-   0        0        0     1510 2024-04-30 21:18:37.000000 django_aux-0.0.84/django_aux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2327 2024-04-30 21:18:37.000000 django_aux-0.0.84/django_aux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 21:18:37.000000 django_aux-0.0.84/django_aux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      228 2024-04-30 21:18:37.000000 django_aux-0.0.84/django_aux.egg-info/requires.txt
--rw-rw-rw-   0        0        0       74 2024-04-30 21:18:37.000000 django_aux-0.0.84/django_aux.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-30 21:18:37.158609 django_aux-0.0.84/django_aux_geo/
--rw-rw-rw-   0        0        0        0 2022-07-04 12:21:58.000000 django_aux-0.0.84/django_aux_geo/__init__.py
--rw-rw-rw-   0        0        0      164 2022-09-16 16:32:11.000000 django_aux-0.0.84/django_aux_geo/apps.py
--rw-rw-rw-   0        0        0      825 2023-12-15 18:18:19.000000 django_aux-0.0.84/django_aux_geo/filters.py
-drwxrwxrwx   0        0        0        0 2024-04-30 21:18:37.161614 django_aux-0.0.84/django_aux_geo/migrations/
--rw-rw-rw-   0        0        0     1393 2023-03-03 14:03:19.000000 django_aux-0.0.84/django_aux_geo/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     2761 2024-02-20 16:34:02.000000 django_aux-0.0.84/django_aux_geo/migrations/0002_address_coordinate_coordinate_unique_coord_and_more.py
--rw-rw-rw-   0        0        0        0 2022-07-04 12:21:58.000000 django_aux-0.0.84/django_aux_geo/migrations/__init__.py
--rw-rw-rw-   0        0        0     5534 2023-12-15 18:06:15.000000 django_aux-0.0.84/django_aux_geo/models.py
--rw-rw-rw-   0        0        0      397 2023-12-15 18:20:05.000000 django_aux-0.0.84/django_aux_geo/tables.py
-drwxrwxrwx   0        0        0        0 2024-04-30 21:18:37.168614 django_aux-0.0.84/django_aux_request/
--rw-rw-rw-   0        0        0        0 2022-07-04 12:21:58.000000 django_aux-0.0.84/django_aux_request/__init__.py
--rw-rw-rw-   0        0        0      172 2023-01-07 16:03:12.000000 django_aux-0.0.84/django_aux_request/apps.py
--rw-rw-rw-   0        0        0     1719 2023-01-07 16:12:42.000000 django_aux-0.0.84/django_aux_request/filters.py
--rw-rw-rw-   0        0        0      251 2023-01-07 16:10:24.000000 django_aux-0.0.84/django_aux_request/tables.py
--rw-rw-rw-   0        0        0      303 2022-08-07 17:31:57.000000 django_aux-0.0.84/django_aux_request/urls.py
--rw-rw-rw-   0        0        0    26226 2023-01-02 22:57:03.000000 django_aux-0.0.84/django_aux_request/views.py
-drwxrwxrwx   0        0        0        0 2024-04-30 21:18:37.174121 django_aux-0.0.84/django_aux_timeperiods/
--rw-rw-rw-   0        0        0        0 2022-07-04 12:21:58.000000 django_aux-0.0.84/django_aux_timeperiods/__init__.py
--rw-rw-rw-   0        0        0       66 2022-07-04 12:21:58.000000 django_aux-0.0.84/django_aux_timeperiods/admin.py
--rw-rw-rw-   0        0        0      179 2022-09-16 15:30:26.000000 django_aux-0.0.84/django_aux_timeperiods/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-30 21:18:37.176128 django_aux-0.0.84/django_aux_timeperiods/migrations/
--rw-rw-rw-   0        0        0     4256 2023-03-03 14:03:19.000000 django_aux-0.0.84/django_aux_timeperiods/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2022-07-04 12:21:58.000000 django_aux-0.0.84/django_aux_timeperiods/migrations/__init__.py
--rw-rw-rw-   0        0        0     9126 2023-03-03 13:47:33.000000 django_aux-0.0.84/django_aux_timeperiods/models.py
-drwxrwxrwx   0        0        0        0 2024-04-30 21:18:37.093605 django_aux-0.0.84/docs/
-drwxrwxrwx   0        0        0        0 2024-04-30 21:18:37.183127 django_aux-0.0.84/docs/source/
--rw-rw-rw-   0        0        0       39 2022-08-28 17:51:16.000000 django_aux-0.0.84/docs/source/conf.py
--rw-rw-rw-   0        0        0      198 2022-08-28 17:45:17.000000 django_aux-0.0.84/docs/source/django_aux.migrations.rst
--rw-rw-rw-   0        0        0     1964 2022-08-28 17:45:17.000000 django_aux-0.0.84/docs/source/django_aux.rst
--rw-rw-rw-   0        0        0      427 2022-08-28 17:45:17.000000 django_aux-0.0.84/docs/source/django_aux.templatetags.rst
--rw-rw-rw-   0        0        0       84 2022-08-28 17:45:17.000000 django_aux-0.0.84/docs/source/modules.rst
--rw-rw-rw-   0        0        0      110 2022-08-28 17:45:17.000000 django_aux-0.0.84/docs/source/setup.rst
--rw-rw-rw-   0        0        0     1247 2024-04-30 21:18:37.202124 django_aux-0.0.84/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-30 17:00:19.000000 django_aux-0.0.84/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 21:18:37.197124 django_aux-0.0.84/tests/
--rw-rw-rw-   0        0        0        0 2022-09-25 11:28:52.000000 django_aux-0.0.84/tests/__init__.py
--rw-rw-rw-   0        0        0      742 2022-10-07 18:01:20.000000 django_aux-0.0.84/tests/filters.py
--rw-rw-rw-   0        0        0      420 2022-12-27 18:48:54.000000 django_aux-0.0.84/tests/forms.py
--rw-rw-rw-   0        0        0     2139 2022-10-07 17:48:51.000000 django_aux-0.0.84/tests/models.py
--rw-rw-rw-   0        0        0      237 2022-10-07 17:55:49.000000 django_aux-0.0.84/tests/tables.py
--rw-rw-rw-   0        0        0     9194 2023-01-22 13:55:18.000000 django_aux-0.0.84/tests/test_daux.py
--rw-rw-rw-   0        0        0      378 2022-10-08 17:40:33.000000 django_aux-0.0.84/tests/test_daux_geo.py
--rw-rw-rw-   0        0        0     5229 2022-11-27 18:54:06.000000 django_aux-0.0.84/tests/test_daux_timeperiods.py
--rw-rw-rw-   0        0        0     1975 2022-10-07 18:35:22.000000 django_aux-0.0.84/tests/test_settings.py
--rw-rw-rw-   0        0        0      323 2022-12-27 18:44:17.000000 django_aux-0.0.84/tests/urls.py
--rw-rw-rw-   0        0        0      564 2023-01-22 13:44:26.000000 django_aux-0.0.84/tests/utils.py
--rw-rw-rw-   0        0        0      791 2022-12-27 19:29:08.000000 django_aux-0.0.84/tests/views.py
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

### Comparing `django_aux-0.0.84/LICENSE` & `django-aux-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django_aux-0.0.84/django_aux/filters.py` & `django-aux-0.0.9/django_aux/filters.py`

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

### Comparing `django_aux-0.0.84/django_aux/models.py` & `django-aux-0.0.9/django_aux/models.py`

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

### Comparing `django_aux-0.0.84/django_aux/static/css/main.css` & `django-aux-0.0.9/django_aux/static/main.css`

 * *Files identical despite different names*

### Comparing `django_aux-0.0.84/django_aux/templates/django_aux/base.html` & `django-aux-0.0.9/django_aux/templates/django_aux/base.html`

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

### Comparing `django_aux-0.0.84/django_aux/templates/django_aux/standard-plotly.html` & `django-aux-0.0.9/django_aux/templates/django_aux/standard.html`

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

### Comparing `django_aux-0.0.84/django_aux/templatetags/aux_tags.py` & `django-aux-0.0.9/django_aux/templatetags/aux_tags.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,19 +15,7 @@
     return True if table.rows.__len__() > 0 else False
 
 
 @register.filter
 def has_items(container):
     ''' A custom template tag that takes an iterable returns true if len > 0 '''
     return True if len(container) > 0 else False
-
-@register.filter
-def render_class_name(obj):
-    ''' A custom template tag that returns the object's class' name '''
-    return obj.__class__.__name__
-
-
-
-@register.filter(name='null_default')
-def null_default(val, default):
-    ''' A custom template tag that will return a default if val is null '''
-    return val if val else str(default)
```

### Comparing `django_aux-0.0.84/setup.cfg` & `django-aux-0.0.9/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,75 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 6175 780d 0a76   = django-aux..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e38 340d  ersion = 0.0.84.
-00000030: 0a64 6573 6372 6970 7469 6f6e 203d 2055  .description = U
-00000040: 7365 6675 6c20 4d69 7869 6e73 2066 6f72  seful Mixins for
-00000050: 2044 6a61 6e67 6f20 5072 6f6a 6563 7473   Django Projects
-00000060: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
-00000070: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
-00000080: 452e 6d64 0d0a 7572 6c20 3d20 6874 7470  E.md..url = http
-00000090: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4a  s://github.com/J
-000000a0: 6f72 6461 6e48 7961 7474 2f64 6a61 6e67  ordanHyatt/djang
-000000b0: 6f2d 6175 780d 0a61 7574 686f 7220 3d20  o-aux..author = 
-000000c0: 4a6f 7264 616e 2048 7961 7474 0d0a 6175  Jordan Hyatt..au
-000000d0: 7468 6f72 5f65 6d61 696c 203d 206a 6f72  thor_email = jor
-000000e0: 6461 6e2e 6879 6174 7440 6175 7869 6c69  dan.hyatt@auxili
-000000f0: 6173 7973 7465 6d73 2e63 6f6d 0d0a 6c69  asystems.com..li
-00000100: 6365 6e73 6520 3d20 4d49 5420 2023 2045  cense = MIT  # E
-00000110: 7861 6d70 6c65 206c 6963 656e 7365 0d0a  xample license..
-00000120: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
-00000130: 0945 6e76 6972 6f6e 6d65 6e74 203a 3a20  .Environment :: 
-00000140: 5765 6220 456e 7669 726f 6e6d 656e 740d  Web Environment.
-00000150: 0a09 4672 616d 6577 6f72 6b20 3a3a 2044  ..Framework :: D
-00000160: 6a61 6e67 6f0d 0a09 4672 616d 6577 6f72  jango...Framewor
-00000170: 6b20 3a3a 2044 6a61 6e67 6f20 3a3a 2034  k :: Django :: 4
-00000180: 2e30 0d0a 0949 6e74 656e 6465 6420 4175  .0...Intended Au
-00000190: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
-000001a0: 7065 7273 0d0a 094c 6963 656e 7365 203a  pers...License :
-000001b0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-000001c0: 3a20 4d49 5420 4c69 6365 6e73 650d 0a09  : MIT License...
-000001d0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-000001e0: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-000001f0: 6e74 0d0a 0950 726f 6772 616d 6d69 6e67  nt...Programming
-00000200: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000210: 686f 6e0d 0a09 5072 6f67 7261 6d6d 696e  hon...Programmin
-00000220: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000230: 7468 6f6e 203a 3a20 330d 0a09 5072 6f67  thon :: 3...Prog
-00000240: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000250: 203a 3a20 5079 7468 6f6e 203a 3a20 3320   :: Python :: 3 
-00000260: 3a3a 204f 6e6c 790d 0a09 5072 6f67 7261  :: Only...Progra
-00000270: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000280: 3a20 5079 7468 6f6e 203a 3a20 332e 380d  : Python :: 3.8.
-00000290: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000002a0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000002b0: 203a 3a20 332e 390d 0a09 5072 6f67 7261   :: 3.9...Progra
-000002c0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000002d0: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
-000002e0: 0d0a 0954 6f70 6963 203a 3a20 496e 7465  ...Topic :: Inte
-000002f0: 726e 6574 203a 3a20 5757 572f 4854 5450  rnet :: WWW/HTTP
-00000300: 0d0a 0954 6f70 6963 203a 3a20 496e 7465  ...Topic :: Inte
-00000310: 726e 6574 203a 3a20 5757 572f 4854 5450  rnet :: WWW/HTTP
-00000320: 203a 3a20 4479 6e61 6d69 6320 436f 6e74   :: Dynamic Cont
-00000330: 656e 740d 0a0d 0a5b 6f70 7469 6f6e 735d  ent....[options]
-00000340: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
-00000350: 655f 6461 7461 203d 2074 7275 650d 0a70  e_data = true..p
-00000360: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
-00000370: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-00000380: 203d 203e 3d33 2e36 0d0a 696e 7374 616c   = >=3.6..instal
-00000390: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
-000003a0: 446a 616e 676f 203e 3d20 332e 300d 0a09  Django >= 3.0...
-000003b0: 646a 616e 676f 2d74 6162 6c65 7332 203e  django-tables2 >
-000003c0: 3d20 322e 300d 0a09 646a 616e 676f 2d66  = 2.0...django-f
-000003d0: 696c 7465 7220 3e3d 2032 312e 300d 0a09  ilter >= 21.0...
-000003e0: 7061 6e64 6173 203e 3d20 322e 300d 0a09  pandas >= 2.0...
-000003f0: 6e75 6d70 7920 3e3d 2031 2e32 300d 0a09  numpy >= 1.20...
-00000400: 646a 616e 676f 2d62 6f6f 7473 7472 6170  django-bootstrap
-00000410: 2d64 6174 6570 6963 6b65 722d 706c 7573  -datepicker-plus
-00000420: 203e 3d20 332e 300d 0a09 646a 616e 676f   >= 3.0...django
-00000430: 2d63 7269 7370 792d 666f 726d 7320 3e3d  -crispy-forms >=
-00000440: 2031 2e31 342e 300d 0a09 646a 616e 676f   1.14.0...django
-00000450: 2d62 6f6f 7473 7472 6170 3420 3e3d 2032  -bootstrap4 >= 2
-00000460: 312e 300d 0a09 646a 616e 676f 2d70 616e  1.0...django-pan
-00000470: 6461 7320 3e3d 2030 2e36 0d0a 0970 6c6f  das >= 0.6...plo
-00000480: 746c 7920 3e3d 2035 2e30 0d0a 0966 6163  tly >= 5.0...fac
-00000490: 746f 7279 5f62 6f79 203e 3d20 332e 322e  tory_boy >= 3.2.
-000004a0: 310d 0a09 6c78 6d6c 203e 3d20 342e 302e  1...lxml >= 4.0.
-000004b0: 300d 0a0d 0a5b 6567 675f 696e 666f 5d0d  0....[egg_info].
-000004c0: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-000004d0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e39 0d0a  ersion = 0.0.9..
+00000030: 6465 7363 7269 7074 696f 6e20 3d20 5573  description = Us
+00000040: 6566 756c 204d 6978 696e 7320 666f 7220  eful Mixins for 
+00000050: 446a 616e 676f 2050 726f 6a65 6374 730d  Django Projects.
+00000060: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+00000070: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
+00000080: 2e6d 640d 0a75 726c 203d 2068 7474 7073  .md..url = https
+00000090: 3a2f 2f67 6974 6875 622e 636f 6d2f 4a6f  ://github.com/Jo
+000000a0: 7264 616e 4879 6174 740d 0a61 7574 686f  rdanHyatt..autho
+000000b0: 7220 3d20 4a6f 7264 616e 2048 7961 7474  r = Jordan Hyatt
+000000c0: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
+000000d0: 206a 6f72 6461 6e2e 6879 6174 7440 6175   jordan.hyatt@au
+000000e0: 7869 6c69 6173 7973 7465 6d73 2e63 6f6d  xiliasystems.com
+000000f0: 0d0a 6c69 6365 6e73 6520 3d20 4d49 5420  ..license = MIT 
+00000100: 2023 2045 7861 6d70 6c65 206c 6963 656e   # Example licen
+00000110: 7365 0d0a 636c 6173 7369 6669 6572 7320  se..classifiers 
+00000120: 3d20 0d0a 0945 6e76 6972 6f6e 6d65 6e74  = ...Environment
+00000130: 203a 3a20 5765 6220 456e 7669 726f 6e6d   :: Web Environm
+00000140: 656e 740d 0a09 4672 616d 6577 6f72 6b20  ent...Framework 
+00000150: 3a3a 2044 6a61 6e67 6f0d 0a09 4672 616d  :: Django...Fram
+00000160: 6577 6f72 6b20 3a3a 2044 6a61 6e67 6f20  ework :: Django 
+00000170: 3a3a 2034 2e30 0d0a 0949 6e74 656e 6465  :: 4.0...Intende
+00000180: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
+00000190: 7665 6c6f 7065 7273 0d0a 094c 6963 656e  velopers...Licen
+000001a0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+000001b0: 6564 203a 3a20 4253 4420 4c69 6365 6e73  ed :: BSD Licens
+000001c0: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
+000001d0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+000001e0: 656e 6465 6e74 0d0a 0950 726f 6772 616d  endent...Program
+000001f0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000200: 2050 7974 686f 6e0d 0a09 5072 6f67 7261   Python...Progra
+00000210: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000220: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
+00000230: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000240: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000250: 3a20 3320 3a3a 204f 6e6c 790d 0a09 5072  : 3 :: Only...Pr
+00000260: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000270: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000280: 332e 380d 0a09 5072 6f67 7261 6d6d 696e  3.8...Programmin
+00000290: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000002a0: 7468 6f6e 203a 3a20 332e 390d 0a09 5072  thon :: 3.9...Pr
+000002b0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000002c0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000002d0: 332e 3130 0d0a 0954 6f70 6963 203a 3a20  3.10...Topic :: 
+000002e0: 496e 7465 726e 6574 203a 3a20 5757 572f  Internet :: WWW/
+000002f0: 4854 5450 0d0a 0954 6f70 6963 203a 3a20  HTTP...Topic :: 
+00000300: 496e 7465 726e 6574 203a 3a20 5757 572f  Internet :: WWW/
+00000310: 4854 5450 203a 3a20 4479 6e61 6d69 6320  HTTP :: Dynamic 
+00000320: 436f 6e74 656e 740d 0a0d 0a5b 6f70 7469  Content....[opti
+00000330: 6f6e 735d 0d0a 696e 636c 7564 655f 7061  ons]..include_pa
+00000340: 636b 6167 655f 6461 7461 203d 2074 7275  ckage_data = tru
+00000350: 650d 0a70 6163 6b61 6765 7320 3d20 6669  e..packages = fi
+00000360: 6e64 3a0d 0a70 7974 686f 6e5f 7265 7175  nd:..python_requ
+00000370: 6972 6573 203d 203e 3d33 2e36 0d0a 696e  ires = >=3.6..in
+00000380: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
+00000390: 200d 0a09 446a 616e 676f 203e 3d20 332e   ...Django >= 3.
+000003a0: 300d 0a09 646a 616e 676f 2d74 6162 6c65  0...django-table
+000003b0: 7332 203e 3d20 322e 300d 0a09 646a 616e  s2 >= 2.0...djan
+000003c0: 676f 2d66 696c 7465 7220 3e3d 2032 312e  go-filter >= 21.
+000003d0: 300d 0a09 7061 6e64 6173 203e 3d20 312e  0...pandas >= 1.
+000003e0: 300d 0a09 6e75 6d70 7920 3e3d 2031 2e32  0...numpy >= 1.2
+000003f0: 300d 0a09 646a 616e 676f 2d62 6f6f 7473  0...django-boots
+00000400: 7472 6170 2d64 6174 6570 6963 6b65 722d  trap-datepicker-
+00000410: 706c 7573 203e 3d20 332e 300d 0a09 646a  plus >= 3.0...dj
+00000420: 616e 676f 2d63 7269 7370 792d 666f 726d  ango-crispy-form
+00000430: 7320 3e3d 2031 2e31 342e 300d 0a09 646a  s >= 1.14.0...dj
+00000440: 616e 676f 2d62 6f6f 7473 7472 6170 3420  ango-bootstrap4 
+00000450: 3e3d 2032 312e 300d 0a09 646a 616e 676f  >= 21.0...django
+00000460: 2d70 616e 6461 7320 3e3d 2030 2e36 0d0a  -pandas >= 0.6..
+00000470: 0970 6c6f 746c 7920 3e3d 2035 2e30 0d0a  .plotly >= 5.0..
+00000480: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000490: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+000004a0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

