# Comparing `tmp/pdfreader-0.1.8.tar.gz` & `tmp/pdfreader-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfreader-0.1.8.tar", last modified: Sat Jan 30 03:35:39 2021, max compression
+gzip compressed data, was "pdfreader-0.1.9.tar", last modified: Mon Feb 22 02:39:48 2021, max compression
```

## Comparing `pdfreader-0.1.8.tar` & `pdfreader-0.1.9.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-01-30 03:35:39.084529 pdfreader-0.1.8/
--rw-r--r--   0 maxp       (502) staff       (20)     1626 2021-01-30 03:30:14.000000 pdfreader-0.1.8/CHANGELOG.txt
--rw-r--r--   0 maxp       (502) staff       (20)      377 2019-11-25 16:57:07.000000 pdfreader-0.1.8/CONTRIBUTING.rst
--rw-r--r--   0 maxp       (502) staff       (20)     1071 2019-11-25 16:57:07.000000 pdfreader-0.1.8/LICENSE
--rw-r--r--   0 maxp       (502) staff       (20)      518 2020-12-17 19:25:24.000000 pdfreader-0.1.8/MANIFEST.in
--rw-r--r--   0 maxp       (502) staff       (20)     4889 2021-01-30 03:35:39.083830 pdfreader-0.1.8/PKG-INFO
--rw-r--r--   0 maxp       (502) staff       (20)     3266 2020-11-14 00:38:48.000000 pdfreader-0.1.8/README.rst
--rw-r--r--   0 maxp       (502) staff       (20)      643 2020-12-17 17:36:24.000000 pdfreader-0.1.8/SECURITY.md
--rw-r--r--   0 maxp       (502) staff       (20)    26134 2020-12-17 16:42:07.000000 pdfreader-0.1.8/THIRD-PARTY-NOTICES
-drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-01-30 03:35:38.909882 pdfreader-0.1.8/doc/
--rw-r--r--   0 maxp       (502) staff       (20)        1 2019-11-25 16:57:07.000000 pdfreader-0.1.8/doc/__init__.py
-drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-01-30 03:35:38.913987 pdfreader-0.1.8/doc/api/
--rw-r--r--   0 maxp       (502) staff       (20)      333 2019-11-25 21:06:14.000000 pdfreader-0.1.8/doc/api/document.rst
--rw-r--r--   0 maxp       (502) staff       (20)     1209 2019-11-26 19:24:18.000000 pdfreader-0.1.8/doc/api/index.rst
--rw-r--r--   0 maxp       (502) staff       (20)     1064 2019-11-26 19:24:18.000000 pdfreader-0.1.8/doc/api/types.rst
--rw-r--r--   0 maxp       (502) staff       (20)     2053 2020-12-17 19:21:07.000000 pdfreader-0.1.8/doc/api/viewer.rst
--rw-r--r--   0 maxp       (502) staff       (20)     5176 2019-11-26 19:24:18.000000 pdfreader-0.1.8/doc/conf.py
-drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-01-30 03:35:38.926904 pdfreader-0.1.8/doc/examples/
--rw-r--r--   0 maxp       (502) staff       (20)     1808 2019-12-11 19:06:26.000000 pdfreader-0.1.8/doc/examples/document_vs_viewer.rst
-drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-01-30 03:35:38.931413 pdfreader-0.1.8/doc/examples/downloads/
--rw-r--r--   0 maxp       (502) staff       (20)    52644 2019-11-21 18:37:24.000000 pdfreader-0.1.8/doc/examples/downloads/example-crash-markdown.txt
--rw-r--r--   0 maxp       (502) staff       (20)      229 2019-11-21 18:17:46.000000 pdfreader-0.1.8/doc/examples/downloads/sample-cmap.txt
--rw-r--r--   0 maxp       (502) staff       (20)    19349 2019-11-21 17:20:49.000000 pdfreader-0.1.8/doc/examples/downloads/tutorial-sample-content-stream-p1.txt
--rw-r--r--   0 maxp       (502) staff       (20)     2550 2019-12-11 19:06:26.000000 pdfreader-0.1.8/doc/examples/extract_cmap.rst
--rw-r--r--   0 maxp       (502) staff       (20)     2216 2019-12-20 15:58:08.000000 pdfreader-0.1.8/doc/examples/extract_fonts.rst
--rw-r--r--   0 maxp       (502) staff       (20)     2306 2019-12-20 15:58:08.000000 pdfreader-0.1.8/doc/examples/extract_form_text.rst
--rw-r--r--   0 maxp       (502) staff       (20)     4603 2019-12-11 19:06:26.000000 pdfreader-0.1.8/doc/examples/extract_image.rst
--rw-r--r--   0 maxp       (502) staff       (20)     4222 2019-12-11 19:06:26.000000 pdfreader-0.1.8/doc/examples/extract_page_text.rst
-drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-01-30 03:35:38.937654 pdfreader-0.1.8/doc/examples/img/
--rw-r--r--   0 maxp       (502) staff       (20)      298 2019-11-25 16:57:07.000000 pdfreader-0.1.8/doc/examples/img/example-image-mask.png
--rw-r--r--   0 maxp       (502) staff       (20)    13625 2019-11-25 16:57:07.000000 pdfreader-0.1.8/doc/examples/img/example-logo.png
--rw-r--r--   0 maxp       (502) staff       (20)   190916 2019-11-25 16:57:07.000000 pdfreader-0.1.8/doc/examples/img/example-parse-form.png
--rw-r--r--   0 maxp       (502) staff       (20)   172197 2019-11-25 16:57:07.000000 pdfreader-0.1.8/doc/examples/img/example-text-crash-report.png
--rw-r--r--   0 maxp       (502) staff       (20)     1229 2019-12-11 19:06:26.000000 pdfreader-0.1.8/doc/examples/index.rst
--rw-r--r--   0 maxp       (502) staff       (20)     3243 2019-12-11 19:06:26.000000 pdfreader-0.1.8/doc/examples/navigate_objects.rst
-drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-01-30 03:35:38.953171 pdfreader-0.1.8/doc/examples/pdfs/
--rw-r--r--   0 maxp       (502) staff       (20)    18764 2020-09-11 19:48:11.000000 pdfreader-0.1.8/doc/examples/pdfs/annot-sample.pdf
--rw-r--r--   0 maxp       (502) staff       (20)    15452 2020-11-14 00:38:48.000000 pdfreader-0.1.8/doc/examples/pdfs/encrypted-with-qwerty.pdf
--rw-r--r--   0 maxp       (502) staff       (20)    63477 2019-11-25 16:57:07.000000 pdfreader-0.1.8/doc/examples/pdfs/example-font.pdf
--rw-r--r--   0 maxp       (502) staff       (20)   556776 2019-11-25 16:57:07.000000 pdfreader-0.1.8/doc/examples/pdfs/example-form.pdf
--rw-r--r--   0 maxp       (502) staff       (20)    49348 2019-11-25 16:57:07.000000 pdfreader-0.1.8/doc/examples/pdfs/example-image-xobject.pdf
--rw-r--r--   0 maxp       (502) staff       (20)   509714 2019-11-25 16:57:07.000000 pdfreader-0.1.8/doc/examples/pdfs/example-text-crash-report.pdf
--rw-r--r--   0 maxp       (502) staff       (20)  1106383 2019-11-25 16:57:07.000000 pdfreader-0.1.8/doc/examples/pdfs/tutorial-example.pdf
--rw-r--r--   0 maxp       (502) staff       (20)    13625 2020-09-11 19:12:35.000000 pdfreader-0.1.8/doc/extract-logo.png
--rw-r--r--   0 maxp       (502) staff       (20)   175641 2020-09-11 19:12:23.000000 pdfreader-0.1.8/doc/fax-from-p8.png
--rw-r--r--   0 maxp       (502) staff       (20)     3526 2019-12-11 19:06:26.000000 pdfreader-0.1.8/doc/index.rst
--rw-r--r--   0 maxp       (502) staff       (20)     1481 2019-12-11 19:06:26.000000 pdfreader-0.1.8/doc/installation.rst
--rw-r--r--   0 maxp       (502) staff       (20)      298 2020-09-11 19:12:38.000000 pdfreader-0.1.8/doc/mask.png
--rw-r--r--   0 maxp       (502) staff       (20)       74 2019-11-25 16:57:07.000000 pdfreader-0.1.8/doc/requirements.txt
--rw-r--r--   0 maxp       (502) staff       (20)    12772 2020-12-17 19:21:07.000000 pdfreader-0.1.8/doc/tutorial.rst
-drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-01-30 03:35:38.970080 pdfreader-0.1.8/pdfreader/
--rw-r--r--   0 maxp       (502) staff       (20)      209 2021-01-30 03:30:02.000000 pdfreader-0.1.8/pdfreader/__init__.py
--rw-r--r--   0 maxp       (502) staff       (20)     4296 2020-02-20 21:04:21.000000 pdfreader-0.1.8/pdfreader/buffer.py
-drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-01-30 03:35:38.997829 pdfreader-0.1.8/pdfreader/codecs/
--rw-r--r--   0 maxp       (502) staff       (20)      298 2019-11-06 17:10:39.000000 pdfreader-0.1.8/pdfreader/codecs/__init__.py
--rw-r--r--   0 maxp       (502) staff       (20)   110596 2019-11-06 17:10:39.000000 pdfreader-0.1.8/pdfreader/codecs/agl.py
-drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-01-30 03:35:39.016586 pdfreader-0.1.8/pdfreader/codecs/cmaps/
--rw-r--r--   0 maxp       (502) staff       (20)     3829 2019-11-11 14:22:22.000000 pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-CNS1-0
--rw-r--r--   0 maxp       (502) staff       (20)     4122 2019-11-11 14:22:22.000000 pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-CNS1-3
--rw-r--r--   0 maxp       (502) staff       (20)     4142 2019-11-11 14:22:22.000000 pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-CNS1-4
--rw-r--r--   0 maxp       (502) staff       (20)     3292 2019-11-11 14:22:22.000000 pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-GB1-0
--rw-r--r--   0 maxp       (502) staff       (20)     4400 2019-11-11 14:22:22.000000 pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-GB1-2
--rw-r--r--   0 maxp       (502) staff       (20)     4951 2019-11-11 14:22:22.000000 pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-GB1-4
--rw-r--r--   0 maxp       (502) staff       (20)     3342 2019-11-11 14:22:22.000000 pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-Japan1-1
--rw-r--r--   0 maxp       (502) staff       (20)     3380 2019-11-11 14:22:22.000000 pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-Japan1-2
--rw-r--r--   0 maxp       (502) staff       (20)     3868 2019-11-11 14:22:22.000000 pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-Japan1-4
--rw-r--r--   0 maxp       (502) staff       (20)     4248 2019-11-11 14:22:22.000000 pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-Japan1-5
--rw-r--r--   0 maxp       (502) staff       (20)     3433 2019-11-11 14:22:22.000000 pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-Korea1-0
--rw-r--r--   0 maxp       (502) staff       (20)     4089 2019-11-11 14:22:22.000000 pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-Korea1-1
--rw-r--r--   0 maxp       (502) staff       (20)     4088 2019-11-11 14:22:22.000000 pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-Korea1-2
--rw-r--r--   0 maxp       (502) staff       (20)     7820 2019-11-11 14:22:22.000000 pdfreader-0.1.8/pdfreader/codecs/cmaps/Identity-H
--rw-r--r--   0 maxp       (502) staff       (20)       54 2019-11-11 14:31:21.000000 pdfreader-0.1.8/pdfreader/codecs/cmaps/README.md
--rw-r--r--   0 maxp       (502) staff       (20)     4571 2019-11-25 16:57:07.000000 pdfreader-0.1.8/pdfreader/codecs/codec.py
--rw-r--r--   0 maxp       (502) staff       (20)     6531 2020-09-09 00:22:21.000000 pdfreader-0.1.8/pdfreader/codecs/decoder.py
--rw-r--r--   0 maxp       (502) staff       (20)     2325 2019-11-26 16:58:10.000000 pdfreader-0.1.8/pdfreader/codecs/differences.py
--rw-r--r--   0 maxp       (502) staff       (20)     7091 2019-12-11 19:17:56.000000 pdfreader-0.1.8/pdfreader/codecs/macroman.py
--rw-r--r--   0 maxp       (502) staff       (20)     7852 2019-11-25 16:57:07.000000 pdfreader-0.1.8/pdfreader/codecs/pdfdoc.py
--rw-r--r--   0 maxp       (502) staff       (20)     4853 2019-11-25 16:57:07.000000 pdfreader-0.1.8/pdfreader/codecs/standard.py
--rw-r--r--   0 maxp       (502) staff       (20)      469 2019-11-11 18:20:02.000000 pdfreader-0.1.8/pdfreader/codecs/tests.py
--rw-r--r--   0 maxp       (502) staff       (20)     7455 2019-12-11 19:17:49.000000 pdfreader-0.1.8/pdfreader/codecs/winansi.py
--rw-r--r--   0 maxp       (502) staff       (20)     3614 2019-11-06 17:10:39.000000 pdfreader-0.1.8/pdfreader/codecs/zapfdingbatsgl.py
--rw-r--r--   0 maxp       (502) staff       (20)     3818 2019-11-11 14:58:52.000000 pdfreader-0.1.8/pdfreader/constants.py
--rw-r--r--   0 maxp       (502) staff       (20)     4226 2020-11-14 00:38:48.000000 pdfreader-0.1.8/pdfreader/document.py
--rw-r--r--   0 maxp       (502) staff       (20)      135 2020-08-27 19:40:05.000000 pdfreader-0.1.8/pdfreader/exceptions.py
-drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-01-30 03:35:39.039860 pdfreader-0.1.8/pdfreader/filters/
--rw-r--r--   0 maxp       (502) staff       (20)      601 2020-09-09 00:22:21.000000 pdfreader-0.1.8/pdfreader/filters/__init__.py
--rw-r--r--   0 maxp       (502) staff       (20)      793 2019-11-08 20:47:35.000000 pdfreader-0.1.8/pdfreader/filters/ascii85.py
--rw-r--r--   0 maxp       (502) staff       (20)     1194 2019-11-08 20:47:35.000000 pdfreader-0.1.8/pdfreader/filters/asciihex.py
--rw-r--r--   0 maxp       (502) staff       (20)    19621 2020-12-17 17:20:54.000000 pdfreader-0.1.8/pdfreader/filters/ccittfax.py
--rw-r--r--   0 maxp       (502) staff       (20)       94 2019-11-06 17:10:39.000000 pdfreader-0.1.8/pdfreader/filters/crypt.py
--rw-r--r--   0 maxp       (502) staff       (20)      108 2020-01-02 19:04:17.000000 pdfreader-0.1.8/pdfreader/filters/dct.py
--rw-r--r--   0 maxp       (502) staff       (20)      675 2019-11-06 17:10:39.000000 pdfreader-0.1.8/pdfreader/filters/flate.py
--rw-r--r--   0 maxp       (502) staff       (20)      106 2019-11-06 17:10:39.000000 pdfreader-0.1.8/pdfreader/filters/jbig2.py
--rw-r--r--   0 maxp       (502) staff       (20)      102 2019-11-06 17:10:39.000000 pdfreader-0.1.8/pdfreader/filters/jpx.py
--rw-r--r--   0 maxp       (502) staff       (20)     8942 2019-11-06 17:10:39.000000 pdfreader-0.1.8/pdfreader/filters/lzw.py
--rw-r--r--   0 maxp       (502) staff       (20)      858 2019-11-06 17:10:39.000000 pdfreader-0.1.8/pdfreader/filters/predictors.py
--rw-r--r--   0 maxp       (502) staff       (20)     1204 2019-11-08 20:47:35.000000 pdfreader-0.1.8/pdfreader/filters/runlength.py
--rw-r--r--   0 maxp       (502) staff       (20)     4524 2020-09-09 00:22:21.000000 pdfreader-0.1.8/pdfreader/filters/test_ccittf_fax.py
--rw-r--r--   0 maxp       (502) staff       (20)      414 2019-11-06 17:10:39.000000 pdfreader-0.1.8/pdfreader/filters/tests.py
-drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-01-30 03:35:39.052669 pdfreader-0.1.8/pdfreader/parsers/
--rw-r--r--   0 maxp       (502) staff       (20)      156 2019-11-25 16:57:07.000000 pdfreader-0.1.8/pdfreader/parsers/__init__.py
--rw-r--r--   0 maxp       (502) staff       (20)    21222 2020-09-09 00:22:21.000000 pdfreader-0.1.8/pdfreader/parsers/base.py
-drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-01-30 03:35:39.065374 pdfreader-0.1.8/pdfreader/parsers/cmap-samples/
--rw-r--r--   0 maxp       (502) staff       (20)      326 2020-01-02 18:43:53.000000 pdfreader-0.1.8/pdfreader/parsers/cmap-samples/cmap-empty-name.txt
--rw-r--r--   0 maxp       (502) staff       (20)     1634 2020-01-02 18:43:53.000000 pdfreader-0.1.8/pdfreader/parsers/cmap-samples/cmap-sample-2.txt
--rw-r--r--   0 maxp       (502) staff       (20)     1742 2020-01-02 18:43:53.000000 pdfreader-0.1.8/pdfreader/parsers/cmap-samples/cmap-sample-3.txt
--rw-r--r--   0 maxp       (502) staff       (20)      847 2020-01-02 18:43:53.000000 pdfreader-0.1.8/pdfreader/parsers/cmap-samples/cmap-sample-bfrange-with-list.txt
--rw-r--r--   0 maxp       (502) staff       (20)      319 2020-01-02 18:43:53.000000 pdfreader-0.1.8/pdfreader/parsers/cmap-samples/cmap-sample-missing-name.txt
--rw-r--r--   0 maxp       (502) staff       (20)     7079 2020-01-02 18:43:53.000000 pdfreader-0.1.8/pdfreader/parsers/cmap-samples/cmap-sample.txt
--rw-r--r--   0 maxp       (502) staff       (20)     9313 2020-09-09 00:22:18.000000 pdfreader-0.1.8/pdfreader/parsers/cmap.py
--rw-r--r--   0 maxp       (502) staff       (20)     2716 2019-11-25 16:57:07.000000 pdfreader-0.1.8/pdfreader/parsers/content.py
--rw-r--r--   0 maxp       (502) staff       (20)    19943 2021-01-30 03:29:29.000000 pdfreader-0.1.8/pdfreader/parsers/document.py
--rw-r--r--   0 maxp       (502) staff       (20)     2248 2020-09-09 00:22:21.000000 pdfreader-0.1.8/pdfreader/parsers/inlineimage.py
--rw-r--r--   0 maxp       (502) staff       (20)      508 2019-08-26 19:18:47.000000 pdfreader-0.1.8/pdfreader/parsers/objstm.py
--rw-r--r--   0 maxp       (502) staff       (20)      580 2019-11-25 16:57:07.000000 pdfreader-0.1.8/pdfreader/parsers/tests.py
--rw-r--r--   0 maxp       (502) staff       (20)     2944 2020-09-09 00:22:21.000000 pdfreader-0.1.8/pdfreader/pillow.py
--rw-r--r--   0 maxp       (502) staff       (20)     1697 2020-11-12 03:26:51.000000 pdfreader-0.1.8/pdfreader/registry.py
--rw-r--r--   0 maxp       (502) staff       (20)    12299 2020-11-14 00:38:48.000000 pdfreader-0.1.8/pdfreader/securityhandler.py
--rw-r--r--   0 maxp       (502) staff       (20)      326 2019-11-25 16:57:07.000000 pdfreader-0.1.8/pdfreader/tests.py
-drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-01-30 03:35:39.076698 pdfreader-0.1.8/pdfreader/types/
--rw-r--r--   0 maxp       (502) staff       (20)      280 2019-11-25 16:57:07.000000 pdfreader-0.1.8/pdfreader/types/__init__.py
--rw-r--r--   0 maxp       (502) staff       (20)    10303 2020-09-09 00:22:21.000000 pdfreader-0.1.8/pdfreader/types/cmap.py
--rw-r--r--   0 maxp       (502) staff       (20)     6056 2019-11-01 17:33:32.000000 pdfreader-0.1.8/pdfreader/types/constants.py
--rw-r--r--   0 maxp       (502) staff       (20)     2457 2019-12-19 20:20:03.000000 pdfreader-0.1.8/pdfreader/types/content.py
--rw-r--r--   0 maxp       (502) staff       (20)     1301 2020-11-14 00:38:48.000000 pdfreader-0.1.8/pdfreader/types/filestructure.py
--rw-r--r--   0 maxp       (502) staff       (20)     5222 2020-11-14 00:38:48.000000 pdfreader-0.1.8/pdfreader/types/native.py
--rw-r--r--   0 maxp       (502) staff       (20)    11424 2020-09-09 00:22:21.000000 pdfreader-0.1.8/pdfreader/types/objects.py
--rw-r--r--   0 maxp       (502) staff       (20)      340 2019-11-06 17:10:39.000000 pdfreader-0.1.8/pdfreader/types/tests.py
--rw-r--r--   0 maxp       (502) staff       (20)     5355 2020-09-09 00:22:21.000000 pdfreader-0.1.8/pdfreader/types/xref.py
--rw-r--r--   0 maxp       (502) staff       (20)      611 2020-09-09 00:22:21.000000 pdfreader-0.1.8/pdfreader/utils.py
-drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-01-30 03:35:39.082345 pdfreader-0.1.8/pdfreader/viewer/
--rw-r--r--   0 maxp       (502) staff       (20)      214 2019-11-25 21:06:14.000000 pdfreader-0.1.8/pdfreader/viewer/__init__.py
--rw-r--r--   0 maxp       (502) staff       (20)     1883 2021-01-27 00:33:49.000000 pdfreader-0.1.8/pdfreader/viewer/canvas.py
--rw-r--r--   0 maxp       (502) staff       (20)     2512 2019-12-11 19:06:26.000000 pdfreader-0.1.8/pdfreader/viewer/graphicsstate.py
--rw-r--r--   0 maxp       (502) staff       (20)     9240 2020-12-17 19:21:07.000000 pdfreader-0.1.8/pdfreader/viewer/pdfviewer.py
--rw-r--r--   0 maxp       (502) staff       (20)     2545 2020-09-11 15:35:40.000000 pdfreader-0.1.8/pdfreader/viewer/resources.py
--rw-r--r--   0 maxp       (502) staff       (20)     7979 2020-12-17 18:00:40.000000 pdfreader-0.1.8/pdfreader/viewer/simple.py
--rw-r--r--   0 maxp       (502) staff       (20)      344 2021-01-27 00:33:49.000000 pdfreader-0.1.8/pdfreader/viewer/tests.py
-drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-01-30 03:35:38.974343 pdfreader-0.1.8/pdfreader.egg-info/
--rw-r--r--   0 maxp       (502) staff       (20)     4889 2021-01-30 03:35:38.000000 pdfreader-0.1.8/pdfreader.egg-info/PKG-INFO
--rw-r--r--   0 maxp       (502) staff       (20)     3905 2021-01-30 03:35:38.000000 pdfreader-0.1.8/pdfreader.egg-info/SOURCES.txt
--rw-r--r--   0 maxp       (502) staff       (20)        1 2021-01-30 03:35:38.000000 pdfreader-0.1.8/pdfreader.egg-info/dependency_links.txt
--rw-r--r--   0 maxp       (502) staff       (20)       20 2021-01-30 03:35:38.000000 pdfreader-0.1.8/pdfreader.egg-info/entry_points.txt
--rw-r--r--   0 maxp       (502) staff       (20)        1 2019-12-20 15:58:58.000000 pdfreader-0.1.8/pdfreader.egg-info/not-zip-safe
--rw-r--r--   0 maxp       (502) staff       (20)       50 2021-01-30 03:35:38.000000 pdfreader-0.1.8/pdfreader.egg-info/requires.txt
--rw-r--r--   0 maxp       (502) staff       (20)       10 2021-01-30 03:35:38.000000 pdfreader-0.1.8/pdfreader.egg-info/top_level.txt
--rw-r--r--   0 maxp       (502) staff       (20)       49 2020-12-17 16:40:13.000000 pdfreader-0.1.8/requirements.txt
--rw-r--r--   0 maxp       (502) staff       (20)       38 2021-01-30 03:35:39.084782 pdfreader-0.1.8/setup.cfg
--rwxr-xr-x   0 maxp       (502) staff       (20)     4085 2021-01-30 03:29:48.000000 pdfreader-0.1.8/setup.py
+drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-02-22 02:39:48.958155 pdfreader-0.1.9/
+-rw-r--r--   0 maxp       (502) staff       (20)     1866 2021-02-22 02:39:15.000000 pdfreader-0.1.9/CHANGELOG.txt
+-rw-r--r--   0 maxp       (502) staff       (20)      377 2019-11-25 16:57:07.000000 pdfreader-0.1.9/CONTRIBUTING.rst
+-rw-r--r--   0 maxp       (502) staff       (20)     1071 2019-11-25 16:57:07.000000 pdfreader-0.1.9/LICENSE
+-rw-r--r--   0 maxp       (502) staff       (20)      518 2020-12-17 19:25:24.000000 pdfreader-0.1.9/MANIFEST.in
+-rw-r--r--   0 maxp       (502) staff       (20)     4889 2021-02-22 02:39:48.957569 pdfreader-0.1.9/PKG-INFO
+-rw-r--r--   0 maxp       (502) staff       (20)     3266 2020-11-14 00:38:48.000000 pdfreader-0.1.9/README.rst
+-rw-r--r--   0 maxp       (502) staff       (20)      643 2020-12-17 17:36:24.000000 pdfreader-0.1.9/SECURITY.md
+-rw-r--r--   0 maxp       (502) staff       (20)    26134 2020-12-17 16:42:07.000000 pdfreader-0.1.9/THIRD-PARTY-NOTICES
+drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-02-22 02:39:48.782726 pdfreader-0.1.9/doc/
+-rw-r--r--   0 maxp       (502) staff       (20)        1 2019-11-25 16:57:07.000000 pdfreader-0.1.9/doc/__init__.py
+drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-02-22 02:39:48.785428 pdfreader-0.1.9/doc/api/
+-rw-r--r--   0 maxp       (502) staff       (20)      366 2021-02-22 01:51:53.000000 pdfreader-0.1.9/doc/api/document.rst
+-rw-r--r--   0 maxp       (502) staff       (20)     1209 2019-11-26 19:24:18.000000 pdfreader-0.1.9/doc/api/index.rst
+-rw-r--r--   0 maxp       (502) staff       (20)     1064 2019-11-26 19:24:18.000000 pdfreader-0.1.9/doc/api/types.rst
+-rw-r--r--   0 maxp       (502) staff       (20)     2086 2021-02-22 01:51:53.000000 pdfreader-0.1.9/doc/api/viewer.rst
+-rw-r--r--   0 maxp       (502) staff       (20)     5176 2019-11-26 19:24:18.000000 pdfreader-0.1.9/doc/conf.py
+drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-02-22 02:39:48.791355 pdfreader-0.1.9/doc/examples/
+-rw-r--r--   0 maxp       (502) staff       (20)     1808 2019-12-11 19:06:26.000000 pdfreader-0.1.9/doc/examples/document_vs_viewer.rst
+drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-02-22 02:39:48.798220 pdfreader-0.1.9/doc/examples/downloads/
+-rw-r--r--   0 maxp       (502) staff       (20)    52644 2019-11-21 18:37:24.000000 pdfreader-0.1.9/doc/examples/downloads/example-crash-markdown.txt
+-rw-r--r--   0 maxp       (502) staff       (20)      229 2019-11-21 18:17:46.000000 pdfreader-0.1.9/doc/examples/downloads/sample-cmap.txt
+-rw-r--r--   0 maxp       (502) staff       (20)    19349 2019-11-21 17:20:49.000000 pdfreader-0.1.9/doc/examples/downloads/tutorial-sample-content-stream-p1.txt
+-rw-r--r--   0 maxp       (502) staff       (20)     2550 2019-12-11 19:06:26.000000 pdfreader-0.1.9/doc/examples/extract_cmap.rst
+-rw-r--r--   0 maxp       (502) staff       (20)     2216 2019-12-20 15:58:08.000000 pdfreader-0.1.9/doc/examples/extract_fonts.rst
+-rw-r--r--   0 maxp       (502) staff       (20)     2306 2019-12-20 15:58:08.000000 pdfreader-0.1.9/doc/examples/extract_form_text.rst
+-rw-r--r--   0 maxp       (502) staff       (20)     4603 2019-12-11 19:06:26.000000 pdfreader-0.1.9/doc/examples/extract_image.rst
+-rw-r--r--   0 maxp       (502) staff       (20)     4222 2019-12-11 19:06:26.000000 pdfreader-0.1.9/doc/examples/extract_page_text.rst
+drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-02-22 02:39:48.804088 pdfreader-0.1.9/doc/examples/img/
+-rw-r--r--   0 maxp       (502) staff       (20)      298 2019-11-25 16:57:07.000000 pdfreader-0.1.9/doc/examples/img/example-image-mask.png
+-rw-r--r--   0 maxp       (502) staff       (20)    13625 2019-11-25 16:57:07.000000 pdfreader-0.1.9/doc/examples/img/example-logo.png
+-rw-r--r--   0 maxp       (502) staff       (20)   190916 2019-11-25 16:57:07.000000 pdfreader-0.1.9/doc/examples/img/example-parse-form.png
+-rw-r--r--   0 maxp       (502) staff       (20)   172197 2019-11-25 16:57:07.000000 pdfreader-0.1.9/doc/examples/img/example-text-crash-report.png
+-rw-r--r--   0 maxp       (502) staff       (20)     1229 2019-12-11 19:06:26.000000 pdfreader-0.1.9/doc/examples/index.rst
+-rw-r--r--   0 maxp       (502) staff       (20)     3243 2019-12-11 19:06:26.000000 pdfreader-0.1.9/doc/examples/navigate_objects.rst
+drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-02-22 02:39:48.828232 pdfreader-0.1.9/doc/examples/pdfs/
+-rw-r--r--   0 maxp       (502) staff       (20)    18764 2020-09-11 19:48:11.000000 pdfreader-0.1.9/doc/examples/pdfs/annot-sample.pdf
+-rw-r--r--   0 maxp       (502) staff       (20)    15452 2020-11-14 00:38:48.000000 pdfreader-0.1.9/doc/examples/pdfs/encrypted-with-qwerty.pdf
+-rw-r--r--   0 maxp       (502) staff       (20)    63477 2019-11-25 16:57:07.000000 pdfreader-0.1.9/doc/examples/pdfs/example-font.pdf
+-rw-r--r--   0 maxp       (502) staff       (20)   556776 2019-11-25 16:57:07.000000 pdfreader-0.1.9/doc/examples/pdfs/example-form.pdf
+-rw-r--r--   0 maxp       (502) staff       (20)    49348 2019-11-25 16:57:07.000000 pdfreader-0.1.9/doc/examples/pdfs/example-image-xobject.pdf
+-rw-r--r--   0 maxp       (502) staff       (20)   509714 2019-11-25 16:57:07.000000 pdfreader-0.1.9/doc/examples/pdfs/example-text-crash-report.pdf
+-rw-r--r--   0 maxp       (502) staff       (20)  1106383 2019-11-25 16:57:07.000000 pdfreader-0.1.9/doc/examples/pdfs/tutorial-example.pdf
+-rw-r--r--   0 maxp       (502) staff       (20)    13625 2020-09-11 19:12:35.000000 pdfreader-0.1.9/doc/extract-logo.png
+-rw-r--r--   0 maxp       (502) staff       (20)   175641 2020-09-11 19:12:23.000000 pdfreader-0.1.9/doc/fax-from-p8.png
+-rw-r--r--   0 maxp       (502) staff       (20)     3526 2019-12-11 19:06:26.000000 pdfreader-0.1.9/doc/index.rst
+-rw-r--r--   0 maxp       (502) staff       (20)     1481 2019-12-11 19:06:26.000000 pdfreader-0.1.9/doc/installation.rst
+-rw-r--r--   0 maxp       (502) staff       (20)      298 2020-09-11 19:12:38.000000 pdfreader-0.1.9/doc/mask.png
+-rw-r--r--   0 maxp       (502) staff       (20)       74 2019-11-25 16:57:07.000000 pdfreader-0.1.9/doc/requirements.txt
+-rw-r--r--   0 maxp       (502) staff       (20)    13147 2021-02-22 01:51:53.000000 pdfreader-0.1.9/doc/tutorial.rst
+drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-02-22 02:39:48.845019 pdfreader-0.1.9/pdfreader/
+-rw-r--r--   0 maxp       (502) staff       (20)      209 2021-02-22 02:39:15.000000 pdfreader-0.1.9/pdfreader/__init__.py
+-rw-r--r--   0 maxp       (502) staff       (20)     4296 2020-02-20 21:04:21.000000 pdfreader-0.1.9/pdfreader/buffer.py
+drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-02-22 02:39:48.873838 pdfreader-0.1.9/pdfreader/codecs/
+-rw-r--r--   0 maxp       (502) staff       (20)      298 2019-11-06 17:10:39.000000 pdfreader-0.1.9/pdfreader/codecs/__init__.py
+-rw-r--r--   0 maxp       (502) staff       (20)   110596 2019-11-06 17:10:39.000000 pdfreader-0.1.9/pdfreader/codecs/agl.py
+drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-02-22 02:39:48.897229 pdfreader-0.1.9/pdfreader/codecs/cmaps/
+-rw-r--r--   0 maxp       (502) staff       (20)     3829 2019-11-11 14:22:22.000000 pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-CNS1-0
+-rw-r--r--   0 maxp       (502) staff       (20)     4122 2019-11-11 14:22:22.000000 pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-CNS1-3
+-rw-r--r--   0 maxp       (502) staff       (20)     4142 2019-11-11 14:22:22.000000 pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-CNS1-4
+-rw-r--r--   0 maxp       (502) staff       (20)     3292 2019-11-11 14:22:22.000000 pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-GB1-0
+-rw-r--r--   0 maxp       (502) staff       (20)     4400 2019-11-11 14:22:22.000000 pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-GB1-2
+-rw-r--r--   0 maxp       (502) staff       (20)     4951 2019-11-11 14:22:22.000000 pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-GB1-4
+-rw-r--r--   0 maxp       (502) staff       (20)     3342 2019-11-11 14:22:22.000000 pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-Japan1-1
+-rw-r--r--   0 maxp       (502) staff       (20)     3380 2019-11-11 14:22:22.000000 pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-Japan1-2
+-rw-r--r--   0 maxp       (502) staff       (20)     3868 2019-11-11 14:22:22.000000 pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-Japan1-4
+-rw-r--r--   0 maxp       (502) staff       (20)     4248 2019-11-11 14:22:22.000000 pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-Japan1-5
+-rw-r--r--   0 maxp       (502) staff       (20)     3433 2019-11-11 14:22:22.000000 pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-Korea1-0
+-rw-r--r--   0 maxp       (502) staff       (20)     4089 2019-11-11 14:22:22.000000 pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-Korea1-1
+-rw-r--r--   0 maxp       (502) staff       (20)     4088 2019-11-11 14:22:22.000000 pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-Korea1-2
+-rw-r--r--   0 maxp       (502) staff       (20)     7820 2019-11-11 14:22:22.000000 pdfreader-0.1.9/pdfreader/codecs/cmaps/Identity-H
+-rw-r--r--   0 maxp       (502) staff       (20)       54 2019-11-11 14:31:21.000000 pdfreader-0.1.9/pdfreader/codecs/cmaps/README.md
+-rw-r--r--   0 maxp       (502) staff       (20)     4571 2019-11-25 16:57:07.000000 pdfreader-0.1.9/pdfreader/codecs/codec.py
+-rw-r--r--   0 maxp       (502) staff       (20)     6531 2020-09-09 00:22:21.000000 pdfreader-0.1.9/pdfreader/codecs/decoder.py
+-rw-r--r--   0 maxp       (502) staff       (20)     2325 2019-11-26 16:58:10.000000 pdfreader-0.1.9/pdfreader/codecs/differences.py
+-rw-r--r--   0 maxp       (502) staff       (20)     7091 2019-12-11 19:17:56.000000 pdfreader-0.1.9/pdfreader/codecs/macroman.py
+-rw-r--r--   0 maxp       (502) staff       (20)     7852 2019-11-25 16:57:07.000000 pdfreader-0.1.9/pdfreader/codecs/pdfdoc.py
+-rw-r--r--   0 maxp       (502) staff       (20)     4853 2019-11-25 16:57:07.000000 pdfreader-0.1.9/pdfreader/codecs/standard.py
+-rw-r--r--   0 maxp       (502) staff       (20)      469 2019-11-11 18:20:02.000000 pdfreader-0.1.9/pdfreader/codecs/tests.py
+-rw-r--r--   0 maxp       (502) staff       (20)     7455 2019-12-11 19:17:49.000000 pdfreader-0.1.9/pdfreader/codecs/winansi.py
+-rw-r--r--   0 maxp       (502) staff       (20)     3614 2019-11-06 17:10:39.000000 pdfreader-0.1.9/pdfreader/codecs/zapfdingbatsgl.py
+-rw-r--r--   0 maxp       (502) staff       (20)     3818 2019-11-11 14:58:52.000000 pdfreader-0.1.9/pdfreader/constants.py
+-rw-r--r--   0 maxp       (502) staff       (20)     4949 2021-02-22 01:51:53.000000 pdfreader-0.1.9/pdfreader/document.py
+-rw-r--r--   0 maxp       (502) staff       (20)      135 2020-08-27 19:40:05.000000 pdfreader-0.1.9/pdfreader/exceptions.py
+drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-02-22 02:39:48.915947 pdfreader-0.1.9/pdfreader/filters/
+-rw-r--r--   0 maxp       (502) staff       (20)      601 2020-09-09 00:22:21.000000 pdfreader-0.1.9/pdfreader/filters/__init__.py
+-rw-r--r--   0 maxp       (502) staff       (20)      793 2019-11-08 20:47:35.000000 pdfreader-0.1.9/pdfreader/filters/ascii85.py
+-rw-r--r--   0 maxp       (502) staff       (20)     1194 2019-11-08 20:47:35.000000 pdfreader-0.1.9/pdfreader/filters/asciihex.py
+-rw-r--r--   0 maxp       (502) staff       (20)    19621 2020-12-17 17:20:54.000000 pdfreader-0.1.9/pdfreader/filters/ccittfax.py
+-rw-r--r--   0 maxp       (502) staff       (20)       94 2019-11-06 17:10:39.000000 pdfreader-0.1.9/pdfreader/filters/crypt.py
+-rw-r--r--   0 maxp       (502) staff       (20)      108 2020-01-02 19:04:17.000000 pdfreader-0.1.9/pdfreader/filters/dct.py
+-rw-r--r--   0 maxp       (502) staff       (20)      675 2019-11-06 17:10:39.000000 pdfreader-0.1.9/pdfreader/filters/flate.py
+-rw-r--r--   0 maxp       (502) staff       (20)      106 2019-11-06 17:10:39.000000 pdfreader-0.1.9/pdfreader/filters/jbig2.py
+-rw-r--r--   0 maxp       (502) staff       (20)      102 2019-11-06 17:10:39.000000 pdfreader-0.1.9/pdfreader/filters/jpx.py
+-rw-r--r--   0 maxp       (502) staff       (20)     8942 2019-11-06 17:10:39.000000 pdfreader-0.1.9/pdfreader/filters/lzw.py
+-rw-r--r--   0 maxp       (502) staff       (20)      858 2019-11-06 17:10:39.000000 pdfreader-0.1.9/pdfreader/filters/predictors.py
+-rw-r--r--   0 maxp       (502) staff       (20)     1204 2019-11-08 20:47:35.000000 pdfreader-0.1.9/pdfreader/filters/runlength.py
+-rw-r--r--   0 maxp       (502) staff       (20)     4524 2020-09-09 00:22:21.000000 pdfreader-0.1.9/pdfreader/filters/test_ccittf_fax.py
+-rw-r--r--   0 maxp       (502) staff       (20)      414 2019-11-06 17:10:39.000000 pdfreader-0.1.9/pdfreader/filters/tests.py
+drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-02-22 02:39:48.929505 pdfreader-0.1.9/pdfreader/parsers/
+-rw-r--r--   0 maxp       (502) staff       (20)      156 2019-11-25 16:57:07.000000 pdfreader-0.1.9/pdfreader/parsers/__init__.py
+-rw-r--r--   0 maxp       (502) staff       (20)    22432 2021-02-22 01:51:53.000000 pdfreader-0.1.9/pdfreader/parsers/base.py
+drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-02-22 02:39:48.935684 pdfreader-0.1.9/pdfreader/parsers/cmap-samples/
+-rw-r--r--   0 maxp       (502) staff       (20)      326 2020-01-02 18:43:53.000000 pdfreader-0.1.9/pdfreader/parsers/cmap-samples/cmap-empty-name.txt
+-rw-r--r--   0 maxp       (502) staff       (20)     1634 2020-01-02 18:43:53.000000 pdfreader-0.1.9/pdfreader/parsers/cmap-samples/cmap-sample-2.txt
+-rw-r--r--   0 maxp       (502) staff       (20)     1742 2020-01-02 18:43:53.000000 pdfreader-0.1.9/pdfreader/parsers/cmap-samples/cmap-sample-3.txt
+-rw-r--r--   0 maxp       (502) staff       (20)      847 2020-01-02 18:43:53.000000 pdfreader-0.1.9/pdfreader/parsers/cmap-samples/cmap-sample-bfrange-with-list.txt
+-rw-r--r--   0 maxp       (502) staff       (20)      319 2020-01-02 18:43:53.000000 pdfreader-0.1.9/pdfreader/parsers/cmap-samples/cmap-sample-missing-name.txt
+-rw-r--r--   0 maxp       (502) staff       (20)     7079 2020-01-02 18:43:53.000000 pdfreader-0.1.9/pdfreader/parsers/cmap-samples/cmap-sample.txt
+-rw-r--r--   0 maxp       (502) staff       (20)     9313 2020-09-09 00:22:18.000000 pdfreader-0.1.9/pdfreader/parsers/cmap.py
+-rw-r--r--   0 maxp       (502) staff       (20)     2716 2019-11-25 16:57:07.000000 pdfreader-0.1.9/pdfreader/parsers/content.py
+-rw-r--r--   0 maxp       (502) staff       (20)    19943 2021-01-30 03:29:29.000000 pdfreader-0.1.9/pdfreader/parsers/document.py
+-rw-r--r--   0 maxp       (502) staff       (20)     2248 2020-09-09 00:22:21.000000 pdfreader-0.1.9/pdfreader/parsers/inlineimage.py
+-rw-r--r--   0 maxp       (502) staff       (20)      508 2019-08-26 19:18:47.000000 pdfreader-0.1.9/pdfreader/parsers/objstm.py
+-rw-r--r--   0 maxp       (502) staff       (20)      580 2019-11-25 16:57:07.000000 pdfreader-0.1.9/pdfreader/parsers/tests.py
+-rw-r--r--   0 maxp       (502) staff       (20)     2944 2020-09-09 00:22:21.000000 pdfreader-0.1.9/pdfreader/pillow.py
+-rw-r--r--   0 maxp       (502) staff       (20)     1697 2020-11-12 03:26:51.000000 pdfreader-0.1.9/pdfreader/registry.py
+-rw-r--r--   0 maxp       (502) staff       (20)    12331 2021-02-22 02:06:55.000000 pdfreader-0.1.9/pdfreader/securityhandler.py
+-rw-r--r--   0 maxp       (502) staff       (20)      462 2021-02-22 01:51:53.000000 pdfreader-0.1.9/pdfreader/tests.py
+drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-02-22 02:39:48.943706 pdfreader-0.1.9/pdfreader/types/
+-rw-r--r--   0 maxp       (502) staff       (20)      280 2019-11-25 16:57:07.000000 pdfreader-0.1.9/pdfreader/types/__init__.py
+-rw-r--r--   0 maxp       (502) staff       (20)    10303 2020-09-09 00:22:21.000000 pdfreader-0.1.9/pdfreader/types/cmap.py
+-rw-r--r--   0 maxp       (502) staff       (20)     6056 2019-11-01 17:33:32.000000 pdfreader-0.1.9/pdfreader/types/constants.py
+-rw-r--r--   0 maxp       (502) staff       (20)     2457 2019-12-19 20:20:03.000000 pdfreader-0.1.9/pdfreader/types/content.py
+-rw-r--r--   0 maxp       (502) staff       (20)     1301 2020-11-14 00:38:48.000000 pdfreader-0.1.9/pdfreader/types/filestructure.py
+-rw-r--r--   0 maxp       (502) staff       (20)     5333 2021-02-22 01:51:53.000000 pdfreader-0.1.9/pdfreader/types/native.py
+-rw-r--r--   0 maxp       (502) staff       (20)    11424 2020-09-09 00:22:21.000000 pdfreader-0.1.9/pdfreader/types/objects.py
+-rw-r--r--   0 maxp       (502) staff       (20)      340 2019-11-06 17:10:39.000000 pdfreader-0.1.9/pdfreader/types/tests.py
+-rw-r--r--   0 maxp       (502) staff       (20)     5355 2020-09-09 00:22:21.000000 pdfreader-0.1.9/pdfreader/types/xref.py
+-rw-r--r--   0 maxp       (502) staff       (20)     1748 2021-02-22 01:51:53.000000 pdfreader-0.1.9/pdfreader/utils.py
+drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-02-22 02:39:48.956087 pdfreader-0.1.9/pdfreader/viewer/
+-rw-r--r--   0 maxp       (502) staff       (20)      214 2019-11-25 21:06:14.000000 pdfreader-0.1.9/pdfreader/viewer/__init__.py
+-rw-r--r--   0 maxp       (502) staff       (20)     1883 2021-01-27 00:33:49.000000 pdfreader-0.1.9/pdfreader/viewer/canvas.py
+-rw-r--r--   0 maxp       (502) staff       (20)     2512 2019-12-11 19:06:26.000000 pdfreader-0.1.9/pdfreader/viewer/graphicsstate.py
+-rw-r--r--   0 maxp       (502) staff       (20)     9461 2021-02-22 02:20:50.000000 pdfreader-0.1.9/pdfreader/viewer/pdfviewer.py
+-rw-r--r--   0 maxp       (502) staff       (20)     2545 2020-09-11 15:35:40.000000 pdfreader-0.1.9/pdfreader/viewer/resources.py
+-rw-r--r--   0 maxp       (502) staff       (20)     8437 2021-02-22 02:39:15.000000 pdfreader-0.1.9/pdfreader/viewer/simple.py
+-rw-r--r--   0 maxp       (502) staff       (20)      344 2021-01-27 00:33:49.000000 pdfreader-0.1.9/pdfreader/viewer/tests.py
+drwxr-xr-x   0 maxp       (502) staff       (20)        0 2021-02-22 02:39:48.859517 pdfreader-0.1.9/pdfreader.egg-info/
+-rw-r--r--   0 maxp       (502) staff       (20)     4889 2021-02-22 02:39:48.000000 pdfreader-0.1.9/pdfreader.egg-info/PKG-INFO
+-rw-r--r--   0 maxp       (502) staff       (20)     3905 2021-02-22 02:39:48.000000 pdfreader-0.1.9/pdfreader.egg-info/SOURCES.txt
+-rw-r--r--   0 maxp       (502) staff       (20)        1 2021-02-22 02:39:48.000000 pdfreader-0.1.9/pdfreader.egg-info/dependency_links.txt
+-rw-r--r--   0 maxp       (502) staff       (20)       20 2021-02-22 02:39:48.000000 pdfreader-0.1.9/pdfreader.egg-info/entry_points.txt
+-rw-r--r--   0 maxp       (502) staff       (20)        1 2019-12-20 15:58:58.000000 pdfreader-0.1.9/pdfreader.egg-info/not-zip-safe
+-rw-r--r--   0 maxp       (502) staff       (20)       73 2021-02-22 02:39:48.000000 pdfreader-0.1.9/pdfreader.egg-info/requires.txt
+-rw-r--r--   0 maxp       (502) staff       (20)       10 2021-02-22 02:39:48.000000 pdfreader-0.1.9/pdfreader.egg-info/top_level.txt
+-rw-r--r--   0 maxp       (502) staff       (20)       72 2021-02-22 01:51:53.000000 pdfreader-0.1.9/requirements.txt
+-rw-r--r--   0 maxp       (502) staff       (20)       38 2021-02-22 02:39:48.958336 pdfreader-0.1.9/setup.cfg
+-rwxr-xr-x   0 maxp       (502) staff       (20)     4111 2021-02-22 02:39:15.000000 pdfreader-0.1.9/setup.py
```

### Comparing `pdfreader-0.1.8/CHANGELOG.txt` & `pdfreader-0.1.9/CHANGELOG.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+pdfreader 0.1.9
+---------------------------
+ - Issue #67: Canvas cache for viewer
+ - Issue #71: Unsupported security handler version: 1
+ - Issue #72: Add a method to return document metadata
+ - Issue #68: Work around wrong stream `Length`
+
 pdfreader 0.1.8
 ---------------------------
  - Issue #63: SimpleCanvas.fromObject images copying issue fixed
  - Issue #64: Allow indirect stream objects have missing `endobj`.
 
 pdfreader 0.1.7
 ---------------------------
