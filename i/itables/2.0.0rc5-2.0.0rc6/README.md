# Comparing `tmp/itables-2.0.0rc5.tar.gz` & `tmp/itables-2.0.0rc6.tar.gz`

## Comparing `itables-2.0.0rc5.tar` & `itables-2.0.0rc6.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 itables-2.0.0rc5/.pre-commit-config.yaml
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 itables-2.0.0rc5/.pylintrc
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 itables-2.0.0rc5/codecov.yml
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 itables-2.0.0rc5/environment.yml
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 itables-2.0.0rc5/.github/workflows/continuous-integration.yml
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 itables-2.0.0rc5/.github/workflows/publish-book.yml
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 itables-2.0.0rc5/.github/workflows/publish.yml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 itables-2.0.0rc5/binder/postBuild
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 itables-2.0.0rc5/binder/requirements.txt
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 itables-2.0.0rc5/binder/labconfig/default_setting_overrides.json
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/_config.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/_toc.yml
--rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/advanced_parameters.md
--rw-r--r--   0        0        0    16798 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/changelog.md
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/contributing.md
--rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/custom_css.md
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/custom_extensions.md
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/developing.md
--rw-r--r--   0        0        0    46135 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/df_example.png
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/downsampling.md
--rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/extensions.md
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/formatting.md
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/pandas_style.md
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/polars_dataframes.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/quarto.md
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/quick_start.md
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/references.md
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/sample_dataframes.md
--rw-r--r--   0        0        0    51851 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/show_df.png
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/supported_editors.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/troubleshooting.md
--rw-r--r--   0        0        0    83555 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/images/code.png
--rw-r--r--   0        0        0    98830 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/images/colab.png
--rw-r--r--   0        0        0   110756 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/images/html.png
--rw-r--r--   0        0        0   108275 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/images/lab.png
--rw-r--r--   0        0        0   129198 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/images/notebook.png
--rw-r--r--   0        0        0   107743 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/images/pycharm.png
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/quarto/quarto_html.qmd
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 itables-2.0.0rc5/docs/quarto/quarto_revealjs.qmd
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/__init__.py
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/datatables_format.py
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/downsample.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/interactive.py
--rw-r--r--   0        0        0    22711 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/javascript.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/options.py
--rw-r--r--   0        0        0    13910 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/sample_dfs.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/shiny.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/utils.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/version.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/dt_for_itables/LICENSE
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/dt_for_itables/README.md
--rw-r--r--   0        0        0    68898 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/dt_for_itables/dt_bundle.css
--rw-r--r--   0        0        0   506028 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/dt_for_itables/dt_bundle.js
--rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/dt_for_itables/package-lock.json
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/dt_for_itables/package.json
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/dt_for_itables/src.js
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/html/datatables_template.html
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/html/column_filters/initComplete.js
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/html/column_filters/pre_dt_code.js
--rw-r--r--   0        0        0    31715 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/samples/countries.csv
--rw-r--r--   0        0        0   420013 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/samples/indicators.csv
--rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 itables-2.0.0rc5/itables/samples/population.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itables-2.0.0rc5/tests/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 itables-2.0.0rc5/tests/conftest.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 itables-2.0.0rc5/tests/test_changelog.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 itables-2.0.0rc5/tests/test_connected_notebook_is_small.py
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 itables-2.0.0rc5/tests/test_datatables_format.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 itables-2.0.0rc5/tests/test_documentation_notebooks_run.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 itables-2.0.0rc5/tests/test_downsample.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 itables-2.0.0rc5/tests/test_html_in_table_header.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 itables-2.0.0rc5/tests/test_init.py
--rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 itables-2.0.0rc5/tests/test_javascript.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 itables-2.0.0rc5/tests/test_json_dumps.py
--rw-r--r--   0        0        0   791362 2020-02-02 00:00:00.000000 itables-2.0.0rc5/tests/test_notebook.ipynb
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 itables-2.0.0rc5/tests/test_polars.py
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 itables-2.0.0rc5/tests/test_sample_dfs.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 itables-2.0.0rc5/tests/test_sample_python_apps.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 itables-2.0.0rc5/tests/test_update_samples.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 itables-2.0.0rc5/tests/sample_python_apps/itables_in_a_shiny_app.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 itables-2.0.0rc5/tests/sample_python_apps/itables_in_a_shiny_app_with_tabs.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 itables-2.0.0rc5/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 itables-2.0.0rc5/LICENSE
--rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 itables-2.0.0rc5/README.md
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 itables-2.0.0rc5/pyproject.toml
--rw-r--r--   0        0        0     6834 2020-02-02 00:00:00.000000 itables-2.0.0rc5/PKG-INFO
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 itables-2.0.0rc6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 itables-2.0.0rc6/.pylintrc
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 itables-2.0.0rc6/codecov.yml
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 itables-2.0.0rc6/environment.yml
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 itables-2.0.0rc6/.github/workflows/continuous-integration.yml
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 itables-2.0.0rc6/.github/workflows/publish-book.yml
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 itables-2.0.0rc6/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 itables-2.0.0rc6/binder/postBuild
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 itables-2.0.0rc6/binder/requirements.txt
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 itables-2.0.0rc6/binder/labconfig/default_setting_overrides.json
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/_config.yml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/_toc.yml
+-rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/advanced_parameters.md
+-rw-r--r--   0        0        0    16798 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/changelog.md
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/contributing.md
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/custom_css.md
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/custom_extensions.md
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/developing.md
+-rw-r--r--   0        0        0    46135 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/df_example.png
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/downsampling.md
+-rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/extensions.md
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/formatting.md
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/pandas_style.md
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/polars_dataframes.md
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/quarto.md
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/quick_start.md
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/references.md
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/sample_dataframes.md
+-rw-r--r--   0        0        0    51851 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/show_df.png
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/supported_editors.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/troubleshooting.md
+-rw-r--r--   0        0        0    83555 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/images/code.png
+-rw-r--r--   0        0        0    98830 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/images/colab.png
+-rw-r--r--   0        0        0   110756 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/images/html.png
+-rw-r--r--   0        0        0   108275 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/images/lab.png
+-rw-r--r--   0        0        0   129198 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/images/notebook.png
+-rw-r--r--   0        0        0   107743 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/images/pycharm.png
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/quarto/quarto_html.qmd
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 itables-2.0.0rc6/docs/quarto/quarto_revealjs.qmd
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/__init__.py
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/datatables_format.py
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/downsample.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/interactive.py
+-rw-r--r--   0        0        0    22588 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/javascript.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/options.py
+-rw-r--r--   0        0        0    13910 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/sample_dfs.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/shiny.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/utils.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/version.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/dt_for_itables/LICENSE
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/dt_for_itables/README.md
+-rw-r--r--   0        0        0    68898 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/dt_for_itables/dt_bundle.css
+-rw-r--r--   0        0        0   506028 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/dt_for_itables/dt_bundle.js
+-rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/dt_for_itables/package-lock.json
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/dt_for_itables/package.json
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/dt_for_itables/src.js
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/html/datatables_template.html
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/html/column_filters/initComplete.js
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/html/column_filters/pre_dt_code.js
+-rw-r--r--   0        0        0    31715 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/samples/countries.csv
+-rw-r--r--   0        0        0   420013 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/samples/indicators.csv
+-rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 itables-2.0.0rc6/itables/samples/population.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itables-2.0.0rc6/tests/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 itables-2.0.0rc6/tests/conftest.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 itables-2.0.0rc6/tests/test_changelog.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 itables-2.0.0rc6/tests/test_connected_notebook_is_small.py
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 itables-2.0.0rc6/tests/test_datatables_format.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 itables-2.0.0rc6/tests/test_documentation_notebooks_run.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 itables-2.0.0rc6/tests/test_downsample.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 itables-2.0.0rc6/tests/test_html_in_table_header.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 itables-2.0.0rc6/tests/test_init.py
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 itables-2.0.0rc6/tests/test_javascript.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 itables-2.0.0rc6/tests/test_json_dumps.py
+-rw-r--r--   0        0        0   791362 2020-02-02 00:00:00.000000 itables-2.0.0rc6/tests/test_notebook.ipynb
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 itables-2.0.0rc6/tests/test_polars.py
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 itables-2.0.0rc6/tests/test_sample_dfs.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 itables-2.0.0rc6/tests/test_sample_python_apps.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 itables-2.0.0rc6/tests/test_update_samples.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 itables-2.0.0rc6/tests/sample_python_apps/itables_in_a_shiny_app.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 itables-2.0.0rc6/tests/sample_python_apps/itables_in_a_shiny_app_with_tabs.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 itables-2.0.0rc6/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 itables-2.0.0rc6/LICENSE
+-rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 itables-2.0.0rc6/README.md
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 itables-2.0.0rc6/pyproject.toml
+-rw-r--r--   0        0        0     6834 2020-02-02 00:00:00.000000 itables-2.0.0rc6/PKG-INFO
```

### Comparing `itables-2.0.0rc5/.pre-commit-config.yaml` & `itables-2.0.0rc6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/.github/workflows/continuous-integration.yml` & `itables-2.0.0rc6/.github/workflows/continuous-integration.yml`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/.github/workflows/publish-book.yml` & `itables-2.0.0rc6/.github/workflows/publish-book.yml`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/.github/workflows/publish.yml` & `itables-2.0.0rc6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/_toc.yml` & `itables-2.0.0rc6/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/advanced_parameters.md` & `itables-2.0.0rc6/docs/advanced_parameters.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/changelog.md` & `itables-2.0.0rc6/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/contributing.md` & `itables-2.0.0rc6/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/custom_css.md` & `itables-2.0.0rc6/docs/custom_css.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/custom_extensions.md` & `itables-2.0.0rc6/docs/custom_extensions.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/developing.md` & `itables-2.0.0rc6/docs/developing.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/df_example.png` & `itables-2.0.0rc6/docs/df_example.png`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/downsampling.md` & `itables-2.0.0rc6/docs/downsampling.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/extensions.md` & `itables-2.0.0rc6/docs/extensions.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/formatting.md` & `itables-2.0.0rc6/docs/formatting.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/pandas_style.md` & `itables-2.0.0rc6/docs/pandas_style.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/polars_dataframes.md` & `itables-2.0.0rc6/docs/polars_dataframes.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/quarto.md` & `itables-2.0.0rc6/docs/quarto.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/quick_start.md` & `itables-2.0.0rc6/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/references.md` & `itables-2.0.0rc6/docs/references.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/sample_dataframes.md` & `itables-2.0.0rc6/docs/sample_dataframes.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/show_df.png` & `itables-2.0.0rc6/docs/show_df.png`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/supported_editors.md` & `itables-2.0.0rc6/docs/supported_editors.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/troubleshooting.md` & `itables-2.0.0rc6/docs/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/images/code.png` & `itables-2.0.0rc6/docs/images/code.png`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/images/colab.png` & `itables-2.0.0rc6/docs/images/colab.png`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/images/html.png` & `itables-2.0.0rc6/docs/images/html.png`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/images/lab.png` & `itables-2.0.0rc6/docs/images/lab.png`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/images/notebook.png` & `itables-2.0.0rc6/docs/images/notebook.png`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/images/pycharm.png` & `itables-2.0.0rc6/docs/images/pycharm.png`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/quarto/quarto_html.qmd` & `itables-2.0.0rc6/docs/quarto/quarto_html.qmd`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/docs/quarto/quarto_revealjs.qmd` & `itables-2.0.0rc6/docs/quarto/quarto_revealjs.qmd`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/itables/datatables_format.py` & `itables-2.0.0rc6/itables/datatables_format.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/itables/downsample.py` & `itables-2.0.0rc6/itables/downsample.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/itables/javascript.py` & `itables-2.0.0rc6/itables/javascript.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import json
 import logging
 import re
 import uuid
 import warnings
 from base64 import b64encode
