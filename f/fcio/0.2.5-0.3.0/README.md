# Comparing `tmp/fcio-0.2.5.tar.gz` & `tmp/fcio-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcio-0.2.5.tar", last modified: Fri Apr 26 16:32:31 2024, max compression
+gzip compressed data, was "fcio-0.3.0.tar", last modified: Tue Apr 30 11:54:00 2024, max compression
```

## Comparing `fcio-0.2.5.tar` & `fcio-0.3.0.tar`

### file list

```diff
@@ -1,91 +1,93 @@
--rw-r--r--   0        0        0     1507 2024-04-26 16:30:08.000000 fcio-0.2.5/.github/workflows/gh-pages-static.yml
--rw-r--r--   0        0        0     1720 2024-04-26 16:30:08.000000 fcio-0.2.5/.github/workflows/main.yml
--rw-r--r--   0        0        0     3178 2024-04-26 16:30:08.000000 fcio-0.2.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0       51 2024-04-26 16:30:08.000000 fcio-0.2.5/.gitignore
--rw-r--r--   0        0        0      761 2024-04-26 16:30:08.000000 fcio-0.2.5/CHANGELOG.md
--rw-r--r--   0        0        0    16726 2024-04-26 16:30:08.000000 fcio-0.2.5/LICENSE
--rw-r--r--   0        0        0      628 2024-04-26 16:30:08.000000 fcio-0.2.5/Makefile
--rw-r--r--   0        0        0     1961 2024-04-26 16:30:08.000000 fcio-0.2.5/README.md
--rw-r--r--   0        0        0      638 2024-04-26 16:30:08.000000 fcio-0.2.5/docs/Makefile
--rw-r--r--   0        0        0      804 2024-04-26 16:30:08.000000 fcio-0.2.5/docs/make.bat
--rw-r--r--   0        0        0       29 2024-04-26 16:30:08.000000 fcio-0.2.5/docs/requirements.txt
--rw-r--r--   0        0        0     1729 2024-04-26 16:30:08.000000 fcio-0.2.5/docs/source/conf.py
--rw-r--r--   0        0        0      238 2024-04-26 16:30:08.000000 fcio-0.2.5/docs/source/fcio.rst
--rw-r--r--   0        0        0      223 2024-04-26 16:30:08.000000 fcio-0.2.5/docs/source/index.rst
--rw-r--r--   0        0        0       45 2024-04-26 16:30:08.000000 fcio-0.2.5/docs/source/readme.rst
--rw-r--r--   0        0        0     1200 2024-04-26 16:30:08.000000 fcio-0.2.5/meson.build
--rw-r--r--   0        0        0     2178 2024-04-26 16:30:08.000000 fcio-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      714 2024-04-26 16:30:08.000000 fcio-0.2.5/src/fcio/__init__.py
--rw-r--r--   0        0        0       92 2024-04-26 16:30:08.000000 fcio-0.2.5/src/fcio/cmds/__init__.py
--rw-r--r--   0        0        0     3071 2024-04-26 16:30:08.000000 fcio-0.2.5/src/fcio/cmds/cmds.py
--rw-r--r--   0        0        0     1943 2024-04-26 16:30:08.000000 fcio-0.2.5/src/fcio/cppyy_fcio/config.py
--rw-r--r--   0        0        0     8387 2024-04-26 16:30:08.000000 fcio-0.2.5/src/fcio/cppyy_fcio/event.py
--rw-r--r--   0        0        0     4344 2024-04-26 16:30:08.000000 fcio-0.2.5/src/fcio/cppyy_fcio/fcio_cppyy.py
--rw-r--r--   0        0        0     2957 2024-04-26 16:30:08.000000 fcio-0.2.5/src/fcio/cppyy_fcio/status.py
--rw-r--r--   0        0        0     4591 2024-04-26 16:30:08.000000 fcio-0.2.5/src/fcio/cy_fcio/cfcio.pxd
--rw-r--r--   0        0        0    10114 2024-04-26 16:30:08.000000 fcio-0.2.5/src/fcio/cy_fcio/cy_fcio.pyx
--rw-r--r--   0        0        0     3740 2024-04-26 16:30:08.000000 fcio-0.2.5/src/fcio/cy_fcio/cy_fcio_config.pyx
--rw-r--r--   0        0        0     5817 2024-04-26 16:30:08.000000 fcio-0.2.5/src/fcio/cy_fcio/cy_fcio_event.pyx
--rw-r--r--   0        0        0     9216 2024-04-26 16:30:08.000000 fcio-0.2.5/src/fcio/cy_fcio/cy_fcio_event_ext.pyx
--rw-r--r--   0        0        0     6415 2024-04-26 16:30:08.000000 fcio-0.2.5/src/fcio/cy_fcio/cy_fcio_status.pyx
--rw-r--r--   0        0        0     1272 2024-02-09 15:22:16.000000 fcio-0.2.5/subprojects/bufio/.drone.star
--rw-r--r--   0        0        0       50 2024-02-09 15:22:16.000000 fcio-0.2.5/subprojects/bufio/.gitignore
--rw-r--r--   0        0        0    16726 2024-02-09 15:22:16.000000 fcio-0.2.5/subprojects/bufio/LICENSE
--rw-r--r--   0        0        0      408 2024-02-09 15:22:16.000000 fcio-0.2.5/subprojects/bufio/Makefile
--rw-r--r--   0        0        0      427 2024-02-09 15:22:16.000000 fcio-0.2.5/subprojects/bufio/README.md
--rw-r--r--   0        0        0     2365 2024-02-09 15:22:16.000000 fcio-0.2.5/subprojects/bufio/examples/bufio_benchmark.c
--rw-r--r--   0        0        0      124 2024-02-09 15:22:16.000000 fcio-0.2.5/subprojects/bufio/examples/meson.build
--rw-r--r--   0        0        0      523 2024-02-09 15:22:16.000000 fcio-0.2.5/subprojects/bufio/meson.build
--rw-r--r--   0        0        0    45364 2024-02-09 15:22:16.000000 fcio-0.2.5/subprojects/bufio/src/bufio.c
--rw-r--r--   0        0        0     3273 2024-02-09 15:22:16.000000 fcio-0.2.5/subprojects/bufio/src/bufio.h
--rw-r--r--   0        0        0      161 2024-02-09 15:22:16.000000 fcio-0.2.5/subprojects/bufio/src/meson.build
--rw-r--r--   0        0        0      927 2024-02-09 15:22:16.000000 fcio-0.2.5/subprojects/bufio/tests/bufio_test_delayed_tcp_connect.c
--rw-r--r--   0        0        0     1189 2024-02-09 15:22:16.000000 fcio-0.2.5/subprojects/bufio/tests/bufio_test_follow.c
--rw-r--r--   0        0        0     1875 2024-02-09 15:22:16.000000 fcio-0.2.5/subprojects/bufio/tests/bufio_test_follow_chunk.c
--rw-r--r--   0        0        0     1902 2024-02-09 15:22:16.000000 fcio-0.2.5/subprojects/bufio/tests/bufio_test_lockedfile.c
--rw-r--r--   0        0        0      887 2024-02-09 15:22:16.000000 fcio-0.2.5/subprojects/bufio/tests/bufio_test_tcp_connect.c
--rw-r--r--   0        0        0     1331 2024-02-09 15:22:16.000000 fcio-0.2.5/subprojects/bufio/tests/bufio_test_wait_on_tcpclose.c
--rw-r--r--   0        0        0     1232 2024-02-09 15:22:16.000000 fcio-0.2.5/subprojects/bufio/tests/bufio_test_wait_on_tcpclose_with_pending_data.c
--rw-r--r--   0        0        0     1739 2024-02-09 15:22:16.000000 fcio-0.2.5/subprojects/bufio/tests/meson.build
--rw-r--r--   0        0        0      479 2024-02-09 15:22:16.000000 fcio-0.2.5/subprojects/bufio/tests/test.h
--rw-r--r--   0        0        0      110 2024-04-26 16:30:08.000000 fcio-0.2.5/subprojects/bufio.wrap
--rw-r--r--   0        0        0      965 2024-03-10 11:25:29.000000 fcio-0.2.5/subprojects/fcio/.drone.star
--rw-r--r--   0        0        0       18 2024-03-10 11:25:29.000000 fcio-0.2.5/subprojects/fcio/.gitignore
--rw-r--r--   0        0        0    16726 2024-03-10 11:25:29.000000 fcio-0.2.5/subprojects/fcio/LICENSE
--rw-r--r--   0        0        0      375 2024-03-10 11:25:29.000000 fcio-0.2.5/subprojects/fcio/Makefile
--rw-r--r--   0        0        0      715 2024-03-10 11:25:29.000000 fcio-0.2.5/subprojects/fcio/README.md
--rw-r--r--   0        0        0      549 2024-03-10 11:25:29.000000 fcio-0.2.5/subprojects/fcio/meson.build
--rw-r--r--   0        0        0    57331 2024-03-10 11:25:29.000000 fcio-0.2.5/subprojects/fcio/src/fcio.c
--rw-r--r--   0        0        0    13863 2024-03-10 11:25:29.000000 fcio-0.2.5/subprojects/fcio/src/fcio.h
--rw-r--r--   0        0        0      199 2024-03-10 11:25:29.000000 fcio-0.2.5/subprojects/fcio/src/meson.build
--rw-r--r--   0        0        0     6190 2024-03-10 11:25:29.000000 fcio-0.2.5/subprojects/fcio/src/time_utils.c
--rw-r--r--   0        0        0      778 2024-03-10 11:25:29.000000 fcio-0.2.5/subprojects/fcio/src/time_utils.h
--rw-r--r--   0        0        0      104 2024-03-10 11:25:29.000000 fcio-0.2.5/subprojects/fcio/subprojects/tmio.wrap
--rw-r--r--   0        0        0      109 2024-04-26 16:30:08.000000 fcio-0.2.5/subprojects/fcio.wrap
--rw-r--r--   0        0        0      965 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/.drone.star
--rw-r--r--   0        0        0       44 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/.gitignore
--rw-r--r--   0        0        0    16726 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/LICENSE
--rw-r--r--   0        0        0      408 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/Makefile
--rw-r--r--   0        0        0     2650 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/README.md
--rw-r--r--   0        0        0      669 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/examples/meson.build
--rw-r--r--   0        0        0     5929 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/examples/timer.c
--rw-r--r--   0        0        0      637 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/examples/timer.h
--rw-r--r--   0        0        0    10493 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/examples/tmio_benchmark.c
--rwxr-xr-x   0        0        0      572 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/examples/tmio_benchmark_disk_read.sh
--rwxr-xr-x   0        0        0      575 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/examples/tmio_benchmark_disk_write.sh
--rwxr-xr-x   0        0        0      539 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/examples/tmio_benchmark_pipe.sh
--rw-r--r--   0        0        0     2389 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/examples/tmio_benchmark_simple.c
--rwxr-xr-x   0        0        0      926 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/examples/tmio_benchmark_tcp.sh
--rw-r--r--   0        0        0     1620 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/examples/tmio_example_reader.c
--rw-r--r--   0        0        0     1822 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/examples/tmio_example_writer.c
--rw-r--r--   0        0        0     4720 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/examples/tmio_sink.c
--rw-r--r--   0        0        0      549 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/meson.build
--rw-r--r--   0        0        0      182 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/src/meson.build
--rw-r--r--   0        0        0    33908 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/src/tmio.c
--rw-r--r--   0        0        0     3723 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/src/tmio.h
--rw-r--r--   0        0        0      106 2024-03-10 11:24:50.000000 fcio-0.2.5/subprojects/tmio/subprojects/bufio.wrap
--rw-r--r--   0        0        0      108 2024-04-26 16:30:08.000000 fcio-0.2.5/subprojects/tmio.wrap
--rwxr-xr-x   0        0        0      526 2024-04-26 16:30:08.000000 fcio-0.2.5/tests/test_platform.py
--rwxr-xr-x   0        0        0      249 2024-04-26 16:30:08.000000 fcio-0.2.5/tools/create-pxd.sh
--rwxr-xr-x   0        0        0     1374 2024-04-26 16:30:08.000000 fcio-0.2.5/tools/version_util.py
--rw-r--r--   0        0        0     3381 2024-04-26 16:32:31.311552 fcio-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1507 2024-04-30 11:50:07.000000 fcio-0.3.0/.github/workflows/gh-pages-static.yml
+-rw-r--r--   0        0        0     1720 2024-04-30 11:50:07.000000 fcio-0.3.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0     3178 2024-04-30 11:50:07.000000 fcio-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       51 2024-04-30 11:50:07.000000 fcio-0.3.0/.gitignore
+-rw-r--r--   0        0        0      761 2024-04-30 11:50:07.000000 fcio-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0    16726 2024-04-30 11:50:07.000000 fcio-0.3.0/LICENSE
+-rw-r--r--   0        0        0      628 2024-04-30 11:50:07.000000 fcio-0.3.0/Makefile
+-rw-r--r--   0        0        0     1961 2024-04-30 11:50:07.000000 fcio-0.3.0/README.md
+-rw-r--r--   0        0        0      638 2024-04-30 11:50:07.000000 fcio-0.3.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2024-04-30 11:50:07.000000 fcio-0.3.0/docs/make.bat
+-rw-r--r--   0        0        0       29 2024-04-30 11:50:07.000000 fcio-0.3.0/docs/requirements.txt
+-rw-r--r--   0        0        0     1729 2024-04-30 11:50:07.000000 fcio-0.3.0/docs/source/conf.py
+-rw-r--r--   0        0        0      238 2024-04-30 11:50:07.000000 fcio-0.3.0/docs/source/fcio.rst
+-rw-r--r--   0        0        0      223 2024-04-30 11:50:07.000000 fcio-0.3.0/docs/source/index.rst
+-rw-r--r--   0        0        0       45 2024-04-30 11:50:07.000000 fcio-0.3.0/docs/source/readme.rst
+-rw-r--r--   0        0        0     1200 2024-04-30 11:50:07.000000 fcio-0.3.0/meson.build
+-rw-r--r--   0        0        0     2178 2024-04-30 11:50:07.000000 fcio-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      714 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cmds/__init__.py
+-rw-r--r--   0        0        0     3071 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cmds/cmds.py
+-rw-r--r--   0        0        0     1943 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cppyy_fcio/config.py
+-rw-r--r--   0        0        0     8387 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cppyy_fcio/event.py
+-rw-r--r--   0        0        0     4344 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cppyy_fcio/fcio_cppyy.py
+-rw-r--r--   0        0        0     2957 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cppyy_fcio/status.py
+-rw-r--r--   0        0        0     4591 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cy_fcio/cfcio.pxd
+-rw-r--r--   0        0        0    10767 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cy_fcio/cy_fcio.pyx
+-rw-r--r--   0        0        0     3742 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_config.pyx
+-rw-r--r--   0        0        0     5827 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_event.pyx
+-rw-r--r--   0        0        0     9108 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_event_ext.pyx
+-rw-r--r--   0        0        0     4896 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_recevent.pyx
+-rw-r--r--   0        0        0     6334 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_recevent_ext.pyx
+-rw-r--r--   0        0        0     6425 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_status.pyx
+-rw-r--r--   0        0        0     1272 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/.drone.star
+-rw-r--r--   0        0        0       50 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/.gitignore
+-rw-r--r--   0        0        0    16726 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/LICENSE
+-rw-r--r--   0        0        0      408 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/Makefile
+-rw-r--r--   0        0        0      427 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/README.md
+-rw-r--r--   0        0        0     2365 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/examples/bufio_benchmark.c
+-rw-r--r--   0        0        0      124 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/examples/meson.build
+-rw-r--r--   0        0        0      523 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/meson.build
+-rw-r--r--   0        0        0    45364 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/src/bufio.c
+-rw-r--r--   0        0        0     3273 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/src/bufio.h
+-rw-r--r--   0        0        0      161 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/src/meson.build
+-rw-r--r--   0        0        0      927 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/tests/bufio_test_delayed_tcp_connect.c
+-rw-r--r--   0        0        0     1189 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/tests/bufio_test_follow.c
+-rw-r--r--   0        0        0     1875 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/tests/bufio_test_follow_chunk.c
+-rw-r--r--   0        0        0     1902 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/tests/bufio_test_lockedfile.c
+-rw-r--r--   0        0        0      887 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/tests/bufio_test_tcp_connect.c
+-rw-r--r--   0        0        0     1331 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/tests/bufio_test_wait_on_tcpclose.c
+-rw-r--r--   0        0        0     1232 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/tests/bufio_test_wait_on_tcpclose_with_pending_data.c
+-rw-r--r--   0        0        0     1739 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/tests/meson.build
+-rw-r--r--   0        0        0      479 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/tests/test.h
+-rw-r--r--   0        0        0      110 2024-04-30 11:50:07.000000 fcio-0.3.0/subprojects/bufio.wrap
+-rw-r--r--   0        0        0      965 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/.drone.star
+-rw-r--r--   0        0        0       18 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/.gitignore
+-rw-r--r--   0        0        0    16726 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/LICENSE
+-rw-r--r--   0        0        0      375 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/Makefile
+-rw-r--r--   0        0        0      715 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/README.md
+-rw-r--r--   0        0        0      549 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/meson.build
+-rw-r--r--   0        0        0    57331 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/src/fcio.c
+-rw-r--r--   0        0        0    13863 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/src/fcio.h
+-rw-r--r--   0        0        0      199 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/src/meson.build
+-rw-r--r--   0        0        0     6190 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/src/time_utils.c
+-rw-r--r--   0        0        0      778 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/src/time_utils.h
+-rw-r--r--   0        0        0      104 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/subprojects/tmio.wrap
+-rw-r--r--   0        0        0      109 2024-04-30 11:50:07.000000 fcio-0.3.0/subprojects/fcio.wrap
+-rw-r--r--   0        0        0      965 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/.drone.star
+-rw-r--r--   0        0        0       44 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/.gitignore
+-rw-r--r--   0        0        0    16726 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/LICENSE
+-rw-r--r--   0        0        0      408 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/Makefile
+-rw-r--r--   0        0        0     2650 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/README.md
+-rw-r--r--   0        0        0      669 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/meson.build
+-rw-r--r--   0        0        0     5929 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/timer.c
+-rw-r--r--   0        0        0      637 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/timer.h
+-rw-r--r--   0        0        0    10493 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark.c
+-rwxr-xr-x   0        0        0      572 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark_disk_read.sh
+-rwxr-xr-x   0        0        0      575 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark_disk_write.sh
+-rwxr-xr-x   0        0        0      539 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark_pipe.sh
+-rw-r--r--   0        0        0     2389 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark_simple.c
+-rwxr-xr-x   0        0        0      926 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark_tcp.sh
+-rw-r--r--   0        0        0     1620 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/tmio_example_reader.c
+-rw-r--r--   0        0        0     1822 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/tmio_example_writer.c
+-rw-r--r--   0        0        0     4720 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/tmio_sink.c
+-rw-r--r--   0        0        0      549 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/meson.build
+-rw-r--r--   0        0        0      182 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/src/meson.build
+-rw-r--r--   0        0        0    33908 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/src/tmio.c
+-rw-r--r--   0        0        0     3723 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/src/tmio.h
+-rw-r--r--   0        0        0      106 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/subprojects/bufio.wrap
+-rw-r--r--   0        0        0      108 2024-04-30 11:50:07.000000 fcio-0.3.0/subprojects/tmio.wrap
+-rwxr-xr-x   0        0        0      526 2024-04-30 11:50:07.000000 fcio-0.3.0/tests/test_platform.py
+-rwxr-xr-x   0        0        0      249 2024-04-30 11:50:07.000000 fcio-0.3.0/tools/create-pxd.sh
+-rwxr-xr-x   0        0        0     1374 2024-04-30 11:50:07.000000 fcio-0.3.0/tools/version_util.py
+-rw-r--r--   0        0        0     3381 2024-04-30 11:54:00.447475 fcio-0.3.0/PKG-INFO
```

### Comparing `fcio-0.2.5/.github/workflows/gh-pages-static.yml` & `fcio-0.3.0/.github/workflows/gh-pages-static.yml`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/.github/workflows/main.yml` & `fcio-0.3.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/.github/workflows/publish.yml` & `fcio-0.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/CHANGELOG.md` & `fcio-0.3.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/LICENSE` & `fcio-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/Makefile` & `fcio-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/README.md` & `fcio-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/docs/Makefile` & `fcio-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/docs/make.bat` & `fcio-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/docs/source/conf.py` & `fcio-0.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/meson.build` & `fcio-0.3.0/meson.build`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/pyproject.toml` & `fcio-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/src/fcio/__init__.py` & `fcio-0.3.0/src/fcio/__init__.py`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/src/fcio/cmds/cmds.py` & `fcio-0.3.0/src/fcio/cmds/cmds.py`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/src/fcio/cppyy_fcio/config.py` & `fcio-0.3.0/src/fcio/cppyy_fcio/config.py`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/src/fcio/cppyy_fcio/event.py` & `fcio-0.3.0/src/fcio/cppyy_fcio/event.py`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/src/fcio/cppyy_fcio/fcio_cppyy.py` & `fcio-0.3.0/src/fcio/cppyy_fcio/fcio_cppyy.py`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/src/fcio/cppyy_fcio/status.py` & `fcio-0.3.0/src/fcio/cppyy_fcio/status.py`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/src/fcio/cy_fcio/cfcio.pxd` & `fcio-0.3.0/src/fcio/cy_fcio/cfcio.pxd`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/src/fcio/cy_fcio/cy_fcio.pyx` & `fcio-0.3.0/src/fcio/cy_fcio/cy_fcio.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from cfcio cimport FCIOOpen, FCIOClose, FCIODebug, FCIOGetRecord, FCIOTimeout, FCIOData, FCIOTag
 from cfcio cimport FCIOMaxChannels,FCIOMaxSamples,FCIOMaxPulses,FCIOTraceBufferLength
 cimport numpy
 import tempfile, os, subprocess
 
 include "cy_fcio_config.pyx"
 include "cy_fcio_event.pyx"
+include "cy_fcio_recevent.pyx"
 include "cy_fcio_status.pyx"
 include "cy_fcio_event_ext.pyx"
+include "cy_fcio_recevent_ext.pyx"
 
 class CyFCIOTag:
   """
   A wrapper class for the fcio tag enum.
   Provides supported tags as attributes.
   """
   Config = FCIOTag.FCIOConfig
@@ -87,18 +89,19 @@
 
   cdef object _compression # compression type, <str>
   cdef object _filename    # path to data file, <str>
   cdef object _compression_process # handle for the subprocess
   
   cdef CyConfig config
   cdef CyEvent event
+  cdef CyRecEvent recevent
   cdef CyStatus status
   cdef bint _extended
 
-  def __cinit__(self, filename : str = None, timeout : int = 0, buffersize : int = 0, debug : int = 0, compression : str = 'auto', extended : bool = True):
+  def __cinit__(self, filename : str = None, timeout : int = 0, buffersize : int = 0, debug : int = 0, compression : str = 'auto', extended : bool = False):
     self._fcio_data = NULL
     self._buffersize = buffersize
     self._timeout = timeout
     self._debug = debug
     self._compression = compression
 
     self._extended = extended
@@ -243,18 +246,22 @@
 
       if self._tag == FCIOTag.FCIOConfig:
         # config must always be allocated first.
         self.config = CyConfig(self)
         self.status = CyStatus(self)
         if self._extended:
           self.event = CyEventExt(self)
+          self.recevent = CyRecEventExt(self)
         else:
           self.event = CyEvent(self)
+          self.recevent = CyRecEvent(self)
       elif self._extended and (self._tag == FCIOTag.FCIOEvent or self._tag == FCIOTag.FCIOSparseEvent):
         self.event.update()
+      elif self._extended and self._tag == FCIOTag.FCIORecEvent:
+        self.recevent.update()
       elif self._tag <= 0:
         return False
 
       return True
     else:
       raise IOError(f"File {self._filename} not opened.")
 
@@ -264,29 +271,36 @@
       returns the current tag
     """
     return self._tag
   
   @property
   def config(self):
     """
-      returns the current FCIOStates record
+      returns the current FCIOConfig record
     """
     return self.config
 
   @property
   def event(self):
     """
-      returns the current FCIOStates record
+      returns the current FCIOEvent record
     """
     return self.event
 
   @property
+  def recevent(self):
+    """
+      returns the current FCIORecEvent record
+    """
+    return self.recevent
+
+  @property
   def status(self):
     """
-      returns the current FCIOStates record
+      returns the current FCIOStatus record
     """
     return self.status
 
   @property
   def tags(self):
     """
       Iterate through all FCIO records in the datastream.
@@ -315,14 +329,25 @@
       Returns the current event.
     """
     while self.get_record():
       if self._tag == FCIOTag.FCIOEvent or self._tag == FCIOTag.FCIOSparseEvent:
         yield self.event
 
   @property
+  def recevents(self):
+    """
+      Iterate through all FCIORecEvent records in the datastream.
+
+      Returns the current event.
+    """
+    while self.get_record():
+      if self._tag == FCIOTag.FCIORecEvent:
+        yield self.recevent
+
+  @property
   def statuses(self):
     """
       Iterate through all FCIOStatus records in the datastream.
 
       Returns the current event.
     """
     while self.get_record():
```