```

### Comparing `pdfreader-0.1.8/LICENSE` & `pdfreader-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/MANIFEST.in` & `pdfreader-0.1.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/PKG-INFO` & `pdfreader-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfreader
-Version: 0.1.8
+Version: 0.1.9
 Summary: Pythonic API for parsing PDF files
 Home-page: http://github.com/maxpmaxp/pdfreader
 Author: Maksym Polshcha
 Author-email: maxp@sterch.net
 Maintainer: Maksym Polshcha
 Maintainer-email: maxp@sterch.net
 License: MIT Licence
```

### Comparing `pdfreader-0.1.8/README.rst` & `pdfreader-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/SECURITY.md` & `pdfreader-0.1.9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/THIRD-PARTY-NOTICES` & `pdfreader-0.1.9/THIRD-PARTY-NOTICES`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/api/index.rst` & `pdfreader-0.1.9/doc/api/index.rst`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/api/types.rst` & `pdfreader-0.1.9/doc/api/types.rst`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/api/viewer.rst` & `pdfreader-0.1.9/doc/api/viewer.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
       .. autoattribute:: gss
         :annotation:
       .. autoattribute:: canvas
         :annotation:
       .. autoattribute:: resources
         :annotation:
 
+      .. autoproperty:: metadata
       .. automethod:: render
       .. automethod:: navigate
       .. automethod:: next
       .. automethod:: prev
       .. autoproperty:: annotations
       .. automethod:: __iter__
       .. automethod:: iter_pages
```