-from copy import deepcopy
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
 from .utils import UNPKG_DT_BUNDLE_CSS, UNPKG_DT_BUNDLE_URL
 from .version import __version__ as itables_version
@@ -471,15 +470,15 @@
     for option in dir(opt):
         if (
             (not use_to_html or (option not in _OPTIONS_NOT_AVAILABLE_WITH_TO_HTML))
             and option not in kwargs
             and not option.startswith("__")
             and option not in {"dt_bundle", "find_package_file", "UNPKG_DT_BUNDLE_URL"}
         ):
-            kwargs[option] = deepcopy(getattr(opt, option))
+            kwargs[option] = getattr(opt, option)
 
     for name, value in kwargs.items():
         if value is None:
             raise ValueError(
                 "Please don't pass an option with a value equal to None ('{}=None')".format(
                     name
                 )
@@ -594,27 +593,27 @@
         )
     else:
         connected_style = f'<link href="{UNPKG_DT_BUNDLE_CSS}" rel="stylesheet">\n'
         output = replace_value(output, connected_style, "")
         connected_import = (
             "import {DataTable, jQuery as $} from '" + UNPKG_DT_BUNDLE_URL + "';"
         )
-        local_import = "const { DataTable, jQuery: $ } = await import(window._datatables_src_for_itables);"
+        local_import = (
+            "const { DataTable, jQuery: $ } = await import(window."
+            + DATATABLES_SRC_FOR_ITABLES
+            + ");"
+        )
         output = replace_value(output, connected_import, local_import)
 
     output = replace_value(
         output,
         '<table id="table_id"><thead><tr><th>A</th></tr></thead></table>',
         html_table,
     )
     output = replace_value(output, "#table_id", "#{}".format(table_id))