### Comparing `fcio-0.2.5/src/fcio/cy_fcio/cy_fcio_config.pyx` & `fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_config.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   cdef int ntraces
 
   def __cinit__(self, fcio : CyFCIO):
     self.config = &fcio._fcio_data.config
 
     self.ntraces = self.config.adcs + self.config.triggers
 
-    cdef unsigned int[:] tracemap_view = self.config.tracemap
+    cdef unsigned int[::1] tracemap_view = self.config.tracemap
     self._tracemap = numpy.ndarray(shape=(self.ntraces,), dtype=numpy.uint32, offset=0, buffer=tracemap_view)
 
   @property
   def telid(self):
     """
     The trace event list id.
     """
```

### Comparing `fcio-0.2.5/src/fcio/cy_fcio/cy_fcio_event.pyx` & `fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_event.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     self.config_ptr = &fcio._fcio_data.config
 
     # helper variables
     self.tracesamples = self.config_ptr.eventsamples + 2
     self.maxtraces = self.config_ptr.adcs + self.config_ptr.triggers
 
     # underlying buffer for trace and header information
-    cdef unsigned short [:] traces_memview = fcio._fcio_data.event.traces
+    cdef unsigned short [::1] traces_memview = fcio._fcio_data.event.traces
 
     shape = (self.maxtraces, self.config_ptr.eventsamples)
     self._np_trace = numpy.ndarray(shape=shape, dtype=numpy.uint16, offset=4, buffer=traces_memview)
     strides = ( (self.tracesamples)*self._np_trace.itemsize, self._np_trace.itemsize)
     self._np_trace = numpy.lib.stride_tricks.as_strided(self._np_trace, shape=shape, strides=strides, writeable=False)
 
     shape = (self.maxtraces, 2)