### Comparing `pdfreader-0.1.8/doc/conf.py` & `pdfreader-0.1.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/examples/document_vs_viewer.rst` & `pdfreader-0.1.9/doc/examples/document_vs_viewer.rst`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/examples/downloads/example-crash-markdown.txt` & `pdfreader-0.1.9/doc/examples/downloads/example-crash-markdown.txt`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/examples/downloads/tutorial-sample-content-stream-p1.txt` & `pdfreader-0.1.9/doc/examples/downloads/tutorial-sample-content-stream-p1.txt`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/examples/extract_cmap.rst` & `pdfreader-0.1.9/doc/examples/extract_cmap.rst`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/examples/extract_fonts.rst` & `pdfreader-0.1.9/doc/examples/extract_fonts.rst`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/examples/extract_form_text.rst` & `pdfreader-0.1.9/doc/examples/extract_form_text.rst`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/examples/extract_image.rst` & `pdfreader-0.1.9/doc/examples/extract_image.rst`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/examples/extract_page_text.rst` & `pdfreader-0.1.9/doc/examples/extract_page_text.rst`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/examples/img/example-logo.png` & `pdfreader-0.1.9/doc/examples/img/example-logo.png`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/examples/img/example-parse-form.png` & `pdfreader-0.1.9/doc/examples/img/example-parse-form.png`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/examples/img/example-text-crash-report.png` & `pdfreader-0.1.9/doc/examples/img/example-text-crash-report.png`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/examples/index.rst` & `pdfreader-0.1.9/doc/examples/index.rst`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/examples/navigate_objects.rst` & `pdfreader-0.1.9/doc/examples/navigate_objects.rst`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/examples/pdfs/annot-sample.pdf` & `pdfreader-0.1.9/doc/examples/pdfs/annot-sample.pdf`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/examples/pdfs/encrypted-with-qwerty.pdf` & `pdfreader-0.1.9/doc/examples/pdfs/encrypted-with-qwerty.pdf`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/examples/pdfs/example-font.pdf` & `pdfreader-0.1.9/doc/examples/pdfs/example-font.pdf`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/examples/pdfs/example-form.pdf` & `pdfreader-0.1.9/doc/examples/pdfs/example-form.pdf`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/examples/pdfs/example-image-xobject.pdf` & `pdfreader-0.1.9/doc/examples/pdfs/example-image-xobject.pdf`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/examples/pdfs/example-text-crash-report.pdf` & `pdfreader-0.1.9/doc/examples/pdfs/example-text-crash-report.pdf`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/examples/pdfs/tutorial-example.pdf` & `pdfreader-0.1.9/doc/examples/pdfs/tutorial-example.pdf`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/extract-logo.png` & `pdfreader-0.1.9/doc/extract-logo.png`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/fax-from-p8.png` & `pdfreader-0.1.9/doc/fax-from-p8.png`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/index.rst` & `pdfreader-0.1.9/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/installation.rst` & `pdfreader-0.1.9/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/doc/tutorial.rst` & `pdfreader-0.1.9/doc/tutorial.rst`

 * *Files 2% similar despite different names*