-    if not connected:
-        output = replace_value(
-            output, "_datatables_src_for_itables", DATATABLES_SRC_FOR_ITABLES
-        )
 
     if column_filters:
         # If the below was false, we would need to concatenate the JS code
         # which might not be trivial...
         assert pre_dt_code == ""
         assert "initComplete" not in kwargs
```

### Comparing `itables-2.0.0rc5/itables/options.py` & `itables-2.0.0rc6/itables/options.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/itables/sample_dfs.py` & `itables-2.0.0rc6/itables/sample_dfs.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/itables/utils.py` & `itables-2.0.0rc6/itables/utils.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/itables/dt_for_itables/LICENSE` & `itables-2.0.0rc6/itables/dt_for_itables/LICENSE`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/itables/dt_for_itables/README.md` & `itables-2.0.0rc6/itables/dt_for_itables/README.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/itables/dt_for_itables/dt_bundle.css` & `itables-2.0.0rc6/itables/dt_for_itables/dt_bundle.css`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/itables/dt_for_itables/dt_bundle.js` & `itables-2.0.0rc6/itables/dt_for_itables/dt_bundle.js`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/itables/dt_for_itables/package-lock.json` & `itables-2.0.0rc6/itables/dt_for_itables/package-lock.json`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/itables/dt_for_itables/package.json` & `itables-2.0.0rc6/itables/dt_for_itables/package.json`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/itables/dt_for_itables/src.js` & `itables-2.0.0rc6/itables/dt_for_itables/src.js`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/itables/html/datatables_template.html` & `itables-2.0.0rc6/itables/html/datatables_template.html`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/itables/samples/countries.csv` & `itables-2.0.0rc6/itables/samples/countries.csv`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/itables/samples/indicators.csv` & `itables-2.0.0rc6/itables/samples/indicators.csv`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/itables/samples/population.csv` & `itables-2.0.0rc6/itables/samples/population.csv`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/tests/conftest.py` & `itables-2.0.0rc6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/tests/test_changelog.py` & `itables-2.0.0rc6/tests/test_changelog.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/tests/test_connected_notebook_is_small.py` & `itables-2.0.0rc6/tests/test_connected_notebook_is_small.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/tests/test_datatables_format.py` & `itables-2.0.0rc6/tests/test_datatables_format.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/tests/test_documentation_notebooks_run.py` & `itables-2.0.0rc6/tests/test_documentation_notebooks_run.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/tests/test_downsample.py` & `itables-2.0.0rc6/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/tests/test_javascript.py` & `itables-2.0.0rc6/tests/test_javascript.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/tests/test_json_dumps.py` & `itables-2.0.0rc6/tests/test_json_dumps.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/tests/test_notebook.ipynb` & `itables-2.0.0rc6/tests/test_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/tests/test_polars.py` & `itables-2.0.0rc6/tests/test_polars.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/tests/test_sample_dfs.py` & `itables-2.0.0rc6/tests/test_sample_dfs.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/tests/test_sample_python_apps.py` & `itables-2.0.0rc6/tests/test_sample_python_apps.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/tests/test_update_samples.py` & `itables-2.0.0rc6/tests/test_update_samples.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/LICENSE` & `itables-2.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/README.md` & `itables-2.0.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/pyproject.toml` & `itables-2.0.0rc6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itables-2.0.0rc5/PKG-INFO` & `itables-2.0.0rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: itables
-Version: 2.0.0rc5
+Version: 2.0.0rc6
 Summary: Pandas and Polar DataFrames as interactive DataTables
 Project-URL: Homepage, https://mwouts.github.io/itables/
 Project-URL: Documentation, https://mwouts.github.io/itables
 Project-URL: Repository, https://github.com/mwouts/itables.git
 Project-URL: Issues, https://github.com/mwouts/itables/issues
 Project-URL: Changelog, https://github.com/mwouts/itables/blob/main/docs/changelog.md
 Author-email: Marc Wouts <marc.wouts@gmail.com>
```