@@ -52,18 +52,18 @@
     self._np_theader = numpy.lib.stride_tricks.as_strided(self._np_theader, shape=shape, strides=strides, writeable=False)
 
     shape = (self.maxtraces, self.tracesamples)
     self._np_traces = numpy.ndarray(shape=shape, dtype=numpy.uint16, offset=0, buffer=traces_memview)
     strides = ( (self.tracesamples)*self._np_traces.itemsize, self._np_traces.itemsize)
     self._np_traces = numpy.lib.stride_tricks.as_strided(self._np_traces, shape=shape, strides=strides, writeable=False)
     
-    cdef int[:] timestamp_memview = fcio._fcio_data.event.timestamp
-    cdef int[:] timeoffset_memview = fcio._fcio_data.event.timeoffset
-    cdef int[:] deadregion_memview = fcio._fcio_data.event.deadregion
-    cdef unsigned short[:] trace_list_memview = fcio._fcio_data.event.trace_list
+    cdef int[::1] timestamp_memview = fcio._fcio_data.event.timestamp
+    cdef int[::1] timeoffset_memview = fcio._fcio_data.event.timeoffset
+    cdef int[::1] deadregion_memview = fcio._fcio_data.event.deadregion
+    cdef unsigned short[::1] trace_list_memview = fcio._fcio_data.event.trace_list
 
     self._np_timestamp = numpy.ndarray(shape=(10,), dtype=numpy.int32, offset=0, buffer=timestamp_memview)
     self._np_timeoffset = numpy.ndarray(shape=(10,), dtype=numpy.int32, offset=0, buffer=timeoffset_memview)
     self._np_deadregion = numpy.ndarray(shape=(10,), dtype=numpy.int32, offset=0, buffer=deadregion_memview)
     self._np_trace_list = numpy.ndarray(shape=(FCIOMaxChannels,), dtype=numpy.uint16, offset=0, buffer=trace_list_memview)
 
   cdef update(self):