```diff
@@ -63,20 +63,23 @@
 .. doctest::
 
   >>> from io import BytesIO
   >>> with open(file_name, "rb") as f:
   ...     stream = BytesIO(f.read())
   >>> doc2 = PDFDocument(stream)
 
-Let's check the PDF version of the document
+Let's check the PDF version of the document and it's metadata
 
 .. doctest::
 
   >>> doc.header.version
   '1.6'
+  >>> doc.metadata
+  {'CreationDate': datetime.datetime(2019, 10, 29, ... 'Producer': 'SAMBox 1.1.19 (www.sejda.org)'}
+
 
 Now we can go ahead to the document catalog and walking through pages.
 
 .. _tutorial-document-catalog:
 
 How to access Document Catalog
 ------------------------------
@@ -174,14 +177,22 @@
 a page on :class:`~pdfreader.viewer.SimpleCanvas`.
 
 .. doctest::
 
   >>> fd = open(file_name, "rb")
   >>> viewer = SimplePDFViewer(fd)
 
+Document metadata is also accessible through :class:`~pdfreader.viewer.SimplePDFViewer` instance:
+
+.. doctest::
+
+  >>> viewer.metadata
+  {'CreationDate': datetime.datetime(2019, 10, 29, ... 'Producer': 'SAMBox 1.1.19 (www.sejda.org)'}
+
+
 The viewer instance gets content you see in your Adobe Acrobat Reader.
 :class:`~pdfreader.viewer.SimplePDFViewer` provides you with :class:`~pdfreader.viewer.SimpleCanvas` objects
 for every page. This object contains page content: images, forms, texts.
 
 The code below walks through all document's pages and extracts data:
 
 .. doctest::
```

