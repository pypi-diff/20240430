# Comparing `tmp/python-docx-1.1.0.tar.gz` & `tmp/python_docx-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-docx-1.1.0.tar", last modified: Sat Nov  4 00:21:05 2023, max compression
+gzip compressed data, was "python_docx-1.1.1.tar", last modified: Tue Apr 30 02:58:01 2024, max compression
```

## Comparing `python-docx-1.1.0.tar` & `python_docx-1.1.1.tar`

### file list

```diff
@@ -1,575 +1,576 @@
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.385486 python-docx-1.1.0/
--rw-r--r--   0 scanny     (501) staff       (20)     7070 2023-11-04 00:15:22.000000 python-docx-1.1.0/HISTORY.rst
--rw-r--r--   0 scanny     (501) staff       (20)     1104 2014-03-01 10:03:55.000000 python-docx-1.1.0/LICENSE
--rw-r--r--   0 scanny     (501) staff       (20)      230 2023-11-03 22:06:50.000000 python-docx-1.1.0/MANIFEST.in
--rw-r--r--   0 scanny     (501) staff       (20)     1993 2023-11-04 00:21:05.384641 python-docx-1.1.0/PKG-INFO
--rw-r--r--   0 scanny     (501) staff       (20)      642 2023-10-10 23:50:32.000000 python-docx-1.1.0/README.md
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:04.928335 python-docx-1.1.0/docs/
--rw-r--r--   0 scanny     (501) staff       (20)     5580 2014-03-01 10:03:55.000000 python-docx-1.1.0/docs/Makefile
--rw-r--r--   0 scanny     (501) staff       (20)      939 2014-06-22 21:06:59.000000 python-docx-1.1.0/docs/Session.vim
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:04.929116 python-docx-1.1.0/docs/_static/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python-docx-1.1.0/docs/_static/.gitignore
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:04.932481 python-docx-1.1.0/docs/_static/img/
--rw-r--r--   0 scanny     (501) staff       (20)    77526 2014-03-01 10:03:55.000000 python-docx-1.1.0/docs/_static/img/example-docx-01.png
--rw-r--r--   0 scanny     (501) staff       (20)    56762 2019-01-08 19:22:46.000000 python-docx-1.1.0/docs/_static/img/hdrftr-01.png
--rw-r--r--   0 scanny     (501) staff       (20)    16218 2019-01-08 19:22:46.000000 python-docx-1.1.0/docs/_static/img/hdrftr-02.png
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:04.933553 python-docx-1.1.0/docs/_templates/
--rw-r--r--   0 scanny     (501) staff       (20)      299 2014-03-01 10:03:55.000000 python-docx-1.1.0/docs/_templates/sidebarlinks.html
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:04.878116 python-docx-1.1.0/docs/_themes/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:04.938006 python-docx-1.1.0/docs/_themes/armstrong/
--rw-r--r--   0 scanny     (501) staff       (20)     1164 2014-01-06 15:34:59.000000 python-docx-1.1.0/docs/_themes/armstrong/LICENSE
--rw-r--r--   0 scanny     (501) staff       (20)     1661 2014-01-06 15:34:59.000000 python-docx-1.1.0/docs/_themes/armstrong/layout.html
--rw-r--r--   0 scanny     (501) staff       (20)     1147 2014-01-06 15:34:59.000000 python-docx-1.1.0/docs/_themes/armstrong/rtd-themes.conf
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:04.956468 python-docx-1.1.0/docs/_themes/armstrong/static/
--rw-r--r--   0 scanny     (501) staff       (20)    16885 2014-01-06 15:34:59.000000 python-docx-1.1.0/docs/_themes/armstrong/static/rtd.css_t
--rw-r--r--   0 scanny     (501) staff       (20)     1147 2014-01-06 15:34:59.000000 python-docx-1.1.0/docs/_themes/armstrong/theme.conf
--rw-r--r--   0 scanny     (501) staff       (20)     1400 2014-01-06 15:34:59.000000 python-docx-1.1.0/docs/_themes/armstrong/theme.conf.orig
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:04.965739 python-docx-1.1.0/docs/api/
--rw-r--r--   0 scanny     (501) staff       (20)      255 2015-02-20 05:47:12.000000 python-docx-1.1.0/docs/api/dml.rst
--rw-r--r--   0 scanny     (501) staff       (20)     3363 2023-10-10 23:50:32.000000 python-docx-1.1.0/docs/api/document.rst
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:04.982234 python-docx-1.1.0/docs/api/enum/
--rw-r--r--   0 scanny     (501) staff       (20)      382 2015-02-20 05:47:12.000000 python-docx-1.1.0/docs/api/enum/MsoColorType.rst
--rw-r--r--   0 scanny     (501) staff       (20)     1270 2015-02-20 05:47:12.000000 python-docx-1.1.0/docs/api/enum/MsoThemeColorIndex.rst
--rw-r--r--   0 scanny     (501) staff       (20)      791 2023-09-28 02:22:55.000000 python-docx-1.1.0/docs/api/enum/WdAlignParagraph.rst
--rw-r--r--   0 scanny     (501) staff       (20)     4567 2023-09-28 02:22:55.000000 python-docx-1.1.0/docs/api/enum/WdBuiltinStyle.rst
--rw-r--r--   0 scanny     (501) staff       (20)      804 2023-09-28 02:22:55.000000 python-docx-1.1.0/docs/api/enum/WdCellVerticalAlignment.rst
--rw-r--r--   0 scanny     (501) staff       (20)      692 2023-09-28 02:22:55.000000 python-docx-1.1.0/docs/api/enum/WdColorIndex.rst
--rw-r--r--   0 scanny     (501) staff       (20)      771 2021-05-15 20:54:03.000000 python-docx-1.1.0/docs/api/enum/WdLineSpacing.rst
--rw-r--r--   0 scanny     (501) staff       (20)      339 2023-09-28 02:22:55.000000 python-docx-1.1.0/docs/api/enum/WdOrientation.rst
--rw-r--r--   0 scanny     (501) staff       (20)      336 2015-02-14 04:32:30.000000 python-docx-1.1.0/docs/api/enum/WdRowAlignment.rst
--rw-r--r--   0 scanny     (501) staff       (20)      519 2023-09-28 02:22:55.000000 python-docx-1.1.0/docs/api/enum/WdRowHeightRule.rst
--rw-r--r--   0 scanny     (501) staff       (20)      486 2023-09-28 02:22:55.000000 python-docx-1.1.0/docs/api/enum/WdSectionStart.rst
--rw-r--r--   0 scanny     (501) staff       (20)      421 2015-02-14 04:32:30.000000 python-docx-1.1.0/docs/api/enum/WdStyleType.rst
--rw-r--r--   0 scanny     (501) staff       (20)      434 2018-06-29 17:21:43.000000 python-docx-1.1.0/docs/api/enum/WdTabAlignment.rst
--rw-r--r--   0 scanny     (501) staff       (20)      285 2018-06-29 17:21:43.000000 python-docx-1.1.0/docs/api/enum/WdTabLeader.rst
--rw-r--r--   0 scanny     (501) staff       (20)      495 2015-02-22 01:10:26.000000 python-docx-1.1.0/docs/api/enum/WdTableDirection.rst
--rw-r--r--   0 scanny     (501) staff       (20)     1334 2014-06-22 22:15:58.000000 python-docx-1.1.0/docs/api/enum/WdUnderline.rst
--rw-r--r--   0 scanny     (501) staff       (20)      446 2018-08-18 20:36:40.000000 python-docx-1.1.0/docs/api/enum/index.rst
--rw-r--r--   0 scanny     (501) staff       (20)      565 2019-01-08 19:22:46.000000 python-docx-1.1.0/docs/api/section.rst
--rw-r--r--   0 scanny     (501) staff       (20)      206 2016-03-01 05:04:14.000000 python-docx-1.1.0/docs/api/settings.rst
--rw-r--r--   0 scanny     (501) staff       (20)      613 2015-02-16 22:54:15.000000 python-docx-1.1.0/docs/api/shape.rst
--rw-r--r--   0 scanny     (501) staff       (20)     1174 2023-10-10 23:50:32.000000 python-docx-1.1.0/docs/api/shared.rst
--rw-r--r--   0 scanny     (501) staff       (20)     1804 2023-10-10 23:50:32.000000 python-docx-1.1.0/docs/api/style.rst
--rw-r--r--   0 scanny     (501) staff       (20)      671 2023-11-03 23:58:05.000000 python-docx-1.1.0/docs/api/table.rst
--rw-r--r--   0 scanny     (501) staff       (20)     1008 2023-10-10 23:50:32.000000 python-docx-1.1.0/docs/api/text.rst
--rw-r--r--   0 scanny     (501) staff       (20)    11139 2023-10-10 23:50:32.000000 python-docx-1.1.0/docs/conf.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:04.879364 python-docx-1.1.0/docs/dev/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:04.983609 python-docx-1.1.0/docs/dev/analysis/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:04.988493 python-docx-1.1.0/docs/dev/analysis/features/
--rw-r--r--   0 scanny     (501) staff       (20)     7557 2015-02-14 04:32:30.000000 python-docx-1.1.0/docs/dev/analysis/features/coreprops.rst
--rw-r--r--   0 scanny     (501) staff       (20)    11261 2023-10-10 23:50:32.000000 python-docx-1.1.0/docs/dev/analysis/features/header.rst
--rw-r--r--   0 scanny     (501) staff       (20)     2015 2014-06-22 22:15:58.000000 python-docx-1.1.0/docs/dev/analysis/features/numbering.rst
--rw-r--r--   0 scanny     (501) staff       (20)    10642 2023-10-10 23:50:32.000000 python-docx-1.1.0/docs/dev/analysis/features/sections.rst
--rw-r--r--   0 scanny     (501) staff       (20)    13252 2019-01-08 19:22:46.000000 python-docx-1.1.0/docs/dev/analysis/features/settings.rst
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:04.991283 python-docx-1.1.0/docs/dev/analysis/features/shapes/
--rw-r--r--   0 scanny     (501) staff       (20)     1935 2023-10-10 23:50:32.000000 python-docx-1.1.0/docs/dev/analysis/features/shapes/index.rst
--rw-r--r--   0 scanny     (501) staff       (20)     9428 2021-05-15 21:03:21.000000 python-docx-1.1.0/docs/dev/analysis/features/shapes/picture.rst
--rw-r--r--   0 scanny     (501) staff       (20)     3459 2016-03-01 05:04:14.000000 python-docx-1.1.0/docs/dev/analysis/features/shapes/shapes-inline-size.rst
--rw-r--r--   0 scanny     (501) staff       (20)     6584 2016-03-01 05:04:14.000000 python-docx-1.1.0/docs/dev/analysis/features/shapes/shapes-inline.rst
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:04.995422 python-docx-1.1.0/docs/dev/analysis/features/styles/
--rw-r--r--   0 scanny     (501) staff       (20)     5471 2023-10-10 23:50:32.000000 python-docx-1.1.0/docs/dev/analysis/features/styles/character-style.rst
--rw-r--r--   0 scanny     (501) staff       (20)    12771 2023-10-10 23:50:32.000000 python-docx-1.1.0/docs/dev/analysis/features/styles/index.rst
--rw-r--r--   0 scanny     (501) staff       (20)     8560 2023-10-10 23:50:33.000000 python-docx-1.1.0/docs/dev/analysis/features/styles/latent-styles.rst
--rw-r--r--   0 scanny     (501) staff       (20)     5508 2015-02-14 04:32:30.000000 python-docx-1.1.0/docs/dev/analysis/features/styles/paragraph-style.rst
--rw-r--r--   0 scanny     (501) staff       (20)    13979 2023-10-10 23:50:33.000000 python-docx-1.1.0/docs/dev/analysis/features/styles/style.rst
--rw-r--r--   0 scanny     (501) staff       (20)     8145 2015-02-14 04:32:30.000000 python-docx-1.1.0/docs/dev/analysis/features/styles/styles.rst
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:04.999610 python-docx-1.1.0/docs/dev/analysis/features/table/
--rw-r--r--   0 scanny     (501) staff       (20)    20675 2018-08-18 20:36:40.000000 python-docx-1.1.0/docs/dev/analysis/features/table/cell-merge.rst
--rw-r--r--   0 scanny     (501) staff       (20)     9218 2018-08-18 16:51:00.000000 python-docx-1.1.0/docs/dev/analysis/features/table/index.rst
--rw-r--r--   0 scanny     (501) staff       (20)     8041 2018-08-18 20:36:40.000000 python-docx-1.1.0/docs/dev/analysis/features/table/table-cell.rst
--rw-r--r--   0 scanny     (501) staff       (20)     7949 2023-10-10 23:50:33.000000 python-docx-1.1.0/docs/dev/analysis/features/table/table-props.rst
--rw-r--r--   0 scanny     (501) staff       (20)     4150 2018-08-18 16:51:00.000000 python-docx-1.1.0/docs/dev/analysis/features/table/table-row.rst
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.014854 python-docx-1.1.0/docs/dev/analysis/features/text/
--rw-r--r--   0 scanny     (501) staff       (20)     7581 2015-02-14 04:32:30.000000 python-docx-1.1.0/docs/dev/analysis/features/text/breaks.rst
--rw-r--r--   0 scanny     (501) staff       (20)     9879 2015-02-20 05:47:12.000000 python-docx-1.1.0/docs/dev/analysis/features/text/font-color.rst
--rw-r--r--   0 scanny     (501) staff       (20)     5902 2016-03-14 03:04:58.000000 python-docx-1.1.0/docs/dev/analysis/features/text/font-highlight-color.rst
--rw-r--r--   0 scanny     (501) staff       (20)    18391 2023-10-10 23:50:33.000000 python-docx-1.1.0/docs/dev/analysis/features/text/font.rst
--rw-r--r--   0 scanny     (501) staff       (20)    13033 2023-10-12 23:37:02.000000 python-docx-1.1.0/docs/dev/analysis/features/text/hyperlink.rst
--rw-r--r--   0 scanny     (501) staff       (20)      172 2023-10-10 23:50:33.000000 python-docx-1.1.0/docs/dev/analysis/features/text/index.rst
--rw-r--r--   0 scanny     (501) staff       (20)    16282 2023-10-10 23:50:33.000000 python-docx-1.1.0/docs/dev/analysis/features/text/paragraph-format.rst
--rw-r--r--   0 scanny     (501) staff       (20)     3094 2015-02-14 04:32:30.000000 python-docx-1.1.0/docs/dev/analysis/features/text/run-content.rst
--rw-r--r--   0 scanny     (501) staff       (20)     9567 2018-06-29 17:21:43.000000 python-docx-1.1.0/docs/dev/analysis/features/text/tab-stops.rst
--rw-r--r--   0 scanny     (501) staff       (20)     4247 2015-02-14 04:32:30.000000 python-docx-1.1.0/docs/dev/analysis/features/text/underline.rst
--rw-r--r--   0 scanny     (501) staff       (20)      576 2021-05-16 21:38:14.000000 python-docx-1.1.0/docs/dev/analysis/index.rst
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.017706 python-docx-1.1.0/docs/dev/analysis/schema/
--rw-r--r--   0 scanny     (501) staff       (20)     7226 2014-06-22 22:15:58.000000 python-docx-1.1.0/docs/dev/analysis/schema/ct_body.rst
--rw-r--r--   0 scanny     (501) staff       (20)     4659 2014-06-22 22:15:58.000000 python-docx-1.1.0/docs/dev/analysis/schema/ct_document.rst
--rw-r--r--   0 scanny     (501) staff       (20)     6406 2014-06-27 09:06:09.000000 python-docx-1.1.0/docs/dev/analysis/schema/ct_p.rst
--rw-r--r--   0 scanny     (501) staff       (20)     3824 2019-01-08 19:22:46.000000 python-docx-1.1.0/docs/index.rst
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.026089 python-docx-1.1.0/docs/user/
--rw-r--r--   0 scanny     (501) staff       (20)     1287 2014-01-06 15:34:59.000000 python-docx-1.1.0/docs/user/api-concepts.rst
--rw-r--r--   0 scanny     (501) staff       (20)     3635 2016-05-26 00:56:49.000000 python-docx-1.1.0/docs/user/documents.rst
--rw-r--r--   0 scanny     (501) staff       (20)     6897 2023-10-10 23:50:33.000000 python-docx-1.1.0/docs/user/hdrftr.rst
--rw-r--r--   0 scanny     (501) staff       (20)     1031 2014-03-01 09:49:51.000000 python-docx-1.1.0/docs/user/install.rst
--rw-r--r--   0 scanny     (501) staff       (20)    11875 2023-10-10 23:50:33.000000 python-docx-1.1.0/docs/user/quickstart.rst
--rw-r--r--   0 scanny     (501) staff       (20)     3950 2023-10-10 23:50:33.000000 python-docx-1.1.0/docs/user/sections.rst
--rw-r--r--   0 scanny     (501) staff       (20)     1477 2023-10-10 23:50:33.000000 python-docx-1.1.0/docs/user/shapes.rst
--rw-r--r--   0 scanny     (501) staff       (20)    12392 2023-10-10 23:50:33.000000 python-docx-1.1.0/docs/user/styles-understanding.rst
--rw-r--r--   0 scanny     (501) staff       (20)    13587 2015-02-14 04:32:30.000000 python-docx-1.1.0/docs/user/styles-using.rst
--rw-r--r--   0 scanny     (501) staff       (20)    14125 2023-10-10 23:50:33.000000 python-docx-1.1.0/docs/user/text.rst
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.072657 python-docx-1.1.0/features/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.076247 python-docx-1.1.0/features/_scratch/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.077848 python-docx-1.1.0/features/_scratch/test_out/
--rw-r--r--   0 scanny     (501) staff       (20)     1738 2013-08-15 22:17:06.000000 python-docx-1.1.0/features/_scratch/test_out/[Content_Types].xml
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.078849 python-docx-1.1.0/features/_scratch/test_out/_rels/
--rw-r--r--   0 scanny     (501) staff       (20)      734 2013-08-13 09:49:22.000000 python-docx-1.1.0/features/_scratch/test_out/_rels/.rels
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.080960 python-docx-1.1.0/features/_scratch/test_out/customXml/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.082112 python-docx-1.1.0/features/_scratch/test_out/customXml/_rels/
--rw-r--r--   0 scanny     (501) staff       (20)      295 2013-08-15 22:17:06.000000 python-docx-1.1.0/features/_scratch/test_out/customXml/_rels/item1.xml.rels
--rw-r--r--   0 scanny     (501) staff       (20)      218 2013-08-15 22:17:06.000000 python-docx-1.1.0/features/_scratch/test_out/customXml/item1.xml
--rw-r--r--   0 scanny     (501) staff       (20)      341 2013-08-15 22:17:06.000000 python-docx-1.1.0/features/_scratch/test_out/customXml/itemProps1.xml
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.084373 python-docx-1.1.0/features/_scratch/test_out/docProps/
--rw-r--r--   0 scanny     (501) staff       (20)     1035 2013-08-13 09:49:22.000000 python-docx-1.1.0/features/_scratch/test_out/docProps/app.xml
--rw-r--r--   0 scanny     (501) staff       (20)      806 2013-08-15 22:17:06.000000 python-docx-1.1.0/features/_scratch/test_out/docProps/core.xml
--rw-r--r--   0 scanny     (501) staff       (20)     8324 2013-08-15 22:17:06.000000 python-docx-1.1.0/features/_scratch/test_out/docProps/thumbnail.jpeg
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.091215 python-docx-1.1.0/features/_scratch/test_out/word/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.092073 python-docx-1.1.0/features/_scratch/test_out/word/_rels/
--rw-r--r--   0 scanny     (501) staff       (20)     1227 2013-08-15 22:17:06.000000 python-docx-1.1.0/features/_scratch/test_out/word/_rels/document.xml.rels
--rw-r--r--   0 scanny     (501) staff       (20)     1758 2013-08-15 22:17:06.000000 python-docx-1.1.0/features/_scratch/test_out/word/document.xml
--rw-r--r--   0 scanny     (501) staff       (20)     2552 2013-08-15 22:17:06.000000 python-docx-1.1.0/features/_scratch/test_out/word/fontTable.xml
--rw-r--r--   0 scanny     (501) staff       (20)     5514 2013-08-15 22:17:06.000000 python-docx-1.1.0/features/_scratch/test_out/word/numbering.xml
--rw-r--r--   0 scanny     (501) staff       (20)     2500 2013-08-15 22:17:06.000000 python-docx-1.1.0/features/_scratch/test_out/word/settings.xml
--rw-r--r--   0 scanny     (501) staff       (20)    26716 2013-08-15 22:17:06.000000 python-docx-1.1.0/features/_scratch/test_out/word/styles.xml
--rw-r--r--   0 scanny     (501) staff       (20)    27582 2013-08-15 22:17:06.000000 python-docx-1.1.0/features/_scratch/test_out/word/stylesWithEffects.xml
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.092681 python-docx-1.1.0/features/_scratch/test_out/word/theme/
--rw-r--r--   0 scanny     (501) staff       (20)     7643 2013-08-13 09:49:22.000000 python-docx-1.1.0/features/_scratch/test_out/word/theme/theme1.xml
--rw-r--r--   0 scanny     (501) staff       (20)      431 2013-08-13 09:49:22.000000 python-docx-1.1.0/features/_scratch/test_out/word/webSettings.xml
--rw-r--r--   0 scanny     (501) staff       (20)    36593 2023-11-03 23:55:40.000000 python-docx-1.1.0/features/_scratch/test_out.docx
--rw-r--r--   0 scanny     (501) staff       (20)      476 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/api-open-document.feature
--rw-r--r--   0 scanny     (501) staff       (20)      407 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/blk-add-paragraph.feature
--rw-r--r--   0 scanny     (501) staff       (20)      378 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/blk-add-table.feature
--rw-r--r--   0 scanny     (501) staff       (20)      963 2023-11-03 23:58:05.000000 python-docx-1.1.0/features/blk-iter-inner-content.feature
--rw-r--r--   0 scanny     (501) staff       (20)      428 2021-05-16 21:38:14.000000 python-docx-1.1.0/features/cel-add-table.feature
--rw-r--r--   0 scanny     (501) staff       (20)      343 2021-05-16 21:38:14.000000 python-docx-1.1.0/features/cel-text.feature
--rw-r--r--   0 scanny     (501) staff       (20)      981 2021-05-16 21:38:14.000000 python-docx-1.1.0/features/doc-access-collections.feature
--rw-r--r--   0 scanny     (501) staff       (20)      395 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/doc-access-sections.feature
--rw-r--r--   0 scanny     (501) staff       (20)      840 2015-02-22 01:10:26.000000 python-docx-1.1.0/features/doc-add-heading.feature
--rw-r--r--   0 scanny     (501) staff       (20)      358 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/doc-add-page-break.feature
--rw-r--r--   0 scanny     (501) staff       (20)      883 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/doc-add-paragraph.feature
--rw-r--r--   0 scanny     (501) staff       (20)      997 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/doc-add-picture.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1110 2019-01-08 19:22:46.000000 python-docx-1.1.0/features/doc-add-section.feature
--rw-r--r--   0 scanny     (501) staff       (20)      729 2015-02-22 01:10:26.000000 python-docx-1.1.0/features/doc-add-table.feature
--rw-r--r--   0 scanny     (501) staff       (20)      892 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/doc-coreprops.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1398 2019-01-08 19:22:46.000000 python-docx-1.1.0/features/doc-settings.feature
--rw-r--r--   0 scanny     (501) staff       (20)      598 2016-03-01 05:04:14.000000 python-docx-1.1.0/features/doc-styles.feature
--rw-r--r--   0 scanny     (501) staff       (20)      268 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/environment.py
--rw-r--r--   0 scanny     (501) staff       (20)     3116 2021-05-16 21:38:14.000000 python-docx-1.1.0/features/hdr-header-footer.feature
--rw-r--r--   0 scanny     (501) staff       (20)     2116 2023-10-12 23:37:02.000000 python-docx-1.1.0/features/hlk-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1499 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/img-characterize-image.feature
--rw-r--r--   0 scanny     (501) staff       (20)      402 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/num-access-numbering-part.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1917 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/par-access-inner-content.feature
--rw-r--r--   0 scanny     (501) staff       (20)      312 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/par-access-parfmt.feature
--rw-r--r--   0 scanny     (501) staff       (20)      527 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/par-add-run.feature
--rw-r--r--   0 scanny     (501) staff       (20)      632 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/par-alignment-prop.feature
--rw-r--r--   0 scanny     (501) staff       (20)      405 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/par-clear-paragraph.feature
--rw-r--r--   0 scanny     (501) staff       (20)      577 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/par-insert-paragraph.feature
--rw-r--r--   0 scanny     (501) staff       (20)      390 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/par-set-text.feature
--rw-r--r--   0 scanny     (501) staff       (20)      871 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/par-style-prop.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1101 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/pbk-split-para.feature
--rw-r--r--   0 scanny     (501) staff       (20)      269 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/run-access-font.feature
--rw-r--r--   0 scanny     (501) staff       (20)      945 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/run-access-inner-content.feature
--rw-r--r--   0 scanny     (501) staff       (20)      458 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/run-add-content.feature
--rw-r--r--   0 scanny     (501) staff       (20)      804 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/run-add-picture.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1173 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/run-char-style.feature
--rw-r--r--   0 scanny     (501) staff       (20)      373 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/run-clear-run.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1757 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/run-enum-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)     5276 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/sct-section.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1070 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/shp-inline-shape-access.feature
--rw-r--r--   0 scanny     (501) staff       (20)      575 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/shp-inline-shape-size.feature
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.111234 python-docx-1.1.0/features/steps/
--rw-r--r--   0 scanny     (501) staff       (20)     1661 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/api.py
--rw-r--r--   0 scanny     (501) staff       (20)     3636 2023-11-03 23:58:05.000000 python-docx-1.1.0/features/steps/block.py
--rw-r--r--   0 scanny     (501) staff       (20)     1376 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/cell.py
--rw-r--r--   0 scanny     (501) staff       (20)     4150 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/coreprops.py
--rw-r--r--   0 scanny     (501) staff       (20)     8815 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/document.py
--rw-r--r--   0 scanny     (501) staff       (20)     6797 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/font.py
--rw-r--r--   0 scanny     (501) staff       (20)     5055 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/hdrftr.py
--rw-r--r--   0 scanny     (501) staff       (20)      836 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/helpers.py
--rw-r--r--   0 scanny     (501) staff       (20)     4588 2023-10-12 23:37:02.000000 python-docx-1.1.0/features/steps/hyperlink.py
--rw-r--r--   0 scanny     (501) staff       (20)     2212 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/image.py
--rw-r--r--   0 scanny     (501) staff       (20)      952 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/numbering.py
--rw-r--r--   0 scanny     (501) staff       (20)     6052 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/pagebreak.py
--rw-r--r--   0 scanny     (501) staff       (20)     8975 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/paragraph.py
--rw-r--r--   0 scanny     (501) staff       (20)     7912 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/parfmt.py
--rw-r--r--   0 scanny     (501) staff       (20)     9750 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/section.py
--rw-r--r--   0 scanny     (501) staff       (20)     1842 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/settings.py
--rw-r--r--   0 scanny     (501) staff       (20)     5169 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/shape.py
--rw-r--r--   0 scanny     (501) staff       (20)      544 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/shared.py
--rw-r--r--   0 scanny     (501) staff       (20)    17994 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/styles.py
--rw-r--r--   0 scanny     (501) staff       (20)    15416 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/table.py
--rw-r--r--   0 scanny     (501) staff       (20)     4645 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/tabstops.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.179297 python-docx-1.1.0/features/steps/test_files/
--rw-r--r--   0 scanny     (501) staff       (20)    25142 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/blk-containing-table.docx
--rw-r--r--   0 scanny     (501) staff       (20)    15649 2023-11-03 23:58:05.000000 python-docx-1.1.0/features/steps/test_files/blk-paras-and-tables.docx
--rw-r--r--   0 scanny     (501) staff       (20)    80603 2023-09-10 05:09:30.000000 python-docx-1.1.0/features/steps/test_files/court-exif.jpg
--rw-r--r--   0 scanny     (501) staff       (20)    25591 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/doc-access-sections.docx
--rw-r--r--   0 scanny     (501) staff       (20)    17956 2019-01-08 19:22:46.000000 python-docx-1.1.0/features/steps/test_files/doc-add-section.docx
--rw-r--r--   0 scanny     (501) staff       (20)    11992 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/doc-coreprops.docx
--rw-r--r--   0 scanny     (501) staff       (20)    21366 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/doc-default.docx
--rw-r--r--   0 scanny     (501) staff       (20)    11394 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/doc-no-coreprops.docx
--rw-r--r--   0 scanny     (501) staff       (20)    17711 2019-01-08 19:22:46.000000 python-docx-1.1.0/features/steps/test_files/doc-odd-even-hdrs.docx
--rw-r--r--   0 scanny     (501) staff       (20)    21309 2015-02-22 01:10:26.000000 python-docx-1.1.0/features/steps/test_files/doc-word-default-blank.docx
--rw-r--r--   0 scanny     (501) staff       (20)    15846 2015-02-20 05:47:12.000000 python-docx-1.1.0/features/steps/test_files/fnt-color.docx
--rw-r--r--   0 scanny     (501) staff       (20)    18079 2019-01-08 19:22:46.000000 python-docx-1.1.0/features/steps/test_files/hdr-header-footer.docx
--rw-r--r--   0 scanny     (501) staff       (20)   355196 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/jfif-300-dpi.jpg
--rw-r--r--   0 scanny     (501) staff       (20)   768608 2023-09-10 05:09:16.000000 python-docx-1.1.0/features/steps/test_files/jpeg420exif.jpg
--rw-r--r--   0 scanny     (501) staff       (20)   263222 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/lena.bmp
--rw-r--r--   0 scanny     (501) staff       (20)    72985 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/lena.gif
--rw-r--r--   0 scanny     (501) staff       (20)   786572 2023-09-10 05:09:00.000000 python-docx-1.1.0/features/steps/test_files/lena.tif
--rw-r--r--   0 scanny     (501) staff       (20)   104428 2023-09-10 05:08:43.000000 python-docx-1.1.0/features/steps/test_files/lena_std.jpg
--rw-r--r--   0 scanny     (501) staff       (20)    64276 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/monty-truth.png
--rw-r--r--   0 scanny     (501) staff       (20)   308280 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/mountain.bmp
--rw-r--r--   0 scanny     (501) staff       (20)    24334 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/num-having-numbering-part.docx
--rw-r--r--   0 scanny     (501) staff       (20)    15126 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/par-alignment.docx
--rw-r--r--   0 scanny     (501) staff       (20)    12071 2023-10-12 23:37:02.000000 python-docx-1.1.0/features/steps/test_files/par-hlink-frags.docx
--rw-r--r--   0 scanny     (501) staff       (20)    12385 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/test_files/par-hyperlinks.docx
--rw-r--r--   0 scanny     (501) staff       (20)    27969 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/par-known-paragraphs.docx
--rw-r--r--   0 scanny     (501) staff       (20)    20901 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/par-known-styles.docx
--rw-r--r--   0 scanny     (501) staff       (20)    12244 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/test_files/par-rendered-page-breaks.docx
--rw-r--r--   0 scanny     (501) staff       (20)     3277 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/python-icon.jpeg
--rw-r--r--   0 scanny     (501) staff       (20)    26645 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/run-char-style.docx
--rw-r--r--   0 scanny     (501) staff       (20)    14645 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/run-enumerated-props.docx
--rw-r--r--   0 scanny     (501) staff       (20)    10409 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/sample.tif
--rw-r--r--   0 scanny     (501) staff       (20)    14849 2019-01-08 19:22:46.000000 python-docx-1.1.0/features/steps/test_files/sct-first-page-hdrftr.docx
--rw-r--r--   0 scanny     (501) staff       (20)    12051 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/test_files/sct-inner-content.docx
--rw-r--r--   0 scanny     (501) staff       (20)    28168 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/sct-section-props.docx
--rw-r--r--   0 scanny     (501) staff       (20)    10760 2016-03-01 05:04:14.000000 python-docx-1.1.0/features/steps/test_files/set-no-settings-part.docx
--rw-r--r--   0 scanny     (501) staff       (20)   122610 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/shp-inline-shape-access.docx
--rw-r--r--   0 scanny     (501) staff       (20)    12195 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/sty-behav-props.docx
--rw-r--r--   0 scanny     (501) staff       (20)     8358 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/sty-having-no-styles-part.docx
--rw-r--r--   0 scanny     (501) staff       (20)    21573 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/sty-having-styles-part.docx
--rw-r--r--   0 scanny     (501) staff       (20)    13560 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/sty-known-styles.docx
--rw-r--r--   0 scanny     (501) staff       (20)    13170 2018-06-29 17:21:43.000000 python-docx-1.1.0/features/steps/test_files/tab-stops.docx
--rw-r--r--   0 scanny     (501) staff       (20)    25129 2015-02-22 01:10:26.000000 python-docx-1.1.0/features/steps/test_files/tbl-2x2-table.docx
--rw-r--r--   0 scanny     (501) staff       (20)    36051 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/tbl-cell-access.docx
--rw-r--r--   0 scanny     (501) staff       (20)    13654 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/tbl-col-props.docx
--rw-r--r--   0 scanny     (501) staff       (20)    50294 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/tbl-having-applied-style.docx
--rw-r--r--   0 scanny     (501) staff       (20)    32010 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/tbl-having-tables.docx
--rw-r--r--   0 scanny     (501) staff       (20)    16017 2015-02-22 01:10:26.000000 python-docx-1.1.0/features/steps/test_files/tbl-on-off-props.docx
--rw-r--r--   0 scanny     (501) staff       (20)    20178 2018-08-18 20:36:40.000000 python-docx-1.1.0/features/steps/test_files/tbl-props.docx
--rw-r--r--   0 scanny     (501) staff       (20)   146892 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/test.png
--rw-r--r--   0 scanny     (501) staff       (20)    12859 2016-03-14 03:04:58.000000 python-docx-1.1.0/features/steps/test_files/txt-font-highlight-color.docx
--rw-r--r--   0 scanny     (501) staff       (20)    37924 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/steps/test_files/txt-font-props.docx
--rw-r--r--   0 scanny     (501) staff       (20)    10059 2023-10-10 23:50:33.000000 python-docx-1.1.0/features/steps/text.py
--rw-r--r--   0 scanny     (501) staff       (20)      463 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/sty-access-font.feature
--rw-r--r--   0 scanny     (501) staff       (20)      568 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/sty-access-latent-styles.feature
--rw-r--r--   0 scanny     (501) staff       (20)      488 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/sty-access-parfmt.feature
--rw-r--r--   0 scanny     (501) staff       (20)      767 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/sty-add-style.feature
--rw-r--r--   0 scanny     (501) staff       (20)      352 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/sty-delete-style.feature
--rw-r--r--   0 scanny     (501) staff       (20)      654 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/sty-latent-add-del.feature
--rw-r--r--   0 scanny     (501) staff       (20)     4102 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/sty-latent-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)     5464 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/sty-style-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1264 2018-06-29 17:21:43.000000 python-docx-1.1.0/features/tab-access-tabs.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1877 2018-06-29 17:21:43.000000 python-docx-1.1.0/features/tab-tabstop-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)      594 2015-02-22 01:10:26.000000 python-docx-1.1.0/features/tbl-add-row-or-col.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1523 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/tbl-cell-access.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1861 2021-05-16 21:38:14.000000 python-docx-1.1.0/features/tbl-cell-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1062 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/tbl-col-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)      944 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/tbl-item-access.feature
--rw-r--r--   0 scanny     (501) staff       (20)     2294 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/tbl-merge-cells.feature
--rw-r--r--   0 scanny     (501) staff       (20)     2907 2015-02-22 01:10:26.000000 python-docx-1.1.0/features/tbl-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1665 2018-08-18 16:51:00.000000 python-docx-1.1.0/features/tbl-row-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1169 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/tbl-style.feature
--rw-r--r--   0 scanny     (501) staff       (20)      645 2015-02-19 07:28:57.000000 python-docx-1.1.0/features/txt-add-break.feature
--rw-r--r--   0 scanny     (501) staff       (20)     2279 2015-02-20 05:47:12.000000 python-docx-1.1.0/features/txt-font-color.feature
--rw-r--r--   0 scanny     (501) staff       (20)     8120 2016-03-14 03:04:58.000000 python-docx-1.1.0/features/txt-font-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)     7648 2018-06-29 17:21:43.000000 python-docx-1.1.0/features/txt-parfmt-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)     3235 2023-11-03 23:58:05.000000 python-docx-1.1.0/pyproject.toml
--rw-r--r--   0 scanny     (501) staff       (20)       60 2023-10-10 23:50:33.000000 python-docx-1.1.0/requirements-dev.txt
--rw-r--r--   0 scanny     (501) staff       (20)       51 2023-10-12 23:37:02.000000 python-docx-1.1.0/requirements-docs.txt
--rw-r--r--   0 scanny     (501) staff       (20)       68 2023-10-10 23:50:33.000000 python-docx-1.1.0/requirements-test.txt
--rw-r--r--   0 scanny     (501) staff       (20)       30 2023-10-10 23:50:33.000000 python-docx-1.1.0/requirements.txt
--rw-r--r--   0 scanny     (501) staff       (20)       38 2023-11-04 00:21:05.385662 python-docx-1.1.0/setup.cfg
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:04.893011 python-docx-1.1.0/src/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.188855 python-docx-1.1.0/src/docx/
--rw-r--r--   0 scanny     (501) staff       (20)     1711 2023-11-04 00:15:22.000000 python-docx-1.1.0/src/docx/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     1164 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/api.py
--rw-r--r--   0 scanny     (501) staff       (20)     3550 2023-11-03 23:58:05.000000 python-docx-1.1.0/src/docx/blkcntnr.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.190108 python-docx-1.1.0/src/docx/dml/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/dml/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     3794 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/dml/color.py
--rw-r--r--   0 scanny     (501) staff       (20)     8040 2023-11-03 23:58:05.000000 python-docx-1.1.0/src/docx/document.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.190936 python-docx-1.1.0/src/docx/drawing/
--rw-r--r--   0 scanny     (501) staff       (20)      452 2023-11-03 23:58:05.000000 python-docx-1.1.0/src/docx/drawing/__init__.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.196149 python-docx-1.1.0/src/docx/enum/
--rw-r--r--   0 scanny     (501) staff       (20)      240 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/enum/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     4917 2023-11-03 23:58:05.000000 python-docx-1.1.0/src/docx/enum/base.py
--rw-r--r--   0 scanny     (501) staff       (20)     3346 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/enum/dml.py
--rw-r--r--   0 scanny     (501) staff       (20)     2391 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/enum/section.py
--rw-r--r--   0 scanny     (501) staff       (20)      396 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/enum/shape.py
--rw-r--r--   0 scanny     (501) staff       (20)    10137 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/enum/style.py
--rw-r--r--   0 scanny     (501) staff       (20)     3943 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/enum/table.py
--rw-r--r--   0 scanny     (501) staff       (20)    10276 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/enum/text.py
--rw-r--r--   0 scanny     (501) staff       (20)      454 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/exceptions.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.204040 python-docx-1.1.0/src/docx/image/
--rw-r--r--   0 scanny     (501) staff       (20)      664 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/image/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     1347 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/image/bmp.py
--rw-r--r--   0 scanny     (501) staff       (20)     3466 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/image/constants.py
--rw-r--r--   0 scanny     (501) staff       (20)      383 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/image/exceptions.py
--rw-r--r--   0 scanny     (501) staff       (20)     1118 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/image/gif.py
--rw-r--r--   0 scanny     (501) staff       (20)     3089 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/image/helpers.py
--rw-r--r--   0 scanny     (501) staff       (20)     8044 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/image/image.py
--rw-r--r--   0 scanny     (501) staff       (20)    15422 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/image/jpeg.py
--rw-r--r--   0 scanny     (501) staff       (20)     8214 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/image/png.py
--rw-r--r--   0 scanny     (501) staff       (20)    10470 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/image/tiff.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.214471 python-docx-1.1.0/src/docx/opc/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/opc/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)    19080 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/opc/constants.py
--rw-r--r--   0 scanny     (501) staff       (20)     3134 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/opc/coreprops.py
--rw-r--r--   0 scanny     (501) staff       (20)      264 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/opc/exceptions.py
--rw-r--r--   0 scanny     (501) staff       (20)     8112 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/opc/oxml.py
--rw-r--r--   0 scanny     (501) staff       (20)     8128 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/opc/package.py
--rw-r--r--   0 scanny     (501) staff       (20)     3708 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/opc/packuri.py
--rw-r--r--   0 scanny     (501) staff       (20)     8286 2023-10-12 23:37:02.000000 python-docx-1.1.0/src/docx/opc/part.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.215841 python-docx-1.1.0/src/docx/opc/parts/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/opc/parts/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     1514 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/opc/parts/coreprops.py
--rw-r--r--   0 scanny     (501) staff       (20)     4005 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/opc/phys_pkg.py
--rw-r--r--   0 scanny     (501) staff       (20)     9640 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/opc/pkgreader.py
--rw-r--r--   0 scanny     (501) staff       (20)     4361 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/opc/pkgwriter.py
--rw-r--r--   0 scanny     (501) staff       (20)     5237 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/opc/rel.py
--rw-r--r--   0 scanny     (501) staff       (20)     1471 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/opc/shared.py
--rw-r--r--   0 scanny     (501) staff       (20)      638 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/opc/spec.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.226518 python-docx-1.1.0/src/docx/oxml/
--rw-r--r--   0 scanny     (501) staff       (20)     7929 2023-10-12 23:37:02.000000 python-docx-1.1.0/src/docx/oxml/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     9938 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/oxml/coreprops.py
--rw-r--r--   0 scanny     (501) staff       (20)     3546 2023-11-03 23:58:05.000000 python-docx-1.1.0/src/docx/oxml/document.py
--rw-r--r--   0 scanny     (501) staff       (20)      397 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/oxml/drawing.py
--rw-r--r--   0 scanny     (501) staff       (20)      261 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/oxml/exceptions.py
--rw-r--r--   0 scanny     (501) staff       (20)     3780 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/oxml/ns.py
--rw-r--r--   0 scanny     (501) staff       (20)     3965 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/oxml/numbering.py
--rw-r--r--   0 scanny     (501) staff       (20)     2223 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/oxml/parser.py
--rw-r--r--   0 scanny     (501) staff       (20)    20505 2023-11-03 23:58:05.000000 python-docx-1.1.0/src/docx/oxml/section.py
--rw-r--r--   0 scanny     (501) staff       (20)     3911 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/oxml/settings.py
--rw-r--r--   0 scanny     (501) staff       (20)     8080 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/oxml/shape.py
--rw-r--r--   0 scanny     (501) staff       (20)     1839 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/oxml/shared.py
--rw-r--r--   0 scanny     (501) staff       (20)    10882 2023-11-03 23:58:05.000000 python-docx-1.1.0/src/docx/oxml/simpletypes.py
--rw-r--r--   0 scanny     (501) staff       (20)    10673 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/oxml/styles.py
--rw-r--r--   0 scanny     (501) staff       (20)    27697 2023-11-03 23:58:05.000000 python-docx-1.1.0/src/docx/oxml/table.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.232180 python-docx-1.1.0/src/docx/oxml/text/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/oxml/text/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)    11652 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/oxml/text/font.py
--rw-r--r--   0 scanny     (501) staff       (20)     1428 2023-10-12 23:37:02.000000 python-docx-1.1.0/src/docx/oxml/text/hyperlink.py
--rw-r--r--   0 scanny     (501) staff       (20)    11262 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/oxml/text/pagebreak.py
--rw-r--r--   0 scanny     (501) staff       (20)     3543 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/oxml/text/paragraph.py
--rw-r--r--   0 scanny     (501) staff       (20)    11214 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/oxml/text/parfmt.py
--rw-r--r--   0 scanny     (501) staff       (20)     9688 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/oxml/text/run.py
--rw-r--r--   0 scanny     (501) staff       (20)    25866 2023-11-03 23:58:05.000000 python-docx-1.1.0/src/docx/oxml/xmlchemy.py
--rw-r--r--   0 scanny     (501) staff       (20)     3855 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/package.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.238666 python-docx-1.1.0/src/docx/parts/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/parts/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     5404 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/parts/document.py
--rw-r--r--   0 scanny     (501) staff       (20)     1610 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/parts/hdrftr.py
--rw-r--r--   0 scanny     (501) staff       (20)     2538 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/parts/image.py
--rw-r--r--   0 scanny     (501) staff       (20)     1056 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/parts/numbering.py
--rw-r--r--   0 scanny     (501) staff       (20)     1300 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/parts/settings.py
--rw-r--r--   0 scanny     (501) staff       (20)     3817 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/parts/story.py
--rw-r--r--   0 scanny     (501) staff       (20)     1413 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/parts/styles.py
--rw-r--r--   0 scanny     (501) staff       (20)    18534 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/section.py
--rw-r--r--   0 scanny     (501) staff       (20)      658 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/settings.py
--rw-r--r--   0 scanny     (501) staff       (20)     2658 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/shape.py
--rw-r--r--   0 scanny     (501) staff       (20)    13528 2023-11-03 23:58:05.000000 python-docx-1.1.0/src/docx/shared.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.241646 python-docx-1.1.0/src/docx/styles/
--rw-r--r--   0 scanny     (501) staff       (20)     1406 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/styles/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     7211 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/styles/latent.py
--rw-r--r--   0 scanny     (501) staff       (20)     8051 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/styles/style.py
--rw-r--r--   0 scanny     (501) staff       (20)     5717 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/styles/styles.py
--rw-r--r--   0 scanny     (501) staff       (20)    14289 2023-11-03 23:58:05.000000 python-docx-1.1.0/src/docx/table.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.246612 python-docx-1.1.0/src/docx/templates/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.248153 python-docx-1.1.0/src/docx/templates/default-docx-template/
--rw-r--r--   0 scanny     (501) staff       (20)     1782 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-docx-template/[Content_Types].xml
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.248998 python-docx-1.1.0/src/docx/templates/default-docx-template/_rels/
--rw-r--r--   0 scanny     (501) staff       (20)      748 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-docx-template/_rels/.rels
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.250680 python-docx-1.1.0/src/docx/templates/default-docx-template/customXml/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.251506 python-docx-1.1.0/src/docx/templates/default-docx-template/customXml/_rels/
--rw-r--r--   0 scanny     (501) staff       (20)      300 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-docx-template/customXml/_rels/item1.xml.rels
--rw-r--r--   0 scanny     (501) staff       (20)      262 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-docx-template/customXml/item1.xml
--rw-r--r--   0 scanny     (501) staff       (20)      354 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-docx-template/customXml/itemProps1.xml
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.253960 python-docx-1.1.0/src/docx/templates/default-docx-template/docProps/
--rw-r--r--   0 scanny     (501) staff       (20)     1132 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-docx-template/docProps/app.xml
--rw-r--r--   0 scanny     (501) staff       (20)      753 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-docx-template/docProps/core.xml
--rw-r--r--   0 scanny     (501) staff       (20)     8324 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-docx-template/docProps/thumbnail.jpeg
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.262498 python-docx-1.1.0/src/docx/templates/default-docx-template/word/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.263723 python-docx-1.1.0/src/docx/templates/default-docx-template/word/_rels/
--rw-r--r--   0 scanny     (501) staff       (20)     1253 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-docx-template/word/_rels/document.xml.rels
--rw-r--r--   0 scanny     (501) staff       (20)     1594 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-docx-template/word/document.xml
--rw-r--r--   0 scanny     (501) staff       (20)     2811 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-docx-template/word/fontTable.xml
--rw-r--r--   0 scanny     (501) staff       (20)     6747 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-docx-template/word/numbering.xml
--rw-r--r--   0 scanny     (501) staff       (20)     2749 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-docx-template/word/settings.xml
--rw-r--r--   0 scanny     (501) staff       (20)   438677 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-docx-template/word/styles.xml
--rw-r--r--   0 scanny     (501) staff       (20)   438131 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-docx-template/word/stylesWithEffects.xml
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.264557 python-docx-1.1.0/src/docx/templates/default-docx-template/word/theme/
--rw-r--r--   0 scanny     (501) staff       (20)    10939 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-docx-template/word/theme/theme1.xml
--rw-r--r--   0 scanny     (501) staff       (20)      438 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-docx-template/word/webSettings.xml
--rw-r--r--   0 scanny     (501) staff       (20)     1395 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-footer.xml
--rw-r--r--   0 scanny     (501) staff       (20)     1395 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-header.xml
--rw-r--r--   0 scanny     (501) staff       (20)     1640 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-settings.xml
--rw-r--r--   0 scanny     (501) staff       (20)    15823 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default-styles.xml
--rw-r--r--   0 scanny     (501) staff       (20)    38116 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/templates/default.docx
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.269800 python-docx-1.1.0/src/docx/text/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/text/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)    13653 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/text/font.py
--rw-r--r--   0 scanny     (501) staff       (20)     5226 2023-11-03 23:58:05.000000 python-docx-1.1.0/src/docx/text/hyperlink.py
--rw-r--r--   0 scanny     (501) staff       (20)     4951 2023-11-03 23:58:05.000000 python-docx-1.1.0/src/docx/text/pagebreak.py
--rw-r--r--   0 scanny     (501) staff       (20)     6896 2023-11-03 23:58:05.000000 python-docx-1.1.0/src/docx/text/paragraph.py
--rw-r--r--   0 scanny     (501) staff       (20)    10339 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/text/parfmt.py
--rw-r--r--   0 scanny     (501) staff       (20)     9698 2023-11-03 23:58:05.000000 python-docx-1.1.0/src/docx/text/run.py
--rw-r--r--   0 scanny     (501) staff       (20)     3910 2023-10-10 23:50:33.000000 python-docx-1.1.0/src/docx/text/tabstops.py
--rw-r--r--   0 scanny     (501) staff       (20)      864 2023-11-03 23:58:05.000000 python-docx-1.1.0/src/docx/types.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.272737 python-docx-1.1.0/src/python_docx.egg-info/
--rw-r--r--   0 scanny     (501) staff       (20)     1993 2023-11-04 00:21:04.000000 python-docx-1.1.0/src/python_docx.egg-info/PKG-INFO
--rw-r--r--   0 scanny     (501) staff       (20)    16600 2023-11-04 00:21:04.000000 python-docx-1.1.0/src/python_docx.egg-info/SOURCES.txt
--rw-r--r--   0 scanny     (501) staff       (20)        1 2023-11-04 00:21:04.000000 python-docx-1.1.0/src/python_docx.egg-info/dependency_links.txt
--rw-r--r--   0 scanny     (501) staff       (20)       30 2023-11-04 00:21:04.000000 python-docx-1.1.0/src/python_docx.egg-info/requires.txt
--rw-r--r--   0 scanny     (501) staff       (20)        5 2023-11-04 00:21:04.000000 python-docx-1.1.0/src/python_docx.egg-info/top_level.txt
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.284815 python-docx-1.1.0/tests/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2013-07-29 10:11:43.000000 python-docx-1.1.0/tests/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)      452 2023-11-03 23:58:05.000000 python-docx-1.1.0/tests/conftest.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.286352 python-docx-1.1.0/tests/dml/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2015-02-20 05:47:12.000000 python-docx-1.1.0/tests/dml/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     5437 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/dml/test_color.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.293215 python-docx-1.1.0/tests/image/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/image/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     1108 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/image/test_bmp.py
--rw-r--r--   0 scanny     (501) staff       (20)      960 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/image/test_gif.py
--rw-r--r--   0 scanny     (501) staff       (20)     1569 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/image/test_helpers.py
--rw-r--r--   0 scanny     (501) staff       (20)    11958 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/image/test_image.py
--rw-r--r--   0 scanny     (501) staff       (20)    21556 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/image/test_jpeg.py
--rw-r--r--   0 scanny     (501) staff       (20)    14741 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/image/test_png.py
--rw-r--r--   0 scanny     (501) staff       (20)    14704 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/image/test_tiff.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.302691 python-docx-1.1.0/tests/opc/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/opc/__init__.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.303993 python-docx-1.1.0/tests/opc/parts/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2015-02-14 04:32:30.000000 python-docx-1.1.0/tests/opc/parts/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     1870 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/opc/parts/test_coreprops.py
--rw-r--r--   0 scanny     (501) staff       (20)     7972 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/opc/test_coreprops.py
--rw-r--r--   0 scanny     (501) staff       (20)     4866 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/opc/test_oxml.py
--rw-r--r--   0 scanny     (501) staff       (20)    17018 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/opc/test_package.py
--rw-r--r--   0 scanny     (501) staff       (20)     3313 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/opc/test_packuri.py
--rw-r--r--   0 scanny     (501) staff       (20)    16257 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/opc/test_part.py
--rw-r--r--   0 scanny     (501) staff       (20)     6289 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/opc/test_phys_pkg.py
--rw-r--r--   0 scanny     (501) staff       (20)    19028 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/opc/test_pkgreader.py
--rw-r--r--   0 scanny     (501) staff       (20)     6823 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/opc/test_pkgwriter.py
--rw-r--r--   0 scanny     (501) staff       (20)     9565 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/opc/test_rel.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.306346 python-docx-1.1.0/tests/opc/unitdata/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/opc/unitdata/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     8626 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/opc/unitdata/rels.py
--rw-r--r--   0 scanny     (501) staff       (20)      765 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/opc/unitdata/types.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.315038 python-docx-1.1.0/tests/oxml/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/oxml/__init__.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.317004 python-docx-1.1.0/tests/oxml/parts/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/oxml/parts/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     1432 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/oxml/parts/test_document.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.318608 python-docx-1.1.0/tests/oxml/parts/unitdata/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/oxml/parts/unitdata/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)      388 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/oxml/parts/unitdata/document.py
--rw-r--r--   0 scanny     (501) staff       (20)     4108 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/oxml/test__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)      587 2023-11-03 23:58:05.000000 python-docx-1.1.0/tests/oxml/test_document.py
--rw-r--r--   0 scanny     (501) staff       (20)     1634 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/oxml/test_ns.py
--rw-r--r--   0 scanny     (501) staff       (20)      592 2023-11-03 23:58:05.000000 python-docx-1.1.0/tests/oxml/test_section.py
--rw-r--r--   0 scanny     (501) staff       (20)     1367 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/oxml/test_styles.py
--rw-r--r--   0 scanny     (501) staff       (20)    13820 2023-11-03 23:58:05.000000 python-docx-1.1.0/tests/oxml/test_table.py
--rw-r--r--   0 scanny     (501) staff       (20)    28193 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/oxml/test_xmlchemy.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.321404 python-docx-1.1.0/tests/oxml/text/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2015-02-14 04:32:30.000000 python-docx-1.1.0/tests/oxml/text/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     1481 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/oxml/text/test_hyperlink.py
--rw-r--r--   0 scanny     (501) staff       (20)     1156 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/oxml/text/test_run.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.326357 python-docx-1.1.0/tests/oxml/unitdata/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/oxml/unitdata/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     1172 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/oxml/unitdata/dml.py
--rw-r--r--   0 scanny     (501) staff       (20)      412 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/oxml/unitdata/numbering.py
--rw-r--r--   0 scanny     (501) staff       (20)      893 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/oxml/unitdata/section.py
--rw-r--r--   0 scanny     (501) staff       (20)      677 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/oxml/unitdata/shared.py
--rw-r--r--   0 scanny     (501) staff       (20)      449 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/oxml/unitdata/styles.py
--rw-r--r--   0 scanny     (501) staff       (20)     1424 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/oxml/unitdata/table.py
--rw-r--r--   0 scanny     (501) staff       (20)     3153 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/oxml/unitdata/text.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.332041 python-docx-1.1.0/tests/parts/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/parts/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)    12295 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/parts/test_document.py
--rw-r--r--   0 scanny     (501) staff       (20)     5062 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/parts/test_hdrftr.py
--rw-r--r--   0 scanny     (501) staff       (20)     3945 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/parts/test_image.py
--rw-r--r--   0 scanny     (501) staff       (20)     2580 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/parts/test_numbering.py
--rw-r--r--   0 scanny     (501) staff       (20)     2576 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/parts/test_settings.py
--rw-r--r--   0 scanny     (501) staff       (20)     5270 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/parts/test_story.py
--rw-r--r--   0 scanny     (501) staff       (20)     1695 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/parts/test_styles.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.335077 python-docx-1.1.0/tests/styles/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2015-02-14 04:32:30.000000 python-docx-1.1.0/tests/styles/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)    14144 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/styles/test_latent.py
--rw-r--r--   0 scanny     (501) staff       (20)    20304 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/styles/test_style.py
--rw-r--r--   0 scanny     (501) staff       (20)    14836 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/styles/test_styles.py
--rw-r--r--   0 scanny     (501) staff       (20)     2327 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/test_api.py
--rw-r--r--   0 scanny     (501) staff       (20)     5451 2023-11-03 23:58:05.000000 python-docx-1.1.0/tests/test_blkcntnr.py
--rw-r--r--   0 scanny     (501) staff       (20)    14036 2023-11-03 23:58:05.000000 python-docx-1.1.0/tests/test_document.py
--rw-r--r--   0 scanny     (501) staff       (20)     3188 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/test_enum.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.357698 python-docx-1.1.0/tests/test_files/
--rw-r--r--   0 scanny     (501) staff       (20)   146892 2014-06-27 08:20:06.000000 python-docx-1.1.0/tests/test_files/150-dpi.png
--rw-r--r--   0 scanny     (501) staff       (20)   125824 2023-09-10 05:05:56.000000 python-docx-1.1.0/tests/test_files/300-dpi.TIF
--rw-r--r--   0 scanny     (501) staff       (20)   355196 2014-06-27 08:20:06.000000 python-docx-1.1.0/tests/test_files/300-dpi.jpg
--rw-r--r--   0 scanny     (501) staff       (20)    39921 2014-06-27 08:20:06.000000 python-docx-1.1.0/tests/test_files/300-dpi.png
--rw-r--r--   0 scanny     (501) staff       (20)     9454 2014-06-27 08:20:06.000000 python-docx-1.1.0/tests/test_files/72-dpi.tiff
--rw-r--r--   0 scanny     (501) staff       (20)     1526 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/test_files/CVS_LOGO.WMF
--rw-r--r--   0 scanny     (501) staff       (20)    11949 2023-11-03 23:58:05.000000 python-docx-1.1.0/tests/test_files/blk-inner-content.docx
--rw-r--r--   0 scanny     (501) staff       (20)   768608 2023-09-10 05:05:40.000000 python-docx-1.1.0/tests/test_files/exif-420-dpi.jpg
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.358770 python-docx-1.1.0/tests/test_files/expanded_docx/
--rw-r--r--   0 scanny     (501) staff       (20)     1738 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/test_files/expanded_docx/[Content_Types].xml
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.359446 python-docx-1.1.0/tests/test_files/expanded_docx/_rels/
--rw-r--r--   0 scanny     (501) staff       (20)      734 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/test_files/expanded_docx/_rels/.rels
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.360820 python-docx-1.1.0/tests/test_files/expanded_docx/customXml/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.361692 python-docx-1.1.0/tests/test_files/expanded_docx/customXml/_rels/
--rw-r--r--   0 scanny     (501) staff       (20)      295 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/test_files/expanded_docx/customXml/_rels/item1.xml.rels
--rw-r--r--   0 scanny     (501) staff       (20)      217 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/test_files/expanded_docx/customXml/item1.xml
--rw-r--r--   0 scanny     (501) staff       (20)      340 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/test_files/expanded_docx/customXml/itemProps1.xml
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.363814 python-docx-1.1.0/tests/test_files/expanded_docx/docProps/
--rw-r--r--   0 scanny     (501) staff       (20)     1036 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/test_files/expanded_docx/docProps/app.xml
--rw-r--r--   0 scanny     (501) staff       (20)      802 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/test_files/expanded_docx/docProps/core.xml
--rw-r--r--   0 scanny     (501) staff       (20)    13032 2014-06-27 08:20:06.000000 python-docx-1.1.0/tests/test_files/expanded_docx/docProps/thumbnail.jpeg
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.369800 python-docx-1.1.0/tests/test_files/expanded_docx/word/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.370499 python-docx-1.1.0/tests/test_files/expanded_docx/word/_rels/
--rw-r--r--   0 scanny     (501) staff       (20)     1227 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/test_files/expanded_docx/word/_rels/document.xml.rels
--rw-r--r--   0 scanny     (501) staff       (20)     1819 2023-09-10 05:07:15.000000 python-docx-1.1.0/tests/test_files/expanded_docx/word/document.xml
--rw-r--r--   0 scanny     (501) staff       (20)     2566 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/test_files/expanded_docx/word/fontTable.xml
--rw-r--r--   0 scanny     (501) staff       (20)     5513 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/test_files/expanded_docx/word/numbering.xml
--rw-r--r--   0 scanny     (501) staff       (20)     2520 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/test_files/expanded_docx/word/settings.xml
--rw-r--r--   0 scanny     (501) staff       (20)    26715 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/test_files/expanded_docx/word/styles.xml
--rw-r--r--   0 scanny     (501) staff       (20)    27581 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/test_files/expanded_docx/word/stylesWithEffects.xml
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.371277 python-docx-1.1.0/tests/test_files/expanded_docx/word/theme/
--rw-r--r--   0 scanny     (501) staff       (20)     7642 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/test_files/expanded_docx/word/theme/theme1.xml
--rw-r--r--   0 scanny     (501) staff       (20)      430 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/test_files/expanded_docx/word/webSettings.xml
--rw-r--r--   0 scanny     (501) staff       (20)   132875 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/test_files/having-images.docx
--rw-r--r--   0 scanny     (501) staff       (20)     7958 2014-06-27 08:20:06.000000 python-docx-1.1.0/tests/test_files/jfif-iguana.jpg
--rw-r--r--   0 scanny     (501) staff       (20)    10409 2014-06-27 08:20:06.000000 python-docx-1.1.0/tests/test_files/little-endian.tif
--rw-r--r--   0 scanny     (501) staff       (20)    64276 2014-06-27 08:20:06.000000 python-docx-1.1.0/tests/test_files/monty-truth.png
--rw-r--r--   0 scanny     (501) staff       (20)     3277 2014-06-27 08:20:06.000000 python-docx-1.1.0/tests/test_files/python-icon.jpeg
--rw-r--r--   0 scanny     (501) staff       (20)     2036 2014-06-27 08:20:06.000000 python-docx-1.1.0/tests/test_files/python-icon.png
--rw-r--r--   0 scanny     (501) staff       (20)     6111 2014-06-27 08:20:06.000000 python-docx-1.1.0/tests/test_files/python-powered.png
--rw-r--r--   0 scanny     (501) staff       (20)    45210 2014-06-27 08:20:06.000000 python-docx-1.1.0/tests/test_files/python.bmp
--rw-r--r--   0 scanny     (501) staff       (20)    12051 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/test_files/sct-inner-content.docx
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.373862 python-docx-1.1.0/tests/test_files/snippets/
--rw-r--r--   0 scanny     (501) staff       (20)     2949 2015-02-22 01:10:26.000000 python-docx-1.1.0/tests/test_files/snippets/add-row-col.txt
--rw-r--r--   0 scanny     (501) staff       (20)     1110 2015-02-16 22:54:15.000000 python-docx-1.1.0/tests/test_files/snippets/inline.txt
--rw-r--r--   0 scanny     (501) staff       (20)     1756 2015-02-22 01:10:26.000000 python-docx-1.1.0/tests/test_files/snippets/new-tbl.txt
--rw-r--r--   0 scanny     (501) staff       (20)     4595 2015-02-14 04:32:30.000000 python-docx-1.1.0/tests/test_files/snippets/tbl-cells.txt
--rw-r--r--   0 scanny     (501) staff       (20)    33273 2014-06-27 08:20:06.000000 python-docx-1.1.0/tests/test_files/sonic.gif
--rw-r--r--   0 scanny     (501) staff       (20)    31773 2014-03-01 10:03:55.000000 python-docx-1.1.0/tests/test_files/test.docx
--rw-r--r--   0 scanny     (501) staff       (20)     5297 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/test_package.py
--rw-r--r--   0 scanny     (501) staff       (20)    31223 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/test_section.py
--rw-r--r--   0 scanny     (501) staff       (20)     2169 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/test_settings.py
--rw-r--r--   0 scanny     (501) staff       (20)     6785 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/test_shape.py
--rw-r--r--   0 scanny     (501) staff       (20)     4385 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/test_shared.py
--rw-r--r--   0 scanny     (501) staff       (20)    34948 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/test_table.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.380528 python-docx-1.1.0/tests/text/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2015-02-14 04:32:30.000000 python-docx-1.1.0/tests/text/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)    15804 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/text/test_font.py
--rw-r--r--   0 scanny     (501) staff       (20)     5192 2023-11-03 23:58:05.000000 python-docx-1.1.0/tests/text/test_hyperlink.py
--rw-r--r--   0 scanny     (501) staff       (20)     5407 2023-11-03 23:58:05.000000 python-docx-1.1.0/tests/text/test_pagebreak.py
--rw-r--r--   0 scanny     (501) staff       (20)    14897 2023-11-03 23:58:05.000000 python-docx-1.1.0/tests/text/test_paragraph.py
--rw-r--r--   0 scanny     (501) staff       (20)    19674 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/text/test_parfmt.py
--rw-r--r--   0 scanny     (501) staff       (20)    15221 2023-11-03 23:58:05.000000 python-docx-1.1.0/tests/text/test_run.py
--rw-r--r--   0 scanny     (501) staff       (20)    11626 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/text/test_tabstops.py
--rw-r--r--   0 scanny     (501) staff       (20)     4186 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/unitdata.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2023-11-04 00:21:05.383360 python-docx-1.1.0/tests/unitutil/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2014-07-12 04:34:21.000000 python-docx-1.1.0/tests/unitutil/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     8157 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/unitutil/cxml.py
--rw-r--r--   0 scanny     (501) staff       (20)     1675 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/unitutil/file.py
--rw-r--r--   0 scanny     (501) staff       (20)     4741 2023-10-10 23:50:33.000000 python-docx-1.1.0/tests/unitutil/mock.py
--rw-r--r--   0 scanny     (501) staff       (20)      165 2023-10-10 23:50:33.000000 python-docx-1.1.0/tox.ini
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.649204 python_docx-1.1.1/
+-rw-r--r--   0 scanny     (501) staff       (20)     7288 2024-04-30 02:51:57.000000 python_docx-1.1.1/HISTORY.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     1104 2014-03-01 10:03:55.000000 python_docx-1.1.1/LICENSE
+-rw-r--r--   0 scanny     (501) staff       (20)      230 2023-11-04 03:19:46.000000 python_docx-1.1.1/MANIFEST.in
+-rw-r--r--   0 scanny     (501) staff       (20)     2008 2024-04-30 02:58:01.648824 python_docx-1.1.1/PKG-INFO
+-rw-r--r--   0 scanny     (501) staff       (20)      642 2023-11-04 03:19:46.000000 python_docx-1.1.1/README.md
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.555899 python_docx-1.1.1/docs/
+-rw-r--r--   0 scanny     (501) staff       (20)     5580 2014-03-01 10:03:55.000000 python_docx-1.1.1/docs/Makefile
+-rw-r--r--   0 scanny     (501) staff       (20)      939 2014-06-22 21:06:59.000000 python_docx-1.1.1/docs/Session.vim
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.556069 python_docx-1.1.1/docs/_static/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.1/docs/_static/.gitignore
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.556631 python_docx-1.1.1/docs/_static/img/
+-rw-r--r--   0 scanny     (501) staff       (20)    77526 2014-03-01 10:03:55.000000 python_docx-1.1.1/docs/_static/img/example-docx-01.png
+-rw-r--r--   0 scanny     (501) staff       (20)    56762 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/_static/img/hdrftr-01.png
+-rw-r--r--   0 scanny     (501) staff       (20)    16218 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/_static/img/hdrftr-02.png
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.556856 python_docx-1.1.1/docs/_templates/
+-rw-r--r--   0 scanny     (501) staff       (20)      299 2014-03-01 10:03:55.000000 python_docx-1.1.1/docs/_templates/sidebarlinks.html
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.547249 python_docx-1.1.1/docs/_themes/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.557621 python_docx-1.1.1/docs/_themes/armstrong/
+-rw-r--r--   0 scanny     (501) staff       (20)     1164 2014-01-06 15:34:59.000000 python_docx-1.1.1/docs/_themes/armstrong/LICENSE
+-rw-r--r--   0 scanny     (501) staff       (20)     1661 2014-01-06 15:34:59.000000 python_docx-1.1.1/docs/_themes/armstrong/layout.html
+-rw-r--r--   0 scanny     (501) staff       (20)     1147 2014-01-06 15:34:59.000000 python_docx-1.1.1/docs/_themes/armstrong/rtd-themes.conf
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.557757 python_docx-1.1.1/docs/_themes/armstrong/static/
+-rw-r--r--   0 scanny     (501) staff       (20)    16885 2014-01-06 15:34:59.000000 python_docx-1.1.1/docs/_themes/armstrong/static/rtd.css_t
+-rw-r--r--   0 scanny     (501) staff       (20)     1147 2014-01-06 15:34:59.000000 python_docx-1.1.1/docs/_themes/armstrong/theme.conf
+-rw-r--r--   0 scanny     (501) staff       (20)     1400 2014-01-06 15:34:59.000000 python_docx-1.1.1/docs/_themes/armstrong/theme.conf.orig
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.559277 python_docx-1.1.1/docs/api/
+-rw-r--r--   0 scanny     (501) staff       (20)      255 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/dml.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     3363 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/document.rst
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.561700 python_docx-1.1.1/docs/api/enum/
+-rw-r--r--   0 scanny     (501) staff       (20)      382 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/MsoColorType.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     1270 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/MsoThemeColorIndex.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      791 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdAlignParagraph.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     4567 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdBuiltinStyle.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      804 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdCellVerticalAlignment.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      692 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdColorIndex.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      771 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdLineSpacing.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      339 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdOrientation.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      336 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdRowAlignment.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      519 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdRowHeightRule.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      486 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdSectionStart.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      421 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdStyleType.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      434 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdTabAlignment.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      285 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdTabLeader.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      495 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdTableDirection.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     1334 2014-06-22 22:15:58.000000 python_docx-1.1.1/docs/api/enum/WdUnderline.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      446 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/index.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      565 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/section.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      206 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/settings.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      613 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/shape.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     1174 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/shared.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     1804 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/style.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      671 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/table.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     1008 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/text.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    11139 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/conf.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.547753 python_docx-1.1.1/docs/dev/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.561856 python_docx-1.1.1/docs/dev/analysis/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.562605 python_docx-1.1.1/docs/dev/analysis/features/
+-rw-r--r--   0 scanny     (501) staff       (20)     7557 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/coreprops.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    11261 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/header.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     2015 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/numbering.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    10642 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/sections.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    13252 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/settings.rst
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.563273 python_docx-1.1.1/docs/dev/analysis/features/shapes/
+-rw-r--r--   0 scanny     (501) staff       (20)     1935 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/shapes/index.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     9428 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/shapes/picture.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     3459 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/shapes/shapes-inline-size.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     6584 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/shapes/shapes-inline.rst
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.564256 python_docx-1.1.1/docs/dev/analysis/features/styles/
+-rw-r--r--   0 scanny     (501) staff       (20)     5471 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/styles/character-style.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    12771 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/styles/index.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     8560 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/styles/latent-styles.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     5508 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/styles/paragraph-style.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    13979 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/styles/style.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     8145 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/styles/styles.rst
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.565008 python_docx-1.1.1/docs/dev/analysis/features/table/
+-rw-r--r--   0 scanny     (501) staff       (20)    20675 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/table/cell-merge.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     9218 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/table/index.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     8041 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/table/table-cell.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     7949 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/table/table-props.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     4150 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/table/table-row.rst
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.566561 python_docx-1.1.1/docs/dev/analysis/features/text/
+-rw-r--r--   0 scanny     (501) staff       (20)     7581 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/text/breaks.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     9879 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/text/font-color.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     5902 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/text/font-highlight-color.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    18391 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/text/font.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    13033 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/text/hyperlink.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      172 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/text/index.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    16282 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/text/paragraph-format.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     3094 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/text/run-content.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     9567 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/text/tab-stops.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     4247 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/text/underline.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      576 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/index.rst
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.566982 python_docx-1.1.1/docs/dev/analysis/schema/
+-rw-r--r--   0 scanny     (501) staff       (20)     7226 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/schema/ct_body.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     4659 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/schema/ct_document.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     6406 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/schema/ct_p.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     3839 2024-04-30 00:55:22.000000 python_docx-1.1.1/docs/index.rst
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.568626 python_docx-1.1.1/docs/user/
+-rw-r--r--   0 scanny     (501) staff       (20)     1287 2014-01-06 15:34:59.000000 python_docx-1.1.1/docs/user/api-concepts.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     3635 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/user/documents.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     6897 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/user/hdrftr.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     1031 2014-03-01 09:49:51.000000 python_docx-1.1.1/docs/user/install.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    11875 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/user/quickstart.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     3950 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/user/sections.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     1477 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/user/shapes.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    12392 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/user/styles-understanding.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    13587 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/user/styles-using.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     6981 2024-04-30 00:55:22.000000 python_docx-1.1.1/docs/user/tables.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    14125 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/user/text.rst
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.578871 python_docx-1.1.1/features/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.579016 python_docx-1.1.1/features/_scratch/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.579223 python_docx-1.1.1/features/_scratch/test_out/
+-rw-r--r--   0 scanny     (501) staff       (20)     1738 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/[Content_Types].xml
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.579374 python_docx-1.1.1/features/_scratch/test_out/_rels/
+-rw-r--r--   0 scanny     (501) staff       (20)      734 2013-08-13 09:49:22.000000 python_docx-1.1.1/features/_scratch/test_out/_rels/.rels
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.579656 python_docx-1.1.1/features/_scratch/test_out/customXml/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.579806 python_docx-1.1.1/features/_scratch/test_out/customXml/_rels/
+-rw-r--r--   0 scanny     (501) staff       (20)      295 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/customXml/_rels/item1.xml.rels
+-rw-r--r--   0 scanny     (501) staff       (20)      218 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/customXml/item1.xml
+-rw-r--r--   0 scanny     (501) staff       (20)      341 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/customXml/itemProps1.xml
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.580254 python_docx-1.1.1/features/_scratch/test_out/docProps/
+-rw-r--r--   0 scanny     (501) staff       (20)     1035 2013-08-13 09:49:22.000000 python_docx-1.1.1/features/_scratch/test_out/docProps/app.xml
+-rw-r--r--   0 scanny     (501) staff       (20)      806 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/docProps/core.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     8324 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/docProps/thumbnail.jpeg
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.581427 python_docx-1.1.1/features/_scratch/test_out/word/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.581576 python_docx-1.1.1/features/_scratch/test_out/word/_rels/
+-rw-r--r--   0 scanny     (501) staff       (20)     1227 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/word/_rels/document.xml.rels
+-rw-r--r--   0 scanny     (501) staff       (20)     1758 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/word/document.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     2552 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/word/fontTable.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     5514 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/word/numbering.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     2500 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/word/settings.xml
+-rw-r--r--   0 scanny     (501) staff       (20)    26716 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/word/styles.xml
+-rw-r--r--   0 scanny     (501) staff       (20)    27582 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/word/stylesWithEffects.xml
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.581728 python_docx-1.1.1/features/_scratch/test_out/word/theme/
+-rw-r--r--   0 scanny     (501) staff       (20)     7643 2013-08-13 09:49:22.000000 python_docx-1.1.1/features/_scratch/test_out/word/theme/theme1.xml
+-rw-r--r--   0 scanny     (501) staff       (20)      431 2013-08-13 09:49:22.000000 python_docx-1.1.1/features/_scratch/test_out/word/webSettings.xml
+-rw-r--r--   0 scanny     (501) staff       (20)    36593 2024-04-30 02:52:59.000000 python_docx-1.1.1/features/_scratch/test_out.docx
+-rw-r--r--   0 scanny     (501) staff       (20)      476 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/api-open-document.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      407 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/blk-add-paragraph.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      378 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/blk-add-table.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      963 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/blk-iter-inner-content.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      981 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-access-collections.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      395 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-access-sections.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      840 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-add-heading.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      358 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-add-page-break.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      883 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-add-paragraph.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      997 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-add-picture.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1110 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-add-section.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      729 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-add-table.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      892 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-coreprops.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1398 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-settings.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      598 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-styles.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      268 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/environment.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3116 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/hdr-header-footer.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     2116 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/hlk-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1499 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/img-characterize-image.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      402 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/num-access-numbering-part.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1917 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/par-access-inner-content.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      312 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/par-access-parfmt.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      527 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/par-add-run.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      632 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/par-alignment-prop.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      405 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/par-clear-paragraph.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      577 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/par-insert-paragraph.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      390 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/par-set-text.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      871 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/par-style-prop.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1101 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/pbk-split-para.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      269 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/run-access-font.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      945 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/run-access-inner-content.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      458 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/run-add-content.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      804 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/run-add-picture.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1173 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/run-char-style.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      373 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/run-clear-run.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1757 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/run-enum-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     5276 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/sct-section.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1070 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/shp-inline-shape-access.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      575 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/shp-inline-shape-size.feature
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.584859 python_docx-1.1.1/features/steps/
+-rw-r--r--   0 scanny     (501) staff       (20)     1661 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/api.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3636 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/block.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4150 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/coreprops.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8815 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/document.py
+-rw-r--r--   0 scanny     (501) staff       (20)     6797 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/font.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5055 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/hdrftr.py
+-rw-r--r--   0 scanny     (501) staff       (20)      836 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/helpers.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4588 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/hyperlink.py
+-rw-r--r--   0 scanny     (501) staff       (20)     2212 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/image.py
+-rw-r--r--   0 scanny     (501) staff       (20)      952 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/numbering.py
+-rw-r--r--   0 scanny     (501) staff       (20)     6052 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/pagebreak.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8975 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/paragraph.py
+-rw-r--r--   0 scanny     (501) staff       (20)     7912 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/parfmt.py
+-rw-r--r--   0 scanny     (501) staff       (20)     9750 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/section.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1842 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/settings.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5169 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/shape.py
+-rw-r--r--   0 scanny     (501) staff       (20)      544 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/shared.py
+-rw-r--r--   0 scanny     (501) staff       (20)    17994 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/styles.py
+-rw-r--r--   0 scanny     (501) staff       (20)    18911 2024-04-30 02:48:37.000000 python_docx-1.1.1/features/steps/table.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4645 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/tabstops.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.597490 python_docx-1.1.1/features/steps/test_files/
+-rw-r--r--   0 scanny     (501) staff       (20)    25142 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/blk-containing-table.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    15649 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/blk-paras-and-tables.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    80603 2023-09-10 05:09:30.000000 python_docx-1.1.1/features/steps/test_files/court-exif.jpg
+-rw-r--r--   0 scanny     (501) staff       (20)    25591 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/doc-access-sections.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    17956 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/doc-add-section.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    11992 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/doc-coreprops.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    21366 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/doc-default.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    11394 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/doc-no-coreprops.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    17711 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/doc-odd-even-hdrs.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    21309 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/doc-word-default-blank.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    15846 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/fnt-color.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    18079 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/hdr-header-footer.docx
+-rw-r--r--   0 scanny     (501) staff       (20)   355196 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/jfif-300-dpi.jpg
+-rw-r--r--   0 scanny     (501) staff       (20)   768608 2023-09-10 05:09:16.000000 python_docx-1.1.1/features/steps/test_files/jpeg420exif.jpg
+-rw-r--r--   0 scanny     (501) staff       (20)   263222 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/lena.bmp
+-rw-r--r--   0 scanny     (501) staff       (20)    72985 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/lena.gif
+-rw-r--r--   0 scanny     (501) staff       (20)   786572 2023-09-10 05:09:00.000000 python_docx-1.1.1/features/steps/test_files/lena.tif
+-rw-r--r--   0 scanny     (501) staff       (20)   104428 2023-09-10 05:08:43.000000 python_docx-1.1.1/features/steps/test_files/lena_std.jpg
+-rw-r--r--   0 scanny     (501) staff       (20)    64276 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/monty-truth.png
+-rw-r--r--   0 scanny     (501) staff       (20)   308280 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/mountain.bmp
+-rw-r--r--   0 scanny     (501) staff       (20)    24334 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/num-having-numbering-part.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    15126 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/par-alignment.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    12071 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/par-hlink-frags.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    12385 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/par-hyperlinks.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    27969 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/par-known-paragraphs.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    20901 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/par-known-styles.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    12244 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/par-rendered-page-breaks.docx
+-rw-r--r--   0 scanny     (501) staff       (20)     3277 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/python-icon.jpeg
+-rw-r--r--   0 scanny     (501) staff       (20)    26645 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/run-char-style.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    14645 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/run-enumerated-props.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    10409 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/sample.tif
+-rw-r--r--   0 scanny     (501) staff       (20)    14849 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/sct-first-page-hdrftr.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    12051 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/sct-inner-content.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    28168 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/sct-section-props.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    10760 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/set-no-settings-part.docx
+-rw-r--r--   0 scanny     (501) staff       (20)   122610 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/shp-inline-shape-access.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    12195 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/sty-behav-props.docx
+-rw-r--r--   0 scanny     (501) staff       (20)     8358 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/sty-having-no-styles-part.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    21573 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/sty-having-styles-part.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    13560 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/sty-known-styles.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    13170 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/tab-stops.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    25129 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/tbl-2x2-table.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    36051 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/tbl-cell-access.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    13773 2024-04-30 02:48:37.000000 python_docx-1.1.1/features/steps/test_files/tbl-cell-props.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    13654 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/tbl-col-props.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    50294 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/tbl-having-applied-style.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    32010 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/tbl-having-tables.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    16017 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/tbl-on-off-props.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    20419 2024-04-30 00:55:22.000000 python_docx-1.1.1/features/steps/test_files/tbl-props.docx
+-rw-r--r--   0 scanny     (501) staff       (20)   146892 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/test.png
+-rw-r--r--   0 scanny     (501) staff       (20)    12859 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/txt-font-highlight-color.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    37924 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/txt-font-props.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    10059 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/text.py
+-rw-r--r--   0 scanny     (501) staff       (20)      463 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/sty-access-font.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      568 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/sty-access-latent-styles.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      488 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/sty-access-parfmt.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      767 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/sty-add-style.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      352 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/sty-delete-style.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      654 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/sty-latent-add-del.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     4102 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/sty-latent-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     5464 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/sty-style-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1264 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/tab-access-tabs.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1877 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/tab-tabstop-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      594 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/tbl-add-row-or-col.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1523 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/tbl-cell-access.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      428 2024-04-30 00:55:22.000000 python_docx-1.1.1/features/tbl-cell-add-table.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     2105 2024-04-30 02:48:37.000000 python_docx-1.1.1/features/tbl-cell-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      343 2024-04-30 00:55:22.000000 python_docx-1.1.1/features/tbl-cell-text.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1062 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/tbl-col-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      944 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/tbl-item-access.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     2294 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/tbl-merge-cells.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     2907 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/tbl-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     2188 2024-04-30 00:55:22.000000 python_docx-1.1.1/features/tbl-row-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1169 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/tbl-style.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      645 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/txt-add-break.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     2279 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/txt-font-color.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     8120 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/txt-font-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     7648 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/txt-parfmt-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     3309 2024-04-30 02:48:37.000000 python_docx-1.1.1/pyproject.toml
+-rw-r--r--   0 scanny     (501) staff       (20)       76 2024-04-30 00:55:22.000000 python_docx-1.1.1/requirements-dev.txt
+-rw-r--r--   0 scanny     (501) staff       (20)       68 2024-04-30 02:48:37.000000 python_docx-1.1.1/requirements-docs.txt
+-rw-r--r--   0 scanny     (501) staff       (20)       81 2024-04-30 00:55:22.000000 python_docx-1.1.1/requirements-test.txt
+-rw-r--r--   0 scanny     (501) staff       (20)       30 2023-11-04 03:19:46.000000 python_docx-1.1.1/requirements.txt
+-rw-r--r--   0 scanny     (501) staff       (20)       38 2024-04-30 02:58:01.649285 python_docx-1.1.1/setup.cfg
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.551441 python_docx-1.1.1/src/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.601019 python_docx-1.1.1/src/docx/
+-rw-r--r--   0 scanny     (501) staff       (20)     1711 2024-04-30 02:51:57.000000 python_docx-1.1.1/src/docx/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1350 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/api.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3469 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/blkcntnr.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.601407 python_docx-1.1.1/src/docx/dml/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/dml/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3794 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/dml/color.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8021 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/document.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.601686 python_docx-1.1.1/src/docx/drawing/
+-rw-r--r--   0 scanny     (501) staff       (20)      504 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/drawing/__init__.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.603264 python_docx-1.1.1/src/docx/enum/
+-rw-r--r--   0 scanny     (501) staff       (20)      240 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/enum/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4888 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/enum/base.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3346 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/enum/dml.py
+-rw-r--r--   0 scanny     (501) staff       (20)     2391 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/enum/section.py
+-rw-r--r--   0 scanny     (501) staff       (20)      396 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/enum/shape.py
+-rw-r--r--   0 scanny     (501) staff       (20)    10137 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/enum/style.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3943 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/enum/table.py
+-rw-r--r--   0 scanny     (501) staff       (20)    10276 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/enum/text.py
+-rw-r--r--   0 scanny     (501) staff       (20)      454 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/exceptions.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.605582 python_docx-1.1.1/src/docx/image/
+-rw-r--r--   0 scanny     (501) staff       (20)      664 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/image/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1347 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/image/bmp.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3466 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/image/constants.py
+-rw-r--r--   0 scanny     (501) staff       (20)      383 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/image/exceptions.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1118 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/image/gif.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3089 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/image/helpers.py
+-rw-r--r--   0 scanny     (501) staff       (20)     7993 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/image/image.py
+-rw-r--r--   0 scanny     (501) staff       (20)    15422 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/image/jpeg.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8214 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/image/png.py
+-rw-r--r--   0 scanny     (501) staff       (20)    10379 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/image/tiff.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.608833 python_docx-1.1.1/src/docx/opc/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/opc/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)    19080 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/opc/constants.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3134 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/opc/coreprops.py
+-rw-r--r--   0 scanny     (501) staff       (20)      264 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/opc/exceptions.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8126 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/opc/oxml.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8425 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/opc/package.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3708 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/opc/packuri.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8388 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/opc/part.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.609175 python_docx-1.1.1/src/docx/opc/parts/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/opc/parts/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1514 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/opc/parts/coreprops.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4005 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/opc/phys_pkg.py
+-rw-r--r--   0 scanny     (501) staff       (20)     9640 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/opc/pkgreader.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4524 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/opc/pkgwriter.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5389 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/opc/rel.py
+-rw-r--r--   0 scanny     (501) staff       (20)      996 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/opc/shared.py
+-rw-r--r--   0 scanny     (501) staff       (20)      638 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/opc/spec.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.612331 python_docx-1.1.1/src/docx/oxml/
+-rw-r--r--   0 scanny     (501) staff       (20)     8100 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/oxml/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     9938 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/oxml/coreprops.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3543 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/oxml/document.py
+-rw-r--r--   0 scanny     (501) staff       (20)      397 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/oxml/drawing.py
+-rw-r--r--   0 scanny     (501) staff       (20)      261 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/oxml/exceptions.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3796 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/oxml/ns.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3965 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/oxml/numbering.py
+-rw-r--r--   0 scanny     (501) staff       (20)     2316 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/oxml/parser.py
+-rw-r--r--   0 scanny     (501) staff       (20)    20395 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/oxml/section.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3911 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/oxml/settings.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8080 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/oxml/shape.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1871 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/oxml/shared.py
+-rw-r--r--   0 scanny     (501) staff       (20)    10834 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/oxml/simpletypes.py
+-rw-r--r--   0 scanny     (501) staff       (20)    10673 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/oxml/styles.py
+-rw-r--r--   0 scanny     (501) staff       (20)    33671 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/oxml/table.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.613681 python_docx-1.1.1/src/docx/oxml/text/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/oxml/text/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)    11652 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/oxml/text/font.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1467 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/oxml/text/hyperlink.py
+-rw-r--r--   0 scanny     (501) staff       (20)    11262 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/oxml/text/pagebreak.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3538 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/oxml/text/paragraph.py
+-rw-r--r--   0 scanny     (501) staff       (20)    11986 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/oxml/text/parfmt.py
+-rw-r--r--   0 scanny     (501) staff       (20)     9629 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/oxml/text/run.py
+-rw-r--r--   0 scanny     (501) staff       (20)    25567 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/oxml/xmlchemy.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3855 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/package.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.615292 python_docx-1.1.1/src/docx/parts/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/parts/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5472 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/parts/document.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1610 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/parts/hdrftr.py
+-rw-r--r--   0 scanny     (501) staff       (20)     2538 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/parts/image.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1056 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/parts/numbering.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1300 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/parts/settings.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3817 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/parts/story.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1413 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/parts/styles.py
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/py.typed
+-rw-r--r--   0 scanny     (501) staff       (20)    18534 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/section.py
+-rw-r--r--   0 scanny     (501) staff       (20)      658 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/settings.py
+-rw-r--r--   0 scanny     (501) staff       (20)     2658 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/shape.py
+-rw-r--r--   0 scanny     (501) staff       (20)    13509 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/shared.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.616099 python_docx-1.1.1/src/docx/styles/
+-rw-r--r--   0 scanny     (501) staff       (20)     1406 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/styles/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     7211 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/styles/latent.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8051 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/styles/style.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5717 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/styles/styles.py
+-rw-r--r--   0 scanny     (501) staff       (20)    19477 2024-04-30 02:52:59.000000 python_docx-1.1.1/src/docx/table.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.617255 python_docx-1.1.1/src/docx/templates/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.617481 python_docx-1.1.1/src/docx/templates/default-docx-template/
+-rw-r--r--   0 scanny     (501) staff       (20)     1782 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/[Content_Types].xml
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.617702 python_docx-1.1.1/src/docx/templates/default-docx-template/_rels/
+-rw-r--r--   0 scanny     (501) staff       (20)      748 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/_rels/.rels
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.618085 python_docx-1.1.1/src/docx/templates/default-docx-template/customXml/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.618262 python_docx-1.1.1/src/docx/templates/default-docx-template/customXml/_rels/
+-rw-r--r--   0 scanny     (501) staff       (20)      300 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/customXml/_rels/item1.xml.rels
+-rw-r--r--   0 scanny     (501) staff       (20)      262 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/customXml/item1.xml
+-rw-r--r--   0 scanny     (501) staff       (20)      354 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/customXml/itemProps1.xml
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.618830 python_docx-1.1.1/src/docx/templates/default-docx-template/docProps/
+-rw-r--r--   0 scanny     (501) staff       (20)     1132 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/docProps/app.xml
+-rw-r--r--   0 scanny     (501) staff       (20)      753 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/docProps/core.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     8324 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/docProps/thumbnail.jpeg
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.620793 python_docx-1.1.1/src/docx/templates/default-docx-template/word/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.621012 python_docx-1.1.1/src/docx/templates/default-docx-template/word/_rels/
+-rw-r--r--   0 scanny     (501) staff       (20)     1253 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/word/_rels/document.xml.rels
+-rw-r--r--   0 scanny     (501) staff       (20)     1594 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/word/document.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     2811 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/word/fontTable.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     6747 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/word/numbering.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     2749 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/word/settings.xml
+-rw-r--r--   0 scanny     (501) staff       (20)   438677 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/word/styles.xml
+-rw-r--r--   0 scanny     (501) staff       (20)   438131 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/word/stylesWithEffects.xml
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.621221 python_docx-1.1.1/src/docx/templates/default-docx-template/word/theme/
+-rw-r--r--   0 scanny     (501) staff       (20)    10939 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/word/theme/theme1.xml
+-rw-r--r--   0 scanny     (501) staff       (20)      438 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/word/webSettings.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     1395 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-footer.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     1395 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-header.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     1640 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-settings.xml
+-rw-r--r--   0 scanny     (501) staff       (20)    15823 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-styles.xml
+-rw-r--r--   0 scanny     (501) staff       (20)    38116 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default.docx
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.622846 python_docx-1.1.1/src/docx/text/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/text/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)    13653 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/text/font.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5257 2024-04-30 02:52:59.000000 python_docx-1.1.1/src/docx/text/hyperlink.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4950 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/text/pagebreak.py
+-rw-r--r--   0 scanny     (501) staff       (20)     6828 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/text/paragraph.py
+-rw-r--r--   0 scanny     (501) staff       (20)    10339 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/text/parfmt.py
+-rw-r--r--   0 scanny     (501) staff       (20)     9645 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/text/run.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3910 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/text/tabstops.py
+-rw-r--r--   0 scanny     (501) staff       (20)      864 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/types.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.648320 python_docx-1.1.1/src/python_docx.egg-info/
+-rw-r--r--   0 scanny     (501) staff       (20)     2008 2024-04-30 02:58:01.000000 python_docx-1.1.1/src/python_docx.egg-info/PKG-INFO
+-rw-r--r--   0 scanny     (501) staff       (20)    16643 2024-04-30 02:58:01.000000 python_docx-1.1.1/src/python_docx.egg-info/SOURCES.txt
+-rw-r--r--   0 scanny     (501) staff       (20)        1 2024-04-30 02:58:01.000000 python_docx-1.1.1/src/python_docx.egg-info/dependency_links.txt
+-rw-r--r--   0 scanny     (501) staff       (20)       45 2024-04-30 02:58:01.000000 python_docx-1.1.1/src/python_docx.egg-info/requires.txt
+-rw-r--r--   0 scanny     (501) staff       (20)        5 2024-04-30 02:58:01.000000 python_docx-1.1.1/src/python_docx.egg-info/top_level.txt
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.626375 python_docx-1.1.1/tests/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2013-07-29 10:11:43.000000 python_docx-1.1.1/tests/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)      452 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/conftest.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.626662 python_docx-1.1.1/tests/dml/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/dml/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5437 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/dml/test_color.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.628545 python_docx-1.1.1/tests/image/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/image/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1108 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/image/test_bmp.py
+-rw-r--r--   0 scanny     (501) staff       (20)      960 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/image/test_gif.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1569 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/image/test_helpers.py
+-rw-r--r--   0 scanny     (501) staff       (20)    11958 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/image/test_image.py
+-rw-r--r--   0 scanny     (501) staff       (20)    21556 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/image/test_jpeg.py
+-rw-r--r--   0 scanny     (501) staff       (20)    14741 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/image/test_png.py
+-rw-r--r--   0 scanny     (501) staff       (20)    14704 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/image/test_tiff.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.630399 python_docx-1.1.1/tests/opc/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/opc/__init__.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.630696 python_docx-1.1.1/tests/opc/parts/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/opc/parts/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1870 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/opc/parts/test_coreprops.py
+-rw-r--r--   0 scanny     (501) staff       (20)     7972 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/opc/test_coreprops.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4866 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/opc/test_oxml.py
+-rw-r--r--   0 scanny     (501) staff       (20)    17017 2024-04-30 00:55:22.000000 python_docx-1.1.1/tests/opc/test_package.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3313 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/opc/test_packuri.py
+-rw-r--r--   0 scanny     (501) staff       (20)    15381 2024-04-30 00:55:22.000000 python_docx-1.1.1/tests/opc/test_part.py
+-rw-r--r--   0 scanny     (501) staff       (20)     6289 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/opc/test_phys_pkg.py
+-rw-r--r--   0 scanny     (501) staff       (20)    19028 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/opc/test_pkgreader.py
+-rw-r--r--   0 scanny     (501) staff       (20)     7218 2024-04-30 00:55:22.000000 python_docx-1.1.1/tests/opc/test_pkgwriter.py
+-rw-r--r--   0 scanny     (501) staff       (20)     9565 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/opc/test_rel.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.631164 python_docx-1.1.1/tests/opc/unitdata/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/opc/unitdata/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8626 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/opc/unitdata/rels.py
+-rw-r--r--   0 scanny     (501) staff       (20)      765 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/opc/unitdata/types.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.632995 python_docx-1.1.1/tests/oxml/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/oxml/__init__.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.633282 python_docx-1.1.1/tests/oxml/parts/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/oxml/parts/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1432 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/parts/test_document.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.633562 python_docx-1.1.1/tests/oxml/parts/unitdata/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/oxml/parts/unitdata/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)      388 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/parts/unitdata/document.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4108 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/test__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)      587 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/test_document.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1634 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/test_ns.py
+-rw-r--r--   0 scanny     (501) staff       (20)      592 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/test_section.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1367 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/test_styles.py
+-rw-r--r--   0 scanny     (501) staff       (20)    13656 2024-04-30 02:48:37.000000 python_docx-1.1.1/tests/oxml/test_table.py
+-rw-r--r--   0 scanny     (501) staff       (20)    28193 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/test_xmlchemy.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.634032 python_docx-1.1.1/tests/oxml/text/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/text/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1481 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/text/test_hyperlink.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1156 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/text/test_run.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.635099 python_docx-1.1.1/tests/oxml/unitdata/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/oxml/unitdata/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1172 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/unitdata/dml.py
+-rw-r--r--   0 scanny     (501) staff       (20)      412 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/unitdata/numbering.py
+-rw-r--r--   0 scanny     (501) staff       (20)      893 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/unitdata/section.py
+-rw-r--r--   0 scanny     (501) staff       (20)      677 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/unitdata/shared.py
+-rw-r--r--   0 scanny     (501) staff       (20)      449 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/unitdata/styles.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3153 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/unitdata/text.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.637199 python_docx-1.1.1/tests/parts/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/parts/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)    12295 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/parts/test_document.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5062 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/parts/test_hdrftr.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3945 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/parts/test_image.py
+-rw-r--r--   0 scanny     (501) staff       (20)     2580 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/parts/test_numbering.py
+-rw-r--r--   0 scanny     (501) staff       (20)     2576 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/parts/test_settings.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5270 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/parts/test_story.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1695 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/parts/test_styles.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.637946 python_docx-1.1.1/tests/styles/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/styles/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)    14144 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/styles/test_latent.py
+-rw-r--r--   0 scanny     (501) staff       (20)    20304 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/styles/test_style.py
+-rw-r--r--   0 scanny     (501) staff       (20)    14836 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/styles/test_styles.py
+-rw-r--r--   0 scanny     (501) staff       (20)     2327 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_api.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5451 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_blkcntnr.py
+-rw-r--r--   0 scanny     (501) staff       (20)    14036 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_document.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3188 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_enum.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.642486 python_docx-1.1.1/tests/test_files/
+-rw-r--r--   0 scanny     (501) staff       (20)   146892 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/150-dpi.png
+-rw-r--r--   0 scanny     (501) staff       (20)   125824 2023-09-10 05:05:56.000000 python_docx-1.1.1/tests/test_files/300-dpi.TIF
+-rw-r--r--   0 scanny     (501) staff       (20)   355196 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/300-dpi.jpg
+-rw-r--r--   0 scanny     (501) staff       (20)    39921 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/300-dpi.png
+-rw-r--r--   0 scanny     (501) staff       (20)     9454 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/72-dpi.tiff
+-rw-r--r--   0 scanny     (501) staff       (20)     1526 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/CVS_LOGO.WMF
+-rw-r--r--   0 scanny     (501) staff       (20)    11949 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_files/blk-inner-content.docx
+-rw-r--r--   0 scanny     (501) staff       (20)   768608 2023-09-10 05:05:40.000000 python_docx-1.1.1/tests/test_files/exif-420-dpi.jpg
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.642681 python_docx-1.1.1/tests/test_files/expanded_docx/
+-rw-r--r--   0 scanny     (501) staff       (20)     1738 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/[Content_Types].xml
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.642863 python_docx-1.1.1/tests/test_files/expanded_docx/_rels/
+-rw-r--r--   0 scanny     (501) staff       (20)      734 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/_rels/.rels
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.643195 python_docx-1.1.1/tests/test_files/expanded_docx/customXml/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.643374 python_docx-1.1.1/tests/test_files/expanded_docx/customXml/_rels/
+-rw-r--r--   0 scanny     (501) staff       (20)      295 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/customXml/_rels/item1.xml.rels
+-rw-r--r--   0 scanny     (501) staff       (20)      217 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/customXml/item1.xml
+-rw-r--r--   0 scanny     (501) staff       (20)      340 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/customXml/itemProps1.xml
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.643870 python_docx-1.1.1/tests/test_files/expanded_docx/docProps/
+-rw-r--r--   0 scanny     (501) staff       (20)     1036 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/docProps/app.xml
+-rw-r--r--   0 scanny     (501) staff       (20)      802 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/docProps/core.xml
+-rw-r--r--   0 scanny     (501) staff       (20)    13032 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/expanded_docx/docProps/thumbnail.jpeg
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.645150 python_docx-1.1.1/tests/test_files/expanded_docx/word/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.645323 python_docx-1.1.1/tests/test_files/expanded_docx/word/_rels/
+-rw-r--r--   0 scanny     (501) staff       (20)     1227 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/word/_rels/document.xml.rels
+-rw-r--r--   0 scanny     (501) staff       (20)     1819 2023-09-10 05:07:15.000000 python_docx-1.1.1/tests/test_files/expanded_docx/word/document.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     2566 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/word/fontTable.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     5513 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/word/numbering.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     2520 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/word/settings.xml
+-rw-r--r--   0 scanny     (501) staff       (20)    26715 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/word/styles.xml
+-rw-r--r--   0 scanny     (501) staff       (20)    27581 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/word/stylesWithEffects.xml
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.645486 python_docx-1.1.1/tests/test_files/expanded_docx/word/theme/
+-rw-r--r--   0 scanny     (501) staff       (20)     7642 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/word/theme/theme1.xml
+-rw-r--r--   0 scanny     (501) staff       (20)      430 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/word/webSettings.xml
+-rw-r--r--   0 scanny     (501) staff       (20)   132875 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/having-images.docx
+-rw-r--r--   0 scanny     (501) staff       (20)     7958 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/jfif-iguana.jpg
+-rw-r--r--   0 scanny     (501) staff       (20)    10409 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/little-endian.tif
+-rw-r--r--   0 scanny     (501) staff       (20)    64276 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/monty-truth.png
+-rw-r--r--   0 scanny     (501) staff       (20)     3277 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/python-icon.jpeg
+-rw-r--r--   0 scanny     (501) staff       (20)     2036 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/python-icon.png
+-rw-r--r--   0 scanny     (501) staff       (20)     6111 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/python-powered.png
+-rw-r--r--   0 scanny     (501) staff       (20)    45210 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/python.bmp
+-rw-r--r--   0 scanny     (501) staff       (20)    12051 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_files/sct-inner-content.docx
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.646203 python_docx-1.1.1/tests/test_files/snippets/
+-rw-r--r--   0 scanny     (501) staff       (20)     2949 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_files/snippets/add-row-col.txt
+-rw-r--r--   0 scanny     (501) staff       (20)     1110 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_files/snippets/inline.txt
+-rw-r--r--   0 scanny     (501) staff       (20)     1756 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_files/snippets/new-tbl.txt
+-rw-r--r--   0 scanny     (501) staff       (20)     4595 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_files/snippets/tbl-cells.txt
+-rw-r--r--   0 scanny     (501) staff       (20)    33273 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/sonic.gif
+-rw-r--r--   0 scanny     (501) staff       (20)    31773 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/test.docx
+-rw-r--r--   0 scanny     (501) staff       (20)     5297 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_package.py
+-rw-r--r--   0 scanny     (501) staff       (20)    31223 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_section.py
+-rw-r--r--   0 scanny     (501) staff       (20)     2169 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_settings.py
+-rw-r--r--   0 scanny     (501) staff       (20)     6785 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_shape.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4385 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_shared.py
+-rw-r--r--   0 scanny     (501) staff       (20)    32484 2024-04-30 02:48:37.000000 python_docx-1.1.1/tests/test_table.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.647414 python_docx-1.1.1/tests/text/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/text/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)    15804 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/text/test_font.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5192 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/text/test_hyperlink.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5407 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/text/test_pagebreak.py
+-rw-r--r--   0 scanny     (501) staff       (20)    14897 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/text/test_paragraph.py
+-rw-r--r--   0 scanny     (501) staff       (20)    19674 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/text/test_parfmt.py
+-rw-r--r--   0 scanny     (501) staff       (20)    15221 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/text/test_run.py
+-rw-r--r--   0 scanny     (501) staff       (20)    11626 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/text/test_tabstops.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4186 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/unitdata.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.648006 python_docx-1.1.1/tests/unitutil/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/unitutil/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8126 2024-04-30 00:55:22.000000 python_docx-1.1.1/tests/unitutil/cxml.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1675 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/unitutil/file.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4741 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/unitutil/mock.py
+-rw-r--r--   0 scanny     (501) staff       (20)      159 2024-04-30 02:48:37.000000 python_docx-1.1.1/tox.ini
```

### Comparing `python-docx-1.1.0/HISTORY.rst` & `python_docx-1.1.1/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 .. :changelog:
 
 Release History
 ---------------
 
+1.1.1 (2024-04-29)
+++++++++++++++++++
+
+- Fix #531, #1146 Index error on table with misaligned borders
+- Fix #1335 Tolerate invalid float value in bottom-margin
+- Fix #1337 Do not require typing-extensions at runtime
+
+
 1.1.0 (2023-11-03)
 ++++++++++++++++++
 
 - Add BlockItemContainer.iter_inner_content()
 
 
 1.0.1 (2023-10-12)
```

### Comparing `python-docx-1.1.0/LICENSE` & `python_docx-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/PKG-INFO` & `python_docx-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-docx
-Version: 1.1.0
+Version: 1.1.1
 Summary: Create, read, and update Microsoft Word .docx files.
 Author-email: Steve Canny <stcanny@gmail.com>
 License: MIT
 Project-URL: Changelog, https://github.com/python-openxml/python-docx/blob/master/HISTORY.rst
 Project-URL: Documentation, https://python-docx.readthedocs.org/en/latest/
 Project-URL: Homepage, https://github.com/python-openxml/python-docx
 Project-URL: Repository, https://github.com/python-openxml/python-docx
@@ -22,16 +22,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business :: Office Suites
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lxml>=3.1.0
-Requires-Dist: typing_extensions
+Requires-Dist: lxml<=4.9.2,>=3.1.0
+Requires-Dist: typing_extensions>=4.9.0
 
 # python-docx
 
 *python-docx* is a Python library for reading, creating, and updating Microsoft Word 2007+ (.docx) files.
 
 ## Installation
```

### Comparing `python-docx-1.1.0/README.md` & `python_docx-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/Makefile` & `python_docx-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/Session.vim` & `python_docx-1.1.1/docs/Session.vim`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/_static/img/example-docx-01.png` & `python_docx-1.1.1/docs/_static/img/example-docx-01.png`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/_static/img/hdrftr-01.png` & `python_docx-1.1.1/docs/_static/img/hdrftr-01.png`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/_static/img/hdrftr-02.png` & `python_docx-1.1.1/docs/_static/img/hdrftr-02.png`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/_themes/armstrong/LICENSE` & `python_docx-1.1.1/docs/_themes/armstrong/LICENSE`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/_themes/armstrong/layout.html` & `python_docx-1.1.1/docs/_themes/armstrong/layout.html`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/_themes/armstrong/rtd-themes.conf` & `python_docx-1.1.1/docs/_themes/armstrong/rtd-themes.conf`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/_themes/armstrong/static/rtd.css_t` & `python_docx-1.1.1/docs/_themes/armstrong/static/rtd.css_t`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/_themes/armstrong/theme.conf` & `python_docx-1.1.1/docs/_themes/armstrong/theme.conf`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/_themes/armstrong/theme.conf.orig` & `python_docx-1.1.1/docs/_themes/armstrong/theme.conf.orig`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/api/document.rst` & `python_docx-1.1.1/docs/api/document.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/api/enum/MsoThemeColorIndex.rst` & `python_docx-1.1.1/docs/api/enum/MsoThemeColorIndex.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/api/enum/WdAlignParagraph.rst` & `python_docx-1.1.1/docs/api/enum/WdAlignParagraph.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/api/enum/WdBuiltinStyle.rst` & `python_docx-1.1.1/docs/api/enum/WdBuiltinStyle.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/api/enum/WdCellVerticalAlignment.rst` & `python_docx-1.1.1/docs/api/enum/WdCellVerticalAlignment.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/api/enum/WdColorIndex.rst` & `python_docx-1.1.1/docs/api/enum/WdColorIndex.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/api/enum/WdLineSpacing.rst` & `python_docx-1.1.1/docs/api/enum/WdLineSpacing.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/api/enum/WdRowHeightRule.rst` & `python_docx-1.1.1/docs/api/enum/WdRowHeightRule.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/api/enum/WdUnderline.rst` & `python_docx-1.1.1/docs/api/enum/WdUnderline.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/api/section.rst` & `python_docx-1.1.1/docs/api/section.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/api/shape.rst` & `python_docx-1.1.1/docs/api/shape.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/api/shared.rst` & `python_docx-1.1.1/docs/api/shared.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/api/style.rst` & `python_docx-1.1.1/docs/api/style.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/api/table.rst` & `python_docx-1.1.1/docs/api/table.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/api/text.rst` & `python_docx-1.1.1/docs/api/text.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/conf.py` & `python_docx-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/coreprops.rst` & `python_docx-1.1.1/docs/dev/analysis/features/coreprops.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/header.rst` & `python_docx-1.1.1/docs/dev/analysis/features/header.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/numbering.rst` & `python_docx-1.1.1/docs/dev/analysis/features/numbering.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/sections.rst` & `python_docx-1.1.1/docs/dev/analysis/features/sections.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/settings.rst` & `python_docx-1.1.1/docs/dev/analysis/features/settings.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/shapes/index.rst` & `python_docx-1.1.1/docs/dev/analysis/features/shapes/index.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/shapes/picture.rst` & `python_docx-1.1.1/docs/dev/analysis/features/shapes/picture.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/shapes/shapes-inline-size.rst` & `python_docx-1.1.1/docs/dev/analysis/features/shapes/shapes-inline-size.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/shapes/shapes-inline.rst` & `python_docx-1.1.1/docs/dev/analysis/features/shapes/shapes-inline.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/styles/character-style.rst` & `python_docx-1.1.1/docs/dev/analysis/features/styles/character-style.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/styles/index.rst` & `python_docx-1.1.1/docs/dev/analysis/features/styles/index.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/styles/latent-styles.rst` & `python_docx-1.1.1/docs/dev/analysis/features/styles/latent-styles.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/styles/paragraph-style.rst` & `python_docx-1.1.1/docs/dev/analysis/features/styles/paragraph-style.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/styles/style.rst` & `python_docx-1.1.1/docs/dev/analysis/features/styles/style.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/styles/styles.rst` & `python_docx-1.1.1/docs/dev/analysis/features/styles/styles.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/table/cell-merge.rst` & `python_docx-1.1.1/docs/dev/analysis/features/table/cell-merge.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/table/index.rst` & `python_docx-1.1.1/docs/dev/analysis/features/table/index.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/table/table-cell.rst` & `python_docx-1.1.1/docs/dev/analysis/features/table/table-cell.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/table/table-props.rst` & `python_docx-1.1.1/docs/dev/analysis/features/table/table-props.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/table/table-row.rst` & `python_docx-1.1.1/docs/dev/analysis/features/table/table-row.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/text/breaks.rst` & `python_docx-1.1.1/docs/dev/analysis/features/text/breaks.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/text/font-color.rst` & `python_docx-1.1.1/docs/dev/analysis/features/text/font-color.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/text/font-highlight-color.rst` & `python_docx-1.1.1/docs/dev/analysis/features/text/font-highlight-color.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/text/font.rst` & `python_docx-1.1.1/docs/dev/analysis/features/text/font.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/text/hyperlink.rst` & `python_docx-1.1.1/docs/dev/analysis/features/text/hyperlink.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/text/paragraph-format.rst` & `python_docx-1.1.1/docs/dev/analysis/features/text/paragraph-format.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/text/run-content.rst` & `python_docx-1.1.1/docs/dev/analysis/features/text/run-content.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/text/tab-stops.rst` & `python_docx-1.1.1/docs/dev/analysis/features/text/tab-stops.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/features/text/underline.rst` & `python_docx-1.1.1/docs/dev/analysis/features/text/underline.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/index.rst` & `python_docx-1.1.1/docs/dev/analysis/index.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/schema/ct_body.rst` & `python_docx-1.1.1/docs/dev/analysis/schema/ct_body.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/schema/ct_document.rst` & `python_docx-1.1.1/docs/dev/analysis/schema/ct_document.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/dev/analysis/schema/ct_p.rst` & `python_docx-1.1.1/docs/dev/analysis/schema/ct_p.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/index.rst` & `python_docx-1.1.1/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 
 .. toctree::
    :maxdepth: 1
 
    user/install
    user/quickstart
    user/documents
+   user/tables
    user/text
    user/sections
    user/hdrftr
    user/api-concepts
    user/styles-understanding
    user/styles-using
    user/shapes
```

### Comparing `python-docx-1.1.0/docs/user/api-concepts.rst` & `python_docx-1.1.1/docs/user/api-concepts.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/user/documents.rst` & `python_docx-1.1.1/docs/user/documents.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/user/hdrftr.rst` & `python_docx-1.1.1/docs/user/hdrftr.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/user/install.rst` & `python_docx-1.1.1/docs/user/install.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/user/quickstart.rst` & `python_docx-1.1.1/docs/user/quickstart.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/user/sections.rst` & `python_docx-1.1.1/docs/user/sections.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/user/shapes.rst` & `python_docx-1.1.1/docs/user/shapes.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/user/styles-understanding.rst` & `python_docx-1.1.1/docs/user/styles-understanding.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/user/styles-using.rst` & `python_docx-1.1.1/docs/user/styles-using.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/docs/user/text.rst` & `python_docx-1.1.1/docs/user/text.rst`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/_scratch/test_out/[Content_Types].xml` & `python_docx-1.1.1/features/_scratch/test_out/[Content_Types].xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/_scratch/test_out/_rels/.rels` & `python_docx-1.1.1/features/_scratch/test_out/_rels/.rels`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/_scratch/test_out/docProps/app.xml` & `python_docx-1.1.1/features/_scratch/test_out/docProps/app.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/_scratch/test_out/docProps/core.xml` & `python_docx-1.1.1/features/_scratch/test_out/docProps/core.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/_scratch/test_out/docProps/thumbnail.jpeg` & `python_docx-1.1.1/features/_scratch/test_out/docProps/thumbnail.jpeg`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/_scratch/test_out/word/_rels/document.xml.rels` & `python_docx-1.1.1/features/_scratch/test_out/word/_rels/document.xml.rels`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/_scratch/test_out/word/document.xml` & `python_docx-1.1.1/features/_scratch/test_out/word/document.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/_scratch/test_out/word/fontTable.xml` & `python_docx-1.1.1/features/_scratch/test_out/word/fontTable.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/_scratch/test_out/word/numbering.xml` & `python_docx-1.1.1/features/_scratch/test_out/word/numbering.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/_scratch/test_out/word/settings.xml` & `python_docx-1.1.1/features/_scratch/test_out/word/settings.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/_scratch/test_out/word/styles.xml` & `python_docx-1.1.1/features/_scratch/test_out/word/styles.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/_scratch/test_out/word/stylesWithEffects.xml` & `python_docx-1.1.1/features/_scratch/test_out/word/stylesWithEffects.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/_scratch/test_out/word/theme/theme1.xml` & `python_docx-1.1.1/features/_scratch/test_out/word/theme/theme1.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/_scratch/test_out.docx` & `python_docx-1.1.1/features/_scratch/test_out.docx`

 * *Format-specific differences are supported for Microsoft Word .docx files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Microsoft Word 2007+*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 504b 0304 1400 0000 0800 f486 6357 ad52  PK..........cW.R
+00000000: 504b 0304 1400 0000 0800 9d9e 9d58 ad52  PK...........X.R
 00000010: a591 9501 0000 ca06 0000 1300 0000 5b43  ..............[C
 00000020: 6f6e 7465 6e74 5f54 7970 6573 5d2e 786d  ontent_Types].xm
 00000030: 6cb5 954d 4fdb 4010 86ef fd15 962f 3e20  l..MO.@....../> 
 00000040: 7b43 0f15 aae2 7028 702c 911a 44af 9bf5  {C....p(p,..D...
 00000050: 3859 d82f ed4c 02f9 f7cc 3a89 55d1 5087  8Y./.L....:.U.P.
 00000060: 062e 919c 99f7 7d1e dbb2 3dbe 7cb6 265b  ......}...=.|.&[
 00000070: 4344 ed5d 5d9c 57a3 2203 a77c a3dd a22e  CD.]].W."..|....
@@ -23,15 +23,15 @@
 00000160: c80f 8635 553f b152 bb41 8f96 c933 3937  ...5U?.R.A...397
 00000170: ff71 ea43 227d f5a0 845b d939 444e 7dbc  .q.C"}...[.9DN}.
 00000180: 445f 3d28 8140 c47b f8f1 0efb e661 05da  D_=(.@.{.....a..
 00000190: 18f8 0c81 aef7 48fc bda6 e575 db82 a263  ......H....u...c
 000001a0: 4c2c 9629 5bfd 951d a411 bf91 61fb 7bfa  L,.)[.......a.{.
 000001b0: 0ba7 ab19 443e c1fc d7a7 dde5 3fca f722  ....D>......?.."
 000001c0: a2fb 144d 5e00 504b 0304 1400 0000 0800  ...M^.PK........
-000001d0: f486 6357 7926 4b40 f800 0000 de02 0000  ..cWy&K@........
+000001d0: 9d9e 9d58 7926 4b40 f800 0000 de02 0000  ...Xy&K@........
 000001e0: 0b00 0000 5f72 656c 732f 2e72 656c 73ad  ...._rels/.rels.
 000001f0: 92cd 4a03 3110 80ef 3e45 c825 a76e b655  ..J.1...>E.%.n.U
 00000200: 44a4 d95e 44e8 4da4 3ec0 98cc eea6 6e7e  D..^D.M.>.....n~
 00000210: 48a6 dabe bd51 445d 5816 c11e e7ef e363  H....QD]X......c
 00000220: 66d6 9ba3 1bd8 2ba6 6c83 5762 59d5 82a1  f.....+.l.WbY...
 00000230: d7c1 58df 29f1 b4bb 5fdc 0896 09bc 8121  ..X.)..._......!
 00000240: 7854 e284 596c 9a8b f523 0e40 6526 f736  xT..Yl...#.@e&.6
@@ -41,15 +41,15 @@
 00000280: 6c77 8af8 3fb6 7448 6080 40ea 9070 1153  lw..?.tH`.@..p.S
 00000290: 994e 6431 1738 a40e 4971 13f4 4349 e7cf  .Nd1.8..Iq..CI..
 000002a0: 8eaa 90b9 9c16 bafa bb50 685b abf1 2ee8  .........Ph[....
 000002b0: 8343 4f53 5e78 24f4 06cd bc12 c438 67b4  .COS^x$......8g.
 000002c0: 3ca7 d1b8 e347 e62d 2423 cd57 7ace 6675  <....G.-$#.Wz.fu
 000002d0: de83 517f 70cf 1eec 30b1 97ef 5ab5 8fd8  ..Q.p...0...Z...
 000002e0: 7d08 c9d1 5b36 ef50 4b03 0414 0000 0008  }...[6.PK.......
-000002f0: 00f4 8663 5788 860b 5369 0100 00d1 0200  ...cW...Si......
+000002f0: 009d 9e9d 5888 860b 5369 0100 00d1 0200  ....X...Si......
 00000300: 0011 0000 0064 6f63 5072 6f70 732f 636f  .....docProps/co
 00000310: 7265 2e78 6d6c 9d92 cb4e c330 1045 f77c  re.xml...N.0.E.|
 00000320: 45d4 4d56 89f3 1008 4549 2a01 ea8a 4a48  E.MV....EI*...JH
 00000330: 1481 d8b9 f634 354d 6ccb 9e36 cddf e3a4  .....45Ml..6....
 00000340: 6d5a a02b 761e df3b c7f3 703e dd37 b5b7  mZ.+v..;..p>.7..
 00000350: 0363 8592 851f 8791 ef81 648a 0b59 15fe  .c........d..Y..
 00000360: db62 16dc fb9e 452a 39ad 9584 c2ef c0fa  .b....E*9.......
@@ -66,15 +66,15 @@
 00000410: 5dab 0cb7 870c 0e96 19a1 d1ed a8ac 4082  ].............@.
 00000420: a108 dc5b 76de 6fc4 a5b1 c7d4 d4e2 dc2d  ...[v.o........-
 00000430: 7325 803f 7464 b833 b013 fdb6 cb38 2797  s%.?td.3.....8'.
 00000440: 617e 9cdd a10e c777 3d67 8709 9d94 f7f4  a~.....w=g......
 00000450: f169 319b 9449 14a7 419c 0449 ba48 d22c  .i1..I..A..I.H.,
 00000460: becd a2e8 b37f ff47 fe19 d81c 2bf8 37f1  .......G....+.7.
 00000470: 0418 ea67 0e5e 29d3 7743 fefc c2f2 1b50  ...g.^).wC.....P
-00000480: 4b03 0414 0000 0008 00f4 8663 57f4 dbdb  K..........cW...
+00000480: 4b03 0414 0000 0008 009d 9e9d 58f4 dbdb  K...........X...
 00000490: 17eb 0100 006c 0400 0010 0000 0064 6f63  .....l.......doc
 000004a0: 5072 6f70 732f 6170 702e 786d 6c9d 54cb  Props/app.xml.T.
 000004b0: 6edb 3010 bcfb 2b04 5d74 8a69 0741 5118  n.0...+.]t.i.AQ.
 000004c0: 9282 d641 d143 dd1a b092 9cb7 d4ca 224a  ...A.C........"J
 000004d0: 9104 b931 e27e 7df9 8815 3986 2ff5 893b  ...1.~}...9./..;
 000004e0: b33b fbb4 cafb d741 6607 b44e 6855 15cb  .;.....Af..NhU..
 000004f0: f9a2 c850 71dd 0ab5 af8a c7e6 dbcd e722  ...Pq.........."
@@ -100,15 +100,15 @@
 00000630: 9f35 1a11 7625 e185 7eb9 01e5 6f27 0594  .5..v%..~...o'..
 00000640: 6b3d 1850 4776 5ae2 1ff7 681a fd10 2ef1  k=.PGvZ...h.....
 00000650: 6d31 e7e0 f975 3d0b ea77 0638 7eb8 b309  m1...u=..w.8~...
 00000660: 1e97 ed09 6cfd c98c cb1e 81b8 6cdf 9795  ....l.......l...
 00000670: 3ecd 57df 243b 879c 1755 7b6c 4f91 97c4  >.W.$;...U{lO...
 00000680: db49 3fa5 4f47 bdbc 9b2f fc2f 1ef0 099b  .I?.OG..././....
 00000690: f9f3 1bff d5f5 ec1f 504b 0304 1400 0000  ........PK......
-000006a0: 0800 f486 6357 059c 75c4 1502 0000 4206  ....cW..u.....B.
+000006a0: 0800 9d9e 9d58 059c 75c4 1502 0000 4206  .....X..u.....B.
 000006b0: 0000 1100 0000 776f 7264 2f64 6f63 756d  ......word/docum
 000006c0: 656e 742e 786d 6ca5 94cb 8eda 3014 86f7  ent.xml.....0...
 000006d0: 7d8a 349b ac20 0ed0 9446 8459 3062 348b  }.4.. ...F.Y0b4.
 000006e0: 4aa8 b40f 601c 27b1 26f1 b16c 4386 3e7d  J...`.'.&..lC.>}
 000006f0: 8f73 8154 9510 1d36 b6cf edf3 ef13 c7ab  .s.T...6........
 00000700: a7f7 baf2 4e5c 1b01 320d a229 093c 2e19  ....N\..2..).<..
 00000710: 6442 1669 f0eb e776 b20c 3c63 a9cc 6805  dB.i...v..<c..h.
@@ -136,15 +136,15 @@
 00000870: 14b7 2a54 b1ff 8d51 bc52 d16c b620 2eb3  ..*T...Q.R.l. ..
 00000880: c4f5 9725 aec3 2ee1 3b75 fb58 c09b 1f2d  ...%....;u.X...-
 00000890: ba14 2d8a 1249 d192 b4e6 01ac 85fa 1aae  ..-..I..........
 000008a0: 783e 8a96 9c66 1cd5 7c9d b566 0e60 4766  x>...f..|..f.`Gf
 000008b0: 71b4 add9 6fc7 a032 e835 8a32 dee5 b46e  q...o..2.5.2...n
 000008c0: ecc8 8b16 9963 0bc9 77c2 3254 398f db68  .....c..w.2T9..h
 000008d0: 3874 a35d 766d 0daf afff fa0f 504b 0304  8t.]vm......PK..
-000008e0: 1400 0000 0800 f486 6357 6e80 1b12 3201  ........cWn...2.
+000008e0: 1400 0000 0800 9d9e 9d58 6e80 1b12 3201  .........Xn...2.
 000008f0: 0000 cb04 0000 1c00 0000 776f 7264 2f5f  ..........word/_
 00000900: 7265 6c73 2f64 6f63 756d 656e 742e 786d  rels/document.xm
 00000910: 6c2e 7265 6c73 ad94 414f 8330 1886 effe  l.rels..AO.0....
 00000920: 0ac2 8593 14a6 6e8b 19ec a226 bb2a 46af  ......n....&.*F.
 00000930: a57c 8546 da92 f643 e5df 5bdd 642c 43e2  .|.F...C..[.d,C.
 00000940: 81e3 f736 7d9f 276d d3cd f653 d6de 3b18  ...6}.'m...S..;.
 00000950: 2bb4 4a82 388c 020f 14d3 8550 6512 3c67  +.J.8......Pe.<g
@@ -159,15 +159,15 @@
 000009e0: 5f04 56f7 9c03 c333 f860 69ca e366 d663  _.V....3.`i..f.c
 000009f0: 0044 77bf 4397 4332 a5b0 9c53 e103 f2a7  .Dw.C.C2...S....
 00000a00: 338b 4138 25b2 9a53 846b 8519 cd6b 386a  3.A8%..S.k...k8j
 00000a10: f4d1 94c4 7a4e 0974 7b07 023f e33e 8ca7  ....zN.t{..?.>..
 00000a20: 1ce2 391d 586b 51cb 5747 eb3d c2f0 9812  ..9.XkQ.WG.=....
 00000a30: 8120 276d 1673 daa8 56e6 60dc 4b38 daf4  . 'm.s..V.`.K8..
 00000a40: d1af 0439 f983 d22f 504b 0304 1400 0000  ...9.../PK......
-00000a50: 0800 f486 6357 07d4 af99 732f 0000 1255  ....cW....s/...U
+00000a50: 0800 9d9e 9d58 07d4 af99 732f 0000 1255  .....X....s/...U
 00000a60: 0500 0f00 0000 776f 7264 2f73 7479 6c65  ......word/style
 00000a70: 732e 786d 6ced 5d5d 93e2 46b2 7dbf bfa2  s.xml.]]..F.}...
 00000a80: a35f fce4 6d90 8400 c7ce 6e00 9276 1c61  ._..m.....n..v.a
 00000a90: 7bbd 9eb1 ef33 4d33 d3ec d0d0 1768 8fed  {....3M3.....h..
 00000aa0: 5f7f 2521 401f 5552 5556 4aaa 92b2 3bc2  _.%!@.URUVJ...;.
 00000ab0: 9e16 5029 e557 9d93 5465 fdfd 9f7f bc6c  ..P).W..Te.....l
 00000ac0: ef7e 5f1f 8e9b fdee dd37 c3bf 0dbe b95b  .~_......7.....[
@@ -921,15 +921,15 @@
 00003980: 8f38 d50f 29d4 ffcc 1a21 057b 3871 a6ec  .8..)....!.{8q..
 00003990: afc5 989b 518c 460a 0d3c 2cde 3a85 da4f  ....Q.F..<,.:..O
 000039a0: ecd5 f370 6145 a450 b20f 328d 14e0 fb20  ...paE.P..2.... 
 000039b0: 0929 1052 a813 29a8 ed14 6a0f 29d4 7fec  .).R..)...j.)...
 000039c0: 9e7e 48a1 fe67 d608 29f8 b6bb 90e9 7061  .~H..g..).....pa
 000039d0: 3452 68e0 6111 0fbc acfb 1449 3d0f bcbc  4Rh.a......I=...
 000039e0: 2185 cbbf 8eff f87f 504b 0304 1400 0000  !.......PK......
-000039f0: 0800 f486 6357 6079 82d3 3935 0000 73af  ....cW`y..95..s.
+000039f0: 0800 9d9e 9d58 6079 82d3 3935 0000 73af  .....X`y..95..s.
 00003a00: 0600 1a00 0000 776f 7264 2f73 7479 6c65  ......word/style
 00003a10: 7357 6974 6845 6666 6563 7473 2e78 6d6c  sWithEffects.xml
 00003a20: ed7d 5d97 a346 b2ed fbf9 15b5 eac5 4f9e  .}]..F........O.
 00003a30: 9600 21c9 cb7d ce12 02c6 5ecb e3f1 99f6  ..!..}....^.....
 00003a40: f83e abab d45d 9aae 92ea 4a2a b7ed 5f7f  .>...]....J*.._.
 00003a50: 409f 8012 c88f 48c8 84ed 7e98 2940 1990  @.....H...~.)@..
 00003a60: b933 73c7 0e88 f8fe 7ffe 7879 befb 7db9  .3s.......xy..}.
@@ -1776,15 +1776,15 @@
 00006ef0: 6691 6df4 95f6 f722 47e1 2862 9778 60cd  f.m...."G.(b.x`.
 00006f00: 151b 58a4 c647 2260 9175 1982 b22c 9222  ..X..G"`.u...,."
 00006f10: 4310 5864 e142 b0c8 beb0 48e9 6c0c b6b3  C.Xd.B....H.l...
 00006f20: c838 08bd 80fd ea15 ebc1 c122 0de9 446b  .8........."..Dk
 00006f30: 5964 e4fa 7391 74a7 7d66 916d f495 6e16  Yd..s.t.}f.m..n.
 00006f40: 1907 f3d9 8c4d b958 73c5 0616 a9f1 9132  .....M.Xs......2
 00006f50: 2cf2 f27f 939d fcff 0050 4b03 0414 0000  ,........PK.....
-00006f60: 0008 00f4 8663 57a3 3f46 5fbf 0300 00e7  .....cW.?F_.....
+00006f60: 0008 009d 9e9d 58a3 3f46 5fbf 0300 00e7  ......X.?F_.....
 00006f70: 0900 0011 0000 0077 6f72 642f 7365 7474  .......word/sett
 00006f80: 696e 6773 2e78 6d6c b556 dd72 da38 14be  ings.xml.V.r.8..
 00006f90: dfa7 60b8 e166 09b6 714c e329 e924 b0de  ..`..f..qL.).$..
 00006fa0: 4d26 6c33 75fa 00b2 7d00 6df4 3792 0ca1  M&l3u...}.m.7...
 00006fb0: 4fdf 23db 8ac9 9666 98ed ec15 f2f9 cebf  O.#....f........
 00006fc0: be73 c4c7 4f2f 9c0d 76a0 0d95 623e 0a2f  .s..O/..v...b>./
 00006fd0: 82d1 0044 292b 2a36 f3d1 d7a7 6cfc 6134  ...D)+*6....l.a4
@@ -1839,15 +1839,15 @@
 000072e0: 3e27 03a3 68c5 c90b 5e6a 10cd 9cf3 4e9b  >'..h...^j....N.
 000072f0: 357b fb8d aec3 9cb2 7aeb a122 96f8 fdf0  5{......z.."....
 00007300: c6b8 9989 7fe5 e2de a192 227f f303 2ffa  ..........".../.
 00007310: e7e5 a22d 8b51 838b 4ce1 4b64 a5f6 d8ef  ...-.Q..L.Kd....
 00007320: 0d16 c658 7479 87a3 87a7 461e c541 1205  ...Xty....F..A..
 00007330: 49f8 0ab7 41ee 38d9 c052 d15e 711a 04dd  I...A.8..R.^q...
 00007340: 80fa bf68 d7df 0150 4b03 0414 0000 0008  ...h...PK.......
-00007350: 00f4 8663 57e8 5ae5 5300 0100 00b6 0100  ...cW.Z.S.......
+00007350: 009d 9e9d 58e8 5ae5 5300 0100 00b6 0100  ....X.Z.S.......
 00007360: 0014 0000 0077 6f72 642f 7765 6253 6574  .....word/webSet
 00007370: 7469 6e67 732e 786d 6c8d d0c1 6ac3 300c  tings.xml...j.0.
 00007380: 00d0 7bbe c2e4 9253 e364 8c31 4292 3218  ..{....S.d.1B.2.
 00007390: 1dbb 9441 b60f 701c 2531 b52d 63b9 cdfa  ...A..p.%1.-c...
 000073a0: f733 5936 18bb f426 21e9 21a9 de7f 1acd  .3Y6...&!.!.....
 000073b0: 2ee0 49a1 6db2 322f 3206 56e2 a0ec d464  ..I.m.2/2.V....d
 000073c0: 1fef 87dd 63c6 2808 3b08 8d16 9aec 0a94  ....c.(.;.......
@@ -1858,15 +1858,15 @@
 00007410: c233 cab3 011b d679 ee41 4711 2dcd cad1  .3.....y.AG.-...
 00007420: 8fb6 dca2 2de8 07e7 5102 51bc c7e8 6fcf  ....-...Q.Q...o.
 00007430: 0865 7f99 f2fe 1f64 94f4 4838 863c 1eb3  .e.....d..H8.<..
 00007440: 6db4 5271 bc2c d6c8 e894 1959 bd4e 16bd  m.Rq.,.....Y.N..
 00007450: e835 3469 84d2 3661 2c7e 5068 8dcb dbf1  .54i..6a,~Ph....
 00007460: 856f f980 470c 9db8 c013 7571 0d0d 07a5  .o..G.....uq....
 00007470: 2116 6bfe e7db 6df2 0550 4b03 0414 0000  !.k...m..PK.....
-00007480: 0008 00f4 8663 57fb 39a0 7363 0200 00fb  .....cW.9.sc....
+00007480: 0008 009d 9e9d 58fb 39a0 7363 0200 00fb  ......X.9.sc....
 00007490: 0a00 0012 0000 0077 6f72 642f 666f 6e74  .......word/font
 000074a0: 5461 626c 652e 786d 6cdd 96c1 6eda 301c  Table.xml...n.0.
 000074b0: c6ef 7d8a 2897 9c4a 6c93 b514 112a c686  ..}.(..Jl....*..
 000074c0: b4cb 0e1b 7b00 131c b016 db91 ed40 b9d2  ....{........@..
 000074d0: fbce 3b6c 8f30 edb0 49bb f46d 907a ed2b  ..;l.0..I..m.z.+
 000074e0: cc24 0182 0819 7443 4803 2139 ffcf f962  .$....tCH.!9...b
 000074f0: fff4 fd1d 5ab7 772c b226 442a 2ab8 efc0  ....Z.w,.&D**...
@@ -1899,15 +1899,15 @@
 000076a0: bb38 a226 6955 41eb a58d 88d2 c89d 2768  .8.&iUA.......'h
 000076b0: b02c 689d 6e49 d00e 68c8 bf0a da62 fe73  .,h.nI..h....b.s
 000076c0: 31ff b5b8 bf5f ccbf 9f3e 6e4c 0c89 fccf  1...._...>nL....
 000076d0: f226 1249 89ac ca1b 3079 3b90 dd69 f296  .&.I....0y;..i..
 000076e0: 3fb6 5ee0 5460 70e4 c196 f33e 9653 c7ac  ?.^.T`p....>.S..
 000076f0: b0e2 6f05 022f cdb1 efe5 7d89 ce75 fc97  ..o../....}..u..
 00007700: be26 eba7 7a4d ae46 aa7d f11b 504b 0304  .&..zM.F.}..PK..
-00007710: 1400 0000 0800 f486 6357 9441 22b8 c606  ........cW.A"...
+00007710: 1400 0000 0800 9d9e 9d58 9441 22b8 c606  .........X.A"...
 00007720: 0000 bb2a 0000 1500 0000 776f 7264 2f74  ...*......word/t
 00007730: 6865 6d65 2f74 6865 6d65 312e 786d 6ced  heme/theme1.xml.
 00007740: 5a4d 6fdb 3618 bef7 5710 bae4 d4fa db75  ZMo.6...W......u
 00007750: 8aba 45ec d8ed d6a6 0d12 b743 8fb4 445b  ..E........C..D[
 00007760: 6c28 5120 e924 be0d ed71 c080 61dd b0c3  l(Q .$...q..a...
 00007770: 0aec b6c3 b0ad 400b ecd2 fd9a 6e1d b60e  ......@.....n...
 00007780: e85f 1829 d98a 2851 72e6 c54d da25 07c7  ._.)..(Qr..M.%..
@@ -2010,29 +2010,29 @@
 00007d90: 670e 69c4 df41 2380 9d43 4322 a4a2 61f6  g.i..A#..CC"..a.
 00007da0: d3a9 ece5 64e7 48b2 d8d0 316b 6d39 d619  ....d.H...1km9..
 00007db0: 87e1 4019 3357 9763 8e59 7499 e5a9 2a66  ..@.3W.c.Yt...*f
 00007dc0: 0edf 242f 6027 0699 238e 6428 240c 1e9d  ..$/`'..#.d($...
 00007dd0: 4562 2f86 b65f b94f 97b4 d102 9f96 57e6  Eb/.._.O......W.
 00007de0: d325 63f0 847c 2a0e 97f0 69ec c5f0 fc9f  .%c..|*...i.....
 00007df0: c95e a5e3 a160 b03b ffe1 992c 0972 8f38  .^...`.;...,.r.8
-00007e00: fdaf 5df8 0750 4b03 0414 0000 0008 00f4  ..]..PK.........
-00007e10: 8663 579e 803a d7a7 0000 0006 0100 0013  .cW..:..........
+00007e00: fdaf 5df8 0750 4b03 0414 0000 0008 009d  ..]..PK.........
+00007e10: 9e9d 589e 803a d7a7 0000 0006 0100 0013  ..X..:..........
 00007e20: 0000 0063 7573 746f 6d58 6d6c 2f69 7465  ...customXml/ite
 00007e30: 6d31 2e78 6d6c ad8c b10a c230 1400 f77e  m1.xml.....0...~
 00007e40: 45c9 92c9 a63a 8814 d352 1027 11a1 0aae  E....:...R.'....
 00007e50: 49fa da06 92bc 92a4 62ff de88 bfe0 7877  I.......b.....xw
 00007e60: 70c7 e66d 4dfe 021f 343a 4eb7 4549 7370  p..mM...4:N.EIsp
 00007e70: 0a7b ed46 4e1f f7f3 e640 f310 85eb 8541  .{.FN....@.....A
 00007e80: 079c ae10 6853 6747 5975 b878 0521 4f03  ....hSgGYu.x.!O.
 00007e90: 172a c9c9 14e3 5c31 16d4 0456 8402 6770  .*....\1...V..gp
 00007ea0: a90d e8ad 8809 fdc8 7018 b482 13aa c582  ........p.......
 00007eb0: 8b6c 5796 7b26 b534 1a47 2fe6 6925 bfd9  .lW.{&.4.G/.i%..
 00007ec0: 7f56 1d18 5011 fa2e ae06 3861 edad 2d9e  .V..P.....8a..-.
 00007ed0: dd25 85af b80a 9b64 7284 d5d9 0750 4b03  .%.....dr....PK.
-00007ee0: 0414 0000 0008 00f4 8663 573e cae5 d5bd  .........cW>....
+00007ee0: 0414 0000 0008 009d 9e9d 583e cae5 d5bd  ..........X>....
 00007ef0: 0000 0027 0100 001e 0000 0063 7573 746f  ...'.......custo
 00007f00: 6d58 6d6c 2f5f 7265 6c73 2f69 7465 6d31  mXml/_rels/item1
 00007f10: 2e78 6d6c 2e72 656c 738d cfb1 6ac3 3010  .xml.rels...j.0.
 00007f20: 06e0 bd4f 21b4 68aa 6567 28a1 58f6 1202  ...O!.h.eg(.X...
 00007f30: d942 7021 ab90 cfb6 88a5 13ba 4b48 debe  .Bp!........KH..
 00007f40: a253 0319 32de 1dff f773 6d7f 0fab b841  .S..2....sm....A
 00007f50: 268f d1a8 a6aa 9580 e870 f471 36ea 67d8  &........p.q6.g.
@@ -2040,15 +2040,15 @@
 00007f70: 3dc1 6ab9 6468 f189 4441 2219 b930 a76f  =.j.dh..DA"..0.o
 00007f80: adc9 2d10 2c55 9820 96cb 8439 582e 639e  ..-.,U. ...9X.c.
 00007f90: 75b2 ee62 67d0 9bba fed2 f9bf 21bb 2753  u..bg.......!.'S
 00007fa0: 1c46 23f3 616c a418 1e09 deb1 719a bc83  .F#.al......q...
 00007fb0: 1dba 6b80 c82f 2ab4 bb12 6338 87f5 98b1  ..k../*...c8....
 00007fc0: 348a c1e6 19d8 48cf 10fe 564d 554c a9bb  4.....H...VMUL..
 00007fd0: 563f fdd7 fd02 504b 0304 1400 0000 0800  V?....PK........
-00007fe0: f486 6357 b5bb 4c4d e100 0000 6201 0000  ..cW..LM....b...
+00007fe0: 9d9e 9d58 b5bb 4c4d e100 0000 6201 0000  ...X..LM....b...
 00007ff0: 1800 0000 6375 7374 6f6d 586d 6c2f 6974  ....customXml/it
 00008000: 656d 5072 6f70 7331 2e78 6d6c 9d90 b16e  emProps1.xml...n
 00008010: 8330 1445 77be c2f2 e2c9 31a0 0468 1488  .0.Ew.....1..h..
 00008020: 4800 296b d54a 5d1d 7880 256c 23db 448d  H.)k.J].x.%l#.D.
 00008030: aafe 7b4d 3a35 63c7 77ae 74ee d53b 1c3f  ..{M:5c.w.t..;.?
 00008040: e584 6e60 acd0 2a27 d126 2408 54ab 3ba1  ..n`..*'.&$.T.;.
 00008050: 869c bcbf 3534 23c8 3aae 3a3e 6905 39b9  ....54#.:.:>i.9.
@@ -2057,15 +2057,15 @@
 00008080: 7a06 e5c3 5e1b c99d 3fcd c074 df8b 162a  z...^...?..t...*
 00008090: dd2e 1294 6371 1826 ac5d bc4b 7ec8 0923  ....cq.&.].K~..#
 000080a0: ef16 5e79 a972 fc55 3771 9a65 5142 eb73  ..^y.r.U7q.eQB.s
 000080b0: d2d0 32d9 eee8 4b98 5634 6de2 5d59 9f4f  ..2...K.V4m.]Y.O
 000080c0: 51b5 2dbf 7111 20b4 4efa ed7c 85de aee4  Q.-.q. .N..|....
 000080d0: 89ad dec5 88ff 0ebc 8aeb 24f4 60f8 3cde  ..........$.`.<.
 000080e0: 317b 34b2 a7ca 07f8 f396 22f8 0150 4b03  1{4......."..PK.
-000080f0: 0414 0000 0008 00f4 8663 5790 d087 896b  .........cW....k
+000080f0: 0414 0000 0008 009d 9e9d 5890 d087 896b  ..........X....k
 00008100: 0300 0089 1500 0012 0000 0077 6f72 642f  ...........word/
 00008110: 6e75 6d62 6572 696e 672e 786d 6ccd 58dd  numbering.xml.X.
 00008120: 6ee2 3818 bddf a740 9146 5cb5 8993 3404  n.8....@.F\...4.
 00008130: 34b4 a240 565d 8d46 23b5 f300 2618 b0ea  4..@V].F#...&...
 00008140: 9fc8 3130 dcee 4bed 63cd 2bac 9d3f a88a  ..10..K.c.+..?..
 00008150: 334c 1276 cb8d 137f df39 fe7c 4efc 05f8  3L.v.....9.|N...
 00008160: fcf0 8392 de0e 8914 7336 ee83 5ba7 df43  ........s6..[..C
@@ -2115,15 +2115,15 @@
 00008420: 7857 7cdf 1d7d 3ae7 aa8e 76ff be0b 4d46  xW|..}:...v...MF
 00008430: 0c1b 1be1 0e07 0150 5e5c f778 5df1 74b5  .......P^\.x].t.
 00008440: f2e1 3f3a 5d2c 3393 9dfe 6e7a e36c b9af  ..?:],3...nz.l..
 00008450: b0a0 6367 60ae 1916 d4c0 3c33 ecae 06f6  ..cg`.....<3....
 00008460: eec7 f611 e6d7 c0ee ccb0 410d 2c30 c3bc  ..........A.,0..
 00008470: 1ad8 c00c 736b 60a1 1906 6a60 4333 cc39  ....sk`...j`C3.9
 00008480: 85d9 27ff a1de ff0b 504b 0304 1400 0000  ..'.....PK......
-00008490: 0800 f486 6357 a2c8 d667 bd05 0000 8420  ....cW...g..... 
+00008490: 0800 9d9e 9d58 a2c8 d667 bd05 0000 8420  .....X...g..... 
 000084a0: 0000 1700 0000 646f 6350 726f 7073 2f74  ......docProps/t
 000084b0: 6875 6d62 6e61 696c 2e6a 7065 67ed 566b  humbnail.jpeg.Vk
 000084c0: 7013 5514 3ebb 7b37 296d cd10 282d 1407  p.U.>.{7)m..(-..
 000084d0: c2bb 32c0 a42d 422b 0236 69da a694 36a4  ..2..-B+.6i...6.
 000084e0: 2daf 7186 4993 4d13 9a26 6177 d396 4e9d  -.q.I.M..&aw..N.
 000084f0: 91fa 00f5 873c 7cff b114 5474 9c71 50d1  .....<|...Tt.qP.
 00008500: 823a 5245 4047 0710 0b14 18c6 226a f135  .:RE@G......"j.5
@@ -2210,79 +2210,79 @@
 00008a10: 8191 f0e3 7275 c38a 16e9 5dab 868f cf5b  ....ru....]....[
 00008a20: 9392 61d9 b079 7bf7 9009 f9ce 7323 eac4  ..a..y{.....s#..
 00008a30: 43a9 9913 67f6 4d3a 4f4b 532a bbb5 c2da  C...g.M:OKS*....
 00008a40: ff53 6503 8525 ea3a 0ee9 1c6e 3823 6784  .Se..%.:...n8#g.
 00008a50: f970 e54a 0e74 b00f a682 061a 68a0 8106  .p.J.t......h...
 00008a60: 1a68 a081 061a 68a0 8106 1a68 a081 061a  .h....h....h....
 00008a70: 68a0 8106 ff33 88f6 c23f 504b 0102 1403  h....3...?PK....
-00008a80: 1400 0000 0800 f486 6357 ad52 a591 9501  ........cW.R....
+00008a80: 1400 0000 0800 9d9e 9d58 ad52 a591 9501  .........X.R....
 00008a90: 0000 ca06 0000 1300 0000 0000 0000 0000  ................
 00008aa0: 0000 8001 0000 0000 5b43 6f6e 7465 6e74  ........[Content
 00008ab0: 5f54 7970 6573 5d2e 786d 6c50 4b01 0214  _Types].xmlPK...
-00008ac0: 0314 0000 0008 00f4 8663 5779 264b 40f8  .........cWy&K@.
+00008ac0: 0314 0000 0008 009d 9e9d 5879 264b 40f8  ..........Xy&K@.
 00008ad0: 0000 00de 0200 000b 0000 0000 0000 0000  ................
 00008ae0: 0000 0080 01c6 0100 005f 7265 6c73 2f2e  ........._rels/.
 00008af0: 7265 6c73 504b 0102 1403 1400 0000 0800  relsPK..........
-00008b00: f486 6357 8886 0b53 6901 0000 d102 0000  ..cW...Si.......
+00008b00: 9d9e 9d58 8886 0b53 6901 0000 d102 0000  ...X...Si.......
 00008b10: 1100 0000 0000 0000 0000 0000 8001 e702  ................
 00008b20: 0000 646f 6350 726f 7073 2f63 6f72 652e  ..docProps/core.
-00008b30: 786d 6c50 4b01 0214 0314 0000 0008 00f4  xmlPK...........
-00008b40: 8663 57f4 dbdb 17eb 0100 006c 0400 0010  .cW........l....
+00008b30: 786d 6c50 4b01 0214 0314 0000 0008 009d  xmlPK...........
+00008b40: 9e9d 58f4 dbdb 17eb 0100 006c 0400 0010  ..X........l....
 00008b50: 0000 0000 0000 0000 0000 0080 017f 0400  ................
 00008b60: 0064 6f63 5072 6f70 732f 6170 702e 786d  .docProps/app.xm
-00008b70: 6c50 4b01 0214 0314 0000 0008 00f4 8663  lPK............c
-00008b80: 5705 9c75 c415 0200 0042 0600 0011 0000  W..u.....B......
+00008b70: 6c50 4b01 0214 0314 0000 0008 009d 9e9d  lPK.............
+00008b80: 5805 9c75 c415 0200 0042 0600 0011 0000  X..u.....B......
 00008b90: 0000 0000 0000 0000 0080 0198 0600 0077  ...............w
 00008ba0: 6f72 642f 646f 6375 6d65 6e74 2e78 6d6c  ord/document.xml
-00008bb0: 504b 0102 1403 1400 0000 0800 f486 6357  PK............cW
+00008bb0: 504b 0102 1403 1400 0000 0800 9d9e 9d58  PK.............X
 00008bc0: 6e80 1b12 3201 0000 cb04 0000 1c00 0000  n...2...........
 00008bd0: 0000 0000 0000 0000 8001 dc08 0000 776f  ..............wo
 00008be0: 7264 2f5f 7265 6c73 2f64 6f63 756d 656e  rd/_rels/documen
 00008bf0: 742e 786d 6c2e 7265 6c73 504b 0102 1403  t.xml.relsPK....
-00008c00: 1400 0000 0800 f486 6357 07d4 af99 732f  ........cW....s/
+00008c00: 1400 0000 0800 9d9e 9d58 07d4 af99 732f  .........X....s/
 00008c10: 0000 1255 0500 0f00 0000 0000 0000 0000  ...U............
 00008c20: 0000 8001 480a 0000 776f 7264 2f73 7479  ....H...word/sty
 00008c30: 6c65 732e 786d 6c50 4b01 0214 0314 0000  les.xmlPK.......
-00008c40: 0008 00f4 8663 5760 7982 d339 3500 0073  .....cW`y..95..s
+00008c40: 0008 009d 9e9d 5860 7982 d339 3500 0073  ......X`y..95..s
 00008c50: af06 001a 0000 0000 0000 0000 0000 0080  ................
 00008c60: 01e8 3900 0077 6f72 642f 7374 796c 6573  ..9..word/styles
 00008c70: 5769 7468 4566 6665 6374 732e 786d 6c50  WithEffects.xmlP
-00008c80: 4b01 0214 0314 0000 0008 00f4 8663 57a3  K............cW.
+00008c80: 4b01 0214 0314 0000 0008 009d 9e9d 58a3  K.............X.
 00008c90: 3f46 5fbf 0300 00e7 0900 0011 0000 0000  ?F_.............
 00008ca0: 0000 0000 0000 0080 0159 6f00 0077 6f72  .........Yo..wor
 00008cb0: 642f 7365 7474 696e 6773 2e78 6d6c 504b  d/settings.xmlPK
-00008cc0: 0102 1403 1400 0000 0800 f486 6357 e85a  ............cW.Z
+00008cc0: 0102 1403 1400 0000 0800 9d9e 9d58 e85a  .............X.Z
 00008cd0: e553 0001 0000 b601 0000 1400 0000 0000  .S..............
 00008ce0: 0000 0000 0000 8001 4773 0000 776f 7264  ........Gs..word
 00008cf0: 2f77 6562 5365 7474 696e 6773 2e78 6d6c  /webSettings.xml
-00008d00: 504b 0102 1403 1400 0000 0800 f486 6357  PK............cW
+00008d00: 504b 0102 1403 1400 0000 0800 9d9e 9d58  PK.............X
 00008d10: fb39 a073 6302 0000 fb0a 0000 1200 0000  .9.sc...........
 00008d20: 0000 0000 0000 0000 8001 7974 0000 776f  ..........yt..wo
 00008d30: 7264 2f66 6f6e 7454 6162 6c65 2e78 6d6c  rd/fontTable.xml
-00008d40: 504b 0102 1403 1400 0000 0800 f486 6357  PK............cW
+00008d40: 504b 0102 1403 1400 0000 0800 9d9e 9d58  PK.............X
 00008d50: 9441 22b8 c606 0000 bb2a 0000 1500 0000  .A"......*......
 00008d60: 0000 0000 0000 0000 8001 0c77 0000 776f  ...........w..wo
 00008d70: 7264 2f74 6865 6d65 2f74 6865 6d65 312e  rd/theme/theme1.
-00008d80: 786d 6c50 4b01 0214 0314 0000 0008 00f4  xmlPK...........
-00008d90: 8663 579e 803a d7a7 0000 0006 0100 0013  .cW..:..........
+00008d80: 786d 6c50 4b01 0214 0314 0000 0008 009d  xmlPK...........
+00008d90: 9e9d 589e 803a d7a7 0000 0006 0100 0013  ..X..:..........
 00008da0: 0000 0000 0000 0000 0000 0080 0105 7e00  ..............~.
 00008db0: 0063 7573 746f 6d58 6d6c 2f69 7465 6d31  .customXml/item1
 00008dc0: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
-00008dd0: f486 6357 3eca e5d5 bd00 0000 2701 0000  ..cW>.......'...
+00008dd0: 9d9e 9d58 3eca e5d5 bd00 0000 2701 0000  ...X>.......'...
 00008de0: 1e00 0000 0000 0000 0000 0000 8001 dd7e  ...............~
 00008df0: 0000 6375 7374 6f6d 586d 6c2f 5f72 656c  ..customXml/_rel
 00008e00: 732f 6974 656d 312e 786d 6c2e 7265 6c73  s/item1.xml.rels
-00008e10: 504b 0102 1403 1400 0000 0800 f486 6357  PK............cW
+00008e10: 504b 0102 1403 1400 0000 0800 9d9e 9d58  PK.............X
 00008e20: b5bb 4c4d e100 0000 6201 0000 1800 0000  ..LM....b.......
 00008e30: 0000 0000 0000 0000 8001 d67f 0000 6375  ..............cu
 00008e40: 7374 6f6d 586d 6c2f 6974 656d 5072 6f70  stomXml/itemProp
 00008e50: 7331 2e78 6d6c 504b 0102 1403 1400 0000  s1.xmlPK........
-00008e60: 0800 f486 6357 90d0 8789 6b03 0000 8915  ....cW....k.....
+00008e60: 0800 9d9e 9d58 90d0 8789 6b03 0000 8915  .....X....k.....
 00008e70: 0000 1200 0000 0000 0000 0000 0000 8001  ................
 00008e80: ed80 0000 776f 7264 2f6e 756d 6265 7269  ....word/numberi
 00008e90: 6e67 2e78 6d6c 504b 0102 1403 1400 0000  ng.xmlPK........
-00008ea0: 0800 f486 6357 a2c8 d667 bd05 0000 8420  ....cW...g..... 
+00008ea0: 0800 9d9e 9d58 a2c8 d667 bd05 0000 8420  .....X...g..... 
 00008eb0: 0000 1700 0000 0000 0000 0000 0000 8001  ................
 00008ec0: 8884 0000 646f 6350 726f 7073 2f74 6875  ....docProps/thu
 00008ed0: 6d62 6e61 696c 2e6a 7065 6750 4b05 0600  mbnail.jpegPK...
 00008ee0: 0000 0011 0011 0061 0400 007a 8a00 0000  .......a...z....
 00008ef0: 00                                       .
```

### Comparing `python-docx-1.1.0/features/blk-iter-inner-content.feature` & `python_docx-1.1.1/features/blk-iter-inner-content.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/doc-access-collections.feature` & `python_docx-1.1.1/features/doc-access-collections.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/doc-add-heading.feature` & `python_docx-1.1.1/features/doc-add-heading.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/doc-add-paragraph.feature` & `python_docx-1.1.1/features/doc-add-paragraph.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/doc-add-picture.feature` & `python_docx-1.1.1/features/doc-add-picture.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/doc-add-section.feature` & `python_docx-1.1.1/features/doc-add-section.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/doc-add-table.feature` & `python_docx-1.1.1/features/doc-add-table.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/doc-coreprops.feature` & `python_docx-1.1.1/features/doc-coreprops.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/doc-settings.feature` & `python_docx-1.1.1/features/doc-settings.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/doc-styles.feature` & `python_docx-1.1.1/features/doc-styles.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/hdr-header-footer.feature` & `python_docx-1.1.1/features/hdr-header-footer.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/hlk-props.feature` & `python_docx-1.1.1/features/hlk-props.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/img-characterize-image.feature` & `python_docx-1.1.1/features/img-characterize-image.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/par-access-inner-content.feature` & `python_docx-1.1.1/features/par-access-inner-content.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/par-add-run.feature` & `python_docx-1.1.1/features/par-add-run.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/par-alignment-prop.feature` & `python_docx-1.1.1/features/par-alignment-prop.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/par-insert-paragraph.feature` & `python_docx-1.1.1/features/par-insert-paragraph.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/par-style-prop.feature` & `python_docx-1.1.1/features/par-style-prop.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/pbk-split-para.feature` & `python_docx-1.1.1/features/pbk-split-para.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/run-access-inner-content.feature` & `python_docx-1.1.1/features/run-access-inner-content.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/run-add-picture.feature` & `python_docx-1.1.1/features/run-add-picture.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/run-char-style.feature` & `python_docx-1.1.1/features/run-char-style.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/run-enum-props.feature` & `python_docx-1.1.1/features/run-enum-props.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/sct-section.feature` & `python_docx-1.1.1/features/sct-section.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/shp-inline-shape-access.feature` & `python_docx-1.1.1/features/shp-inline-shape-access.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/shp-inline-shape-size.feature` & `python_docx-1.1.1/features/shp-inline-shape-size.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/api.py` & `python_docx-1.1.1/features/steps/api.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/block.py` & `python_docx-1.1.1/features/steps/block.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/coreprops.py` & `python_docx-1.1.1/features/steps/coreprops.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/document.py` & `python_docx-1.1.1/features/steps/document.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/font.py` & `python_docx-1.1.1/features/steps/font.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/hdrftr.py` & `python_docx-1.1.1/features/steps/hdrftr.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/helpers.py` & `python_docx-1.1.1/features/steps/helpers.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/hyperlink.py` & `python_docx-1.1.1/features/steps/hyperlink.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/image.py` & `python_docx-1.1.1/features/steps/image.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/numbering.py` & `python_docx-1.1.1/features/steps/numbering.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/pagebreak.py` & `python_docx-1.1.1/features/steps/pagebreak.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/paragraph.py` & `python_docx-1.1.1/features/steps/paragraph.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/parfmt.py` & `python_docx-1.1.1/features/steps/parfmt.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/section.py` & `python_docx-1.1.1/features/steps/section.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/settings.py` & `python_docx-1.1.1/features/steps/settings.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/shape.py` & `python_docx-1.1.1/features/steps/shape.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/shared.py` & `python_docx-1.1.1/features/steps/shared.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/styles.py` & `python_docx-1.1.1/features/steps/styles.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/table.py` & `python_docx-1.1.1/features/steps/table.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,481 +1,558 @@
+# pyright: reportPrivateUsage=false
+
 """Step implementations for table-related features."""
 
 from behave import given, then, when
+from behave.runner import Context
 
 from docx import Document
 from docx.enum.table import (
     WD_ALIGN_VERTICAL,
     WD_ROW_HEIGHT_RULE,
     WD_TABLE_ALIGNMENT,
     WD_TABLE_DIRECTION,
 )
 from docx.shared import Inches
-from docx.table import _Column, _Columns, _Row, _Rows
+from docx.table import Table, _Cell, _Column, _Columns, _Row, _Rows
 
 from helpers import test_docx
 
 # given ===================================================
 
 
 @given("a 2 x 2 table")
-def given_a_2x2_table(context):
+def given_a_2x2_table(context: Context):
     context.table_ = Document().add_table(rows=2, cols=2)
 
 
 @given("a 3x3 table having {span_state}")
-def given_a_3x3_table_having_span_state(context, span_state):
+def given_a_3x3_table_having_span_state(context: Context, span_state: str):
     table_idx = {
         "only uniform cells": 0,
         "a horizontal span": 1,
         "a vertical span": 2,
         "a combined span": 3,
     }[span_state]
     document = Document(test_docx("tbl-cell-access"))
     context.table_ = document.tables[table_idx]
 
 
+@given("a _Cell object spanning {count} layout-grid cells")
+def given_a_Cell_object_spanning_count_layout_grid_cells(context: Context, count: str):
+    document = Document(test_docx("tbl-cell-props"))
+    table = document.tables[0]
+    context.cell = _Cell(table._tbl.tr_lst[int(count)].tc_lst[0], table)
+
+
 @given("a _Cell object with {state} vertical alignment as cell")
-def given_a_Cell_object_with_vertical_alignment_as_cell(context, state):
+def given_a_Cell_object_with_vertical_alignment_as_cell(context: Context, state: str):
     table_idx = {
         "inherited": 0,
         "bottom": 1,
         "center": 2,
         "top": 3,
     }[state]
     document = Document(test_docx("tbl-props"))
     table = document.tables[table_idx]
     context.cell = table.cell(0, 0)
 
 
 @given("a column collection having two columns")
-def given_a_column_collection_having_two_columns(context):
+def given_a_column_collection_having_two_columns(context: Context):
     docx_path = test_docx("blk-containing-table")
     document = Document(docx_path)
     context.columns = document.tables[0].columns
 
 
 @given("a row collection having two rows")
-def given_a_row_collection_having_two_rows(context):
+def given_a_row_collection_having_two_rows(context: Context):
     docx_path = test_docx("blk-containing-table")
     document = Document(docx_path)
     context.rows = document.tables[0].rows
 
 
 @given("a table")
-def given_a_table(context):
+def given_a_table(context: Context):
     context.table_ = Document().add_table(rows=2, cols=2)
 
 
+@given("a table cell")
+def given_a_table_cell(context: Context):
+    table = Document(test_docx("tbl-2x2-table")).tables[0]
+    context.cell = table.cell(0, 0)
+
+
 @given("a table cell having a width of {width}")
-def given_a_table_cell_having_a_width_of_width(context, width):
+def given_a_table_cell_having_a_width_of_width(context: Context, width: str):
     table_idx = {"no explicit setting": 0, "1 inch": 1, "2 inches": 2}[width]
     document = Document(test_docx("tbl-props"))
     table = document.tables[table_idx]
     cell = table.cell(0, 0)
     context.cell = cell
 
 
 @given("a table column having a width of {width_desc}")
-def given_a_table_having_a_width_of_width_desc(context, width_desc):
+def given_a_table_having_a_width_of_width_desc(context: Context, width_desc: str):
     col_idx = {
         "no explicit setting": 0,
         "1440": 1,
     }[width_desc]
     docx_path = test_docx("tbl-col-props")
     document = Document(docx_path)
     context.column = document.tables[0].columns[col_idx]
 
 
 @given("a table having {alignment} alignment")
-def given_a_table_having_alignment_alignment(context, alignment):
+def given_a_table_having_alignment_alignment(context: Context, alignment: str):
     table_idx = {
         "inherited": 3,
         "left": 4,
         "right": 5,
         "center": 6,
     }[alignment]
     docx_path = test_docx("tbl-props")
     document = Document(docx_path)
     context.table_ = document.tables[table_idx]
 
 
 @given("a table having an autofit layout of {autofit}")
-def given_a_table_having_an_autofit_layout_of_autofit(context, autofit):
+def given_a_table_having_an_autofit_layout_of_autofit(context: Context, autofit: str):
     tbl_idx = {
         "no explicit setting": 0,
         "autofit": 1,
         "fixed": 2,
     }[autofit]
     document = Document(test_docx("tbl-props"))
     context.table_ = document.tables[tbl_idx]
 
 
 @given("a table having {style} style")
-def given_a_table_having_style(context, style):
+def given_a_table_having_style(context: Context, style: str):
     table_idx = {
         "no explicit": 0,
         "Table Grid": 1,
         "Light Shading - Accent 1": 2,
     }[style]
     document = Document(test_docx("tbl-having-applied-style"))
     context.document = document
     context.table_ = document.tables[table_idx]
 
 
 @given("a table having table direction set {setting}")
-def given_a_table_having_table_direction_setting(context, setting):
+def given_a_table_having_table_direction_setting(context: Context, setting: str):
     table_idx = ["to inherit", "right-to-left", "left-to-right"].index(setting)
     document = Document(test_docx("tbl-on-off-props"))
     context.table_ = document.tables[table_idx]
 
 
 @given("a table having two columns")
-def given_a_table_having_two_columns(context):
+def given_a_table_having_two_columns(context: Context):
     docx_path = test_docx("blk-containing-table")
     document = Document(docx_path)
     # context.table is used internally by behave, underscore added
     # to distinguish this one
     context.table_ = document.tables[0]
 
 
 @given("a table having two rows")
-def given_a_table_having_two_rows(context):
+def given_a_table_having_two_rows(context: Context):
     docx_path = test_docx("blk-containing-table")
     document = Document(docx_path)
     context.table_ = document.tables[0]
 
 
+@given("a table row ending with {count} empty grid columns")
+def given_a_table_row_ending_with_count_empty_grid_columns(context: Context, count: str):
+    document = Document(test_docx("tbl-props"))
+    table = document.tables[8]
+    context.row = table.rows[int(count)]
+
+
 @given("a table row having height of {state}")
-def given_a_table_row_having_height_of_state(context, state):
+def given_a_table_row_having_height_of_state(context: Context, state: str):
     table_idx = {"no explicit setting": 0, "2 inches": 2, "3 inches": 3}[state]
     document = Document(test_docx("tbl-props"))
     table = document.tables[table_idx]
     context.row = table.rows[0]
 
 
 @given("a table row having height rule {state}")
-def given_a_table_row_having_height_rule_state(context, state):
-    table_idx = {"no explicit setting": 0, "automatic": 1, "at least": 2, "exactly": 3}[
-        state
-    ]
+def given_a_table_row_having_height_rule_state(context: Context, state: str):
+    table_idx = {"no explicit setting": 0, "automatic": 1, "at least": 2, "exactly": 3}[state]
     document = Document(test_docx("tbl-props"))
     table = document.tables[table_idx]
     context.row = table.rows[0]
 
 
+@given("a table row starting with {count} empty grid columns")
+def given_a_table_row_starting_with_count_empty_grid_columns(context: Context, count: str):
+    document = Document(test_docx("tbl-props"))
+    table = document.tables[7]
+    context.row = table.rows[int(count)]
+
+
 # when =====================================================
 
 
 @when("I add a 1.0 inch column to the table")
-def when_I_add_a_1_inch_column_to_table(context):
+def when_I_add_a_1_inch_column_to_table(context: Context):
     context.column = context.table_.add_column(Inches(1.0))
 
 
+@when("I add a 2 x 2 table into the first cell")
+def when_I_add_a_2x2_table_into_the_first_cell(context: Context):
+    context.table_ = context.cell.add_table(2, 2)
+
+
 @when("I add a row to the table")
-def when_add_row_to_table(context):
+def when_add_row_to_table(context: Context):
     table = context.table_
     context.row = table.add_row()
 
 
+@when("I assign a string to the cell text attribute")
+def when_assign_string_to_cell_text_attribute(context: Context):
+    cell = context.cell
+    text = "foobar"
+    cell.text = text
+    context.expected_text = text
+
+
 @when("I assign {value} to cell.vertical_alignment")
-def when_I_assign_value_to_cell_vertical_alignment(context, value):
+def when_I_assign_value_to_cell_vertical_alignment(context: Context, value: str):
     context.cell.vertical_alignment = eval(value)
 
 
 @when("I assign {value} to row.height")
-def when_I_assign_value_to_row_height(context, value):
+def when_I_assign_value_to_row_height(context: Context, value: str):
     new_value = None if value == "None" else int(value)
     context.row.height = new_value
 
 
 @when("I assign {value} to row.height_rule")
-def when_I_assign_value_to_row_height_rule(context, value):
+def when_I_assign_value_to_row_height_rule(context: Context, value: str):
     new_value = None if value == "None" else getattr(WD_ROW_HEIGHT_RULE, value)
     context.row.height_rule = new_value
 
 
 @when("I assign {value_str} to table.alignment")
-def when_I_assign_value_to_table_alignment(context, value_str):
+def when_I_assign_value_to_table_alignment(context: Context, value_str: str):
     value = {
         "None": None,
         "WD_TABLE_ALIGNMENT.LEFT": WD_TABLE_ALIGNMENT.LEFT,
         "WD_TABLE_ALIGNMENT.RIGHT": WD_TABLE_ALIGNMENT.RIGHT,
         "WD_TABLE_ALIGNMENT.CENTER": WD_TABLE_ALIGNMENT.CENTER,
     }[value_str]
     table = context.table_
     table.alignment = value
 
 
 @when("I assign {value} to table.style")
-def when_apply_value_to_table_style(context, value):
+def when_apply_value_to_table_style(context: Context, value: str):
     table, styles = context.table_, context.document.styles
     if value == "None":
         new_value = None
     elif value.startswith("styles["):
         new_value = styles[value.split("'")[1]]
     else:
         new_value = styles[value]
     table.style = new_value
 
 
 @when("I assign {value} to table.table_direction")
-def when_assign_value_to_table_table_direction(context, value):
+def when_assign_value_to_table_table_direction(context: Context, value: str):
     new_value = None if value == "None" else getattr(WD_TABLE_DIRECTION, value)
     context.table_.table_direction = new_value
 
 
 @when("I merge from cell {origin} to cell {other}")
-def when_I_merge_from_cell_origin_to_cell_other(context, origin, other):
-    def cell(table, idx):
+def when_I_merge_from_cell_origin_to_cell_other(context: Context, origin: str, other: str):
+    def cell(table: Table, idx: int):
         row, col = idx // 3, idx % 3
         return table.cell(row, col)
 
     a_idx, b_idx = int(origin) - 1, int(other) - 1
     table = context.table_
     a, b = cell(table, a_idx), cell(table, b_idx)
     a.merge(b)
 
 
 @when("I set the cell width to {width}")
-def when_I_set_the_cell_width_to_width(context, width):
+def when_I_set_the_cell_width_to_width(context: Context, width: str):
     new_value = {"1 inch": Inches(1)}[width]
     context.cell.width = new_value
 
 
 @when("I set the column width to {width_emu}")
-def when_I_set_the_column_width_to_width_emu(context, width_emu):
+def when_I_set_the_column_width_to_width_emu(context: Context, width_emu: str):
     new_value = None if width_emu == "None" else int(width_emu)
     context.column.width = new_value
 
 
 @when("I set the table autofit to {setting}")
-def when_I_set_the_table_autofit_to_setting(context, setting):
+def when_I_set_the_table_autofit_to_setting(context: Context, setting: str):
     new_value = {"autofit": True, "fixed": False}[setting]
     table = context.table_
     table.autofit = new_value
 
 
 # then =====================================================
 
 
+@then("cell.grid_span is {count}")
+def then_cell_grid_span_is_count(context: Context, count: str):
+    expected = int(count)
+    actual = context.cell.grid_span
+    assert actual == expected, f"expected {expected}, got {actual}"
+
+
+@then("cell.tables[0] is a 2 x 2 table")
+def then_cell_tables_0_is_a_2x2_table(context: Context):
+    cell = context.cell
+    table = cell.tables[0]
+    assert len(table.rows) == 2
+    assert len(table.columns) == 2
+
+
 @then("cell.vertical_alignment is {value}")
-def then_cell_vertical_alignment_is_value(context, value):
+def then_cell_vertical_alignment_is_value(context: Context, value: str):
     expected_value = {
         "None": None,
         "WD_ALIGN_VERTICAL.BOTTOM": WD_ALIGN_VERTICAL.BOTTOM,
         "WD_ALIGN_VERTICAL.CENTER": WD_ALIGN_VERTICAL.CENTER,
     }[value]
     actual_value = context.cell.vertical_alignment
-    assert actual_value is expected_value, (
-        "cell.vertical_alignment is %s" % actual_value
-    )
+    assert actual_value is expected_value, "cell.vertical_alignment is %s" % actual_value
 
 
 @then("I can access a collection column by index")
-def then_can_access_collection_column_by_index(context):
+def then_can_access_collection_column_by_index(context: Context):
     columns = context.columns
     for idx in range(2):
         column = columns[idx]
         assert isinstance(column, _Column)
 
 
 @then("I can access a collection row by index")
-def then_can_access_collection_row_by_index(context):
+def then_can_access_collection_row_by_index(context: Context):
     rows = context.rows
     for idx in range(2):
         row = rows[idx]
         assert isinstance(row, _Row)
 
 
 @then("I can access the column collection of the table")
-def then_can_access_column_collection_of_table(context):
+def then_can_access_column_collection_of_table(context: Context):
     table = context.table_
     columns = table.columns
     assert isinstance(columns, _Columns)
 
 
 @then("I can access the row collection of the table")
-def then_can_access_row_collection_of_table(context):
+def then_can_access_row_collection_of_table(context: Context):
     table = context.table_
     rows = table.rows
     assert isinstance(rows, _Rows)
 
 
 @then("I can iterate over the column collection")
-def then_can_iterate_over_column_collection(context):
+def then_can_iterate_over_column_collection(context: Context):
     columns = context.columns
     actual_count = 0
     for column in columns:
         actual_count += 1
         assert isinstance(column, _Column)
     assert actual_count == 2
 
 
 @then("I can iterate over the row collection")
-def then_can_iterate_over_row_collection(context):
+def then_can_iterate_over_row_collection(context: Context):
     rows = context.rows
     actual_count = 0
     for row in rows:
         actual_count += 1
         assert isinstance(row, _Row)
     assert actual_count == 2
 
 
+@then("row.grid_cols_after is {value}")
+def then_row_grid_cols_after_is_value(context: Context, value: str):
+    expected = int(value)
+    actual = context.row.grid_cols_after
+    assert actual == expected, "expected %s, got %s" % (expected, actual)
+
+
+@then("row.grid_cols_before is {value}")
+def then_row_grid_cols_before_is_value(context: Context, value: str):
+    expected = int(value)
+    actual = context.row.grid_cols_before
+    assert actual == expected, "expected %s, got %s" % (expected, actual)
+
+
 @then("row.height is {value}")
-def then_row_height_is_value(context, value):
+def then_row_height_is_value(context: Context, value: str):
     expected_height = None if value == "None" else int(value)
     actual_height = context.row.height
     assert actual_height == expected_height, "expected %s, got %s" % (
         expected_height,
         actual_height,
     )
 
 
 @then("row.height_rule is {value}")
-def then_row_height_rule_is_value(context, value):
+def then_row_height_rule_is_value(context: Context, value: str):
     expected_rule = None if value == "None" else getattr(WD_ROW_HEIGHT_RULE, value)
     actual_rule = context.row.height_rule
     assert actual_rule == expected_rule, "expected %s, got %s" % (
         expected_rule,
         actual_rule,
     )
 
 
 @then("table.alignment is {value_str}")
-def then_table_alignment_is_value(context, value_str):
+def then_table_alignment_is_value(context: Context, value_str: str):
     value = {
         "None": None,
         "WD_TABLE_ALIGNMENT.LEFT": WD_TABLE_ALIGNMENT.LEFT,
         "WD_TABLE_ALIGNMENT.RIGHT": WD_TABLE_ALIGNMENT.RIGHT,
         "WD_TABLE_ALIGNMENT.CENTER": WD_TABLE_ALIGNMENT.CENTER,
     }[value_str]
     table = context.table_
     assert table.alignment == value, "got %s" % table.alignment
 
 
 @then("table.cell({row}, {col}).text is {expected_text}")
-def then_table_cell_row_col_text_is_text(context, row, col, expected_text):
+def then_table_cell_row_col_text_is_text(context: Context, row: str, col: str, expected_text: str):
     table = context.table_
     row_idx, col_idx = int(row), int(col)
     cell_text = table.cell(row_idx, col_idx).text
     assert cell_text == expected_text, "got %s" % cell_text
 
 
 @then("table.style is styles['{style_name}']")
-def then_table_style_is_styles_style_name(context, style_name):
+def then_table_style_is_styles_style_name(context: Context, style_name: str):
     table, styles = context.table_, context.document.styles
     expected_style = styles[style_name]
     assert table.style == expected_style, "got '%s'" % table.style
 
 
 @then("table.table_direction is {value}")
-def then_table_table_direction_is_value(context, value):
+def then_table_table_direction_is_value(context: Context, value: str):
     expected_value = None if value == "None" else getattr(WD_TABLE_DIRECTION, value)
     actual_value = context.table_.table_direction
     assert actual_value == expected_value, "got '%s'" % actual_value
 
 
+@then("the cell contains the string I assigned")
+def then_cell_contains_string_assigned(context: Context):
+    cell, expected_text = context.cell, context.expected_text
+    text = cell.paragraphs[0].runs[0].text
+    msg = "expected '%s', got '%s'" % (expected_text, text)
+    assert text == expected_text, msg
+
+
 @then("the column cells text is {expected_text}")
-def then_the_column_cells_text_is_expected_text(context, expected_text):
+def then_the_column_cells_text_is_expected_text(context: Context, expected_text: str):
     table = context.table_
     cells_text = " ".join(c.text for col in table.columns for c in col.cells)
     assert cells_text == expected_text, "got %s" % cells_text
 
 
 @then("the length of the column collection is 2")
-def then_len_of_column_collection_is_2(context):
+def then_len_of_column_collection_is_2(context: Context):
     columns = context.table_.columns
     assert len(columns) == 2
 
 
 @then("the length of the row collection is 2")
-def then_len_of_row_collection_is_2(context):
+def then_len_of_row_collection_is_2(context: Context):
     rows = context.table_.rows
     assert len(rows) == 2
 
 
 @then("the new column has 2 cells")
-def then_new_column_has_2_cells(context):
+def then_new_column_has_2_cells(context: Context):
     assert len(context.column.cells) == 2
 
 
 @then("the new column is 1.0 inches wide")
-def then_new_column_is_1_inches_wide(context):
+def then_new_column_is_1_inches_wide(context: Context):
     assert context.column.width == Inches(1)
 
 
 @then("the new row has 2 cells")
-def then_new_row_has_2_cells(context):
+def then_new_row_has_2_cells(context: Context):
     assert len(context.row.cells) == 2
 
 
 @then("the reported autofit setting is {autofit}")
-def then_the_reported_autofit_setting_is_autofit(context, autofit):
+def then_the_reported_autofit_setting_is_autofit(context: Context, autofit: str):
     expected_value = {"autofit": True, "fixed": False}[autofit]
     table = context.table_
     assert table.autofit is expected_value
 
 
 @then("the reported column width is {width_emu}")
-def then_the_reported_column_width_is_width_emu(context, width_emu):
+def then_the_reported_column_width_is_width_emu(context: Context, width_emu: str):
     expected_value = None if width_emu == "None" else int(width_emu)
     assert context.column.width == expected_value, "got %s" % context.column.width
 
 
 @then("the reported width of the cell is {width}")
-def then_the_reported_width_of_the_cell_is_width(context, width):
+def then_the_reported_width_of_the_cell_is_width(context: Context, width: str):
     expected_width = {"None": None, "1 inch": Inches(1)}[width]
     actual_width = context.cell.width
     assert actual_width == expected_width, "expected %s, got %s" % (
         expected_width,
         actual_width,
     )
 
 
 @then("the row cells text is {encoded_text}")
-def then_the_row_cells_text_is_expected_text(context, encoded_text):
+def then_the_row_cells_text_is_expected_text(context: Context, encoded_text: str):
     expected_text = encoded_text.replace("\\", "\n")
     table = context.table_
     cells_text = " ".join(c.text for row in table.rows for c in row.cells)
     assert cells_text == expected_text, "got %s" % cells_text
 
 
 @then("the table has {count} columns")
-def then_table_has_count_columns(context, count):
+def then_table_has_count_columns(context: Context, count: str):
     column_count = int(count)
     columns = context.table_.columns
     assert len(columns) == column_count
 
 
 @then("the table has {count} rows")
-def then_table_has_count_rows(context, count):
+def then_table_has_count_rows(context: Context, count: str):
     row_count = int(count)
     rows = context.table_.rows
     assert len(rows) == row_count
 
 
 @then("the width of cell {n_str} is {inches_str} inches")
-def then_the_width_of_cell_n_is_x_inches(context, n_str, inches_str):
-    def _cell(table, idx):
+def then_the_width_of_cell_n_is_x_inches(context: Context, n_str: str, inches_str: str):
+    def _cell(table: Table, idx: int):
         row, col = idx // 3, idx % 3
         return table.cell(row, col)
 
     idx, inches = int(n_str) - 1, float(inches_str)
     cell = _cell(context.table_, idx)
+    assert cell.width is not None
     assert cell.width == Inches(inches), "got %s" % cell.width.inches
 
 
 @then("the width of each cell is {inches} inches")
-def then_the_width_of_each_cell_is_inches(context, inches):
+def then_the_width_of_each_cell_is_inches(context: Context, inches: str):
     table = context.table_
     expected_width = Inches(float(inches))
     for cell in table._cells:
         assert cell.width == expected_width, "got %s" % cell.width.inches
 
 
 @then("the width of each column is {inches} inches")
-def then_the_width_of_each_column_is_inches(context, inches):
+def then_the_width_of_each_column_is_inches(context: Context, inches: str):
     table = context.table_
     expected_width = Inches(float(inches))
     for column in table.columns:
         assert column.width == expected_width, "got %s" % column.width.inches
```

### Comparing `python-docx-1.1.0/features/steps/tabstops.py` & `python_docx-1.1.1/features/steps/tabstops.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/blk-containing-table.docx` & `python_docx-1.1.1/features/steps/test_files/blk-containing-table.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/blk-paras-and-tables.docx` & `python_docx-1.1.1/features/steps/test_files/blk-paras-and-tables.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/court-exif.jpg` & `python_docx-1.1.1/features/steps/test_files/court-exif.jpg`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/doc-access-sections.docx` & `python_docx-1.1.1/features/steps/test_files/doc-access-sections.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/doc-add-section.docx` & `python_docx-1.1.1/features/steps/test_files/doc-add-section.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/doc-coreprops.docx` & `python_docx-1.1.1/features/steps/test_files/doc-coreprops.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/doc-default.docx` & `python_docx-1.1.1/features/steps/test_files/doc-default.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/doc-no-coreprops.docx` & `python_docx-1.1.1/features/steps/test_files/doc-no-coreprops.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/doc-odd-even-hdrs.docx` & `python_docx-1.1.1/features/steps/test_files/doc-odd-even-hdrs.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/doc-word-default-blank.docx` & `python_docx-1.1.1/features/steps/test_files/doc-word-default-blank.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/fnt-color.docx` & `python_docx-1.1.1/features/steps/test_files/fnt-color.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/hdr-header-footer.docx` & `python_docx-1.1.1/features/steps/test_files/hdr-header-footer.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/jfif-300-dpi.jpg` & `python_docx-1.1.1/features/steps/test_files/jfif-300-dpi.jpg`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/jpeg420exif.jpg` & `python_docx-1.1.1/features/steps/test_files/jpeg420exif.jpg`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/lena.bmp` & `python_docx-1.1.1/features/steps/test_files/lena.bmp`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/lena.gif` & `python_docx-1.1.1/features/steps/test_files/lena.gif`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/lena.tif` & `python_docx-1.1.1/features/steps/test_files/lena.tif`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/lena_std.jpg` & `python_docx-1.1.1/features/steps/test_files/lena_std.jpg`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/monty-truth.png` & `python_docx-1.1.1/features/steps/test_files/monty-truth.png`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/mountain.bmp` & `python_docx-1.1.1/features/steps/test_files/mountain.bmp`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/num-having-numbering-part.docx` & `python_docx-1.1.1/features/steps/test_files/num-having-numbering-part.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/par-alignment.docx` & `python_docx-1.1.1/features/steps/test_files/par-alignment.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/par-hlink-frags.docx` & `python_docx-1.1.1/features/steps/test_files/par-hlink-frags.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/par-hyperlinks.docx` & `python_docx-1.1.1/features/steps/test_files/par-hyperlinks.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/par-known-paragraphs.docx` & `python_docx-1.1.1/features/steps/test_files/par-known-paragraphs.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/par-known-styles.docx` & `python_docx-1.1.1/features/steps/test_files/par-known-styles.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/par-rendered-page-breaks.docx` & `python_docx-1.1.1/features/steps/test_files/par-rendered-page-breaks.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/python-icon.jpeg` & `python_docx-1.1.1/features/steps/test_files/python-icon.jpeg`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/run-char-style.docx` & `python_docx-1.1.1/features/steps/test_files/run-char-style.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/run-enumerated-props.docx` & `python_docx-1.1.1/features/steps/test_files/run-enumerated-props.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/sample.tif` & `python_docx-1.1.1/features/steps/test_files/sample.tif`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/sct-first-page-hdrftr.docx` & `python_docx-1.1.1/features/steps/test_files/sct-first-page-hdrftr.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/sct-inner-content.docx` & `python_docx-1.1.1/features/steps/test_files/sct-inner-content.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/sct-section-props.docx` & `python_docx-1.1.1/features/steps/test_files/sct-section-props.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/set-no-settings-part.docx` & `python_docx-1.1.1/features/steps/test_files/set-no-settings-part.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/shp-inline-shape-access.docx` & `python_docx-1.1.1/features/steps/test_files/shp-inline-shape-access.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/sty-behav-props.docx` & `python_docx-1.1.1/features/steps/test_files/sty-behav-props.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/sty-having-no-styles-part.docx` & `python_docx-1.1.1/features/steps/test_files/sty-having-no-styles-part.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/sty-having-styles-part.docx` & `python_docx-1.1.1/features/steps/test_files/sty-having-styles-part.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/sty-known-styles.docx` & `python_docx-1.1.1/features/steps/test_files/sty-known-styles.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/tab-stops.docx` & `python_docx-1.1.1/features/steps/test_files/tab-stops.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/tbl-2x2-table.docx` & `python_docx-1.1.1/features/steps/test_files/tbl-2x2-table.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/tbl-cell-access.docx` & `python_docx-1.1.1/features/steps/test_files/tbl-cell-access.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/tbl-col-props.docx` & `python_docx-1.1.1/features/steps/test_files/tbl-col-props.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/tbl-having-applied-style.docx` & `python_docx-1.1.1/features/steps/test_files/tbl-having-applied-style.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/tbl-having-tables.docx` & `python_docx-1.1.1/features/steps/test_files/tbl-having-tables.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/tbl-on-off-props.docx` & `python_docx-1.1.1/features/steps/test_files/tbl-on-off-props.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/tbl-props.docx` & `python_docx-1.1.1/features/steps/test_files/tbl-props.docx`

 * *Files 10% similar despite different names*

```diff
@@ -658,605 +658,620 @@
 00002910: 9029 5d05 28e8 ce89 4316 e527 292e e6a4  .)].(...C..')...
 00002920: 7887 cde3 01c8 c89c 60b9 9c93 455b 8385  x.......`...E[..
 00002930: dcb4 f047 f26b 4d70 2ce7 e4c0 b03b 62d8  ...G.kMp,....;b.
 00002940: ca6f 339d c048 673d 101c 5a18 9fc7 564f  .o3..Hg=..Z...VO
 00002950: 102c 4e10 748d 72d6 5b8d b1b2 dd4f f957  .,N.t.r.[....O.W
 00002960: e9d5 d1d2 e706 eb3b ad41 e141 ff68 b443  .......;.A.A.h.C
 00002970: c9f8 de1f cca3 4f50 4b03 0414 0000 0008  ......OPK.......
-00002980: 00b7 8964 4923 5256 afc3 0500 00e9 3500  ...dI#RV......5.
-00002990: 0011 0000 0077 6f72 642f 646f 6375 6d65  .....word/docume
-000029a0: 6e74 2e78 6d6c ed5b 5b73 9b38 147e efaf  nt.xml.[[s.8.~..
-000029b0: f0f8 254f ad25 2110 789a 7610 866e 67da  ..%O.%!.x.v..ng.
-000029c0: 994c d3dd 7ddc 5130 b6d9 0062 408e 93fd  .L..}.Q0...b@...
-000029d0: f52b 71b1 719c daf8 92d8 8d93 1773 74f9  .+q.q........st.
-000029e0: f49d 7374 8e0e 977c fc7c 1f47 9dbb 20cb  ..st...|.|.G.. .
-000029f0: 439e 5c5e c00f e0a2 1324 3e1f 86c9 f8f2  C.\^.....$>.....
-00002a00: e2cf 9fde 7bf3 a293 0b96 0c59 c493 e0f2  ....{......Y....
-00002a10: e221 c82f 3e7f 7af7 71d6 1f72 7f1a 0789  .!./>.z.q..r....
-00002a20: e848 8424 efcf 52ff b23b 1122 edf7 7ab9  .H.$..R..;."..z.
-00002a30: 3f09 6296 7f88 433f e339 1f89 0f3e 8f7b  ?.b...C?.9...>.{
-00002a40: 7c34 0afd a037 e3d9 b087 0004 c555 9a71  |4...7.......U.q
-00002a50: 3fc8 73b9 9cc3 923b 9677 2bb8 98b7 438b  ?.s....;.w+...C.
-00002a60: 995f 5f22 004c 2987 c91c 6395 114f 8344  .__".L)...c..O.D
-00002a70: 768e 7816 3321 c56c 2c67 64b7 d3f4 bdc4  v.x.3!.l,gd.....
-00002a80: 4c99 086f c228 140f 0acb 98c3 dc5d 76a7  L..o.(.......]v.
-00002a90: 59d2 af30 decf 79a8 397d 49a0 7f17 47f5  Y..0..y.9}I...G.
-00002aa0: 60be 6e6c 49b4 faa9 6764 6d48 9653 0695  `.nlI...gdmH.S..
-00002ab0: c90b 7abd 2c88 2461 9ee4 9330 5dd8 6d57  ..z.,.$a...0].mW
-00002ac0: 34d9 39a9 41d6 2adc 5076 9642 bc9f d307  4.9.A.*.Pv.B....
-00002ad0: 199b c99f 0560 1bfa c372 521c 95cc d723  .....`...rR....#
-00002ae0: 42d0 c223 0a62 3ea3 0d85 e535 6b26 cdcd  B..#.b>....5k&..
-00002af0: 37db cd34 4de3 8ef7 b3ed 978c 4fd3 055a  7..4M.......O..Z
-00002b00: b81f dad7 e476 8e25 13c1 3658 958f 9aaa  .....v.%..6X....
-00002b10: e5fb 91b9 9eb0 5406 50ec f7bf 8e13 9eb1  ......T.P.......
-00002b20: 9b48 3292 16ef a81d d9fd f4ae d391 09ea  .H2.............
-00002b30: 860f 1fd4 6521 889b a8bc aea5 abac 96eb  ....e!..........
-00002b40: 966b f110 059d 59ff 8e45 97dd 9f0a f34b  .k....Y..E.....K
-00002b50: 160e bbbd c7e3 fe96 63e4 2601 5df9 2b1e  ........c.&.].+.
-00002b60: 52b9 329b 0abe 3aee 1be7 b735 1cc0 7631  R.2...:....5..v1
-00002b70: 7e14 66b9 f8c1 e574 a8c4 8855 d2a2 d3e1  ~.f....t...U....
-00002b80: d134 4e1a fd75 4331 24e1 7f50 998c e7d2  .4N..uC1$..P....
-00002b90: 5fa5 0417 ab7f ec3d 52af 24a3 5459 2238  _......=R.$.TY"8
-00002ba0: 960d 12ba d405 21b4 82d0 9ca1 3032 3954  ......!.....029T
-00002bb0: 1e13 c31f 7271 6053 0d58 8a22 c4fd 9465  ....rq`S.X."...e
-00002bc0: ecab 2481 5c8f 10e2 e865 ab08 ee85 6a25  ..$.\....e....j%
-00002bd0: d55f b79a fe33 6bcc 5f36 99bf 10ab 86a6  ._...3k._6......
-00002be0: 93e6 8d9b ed5f e9f0 68ba 9c9c 2e11 063a  ....._..h......:
-00002bf0: 7609 f5dc f584 97f5 2d9b 06c1 884d 23d1  v.......-....M#.
-00002c00: e869 7abf d7d4 a590 2a1e 9565 e79b 7299  .iz.....*..e..r.
-00002c10: 8e61 50db 321d d882 0ed4 01c1 f429 3a55  .aP.2........):U
-00002c20: 4fef 981b df09 a2e8 3b7b 6cfb 2818 8912  O.......;{l.(...
-00002c30: 0042 7d01 31bc 678f 5c27 950a c793 1663  .B}.1.g.\'.....c
-00002c40: 2b73 ae2c f7db 851f c418 ec1f 7f40 7321  +s.,.........@s!
-00002c50: 31bc 0dfb 674d fc65 2bf1 22b2 3f82 ca17  1...gM.e+.".?...
-00002c60: a51d 15ca e4c7 347a caf7 bdc7 10db c774  ......4z.......t
-00002c70: 6188 5f6f 8d62 f09d 1d85 e3a4 6674 c385  a._o.b......ft..
-00002c80: e0f1 0ec1 0f3d 5383 0e1e 9c48 f013 6a39  .....=S....H..j9
-00002c90: 1645 f480 748e 74ea b107 3e15 f341 a3f0  .E..t.t...>..A..
-00002ca0: 3e78 02ed 2d45 6c7b 429b e601 5204 d20c  >x..-El{B...R...
-00002cb0: 6212 c379 c614 5110 6d64 09f1 2d90 263a  b..y..Q.md..-.&:
-00002cc0: 74a2 a857 699f 287c 79a7 1364 3b24 0a0c  t..Wi.(|y..d;$..
-00002cd0: 3d8b 6ae4 5412 85ae 3bc8 335d d082 8e6e  =.j.T...;.3]...n
-00002ce0: 0287 e2a7 e82c f75c 359a 8e9b 3b7e 9f78  .....,.\5...;~.x
-00002cf0: 5c3e b2f7 ed6f 13cf 739f 358f 7c8f 581e  \>...o..s.5.|.X.
-00002d00: c6b8 4d3c 5b3a f406 c6d6 f18c 35d4 8ce7  ..M<[:......5...
-00002d10: e09e f907 8fe6 ed8f 7dc1 d31d 4259 d306  ........}...BY..
-00002d20: 880c cc0d 7728 dbc7 4e65 da5f 46f7 33d8  ....w(..Ne._F.3.
-00002d30: a495 be68 800c 0d90 0de9 fe35 e90b 5dea  ...h.......5..].
-00002d40: ea6d 6ee8 0eaa 6f33 7bb7 8c5c 0d99 d4d2  .mn...o3{..\....
-00002d50: 1c6d e7c8 7d79 ebea 5896 a8f2 e839 97dd  .m..}y..X....9..
-00002d60: 0489 0d3d 0358 e7a2 af46 0d93 386e 9be7  ...=.X...F..8n..
-00002d70: 0fcf 163d eb6b 1fe4 5140 2ce3 e00c 8f5e  ...=.k..Q@,....^
-00002d80: fbfc ebd7 48ea 16e8 ad30 dabb 30d2 9165  ....H....0..0..e
-00002d90: 611b 9367 2c8c 7462 1cbb 306a 7728 0234  a..g,.tb..0jw(.4
-00002da0: d06d 6383 295e 4f1a 0386 075d ec7a 67a3  .mc.)^O....].zg.
-00002db0: afe9 9a98 6a47 4ddb 6da3 1250 c7d4 ec0d  ....jGM.m..P....
-00002dc0: 27ea 6915 3d03 47d3 4b72 67b1 9b90 e579  '.i.=.G.Krg....y
-00002dd0: d8b2 ce26 7a30 a426 32bc 364f 778e 54f4  ...&z0.&2.6Ow.T.
-00002de0: 1814 6a03 871e fc26 ee84 8a9e e261 ee5b  ..j....&.....a.[
-00002df0: d5b3 77d5 836c db04 146d 08de 32bf 56f3  ..w..l...m..2.V.
-00002e00: 3755 3deb 9c74 2205 0ec1 8078 167a f110  7U=..t"....x.z..
-00002e10: 3e9a bec0 f590 dbea cdd5 abd0 17a1 01c0  >...............
-00002e20: 9afa 1eeb f40b 1cd3 1e68 80d8 e715 80b2  .........h......
-00002e30: aa83 0e70 cf67 436a 1079 06dc f0d4 fd15  ...p.gCj.y......
-00002e40: e96b 1102 0d7b c3ae 3e66 8d04 08b2 6cdd  .k...{..>f....l.
-00002e50: 68f3 f6fc 77ad 9156 df5f be15 49bb bd33  h...w..V._..I..3
-00002e60: 7310 d509 68f5 99cc d639 fa09 2f9d 4892  s...h....9../.H.
-00002e70: 3634 4aa9 a73f 57d2 5a21 7f23 f7a5 fab4  64J..?W.Z!.#....
-00002e80: fa5a b04c 3d33 0be7 db89 c552 897f be70  .Z.L=3.....R...p
-00002e90: cafc db55 45d2 53cb 7e1a b689 0bbd f379  ...UE.S.~......y
-00002ea0: 0240 2c6c 23f3 c54f b75d 5ea2 7980 526b  .@,l#..O.]^.y.Rk
-00002eb0: d307 9caf 2e94 894e 7593 ba2f 7e1e 1fed  .......Nu../~...
-00002ec0: 191c 7074 53f7 d0b9 e88b 3105 0645 e6d1  ..ptS.....1..E..
-00002ed0: 23b0 cee1 6e32 9c67 f0ba 165a 5b8f 699e  #...n2.g...Z[.i.
-00002ee0: 4b11 b60f a2c1 a2f8 ca03 5f5c 3d9d 148a  K........._\=...
-00002ef0: a66b d9af 5a81 860d b838 9214 bbf1 f57f  .k..Z....8......
-00002f00: 957f 102a 1d34 91d7 bab9 5450 a871 df99  ...*.4....TP.q..
-00002f10: 5a40 f074 e1ca e2be 4b8a 2628 c4f2 8bd3  Z@.t....K.&(....
-00002f20: 45b7 7a63 b7e8 9d04 6c18 c884 43ca af66  E.zc....l...C..f
-00002f30: 469c 8b86 389e 8a42 5c5e d5e7 512e 3bf3  F...8..B\^..Q.;.
-00002f40: 94f9 4139 b4d9 3be4 beaa 71d4 4a61 125c  ..A9..;...q.Ja.\
-00002f50: 85c2 97d4 3563 c913 a565 94ac a4f2 1f1f  ....5c...e......
-00002f60: d455 fd3f 5a9f defd 0f50 4b03 0414 0000  .U.?Z....PK.....
-00002f70: 0008 00b7 8964 491b eedb 0322 0200 00ac  .....dI...."....
-00002f80: 0800 0012 0000 0077 6f72 642f 666f 6e74  .......word/font
-00002f90: 5461 626c 652e 786d 6ce5 953f 6edb 3014  Table.xml..?n.0.
-00002fa0: c677 9f82 d0a2 2916 252b a96b 580e dab4  .w....).%+.kX...
-00002fb0: 06ba 7428 dc03 d034 6513 e51f 81a4 ec78  ..t(...4e......x
-00002fc0: 75f6 ce1d da23 141d 5aa0 4b6e 6320 6bae  u....#..Z.Knc k.
-00002fd0: 9017 5a56 1434 76e3 a129 d052 1044 be8f  ..ZV.4v..).R.D..
-00002fe0: fcf4 f8c3 23d8 3f3d 9702 cd99 b15c ab2c  ....#.?=.....\.,
-00002ff0: 8cdb 3844 4c51 3de1 6a9a 85ef 47c3 a36e  ..8DLQ=.j...G..n
-00003000: 88ac 236a 4284 562c 0b97 cc86 a783 567f  ..#jB.V,......V.
-00003010: d1cb b572 16c1 7265 7b92 66c1 ccb9 a217  ...r..re{.f.....
-00003020: 4596 ce98 24b6 ad0b a640 ccb5 91c4 c1d0  E...$....@......
-00003030: 4c23 49cc 87b2 38a2 5a16 c4f1 3117 dc2d  L#I...8.Z...1..-
-00003040: a304 e393 a0b2 318f 71d1 79ce 297b a569  ......1.q.y.){.i
-00003050: 2999 727e 7d64 9800 47ad ec8c 1776 ebb6  ).r~}d..G....v..
-00003060: 788c db42 9b49 6134 65d6 c296 a5d8 f849  x..B.Ia4e......I
-00003070: c255 6d13 a7bf 1849 4e8d b63a 776d d84c  .Um....IN..:wm.L
-00003080: 9591 b782 e531 f63d 2902 2469 efcd 5469  .....1.=).$i..Ti
-00003090: 43c6 8265 0118 0583 1642 153b b4e8 2922  C..e.....B.;..)"
-000030a0: 217e 46e4 d870 e235 af16 4469 cb62 9830  !~F..p.5..Di.b.0
-000030b0: 2722 0b70 8253 7c8c 3bf0 a6f8 04be 300e  '".p.S|.;.....0.
-000030c0: a27a 369d 1163 99ab 67e3 8696 13c9 c572  .z6..c..g......r
-000030d0: 2b91 d2e9 8658 7047 675b 6d4e 2005 48b3  +....XpGg[mN .H.
-000030e0: a15b 3e05 b5b4 639c 05af 31b4 6438 0c36  .[>...c...1.d8.6
-000030f0: 9138 0bd2 db48 5a47 92db 3f6f 5a15 e9dc  .8...HZG..?oZ...
-00003100: 8f50 efe3 87f1 f361 1589 1b73 fc8f fbd1  .P.....a...s....
-00003110: 06ce 439c ae2f bf5e 5f7e 4757 9f3e 5e7d  ..C../.^_~GW.>^}
-00003120: feb2 9bd6 036d 37ad ee6e 5a46 4ba2 1aaa  .....m7..nZFK...
-00003130: d26e 644a 365a 166c 07c3 9c9f b3c9 0e80  .ndJ6Z.l........
-00003140: 5526 f11d 40dc c5cf 1ab8 6a80 f1ef 0026  U&..@.....j....&
-00003150: 8dc8 4100 475c 328b deb2 057a e7f7 b6a7  ..A.G\2....z....
-00003160: e012 5f68 c7be f012 e83d 79c1 559b ea34  .._h.....=y.U..4
-00003170: 78dd 2faf 430a aee2 7e28 af17 90a1 d847  x./.C...~(.....G
-00003180: e925 504a 3dad cdf3 5f52 aa8e e57a f563  .%PJ=..._R...z.c
-00003190: bdfa b9be b858 afbe fdf9 c329 f584 997f  .....X.....)....
-000031a0: eb74 9e11 c1e1 1ed8 576f 437f 1a7d a5fd  .t......WoC..}..
-000031b0: 9d6b e0e9 eb6d dbb3 83d6 0d50 4b03 0414  .k...m.....PK...
-000031c0: 0000 0008 00b7 8964 4975 6432 89c1 0300  .......dIud2....
-000031d0: 0032 0a00 0011 0000 0077 6f72 642f 7365  .2.......word/se
-000031e0: 7474 696e 6773 2e78 6d6c b556 db6e e336  ttings.xml.V.n.6
-000031f0: 107d cf57 087a f14b 1d49 be25 35e2 2c92  .}.W.z.K.I.%5.,.
-00003200: b86e 13c4 dda0 ca7e 0025 8d6d 36bc 81a4  .n.....~.%.m6...
-00003210: ec78 bfbe 4349 9464 04e9 1a5d f4c9 9a39  .x..CI.d...]...9
-00003220: 672e 1cce 0c7d f3e5 9db3 600f da50 2916  g....}....`..P).
-00003230: 83e4 321e 0420 7259 50b1 5d0c bebd ae86  ..2.. rYP.].....
-00003240: d783 c058 220a c2a4 80c5 e008 66f0 e5f6  ...X".......f...
-00003250: e2e6 3037 602d b24c 801e 8499 f37c 11ee  ..07`-.L.....|..
-00003260: ac55 f328 32f9 0e38 3197 5281 4070 2335  .U.(2..81.R.@p#5
-00003270: 2716 45bd 8d38 d16f a51a e692 2b62 6946  '.E..8.o....+biF
-00003280: 19b5 c768 14c7 b3b0 7123 1761 a9c5 bc71  ...h....q#.a...q
-00003290: 31e4 34d7 d2c8 8d75 2673 b9d9 d01c 9a1f  1.4....u&s......
-000032a0: 6fa1 cf89 5b9b 2c65 5e72 10b6 8a18 6960  o...[.,e^r....i`
-000032b0: 9883 1466 4795 f1de f87f f586 e0ce 3bd9  ...fG.........;.
-000032c0: ffdb 21f6 9c79 de21 89cf 38ee 41ea a2b5  ..!..y.!..8.A...
-000032d0: 3827 3d67 a0b4 ccc1 18bc 20ce 7c82 5474  8'=g...... .|.Tt
-000032e0: 8127 1f1c b5b1 2f31 7673 c4ca 159a 2771  .'..../1vs....'q
-000032f0: f5d5 656e d839 89d4 d033 cd34 d1c7 7e16  ..en.9...3.4..~.
-00003300: 3c9f 3f6e 85d4 2463 b008 319b f0f6 2208  <.?n..$c..1...".
-00003310: b0a9 be4b c983 c37c 4fd0 7f06 c6ae a80d  ...K...|O.......
-00003320: 5156 a073 acf4 221c 25d7 61d4 70f1 8872  QV.s..".%.a.p..r
-00003330: 935a 6201 1946 0163 ae69 c39c 0111 ce68  .Zb..F.c.i.....h
-00003340: ab09 c77e f31a 6f56 c086 94cc be92 2cb5  ...~..oV......,.
-00003350: 52f9 6057 a3b8 65e4 3ba2 496e 41a7 8ae4  R.`W..e.;.InA...
-00003360: e8f3 410a ab25 f3d4 42fe 29ed 0376 b0c6  ..A..%..B.)..v..
-00003370: 02b7 4686 ece1 45c3 9ec2 e185 e6b6 d4d0  ..F...E.........
-00003380: baab 9add 0995 581a 58fd f64c 8eb2 b451  ......X.X..L...Q
-00003390: abac 3969 3d52 1848 108e 8539 1993 b52c  ..9i=R.H...9...,
-000033a0: c01d abd4 f4fc bb0b 7dd2 58e2 1f45 93b8  ........}.X..E..
-000033b0: 0634 2de0 d5dd 4a6a 8f0c 5678 f094 7e87  .4-...Jj..Vx..~.
-000033c0: 3b51 3c95 c652 745b 4dcc 4fa4 f1c3 2c40  ;Q<..Rt[M.O...,@
-000033d0: b8f0 5fb1 995e 8f0a 5640 5c29 cdff 19b1  .._..^..V@\)....
-000033e0: bacf 15a3 6a4d b596 fa51 14d8 6a3f 1ff1  ....jM...Q..j?..
-000033f0: 26ea 5f3d 46c7 1d5b 9836 1727 fd25 a5f5  &._=F..[.6.'.%..
-00003400: 5671 7c77 3f8e 7fed a7eb 281d 1c8f 27b3  Vq|w?.....(...'.
-00003410: 64f6 299c 4ce3 abc9 fda7 f0f4 3a7e b89f  d.).L.......:~..
-00003420: 7c0a f763 bbc4 db5c 6ff8 dc6d b617 dd18  |..c...\o..m....
-00003430: d6a2 6b8c 80d7 c60f 8467 9a92 60ed 1660  ..k......g..`..`
-00003440: d4d2 32fd 764f 8527 6580 7b01 3ec0 6999  ..2.vO.'e.{.>.i.
-00003450: 79c6 70d8 430d 278c ad70 083d 1af7 c082  y.p.C.'..p.=....
-00003460: 1ab5 844d a760 6ba2 b75d ac3e 577f 0ee1  ...M.`k..].>W...
-00003470: 1e78 6afd bbed 02fa 772d 4bd5 a31c 3451  .xj.....w-K...4Q
-00003480: 753b 785e 3299 f47d 5061 9f29 f7a0 29b3  u;x^2..}Pa.)..).
-00003490: f4c4 5ee0 daeb e1a5 28be eeb5 2f72 bfb0  ..^.....(.../r..
-000034a0: 781f 16db ab1a b867 52f5 6665 0162 f82d  x......gR.fe.b.-
-000034b0: 758d 05c4 d83b 43c9 22fc 9b0c 9f5e ba55  u....;C."....^.U
-000034c0: c574 ea1a 13d6 44a9 baa9 b36d b208 19dd  .t....D....m....
-000034d0: ee6c e22c 2d4a 05be ba95 906d 470d 36aa  .l.,-J.....mG.6.
-000034e0: b051 8d55 02c9 5d11 90dd 7c74 ba91 d7f5  .Q.U..]...|t....
-000034f0: 7863 af1b 77ba 89d7 4d3a ddd4 eba6 9d6e  xc..w...M:.....n
-00003500: e675 33a7 dbe1 986b 5cdd 6f38 6afe d3e9  .u3....k\.o8j...
-00003510: 3792 3179 80e2 8f0e ffa0 ea96 ba9b e1bb  7.1y............
-00003520: d24a bf97 9b1d 6cda f5bc 230a 96f5 eaf7  .J....l...#.....
-00003530: 4328 6b6d f320 9860 3f87 777c 63a0 708f  C(km. .`?.w|c.p.
-00003540: 8e51 b4e0 e41d af3c 1e5d b577 da98 b06a  .Q.....<.].w...j
-00003550: 7d9f 18d4 848a e20c d5a9 b782 58d2 df45  }...........X..E
-00003560: d189 233f 751f 92ac 9eab 9ce2 34a4 479e  ..#?u.......4.G.
-00003570: 754f d065 7b70 460d 2e34 850f 9695 dac3  uO.e{pF..4......
-00003580: bf78 3899 6065 f247 1c74 fcaa a0c9 7836  .x8.`e.G.t....x6
-00003590: 5dad ae97 7d46 1df0 9193 2d2c 15ed b8e3  ]...}F....-,....
-000035a0: b8ea f52a b3e6 cfde edc5 3f50 4b03 0414  ...*......?PK...
-000035b0: 0000 0008 00b7 8964 4900 e7c1 3558 0600  .......dI...5X..
-000035c0: 005a 4100 000f 0000 0077 6f72 642f 7374  .ZA......word/st
-000035d0: 796c 6573 2e78 6d6c e59b 4b73 e328 10c7  yles.xml..Ks.(..
-000035e0: eff3 2954 baf8 94f8 95d8 712a 9ea9 bc66  ..)T......q*...f
-000035f0: 93aa cc4c 669c ec9e 31c2 1615 09b4 80f3  ...Lf...1.......
-00003600: 984f 3fe8 65cb 916d b5ac de5c f666 21ba  .O?.e..m...\.f!.
-00003610: 7f0d 34fc 910b cebe bc86 81f3 cc94 e652  ..4............R
-00003620: 8c5b ddc3 4ecb 6182 4a8f 8bf9 b8f5 f8f0  .[..N.a.J.......
-00003630: f5e0 a4e5 6843 8447 0229 d8b8 f5c6 74eb  ....hC.G.)....t.
-00003640: cbe7 4f67 2fa7 dabc 054c 3bd6 5ee8 d390  ..Og/....L;.^...
-00003650: 8e5d df98 e8b4 ddd6 d467 21d1 8732 62c2  .].......g!..2b.
-00003660: be9c 4915 1263 1fd5 bc1d 12f5 b488 0ea8  ..I..c..........
-00003670: 0c23 62f8 9407 dcbc b57b 9dce c0cd dc28  .#b......{.....(
-00003680: 8817 399b 71ca ae24 5d84 4c98 c4be ad58  ..9.q..$].L....X
-00003690: 603d 4aa1 7d1e e9dc db0b c4db 8b54 5ea4  `=J.}........T^.
-000036a0: 2465 5adb 3687 41ea 2f24 5c2c dd74 8f4a  $eZ.6.A./$\,.t.J
-000036b0: 8e42 4e95 d472 660e 6d63 b288 1257 d6bc  .BN..rf.mc...W..
-000036c0: db49 7e85 81eb 84f4 f476 2ea4 22d3 808d  .I~......v.."...
-000036d0: 5deb c8fd fcc9 716c e779 925e b119 5904  ].....ql.y.^..Y.
-000036e0: 46c7 2549 99ba 5759 595a 9417 e64f e9f3  F.%I..WYYZ...O..
-000036f0: 5729 8c76 5e4e 89a6 9c3f d868 ace3 905b  W).v^N...?.h...[
-00003700: c6cd b9d0 dcb5 6f18 d1e6 5c73 527c 799d  ......o...\sR|y.
-00003710: 95c5 effd b8e2 464b aa4d a1f8 827b dc6d  ......FK.M...{.m
-00003720: afd1 f56f 5beb 9904 63b7 7754 7a75 a9b7  ...o[...c.wTzu..
-00003730: be0c 8898 e72f 9938 789c 14e3 2c14 4d2d  ...../.8x...,.M-
-00003740: 72ec 1275 3039 5f79 386b 17ba 217b 58eb  r..u09_y8k..!{X.
-00003750: 280b 8896 4589 595c eb5d 1727 5118 9b30  (...E.Y\.].'Q..0
-00003760: 9334 6f6d 0536 bb93 f489 7913 635f 8cdd  .4om.6....y.c_..
-00003770: 8e9b 163e dede 2b2e 95cd cdb1 3b1a 6585  ...>..+.....;.e.
-00003780: 1316 f21b ee79 4c8c dd6e 5e51 f8dc 63ff  .....yL..n^Q..c.
-00003790: f84c 3c6a e6ad ca7f 7e4d f22b f348 e542  .L<j....~M.+.H.B
-000037a0: d8df bde1 c05d 861b 68ef fa95 b228 4e59  .....]..h....(NY
-000037b0: 5b45 90b8 d3bf c756 416c a20b b0c4 c782  [E.....VAl......
-000037c0: af42 4a0b dea1 93c2 7f73 6e37 efbc 6d28  .BJ......sn7..m(
-000037d0: 9f91 7886 3bdd 4ada 0891 d6db e8bc be9f  ..x.;.J.........
-000037e0: 3e92 9f23 243f c748 7e06 487e 8648 7e4e  >..#$?.H~.H~.H~N
-000037f0: 90fc 8c1a fa31 92a6 995a f4d1 1f41 cc4a  .....1...Z...A.J
-00003800: 2907 332b 6518 ccac 9450 30b3 52fe c0cc  ).3+e....P0.R...
-00003810: 4ae9 0233 2b65 07cc ac94 0c30 b3d2 d857  J..3+e.....0...W
-00003820: 9b51 923c 970c 8feb 65cd 0337 01ab 5cdf  .Q.<....e..7..\.
-00003830: ba18 cb69 a633 ce3d 5164 ae48 e43b b14a  ...i.3.=Qd.H.;.J
-00003840: 9750 556e 268b a981 05dd 4508 7a62 9414  .PUn&.....E.zb..
-00003850: f34a 56af 87c0 ba0e 239f 68ae ab69 18c3  .JV.....#.h..i..
-00003860: f110 6fb7 9cbf 14f7 2a79 c75b f4ad 8270  ..o.....*y.[...p
-00003870: 1f10 ca7c 1978 4c39 0fec d5ec e5e4 bb74  ...|.xL9.......t
-00003880: 2611 a11c 3008 18e3 7dc7 e7be 7126 7eb2  &...0...}...q&~.
-00003890: 2657 1207 5b06 0204 b9e3 da54 13b6 340a  &W..[......T..4.
-000038a0: 4400 0dee 604b ea56 10be 318f 2fc2 bca7  D...`K.V..1./...
-000038b0: 007b a441 1f83 d3ab e61c 35e1 c483 0269  .{.A......5....i
-000038c0: cc71 6308 a025 8326 9078 f021 2d19 3686  .qc..%.&.x.!-.6.
-000038d0: 005a 72d2 18d2 af86 ecb7 4a5d d9cf 6dd8  .Zr.......J]..m.
-000038e0: 5c1c ee37 db2f 6520 d56c 1180 5795 e17e  \..7./e .l..W..~
-000038f0: 737e c981 3566 bf69 bf84 80d6 96e1 7e73  s~..5f.i......~s
-00003900: 7e6d 1176 ce29 b51f a490 546e ba1a d740  ~m.v.)....Tn...@
-00003910: 355d 966b a070 d6e7 1a40 9c85 ba06 1061  5].k.p...@.....a
-00003920: c5ae 41db 6fe9 fec5 9eb9 ce37 dcf5 c75d  ..A.o......7...]
-00003930: 17f6 bd95 21f6 b774 48ad 9dcc cf85 34d5  ....!..tH.....4.
-00003940: 9be4 1ec6 5f17 b7c2 30a1 9903 43f6 3176  ...._...0...C.1v
-00003950: af6b 4a5a 63f0 1124 b506 0d41 5b6b d010  .kJZc..$...A[k..
-00003960: 44b6 06ad a1da c249 48b2 5b03 88a0 bf35  D......IH.[....5
-00003970: 6808 425c 8386 a8c8 807d 1f96 2203 5058  h.B\.....}..".PX
-00003980: 8a0c 40e1 2a32 0088 abc8 1ff3 0d55 8386  ..@.*2.......U..
-00003990: f031 5583 8628 0100 1aa2 047c cc77 560d  .1U..(.....|.wV.
-000039a0: 1a92 0454 9390 2500 0044 9400 000d 5102  ...T..%..D....Q.
-000039b0: 0034 4409 007c 9563 4900 0085 2501 0014  .4D..|.cI...%...
-000039c0: ae04 0080 b812 0000 224a 0080 8628 0100  ........"J...(..
-000039d0: 1aa2 0400 6888 1200 a021 4ac0 7fff 9f1b  ....h....!J.....
-000039e0: 9c84 2c01 0020 a204 0068 8812 00a0 214a  ..,.. ...h....!J
-000039f0: c0d1 c749 0000 8525 0100 14ae 0400 80b8  ...I...%........
-00003a00: 1200 0022 4a00 8086 2801 001a a204 0068  ..."J...(......h
-00003a10: 8812 00a0 214a 0080 8624 01d5 2464 0900  ....!J...$..$d..
-00003a20: 0011 2500 4043 9400 000d 5102 8e3f 4e02  ..%.@C....Q..?N.
-00003a30: 0028 2c09 00a0 7025 0000 c495 0000 1051  .(,...p%.......Q
-00003a40: 0200 3444 0900 d010 2500 4043 9400 000d  ..4D....%.@C....
-00003a50: 5102 0034 2409 a826 214b 0000 8828 0100  Q..4$..&!K...(..
-00003a60: 1aa2 0400 6888 1230 f838 0900 a0b0 2400  ....h..0.8....$.
-00003a70: 80c2 9500 0010 5702 0040 4409 00d0 1025  ......W..@D....%
-00003a80: 0040 4394 0000 0d51 0200 3444 0900 d090  .@C....Q..4D....
-00003a90: 24a0 9a84 2c01 0020 a204 0068 8812 00a0  $...,.. ...h....
-00003aa0: edb7 9ac4 67b0 03e6 800f 2c77 314f 99c0  ....g.....,w1O..
-00003ab0: 8f49 a31c 004f 9bfa 8bcd 9862 8202 8eb7  .I...O.....b....
-00003ac0: 6050 f3b6 d6c0 629c 40bf 90f2 c981 5d09  `P....b.@.....].
-00003ad0: e86f c99c 7a3c 3e0d b84c 0e45 bd95 00c3  .o..z<>..L.E....
-00003ae0: ca13 ec3f 2e9d 1bb6 3c53 f9ee fec4 8640  ...?....<S.....@
-00003af0: e20b 6fc5 eb6d 4959 7647 d356 376f 91f5  ..o..mIYvG.V7o..
-00003b00: 1a15 8f69 79e9 9d85 ec6c 7952 f1d6 5b5e  ...iy....lyR..[^
-00003b10: 425b 8617 c7e3 6437 f7b2 77ab d8b3 2896  B[....d7..w...(.
-00003b20: 1124 5e36 a2a9 6fd9 d430 b503 9ddd a258  .$^6..o..0.....X
-00003b30: 1e26 4bee 506c 0c64 cb7d 8b55 60ab 0ecb  .&K.Pl.d.}.U`...
-00003b40: 4d8a 03b6 1afd 82c5 da70 035a 64e2 4b06  M........p.Zd.K.
-00003b50: 3b5a 935c 42a8 ee4d 27a9 b733 f4d1 a87e  ;Z.\B..M'..3...~
-00003b60: ec49 b999 06ab dba3 e9f3 adf0 acdb 972c  .I.............,
-00003b70: 9dd3 9678 af24 07e4 d52e 5910 7c23 eb37  ...x.$....Y.|#.7
-00003b80: 4f8d 8c76 9ba6 e9cc 6626 add6 ed9c ecaa  O..v....f&......
-00003b90: 3895 c6c8 10e0 5125 7bd7 0a97 f158 bd8f  8.....Q%{....X..
-00003ba0: 3b2b 4bbb 60f7 608a 4538 652a 9b6d 5b67  ;+K.`.`.E8e*.m[g
-00003bb0: 4672 fa78 cb58 a647 93b1 8711 9882 eb49  Fr.x.X.G.......I
-00003bc0: 979c 5fde 1866 e162 cc0a 3b25 96f6 43ac  .._..f.b..;%..C.
-00003bd0: d529 cdf4 7273 8e8b cd51 9a7b f98b 4ee7  .)..rs...Q.{..N.
-00003be0: fca2 df19 1527 dcfe 8978 2195 c794 de90  .....'...x!.....
-00003bf0: 8809 2bbe b29d 75c1 efb1 9bfe 3518 11ca  ..+...u.....5...
-00003c00: 32b7 34de 3a8c 5db2 3072 739a 3673 b24c  2.4.:.].0rs.6s.L
-00003c10: e166 6ef2 046f e685 0b3b 06ec 06c9 cfdf  .fn..o...;......
-00003c20: 4dfc 6413 efdd d8fd 0f56 96e5 4fdb e83f  M.d......V..O..?
-00003c30: 504b 0304 1400 0000 0800 b789 6449 44cd  PK..........dID.
-00003c40: e5e6 db06 0000 bc44 0000 1a00 0000 776f  .......D......wo
-00003c50: 7264 2f73 7479 6c65 7357 6974 6845 6666  rd/stylesWithEff
-00003c60: 6563 7473 2e78 6d6c e59b 4b73 e238 10c7  ects.xml..Ks.8..
-00003c70: eff3 295c bee4 94e1 9590 400d 3395 c7cc  ..)\......@.3...
-00003c80: 2455 f3c8 0cc9 ee59 c802 ab62 4b5e 4984  $U.....Y...bK^I.
-00003c90: 643e fdca 4f4c 0cb8 8d7b 73d9 1358 56f7  d>..OL...{s..XV.
-00003ca0: af25 b5f4 1794 f4e1 d373 1838 4f4c 692e  .%.......s.8OLi.
-00003cb0: c5e4 a8f7 be7b e430 41a5 c7c5 6272 f470  .....{.0A...br.p
-00003cc0: ffe5 f8fc c8d1 8608 8f04 52b0 c9d1 0bd3  ..........R.....
-00003cd0: 479f 3ebe fbb0 1a6b f312 30ed 587b a1c7  G.>....k..0.X{..
-00003ce0: ab88 4e5c df98 68dc e968 eab3 90e8 f721  ..N\..h..h.....!
-00003cf0: a74a 6a39 37ef a90c 3b72 3ee7 9475 5652  .Jj97...;r>..uVR
-00003d00: 799d 7eb7 d74d be45 4a52 a6b5 855d 11f1  y.~..M.EJR...]..
-00003d10: 44b4 9bb9 0b25 cc5b 4868 feb5 dfed 9edb  D....%.[Hh......
-00003d20: 672e 0a1f d588 64c4 847d 3997 2a24 c63e  g.....d..}9.*$.>
-00003d30: aa85 b550 8fcb e8d8 fa8c 88e1 331e 70f3  ...P........3.p.
-00003d40: 12fb 1a16 6e9e 26ee 5289 71e6 e3b8 8823  ....n.&.R.q....#
-00003d50: b619 db00 c64f 6190 5796 fbea a681 661f  .....Oa.W.....f.
-00003d60: b985 8204 999a 5c4b ba0c 9930 4978 1dc5  ......\K...0Ix..
-00003d70: 021b b014 dae7 d1ba df0e f566 5ffa b993  ...........f_...
-00003d80: bd0d 2e35 7615 f54e da0d fab5 222b fbb1  ...5v..N...."+..
-00003d90: 7608 09df 4b8d c220 8d7c bfc7 5e17 3022  v...K.. .|..^.0"
-00003da0: b18b c202 12c2 2633 8fa4 9c7c abc3 baa6  ......&3...|....
-00003db0: dcb9 8b76 7dfb 55c9 65b4 f6c6 db79 bb15  ...v}.U.e....y..
-00003dc0: 8f85 2fbb 0c34 f195 8d51 b969 ba5d 3053  ../..4...Q.i.]0S
-00003dd0: 9f44 7602 8574 7cbb 1052 9159 6023 b23d  .Dv..t|..R.Y`#.=
-00003de0: eec4 19e9 7e7c e738 7679 f224 bd66 73b2  ....~|.8vy.$.fs.
-00003df0: 0c8c 8e4b 9232 75a7 b2b2 b428 2fcc 9fd2  ...K.2u....(/...
-00003e00: e72f 5218 edac c644 53ce ef6d 7cd6 7bc8  ./R....DS..m|.{.
-00003e10: 2de8 e642 68ee da37 8c68 73a1 3929 bffc  -..Bh..7.hs.9)..
-00003e20: 9c95 c5ef fdb8 e256 4baa 4da9 f892 7bdc  .......VK.M...{.
-00003e30: ed6c d0f5 1f5b eb89 0413 b77f 5279 75a5  .l...[......Ryu.
-00003e40: 77be 0c88 58e4 2f99 387e 9896 e32c 15cd  w...X./.8~...,..
-00003e50: 2c72 e212 753c bd58 7bf8 d029 7543 f6b0  ,r..u<.X{..)uC..
-00003e60: d151 1610 1545 8959 5ceb 5517 2751 18bb  .Q...E.Y\.U.'Q..
-00003e70: a44c 5365 b015 d8fc 9ba4 8fcc 9b1a fb62  .LSe...........b
-00003e80: e276 ddb4 f0e1 f64e 71a9 ec52 3b71 47a3  .v.....Nq..R;qG.
-00003e90: ac70 ca42 7ec3 3d8f 8989 dbcb 2b0a 9f7b  .p.B~.=.....+..{
-00003ea0: ec6f 9f89 07cd bc75 f9af 2fc9 6ccc 3c52  .o.....u../.l.<R
-00003eb0: b914 f67b ff6c e816 e106 dafb fc4c 5914  ...{.l.......LY.
-00003ec0: 2f91 b68a 2071 a7ff 88ad 82d8 4497 6089  /... q......D.`.
-00003ed0: 8f25 5f87 9416 bc42 2785 ffe4 dc5e de79  .%_....B'....^.y
-00003ee0: bb50 3e23 b186 3abd 5ada 0891 d6df eabc  .P>#..:.Z.......
-00003ef0: b99f 0192 9f13 243f a748 7e86 487e ce90  ......$?.H~.H~..
-00003f00: fc9c 23f9 19b5 f463 244d 33b5 ec63 3082  ..#....c$M3..c0.
-00003f10: 9855 520e 6656 c930 9859 25a1 6066 95fc  .UR.fV.0.Y%.`f..
-00003f20: 8199 55d2 0566 56c9 0e98 5925 1960 6695  ..U..fV...Y%.`f.
-00003f30: b1af 37a3 2479 ae18 9e36 cb9a 7b6e 0256  ..7.$y...6..{n.V
-00003f40: bbbe f530 96d3 4c67 9c3b a2c8 4291 c877  ...0..Lg.;..B..w
-00003f50: 6295 aea0 eadc 4c97 3303 0bba 8710 f4d4  b.....L.3.......
-00003f60: 2819 ef45 6b58 fd3e 02eb 7318 f944 735d  (..EkX.>..s..Ds]
-00003f70: 4fc3 188e fb78 cfe5 7c55 dcab e59d eed0  O....x..|U......
-00003f80: b71a c25d 4028 f365 e031 e5dc b367 7390  ...]@(.e.1...gs.
-00003f90: 931f d299 4684 72c0 2060 8cf7 37be f08d  ....F.r. `..7...
-00003fa0: 6377 a71e 8438 dc31 1020 c837 ae4d 3d61  cw...8.1. .7.M=a
-00003fb0: 47a3 4004 d0e0 0e77 a46e 0de1 3bf3 f832  G.@....w.n..;..2
-00003fc0: cc7b 0ab0 471a 0e30 38fd 7ace 491b 4e3c  .{..G..08.z.I.N<
-00003fd0: 2890 c69c b686 005a 326c 0389 071f d292  (......Z2l......
-00003fe0: b3d6 1040 4bce 5b43 06f5 90c3 56a9 6ba2  ...@K.[C....V.k.
-00003ff0: 1e61 73f1 ecb0 d97e 2503 a9e6 cb00 bcaa  .as....~%.......
-00004000: 9c1d 36e7 0b0e ac31 874d fb02 025a 5bce  ..6....1.M...Z[.
-00004010: 0e9b f31b 8bb0 7341 a9fd 410a 49e5 b6ab  ......sA..A.I...
-00004020: 7103 54db 65b9 010a 677d 6e00 c459 a81b  q.T.e...g}n..Y..
-00004030: 0011 56ec 06b4 c396 eedf ec89 eb7c c3dd  ..V..........|..
-00004040: 7cdc 7569 df5b 1be2 6047 8734 dac9 fc5a  |.ui.[..`G.4...Z
-00004050: 4a53 bf49 ee63 fc75 712b 0c13 9a39 30e4  JS.I.c.uq+...90.
-00004060: 0063 f7ba a1a4 0d06 1f41 521b d010 b4b5  .c.......AR.....
-00004070: 010d 4164 1bd0 5aaa 2d9c 8424 bb0d 8008  ..Ad..Z.-..$....
-00004080: fadb 8086 20c4 0d68 888a 0cd8 f761 2932  .... ..h.....a)2
-00004090: 0085 a5c8 0014 ae22 0380 b88a fc36 bfa1  .......".....6..
-000040a0: 1ad0 107e 4c35 a021 4a00 8086 2801 6ff3  ...~L5.!J...(.o.
-000040b0: 3bab 010d 4902 ea49 c812 0000 224a 0080  ;...I..I...."J..
-000040c0: 8628 0100 1aa2 0400 7e95 6349 0000 8525  .(......~.cI...%
-000040d0: 0100 14ae 0400 80b8 1200 0022 4a00 8086  ..........."J...
-000040e0: 2801 001a a204 0068 8812 00a0 214a c07f  (......h....!J..
-000040f0: ff9f 1b9c 842c 0100 20a2 0400 6888 1200  .....,.. ...h...
-00004100: a021 4ac0 c9db 4900 0085 2501 0014 ae04  .!J...I...%.....
-00004110: 0080 b812 0000 224a 0080 8628 0100 1aa2  ......"J...(....
-00004120: 0400 6888 1200 a021 4a00 8086 2401 f524  ..h....!J...$..$
-00004130: 6409 0000 1125 0040 4394 0000 0d51 024e  d....%.@C....Q.N
-00004140: df4e 0200 282c 0900 a070 2500 00c4 9500  .N..(,...p%.....
-00004150: 0010 5102 0034 4409 00d0 1025 0040 4394  ..Q..4D....%.@C.
-00004160: 0000 0d51 0200 3424 09a8 2721 4b00 0088  ...Q..4$..'!K...
-00004170: 2801 001a a204 0068 8812 307c 3b09 00a0  (......h..0|;...
-00004180: b024 0080 c295 0000 1057 0200 4044 0900  .$.......W..@D..
-00004190: d010 2500 4043 9400 000d 5102 0034 4409  ..%.@C....Q..4D.
-000041a0: 00d0 9024 a09e 842c 0100 20a2 0400 6888  ...$...,.. ...h.
-000041b0: 1200 a01d b69a c467 b003 e680 0f2c f730  .......g.....,.0
-000041c0: 4f99 c08f 49a3 1c00 4f9b fa9b cd99 6282  O...I...O.....b.
-000041d0: 028e b760 50f3 b636 c062 9c40 bf94 f2d1  ...`P..6.b.@....
-000041e0: 815d 0918 ecc8 9c66 3c3e 0bb8 4c0e 45bd  .].....f<>..L.E.
-000041f0: 5400 67b5 27d8 7f5e 3937 ac38 53f9 eafe  T.g.'..^97.8S...
-00004200: c496 40e2 0b6f e5eb 6d49 5976 0bda 5637  ..@..o..mIYv..V7
-00004210: 2f91 f51a 958f 6979 e99d 85ec 6c79 52f1  /.....iy....lyR.
-00004220: d62b 2ea1 15e1 c5f1 38d9 cdbd ecdd 3af6  .+......8.....:.
-00004230: 2c8a 2282 c4cb 5634 f52d 9b1a a6f6 a0b3  ,."...V4.-......
-00004240: 5b14 c561 b2e4 0ec5 d640 76dc b758 07b6  [..a.....@v..X..
-00004250: eeb0 dca4 3c60 ebd1 2f59 6c0c 37a0 4526  ....<`../Yl.7.E&
-00004260: be64 b0a7 35c9 2584 fade 7492 7a7b 431f  .d..5.%...t.z{C.
-00004270: 8d9a c79e 949b 59b0 be3d 9a3e df0a cfba  ......Y..=.>....
-00004280: 5d65 e99c b6c4 7b26 3920 af76 c582 e03b  ]e....{&9 .v...;
-00004290: d9bc 796a 64b4 df34 4d67 3637 69b5 5ef7  ..yjd..4Mg67i.^.
-000042a0: 7c5f c599 3446 8600 8f2a d9bb d6b8 8cc7  |_..4F...*......
-000042b0: ea75 dc59 59da 05fb 0753 2cc3 1953 d96c  .u.YY....S,..S.l
-000042c0: db39 3392 d3c7 3bc6 323d 9a8c 3d8c c014  .93...;.2=..=...
-000042d0: dc4c bae4 fcf2 d630 4b17 63d6 d819 b1b4  .L.....0K.c.....
-000042e0: 9f62 a34e 65a6 579b 735a 6e8e d2dc cb5f  .b.Ne.W.sZn...._
-000042f0: 74bb 1797 83ee a83c e10e 4fc4 4ba9 3ca6  t......<..O.K.<.
-00004300: f496 444c 58f1 7deb ac0b fe4c dcf4 afc1  ..DLX.}....L....
-00004310: 8850 96b9 a5f1 d661 e292 a591 dbd3 b49d  .P.....a........
-00004320: 9322 85db b9c9 13bc 9d17 2eec 18b0 1b24  .".............$
-00004330: 3f7f b5f1 934d bc57 63f7 3f58 598a afb6  ?....M.Wc.?XY...
-00004340: d1ff 0250 4b03 0414 0000 0008 00b7 8964  ...PK..........d
-00004350: 4994 4122 b8c6 0600 00bb 2a00 0015 0000  I.A"......*.....
-00004360: 0077 6f72 642f 7468 656d 652f 7468 656d  .word/theme/them
-00004370: 6531 2e78 6d6c ed5a 4d6f db36 18be f757  e1.xml.ZMo.6...W
-00004380: 10ba e4d4 fadb 758a ba45 ecd8 edd6 a60d  ......u..E......
-00004390: 12b7 438f b444 5b6c 2851 20e9 24be 0ded  ..C..D[l(Q .$...
-000043a0: 71c0 8061 ddb0 c30a ecb6 c3b0 ad40 0bec  q..a.........@..
-000043b0: d2fd 9a6e 1db6 0ee8 5f18 29d9 8a28 5172  ...n...._.)..(Qr
-000043c0: e6c5 4dda 2507 c722 f93c 7cbf 5f52 f0d5  ..M.%..".<|._R..
-000043d0: eb87 1e01 fb88 714c fdf6 5ae5 5279 0d20  ......qL..Z.Ry. 
-000043e0: dfa6 0ef6 c7ed b57b 83fe c5d6 1ae0 02fa  .......{........
-000043f0: 0e24 d447 edb5 29e2 6bd7 af5d b80a af08  .$.G..).k..]....
-00004400: 1779 0848 b8cf afc0 b6e5 0a11 5c29 95b8  .y.H........\)..
-00004410: 2d87 21bf 4403 e4cb b911 651e 14f2 918d  -.!.D.....e.....
-00004420: 4b0e 8307 92d6 23a5 6ab9 dc2c 7910 fb16  K.....#.j..,y...
-00004430: f0a1 87da d6dd d108 db08 0c14 a575 ed02  .............u..
-00004440: 0073 fe1e 911f bee0 6a2c 1cb5 09db b5c3  .s......j,......
-00004450: 9d93 482b 9a0f 5738 7b95 f953 f8cc a7bc  ..H+..W8{..S....
-00004460: 4b18 d887 a46d c9fd 1d7a 3040 87c2 0204  K....m...z0@....
-00004470: 7221 27da 5639 fcb3 4a31 4749 2391 1444  r!'.V9..J1GI#..D
-00004480: 2ca2 4cd0 f5c3 3f9d 2e41 104a 58d5 e9d8  ,.L...?..A.JX...
-00004490: 7818 f355 faf5 f5cb 9b69 69aa 9a34 05f0  x..U.....ii..4..
-000044a0: 5eaf d7ed 55d2 bb27 e1d0 b6a5 452b f914  ^...U..'....E+..
-000044b0: f57e abd2 4949 9002 c534 0592 74cb 8d72  .~..II...4..t..r
-000044c0: dd48 9395 a696 4fb3 dee9 741a eb26 9a5a  .H....O...t..&.Z
-000044d0: 86a6 9e4f d32a 37eb 1b55 134d 3d43 d328  ...O.*7..U.M=C.(
-000044e0: b04d 67a3 db6d 9a68 1a19 9a66 3e4d fff2  .Mg..m.h...f>M..
-000044f0: 7ab3 6ea4 6926 685c 82fd bd7c 1215 b5e9  z.n.i&h\...|....
-00004500: 40d3 2012 30a2 e466 314b 4bb2 b452 d1af  @. .0..f1KK..R..
-00004510: a3d4 489c 7671 228e a82f 1664 a207 1f52  ..H.vq"../.d...R
-00004520: d697 ebb4 dd09 14d8 0762 1aa0 11b4 25ae  .........b....%.
-00004530: 0b09 1e32 7c24 41b8 0ac1 c492 d49c cdf3  ...2|$A.........
-00004540: e794 5880 db0c 07a2 6d7d 1c40 5962 8ed6  ..X.....m}.@Yb..
-00004550: be7d f9e3 db97 cfc1 ab47 2f5e 3dfa e5d5  .}.......G/^=...
-00004560: e3c7 af1e fd5c 04bf 09fd 7112 fee6 fb2f  .....\....q..../
-00004570: fe7e fa29 f8eb f977 6f9e 7cb5 00c8 93c0  .~.)...wo.|.....
-00004580: df7f faec b75f bf5c 8010 49c4 ebaf 9ffd  ....._.\..I.....
-00004590: f1e2 d9eb 6f3e fff3 8727 45b8 0d06 8749  ....o>...'E....I
-000045a0: dc00 7b88 833b e800 ec50 4f2a 5fb4 251a  ..{..;...PO*_.%.
-000045b0: b225 a103 17e2 2474 c31f 73e8 4305 2e82  .%....$t..s.C...
-000045c0: f584 abc1 ee4c 2181 4580 0ed2 1d70 9fc9  .....L!.E....p..
-000045d0: 625b 88b8 3179 a829 b5eb b289 48c7 9686  b[..1y.)....H...
-000045e0: b8e5 7a1a 628b 52d2 a1ac d800 b794 1849  ..z.b.R........I
-000045f0: db4d fcf1 02b9 d824 09d8 8170 bf50 ac6e  .M.....$...p.P.n
-00004600: 2a84 7a93 40e6 1a2e dca4 eb22 4d95 6d22  *.z.@......"M.m"
-00004610: a30a 8e91 8f04 5073 740f a122 fc03 8c35  ......Pst.."...5
-00004620: ff6c 619b 514e 4702 3cc0 a003 71b1 2107  .la.QNG.<...q.!.
-00004630: 7828 cce8 9bd8 938e 9e16 ca2e 434a b3e8  x(..........CJ..
-00004640: d67d d0a1 a470 c34d b4af 4364 ba42 52b8  .}...p.M..Cd.BR.
-00004650: 0922 9a17 6ec0 8980 5eb1 56d0 2349 c86d  ."..n...^.V.#I.m
-00004660: 28dc 4245 76a7 ccd6 1cc7 850c a631 2214  (.BEv........1".
-00004670: f41c c479 21f8 2e9b 6a2a dd92 b571 4164  ...y!...j*...qAd
-00004680: 6d91 a9a7 4398 c07b 8590 db90 d224 6493  m...C..{.....$d.
-00004690: ee75 5de8 05c5 7a61 df4d 823e e27b 3253  .u]...za.M.>.{2S
-000046a0: 20d8 a6a2 583e aae7 b07a 968e 85fe e288   ...X>...z......
-000046b0: ba8f 9158 b242 ddc3 63d7 1c8c 6a66 c20a  ...X.B..c...jf..
-000046c0: 7315 51bd 864c c908 a2c4 76aa 2166 7a9b  s.Q..L....v.!fz.
-000046d0: ea77 d83f 56bf f364 bb4b db6c 95fd 4eb6  .w.?V..d.K.l..N.
-000046e0: 91d7 df3e fdc0 3add 86b4 6161 b2a7 fbdb  ...>..:...aa....
-000046f0: 4240 baab 7529 73f0 87d1 d436 e1c4 df46  B@..u)s....6...F
-00004700: 3281 cf7b da79 4f3b ef69 67a8 a72d ac4a  2..{.yO;.ig..-.J
-00004710: abef 647a d78a ee7f f3bb ddd1 75cf 5b74  ..dz........u.[t
-00004720: db1b 6142 76c5 94a0 db5c 6f80 5c9a c6e9  ..aBv....\o.\...
-00004730: cbd9 a3d1 683c e48b 2fa2 812b bf6a da94  ....h<../..+.j..
-00004740: 8c58 891c 3318 0e02 46c5 2758 b8bb 2e0c  .X..3...F.'X....
-00004750: a44c 152b b5c3 986b b2c4 a320 a05c de9f  .L.+...k... .\..
-00004760: 2d7d 2a5f a8f4 bae8 fd14 9696 0e17 35f4  -}*_..........5.
-00004770: f747 3a1f 145b d489 d6d5 cae6 85a1 a2f3  .G:..[..........
-00004780: 7d53 e296 94bc b92a d4d4 d627 a546 edf2  }S.....*...'.F..
-00004790: 69a9 5189 184f 488f 4ae3 987a e4f8 ed5f  i.Q..OH.J..z..._
-000047a0: e911 8da4 c24c 9dfa e499 4f96 4829 4db3  .....L....O.H)M.
-000047b0: 1a69 27b3 1212 e4a8 304d 05f9 3c9c cf72  .i'.....0M..<..r
-000047c0: 8c57 729c 1e11 bad0 41c7 5997 b07e a576  .Wr.....A.Y..~.v
-000047d0: b6a3 a830 a997 d0f7 b4a2 adbc 28da c282  ...0........(...
-000047e0: 6fa8 dd8a d637 1674 e283 83b6 b5de a836  o....7.t.......6
-000047f0: 2c60 c3a0 6d8d e41d 477e f502 b91f 57ad  ,`..m...G~....W.
-00004800: 1192 b1df b66c c1d2 d16a ec05 c7f7 916e  .....l...j.....n
-00004810: fb75 73a2 a703 ad6c 5a96 6bf6 9cae 13d2  .us....lZ.k.....
-00004820: 068c 8b4d c8dd 8838 5c95 b62e f10d a6aa  ...M...8\.......
-00004830: 36ea ca25 abb5 5569 d55a d45a 95f7 558b  6..%..Ui.Z.Z..U.
-00004840: e8c9 10e1 6834 42b6 3046 7962 2ab5 7534  ....h4B.0Fyb*.u4
-00004850: 632a bb74 2210 db75 9d03 3024 13b6 03a5  c*.t"..u..0$....
-00004860: 75ea 513a 3a98 cb03 5975 fec0 6481 a9cf  u.Q::...Yu..d...
-00004870: 3255 2ff0 e602 967e ef6f a873 e142 4802  2U/....~.o.s.BH.
-00004880: 17ce 0a4e 2bbf de44 74d9 8c88 e54f 7bc1  ...N+..Dt....O{.
-00004890: a0f2 d170 ca46 abb2 5ded 1dda 2ea7 b29c  ...p.F..].......
-000048a0: dbee f46d 37ab 1dc8 4735 2763 085b 5e4e  ...m7...G5'c.[^N
-000048b0: 1804 aa38 b42d ca84 4b65 bb0b 5c6c f799  ...8.-..Ke..\l..
-000048c0: bcd3 9854 9456 00b2 9829 0300 42fd f03f  ...T.V...)..B..?
-000048d0: 43fb a9c6 3997 27e2 cf6c 4be4 554c ece0  C...9.'..lK.UL..
-000048e0: 3160 5836 61e1 3284 b6c5 ccde ff6e d74a  1`X6a.2......n.J
-000048f0: d578 a008 0bd8 6c93 4c85 ccda 4259 2830  .x....l.L...BY(0
-00004900: 9867 88f6 1119 a862 de54 6eb2 803b 6f4e  .g.....b.Tn..;oN
-00004910: d9ba abe1 7302 3635 acd7 d6e1 b8ff bfbd  ....s.65........
-00004920: 12d6 dfe5 a950 53a1 7e92 87e0 7ad1 552a  .....PS.~...z.U*
-00004930: 7110 5b3f 2d6d 4fe2 cc9f 50a4 7a4c b755  q.[?-mO...P.zL.U
-00004940: 1b05 45ee bf1e e603 285c a03e e479 0a33  ..E.....(\.>.y.3
-00004950: 9b20 2ba3 be3a af0f e88e cc3b 105f 5580  . +..:.....;._U.
-00004960: ac26 175b b3d2 1e0f 0ea5 8d5a 59ad d4de  .&.[.......ZY...
-00004970: 6a8b f7ef 226a 50c6 e8a2 b3f9 9622 116b  j..."jP......".k
-00004980: 39f7 df6c ac9d 8422 2b88 b586 21d4 0cf9  9..l..."+...!...
-00004990: 7dbc 4853 63a6 7e11 5e4e bdc4 cb48 3590  }.HSc.~.^N...H5.
-000049a0: f965 983a 010d 1f4a 0937 d108 4e48 e2e7  .e.:...J.7..NH..
-000049b0: 623c 9043 899e c483 6d56 4a3c 0fa9 33d5  b<.C....mVJ<..3.
-000049c0: 4708 8f7a 5972 8c67 0e69 c4df 4123 809d  G..zYr.g.i..A#..
-000049d0: 4343 22a4 a261 f6d3 a9ec e564 e748 b2d8  CC"..a.....d.H..
-000049e0: d031 6b6d 39d6 1987 e140 1933 5797 638e  .1km9....@.3W.c.
-000049f0: 5974 99e5 a92a 660e df24 2f60 2706 9923  Yt...*f..$/`'..#
-00004a00: 8e64 2824 0c1e 9d45 622f 86b6 5fb9 4f97  .d($...Eb/.._.O.
-00004a10: b4d1 029f 9657 e6d3 2563 f084 7c2a 0e97  .....W..%c..|*..
-00004a20: f069 ecc5 f0fc 9fc9 5ea5 e3a1 60b0 3bff  .i......^...`.;.
-00004a30: e199 2c09 728f 38fd af5d f807 504b 0304  ..,.r.8..]..PK..
-00004a40: 1400 0000 0800 b789 6449 e85a e553 0001  ........dI.Z.S..
-00004a50: 0000 b601 0000 1400 0000 776f 7264 2f77  ..........word/w
-00004a60: 6562 5365 7474 696e 6773 2e78 6d6c 8dd0  ebSettings.xml..
-00004a70: c16a c330 0c00 d07b bec2 e492 53e3 648c  .j.0...{....S.d.
-00004a80: 3142 9232 181d bb94 41b6 0f70 1c25 31b5  1B.2....A..p.%1.
-00004a90: 2d63 b9cd faf7 3359 3618 bbf4 2621 e921  -c....3Y6...&!.!
-00004aa0: a9de 7f1a cd2e e049 a16d b232 2f32 0656  .......I.m.2/2.V
-00004ab0: e2a0 ecd4 641f ef87 dd63 c628 083b 088d  ....d....c.(.;..
-00004ac0: 169a ec0a 94ed dba4 5eaa 05fa 0e42 888d  ........^....B..
-00004ad0: c422 62a9 32b2 49e7 105c c539 c919 8ca0  ."b.2.I..\.9....
-00004ae0: 1c1d d858 1cd1 1b11 62ea 276e 843f 9ddd  ...X....b.'n.?..
-00004af0: 4ea2 7122 a85e 6915 aefc ae28 1ed2 8df1  N.q".^i....(....
-00004b00: b728 388e 4ac2 33ca b301 1bd6 79ee 4147  .(8.J.3.....y.AG
-00004b10: 112d cdca d18f b6dc a22d e807 e751 0251  .-.......-...Q.Q
-00004b20: bcc7 e86f cf08 657f 99f2 fe1f 6494 f448  ...o..e.....d..H
-00004b30: 3886 3c1e b36d b452 71bc 2cd6 c8e8 9419  8.<..m.Rq.,.....
-00004b40: 59bd 4e16 bde8 3534 6984 d236 612c 7e50  Y.N...54i..6a,~P
-00004b50: 688d cbdb f185 6ff9 8047 0c9d b8c0 1375  h.....o..G.....u
-00004b60: 710d 0d07 a521 166b fee7 db6d f205 504b  q....!.k...m..PK
-00004b70: 0102 1403 1400 0000 0800 b789 6449 2914  ............dI).
-00004b80: c70a 7801 0000 e705 0000 1300 0000 0000  ..x.............
-00004b90: 0000 0000 0000 8001 0000 0000 5b43 6f6e  ............[Con
-00004ba0: 7465 6e74 5f54 7970 6573 5d2e 786d 6c50  tent_Types].xmlP
-00004bb0: 4b01 0214 0314 0000 0008 00b7 8964 490e  K............dI.
-00004bc0: eeab 75fd 0000 00ec 0200 000b 0000 0000  ..u.............
-00004bd0: 0000 0000 0000 0080 01a9 0100 005f 7265  ............._re
-00004be0: 6c73 2f2e 7265 6c73 504b 0102 1403 1400  ls/.relsPK......
-00004bf0: 0000 0800 b789 6449 705a 4d79 8f01 0000  ......dIpZMy....
-00004c00: 0e03 0000 1000 0000 0000 0000 0000 0000  ................
-00004c10: 8001 cf02 0000 646f 6350 726f 7073 2f61  ......docProps/a
-00004c20: 7070 2e78 6d6c 504b 0102 1403 1400 0000  pp.xmlPK........
-00004c30: 0800 b789 6449 2383 c6e8 7601 0000 d902  ....dI#...v.....
-00004c40: 0000 1100 0000 0000 0000 0000 0000 8001  ................
-00004c50: 8c04 0000 646f 6350 726f 7073 2f63 6f72  ....docProps/cor
-00004c60: 652e 786d 6c50 4b01 0214 0314 0000 0008  e.xmlPK.........
-00004c70: 00b7 8964 494c 7849 6ac3 2100 00e8 4400  ...dILxIj.!...D.
-00004c80: 0017 0000 0000 0000 0000 0000 0080 0131  ...............1
-00004c90: 0600 0064 6f63 5072 6f70 732f 7468 756d  ...docProps/thum
-00004ca0: 626e 6169 6c2e 6a70 6567 504b 0102 1403  bnail.jpegPK....
-00004cb0: 1400 0000 0800 b789 6449 1559 4ccc 1401  ........dI.YL...
-00004cc0: 0000 cc03 0000 1c00 0000 0000 0000 0000  ................
-00004cd0: 0000 8001 2928 0000 776f 7264 2f5f 7265  ....)(..word/_re
-00004ce0: 6c73 2f64 6f63 756d 656e 742e 786d 6c2e  ls/document.xml.
-00004cf0: 7265 6c73 504b 0102 1403 1400 0000 0800  relsPK..........
-00004d00: b789 6449 2352 56af c305 0000 e935 0000  ..dI#RV......5..
-00004d10: 1100 0000 0000 0000 0000 0000 8001 7729  ..............w)
-00004d20: 0000 776f 7264 2f64 6f63 756d 656e 742e  ..word/document.
-00004d30: 786d 6c50 4b01 0214 0314 0000 0008 00b7  xmlPK...........
-00004d40: 8964 491b eedb 0322 0200 00ac 0800 0012  .dI...."........
-00004d50: 0000 0000 0000 0000 0000 0080 0169 2f00  .............i/.
-00004d60: 0077 6f72 642f 666f 6e74 5461 626c 652e  .word/fontTable.
-00004d70: 786d 6c50 4b01 0214 0314 0000 0008 00b7  xmlPK...........
-00004d80: 8964 4975 6432 89c1 0300 0032 0a00 0011  .dIud2.....2....
-00004d90: 0000 0000 0000 0000 0000 0080 01bb 3100  ..............1.
-00004da0: 0077 6f72 642f 7365 7474 696e 6773 2e78  .word/settings.x
-00004db0: 6d6c 504b 0102 1403 1400 0000 0800 b789  mlPK............
-00004dc0: 6449 00e7 c135 5806 0000 5a41 0000 0f00  dI...5X...ZA....
-00004dd0: 0000 0000 0000 0000 0000 8001 ab35 0000  .............5..
-00004de0: 776f 7264 2f73 7479 6c65 732e 786d 6c50  word/styles.xmlP
-00004df0: 4b01 0214 0314 0000 0008 00b7 8964 4944  K............dID
-00004e00: cde5 e6db 0600 00bc 4400 001a 0000 0000  ........D.......
-00004e10: 0000 0000 0000 0080 0130 3c00 0077 6f72  .........0<..wor
-00004e20: 642f 7374 796c 6573 5769 7468 4566 6665  d/stylesWithEffe
-00004e30: 6374 732e 786d 6c50 4b01 0214 0314 0000  cts.xmlPK.......
-00004e40: 0008 00b7 8964 4994 4122 b8c6 0600 00bb  .....dI.A"......
-00004e50: 2a00 0015 0000 0000 0000 0000 0000 0080  *...............
-00004e60: 0143 4300 0077 6f72 642f 7468 656d 652f  .CC..word/theme/
-00004e70: 7468 656d 6531 2e78 6d6c 504b 0102 1403  theme1.xmlPK....
-00004e80: 1400 0000 0800 b789 6449 e85a e553 0001  ........dI.Z.S..
-00004e90: 0000 b601 0000 1400 0000 0000 0000 0000  ................
-00004ea0: 0000 8001 3c4a 0000 776f 7264 2f77 6562  ....<J..word/web
-00004eb0: 5365 7474 696e 6773 2e78 6d6c 504b 0506  Settings.xmlPK..
-00004ec0: 0000 0000 0d00 0d00 4e03 0000 6e4b 0000  ........N...nK..
-00004ed0: 0000                                     ..
+00002980: 0091 819b 58ba 6b84 6e80 0600 004e 3e00  ....X.k.n....N>.
+00002990: 0011 001c 0077 6f72 642f 646f 6375 6d65  .....word/docume
+000029a0: 6e74 2e78 6d6c 5554 0900 0362 862d 6662  nt.xmlUT...b.-fb
+000029b0: 862d 6675 780b 0001 04f5 0100 0004 1400  .-fux...........
+000029c0: 0000 ed5b 4b73 a338 10be cfaf 607d c9ee  ...[Ks.8....`}..
+000029d0: 2163 211e 0257 9229 8461 66aa 66aa 5293  !c!..W.).af.f.R.
+000029e0: d9dd e316 c6b2 cd06 1005 b29d ecaf 5f89  .............._.
+000029f0: 878d edc4 c68f c49e 3839 38b4 a46e 7ddd  ........898..n}.
+00002a00: ea6e 3502 ae3e 3d44 a134 2169 16d0 f8fa  .n5..>=D.4!i....
+00002a10: 42fe 082e 2412 fbb4 1fc4 c3eb 8b3f 7fba  B...$........?..
+00002a20: 97c6 8594 312f ee7b 218d c9f5 c523 c92e  ....1/.{!....#..
+00002a30: 3edd 7cb8 9a76 fad4 1f47 2466 1297 1067  >.|..v...G$f...g
+00002a40: 9d69 e25f b746 8c25 9d76 3bf3 4724 f2b2  .i._.F.%.v;.G$..
+00002a50: 8f51 e0a7 34a3 03f6 d1a7 519b 0e06 814f  .Q..4.....Q....O
+00002a60: da53 9af6 db10 c820 bf4a 52ea 932c e3d3  .S..... .JR..,..
+00002a70: d95e 3cf1 b256 292e a2cd a445 9e5f 5d42  .^<..V)....E._]B
+00002a80: 000c 4e07 f14c c62a 229a 9098 770e 681a  ..N..L.*"...w.h.
+00002a90: 798c 93e9 9073 a4f7 e3e4 92cb 4c3c 16f4  y....s......L<..
+00002aa0: 8230 608f 4296 3e13 33b9 6e8d d3b8 53ca  .0`.B.>.3.n...S.
+00002ab0: b89c e110 3c1d 0ea0 3389 c26a 305d 37b6  ....<...3..j0]7.
+00002ac0: 005a feab 38d2 2620 0b96 6e69 f21c 5e3b  .Z..8.& ..ni..^;
+00002ad0: 2521 074c e36c 1424 73bb ed2a 8d77 8e2a  %!.L.l.$s..*.w.*
+00002ae0: 216b 15ae 293b 4d64 75bf 45ef a6de 94ff  !k..);Mdu.E.....
+00002af0: 9b0b 6c02 bf5f 3045 6181 7cbd 4419 3458  ..l.._0Ea.|.D.4X
+00002b00: 1121 62c6 d104 c2e2 9c15 92ba f34d 7733  .!b..........Mw3
+00002b10: 4ddd b8c3 fd6c fb39 a5e3 642e 2dd8 4fda  M....l.9..d.-.O.
+00002b20: d7f8 7e26 8b27 826d 6495 6b54 572d db0f  ..~&.'.md.kTW-..
+00002b30: ccdd c84b 7800 457e e7eb 30a6 a9d7 0b39  ...Kx.E~..0....9
+00002b40: 226e 7149 7864 ebe6 8324 f104 d5a3 fd47  "nqIxd...$.....G
+00002b50: 7199 13ac 1716 d715 759b 5674 d572 c71e  q.......u.Vt.r..
+00002b60: 4322 4d3b 132f bc6e fd14 323f a741 bfd5  C"M;./.n..2?.A..
+00002b70: 5e1e f737 1fc3 9d04 b4f8 7ff6 98f0 99bd  ^..7............
+00002b80: 31a3 abe3 be51 7a5f 8903 aa95 8f1f 0469  1....Qz_.......i
+00002b90: c67e 50ce 2e0b 32f4 4a6a de69 d370 1cc5  .~P...2.Jj.i.p..
+00002ba0: b5fe aa21 1f12 d32f 9827 e319 f557 41c9  ...!.../.'...WA.
+00002bb0: f3d9 afda 4bea 1560 842a 0b00 87bc 818b  ....K..`.*......
+00002bc0: 2e74 8110 ae48 a873 0819 291f cab7 89fe  .t...H.s..).....
+00002bd0: 0f3e 39b0 b002 4c01 5156 3b89 977a 5f39  .>9...L.QV;..z_9
+00002be0: 08e8 b808 215b 2b5a 1979 60a2 1595 7fad  ....![+Z.y`.....
+00002bf0: 92fd 675a e35f 3499 3f27 cb86 fa22 cd1a  ..gZ._4.?'..."..
+00002c00: 37db bfd4 6189 9d33 270b 8081 a63a 08bb  7...a..3'....:..
+00002c10: ce7a c08b fa16 4d5d 32f0 c621 abf5 d457  .z....M]2..!...W
+00002c20: bf5d d725 a74a 1ca5 6567 4eb9 0847 d7b1  .].%.J..egN..G..
+00002c30: 651a b6dc 008e ac01 a4e2 a7e0 943d ed63  e............=.c
+00002c40: 3abe 4dc2 f0bb b76c fb90 0c58 2140 96b5  :.M....l...X!@..
+00002c50: b988 fe83 b7b4 745c a960 386a 30b6 34e7  ......t\.`8j0.4.
+00002c60: ca74 bf5c f8c9 aa0a f68f 3fa0 3832 d2dd  .t.\......?.82..
+00002c70: 0dfe b326 fed2 9578 61e9 1752 ae45 6147  ...&...xa..R.EaG
+00002c80: 2165 f463 1c3e b5f6 ed65 11db c774 6e88  !e.c.>...e...tn.
+00002c90: e75d 231f 3cb1 c260 1857 887a 9431 1aed  .]#.<..`.W.z.1..
+00002ca0: 10fc b26b 28b2 ad76 4f24 f811 366d 1343  ...k(..vO$..6m.C
+00002cb0: 7c40 3847 daf5 bc47 3a66 b341 83e0 813c  |@8G...G:f.A...<
+00002cc0: 21ed 3d45 6cbb 431b c601 5204 5474 6420  !.=El.C...R.Ttd 
+00002cd0: dd7e c114 9103 ad65 09f6 8d70 131d 3a51  .~.....e...p..:Q
+00002ce0: 54b3 344f 143e bfd3 21e9 0e89 4295 5d13  T.4O.>..!...B.].
+00002cf0: 2be8 5412 85a6 d9d0 351c d000 8e66 001b  +.T.....5....f..
+00002d00: ab4f c159 ecb9 ad35 1d37 77fc 3af1 b8b8  .O.Y...5.7w.:...
+00002d10: 65ef dbdf 249e 676b 56df f25d 64ba aaaa  e...$.gkV..]d...
+00002d20: 3689 6753 93dd aebe 753c ab0a acc7 3379  6.gS....u<....3y
+00002d30: f0fc 8347 f3f6 db3e a3c9 0ea1 ac28 5d88  ...G...>.....(].
+00002d40: bac6 863b 94ed 63a7 34ed b3d1 fd02 3669  ...;..c.4.....6i
+00002d50: a42f ec42 5d01 6843 ba7f 4bfa ca0e 76b4  ./.B].hC..K...v.
+00002d60: 2637 7407 d5b7 9ebd 1b46 ae02 0d6c 2ab6  &7t......F...l*.
+00002d70: b273 e4be be75 3595 97a8 7ceb 3917 6f92  .s...u5...|.9.o.
+00002d80: 9125 bb3a 30cf 455f 05eb 06b2 9d26 e70f  .%.:0.E_.....&..
+00002d90: 2f16 3deb 6b1f e862 804c fde0 088f 5efb  /.=.k..b.L....^.
+00002da0: fceb 5792 c42d d07b 61b4 7761 a441 d354  ..W..-.{a.wa.A.T
+00002db0: 2d15 bd60 61a4 21fd d885 51b3 4d11 c0ae  -..`a.!...Q.M...
+00002dc0: 66e9 1b4c f176 d218 d05d d951 1df7 6cf4  f..L.v...].Q..l.
+00002dd0: 351c 43c5 ca51 d376 d3a8 04d8 3614 6bc3  5.C..Q.v....6.k.
+00002de0: 8e7a 5a45 4fd7 56b4 02dc 5978 1334 5d57  .zZEO.V...Yx.4]W
+00002df0: 35cd b389 1e55 c606 d4dd 26a7 3b47 2a7a  5....U....&.;G*z
+00002e00: 742c 2b5d 1b1f fc26 ee84 8a9e fc30 f7bd  t,+]...&.....0..
+00002e10: ead9 bbea 8196 6500 0c37 046f 915f 4bfe  ......e..7.o._K.
+00002e20: 4d55 cfba 453a 9102 07a9 00b9 267c f510  MU..E:......&|..
+00002e30: 3e9a bec0 71a1 d3e8 c9d5 9bd0 17c2 2e50  >...q..........P
+00002e40: 15f1 3ed6 e917 3886 d555 00b2 ce2b 0079  ..>...8..U...+.y
+00002e50: 5527 dbc0 391f 8754 64e8 eaf2 8653 f737  U'..9..Td....S.7
+00002e60: a4af 8990 ac5b 1bbc fa98 3512 40d0 b434  .....[....5.@..4
+00002e70: bdc9 d3f3 5fb5 465a 7d7e f95e 24ed f6cc  ...._.FZ}~.^$...
+00002e80: cc86 5843 a0d1 6b32 5be7 e827 56e9 4492  ..XC..k2[..'V.D.
+00002e90: b4ae 608c 5ded a592 d60a f81e f74b f16a  ..`.]........K.j
+00002ea0: f51d f352 7166 16cc dcc9 8bb8 12ff 7ca6  ...Rqf........|.
+00002eb0: d8f3 ef57 1549 4e2d fb29 aa85 1cd9 3d9f  ...W.IN-.)....=.
+00002ec0: 1300 64aa 1634 5e7d 77db e521 9a0b 3036  ..d..4^}w..!..06
+00002ed0: 37bd c0f9 e642 1969 5833 b0f3 eafb f1d1  7....B.iX3......
+00002ee0: cee0 80ad 199a 0bcf 455f 55c5 40c7 d038  ........E_U.@..8
+00002ef0: 7a04 5639 dc89 fbb3 0c5e d542 6beb 31c5  z.V9.....^.Bk.1.
+00002f00: 7530 54ad 8368 c027 2c26 f9ed f252 62a2  u0T..h.',&...Rb.
+00002f10: 9e92 46de 2488 8752 4aa7 99f8 3829 6582  ..F.$..RJ...8)e.
+00002f20: 9a06 6c24 9128 618f 92a8 1aa4 8466 41fe  ..l$.(a......fA.
+00002f30: 798c f47b 5147 6032 a029 f943 babc 7cbe  y..{QG`2.).C..|.
+00002f40: 9c5b 5fc0 6860 6d7d 72c0 ee85 e2a6 9e12  .[_.h`m}r.......
+00002f50: 977d 5398 5efc a4e2 87dd 7839 e38d f84d  .}S.^.....x9...M
+00002f60: 6f8a edf4 699f 5ee2 ebed c8e7 efc8 d7df  o...i.^.........
+00002f70: c457 f9e2 f3ba 8b44 7c55 5fd9 2a71 8b32  .W.....D|U_.*q.2
+00002f80: f5b9 54bd 0483 ec08 7fb0 23df f005 d586  ..T.......#.....
+00002f90: cdd5 1eed 083f 7841 f84a 73f8 ff36 8551  .....?xA.Js..6.Q
+00002fa0: 8ba4 f549 84c4 fdf7 1472 d629 c41a f062  ...I.....r.)...b
+00002fb0: efec 32c8 82d6 2797 4096 42f7 75be 97ca  ..2...'.@.B.u...
+00002fc0: 88cf 6e9f bef3 c89b ee78 bf68 058a aacb  ..n......x.h....
+00002fd0: f3fb 5e81 6e78 f75f 5904 4258 5481 237e  ..^.nx._Y.BXT.#~
+00002fe0: ad19 0ba7 1662 dc77 4f4c c068 32af 17f3  .....b.wOL.h2...
+00002ff0: c35d 4e1a 2027 8bcf 5ae6 dde2 b5a0 79ef  .]N. '..Z.....y.
+00003000: 8878 7dc2 ef6a 50f1 6aee 8052 5623 8763  .x}..jP.j..RV#.c
+00003010: 9693 8bb3 fa34 cc78 6796 783e 2986 d67b  .....4.xg.x>)..{
+00003020: fbd4 1789 42cc 14c4 e436 603e 87ae e80b  ....B....6`>....
+00003030: e55e 6119 410b aaf8 ba52 5c55 1f82 df7c  .^a.A....R\U...|
+00003040: f81f 504b 0304 1400 0000 0800 b789 6449  ..PK..........dI
+00003050: 1bee db03 2202 0000 ac08 0000 1200 0000  ...."...........
+00003060: 776f 7264 2f66 6f6e 7454 6162 6c65 2e78  word/fontTable.x
+00003070: 6d6c e595 3f6e db30 14c6 779f 82d0 a229  ml..?n.0..w....)
+00003080: 1625 2ba9 6b58 0eda b406 ba74 28dc 03d0  .%+.kX.....t(...
+00003090: 3465 13e5 1f81 a4ec 7875 f6ce 1dda 2314  4e......xu....#.
+000030a0: 1d5a a04b 6e63 206b ae90 175a 5614 3476  .Z.Knc k...ZV.4v
+000030b0: e3a1 29d0 5210 44be 8ffc f4f8 c323 d83f  ..).R.D......#.?
+000030c0: 3d97 02cd 99b1 5cab 2c8c db38 444c 513d  =.....\.,..8DLQ=
+000030d0: e16a 9a85 ef47 c3a3 6e88 ac23 6a42 8456  .j...G..n..#jB.V
+000030e0: 2c0b 97cc 86a7 8356 7fd1 cbb5 7216 c172  ,......V....r..r
+000030f0: 657b 9266 c1cc b9a2 1745 96ce 9824 b6ad  e{.f.....E...$..
+00003100: 0ba6 40cc b591 c4c1 d04c 2349 cc87 b238  ..@......L#I...8
+00003110: a25a 16c4 f131 17dc 2da3 04e3 93a0 b231  .Z...1..-......1
+00003120: 8f71 d179 ce29 7ba5 6929 9972 7e7d 6498  .q.y.){.i).r~}d.
+00003130: 0047 adec 8c17 76eb b678 8cdb 429b 4961  .G....v..x..B.Ia
+00003140: 3465 d6c2 96a5 d8f8 49c2 556d 13a7 bf18  4e......I.Um....
+00003150: 494e 8db6 3a77 6dd8 4c95 91b7 82e5 31f6  IN..:wm.L.....1.
+00003160: 3d29 0224 69ef cd54 6943 c682 6501 1805  =).$i..TiC..e...
+00003170: 8316 4215 3bb4 e829 2221 7e46 e4d8 70e2  ..B.;..)"!~F..p.
+00003180: 35af 1644 69cb 6298 3027 220b 7082 537c  5..Di.b.0'".p.S|
+00003190: 8c3b f0a6 f804 be30 0ea2 7a36 9d11 6399  .;.....0..z6..c.
+000031a0: ab67 e386 9613 c9c5 722b 91d2 e986 5870  .g......r+....Xp
+000031b0: 4767 5b6d 4e20 0548 b3a1 5b3e 05b5 b463  Gg[mN .H..[>...c
+000031c0: 9c05 af31 b464 380c 3691 380b d2db 485a  ...1.d8.6.8...HZ
+000031d0: 4792 db3f 6f5a 15e9 dc8f 50ef e387 f1f3  G..?oZ....P.....
+000031e0: 6115 891b 73fc 8ffb d106 ce43 9cae 2fbf  a...s......C../.
+000031f0: 5e5f 7e47 579f 3e5e 7dfe b29b d603 6d37  ^_~GW.>^}.....m7
+00003200: adee 6e5a 464b a21a aad2 6e64 4a36 5a16  ..nZFK....ndJ6Z.
+00003210: 6c07 c39c 9fb3 c90e 8055 26f1 1d40 dcc5  l........U&..@..
+00003220: cf1a b86a 80f1 ef00 268d c841 0047 5c32  ...j....&..A.G\2
+00003230: 8bde b205 7ae7 f7b6 a7e0 125f 68c7 bef0  ....z......_h...
+00003240: 12e8 3d79 c155 9bea 3478 dd2f af43 0aae  ..=y.U..4x./.C..
+00003250: e27e 28af 1790 a1d8 47e9 2550 4a3d adcd  .~(.....G.%PJ=..
+00003260: f35f 52aa 8ee5 7af5 63bd fab9 beb8 58af  ._R...z.c.....X.
+00003270: befd f9c3 29f5 8499 7feb 749e 11c1 e11e  ....).....t.....
+00003280: d857 6f43 7f1a 7da5 fd9d 6be0 e9eb 6ddb  .WoC..}...k...m.
+00003290: b383 d60d 504b 0304 1400 0000 0800 b789  ....PK..........
+000032a0: 6449 7564 3289 c103 0000 320a 0000 1100  dIud2.....2.....
+000032b0: 0000 776f 7264 2f73 6574 7469 6e67 732e  ..word/settings.
+000032c0: 786d 6cb5 56db 6ee3 3610 7dcf 5708 7af1  xml.V.n.6.}.W.z.
+000032d0: 4b1d 49be 2535 e22c 92b8 6e13 c4dd a0ca  K.I.%5.,..n.....
+000032e0: 7e00 258d 6d36 bc81 a4ec 78bf be43 4994  ~.%.m6....x..CI.
+000032f0: 6404 e91a 5df4 c99a 3967 2e1c ce0c 7df3  d...]...9g....}.
+00003300: e59d b360 0fda 5029 1683 e432 1e04 2072  ...`..P)...2.. r
+00003310: 5950 b15d 0cbe bdae 86d7 83c0 5822 0ac2  YP.]........X"..
+00003320: a480 c5e0 0866 f0e5 f6e2 e630 3760 2db2  .....f.....07`-.
+00003330: 4c80 1e84 99f3 7c11 eeac 55f3 2832 f90e  L.....|...U.(2..
+00003340: 3831 9752 8140 7023 3527 1645 bd8d 38d1  81.R.@p#5'.E..8.
+00003350: 6fa5 1ae6 922b 6269 4619 b5c7 6814 c7b3  o....+biF...h...
+00003360: b071 2317 61a9 c5bc 7131 e434 d7d2 c88d  .q#.a...q1.4....
+00003370: 7526 73b9 d9d0 1c9a 1f6f a1cf 895b 9b2c  u&s......o...[.,
+00003380: 655e 7210 b68a 1869 6098 8314 6647 95f1  e^r....i`...fG..
+00003390: def8 7ff5 86e0 ce3b d9ff db21 f69c 79de  .......;...!..y.
+000033a0: 2189 cf38 ee41 eaa2 b538 273d 67a0 b4cc  !..8.A...8'=g...
+000033b0: c118 bc20 ce7c 8254 7481 271f 1cb5 b12f  ... .|.Tt.'..../
+000033c0: 3176 73c4 ca15 9a27 71f5 d565 6ed8 3989  1vs....'q..en.9.
+000033d0: d4d0 33cd 34d1 c77e 163c 9f3f 6e85 d424  ..3.4..~.<.?n..$
+000033e0: 63b0 0831 9bf0 f622 08b0 a9be 4bc9 83c3  c..1..."....K...
+000033f0: 7c4f d07f 06c6 aea8 0d51 56a0 73ac f422  |O.......QV.s.."
+00003400: 1c25 d761 d470 f188 7293 5a62 0119 4601  .%.a.p..r.Zb..F.
+00003410: 63ae 69c3 9c01 11ce 68ab 09c7 7ef3 1a6f  c.i.....h...~..o
+00003420: 56c0 8694 ccbe 922c b552 f960 57a3 b865  V......,.R.`W..e
+00003430: e43b a249 6e41 a78a e4e8 f341 0aab 25f3  .;.InA.....A..%.
+00003440: d442 fe29 ed03 76b0 c602 b746 86ec e145  .B.)..v....F...E
+00003450: c39e c2e1 85e6 b6d4 d0ba ab9a dd09 9558  ...............X
+00003460: 1a58 fdf6 4c8e b2b4 51ab ac39 693d 5218  .X..L...Q..9i=R.
+00003470: 4810 8e85 3919 93b5 2cc0 1dab d4f4 fcbb  H...9...,.......
+00003480: 0b7d d258 e21f 4593 b806 342d e0d5 dd4a  .}.X..E...4-...J
+00003490: 6a8f 0c56 78f0 947e 873b 513c 95c6 5274  j..Vx..~.;Q<..Rt
+000034a0: 5b4d cc4f a4f1 c32c 40b8 f05f b199 5e8f  [M.O...,@.._..^.
+000034b0: 0a56 405c 29cd ff19 b1ba cf15 a36a 4db5  .V@\)........jM.
+000034c0: 96fa 5114 d86a 3f1f f126 ea5f 3d46 c71d  ..Q..j?..&._=F..
+000034d0: 5b98 3617 27fd 25a5 f556 717c 773f 8e7f  [.6.'.%..Vq|w?..
+000034e0: eda7 eb28 1d1c 8f27 b364 f629 9c4c e3ab  ...(...'.d.).L..
+000034f0: c9fd a7f0 f43a 7eb8 9f7c 0af7 63bb c4db  .....:~..|..c...
+00003500: 5c6f f8dc 6db6 17dd 18d6 a26b 8c80 d7c6  \o..m......k....
+00003510: 0f84 679a 9260 ed16 60d4 d232 fd76 4f85  ..g..`..`..2.vO.
+00003520: 2765 807b 013e c069 9979 c670 d843 0d27  'e.{.>.i.y.p.C.'
+00003530: 8cad 7008 3d1a f7c0 821a b584 4da7 606b  ..p.=.......M.`k
+00003540: a2b7 5dac 3e57 7f0e e11e 786a fdbb ed02  ..].>W....xj....
+00003550: fa77 2d4b d5a3 1c34 5175 3b78 5e32 99f4  .w-K...4Qu;x^2..
+00003560: 7d50 619f 29f7 a029 b3f4 c45e e0da ebe1  }Pa.)..)...^....
+00003570: a528 beee b52f 72bf b078 1f16 dbab 1ab8  .(.../r..x......
+00003580: 6752 f566 6501 62f8 2d75 8d05 c4d8 3b43  gR.fe.b.-u....;C
+00003590: c922 fc9b 0c9f 5eba 55c5 74ea 1a13 d644  ."....^.U.t....D
+000035a0: a9ba a9b3 6db2 0819 ddee 6ce2 2c2d 4a05  ....m.....l.,-J.
+000035b0: beba 9590 6d47 0d36 aab0 518d 5502 c95d  ....mG.6..Q.U..]
+000035c0: 1190 dd7c 74ba 91d7 f578 63af 1b77 ba89  ...|t....xc..w..
+000035d0: d74d 3add d4eb a69d 6ee6 7533 a7db e198  .M:.....n.u3....
+000035e0: 6b5c dd6f 386a fed3 e937 9231 7980 e28f  k\.o8j...7.1y...
+000035f0: 0eff a0ea 96ba 9be1 bbd2 4abf 979b 1d6c  ..........J....l
+00003600: daf5 bc23 0a96 f5ea f743 286b 6df3 2098  ...#.....C(km. .
+00003610: 603f 8777 7c63 a070 8f8e 51b4 e0e4 1daf  `?.w|c.p..Q.....
+00003620: 3c1e 5db5 77da 98b0 6a7d 9f18 d484 8ae2  <.].w...j}......
+00003630: 0cd5 a9b7 8258 d2df 45d1 8923 3f75 1f92  .....X..E..#?u..
+00003640: ac9e ab9c e234 a447 9e75 4fd0 657b 7046  .....4.G.uO.e{pF
+00003650: 0d2e 3485 0f96 95da c3bf 7838 9960 65f2  ..4.......x8.`e.
+00003660: 471c 74fc aaa0 c978 365d adae 977d 461d  G.t....x6]...}F.
+00003670: f091 932d 2c15 edb8 e3b8 eaf5 2ab3 e6cf  ...-,.......*...
+00003680: deed c53f 504b 0304 1400 0000 0800 b789  ...?PK..........
+00003690: 6449 00e7 c135 5806 0000 5a41 0000 0f00  dI...5X...ZA....
+000036a0: 0000 776f 7264 2f73 7479 6c65 732e 786d  ..word/styles.xm
+000036b0: 6ce5 9b4b 73e3 2810 c7ef f329 54ba f894  l..Ks.(....)T...
+000036c0: f895 d871 2a9e a9bc 6693 aacc 4c66 9cec  ...q*...f...Lf..
+000036d0: 9e31 c216 1509 b480 f398 4f3f e865 cb91  .1........O?.e..
+000036e0: 6db5 acde 5cf6 6621 ba7f 0d34 fc91 0bce  m...\.f!...4....
+000036f0: bebc 8681 f3cc 94e6 528c 5bdd c34e cb61  ........R.[..N.a
+00003700: 824a 8f8b f9b8 f5f8 f0f5 e0a4 e568 4384  .J...........hC.
+00003710: 4702 29d8 b8f5 c674 ebcb e74f 672f a7da  G.)....t...Og/..
+00003720: bc05 4c3b d65e e8d3 908e 5ddf 98e8 b4dd  ..L;.^....].....
+00003730: d6d4 6721 d187 3262 c2be 9c49 1512 631f  ..g!..2b...I..c.
+00003740: d5bc 1d12 f5b4 880e a80c 2362 f894 07dc  ..........#b....
+00003750: bcb5 7b9d cec0 cddc 2888 1739 9b71 caae  ..{.....(..9.q..
+00003760: 245d 844c 98c4 bead 5860 3d4a a17d 1ee9  $].L....X`=J.}..
+00003770: dcdb 0bc4 db8b 545e a424 655a db36 8741  ......T^.$eZ.6.A
+00003780: ea2f 245c 2cdd 748f 4a8e 424e 95d4 7266  ./$\,.t.J.BN..rf
+00003790: 0e6d 63b2 8812 57d6 bcdb 497e 8581 eb84  .mc...W...I~....
+000037a0: f4f4 762e a422 d380 8d5d ebc8 fdfc c971  ..v.."...].....q
+000037b0: 6ce7 7992 5eb1 1959 0446 c725 4999 ba57  l.y.^..Y.F.%I..W
+000037c0: 5959 5a94 17e6 4fe9 f357 298c 765e 4e89  YYZ...O..W).v^N.
+000037d0: a69c 3fd8 68ac e390 5bc6 cdb9 d0dc b56f  ..?.h...[......o
+000037e0: 18d1 e65c 7352 7c79 9d95 c5ef fdb8 e246  ...\sR|y.......F
+000037f0: 4baa 4da1 f882 7bdc 6daf d1f5 6f5b eb99  K.M...{.m...o[..
+00003800: 0463 b777 547a 75a9 b7be 0c88 98e7 2f99  .c.wTzu......./.
+00003810: 3878 9c14 e32c 144d 2d72 ec12 7530 395f  8x...,.M-r..u09_
+00003820: 7938 6b17 ba21 7b58 eb28 0b88 9645 8959  y8k..!{X.(...E.Y
+00003830: 5ceb 5d17 2751 189b 3093 346f 6d05 36bb  \.].'Q..0.4om.6.
+00003840: 93f4 8979 1363 5f8c dd8e 9b16 3ede de2b  ...y.c_.....>..+
+00003850: 2e95 cdcd b13b 1a65 8513 16f2 1bee 794c  .....;.e......yL
+00003860: 8cdd 6e5e 51f8 dc63 fff8 4c3c 6ae6 adca  ..n^Q..c..L<j...
+00003870: 7f7e 4df2 2bf3 48e5 42d8 dfbd e1c0 5d86  .~M.+.H.B.....].
+00003880: 1b68 effa 95b2 284e 595b 4590 b8d3 bfc7  .h....(NY[E.....
+00003890: 5641 6ca2 0bb0 c4c7 82af 424a 0bde a193  VAl.......BJ....
+000038a0: c27f 736e 37ef bc6d 289f 9178 863b dd4a  ..sn7..m(..x.;.J
+000038b0: da08 91d6 dbe8 bcbe 9f3e 929f 2324 3fc7  .........>..#$?.
+000038c0: 487e 0648 7e86 487e 4e90 fc8c 1afa 3192  H~.H~.H~N.....1.
+000038d0: a699 5af4 d11f 41cc 4a29 0733 2b65 18cc  ..Z...A.J).3+e..
+000038e0: ac94 5030 b352 fec0 cc4a e902 332b 6507  ..P0.R...J..3+e.
+000038f0: ccac 940c 30b3 d2d8 579b 5192 3c97 0c8f  ....0...W.Q.<...
+00003900: eb65 cd03 3701 ab5c dfba 18cb 69a6 33ce  .e..7..\....i.3.
+00003910: 3d51 64ae 48e4 3bb1 4a97 5055 6e26 8ba9  =Qd.H.;.J.PUn&..
+00003920: 8105 dd45 087a 6294 14f3 4a56 af87 c0ba  ...E.zb...JV....
+00003930: 0e23 9f68 aeab 6918 c3f1 106f b79c bf14  .#.h..i....o....
+00003940: f72a 79c7 5bf4 ad82 701f 10ca 7c19 784c  .*y.[...p...|.xL
+00003950: 390f ecd5 ece5 e4bb 7426 11a1 1c30 0818  9.......t&...0..
+00003960: e37d c7e7 be71 267e b226 5712 075b 0602  .}...q&~.&W..[..
+00003970: 04b9 e3da 5413 b634 0a44 000d ee60 4bea  ....T..4.D...`K.
+00003980: 5610 be31 8f2f c2bc a700 7ba4 411f 83d3  V..1./....{.A...
+00003990: abe6 1c35 e1c4 8302 69cc 7163 08a0 2583  ...5....i.qc..%.
+000039a0: 2690 78f0 212d 1936 8600 5a72 d218 d2af  &.x.!-.6..Zr....
+000039b0: 86ec b74a 5dd9 cf6d d85c 1cee 37db 2f65  ...J]..m.\..7./e
+000039c0: 20d5 6c11 8057 95e1 7e73 7ec9 8135 66bf   .l..W..~s~..5f.
+000039d0: 69bf 8480 d696 e17e 737e 6d11 76ce 29b5  i......~s~m.v.).
+000039e0: 1fa4 9054 6eba 1ad7 4035 5d96 6ba0 70d6  ...Tn...@5].k.p.
+000039f0: e71a 409c 85ba 0610 61c5 ae41 db6f e9fe  ..@.....a..A.o..
+00003a00: c59e b9ce 37dc f5c7 5d17 f6bd 9521 f6b7  ....7...]....!..
+00003a10: 7448 ad9d cccf 8534 d59b e41e c65f 17b7  tH.....4....._..
+00003a20: c230 a199 0343 f631 76af 6b4a 5a63 f011  .0...C.1v.kJZc..
+00003a30: 24b5 060d 415b 6bd0 1044 b606 ada1 dac2  $...A[k..D......
+00003a40: 4948 b25b 0388 a0bf 3568 0842 5c83 86a8  IH.[....5h.B\...
+00003a50: c880 7d1f 9622 0350 588a 0c40 e12a 3200  ..}..".PX..@.*2.
+00003a60: 88ab c81f f30d 5583 86f0 3155 8386 2801  ......U...1U..(.
+00003a70: 001a a204 7ccc 7756 0d1a 9204 5493 9025  ....|.wV....T..%
+00003a80: 0000 4494 0000 0d51 0200 3444 0900 7c95  ..D....Q..4D..|.
+00003a90: 6349 0000 8525 0100 14ae 0400 80b8 1200  cI...%..........
+00003aa0: 0022 4a00 8086 2801 001a a204 0068 8812  ."J...(......h..
+00003ab0: 00a0 214a c07f ff9f 1b9c 842c 0100 20a2  ..!J.......,.. .
+00003ac0: 0400 6888 1200 a021 4ac0 d1c7 4900 0085  ..h....!J...I...
+00003ad0: 2501 0014 ae04 0080 b812 0000 224a 0080  %..........."J..
+00003ae0: 8628 0100 1aa2 0400 6888 1200 a021 4a00  .(......h....!J.
+00003af0: 8086 2401 d524 6409 0000 1125 0040 4394  ..$..$d....%.@C.
+00003b00: 0000 0d51 028e 3f4e 0200 282c 0900 a070  ...Q..?N..(,...p
+00003b10: 2500 00c4 9500 0010 5102 0034 4409 00d0  %.......Q..4D...
+00003b20: 1025 0040 4394 0000 0d51 0200 3424 09a8  .%.@C....Q..4$..
+00003b30: 2621 4b00 0088 2801 001a a204 0068 8812  &!K...(......h..
+00003b40: 30f8 3809 00a0 b024 0080 c295 0000 1057  0.8....$.......W
+00003b50: 0200 4044 0900 d010 2500 4043 9400 000d  ..@D....%.@C....
+00003b60: 5102 0034 4409 00d0 9024 a09a 842c 0100  Q..4D....$...,..
+00003b70: 20a2 0400 6888 1200 a0ed b79a c467 b003   ...h........g..
+00003b80: e680 0f2c 7731 4f99 c08f 49a3 1c00 4f9b  ...,w1O...I...O.
+00003b90: fa8b cd98 6282 028e b760 50f3 b6d6 c062  ....b....`P....b
+00003ba0: 9c40 bf90 f2c9 815d 09e8 6fc9 9c7a 3c3e  .@.....]..o..z<>
+00003bb0: 0db8 4c0e 45bd 9500 c3ca 13ec 3f2e 9d1b  ..L.E.......?...
+00003bc0: b63c 53f9 eefe c486 40e2 0b6f c5eb 6d49  .<S.....@..o..mI
+00003bd0: 5976 47d3 5637 6f91 f51a 158f 6979 e99d  YvG.V7o.....iy..
+00003be0: 85ec 6c79 52f1 d65b 5e42 5b86 17c7 e364  ..lyR..[^B[....d
+00003bf0: 37f7 b277 abd8 b328 9611 245e 36a2 a96f  7..w...(..$^6..o
+00003c00: d9d4 30b5 039d dda2 581e 264b ee50 6c0c  ..0.....X.&K.Pl.
+00003c10: 64cb 7d8b 5560 ab0e cb4d 8a03 b61a fd82  d.}.U`...M......
+00003c20: c5da 7003 5a64 e24b 063b 5a93 5c42 a8ee  ..p.Zd.K.;Z.\B..
+00003c30: 4d27 a9b7 33f4 d1a8 7eec 49b9 9906 abdb  M'..3...~.I.....
+00003c40: a3e9 f3ad f0ac db97 2c9d d396 78af 2407  ........,...x.$.
+00003c50: e4d5 2e59 107c 23eb 374f 8d8c 769b a6e9  ...Y.|#.7O..v...
+00003c60: cc66 26ad d6ed 9cec aa38 95c6 c810 e051  .f&......8.....Q
+00003c70: 257b d70a 97f1 58bd 8f3b 2b4b bb60 f760  %{....X..;+K.`.`
+00003c80: 8a45 3865 2a9b 6d5b 6746 72fa 78cb 58a6  .E8e*.m[gFr.x.X.
+00003c90: 4793 b187 1198 82eb 4997 9c5f de18 66e1  G.......I.._..f.
+00003ca0: 62cc 0a3b 2596 f643 acd5 29cd f472 738e  b..;%..C..)..rs.
+00003cb0: 8bcd 519a 7bf9 8b4e e7fc a2df 1915 27dc  ..Q.{..N......'.
+00003cc0: fe89 7821 95c7 94de 9088 092b beb2 9d75  ..x!.......+...u
+00003cd0: c1ef b19b fe35 1811 ca32 b734 de3a 8c5d  .....5...2.4.:.]
+00003ce0: b230 7273 9a36 73b2 4ce1 666e f204 6fe6  .0rs.6s.L.fn..o.
+00003cf0: 850b 3b06 ec06 c9cf df4d fc64 13ef ddd8  ..;......M.d....
+00003d00: fd0f 5696 e54f dbe8 3f50 4b03 0414 0000  ..V..O..?PK.....
+00003d10: 0008 00b7 8964 4944 cde5 e6db 0600 00bc  .....dID........
+00003d20: 4400 001a 0000 0077 6f72 642f 7374 796c  D......word/styl
+00003d30: 6573 5769 7468 4566 6665 6374 732e 786d  esWithEffects.xm
+00003d40: 6ce5 9b4b 73e2 3810 c7ef f329 5cbe e494  l..Ks.8....)\...
+00003d50: e195 9040 0d33 95c7 cc24 55f3 c80c c9ee  ...@.3...$U.....
+00003d60: 59c8 02ab 624b 5e49 8464 3efd ca4f 4c0c  Y...bK^I.d>..OL.
+00003d70: b88d 7b73 d913 5856 f7af 25b5 f417 94f4  ..{s..XV..%.....
+00003d80: e1d3 7318 384f 4c69 2ec5 e4a8 f7be 7be4  ..s.8OLi......{.
+00003d90: 3041 a5c7 c562 72f4 70ff e5f8 fcc8 d186  0A...br.p.......
+00003da0: 088f 0452 b0c9 d10b d347 9f3e befb b01a  ...R.....G.>....
+00003db0: 6bf3 1230 ed58 7ba1 c7ab 884e 5cdf 9868  k..0.X{....N\..h
+00003dc0: dce9 68ea b390 e8f7 21a7 4a6a 3937 efa9  ..h.....!.Jj97..
+00003dd0: 0c3b 723e e794 7556 5279 9d7e b7d7 4dbe  .;r>..uVRy.~..M.
+00003de0: 454a 52a6 b585 5d11 f144 b49b b90b 25cc  EJR...]..D....%.
+00003df0: 5b48 68fe b5df ed9e db67 2e0a 1fd5 8864  [Hh......g.....d
+00003e00: c484 7d39 972a 24c6 3eaa 85b5 508f cbe8  ..}9.*$.>...P...
+00003e10: d8fa 8c88 e133 1e70 f312 fb1a 166e 9e26  .....3.p.....n.&
+00003e20: ee52 8971 e6e3 b888 23b6 19db 00c6 4f61  .R.q....#.....Oa
+00003e30: 9057 96fb eaa6 8166 1fb9 8582 0499 9a5c  .W.....f.......\
+00003e40: 4bba 0c99 3049 781d c502 1bb0 14da e7d1  K...0Ix.........
+00003e50: badf 0ef5 665f fab9 93bd 0d2e 3576 15f5  ....f_......5v..
+00003e60: 4eda 0dfa b522 2bfb b176 0809 df4b 8dc2  N...."+..v...K..
+00003e70: 208d 7cbf c75e 1730 22b1 8bc2 0212 c226   .|..^.0"......&
+00003e80: 338f a49c 7cab c3ba a6dc b98b 767d fb55  3...|.......v}.U
+00003e90: c965 b4f6 c6db 79bb 158f 852f bb0c 34f1  .e....y..../..4.
+00003ea0: 958d 51b9 69ba 5d30 539f 4476 0285 747c  ..Q.i.]0S.Dv..t|
+00003eb0: bb10 5291 5960 23b2 3dee c419 e97e 7ce7  ..R.Y`#.=....~|.
+00003ec0: 3876 79f2 24bd 6673 b20c 8c8e 4b92 3275  8vy.$.fs....K.2u
+00003ed0: a7b2 b2b4 282f cc9f d2e7 2f52 18ed acc6  ....(/..../R....
+00003ee0: 4453 ceef 6d7c d67b c82d e8e6 4268 eeda  DS..m|.{.-..Bh..
+00003ef0: 378c 6873 a139 29bf fc9c 95c5 effd b8e2  7.hs.9).........
+00003f00: 564b aa4d a9f8 927b dced 6cd0 f51f 5beb  VK.M...{..l...[.
+00003f10: 8904 13b7 7f52 7975 a577 be0c 8858 e42f  .....Ryu.w...X./
+00003f20: 9938 7e98 96e3 2c15 cd2c 72e2 1275 3cbd  .8~...,..,r..u<.
+00003f30: 587b f8d0 2975 43f6 b0d1 5116 1015 4589  X{..)uC...Q...E.
+00003f40: 595c eb55 1727 5118 bba4 4c53 65b0 15d8  Y\.U.'Q...LSe...
+00003f50: fc9b a48f cc9b 1afb 62e2 76dd b4f0 e1f6  ........b.v.....
+00003f60: 4e71 a9ec 523b 7147 a3ac 70ca 427e c33d  Nq..R;qG..p.B~.=
+00003f70: 8f89 89db cb2b 0a9f 7bec 6f9f 8907 cdbc  .....+..{.o.....
+00003f80: 75f9 af2f c96c cc3c 52b9 14f6 7bff 6ce8  u../.l.<R...{.l.
+00003f90: 16e1 06da fbfc 4c59 142f 91b6 8a20 71a7  ......LY./... q.
+00003fa0: ff88 ad82 d844 9760 898f 255f 8794 16bc  .....D.`..%_....
+00003fb0: 4227 85ff e4dc 5ede 79bb 503e 23b1 863a  B'....^.y.P>#..:
+00003fc0: bd5a da08 91d6 dfea bcb9 9f01 929f 1324  .Z.............$
+00003fd0: 3fa7 487e 8648 7ece 90fc 9c23 f919 b5f4  ?.H~.H~....#....
+00003fe0: 6324 4d33 b5ec 6330 8298 5552 0e66 56c9  c$M3..c0..UR.fV.
+00003ff0: 3098 5925 a160 6695 fc81 9955 d205 6656  0.Y%.`f....U..fV
+00004000: c90e 9859 2519 6066 95b1 af37 a324 79ae  ...Y%.`f...7.$y.
+00004010: 189e 36cb 9a7b 6e02 56bb bef5 3096 d34c  ..6..{n.V...0..L
+00004020: 679c 3ba2 c842 91c8 7762 95ae a0ea dc4c  g.;..B..wb.....L
+00004030: 9733 030b ba87 10f4 d428 19ef 456b 58fd  .3.......(..EkX.
+00004040: 3e02 eb73 18f9 4473 5d4f c318 8efb 78cf  >..s..Ds]O....x.
+00004050: e57c 55dc abe5 9dee d0b7 1ac2 5d40 28f3  .|U.........]@(.
+00004060: 65e0 31e5 dcb3 6773 9093 1fd2 9946 8472  e.1...gs.....F.r
+00004070: c020 608c f737 bef0 8d63 77a7 1e84 38dc  . `..7...cw...8.
+00004080: 3110 20c8 37ae 4d3d 6147 a340 04d0 e00e  1. .7.M=aG.@....
+00004090: 77a4 6e0d e13b f3f8 32cc 7b0a b047 1a0e  w.n..;..2.{..G..
+000040a0: 3038 fd7a ce49 1b4e 3c28 90c6 9cb6 8600  08.z.I.N<(......
+000040b0: 5a32 6c03 8907 1fd2 92b3 d610 404b ce5b  Z2l.........@K.[
+000040c0: 4306 f590 c356 a96b a21e 6173 f1ec b0d9  C....V.k..as....
+000040d0: 7e25 03a9 e6cb 00bc aa9c 1d36 e70b 0eac  ~%.........6....
+000040e0: 3187 4dfb 0202 5a5b ce0e 9bf3 1b8b b073  1.M...Z[.......s
+000040f0: 41a9 fd41 0a49 e5b6 ab71 0354 db65 b901  A..A.I...q.T.e..
+00004100: 0a67 7d6e 00c4 59a8 1b00 1156 ec06 b4c3  .g}n..Y....V....
+00004110: 96ee dfec 89eb 7cc3 dd7c dc75 69df 5b1b  ......|..|.ui.[.
+00004120: e260 4787 34da c9fc 5a4a 53bf 49ee 63fc  .`G.4...ZJS.I.c.
+00004130: 7571 2b0c 139a 3930 e400 63f7 baa1 a40d  uq+...90..c.....
+00004140: 061f 4152 1bd0 10b4 b501 0d41 641b d05a  ..AR.......Ad..Z
+00004150: aa2d 9c84 24bb 0d80 08fa db80 8620 c40d  .-..$........ ..
+00004160: 6888 8a0c d8f7 6129 3200 85a5 c800 14ae  h.....a)2.......
+00004170: 2203 80b8 8afc 36bf a11a d010 7e4c 35a0  ".....6.....~L5.
+00004180: 214a 0080 8628 016f f33b ab01 0d49 02ea  !J...(.o.;...I..
+00004190: 49c8 1200 0022 4a00 8086 2801 001a a204  I...."J...(.....
+000041a0: 007e 9563 4900 0085 2501 0014 ae04 0080  .~.cI...%.......
+000041b0: b812 0000 224a 0080 8628 0100 1aa2 0400  ...."J...(......
+000041c0: 6888 1200 a021 4ac0 7fff 9f1b 9c84 2c01  h....!J.......,.
+000041d0: 0020 a204 0068 8812 00a0 214a c0c9 db49  . ...h....!J...I
+000041e0: 0000 8525 0100 14ae 0400 80b8 1200 0022  ...%..........."
+000041f0: 4a00 8086 2801 001a a204 0068 8812 00a0  J...(......h....
+00004200: 214a 0080 8624 01f5 2464 0900 0011 2500  !J...$..$d....%.
+00004210: 4043 9400 000d 5102 4edf 4e02 0028 2c09  @C....Q.N.N..(,.
+00004220: 00a0 7025 0000 c495 0000 1051 0200 3444  ..p%.......Q..4D
+00004230: 0900 d010 2500 4043 9400 000d 5102 0034  ....%.@C....Q..4
+00004240: 2409 a827 214b 0000 8828 0100 1aa2 0400  $..'!K...(......
+00004250: 6888 1230 7c3b 0900 a0b0 2400 80c2 9500  h..0|;....$.....
+00004260: 0010 5702 0040 4409 00d0 1025 0040 4394  ..W..@D....%.@C.
+00004270: 0000 0d51 0200 3444 0900 d090 24a0 9e84  ...Q..4D....$...
+00004280: 2c01 0020 a204 0068 8812 00a0 1db6 9ac4  ,.. ...h........
+00004290: 67b0 03e6 800f 2cf7 304f 99c0 8f49 a31c  g.....,.0O...I..
+000042a0: 004f 9bfa 9bcd 9962 8202 8eb7 6050 f3b6  .O.....b....`P..
+000042b0: 36c0 629c 40bf 94f2 d181 5d09 18ec c89c  6.b.@.....].....
+000042c0: 663c 3e0b b84c 0e45 bd54 0067 b527 d87f  f<>..L.E.T.g.'..
+000042d0: 5e39 37ac 3853 f9ea fec4 9640 e20b 6fe5  ^97.8S.....@..o.
+000042e0: eb6d 4959 760b da56 372f 91f5 1a95 8f69  .mIYv..V7/.....i
+000042f0: 79e9 9d85 ec6c 7952 f1d6 2b2e a115 e1c5  y....lyR..+.....
+00004300: f138 d9cd bdec dd3a f62c 8a22 82c4 cb56  .8.....:.,."...V
+00004310: 34f5 2d9b 1aa6 f6a0 b35b 14c5 61b2 e40e  4.-......[..a...
+00004320: c5d6 4076 dcb7 5807 b6ee b0dc a43c 60eb  ..@v..X......<`.
+00004330: d12f 596c 0c37 a045 26be 64b0 a735 c925  ./Yl.7.E&.d..5.%
+00004340: 84fa de74 927a 7b43 1f8d 9ac7 9e94 9b59  ...t.z{C.......Y
+00004350: b0be 3d9a 3edf 0acf ba5d 65e9 9cb6 c47b  ..=.>....]e....{
+00004360: 2639 20af 76c5 82e0 3bd9 bc79 6a64 b4df  &9 .v...;..yjd..
+00004370: 344d 6736 3769 b55e f77c 5fc5 9934 4686  4Mg67i.^.|_..4F.
+00004380: 008f 2ad9 bbd6 b88c c7ea 75dc 5959 da05  ..*.......u.YY..
+00004390: fb07 532c c319 53d9 6cdb 3933 92d3 c73b  ..S,..S.l.93...;
+000043a0: c632 3d9a 8c3d 8cc0 14dc 4cba e4fc f2d6  .2=..=....L.....
+000043b0: 304b 1763 d6d8 19b1 b49f 62a3 4e65 a657  0K.c......b.Ne.W
+000043c0: 9b73 5a6e 8ed2 dccb 5f74 bb17 9783 eea8  .sZn...._t......
+000043d0: 3ce1 0e4f c44b a93c a6f4 9644 4c58 f17d  <..O.K.<...DLX.}
+000043e0: ebac 0bfe 4cdc f4af c188 5096 b9a5 f1d6  ....L.....P.....
+000043f0: 61e2 92a5 91db d3b4 9d93 2285 dbb9 c913  a.........".....
+00004400: bc9d 172e ec18 b01b 243f 7fb5 f193 4dbc  ........$?....M.
+00004410: 5763 f73f 5859 8aaf b6d1 ff02 504b 0304  Wc.?XY......PK..
+00004420: 1400 0000 0800 b789 6449 9441 22b8 c606  ........dI.A"...
+00004430: 0000 bb2a 0000 1500 0000 776f 7264 2f74  ...*......word/t
+00004440: 6865 6d65 2f74 6865 6d65 312e 786d 6ced  heme/theme1.xml.
+00004450: 5a4d 6fdb 3618 bef7 5710 bae4 d4fa db75  ZMo.6...W......u
+00004460: 8aba 45ec d8ed d6a6 0d12 b743 8fb4 445b  ..E........C..D[
+00004470: 6c28 5120 e924 be0d ed71 c080 61dd b0c3  l(Q .$...q..a...
+00004480: 0aec b6c3 b0ad 400b ecd2 fd9a 6e1d b60e  ......@.....n...
+00004490: e85f 1829 d98a 2851 72e6 c54d da25 07c7  ._.)..(Qr..M.%..
+000044a0: 22f9 3c7c bf5f 52f0 d5eb 871e 01fb 8871  ".<|._R........q
+000044b0: 4cfd f65a e552 790d 20df a60e f6c7 edb5  L..Z.Ry. .......
+000044c0: 7b83 fec5 d61a e002 fa0e 24d4 47ed b529  {.........$.G..)
+000044d0: e26b d7af 5db8 0aaf 0817 7908 48b8 cfaf  .k..].....y.H...
+000044e0: c0b6 e50a 115c 2995 b82d 8721 bf44 03e4  .....\)..-.!.D..
+000044f0: cbb9 1165 1e14 f291 8d4b 0e83 0792 d623  ...e.....K.....#
+00004500: a56a b9dc 2c79 10fb 16f0 a187 dad6 ddd1  .j..,y..........
+00004510: 08db 080c 14a5 75ed 0200 73fe 1e91 1fbe  ......u...s.....
+00004520: e06a 2c1c b509 dbb5 c39d 9348 2b9a 0f57  .j,........H+..W
+00004530: 387b 95f9 53f8 cca7 bc4b 18d8 87a4 6dc9  8{..S....K....m.
+00004540: fd1d 7a30 4087 c202 0472 2127 da56 39fc  ..z0@....r!'.V9.
+00004550: b34a 3147 4923 9114 442c a24c d0f5 c33f  .J1GI#..D,.L...?
+00004560: 9d2e 4110 4a58 d5e9 d878 18f3 55fa f5f5  ..A.JX...x..U...
+00004570: cb9b 6969 aa9a 3405 f05e afd7 ed55 d2bb  ..ii..4..^...U..
+00004580: 27e1 d0b6 a545 2bf9 14f5 7eab d249 4990  '....E+...~..II.
+00004590: 02c5 3405 9274 cb8d 72dd 4893 95a6 964f  ..4..t..r.H....O
+000045a0: b3de e974 1aeb 269a 5a86 a69e 4fd3 2a37  ...t..&.Z...O.*7
+000045b0: eb1b 5513 4d3d 43d3 28b0 4d67 a3db 6d9a  ..U.M=C.(.Mg..m.
+000045c0: 681a 199a 663e 4dff f27a b36e a469 2668  h...f>M..z.n.i&h
+000045d0: 5c82 fdbd 7c12 15b5 e940 d320 1230 a2e4  \...|....@. .0..
+000045e0: 6631 4b4b b2b4 52d1 afa3 d448 9c76 7122  f1KK..R....H.vq"
+000045f0: 8ea8 2f16 64a2 071f 52d6 97eb b4dd 0914  ../.d...R.......
+00004600: d807 621a a011 b425 ae0b 091e 327c 2441  ..b....%....2|$A
+00004610: b80a c1c4 92d4 9ccd f3e7 9458 80db 0c07  ...........X....
+00004620: a26d 7d1c 4059 628e d6be 7df9 e3db 97cf  .m}.@Yb...}.....
+00004630: c1ab 472f 5e3d fae5 d5e3 c7af 1efd 5c04  ..G/^=........\.
+00004640: bf09 fd71 12fe e6fb 2ffe 7efa 29f8 ebf9  ...q..../.~.)...
+00004650: 776f 9e7c b500 c893 c0df 7ffa ecb7 5fbf  wo.|.........._.
+00004660: 5c80 1049 c4eb af9f fdf1 e2d9 eb6f 3eff  \..I.........o>.
+00004670: f387 2745 b80d 0687 49dc 007b 8883 3be8  ..'E....I..{..;.
+00004680: 00ec 504f 2a5f b425 1ab2 25a1 0317 e224  ..PO*_.%..%....$
+00004690: 74c3 1f73 e843 052e 82f5 84ab c1ee 4c21  t..s.C........L!
+000046a0: 8145 800e d21d 709f c962 5b88 b831 79a8  .E....p..b[..1y.
+000046b0: 29b5 ebb2 8948 c796 86b8 e57a 1a62 8b52  )....H.....z.b.R
+000046c0: d2a1 acd8 00b7 9418 49db 4dfc f102 b9d8  ........I.M.....
+000046d0: 2409 d881 70bf 50ac 6e2a 847a 9340 e61a  $...p.P.n*.z.@..
+000046e0: 2edc a4eb 224d 956d 22a3 0a8e 918f 0450  ...."M.m"......P
+000046f0: 7374 0fa1 22fc 038c 35ff 6c61 9b51 4e47  st.."...5.la.QNG
+00004700: 023c c0a0 0371 b121 0778 28cc e89b d893  .<...q.!.x(.....
+00004710: 8e9e 16ca 2e43 4ab3 e8d6 7dd0 a1a4 70c3  .....CJ...}...p.
+00004720: 4db4 af43 64ba 4252 b809 229a 176e c089  M..Cd.BR.."..n..
+00004730: 805e b156 d023 49c8 6d28 dc42 4576 a7cc  .^.V.#I.m(.BEv..
+00004740: d61c c785 0ca6 3122 14f4 1cc4 7921 f82e  ......1"....y!..
+00004750: 9b6a 2add 92b5 7141 646d 91a9 a743 98c0  .j*...qAdm...C..
+00004760: 7b85 90db 90d2 2464 93ee 755d e805 c57a  {.....$d..u]...z
+00004770: 61df 4d82 3ee2 7b32 5320 d8a6 a258 3eaa  a.M.>.{2S ...X>.
+00004780: e7b0 7a96 8e85 fee2 88ba 8f91 58b2 42dd  ..z.........X.B.
+00004790: c363 d71c 8c6a 66c2 0a73 1551 bd86 4cc9  .c...jf..s.Q..L.
+000047a0: 08a2 c476 aa21 667a 9bea 77d8 3f56 bff3  ...v.!fz..w.?V..
+000047b0: 64bb 4bdb 6c95 fd4e b691 d7df 3efd c03a  d.K.l..N....>..:
+000047c0: dd86 b461 61b2 a7fb db42 40ba ab75 2973  ...aa....B@..u)s
+000047d0: f087 d1d4 36e1 c4df 4632 81cf 7bda 794f  ....6...F2..{.yO
+000047e0: 3bef 6967 a8a7 2dac 4aab ef64 7ad7 8aee  ;.ig..-.J..dz...
+000047f0: 7ff3 bbdd d175 cf5b 74db 1b61 4276 c594  .....u.[t..aBv..
+00004800: a0db 5c6f 805c 9ac6 e9cb d9a3 d168 3ce4  ..\o.\.......h<.
+00004810: 8b2f a281 2bbf 6ada 948c 5889 1c33 180e  ./..+.j...X..3..
+00004820: 0246 c527 58b8 bb2e 0ca4 4c15 2bb5 c398  .F.'X.....L.+...
+00004830: 6bb2 c4a3 20a0 5cde 9f2d 7d2a 5fa8 f4ba  k... .\..-}*_...
+00004840: e8fd 1496 960e 1735 f4f7 473a 1f14 5bd4  .......5..G:..[.
+00004850: 89d6 d5ca e685 a1a2 f37d 53e2 9694 bcb9  .........}S.....
+00004860: 2ad4 d4d6 27a5 46ed f269 a951 8918 4f48  *...'.F..i.Q..OH
+00004870: 8f4a e398 7ae4 f8ed 5fe9 118d a4c2 4c9d  .J..z..._.....L.
+00004880: fae4 994f 9648 294d b31a 6927 b312 12e4  ...O.H)M..i'....
+00004890: a830 4d05 f93c 9ccf 728c 5772 9c1e 11ba  .0M..<..r.Wr....
+000048a0: d041 c759 97b0 7ea5 76b6 a3a8 30a9 97d0  .A.Y..~.v...0...
+000048b0: f7b4 a2ad bc28 dac2 826f a8dd 8ad6 3716  .....(...o....7.
+000048c0: 74e2 8383 b6b5 dea8 362c 60c3 a06d 8de4  t.......6,`..m..
+000048d0: 1d47 7ef5 02b9 1f57 ad11 92b1 dfb6 6cc1  .G~....W......l.
+000048e0: d2d1 6aec 05c7 f791 6efb 7573 a2a7 03ad  ..j.....n.us....
+000048f0: 6c5a 966b f69c ae13 d206 8c8b 4dc8 dd88  lZ.k........M...
+00004900: 385c 95b6 2ef1 0da6 aa36 eaca 25ab b555  8\.......6..%..U
+00004910: 69d5 5ad4 5a95 f755 8be8 c910 e168 3442  i.Z.Z..U.....h4B
+00004920: b630 4679 622a b575 3463 2abb 7422 10db  .0Fyb*.u4c*.t"..
+00004930: 759d 0330 2413 b603 a575 ea51 3a3a 98cb  u..0$....u.Q::..
+00004940: 0359 75fe c064 81a9 cf32 552f f0e6 0296  .Yu..d...2U/....
+00004950: 7eef 6fa8 73e1 4248 0217 ce0a 4e2b bfde  ~.o.s.BH....N+..
+00004960: 4474 d98c 88e5 4f7b c1a0 f2d1 70ca 46ab  Dt....O{....p.F.
+00004970: b25d ed1d da2e a7b2 9cdb eef4 6d37 ab1d  .]..........m7..
+00004980: c847 3527 6308 5b5e 4e18 04aa 38b4 2dca  .G5'c.[^N...8.-.
+00004990: 844b 65bb 0b5c 6cf7 99bc d398 5494 5600  .Ke..\l.....T.V.
+000049a0: b298 2903 0042 fdf0 3f43 fba9 c639 9727  ..)..B..?C...9.'
+000049b0: e2cf 6c4b e455 4cec e031 6058 3661 e132  ..lK.UL..1`X6a.2
+000049c0: 84b6 c5cc deff 6ed7 4ad5 78a0 080b d86c  ......n.J.x....l
+000049d0: 934c 85cc da42 5928 3098 6788 f611 19a8  .L...BY(0.g.....
+000049e0: 62de 546e b280 3b6f 4ed9 baab e173 0236  b.Tn..;oN....s.6
+000049f0: 35ac d7d6 e1b8 ffbf bd12 d6df e5a9 5053  5.............PS
+00004a00: a17e 9287 e07a d155 2a71 105b 3f2d 6d4f  .~...z.U*q.[?-mO
+00004a10: e2cc 9f50 a47a 4cb7 551b 0545 eebf 1ee6  ...P.zL.U..E....
+00004a20: 0328 5ca0 3ee4 790a 339b 202b a3be 3aaf  .(\.>.y.3. +..:.
+00004a30: 0fe8 8ecc 3b10 5f55 80ac 2617 5bb3 d21e  ....;._U..&.[...
+00004a40: 0f0e a58d 5a59 add4 de6a 8bf7 ef22 6a50  ....ZY...j..."jP
+00004a50: c6e8 a2b3 f996 2211 6b39 f7df 6cac 9d84  ......".k9..l...
+00004a60: 222b 88b5 8621 d40c f97d bc48 5363 a67e  "+...!...}.HSc.~
+00004a70: 115e 4ebd c4cb 4835 90f9 6598 3a01 0d1f  .^N...H5..e.:...
+00004a80: 4a09 37d1 084e 48e2 e762 3c90 4389 9ec4  J.7..NH..b<.C...
+00004a90: 836d 564a 3c0f a933 d547 088f 7a59 728c  .mVJ<..3.G..zYr.
+00004aa0: 670e 69c4 df41 2380 9d43 4322 a4a2 61f6  g.i..A#..CC"..a.
+00004ab0: d3a9 ece5 64e7 48b2 d8d0 316b 6d39 d619  ....d.H...1km9..
+00004ac0: 87e1 4019 3357 9763 8e59 7499 e5a9 2a66  ..@.3W.c.Yt...*f
+00004ad0: 0edf 242f 6027 0699 238e 6428 240c 1e9d  ..$/`'..#.d($...
+00004ae0: 4562 2f86 b65f b94f 97b4 d102 9f96 57e6  Eb/.._.O......W.
+00004af0: d325 63f0 847c 2a0e 97f0 69ec c5f0 fc9f  .%c..|*...i.....
+00004b00: c95e a5e3 a160 b03b ffe1 992c 0972 8f38  .^...`.;...,.r.8
+00004b10: fdaf 5df8 0750 4b03 0414 0000 0008 00b7  ..]..PK.........
+00004b20: 8964 49e8 5ae5 5300 0100 00b6 0100 0014  .dI.Z.S.........
+00004b30: 0000 0077 6f72 642f 7765 6253 6574 7469  ...word/webSetti
+00004b40: 6e67 732e 786d 6c8d d0c1 6ac3 300c 00d0  ngs.xml...j.0...
+00004b50: 7bbe c2e4 9253 e364 8c31 4292 3218 1dbb  {....S.d.1B.2...
+00004b60: 9441 b60f 701c 2531 b52d 63b9 cdfa f733  .A..p.%1.-c....3
+00004b70: 5936 18bb f426 21e9 21a9 de7f 1acd 2ee0  Y6...&!.!.......
+00004b80: 49a1 6db2 322f 3206 56e2 a0ec d464 1fef  I.m.2/2.V....d..
+00004b90: 87dd 63c6 2808 3b08 8d16 9aec 0a94 eddb  ..c.(.;.........
+00004ba0: a45e aa05 fa0e 4288 8dc4 2262 a932 b249  .^....B..."b.2.I
+00004bb0: e710 5cc5 39c9 198c a01c 1dd8 581c d11b  ..\.9.......X...
+00004bc0: 1162 ea27 6e84 3f9d dd4e a271 22a8 5e69  .b.'n.?..N.q".^i
+00004bd0: 15ae fcae 281e d28d f1b7 2838 8e4a c233  ....(.....(8.J.3
+00004be0: cab3 011b d679 ee41 4711 2dcd cad1 8fb6  .....y.AG.-.....
+00004bf0: dca2 2de8 07e7 5102 51bc c7e8 6fcf 0865  ..-...Q.Q...o..e
+00004c00: 7f99 f2fe 1f64 94f4 4838 863c 1eb3 6db4  .....d..H8.<..m.
+00004c10: 5271 bc2c d6c8 e894 1959 bd4e 16bd e835  Rq.,.....Y.N...5
+00004c20: 3469 84d2 3661 2c7e 5068 8dcb dbf1 856f  4i..6a,~Ph.....o
+00004c30: f980 470c 9db8 c013 7571 0d0d 07a5 2116  ..G.....uq....!.
+00004c40: 6bfe e7db 6df2 0550 4b01 0214 0314 0000  k...m..PK.......
+00004c50: 0008 00b7 8964 4929 14c7 0a78 0100 00e7  .....dI)...x....
+00004c60: 0500 0013 0000 0000 0000 0000 0000 0080  ................
+00004c70: 0100 0000 005b 436f 6e74 656e 745f 5479  .....[Content_Ty
+00004c80: 7065 735d 2e78 6d6c 504b 0102 1403 1400  pes].xmlPK......
+00004c90: 0000 0800 b789 6449 0eee ab75 fd00 0000  ......dI...u....
+00004ca0: ec02 0000 0b00 0000 0000 0000 0000 0000  ................
+00004cb0: 8001 a901 0000 5f72 656c 732f 2e72 656c  ......_rels/.rel
+00004cc0: 7350 4b01 0214 0314 0000 0008 00b7 8964  sPK............d
+00004cd0: 4970 5a4d 798f 0100 000e 0300 0010 0000  IpZMy...........
+00004ce0: 0000 0000 0000 0000 0080 01cf 0200 0064  ...............d
+00004cf0: 6f63 5072 6f70 732f 6170 702e 786d 6c50  ocProps/app.xmlP
+00004d00: 4b01 0214 0314 0000 0008 00b7 8964 4923  K............dI#
+00004d10: 83c6 e876 0100 00d9 0200 0011 0000 0000  ...v............
+00004d20: 0000 0000 0000 0080 018c 0400 0064 6f63  .............doc
+00004d30: 5072 6f70 732f 636f 7265 2e78 6d6c 504b  Props/core.xmlPK
+00004d40: 0102 1403 1400 0000 0800 b789 6449 4c78  ............dILx
+00004d50: 496a c321 0000 e844 0000 1700 0000 0000  Ij.!...D........
+00004d60: 0000 0000 0000 8001 3106 0000 646f 6350  ........1...docP
+00004d70: 726f 7073 2f74 6875 6d62 6e61 696c 2e6a  rops/thumbnail.j
+00004d80: 7065 6750 4b01 0214 0314 0000 0008 00b7  pegPK...........
+00004d90: 8964 4915 594c cc14 0100 00cc 0300 001c  .dI.YL..........
+00004da0: 0000 0000 0000 0000 0000 0080 0129 2800  .............)(.
+00004db0: 0077 6f72 642f 5f72 656c 732f 646f 6375  .word/_rels/docu
+00004dc0: 6d65 6e74 2e78 6d6c 2e72 656c 7350 4b01  ment.xml.relsPK.
+00004dd0: 021e 0314 0000 0008 0091 819b 58ba 6b84  ............X.k.
+00004de0: 6e80 0600 004e 3e00 0011 0018 0000 0000  n....N>.........
+00004df0: 0001 0000 00a4 8177 2900 0077 6f72 642f  .......w)..word/
+00004e00: 646f 6375 6d65 6e74 2e78 6d6c 5554 0500  document.xmlUT..
+00004e10: 0362 862d 6675 780b 0001 04f5 0100 0004  .b.-fux.........
+00004e20: 1400 0000 504b 0102 1403 1400 0000 0800  ....PK..........
+00004e30: b789 6449 1bee db03 2202 0000 ac08 0000  ..dI....".......
+00004e40: 1200 0000 0000 0000 0000 0000 8001 4230  ..............B0
+00004e50: 0000 776f 7264 2f66 6f6e 7454 6162 6c65  ..word/fontTable
+00004e60: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
+00004e70: b789 6449 7564 3289 c103 0000 320a 0000  ..dIud2.....2...
+00004e80: 1100 0000 0000 0000 0000 0000 8001 9432  ...............2
+00004e90: 0000 776f 7264 2f73 6574 7469 6e67 732e  ..word/settings.
+00004ea0: 786d 6c50 4b01 0214 0314 0000 0008 00b7  xmlPK...........
+00004eb0: 8964 4900 e7c1 3558 0600 005a 4100 000f  .dI...5X...ZA...
+00004ec0: 0000 0000 0000 0000 0000 0080 0184 3600  ..............6.
+00004ed0: 0077 6f72 642f 7374 796c 6573 2e78 6d6c  .word/styles.xml
+00004ee0: 504b 0102 1403 1400 0000 0800 b789 6449  PK............dI
+00004ef0: 44cd e5e6 db06 0000 bc44 0000 1a00 0000  D........D......
+00004f00: 0000 0000 0000 0000 8001 093d 0000 776f  ...........=..wo
+00004f10: 7264 2f73 7479 6c65 7357 6974 6845 6666  rd/stylesWithEff
+00004f20: 6563 7473 2e78 6d6c 504b 0102 1403 1400  ects.xmlPK......
+00004f30: 0000 0800 b789 6449 9441 22b8 c606 0000  ......dI.A".....
+00004f40: bb2a 0000 1500 0000 0000 0000 0000 0000  .*..............
+00004f50: 8001 1c44 0000 776f 7264 2f74 6865 6d65  ...D..word/theme
+00004f60: 2f74 6865 6d65 312e 786d 6c50 4b01 0214  /theme1.xmlPK...
+00004f70: 0314 0000 0008 00b7 8964 49e8 5ae5 5300  .........dI.Z.S.
+00004f80: 0100 00b6 0100 0014 0000 0000 0000 0000  ................
+00004f90: 0000 0080 0115 4b00 0077 6f72 642f 7765  ......K..word/we
+00004fa0: 6253 6574 7469 6e67 732e 786d 6c50 4b05  bSettings.xmlPK.
+00004fb0: 0600 0000 000d 000d 0066 0300 0047 4c00  .........f...GL.
+00004fc0: 0000 00                                  ...
```

### Comparing `python-docx-1.1.0/features/steps/test_files/test.png` & `python_docx-1.1.1/features/steps/test_files/test.png`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/txt-font-highlight-color.docx` & `python_docx-1.1.1/features/steps/test_files/txt-font-highlight-color.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/test_files/txt-font-props.docx` & `python_docx-1.1.1/features/steps/test_files/txt-font-props.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/steps/text.py` & `python_docx-1.1.1/features/steps/text.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/sty-access-latent-styles.feature` & `python_docx-1.1.1/features/sty-access-latent-styles.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/sty-add-style.feature` & `python_docx-1.1.1/features/sty-add-style.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/sty-latent-add-del.feature` & `python_docx-1.1.1/features/sty-latent-add-del.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/sty-latent-props.feature` & `python_docx-1.1.1/features/sty-latent-props.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/sty-style-props.feature` & `python_docx-1.1.1/features/sty-style-props.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/tab-access-tabs.feature` & `python_docx-1.1.1/features/tab-access-tabs.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/tab-tabstop-props.feature` & `python_docx-1.1.1/features/tab-tabstop-props.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/tbl-add-row-or-col.feature` & `python_docx-1.1.1/features/tbl-add-row-or-col.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/tbl-cell-access.feature` & `python_docx-1.1.1/features/tbl-cell-access.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/tbl-cell-props.feature` & `python_docx-1.1.1/features/tbl-cell-props.feature`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 Feature: Get and set table cell properties
   In order to format a table cell to my requirements
   As a developer using python-docx
   I need a way to get and set the properties of a table cell
 
 
+  Scenario Outline: Get _Cell.grid_span
+    Given a _Cell object spanning <count> layout-grid cells
+     Then cell.grid_span is <count>
+
+    Examples: Cell.grid_span value cases
+      | count |
+      | 1     |
+      | 2     |
+      | 4     |
+
+
   Scenario Outline: Get _Cell.vertical_alignment
     Given a _Cell object with <state> vertical alignment as cell
      Then cell.vertical_alignment is <value>
 
     Examples: Cell.vertical_alignment value cases
       | state     | value                    |
       | inherited | None                     |
```

### Comparing `python-docx-1.1.0/features/tbl-col-props.feature` & `python_docx-1.1.1/features/tbl-col-props.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/tbl-item-access.feature` & `python_docx-1.1.1/features/tbl-item-access.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/tbl-merge-cells.feature` & `python_docx-1.1.1/features/tbl-merge-cells.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/tbl-props.feature` & `python_docx-1.1.1/features/tbl-props.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/tbl-style.feature` & `python_docx-1.1.1/features/tbl-style.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/txt-add-break.feature` & `python_docx-1.1.1/features/txt-add-break.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/txt-font-color.feature` & `python_docx-1.1.1/features/txt-font-color.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/txt-font-props.feature` & `python_docx-1.1.1/features/txt-font-props.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/features/txt-parfmt-props.feature` & `python_docx-1.1.1/features/txt-parfmt-props.feature`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/pyproject.toml` & `python_docx-1.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Office/Business :: Office Suites",
     "Topic :: Software Development :: Libraries",
 ]
 dependencies = [
-    "lxml>=3.1.0",
-    "typing_extensions",
+    "lxml>=3.1.0,<=4.9.2",
+    "typing_extensions>=4.9.0",
 ]
 description = "Create, read, and update Microsoft Word .docx files."
 dynamic = ["version"]
 keywords = ["docx", "office", "openxml", "word"]
 license = { text = "MIT" }
 readme = "README.md"
 requires-python = ">=3.7"
@@ -35,14 +35,15 @@
 [project.urls]
 Changelog = "https://github.com/python-openxml/python-docx/blob/master/HISTORY.rst"
 Documentation = "https://python-docx.readthedocs.org/en/latest/"
 Homepage = "https://github.com/python-openxml/python-docx"
 Repository = "https://github.com/python-openxml/python-docx"
 
 [tool.black]
+line-length = 100
 target-version = ["py37", "py38", "py39", "py310", "py311"]
 
 [tool.pytest.ini_options]
 filterwarnings = [
     # -- exit on any warning not explicitly ignored here --
     "error",
 
@@ -65,14 +66,18 @@
 ]
 python_files = ["test_*.py"]
 python_classes = ["Test", "Describe"]
 python_functions = ["it_", "its_", "they_", "and_", "but_"]
 
 [tool.ruff]
 exclude = []
+line-length = 100
+target-version = "py38"
+
+[tool.ruff.lint]
 ignore = [
     "COM812",   # -- over-aggressively insists on trailing commas where not desired --
     "PT001",    # -- wants @pytest.fixture() instead of @pytest.fixture --
     "PT005",    # -- wants @pytest.fixture() instead of @pytest.fixture --
 ]
 select = [
     "C4",       # -- flake8-comprehensions --
@@ -84,15 +89,14 @@
     "PT",       # -- flake8-pytest-style --
     "SIM",      # -- flake8-simplify --
     "UP015",    # -- redundant `open()` mode parameter (like "r" is default) --
     "UP018",    # -- Unnecessary {literal_type} call like `str("abc")`. (rewrite as a literal) --
     "UP032",    # -- Use f-string instead of `.format()` call --
     "UP034",    # -- Avoid extraneous parentheses --
 ]
-target-version = "py37"
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["docx"]
 known-local-folder = ["helpers"]
 
 [tool.setuptools.dynamic]
 version = {attr = "docx.__version__"}
```

### Comparing `python-docx-1.1.0/src/docx/__init__.py` & `python_docx-1.1.1/src/docx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import TYPE_CHECKING, Type
 
 from docx.api import Document
 
 if TYPE_CHECKING:
     from docx.opc.part import Part
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 
 __all__ = ["Document"]
 
 
 # -- register custom Part classes with opc package reader --
```

### Comparing `python-docx-1.1.0/src/docx/api.py` & `python_docx-1.1.1/src/docx/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,29 +2,33 @@
 
 Provides a syntactically more convenient API for interacting with the OpcPackage graph.
 """
 
 from __future__ import annotations
 
 import os
-from typing import IO
+from typing import IO, TYPE_CHECKING, cast
 
 from docx.opc.constants import CONTENT_TYPE as CT
 from docx.package import Package
 
+if TYPE_CHECKING:
+    from docx.document import Document as DocumentObject
+    from docx.parts.document import DocumentPart
 
-def Document(docx: str | IO[bytes] | None = None):
+
+def Document(docx: str | IO[bytes] | None = None) -> DocumentObject:
     """Return a |Document| object loaded from `docx`, where `docx` can be either a path
     to a ``.docx`` file (a string) or a file-like object.
 
     If `docx` is missing or ``None``, the built-in default document "template" is
     loaded.
     """
     docx = _default_docx_path() if docx is None else docx
-    document_part = Package.open(docx).main_document_part
+    document_part = cast("DocumentPart", Package.open(docx).main_document_part)
     if document_part.content_type != CT.WML_DOCUMENT_MAIN:
         tmpl = "file '%s' is not a Word file, content type is '%s'"
         raise ValueError(tmpl % (docx, document_part.content_type))
     return document_part.document
 
 
 def _default_docx_path():
```

### Comparing `python-docx-1.1.0/src/docx/blkcntnr.py` & `python_docx-1.1.1/src/docx/blkcntnr.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from docx.oxml.table import CT_Tbl
 from docx.oxml.text.paragraph import CT_P
 from docx.shared import StoryChild
 from docx.text.paragraph import Paragraph
 
 if TYPE_CHECKING:
-    from docx import types as t
+    import docx.types as t
     from docx.oxml.document import CT_Body
     from docx.oxml.section import CT_HdrFtr
     from docx.oxml.table import CT_Tc
     from docx.shared import Length
     from docx.styles.style import ParagraphStyle
     from docx.table import Table
 
@@ -37,17 +37,15 @@
     paragraph or table.
     """
 
     def __init__(self, element: BlockItemElement, parent: t.ProvidesStoryPart):
         super(BlockItemContainer, self).__init__(parent)
         self._element = element
 
-    def add_paragraph(
-        self, text: str = "", style: str | ParagraphStyle | None = None
-    ) -> Paragraph:
+    def add_paragraph(self, text: str = "", style: str | ParagraphStyle | None = None) -> Paragraph:
         """Return paragraph newly added to the end of the content in this container.
 
         The paragraph has `text` in a single run if present, and is given paragraph
         style `style`.
 
         If `style` is |None|, no paragraph style is applied, which has the same effect
         as applying the 'Normal' style.
@@ -73,19 +71,15 @@
         return Table(tbl, self)
 
     def iter_inner_content(self) -> Iterator[Paragraph | Table]:
         """Generate each `Paragraph` or `Table` in this container in document order."""
         from docx.table import Table
 
         for element in self._element.inner_content_elements:
-            yield (
-                Paragraph(element, self)
-                if isinstance(element, CT_P)
-                else Table(element, self)
-            )
+            yield (Paragraph(element, self) if isinstance(element, CT_P) else Table(element, self))
 
     @property
     def paragraphs(self):
         """A list containing the paragraphs in this container, in document order.
 
         Read-only.
         """
```

### Comparing `python-docx-1.1.0/src/docx/dml/color.py` & `python_docx-1.1.1/src/docx/dml/color.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/document.py` & `python_docx-1.1.1/src/docx/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from docx.blkcntnr import BlockItemContainer
 from docx.enum.section import WD_SECTION
 from docx.enum.text import WD_BREAK
 from docx.section import Section, Sections
 from docx.shared import ElementProxy, Emu
 
 if TYPE_CHECKING:
-    from docx import types as t
+    import docx.types as t
     from docx.oxml.document import CT_Body, CT_Document
     from docx.parts.document import DocumentPart
     from docx.settings import Settings
     from docx.shared import Length
     from docx.styles.style import ParagraphStyle, _TableStyle
     from docx.table import Table
     from docx.text.paragraph import Paragraph
@@ -52,17 +52,15 @@
 
     def add_page_break(self):
         """Return newly |Paragraph| object containing only a page break."""
         paragraph = self.add_paragraph()
         paragraph.add_run().add_break(WD_BREAK.PAGE)
         return paragraph
 
-    def add_paragraph(
-        self, text: str = "", style: str | ParagraphStyle | None = None
-    ) -> Paragraph:
+    def add_paragraph(self, text: str = "", style: str | ParagraphStyle | None = None) -> Paragraph:
         """Return paragraph newly added to the end of the document.
 
         The paragraph is populated with `text` and having paragraph style `style`.
 
         `text` can contain tab (``\\t``) characters, which are converted to the
         appropriate XML form for a tab. `text` can also include newline (``\\n``) or
         carriage return (``\\r``) characters, each of which is converted to a line
```

### Comparing `python-docx-1.1.0/src/docx/enum/base.py` & `python_docx-1.1.1/src/docx/enum/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Base classes and other objects used by enumerations."""
 
 from __future__ import annotations
 
 import enum
 import textwrap
-from typing import Any, Dict, Type, TypeVar
+from typing import TYPE_CHECKING, Any, Dict, Type, TypeVar
 
-from typing_extensions import Self
+if TYPE_CHECKING:
+    from typing_extensions import Self
 
 _T = TypeVar("_T", bound="BaseXmlEnum")
 
 
 class BaseEnum(int, enum.Enum):
     """Base class for Enums that do not map XML attr values.
 
@@ -65,15 +66,15 @@
         return member
 
     @classmethod
     def to_xml(cls: Type[_T], value: int | _T | None) -> str | None:
         """XML value of this enum member, generally an XML attribute value."""
         # -- presence of multi-arg `__new__()` method fools type-checker, but getting a
         # -- member by its value using EnumCls(val) works as usual.
-        return cls(value).xml_value  # pyright: ignore[reportGeneralTypeIssues]
+        return cls(value).xml_value
 
 
 class DocsPageFormatter:
     """Generate an .rst doc page for an enumeration.
 
     Formats a RestructuredText documention page (string) for the enumeration class parts
     passed to the constructor. An immutable one-shot service object.
@@ -125,17 +126,15 @@
         return "%s\n%s\n" % (member.name, member_docstring)
 
     @property
     def _member_defs(self):
         """A single string containing the aggregated member definitions section of the
         documentation page."""
         members = self._clsdict["__members__"]
-        member_defs = [
-            self._member_def(member) for member in members if member.name is not None
-        ]
+        member_defs = [self._member_def(member) for member in members if member.name is not None]
         return "\n".join(member_defs)
 
     @property
     def _ms_name(self):
         """The Microsoft API name for this enumeration."""
         return self._clsdict["__ms_name__"]
```

### Comparing `python-docx-1.1.0/src/docx/enum/dml.py` & `python_docx-1.1.1/src/docx/enum/dml.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/enum/section.py` & `python_docx-1.1.1/src/docx/enum/section.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/enum/style.py` & `python_docx-1.1.1/src/docx/enum/style.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/enum/table.py` & `python_docx-1.1.1/src/docx/enum/table.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/enum/text.py` & `python_docx-1.1.1/src/docx/enum/text.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/image/__init__.py` & `python_docx-1.1.1/src/docx/image/__init__.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/image/bmp.py` & `python_docx-1.1.1/src/docx/image/bmp.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/image/constants.py` & `python_docx-1.1.1/src/docx/image/constants.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/image/gif.py` & `python_docx-1.1.1/src/docx/image/gif.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/image/helpers.py` & `python_docx-1.1.1/src/docx/image/helpers.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/image/image.py` & `python_docx-1.1.1/src/docx/image/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 from __future__ import annotations
 
 import hashlib
 import io
 import os
 from typing import IO, Tuple
 
-from typing_extensions import Self
-
 from docx.image.exceptions import UnrecognizedImageError
 from docx.shared import Emu, Inches, Length, lazyproperty
 
 
 class Image:
     """Graphical image stream such as JPEG, PNG, or GIF with properties and methods
     required by ImagePart."""
@@ -24,22 +22,22 @@
     def __init__(self, blob: bytes, filename: str, image_header: BaseImageHeader):
         super(Image, self).__init__()
         self._blob = blob
         self._filename = filename
         self._image_header = image_header
 
     @classmethod
-    def from_blob(cls, blob: bytes) -> Self:
+    def from_blob(cls, blob: bytes) -> Image:
         """Return a new |Image| subclass instance parsed from the image binary contained
         in `blob`."""
         stream = io.BytesIO(blob)
         return cls._from_stream(stream, blob)
 
     @classmethod
-    def from_file(cls, image_descriptor):
+    def from_file(cls, image_descriptor: str | IO[bytes]):
         """Return a new |Image| subclass instance loaded from the image file identified
         by `image_descriptor`, a path or file-like object."""
         if isinstance(image_descriptor, str):
             path = image_descriptor
             with open(path, "rb") as f:
                 blob = f.read()
                 stream = io.BytesIO(blob)
@@ -53,15 +51,15 @@
 
     @property
     def blob(self):
         """The bytes of the image 'file'."""
         return self._blob
 
     @property
-    def content_type(self):
+    def content_type(self) -> str:
         """MIME content type for this image, e.g. ``'image/jpeg'`` for a JPEG image."""
         return self._image_header.content_type
 
     @lazyproperty
     def ext(self):
         """The file extension for the image.
 
@@ -163,20 +161,19 @@
         image in `stream`."""
         image_header = _ImageHeaderFactory(stream)
         if filename is None:
             filename = "image.%s" % image_header.default_ext
         return cls(blob, filename, image_header)
 
 
-def _ImageHeaderFactory(stream):
-    """Return a |BaseImageHeader| subclass instance that knows how to parse the headers
-    of the image in `stream`."""
+def _ImageHeaderFactory(stream: IO[bytes]):
+    """A |BaseImageHeader| subclass instance that can parse headers of image in `stream`."""
     from docx.image import SIGNATURES
 
-    def read_32(stream):
+    def read_32(stream: IO[bytes]):
         stream.seek(0)
         return stream.read(32)
 
     header = read_32(stream)
     for cls, offset, signature_bytes in SIGNATURES:
         end = offset + len(signature_bytes)
         found_bytes = header[offset:end]
@@ -184,40 +181,35 @@
             return cls.from_stream(stream)
     raise UnrecognizedImageError
 
 
 class BaseImageHeader:
     """Base class for image header subclasses like |Jpeg| and |Tiff|."""
 
-    def __init__(self, px_width, px_height, horz_dpi, vert_dpi):
+    def __init__(self, px_width: int, px_height: int, horz_dpi: int, vert_dpi: int):
         self._px_width = px_width
         self._px_height = px_height
         self._horz_dpi = horz_dpi
         self._vert_dpi = vert_dpi
 
     @property
-    def content_type(self):
+    def content_type(self) -> str:
         """Abstract property definition, must be implemented by all subclasses."""
-        msg = (
-            "content_type property must be implemented by all subclasses of "
-            "BaseImageHeader"
-        )
+        msg = "content_type property must be implemented by all subclasses of " "BaseImageHeader"
         raise NotImplementedError(msg)
 
     @property
-    def default_ext(self):
+    def default_ext(self) -> str:
         """Default filename extension for images of this type.
 
         An abstract property definition, must be implemented by all subclasses.
         """
-        msg = (
-            "default_ext property must be implemented by all subclasses of "
-            "BaseImageHeader"
+        raise NotImplementedError(
+            "default_ext property must be implemented by all subclasses of " "BaseImageHeader"
         )
-        raise NotImplementedError(msg)
 
     @property
     def px_width(self):
         """The horizontal pixel dimension of the image."""
         return self._px_width
 
     @property
```

### Comparing `python-docx-1.1.0/src/docx/image/jpeg.py` & `python_docx-1.1.1/src/docx/image/jpeg.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/image/png.py` & `python_docx-1.1.1/src/docx/image/png.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/image/tiff.py` & `python_docx-1.1.1/src/docx/image/tiff.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,19 +94,15 @@
         """
         ifd_entries = self._ifd_entries
 
         if resolution_tag not in ifd_entries:
             return 72
 
         # resolution unit defaults to inches (2)
-        resolution_unit = (
-            ifd_entries[TIFF_TAG.RESOLUTION_UNIT]
-            if TIFF_TAG.RESOLUTION_UNIT in ifd_entries
-            else 2
-        )
+        resolution_unit = ifd_entries.get(TIFF_TAG.RESOLUTION_UNIT, 2)
 
         if resolution_unit == 1:  # aspect ratio only
             return 72
         # resolution_unit == 2 for inches, 3 for centimeters
         units_per_inch = 1 if resolution_unit == 2 else 2.54
         dots_per_unit = ifd_entries[resolution_tag]
         return int(round(dots_per_unit * units_per_inch))
```

### Comparing `python-docx-1.1.0/src/docx/opc/constants.py` & `python_docx-1.1.1/src/docx/opc/constants.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/opc/coreprops.py` & `python_docx-1.1.1/src/docx/opc/coreprops.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/opc/oxml.py` & `python_docx-1.1.1/src/docx/opc/oxml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pyright: reportPrivateUsage=false
+
 """Temporary stand-in for main oxml module.
 
 This module came across with the PackageReader transplant. Probably much will get
 replaced with objects from the pptx.oxml.core and then this module will either get
 deleted or only hold the package related custom element classes.
 """
 
@@ -23,15 +25,15 @@
 
 
 # ===========================================================================
 # functions
 # ===========================================================================
 
 
-def parse_xml(text: str) -> etree._Element:  # pyright: ignore[reportPrivateUsage]
+def parse_xml(text: str) -> etree._Element:
     """`etree.fromstring()` replacement that uses oxml parser."""
     return etree.fromstring(text, oxml_parser)
 
 
 def qn(tag):
     """Stands for "qualified name", a utility function to turn a namespace prefixed tag
     name into a Clark-notation qualified tag name for lxml.
@@ -40,15 +42,15 @@
     example, ``qn('p:cSld')`` returns ``'{http://schemas.../main}cSld'``.
     """
     prefix, tagroot = tag.split(":")
     uri = nsmap[prefix]
     return "{%s}%s" % (uri, tagroot)
 
 
-def serialize_part_xml(part_elm):
+def serialize_part_xml(part_elm: etree._Element):
     """Serialize `part_elm` etree element to XML suitable for storage as an XML part.
 
     That is to say, no insignificant whitespace added for readability, and an
     appropriate XML declaration added with UTF-8 encoding specified.
     """
     return etree.tostring(part_elm, encoding="UTF-8", standalone=True)
```

### Comparing `python-docx-1.1.0/src/docx/opc/package.py` & `python_docx-1.1.1/src/docx/opc/part.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,208 +1,233 @@
-"""Objects that implement reading and writing OPC packages."""
+"""Open Packaging Convention (OPC) objects related to package parts."""
 
-from docx.opc.constants import RELATIONSHIP_TYPE as RT
-from docx.opc.packuri import PACKAGE_URI, PackURI
-from docx.opc.part import PartFactory
-from docx.opc.parts.coreprops import CorePropertiesPart
-from docx.opc.pkgreader import PackageReader
-from docx.opc.pkgwriter import PackageWriter
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Callable, Dict, Type
+
+from docx.opc.oxml import serialize_part_xml
+from docx.opc.packuri import PackURI
 from docx.opc.rel import Relationships
-from docx.opc.shared import lazyproperty
+from docx.opc.shared import cls_method_fn
+from docx.oxml.parser import parse_xml
+from docx.shared import lazyproperty
+
+if TYPE_CHECKING:
+    from docx.package import Package
 
 
-class OpcPackage:
-    """Main API class for |python-opc|.
+class Part:
+    """Base class for package parts.
 
-    A new instance is constructed by calling the :meth:`open` class method with a path
-    to a package file or file-like object containing one.
+    Provides common properties and methods, but intended to be subclassed in client code
+    to implement specific part behaviors.
     """
 
-    def __init__(self):
-        super(OpcPackage, self).__init__()
+    def __init__(
+        self,
+        partname: str,
+        content_type: str,
+        blob: bytes | None = None,
+        package: Package | None = None,
+    ):
+        super(Part, self).__init__()
+        self._partname = partname
+        self._content_type = content_type
+        self._blob = blob
+        self._package = package
 
     def after_unmarshal(self):
-        """Entry point for any post-unmarshaling processing.
+        """Entry point for post-unmarshaling processing, for example to parse the part
+        XML.
+
+        May be overridden by subclasses without forwarding call to super.
+        """
+        # don't place any code here, just catch call if not overridden by
+        # subclass
+        pass
+
+    def before_marshal(self):
+        """Entry point for pre-serialization processing, for example to finalize part
+        naming if necessary.
 
         May be overridden by subclasses without forwarding call to super.
         """
         # don't place any code here, just catch call if not overridden by
         # subclass
         pass
 
     @property
-    def core_properties(self):
-        """|CoreProperties| object providing read/write access to the Dublin Core
-        properties for this document."""
-        return self._core_properties_part.core_properties
-
-    def iter_rels(self):
-        """Generate exactly one reference to each relationship in the package by
-        performing a depth-first traversal of the rels graph."""
-
-        def walk_rels(source, visited=None):
-            visited = [] if visited is None else visited
-            for rel in source.rels.values():
-                yield rel
-                if rel.is_external:
-                    continue
-                part = rel.target_part
-                if part in visited:
-                    continue
-                visited.append(part)
-                new_source = part
-                for rel in walk_rels(new_source, visited):
-                    yield rel
-
-        for rel in walk_rels(self):
-            yield rel
-
-    def iter_parts(self):
-        """Generate exactly one reference to each of the parts in the package by
-        performing a depth-first traversal of the rels graph."""
-
-        def walk_parts(source, visited=[]):
-            for rel in source.rels.values():
-                if rel.is_external:
-                    continue
-                part = rel.target_part
-                if part in visited:
-                    continue
-                visited.append(part)
-                yield part
-                new_source = part
-                for part in walk_parts(new_source, visited):
-                    yield part
-
-        for part in walk_parts(self):
-            yield part
-
-    def load_rel(self, reltype, target, rId, is_external=False):
-        """Return newly added |_Relationship| instance of `reltype` between this part
-        and `target` with key `rId`.
+    def blob(self):
+        """Contents of this package part as a sequence of bytes.
 
-        Target mode is set to ``RTM.EXTERNAL`` if `is_external` is |True|. Intended for
-        use during load from a serialized package, where the rId is well known. Other
-        methods exist for adding a new relationship to the package during processing.
+        May be text or binary. Intended to be overridden by subclasses. Default behavior
+        is to return load blob.
         """
-        return self.rels.add_relationship(reltype, target, rId, is_external)
+        return self._blob
 
     @property
-    def main_document_part(self):
-        """Return a reference to the main document part for this package.
+    def content_type(self):
+        """Content type of this part."""
+        return self._content_type
+
+    def drop_rel(self, rId: str):
+        """Remove the relationship identified by `rId` if its reference count is less
+        than 2.
 
-        Examples include a document part for a WordprocessingML package, a presentation
-        part for a PresentationML package, or a workbook part for a SpreadsheetML
-        package.
-        """
-        return self.part_related_by(RT.OFFICE_DOCUMENT)
-
-    def next_partname(self, template):
-        """Return a |PackURI| instance representing partname matching `template`.
-
-        The returned part-name has the next available numeric suffix to distinguish it
-        from other parts of its type. `template` is a printf (%)-style template string
-        containing a single replacement item, a '%d' to be used to insert the integer
-        portion of the partname. Example: "/word/header%d.xml"
-        """
-        partnames = {part.partname for part in self.iter_parts()}
-        for n in range(1, len(partnames) + 2):
-            candidate_partname = template % n
-            if candidate_partname not in partnames:
-                return PackURI(candidate_partname)
+        Relationships with a reference count of 0 are implicit relationships.
+        """
+        if self._rel_ref_count(rId) < 2:
+            del self.rels[rId]
 
     @classmethod
-    def open(cls, pkg_file):
-        """Return an |OpcPackage| instance loaded with the contents of `pkg_file`."""
-        pkg_reader = PackageReader.from_file(pkg_file)
-        package = cls()
-        Unmarshaller.unmarshal(pkg_reader, package, PartFactory)
-        return package
+    def load(cls, partname: str, content_type: str, blob: bytes, package: Package):
+        return cls(partname, content_type, blob, package)
+
+    def load_rel(self, reltype: str, target: Part | str, rId: str, is_external: bool = False):
+        """Return newly added |_Relationship| instance of `reltype`.
+
+        The new relationship relates the `target` part to this part with key `rId`.
+
+        Target mode is set to ``RTM.EXTERNAL`` if `is_external` is |True|. Intended for
+        use during load from a serialized package, where the rId is well-known. Other
+        methods exist for adding a new relationship to a part when manipulating a part.
+        """
+        return self.rels.add_relationship(reltype, target, rId, is_external)
+
+    @property
+    def package(self):
+        """|OpcPackage| instance this part belongs to."""
+        return self._package
+
+    @property
+    def partname(self):
+        """|PackURI| instance holding partname of this part, e.g.
+        '/ppt/slides/slide1.xml'."""
+        return self._partname
+
+    @partname.setter
+    def partname(self, partname):
+        if not isinstance(partname, PackURI):
+            tmpl = "partname must be instance of PackURI, got '%s'"
+            raise TypeError(tmpl % type(partname).__name__)
+        self._partname = partname
 
-    def part_related_by(self, reltype):
-        """Return part to which this package has a relationship of `reltype`.
+    def part_related_by(self, reltype: str) -> Part:
+        """Return part to which this part has a relationship of `reltype`.
 
         Raises |KeyError| if no such relationship is found and |ValueError| if more than
-        one such relationship is found.
+        one such relationship is found. Provides ability to resolve implicitly related
+        part, such as Slide -> SlideLayout.
         """
         return self.rels.part_with_reltype(reltype)
 
+    def relate_to(self, target: Part | str, reltype: str, is_external: bool = False) -> str:
+        """Return rId key of relationship of `reltype` to `target`.
+
+        The returned `rId` is from an existing relationship if there is one, otherwise a
+        new relationship is created.
+        """
+        if is_external:
+            return self.rels.get_or_add_ext_rel(reltype, target)
+        else:
+            rel = self.rels.get_or_add(reltype, target)
+            return rel.rId
+
     @property
-    def parts(self):
-        """Return a list containing a reference to each of the parts in this package."""
-        return list(self.iter_parts())
-
-    def relate_to(self, part, reltype):
-        """Return rId key of relationship to `part`, from the existing relationship if
-        there is one, otherwise a newly created one."""
-        rel = self.rels.get_or_add(reltype, part)
-        return rel.rId
+    def related_parts(self):
+        """Dictionary mapping related parts by rId, so child objects can resolve
+        explicit relationships present in the part XML, e.g. sldIdLst to a specific
+        |Slide| instance."""
+        return self.rels.related_parts
 
     @lazyproperty
     def rels(self):
-        """Return a reference to the |Relationships| instance holding the collection of
-        relationships for this package."""
-        return Relationships(PACKAGE_URI.baseURI)
-
-    def save(self, pkg_file):
-        """Save this package to `pkg_file`, where `file` can be either a path to a file
-        (a string) or a file-like object."""
-        for part in self.parts:
-            part.before_marshal()
-        PackageWriter.write(pkg_file, self.rels, self.parts)
-
-    @property
-    def _core_properties_part(self):
-        """|CorePropertiesPart| object related to this package.
-
-        Creates a default core properties part if one is not present (not common).
-        """
-        try:
-            return self.part_related_by(RT.CORE_PROPERTIES)
-        except KeyError:
-            core_properties_part = CorePropertiesPart.default(self)
-            self.relate_to(core_properties_part, RT.CORE_PROPERTIES)
-            return core_properties_part
-
-
-class Unmarshaller:
-    """Hosts static methods for unmarshalling a package from a |PackageReader|."""
-
-    @staticmethod
-    def unmarshal(pkg_reader, package, part_factory):
-        """Construct graph of parts and realized relationships based on the contents of
-        `pkg_reader`, delegating construction of each part to `part_factory`.
-
-        Package relationships are added to `pkg`.
-        """
-        parts = Unmarshaller._unmarshal_parts(pkg_reader, package, part_factory)
-        Unmarshaller._unmarshal_relationships(pkg_reader, package, parts)
-        for part in parts.values():
-            part.after_unmarshal()
-        package.after_unmarshal()
-
-    @staticmethod
-    def _unmarshal_parts(pkg_reader, package, part_factory):
-        """Return a dictionary of |Part| instances unmarshalled from `pkg_reader`, keyed
-        by partname.
-
-        Side-effect is that each part in `pkg_reader` is constructed using
-        `part_factory`.
-        """
-        parts = {}
-        for partname, content_type, reltype, blob in pkg_reader.iter_sparts():
-            parts[partname] = part_factory(
-                partname, content_type, reltype, blob, package
-            )
-        return parts
-
-    @staticmethod
-    def _unmarshal_relationships(pkg_reader, package, parts):
-        """Add a relationship to the source object corresponding to each of the
-        relationships in `pkg_reader` with its target_part set to the actual target part
-        in `parts`."""
-        for source_uri, srel in pkg_reader.iter_srels():
-            source = package if source_uri == "/" else parts[source_uri]
-            target = (
-                srel.target_ref if srel.is_external else parts[srel.target_partname]
-            )
-            source.load_rel(srel.reltype, target, srel.rId, srel.is_external)
+        """|Relationships| instance holding the relationships for this part."""
+        return Relationships(self._partname.baseURI)
+
+    def target_ref(self, rId: str) -> str:
+        """Return URL contained in target ref of relationship identified by `rId`."""
+        rel = self.rels[rId]
+        return rel.target_ref
+
+    def _rel_ref_count(self, rId):
+        """Return the count of references in this part's XML to the relationship
+        identified by `rId`."""
+        rIds = self._element.xpath("//@r:id")
+        return len([_rId for _rId in rIds if _rId == rId])
+
+
+class PartFactory:
+    """Provides a way for client code to specify a subclass of |Part| to be constructed
+    by |Unmarshaller| based on its content type and/or a custom callable.
+
+    Setting ``PartFactory.part_class_selector`` to a callable object will cause that
+    object to be called with the parameters ``content_type, reltype``, once for each
+    part in the package. If the callable returns an object, it is used as the class for
+    that part. If it returns |None|, part class selection falls back to the content type
+    map defined in ``PartFactory.part_type_for``. If no class is returned from either of
+    these, the class contained in ``PartFactory.default_part_type`` is used to construct
+    the part, which is by default ``opc.package.Part``.
+    """
+
+    part_class_selector: Callable[[str, str], Type[Part] | None] | None
+    part_type_for: Dict[str, Type[Part]] = {}
+    default_part_type = Part
+
+    def __new__(
+        cls,
+        partname: str,
+        content_type: str,
+        reltype: str,
+        blob: bytes,
+        package: Package,
+    ):
+        PartClass: Type[Part] | None = None
+        if cls.part_class_selector is not None:
+            part_class_selector = cls_method_fn(cls, "part_class_selector")
+            PartClass = part_class_selector(content_type, reltype)
+        if PartClass is None:
+            PartClass = cls._part_cls_for(content_type)
+        return PartClass.load(partname, content_type, blob, package)
+
+    @classmethod
+    def _part_cls_for(cls, content_type: str):
+        """Return the custom part class registered for `content_type`, or the default
+        part class if no custom class is registered for `content_type`."""
+        if content_type in cls.part_type_for:
+            return cls.part_type_for[content_type]
+        return cls.default_part_type
+
+
+class XmlPart(Part):
+    """Base class for package parts containing an XML payload, which is most of them.
+
+    Provides additional methods to the |Part| base class that take care of parsing and
+    reserializing the XML payload and managing relationships to other parts.
+    """
+
+    def __init__(self, partname, content_type, element, package):
+        super(XmlPart, self).__init__(partname, content_type, package=package)
+        self._element = element
+
+    @property
+    def blob(self):
+        return serialize_part_xml(self._element)
+
+    @property
+    def element(self):
+        """The root XML element of this XML part."""
+        return self._element
+
+    @classmethod
+    def load(cls, partname, content_type, blob, package):
+        element = parse_xml(blob)
+        return cls(partname, content_type, element, package)
+
+    @property
+    def part(self):
+        """Part of the parent protocol, "children" of the document will not know the
+        part that contains them so must ask their parent object.
+
+        That chain of delegation ends here for child objects.
+        """
+        return self
```

### Comparing `python-docx-1.1.0/src/docx/opc/packuri.py` & `python_docx-1.1.1/src/docx/opc/packuri.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/opc/part.py` & `python_docx-1.1.1/src/docx/opc/pkgreader.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,231 +1,258 @@
-"""Open Packaging Convention (OPC) objects related to package parts."""
+"""Low-level, read-only API to a serialized Open Packaging Convention (OPC) package."""
 
-from __future__ import annotations
+from docx.opc.constants import RELATIONSHIP_TARGET_MODE as RTM
+from docx.opc.oxml import parse_xml
+from docx.opc.packuri import PACKAGE_URI, PackURI
+from docx.opc.phys_pkg import PhysPkgReader
+from docx.opc.shared import CaseInsensitiveDict
+
+
+class PackageReader:
+    """Provides access to the contents of a zip-format OPC package via its
+    :attr:`serialized_parts` and :attr:`pkg_srels` attributes."""
+
+    def __init__(self, content_types, pkg_srels, sparts):
+        super(PackageReader, self).__init__()
+        self._pkg_srels = pkg_srels
+        self._sparts = sparts
+
+    @staticmethod
+    def from_file(pkg_file):
+        """Return a |PackageReader| instance loaded with contents of `pkg_file`."""
+        phys_reader = PhysPkgReader(pkg_file)
+        content_types = _ContentTypeMap.from_xml(phys_reader.content_types_xml)
+        pkg_srels = PackageReader._srels_for(phys_reader, PACKAGE_URI)
+        sparts = PackageReader._load_serialized_parts(
+            phys_reader, pkg_srels, content_types
+        )
+        phys_reader.close()
+        return PackageReader(content_types, pkg_srels, sparts)
+
+    def iter_sparts(self):
+        """Generate a 4-tuple `(partname, content_type, reltype, blob)` for each of the
+        serialized parts in the package."""
+        for s in self._sparts:
+            yield (s.partname, s.content_type, s.reltype, s.blob)
+
+    def iter_srels(self):
+        """Generate a 2-tuple `(source_uri, srel)` for each of the relationships in the
+        package."""
+        for srel in self._pkg_srels:
+            yield (PACKAGE_URI, srel)
+        for spart in self._sparts:
+            for srel in spart.srels:
+                yield (spart.partname, srel)
+
+    @staticmethod
+    def _load_serialized_parts(phys_reader, pkg_srels, content_types):
+        """Return a list of |_SerializedPart| instances corresponding to the parts in
+        `phys_reader` accessible by walking the relationship graph starting with
+        `pkg_srels`."""
+        sparts = []
+        part_walker = PackageReader._walk_phys_parts(phys_reader, pkg_srels)
+        for partname, blob, reltype, srels in part_walker:
+            content_type = content_types[partname]
+            spart = _SerializedPart(partname, content_type, reltype, blob, srels)
+            sparts.append(spart)
+        return tuple(sparts)
+
+    @staticmethod
+    def _srels_for(phys_reader, source_uri):
+        """Return |_SerializedRelationships| instance populated with relationships for
+        source identified by `source_uri`."""
+        rels_xml = phys_reader.rels_xml_for(source_uri)
+        return _SerializedRelationships.load_from_xml(source_uri.baseURI, rels_xml)
+
+    @staticmethod
+    def _walk_phys_parts(phys_reader, srels, visited_partnames=None):
+        """Generate a 4-tuple `(partname, blob, reltype, srels)` for each of the parts
+        in `phys_reader` by walking the relationship graph rooted at srels."""
+        if visited_partnames is None:
+            visited_partnames = []
+        for srel in srels:
+            if srel.is_external:
+                continue
+            partname = srel.target_partname
+            if partname in visited_partnames:
+                continue
+            visited_partnames.append(partname)
+            reltype = srel.reltype
+            part_srels = PackageReader._srels_for(phys_reader, partname)
+            blob = phys_reader.blob_for(partname)
+            yield (partname, blob, reltype, part_srels)
+            next_walker = PackageReader._walk_phys_parts(
+                phys_reader, part_srels, visited_partnames
+            )
+            for partname, blob, reltype, srels in next_walker:
+                yield (partname, blob, reltype, srels)
+
+
+class _ContentTypeMap:
+    """Value type providing dictionary semantics for looking up content type by part
+    name, e.g. ``content_type = cti['/ppt/presentation.xml']``."""
+
+    def __init__(self):
+        super(_ContentTypeMap, self).__init__()
+        self._overrides = CaseInsensitiveDict()
+        self._defaults = CaseInsensitiveDict()
 
-from typing import TYPE_CHECKING, Callable, Dict, Type
-
-from docx.opc.oxml import serialize_part_xml
-from docx.opc.packuri import PackURI
-from docx.opc.rel import Relationships
-from docx.opc.shared import cls_method_fn, lazyproperty
-from docx.oxml.parser import parse_xml
-
-if TYPE_CHECKING:
-    from docx.package import Package
+    def __getitem__(self, partname):
+        """Return content type for part identified by `partname`."""
+        if not isinstance(partname, PackURI):
+            tmpl = "_ContentTypeMap key must be <type 'PackURI'>, got %s"
+            raise KeyError(tmpl % type(partname))
+        if partname in self._overrides:
+            return self._overrides[partname]
+        if partname.ext in self._defaults:
+            return self._defaults[partname.ext]
+        tmpl = "no content type for partname '%s' in [Content_Types].xml"
+        raise KeyError(tmpl % partname)
+
+    @staticmethod
+    def from_xml(content_types_xml):
+        """Return a new |_ContentTypeMap| instance populated with the contents of
+        `content_types_xml`."""
+        types_elm = parse_xml(content_types_xml)
+        ct_map = _ContentTypeMap()
+        for o in types_elm.overrides:
+            ct_map._add_override(o.partname, o.content_type)
+        for d in types_elm.defaults:
+            ct_map._add_default(d.extension, d.content_type)
+        return ct_map
+
+    def _add_default(self, extension, content_type):
+        """Add the default mapping of `extension` to `content_type` to this content type
+        mapping."""
+        self._defaults[extension] = content_type
+
+    def _add_override(self, partname, content_type):
+        """Add the default mapping of `partname` to `content_type` to this content type
+        mapping."""
+        self._overrides[partname] = content_type
 
 
-class Part:
-    """Base class for package parts.
+class _SerializedPart:
+    """Value object for an OPC package part.
 
-    Provides common properties and methods, but intended to be subclassed in client code
-    to implement specific part behaviors.
+    Provides access to the partname, content type, blob, and serialized relationships
+    for the part.
     """
 
-    def __init__(
-        self,
-        partname: str,
-        content_type: str,
-        blob: bytes | None = None,
-        package: Package | None = None,
-    ):
-        super(Part, self).__init__()
+    def __init__(self, partname, content_type, reltype, blob, srels):
+        super(_SerializedPart, self).__init__()
         self._partname = partname
         self._content_type = content_type
+        self._reltype = reltype
         self._blob = blob
-        self._package = package
-
-    def after_unmarshal(self):
-        """Entry point for post-unmarshaling processing, for example to parse the part
-        XML.
-
-        May be overridden by subclasses without forwarding call to super.
-        """
-        # don't place any code here, just catch call if not overridden by
-        # subclass
-        pass
-
-    def before_marshal(self):
-        """Entry point for pre-serialization processing, for example to finalize part
-        naming if necessary.
-
-        May be overridden by subclasses without forwarding call to super.
-        """
-        # don't place any code here, just catch call if not overridden by
-        # subclass
-        pass
+        self._srels = srels
 
     @property
-    def blob(self):
-        """Contents of this package part as a sequence of bytes.
-
-        May be text or binary. Intended to be overridden by subclasses. Default behavior
-        is to return load blob.
-        """
-        return self._blob
+    def partname(self):
+        return self._partname
 
     @property
     def content_type(self):
-        """Content type of this part."""
         return self._content_type
 
-    def drop_rel(self, rId: str):
-        """Remove the relationship identified by `rId` if its reference count is less
-        than 2.
-
-        Relationships with a reference count of 0 are implicit relationships.
-        """
-        if self._rel_ref_count(rId) < 2:
-            del self.rels[rId]
-
-    @classmethod
-    def load(cls, partname: str, content_type: str, blob: bytes, package: Package):
-        return cls(partname, content_type, blob, package)
-
-    def load_rel(self, reltype, target, rId, is_external=False):
-        """Return newly added |_Relationship| instance of `reltype` between this part
-        and `target` with key `rId`.
-
-        Target mode is set to ``RTM.EXTERNAL`` if `is_external` is |True|. Intended for
-        use during load from a serialized package, where the rId is well-known. Other
-        methods exist for adding a new relationship to a part when manipulating a part.
-        """
-        return self.rels.add_relationship(reltype, target, rId, is_external)
-
     @property
-    def package(self):
-        """|OpcPackage| instance this part belongs to."""
-        return self._package
+    def blob(self):
+        return self._blob
 
     @property
-    def partname(self):
-        """|PackURI| instance holding partname of this part, e.g.
-        '/ppt/slides/slide1.xml'."""
-        return self._partname
-
-    @partname.setter
-    def partname(self, partname):
-        if not isinstance(partname, PackURI):
-            tmpl = "partname must be instance of PackURI, got '%s'"
-            raise TypeError(tmpl % type(partname).__name__)
-        self._partname = partname
+    def reltype(self):
+        """The referring relationship type of this part."""
+        return self._reltype
 
-    def part_related_by(self, reltype: str) -> Part:
-        """Return part to which this part has a relationship of `reltype`.
+    @property
+    def srels(self):
+        return self._srels
 
-        Raises |KeyError| if no such relationship is found and |ValueError| if more than
-        one such relationship is found. Provides ability to resolve implicitly related
-        part, such as Slide -> SlideLayout.
-        """
-        return self.rels.part_with_reltype(reltype)
 
-    def relate_to(self, target: Part, reltype: str, is_external: bool = False) -> str:
-        """Return rId key of relationship of `reltype` to `target`.
+class _SerializedRelationship:
+    """Value object representing a serialized relationship in an OPC package.
 
-        The returned `rId` is from an existing relationship if there is one, otherwise a
-        new relationship is created.
-        """
-        if is_external:
-            return self.rels.get_or_add_ext_rel(reltype, target)
-        else:
-            rel = self.rels.get_or_add(reltype, target)
-            return rel.rId
-
-    @property
-    def related_parts(self):
-        """Dictionary mapping related parts by rId, so child objects can resolve
-        explicit relationships present in the part XML, e.g. sldIdLst to a specific
-        |Slide| instance."""
-        return self.rels.related_parts
-
-    @lazyproperty
-    def rels(self):
-        """|Relationships| instance holding the relationships for this part."""
-        return Relationships(self._partname.baseURI)
-
-    def target_ref(self, rId):
-        """Return URL contained in target ref of relationship identified by `rId`."""
-        rel = self.rels[rId]
-        return rel.target_ref
-
-    def _rel_ref_count(self, rId):
-        """Return the count of references in this part's XML to the relationship
-        identified by `rId`."""
-        rIds = self._element.xpath("//@r:id")
-        return len([_rId for _rId in rIds if _rId == rId])
-
-
-class PartFactory:
-    """Provides a way for client code to specify a subclass of |Part| to be constructed
-    by |Unmarshaller| based on its content type and/or a custom callable.
-
-    Setting ``PartFactory.part_class_selector`` to a callable object will cause that
-    object to be called with the parameters ``content_type, reltype``, once for each
-    part in the package. If the callable returns an object, it is used as the class for
-    that part. If it returns |None|, part class selection falls back to the content type
-    map defined in ``PartFactory.part_type_for``. If no class is returned from either of
-    these, the class contained in ``PartFactory.default_part_type`` is used to construct
-    the part, which is by default ``opc.package.Part``.
+    Serialized, in this case, means any target part is referred to via its partname
+    rather than a direct link to an in-memory |Part| object.
     """
 
-    part_class_selector: Callable[[str, str], Type[Part] | None] | None
-    part_type_for: Dict[str, Type[Part]] = {}
-    default_part_type = Part
-
-    def __new__(
-        cls,
-        partname: str,
-        content_type: str,
-        reltype: str,
-        blob: bytes,
-        package: Package,
-    ):
-        PartClass: Type[Part] | None = None
-        if cls.part_class_selector is not None:
-            part_class_selector = cls_method_fn(cls, "part_class_selector")
-            PartClass = part_class_selector(content_type, reltype)
-        if PartClass is None:
-            PartClass = cls._part_cls_for(content_type)
-        return PartClass.load(partname, content_type, blob, package)
-
-    @classmethod
-    def _part_cls_for(cls, content_type: str):
-        """Return the custom part class registered for `content_type`, or the default
-        part class if no custom class is registered for `content_type`."""
-        if content_type in cls.part_type_for:
-            return cls.part_type_for[content_type]
-        return cls.default_part_type
+    def __init__(self, baseURI, rel_elm):
+        super(_SerializedRelationship, self).__init__()
+        self._baseURI = baseURI
+        self._rId = rel_elm.rId
+        self._reltype = rel_elm.reltype
+        self._target_mode = rel_elm.target_mode
+        self._target_ref = rel_elm.target_ref
 
+    @property
+    def is_external(self):
+        """True if target_mode is ``RTM.EXTERNAL``"""
+        return self._target_mode == RTM.EXTERNAL
 
-class XmlPart(Part):
-    """Base class for package parts containing an XML payload, which is most of them.
-
-    Provides additional methods to the |Part| base class that take care of parsing and
-    reserializing the XML payload and managing relationships to other parts.
-    """
-
-    def __init__(self, partname, content_type, element, package):
-        super(XmlPart, self).__init__(partname, content_type, package=package)
-        self._element = element
+    @property
+    def reltype(self):
+        """Relationship type, like ``RT.OFFICE_DOCUMENT``"""
+        return self._reltype
 
     @property
-    def blob(self):
-        return serialize_part_xml(self._element)
+    def rId(self):
+        """Relationship id, like 'rId9', corresponds to the ``Id`` attribute on the
+        ``CT_Relationship`` element."""
+        return self._rId
 
     @property
-    def element(self):
-        """The root XML element of this XML part."""
-        return self._element
+    def target_mode(self):
+        """String in ``TargetMode`` attribute of ``CT_Relationship`` element, one of
+        ``RTM.INTERNAL`` or ``RTM.EXTERNAL``."""
+        return self._target_mode
 
-    @classmethod
-    def load(cls, partname, content_type, blob, package):
-        element = parse_xml(blob)
-        return cls(partname, content_type, element, package)
+    @property
+    def target_ref(self):
+        """String in ``Target`` attribute of ``CT_Relationship`` element, a relative
+        part reference for internal target mode or an arbitrary URI, e.g. an HTTP URL,
+        for external target mode."""
+        return self._target_ref
 
     @property
-    def part(self):
-        """Part of the parent protocol, "children" of the document will not know the
-        part that contains them so must ask their parent object.
+    def target_partname(self):
+        """|PackURI| instance containing partname targeted by this relationship.
+
+        Raises ``ValueError`` on reference if target_mode is ``'External'``. Use
+        :attr:`target_mode` to check before referencing.
+        """
+        if self.is_external:
+            msg = (
+                "target_partname attribute on Relationship is undefined w"
+                'here TargetMode == "External"'
+            )
+            raise ValueError(msg)
+        # lazy-load _target_partname attribute
+        if not hasattr(self, "_target_partname"):
+            self._target_partname = PackURI.from_rel_ref(self._baseURI, self.target_ref)
+        return self._target_partname
+
+
+class _SerializedRelationships:
+    """Read-only sequence of |_SerializedRelationship| instances corresponding to the
+    relationships item XML passed to constructor."""
+
+    def __init__(self):
+        super(_SerializedRelationships, self).__init__()
+        self._srels = []
+
+    def __iter__(self):
+        """Support iteration, e.g. 'for x in srels:'."""
+        return self._srels.__iter__()
+
+    @staticmethod
+    def load_from_xml(baseURI, rels_item_xml):
+        """Return |_SerializedRelationships| instance loaded with the relationships
+        contained in `rels_item_xml`.
 
-        That chain of delegation ends here for child objects.
+        Returns an empty collection if `rels_item_xml` is |None|.
         """
-        return self
+        srels = _SerializedRelationships()
+        if rels_item_xml is not None:
+            rels_elm = parse_xml(rels_item_xml)
+            for rel_elm in rels_elm.Relationship_lst:
+                srels._srels.append(_SerializedRelationship(baseURI, rel_elm))
+        return srels
```

### Comparing `python-docx-1.1.0/src/docx/opc/parts/coreprops.py` & `python_docx-1.1.1/src/docx/opc/parts/coreprops.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/opc/phys_pkg.py` & `python_docx-1.1.1/src/docx/opc/phys_pkg.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/opc/pkgreader.py` & `python_docx-1.1.1/tests/opc/unitdata/rels.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,258 +1,302 @@
-"""Low-level, read-only API to a serialized Open Packaging Convention (OPC) package."""
+"""Test data for relationship-related unit tests."""
 
-from docx.opc.constants import RELATIONSHIP_TARGET_MODE as RTM
+from docx.opc.constants import NAMESPACE as NS
+from docx.opc.constants import RELATIONSHIP_TYPE as RT
 from docx.opc.oxml import parse_xml
-from docx.opc.packuri import PACKAGE_URI, PackURI
-from docx.opc.phys_pkg import PhysPkgReader
-from docx.opc.shared import CaseInsensitiveDict
-
-
-class PackageReader:
-    """Provides access to the contents of a zip-format OPC package via its
-    :attr:`serialized_parts` and :attr:`pkg_srels` attributes."""
-
-    def __init__(self, content_types, pkg_srels, sparts):
-        super(PackageReader, self).__init__()
-        self._pkg_srels = pkg_srels
-        self._sparts = sparts
-
-    @staticmethod
-    def from_file(pkg_file):
-        """Return a |PackageReader| instance loaded with contents of `pkg_file`."""
-        phys_reader = PhysPkgReader(pkg_file)
-        content_types = _ContentTypeMap.from_xml(phys_reader.content_types_xml)
-        pkg_srels = PackageReader._srels_for(phys_reader, PACKAGE_URI)
-        sparts = PackageReader._load_serialized_parts(
-            phys_reader, pkg_srels, content_types
-        )
-        phys_reader.close()
-        return PackageReader(content_types, pkg_srels, sparts)
+from docx.opc.rel import Relationships
 
-    def iter_sparts(self):
-        """Generate a 4-tuple `(partname, content_type, reltype, blob)` for each of the
-        serialized parts in the package."""
-        for s in self._sparts:
-            yield (s.partname, s.content_type, s.reltype, s.blob)
-
-    def iter_srels(self):
-        """Generate a 2-tuple `(source_uri, srel)` for each of the relationships in the
-        package."""
-        for srel in self._pkg_srels:
-            yield (PACKAGE_URI, srel)
-        for spart in self._sparts:
-            for srel in spart.srels:
-                yield (spart.partname, srel)
-
-    @staticmethod
-    def _load_serialized_parts(phys_reader, pkg_srels, content_types):
-        """Return a list of |_SerializedPart| instances corresponding to the parts in
-        `phys_reader` accessible by walking the relationship graph starting with
-        `pkg_srels`."""
-        sparts = []
-        part_walker = PackageReader._walk_phys_parts(phys_reader, pkg_srels)
-        for partname, blob, reltype, srels in part_walker:
-            content_type = content_types[partname]
-            spart = _SerializedPart(partname, content_type, reltype, blob, srels)
-            sparts.append(spart)
-        return tuple(sparts)
-
-    @staticmethod
-    def _srels_for(phys_reader, source_uri):
-        """Return |_SerializedRelationships| instance populated with relationships for
-        source identified by `source_uri`."""
-        rels_xml = phys_reader.rels_xml_for(source_uri)
-        return _SerializedRelationships.load_from_xml(source_uri.baseURI, rels_xml)
-
-    @staticmethod
-    def _walk_phys_parts(phys_reader, srels, visited_partnames=None):
-        """Generate a 4-tuple `(partname, blob, reltype, srels)` for each of the parts
-        in `phys_reader` by walking the relationship graph rooted at srels."""
-        if visited_partnames is None:
-            visited_partnames = []
-        for srel in srels:
-            if srel.is_external:
-                continue
-            partname = srel.target_partname
-            if partname in visited_partnames:
-                continue
-            visited_partnames.append(partname)
-            reltype = srel.reltype
-            part_srels = PackageReader._srels_for(phys_reader, partname)
-            blob = phys_reader.blob_for(partname)
-            yield (partname, blob, reltype, part_srels)
-            next_walker = PackageReader._walk_phys_parts(
-                phys_reader, part_srels, visited_partnames
-            )
-            for partname, blob, reltype, srels in next_walker:
-                yield (partname, blob, reltype, srels)
 
+class BaseBuilder:
+    """
+    Provides common behavior for all data builders.
+    """
 
-class _ContentTypeMap:
-    """Value type providing dictionary semantics for looking up content type by part
-    name, e.g. ``content_type = cti['/ppt/presentation.xml']``."""
+    @property
+    def element(self):
+        """Return element based on XML generated by builder"""
+        return parse_xml(self.xml)
+
+    def with_indent(self, indent):
+        """Add integer `indent` spaces at beginning of element XML"""
+        self._indent = indent
+        return self
+
+
+class RelationshipsBuilder:
+    """Builder class for test Relationships"""
+
+    partname_tmpls = {
+        RT.SLIDE_MASTER: "/ppt/slideMasters/slideMaster%d.xml",
+        RT.SLIDE: "/ppt/slides/slide%d.xml",
+    }
 
     def __init__(self):
-        super(_ContentTypeMap, self).__init__()
-        self._overrides = CaseInsensitiveDict()
-        self._defaults = CaseInsensitiveDict()
-
-    def __getitem__(self, partname):
-        """Return content type for part identified by `partname`."""
-        if not isinstance(partname, PackURI):
-            tmpl = "_ContentTypeMap key must be <type 'PackURI'>, got %s"
-            raise KeyError(tmpl % type(partname))
-        if partname in self._overrides:
-            return self._overrides[partname]
-        if partname.ext in self._defaults:
-            return self._defaults[partname.ext]
-        tmpl = "no content type for partname '%s' in [Content_Types].xml"
-        raise KeyError(tmpl % partname)
-
-    @staticmethod
-    def from_xml(content_types_xml):
-        """Return a new |_ContentTypeMap| instance populated with the contents of
-        `content_types_xml`."""
-        types_elm = parse_xml(content_types_xml)
-        ct_map = _ContentTypeMap()
-        for o in types_elm.overrides:
-            ct_map._add_override(o.partname, o.content_type)
-        for d in types_elm.defaults:
-            ct_map._add_default(d.extension, d.content_type)
-        return ct_map
-
-    def _add_default(self, extension, content_type):
-        """Add the default mapping of `extension` to `content_type` to this content type
-        mapping."""
-        self._defaults[extension] = content_type
-
-    def _add_override(self, partname, content_type):
-        """Add the default mapping of `partname` to `content_type` to this content type
-        mapping."""
-        self._overrides[partname] = content_type
-
-
-class _SerializedPart:
-    """Value object for an OPC package part.
+        self.relationships = []
+        self.next_rel_num = 1
+        self.next_partnums = {}
+
+    def _next_partnum(self, reltype):
+        if reltype not in self.next_partnums:
+            self.next_partnums[reltype] = 1
+        partnum = self.next_partnums[reltype]
+        self.next_partnums[reltype] = partnum + 1
+        return partnum
+
+    @property
+    def next_rId(self):
+        rId = "rId%d" % self.next_rel_num
+        self.next_rel_num += 1
+        return rId
+
+    def _next_tuple_partname(self, reltype):
+        partname_tmpl = self.partname_tmpls[reltype]
+        partnum = self._next_partnum(reltype)
+        return partname_tmpl % partnum
+
+    def build(self):
+        rels = Relationships()
+        for rel in self.relationships:
+            rels.add_rel(rel)
+        return rels
+
 
-    Provides access to the partname, content type, blob, and serialized relationships
-    for the part.
+class CT_DefaultBuilder(BaseBuilder):
+    """
+    Test data builder for CT_Default (Default) XML element that appears in
+    `[Content_Types].xml`.
     """
 
-    def __init__(self, partname, content_type, reltype, blob, srels):
-        super(_SerializedPart, self).__init__()
-        self._partname = partname
+    def __init__(self):
+        """Establish instance variables with default values"""
+        self._content_type = "application/xml"
+        self._extension = "xml"
+        self._indent = 0
+        self._namespace = ' xmlns="%s"' % NS.OPC_CONTENT_TYPES
+
+    def with_content_type(self, content_type):
+        """Set ContentType attribute to `content_type`"""
         self._content_type = content_type
-        self._reltype = reltype
-        self._blob = blob
-        self._srels = srels
+        return self
 
-    @property
-    def partname(self):
-        return self._partname
+    def with_extension(self, extension):
+        """Set Extension attribute to `extension`"""
+        self._extension = extension
+        return self
 
-    @property
-    def content_type(self):
-        return self._content_type
+    def without_namespace(self):
+        """Don't include an 'xmlns=' attribute"""
+        self._namespace = ""
+        return self
 
     @property
-    def blob(self):
-        return self._blob
+    def xml(self):
+        """Return Default element"""
+        tmpl = '%s<Default%s Extension="%s" ContentType="%s"/>\n'
+        indent = " " * self._indent
+        return tmpl % (indent, self._namespace, self._extension, self._content_type)
 
-    @property
-    def reltype(self):
-        """The referring relationship type of this part."""
-        return self._reltype
 
-    @property
-    def srels(self):
-        return self._srels
+class CT_OverrideBuilder(BaseBuilder):
+    """
+    Test data builder for CT_Override (Override) XML element that appears in
+    `[Content_Types].xml`.
+    """
 
+    def __init__(self):
+        """Establish instance variables with default values"""
+        self._content_type = "app/vnd.type"
+        self._indent = 0
+        self._namespace = ' xmlns="%s"' % NS.OPC_CONTENT_TYPES
+        self._partname = "/part/name.xml"
 
-class _SerializedRelationship:
-    """Value object representing a serialized relationship in an OPC package.
+    def with_content_type(self, content_type):
+        """Set ContentType attribute to `content_type`"""
+        self._content_type = content_type
+        return self
 
-    Serialized, in this case, means any target part is referred to via its partname
-    rather than a direct link to an in-memory |Part| object.
-    """
+    def with_partname(self, partname):
+        """Set PartName attribute to `partname`"""
+        self._partname = partname
+        return self
 
-    def __init__(self, baseURI, rel_elm):
-        super(_SerializedRelationship, self).__init__()
-        self._baseURI = baseURI
-        self._rId = rel_elm.rId
-        self._reltype = rel_elm.reltype
-        self._target_mode = rel_elm.target_mode
-        self._target_ref = rel_elm.target_ref
+    def without_namespace(self):
+        """Don't include an 'xmlns=' attribute"""
+        self._namespace = ""
+        return self
 
     @property
-    def is_external(self):
-        """True if target_mode is ``RTM.EXTERNAL``"""
-        return self._target_mode == RTM.EXTERNAL
+    def xml(self):
+        """Return Override element"""
+        tmpl = '%s<Override%s PartName="%s" ContentType="%s"/>\n'
+        indent = " " * self._indent
+        return tmpl % (indent, self._namespace, self._partname, self._content_type)
 
-    @property
-    def reltype(self):
-        """Relationship type, like ``RT.OFFICE_DOCUMENT``"""
-        return self._reltype
 
-    @property
-    def rId(self):
-        """Relationship id, like 'rId9', corresponds to the ``Id`` attribute on the
-        ``CT_Relationship`` element."""
-        return self._rId
+class CT_RelationshipBuilder(BaseBuilder):
+    """
+    Test data builder for CT_Relationship (Relationship) XML element that
+    appears in .rels files
+    """
+
+    def __init__(self):
+        """Establish instance variables with default values"""
+        self._rId = "rId9"
+        self._reltype = "ReLtYpE"
+        self._target = "docProps/core.xml"
+        self._target_mode = None
+        self._indent = 0
+        self._namespace = ' xmlns="%s"' % NS.OPC_RELATIONSHIPS
+
+    def with_rId(self, rId):
+        """Set Id attribute to `rId`"""
+        self._rId = rId
+        return self
+
+    def with_reltype(self, reltype):
+        """Set Type attribute to `reltype`"""
+        self._reltype = reltype
+        return self
+
+    def with_target(self, target):
+        """Set XXX attribute to `target`"""
+        self._target = target
+        return self
+
+    def with_target_mode(self, target_mode):
+        """Set TargetMode attribute to `target_mode`"""
+        self._target_mode = None if target_mode == "Internal" else target_mode
+        return self
+
+    def without_namespace(self):
+        """Don't include an 'xmlns=' attribute"""
+        self._namespace = ""
+        return self
 
     @property
     def target_mode(self):
-        """String in ``TargetMode`` attribute of ``CT_Relationship`` element, one of
-        ``RTM.INTERNAL`` or ``RTM.EXTERNAL``."""
-        return self._target_mode
+        if self._target_mode is None:
+            return ""
+        return ' TargetMode="%s"' % self._target_mode
+
+    @property
+    def xml(self):
+        """Return Relationship element"""
+        tmpl = '%s<Relationship%s Id="%s" Type="%s" Target="%s"%s/>\n'
+        indent = " " * self._indent
+        return tmpl % (
+            indent,
+            self._namespace,
+            self._rId,
+            self._reltype,
+            self._target,
+            self.target_mode,
+        )
 
-    @property
-    def target_ref(self):
-        """String in ``Target`` attribute of ``CT_Relationship`` element, a relative
-        part reference for internal target mode or an arbitrary URI, e.g. an HTTP URL,
-        for external target mode."""
-        return self._target_ref
 
-    @property
-    def target_partname(self):
-        """|PackURI| instance containing partname targeted by this relationship.
+class CT_RelationshipsBuilder(BaseBuilder):
+    """
+    Test data builder for CT_Relationships (Relationships) XML element, the
+    root element in .rels files.
+    """
+
+    def __init__(self):
+        """Establish instance variables with default values"""
+        self._rels = (
+            ("rId1", "http://reltype1", "docProps/core.xml", "Internal"),
+            ("rId2", "http://linktype", "http://some/link", "External"),
+            ("rId3", "http://reltype2", "../slides/slide1.xml", "Internal"),
+        )
 
-        Raises ``ValueError`` on reference if target_mode is ``'External'``. Use
-        :attr:`target_mode` to check before referencing.
+    @property
+    def xml(self):
+        """
+        Return XML string based on settings accumulated via method calls.
         """
-        if self.is_external:
-            msg = (
-                "target_partname attribute on Relationship is undefined w"
-                'here TargetMode == "External"'
+        xml = '<Relationships xmlns="%s">\n' % NS.OPC_RELATIONSHIPS
+        for rId, reltype, target, target_mode in self._rels:
+            xml += (
+                a_Relationship()
+                .with_rId(rId)
+                .with_reltype(reltype)
+                .with_target(target)
+                .with_target_mode(target_mode)
+                .with_indent(2)
+                .without_namespace()
+                .xml
             )
-            raise ValueError(msg)
-        # lazy-load _target_partname attribute
-        if not hasattr(self, "_target_partname"):
-            self._target_partname = PackURI.from_rel_ref(self._baseURI, self.target_ref)
-        return self._target_partname
+        xml += "</Relationships>\n"
+        return xml
 
 
-class _SerializedRelationships:
-    """Read-only sequence of |_SerializedRelationship| instances corresponding to the
-    relationships item XML passed to constructor."""
+class CT_TypesBuilder(BaseBuilder):
+    """
+    Test data builder for CT_Types (<Types>) XML element, the root element in
+    [Content_Types].xml files
+    """
 
     def __init__(self):
-        super(_SerializedRelationships, self).__init__()
-        self._srels = []
+        """Establish instance variables with default values"""
+        self._defaults = (
+            ("xml", "application/xml"),
+            ("jpeg", "image/jpeg"),
+        )
+        self._empty = False
+        self._overrides = (
+            ("/docProps/core.xml", "app/vnd.type1"),
+            ("/ppt/presentation.xml", "app/vnd.type2"),
+            ("/docProps/thumbnail.jpeg", "image/jpeg"),
+        )
 
-    def __iter__(self):
-        """Support iteration, e.g. 'for x in srels:'."""
-        return self._srels.__iter__()
-
-    @staticmethod
-    def load_from_xml(baseURI, rels_item_xml):
-        """Return |_SerializedRelationships| instance loaded with the relationships
-        contained in `rels_item_xml`.
+    def empty(self):
+        self._empty = True
+        return self
 
-        Returns an empty collection if `rels_item_xml` is |None|.
+    @property
+    def xml(self):
         """
-        srels = _SerializedRelationships()
-        if rels_item_xml is not None:
-            rels_elm = parse_xml(rels_item_xml)
-            for rel_elm in rels_elm.Relationship_lst:
-                srels._srels.append(_SerializedRelationship(baseURI, rel_elm))
-        return srels
+        Return XML string based on settings accumulated via method calls
+        """
+        if self._empty:
+            return '<Types xmlns="%s"/>\n' % NS.OPC_CONTENT_TYPES
+
+        xml = '<Types xmlns="%s">\n' % NS.OPC_CONTENT_TYPES
+        for extension, content_type in self._defaults:
+            xml += (
+                a_Default()
+                .with_extension(extension)
+                .with_content_type(content_type)
+                .with_indent(2)
+                .without_namespace()
+                .xml
+            )
+        for partname, content_type in self._overrides:
+            xml += (
+                an_Override()
+                .with_partname(partname)
+                .with_content_type(content_type)
+                .with_indent(2)
+                .without_namespace()
+                .xml
+            )
+        xml += "</Types>\n"
+        return xml
+
+
+def a_Default():
+    return CT_DefaultBuilder()
+
+
+def a_Relationship():
+    return CT_RelationshipBuilder()
+
+
+def a_Relationships():
+    return CT_RelationshipsBuilder()
+
+
+def a_Types():
+    return CT_TypesBuilder()
+
+
+def an_Override():
+    return CT_OverrideBuilder()
```

### Comparing `python-docx-1.1.0/src/docx/opc/pkgwriter.py` & `python_docx-1.1.1/src/docx/opc/pkgwriter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 """Provides low-level, write-only API to serialized (OPC) package.
 
 OPC stands for Open Packaging Convention. This is e, essentially an implementation of
 OpcPackage.save().
 """
 
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Iterable
+
 from docx.opc.constants import CONTENT_TYPE as CT
 from docx.opc.oxml import CT_Types, serialize_part_xml
 from docx.opc.packuri import CONTENT_TYPES_URI, PACKAGE_URI
 from docx.opc.phys_pkg import PhysPkgWriter
 from docx.opc.shared import CaseInsensitiveDict
 from docx.opc.spec import default_content_types
 
+if TYPE_CHECKING:
+    from docx.opc.part import Part
+
 
 class PackageWriter:
     """Writes a zip-format OPC package to `pkg_file`, where `pkg_file` can be either a
     path to a zip file (a string) or a file-like object.
 
     Its single API method, :meth:`write`, is static, so this class is not intended to be
     instantiated.
@@ -34,21 +41,21 @@
     def _write_content_types_stream(phys_writer, parts):
         """Write ``[Content_Types].xml`` part to the physical package with an
         appropriate content type lookup target for each part in `parts`."""
         cti = _ContentTypesItem.from_parts(parts)
         phys_writer.write(CONTENT_TYPES_URI, cti.blob)
 
     @staticmethod
-    def _write_parts(phys_writer, parts):
+    def _write_parts(phys_writer: PhysPkgWriter, parts: Iterable[Part]):
         """Write the blob of each part in `parts` to the package, along with a rels item
         for its relationships if and only if it has any."""
         for part in parts:
             phys_writer.write(part.partname, part.blob)
-            if len(part._rels):
-                phys_writer.write(part.partname.rels_uri, part._rels.xml)
+            if len(part.rels):
+                phys_writer.write(part.partname.rels_uri, part.rels.xml)
 
     @staticmethod
     def _write_pkg_rels(phys_writer, pkg_rels):
         """Write the XML rels item for `pkg_rels` ('/_rels/.rels') to the package."""
         phys_writer.write(PACKAGE_URI.rels_uri, pkg_rels.xml)
```

### Comparing `python-docx-1.1.0/src/docx/opc/rel.py` & `python_docx-1.1.1/src/docx/opc/rel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 """Relationship-related objects."""
 
 from __future__ import annotations
 
-from typing import Any, Dict
+from typing import TYPE_CHECKING, Any, Dict
 
 from docx.opc.oxml import CT_Relationships
 
+if TYPE_CHECKING:
+    from docx.opc.part import Part
+
 
 class Relationships(Dict[str, "_Relationship"]):
     """Collection object for |_Relationship| instances, having list semantics."""
 
     def __init__(self, baseURI: str):
         super(Relationships, self).__init__()
         self._baseURI = baseURI
         self._target_parts_by_rId: Dict[str, Any] = {}
 
     def add_relationship(
-        self, reltype: str, target: str | Any, rId: str, is_external: bool = False
+        self, reltype: str, target: Part | str, rId: str, is_external: bool = False
     ) -> "_Relationship":
         """Return a newly added |_Relationship| instance."""
         rel = _Relationship(rId, reltype, target, self._baseURI, is_external)
         self[rId] = rel
         if not is_external:
             self._target_parts_by_rId[rId] = target
         return rel
 
-    def get_or_add(self, reltype, target_part):
+    def get_or_add(self, reltype: str, target_part: Part) -> _Relationship:
         """Return relationship of `reltype` to `target_part`, newly added if not already
         present in collection."""
         rel = self._get_matching(reltype, target_part)
         if rel is None:
             rId = self._next_rId
             rel = self.add_relationship(reltype, target_part, rId)
         return rel
@@ -60,15 +63,17 @@
         """Serialize this relationship collection into XML suitable for storage as a
         .rels file in an OPC package."""
         rels_elm = CT_Relationships.new()
         for rel in self.values():
             rels_elm.add_rel(rel.rId, rel.reltype, rel.target_ref, rel.is_external)
         return rels_elm.xml
 
-    def _get_matching(self, reltype, target, is_external=False):
+    def _get_matching(
+        self, reltype: str, target: Part | str, is_external: bool = False
+    ) -> _Relationship | None:
         """Return relationship of matching `reltype`, `target`, and `is_external` from
         collection, or None if not found."""
 
         def matches(rel, reltype, target, is_external):
             if rel.reltype != reltype:
                 return False
             if rel.is_external != is_external:
@@ -95,15 +100,15 @@
             raise KeyError(tmpl % reltype)
         if len(matching) > 1:
             tmpl = "multiple relationships of type '%s' in collection"
             raise ValueError(tmpl % reltype)
         return matching[0]
 
     @property
-    def _next_rId(self):
+    def _next_rId(self) -> str:
         """Next available rId in collection, starting from 'rId1' and making use of any
         gaps in numbering, e.g. 'rId2' for rIds ['rId1', 'rId3']."""
         for n in range(1, len(self) + 2):
             rId_candidate = "rId%d" % n  # like 'rId19'
             if rId_candidate not in self:
                 return rId_candidate
 
@@ -131,16 +136,15 @@
     def rId(self):
         return self._rId
 
     @property
     def target_part(self):
         if self._is_external:
             raise ValueError(
-                "target_part property on _Relationship is undef"
-                "ined when target mode is External"
+                "target_part property on _Relationship is undef" "ined when target mode is External"
             )
         return self._target
 
     @property
     def target_ref(self) -> str:
         if self._is_external:
             return self._target
```

### Comparing `python-docx-1.1.0/src/docx/opc/spec.py` & `python_docx-1.1.1/src/docx/opc/spec.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/oxml/__init__.py` & `python_docx-1.1.1/src/docx/oxml/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,29 +145,33 @@
     CT_Height,
     CT_Row,
     CT_Tbl,
     CT_TblGrid,
     CT_TblGridCol,
     CT_TblLayoutType,
     CT_TblPr,
+    CT_TblPrEx,
     CT_TblWidth,
     CT_Tc,
     CT_TcPr,
     CT_TrPr,
     CT_VMerge,
     CT_VerticalJc,
 )
 
 register_element_cls("w:bidiVisual", CT_OnOff)
+register_element_cls("w:gridAfter", CT_DecimalNumber)
+register_element_cls("w:gridBefore", CT_DecimalNumber)
 register_element_cls("w:gridCol", CT_TblGridCol)
 register_element_cls("w:gridSpan", CT_DecimalNumber)
 register_element_cls("w:tbl", CT_Tbl)
 register_element_cls("w:tblGrid", CT_TblGrid)
 register_element_cls("w:tblLayout", CT_TblLayoutType)
 register_element_cls("w:tblPr", CT_TblPr)
+register_element_cls("w:tblPrEx", CT_TblPrEx)
 register_element_cls("w:tblStyle", CT_String)
 register_element_cls("w:tc", CT_Tc)
 register_element_cls("w:tcPr", CT_TcPr)
 register_element_cls("w:tcW", CT_TblWidth)
 register_element_cls("w:tr", CT_Row)
 register_element_cls("w:trHeight", CT_Height)
 register_element_cls("w:trPr", CT_TrPr)
```

### Comparing `python-docx-1.1.0/src/docx/oxml/coreprops.py` & `python_docx-1.1.1/src/docx/oxml/coreprops.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/oxml/document.py` & `python_docx-1.1.1/src/docx/oxml/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     p_lst: List[CT_P]
     tbl_lst: List[CT_Tbl]
 
     _insert_tbl: Callable[[CT_Tbl], CT_Tbl]
 
     p = ZeroOrMore("w:p", successors=("w:sectPr",))
     tbl = ZeroOrMore("w:tbl", successors=("w:sectPr",))
-    sectPr: CT_SectPr | None = ZeroOrOne(  # pyright: ignore[reportGeneralTypeIssues]
+    sectPr: CT_SectPr | None = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
         "w:sectPr", successors=()
     )
 
     def add_section_break(self) -> CT_SectPr:
         """Return `w:sectPr` element for new section added at end of document.
 
         The last `w:sectPr` becomes the second-to-last, with the new `w:sectPr` being an
```

### Comparing `python-docx-1.1.0/src/docx/oxml/ns.py` & `python_docx-1.1.1/src/docx/oxml/ns.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Namespace-related objects."""
 
-from typing import Any, Dict
+from __future__ import annotations
 
-from typing_extensions import Self
+from typing import Any, Dict
 
 nsmap = {
     "a": "http://schemas.openxmlformats.org/drawingml/2006/main",
     "c": "http://schemas.openxmlformats.org/drawingml/2006/chart",
     "cp": "http://schemas.openxmlformats.org/package/2006/metadata/core-properties",
     "dc": "http://purl.org/dc/elements/1.1/",
     "dcmitype": "http://purl.org/dc/dcmitype/",
@@ -37,15 +37,15 @@
         self._ns_uri = nsmap[self._pfx]
 
     @property
     def clark_name(self) -> str:
         return "{%s}%s" % (self._ns_uri, self._local_part)
 
     @classmethod
-    def from_clark_name(cls, clark_name: str) -> Self:
+    def from_clark_name(cls, clark_name: str) -> NamespacePrefixedTag:
         nsuri, local_name = clark_name[1:].split("}")
         nstag = "%s:%s" % (pfxmap[nsuri], local_name)
         return cls(nstag)
 
     @property
     def local_part(self) -> str:
         """The local part of this tag.
```

### Comparing `python-docx-1.1.0/src/docx/oxml/numbering.py` & `python_docx-1.1.1/src/docx/oxml/numbering.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/oxml/parser.py` & `python_docx-1.1.1/src/docx/oxml/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pyright: reportImportCycles=false
+
 """XML parser for python-docx."""
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, Type, cast
 
 from lxml import etree
@@ -39,15 +41,15 @@
     namespace[tagroot] = cls
 
 
 def OxmlElement(
     nsptag_str: str,
     attrs: Dict[str, str] | None = None,
     nsdecls: Dict[str, str] | None = None,
-) -> BaseOxmlElement:
+) -> BaseOxmlElement | etree._Element:  # pyright: ignore[reportPrivateUsage]
     """Return a 'loose' lxml element having the tag specified by `nsptag_str`.
 
     The tag in `nsptag_str` must contain the standard namespace prefix, e.g. `a:tbl`.
     The resulting element is an instance of the custom element class for this tag name
     if one is defined. A dictionary of attribute values may be provided as `attrs`; they
     are set if present. All namespaces defined in the dict `nsdecls` are declared in the
     element using the key as the prefix and the value as the namespace name. If
```

### Comparing `python-docx-1.1.0/src/docx/oxml/section.py` & `python_docx-1.1.1/src/docx/oxml/section.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,63 +47,57 @@
         """
         return self.xpath("./w:p | ./w:tbl")
 
 
 class CT_HdrFtrRef(BaseOxmlElement):
     """`w:headerReference` and `w:footerReference` elements."""
 
-    type_: WD_HEADER_FOOTER = (
-        RequiredAttribute(  # pyright: ignore[reportGeneralTypeIssues]
-            "w:type", WD_HEADER_FOOTER
-        )
-    )
-    rId: str = RequiredAttribute(  # pyright: ignore[reportGeneralTypeIssues]
-        "r:id", XsdString
+    type_: WD_HEADER_FOOTER = RequiredAttribute(  # pyright: ignore[reportAssignmentType]
+        "w:type", WD_HEADER_FOOTER
     )
+    rId: str = RequiredAttribute("r:id", XsdString)  # pyright: ignore[reportAssignmentType]
 
 
 class CT_PageMar(BaseOxmlElement):
     """``<w:pgMar>`` element, defining page margins."""
 
-    top: Length | None = OptionalAttribute(  # pyright: ignore[reportGeneralTypeIssues]
+    top: Length | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
         "w:top", ST_SignedTwipsMeasure
     )
-    right: Length | None = OptionalAttribute(  # pyright: ignore
+    right: Length | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
         "w:right", ST_TwipsMeasure
     )
-    bottom: Length | None = OptionalAttribute(  # pyright: ignore
+    bottom: Length | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
         "w:bottom", ST_SignedTwipsMeasure
     )
-    left: Length | None = OptionalAttribute(  # pyright: ignore[reportGeneralTypeIssues]
+    left: Length | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
         "w:left", ST_TwipsMeasure
     )
-    header: Length | None = OptionalAttribute(  # pyright: ignore
+    header: Length | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
         "w:header", ST_TwipsMeasure
     )
-    footer: Length | None = OptionalAttribute(  # pyright: ignore
+    footer: Length | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
         "w:footer", ST_TwipsMeasure
     )
-    gutter: Length | None = OptionalAttribute(  # pyright: ignore
+    gutter: Length | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
         "w:gutter", ST_TwipsMeasure
     )
 
 
 class CT_PageSz(BaseOxmlElement):
     """``<w:pgSz>`` element, defining page dimensions and orientation."""
 
-    w: Length | None = OptionalAttribute(  # pyright: ignore[reportGeneralTypeIssues]
+    w: Length | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
         "w:w", ST_TwipsMeasure
     )
-    h: Length | None = OptionalAttribute(  # pyright: ignore[reportGeneralTypeIssues]
+    h: Length | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
         "w:h", ST_TwipsMeasure
     )
-    orient: WD_ORIENTATION = (
-        OptionalAttribute(  # pyright: ignore[reportGeneralTypeIssues]
-            "w:orient", WD_ORIENTATION, default=WD_ORIENTATION.PORTRAIT
-        )
+    orient: WD_ORIENTATION = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
+        "w:orient", WD_ORIENTATION, default=WD_ORIENTATION.PORTRAIT
     )
 
 
 class CT_SectPr(BaseOxmlElement):
     """`w:sectPr` element, the container element for section properties."""
 
     get_or_add_pgMar: Callable[[], CT_PageMar]
@@ -135,24 +129,24 @@
         "w:rtlGutter",
         "w:docGrid",
         "w:printerSettings",
         "w:sectPrChange",
     )
     headerReference = ZeroOrMore("w:headerReference", successors=_tag_seq)
     footerReference = ZeroOrMore("w:footerReference", successors=_tag_seq)
-    type: CT_SectType | None = ZeroOrOne(  # pyright: ignore[reportGeneralTypeIssues]
+    type: CT_SectType | None = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
         "w:type", successors=_tag_seq[3:]
     )
-    pgSz: CT_PageSz | None = ZeroOrOne(  # pyright: ignore[reportGeneralTypeIssues]
+    pgSz: CT_PageSz | None = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
         "w:pgSz", successors=_tag_seq[4:]
     )
-    pgMar: CT_PageMar | None = ZeroOrOne(  # pyright: ignore[reportGeneralTypeIssues]
+    pgMar: CT_PageMar | None = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
         "w:pgMar", successors=_tag_seq[5:]
     )
-    titlePg: CT_OnOff | None = ZeroOrOne(  # pyright: ignore[reportGeneralTypeIssues]
+    titlePg: CT_OnOff | None = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
         "w:titlePg", successors=_tag_seq[14:]
     )
     del _tag_seq
 
     def add_footerReference(self, type_: WD_HEADER_FOOTER, rId: str) -> CT_HdrFtrRef:
         """Return newly added CT_HdrFtrRef element of `type_` with `rId`.
 
@@ -183,17 +177,15 @@
         if pgMar is None:
             return None
         return pgMar.bottom
 
     @bottom_margin.setter
     def bottom_margin(self, value: int | Length | None):
         pgMar = self.get_or_add_pgMar()
-        pgMar.bottom = (
-            value if value is None or isinstance(value, Length) else Length(value)
-        )
+        pgMar.bottom = value if value is None or isinstance(value, Length) else Length(value)
 
     def clone(self) -> CT_SectPr:
         """Return an exact duplicate of this ``<w:sectPr>`` element tree suitable for
         use in adding a section break.
 
         All rsid* attributes are removed from the root ``<w:sectPr>`` element.
         """
@@ -213,17 +205,15 @@
         if pgMar is None:
             return None
         return pgMar.footer
 
     @footer.setter
     def footer(self, value: int | Length | None):
         pgMar = self.get_or_add_pgMar()
-        pgMar.footer = (
-            value if value is None or isinstance(value, Length) else Length(value)
-        )
+        pgMar.footer = value if value is None or isinstance(value, Length) else Length(value)
 
     def get_footerReference(self, type_: WD_HEADER_FOOTER) -> CT_HdrFtrRef | None:
         """Return footerReference element of `type_` or None if not present."""
         path = "./w:footerReference[@w:type='%s']" % WD_HEADER_FOOTER.to_xml(type_)
         footerReferences = self.xpath(path)
         if not footerReferences:
             return None
@@ -247,17 +237,15 @@
         if pgMar is None:
             return None
         return pgMar.gutter
 
     @gutter.setter
     def gutter(self, value: int | Length | None):
         pgMar = self.get_or_add_pgMar()
-        pgMar.gutter = (
-            value if value is None or isinstance(value, Length) else Length(value)
-        )
+        pgMar.gutter = value if value is None or isinstance(value, Length) else Length(value)
 
     @property
     def header(self) -> Length | None:
         """Distance from top edge of page to top edge of header.
 
         This value comes from the `w:header` attribute on the `w:pgMar` child element.
         |None| if either the element or the attribute is not present.
@@ -266,17 +254,15 @@
         if pgMar is None:
             return None
         return pgMar.header
 
     @header.setter
     def header(self, value: int | Length | None):
         pgMar = self.get_or_add_pgMar()
-        pgMar.header = (
-            value if value is None or isinstance(value, Length) else Length(value)
-        )
+        pgMar.header = value if value is None or isinstance(value, Length) else Length(value)
 
     def iter_inner_content(self) -> Iterator[CT_P | CT_Tbl]:
         """Generate all `w:p` and `w:tbl` elements in this section.
 
         Elements appear in document order. Elements shaded by nesting in a `w:ins` or
         other "wrapper" element will not be included.
         """
@@ -291,17 +277,15 @@
         if pgMar is None:
             return None
         return pgMar.left
 
     @left_margin.setter
     def left_margin(self, value: int | Length | None):
         pgMar = self.get_or_add_pgMar()
-        pgMar.left = (
-            value if value is None or isinstance(value, Length) else Length(value)
-        )
+        pgMar.left = value if value is None or isinstance(value, Length) else Length(value)
 
     @property
     def orientation(self) -> WD_ORIENTATION:
         """`WD_ORIENTATION` member indicating page-orientation for this section.
 
         This is the value of the `orient` attribute on the `w:pgSz` child, or
         `WD_ORIENTATION.PORTRAIT` if not present.
@@ -438,16 +422,16 @@
         pgMar = self.get_or_add_pgMar()
         pgMar.top = value
 
 
 class CT_SectType(BaseOxmlElement):
     """``<w:sectType>`` element, defining the section start type."""
 
-    val: WD_SECTION_START | None = (  # pyright: ignore[reportGeneralTypeIssues]
-        OptionalAttribute("w:val", WD_SECTION_START)
+    val: WD_SECTION_START | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
+        "w:val", WD_SECTION_START
     )
 
 
 # == HELPERS =========================================================================
 
 
 class _SectBlockElementIterator:
```

### Comparing `python-docx-1.1.0/src/docx/oxml/settings.py` & `python_docx-1.1.1/src/docx/oxml/settings.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/oxml/shape.py` & `python_docx-1.1.1/src/docx/oxml/shape.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/oxml/shared.py` & `python_docx-1.1.1/src/docx/oxml/shared.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 class CT_DecimalNumber(BaseOxmlElement):
     """Used for ``<w:numId>``, ``<w:ilvl>``, ``<w:abstractNumId>`` and several others,
     containing a text representation of a decimal number (e.g. 42) in its ``val``
     attribute."""
 
-    val = RequiredAttribute("w:val", ST_DecimalNumber)
+    val: int = RequiredAttribute("w:val", ST_DecimalNumber)  # pyright: ignore[reportAssignmentType]
 
     @classmethod
     def new(cls, nsptagname, val):
         """Return a new ``CT_DecimalNumber`` element having tagname `nsptagname` and
         ``val`` attribute set to `val`."""
         return OxmlElement(nsptagname, attrs={qn("w:val"): str(val)})
 
@@ -38,17 +38,15 @@
 
 class CT_String(BaseOxmlElement):
     """Used for `w:pStyle` and `w:tblStyle` elements and others.
 
     In those cases, it containing a style name in its `val` attribute.
     """
 
-    val: str = RequiredAttribute(  # pyright: ignore[reportGeneralTypeIssues]
-        "w:val", ST_String
-    )
+    val: str = RequiredAttribute("w:val", ST_String)  # pyright: ignore[reportGeneralTypeIssues]
 
     @classmethod
     def new(cls, nsptagname: str, val: str):
         """Return a new ``CT_String`` element with tagname `nsptagname` and ``val``
         attribute set to `val`."""
         elm = cast(CT_String, OxmlElement(nsptagname))
         elm.val = val
```

### Comparing `python-docx-1.1.0/src/docx/oxml/simpletypes.py` & `python_docx-1.1.1/src/docx/oxml/simpletypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,30 +32,26 @@
         return str_value
 
     @classmethod
     def convert_from_xml(cls, str_value: str) -> Any:
         return int(str_value)
 
     @classmethod
-    def convert_to_xml(cls, value: Any) -> str:
-        ...
+    def convert_to_xml(cls, value: Any) -> str: ...
 
     @classmethod
-    def validate(cls, value: Any) -> None:
-        ...
+    def validate(cls, value: Any) -> None: ...
 
     @classmethod
     def validate_int(cls, value: object):
         if not isinstance(value, int):
             raise TypeError("value must be <type 'int'>, got %s" % type(value))
 
     @classmethod
-    def validate_int_in_range(
-        cls, value: int, min_inclusive: int, max_inclusive: int
-    ) -> None:
+    def validate_int_in_range(cls, value: int, min_inclusive: int, max_inclusive: int) -> None:
         cls.validate_int(value)
         if value < min_inclusive or value > max_inclusive:
             raise ValueError(
                 "value must be in range %d to %d inclusive, got %d"
                 % (min_inclusive, max_inclusive, value)
             )
 
@@ -125,16 +121,15 @@
     def convert_to_xml(cls, value: bool) -> str:
         return {True: "1", False: "0"}[value]
 
     @classmethod
     def validate(cls, value: Any) -> None:
         if value not in (True, False):
             raise TypeError(
-                "only True or False (and possibly None) may be assigned, got"
-                " '%s'" % value
+                "only True or False (and possibly None) may be assigned, got" " '%s'" % value
             )
 
 
 class XsdId(BaseStringType):
     """String that must begin with a letter or underscore and cannot contain any colons.
 
     Not fully validated because not used in external API.
@@ -244,16 +239,15 @@
         return "%02X%02X%02X" % value
 
     @classmethod
     def validate(cls, value: Any) -> None:
         # must be an RGBColor object ---
         if not isinstance(value, RGBColor):
             raise ValueError(
-                "rgb color value must be RGBColor object, got %s %s"
-                % (type(value), value)
+                "rgb color value must be RGBColor object, got %s %s" % (type(value), value)
             )
 
 
 class ST_HexColorAuto(XsdStringEnumeration):
     """Value for `w:color/[@val="auto"] attribute setting."""
 
     AUTO = "auto"
@@ -312,15 +306,15 @@
 
 
 class ST_SignedTwipsMeasure(XsdInt):
     @classmethod
     def convert_from_xml(cls, str_value: str) -> Length:
         if "i" in str_value or "m" in str_value or "p" in str_value:
             return ST_UniversalMeasure.convert_from_xml(str_value)
-        return Twips(int(str_value))
+        return Twips(int(round(float(str_value))))
 
     @classmethod
     def convert_to_xml(cls, value: int | Length) -> str:
         emu = Emu(value)
         twips = emu.twips
         return str(twips)
```

### Comparing `python-docx-1.1.0/src/docx/oxml/styles.py` & `python_docx-1.1.1/src/docx/oxml/styles.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/oxml/table.py` & `python_docx-1.1.1/src/docx/oxml/table.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,139 +1,180 @@
 """Custom element classes for tables."""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Callable, List
+from typing import TYPE_CHECKING, Callable, cast
 
-from docx.enum.table import WD_CELL_VERTICAL_ALIGNMENT, WD_ROW_HEIGHT_RULE
+from docx.enum.table import WD_CELL_VERTICAL_ALIGNMENT, WD_ROW_HEIGHT_RULE, WD_TABLE_DIRECTION
 from docx.exceptions import InvalidSpanError
 from docx.oxml.ns import nsdecls, qn
 from docx.oxml.parser import parse_xml
+from docx.oxml.shared import CT_DecimalNumber
 from docx.oxml.simpletypes import (
     ST_Merge,
     ST_TblLayoutType,
     ST_TblWidth,
     ST_TwipsMeasure,
     XsdInt,
 )
+from docx.oxml.text.paragraph import CT_P
 from docx.oxml.xmlchemy import (
     BaseOxmlElement,
     OneAndOnlyOne,
     OneOrMore,
     OptionalAttribute,
     RequiredAttribute,
     ZeroOrMore,
     ZeroOrOne,
 )
-from docx.shared import Emu, Twips
+from docx.shared import Emu, Length, Twips
 
 if TYPE_CHECKING:
-    from docx.oxml.text.paragraph import CT_P
-    from docx.shared import Length
+    from docx.enum.table import WD_TABLE_ALIGNMENT
+    from docx.enum.text import WD_ALIGN_PARAGRAPH
+    from docx.oxml.shared import CT_OnOff, CT_String
+    from docx.oxml.text.parfmt import CT_Jc
 
 
 class CT_Height(BaseOxmlElement):
-    """Used for ``<w:trHeight>`` to specify a row height and row height rule."""
+    """Used for `w:trHeight` to specify a row height and row height rule."""
 
-    val = OptionalAttribute("w:val", ST_TwipsMeasure)
-    hRule = OptionalAttribute("w:hRule", WD_ROW_HEIGHT_RULE)
+    val: Length | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
+        "w:val", ST_TwipsMeasure
+    )
+    hRule: WD_ROW_HEIGHT_RULE | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
+        "w:hRule", WD_ROW_HEIGHT_RULE
+    )
 
 
 class CT_Row(BaseOxmlElement):
     """``<w:tr>`` element."""
 
-    tblPrEx = ZeroOrOne("w:tblPrEx")  # custom inserter below
-    trPr = ZeroOrOne("w:trPr")  # custom inserter below
+    add_tc: Callable[[], CT_Tc]
+    get_or_add_trPr: Callable[[], CT_TrPr]
+    _add_trPr: Callable[[], CT_TrPr]
+
+    tc_lst: list[CT_Tc]
+    # -- custom inserter below --
+    tblPrEx: CT_TblPrEx | None = ZeroOrOne("w:tblPrEx")  # pyright: ignore[reportAssignmentType]
+    # -- custom inserter below --
+    trPr: CT_TrPr | None = ZeroOrOne("w:trPr")  # pyright: ignore[reportAssignmentType]
     tc = ZeroOrMore("w:tc")
 
-    def tc_at_grid_col(self, idx):
-        """The ``<w:tc>`` element appearing at grid column `idx`.
+    @property
+    def grid_after(self) -> int:
+        """The number of unpopulated layout-grid cells at the end of this row."""
+        trPr = self.trPr
+        if trPr is None:
+            return 0
+        return trPr.grid_after
+
+    @property
+    def grid_before(self) -> int:
+        """The number of unpopulated layout-grid cells at the start of this row."""
+        trPr = self.trPr
+        if trPr is None:
+            return 0
+        return trPr.grid_before
+
+    def tc_at_grid_offset(self, grid_offset: int) -> CT_Tc:
+        """The `tc` element in this tr at exact `grid offset`.
 
-        Raises |ValueError| if no ``w:tc`` element begins at that grid column.
+        Raises ValueError when this `w:tr` contains no `w:tc` with exact starting `grid_offset`.
         """
-        grid_col = 0
+        # -- account for omitted cells at the start of the row --
+        remaining_offset = grid_offset - self.grid_before
+
         for tc in self.tc_lst:
-            if grid_col == idx:
+            # -- We've gone past grid_offset without finding a tc, no sense searching further. --
+            if remaining_offset < 0:
+                break
+            # -- We've arrived at grid_offset, this is the `w:tc` we're looking for. --
+            if remaining_offset == 0:
                 return tc
-            grid_col += tc.grid_span
-            if grid_col > idx:
-                raise ValueError("no cell on grid column %d" % idx)
-        raise ValueError("index out of bounds")
+            # -- We're not there yet, skip forward the number of layout-grid cells this cell
+            # -- occupies.
+            remaining_offset -= tc.grid_span
+
+        raise ValueError(f"no `tc` element at grid_offset={grid_offset}")
 
     @property
-    def tr_idx(self):
-        """The index of this ``<w:tr>`` element within its parent ``<w:tbl>``
-        element."""
-        return self.getparent().tr_lst.index(self)
+    def tr_idx(self) -> int:
+        """Index of this `w:tr` element within its parent `w:tbl` element."""
+        tbl = cast(CT_Tbl, self.getparent())
+        return tbl.tr_lst.index(self)
 
     @property
-    def trHeight_hRule(self):
-        """Return the value of `w:trPr/w:trHeight@w:hRule`, or |None| if not present."""
+    def trHeight_hRule(self) -> WD_ROW_HEIGHT_RULE | None:
+        """The value of `./w:trPr/w:trHeight/@w:hRule`, or |None| if not present."""
         trPr = self.trPr
         if trPr is None:
             return None
         return trPr.trHeight_hRule
 
     @trHeight_hRule.setter
-    def trHeight_hRule(self, value):
+    def trHeight_hRule(self, value: WD_ROW_HEIGHT_RULE | None):
         trPr = self.get_or_add_trPr()
         trPr.trHeight_hRule = value
 
     @property
     def trHeight_val(self):
         """Return the value of `w:trPr/w:trHeight@w:val`, or |None| if not present."""
         trPr = self.trPr
         if trPr is None:
             return None
         return trPr.trHeight_val
 
     @trHeight_val.setter
-    def trHeight_val(self, value):
+    def trHeight_val(self, value: Length | None):
         trPr = self.get_or_add_trPr()
         trPr.trHeight_val = value
 
-    def _insert_tblPrEx(self, tblPrEx):
+    def _insert_tblPrEx(self, tblPrEx: CT_TblPrEx):
         self.insert(0, tblPrEx)
 
-    def _insert_trPr(self, trPr):
+    def _insert_trPr(self, trPr: CT_TrPr):
         tblPrEx = self.tblPrEx
         if tblPrEx is not None:
             tblPrEx.addnext(trPr)
         else:
             self.insert(0, trPr)
 
     def _new_tc(self):
         return CT_Tc.new()
 
 
 class CT_Tbl(BaseOxmlElement):
     """``<w:tbl>`` element."""
 
-    tblPr = OneAndOnlyOne("w:tblPr")
-    tblGrid = OneAndOnlyOne("w:tblGrid")
+    add_tr: Callable[[], CT_Row]
+    tr_lst: list[CT_Row]
+
+    tblPr: CT_TblPr = OneAndOnlyOne("w:tblPr")  # pyright: ignore[reportAssignmentType]
+    tblGrid: CT_TblGrid = OneAndOnlyOne("w:tblGrid")  # pyright: ignore[reportAssignmentType]
     tr = ZeroOrMore("w:tr")
 
     @property
-    def bidiVisual_val(self):
-        """Value of `w:tblPr/w:bidiVisual/@w:val` or |None| if not present.
+    def bidiVisual_val(self) -> bool | None:
+        """Value of `./w:tblPr/w:bidiVisual/@w:val` or |None| if not present.
 
         Controls whether table cells are displayed right-to-left or left-to-right.
         """
         bidiVisual = self.tblPr.bidiVisual
         if bidiVisual is None:
             return None
         return bidiVisual.val
 
     @bidiVisual_val.setter
-    def bidiVisual_val(self, value):
+    def bidiVisual_val(self, value: WD_TABLE_DIRECTION | None):
         tblPr = self.tblPr
         if value is None:
-            tblPr._remove_bidiVisual()
+            tblPr._remove_bidiVisual()  # pyright: ignore[reportPrivateUsage]
         else:
-            tblPr.get_or_add_bidiVisual().val = value
+            tblPr.get_or_add_bidiVisual().val = bool(value)
 
     @property
     def col_count(self):
         """The number of grid columns in this table."""
         return len(self.tblGrid.gridCol_lst)
 
     def iter_tcs(self):
@@ -149,119 +190,126 @@
 
     @classmethod
     def new_tbl(cls, rows: int, cols: int, width: Length) -> CT_Tbl:
         """Return a new `w:tbl` element having `rows` rows and `cols` columns.
 
         `width` is distributed evenly between the columns.
         """
-        return parse_xml(cls._tbl_xml(rows, cols, width))
+        return cast(CT_Tbl, parse_xml(cls._tbl_xml(rows, cols, width)))
 
     @property
-    def tblStyle_val(self):
-        """Value of `w:tblPr/w:tblStyle/@w:val` (a table style id) or |None| if not
-        present."""
+    def tblStyle_val(self) -> str | None:
+        """`w:tblPr/w:tblStyle/@w:val` (a table style id) or |None| if not present."""
         tblStyle = self.tblPr.tblStyle
         if tblStyle is None:
             return None
         return tblStyle.val
 
     @tblStyle_val.setter
-    def tblStyle_val(self, styleId):
+    def tblStyle_val(self, styleId: str | None) -> None:
         """Set the value of `w:tblPr/w:tblStyle/@w:val` (a table style id) to `styleId`.
 
         If `styleId` is None, remove the `w:tblStyle` element.
         """
         tblPr = self.tblPr
-        tblPr._remove_tblStyle()
+        tblPr._remove_tblStyle()  # pyright: ignore[reportPrivateUsage]
         if styleId is None:
             return
-        tblPr._add_tblStyle().val = styleId
+        tblPr._add_tblStyle().val = styleId  # pyright: ignore[reportPrivateUsage]
 
     @classmethod
     def _tbl_xml(cls, rows: int, cols: int, width: Length) -> str:
-        col_width = Emu(width / cols) if cols > 0 else Emu(0)
+        col_width = Emu(width // cols) if cols > 0 else Emu(0)
         return (
-            "<w:tbl %s>\n"
-            "  <w:tblPr>\n"
-            '    <w:tblW w:type="auto" w:w="0"/>\n'
-            '    <w:tblLook w:firstColumn="1" w:firstRow="1"\n'
-            '               w:lastColumn="0" w:lastRow="0" w:noHBand="0"\n'
-            '               w:noVBand="1" w:val="04A0"/>\n'
-            "  </w:tblPr>\n"
-            "%s"  # tblGrid
-            "%s"  # trs
-            "</w:tbl>\n"
-        ) % (
-            nsdecls("w"),
-            cls._tblGrid_xml(cols, col_width),
-            cls._trs_xml(rows, cols, col_width),
+            f"<w:tbl {nsdecls('w')}>\n"
+            f"  <w:tblPr>\n"
+            f'    <w:tblW w:type="auto" w:w="0"/>\n'
+            f'    <w:tblLook w:firstColumn="1" w:firstRow="1"\n'
+            f'               w:lastColumn="0" w:lastRow="0" w:noHBand="0"\n'
+            f'               w:noVBand="1" w:val="04A0"/>\n'
+            f"  </w:tblPr>\n"
+            f"{cls._tblGrid_xml(cols, col_width)}"
+            f"{cls._trs_xml(rows, cols, col_width)}"
+            f"</w:tbl>\n"
         )
 
     @classmethod
-    def _tblGrid_xml(cls, col_count, col_width):
+    def _tblGrid_xml(cls, col_count: int, col_width: Length) -> str:
         xml = "  <w:tblGrid>\n"
-        for i in range(col_count):
+        for _ in range(col_count):
             xml += '    <w:gridCol w:w="%d"/>\n' % col_width.twips
         xml += "  </w:tblGrid>\n"
         return xml
 
     @classmethod
-    def _trs_xml(cls, row_count, col_count, col_width):
-        xml = ""
-        for i in range(row_count):
-            xml += ("  <w:tr>\n" "%s" "  </w:tr>\n") % cls._tcs_xml(
-                col_count, col_width
-            )
-        return xml
+    def _trs_xml(cls, row_count: int, col_count: int, col_width: Length) -> str:
+        return f"  <w:tr>\n{cls._tcs_xml(col_count, col_width)}  </w:tr>\n" * row_count
 
     @classmethod
-    def _tcs_xml(cls, col_count, col_width):
-        xml = ""
-        for i in range(col_count):
-            xml += (
-                "    <w:tc>\n"
-                "      <w:tcPr>\n"
-                '        <w:tcW w:type="dxa" w:w="%d"/>\n'
-                "      </w:tcPr>\n"
-                "      <w:p/>\n"
-                "    </w:tc>\n"
-            ) % col_width.twips
-        return xml
+    def _tcs_xml(cls, col_count: int, col_width: Length) -> str:
+        return (
+            f"    <w:tc>\n"
+            f"      <w:tcPr>\n"
+            f'        <w:tcW w:type="dxa" w:w="{col_width.twips}"/>\n'
+            f"      </w:tcPr>\n"
+            f"      <w:p/>\n"
+            f"    </w:tc>\n"
+        ) * col_count
 
 
 class CT_TblGrid(BaseOxmlElement):
-    """``<w:tblGrid>`` element, child of ``<w:tbl>``, holds ``<w:gridCol>`` elements
-    that define column count, width, etc."""
+    """`w:tblGrid` element.
+
+    Child of `w:tbl`, holds `w:gridCol> elements that define column count, width, etc.
+    """
+
+    add_gridCol: Callable[[], CT_TblGridCol]
+    gridCol_lst: list[CT_TblGridCol]
 
     gridCol = ZeroOrMore("w:gridCol", successors=("w:tblGridChange",))
 
 
 class CT_TblGridCol(BaseOxmlElement):
-    """``<w:gridCol>`` element, child of ``<w:tblGrid>``, defines a table column."""
+    """`w:gridCol` element, child of `w:tblGrid`, defines a table column."""
 
-    w = OptionalAttribute("w:w", ST_TwipsMeasure)
+    w: Length | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
+        "w:w", ST_TwipsMeasure
+    )
 
     @property
-    def gridCol_idx(self):
-        """The index of this ``<w:gridCol>`` element within its parent ``<w:tblGrid>``
-        element."""
-        return self.getparent().gridCol_lst.index(self)
+    def gridCol_idx(self) -> int:
+        """Index of this `w:gridCol` element within its parent `w:tblGrid` element."""
+        tblGrid = cast(CT_TblGrid, self.getparent())
+        return tblGrid.gridCol_lst.index(self)
 
 
 class CT_TblLayoutType(BaseOxmlElement):
-    """``<w:tblLayout>`` element, specifying whether column widths are fixed or can be
-    automatically adjusted based on content."""
+    """`w:tblLayout` element.
 
-    type = OptionalAttribute("w:type", ST_TblLayoutType)
+    Specifies whether column widths are fixed or can be automatically adjusted based on
+    content.
+    """
+
+    type: str | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
+        "w:type", ST_TblLayoutType
+    )
 
 
 class CT_TblPr(BaseOxmlElement):
     """``<w:tblPr>`` element, child of ``<w:tbl>``, holds child elements that define
     table properties such as style and borders."""
 
+    get_or_add_bidiVisual: Callable[[], CT_OnOff]
+    get_or_add_jc: Callable[[], CT_Jc]
+    get_or_add_tblLayout: Callable[[], CT_TblLayoutType]
+    _add_tblStyle: Callable[[], CT_String]
+    _remove_bidiVisual: Callable[[], None]
+    _remove_jc: Callable[[], None]
+    _remove_tblStyle: Callable[[], None]
+
     _tag_seq = (
         "w:tblStyle",
         "w:tblpPr",
         "w:tblOverlap",
         "w:bidiVisual",
         "w:tblStyleRowBandSize",
         "w:tblStyleColBandSize",
@@ -274,39 +322,43 @@
         "w:tblLayout",
         "w:tblCellMar",
         "w:tblLook",
         "w:tblCaption",
         "w:tblDescription",
         "w:tblPrChange",
     )
-    tblStyle = ZeroOrOne("w:tblStyle", successors=_tag_seq[1:])
-    bidiVisual = ZeroOrOne("w:bidiVisual", successors=_tag_seq[4:])
-    jc = ZeroOrOne("w:jc", successors=_tag_seq[8:])
-    tblLayout = ZeroOrOne("w:tblLayout", successors=_tag_seq[13:])
+    tblStyle: CT_String | None = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
+        "w:tblStyle", successors=_tag_seq[1:]
+    )
+    bidiVisual: CT_OnOff | None = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
+        "w:bidiVisual", successors=_tag_seq[4:]
+    )
+    jc: CT_Jc | None = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
+        "w:jc", successors=_tag_seq[8:]
+    )
+    tblLayout: CT_TblLayoutType | None = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
+        "w:tblLayout", successors=_tag_seq[13:]
+    )
     del _tag_seq
 
     @property
-    def alignment(self):
-        """Member of :ref:`WdRowAlignment` enumeration or |None|, based on the contents
-        of the `w:val` attribute of `./w:jc`.
-
-        |None| if no `w:jc` element is present.
-        """
+    def alignment(self) -> WD_TABLE_ALIGNMENT | None:
+        """Horizontal alignment of table, |None| if `./w:jc` is not present."""
         jc = self.jc
         if jc is None:
             return None
-        return jc.val
+        return cast("WD_TABLE_ALIGNMENT | None", jc.val)
 
     @alignment.setter
-    def alignment(self, value):
+    def alignment(self, value: WD_TABLE_ALIGNMENT | None):
         self._remove_jc()
         if value is None:
             return
         jc = self.get_or_add_jc()
-        jc.val = value
+        jc.val = cast("WD_ALIGN_PARAGRAPH", value)
 
     @property
     def autofit(self) -> bool:
         """|False| when there is a `w:tblLayout` child with `@w:type="fixed"`.
 
         Otherwise |True|.
         """
@@ -324,103 +376,119 @@
         |None| if not present."""
         tblStyle = self.tblStyle
         if tblStyle is None:
             return None
         return tblStyle.val
 
     @style.setter
-    def style(self, value):
+    def style(self, value: str | None):
         self._remove_tblStyle()
         if value is None:
             return
-        self._add_tblStyle(val=value)
+        self._add_tblStyle().val = value
+
+
+class CT_TblPrEx(BaseOxmlElement):
+    """`w:tblPrEx` element, exceptions to table-properties.
+
+    Applied at a lower level, like a `w:tr` to modify the appearance. Possibly used when
+    two tables are merged. For more see:
+    http://officeopenxml.com/WPtablePropertyExceptions.php
+    """
 
 
 class CT_TblWidth(BaseOxmlElement):
-    """Used for ``<w:tblW>`` and ``<w:tcW>`` elements and many others, to specify a
-    table-related width."""
+    """Used for `w:tblW` and `w:tcW` and others, specifies a table-related width."""
 
     # the type for `w` attr is actually ST_MeasurementOrPercent, but using
     # XsdInt for now because only dxa (twips) values are being used. It's not
     # entirely clear what the semantics are for other values like -01.4mm
-    w = RequiredAttribute("w:w", XsdInt)
+    w: int = RequiredAttribute("w:w", XsdInt)  # pyright: ignore[reportAssignmentType]
     type = RequiredAttribute("w:type", ST_TblWidth)
 
     @property
-    def width(self):
-        """Return the EMU length value represented by the combined ``w:w`` and
-        ``w:type`` attributes."""
+    def width(self) -> Length | None:
+        """EMU length indicated by the combined `w:w` and `w:type` attrs."""
         if self.type != "dxa":
             return None
         return Twips(self.w)
 
     @width.setter
-    def width(self, value):
+    def width(self, value: Length):
         self.type = "dxa"
         self.w = Emu(value).twips
 
 
 class CT_Tc(BaseOxmlElement):
     """`w:tc` table cell element."""
 
     add_p: Callable[[], CT_P]
-    p_lst: List[CT_P]
-    tbl_lst: List[CT_Tbl]
-
+    get_or_add_tcPr: Callable[[], CT_TcPr]
+    p_lst: list[CT_P]
+    tbl_lst: list[CT_Tbl]
     _insert_tbl: Callable[[CT_Tbl], CT_Tbl]
+    _new_p: Callable[[], CT_P]
 
-    tcPr = ZeroOrOne("w:tcPr")  # bunches of successors, overriding insert
+    # -- tcPr has many successors, `._insert_tcPr()` is overridden below --
+    tcPr: CT_TcPr | None = ZeroOrOne("w:tcPr")  # pyright: ignore[reportAssignmentType]
     p = OneOrMore("w:p")
     tbl = OneOrMore("w:tbl")
 
     @property
-    def bottom(self):
+    def bottom(self) -> int:
         """The row index that marks the bottom extent of the vertical span of this cell.
 
         This is one greater than the index of the bottom-most row of the span, similar
         to how a slice of the cell's rows would be specified.
         """
         if self.vMerge is not None:
             tc_below = self._tc_below
             if tc_below is not None and tc_below.vMerge == ST_Merge.CONTINUE:
                 return tc_below.bottom
         return self._tr_idx + 1
 
     def clear_content(self):
-        """Remove all content child elements, preserving the ``<w:tcPr>`` element if
-        present.
+        """Remove all content elements, preserving `w:tcPr` element if present.
 
-        Note that this leaves the ``<w:tc>`` element in an invalid state because it
-        doesn't contain at least one block-level element. It's up to the caller to add a
-        ``<w:p>``child element as the last content element.
+        Note that this leaves the `w:tc` element in an invalid state because it doesn't
+        contain at least one block-level element. It's up to the caller to add a
+        `w:p`child element as the last content element.
         """
-        new_children = []
-        tcPr = self.tcPr
-        if tcPr is not None:
-            new_children.append(tcPr)
-        self[:] = new_children
+        # -- remove all cell inner-content except a `w:tcPr` when present. --
+        for e in self.xpath("./*[not(self::w:tcPr)]"):
+            self.remove(e)
 
     @property
-    def grid_span(self):
+    def grid_offset(self) -> int:
+        """Starting offset of `tc` in the layout-grid columns of its table.
+
+        A cell in the leftmost grid-column has offset 0.
+        """
+        grid_before = self._tr.grid_before
+        preceding_tc_grid_spans = sum(
+            tc.grid_span for tc in self.xpath("./preceding-sibling::w:tc")
+        )
+        return grid_before + preceding_tc_grid_spans
+
+    @property
+    def grid_span(self) -> int:
         """The integer number of columns this cell spans.
 
         Determined by ./w:tcPr/w:gridSpan/@val, it defaults to 1.
         """
         tcPr = self.tcPr
-        if tcPr is None:
-            return 1
-        return tcPr.grid_span
+        return 1 if tcPr is None else tcPr.grid_span
 
     @grid_span.setter
-    def grid_span(self, value):
+    def grid_span(self, value: int):
         tcPr = self.get_or_add_tcPr()
         tcPr.grid_span = value
 
     @property
-    def inner_content_elements(self) -> List[CT_P | CT_Tbl]:
+    def inner_content_elements(self) -> list[CT_P | CT_Tbl]:
         """Generate all `w:p` and `w:tbl` elements in this document-body.
 
         Elements appear in document order. Elements shaded by nesting in a `w:ins` or
         other "wrapper" element will not be included.
         """
         return self.xpath("./w:p | ./w:tbl")
 
@@ -429,179 +497,183 @@
         cell, in the order they appear."""
         block_item_tags = (qn("w:p"), qn("w:tbl"), qn("w:sdt"))
         for child in self:
             if child.tag in block_item_tags:
                 yield child
 
     @property
-    def left(self):
+    def left(self) -> int:
         """The grid column index at which this ``<w:tc>`` element appears."""
-        return self._grid_col
+        return self.grid_offset
+
+    def merge(self, other_tc: CT_Tc) -> CT_Tc:
+        """Return top-left `w:tc` element of a new span.
 
-    def merge(self, other_tc):
-        """Return the top-left ``<w:tc>`` element of a new span formed by merging the
-        rectangular region defined by using this tc element and `other_tc` as diagonal
-        corners."""
+        Span is formed by merging the rectangular region defined by using this tc
+        element and `other_tc` as diagonal corners.
+        """
         top, left, height, width = self._span_dimensions(other_tc)
-        top_tc = self._tbl.tr_lst[top].tc_at_grid_col(left)
+        top_tc = self._tbl.tr_lst[top].tc_at_grid_offset(left)
         top_tc._grow_to(width, height)
         return top_tc
 
     @classmethod
-    def new(cls):
-        """Return a new ``<w:tc>`` element, containing an empty paragraph as the
-        required EG_BlockLevelElt."""
-        return parse_xml("<w:tc %s>\n" "  <w:p/>\n" "</w:tc>" % nsdecls("w"))
+    def new(cls) -> CT_Tc:
+        """A new `w:tc` element, containing an empty paragraph as the required EG_BlockLevelElt."""
+        return cast(CT_Tc, parse_xml("<w:tc %s>\n" "  <w:p/>\n" "</w:tc>" % nsdecls("w")))
 
     @property
-    def right(self):
+    def right(self) -> int:
         """The grid column index that marks the right-side extent of the horizontal span
         of this cell.
 
         This is one greater than the index of the right-most column of the span, similar
         to how a slice of the cell's columns would be specified.
         """
-        return self._grid_col + self.grid_span
+        return self.grid_offset + self.grid_span
 
     @property
-    def top(self):
+    def top(self) -> int:
         """The top-most row index in the vertical span of this cell."""
         if self.vMerge is None or self.vMerge == ST_Merge.RESTART:
             return self._tr_idx
         return self._tc_above.top
 
     @property
-    def vMerge(self):
-        """The value of the ./w:tcPr/w:vMerge/@val attribute, or |None| if the w:vMerge
-        element is not present."""
+    def vMerge(self) -> str | None:
+        """Value of ./w:tcPr/w:vMerge/@val, |None| if w:vMerge is not present."""
         tcPr = self.tcPr
         if tcPr is None:
             return None
         return tcPr.vMerge_val
 
     @vMerge.setter
-    def vMerge(self, value):
+    def vMerge(self, value: str | None):
         tcPr = self.get_or_add_tcPr()
         tcPr.vMerge_val = value
 
     @property
-    def width(self):
-        """Return the EMU length value represented in the ``./w:tcPr/w:tcW`` child
-        element or |None| if not present."""
+    def width(self) -> Length | None:
+        """EMU length represented in `./w:tcPr/w:tcW` or |None| if not present."""
         tcPr = self.tcPr
         if tcPr is None:
             return None
         return tcPr.width
 
     @width.setter
-    def width(self, value):
+    def width(self, value: Length):
         tcPr = self.get_or_add_tcPr()
         tcPr.width = value
 
-    def _add_width_of(self, other_tc):
+    def _add_width_of(self, other_tc: CT_Tc):
         """Add the width of `other_tc` to this cell.
 
         Does nothing if either this tc or `other_tc` does not have a specified width.
         """
         if self.width and other_tc.width:
-            self.width += other_tc.width
+            self.width = Length(self.width + other_tc.width)
 
-    @property
-    def _grid_col(self):
-        """The grid column at which this cell begins."""
-        tr = self._tr
-        idx = tr.tc_lst.index(self)
-        preceding_tcs = tr.tc_lst[:idx]
-        return sum(tc.grid_span for tc in preceding_tcs)
-
-    def _grow_to(self, width, height, top_tc=None):
-        """Grow this cell to `width` grid columns and `height` rows by expanding
-        horizontal spans and creating continuation cells to form vertical spans."""
-
-        def vMerge_val(top_tc):
-            if top_tc is not self:
-                return ST_Merge.CONTINUE
-            if height == 1:
-                return None
-            return ST_Merge.RESTART
+    def _grow_to(self, width: int, height: int, top_tc: CT_Tc | None = None):
+        """Grow this cell to `width` grid columns and `height` rows.
+
+        This is accomplished by expanding horizontal spans and creating continuation
+        cells to form vertical spans.
+        """
+
+        def vMerge_val(top_tc: CT_Tc):
+            return (
+                ST_Merge.CONTINUE
+                if top_tc is not self
+                else None if height == 1 else ST_Merge.RESTART
+            )
 
         top_tc = self if top_tc is None else top_tc
         self._span_to_width(width, top_tc, vMerge_val(top_tc))
         if height > 1:
-            self._tc_below._grow_to(width, height - 1, top_tc)
+            tc_below = self._tc_below
+            assert tc_below is not None
+            tc_below._grow_to(width, height - 1, top_tc)
 
-    def _insert_tcPr(self, tcPr):
-        """``tcPr`` has a bunch of successors, but it comes first if it appears, so just
-        overriding and using insert(0, ...) rather than spelling out successors."""
+    def _insert_tcPr(self, tcPr: CT_TcPr) -> CT_TcPr:
+        """Override default `._insert_tcPr()`."""
+        # -- `tcPr`` has a large number of successors, but always comes first if it appears,
+        # -- so just using insert(0, ...) rather than spelling out successors.
         self.insert(0, tcPr)
         return tcPr
 
     @property
-    def _is_empty(self):
-        """True if this cell contains only a single empty ``<w:p>`` element."""
+    def _is_empty(self) -> bool:
+        """True if this cell contains only a single empty `w:p` element."""
         block_items = list(self.iter_block_items())
         if len(block_items) > 1:
             return False
-        p = block_items[0]  # cell must include at least one <w:p> element
-        if len(p.r_lst) == 0:
+        # -- cell must include at least one block item but can be a `w:tbl`, `w:sdt`,
+        # -- `w:customXml` or a `w:p`
+        only_item = block_items[0]
+        if isinstance(only_item, CT_P) and len(only_item.r_lst) == 0:
             return True
         return False
 
-    def _move_content_to(self, other_tc):
-        """Append the content of this cell to `other_tc`, leaving this cell with a
-        single empty ``<w:p>`` element."""
+    def _move_content_to(self, other_tc: CT_Tc):
+        """Append the content of this cell to `other_tc`.
+
+        Leaves this cell with a single empty ``<w:p>`` element.
+        """
         if other_tc is self:
             return
         if self._is_empty:
             return
         other_tc._remove_trailing_empty_p()
-        # appending moves each element from self to other_tc
+        # -- appending moves each element from self to other_tc --
         for block_element in self.iter_block_items():
             other_tc.append(block_element)
-        # add back the required minimum single empty <w:p> element
+        # -- add back the required minimum single empty <w:p> element --
         self.append(self._new_p())
 
-    def _new_tbl(self):
-        return CT_Tbl.new()
+    def _new_tbl(self) -> None:
+        raise NotImplementedError(
+            "use CT_Tbl.new_tbl() to add a new table, specifying rows and columns"
+        )
 
     @property
-    def _next_tc(self):
+    def _next_tc(self) -> CT_Tc | None:
         """The `w:tc` element immediately following this one in this row, or |None| if
         this is the last `w:tc` element in the row."""
         following_tcs = self.xpath("./following-sibling::w:tc")
         return following_tcs[0] if following_tcs else None
 
     def _remove(self):
         """Remove this `w:tc` element from the XML tree."""
-        self.getparent().remove(self)
+        parent_element = self.getparent()
+        assert parent_element is not None
+        parent_element.remove(self)
 
     def _remove_trailing_empty_p(self):
-        """Remove the last content element from this cell if it is an empty ``<w:p>``
-        element."""
+        """Remove last content element from this cell if it's an empty `w:p` element."""
         block_items = list(self.iter_block_items())
         last_content_elm = block_items[-1]
-        if last_content_elm.tag != qn("w:p"):
+        if not isinstance(last_content_elm, CT_P):
             return
         p = last_content_elm
         if len(p.r_lst) > 0:
             return
         self.remove(p)
 
-    def _span_dimensions(self, other_tc):
+    def _span_dimensions(self, other_tc: CT_Tc) -> tuple[int, int, int, int]:
         """Return a (top, left, height, width) 4-tuple specifying the extents of the
         merged cell formed by using this tc and `other_tc` as opposite corner
         extents."""
 
-        def raise_on_inverted_L(a, b):
+        def raise_on_inverted_L(a: CT_Tc, b: CT_Tc):
             if a.top == b.top and a.bottom != b.bottom:
                 raise InvalidSpanError("requested span not rectangular")
             if a.left == b.left and a.right != b.right:
                 raise InvalidSpanError("requested span not rectangular")
 
-        def raise_on_tee_shaped(a, b):
+        def raise_on_tee_shaped(a: CT_Tc, b: CT_Tc):
             top_most, other = (a, b) if a.top < b.top else (b, a)
             if top_most.top < other.top and top_most.bottom > other.bottom:
                 raise InvalidSpanError("requested span not rectangular")
 
             left_most, other = (a, b) if a.left < b.left else (b, a)
             if left_most.left < other.left and left_most.right > other.right:
                 raise InvalidSpanError("requested span not rectangular")
@@ -612,109 +684,118 @@
         top = min(self.top, other_tc.top)
         left = min(self.left, other_tc.left)
         bottom = max(self.bottom, other_tc.bottom)
         right = max(self.right, other_tc.right)
 
         return top, left, bottom - top, right - left
 
-    def _span_to_width(self, grid_width, top_tc, vMerge):
-        """Incorporate and then remove `w:tc` elements to the right of this one until
-        this cell spans `grid_width`.
+    def _span_to_width(self, grid_width: int, top_tc: CT_Tc, vMerge: str | None):
+        """Incorporate `w:tc` elements to the right until this cell spans `grid_width`.
+
+        Incorporated `w:tc` elements are removed (replaced by gridSpan value).
 
         Raises |ValueError| if `grid_width` cannot be exactly achieved, such as when a
         merged cell would drive the span width greater than `grid_width` or if not
         enough grid columns are available to make this cell that wide. All content from
         incorporated cells is appended to `top_tc`. The val attribute of the vMerge
         element on the single remaining cell is set to `vMerge`. If `vMerge` is |None|,
         the vMerge element is removed if present.
         """
         self._move_content_to(top_tc)
         while self.grid_span < grid_width:
             self._swallow_next_tc(grid_width, top_tc)
         self.vMerge = vMerge
 
-    def _swallow_next_tc(self, grid_width, top_tc):
+    def _swallow_next_tc(self, grid_width: int, top_tc: CT_Tc):
         """Extend the horizontal span of this `w:tc` element to incorporate the
         following `w:tc` element in the row and then delete that following `w:tc`
         element.
 
         Any content in the following `w:tc` element is appended to the content of
         `top_tc`. The width of the following `w:tc` element is added to this one, if
         present. Raises |InvalidSpanError| if the width of the resulting cell is greater
         than `grid_width` or if there is no next `<w:tc>` element in the row.
         """
 
-        def raise_on_invalid_swallow(next_tc):
+        def raise_on_invalid_swallow(next_tc: CT_Tc | None):
             if next_tc is None:
                 raise InvalidSpanError("not enough grid columns")
             if self.grid_span + next_tc.grid_span > grid_width:
                 raise InvalidSpanError("span is not rectangular")
 
         next_tc = self._next_tc
         raise_on_invalid_swallow(next_tc)
+        assert next_tc is not None
         next_tc._move_content_to(top_tc)
         self._add_width_of(next_tc)
         self.grid_span += next_tc.grid_span
         next_tc._remove()
 
     @property
-    def _tbl(self):
+    def _tbl(self) -> CT_Tbl:
         """The tbl element this tc element appears in."""
-        return self.xpath("./ancestor::w:tbl[position()=1]")[0]
+        return cast(CT_Tbl, self.xpath("./ancestor::w:tbl[position()=1]")[0])
 
     @property
-    def _tc_above(self):
+    def _tc_above(self) -> CT_Tc:
         """The `w:tc` element immediately above this one in its grid column."""
-        return self._tr_above.tc_at_grid_col(self._grid_col)
+        return self._tr_above.tc_at_grid_offset(self.grid_offset)
 
     @property
-    def _tc_below(self):
+    def _tc_below(self) -> CT_Tc | None:
         """The tc element immediately below this one in its grid column."""
         tr_below = self._tr_below
         if tr_below is None:
             return None
-        return tr_below.tc_at_grid_col(self._grid_col)
+        return tr_below.tc_at_grid_offset(self.grid_offset)
 
     @property
-    def _tr(self):
+    def _tr(self) -> CT_Row:
         """The tr element this tc element appears in."""
-        return self.xpath("./ancestor::w:tr[position()=1]")[0]
+        return cast(CT_Row, self.xpath("./ancestor::w:tr[position()=1]")[0])
 
     @property
-    def _tr_above(self):
+    def _tr_above(self) -> CT_Row:
         """The tr element prior in sequence to the tr this cell appears in.
 
         Raises |ValueError| if called on a cell in the top-most row.
         """
-        tr_lst = self._tbl.tr_lst
-        tr_idx = tr_lst.index(self._tr)
-        if tr_idx == 0:
-            raise ValueError("no tr above topmost tr")
-        return tr_lst[tr_idx - 1]
+        tr_aboves = self.xpath("./ancestor::w:tr[position()=1]/preceding-sibling::w:tr[1]")
+        if not tr_aboves:
+            raise ValueError("no tr above topmost tr in w:tbl")
+        return tr_aboves[0]
 
     @property
-    def _tr_below(self):
+    def _tr_below(self) -> CT_Row | None:
         """The tr element next in sequence after the tr this cell appears in, or |None|
         if this cell appears in the last row."""
         tr_lst = self._tbl.tr_lst
         tr_idx = tr_lst.index(self._tr)
         try:
             return tr_lst[tr_idx + 1]
         except IndexError:
             return None
 
     @property
-    def _tr_idx(self):
+    def _tr_idx(self) -> int:
         """The row index of the tr element this tc element appears in."""
         return self._tbl.tr_lst.index(self._tr)
 
 
 class CT_TcPr(BaseOxmlElement):
     """``<w:tcPr>`` element, defining table cell properties."""
 
+    get_or_add_gridSpan: Callable[[], CT_DecimalNumber]
+    get_or_add_tcW: Callable[[], CT_TblWidth]
+    get_or_add_vAlign: Callable[[], CT_VerticalJc]
+    _add_vMerge: Callable[[], CT_VMerge]
+    _remove_gridSpan: Callable[[], None]
+    _remove_vAlign: Callable[[], None]
+    _remove_vMerge: Callable[[], None]
+
     _tag_seq = (
         "w:cnfStyle",
         "w:tcW",
         "w:gridSpan",
         "w:hMerge",
         "w:vMerge",
         "w:tcBorders",
@@ -727,33 +808,39 @@
         "w:hideMark",
         "w:headers",
         "w:cellIns",
         "w:cellDel",
         "w:cellMerge",
         "w:tcPrChange",
     )
-    tcW = ZeroOrOne("w:tcW", successors=_tag_seq[2:])
-    gridSpan = ZeroOrOne("w:gridSpan", successors=_tag_seq[3:])
-    vMerge = ZeroOrOne("w:vMerge", successors=_tag_seq[5:])
-    vAlign = ZeroOrOne("w:vAlign", successors=_tag_seq[12:])
+    tcW: CT_TblWidth | None = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
+        "w:tcW", successors=_tag_seq[2:]
+    )
+    gridSpan: CT_DecimalNumber | None = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
+        "w:gridSpan", successors=_tag_seq[3:]
+    )
+    vMerge: CT_VMerge | None = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
+        "w:vMerge", successors=_tag_seq[5:]
+    )
+    vAlign: CT_VerticalJc | None = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
+        "w:vAlign", successors=_tag_seq[12:]
+    )
     del _tag_seq
 
     @property
-    def grid_span(self):
+    def grid_span(self) -> int:
         """The integer number of columns this cell spans.
 
         Determined by ./w:gridSpan/@val, it defaults to 1.
         """
         gridSpan = self.gridSpan
-        if gridSpan is None:
-            return 1
-        return gridSpan.val
+        return 1 if gridSpan is None else gridSpan.val
 
     @grid_span.setter
-    def grid_span(self, value):
+    def grid_span(self, value: int):
         self._remove_gridSpan()
         if value > 1:
             self.get_or_add_gridSpan().val = value
 
     @property
     def vAlign_val(self):
         """Value of `w:val` attribute on  `w:vAlign` child.
@@ -763,15 +850,15 @@
         """
         vAlign = self.vAlign
         if vAlign is None:
             return None
         return vAlign.val
 
     @vAlign_val.setter
-    def vAlign_val(self, value):
+    def vAlign_val(self, value: WD_CELL_VERTICAL_ALIGNMENT | None):
         if value is None:
             self._remove_vAlign()
             return
         self.get_or_add_vAlign().val = value
 
     @property
     def vMerge_val(self):
@@ -779,37 +866,38 @@
         is not present."""
         vMerge = self.vMerge
         if vMerge is None:
             return None
         return vMerge.val
 
     @vMerge_val.setter
-    def vMerge_val(self, value):
+    def vMerge_val(self, value: str | None):
         self._remove_vMerge()
         if value is not None:
             self._add_vMerge().val = value
 
     @property
-    def width(self):
-        """Return the EMU length value represented in the ``<w:tcW>`` child element or
-        |None| if not present or its type is not 'dxa'."""
+    def width(self) -> Length | None:
+        """EMU length in `./w:tcW` or |None| if not present or its type is not 'dxa'."""
         tcW = self.tcW
         if tcW is None:
             return None
         return tcW.width
 
     @width.setter
-    def width(self, value):
+    def width(self, value: Length):
         tcW = self.get_or_add_tcW()
         tcW.width = value
 
 
 class CT_TrPr(BaseOxmlElement):
     """``<w:trPr>`` element, defining table row properties."""
 
+    get_or_add_trHeight: Callable[[], CT_Height]
+
     _tag_seq = (
         "w:cnfStyle",
         "w:divId",
         "w:gridBefore",
         "w:gridAfter",
         "w:wBefore",
         "w:wAfter",
@@ -819,51 +907,71 @@
         "w:tblCellSpacing",
         "w:jc",
         "w:hidden",
         "w:ins",
         "w:del",
         "w:trPrChange",
     )
-    trHeight = ZeroOrOne("w:trHeight", successors=_tag_seq[8:])
+    gridAfter: CT_DecimalNumber | None = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
+        "w:gridAfter", successors=_tag_seq[4:]
+    )
+    gridBefore: CT_DecimalNumber | None = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
+        "w:gridBefore", successors=_tag_seq[3:]
+    )
+    trHeight: CT_Height | None = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
+        "w:trHeight", successors=_tag_seq[8:]
+    )
     del _tag_seq
 
     @property
-    def trHeight_hRule(self):
+    def grid_after(self) -> int:
+        """The number of unpopulated layout-grid cells at the end of this row."""
+        gridAfter = self.gridAfter
+        return 0 if gridAfter is None else gridAfter.val
+
+    @property
+    def grid_before(self) -> int:
+        """The number of unpopulated layout-grid cells at the start of this row."""
+        gridBefore = self.gridBefore
+        return 0 if gridBefore is None else gridBefore.val
+
+    @property
+    def trHeight_hRule(self) -> WD_ROW_HEIGHT_RULE | None:
         """Return the value of `w:trHeight@w:hRule`, or |None| if not present."""
         trHeight = self.trHeight
-        if trHeight is None:
-            return None
-        return trHeight.hRule
+        return None if trHeight is None else trHeight.hRule
 
     @trHeight_hRule.setter
-    def trHeight_hRule(self, value):
+    def trHeight_hRule(self, value: WD_ROW_HEIGHT_RULE | None):
         if value is None and self.trHeight is None:
             return
         trHeight = self.get_or_add_trHeight()
         trHeight.hRule = value
 
     @property
     def trHeight_val(self):
         """Return the value of `w:trHeight@w:val`, or |None| if not present."""
         trHeight = self.trHeight
-        if trHeight is None:
-            return None
-        return trHeight.val
+        return None if trHeight is None else trHeight.val
 
     @trHeight_val.setter
-    def trHeight_val(self, value):
+    def trHeight_val(self, value: Length | None):
         if value is None and self.trHeight is None:
             return
         trHeight = self.get_or_add_trHeight()
         trHeight.val = value
 
 
 class CT_VerticalJc(BaseOxmlElement):
     """`w:vAlign` element, specifying vertical alignment of cell."""
 
-    val = RequiredAttribute("w:val", WD_CELL_VERTICAL_ALIGNMENT)
+    val: WD_CELL_VERTICAL_ALIGNMENT = RequiredAttribute(  # pyright: ignore[reportAssignmentType]
+        "w:val", WD_CELL_VERTICAL_ALIGNMENT
+    )
 
 
 class CT_VMerge(BaseOxmlElement):
     """``<w:vMerge>`` element, specifying vertical merging behavior of a cell."""
 
-    val = OptionalAttribute("w:val", ST_Merge, default=ST_Merge.CONTINUE)
+    val: str | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
+        "w:val", ST_Merge, default=ST_Merge.CONTINUE  # pyright: ignore[reportArgumentType]
+    )
```

### Comparing `python-docx-1.1.0/src/docx/oxml/text/font.py` & `python_docx-1.1.1/src/docx/oxml/text/font.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/oxml/text/hyperlink.py` & `python_docx-1.1.1/src/docx/oxml/text/hyperlink.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,29 +17,29 @@
 
 
 class CT_Hyperlink(BaseOxmlElement):
     """`<w:hyperlink>` element, containing the text and address for a hyperlink."""
 
     r_lst: List[CT_R]
 
-    rId: str | None = OptionalAttribute(  # pyright: ignore[reportGeneralTypeIssues]
-        "r:id", XsdString
-    )
-    anchor: str | None = OptionalAttribute(  # pyright: ignore[reportGeneralTypeIssues]
+    rId: str | None = OptionalAttribute("r:id", XsdString)  # pyright: ignore[reportAssignmentType]
+    anchor: str | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
         "w:anchor", ST_String
     )
-    history = OptionalAttribute("w:history", ST_OnOff, default=True)
+    history: bool = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
+        "w:history", ST_OnOff, default=True
+    )
 
     r = ZeroOrMore("w:r")
 
     @property
     def lastRenderedPageBreaks(self) -> List[CT_LastRenderedPageBreak]:
         """All `w:lastRenderedPageBreak` descendants of this hyperlink."""
         return self.xpath("./w:r/w:lastRenderedPageBreak")
 
-    @property  # pyright: ignore[reportIncompatibleVariableOverride]
-    def text(self) -> str:
+    @property
+    def text(self) -> str:  # pyright: ignore[reportIncompatibleMethodOverride]
         """The textual content of this hyperlink.
 
         `CT_Hyperlink` stores the hyperlink-text as one or more `w:r` children.
         """
         return "".join(r.text for r in self.xpath("w:r"))
```

### Comparing `python-docx-1.1.0/src/docx/oxml/text/pagebreak.py` & `python_docx-1.1.1/src/docx/oxml/text/pagebreak.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/oxml/text/paragraph.py` & `python_docx-1.1.1/src/docx/oxml/text/paragraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     """`<w:p>` element, containing the properties and text for a paragraph."""
 
     add_r: Callable[[], CT_R]
     get_or_add_pPr: Callable[[], CT_PPr]
     hyperlink_lst: List[CT_Hyperlink]
     r_lst: List[CT_R]
 
-    pPr: CT_PPr | None = ZeroOrOne("w:pPr")  # pyright: ignore[reportGeneralTypeIssues]
+    pPr: CT_PPr | None = ZeroOrOne("w:pPr")  # pyright: ignore[reportAssignmentType]
     hyperlink = ZeroOrMore("w:hyperlink")
     r = ZeroOrMore("w:r")
 
     def add_p_before(self) -> CT_P:
         """Return a new `<w:p>` element inserted directly prior to this one."""
         new_p = cast(CT_P, OxmlElement("w:p"))
         self.addprevious(new_p)
@@ -88,16 +88,16 @@
         return pPr.style
 
     @style.setter
     def style(self, style: str | None):
         pPr = self.get_or_add_pPr()
         pPr.style = style
 
-    @property  # pyright: ignore[reportIncompatibleVariableOverride]
-    def text(self):
+    @property
+    def text(self):  # pyright: ignore[reportIncompatibleMethodOverride]
         """The textual content of this paragraph.
 
         Inner-content child elements like `w:r` and `w:hyperlink` are translated to
         their text equivalent.
         """
         return "".join(e.text for e in self.xpath("w:r | w:hyperlink"))
```

### Comparing `python-docx-1.1.0/src/docx/oxml/text/parfmt.py` & `python_docx-1.1.1/src/docx/oxml/text/parfmt.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,29 +24,40 @@
     from docx.oxml.section import CT_SectPr
     from docx.oxml.shared import CT_String
 
 
 class CT_Ind(BaseOxmlElement):
     """``<w:ind>`` element, specifying paragraph indentation."""
 
-    left = OptionalAttribute("w:left", ST_SignedTwipsMeasure)
-    right = OptionalAttribute("w:right", ST_SignedTwipsMeasure)
-    firstLine = OptionalAttribute("w:firstLine", ST_TwipsMeasure)
-    hanging = OptionalAttribute("w:hanging", ST_TwipsMeasure)
+    left: Length | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
+        "w:left", ST_SignedTwipsMeasure
+    )
+    right: Length | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
+        "w:right", ST_SignedTwipsMeasure
+    )
+    firstLine: Length | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
+        "w:firstLine", ST_TwipsMeasure
+    )
+    hanging: Length | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
+        "w:hanging", ST_TwipsMeasure
+    )
 
 
 class CT_Jc(BaseOxmlElement):
     """``<w:jc>`` element, specifying paragraph justification."""
 
-    val = RequiredAttribute("w:val", WD_ALIGN_PARAGRAPH)
+    val: WD_ALIGN_PARAGRAPH = RequiredAttribute(  # pyright: ignore[reportAssignmentType]
+        "w:val", WD_ALIGN_PARAGRAPH
+    )
 
 
 class CT_PPr(BaseOxmlElement):
     """``<w:pPr>`` element, containing the properties for a paragraph."""
 
+    get_or_add_ind: Callable[[], CT_Ind]
     get_or_add_pStyle: Callable[[], CT_String]
     _insert_sectPr: Callable[[CT_SectPr], None]
     _remove_pStyle: Callable[[], None]
     _remove_sectPr: Callable[[], None]
 
     _tag_seq = (
         "w:pStyle",
@@ -82,31 +93,33 @@
         "w:outlineLvl",
         "w:divId",
         "w:cnfStyle",
         "w:rPr",
         "w:sectPr",
         "w:pPrChange",
     )
-    pStyle: CT_String | None = ZeroOrOne(  # pyright: ignore[reportGeneralTypeIssues]
+    pStyle: CT_String | None = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
         "w:pStyle", successors=_tag_seq[1:]
     )
     keepNext = ZeroOrOne("w:keepNext", successors=_tag_seq[2:])
     keepLines = ZeroOrOne("w:keepLines", successors=_tag_seq[3:])
     pageBreakBefore = ZeroOrOne("w:pageBreakBefore", successors=_tag_seq[4:])
     widowControl = ZeroOrOne("w:widowControl", successors=_tag_seq[6:])
     numPr = ZeroOrOne("w:numPr", successors=_tag_seq[7:])
     tabs = ZeroOrOne("w:tabs", successors=_tag_seq[11:])
     spacing = ZeroOrOne("w:spacing", successors=_tag_seq[22:])
-    ind = ZeroOrOne("w:ind", successors=_tag_seq[23:])
+    ind: CT_Ind | None = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
+        "w:ind", successors=_tag_seq[23:]
+    )
     jc = ZeroOrOne("w:jc", successors=_tag_seq[27:])
     sectPr = ZeroOrOne("w:sectPr", successors=_tag_seq[35:])
     del _tag_seq
 
     @property
-    def first_line_indent(self):
+    def first_line_indent(self) -> Length | None:
         """A |Length| value calculated from the values of `w:ind/@w:firstLine` and
         `w:ind/@w:hanging`.
 
         Returns |None| if the `w:ind` child is not present.
         """
         ind = self.ind
         if ind is None:
@@ -116,51 +129,51 @@
             return Length(-hanging)
         firstLine = ind.firstLine
         if firstLine is None:
             return None
         return firstLine
 
     @first_line_indent.setter
-    def first_line_indent(self, value):
+    def first_line_indent(self, value: Length | None):
         if self.ind is None and value is None:
             return
         ind = self.get_or_add_ind()
         ind.firstLine = ind.hanging = None
         if value is None:
             return
         elif value < 0:
             ind.hanging = -value
         else:
             ind.firstLine = value
 
     @property
-    def ind_left(self):
+    def ind_left(self) -> Length | None:
         """The value of `w:ind/@w:left` or |None| if not present."""
         ind = self.ind
         if ind is None:
             return None
         return ind.left
 
     @ind_left.setter
-    def ind_left(self, value):
+    def ind_left(self, value: Length | None):
         if value is None and self.ind is None:
             return
         ind = self.get_or_add_ind()
         ind.left = value
 
     @property
-    def ind_right(self):
+    def ind_right(self) -> Length | None:
         """The value of `w:ind/@w:right` or |None| if not present."""
         ind = self.ind
         if ind is None:
             return None
         return ind.right
 
     @ind_right.setter
-    def ind_right(self, value):
+    def ind_right(self, value: Length | None):
         if value is None and self.ind is None:
             return
         ind = self.get_or_add_ind()
         ind.right = value
 
     @property
     def jc_val(self) -> WD_ALIGN_PARAGRAPH | None:
@@ -334,17 +347,23 @@
 class CT_TabStop(BaseOxmlElement):
     """`<w:tab>` element, representing an individual tab stop.
 
     Overloaded to use for a tab-character in a run, which also uses the w:tab tag but
     only needs a __str__ method.
     """
 
-    val = RequiredAttribute("w:val", WD_TAB_ALIGNMENT)
-    leader = OptionalAttribute("w:leader", WD_TAB_LEADER, default=WD_TAB_LEADER.SPACES)
-    pos = RequiredAttribute("w:pos", ST_SignedTwipsMeasure)
+    val: WD_TAB_ALIGNMENT = RequiredAttribute(  # pyright: ignore[reportAssignmentType]
+        "w:val", WD_TAB_ALIGNMENT
+    )
+    leader: WD_TAB_LEADER | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
+        "w:leader", WD_TAB_LEADER, default=WD_TAB_LEADER.SPACES
+    )
+    pos: Length = RequiredAttribute(  # pyright: ignore[reportAssignmentType]
+        "w:pos", ST_SignedTwipsMeasure
+    )
 
     def __str__(self) -> str:
         """Text equivalent of a `w:tab` element appearing in a run.
 
         Allows text of run inner-content to be accessed consistently across all text
         inner-content.
         """
```

### Comparing `python-docx-1.1.0/src/docx/oxml/text/run.py` & `python_docx-1.1.1/src/docx/oxml/text/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     add_br: Callable[[], CT_Br]
     add_tab: Callable[[], CT_TabStop]
     get_or_add_rPr: Callable[[], CT_RPr]
     _add_drawing: Callable[[], CT_Drawing]
     _add_t: Callable[..., CT_Text]
 
-    rPr: CT_RPr | None = ZeroOrOne("w:rPr")  # pyright: ignore[reportGeneralTypeIssues]
+    rPr: CT_RPr | None = ZeroOrOne("w:rPr")  # pyright: ignore[reportAssignmentType]
     br = ZeroOrMore("w:br")
     cr = ZeroOrMore("w:cr")
     drawing = ZeroOrMore("w:drawing")
     t = ZeroOrMore("w:t")
     tab = ZeroOrMore("w:tab")
 
     def add_t(self, text: str) -> CT_Text:
@@ -116,20 +116,19 @@
     def text(self) -> str:
         """The textual content of this run.
 
         Inner-content child elements like `w:tab` are translated to their text
         equivalent.
         """
         return "".join(
-            str(e)
-            for e in self.xpath("w:br | w:cr | w:noBreakHyphen | w:ptab | w:t | w:tab")
+            str(e) for e in self.xpath("w:br | w:cr | w:noBreakHyphen | w:ptab | w:t | w:tab")
         )
 
-    @text.setter  # pyright: ignore[reportIncompatibleVariableOverride]
-    def text(self, text: str):
+    @text.setter
+    def text(self, text: str):  # pyright: ignore[reportIncompatibleMethodOverride]
         self.clear_content()
         _RunContentAppender.append_to_run_from_text(self, text)
 
     def _insert_rPr(self, rPr: CT_RPr) -> CT_RPr:
         self.insert(0, rPr)
         return rPr
 
@@ -137,20 +136,18 @@
 # ------------------------------------------------------------------------------------
 # Run inner-content elements
 
 
 class CT_Br(BaseOxmlElement):
     """`<w:br>` element, indicating a line, page, or column break in a run."""
 
-    type: str | None = OptionalAttribute(  # pyright: ignore[reportGeneralTypeIssues]
+    type: str | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
         "w:type", ST_BrType, default="textWrapping"
     )
-    clear: str | None = OptionalAttribute(  # pyright: ignore[reportGeneralTypeIssues]
-        "w:clear", ST_BrClear
-    )
+    clear: str | None = OptionalAttribute("w:clear", ST_BrClear)  # pyright: ignore
 
     def __str__(self) -> str:
         """Text equivalent of this element. Actual value depends on break type.
 
         A line break is translated as "\n". Column and page breaks produce the empty
         string ("").
```

### Comparing `python-docx-1.1.0/src/docx/oxml/xmlchemy.py` & `python_docx-1.1.1/src/docx/oxml/xmlchemy.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,24 +122,20 @@
 
 class BaseAttribute:
     """Base class for OptionalAttribute and RequiredAttribute.
 
     Provides common methods.
     """
 
-    def __init__(
-        self, attr_name: str, simple_type: Type[BaseXmlEnum] | Type[BaseSimpleType]
-    ):
+    def __init__(self, attr_name: str, simple_type: Type[BaseXmlEnum] | Type[BaseSimpleType]):
         super(BaseAttribute, self).__init__()
         self._attr_name = attr_name
         self._simple_type = simple_type
 
-    def populate_class_members(
-        self, element_cls: MetaOxmlElement, prop_name: str
-    ) -> None:
+    def populate_class_members(self, element_cls: MetaOxmlElement, prop_name: str) -> None:
         """Add the appropriate methods to `element_cls`."""
         self._element_cls = element_cls
         self._prop_name = prop_name
 
         self._add_attr_property()
 
     def _add_attr_property(self):
@@ -155,37 +151,35 @@
     @property
     def _clark_name(self):
         if ":" in self._attr_name:
             return qn(self._attr_name)
         return self._attr_name
 
     @property
-    def _getter(self) -> Callable[[BaseOxmlElement], Any | None]:
-        ...
+    def _getter(self) -> Callable[[BaseOxmlElement], Any | None]: ...
 
     @property
     def _setter(
         self,
-    ) -> Callable[[BaseOxmlElement, Any | None], None]:
-        ...
+    ) -> Callable[[BaseOxmlElement, Any | None], None]: ...
 
 
 class OptionalAttribute(BaseAttribute):
     """Defines an optional attribute on a custom element class.
 
     An optional attribute returns a default value when not present for reading. When
     assigned |None|, the attribute is removed, but still returns the default value when
     one is specified.
     """
 
     def __init__(
         self,
         attr_name: str,
         simple_type: Type[BaseXmlEnum] | Type[BaseSimpleType],
-        default: BaseXmlEnum | BaseSimpleType | None = None,
+        default: BaseXmlEnum | BaseSimpleType | str | bool | None = None,
     ):
         super(OptionalAttribute, self).__init__(attr_name, simple_type)
         self._default = default
 
     @property
     def _docstring(self):
         """String to use as `__doc__` attribute of attribute property."""
@@ -255,16 +249,15 @@
     def _getter(self) -> Callable[[BaseOxmlElement], Any]:
         """function object suitable for "get" side of attr property descriptor."""
 
         def get_attr_value(obj: BaseOxmlElement) -> Any | None:
             attr_str_value = obj.get(self._clark_name)
             if attr_str_value is None:
                 raise InvalidXmlError(
-                    "required '%s' attribute not present on element %s"
-                    % (self._attr_name, obj.tag)
+                    "required '%s' attribute not present on element %s" % (self._attr_name, obj.tag)
                 )
             return self._simple_type.from_xml(attr_str_value)
 
         get_attr_value.__doc__ = self._docstring
         return get_attr_value
 
     @property
@@ -288,17 +281,15 @@
     """
 
     def __init__(self, nsptagname: str, successors: Tuple[str, ...] = ()):
         super(_BaseChildElement, self).__init__()
         self._nsptagname = nsptagname
         self._successors = successors
 
-    def populate_class_members(
-        self, element_cls: MetaOxmlElement, prop_name: str
-    ) -> None:
+    def populate_class_members(self, element_cls: MetaOxmlElement, prop_name: str) -> None:
         """Baseline behavior for adding the appropriate methods to `element_cls`."""
         self._element_cls = element_cls
         self._prop_name = prop_name
 
     def _add_adder(self):
         """Add an ``_add_x()`` method to the element class for this child element."""
 
@@ -504,17 +495,15 @@
 
 class OneAndOnlyOne(_BaseChildElement):
     """Defines a required child element for MetaOxmlElement."""
 
     def __init__(self, nsptagname: str):
         super(OneAndOnlyOne, self).__init__(nsptagname, ())
 
-    def populate_class_members(
-        self, element_cls: MetaOxmlElement, prop_name: str
-    ) -> None:
+    def populate_class_members(self, element_cls: MetaOxmlElement, prop_name: str) -> None:
         """Add the appropriate methods to `element_cls`."""
         super(OneAndOnlyOne, self).populate_class_members(element_cls, prop_name)
         self._add_getter()
 
     @property
     def _getter(self):
         """Return a function object suitable for the "get" side of the property
@@ -524,59 +513,51 @@
             child = obj.find(qn(self._nsptagname))
             if child is None:
                 raise InvalidXmlError(
                     "required ``<%s>`` child element not present" % self._nsptagname
                 )
             return child
 
-        get_child_element.__doc__ = (
-            "Required ``<%s>`` child element." % self._nsptagname
-        )
+        get_child_element.__doc__ = "Required ``<%s>`` child element." % self._nsptagname
         return get_child_element
 
 
 class OneOrMore(_BaseChildElement):
     """Defines a repeating child element for MetaOxmlElement that must appear at least
     once."""
 
-    def populate_class_members(
-        self, element_cls: MetaOxmlElement, prop_name: str
-    ) -> None:
+    def populate_class_members(self, element_cls: MetaOxmlElement, prop_name: str) -> None:
         """Add the appropriate methods to `element_cls`."""
         super(OneOrMore, self).populate_class_members(element_cls, prop_name)
         self._add_list_getter()
         self._add_creator()
         self._add_inserter()
         self._add_adder()
         self._add_public_adder()
         delattr(element_cls, prop_name)
 
 
 class ZeroOrMore(_BaseChildElement):
     """Defines an optional repeating child element for MetaOxmlElement."""
 
-    def populate_class_members(
-        self, element_cls: MetaOxmlElement, prop_name: str
-    ) -> None:
+    def populate_class_members(self, element_cls: MetaOxmlElement, prop_name: str) -> None:
         """Add the appropriate methods to `element_cls`."""
         super(ZeroOrMore, self).populate_class_members(element_cls, prop_name)
         self._add_list_getter()
         self._add_creator()
         self._add_inserter()
         self._add_adder()
         self._add_public_adder()
         delattr(element_cls, prop_name)
 
 
 class ZeroOrOne(_BaseChildElement):
     """Defines an optional child element for MetaOxmlElement."""
 
-    def populate_class_members(
-        self, element_cls: MetaOxmlElement, prop_name: str
-    ) -> None:
+    def populate_class_members(self, element_cls: MetaOxmlElement, prop_name: str) -> None:
         """Add the appropriate methods to `element_cls`."""
         super(ZeroOrOne, self).populate_class_members(element_cls, prop_name)
         self._add_getter()
         self._add_creator()
         self._add_inserter()
         self._add_adder()
         self._add_get_or_adder()
@@ -600,17 +581,15 @@
 
     def _add_remover(self):
         """Add a ``_remove_x()`` method to the element class for this child element."""
 
         def _remove_child(obj: BaseOxmlElement):
             obj.remove_all(self._nsptagname)
 
-        _remove_child.__doc__ = (
-            "Remove all ``<%s>`` child elements."
-        ) % self._nsptagname
+        _remove_child.__doc__ = ("Remove all ``<%s>`` child elements.") % self._nsptagname
         self._add_to_class(self._remove_method_name, _remove_child)
 
     @lazyproperty
     def _get_or_add_method_name(self):
         return "get_or_add_%s" % self._prop_name
 
 
@@ -618,24 +597,20 @@
     """Correspondes to an ``EG_*`` element group where at most one of its members may
     appear as a child."""
 
     def __init__(self, choices: Sequence[Choice], successors: Tuple[str, ...] = ()):
         self._choices = choices
         self._successors = successors
 
-    def populate_class_members(
-        self, element_cls: MetaOxmlElement, prop_name: str
-    ) -> None:
+    def populate_class_members(self, element_cls: MetaOxmlElement, prop_name: str) -> None:
         """Add the appropriate methods to `element_cls`."""
         super(ZeroOrOneChoice, self).populate_class_members(element_cls, prop_name)
         self._add_choice_getter()
         for choice in self._choices:
-            choice.populate_class_members(
-                element_cls, self._prop_name, self._successors
-            )
+            choice.populate_class_members(element_cls, self._prop_name, self._successors)
         self._add_group_remover()
 
     def _add_choice_getter(self):
         """Add a read-only ``{prop_name}`` property to the element class that returns
         the present member of this group, or |None| if none are present."""
         property_ = property(self._choice_getter, None, None)
         # assign unconditionally to overwrite element name definition
@@ -645,17 +620,15 @@
         """Add a ``_remove_eg_x()`` method to the element class for this choice
         group."""
 
         def _remove_choice_group(obj: BaseOxmlElement):
             for tagname in self._member_nsptagnames:
                 obj.remove_all(tagname)
 
-        _remove_choice_group.__doc__ = (
-            "Remove the current choice group child element if present."
-        )
+        _remove_choice_group.__doc__ = "Remove the current choice group child element if present."
         self._add_to_class(self._remove_choice_group_method_name, _remove_choice_group)
 
     @property
     def _choice_getter(self):
         """Return a function object suitable for the "get" side of the property
         descriptor."""
 
@@ -676,17 +649,15 @@
 
     @lazyproperty
     def _remove_choice_group_method_name(self):
         return "_remove_%s" % self._prop_name
 
 
 # -- lxml typing isn't quite right here, just ignore this error on _Element --
-class BaseOxmlElement(  # pyright: ignore[reportGeneralTypeIssues]
-    etree.ElementBase, metaclass=MetaOxmlElement
-):
+class BaseOxmlElement(etree.ElementBase, metaclass=MetaOxmlElement):
     """Effective base class for all custom element classes.
 
     Adds standardized behavior to all classes in one place.
     """
 
     def __repr__(self):
         return "<%s '<%s>' at 0x%0x>" % (
@@ -722,17 +693,15 @@
     def xml(self) -> str:
         """XML string for this element, suitable for testing purposes.
 
         Pretty printed for readability and without an XML declaration at the top.
         """
         return serialize_for_reading(self)
 
-    def xpath(  # pyright: ignore[reportIncompatibleMethodOverride]
-        self, xpath_str: str
-    ) -> Any:
+    def xpath(self, xpath_str: str) -> Any:  # pyright: ignore[reportIncompatibleMethodOverride]
         """Override of `lxml` _Element.xpath() method.
 
         Provides standard Open XML namespace mapping (`nsmap`) in centralized location.
         """
         return super().xpath(xpath_str, namespaces=nsmap)
 
     @property
```

### Comparing `python-docx-1.1.0/src/docx/package.py` & `python_docx-1.1.1/src/docx/package.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/parts/document.py` & `python_docx-1.1.1/src/docx/parts/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from docx.parts.settings import SettingsPart
 from docx.parts.story import StoryPart
 from docx.parts.styles import StylesPart
 from docx.shape import InlineShapes
 from docx.shared import lazyproperty
 
 if TYPE_CHECKING:
+    from docx.opc.coreprops import CoreProperties
     from docx.styles.style import BaseStyle
 
 
 class DocumentPart(StoryPart):
     """Main document part of a WordprocessingML (WML) package, aka a .docx file.
 
     Acts as broker to other parts such as image, core properties, and style parts. It
@@ -37,15 +38,15 @@
     def add_header_part(self):
         """Return (header_part, rId) pair for newly-created header part."""
         header_part = HeaderPart.new(self.package)
         rId = self.relate_to(header_part, RT.HEADER)
         return header_part, rId
 
     @property
-    def core_properties(self):
+    def core_properties(self) -> CoreProperties:
         """A |CoreProperties| object providing read/write access to the core properties
         of this document."""
         return self.package.core_properties
 
     @property
     def document(self):
         """A |Document| object providing access to the content of this document."""
```

### Comparing `python-docx-1.1.0/src/docx/parts/hdrftr.py` & `python_docx-1.1.1/src/docx/parts/hdrftr.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/parts/image.py` & `python_docx-1.1.1/src/docx/parts/image.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/parts/numbering.py` & `python_docx-1.1.1/src/docx/parts/numbering.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/parts/settings.py` & `python_docx-1.1.1/src/docx/parts/settings.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/parts/story.py` & `python_docx-1.1.1/src/docx/parts/story.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/parts/styles.py` & `python_docx-1.1.1/src/docx/parts/styles.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/section.py` & `python_docx-1.1.1/src/docx/section.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/settings.py` & `python_docx-1.1.1/src/docx/settings.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/shape.py` & `python_docx-1.1.1/src/docx/shape.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/shared.py` & `python_docx-1.1.1/src/docx/shared.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     List,
     Tuple,
     TypeVar,
     cast,
 )
 
 if TYPE_CHECKING:
-    from docx import types as t
+    import docx.types as t
     from docx.opc.part import XmlPart
     from docx.oxml.xmlchemy import BaseOxmlElement
     from docx.parts.story import StoryPart
 
 
 class Length(int):
     """Base class for length constructor classes Inches, Cm, Mm, Px, and Emu.
@@ -280,17 +280,15 @@
     """Base class for lxml element proxy classes.
 
     An element proxy class is one whose primary responsibilities are fulfilled by
     manipulating the attributes and child elements of an XML element. They are the most
     common type of class in python-docx other than custom element (oxml) classes.
     """
 
-    def __init__(
-        self, element: BaseOxmlElement, parent: t.ProvidesXmlPart | None = None
-    ):
+    def __init__(self, element: BaseOxmlElement, parent: t.ProvidesXmlPart | None = None):
         self._element = element
         self._parent = parent
 
     def __eq__(self, other: object):
         """Return |True| if this proxy object refers to the same oxml element as does
         `other`.
```

### Comparing `python-docx-1.1.0/src/docx/styles/__init__.py` & `python_docx-1.1.1/src/docx/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/styles/latent.py` & `python_docx-1.1.1/src/docx/styles/latent.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/styles/style.py` & `python_docx-1.1.1/src/docx/styles/style.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/styles/styles.py` & `python_docx-1.1.1/src/docx/styles/styles.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/table.py` & `python_docx-1.1.1/src/docx/table.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 """The |Table| object and related proxy classes."""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, List, Tuple, overload
+from typing import TYPE_CHECKING, Iterator, cast, overload
+
+from typing_extensions import TypeAlias
 
 from docx.blkcntnr import BlockItemContainer
 from docx.enum.style import WD_STYLE_TYPE
+from docx.enum.table import WD_CELL_VERTICAL_ALIGNMENT
 from docx.oxml.simpletypes import ST_Merge
-from docx.shared import Inches, Parented, lazyproperty
+from docx.oxml.table import CT_TblGridCol
+from docx.shared import Inches, Parented, StoryChild, lazyproperty
 
 if TYPE_CHECKING:
-    from docx import types as t
-    from docx.enum.table import WD_TABLE_ALIGNMENT, WD_TABLE_DIRECTION
-    from docx.oxml.table import CT_Tbl, CT_TblPr
+    import docx.types as t
+    from docx.enum.table import WD_ROW_HEIGHT_RULE, WD_TABLE_ALIGNMENT, WD_TABLE_DIRECTION
+    from docx.oxml.table import CT_Row, CT_Tbl, CT_TblPr, CT_Tc
     from docx.shared import Length
-    from docx.styles.style import _TableStyle  # pyright: ignore[reportPrivateUsage]
+    from docx.styles.style import (
+        ParagraphStyle,
+        _TableStyle,  # pyright: ignore[reportPrivateUsage]
+    )
+
+TableParent: TypeAlias = "Table | _Columns | _Rows"
 
 
-class Table(Parented):
+class Table(StoryChild):
     """Proxy class for a WordprocessingML ``<w:tbl>`` element."""
 
-    def __init__(self, tbl: CT_Tbl, parent: t.StoryChild):
+    def __init__(self, tbl: CT_Tbl, parent: t.ProvidesStoryPart):
         super(Table, self).__init__(parent)
-        self._element = self._tbl = tbl
+        self._element = tbl
+        self._tbl = tbl
 
     def add_column(self, width: Length):
         """Return a |_Column| object of `width`, newly added rightmost to the table."""
         tblGrid = self._tbl.tblGrid
         gridCol = tblGrid.add_gridCol()
         gridCol.w = width
         for tr in self._tbl.tr_lst:
@@ -36,15 +46,16 @@
 
     def add_row(self):
         """Return a |_Row| instance, newly added bottom-most to the table."""
         tbl = self._tbl
         tr = tbl.add_tr()
         for gridCol in tbl.tblGrid.gridCol_lst:
             tc = tr.add_tc()
-            tc.width = gridCol.w
+            if gridCol.w is not None:
+                tc.width = gridCol.w
         return _Row(tr, self)
 
     @property
     def alignment(self) -> WD_TABLE_ALIGNMENT | None:
         """Read/write.
 
         A member of :ref:`WdRowAlignment` or None, specifying the positioning of this
@@ -75,27 +86,30 @@
         """|_Cell| at `row_idx`, `col_idx` intersection.
 
         (0, 0) is the top, left-most cell.
         """
         cell_idx = col_idx + (row_idx * self._column_count)
         return self._cells[cell_idx]
 
-    def column_cells(self, column_idx: int) -> List[_Cell]:
+    def column_cells(self, column_idx: int) -> list[_Cell]:
         """Sequence of cells in the column at `column_idx` in this table."""
         cells = self._cells
         idxs = range(column_idx, len(cells), self._column_count)
         return [cells[idx] for idx in idxs]
 
     @lazyproperty
     def columns(self):
         """|_Columns| instance representing the sequence of columns in this table."""
         return _Columns(self._tbl, self)
 
-    def row_cells(self, row_idx: int) -> List[_Cell]:
-        """Sequence of cells in the row at `row_idx` in this table."""
+    def row_cells(self, row_idx: int) -> list[_Cell]:
+        """DEPRECATED: Use `table.rows[row_idx].cells` instead.
+
+        Sequence of cells in the row at `row_idx` in this table.
+        """
         column_count = self._column_count
         start = row_idx * column_count
         end = start + column_count
         return self._cells[start:end]
 
     @lazyproperty
     def rows(self) -> _Rows:
@@ -112,18 +126,18 @@
         default table style of the document.
 
         Note that the style name of a table style differs slightly from that displayed
         in the user interface; a hyphen, if it appears, must be removed. For example,
         `Light Shading - Accent 1` becomes `Light Shading Accent 1`.
         """
         style_id = self._tbl.tblStyle_val
-        return self.part.get_style(style_id, WD_STYLE_TYPE.TABLE)
+        return cast("_TableStyle | None", self.part.get_style(style_id, WD_STYLE_TYPE.TABLE))
 
     @style.setter
-    def style(self, style_or_name: _TableStyle | None):
+    def style(self, style_or_name: _TableStyle | str | None):
         style_id = self.part.get_style_id(style_or_name, WD_STYLE_TYPE.TABLE)
         self._tbl.tblStyle_val = style_id
 
     @property
     def table(self):
         """Provide child objects with reference to the |Table| object they belong to,
         without them having to know their direct parent is a |Table| object.
@@ -136,29 +150,29 @@
     @property
     def table_direction(self) -> WD_TABLE_DIRECTION | None:
         """Member of :ref:`WdTableDirection` indicating cell-ordering direction.
 
         For example: `WD_TABLE_DIRECTION.LTR`. |None| indicates the value is inherited
         from the style hierarchy.
         """
-        return self._element.bidiVisual_val
+        return cast("WD_TABLE_DIRECTION | None", self._tbl.bidiVisual_val)
 
     @table_direction.setter
     def table_direction(self, value: WD_TABLE_DIRECTION | None):
         self._element.bidiVisual_val = value
 
     @property
-    def _cells(self) -> List[_Cell]:
+    def _cells(self) -> list[_Cell]:
         """A sequence of |_Cell| objects, one for each cell of the layout grid.
 
         If the table contains a span, one or more |_Cell| object references are
         repeated.
         """
         col_count = self._column_count
-        cells = []
+        cells: list[_Cell] = []
         for tc in self._tbl.iter_tcs():
             for grid_span_idx in range(tc.grid_span):
                 if tc.vMerge == ST_Merge.CONTINUE:
                     cells.append(cells[-col_count])
                 elif grid_span_idx > 0:
                     cells.append(cells[-1])
                 else:
@@ -174,44 +188,57 @@
     def _tblPr(self) -> CT_TblPr:
         return self._tbl.tblPr
 
 
 class _Cell(BlockItemContainer):
     """Table cell."""
 
-    def __init__(self, tc, parent):
-        super(_Cell, self).__init__(tc, parent)
+    def __init__(self, tc: CT_Tc, parent: TableParent):
+        super(_Cell, self).__init__(tc, cast("t.ProvidesStoryPart", parent))
+        self._parent = parent
         self._tc = self._element = tc
 
-    def add_paragraph(self, text="", style=None):
+    def add_paragraph(self, text: str = "", style: str | ParagraphStyle | None = None):
         """Return a paragraph newly added to the end of the content in this cell.
 
         If present, `text` is added to the paragraph in a single run. If specified, the
         paragraph style `style` is applied. If `style` is not specified or is |None|,
         the result is as though the 'Normal' style was applied. Note that the formatting
         of text in a cell can be influenced by the table style. `text` can contain tab
         (``\\t``) characters, which are converted to the appropriate XML form for a tab.
         `text` can also include newline (``\\n``) or carriage return (``\\r``)
         characters, each of which is converted to a line break.
         """
         return super(_Cell, self).add_paragraph(text, style)
 
-    def add_table(self, rows, cols):
-        """Return a table newly added to this cell after any existing cell content,
-        having `rows` rows and `cols` columns.
+    def add_table(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, rows: int, cols: int
+    ) -> Table:
+        """Return a table newly added to this cell after any existing cell content.
+
+        The new table will have `rows` rows and `cols` columns.
 
         An empty paragraph is added after the table because Word requires a paragraph
         element as the last element in every cell.
         """
         width = self.width if self.width is not None else Inches(1)
         table = super(_Cell, self).add_table(rows, cols, width)
         self.add_paragraph()
         return table
 
-    def merge(self, other_cell):
+    @property
+    def grid_span(self) -> int:
+        """Number of layout-grid cells this cell spans horizontally.
+
+        A "normal" cell has a grid-span of 1. A horizontally merged cell has a grid-span of 2 or
+        more.
+        """
+        return self._tc.grid_span
+
+    def merge(self, other_cell: _Cell):
         """Return a merged cell created by spanning the rectangular region having this
         cell and `other_cell` as diagonal corners.
 
         Raises |InvalidSpanError| if the cells do not define a rectangular region.
         """
         tc, tc_2 = self._tc, other_cell._tc
         merged_tc = tc.merge(tc_2)
@@ -240,15 +267,15 @@
 
         Assigning a string to this property replaces all existing content with a single
         paragraph containing the assigned text in a single run.
         """
         return "\n".join(p.text for p in self.paragraphs)
 
     @text.setter
-    def text(self, text):
+    def text(self, text: str):
         """Write-only.
 
         Set entire contents of cell to the string `text`. Any existing content or
         revisions are replaced.
         """
         tc = self._tc
         tc.clear_content()
@@ -266,71 +293,73 @@
         """
         tcPr = self._element.tcPr
         if tcPr is None:
             return None
         return tcPr.vAlign_val
 
     @vertical_alignment.setter
-    def vertical_alignment(self, value):
+    def vertical_alignment(self, value: WD_CELL_VERTICAL_ALIGNMENT | None):
         tcPr = self._element.get_or_add_tcPr()
         tcPr.vAlign_val = value
 
     @property
     def width(self):
         """The width of this cell in EMU, or |None| if no explicit width is set."""
         return self._tc.width
 
     @width.setter
-    def width(self, value):
+    def width(self, value: Length):
         self._tc.width = value
 
 
 class _Column(Parented):
     """Table column."""
 
-    def __init__(self, gridCol, parent):
+    def __init__(self, gridCol: CT_TblGridCol, parent: TableParent):
         super(_Column, self).__init__(parent)
+        self._parent = parent
         self._gridCol = gridCol
 
     @property
-    def cells(self):
+    def cells(self) -> tuple[_Cell, ...]:
         """Sequence of |_Cell| instances corresponding to cells in this column."""
         return tuple(self.table.column_cells(self._index))
 
     @property
-    def table(self):
+    def table(self) -> Table:
         """Reference to the |Table| object this column belongs to."""
         return self._parent.table
 
     @property
-    def width(self):
+    def width(self) -> Length | None:
         """The width of this column in EMU, or |None| if no explicit width is set."""
         return self._gridCol.w
 
     @width.setter
-    def width(self, value):
+    def width(self, value: Length | None):
         self._gridCol.w = value
 
     @property
     def _index(self):
         """Index of this column in its table, starting from zero."""
         return self._gridCol.gridCol_idx
 
 
 class _Columns(Parented):
     """Sequence of |_Column| instances corresponding to the columns in a table.
 
     Supports ``len()``, iteration and indexed access.
     """
 
-    def __init__(self, tbl, parent):
+    def __init__(self, tbl: CT_Tbl, parent: TableParent):
         super(_Columns, self).__init__(parent)
+        self._parent = parent
         self._tbl = tbl
 
-    def __getitem__(self, idx):
+    def __getitem__(self, idx: int):
         """Provide indexed access, e.g. 'columns[0]'."""
         try:
             gridCol = self._gridCol_lst[idx]
         except IndexError:
             msg = "column index [%d] is out of range" % idx
             raise IndexError(msg)
         return _Column(gridCol, self)
@@ -339,94 +368,170 @@
         for gridCol in self._gridCol_lst:
             yield _Column(gridCol, self)
 
     def __len__(self):
         return len(self._gridCol_lst)
 
     @property
-    def table(self):
+    def table(self) -> Table:
         """Reference to the |Table| object this column collection belongs to."""
         return self._parent.table
 
     @property
     def _gridCol_lst(self):
         """Sequence containing ``<w:gridCol>`` elements for this table, each
         representing a table column."""
         tblGrid = self._tbl.tblGrid
         return tblGrid.gridCol_lst
 
 
 class _Row(Parented):
     """Table row."""
 
-    def __init__(self, tr, parent):
+    def __init__(self, tr: CT_Row, parent: TableParent):
         super(_Row, self).__init__(parent)
+        self._parent = parent
         self._tr = self._element = tr
 
     @property
-    def cells(self) -> Tuple[_Cell]:
-        """Sequence of |_Cell| instances corresponding to cells in this row."""
-        return tuple(self.table.row_cells(self._index))
+    def cells(self) -> tuple[_Cell, ...]:
+        """Sequence of |_Cell| instances corresponding to cells in this row.
+
+        Note that Word allows table rows to start later than the first column and end before the
+        last column.
+
+        - Only cells actually present are included in the return value.
+        - This implies the length of this cell sequence may differ between rows of the same table.
+        - If you are reading the cells from each row to form a rectangular "matrix" data structure
+          of the table cell values, you will need to account for empty leading and/or trailing
+          layout-grid positions using `.grid_cols_before` and `.grid_cols_after`.
+
+        """
+
+        def iter_tc_cells(tc: CT_Tc) -> Iterator[_Cell]:
+            """Generate a cell object for each layout-grid cell in `tc`.
+
+            In particular, a `<w:tc>` element with a horizontal "span" with generate the same cell
+            multiple times, one for each grid-cell being spanned. This approximates a row in a
+            "uniform" table, where each row has a cell for each column in the table.
+            """
+            # -- a cell comprising the second or later row of a vertical span is indicated by
+            # -- tc.vMerge="continue" (the default value of the `w:vMerge` attribute, when it is
+            # -- present in the XML). The `w:tc` element at the same grid-offset in the prior row
+            # -- is guaranteed to be the same width (gridSpan). So we can delegate content
+            # -- discovery to that prior-row `w:tc` element (recursively) until we arrive at the
+            # -- "root" cell -- for the vertical span.
+            if tc.vMerge == "continue":
+                yield from iter_tc_cells(tc._tc_above)  # pyright: ignore[reportPrivateUsage]
+                return
+
+            # -- Otherwise, vMerge is either "restart" or None, meaning this `tc` holds the actual
+            # -- content of the cell (whether it is vertically merged or not).
+            cell = _Cell(tc, self.table)
+            for _ in range(tc.grid_span):
+                yield cell
+
+        def _iter_row_cells() -> Iterator[_Cell]:
+            """Generate `_Cell` instance for each populated layout-grid cell in this row."""
+            for tc in self._tr.tc_lst:
+                yield from iter_tc_cells(tc)
+
+        return tuple(_iter_row_cells())
+
+    @property
+    def grid_cols_after(self) -> int:
+        """Count of unpopulated grid-columns after the last cell in this row.
+
+        Word allows a row to "end early", meaning that one or more cells are not present at the
+        end of that row.
+
+        Note these are not simply "empty" cells. The renderer reads this value and "skips" this
+        many columns after drawing the last cell.
+
+        Note this also implies that not all rows are guaranteed to have the same number of cells,
+        e.g. `_Row.cells` could have length `n` for one row and `n - m` for the next row in the same
+        table. Visually this appears as a column (at the beginning or end, not in the middle) with
+        one or more cells missing.
+        """
+        return self._tr.grid_after
 
     @property
-    def height(self):
+    def grid_cols_before(self) -> int:
+        """Count of unpopulated grid-columns before the first cell in this row.
+
+        Word allows a row to "start late", meaning that one or more cells are not present at the
+        beginning of that row.
+
+        Note these are not simply "empty" cells. The renderer reads this value and skips forward to
+        the table layout-grid position of the first cell in this row; the renderer "skips" this many
+        columns before drawing the first cell.
+
+        Note this also implies that not all rows are guaranteed to have the same number of cells,
+        e.g. `_Row.cells` could have length `n` for one row and `n - m` for the next row in the same
+        table.
+        """
+        return self._tr.grid_before
+
+    @property
+    def height(self) -> Length | None:
         """Return a |Length| object representing the height of this cell, or |None| if
         no explicit height is set."""
         return self._tr.trHeight_val
 
     @height.setter
-    def height(self, value):
+    def height(self, value: Length | None):
         self._tr.trHeight_val = value
 
     @property
-    def height_rule(self):
-        """Return the height rule of this cell as a member of the :ref:`WdRowHeightRule`
-        enumeration, or |None| if no explicit height_rule is set."""
+    def height_rule(self) -> WD_ROW_HEIGHT_RULE | None:
+        """Return the height rule of this cell as a member of the :ref:`WdRowHeightRule`.
+
+        This value is |None| if no explicit height_rule is set.
+        """
         return self._tr.trHeight_hRule
 
     @height_rule.setter
-    def height_rule(self, value):
+    def height_rule(self, value: WD_ROW_HEIGHT_RULE | None):
         self._tr.trHeight_hRule = value
 
     @property
-    def table(self):
+    def table(self) -> Table:
         """Reference to the |Table| object this row belongs to."""
         return self._parent.table
 
     @property
-    def _index(self):
+    def _index(self) -> int:
         """Index of this row in its table, starting from zero."""
         return self._tr.tr_idx
 
 
 class _Rows(Parented):
     """Sequence of |_Row| objects corresponding to the rows in a table.
 
     Supports ``len()``, iteration, indexed access, and slicing.
     """
 
-    def __init__(self, tbl, parent):
+    def __init__(self, tbl: CT_Tbl, parent: TableParent):
         super(_Rows, self).__init__(parent)
+        self._parent = parent
         self._tbl = tbl
 
     @overload
-    def __getitem__(self, idx: int) -> _Row:
-        ...
+    def __getitem__(self, idx: int) -> _Row: ...
 
     @overload
-    def __getitem__(self, idx: slice) -> List[_Row]:
-        ...
+    def __getitem__(self, idx: slice) -> list[_Row]: ...
 
-    def __getitem__(self, idx: int | slice) -> _Row | List[_Row]:
+    def __getitem__(self, idx: int | slice) -> _Row | list[_Row]:
         """Provide indexed access, (e.g. `rows[0]` or `rows[1:3]`)"""
         return list(self)[idx]
 
     def __iter__(self):
         return (_Row(tr, self) for tr in self._tbl.tr_lst)
 
     def __len__(self):
         return len(self._tbl.tr_lst)
 
     @property
-    def table(self):
+    def table(self) -> Table:
         """Reference to the |Table| object this row collection belongs to."""
         return self._parent.table
```

### Comparing `python-docx-1.1.0/src/docx/templates/default-docx-template/[Content_Types].xml` & `python_docx-1.1.1/src/docx/templates/default-docx-template/[Content_Types].xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/templates/default-docx-template/_rels/.rels` & `python_docx-1.1.1/src/docx/templates/default-docx-template/_rels/.rels`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/templates/default-docx-template/docProps/app.xml` & `python_docx-1.1.1/src/docx/templates/default-docx-template/docProps/app.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/templates/default-docx-template/docProps/core.xml` & `python_docx-1.1.1/src/docx/templates/default-docx-template/docProps/core.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/templates/default-docx-template/docProps/thumbnail.jpeg` & `python_docx-1.1.1/src/docx/templates/default-docx-template/docProps/thumbnail.jpeg`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/templates/default-docx-template/word/_rels/document.xml.rels` & `python_docx-1.1.1/src/docx/templates/default-docx-template/word/_rels/document.xml.rels`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/templates/default-docx-template/word/document.xml` & `python_docx-1.1.1/src/docx/templates/default-docx-template/word/document.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/templates/default-docx-template/word/fontTable.xml` & `python_docx-1.1.1/src/docx/templates/default-docx-template/word/fontTable.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/templates/default-docx-template/word/numbering.xml` & `python_docx-1.1.1/src/docx/templates/default-docx-template/word/numbering.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/templates/default-docx-template/word/settings.xml` & `python_docx-1.1.1/src/docx/templates/default-docx-template/word/settings.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/templates/default-docx-template/word/styles.xml` & `python_docx-1.1.1/src/docx/templates/default-docx-template/word/styles.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/templates/default-docx-template/word/stylesWithEffects.xml` & `python_docx-1.1.1/src/docx/templates/default-docx-template/word/stylesWithEffects.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/templates/default-docx-template/word/theme/theme1.xml` & `python_docx-1.1.1/src/docx/templates/default-docx-template/word/theme/theme1.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/templates/default-footer.xml` & `python_docx-1.1.1/src/docx/templates/default-footer.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/templates/default-header.xml` & `python_docx-1.1.1/src/docx/templates/default-header.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/templates/default-settings.xml` & `python_docx-1.1.1/src/docx/templates/default-settings.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/templates/default-styles.xml` & `python_docx-1.1.1/src/docx/templates/default-styles.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/templates/default.docx` & `python_docx-1.1.1/src/docx/templates/default.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/text/font.py` & `python_docx-1.1.1/src/docx/text/font.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/text/hyperlink.py` & `python_docx-1.1.1/src/docx/text/hyperlink.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 A hyperlink occurs in a paragraph, at the same level as a Run, and a hyperlink itself
 contains runs, which is where the visible text of the hyperlink is stored. So it's kind
 of in-between, less than a paragraph and more than a run. So it gets its own module.
 """
 
 from __future__ import annotations
 
-from typing import List
+from typing import TYPE_CHECKING
 
-from docx import types as t
-from docx.oxml.text.hyperlink import CT_Hyperlink
 from docx.shared import Parented
 from docx.text.run import Run
 
+if TYPE_CHECKING:
+    import docx.types as t
+    from docx.oxml.text.hyperlink import CT_Hyperlink
+
 
 class Hyperlink(Parented):
     """Proxy object wrapping a `<w:hyperlink>` element.
 
     A hyperlink occurs as a child of a paragraph, at the same level as a Run. A
     hyperlink itself contains runs, which is where the visible text of the hyperlink is
     stored.
@@ -74,15 +76,15 @@
         Word sometimes stores a fragment in this property (an XML attribute) and
         sometimes with the address, depending on how the URL is inserted, so don't
         depend on this field being empty to indicate no fragment is present.
         """
         return self._hyperlink.anchor or ""
 
     @property
-    def runs(self) -> List[Run]:
+    def runs(self) -> list[Run]:
         """List of |Run| instances in this hyperlink.
 
         Together these define the visible text of the hyperlink. The text of a hyperlink
         is typically contained in a single run will be broken into multiple runs if for
         example part of the hyperlink is bold or the text was changed after the document
         was saved.
         """
```

### Comparing `python-docx-1.1.0/src/docx/text/pagebreak.py` & `python_docx-1.1.1/src/docx/text/pagebreak.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Proxy objects related to rendered page-breaks."""
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from docx import types as t
 from docx.oxml.text.pagebreak import CT_LastRenderedPageBreak
 from docx.shared import Parented
 
 if TYPE_CHECKING:
+    import docx.types as t
     from docx.text.paragraph import Paragraph
 
 
 class RenderedPageBreak(Parented):
     """A page-break inserted by Word during page-layout for print or display purposes.
 
     This usually does not correspond to a "hard" page-break inserted by the document
```

### Comparing `python-docx-1.1.0/src/docx/text/paragraph.py` & `python_docx-1.1.1/src/docx/text/paragraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 """Paragraph-related proxy types."""
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Iterator, List, cast
 
-from typing_extensions import Self
-
-from docx import types as t
 from docx.enum.style import WD_STYLE_TYPE
 from docx.oxml.text.run import CT_R
 from docx.shared import StoryChild
 from docx.styles.style import ParagraphStyle
 from docx.text.hyperlink import Hyperlink
 from docx.text.pagebreak import RenderedPageBreak
 from docx.text.parfmt import ParagraphFormat
 from docx.text.run import Run
 
 if TYPE_CHECKING:
+    import docx.types as t
     from docx.enum.text import WD_PARAGRAPH_ALIGNMENT
     from docx.oxml.text.paragraph import CT_P
     from docx.styles.style import CharacterStyle
 
 
 class Paragraph(StoryChild):
     """Proxy object wrapping a `<w:p>` element."""
 
     def __init__(self, p: CT_P, parent: t.ProvidesStoryPart):
         super(Paragraph, self).__init__(parent)
         self._p = self._element = p
 
-    def add_run(
-        self, text: str | None = None, style: str | CharacterStyle | None = None
-    ) -> Run:
+    def add_run(self, text: str | None = None, style: str | CharacterStyle | None = None) -> Run:
         """Append run containing `text` and having character-style `style`.
 
         `text` can contain tab (``\\t``) characters, which are converted to the
         appropriate XML form for a tab. `text` can also include newline (``\\n``) or
         carriage return (``\\r``) characters, each of which is converted to a line
         break. When `text` is `None`, the new run is empty.
         """
@@ -78,15 +74,15 @@
     @property
     def hyperlinks(self) -> List[Hyperlink]:
         """A |Hyperlink| instance for each hyperlink in this paragraph."""
         return [Hyperlink(hyperlink, self) for hyperlink in self._p.hyperlink_lst]
 
     def insert_paragraph_before(
         self, text: str | None = None, style: str | ParagraphStyle | None = None
-    ) -> Self:
+    ) -> Paragraph:
         """Return a newly created paragraph, inserted directly before this paragraph.
 
         If `text` is supplied, the new paragraph contains that text in a single run. If
         `style` is provided, that style is assigned to the new paragraph.
         """
         paragraph = self._insert_paragraph_before()
         if text:
@@ -119,17 +115,15 @@
     @property
     def rendered_page_breaks(self) -> List[RenderedPageBreak]:
         """All rendered page-breaks in this paragraph.
 
         Most often an empty list, sometimes contains one page-break, but can contain
         more than one is rare or contrived cases.
         """
-        return [
-            RenderedPageBreak(lrpb, self) for lrpb in self._p.lastRenderedPageBreaks
-        ]
+        return [RenderedPageBreak(lrpb, self) for lrpb in self._p.lastRenderedPageBreaks]
 
     @property
     def runs(self) -> List[Run]:
         """Sequence of |Run| instances corresponding to the <w:r> elements in this
         paragraph."""
         return [Run(r, self) for r in self._p.r_lst]
```

### Comparing `python-docx-1.1.0/src/docx/text/parfmt.py` & `python_docx-1.1.1/src/docx/text/parfmt.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/text/run.py` & `python_docx-1.1.1/src/docx/text/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Run-related proxy objects for python-docx, Run in particular."""
 
 from __future__ import annotations
 
 from typing import IO, TYPE_CHECKING, Iterator, cast
 
-from docx import types as t
 from docx.drawing import Drawing
 from docx.enum.style import WD_STYLE_TYPE
 from docx.enum.text import WD_BREAK
 from docx.oxml.drawing import CT_Drawing
 from docx.oxml.text.pagebreak import CT_LastRenderedPageBreak
 from docx.shape import InlineShape
 from docx.shared import StoryChild
 from docx.styles.style import CharacterStyle
 from docx.text.font import Font
 from docx.text.pagebreak import RenderedPageBreak
 
 if TYPE_CHECKING:
+    import docx.types as t
     from docx.enum.text import WD_UNDERLINE
     from docx.oxml.text.run import CT_R, CT_Text
     from docx.shared import Length
 
 
 class Run(StoryChild):
     """Proxy object wrapping `<w:r>` element.
@@ -166,32 +166,28 @@
         other elements are ignored.
         """
         for item in self._r.inner_content_items:
             if isinstance(item, str):
                 yield item
             elif isinstance(item, CT_LastRenderedPageBreak):
                 yield RenderedPageBreak(item, self)
-            elif isinstance(  # pyright: ignore[reportUnnecessaryIsInstance]
-                item, CT_Drawing
-            ):
+            elif isinstance(item, CT_Drawing):  # pyright: ignore[reportUnnecessaryIsInstance]
                 yield Drawing(item, self)
 
     @property
     def style(self) -> CharacterStyle:
         """Read/write.
 
         A |CharacterStyle| object representing the character style applied to this run.
         The default character style for the document (often `Default Character Font`) is
         returned if the run has no directly-applied character style. Setting this
         property to |None| removes any directly-applied character style.
         """
         style_id = self._r.style
-        return cast(
-            CharacterStyle, self.part.get_style(style_id, WD_STYLE_TYPE.CHARACTER)
-        )
+        return cast(CharacterStyle, self.part.get_style(style_id, WD_STYLE_TYPE.CHARACTER))
 
     @style.setter
     def style(self, style_or_name: str | CharacterStyle | None):
         style_id = self.part.get_style_id(style_or_name, WD_STYLE_TYPE.CHARACTER)
         self._r.style = style_id
 
     @property
```

### Comparing `python-docx-1.1.0/src/docx/text/tabstops.py` & `python_docx-1.1.1/src/docx/text/tabstops.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/docx/types.py` & `python_docx-1.1.1/src/docx/types.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/src/python_docx.egg-info/PKG-INFO` & `python_docx-1.1.1/src/python_docx.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-docx
-Version: 1.1.0
+Version: 1.1.1
 Summary: Create, read, and update Microsoft Word .docx files.
 Author-email: Steve Canny <stcanny@gmail.com>
 License: MIT
 Project-URL: Changelog, https://github.com/python-openxml/python-docx/blob/master/HISTORY.rst
 Project-URL: Documentation, https://python-docx.readthedocs.org/en/latest/
 Project-URL: Homepage, https://github.com/python-openxml/python-docx
 Project-URL: Repository, https://github.com/python-openxml/python-docx
@@ -22,16 +22,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business :: Office Suites
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lxml>=3.1.0
-Requires-Dist: typing_extensions
+Requires-Dist: lxml<=4.9.2,>=3.1.0
+Requires-Dist: typing_extensions>=4.9.0
 
 # python-docx
 
 *python-docx* is a Python library for reading, creating, and updating Microsoft Word 2007+ (.docx) files.
 
 ## Installation
```

### Comparing `python-docx-1.1.0/src/python_docx.egg-info/SOURCES.txt` & `python_docx-1.1.1/src/python_docx.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -88,21 +88,20 @@
 docs/user/hdrftr.rst
 docs/user/install.rst
 docs/user/quickstart.rst
 docs/user/sections.rst
 docs/user/shapes.rst
 docs/user/styles-understanding.rst
 docs/user/styles-using.rst
+docs/user/tables.rst
 docs/user/text.rst
 features/api-open-document.feature
 features/blk-add-paragraph.feature
 features/blk-add-table.feature
 features/blk-iter-inner-content.feature
-features/cel-add-table.feature
-features/cel-text.feature
 features/doc-access-collections.feature
 features/doc-access-sections.feature
 features/doc-add-heading.feature
 features/doc-add-page-break.feature
 features/doc-add-paragraph.feature
 features/doc-add-picture.feature
 features/doc-add-section.feature
@@ -142,15 +141,17 @@
 features/sty-latent-add-del.feature
 features/sty-latent-props.feature
 features/sty-style-props.feature
 features/tab-access-tabs.feature
 features/tab-tabstop-props.feature
 features/tbl-add-row-or-col.feature
 features/tbl-cell-access.feature
+features/tbl-cell-add-table.feature
 features/tbl-cell-props.feature
+features/tbl-cell-text.feature
 features/tbl-col-props.feature
 features/tbl-item-access.feature
 features/tbl-merge-cells.feature
 features/tbl-props.feature
 features/tbl-row-props.feature
 features/tbl-style.feature
 features/txt-add-break.feature
@@ -173,15 +174,14 @@
 features/_scratch/test_out/word/styles.xml
 features/_scratch/test_out/word/stylesWithEffects.xml
 features/_scratch/test_out/word/webSettings.xml
 features/_scratch/test_out/word/_rels/document.xml.rels
 features/_scratch/test_out/word/theme/theme1.xml
 features/steps/api.py
 features/steps/block.py
-features/steps/cell.py
 features/steps/coreprops.py
 features/steps/document.py
 features/steps/font.py
 features/steps/hdrftr.py
 features/steps/helpers.py
 features/steps/hyperlink.py
 features/steps/image.py
@@ -236,28 +236,30 @@
 features/steps/test_files/sty-behav-props.docx
 features/steps/test_files/sty-having-no-styles-part.docx
 features/steps/test_files/sty-having-styles-part.docx
 features/steps/test_files/sty-known-styles.docx
 features/steps/test_files/tab-stops.docx
 features/steps/test_files/tbl-2x2-table.docx
 features/steps/test_files/tbl-cell-access.docx
+features/steps/test_files/tbl-cell-props.docx
 features/steps/test_files/tbl-col-props.docx
 features/steps/test_files/tbl-having-applied-style.docx
 features/steps/test_files/tbl-having-tables.docx
 features/steps/test_files/tbl-on-off-props.docx
 features/steps/test_files/tbl-props.docx
 features/steps/test_files/test.png
 features/steps/test_files/txt-font-highlight-color.docx
 features/steps/test_files/txt-font-props.docx
 src/docx/__init__.py
 src/docx/api.py
 src/docx/blkcntnr.py
 src/docx/document.py
 src/docx/exceptions.py
 src/docx/package.py
+src/docx/py.typed
 src/docx/section.py
 src/docx/settings.py
 src/docx/shape.py
 src/docx/shared.py
 src/docx/table.py
 src/docx/types.py
 src/docx/dml/__init__.py
@@ -422,15 +424,14 @@
 tests/oxml/text/test_run.py
 tests/oxml/unitdata/__init__.py
 tests/oxml/unitdata/dml.py
 tests/oxml/unitdata/numbering.py
 tests/oxml/unitdata/section.py
 tests/oxml/unitdata/shared.py
 tests/oxml/unitdata/styles.py
-tests/oxml/unitdata/table.py
 tests/oxml/unitdata/text.py
 tests/parts/__init__.py
 tests/parts/test_document.py
 tests/parts/test_hdrftr.py
 tests/parts/test_image.py
 tests/parts/test_numbering.py
 tests/parts/test_settings.py
```

### Comparing `python-docx-1.1.0/tests/dml/test_color.py` & `python_docx-1.1.1/tests/dml/test_color.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/image/test_bmp.py` & `python_docx-1.1.1/tests/image/test_bmp.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/image/test_gif.py` & `python_docx-1.1.1/tests/image/test_gif.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/image/test_helpers.py` & `python_docx-1.1.1/tests/image/test_helpers.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/image/test_image.py` & `python_docx-1.1.1/tests/image/test_image.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/image/test_jpeg.py` & `python_docx-1.1.1/tests/image/test_jpeg.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/image/test_png.py` & `python_docx-1.1.1/tests/image/test_png.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/image/test_tiff.py` & `python_docx-1.1.1/tests/image/test_tiff.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/opc/parts/test_coreprops.py` & `python_docx-1.1.1/tests/opc/parts/test_coreprops.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/opc/test_coreprops.py` & `python_docx-1.1.1/tests/opc/test_coreprops.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/opc/test_oxml.py` & `python_docx-1.1.1/tests/opc/test_oxml.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/opc/test_package.py` & `python_docx-1.1.1/tests/opc/test_package.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,40 @@
+# pyright: reportPrivateUsage=false
+
 """Unit test suite for docx.opc.package module"""
 
+from __future__ import annotations
+
 import pytest
 
 from docx.opc.constants import RELATIONSHIP_TYPE as RT
 from docx.opc.coreprops import CoreProperties
 from docx.opc.package import OpcPackage, Unmarshaller
 from docx.opc.packuri import PACKAGE_URI, PackURI
 from docx.opc.part import Part
 from docx.opc.parts.coreprops import CorePropertiesPart
 from docx.opc.pkgreader import PackageReader
 from docx.opc.rel import Relationships, _Relationship
 
 from ..unitutil.mock import (
+    FixtureRequest,
     Mock,
-    PropertyMock,
     call,
     class_mock,
     instance_mock,
     loose_mock,
     method_mock,
     patch,
     property_mock,
 )
 
 
 class DescribeOpcPackage:
+    """Unit-test suite for `docx.opc.package.OpcPackage` objects."""
+
     def it_can_open_a_pkg_file(self, PackageReader_, PartFactory_, Unmarshaller_):
         # mockery ----------------------
         pkg_file = Mock(name="pkg_file")
         pkg_reader = PackageReader_.from_file.return_value
         # exercise ---------------------
         pkg = OpcPackage.open(pkg_file)
         # verify -----------------------
@@ -38,50 +44,57 @@
 
     def it_initializes_its_rels_collection_on_first_reference(self, Relationships_):
         pkg = OpcPackage()
         rels = pkg.rels
         Relationships_.assert_called_once_with(PACKAGE_URI.baseURI)
         assert rels == Relationships_.return_value
 
-    def it_can_add_a_relationship_to_a_part(self, pkg_with_rels_, rel_attrs_):
-        reltype, target, rId = rel_attrs_
-        pkg = pkg_with_rels_
-        # exercise ---------------------
-        pkg.load_rel(reltype, target, rId)
-        # verify -----------------------
-        pkg._rels.add_relationship.assert_called_once_with(reltype, target, rId, False)
+    def it_can_add_a_relationship_to_a_part(self, rels_prop_: Mock, rels_: Mock, part_: Mock):
+        rels_prop_.return_value = rels_
+        pkg = OpcPackage()
+
+        pkg.load_rel("http://rel/type", part_, "rId99")
 
-    def it_can_establish_a_relationship_to_another_part(self, relate_to_part_fixture_):
-        pkg, part_, reltype, rId = relate_to_part_fixture_
-        _rId = pkg.relate_to(part_, reltype)
-        pkg.rels.get_or_add.assert_called_once_with(reltype, part_)
-        assert _rId == rId
+        rels_.add_relationship.assert_called_once_with("http://rel/type", part_, "rId99", False)
+
+    def it_can_establish_a_relationship_to_another_part(
+        self, rels_prop_: Mock, rels_: Mock, rel_: Mock, part_: Mock
+    ):
+        rel_.rId = "rId99"
+        rels_.get_or_add.return_value = rel_
+        rels_prop_.return_value = rels_
+        pkg = OpcPackage()
+
+        rId = pkg.relate_to(part_, "http://rel/type")
+
+        rels_.get_or_add.assert_called_once_with("http://rel/type", part_)
+        assert rId == "rId99"
 
     def it_can_provide_a_list_of_the_parts_it_contains(self):
         # mockery ----------------------
         parts = [Mock(name="part1"), Mock(name="part2")]
         pkg = OpcPackage()
         # verify -----------------------
         with patch.object(OpcPackage, "iter_parts", return_value=parts):
             assert pkg.parts == [parts[0], parts[1]]
 
-    def it_can_iterate_over_parts_by_walking_rels_graph(self):
+    def it_can_iterate_over_parts_by_walking_rels_graph(self, rels_prop_: Mock):
         # +----------+       +--------+
         # | pkg_rels |-----> | part_1 |
         # +----------+       +--------+
         #      |               |    ^
         #      v               v    |
         #   external         +--------+
         #                    | part_2 |
         #                    +--------+
         part1, part2 = (Mock(name="part1"), Mock(name="part2"))
         part1.rels = {1: Mock(name="rel1", is_external=False, target_part=part2)}
         part2.rels = {1: Mock(name="rel2", is_external=False, target_part=part1)}
         pkg = OpcPackage()
-        pkg._rels = {
+        rels_prop_.return_value = {
             1: Mock(name="rel3", is_external=False, target_part=part1),
             2: Mock(name="rel4", is_external=True),
         }
         # verify -----------------------
         assert part1 in pkg.iter_parts()
         assert part2 in pkg.iter_parts()
         assert len(list(pkg.iter_parts())) == 2
@@ -102,46 +115,45 @@
 
     def it_can_find_a_part_related_by_reltype(self, related_part_fixture_):
         pkg, reltype, related_part_ = related_part_fixture_
         related_part = pkg.part_related_by(reltype)
         pkg.rels.part_with_reltype.assert_called_once_with(reltype)
         assert related_part is related_part_
 
-    def it_can_save_to_a_pkg_file(self, pkg_file_, PackageWriter_, parts, parts_):
+    def it_can_save_to_a_pkg_file(
+        self, pkg_file_: Mock, PackageWriter_: Mock, parts_prop_: Mock, parts_: list[Mock]
+    ):
+        parts_prop_.return_value = parts_
         pkg = OpcPackage()
         pkg.save(pkg_file_)
         for part in parts_:
             part.before_marshal.assert_called_once_with()
-        PackageWriter_.write.assert_called_once_with(pkg_file_, pkg._rels, parts_)
+        PackageWriter_.write.assert_called_once_with(pkg_file_, pkg.rels, parts_)
 
     def it_provides_access_to_the_core_properties(self, core_props_fixture):
         opc_package, core_properties_ = core_props_fixture
         core_properties = opc_package.core_properties
         assert core_properties is core_properties_
 
-    def it_provides_access_to_the_core_properties_part_to_help(
-        self, core_props_part_fixture
-    ):
+    def it_provides_access_to_the_core_properties_part_to_help(self, core_props_part_fixture):
         opc_package, core_properties_part_ = core_props_part_fixture
         core_properties_part = opc_package._core_properties_part
         assert core_properties_part is core_properties_part_
 
     def it_creates_a_default_core_props_part_if_none_present(
         self, part_related_by_, CorePropertiesPart_, relate_to_, core_properties_part_
     ):
         part_related_by_.side_effect = KeyError
         CorePropertiesPart_.default.return_value = core_properties_part_
         opc_package = OpcPackage()
 
         core_properties_part = opc_package._core_properties_part
 
         CorePropertiesPart_.default.assert_called_once_with(opc_package)
-        relate_to_.assert_called_once_with(
-            opc_package, core_properties_part_, RT.CORE_PROPERTIES
-        )
+        relate_to_.assert_called_once_with(opc_package, core_properties_part_, RT.CORE_PROPERTIES)
         assert core_properties_part is core_properties_part_
 
     # fixtures ---------------------------------------------
 
     @pytest.fixture
     def core_props_fixture(
         self, _core_properties_part_prop_, core_properties_part_, core_properties_
@@ -157,142 +169,114 @@
         part_related_by_.return_value = core_properties_part_
         return opc_package, core_properties_part_
 
     @pytest.fixture(params=[((), 1), ((1,), 2), ((1, 2), 3), ((2, 3), 1), ((1, 3), 2)])
     def next_partname_fixture(self, request, iter_parts_):
         existing_partname_ns, next_partname_n = request.param
         parts_ = [
-            instance_mock(
-                request, Part, name="part[%d]" % idx, partname="/foo/bar/baz%d.xml" % n
-            )
+            instance_mock(request, Part, name="part[%d]" % idx, partname="/foo/bar/baz%d.xml" % n)
             for idx, n in enumerate(existing_partname_ns)
         ]
         expected_value = "/foo/bar/baz%d.xml" % next_partname_n
         return parts_, expected_value
 
     @pytest.fixture
-    def relate_to_part_fixture_(self, request, pkg, rels_, reltype):
-        rId = "rId99"
-        rel_ = instance_mock(request, _Relationship, name="rel_", rId=rId)
-        rels_.get_or_add.return_value = rel_
-        pkg._rels = rels_
-        part_ = instance_mock(request, Part, name="part_")
-        return pkg, part_, reltype, rId
-
-    @pytest.fixture
-    def related_part_fixture_(self, request, rels_, reltype):
+    def related_part_fixture_(self, request: FixtureRequest, rels_prop_: Mock, rels_: Mock):
         related_part_ = instance_mock(request, Part, name="related_part_")
         rels_.part_with_reltype.return_value = related_part_
         pkg = OpcPackage()
-        pkg._rels = rels_
-        return pkg, reltype, related_part_
+        rels_prop_.return_value = rels_
+        return pkg, "http://rel/type", related_part_
 
     # fixture components -----------------------------------
 
     @pytest.fixture
-    def CorePropertiesPart_(self, request):
+    def CorePropertiesPart_(self, request: FixtureRequest):
         return class_mock(request, "docx.opc.package.CorePropertiesPart")
 
     @pytest.fixture
-    def core_properties_(self, request):
+    def core_properties_(self, request: FixtureRequest):
         return instance_mock(request, CoreProperties)
 
     @pytest.fixture
-    def core_properties_part_(self, request):
+    def core_properties_part_(self, request: FixtureRequest):
         return instance_mock(request, CorePropertiesPart)
 
     @pytest.fixture
-    def _core_properties_part_prop_(self, request):
+    def _core_properties_part_prop_(self, request: FixtureRequest):
         return property_mock(request, OpcPackage, "_core_properties_part")
 
     @pytest.fixture
-    def iter_parts_(self, request):
+    def iter_parts_(self, request: FixtureRequest):
         return method_mock(request, OpcPackage, "iter_parts")
 
     @pytest.fixture
-    def PackageReader_(self, request):
+    def PackageReader_(self, request: FixtureRequest):
         return class_mock(request, "docx.opc.package.PackageReader")
 
     @pytest.fixture
-    def PackURI_(self, request):
+    def PackURI_(self, request: FixtureRequest):
         return class_mock(request, "docx.opc.package.PackURI")
 
     @pytest.fixture
-    def packuri_(self, request):
+    def packuri_(self, request: FixtureRequest):
         return instance_mock(request, PackURI)
 
     @pytest.fixture
-    def PackageWriter_(self, request):
+    def PackageWriter_(self, request: FixtureRequest):
         return class_mock(request, "docx.opc.package.PackageWriter")
 
     @pytest.fixture
-    def PartFactory_(self, request):
+    def PartFactory_(self, request: FixtureRequest):
         return class_mock(request, "docx.opc.package.PartFactory")
 
     @pytest.fixture
-    def part_related_by_(self, request):
-        return method_mock(request, OpcPackage, "part_related_by")
+    def part_(self, request: FixtureRequest):
+        return instance_mock(request, Part)
 
     @pytest.fixture
-    def parts(self, parts_):
-        """
-        Return a mock patching property OpcPackage.parts, reversing the
-        patch after each use.
-        """
-        p = patch.object(
-            OpcPackage, "parts", new_callable=PropertyMock, return_value=parts_
-        )
-        yield p.start()
-        p.stop()
+    def part_related_by_(self, request: FixtureRequest):
+        return method_mock(request, OpcPackage, "part_related_by")
 
     @pytest.fixture
-    def parts_(self, request):
+    def parts_(self, request: FixtureRequest):
         part_ = instance_mock(request, Part, name="part_")
         part_2_ = instance_mock(request, Part, name="part_2_")
         return [part_, part_2_]
 
     @pytest.fixture
-    def pkg(self, request):
-        return OpcPackage()
+    def parts_prop_(self, request: FixtureRequest):
+        return property_mock(request, OpcPackage, "parts")
 
     @pytest.fixture
-    def pkg_file_(self, request):
+    def pkg_file_(self, request: FixtureRequest):
         return loose_mock(request)
 
     @pytest.fixture
-    def pkg_with_rels_(self, request, rels_):
-        pkg = OpcPackage()
-        pkg._rels = rels_
-        return pkg
-
-    @pytest.fixture
-    def Relationships_(self, request):
+    def Relationships_(self, request: FixtureRequest):
         return class_mock(request, "docx.opc.package.Relationships")
 
     @pytest.fixture
-    def rel_attrs_(self, request):
-        reltype = "http://rel/type"
-        target_ = instance_mock(request, Part, name="target_")
-        rId = "rId99"
-        return reltype, target_, rId
+    def rel_(self, request: FixtureRequest):
+        return instance_mock(request, _Relationship)
 
     @pytest.fixture
-    def relate_to_(self, request):
+    def relate_to_(self, request: FixtureRequest):
         return method_mock(request, OpcPackage, "relate_to")
 
     @pytest.fixture
-    def rels_(self, request):
+    def rels_(self, request: FixtureRequest):
         return instance_mock(request, Relationships)
 
     @pytest.fixture
-    def reltype(self, request):
-        return "http://rel/type"
+    def rels_prop_(self, request: FixtureRequest):
+        return property_mock(request, OpcPackage, "rels")
 
     @pytest.fixture
-    def Unmarshaller_(self, request):
+    def Unmarshaller_(self, request: FixtureRequest):
         return class_mock(request, "docx.opc.package.Unmarshaller")
 
 
 class DescribeUnmarshaller:
     def it_can_unmarshal_from_a_pkg_reader(
         self,
         pkg_reader_,
@@ -302,17 +286,15 @@
         _unmarshal_relationships_,
         parts_dict_,
     ):
         _unmarshal_parts_.return_value = parts_dict_
         Unmarshaller.unmarshal(pkg_reader_, pkg_, part_factory_)
 
         _unmarshal_parts_.assert_called_once_with(pkg_reader_, pkg_, part_factory_)
-        _unmarshal_relationships_.assert_called_once_with(
-            pkg_reader_, pkg_, parts_dict_
-        )
+        _unmarshal_relationships_.assert_called_once_with(pkg_reader_, pkg_, parts_dict_)
         for part in parts_dict_.values():
             part.after_unmarshal.assert_called_once_with()
         pkg_.after_unmarshal.assert_called_once_with()
 
     def it_can_unmarshal_parts(
         self,
         pkg_reader_,
@@ -402,51 +384,51 @@
             call.part2.load_rel(reltype, "target_ref_2", "rId4", True),
         ]
         assert pkg.mock_calls == expected_pkg_calls
 
     # fixtures ---------------------------------------------
 
     @pytest.fixture
-    def blobs_(self, request):
+    def blobs_(self, request: FixtureRequest):
         blob_ = loose_mock(request, spec=str, name="blob_")
         blob_2_ = loose_mock(request, spec=str, name="blob_2_")
         return blob_, blob_2_
 
     @pytest.fixture
-    def content_types_(self, request):
+    def content_types_(self, request: FixtureRequest):
         content_type_ = loose_mock(request, spec=str, name="content_type_")
         content_type_2_ = loose_mock(request, spec=str, name="content_type_2_")
         return content_type_, content_type_2_
 
     @pytest.fixture
     def part_factory_(self, request, parts_):
         part_factory_ = loose_mock(request, spec=Part)
         part_factory_.side_effect = parts_
         return part_factory_
 
     @pytest.fixture
-    def partnames_(self, request):
+    def partnames_(self, request: FixtureRequest):
         partname_ = loose_mock(request, spec=str, name="partname_")
         partname_2_ = loose_mock(request, spec=str, name="partname_2_")
         return partname_, partname_2_
 
     @pytest.fixture
-    def parts_(self, request):
+    def parts_(self, request: FixtureRequest):
         part_ = instance_mock(request, Part, name="part_")
         part_2_ = instance_mock(request, Part, name="part_2")
         return part_, part_2_
 
     @pytest.fixture
     def parts_dict_(self, request, partnames_, parts_):
         partname_, partname_2_ = partnames_
         part_, part_2_ = parts_
         return {partname_: part_, partname_2_: part_2_}
 
     @pytest.fixture
-    def pkg_(self, request):
+    def pkg_(self, request: FixtureRequest):
         return instance_mock(request, OpcPackage)
 
     @pytest.fixture
     def pkg_reader_(self, request, partnames_, content_types_, reltypes_, blobs_):
         partname_, partname_2_ = partnames_
         content_type_, content_type_2_ = content_types_
         reltype_, reltype_2_ = reltypes_
@@ -456,21 +438,19 @@
             (partname_2_, content_type_2_, reltype_2_, blob_2_),
         )
         pkg_reader_ = instance_mock(request, PackageReader)
         pkg_reader_.iter_sparts.return_value = iter_spart_items
         return pkg_reader_
 
     @pytest.fixture
-    def reltypes_(self, request):
+    def reltypes_(self, request: FixtureRequest):
         reltype_ = instance_mock(request, str, name="reltype_")
         reltype_2_ = instance_mock(request, str, name="reltype_2")
         return reltype_, reltype_2_
 
     @pytest.fixture
-    def _unmarshal_parts_(self, request):
+    def _unmarshal_parts_(self, request: FixtureRequest):
         return method_mock(request, Unmarshaller, "_unmarshal_parts", autospec=False)
 
     @pytest.fixture
-    def _unmarshal_relationships_(self, request):
-        return method_mock(
-            request, Unmarshaller, "_unmarshal_relationships", autospec=False
-        )
+    def _unmarshal_relationships_(self, request: FixtureRequest):
+        return method_mock(request, Unmarshaller, "_unmarshal_relationships", autospec=False)
```

### Comparing `python-docx-1.1.0/tests/opc/test_packuri.py` & `python_docx-1.1.1/tests/opc/test_packuri.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/opc/test_part.py` & `python_docx-1.1.1/tests/opc/test_part.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,33 @@
+# pyright: reportPrivateUsage=false
+
 """Unit test suite for docx.opc.part module"""
 
+from __future__ import annotations
+
 import pytest
 
 from docx.opc.package import OpcPackage
 from docx.opc.packuri import PackURI
 from docx.opc.part import Part, PartFactory, XmlPart
 from docx.opc.rel import Relationships, _Relationship
 from docx.oxml.xmlchemy import BaseOxmlElement
 
 from ..unitutil.cxml import element
 from ..unitutil.mock import (
     ANY,
+    FixtureRequest,
     Mock,
     class_mock,
     cls_attr_mock,
     function_mock,
     initializer_mock,
     instance_mock,
     loose_mock,
+    property_mock,
 )
 
 
 class DescribePart:
     def it_can_be_constructed_by_PartFactory(
         self, partname_, content_type_, blob_, package_, __init_
     ):
@@ -113,158 +119,134 @@
 
     @pytest.fixture
     def partname_(self, request):
         return instance_mock(request, PackURI)
 
 
 class DescribePartRelationshipManagementInterface:
-    def it_provides_access_to_its_relationships(self, rels_fixture):
-        part, Relationships_, partname_, rels_ = rels_fixture
+    """Unit-test suite for `docx.opc.package.Part` relationship behaviors."""
+
+    def it_provides_access_to_its_relationships(
+        self, Relationships_: Mock, partname_: Mock, rels_: Mock
+    ):
+        Relationships_.return_value = rels_
+        part = Part(partname_, "content_type")
+
         rels = part.rels
+
         Relationships_.assert_called_once_with(partname_.baseURI)
         assert rels is rels_
 
-    def it_can_load_a_relationship(self, load_rel_fixture):
-        part, rels_, reltype_, target_, rId_ = load_rel_fixture
-        part.load_rel(reltype_, target_, rId_)
-        rels_.add_relationship.assert_called_once_with(reltype_, target_, rId_, False)
-
-    def it_can_establish_a_relationship_to_another_part(self, relate_to_part_fixture):
-        part, target_, reltype_, rId_ = relate_to_part_fixture
-        rId = part.relate_to(target_, reltype_)
-        part.rels.get_or_add.assert_called_once_with(reltype_, target_)
-        assert rId is rId_
-
-    def it_can_establish_an_external_relationship(self, relate_to_url_fixture):
-        part, url_, reltype_, rId_ = relate_to_url_fixture
-        rId = part.relate_to(url_, reltype_, is_external=True)
-        part.rels.get_or_add_ext_rel.assert_called_once_with(reltype_, url_)
-        assert rId is rId_
-
-    def it_can_drop_a_relationship(self, drop_rel_fixture):
-        part, rId, rel_should_be_gone = drop_rel_fixture
-        part.drop_rel(rId)
-        if rel_should_be_gone:
-            assert rId not in part.rels
-        else:
-            assert rId in part.rels
-
-    def it_can_find_a_related_part_by_reltype(self, related_part_fixture):
-        part, reltype_, related_part_ = related_part_fixture
-        related_part = part.part_related_by(reltype_)
-        part.rels.part_with_reltype.assert_called_once_with(reltype_)
-        assert related_part is related_part_
-
-    def it_can_find_a_related_part_by_rId(self, related_parts_fixture):
-        part, related_parts_ = related_parts_fixture
-        assert part.related_parts is related_parts_
-
-    def it_can_find_the_uri_of_an_external_relationship(self, target_ref_fixture):
-        part, rId_, url_ = target_ref_fixture
-        url = part.target_ref(rId_)
-        assert url == url_
+    def it_can_load_a_relationship(self, rels_prop_: Mock, rels_: Mock, other_part_: Mock):
+        rels_prop_.return_value = rels_
+        part = Part("partname", "content_type")
 
-    # fixtures ---------------------------------------------
+        part.load_rel("http://rel/type", other_part_, "rId42")
+
+        rels_.add_relationship.assert_called_once_with(
+            "http://rel/type", other_part_, "rId42", False
+        )
+
+    def it_can_establish_a_relationship_to_another_part(
+        self, rels_prop_: Mock, rels_: Mock, rel_: Mock, other_part_: Mock
+    ):
+        rels_prop_.return_value = rels_
+        rels_.get_or_add.return_value = rel_
+        rel_.rId = "rId18"
+        part = Part("partname", "content_type")
+
+        rId = part.relate_to(other_part_, "http://rel/type")
 
-    @pytest.fixture(
-        params=[
+        rels_.get_or_add.assert_called_once_with("http://rel/type", other_part_)
+        assert rId == "rId18"
+
+    def it_can_establish_an_external_relationship(self, rels_prop_: Mock, rels_: Mock):
+        rels_prop_.return_value = rels_
+        rels_.get_or_add_ext_rel.return_value = "rId27"
+        part = Part("partname", "content_type")
+
+        rId = part.relate_to("https://hyper/link", "http://rel/type", is_external=True)
+
+        rels_.get_or_add_ext_rel.assert_called_once_with("http://rel/type", "https://hyper/link")
+        assert rId == "rId27"
+
+    @pytest.mark.parametrize(
+        ("part_cxml", "rel_should_be_dropped"),
+        [
             ("w:p", True),
             ("w:p/r:a{r:id=rId42}", True),
             ("w:p/r:a{r:id=rId42}/r:b{r:id=rId42}", False),
-        ]
+        ],
     )
-    def drop_rel_fixture(self, request, part):
-        part_cxml, rel_should_be_dropped = request.param
-        rId = "rId42"
-        part._element = element(part_cxml)
-        part._rels = {rId: None}
-        return part, rId, rel_should_be_dropped
+    def it_can_drop_a_relationship(
+        self, part_cxml: str, rel_should_be_dropped: bool, rels_prop_: Mock
+    ):
+        rels_prop_.return_value = {"rId42": None}
+        part = Part("partname", "content_type")
+        part._element = element(part_cxml)  # pyright: ignore[reportAttributeAccessIssue]
 
-    @pytest.fixture
-    def load_rel_fixture(self, part, rels_, reltype_, part_, rId_):
-        part._rels = rels_
-        return part, rels_, reltype_, part_, rId_
+        part.drop_rel("rId42")
 
-    @pytest.fixture
-    def relate_to_part_fixture(self, request, part, reltype_, part_, rels_, rId_):
-        part._rels = rels_
-        target_ = part_
-        return part, target_, reltype_, rId_
+        assert ("rId42" not in part.rels) is rel_should_be_dropped
 
-    @pytest.fixture
-    def relate_to_url_fixture(self, request, part, rels_, url_, reltype_, rId_):
-        part._rels = rels_
-        return part, url_, reltype_, rId_
+    def it_can_find_a_related_part_by_reltype(
+        self, rels_prop_: Mock, rels_: Mock, other_part_: Mock
+    ):
+        rels_prop_.return_value = rels_
+        rels_.part_with_reltype.return_value = other_part_
+        part = Part("partname", "content_type")
 
-    @pytest.fixture
-    def related_part_fixture(self, request, part, rels_, reltype_, part_):
-        part._rels = rels_
-        return part, reltype_, part_
+        related_part = part.part_related_by("http://rel/type")
 
-    @pytest.fixture
-    def related_parts_fixture(self, request, part, rels_, related_parts_):
-        part._rels = rels_
-        return part, related_parts_
+        rels_.part_with_reltype.assert_called_once_with("http://rel/type")
+        assert related_part is other_part_
 
-    @pytest.fixture
-    def rels_fixture(self, Relationships_, partname_, rels_):
-        part = Part(partname_, None)
-        return part, Relationships_, partname_, rels_
+    def it_can_find_a_related_part_by_rId(self, rels_prop_: Mock, rels_: Mock, other_part_: Mock):
+        rels_prop_.return_value = rels_
+        rels_.related_parts = {"rId24": other_part_}
+        part = Part("partname", "content_type")
 
-    @pytest.fixture
-    def target_ref_fixture(self, request, part, rId_, rel_, url_):
-        part._rels = {rId_: rel_}
-        return part, rId_, url_
+        assert part.related_parts["rId24"] is other_part_
 
-    # fixture components ---------------------------------------------
+    def it_can_find_the_uri_of_an_external_relationship(
+        self, rels_prop_: Mock, rel_: Mock, other_part_: Mock
+    ):
+        rels_prop_.return_value = {"rId7": rel_}
+        rel_.target_ref = "https://hyper/link"
+        part = Part("partname", "content_type")
 
-    @pytest.fixture
-    def part(self):
-        return Part(None, None)
+        url = part.target_ref("rId7")
 
-    @pytest.fixture
-    def part_(self, request):
-        return instance_mock(request, Part)
+        assert url == "https://hyper/link"
 
-    @pytest.fixture
-    def partname_(self, request):
-        return instance_mock(request, PackURI)
-
-    @pytest.fixture
-    def Relationships_(self, request, rels_):
-        return class_mock(request, "docx.opc.part.Relationships", return_value=rels_)
+    # fixtures ---------------------------------------------
 
     @pytest.fixture
-    def rel_(self, request, rId_, url_):
-        return instance_mock(request, _Relationship, rId=rId_, target_ref=url_)
+    def other_part_(self, request: FixtureRequest):
+        return instance_mock(request, Part)
 
     @pytest.fixture
-    def rels_(self, request, part_, rel_, rId_, related_parts_):
-        rels_ = instance_mock(request, Relationships)
-        rels_.part_with_reltype.return_value = part_
-        rels_.get_or_add.return_value = rel_
-        rels_.get_or_add_ext_rel.return_value = rId_
-        rels_.related_parts = related_parts_
-        return rels_
+    def partname_(self, request: FixtureRequest):
+        return instance_mock(request, PackURI)
 
     @pytest.fixture
-    def related_parts_(self, request):
-        return instance_mock(request, dict)
+    def Relationships_(self, request: FixtureRequest):
+        return class_mock(request, "docx.opc.part.Relationships")
 
     @pytest.fixture
-    def reltype_(self, request):
-        return instance_mock(request, str)
+    def rel_(self, request: FixtureRequest):
+        return instance_mock(request, _Relationship)
 
     @pytest.fixture
-    def rId_(self, request):
-        return instance_mock(request, str)
+    def rels_(self, request: FixtureRequest):
+        return instance_mock(request, Relationships)
 
     @pytest.fixture
-    def url_(self, request):
-        return instance_mock(request, str)
+    def rels_prop_(self, request: FixtureRequest):
+        return property_mock(request, Part, "rels")
 
 
 class DescribePartFactory:
     def it_constructs_part_from_selector_if_defined(self, cls_selector_fixture):
         # fixture ----------------------
         (
             cls_selector_fn_,
@@ -274,58 +256,50 @@
         ) = cls_selector_fixture
         partname, content_type, reltype, blob, package = part_load_params
         # exercise ---------------------
         PartFactory.part_class_selector = cls_selector_fn_
         part = PartFactory(partname, content_type, reltype, blob, package)
         # verify -----------------------
         cls_selector_fn_.assert_called_once_with(content_type, reltype)
-        CustomPartClass_.load.assert_called_once_with(
-            partname, content_type, blob, package
-        )
+        CustomPartClass_.load.assert_called_once_with(partname, content_type, blob, package)
         assert part is part_of_custom_type_
 
     def it_constructs_custom_part_type_for_registered_content_types(
         self, part_args_, CustomPartClass_, part_of_custom_type_
     ):
         # fixture ----------------------
         partname, content_type, reltype, package, blob = part_args_
         # exercise ---------------------
         PartFactory.part_type_for[content_type] = CustomPartClass_
         part = PartFactory(partname, content_type, reltype, blob, package)
         # verify -----------------------
-        CustomPartClass_.load.assert_called_once_with(
-            partname, content_type, blob, package
-        )
+        CustomPartClass_.load.assert_called_once_with(partname, content_type, blob, package)
         assert part is part_of_custom_type_
 
     def it_constructs_part_using_default_class_when_no_custom_registered(
         self, part_args_2_, DefaultPartClass_, part_of_default_type_
     ):
         partname, content_type, reltype, blob, package = part_args_2_
         part = PartFactory(partname, content_type, reltype, blob, package)
-        DefaultPartClass_.load.assert_called_once_with(
-            partname, content_type, blob, package
-        )
+        DefaultPartClass_.load.assert_called_once_with(partname, content_type, blob, package)
         assert part is part_of_default_type_
 
     # fixtures ---------------------------------------------
 
     @pytest.fixture
     def blob_(self, request):
         return instance_mock(request, str)
 
     @pytest.fixture
     def blob_2_(self, request):
         return instance_mock(request, str)
 
     @pytest.fixture
     def cls_method_fn_(self, request, cls_selector_fn_):
-        return function_mock(
-            request, "docx.opc.part.cls_method_fn", return_value=cls_selector_fn_
-        )
+        return function_mock(request, "docx.opc.part.cls_method_fn", return_value=cls_selector_fn_)
 
     @pytest.fixture
     def cls_selector_fixture(
         self,
         cls_selector_fn_,
         cls_method_fn_,
         part_load_params,
@@ -401,17 +375,15 @@
         return instance_mock(request, PackURI)
 
     @pytest.fixture
     def part_args_(self, request, partname_, content_type_, reltype_, package_, blob_):
         return partname_, content_type_, reltype_, blob_, package_
 
     @pytest.fixture
-    def part_args_2_(
-        self, request, partname_2_, content_type_2_, reltype_2_, package_2_, blob_2_
-    ):
+    def part_args_2_(self, request, partname_2_, content_type_2_, reltype_2_, package_2_, blob_2_):
         return partname_2_, content_type_2_, reltype_2_, blob_2_, package_2_
 
     @pytest.fixture
     def reltype_(self, request):
         return instance_mock(request, str)
 
     @pytest.fixture
@@ -422,17 +394,15 @@
 class DescribeXmlPart:
     def it_can_be_constructed_by_PartFactory(
         self, partname_, content_type_, blob_, package_, element_, parse_xml_, __init_
     ):
         part = XmlPart.load(partname_, content_type_, blob_, package_)
 
         parse_xml_.assert_called_once_with(blob_)
-        __init_.assert_called_once_with(
-            ANY, partname_, content_type_, element_, package_
-        )
+        __init_.assert_called_once_with(ANY, partname_, content_type_, element_, package_)
         assert isinstance(part, XmlPart)
 
     def it_can_serialize_to_xml(self, blob_fixture):
         xml_part, element_, serialize_part_xml_ = blob_fixture
         blob = xml_part.blob
         serialize_part_xml_.assert_called_once_with(element_)
         assert blob is serialize_part_xml_.return_value
```

### Comparing `python-docx-1.1.0/tests/opc/test_phys_pkg.py` & `python_docx-1.1.1/tests/opc/test_phys_pkg.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/opc/test_pkgreader.py` & `python_docx-1.1.1/tests/opc/test_pkgreader.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/opc/test_pkgwriter.py` & `python_docx-1.1.1/tests/opc/test_pkgwriter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+# pyright: reportPrivateUsage=false
+
 """Test suite for opc.pkgwriter module."""
 
+from __future__ import annotations
+
 import pytest
 
 from docx.opc.constants import CONTENT_TYPE as CT
 from docx.opc.packuri import PackURI
 from docx.opc.part import Part
 from docx.opc.phys_pkg import _ZipPkgWriter
 from docx.opc.pkgwriter import PackageWriter, _ContentTypesItem
+from docx.opc.rel import Relationships
 
 from ..unitutil.mock import (
-    MagicMock,
+    FixtureRequest,
     Mock,
     call,
     class_mock,
     instance_mock,
     method_mock,
     patch,
 )
@@ -50,62 +55,73 @@
         phys_writer = Mock(name="phys_writer")
         pkg_rels = Mock(name="pkg_rels")
         # exercise ---------------------
         PackageWriter._write_pkg_rels(phys_writer, pkg_rels)
         # verify -----------------------
         phys_writer.write.assert_called_once_with("/_rels/.rels", pkg_rels.xml)
 
-    def it_can_write_a_list_of_parts(self):
-        # mockery ----------------------
-        phys_writer = Mock(name="phys_writer")
-        rels = MagicMock(name="rels")
-        rels.__len__.return_value = 1
-        part1 = Mock(name="part1", _rels=rels)
-        part2 = Mock(name="part2", _rels=[])
-        # exercise ---------------------
-        PackageWriter._write_parts(phys_writer, [part1, part2])
-        # verify -----------------------
+    def it_can_write_a_list_of_parts(
+        self, phys_pkg_writer_: Mock, part_: Mock, part_2_: Mock, rels_: Mock
+    ):
+        rels_.__len__.return_value = 1
+        part_.rels = rels_
+        part_2_.rels = []
+
+        PackageWriter._write_parts(phys_pkg_writer_, [part_, part_2_])
+
         expected_calls = [
-            call(part1.partname, part1.blob),
-            call(part1.partname.rels_uri, part1._rels.xml),
-            call(part2.partname, part2.blob),
+            call(part_.partname, part_.blob),
+            call(part_.partname.rels_uri, part_.rels.xml),
+            call(part_2_.partname, part_2_.blob),
         ]
-        assert phys_writer.write.mock_calls == expected_calls
+        assert phys_pkg_writer_.write.mock_calls == expected_calls
 
     # fixtures ---------------------------------------------
 
     @pytest.fixture
-    def blob_(self, request):
+    def blob_(self, request: FixtureRequest):
         return instance_mock(request, str)
 
     @pytest.fixture
-    def cti_(self, request, blob_):
+    def cti_(self, request: FixtureRequest, blob_):
         return instance_mock(request, _ContentTypesItem, blob=blob_)
 
     @pytest.fixture
-    def _ContentTypesItem_(self, request, cti_):
+    def _ContentTypesItem_(self, request: FixtureRequest, cti_):
         _ContentTypesItem_ = class_mock(request, "docx.opc.pkgwriter._ContentTypesItem")
         _ContentTypesItem_.from_parts.return_value = cti_
         return _ContentTypesItem_
 
     @pytest.fixture
-    def parts_(self, request):
+    def part_(self, request: FixtureRequest):
+        return instance_mock(request, Part)
+
+    @pytest.fixture
+    def part_2_(self, request: FixtureRequest):
+        return instance_mock(request, Part)
+
+    @pytest.fixture
+    def parts_(self, request: FixtureRequest):
         return instance_mock(request, list)
 
     @pytest.fixture
     def PhysPkgWriter_(self):
         p = patch("docx.opc.pkgwriter.PhysPkgWriter")
         yield p.start()
         p.stop()
 
     @pytest.fixture
-    def phys_pkg_writer_(self, request):
+    def phys_pkg_writer_(self, request: FixtureRequest):
         return instance_mock(request, _ZipPkgWriter)
 
     @pytest.fixture
+    def rels_(self, request: FixtureRequest):
+        return instance_mock(request, Relationships)
+
+    @pytest.fixture
     def write_cti_fixture(self, _ContentTypesItem_, parts_, phys_pkg_writer_, blob_):
         return _ContentTypesItem_, parts_, phys_pkg_writer_, blob_
 
     @pytest.fixture
     def _write_methods(self):
         """Mock that patches all the _write_* methods of PackageWriter"""
         root_mock = Mock(name="PackageWriter")
@@ -119,44 +135,42 @@
         yield root_mock
 
         patch1.stop()
         patch2.stop()
         patch3.stop()
 
     @pytest.fixture
-    def xml_for_(self, request):
+    def xml_for_(self, request: FixtureRequest):
         return method_mock(request, _ContentTypesItem, "xml_for")
 
 
 class Describe_ContentTypesItem:
     def it_can_compose_content_types_element(self, xml_for_fixture):
         cti, expected_xml = xml_for_fixture
         types_elm = cti._element
         assert types_elm.xml == expected_xml
 
     # fixtures ---------------------------------------------
 
-    def _mock_part(self, request, name, partname_str, content_type):
+    def _mock_part(self, request: FixtureRequest, name, partname_str, content_type):
         partname = PackURI(partname_str)
-        return instance_mock(
-            request, Part, name=name, partname=partname, content_type=content_type
-        )
+        return instance_mock(request, Part, name=name, partname=partname, content_type=content_type)
 
     @pytest.fixture(
         params=[
             ("Default", "/ppt/MEDIA/image.PNG", CT.PNG),
             ("Default", "/ppt/media/image.xml", CT.XML),
             ("Default", "/ppt/media/image.rels", CT.OPC_RELATIONSHIPS),
             ("Default", "/ppt/media/image.jpeg", CT.JPEG),
             ("Override", "/docProps/core.xml", "app/vnd.core"),
             ("Override", "/ppt/slides/slide1.xml", "app/vnd.ct_sld"),
             ("Override", "/zebra/foo.bar", "app/vnd.foobar"),
         ]
     )
-    def xml_for_fixture(self, request):
+    def xml_for_fixture(self, request: FixtureRequest):
         elm_type, partname_str, content_type = request.param
         part_ = self._mock_part(request, "part_", partname_str, content_type)
         cti = _ContentTypesItem.from_parts([part_])
         # expected_xml -----------------
         types_bldr = a_Types().with_nsdecls()
         ext = partname_str.split(".")[-1].lower()
         if elm_type == "Default" and ext not in ("rels", "xml"):
@@ -164,17 +178,15 @@
             default_bldr.with_Extension(ext)
             default_bldr.with_ContentType(content_type)
             types_bldr.with_child(default_bldr)
 
         types_bldr.with_child(
             a_Default().with_Extension("rels").with_ContentType(CT.OPC_RELATIONSHIPS)
         )
-        types_bldr.with_child(
-            a_Default().with_Extension("xml").with_ContentType(CT.XML)
-        )
+        types_bldr.with_child(a_Default().with_Extension("xml").with_ContentType(CT.XML))
 
         if elm_type == "Override":
             override_bldr = an_Override()
             override_bldr.with_PartName(partname_str)
             override_bldr.with_ContentType(content_type)
             types_bldr.with_child(override_bldr)
```

### Comparing `python-docx-1.1.0/tests/opc/test_rel.py` & `python_docx-1.1.1/tests/opc/test_rel.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/opc/unitdata/types.py` & `python_docx-1.1.1/tests/opc/unitdata/types.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/oxml/parts/test_document.py` & `python_docx-1.1.1/tests/oxml/parts/test_document.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/oxml/test__init__.py` & `python_docx-1.1.1/tests/oxml/test__init__.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/oxml/test_document.py` & `python_docx-1.1.1/tests/oxml/test_document.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/oxml/test_ns.py` & `python_docx-1.1.1/tests/oxml/test_ns.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/oxml/test_section.py` & `python_docx-1.1.1/tests/oxml/test_section.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/oxml/test_styles.py` & `python_docx-1.1.1/tests/oxml/test_styles.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/oxml/test_table.py` & `python_docx-1.1.1/tests/oxml/test_table.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pyright: reportPrivateUsage=false
+
 """Test suite for the docx.oxml.text module."""
 
 from __future__ import annotations
 
 from typing import cast
 
 import pytest
@@ -9,292 +11,214 @@
 from docx.exceptions import InvalidSpanError
 from docx.oxml.parser import parse_xml
 from docx.oxml.table import CT_Row, CT_Tbl, CT_Tc
 from docx.oxml.text.paragraph import CT_P
 
 from ..unitutil.cxml import element, xml
 from ..unitutil.file import snippet_seq
-from ..unitutil.mock import call, instance_mock, method_mock, property_mock
+from ..unitutil.mock import FixtureRequest, Mock, call, instance_mock, method_mock, property_mock
 
 
 class DescribeCT_Row:
-    def it_can_add_a_trPr(self, add_trPr_fixture):
-        tr, expected_xml = add_trPr_fixture
-        tr._add_trPr()
-        assert tr.xml == expected_xml
 
-    def it_raises_on_tc_at_grid_col(self, tc_raise_fixture):
-        tr, idx = tc_raise_fixture
-        with pytest.raises(ValueError):  # noqa: PT011
-            tr.tc_at_grid_col(idx)
-
-    # fixtures -------------------------------------------------------
-
-    @pytest.fixture(
-        params=[
+    @pytest.mark.parametrize(
+        ("tr_cxml", "expected_cxml"),
+        [
             ("w:tr", "w:tr/w:trPr"),
             ("w:tr/w:tblPrEx", "w:tr/(w:tblPrEx,w:trPr)"),
             ("w:tr/w:tc", "w:tr/(w:trPr,w:tc)"),
             ("w:tr/(w:sdt,w:del,w:tc)", "w:tr/(w:trPr,w:sdt,w:del,w:tc)"),
-        ]
+        ],
     )
-    def add_trPr_fixture(self, request):
-        tr_cxml, expected_cxml = request.param
-        tr = element(tr_cxml)
-        expected_xml = xml(expected_cxml)
-        return tr, expected_xml
-
-    @pytest.fixture(params=[(0, 0, 3), (1, 0, 1)])
-    def tc_raise_fixture(self, request):
-        snippet_idx, row_idx, col_idx = request.param
-        tbl = parse_xml(snippet_seq("tbl-cells")[snippet_idx])
-        tr = tbl.tr_lst[row_idx]
-        return tr, col_idx
+    def it_can_add_a_trPr(self, tr_cxml: str, expected_cxml: str):
+        tr = cast(CT_Row, element(tr_cxml))
+        tr._add_trPr()
+        assert tr.xml == xml(expected_cxml)
+
+    @pytest.mark.parametrize(("snippet_idx", "row_idx", "col_idx"), [(0, 0, 3), (1, 0, 1)])
+    def it_raises_on_tc_at_grid_col(self, snippet_idx: int, row_idx: int, col_idx: int):
+        tr = cast(CT_Tbl, parse_xml(snippet_seq("tbl-cells")[snippet_idx])).tr_lst[row_idx]
+        with pytest.raises(ValueError, match=f"no `tc` element at grid_offset={col_idx}"):
+            tr.tc_at_grid_offset(col_idx)
 
 
 class DescribeCT_Tc:
+    """Unit-test suite for `docx.oxml.table.CT_Tc` objects."""
+
+    @pytest.mark.parametrize(
+        ("tr_cxml", "tc_idx", "expected_value"),
+        [
+            ("w:tr/(w:tc/w:p,w:tc/w:p)", 0, 0),
+            ("w:tr/(w:tc/w:p,w:tc/w:p)", 1, 1),
+            ("w:tr/(w:trPr/w:gridBefore{w:val=2},w:tc/w:p,w:tc/w:p)", 0, 2),
+            ("w:tr/(w:trPr/w:gridBefore{w:val=2},w:tc/w:p,w:tc/w:p)", 1, 3),
+            ("w:tr/(w:trPr/w:gridBefore{w:val=4},w:tc/w:p,w:tc/w:p,w:tc/w:p,w:tc/w:p)", 2, 6),
+        ],
+    )
+    def it_knows_its_grid_offset(self, tr_cxml: str, tc_idx: int, expected_value: int):
+        tr = cast(CT_Row, element(tr_cxml))
+        tc = tr.tc_lst[tc_idx]
+
+        assert tc.grid_offset == expected_value
+
     def it_can_merge_to_another_tc(
-        self, tr_, _span_dimensions_, _tbl_, _grow_to_, top_tc_
+        self, tr_: Mock, _span_dimensions_: Mock, _tbl_: Mock, _grow_to_: Mock, top_tc_: Mock
     ):
         top_tr_ = tr_
-        tc, other_tc = element("w:tc"), element("w:tc")
+        tc, other_tc = cast(CT_Tc, element("w:tc")), cast(CT_Tc, element("w:tc"))
         top, left, height, width = 0, 1, 2, 3
         _span_dimensions_.return_value = top, left, height, width
         _tbl_.return_value.tr_lst = [tr_]
-        tr_.tc_at_grid_col.return_value = top_tc_
+        tr_.tc_at_grid_offset.return_value = top_tc_
 
         merged_tc = tc.merge(other_tc)
 
         _span_dimensions_.assert_called_once_with(tc, other_tc)
-        top_tr_.tc_at_grid_col.assert_called_once_with(left)
+        top_tr_.tc_at_grid_offset.assert_called_once_with(left)
         top_tc_._grow_to.assert_called_once_with(width, height)
         assert merged_tc is top_tc_
 
-    def it_knows_its_extents_to_help(self, extents_fixture):
-        tc, attr_name, expected_value = extents_fixture
-        extent = getattr(tc, attr_name)
-        assert extent == expected_value
-
-    def it_calculates_the_dimensions_of_a_span_to_help(self, span_fixture):
-        tc, other_tc, expected_dimensions = span_fixture
-        dimensions = tc._span_dimensions(other_tc)
-        assert dimensions == expected_dimensions
-
-    def it_raises_on_invalid_span(self, span_raise_fixture):
-        tc, other_tc = span_raise_fixture
-        with pytest.raises(InvalidSpanError):
-            tc._span_dimensions(other_tc)
-
-    def it_can_grow_itself_to_help_merge(self, grow_to_fixture):
-        tc, width, height, top_tc, expected_calls = grow_to_fixture
-        tc._grow_to(width, height, top_tc)
-        assert tc._span_to_width.call_args_list == expected_calls
-
-    def it_can_extend_its_horz_span_to_help_merge(
-        self, top_tc_, grid_span_, _move_content_to_, _swallow_next_tc_
-    ):
-        grid_span_.side_effect = [1, 3, 4]
-        grid_width, vMerge = 4, "continue"
-        tc = element("w:tc")
-
-        tc._span_to_width(grid_width, top_tc_, vMerge)
-
-        _move_content_to_.assert_called_once_with(tc, top_tc_)
-        assert _swallow_next_tc_.call_args_list == [
-            call(tc, grid_width, top_tc_),
-            call(tc, grid_width, top_tc_),
-        ]
-        assert tc.vMerge == vMerge
-
-    def it_knows_its_inner_content_block_item_elements(self):
-        tc = cast(CT_Tc, element("w:tc/(w:p,w:tbl,w:p)"))
-        assert [type(e) for e in tc.inner_content_elements] == [CT_P, CT_Tbl, CT_P]
-
-    def it_can_swallow_the_next_tc_help_merge(self, swallow_fixture):
-        tc, grid_width, top_tc, tr, expected_xml = swallow_fixture
-        tc._swallow_next_tc(grid_width, top_tc)
-        assert tr.xml == expected_xml
-
-    def it_adds_cell_widths_on_swallow(self, add_width_fixture):
-        tc, grid_width, top_tc, tr, expected_xml = add_width_fixture
-        tc._swallow_next_tc(grid_width, top_tc)
-        assert tr.xml == expected_xml
-
-    def it_raises_on_invalid_swallow(self, swallow_raise_fixture):
-        tc, grid_width, top_tc, tr = swallow_raise_fixture
-        with pytest.raises(InvalidSpanError):
-            tc._swallow_next_tc(grid_width, top_tc)
-
-    def it_can_move_its_content_to_help_merge(self, move_fixture):
-        tc, tc_2, expected_tc_xml, expected_tc_2_xml = move_fixture
-        tc._move_content_to(tc_2)
-        assert tc.xml == expected_tc_xml
-        assert tc_2.xml == expected_tc_2_xml
-
-    def it_raises_on_tr_above(self, tr_above_raise_fixture):
-        tc = tr_above_raise_fixture
-        with pytest.raises(ValueError, match="no tr above topmost tr"):
-            tc._tr_above
-
-    # fixtures -------------------------------------------------------
-
-    @pytest.fixture(
-        params=[
-            # both cells have a width
-            (
-                "w:tr/(w:tc/(w:tcPr/w:tcW{w:w=1440,w:type=dxa},w:p),"
-                "w:tc/(w:tcPr/w:tcW{w:w=1440,w:type=dxa},w:p))",
-                0,
-                2,
-                "w:tr/(w:tc/(w:tcPr/(w:tcW{w:w=2880,w:type=dxa},"
-                "w:gridSpan{w:val=2}),w:p))",
-            ),
-            # neither have a width
-            (
-                "w:tr/(w:tc/w:p,w:tc/w:p)",
-                0,
-                2,
-                "w:tr/(w:tc/(w:tcPr/w:gridSpan{w:val=2},w:p))",
-            ),
-            # only second one has a width
-            (
-                "w:tr/(w:tc/w:p," "w:tc/(w:tcPr/w:tcW{w:w=1440,w:type=dxa},w:p))",
-                0,
-                2,
-                "w:tr/(w:tc/(w:tcPr/w:gridSpan{w:val=2},w:p))",
-            ),
-            # only first one has a width
-            (
-                "w:tr/(w:tc/(w:tcPr/w:tcW{w:w=1440,w:type=dxa},w:p)," "w:tc/w:p)",
-                0,
-                2,
-                "w:tr/(w:tc/(w:tcPr/(w:tcW{w:w=1440,w:type=dxa},"
-                "w:gridSpan{w:val=2}),w:p))",
-            ),
-        ]
-    )
-    def add_width_fixture(self, request):
-        tr_cxml, tc_idx, grid_width, expected_tr_cxml = request.param
-        tr = element(tr_cxml)
-        tc = top_tc = tr[tc_idx]
-        expected_tr_xml = xml(expected_tr_cxml)
-        return tc, grid_width, top_tc, tr, expected_tr_xml
-
-    @pytest.fixture(
-        params=[
+    @pytest.mark.parametrize(
+        ("snippet_idx", "row", "col", "attr_name", "expected_value"),
+        [
             (0, 0, 0, "top", 0),
             (2, 0, 1, "top", 0),
             (2, 1, 1, "top", 0),
             (4, 2, 1, "top", 1),
             (0, 0, 0, "left", 0),
             (1, 0, 1, "left", 2),
             (3, 1, 0, "left", 0),
             (3, 1, 1, "left", 2),
             (0, 0, 0, "bottom", 1),
             (1, 0, 0, "bottom", 1),
             (2, 0, 1, "bottom", 2),
             (4, 1, 1, "bottom", 3),
             (0, 0, 0, "right", 1),
             (1, 0, 0, "right", 2),
-            (0, 0, 0, "right", 1),
             (4, 2, 1, "right", 3),
-        ]
+        ],
     )
-    def extents_fixture(self, request):
-        snippet_idx, row, col, attr_name, expected_value = request.param
+    def it_knows_its_extents_to_help(
+        self, snippet_idx: int, row: int, col: int, attr_name: str, expected_value: int
+    ):
         tbl = self._snippet_tbl(snippet_idx)
         tc = tbl.tr_lst[row].tc_lst[col]
-        return tc, attr_name, expected_value
 
-    @pytest.fixture(
-        params=[
-            (0, 0, 0, 2, 1),
-            (0, 0, 1, 1, 2),
-            (0, 1, 1, 2, 2),
-            (1, 0, 0, 2, 2),
-            (2, 0, 0, 2, 2),
-            (2, 1, 2, 1, 2),
-        ]
-    )
-    def grow_to_fixture(self, request, _span_to_width_):
-        snippet_idx, row, col, width, height = request.param
-        tbl = self._snippet_tbl(snippet_idx)
-        tc = tbl.tr_lst[row].tc_lst[col]
-        start = 0 if height == 1 else 1
-        end = start + height
-        expected_calls = [
-            call(width, tc, None),
-            call(width, tc, "restart"),
-            call(width, tc, "continue"),
-            call(width, tc, "continue"),
-        ][start:end]
-        return tc, width, height, None, expected_calls
+        extent = getattr(tc, attr_name)
 
-    @pytest.fixture(
-        params=[
-            ("w:tc/w:p", "w:tc/w:p", "w:tc/w:p", "w:tc/w:p"),
-            ("w:tc/w:p", "w:tc/w:p/w:r", "w:tc/w:p", "w:tc/w:p/w:r"),
-            ("w:tc/w:p/w:r", "w:tc/w:p", "w:tc/w:p", "w:tc/w:p/w:r"),
-            ("w:tc/(w:p/w:r,w:sdt)", "w:tc/w:p", "w:tc/w:p", "w:tc/(w:p/w:r,w:sdt)"),
-            (
-                "w:tc/(w:p/w:r,w:sdt)",
-                "w:tc/(w:tbl,w:p)",
-                "w:tc/w:p",
-                "w:tc/(w:tbl,w:p/w:r,w:sdt)",
-            ),
-        ]
-    )
-    def move_fixture(self, request):
-        tc_cxml, tc_2_cxml, expected_tc_cxml, expected_tc_2_cxml = request.param
-        tc, tc_2 = element(tc_cxml), element(tc_2_cxml)
-        expected_tc_xml = xml(expected_tc_cxml)
-        expected_tc_2_xml = xml(expected_tc_2_cxml)
-        return tc, tc_2, expected_tc_xml, expected_tc_2_xml
+        assert extent == expected_value
 
-    @pytest.fixture(
-        params=[
+    @pytest.mark.parametrize(
+        ("snippet_idx", "row", "col", "row_2", "col_2", "expected_value"),
+        [
             (0, 0, 0, 0, 1, (0, 0, 1, 2)),
             (0, 0, 1, 2, 1, (0, 1, 3, 1)),
             (0, 2, 2, 1, 1, (1, 1, 2, 2)),
             (0, 1, 2, 1, 0, (1, 0, 1, 3)),
             (1, 0, 0, 1, 1, (0, 0, 2, 2)),
             (1, 0, 1, 0, 0, (0, 0, 1, 3)),
             (2, 0, 1, 2, 1, (0, 1, 3, 1)),
             (2, 0, 1, 1, 0, (0, 0, 2, 2)),
             (2, 1, 2, 0, 1, (0, 1, 2, 2)),
             (4, 0, 1, 0, 0, (0, 0, 1, 3)),
-        ]
+        ],
     )
-    def span_fixture(self, request):
-        snippet_idx, row, col, row_2, col_2, expected_value = request.param
+    def it_calculates_the_dimensions_of_a_span_to_help(
+        self,
+        snippet_idx: int,
+        row: int,
+        col: int,
+        row_2: int,
+        col_2: int,
+        expected_value: tuple[int, int, int, int],
+    ):
         tbl = self._snippet_tbl(snippet_idx)
         tc = tbl.tr_lst[row].tc_lst[col]
-        tc_2 = tbl.tr_lst[row_2].tc_lst[col_2]
-        return tc, tc_2, expected_value
+        other_tc = tbl.tr_lst[row_2].tc_lst[col_2]
+
+        dimensions = tc._span_dimensions(other_tc)
+
+        assert dimensions == expected_value
 
-    @pytest.fixture(
-        params=[
+    @pytest.mark.parametrize(
+        ("snippet_idx", "row", "col", "row_2", "col_2"),
+        [
             (1, 0, 0, 1, 0),  # inverted-L horz
             (1, 1, 0, 0, 0),  # same in opposite order
             (2, 0, 2, 0, 1),  # inverted-L vert
             (5, 0, 1, 1, 0),  # tee-shape horz bar
             (5, 1, 0, 2, 1),  # same, opposite side
             (6, 1, 0, 0, 1),  # tee-shape vert bar
             (6, 0, 1, 1, 2),  # same, opposite side
-        ]
+        ],
     )
-    def span_raise_fixture(self, request):
-        snippet_idx, row, col, row_2, col_2 = request.param
+    def it_raises_on_invalid_span(
+        self, snippet_idx: int, row: int, col: int, row_2: int, col_2: int
+    ):
         tbl = self._snippet_tbl(snippet_idx)
         tc = tbl.tr_lst[row].tc_lst[col]
-        tc_2 = tbl.tr_lst[row_2].tc_lst[col_2]
-        return tc, tc_2
+        other_tc = tbl.tr_lst[row_2].tc_lst[col_2]
+
+        with pytest.raises(InvalidSpanError):
+            tc._span_dimensions(other_tc)
+
+    @pytest.mark.parametrize(
+        ("snippet_idx", "row", "col", "width", "height"),
+        [
+            (0, 0, 0, 2, 1),
+            (0, 0, 1, 1, 2),
+            (0, 1, 1, 2, 2),
+            (1, 0, 0, 2, 2),
+            (2, 0, 0, 2, 2),
+            (2, 1, 2, 1, 2),
+        ],
+    )
+    def it_can_grow_itself_to_help_merge(
+        self, snippet_idx: int, row: int, col: int, width: int, height: int, _span_to_width_: Mock
+    ):
+        tbl = self._snippet_tbl(snippet_idx)
+        tc = tbl.tr_lst[row].tc_lst[col]
+        start = 0 if height == 1 else 1
+        end = start + height
 
-    @pytest.fixture(
-        params=[
+        tc._grow_to(width, height, None)
+
+        assert (
+            _span_to_width_.call_args_list
+            == [
+                call(width, tc, None),
+                call(width, tc, "restart"),
+                call(width, tc, "continue"),
+                call(width, tc, "continue"),
+            ][start:end]
+        )
+
+    def it_can_extend_its_horz_span_to_help_merge(
+        self, top_tc_: Mock, grid_span_: Mock, _move_content_to_: Mock, _swallow_next_tc_: Mock
+    ):
+        grid_span_.side_effect = [1, 3, 4]
+        grid_width, vMerge = 4, "continue"
+        tc = cast(CT_Tc, element("w:tc"))
+
+        tc._span_to_width(grid_width, top_tc_, vMerge)
+
+        _move_content_to_.assert_called_once_with(tc, top_tc_)
+        assert _swallow_next_tc_.call_args_list == [
+            call(tc, grid_width, top_tc_),
+            call(tc, grid_width, top_tc_),
+        ]
+        assert tc.vMerge == vMerge
+
+    def it_knows_its_inner_content_block_item_elements(self):
+        tc = cast(CT_Tc, element("w:tc/(w:p,w:tbl,w:p)"))
+        assert [type(e) for e in tc.inner_content_elements] == [CT_P, CT_Tbl, CT_P]
+
+    @pytest.mark.parametrize(
+        ("tr_cxml", "tc_idx", "grid_width", "expected_cxml"),
+        [
             (
                 "w:tr/(w:tc/w:p,w:tc/w:p)",
                 0,
                 2,
                 "w:tr/(w:tc/(w:tcPr/w:gridSpan{w:val=2},w:p))",
             ),
             (
@@ -303,94 +227,163 @@
                 2,
                 "w:tr/(w:tc/w:p,w:tc/(w:tcPr/w:gridSpan{w:val=2},w:p))",
             ),
             (
                 'w:tr/(w:tc/w:p/w:r/w:t"a",w:tc/w:p/w:r/w:t"b")',
                 0,
                 2,
-                'w:tr/(w:tc/(w:tcPr/w:gridSpan{w:val=2},w:p/w:r/w:t"a",'
-                'w:p/w:r/w:t"b"))',
+                'w:tr/(w:tc/(w:tcPr/w:gridSpan{w:val=2},w:p/w:r/w:t"a",' 'w:p/w:r/w:t"b"))',
             ),
             (
                 "w:tr/(w:tc/(w:tcPr/w:gridSpan{w:val=2},w:p),w:tc/w:p)",
                 0,
                 3,
                 "w:tr/(w:tc/(w:tcPr/w:gridSpan{w:val=3},w:p))",
             ),
             (
                 "w:tr/(w:tc/w:p,w:tc/(w:tcPr/w:gridSpan{w:val=2},w:p))",
                 0,
                 3,
                 "w:tr/(w:tc/(w:tcPr/w:gridSpan{w:val=3},w:p))",
             ),
-        ]
+        ],
+    )
+    def it_can_swallow_the_next_tc_help_merge(
+        self, tr_cxml: str, tc_idx: int, grid_width: int, expected_cxml: str
+    ):
+        tr = cast(CT_Row, element(tr_cxml))
+        tc = top_tc = tr.tc_lst[tc_idx]
+
+        tc._swallow_next_tc(grid_width, top_tc)
+
+        assert tr.xml == xml(expected_cxml)
+
+    @pytest.mark.parametrize(
+        ("tr_cxml", "tc_idx", "grid_width", "expected_cxml"),
+        [
+            # both cells have a width
+            (
+                "w:tr/(w:tc/(w:tcPr/w:tcW{w:w=1440,w:type=dxa},w:p),"
+                "w:tc/(w:tcPr/w:tcW{w:w=1440,w:type=dxa},w:p))",
+                0,
+                2,
+                "w:tr/(w:tc/(w:tcPr/(w:tcW{w:w=2880,w:type=dxa}," "w:gridSpan{w:val=2}),w:p))",
+            ),
+            # neither have a width
+            (
+                "w:tr/(w:tc/w:p,w:tc/w:p)",
+                0,
+                2,
+                "w:tr/(w:tc/(w:tcPr/w:gridSpan{w:val=2},w:p))",
+            ),
+            # only second one has a width
+            (
+                "w:tr/(w:tc/w:p," "w:tc/(w:tcPr/w:tcW{w:w=1440,w:type=dxa},w:p))",
+                0,
+                2,
+                "w:tr/(w:tc/(w:tcPr/w:gridSpan{w:val=2},w:p))",
+            ),
+            # only first one has a width
+            (
+                "w:tr/(w:tc/(w:tcPr/w:tcW{w:w=1440,w:type=dxa},w:p)," "w:tc/w:p)",
+                0,
+                2,
+                "w:tr/(w:tc/(w:tcPr/(w:tcW{w:w=1440,w:type=dxa}," "w:gridSpan{w:val=2}),w:p))",
+            ),
+        ],
     )
-    def swallow_fixture(self, request):
-        tr_cxml, tc_idx, grid_width, expected_tr_cxml = request.param
-        tr = element(tr_cxml)
-        tc = top_tc = tr[tc_idx]
-        expected_tr_xml = xml(expected_tr_cxml)
-        return tc, grid_width, top_tc, tr, expected_tr_xml
+    def it_adds_cell_widths_on_swallow(
+        self, tr_cxml: str, tc_idx: int, grid_width: int, expected_cxml: str
+    ):
+        tr = cast(CT_Row, element(tr_cxml))
+        tc = top_tc = tr.tc_lst[tc_idx]
+        tc._swallow_next_tc(grid_width, top_tc)
+        assert tr.xml == xml(expected_cxml)
 
-    @pytest.fixture(
-        params=[
+    @pytest.mark.parametrize(
+        ("tr_cxml", "tc_idx", "grid_width"),
+        [
             ("w:tr/w:tc/w:p", 0, 2),
             ("w:tr/(w:tc/w:p,w:tc/(w:tcPr/w:gridSpan{w:val=2},w:p))", 0, 2),
-        ]
+        ],
     )
-    def swallow_raise_fixture(self, request):
-        tr_cxml, tc_idx, grid_width = request.param
-        tr = element(tr_cxml)
-        tc = top_tc = tr[tc_idx]
-        return tc, grid_width, top_tc, tr
-
-    @pytest.fixture(params=[(0, 0, 0), (4, 0, 0)])
-    def tr_above_raise_fixture(self, request):
-        snippet_idx, row_idx, col_idx = request.param
-        tbl = parse_xml(snippet_seq("tbl-cells")[snippet_idx])
+    def it_raises_on_invalid_swallow(self, tr_cxml: str, tc_idx: int, grid_width: int):
+        tr = cast(CT_Row, element(tr_cxml))
+        tc = top_tc = tr.tc_lst[tc_idx]
+
+        with pytest.raises(InvalidSpanError):
+            tc._swallow_next_tc(grid_width, top_tc)
+
+    @pytest.mark.parametrize(
+        ("tc_cxml", "tc_2_cxml", "expected_tc_cxml", "expected_tc_2_cxml"),
+        [
+            ("w:tc/w:p", "w:tc/w:p", "w:tc/w:p", "w:tc/w:p"),
+            ("w:tc/w:p", "w:tc/w:p/w:r", "w:tc/w:p", "w:tc/w:p/w:r"),
+            ("w:tc/w:p/w:r", "w:tc/w:p", "w:tc/w:p", "w:tc/w:p/w:r"),
+            ("w:tc/(w:p/w:r,w:sdt)", "w:tc/w:p", "w:tc/w:p", "w:tc/(w:p/w:r,w:sdt)"),
+            (
+                "w:tc/(w:p/w:r,w:sdt)",
+                "w:tc/(w:tbl,w:p)",
+                "w:tc/w:p",
+                "w:tc/(w:tbl,w:p/w:r,w:sdt)",
+            ),
+        ],
+    )
+    def it_can_move_its_content_to_help_merge(
+        self, tc_cxml: str, tc_2_cxml: str, expected_tc_cxml: str, expected_tc_2_cxml: str
+    ):
+        tc, tc_2 = cast(CT_Tc, element(tc_cxml)), cast(CT_Tc, element(tc_2_cxml))
+
+        tc._move_content_to(tc_2)
+
+        assert tc.xml == xml(expected_tc_cxml)
+        assert tc_2.xml == xml(expected_tc_2_cxml)
+
+    @pytest.mark.parametrize(("snippet_idx", "row_idx", "col_idx"), [(0, 0, 0), (4, 0, 0)])
+    def it_raises_on_tr_above(self, snippet_idx: int, row_idx: int, col_idx: int):
+        tbl = cast(CT_Tbl, parse_xml(snippet_seq("tbl-cells")[snippet_idx]))
         tc = tbl.tr_lst[row_idx].tc_lst[col_idx]
-        return tc
 
-    # fixture components ---------------------------------------------
+        with pytest.raises(ValueError, match="no tr above topmost tr"):
+            tc._tr_above
+
+    # fixtures -------------------------------------------------------
 
     @pytest.fixture
-    def grid_span_(self, request):
+    def grid_span_(self, request: FixtureRequest):
         return property_mock(request, CT_Tc, "grid_span")
 
     @pytest.fixture
-    def _grow_to_(self, request):
+    def _grow_to_(self, request: FixtureRequest):
         return method_mock(request, CT_Tc, "_grow_to")
 
     @pytest.fixture
-    def _move_content_to_(self, request):
+    def _move_content_to_(self, request: FixtureRequest):
         return method_mock(request, CT_Tc, "_move_content_to")
 
     @pytest.fixture
-    def _span_dimensions_(self, request):
+    def _span_dimensions_(self, request: FixtureRequest):
         return method_mock(request, CT_Tc, "_span_dimensions")
 
     @pytest.fixture
-    def _span_to_width_(self, request):
+    def _span_to_width_(self, request: FixtureRequest):
         return method_mock(request, CT_Tc, "_span_to_width", autospec=False)
 
-    def _snippet_tbl(self, idx):
-        """
-        Return a <w:tbl> element for snippet at `idx` in 'tbl-cells' snippet
-        file.
-        """
-        return parse_xml(snippet_seq("tbl-cells")[idx])
+    def _snippet_tbl(self, idx: int) -> CT_Tbl:
+        """A <w:tbl> element for snippet at `idx` in 'tbl-cells' snippet file."""
+        return cast(CT_Tbl, parse_xml(snippet_seq("tbl-cells")[idx]))
 
     @pytest.fixture
-    def _swallow_next_tc_(self, request):
+    def _swallow_next_tc_(self, request: FixtureRequest):
         return method_mock(request, CT_Tc, "_swallow_next_tc")
 
     @pytest.fixture
-    def _tbl_(self, request):
+    def _tbl_(self, request: FixtureRequest):
         return property_mock(request, CT_Tc, "_tbl")
 
     @pytest.fixture
-    def top_tc_(self, request):
+    def top_tc_(self, request: FixtureRequest):
         return instance_mock(request, CT_Tc)
 
     @pytest.fixture
-    def tr_(self, request):
+    def tr_(self, request: FixtureRequest):
         return instance_mock(request, CT_Row)
```

### Comparing `python-docx-1.1.0/tests/oxml/test_xmlchemy.py` & `python_docx-1.1.1/tests/oxml/test_xmlchemy.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/oxml/text/test_hyperlink.py` & `python_docx-1.1.1/tests/oxml/text/test_hyperlink.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/oxml/text/test_run.py` & `python_docx-1.1.1/tests/oxml/text/test_run.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/oxml/unitdata/dml.py` & `python_docx-1.1.1/tests/oxml/unitdata/dml.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/oxml/unitdata/section.py` & `python_docx-1.1.1/tests/oxml/unitdata/section.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/oxml/unitdata/shared.py` & `python_docx-1.1.1/tests/oxml/unitdata/shared.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/oxml/unitdata/text.py` & `python_docx-1.1.1/tests/oxml/unitdata/text.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/parts/test_document.py` & `python_docx-1.1.1/tests/parts/test_document.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/parts/test_hdrftr.py` & `python_docx-1.1.1/tests/parts/test_hdrftr.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/parts/test_image.py` & `python_docx-1.1.1/tests/parts/test_image.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/parts/test_numbering.py` & `python_docx-1.1.1/tests/parts/test_numbering.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/parts/test_settings.py` & `python_docx-1.1.1/tests/parts/test_settings.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/parts/test_story.py` & `python_docx-1.1.1/tests/parts/test_story.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/parts/test_styles.py` & `python_docx-1.1.1/tests/parts/test_styles.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/styles/test_latent.py` & `python_docx-1.1.1/tests/styles/test_latent.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/styles/test_style.py` & `python_docx-1.1.1/tests/styles/test_style.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/styles/test_styles.py` & `python_docx-1.1.1/tests/styles/test_styles.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_api.py` & `python_docx-1.1.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_blkcntnr.py` & `python_docx-1.1.1/tests/test_blkcntnr.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_document.py` & `python_docx-1.1.1/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_enum.py` & `python_docx-1.1.1/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/150-dpi.png` & `python_docx-1.1.1/tests/test_files/150-dpi.png`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/300-dpi.TIF` & `python_docx-1.1.1/tests/test_files/300-dpi.TIF`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/300-dpi.jpg` & `python_docx-1.1.1/tests/test_files/300-dpi.jpg`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/300-dpi.png` & `python_docx-1.1.1/tests/test_files/300-dpi.png`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/72-dpi.tiff` & `python_docx-1.1.1/tests/test_files/72-dpi.tiff`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/CVS_LOGO.WMF` & `python_docx-1.1.1/tests/test_files/CVS_LOGO.WMF`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/blk-inner-content.docx` & `python_docx-1.1.1/tests/test_files/blk-inner-content.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/exif-420-dpi.jpg` & `python_docx-1.1.1/tests/test_files/exif-420-dpi.jpg`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/expanded_docx/[Content_Types].xml` & `python_docx-1.1.1/tests/test_files/expanded_docx/[Content_Types].xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/expanded_docx/_rels/.rels` & `python_docx-1.1.1/tests/test_files/expanded_docx/_rels/.rels`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/expanded_docx/docProps/app.xml` & `python_docx-1.1.1/tests/test_files/expanded_docx/docProps/app.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/expanded_docx/docProps/core.xml` & `python_docx-1.1.1/tests/test_files/expanded_docx/docProps/core.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/expanded_docx/docProps/thumbnail.jpeg` & `python_docx-1.1.1/tests/test_files/expanded_docx/docProps/thumbnail.jpeg`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/expanded_docx/word/_rels/document.xml.rels` & `python_docx-1.1.1/tests/test_files/expanded_docx/word/_rels/document.xml.rels`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/expanded_docx/word/document.xml` & `python_docx-1.1.1/tests/test_files/expanded_docx/word/document.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/expanded_docx/word/fontTable.xml` & `python_docx-1.1.1/tests/test_files/expanded_docx/word/fontTable.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/expanded_docx/word/numbering.xml` & `python_docx-1.1.1/tests/test_files/expanded_docx/word/numbering.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/expanded_docx/word/settings.xml` & `python_docx-1.1.1/tests/test_files/expanded_docx/word/settings.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/expanded_docx/word/styles.xml` & `python_docx-1.1.1/tests/test_files/expanded_docx/word/styles.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/expanded_docx/word/stylesWithEffects.xml` & `python_docx-1.1.1/tests/test_files/expanded_docx/word/stylesWithEffects.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/expanded_docx/word/theme/theme1.xml` & `python_docx-1.1.1/tests/test_files/expanded_docx/word/theme/theme1.xml`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/having-images.docx` & `python_docx-1.1.1/tests/test_files/having-images.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/jfif-iguana.jpg` & `python_docx-1.1.1/tests/test_files/jfif-iguana.jpg`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/little-endian.tif` & `python_docx-1.1.1/tests/test_files/little-endian.tif`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/monty-truth.png` & `python_docx-1.1.1/tests/test_files/monty-truth.png`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/python-icon.jpeg` & `python_docx-1.1.1/tests/test_files/python-icon.jpeg`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/python-icon.png` & `python_docx-1.1.1/tests/test_files/python-icon.png`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/python-powered.png` & `python_docx-1.1.1/tests/test_files/python-powered.png`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/python.bmp` & `python_docx-1.1.1/tests/test_files/python.bmp`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/sct-inner-content.docx` & `python_docx-1.1.1/tests/test_files/sct-inner-content.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/snippets/add-row-col.txt` & `python_docx-1.1.1/tests/test_files/snippets/add-row-col.txt`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/snippets/inline.txt` & `python_docx-1.1.1/tests/test_files/snippets/inline.txt`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/snippets/new-tbl.txt` & `python_docx-1.1.1/tests/test_files/snippets/new-tbl.txt`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/snippets/tbl-cells.txt` & `python_docx-1.1.1/tests/test_files/snippets/tbl-cells.txt`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/sonic.gif` & `python_docx-1.1.1/tests/test_files/sonic.gif`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_files/test.docx` & `python_docx-1.1.1/tests/test_files/test.docx`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_package.py` & `python_docx-1.1.1/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_section.py` & `python_docx-1.1.1/tests/test_section.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_settings.py` & `python_docx-1.1.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_shape.py` & `python_docx-1.1.1/tests/test_shape.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/test_shared.py` & `python_docx-1.1.1/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/text/test_font.py` & `python_docx-1.1.1/tests/text/test_font.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/text/test_hyperlink.py` & `python_docx-1.1.1/tests/text/test_hyperlink.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/text/test_pagebreak.py` & `python_docx-1.1.1/tests/text/test_pagebreak.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/text/test_paragraph.py` & `python_docx-1.1.1/tests/text/test_paragraph.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/text/test_parfmt.py` & `python_docx-1.1.1/tests/text/test_parfmt.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/text/test_run.py` & `python_docx-1.1.1/tests/text/test_run.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/text/test_tabstops.py` & `python_docx-1.1.1/tests/text/test_tabstops.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/unitdata.py` & `python_docx-1.1.1/tests/unitdata.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/unitutil/cxml.py` & `python_docx-1.1.1/tests/unitutil/cxml.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
     @classmethod
     def from_token(cls, token):
         """
         Return an ``Element`` object constructed from a parser element token.
         """
         tagname = token.tagname
-        attrs = [(name, value) for name, value in token.attr_list]
+        attrs = [tuple(a) for a in token.attr_list]
         text = token.text
         return cls(tagname, attrs, text)
 
     @property
     def is_root(self):
         """
         |True| if this element is the root of the tree and should include the
@@ -259,16 +259,14 @@
     node = Group(
         element("element") + Group(Optional(slash + child_node_list))("child_node_list")
     ).setParseAction(connect_node_children)
 
     child_node_list << (open_paren + delimitedList(node) + close_paren | node)
 
     root_node = (
-        element("element")
-        + Group(Optional(slash + child_node_list))("child_node_list")
-        + stringEnd
+        element("element") + Group(Optional(slash + child_node_list))("child_node_list") + stringEnd
     ).setParseAction(connect_root_node_children)
 
     return root_node
 
 
 root_node = grammar()
```

### Comparing `python-docx-1.1.0/tests/unitutil/file.py` & `python_docx-1.1.1/tests/unitutil/file.py`

 * *Files identical despite different names*

### Comparing `python-docx-1.1.0/tests/unitutil/mock.py` & `python_docx-1.1.1/tests/unitutil/mock.py`

 * *Files identical despite different names*