```

### Comparing `fcio-0.2.5/src/fcio/cy_fcio/cy_fcio_event_ext.pyx` & `fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_event_ext.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -13,46 +13,37 @@
   All fields are exposes as numpy scalars or arrays with their corresponsing datatype and size.
 
   Additionally CyEventExt offers some extension to the basic CyEvent attributes. These represent either
   convenient names values in some field, or offer some required pre-calculation.
 
   All CyEvent attributes are still available.
   """
+  cdef numpy.int32_t _wait_for_first_event
 
+  cdef numpy.ndarray _tracemap
   cdef numpy.ndarray _card_addresses
   cdef numpy.ndarray _card_channels
-
   
   cdef numpy.int64_t _utc_unix_ns
   cdef numpy.float64_t _utc_unix
   
   cdef numpy.int64_t _run_time_ns
   cdef numpy.float64_t _run_time
 
-  cdef numpy.int32_t _wait_for_first_event
+  cdef numpy.int32_t _allowed_gps_error_ns
   
   cdef numpy.int64_t _start_time_ns
-
-  # cdef numpy.int64_t _dead_time_ns
-  # cdef numpy.int64_t _total_dead_time_ns
-
   cdef numpy.ndarray _dead_time_ns
   cdef numpy.ndarray _total_dead_time_ns
-
-  cdef numpy.int32_t _allowed_gps_error_ns
-
   cdef int _current_dead_time_end_pps
   cdef int _current_dead_time_end_ticks
 
-  cdef numpy.ndarray _tracemap
-
-  # def __cinit__(self):
   def __cinit__(self, fcio : CyFCIO):
 
-    cdef unsigned int[:] tracemap_view = self.config_ptr.tracemap
+    cdef unsigned int[::1] tracemap_view = self.config_ptr.tracemap
     self._tracemap = numpy.ndarray(shape=(self.maxtraces,), dtype=numpy.uint32, offset=0, buffer=tracemap_view)
 
     self._card_addresses = self._tracemap >> 16 # upper 16bit
     self._card_channels = self._tracemap % (1 << 16) # lower 16bit
 
     self._dead_time_ns = numpy.zeros(shape=(self.config_ptr.adcs,),dtype=numpy.int64)
     self._total_dead_time_ns = numpy.zeros(shape=(self.config_ptr.adcs,),dtype=numpy.int64)
@@ -65,20 +56,20 @@
     cdef numpy.int64_t _event_deadtime
 
     if self._wait_for_first_event:
       self._start_time_ns = self.event_ptr.deadregion[2] * 1000000000L + self.event_ptr.deadregion[3] * 4
       self._wait_for_first_event = False
     else:
       # determine if we have a new dead region end and update the counters
-      if self._current_dead_time_end_pps != self.event_ptr.deadregion[2] or self._current_dead_time_end_ticks != self.event_ptr.deadregion[3]:
+      if self._current_dead_time_end_pps == self.event_ptr.deadregion[2] and self._current_dead_time_end_ticks == self.event_ptr.deadregion[3]:
+        self._dead_time_ns[:] = 0
+      else:
         _event_deadtime = (self.event_ptr.deadregion[2]-self.event_ptr.deadregion[0]) * 1000000000L + (self.event_ptr.deadregion[3]-self.event_ptr.deadregion[1]) * 4
         self._dead_time_ns[self.event_ptr.deadregion[5] : self.event_ptr.deadregion[5] + self.event_ptr.deadregion[6]] = _event_deadtime
         self._total_dead_time_ns[self.event_ptr.deadregion[5] : self.event_ptr.deadregion[5] + self.event_ptr.deadregion[6]] += _event_deadtime
-      else:
-        self._dead_time_ns[:] = 0
     
     cdef expected_max_ticks = 249999999
     
     cdef numpy.int64_t _current_clock_offset
 
     _current_clock_offset = abs(self.timestamp[3] - expected_max_ticks) * 4
```

### Comparing `fcio-0.2.5/src/fcio/cy_fcio/cy_fcio_status.pyx` & `fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_status.pyx`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
   def __cinit__(self, cy_status : CyStatus, index):
 
     self.status = cy_status.status
     self.card_status = &cy_status.status.data[index]
     self.index = index
 
-    cdef unsigned int[:] linkstates_view = self.card_status.linkstates
-    cdef unsigned int[:] ctilinks_view = self.card_status.ctilinks
-    cdef unsigned int[:] othererrors_view = self.card_status.othererrors
-    cdef int[:] environment_view = self.card_status.environment
+    cdef unsigned int[::1] linkstates_view = self.card_status.linkstates
+    cdef unsigned int[::1] ctilinks_view = self.card_status.ctilinks
+    cdef unsigned int[::1] othererrors_view = self.card_status.othererrors
+    cdef int[::1] environment_view = self.card_status.environment
 
     self._linkstates = numpy.ndarray(shape=(256), dtype=numpy.uint32, offset=0, buffer=linkstates_view)
     self._ctilinks = numpy.ndarray(shape=(4), dtype=numpy.uint32, offset=0, buffer=ctilinks_view)
     self._environment = numpy.ndarray(shape=(16), dtype=numpy.int32, offset=0, buffer=environment_view)
     self._othererrors = numpy.ndarray(shape=(5), dtype=numpy.uint32, offset=0, buffer=othererrors_view)
 
   @property
@@ -182,15 +182,15 @@
   def __cinit__(self, fcio : CyFCIO):
     self.status = &fcio._fcio_data.status
     self.config = &fcio._fcio_data.config
     self.num_cards = self.config.mastercards + self.config.triggercards + self.config.adccards
 
     self._data = numpy.array([CyCardStatus(self, index) for index in range(self.num_cards)], dtype=object)
 
-    cdef int[:] statustime_view = self.status.statustime
+    cdef int[::1] statustime_view = self.status.statustime
     self._statustime = numpy.ndarray(shape=(10,), dtype=numpy.int32, offset=0, buffer=statustime_view)
 
   @property
   def status(self):
     """
     Overall status flag of the system.
     1 : no errors