### Comparing `pdfreader-0.1.8/pdfreader/buffer.py` & `pdfreader-0.1.9/pdfreader/buffer.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/agl.py` & `pdfreader-0.1.9/pdfreader/codecs/agl.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-CNS1-0` & `pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-CNS1-0`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-CNS1-3` & `pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-CNS1-3`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-CNS1-4` & `pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-CNS1-4`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-GB1-0` & `pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-GB1-0`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-GB1-2` & `pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-GB1-2`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-GB1-4` & `pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-GB1-4`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-Japan1-1` & `pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-Japan1-1`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-Japan1-2` & `pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-Japan1-2`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-Japan1-4` & `pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-Japan1-4`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-Japan1-5` & `pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-Japan1-5`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-Korea1-0` & `pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-Korea1-0`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-Korea1-1` & `pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-Korea1-1`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/cmaps/Adobe-Korea1-2` & `pdfreader-0.1.9/pdfreader/codecs/cmaps/Adobe-Korea1-2`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/cmaps/Identity-H` & `pdfreader-0.1.9/pdfreader/codecs/cmaps/Identity-H`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/codec.py` & `pdfreader-0.1.9/pdfreader/codecs/codec.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/decoder.py` & `pdfreader-0.1.9/pdfreader/codecs/decoder.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/differences.py` & `pdfreader-0.1.9/pdfreader/codecs/differences.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/macroman.py` & `pdfreader-0.1.9/pdfreader/codecs/macroman.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/pdfdoc.py` & `pdfreader-0.1.9/pdfreader/codecs/pdfdoc.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/standard.py` & `pdfreader-0.1.9/pdfreader/codecs/standard.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/winansi.py` & `pdfreader-0.1.9/pdfreader/codecs/winansi.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/codecs/zapfdingbatsgl.py` & `pdfreader-0.1.9/pdfreader/codecs/zapfdingbatsgl.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/constants.py` & `pdfreader-0.1.9/pdfreader/constants.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/document.py` & `pdfreader-0.1.9/pdfreader/document.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 from .registry import Registry
 from .parsers import RegistryPDFParser
 from .securityhandler import security_handler_factory
 from .types import IndirectObject, Stream, Array, Dictionary, IndirectReference, obj_factory
