# Comparing `tmp/manim_slides-5.1.4.tar.gz` & `tmp/manim_slides-5.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim_slides-5.1.4.tar", last modified: Tue Apr 16 15:37:41 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `manim_slides-5.1.4.tar` & `manim_slides-5.1.5.tar`

### file list

```diff
@@ -1,56 +1,141 @@
--rw-r--r--   0        0        0     1078 2024-04-16 15:37:25.896284 manim_slides-5.1.4/LICENSE.md
--rw-r--r--   0        0        0     9734 2024-04-16 15:37:25.896284 manim_slides-5.1.4/README.md
--rw-r--r--   0        0        0     1639 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/__init__.py
--rw-r--r--   0        0        0     2550 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/__main__.py
--rw-r--r--   0        0        0       22 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/__version__.py
--rw-r--r--   0        0        0     2203 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/commons.py
--rw-r--r--   0        0        0    11054 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/config.py
--rw-r--r--   0        0        0    21294 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/convert.py
--rw-r--r--   0        0        0      110 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/defaults.py
--rw-r--r--   0        0        0        0 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/docs/__init__.py
--rw-r--r--   0        0        0    15913 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/docs/manim_slides_directive.py
--rw-r--r--   0        0        0    10370 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/ipython/ipython_magic.py
--rw-r--r--   0        0        0     1161 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/logger.py
--rw-r--r--   0        0        0    10490 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/present/__init__.py
--rw-r--r--   0        0        0    18068 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/present/player.py
--rw-r--r--   0        0        0      254 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/qt_utils.py
--rw-r--r--   0        0        0     1511 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/render.py
--rw-r--r--   0        0        0     7448 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/resources.py
--rw-r--r--   0        0        0     1317 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/slide/__init__.py
--rw-r--r--   0        0        0     5105 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/slide/animation.py
--rw-r--r--   0        0        0    20747 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/slide/base.py
--rw-r--r--   0        0        0     4432 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/slide/manim.py
--rw-r--r--   0        0        0     2129 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/slide/manimlib.py
--rw-r--r--   0        0        0        0 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/templates/__init__.py
--rw-r--r--   0        0        0    14662 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/templates/revealjs.html
--rw-r--r--   0        0        0     4303 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/utils.py
--rw-r--r--   0        0        0     2317 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/wizard/__init__.py
--rw-r--r--   0        0        0     3651 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/wizard/wizard.py
--rw-r--r--   0        0        0     3795 2024-04-16 15:37:41.840191 manim_slides-5.1.4/pyproject.toml
--rw-r--r--   0        0        0     2056 2024-04-16 15:37:25.908284 manim_slides-5.1.4/tests/conftest.py
--rw-r--r--   0        0        0      834 2024-04-16 15:37:25.908284 manim_slides-5.1.4/tests/data/slides.py
--rw-r--r--   0        0        0     1155 2024-04-16 15:37:25.908284 manim_slides-5.1.4/tests/data/slides/BasicSlide.json
--rw-r--r--   0        0        0    50327 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511.mp4
--rw-r--r--   0        0        0    45042 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511_reversed.mp4
--rw-r--r--   0        0        0    23621 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c.mp4
--rw-r--r--   0        0        0    23195 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c_reversed.mp4
--rw-r--r--   0        0        0    17527 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077.mp4
--rw-r--r--   0        0        0    17349 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077_reversed.mp4
--rw-r--r--   0        0        0    36367 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368.mp4
--rw-r--r--   0        0        0    30504 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368_reversed.mp4
--rw-r--r--   0        0        0    30504 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/data/video.mp4
--rw-r--r--   0        0        0    40695 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/data/video_data_uri.txt
--rw-r--r--   0        0        0     3469 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_base_slide.py
--rw-r--r--   0        0        0     3443 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_commons.py
--rw-r--r--   0        0        0     1103 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_config.py
--rw-r--r--   0        0        0     4574 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_convert.py
--rw-r--r--   0        0        0      249 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_defaults.py
--rw-r--r--   0        0        0     2972 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_main.py
--rw-r--r--   0        0        0     1987 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_manim.py
--rw-r--r--   0        0        0        7 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_player.py
--rw-r--r--   0        0        0     3982 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_present.py
--rw-r--r--   0        0        0      250 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_qt_utils.py
--rw-r--r--   0        0        0     9508 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_slide.py
--rw-r--r--   0        0        0      608 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_utils.py
--rw-r--r--   0        0        0     5074 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_wizard.py
--rw-r--r--   0        0        0    12733 1970-01-01 00:00:00.000000 manim_slides-5.1.4/PKG-INFO
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.bumpversion.cfg
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.mdlc.json
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.python-version
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.readthedocs.yaml
+-rw-r--r--   0        0        0    11291 2020-02-02 00:00:00.000000 manim_slides-5.1.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 manim_slides-5.1.5/CITATION.cff
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 manim_slides-5.1.5/custom_config.yml
+-rw-r--r--   0        0        0     8412 2020-02-02 00:00:00.000000 manim_slides-5.1.5/example.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim-slides.qrc
+-rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 manim_slides-5.1.5/requirements-dev.lock
+-rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 manim_slides-5.1.5/requirements.lock
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.github/FUNDING.yml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.github/dependabot.yml
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.github/ISSUE_TEMPLATE/documentation.yml
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.github/ISSUE_TEMPLATE/support.yml
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.github/scripts/check_github_issues.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.github/workflows/clearcache.yml
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.github/workflows/draft-pdf.yml
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.github/workflows/languagetool.yml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.github/workflows/latest_tag.yml
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docker/Dockerfile
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docker/README.md
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docker/texlive-profile.txt
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/make.bat
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/changelog.md
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/conf.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/docutils.conf
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/faq.md
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/features_table.md
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/index.md
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/installation.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/license.md
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/manim_or_manimgl.md
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/quickstart.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/_static/favicon.png -> ../../../static/favicon.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/_static/logo.png -> ../../../static/logo.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/_static/logo_dark_docs.png -> ../../../static/logo_dark_docs.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/_static/logo_dark_github.png -> ../../../static/logo_dark_github.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/_static/logo_dark_transparent.png -> ../../../static/logo_dark_transparent.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/_static/logo_light_transparent.png -> ../../../static/logo_light_transparent.png
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/_static/template.diff
+-rw-r--r--   0        0        0    17358 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/_static/template.html
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/_static/wizard_dark.png -> ../../../static/wizard_dark.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/_static/wizard_light.png -> ../../../static/wizard_light.png
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/contributing/index.md
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/contributing/internals.md
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/contributing/workflow.md
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/reference/api.md
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/reference/cli.md
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/reference/customize_html.md
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/reference/examples.md
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/reference/gui.md
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/reference/html.md
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/reference/index.md
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/reference/ipython_magic.md
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/reference/magic_example.ipynb
+-rw-r--r--   0        0        0     6947 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/reference/sharing.md
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 manim_slides-5.1.5/docs/source/reference/sphinx_extension.md
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/__init__.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/__version__.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/commons.py
+-rw-r--r--   0        0        0    11123 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/config.py
+-rw-r--r--   0        0        0    21230 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/convert.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/defaults.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/logger.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/qt_utils.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/render.py
+-rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/resources.py
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/docs/__init__.py
+-rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/docs/manim_slides_directive.py
+-rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/ipython/ipython_magic.py
+-rw-r--r--   0        0        0    10490 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/present/__init__.py
+-rw-r--r--   0        0        0    18061 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/present/player.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/slide/__init__.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/slide/animation.py
+-rw-r--r--   0        0        0    20762 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/slide/base.py
+-rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/slide/manim.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/slide/manimlib.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/templates/__init__.py
+-rw-r--r--   0        0        0    14662 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/templates/revealjs.html
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/wizard/__init__.py
+-rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 manim_slides-5.1.5/manim_slides/wizard/wizard.py
+-rw-r--r--   0        0        0   161325 2020-02-02 00:00:00.000000 manim_slides-5.1.5/paper/docs.png
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 manim_slides-5.1.5/paper/paper.bib
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 manim_slides-5.1.5/paper/paper.md
+-rw-r--r--   0        0        0   181998 2020-02-02 00:00:00.000000 manim_slides-5.1.5/static/docs.png
+-rw-r--r--   0        0        0   496568 2020-02-02 00:00:00.000000 manim_slides-5.1.5/static/example.gif
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 manim_slides-5.1.5/static/favicon.png
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 manim_slides-5.1.5/static/icon.png
+-rw-r--r--   0        0        0    92151 2020-02-02 00:00:00.000000 manim_slides-5.1.5/static/logo.png
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 manim_slides-5.1.5/static/logo.py
+-rw-r--r--   0        0        0    88069 2020-02-02 00:00:00.000000 manim_slides-5.1.5/static/logo_dark_docs.png
+-rw-r--r--   0        0        0    88377 2020-02-02 00:00:00.000000 manim_slides-5.1.5/static/logo_dark_github.png
+-rw-r--r--   0        0        0   112081 2020-02-02 00:00:00.000000 manim_slides-5.1.5/static/logo_dark_transparent.png
+-rw-r--r--   0        0        0   104821 2020-02-02 00:00:00.000000 manim_slides-5.1.5/static/logo_light_transparent.png
+-rwxr-xr-x   0        0        0      231 2020-02-02 00:00:00.000000 manim_slides-5.1.5/static/make_favicon.sh
+-rwxr-xr-x   0        0        0     1364 2020-02-02 00:00:00.000000 manim_slides-5.1.5/static/make_logo.sh
+-rw-r--r--   0        0        0    29891 2020-02-02 00:00:00.000000 manim_slides-5.1.5/static/windows_quality_fix.png
+-rw-r--r--   0        0        0    26333 2020-02-02 00:00:00.000000 manim_slides-5.1.5/static/wizard_dark.png
+-rw-r--r--   0        0        0    24815 2020-02-02 00:00:00.000000 manim_slides-5.1.5/static/wizard_light.png
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/conftest.py
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/test_base_slide.py
+-rw-r--r--   0        0        0     3443 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/test_commons.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/test_config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/test_convert.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/test_defaults.py
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/test_main.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/test_manim.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/test_player.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/test_present.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/test_qt_utils.py
+-rw-r--r--   0        0        0     9760 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/test_slide.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/test_utils.py
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/test_wizard.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/data/slides.py
+-rw-r--r--   0        0        0    30504 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/data/video.mp4
+-rw-r--r--   0        0        0    40695 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/data/video_data_uri.txt
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/data/slides/BasicSlide.json
+-rw-r--r--   0        0        0    50327 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511.mp4
+-rw-r--r--   0        0        0    45042 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511_reversed.mp4
+-rw-r--r--   0        0        0    23621 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c.mp4
+-rw-r--r--   0        0        0    23195 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c_reversed.mp4
+-rw-r--r--   0        0        0    17527 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077.mp4
+-rw-r--r--   0        0        0    17349 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077_reversed.mp4
+-rw-r--r--   0        0        0    36367 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368.mp4
+-rw-r--r--   0        0        0    30504 2020-02-02 00:00:00.000000 manim_slides-5.1.5/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368_reversed.mp4
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 manim_slides-5.1.5/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 manim_slides-5.1.5/LICENSE.md
+-rw-r--r--   0        0        0     9076 2020-02-02 00:00:00.000000 manim_slides-5.1.5/README.md
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 manim_slides-5.1.5/pyproject.toml
+-rw-r--r--   0        0        0    12829 2020-02-02 00:00:00.000000 manim_slides-5.1.5/PKG-INFO
```