```

### Comparing `fcio-0.2.5/subprojects/bufio/.drone.star` & `fcio-0.3.0/subprojects/bufio/.drone.star`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/bufio/LICENSE` & `fcio-0.3.0/subprojects/bufio/LICENSE`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/bufio/examples/bufio_benchmark.c` & `fcio-0.3.0/subprojects/bufio/examples/bufio_benchmark.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/bufio/meson.build` & `fcio-0.3.0/subprojects/bufio/meson.build`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/bufio/src/bufio.c` & `fcio-0.3.0/subprojects/bufio/src/bufio.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/bufio/src/bufio.h` & `fcio-0.3.0/subprojects/bufio/src/bufio.h`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/bufio/tests/bufio_test_delayed_tcp_connect.c` & `fcio-0.3.0/subprojects/bufio/tests/bufio_test_delayed_tcp_connect.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/bufio/tests/bufio_test_follow.c` & `fcio-0.3.0/subprojects/bufio/tests/bufio_test_follow.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/bufio/tests/bufio_test_follow_chunk.c` & `fcio-0.3.0/subprojects/bufio/tests/bufio_test_follow_chunk.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/bufio/tests/bufio_test_lockedfile.c` & `fcio-0.3.0/subprojects/bufio/tests/bufio_test_lockedfile.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/bufio/tests/bufio_test_tcp_connect.c` & `fcio-0.3.0/subprojects/bufio/tests/bufio_test_tcp_connect.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/bufio/tests/bufio_test_wait_on_tcpclose.c` & `fcio-0.3.0/subprojects/bufio/tests/bufio_test_wait_on_tcpclose.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/bufio/tests/bufio_test_wait_on_tcpclose_with_pending_data.c` & `fcio-0.3.0/subprojects/bufio/tests/bufio_test_wait_on_tcpclose_with_pending_data.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/bufio/tests/meson.build` & `fcio-0.3.0/subprojects/bufio/tests/meson.build`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/fcio/.drone.star` & `fcio-0.3.0/subprojects/fcio/.drone.star`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/fcio/LICENSE` & `fcio-0.3.0/subprojects/fcio/LICENSE`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/fcio/README.md` & `fcio-0.3.0/subprojects/fcio/README.md`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/fcio/meson.build` & `fcio-0.3.0/subprojects/fcio/meson.build`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/fcio/src/fcio.c` & `fcio-0.3.0/subprojects/fcio/src/fcio.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/fcio/src/fcio.h` & `fcio-0.3.0/subprojects/fcio/src/fcio.h`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/fcio/src/time_utils.c` & `fcio-0.3.0/subprojects/fcio/src/time_utils.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/fcio/src/time_utils.h` & `fcio-0.3.0/subprojects/fcio/src/time_utils.h`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/tmio/.drone.star` & `fcio-0.3.0/subprojects/tmio/.drone.star`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/tmio/LICENSE` & `fcio-0.3.0/subprojects/tmio/LICENSE`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/tmio/README.md` & `fcio-0.3.0/subprojects/tmio/README.md`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/tmio/examples/meson.build` & `fcio-0.3.0/subprojects/tmio/examples/meson.build`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/tmio/examples/timer.c` & `fcio-0.3.0/subprojects/tmio/examples/timer.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/tmio/examples/timer.h` & `fcio-0.3.0/subprojects/tmio/examples/timer.h`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/tmio/examples/tmio_benchmark.c` & `fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/tmio/examples/tmio_benchmark_disk_read.sh` & `fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark_disk_read.sh`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/tmio/examples/tmio_benchmark_disk_write.sh` & `fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark_disk_write.sh`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/tmio/examples/tmio_benchmark_pipe.sh` & `fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark_pipe.sh`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/tmio/examples/tmio_benchmark_simple.c` & `fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark_simple.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/tmio/examples/tmio_benchmark_tcp.sh` & `fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark_tcp.sh`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/tmio/examples/tmio_example_reader.c` & `fcio-0.3.0/subprojects/tmio/examples/tmio_example_reader.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/tmio/examples/tmio_example_writer.c` & `fcio-0.3.0/subprojects/tmio/examples/tmio_example_writer.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/tmio/examples/tmio_sink.c` & `fcio-0.3.0/subprojects/tmio/examples/tmio_sink.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/tmio/meson.build` & `fcio-0.3.0/subprojects/tmio/meson.build`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/tmio/src/tmio.c` & `fcio-0.3.0/subprojects/tmio/src/tmio.c`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/subprojects/tmio/src/tmio.h` & `fcio-0.3.0/subprojects/tmio/src/tmio.h`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/tests/test_platform.py` & `fcio-0.3.0/tests/test_platform.py`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/tools/version_util.py` & `fcio-0.3.0/tools/version_util.py`

 * *Files identical despite different names*

### Comparing `fcio-0.2.5/PKG-INFO` & `fcio-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fcio
-Version: 0.2.5
+Version: 0.3.0
 Summary: FlashCam File Format (FCIO) reader for python.
 Author-Email: Simon Sailer <simon.sailer@mpi-hd.mpg.de>
 License: MPL-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