-from .utils import cached_property
+from .utils import cached_property, from_pdf_datetime
 
 
 class PDFDocument(object):
     """
     Represents PDF document structure
 
     :param fobj: file-like object: binary file descriptor, BytesIO stream etc.
@@ -119,12 +119,32 @@
         """
         Yields document pages one by one.
 
         :return:  :class:`~pdfreader.types.objects.Page` generator.
         """
         return self.root.Pages.pages()
 
+    @property
+    def metadata(self):
+        """
+        Returns document metadata from file's trailer info dict
+
+        :return: dict, if metadata exists `None` otherwise.
+        """
+        res = None
+        info = self.trailer.info
+        if info:
+            res = self.locate_object(info.num, info.gen)
+            for k, v in res.items():
+                if isinstance(v, bytes):
+                    try:
+                        res[k] = v.decode()
+                        if k in ('CreationDate', 'ModDate'):
+                            res[k] = from_pdf_datetime(res[k])
+                    except (UnicodeDecodeError, ValueError, TypeError):
+                        pass
+        return res
+
 
 if __name__ == "__main__":
     import doctest
     doctest.testmod()
-
```

### Comparing `pdfreader-0.1.8/pdfreader/filters/__init__.py` & `pdfreader-0.1.9/pdfreader/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/filters/ascii85.py` & `pdfreader-0.1.9/pdfreader/filters/ascii85.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/filters/asciihex.py` & `pdfreader-0.1.9/pdfreader/filters/asciihex.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/filters/ccittfax.py` & `pdfreader-0.1.9/pdfreader/filters/ccittfax.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/filters/flate.py` & `pdfreader-0.1.9/pdfreader/filters/flate.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/filters/lzw.py` & `pdfreader-0.1.9/pdfreader/filters/lzw.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/filters/predictors.py` & `pdfreader-0.1.9/pdfreader/filters/predictors.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/filters/runlength.py` & `pdfreader-0.1.9/pdfreader/filters/runlength.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/filters/test_ccittf_fax.py` & `pdfreader-0.1.9/pdfreader/filters/test_ccittf_fax.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/parsers/base.py` & `pdfreader-0.1.9/pdfreader/parsers/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -421,36 +421,67 @@
         >>> BasicTypesParser(s, 0)._stream(d).stream
         b'***data***'
 
         >>> s = b'stream\\n***data***\\rendstream'
         >>> BasicTypesParser(s, 0)._stream(d).stream
         b'***data***'
 
+        Work around wrong length. See https://github.com/maxpmaxp/pdfreader/issues/68
+        1. Length greater than real data length
+        >>> d = dict(Length=2)
+        >>> s = b'''stream\\n\\nendstream\\n\\n\\n\\n\\n\\n'''
+        >>> BasicTypesParser(s, 0)._stream(d).stream
+        b''
+
+        2. Length less than real data length
+        >>> d = dict(Length=1)
+        >>> s = b'''stream\\n***data***\\nendstream\\n\\n\\n\\n\\n'''
+        >>> BasicTypesParser(s, 0)._stream(d).stream
+        b'***data***'
         """
         length = d['Length']
         token = self.read(6)
         if token != b'stream':
             self.on_parser_error("stream expected")
         # `stream` keyword must be followed by CR+LF or by LF, but NOT by CR alone
         ch = self.next()
         if ch == CR:
             ch = self.next()
         if ch != LF:
-            self.on_parser_error("Wrong stream newline: [CR]LF expected")
+            logging.warning("Missing LF after `stream` token - [CR]LF expected. Trying to proceed.")
+            self.prev()
+
+        state = self.get_state()
+
         data = self.read(length)
-        # According to the spec EOL should be afterthe data and before endstream
+        # According to the spec EOL should be after the data and before endstream
         # But some files do not follow this.
         #
         # See data/leesoil-cases-2.pdf
         #
         # self.eol()
         self.maybe_spaces()
         token = self.read(9)
         if token != b'endstream':
-            self.on_parser_error("endstream expected")
+            # Work around wrong length. See https://github.com/maxpmaxp/pdfreader/issues/68
+            err_state = self.get_state()
+            logging.warning("Wrong stream length: {}. Trying to work around the issue.".format(length))
+            self.set_state(state)
+            data = self.read(9)
+            while not data.endswith(b'endstream'):
+                ch = self.next()
+                if ch is None:
+                    self.set_state(err_state)
+                    self.on_parser_error("endstream expected")
+                data += ch
+
+            data = data[:-9]
+            while data and data[-1:] in EOL:
+                data = data[:-1]
+
         return Stream(d, data)
 
     def hexstring(self):
         """
         >>> s = b'<01020a0B>'
         >>> BasicTypesParser(s, 0).hexstring()
         '01020A0B'
```

### Comparing `pdfreader-0.1.8/pdfreader/parsers/cmap-samples/cmap-sample-2.txt` & `pdfreader-0.1.9/pdfreader/parsers/cmap-samples/cmap-sample-2.txt`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/parsers/cmap-samples/cmap-sample-3.txt` & `pdfreader-0.1.9/pdfreader/parsers/cmap-samples/cmap-sample-3.txt`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/parsers/cmap-samples/cmap-sample-bfrange-with-list.txt` & `pdfreader-0.1.9/pdfreader/parsers/cmap-samples/cmap-sample-bfrange-with-list.txt`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/parsers/cmap-samples/cmap-sample.txt` & `pdfreader-0.1.9/pdfreader/parsers/cmap-samples/cmap-sample.txt`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/parsers/cmap.py` & `pdfreader-0.1.9/pdfreader/parsers/cmap.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/parsers/content.py` & `pdfreader-0.1.9/pdfreader/parsers/content.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/parsers/document.py` & `pdfreader-0.1.9/pdfreader/parsers/document.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/parsers/inlineimage.py` & `pdfreader-0.1.9/pdfreader/parsers/inlineimage.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/parsers/tests.py` & `pdfreader-0.1.9/pdfreader/parsers/tests.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/pillow.py` & `pdfreader-0.1.9/pdfreader/pillow.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/registry.py` & `pdfreader-0.1.9/pdfreader/registry.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/securityhandler.py` & `pdfreader-0.1.9/pdfreader/securityhandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,12 +321,13 @@
         return super(StandardSecurityHandlerV5, self).decrypt(obj)
 
     def decrypt_aes256(self, objid, genno, data):
         return AES.new(self.key, mode=AES.MODE_CBC, IV=data[:16]).decrypt(data[16:])
 
 
 SECURITY_HANDLERS_BY_VERSION = {
+    1: StandardSecurityHandler,
     2: StandardSecurityHandler,
     3: StandardSecurityHandler,
     4: StandardSecurityHandlerV4,
     5: StandardSecurityHandlerV5
 }
```

### Comparing `pdfreader-0.1.8/pdfreader/types/cmap.py` & `pdfreader-0.1.9/pdfreader/types/cmap.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/types/constants.py` & `pdfreader-0.1.9/pdfreader/types/constants.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/types/content.py` & `pdfreader-0.1.9/pdfreader/types/content.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/types/filestructure.py` & `pdfreader-0.1.9/pdfreader/types/filestructure.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/types/native.py` & `pdfreader-0.1.9/pdfreader/types/native.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,15 +77,16 @@
         if not isinstance(binary_stream, bytes):
             raise AssertionError
 
         if "Length" not in info_dict:
             raise KeyError("Missing stream length")
 
         if info_dict["Length"] != len(binary_stream):
-            raise ValueError("Inconsistent stream")
+            logging.warning("Inconsistent stream: defined length {}, real length {}"
+                            .format(info_dict["Length"], len(binary_stream)))
 
         self.dictionary = info_dict
         self.stream = binary_stream
 
     def __getitem__(self, item):
         return self.dictionary.__getitem__(item)
```

### Comparing `pdfreader-0.1.8/pdfreader/types/objects.py` & `pdfreader-0.1.9/pdfreader/types/objects.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/types/xref.py` & `pdfreader-0.1.9/pdfreader/types/xref.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/viewer/canvas.py` & `pdfreader-0.1.9/pdfreader/viewer/canvas.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/viewer/graphicsstate.py` & `pdfreader-0.1.9/pdfreader/viewer/graphicsstate.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/viewer/pdfviewer.py` & `pdfreader-0.1.9/pdfreader/viewer/pdfviewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,14 +216,23 @@
         """ Constructor method """
         self._pages = {}  # pages cache
         self.current_page_number = None
         self.doc = PDFDocument(fobj, password=password)
         super(PDFViewer, self).__init__(None, Resources(), self.graphics_state_stack_class())
 
     @property
+    def metadata(self):
+        """
+        Returns document metadata from file's trailer info dict
+
+        :return: dict, if metadata exists `None` otherwise.
+        """
+        return self.doc.metadata
+
+    @property
     def current_page(self):
         """ :return: Current :class:`~pdfreader.types.objects.Page` instance """
         return self._pages[self.current_page_number]
 
     def navigate(self, n):
         """
         Navigates viewer to n-th page of the document.