### Comparing `manim_slides-5.1.4/LICENSE.md` & `manim_slides-5.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/README.md` & `manim_slides-5.1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 > This project extends the work of
 > [`manim-presentation`](https://github.com/galatolofederico/manim-presentation),
 > with a lot more features!
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Comparison with Similar Tools](#comparison-with-similar-tools)
-- [F.A.Q](#faq)
-  * [How to increase quality on Windows](#how-to-increase-quality-on-windows)
+- [F.A.Q](https://eertmans.be/manim-slides/latest/faq.html)
 - [Contributing](#contributing)
   * [Reporting an Issue](#reporting-an-issue)
   * [Seeking for Help](#seeking-for-help)
   * [Contact](#contact)
 
 ## Installation
 
@@ -45,23 +44,23 @@
 ## Usage
 
 <!-- start usage -->
 
 Using Manim Slides is a two-step process:
 1. Render animations using `Slide` (resp. `ThreeDSlide`) as a base class instead
    of `Scene` (resp. `ThreeDScene`), and add calls to `self.next_slide()`
-   everytime you want to create a new slide.
+   every time you want to create a new slide.
 2. Run `manim-slides` on rendered animations and display them like a
    *PowerPoint* presentation.
 
 The documentation is available [online](https://eertmans.be/manim-slides/).
 
 ### Basic Example
 
-Call `self.next_slide()` everytime you want to create a pause between
+Call `self.next_slide()` every time you want to create a pause between
 animations, and `self.next_slide(loop=True)` if you want the next slide to loop
 over animations until the user presses continue:
 
 ```python
 from manim import *  # or: from manimlib import *
 
 from manim_slides import Slide
@@ -114,15 +113,15 @@
 <!-- end more-usage -->
 
 <p align="center">
   <img alt="Example GIF" src="https://raw.githubusercontent.com/jeertmans/manim-slides/main/static/example.gif">
 </p>
 
 For detailed usage documentation, run `manim-slides --help`, or go to the
-[documentation](https://eertmans.be/manim-slides/reference/cli.html).
+[documentation](https://eertmans.be/manim-slides/latest/reference/cli.html).
 
 ## Interactive Tutorial
 
 Click on the image to watch a slides presentation that explains to you how
 to use Manim Slides.
 
 [![Manim Slides Docs](https://raw.githubusercontent.com/jeertmans/manim-slides/main/static/docs.png)](https://eertmans.be/manim-slides/)
@@ -146,35 +145,18 @@
 | Activity | [![GitHub Repo stars](https://img.shields.io/github/last-commit/jeertmans/manim-slides?style=social)](https://github.com/jeertmans/manim-slides) | [![GitHub Repo stars](https://img.shields.io/github/last-commit/galatolofederico/manim-presentation?style=social)](https://github.com/galatolofederico/manim-presentation) | [![GitHub Repo stars](https://img.shields.io/github/last-commit/ManimCommunity/manim_editor?style=social)](https://github.com/ManimCommunity/manim_editor) | [![GitHub Repo stars](https://img.shields.io/github/last-commit/jupyter/notebook?style=social)](https://github.com/jupyter/notebook) |
 | Usage | Command-line | Command-line | Web Browser | Notebook |
 | Note | Requires minimal modif. in scenes files | Requires minimal modif. in scenes files |  Requires the usage of sections, and configuration through graphical interface | Relies on `nbconvert` to create slides from a Notebook |
 | Support for ManimGL | Yes | No | No | No |
 | Web Browser presentations | Yes | No | Yes | No |
 | Offline presentations | Yes, with Qt | Yes, with OpenCV | No | No
 
-## F.A.Q
-
-### How to increase quality on Windows
-
-On Windows platform, one may encounter a lower image resolution than expected.
-Usually, this is observed because Windows rescales every application to
-fit the screen.
-As found by [@arashash](https://github.com/arashash),
-in [#20](https://github.com/jeertmans/manim-slides/issues/20),
-the problem can be addressed by changing the scaling factor to 100%:
-
-<p align="center">
-  <img alt="Windows Fix Scaling" src="https://raw.githubusercontent.com/jeertmans/manim-slides/main/static/windows_quality_fix.png">
-</p>
-
-in *Settings*->*Display*.
-
 ## Contributing
 
 Contributions are more than welcome! Please read through
-[our contributing section](https://eertmans.be/manim-slides/contributing/index.html).
+[our contributing section](https://eertmans.be/manim-slides/latest/contributing/index.html).
 
 ### Reporting an Issue
 
 <!-- start reporting-an-issue -->
 
 If you think you found a bug,
 an error in the documentation,
@@ -198,20 +180,18 @@
 ### Seeking for help
 
 <!-- start seeking-for-help -->
 
 Sometimes, you may have a question about Manim Slides,
 not necessarily an issue.
 
-There are two ways you can reach us for questions:
-
-- via the `Question/Help/Support` topic when
-[choosing an issue template](https://github.com/jeertmans/manim-slides/issues/new/choose);
-- or via
-[GitHub discussions](https://github.com/jeertmans/manim-slides/discussions).
+First, make sure to read the
+[F.A.Q](https://eertmans.be/manim-slides/latest/faq.html) to see if
+your question has already been answered. If not, please follow the
+recommendation (from that page) to reach us for questions.
 
 <!-- end seeking-for-help -->
 
 ### Contact
 
 <!-- start contact -->
```

### Comparing `manim_slides-5.1.4/manim_slides/__init__.py` & `manim_slides-5.1.5/manim_slides/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             if ipy is not None:
                 ipy.register_magics(magic)
 
             return magic
 
         return ModuleType.__getattribute__(self, name)
 
-    def __dir__(self) -> List[str]:
+    def __dir__(self) -> list[str]:
         result = list(new_module.__all__)
         result.extend(
             (
                 "__file__",
                 "__doc__",
                 "__all__",
                 "__docformat__",
```

### Comparing `manim_slides-5.1.4/manim_slides/__main__.py` & `manim_slides-5.1.5/manim_slides/__main__.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/manim_slides/commons.py` & `manim_slides-5.1.5/manim_slides/commons.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/manim_slides/config.py` & `manim_slides-5.1.5/manim_slides/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import shutil
 from functools import wraps
 from inspect import Parameter, signature
 from pathlib import Path
 from textwrap import dedent
-from typing import Any, Callable, Dict, List, Optional, Set, Tuple
+from typing import Any, Callable, Optional
 
 import rtoml
 from pydantic import (
     BaseModel,
     Field,
     FilePath,
     PositiveInt,
@@ -20,15 +20,15 @@
 
 from .logger import logger
 
 Receiver = Callable[..., Any]
 
 
 class Signal(BaseModel):  # type: ignore[misc]
-    __receivers: List[Receiver] = PrivateAttr(default_factory=list)
+    __receivers: list[Receiver] = PrivateAttr(default_factory=list)
 
     def connect(self, receiver: Receiver) -> None:
         self.__receivers.append(receiver)
 
     def disconnect(self, receiver: Receiver) -> None:
         self.__receivers.remove(receiver)
 
@@ -43,22 +43,22 @@
 
     return getattr(Qt, f"Key_{name}")
 
 
 class Key(BaseModel):  # type: ignore[misc]
     """Represents a list of key codes, with optionally a name."""
 
-    ids: List[PositiveInt] = Field(unique=True)
+    ids: list[PositiveInt] = Field(unique=True)
     name: Optional[str] = None
 
     __signal: Signal = PrivateAttr(default_factory=Signal)
 
     @field_validator("ids")
     @classmethod
-    def ids_is_non_empty_set(cls, ids: Set[Any]) -> Set[Any]:
+    def ids_is_non_empty_set(cls, ids: set[Any]) -> set[Any]:
         if len(ids) <= 0:
             raise ValueError("Key's ids must be a non-empty set")
         return ids
 
     def set_ids(self, *ids: int) -> None:
         self.ids = list(set(ids))
 
@@ -94,16 +94,16 @@
     )
     HIDE_MOUSE: Key = Field(
         default_factory=lambda: Key(ids=[key_id("H")], name="HIDE / SHOW MOUSE")
     )
 
     @model_validator(mode="before")
     @classmethod
-    def ids_are_unique_across_keys(cls, values: Dict[str, Key]) -> Dict[str, Key]:
-        ids: Set[int] = set()
+    def ids_are_unique_across_keys(cls, values: dict[str, Key]) -> dict[str, Key]:
+        ids: set[int] = set()
 
         for key in values.values():
             if len(ids.intersection(key["ids"])) != 0:
                 raise ValueError(
                     "Two or more keys share a common key code: please make sure each key has distinct key codes"
                 )
             ids.update(key["ids"])
@@ -245,15 +245,19 @@
     @classmethod
     def start_animation_is_before_end(
         cls, pre_slide_config: "PreSlideConfig"
     ) -> "PreSlideConfig":
         if pre_slide_config.start_animation >= pre_slide_config.end_animation:
             if pre_slide_config.start_animation == pre_slide_config.end_animation == 0:
                 raise ValueError(
-                    "You have to play at least one animation (e.g., `self.wait()`) before pausing. If you want to start paused, use the approriate command-line option when presenting. IMPORTANT: when using ManimGL, `self.wait()` is not considered to be an animation, so prefer to directly use `self.play(...)`."
+                    "You have to play at least one animation (e.g., `self.wait()`) "
+                    "before pausing. If you want to start paused, use the appropriate "
+                    "command-line option when presenting. "
+                    "IMPORTANT: when using ManimGL, `self.wait()` is not considered "
+                    "to be an animation, so prefer to directly use `self.play(...)`."
                 )
 
             raise ValueError(
                 "Start animation index must be strictly lower than end animation index"
             )
 
         return pre_slide_config
@@ -288,16 +292,16 @@
     def from_pre_slide_config_and_files(
         cls, pre_slide_config: PreSlideConfig, file: Path, rev_file: Path
     ) -> "SlideConfig":
         return cls(file=file, rev_file=rev_file, **pre_slide_config.dict())
 
 
 class PresentationConfig(BaseModel):  # type: ignore[misc]
-    slides: List[SlideConfig] = Field(min_length=1)
-    resolution: Tuple[PositiveInt, PositiveInt] = (1920, 1080)
+    slides: list[SlideConfig] = Field(min_length=1)
+    resolution: tuple[PositiveInt, PositiveInt] = (1920, 1080)
     background_color: Color = "black"
 
     @classmethod
     def from_file(cls, path: Path) -> "PresentationConfig":
         """Read a presentation configuration from a file."""
         with open(path) as f:
             obj = json.load(f)
```

### Comparing `manim_slides-5.1.4/manim_slides/convert.py` & `manim_slides-5.1.5/manim_slides/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import mimetypes
 import os
 import platform
 import subprocess
-import sys
 import tempfile
 import webbrowser
 from base64 import b64encode
 from collections import deque
 from enum import Enum
 from importlib import resources
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, Type, Union
+from typing import Any, Callable, Optional, Union
 
 import av
 import click
 import pptx
 from click import Context, Parameter
 from jinja2 import Template
 from lxml import etree
@@ -49,15 +48,15 @@
         os.startfile(str(file))  # type: ignore[attr-defined]
     else:
         subprocess.call(("xdg-open", str(file)))
 
 
 def validate_config_option(
     ctx: Context, param: Parameter, value: Any
-) -> Dict[str, str]:
+) -> dict[str, str]:
     config = {}
 
     for c_option in value:
         try:
             key, value = c_option.split("=")
             config[key] = value
         except ValueError:
@@ -117,15 +116,15 @@
         return ""
 
     def open(self, file: Path) -> Any:
         """Open a file, generated with converter, using appropriate application."""
         raise NotImplementedError
 
     @classmethod
-    def from_string(cls, s: str) -> Type["Converter"]:
+    def from_string(cls, s: str) -> type["Converter"]:
         """Return the appropriate converter from a string name."""
         return {
             "html": RevealJS,
             "pdf": PDF,
             "pptx": PowerPoint,
         }[s]
 
@@ -325,15 +324,15 @@
     auto_play_media: AutoPlayMedia = AutoPlayMedia.null
     preload_iframes: PreloadIframes = PreloadIframes.null
     auto_animate: JsBool = JsBool.true
     auto_animate_matcher: Union[AutoAnimateMatcher, Function] = AutoAnimateMatcher.null
     auto_animate_easing: AutoAnimateEasing = AutoAnimateEasing.ease
     auto_animate_duration: float = 1.0
     auto_animate_unmatched: JsBool = JsBool.true
-    auto_animate_styles: List[str] = Field(
+    auto_animate_styles: list[str] = Field(
         default_factory=lambda: [
             "opacity",
             "color",
             "background-color",
             "padding",
             "font-size",
             "line-height",
@@ -375,17 +374,14 @@
     model_config = ConfigDict(use_enum_values=True, extra="forbid")
 
     def load_template(self) -> str:
         """Return the RevealJS HTML template as a string."""
         if isinstance(self.template, Path):
             return self.template.read_text()
 
-        if sys.version_info < (3, 9):
-            return resources.read_text(templates, "revealjs.html")
-
         return resources.files(templates).joinpath("revealjs.html").read_text()
 
     def open(self, file: Path) -> bool:
         return webbrowser.open(file.absolute().as_uri())
 
     def convert_to(self, dest: Path) -> None:
         """
@@ -564,19 +560,22 @@
 
     def callback(ctx: Context, param: Parameter, value: bool) -> None:
         if not value or ctx.resilient_parsing:
             return
 
         to = ctx.params.get("to", "html")
 
-        converter = Converter.from_string(to)(
-            presentation_configs=[PresentationConfig()]
-        )
-        for key, value in converter.dict().items():
-            click.echo(f"{key}: {value!r}")
+        converter = Converter.from_string(to)
+
+        for key, field in converter.model_fields.items():
+            if field.is_required():
+                continue
+
+            default = field.get_default(call_default_factory=True)
+            click.echo(f"{key}: {default}")
 
         ctx.exit()
 
     return click.option(  # type: ignore
         "--show-config",
         is_flag=True,
         help="Show supported options for given format and exit.",
@@ -627,15 +626,15 @@
     show_default=True,
     help="Set the conversion format to use. Use 'auto' to detect format from DEST.",
 )
 @click.option(
     "--open",
     "open_result",
     is_flag=True,
-    help="Open the newly created file using the approriate application.",
+    help="Open the newly created file using the appropriate application.",
 )
 @click.option("-f", "--force", is_flag=True, help="Overwrite any existing file.")
 @click.option(
     "-c",
     "--config",
     "config_options",
     multiple=True,
@@ -651,21 +650,21 @@
     help="Use the template given by FILE instead of default one. "
     "To echo the default template, use ``--show-template``.",
 )
 @show_template_option
 @show_config_options
 @verbosity_option
 def convert(
-    scenes: List[str],
+    scenes: list[str],
     folder: Path,
     dest: Path,
     to: str,
     open_result: bool,
     force: bool,
-    config_options: Dict[str, str],
+    config_options: dict[str, str],
     template: Optional[Path],
 ) -> None:
     """Convert SCENE(s) into a given format and writes the result in DEST."""
     presentation_configs = get_scenes_presentation_config(scenes, folder)
 
     try:
         if to == "auto":
@@ -691,15 +690,15 @@
         if open_result:
             converter.open(dest)
 
     except ValidationError as e:
         errors = e.errors()
 
         msg = [
-            f"{len(errors)} error(s) occured with configuration options for '{to}', see below."
+            f"{len(errors)} error(s) occurred with configuration options for '{to}', see below."
         ]
 
         for error in errors:
             option = error["loc"][0]
             _msg = error["msg"]
             msg.append(f"Option '{option}': {_msg}")
```

### Comparing `manim_slides-5.1.4/manim_slides/docs/manim_slides_directive.py` & `manim_slides-5.1.5/manim_slides/docs/manim_slides_directive.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/manim_slides/ipython/ipython_magic.py` & `manim_slides-5.1.5/manim_slides/ipython/ipython_magic.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/manim_slides/logger.py` & `manim_slides-5.1.5/manim_slides/logger.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/manim_slides/present/__init__.py` & `manim_slides-5.1.5/manim_slides/present/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 @verbosity_option
 def list_scenes(folder: Path) -> None:
     """List available scenes."""
     for i, scene in enumerate(_list_scenes(folder), start=1):
         click.secho(f"{i}: {scene}", fg="green")
 
 
-def _list_scenes(folder: Path) -> List[str]:
+def _list_scenes(folder: Path) -> list[str]:
     """List available scenes in given directory."""
     scenes = []
 
     for filepath in folder.glob("*.json"):
         try:
             _ = PresentationConfig.from_file(filepath)
             scenes.append(filepath.stem)
@@ -55,27 +55,27 @@
             )
 
     logger.debug(f"Found {len(scenes)} valid scene configuration files in `{folder}`.")
 
     return scenes
 
 
-def prompt_for_scenes(folder: Path) -> List[str]:
+def prompt_for_scenes(folder: Path) -> list[str]:
     """Prompt the user to select scenes within a given folder."""
     scene_choices = dict(enumerate(_list_scenes(folder), start=1))
 
     for i, scene in scene_choices.items():
         click.secho(f"{i}: {scene}", fg="green")
 
     click.echo()
 
     click.echo("Choose number corresponding to desired scene/arguments.")
     click.echo("(Use comma separated list for multiple entries)")
 
-    def value_proc(value: Optional[str]) -> List[str]:
+    def value_proc(value: Optional[str]) -> list[str]:
         indices = list(map(int, (value or "").strip().replace(" ", "").split(",")))
 
         if not all(0 < i <= len(scene_choices) for i in indices):
             raise click.UsageError("Please only enter numbers displayed on the screen.")
 
         return [scene_choices[i] for i in indices]
 
@@ -89,16 +89,16 @@
             scenes = click.prompt("Choice(s)", value_proc=value_proc)
             return scenes  # type: ignore
         except ValueError as e:
             raise click.UsageError(str(e)) from None
 
 
 def get_scenes_presentation_config(
-    scenes: List[str], folder: Path
-) -> List[PresentationConfig]:
+    scenes: list[str], folder: Path
+) -> list[PresentationConfig]:
     """Return a list of presentation configurations based on the user input."""
     if len(scenes) == 0:
         scenes = prompt_for_scenes(folder)
 
     presentation_configs = []
     for scene in scenes:
         config_file = folder / f"{scene}.json"
@@ -112,15 +112,15 @@
             raise click.UsageError(str(e)) from None
 
     return presentation_configs
 
 
 def start_at_callback(
     ctx: Context, param: Parameter, values: str
-) -> Tuple[Optional[int], ...]:
+) -> tuple[Optional[int], ...]:
     if values == "(None, None)":
         return (None, None)
 
     def str_to_int_or_none(value: str) -> Optional[int]:
         if value.lower().strip() == "":
             return None
         else:
@@ -249,24 +249,24 @@
     type=int,
     default=None,
     help="Put info window on the given screen (a.k.a. display).",
 )
 @click.help_option("-h", "--help")
 @verbosity_option
 def present(
-    scenes: List[str],
+    scenes: list[str],
     config_path: Path,
     folder: Path,
     start_paused: bool,
     full_screen: bool,
     skip_all: bool,
     exit_after_last_slide: bool,
     hide_mouse: bool,
     aspect_ratio: str,
-    start_at: Tuple[Optional[int], Optional[int], Optional[int]],
+    start_at: tuple[Optional[int], Optional[int], Optional[int]],
     start_at_scene_number: int,
     start_at_slide_number: int,
     screen_number: Optional[int],
     playback_rate: float,
     next_terminates_loop: bool,
     hide_info_window: bool,
     info_window_screen_number: Optional[int],
```

### Comparing `manim_slides-5.1.4/manim_slides/present/player.py` & `manim_slides-5.1.5/manim_slides/present/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
 from pathlib import Path
-from typing import List, Optional
+from typing import Optional
 
 from qtpy.QtCore import Qt, QTimer, QUrl, Signal, Slot
 from qtpy.QtGui import QCloseEvent, QIcon, QKeyEvent, QScreen
 from qtpy.QtMultimedia import QAudioOutput, QMediaPlayer
 from qtpy.QtMultimediaWidgets import QVideoWidget
 from qtpy.QtWidgets import (
     QHBoxLayout,
@@ -52,15 +52,15 @@
         )
         main_video_widget = QVideoWidget()
         main_video_widget.setAspectRatioMode(aspect_ratio_mode)
         main_video_widget.setFixedSize(720, 480)
         self.video_sink = main_video_widget.videoSink()
         left_layout.addWidget(main_video_widget)
 
-        # Current slide informations
+        # Current slide information
 
         self.scene_label = QLabel()
         self.slide_label = QLabel()
         self.start_time = datetime.now()
         self.time_label = QLabel()
         self.elapsed_label = QLabel("00h00m00s")
         self.timer = QTimer()
@@ -165,15 +165,15 @@
 class Player(QMainWindow):  # type: ignore[misc]
     presentation_changed: Signal = Signal()
     slide_changed: Signal = Signal()
 
     def __init__(
         self,
         config: Config,
-        presentation_configs: List[PresentationConfig],
+        presentation_configs: list[PresentationConfig],
         *,
         start_paused: bool = False,
         full_screen: bool = False,
         skip_all: bool = False,
         exit_after_last_slide: bool = False,
         hide_mouse: bool = False,
         aspect_ratio_mode: Qt.AspectRatioMode = Qt.KeepAspectRatio,
```

### Comparing `manim_slides-5.1.4/manim_slides/render.py` & `manim_slides-5.1.5/manim_slides/render.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 1. You can are sure to execute the rendering command with the same Python environment
    as for ``manim-slides``.
 2. You can pass options to the config.
 """
 
 import subprocess
 import sys
-from typing import Tuple
 
 import click
 
 
 @click.command(
     context_settings=dict(
         ignore_unknown_options=True, allow_extra_args=True, help_option_names=("-h",)
@@ -35,15 +34,15 @@
     "--GL",
     is_flag=True,
     envvar="MANIMGL_RENDERER",
     show_envvar=True,
     help="If set, use ManimGL renderer.",
 )
 @click.argument("args", metavar="[RENDERER_ARGS]...", nargs=-1, type=click.UNPROCESSED)
-def render(ce: bool, gl: bool, args: Tuple[str, ...]) -> None:
+def render(ce: bool, gl: bool, args: tuple[str, ...]) -> None:
     """
     Render SCENE(s) from the input FILE, using the specified renderer.
 
     Use ``manim-slides render --help`` to see help information for
     a specific renderer.
     """
     if ce and gl:
```

### Comparing `manim_slides-5.1.4/manim_slides/resources.py` & `manim_slides-5.1.5/manim_slides/resources.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/manim_slides/slide/__init__.py` & `manim_slides-5.1.5/manim_slides/slide/__init__.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/manim_slides/slide/animation.py` & `manim_slides-5.1.5/manim_slides/slide/animation.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 For each of the provided classes, there exists a method variant
 that directly calls ``self.play(Animation(...))``, see
 :class:`Slide<manim_slides.slide.Slide>`.
 """
 
 __all__ = ["Wipe", "Zoom"]
 
-from typing import Any, Mapping, Optional, Sequence
+from collections.abc import Mapping, Sequence
+from typing import Any, Optional
 
 import numpy as np
 
 from . import MANIM
 
 if MANIM:
     from manim import LEFT, AnimationGroup, FadeIn, FadeOut
```

### Comparing `manim_slides-5.1.4/manim_slides/slide/base.py` & `manim_slides-5.1.5/manim_slides/slide/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from __future__ import annotations
 
 __all__ = ["BaseSlide"]
 
 import platform
 from abc import abstractmethod
+from collections.abc import MutableMapping, Sequence, ValuesView
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
-    MutableMapping,
-    Sequence,
-    ValuesView,
 )
 
 import numpy as np
 from tqdm import tqdm
 
 from ..config import BaseSlideConfig, PresentationConfig, PreSlideConfig, SlideConfig
 from ..defaults import FOLDER_PATH
```

### Comparing `manim_slides-5.1.4/manim_slides/slide/manim.py` & `manim_slides-5.1.5/manim_slides/slide/manim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Any, List, Optional, Tuple
+from typing import Any, Optional
 
 from manim import Scene, ThreeDScene, config
 
 from ..config import BaseSlideConfig
 from .base import BaseSlide
 
 
@@ -26,19 +26,19 @@
         color = self.camera.background_color
         if hex_color := getattr(color, "hex", None):
             return hex_color  # type: ignore
         else:  # manim>=0.18, see https://github.com/ManimCommunity/manim/pull/3020
             return color.to_hex()  # type: ignore
 
     @property
-    def _resolution(self) -> Tuple[int, int]:
+    def _resolution(self) -> tuple[int, int]:
         return config["pixel_width"], config["pixel_height"]
 
     @property
-    def _partial_movie_files(self) -> List[Path]:
+    def _partial_movie_files(self) -> list[Path]:
         # When rendering with -na,b (manim only)
         # the animations not in [a,b] will be skipped,
         # but animation before a will have a None source file.
         return [
             Path(file)
             for file in self.renderer.file_writer.partial_movie_files
             if file is not None
```

### Comparing `manim_slides-5.1.4/manim_slides/slide/manimlib.py` & `manim_slides-5.1.5/manim_slides/slide/manimlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Any, ClassVar, Dict, List, Optional, Tuple
+from typing import Any, ClassVar, Optional
 
 from manimlib import Scene, ThreeDCamera
 from manimlib.utils.file_ops import get_sorted_integer_files
 
 from .base import BaseSlide
 
 
@@ -27,19 +27,19 @@
         return self.camera.frame.get_width()  # type: ignore
 
     @property
     def _background_color(self) -> str:
         return self.camera_config["background_color"].hex  # type: ignore
 
     @property
-    def _resolution(self) -> Tuple[int, int]:
+    def _resolution(self) -> tuple[int, int]:
         return self.camera_config["pixel_width"], self.camera_config["pixel_height"]
 
     @property
-    def _partial_movie_files(self) -> List[Path]:
+    def _partial_movie_files(self) -> list[Path]:
         kwargs = {
             "remove_non_integer_files": True,
             "extension": self.file_writer.movie_file_extension,
         }
         return [
             Path(file)
             for file in get_sorted_integer_files(
@@ -62,11 +62,11 @@
     def run(self, *args: Any, **kwargs: Any) -> None:
         """MANIMGL renderer."""
         super().run(*args, **kwargs)
         self._save_slides(use_cache=False)
 
 
 class ThreeDSlide(Slide):
-    CONFIG: ClassVar[Dict[str, Any]] = {
+    CONFIG: ClassVar[dict[str, Any]] = {
         "camera_class": ThreeDCamera,
     }
     pass
```

### Comparing `manim_slides-5.1.4/manim_slides/templates/revealjs.html` & `manim_slides-5.1.5/manim_slides/templates/revealjs.html`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
         // speaker view
         defaultTiming: {{ default_timing }},
 
         // Enable slide navigation via mouse wheel
         mouseWheel: {{ mouse_wheel }},
 
         // Opens links in an iframe preview overlay
-        // Add `data-preview-link` and `data-preview-link="false"` to customise each link
+        // Add `data-preview-link` and `data-preview-link="false"` to customize each link
         // individually
         previewLinks: {{ preview_links }},
 
         // Exposes the reveal.js API through window.postMessage
         postMessage: {{ post_message }},
 
         // Dispatches all reveal.js events to the parent window through postMessage
```

### Comparing `manim_slides-5.1.4/manim_slides/utils.py` & `manim_slides-5.1.5/manim_slides/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import hashlib
 import os
 import tempfile
+from collections.abc import Iterator
 from pathlib import Path
-from typing import Iterator, List
 
 import av
 
 from .logger import logger
 
 
-def concatenate_video_files(files: List[Path], dest: Path) -> None:
+def concatenate_video_files(files: list[Path], dest: Path) -> None:
     """Concatenate multiple video files into one."""
 
-    def _filter(files: List[Path]) -> Iterator[Path]:
+    def _filter(files: list[Path]) -> Iterator[Path]:
         """Patch possibly empty video files."""
         for file in files:
             with av.open(str(file)) as container:
                 if len(container.streams.video) > 0:
                     yield file
                 else:
                     logger.warn(
@@ -26,17 +26,18 @@
                         "https://github.com/jeertmans/manim-slides/issues/390."
                     )
 
     with tempfile.NamedTemporaryFile(mode="w", suffix=".txt", delete=False) as f:
         f.writelines(f"file '{file}'\n" for file in _filter(files))
         tmp_file = f.name
 
-    with av.open(
-        tmp_file, format="concat", options={"safe": "0"}
-    ) as input_container, av.open(str(dest), mode="w") as output_container:
+    with (
+        av.open(tmp_file, format="concat", options={"safe": "0"}) as input_container,
+        av.open(str(dest), mode="w") as output_container,
+    ):
         input_video_stream = input_container.streams.video[0]
         output_video_stream = output_container.add_stream(
             template=input_video_stream,
         )
 
         if len(input_container.streams.audio) > 0:
             input_audio_stream = input_container.streams.audio[0]
@@ -57,15 +58,15 @@
             else:
                 continue  # We don't support subtitles
             output_container.mux(packet)
 
     os.unlink(tmp_file)  # https://stackoverflow.com/a/54768241
 
 
-def merge_basenames(files: List[Path]) -> Path:
+def merge_basenames(files: list[Path]) -> Path:
     """Merge multiple filenames by concatenating basenames."""
     if len(files) == 0:
         raise ValueError("Cannot merge an empty list of files!")
 
     dirname: Path = files[0].parent
     ext = files[0].suffix
 
@@ -85,21 +86,22 @@
 def link_nodes(*nodes: av.filter.context.FilterContext) -> None:
     """Code from https://github.com/PyAV-Org/PyAV/issues/239."""
     for c, n in zip(nodes, nodes[1:]):
         c.link_to(n)
 
 
 def reverse_video_file(src: Path, dest: Path) -> None:
-    """Reverses a video file, writting the result to `dest`."""
-    with av.open(str(src)) as input_container, av.open(
-        str(dest), mode="w"
-    ) as output_container:
+    """Reverses a video file, writing the result to `dest`."""
+    with (
+        av.open(str(src)) as input_container,
+        av.open(str(dest), mode="w") as output_container,
+    ):
         input_stream = input_container.streams.video[0]
         output_stream = output_container.add_stream(
-            codec_name=input_stream.codec_context.name, rate=input_stream.base_rate
+            codec_name="libx264", rate=input_stream.base_rate
         )
         output_stream.width = input_stream.width
         output_stream.height = input_stream.height
         output_stream.pix_fmt = input_stream.pix_fmt
 
         graph = av.filter.Graph()
         link_nodes(
@@ -114,13 +116,12 @@
             graph.push(frame)
             frames_count += 1
 
         graph.push(None)  # EOF: https://github.com/PyAV-Org/PyAV/issues/886.
 
         for _ in range(frames_count):
             frame = graph.pull()
-
-            for packet in output_stream.encode(frame):
-                output_container.mux(packet)
+            frame.pict_type = 5  # Otherwise we get a warning saying it is changed
+            output_container.mux(output_stream.encode(frame))
 
         for packet in output_stream.encode():
             output_container.mux(packet)
```

### Comparing `manim_slides-5.1.4/manim_slides/wizard/__init__.py` & `manim_slides-5.1.5/manim_slides/wizard/__init__.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/manim_slides/wizard/wizard.py` & `manim_slides-5.1.5/manim_slides/wizard/wizard.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/tests/conftest.py` & `manim_slides-5.1.5/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
 import string
+from collections.abc import Generator, Iterator
 from pathlib import Path
-from typing import Generator, Iterator, List
 
 import pytest
 
 from manim_slides.config import PresentationConfig
 
 
 @pytest.fixture(scope="session")
@@ -61,15 +61,15 @@
     if touch:
         filepath.touch()
 
     return filepath.resolve(strict=touch)
 
 
 @pytest.fixture
-def paths() -> Generator[List[Path], None, None]:
+def paths() -> Generator[list[Path], None, None]:
     random.seed(1234)
 
     yield [random_path() for _ in range(20)]
 
 
 @pytest.fixture(scope="session")
 def presentation_config(
```

### Comparing `manim_slides-5.1.4/tests/data/slides.py` & `manim_slides-5.1.5/tests/data/slides.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/tests/data/slides/BasicSlide.json` & `manim_slides-5.1.5/tests/data/slides/BasicSlide.json`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511.mp4` & `manim_slides-5.1.5/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511_reversed.mp4` & `manim_slides-5.1.5/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511_reversed.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c.mp4` & `manim_slides-5.1.5/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c_reversed.mp4` & `manim_slides-5.1.5/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c_reversed.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077.mp4` & `manim_slides-5.1.5/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077_reversed.mp4` & `manim_slides-5.1.5/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077_reversed.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368.mp4` & `manim_slides-5.1.5/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368_reversed.mp4` & `manim_slides-5.1.5/tests/data/video.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/tests/data/video.mp4` & `manim_slides-5.1.5/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368_reversed.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/tests/data/video_data_uri.txt` & `manim_slides-5.1.5/tests/data/video_data_uri.txt`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/tests/test_base_slide.py` & `manim_slides-5.1.5/tests/test_base_slide.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import MutableMapping
+from collections.abc import MutableMapping
 
 import pytest
 
 from manim_slides.slide.base import BaseSlide
 
 
 @pytest.fixture
```

### Comparing `manim_slides-5.1.4/tests/test_commons.py` & `manim_slides-5.1.5/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/tests/test_config.py` & `manim_slides-5.1.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/tests/test_convert.py` & `manim_slides-5.1.5/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/tests/test_main.py` & `manim_slides-5.1.5/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/tests/test_manim.py` & `manim_slides-5.1.5/tests/test_manim.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
     assert slide.API_NAME == api_name
     assert slide.MANIM == manim
     assert slide.MANIMGL == manimgl
 
 
 def test_force_api() -> None:
+    pytest.importorskip("manimlib")
     import manim  # noqa: F401
 
     if "manimlib" in sys.modules:
         del sys.modules["manimlib"]
 
     os.environ[slide.MANIM_API] = "manimlib"
     os.environ[slide.FORCE_MANIM_API] = "1"
@@ -50,14 +51,15 @@
         )
 
     del os.environ[slide.MANIM_API]
 
 
 @pytest.mark.filterwarnings("ignore:assert_import")
 def test_manim_and_manimgl_imported() -> None:
+    pytest.importorskip("manimlib")
     import manim  # noqa: F401
     import manimlib  # noqa: F401
 
     assert_import(
         api_name="manim",
         manim=True,
         manimgl=False,
@@ -74,14 +76,15 @@
         api_name="manim",
         manim=True,
         manimgl=False,
     )
 
 
 def test_manimgl_imported() -> None:
+    pytest.importorskip("manimlib")
     import manimlib  # noqa: F401
 
     if "manim" in sys.modules:
         del sys.modules["manim"]
 
     assert_import(
         api_name="manimlib",
```

### Comparing `manim_slides-5.1.4/tests/test_present.py` & `manim_slides-5.1.5/tests/test_present.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from collections.abc import Iterator
 from pathlib import Path
-from typing import Iterator, Tuple
 
 import pytest
 from click.testing import CliRunner
 from qtpy.QtWidgets import QApplication
 
 from manim_slides.present import present
 
@@ -16,126 +16,126 @@
     yield
 
     if app := QApplication.instance():
         app.quit()
 
 
 @pytest.fixture(scope="session")
-def args(slides_folder: Path) -> Iterator[Tuple[str, ...]]:
+def args(slides_folder: Path) -> Iterator[tuple[str, ...]]:
     yield ("--folder", str(slides_folder), "--skip-all", "--playback-rate", "25")
 
 
-def test_present(args: Tuple[str, ...]) -> None:
+def test_present(args: tuple[str, ...]) -> None:
     runner = CliRunner()
 
     with runner.isolated_filesystem():
         results = runner.invoke(present, ["BasicSlide", *args])
 
         assert results.exit_code == 0
         assert results.stdout == ""
 
 
-def test_present_unexisting_slide(args: Tuple[str, ...]) -> None:
+def test_present_unexisting_slide(args: tuple[str, ...]) -> None:
     runner = CliRunner()
 
     with runner.isolated_filesystem():
         results = runner.invoke(present, ["UnexistingSlide", *args])
 
         assert results.exit_code != 0
         assert "UnexistingSlide.json does not exist" in results.stdout
 
 
-def test_present_full_screen(args: Tuple[str, ...]) -> None:
+def test_present_full_screen(args: tuple[str, ...]) -> None:
     runner = CliRunner()
 
     with runner.isolated_filesystem():
         results = runner.invoke(present, ["BasicSlide", "--fullscreen", *args])
 
         assert results.exit_code == 0
         assert results.stdout == ""
 
 
-def test_present_hide_mouse(args: Tuple[str, ...]) -> None:
+def test_present_hide_mouse(args: tuple[str, ...]) -> None:
     runner = CliRunner()
 
     with runner.isolated_filesystem():
         results = runner.invoke(present, ["BasicSlide", "--hide-mouse", *args])
 
         assert results.exit_code == 0
         assert results.stdout == ""
 
 
-def test_present_ignore_aspect_ratio(args: Tuple[str, ...]) -> None:
+def test_present_ignore_aspect_ratio(args: tuple[str, ...]) -> None:
     runner = CliRunner()
 
     with runner.isolated_filesystem():
         results = runner.invoke(
             present, ["BasicSlide", "--aspect-ratio", "ignore", *args]
         )
 
         assert results.exit_code == 0
         assert results.stdout == ""
 
 
-def test_present_start_at(args: Tuple[str, ...]) -> None:
+def test_present_start_at(args: tuple[str, ...]) -> None:
     runner = CliRunner()
 
     with runner.isolated_filesystem():
         results = runner.invoke(present, ["BasicSlide", "--start-at", "-1,-1", *args])
 
         assert results.exit_code == 0
         assert results.stdout == ""
 
 
-def test_present_start_at_invalid(args: Tuple[str, ...]) -> None:
+def test_present_start_at_invalid(args: tuple[str, ...]) -> None:
     runner = CliRunner()
 
     with runner.isolated_filesystem():
         results = runner.invoke(present, ["BasicSlide", "--start-at", "0,1234", *args])
 
         assert results.exit_code == 0
         assert "Could not set presentation index to 1234"
 
 
-def test_present_start_at_scene_number(args: Tuple[str, ...]) -> None:
+def test_present_start_at_scene_number(args: tuple[str, ...]) -> None:
     runner = CliRunner()
 
     with runner.isolated_filesystem():
         results = runner.invoke(
             present, ["BasicSlide", "BasicSlide", "--start-at-scene-number", "1", *args]
         )
 
         assert results.exit_code == 0
         assert results.stdout == ""
 
 
-def test_present_start_at_slide_number(args: Tuple[str, ...]) -> None:
+def test_present_start_at_slide_number(args: tuple[str, ...]) -> None:
     runner = CliRunner()
 
     with runner.isolated_filesystem():
         results = runner.invoke(
             present, ["BasicSlide", "--start-at-slide-number", "1", *args]
         )
 
         assert results.exit_code == 0
         assert results.stdout == ""
 
 
-def test_present_set_screen(args: Tuple[str, ...]) -> None:
+def test_present_set_screen(args: tuple[str, ...]) -> None:
     runner = CliRunner()
 
     with runner.isolated_filesystem():
         results = runner.invoke(present, ["BasicSlide", "--screen", "0", *args])
 
         assert results.exit_code == 0
         assert results.stdout == ""
 
 
 @pytest.mark.skip(reason="Fails when running the whole test suite.")
-def test_present_set_invalid_screen(args: Tuple[str, ...]) -> None:
+def test_present_set_invalid_screen(args: tuple[str, ...]) -> None:
     runner = CliRunner()
 
     with runner.isolated_filesystem():
         results = runner.invoke(present, ["BasicSlide", "--screen", "999", *args])
 
         assert results.exit_code == 0
         assert "Invalid screen number 999" in results.stdout
```

### Comparing `manim_slides-5.1.4/tests/test_slide.py` & `manim_slides-5.1.5/tests/test_slide.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import random
 import shutil
+import sys
 from pathlib import Path
 
+import manim
 import numpy as np
 import pytest
 from click.testing import CliRunner
 from manim import (
     BLACK,
     BLUE,
     DOWN,
@@ -31,16 +33,17 @@
 @pytest.mark.parametrize(
     "renderer",
     [
         "--CE",
         pytest.param(
             "--GL",
             marks=pytest.mark.skipif(
-                version.parse(np.__version__) >= version.parse("1.25"),
-                reason="ManimGL requires numpy<1.25, which is outdate",
+                version.parse(np.__version__) >= version.parse("1.25")
+                or sys.version_info >= (3, 12),
+                reason="ManimGL requires numpy<1.25, which is outdated and Python < 3.12",
             ),
         ),
     ],
 )
 def test_render_basic_slide(
     renderer: str,
     slides_file: Path,
@@ -105,14 +108,18 @@
             assert self._output_folder == FOLDER_PATH
             assert len(self._slides) == 0
             assert self._current_slide == 1
             assert self._start_animation == 0
             assert len(self._canvas) == 0
             assert self._wait_time_between_slides == 0.0
 
+    @pytest.mark.skipif(
+        version.parse(manim.__version__) < version.parse("0.18"),
+        reason="Manim change how color are represented in 0.18",
+    )
     @assert_constructs
     class TestBackgroundColor(Slide):
         def construct(self) -> None:
             assert self._background_color == BLACK.to_hex()  # DEFAULT
             self.camera.background_color = BLUE
             assert self._background_color == BLUE.to_hex()
```

### Comparing `manim_slides-5.1.4/tests/test_utils.py` & `manim_slides-5.1.5/tests/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from pathlib import Path
-from typing import List
 
 from manim_slides.utils import merge_basenames
 
 
-def test_merge_basenames(paths: List[Path]) -> None:
+def test_merge_basenames(paths: list[Path]) -> None:
     path = merge_basenames(paths)
     assert path.suffix == paths[0].suffix
     assert path.parent == paths[0].parent
 
 
 def test_merge_basenames_same_with_different_parent_directories(
-    paths: List[Path],
+    paths: list[Path],
 ) -> None:
     d1 = Path("a/b/c")
     d2 = Path("d/e/f")
     p1 = d1 / "one.txt"
     p2 = d1 / "a/b/c/two.txt"
     p3 = d2 / "d/e/f/one.txt"
     p4 = d2 / "d/e/f/two.txt"
```

### Comparing `manim_slides-5.1.4/tests/test_wizard.py` & `manim_slides-5.1.5/tests/test_wizard.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.4/PKG-INFO` & `manim_slides-5.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,92 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: manim-slides
-Version: 5.1.4
+Version: 5.1.5
 Summary: Tool for live presentations using manim
-Keywords: manim,slides,plugin,manimgl
-Author-Email: =?utf-8?q?J=C3=A9rome_Eertmans?= <jeertmans@icloud.com>
+Project-URL: Changelog, https://github.com/jeertmans/manim-slides/releases
+Project-URL: Documentation, https://eertmans.be/manim-slides
+Project-URL: Founding, https://github.com/sponsors/jeertmans
+Project-URL: Homepage, https://github.com/jeertmans/manim-slides
+Project-URL: Repository, https://github.com/jeertmans/manim-slides
+Author-email: Jérome Eertmans <jeertmans@icloud.com>
 License: MIT
+License-File: LICENSE.md
+Keywords: manim,manimgl,plugin,slides
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Multimedia :: Graphics
+Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Scientific/Engineering
-Project-URL: Changelog, https://github.com/jeertmans/manim-slides/releases
-Project-URL: Documentation, https://eertmans.be/manim-slides
-Project-URL: Founding, https://github.com/sponsors/jeertmans
-Project-URL: Homepage, https://github.com/jeertmans/manim-slides
-Project-URL: Repository, https://github.com/jeertmans/manim-slides
-Requires-Python: <3.13,>=3.9
+Requires-Python: >=3.9
 Requires-Dist: av>=9.0.0
-Requires-Dist: click>=8.1.3
 Requires-Dist: click-default-group>=1.2.2
+Requires-Dist: click>=8.1.3
 Requires-Dist: jinja2>=3.1.2
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: numpy>=1.19
 Requires-Dist: pillow>=9.5.0
-Requires-Dist: pydantic>=2.0.1
 Requires-Dist: pydantic-extra-types>=2.0.0
+Requires-Dist: pydantic>=2.0.1
 Requires-Dist: python-pptx>=0.6.21
 Requires-Dist: qtpy>=2.4.1
 Requires-Dist: requests>=2.28.1
 Requires-Dist: rich>=13.3.2
 Requires-Dist: rtoml>=0.9.0
 Requires-Dist: tqdm>=4.64.1
-Requires-Dist: manim-slides[magic,sphinx-directive]; extra == "docs"
-Requires-Dist: furo>=2023.5.20; extra == "docs"
-Requires-Dist: ipykernel>=6.25.1; extra == "docs"
-Requires-Dist: myst-parser>=2.0.0; extra == "docs"
-Requires-Dist: nbsphinx>=0.9.2; extra == "docs"
-Requires-Dist: pandoc>=2.3; extra == "docs"
-Requires-Dist: sphinx>=7.0.1; extra == "docs"
-Requires-Dist: sphinx-click>=4.4.0; extra == "docs"
-Requires-Dist: sphinx-copybutton>=0.5.1; extra == "docs"
-Requires-Dist: sphinxext-opengraph>=0.7.5; extra == "docs"
-Requires-Dist: manim-slides[magic,manim,manimgl,sphinx-directive]; extra == "full"
-Requires-Dist: manim-slides[manim]; extra == "magic"
-Requires-Dist: ipython>=8.12.2; extra == "magic"
-Requires-Dist: manim>=0.17.3; extra == "manim"
-Requires-Dist: manimgl>=1.6.1; extra == "manimgl"
-Requires-Dist: pyqt6>=6.6.1; extra == "pyqt6"
-Requires-Dist: manim-slides[full,pyqt6]; extra == "pyqt6-full"
-Requires-Dist: pyside6<6.5.3,>=6.5.1; python_version < "3.12" and extra == "pyside6"
-Requires-Dist: manim-slides[full,pyside6]; extra == "pyside6-full"
-Requires-Dist: docutils>=0.20.1; extra == "sphinx-directive"
-Requires-Dist: manim-slides[manim]; extra == "sphinx-directive"
 Provides-Extra: docs
+Requires-Dist: docutils>=0.20.1; extra == 'docs'
+Requires-Dist: furo>=2023.5.20; extra == 'docs'
+Requires-Dist: ipykernel>=6.25.1; extra == 'docs'
+Requires-Dist: ipython>=8.12.2; extra == 'docs'
+Requires-Dist: manim>=0.17.3; extra == 'docs'
+Requires-Dist: myst-parser>=2.0.0; extra == 'docs'
+Requires-Dist: nbsphinx>=0.9.2; extra == 'docs'
+Requires-Dist: pandoc>=2.3; extra == 'docs'
+Requires-Dist: sphinx-click>=4.4.0; extra == 'docs'
+Requires-Dist: sphinx-copybutton>=0.5.1; extra == 'docs'
+Requires-Dist: sphinx>=7.0.1; extra == 'docs'
+Requires-Dist: sphinxext-opengraph>=0.7.5; extra == 'docs'
 Provides-Extra: full
+Requires-Dist: docutils>=0.20.1; extra == 'full'
+Requires-Dist: ipython>=8.12.2; extra == 'full'
+Requires-Dist: manim>=0.17.3; extra == 'full'
+Provides-Extra: full-gl
+Requires-Dist: docutils>=0.20.1; extra == 'full-gl'
+Requires-Dist: ipython>=8.12.2; extra == 'full-gl'
+Requires-Dist: manim>=0.17.3; extra == 'full-gl'
+Requires-Dist: manimgl>=1.6.1; (python_version < '3.12') and extra == 'full-gl'
 Provides-Extra: magic
+Requires-Dist: ipython>=8.12.2; extra == 'magic'
+Requires-Dist: manim>=0.17.3; extra == 'magic'
 Provides-Extra: manim
+Requires-Dist: manim>=0.17.3; extra == 'manim'
 Provides-Extra: manimgl
+Requires-Dist: manimgl>=1.6.1; (python_version < '3.12') and extra == 'manimgl'
 Provides-Extra: pyqt6
+Requires-Dist: pyqt6>=6.6.1; extra == 'pyqt6'
 Provides-Extra: pyqt6-full
+Requires-Dist: docutils>=0.20.1; extra == 'pyqt6-full'
+Requires-Dist: ipython>=8.12.2; extra == 'pyqt6-full'
+Requires-Dist: manim>=0.17.3; extra == 'pyqt6-full'
+Requires-Dist: pyqt6>=6.6.1; extra == 'pyqt6-full'
 Provides-Extra: pyside6
+Requires-Dist: pyside6<6.5.3,>=6.5.1; (python_version < '3.12') and extra == 'pyside6'
 Provides-Extra: pyside6-full
+Requires-Dist: docutils>=0.20.1; extra == 'pyside6-full'
+Requires-Dist: ipython>=8.12.2; extra == 'pyside6-full'
+Requires-Dist: manim>=0.17.3; extra == 'pyside6-full'
+Requires-Dist: pyside6<6.5.3,>=6.5.1; (python_version < '3.12') and extra == 'pyside6-full'
 Provides-Extra: sphinx-directive
+Requires-Dist: docutils>=0.20.1; extra == 'sphinx-directive'
+Requires-Dist: manim>=0.17.3; extra == 'sphinx-directive'
 Description-Content-Type: text/markdown
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/jeertmans/manim-slides/main/static/logo_dark_transparent.png">
   <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/jeertmans/manim-slides/main/static/logo_light_transparent.png">
   <img alt="Manim Slides Logo" src="https://raw.githubusercontent.com/jeertmans/manim-slides/main/static/logo.png">
 </picture>
@@ -95,16 +111,15 @@
 > This project extends the work of
 > [`manim-presentation`](https://github.com/galatolofederico/manim-presentation),
 > with a lot more features!
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Comparison with Similar Tools](#comparison-with-similar-tools)
-- [F.A.Q](#faq)
-  * [How to increase quality on Windows](#how-to-increase-quality-on-windows)
+- [F.A.Q](https://eertmans.be/manim-slides/latest/faq.html)
 - [Contributing](#contributing)
   * [Reporting an Issue](#reporting-an-issue)
   * [Seeking for Help](#seeking-for-help)
   * [Contact](#contact)
 
 ## Installation
 
@@ -116,23 +131,23 @@
 ## Usage
 
 <!-- start usage -->
 
 Using Manim Slides is a two-step process:
 1. Render animations using `Slide` (resp. `ThreeDSlide`) as a base class instead
    of `Scene` (resp. `ThreeDScene`), and add calls to `self.next_slide()`
-   everytime you want to create a new slide.
+   every time you want to create a new slide.
 2. Run `manim-slides` on rendered animations and display them like a
    *PowerPoint* presentation.
 
 The documentation is available [online](https://eertmans.be/manim-slides/).
 
 ### Basic Example
 
-Call `self.next_slide()` everytime you want to create a pause between
+Call `self.next_slide()` every time you want to create a pause between
 animations, and `self.next_slide(loop=True)` if you want the next slide to loop
 over animations until the user presses continue:
 
 ```python
 from manim import *  # or: from manimlib import *
 
 from manim_slides import Slide
@@ -185,15 +200,15 @@
 <!-- end more-usage -->
 
 <p align="center">
   <img alt="Example GIF" src="https://raw.githubusercontent.com/jeertmans/manim-slides/main/static/example.gif">
 </p>
 
 For detailed usage documentation, run `manim-slides --help`, or go to the
-[documentation](https://eertmans.be/manim-slides/reference/cli.html).
+[documentation](https://eertmans.be/manim-slides/latest/reference/cli.html).
 
 ## Interactive Tutorial
 
 Click on the image to watch a slides presentation that explains to you how
 to use Manim Slides.
 
 [![Manim Slides Docs](https://raw.githubusercontent.com/jeertmans/manim-slides/main/static/docs.png)](https://eertmans.be/manim-slides/)
@@ -217,35 +232,18 @@
 | Activity | [![GitHub Repo stars](https://img.shields.io/github/last-commit/jeertmans/manim-slides?style=social)](https://github.com/jeertmans/manim-slides) | [![GitHub Repo stars](https://img.shields.io/github/last-commit/galatolofederico/manim-presentation?style=social)](https://github.com/galatolofederico/manim-presentation) | [![GitHub Repo stars](https://img.shields.io/github/last-commit/ManimCommunity/manim_editor?style=social)](https://github.com/ManimCommunity/manim_editor) | [![GitHub Repo stars](https://img.shields.io/github/last-commit/jupyter/notebook?style=social)](https://github.com/jupyter/notebook) |
 | Usage | Command-line | Command-line | Web Browser | Notebook |
 | Note | Requires minimal modif. in scenes files | Requires minimal modif. in scenes files |  Requires the usage of sections, and configuration through graphical interface | Relies on `nbconvert` to create slides from a Notebook |
 | Support for ManimGL | Yes | No | No | No |
 | Web Browser presentations | Yes | No | Yes | No |
 | Offline presentations | Yes, with Qt | Yes, with OpenCV | No | No
 
-## F.A.Q
-
-### How to increase quality on Windows
-
-On Windows platform, one may encounter a lower image resolution than expected.
-Usually, this is observed because Windows rescales every application to
-fit the screen.
-As found by [@arashash](https://github.com/arashash),
-in [#20](https://github.com/jeertmans/manim-slides/issues/20),
-the problem can be addressed by changing the scaling factor to 100%:
-
-<p align="center">
-  <img alt="Windows Fix Scaling" src="https://raw.githubusercontent.com/jeertmans/manim-slides/main/static/windows_quality_fix.png">
-</p>
-
-in *Settings*->*Display*.
-
 ## Contributing
 
 Contributions are more than welcome! Please read through
-[our contributing section](https://eertmans.be/manim-slides/contributing/index.html).
+[our contributing section](https://eertmans.be/manim-slides/latest/contributing/index.html).
 
 ### Reporting an Issue
 
 <!-- start reporting-an-issue -->
 
 If you think you found a bug,
 an error in the documentation,
@@ -269,20 +267,18 @@
 ### Seeking for help
 
 <!-- start seeking-for-help -->
 
 Sometimes, you may have a question about Manim Slides,
 not necessarily an issue.
 
-There are two ways you can reach us for questions:
-
-- via the `Question/Help/Support` topic when
-[choosing an issue template](https://github.com/jeertmans/manim-slides/issues/new/choose);
-- or via
-[GitHub discussions](https://github.com/jeertmans/manim-slides/discussions).
+First, make sure to read the
+[F.A.Q](https://eertmans.be/manim-slides/latest/faq.html) to see if
+your question has already been answered. If not, please follow the
+recommendation (from that page) to reach us for questions.
 
 <!-- end seeking-for-help -->
 
 ### Contact
 
 <!-- start contact -->
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