```

### Comparing `pdfreader-0.1.8/pdfreader/viewer/resources.py` & `pdfreader-0.1.9/pdfreader/viewer/resources.py`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/pdfreader/viewer/simple.py` & `pdfreader-0.1.9/pdfreader/viewer/simple.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,14 +185,25 @@
 
     #: Current page resources. :class:`~pdfreader.viewer.Resources` instance.
     resources = None
 
     #: Contains current page number
     current_page_number = None
 
+    def __init__(self, *args, **kwargs):
+        self._canvas_cache = {} # canvas cache
+        super(SimplePDFViewer, self).__init__(*args, **kwargs)
+
+    def render(self):
+        if self.current_page_number not in self._canvas_cache:
+            super(SimplePDFViewer, self).render()
+            self._canvas_cache[self.current_page_number] = self.canvas.copy()
+        else:
+            self.canvas = self._canvas_cache[self.current_page_number].copy()
+
     def after_navigate(self, n):
         self._decoders = {}
         self.bracket_commands_stack = []
         super(SimplePDFViewer, self).after_navigate(n)
 
     def on_Do(self, op):
         name = op.args[0]
```

### Comparing `pdfreader-0.1.8/pdfreader.egg-info/PKG-INFO` & `pdfreader-0.1.9/pdfreader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfreader
-Version: 0.1.8
+Version: 0.1.9
 Summary: Pythonic API for parsing PDF files
 Home-page: http://github.com/maxpmaxp/pdfreader
 Author: Maksym Polshcha
 Author-email: maxp@sterch.net
 Maintainer: Maksym Polshcha
 Maintainer-email: maxp@sterch.net
 License: MIT Licence
```

### Comparing `pdfreader-0.1.8/pdfreader.egg-info/SOURCES.txt` & `pdfreader-0.1.9/pdfreader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdfreader-0.1.8/setup.py` & `pdfreader-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     raise RuntimeError("Python version >= 3.4 required.")
 
 import warnings
 
 if sys.version_info[:2] < (3, 6):
     warnings.warn("Python version >= 3.6 required.")
 
-version = '0.1.8'
+version = '0.1.9'
 
 
 import os.path
 
 from setuptools import setup, find_packages
 from distutils.cmd import Command
 
@@ -135,15 +135,15 @@
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries :: Python Modules",
       ],
 
       packages=find_packages(exclude=["doc"]),
       package_data={'doc': ['doc/*']},
       zip_safe=False,
-      install_requires=['bitarray>=1.1.0', 'pillow>=7.1.0', 'pycryptodome>=3.9.9'],
+      install_requires=['bitarray>=1.1.0', 'pillow>=7.1.0', 'pycryptodome>=3.9.9', 'python-dateutil>=2.8.1'],
       entry_points={
         'console_scripts':
                 [],
       },
       cmdclass={"doc": doc,
                 "test": test}
   )
```

