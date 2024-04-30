# Comparing `tmp/tdda-2.0.9.tar.gz` & `tmp/tdda-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdda-2.0.9.tar", last modified: Fri Feb 10 19:50:14 2023, max compression
+gzip compressed data, was "tdda-2.1.2.tar", last modified: Tue Apr 30 16:28:19 2024, max compression
```

## Comparing `tdda-2.0.9.tar` & `tdda-2.1.2.tar`

### file list

```diff
@@ -1,220 +1,237 @@
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.430385 tdda-2.0.9/
--rw-r--r--   0 njr        (501) staff       (20)     1100 2022-04-01 21:00:40.000000 tdda-2.0.9/LICENSE.txt
--rw-r--r--   0 njr        (501) staff       (20)       38 2022-04-01 21:00:40.000000 tdda-2.0.9/MANIFEST.in
--rw-r--r--   0 njr        (501) staff       (20)     4504 2023-02-10 19:50:14.430451 tdda-2.0.9/PKG-INFO
--rw-r--r--   0 njr        (501) staff       (20)     4166 2022-04-01 21:00:40.000000 tdda-2.0.9/README.md
--rw-r--r--   0 njr        (501) staff       (20)      140 2023-02-10 16:41:34.000000 tdda-2.0.9/pyproject.toml
--rw-r--r--   0 njr        (501) staff       (20)      200 2023-02-10 19:50:14.430665 tdda-2.0.9/setup.cfg
--rw-r--r--   0 njr        (501) staff       (20)     2309 2023-02-10 16:47:58.000000 tdda-2.0.9/setup.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.398115 tdda-2.0.9/tdda/
--rw-r--r--   0 njr        (501) staff       (20)    21066 2023-02-10 19:49:27.000000 tdda-2.0.9/tdda/CHANGES.py
--rw-r--r--   0 njr        (501) staff       (20)      987 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/__init__.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.401316 tdda-2.0.9/tdda/constraints/
--rw-r--r--   0 njr        (501) staff       (20)      455 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/__init__.py
--rw-r--r--   0 njr        (501) staff       (20)    36493 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/base.py
--rw-r--r--   0 njr        (501) staff       (20)    24998 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/baseconstraints.py
--rw-r--r--   0 njr        (501) staff       (20)     8001 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/console.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.402441 tdda-2.0.9/tdda/constraints/db/
--rw-r--r--   0 njr        (501) staff       (20)        0 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/db/__init__.py
--rw-r--r--   0 njr        (501) staff       (20)    17342 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/db/constraints.py
--rw-r--r--   0 njr        (501) staff       (20)     2754 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/db/detect.py
--rw-r--r--   0 njr        (501) staff       (20)     2934 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/db/discover.py
--rw-r--r--   0 njr        (501) staff       (20)    30601 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/db/drivers.py
--rw-r--r--   0 njr        (501) staff       (20)     1444 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/db/extension.py
--rw-r--r--   0 njr        (501) staff       (20)    13836 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/db/testdbconstraints.py
--rw-r--r--   0 njr        (501) staff       (20)     2491 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/db/verify.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.405521 tdda-2.0.9/tdda/constraints/examples/
--rw-r--r--   0 njr        (501) staff       (20)     7336 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/README.md
--rw-r--r--   0 njr        (501) staff       (20)     4700 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/accounts25k.tdda
--rw-r--r--   0 njr        (501) staff       (20)      326 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/accounts_detect_25k_against_1k.py
--rw-r--r--   0 njr        (501) staff       (20)      327 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/accounts_discover_1k.py
--rw-r--r--   0 njr        (501) staff       (20)      223 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/accounts_verify_1k.py
--rw-r--r--   0 njr        (501) staff       (20)      226 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/accounts_verify_25k.py
--rw-r--r--   0 njr        (501) staff       (20)      236 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/accounts_verify_25k_against_1k.py
--rw-r--r--   0 njr        (501) staff       (20)      398 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/accounts_verify_25k_against_1k_feather.py
--rw-r--r--   0 njr        (501) staff       (20)      264 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/accounts_verify_25k_to_frame.py
--rw-r--r--   0 njr        (501) staff       (20)     2800 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/elements118.tdda
--rw-r--r--   0 njr        (501) staff       (20)      326 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/elements_detect_118_against_92.py
--rw-r--r--   0 njr        (501) staff       (20)      327 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/elements_discover_92.py
--rw-r--r--   0 njr        (501) staff       (20)      226 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/elements_verify_118.py
--rw-r--r--   0 njr        (501) staff       (20)      236 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/elements_verify_118_against_92.py
--rw-r--r--   0 njr        (501) staff       (20)      398 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/elements_verify_118_against_92_feather.py
--rw-r--r--   0 njr        (501) staff       (20)      223 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/elements_verify_92.py
--rw-r--r--   0 njr        (501) staff       (20)    13795 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/files_extension.py
--rw-r--r--   0 njr        (501) staff       (20)     1078 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/simple_discovery.py
--rw-r--r--   0 njr        (501) staff       (20)     2176 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/simple_verification.py
--rw-r--r--   0 njr        (501) staff       (20)      373 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/simple_verify_fail.py
--rw-r--r--   0 njr        (501) staff       (20)      316 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/simple_verify_pass.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.408809 tdda-2.0.9/tdda/constraints/examples/testdata/
--rw-r--r--   0 njr        (501) staff       (20)  1723312 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/testdata/accounts.zip
--rw-r--r--   0 njr        (501) staff       (20)     4881 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/testdata/accounts1k.tdda
--rw-r--r--   0 njr        (501) staff       (20)      703 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/testdata/ddd.csv
--rw-r--r--   0 njr        (501) staff       (20)     2709 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/testdata/ddd.tdda
--rw-r--r--   0 njr        (501) staff       (20)    13780 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/testdata/elements118.csv
--rw-r--r--   0 njr        (501) staff       (20)    19560 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/testdata/elements118.feather
--rw-r--r--   0 njr        (501) staff       (20)    15835 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/testdata/elements118.pmm
--rw-r--r--   0 njr        (501) staff       (20)    11460 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/testdata/elements92.csv
--rw-r--r--   0 njr        (501) staff       (20)     2954 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples/testdata/elements92.tdda
--rw-r--r--   0 njr        (501) staff       (20)      511 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/examples.py
--rw-r--r--   0 njr        (501) staff       (20)    14680 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/extension.py
--rw-r--r--   0 njr        (501) staff       (20)     9008 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/flags.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.409852 tdda-2.0.9/tdda/constraints/pd/
--rw-r--r--   0 njr        (501) staff       (20)        0 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/pd/__init__.py
--rw-r--r--   0 njr        (501) staff       (20)    49925 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/pd/constraints.py
--rw-r--r--   0 njr        (501) staff       (20)     3290 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/pd/detect.py
--rw-r--r--   0 njr        (501) staff       (20)     2905 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/pd/discover.py
--rw-r--r--   0 njr        (501) staff       (20)     1213 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/pd/extension.py
--rw-r--r--   0 njr        (501) staff       (20)    69043 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/pd/testpdconstraints.py
--rw-r--r--   0 njr        (501) staff       (20)     2987 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/pd/verify.py
--rw-r--r--   0 njr        (501) staff       (20)      130 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/pdconstraints.py
--rw-r--r--   0 njr        (501) staff       (20)      128 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/pddiscover.py
--rw-r--r--   0 njr        (501) staff       (20)      126 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/pdverify.py
--rw-r--r--   0 njr        (501) staff       (20)     9858 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/tdda_json_file_format.md
--rw-r--r--   0 njr        (501) staff       (20)     6805 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testbase.py
--rw-r--r--   0 njr        (501) staff       (20)      641 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testconstraints.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.415755 tdda-2.0.9/tdda/constraints/testdata/
--rw-r--r--   0 njr        (501) staff       (20)      703 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/ddd.csv
--rw-r--r--   0 njr        (501) staff       (20)     2601 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/ddd.tdda
--rw-r--r--   0 njr        (501) staff       (20)     5007 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/detect-els-cmdline-interleaved.csv
--rw-r--r--   0 njr        (501) staff       (20)     5116 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/detect-els-cmdline.csv
--rw-r--r--   0 njr        (501) staff       (20)     5111 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/detect-els-cmdline2.csv
--rw-r--r--   0 njr        (501) staff       (20)      207 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/detect_dups.df
--rw-r--r--   0 njr        (501) staff       (20)    13780 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements118.csv
--rw-r--r--   0 njr        (501) staff       (20)     2158 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements118.df
--rw-r--r--   0 njr        (501) staff       (20)    19560 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements118.feather
--rw-r--r--   0 njr        (501) staff       (20)    15835 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements118.pmm
--rw-r--r--   0 njr        (501) staff       (20)     3278 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements118.tdda
--rw-r--r--   0 njr        (501) staff       (20)     2778 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements118_detect_from_csv.csv
--rw-r--r--   0 njr        (501) staff       (20)     2773 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements118_detect_from_feather.csv
--rw-r--r--   0 njr        (501) staff       (20)      688 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements118_detect_from_feather.feather
--rw-r--r--   0 njr        (501) staff       (20)     5713 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements118oldrex-3.tdda
--rw-r--r--   0 njr        (501) staff       (20)     5949 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements118oldrex.tdda
--rw-r--r--   0 njr        (501) staff       (20)     5770 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements118rex-3.tdda
--rw-r--r--   0 njr        (501) staff       (20)     2277 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements118rex.df
--rw-r--r--   0 njr        (501) staff       (20)     5770 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements118rex.tdda
--rw-r--r--   0 njr        (501) staff       (20)      173 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements118rex_detect.csv
--rw-r--r--   0 njr        (501) staff       (20)      666 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements118rex_detect.df
--rw-r--r--   0 njr        (501) staff       (20)     2994 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements118rex_detect_perc.csv
--rw-r--r--   0 njr        (501) staff       (20)    11460 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements92.csv
--rw-r--r--   0 njr        (501) staff       (20)     2954 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements92.tdda
--rw-r--r--   0 njr        (501) staff       (20)     3458 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements92_pandas.tdda
--rw-r--r--   0 njr        (501) staff       (20)     5376 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements92oldrex.tdda
--rw-r--r--   0 njr        (501) staff       (20)     5332 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/elements92rex.tdda
--rw-r--r--   0 njr        (501) staff       (20)    14504 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/example.csv
--rw-r--r--   0 njr        (501) staff       (20)    24576 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/example.db
--rw-r--r--   0 njr        (501) staff       (20)     1940 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/example.sql
--rw-r--r--   0 njr        (501) staff       (20)     3632 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/ref-accounts1k.tdda
--rw-r--r--   0 njr        (501) staff       (20)     3414 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/ref-accounts25k.tdda
--rw-r--r--   0 njr        (501) staff       (20)      907 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/ref-detect25k-failures.txt
--rw-r--r--   0 njr        (501) staff       (20)       51 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/constraints/testdata/sqlite.conn
--rw-r--r--   0 njr        (501) staff       (20)     2617 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/examples.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.415933 tdda-2.0.9/tdda/gentest/
--rw-r--r--   0 njr        (501) staff       (20)        0 2023-02-10 16:53:23.000000 tdda-2.0.9/tdda/gentest/__init__.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.416672 tdda-2.0.9/tdda/gentest/examples/
--rw-r--r--   0 njr        (501) staff       (20)     1915 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/gentest/examples/README.md
--rw-r--r--   0 njr        (501) staff       (20)      311 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/gentest/examples/example2.sh
--rw-r--r--   0 njr        (501) staff       (20)       11 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/gentest/examples/hey
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.418826 tdda-2.0.9/tdda/gentest/examples/r-examples/
--rw-r--r--   0 njr        (501) staff       (20)      541 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/gentest/examples/r-examples/0-set-variables.R
--rw-r--r--   0 njr        (501) staff       (20)       54 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/gentest/examples/r-examples/00-install.R
--rw-r--r--   0 njr        (501) staff       (20)      389 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/gentest/examples/r-examples/1-compute-weighted-average-tolerance-values.R
--rw-r--r--   0 njr        (501) staff       (20)     1725 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/gentest/examples/r-examples/2-compute-cumulative-percentiles.R
--rw-r--r--   0 njr        (501) staff       (20)     2750 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/gentest/examples/r-examples/3-parametric-regression.R
--rw-r--r--   0 njr        (501) staff       (20)     1778 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/gentest/examples/r-examples/4-non-parametric-regression.R
--rw-r--r--   0 njr        (501) staff       (20)     7686 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/gentest/examples/r-examples/README.md
--rw-r--r--   0 njr        (501) staff       (20)     5426 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/gentest/examples/r-examples/env.data.or.txt
--rw-r--r--   0 njr        (501) staff       (20)    19410 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/gentest/examples/r-examples/env.data.txt
--rw-r--r--   0 njr        (501) staff       (20)   199154 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/gentest/examples/r-examples/site.species.or.txt
--rw-r--r--   0 njr        (501) staff       (20)   354013 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/gentest/examples/r-examples/site.species.txt
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.421818 tdda-2.0.9/tdda/referencetest/
--rw-r--r--   0 njr        (501) staff       (20)     6515 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/__init__.py
--rw-r--r--   0 njr        (501) staff       (20)     3260 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/basecomparison.py
--rw-r--r--   0 njr        (501) staff       (20)     1131 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/captureoutput.py
--rw-r--r--   0 njr        (501) staff       (20)    40454 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/checkfiles.py
--rw-r--r--   0 njr        (501) staff       (20)    20411 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/checkpandas.py
--rw-r--r--   0 njr        (501) staff       (20)     4328 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/diffrex.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.422251 tdda-2.0.9/tdda/referencetest/examples/
--rw-r--r--   0 njr        (501) staff       (20)     4851 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/README.md
--rw-r--r--   0 njr        (501) staff       (20)      888 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/dataframes.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.394782 tdda-2.0.9/tdda/referencetest/examples/exercises-pytest/
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.422908 tdda-2.0.9/tdda/referencetest/examples/exercises-pytest/exercise1/
--rw-r--r--   0 njr        (501) staff       (20)      478 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/exercises-pytest/exercise1/conftest.py
--rw-r--r--   0 njr        (501) staff       (20)     9048 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/exercises-pytest/exercise1/expected.html
--rw-r--r--   0 njr        (501) staff       (20)     4047 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/exercises-pytest/exercise1/generators.py
--rw-r--r--   0 njr        (501) staff       (20)      489 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/exercises-pytest/exercise1/test_all.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.423571 tdda-2.0.9/tdda/referencetest/examples/exercises-pytest/exercise2/
--rw-r--r--   0 njr        (501) staff       (20)      476 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/exercises-pytest/exercise2/conftest.py
--rw-r--r--   0 njr        (501) staff       (20)     9048 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/exercises-pytest/exercise2/expected.html
--rw-r--r--   0 njr        (501) staff       (20)     4047 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/exercises-pytest/exercise2/generators.py
--rw-r--r--   0 njr        (501) staff       (20)      654 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/exercises-pytest/exercise2/test_all.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.395002 tdda-2.0.9/tdda/referencetest/examples/exercises-unittest/
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.424035 tdda-2.0.9/tdda/referencetest/examples/exercises-unittest/exercise1/
--rw-r--r--   0 njr        (501) staff       (20)     9048 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/exercises-unittest/exercise1/expected.html
--rw-r--r--   0 njr        (501) staff       (20)     4047 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/exercises-unittest/exercise1/generators.py
--rw-r--r--   0 njr        (501) staff       (20)      606 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/exercises-unittest/exercise1/test_all.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.424528 tdda-2.0.9/tdda/referencetest/examples/exercises-unittest/exercise2/
--rw-r--r--   0 njr        (501) staff       (20)     9048 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/exercises-unittest/exercise2/expected.html
--rw-r--r--   0 njr        (501) staff       (20)     4047 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/exercises-unittest/exercise2/generators.py
--rw-r--r--   0 njr        (501) staff       (20)      887 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/exercises-unittest/exercise2/test_all.py
--rw-r--r--   0 njr        (501) staff       (20)     4047 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/generators.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.424986 tdda-2.0.9/tdda/referencetest/examples/pytest/
--rw-r--r--   0 njr        (501) staff       (20)      631 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/pytest/conftest.py
--rw-r--r--   0 njr        (501) staff       (20)     5785 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/pytest/test_using_referencepytest.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.425874 tdda-2.0.9/tdda/referencetest/examples/reference/
--rw-r--r--   0 njr        (501) staff       (20)      530 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/reference/dataframe_result.csv
--rw-r--r--   0 njr        (501) staff       (20)     1096 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/reference/dataframe_result2.csv
--rw-r--r--   0 njr        (501) staff       (20)     1570 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/reference/file_result.html
--rw-r--r--   0 njr        (501) staff       (20)     9048 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/reference/string_result.html
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.426059 tdda-2.0.9/tdda/referencetest/examples/unittest/
--rw-r--r--   0 njr        (501) staff       (20)     6643 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples/unittest/test_using_referencetestcase.py
--rw-r--r--   0 njr        (501) staff       (20)      556 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/examples.py
--rw-r--r--   0 njr        (501) staff       (20)    55226 2023-02-10 19:47:45.000000 tdda-2.0.9/tdda/referencetest/gentest.py
--rw-r--r--   0 njr        (501) staff       (20)      962 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/gentest_boilerplate.py
--rw-r--r--   0 njr        (501) staff       (20)     1500 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/pytestconfig.py
--rw-r--r--   0 njr        (501) staff       (20)    10499 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/referencepytest.py
--rw-r--r--   0 njr        (501) staff       (20)    36489 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/referencetest.py
--rw-r--r--   0 njr        (501) staff       (20)    11082 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/referencetestcase.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.427343 tdda-2.0.9/tdda/referencetest/tests/
--rw-r--r--   0 njr        (501) staff       (20)        0 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/tests/__init__.py
--rw-r--r--   0 njr        (501) staff       (20)      484 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/tests/alltests.py
--rw-r--r--   0 njr        (501) staff       (20)     1701 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/tests/testbase.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.428535 tdda-2.0.9/tdda/referencetest/tests/testdata/
--rw-r--r--   0 njr        (501) staff       (20)     4389 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/tests/testdata/colours.txt
--rw-r--r--   0 njr        (501) staff       (20)       28 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/tests/testdata/double.txt
--rw-r--r--   0 njr        (501) staff       (20)        0 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/tests/testdata/empty.txt
--rw-r--r--   0 njr        (501) staff       (20)      218 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/tests/testdata/left.txt
--rw-r--r--   0 njr        (501) staff       (20)      171 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/tests/testdata/ref.txt
--rw-r--r--   0 njr        (501) staff       (20)      198 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/tests/testdata/removals.txt
--rw-r--r--   0 njr        (501) staff       (20)       14 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/tests/testdata/single.txt
--rw-r--r--   0 njr        (501) staff       (20)       14 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/tests/testdata/single2.txt
--rw-r--r--   0 njr        (501) staff       (20)    15273 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/tests/testfiles.py
--rw-r--r--   0 njr        (501) staff       (20)     4446 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/tests/testpandas.py
--rw-r--r--   0 njr        (501) staff       (20)     2113 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/tests/testregeneration.py
--rw-r--r--   0 njr        (501) staff       (20)    11656 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/tests/teststrings.py
--rw-r--r--   0 njr        (501) staff       (20)     2610 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/referencetest/utils.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.429754 tdda-2.0.9/tdda/rexpy/
--rw-r--r--   0 njr        (501) staff       (20)      176 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/rexpy/__init__.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.430237 tdda-2.0.9/tdda/rexpy/examples/
--rw-r--r--   0 njr        (501) staff       (20)     1126 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/rexpy/examples/agents9.txt
--rw-r--r--   0 njr        (501) staff       (20)       44 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/rexpy/examples/headed-ids.txt
--rw-r--r--   0 njr        (501) staff       (20)      230 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/rexpy/examples/ids.py
--rw-r--r--   0 njr        (501) staff       (20)      364 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/rexpy/examples/pandas_ids.py
--rw-r--r--   0 njr        (501) staff       (20)      465 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/rexpy/examples.py
--rw-r--r--   0 njr        (501) staff       (20)      412 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/rexpy/relib.py
--rw-r--r--   0 njr        (501) staff       (20)    91873 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/rexpy/rexpy.py
--rw-r--r--   0 njr        (501) staff       (20)     3230 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/rexpy/seq.py
--rw-r--r--   0 njr        (501) staff       (20)     1033 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/rexpy/testhypo.py
--rw-r--r--   0 njr        (501) staff       (20)    74007 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/rexpy/testrexpy.py
--rw-r--r--   0 njr        (501) staff       (20)      716 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/rexpy/testseq.py
--rw-r--r--   0 njr        (501) staff       (20)     1090 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/testconfig.py
--rw-r--r--   0 njr        (501) staff       (20)      708 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/testtdda.py
--rw-r--r--   0 njr        (501) staff       (20)      246 2023-02-10 19:49:27.000000 tdda-2.0.9/tdda/version.py
--rw-r--r--   0 njr        (501) staff       (20)    10442 2022-04-01 21:00:40.000000 tdda-2.0.9/tdda/writabletestcase.py
-drwxr-xr-x   0 njr        (501) staff       (20)        0 2023-02-10 19:50:14.399189 tdda-2.0.9/tdda.egg-info/
--rw-r--r--   0 njr        (501) staff       (20)     4504 2023-02-10 19:50:14.000000 tdda-2.0.9/tdda.egg-info/PKG-INFO
--rw-r--r--   0 njr        (501) staff       (20)     8049 2023-02-10 19:50:14.000000 tdda-2.0.9/tdda.egg-info/SOURCES.txt
--rw-r--r--   0 njr        (501) staff       (20)        1 2023-02-10 19:50:14.000000 tdda-2.0.9/tdda.egg-info/dependency_links.txt
--rw-r--r--   0 njr        (501) staff       (20)       85 2023-02-10 19:50:14.000000 tdda-2.0.9/tdda.egg-info/entry_points.txt
--rw-r--r--   0 njr        (501) staff       (20)        1 2023-02-10 16:16:28.000000 tdda-2.0.9/tdda.egg-info/not-zip-safe
--rw-r--r--   0 njr        (501) staff       (20)       28 2023-02-10 19:50:14.000000 tdda-2.0.9/tdda.egg-info/requires.txt
--rw-r--r--   0 njr        (501) staff       (20)        5 2023-02-10 19:50:14.000000 tdda-2.0.9/tdda.egg-info/top_level.txt
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.022753 tdda-2.1.2/
+-rw-r--r--   0 njr        (501) staff       (20)     1100 2022-04-01 21:00:40.000000 tdda-2.1.2/LICENSE.txt
+-rw-r--r--   0 njr        (501) staff       (20)       38 2022-04-01 21:00:40.000000 tdda-2.1.2/MANIFEST.in
+-rw-r--r--   0 njr        (501) staff       (20)     4616 2024-04-30 16:28:19.022669 tdda-2.1.2/PKG-INFO
+-rw-r--r--   0 njr        (501) staff       (20)     4233 2024-04-30 15:44:51.000000 tdda-2.1.2/README.md
+-rw-r--r--   0 njr        (501) staff       (20)      438 2024-04-30 16:23:26.000000 tdda-2.1.2/pyproject.toml
+-rw-r--r--   0 njr        (501) staff       (20)      200 2024-04-30 16:28:19.022986 tdda-2.1.2/setup.cfg
+-rw-r--r--   0 njr        (501) staff       (20)     2309 2024-02-12 09:13:47.000000 tdda-2.1.2/setup.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:18.995695 tdda-2.1.2/tdda/
+-rw-r--r--   0 njr        (501) staff       (20)    28592 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/CHANGES.py
+-rw-r--r--   0 njr        (501) staff       (20)      987 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/__init__.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:18.998339 tdda-2.1.2/tdda/constraints/
+-rw-r--r--   0 njr        (501) staff       (20)      455 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/__init__.py
+-rw-r--r--   0 njr        (501) staff       (20)    36493 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/base.py
+-rw-r--r--   0 njr        (501) staff       (20)    24998 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/baseconstraints.py
+-rw-r--r--   0 njr        (501) staff       (20)     8001 2024-02-19 15:49:06.000000 tdda-2.1.2/tdda/constraints/console.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:18.999360 tdda-2.1.2/tdda/constraints/db/
+-rw-r--r--   0 njr        (501) staff       (20)        0 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/db/__init__.py
+-rw-r--r--   0 njr        (501) staff       (20)    17342 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/db/constraints.py
+-rw-r--r--   0 njr        (501) staff       (20)     2754 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/db/detect.py
+-rw-r--r--   0 njr        (501) staff       (20)     2934 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/db/discover.py
+-rw-r--r--   0 njr        (501) staff       (20)    30601 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/db/drivers.py
+-rw-r--r--   0 njr        (501) staff       (20)     1444 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/db/extension.py
+-rw-r--r--   0 njr        (501) staff       (20)    13836 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/db/testdbconstraints.py
+-rw-r--r--   0 njr        (501) staff       (20)     2491 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/db/verify.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.001838 tdda-2.1.2/tdda/constraints/examples/
+-rw-r--r--   0 njr        (501) staff       (20)     7336 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/README.md
+-rw-r--r--   0 njr        (501) staff       (20)     4700 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/accounts25k.tdda
+-rw-r--r--   0 njr        (501) staff       (20)      326 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/accounts_detect_25k_against_1k.py
+-rw-r--r--   0 njr        (501) staff       (20)      327 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/accounts_discover_1k.py
+-rw-r--r--   0 njr        (501) staff       (20)      223 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/accounts_verify_1k.py
+-rw-r--r--   0 njr        (501) staff       (20)      226 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/accounts_verify_25k.py
+-rw-r--r--   0 njr        (501) staff       (20)      236 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/accounts_verify_25k_against_1k.py
+-rw-r--r--   0 njr        (501) staff       (20)      398 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/accounts_verify_25k_against_1k_feather.py
+-rw-r--r--   0 njr        (501) staff       (20)      264 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/accounts_verify_25k_to_frame.py
+-rw-r--r--   0 njr        (501) staff       (20)     2800 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/elements118.tdda
+-rw-r--r--   0 njr        (501) staff       (20)      326 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/elements_detect_118_against_92.py
+-rw-r--r--   0 njr        (501) staff       (20)      327 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/elements_discover_92.py
+-rw-r--r--   0 njr        (501) staff       (20)      226 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/elements_verify_118.py
+-rw-r--r--   0 njr        (501) staff       (20)      236 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/elements_verify_118_against_92.py
+-rw-r--r--   0 njr        (501) staff       (20)      398 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/elements_verify_118_against_92_feather.py
+-rw-r--r--   0 njr        (501) staff       (20)      223 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/elements_verify_92.py
+-rw-r--r--   0 njr        (501) staff       (20)    13795 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/files_extension.py
+-rw-r--r--   0 njr        (501) staff       (20)     1078 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/simple_discovery.py
+-rw-r--r--   0 njr        (501) staff       (20)     2176 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/simple_verification.py
+-rw-r--r--   0 njr        (501) staff       (20)      373 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/simple_verify_fail.py
+-rw-r--r--   0 njr        (501) staff       (20)      316 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/simple_verify_pass.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.003691 tdda-2.1.2/tdda/constraints/examples/testdata/
+-rw-r--r--   0 njr        (501) staff       (20)  1723312 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/testdata/accounts.zip
+-rw-r--r--   0 njr        (501) staff       (20)     4881 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/testdata/accounts1k.tdda
+-rw-r--r--   0 njr        (501) staff       (20)      703 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/testdata/ddd.csv
+-rw-r--r--   0 njr        (501) staff       (20)     2709 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/testdata/ddd.tdda
+-rw-r--r--   0 njr        (501) staff       (20)    13780 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/testdata/elements118.csv
+-rw-r--r--   0 njr        (501) staff       (20)    19560 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/testdata/elements118.feather
+-rw-r--r--   0 njr        (501) staff       (20)    15835 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/testdata/elements118.pmm
+-rw-r--r--   0 njr        (501) staff       (20)    11460 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/testdata/elements92.csv
+-rw-r--r--   0 njr        (501) staff       (20)     2954 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/examples/testdata/elements92.tdda
+-rw-r--r--   0 njr        (501) staff       (20)      511 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/examples.py
+-rw-r--r--   0 njr        (501) staff       (20)    14680 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/extension.py
+-rw-r--r--   0 njr        (501) staff       (20)     9008 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/flags.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.004597 tdda-2.1.2/tdda/constraints/pd/
+-rw-r--r--   0 njr        (501) staff       (20)        0 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/pd/__init__.py
+-rw-r--r--   0 njr        (501) staff       (20)    53538 2024-04-30 15:49:32.000000 tdda-2.1.2/tdda/constraints/pd/constraints.py
+-rw-r--r--   0 njr        (501) staff       (20)     3261 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/constraints/pd/detect.py
+-rw-r--r--   0 njr        (501) staff       (20)     2987 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/constraints/pd/discover.py
+-rw-r--r--   0 njr        (501) staff       (20)     1364 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/constraints/pd/extension.py
+-rw-r--r--   0 njr        (501) staff       (20)    73648 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/constraints/pd/testpdconstraints.py
+-rw-r--r--   0 njr        (501) staff       (20)     2926 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/constraints/pd/verify.py
+-rw-r--r--   0 njr        (501) staff       (20)      130 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/pdconstraints.py
+-rw-r--r--   0 njr        (501) staff       (20)      128 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/pddiscover.py
+-rw-r--r--   0 njr        (501) staff       (20)      126 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/pdverify.py
+-rw-r--r--   0 njr        (501) staff       (20)     9858 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/tdda_json_file_format.md
+-rw-r--r--   0 njr        (501) staff       (20)     6805 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/testbase.py
+-rw-r--r--   0 njr        (501) staff       (20)      641 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/constraints/testconstraints.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.009089 tdda-2.1.2/tdda/constraints/testdata/
+-rw-r--r--   0 njr        (501) staff       (20)      703 2024-01-29 09:44:59.000000 tdda-2.1.2/tdda/constraints/testdata/d.csv
+-rw-r--r--   0 njr        (501) staff       (20)      703 2024-01-29 09:59:11.000000 tdda-2.1.2/tdda/constraints/testdata/ddd.csv
+-rw-r--r--   0 njr        (501) staff       (20)     2601 2024-01-29 09:59:11.000000 tdda-2.1.2/tdda/constraints/testdata/ddd.tdda
+-rw-r--r--   0 njr        (501) staff       (20)     5007 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/detect-els-cmdline-interleaved.csv
+-rw-r--r--   0 njr        (501) staff       (20)     5116 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/detect-els-cmdline.csv
+-rw-r--r--   0 njr        (501) staff       (20)     5111 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/detect-els-cmdline2.csv
+-rw-r--r--   0 njr        (501) staff       (20)      207 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/detect_dups.df
+-rw-r--r--   0 njr        (501) staff       (20)    13780 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118.csv
+-rw-r--r--   0 njr        (501) staff       (20)     2158 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118.df
+-rw-r--r--   0 njr        (501) staff       (20)    19560 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118.feather
+-rw-r--r--   0 njr        (501) staff       (20)    16972 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/constraints/testdata/elements118.parquet
+-rw-r--r--   0 njr        (501) staff       (20)    15835 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118.pmm
+-rw-r--r--   0 njr        (501) staff       (20)     3278 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118.tdda
+-rw-r--r--   0 njr        (501) staff       (20)     2778 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118_detect_from_csv.csv
+-rw-r--r--   0 njr        (501) staff       (20)     2773 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118_detect_from_feather.csv
+-rw-r--r--   0 njr        (501) staff       (20)      688 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118_detect_from_feather.feather
+-rw-r--r--   0 njr        (501) staff       (20)     5713 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118oldrex-3.tdda
+-rw-r--r--   0 njr        (501) staff       (20)     5949 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118oldrex.tdda
+-rw-r--r--   0 njr        (501) staff       (20)     5770 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118rex-3.tdda
+-rw-r--r--   0 njr        (501) staff       (20)     2277 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118rex.df
+-rw-r--r--   0 njr        (501) staff       (20)     5770 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118rex.tdda
+-rw-r--r--   0 njr        (501) staff       (20)      173 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118rex_detect.csv
+-rw-r--r--   0 njr        (501) staff       (20)      666 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118rex_detect.df
+-rw-r--r--   0 njr        (501) staff       (20)     2994 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements118rex_detect_perc.csv
+-rw-r--r--   0 njr        (501) staff       (20)    11460 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements92.csv
+-rw-r--r--   0 njr        (501) staff       (20)    15459 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/constraints/testdata/elements92.parquet
+-rw-r--r--   0 njr        (501) staff       (20)     2954 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements92.tdda
+-rw-r--r--   0 njr        (501) staff       (20)     3458 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements92_pandas.tdda
+-rw-r--r--   0 njr        (501) staff       (20)     5376 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements92oldrex.tdda
+-rw-r--r--   0 njr        (501) staff       (20)     5332 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/elements92rex.tdda
+-rw-r--r--   0 njr        (501) staff       (20)    14504 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/example.csv
+-rw-r--r--   0 njr        (501) staff       (20)    24576 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/example.db
+-rw-r--r--   0 njr        (501) staff       (20)     1940 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/example.sql
+-rw-r--r--   0 njr        (501) staff       (20)     3632 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/ref-accounts1k.tdda
+-rw-r--r--   0 njr        (501) staff       (20)     3414 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/ref-accounts25k.tdda
+-rw-r--r--   0 njr        (501) staff       (20)      907 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/ref-detect25k-failures.txt
+-rw-r--r--   0 njr        (501) staff       (20)       51 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/constraints/testdata/sqlite.conn
+-rw-r--r--   0 njr        (501) staff       (20)     2617 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/examples.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.009223 tdda-2.1.2/tdda/gentest/
+-rw-r--r--   0 njr        (501) staff       (20)        0 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/__init__.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.009592 tdda-2.1.2/tdda/gentest/examples/
+-rw-r--r--   0 njr        (501) staff       (20)     1915 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/README.md
+-rw-r--r--   0 njr        (501) staff       (20)      311 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/example2.sh
+-rw-r--r--   0 njr        (501) staff       (20)       11 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/hey
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.011363 tdda-2.1.2/tdda/gentest/examples/r-examples/
+-rw-r--r--   0 njr        (501) staff       (20)      541 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/0-set-variables.R
+-rw-r--r--   0 njr        (501) staff       (20)       54 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/00-install.R
+-rw-r--r--   0 njr        (501) staff       (20)      389 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/1-compute-weighted-average-tolerance-values.R
+-rw-r--r--   0 njr        (501) staff       (20)     1725 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/2-compute-cumulative-percentiles.R
+-rw-r--r--   0 njr        (501) staff       (20)     2750 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/3-parametric-regression.R
+-rw-r--r--   0 njr        (501) staff       (20)     1778 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/4-non-parametric-regression.R
+-rw-r--r--   0 njr        (501) staff       (20)     7686 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/README.md
+-rw-r--r--   0 njr        (501) staff       (20)     5426 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/env.data.or.txt
+-rw-r--r--   0 njr        (501) staff       (20)    19410 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/env.data.txt
+-rw-r--r--   0 njr        (501) staff       (20)   199154 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/site.species.or.txt
+-rw-r--r--   0 njr        (501) staff       (20)   354013 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/gentest/examples/r-examples/site.species.txt
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.013789 tdda-2.1.2/tdda/referencetest/
+-rw-r--r--   0 njr        (501) staff       (20)     6515 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/__init__.py
+-rw-r--r--   0 njr        (501) staff       (20)     3260 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/basecomparison.py
+-rw-r--r--   0 njr        (501) staff       (20)     1131 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/captureoutput.py
+-rw-r--r--   0 njr        (501) staff       (20)    40454 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/checkfiles.py
+-rw-r--r--   0 njr        (501) staff       (20)    22759 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/referencetest/checkpandas.py
+-rw-r--r--   0 njr        (501) staff       (20)     4328 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/diffrex.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.014228 tdda-2.1.2/tdda/referencetest/examples/
+-rw-r--r--   0 njr        (501) staff       (20)     4851 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/README.md
+-rw-r--r--   0 njr        (501) staff       (20)      888 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/dataframes.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:18.993083 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.014880 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise1/
+-rw-r--r--   0 njr        (501) staff       (20)      478 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise1/conftest.py
+-rw-r--r--   0 njr        (501) staff       (20)     9048 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise1/expected.html
+-rw-r--r--   0 njr        (501) staff       (20)     4047 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise1/generators.py
+-rw-r--r--   0 njr        (501) staff       (20)      489 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise1/test_all.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.015493 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise2/
+-rw-r--r--   0 njr        (501) staff       (20)      476 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise2/conftest.py
+-rw-r--r--   0 njr        (501) staff       (20)     9048 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise2/expected.html
+-rw-r--r--   0 njr        (501) staff       (20)     4047 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise2/generators.py
+-rw-r--r--   0 njr        (501) staff       (20)      654 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise2/test_all.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:18.993258 tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.015938 tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise1/
+-rw-r--r--   0 njr        (501) staff       (20)     9048 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise1/expected.html
+-rw-r--r--   0 njr        (501) staff       (20)     4047 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise1/generators.py
+-rw-r--r--   0 njr        (501) staff       (20)      606 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise1/test_all.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.016377 tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise2/
+-rw-r--r--   0 njr        (501) staff       (20)     9048 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise2/expected.html
+-rw-r--r--   0 njr        (501) staff       (20)     4047 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise2/generators.py
+-rw-r--r--   0 njr        (501) staff       (20)      887 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise2/test_all.py
+-rw-r--r--   0 njr        (501) staff       (20)     4047 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/generators.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.016662 tdda-2.1.2/tdda/referencetest/examples/pytest/
+-rw-r--r--   0 njr        (501) staff       (20)      631 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/pytest/conftest.py
+-rw-r--r--   0 njr        (501) staff       (20)     5785 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/pytest/test_using_referencepytest.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.017192 tdda-2.1.2/tdda/referencetest/examples/reference/
+-rw-r--r--   0 njr        (501) staff       (20)      530 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/reference/dataframe_result.csv
+-rw-r--r--   0 njr        (501) staff       (20)     1096 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/reference/dataframe_result2.csv
+-rw-r--r--   0 njr        (501) staff       (20)     1570 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/reference/file_result.html
+-rw-r--r--   0 njr        (501) staff       (20)     9048 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/reference/string_result.html
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.017332 tdda-2.1.2/tdda/referencetest/examples/unittest/
+-rw-r--r--   0 njr        (501) staff       (20)     6643 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/examples/unittest/test_using_referencetestcase.py
+-rw-r--r--   0 njr        (501) staff       (20)      556 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/examples.py
+-rw-r--r--   0 njr        (501) staff       (20)    55226 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/gentest.py
+-rw-r--r--   0 njr        (501) staff       (20)      962 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/gentest_boilerplate.py
+-rw-r--r--   0 njr        (501) staff       (20)     3962 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/referencetest/pddates.py
+-rw-r--r--   0 njr        (501) staff       (20)     1500 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/pytestconfig.py
+-rw-r--r--   0 njr        (501) staff       (20)    10499 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/referencepytest.py
+-rw-r--r--   0 njr        (501) staff       (20)    36641 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/referencetest/referencetest.py
+-rw-r--r--   0 njr        (501) staff       (20)    11082 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/referencetestcase.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.018080 tdda-2.1.2/tdda/referencetest/tests/
+-rw-r--r--   0 njr        (501) staff       (20)        0 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/__init__.py
+-rw-r--r--   0 njr        (501) staff       (20)      484 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/alltests.py
+-rw-r--r--   0 njr        (501) staff       (20)     1701 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testbase.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.019447 tdda-2.1.2/tdda/referencetest/tests/testdata/
+-rw-r--r--   0 njr        (501) staff       (20)     4389 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/colours.txt
+-rw-r--r--   0 njr        (501) staff       (20)       28 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/double.txt
+-rw-r--r--   0 njr        (501) staff       (20)        0 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/empty.txt
+-rw-r--r--   0 njr        (501) staff       (20)      219 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/frames_fail1.txt
+-rw-r--r--   0 njr        (501) staff       (20)       64 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/frames_fail2.txt
+-rw-r--r--   0 njr        (501) staff       (20)       66 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/frames_fail3.txt
+-rw-r--r--   0 njr        (501) staff       (20)      218 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/left.txt
+-rw-r--r--   0 njr        (501) staff       (20)      171 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/ref.txt
+-rw-r--r--   0 njr        (501) staff       (20)      198 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/removals.txt
+-rw-r--r--   0 njr        (501) staff       (20)       14 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/single.txt
+-rw-r--r--   0 njr        (501) staff       (20)       14 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testdata/single2.txt
+-rw-r--r--   0 njr        (501) staff       (20)    15273 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testfiles.py
+-rw-r--r--   0 njr        (501) staff       (20)     6971 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/referencetest/tests/testpandas.py
+-rw-r--r--   0 njr        (501) staff       (20)     2113 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/testregeneration.py
+-rw-r--r--   0 njr        (501) staff       (20)    11656 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/referencetest/tests/teststrings.py
+-rw-r--r--   0 njr        (501) staff       (20)     2610 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/referencetest/utils.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.020643 tdda-2.1.2/tdda/rexpy/
+-rw-r--r--   0 njr        (501) staff       (20)      176 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/rexpy/__init__.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.021164 tdda-2.1.2/tdda/rexpy/examples/
+-rw-r--r--   0 njr        (501) staff       (20)     1126 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/rexpy/examples/agents9.txt
+-rw-r--r--   0 njr        (501) staff       (20)       44 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/rexpy/examples/headed-ids.txt
+-rw-r--r--   0 njr        (501) staff       (20)      230 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/rexpy/examples/ids.py
+-rw-r--r--   0 njr        (501) staff       (20)      364 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/rexpy/examples/pandas_ids.py
+-rw-r--r--   0 njr        (501) staff       (20)      465 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/rexpy/examples.py
+-rw-r--r--   0 njr        (501) staff       (20)       50 2023-03-27 07:08:57.000000 tdda-2.1.2/tdda/rexpy/quality.py
+-rw-r--r--   0 njr        (501) staff       (20)      412 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/rexpy/relib.py
+-rw-r--r--   0 njr        (501) staff       (20)    91873 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/rexpy/rexpy.py
+-rw-r--r--   0 njr        (501) staff       (20)     3230 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/rexpy/seq.py
+-rw-r--r--   0 njr        (501) staff       (20)     1033 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/rexpy/testhypo.py
+-rw-r--r--   0 njr        (501) staff       (20)    74007 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/rexpy/testrexpy.py
+-rw-r--r--   0 njr        (501) staff       (20)      716 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/rexpy/testseq.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.022202 tdda-2.1.2/tdda/serial/
+-rw-r--r--   0 njr        (501) staff       (20)       93 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/serial/__init__.py
+-rw-r--r--   0 njr        (501) staff       (20)     6088 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/serial/base.py
+-rw-r--r--   0 njr        (501) staff       (20)     1449 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/serial/cli.py
+-rw-r--r--   0 njr        (501) staff       (20)    11284 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/serial/csvw.py
+-rw-r--r--   0 njr        (501) staff       (20)     1478 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/serial/pandasio.py
+-rw-r--r--   0 njr        (501) staff       (20)     4948 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/serial/reader.py
+-rw-r--r--   0 njr        (501) staff       (20)    17656 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/serial/testserialmetadata.py
+-rw-r--r--   0 njr        (501) staff       (20)     1484 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/serial/utils.py
+-rw-r--r--   0 njr        (501) staff       (20)     1090 2022-04-01 21:00:40.000000 tdda-2.1.2/tdda/testconfig.py
+-rw-r--r--   0 njr        (501) staff       (20)      753 2024-04-30 15:41:12.000000 tdda-2.1.2/tdda/testtdda.py
+-rw-r--r--   0 njr        (501) staff       (20)      246 2024-04-30 16:26:42.000000 tdda-2.1.2/tdda/version.py
+-rw-r--r--   0 njr        (501) staff       (20)    10442 2024-02-12 09:13:47.000000 tdda-2.1.2/tdda/writabletestcase.py
+drwxr-xr-x   0 njr        (501) staff       (20)        0 2024-04-30 16:28:19.022424 tdda-2.1.2/tdda.egg-info/
+-rw-r--r--   0 njr        (501) staff       (20)     4616 2024-04-30 16:28:18.000000 tdda-2.1.2/tdda.egg-info/PKG-INFO
+-rw-r--r--   0 njr        (501) staff       (20)     8561 2024-04-30 16:28:18.000000 tdda-2.1.2/tdda.egg-info/SOURCES.txt
+-rw-r--r--   0 njr        (501) staff       (20)        1 2024-04-30 16:28:18.000000 tdda-2.1.2/tdda.egg-info/dependency_links.txt
+-rw-r--r--   0 njr        (501) staff       (20)       85 2024-04-30 16:28:18.000000 tdda-2.1.2/tdda.egg-info/entry_points.txt
+-rw-r--r--   0 njr        (501) staff       (20)        1 2023-02-10 16:16:28.000000 tdda-2.1.2/tdda.egg-info/not-zip-safe
+-rw-r--r--   0 njr        (501) staff       (20)       28 2024-04-30 16:28:18.000000 tdda-2.1.2/tdda.egg-info/requires.txt
+-rw-r--r--   0 njr        (501) staff       (20)        5 2024-04-30 16:28:18.000000 tdda-2.1.2/tdda.egg-info/top_level.txt
```

### Comparing `tdda-2.0.9/LICENSE.txt` & `tdda-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/PKG-INFO` & `tdda-2.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: tdda
-Version: 2.0.9
-Summary: Test Driven Data Analysis
+Version: 2.1.2
 Home-page: http://www.stochasticsolutions.com
 Download-URL: https://github.com/tdda/tdda
-Author: Stochastic Solutions Limited
-Author-email: info@StochasticSolutions.com
+Author: Simon Brown
+Author-email: Nick Radcliffe <njr@stochasticsolutions.com>
 License: MIT
 Keywords: tdda constraint referencetest rexpy
+Requires-Python: >=3.8
 License-File: LICENSE.txt
+Requires-Dist: numpy>=1.20.3
+Requires-Dist: pandas>=1.5.2
 
 Test-Driven Data Analysis (Python TDDA library)
 ===============================================
 
 What is it?
 -----------
 
@@ -120,9 +122,12 @@
   * General Notes on Constraints and Assertions: http://www.tdda.info/constraints-and-assertions
   * Notes on using the Pandas constraints library:
     http://www.tdda.info/constraint-discovery-and-verification-for-pandas-dataframes
   * PyCon UK Talk on TDDA:
       - Video: https://www.youtube.com/watch?v=FIw_7aUuY50
       - Slides and Rough Transcript:   http://www.tdda.info/slides-and-rough-transcript-of-tdda-talk-from-pycon-uk-2016
 
+  * <a rel="me" href="https://mathstodon.xyz/@tdda">Mastodon</a>
+
+
 All examples, tests and code run under Python 2.7, Python 3.5 and Python 3.6.
```

### Comparing `tdda-2.0.9/README.md` & `tdda-2.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -108,9 +108,12 @@
   * General Notes on Constraints and Assertions: http://www.tdda.info/constraints-and-assertions
   * Notes on using the Pandas constraints library:
     http://www.tdda.info/constraint-discovery-and-verification-for-pandas-dataframes
   * PyCon UK Talk on TDDA:
       - Video: https://www.youtube.com/watch?v=FIw_7aUuY50
       - Slides and Rough Transcript:   http://www.tdda.info/slides-and-rough-transcript-of-tdda-talk-from-pycon-uk-2016
 
+  * <a rel="me" href="https://mathstodon.xyz/@tdda">Mastodon</a>
+
+
 All examples, tests and code run under Python 2.7, Python 3.5 and Python 3.6.
```

### Comparing `tdda-2.0.9/setup.py` & `tdda-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/CHANGES.py` & `tdda-2.1.2/tdda/CHANGES.py`

 * *Files 25% similar despite different names*

```diff
@@ -531,8 +531,233 @@
 Now catch this and just don't check IP address.
 
 conf.py had a bad path manipulation to get the version;
 should be fixed now.
 
 10.02.2023 2.0.09
 *Actually* fix the IPv6 etc. issue
+
+26.01.2024 2.0.10
+Remove leading zeros in gentest test
+
+----------------------------- pandas2 branch -----------------------------
+
+12-02-2024
+Pandas 2 doesn't like inferring dates, so we now do this ourselves
+when reading CSVs. Obviously, this isn't ideal, and in time we'll
+encourage people to specify formats in metadata files.
+
+Pandas 2 also doesn't like old version of pyarrow, so we're adding
+a requirement for a more modern version.
+
+19-02-2024
+Added support for reading and writin parquet and started to deprecate
+feather.
+
+Also started adding support for using csvmetadata, csvw metadata
+and frictionless metadata, but incomplete. Currently it is just
+assuming the csvmetadata library is around; before release that
+will need to be made a proper dependency or partly moved under
+this project or something.
+
+23-02-2024
+Update data frame comparisons and difference reporting.
+Changes test to reflect new reporting.
+changed test to use assertStringCorrect.
+
+------------------------- end of pandas2 branch --------------------------
+
+------------------------- serial metdata branch --------------------------
+
+Imported work previously in different csvmetadata repo as
+tdda.serial.  Commit history:
+
+    commit c0e29f2920312d1567b0b9f1471320335d815739
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Mon Jan 29 18:25:54 2024 +0000
+
+        Initial commit
+
+    commit 7eeee6d1fd0dc6d2e7a33037e75957ac92dfb96a
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Mon Jan 29 18:35:12 2024 +0000
+
+        Initial commit
+
+    commit 337a41a15b506430bd7584ebb719ccac657970da
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Mon Jan 29 18:37:39 2024 +0000
+
+        Update README.md
+
+    commit d8599934ecda556414a1e8e4c867a18ce551e296
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Thu Feb 1 09:10:03 2024 +0000
+
+        Add embryonic csvmetadata.py
+
+    commit 7457ec89bb9c35bbedfef5d1d59305b582f5c4be
+    Merge: d859993 337a41a
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Thu Feb 1 09:10:20 2024 +0000
+
+        Merge branch 'main' of github.com:njr0/csvw2pd
+
+    commit 99dbcc015b933c479e11dd7d1478f50672bd425f
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Thu Feb 1 21:11:52 2024 +0000
+
+        Generalized by using intermediate Metadata object
+
+    commit b21f084d110427e88453ae1560de12adff6df4be
+    Author: overskilling <neil.skilling@overskilling.com>
+    Date:   Sat Feb 3 17:13:40 2024 +0000
+
+        Working with pytest
+
+        I had to make some modifications to make this work out of the
+        box with a fresh environment and pytest. You probably have
+        some stuff installed globally.
+
+        __init__.py was preventing pytest loading the functions it
+        needed as this is not a module csvw2pd.py was referencing
+        outpath when it meant inpath Added requirements.in - pip
+        install pip-tools and then run pip-compile to get the
+        requirements.txt file
+
+    commit 8173ea4bccc1964e354fddda44ca07d831c3cb0e
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Sat Feb 3 17:19:01 2024 +0000
+
+        Add __str__ to CSVMetadata
+
+    commit 562882fb28111a850c406a9d98d177c5ff774d7a
+    Merge: 99dbcc0 b21f084
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Sat Feb 3 17:31:30 2024 +0000
+
+        Merge pull request #1 from njr0/pytest
+
+        Working with pytest
+
+    commit e725da17fd07b7015251dc4e2607e9031e28f661
+    Merge: 8173ea4 562882f
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Sat Feb 3 17:32:45 2024 +0000
+
+        Merge branch 'main' of github.com:njr0/csvw2pd
+
+    commit 4852a0acd1d2dfcd105a75e4bb4c173f2aca00f3
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Sat Feb 3 17:48:15 2024 +0000
+
+        Add missing test (result) file.
+
+    commit 803142996f207ee0d4c315e4dce7d7796c14ab8b
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Sun Feb 4 15:14:55 2024 +0000
+
+        Moved CSVW reading into CSVWMetadata class.
+
+        This subclasses CSVMetadata and stores CSVW-specifi
+        information in various _prefixed attributes.
+
+        There's probably too much stuff allowed in CSVW to read/check it all,
+        but it is now reading the @context and @url, which are both mandatory
+        in CSVW (though it is supposed to be relative to the CSVW -metadata.json
+        file) and there is some suggestion it might be permitted to be null.
+
+
+    commit 30e0ad6f46dc95bf958b81d515d2aee5922534dc
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Sun Feb 4 19:27:14 2024 +0000
+
+        Read more properties from CSVW
+
+    commit 6499df06d2151da398e4d73212022d748d4a2842
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Mon Feb 5 11:38:24 2024 +0000
+
+        Renamed from csvw2pd to csvmetadata.
+
+        Also moved everything down a level (as will be needed for release)
+        and renamed csvmetadata.py to base.py and csvw2pd.py to cli.py.
+
+        Will add command line tools before too long.
+
+    commit 16027647bb2755a3df7a31b004582cb6bded7f65
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Mon Feb 5 11:57:49 2024 +0000
+
+        Add pyproject.toml and __init__.py
+
+    commit dd1b945aae798f72f6df2d92467c31673bf1f3e6
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Tue Feb 6 08:35:32 2024 +0000
+
+        Refactor
+
+    commit eec40aa48459eb22f9f2b03d40deb130c8d631e5
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Tue Feb 6 08:43:22 2024 +0000
+
+        Change fields from dictionary to list.
+
+    commit a6e4071a3117a7d600fbaef9f02fd359f4bc7db7
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Mon Feb 19 17:50:22 2024 +0000
+
+        Checkpoint.
+
+        Various changes for use by tdda library etc.
+        (only partly used so far). This is mainly
+        in the area of trying to find and identify
+        metadata files.
+
+        Have also broken some functionality into new files.
+
+    commit 86a7f7eac2edf5424e02eacbd59c073a3ce74d29
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Fri Feb 23 22:30:58 2024 +0000
+
+        Add csv2pandas
+
+        ...and add a single test for this (for now)
+        and fix a bunch of things to make this all work.
+
+    commit 8167b3c1e300598e6db013548680039de064237e
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Mon Feb 26 08:46:15 2024 +0000
+
+        Add test files (unused)
+
+    commit d08654fb4d20c4a56be06d2c93e847d8af77c484
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Mon Feb 26 08:48:44 2024 +0000
+
+        Add dev dir with utils
+
+    commit 0d78a5be8bb7879427efdfac487267f82608367e
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Mon Feb 26 19:30:25 2024 +0000
+
+        Add some tests for encodings
+
+    commit 8d70e9cf5f39b6303adf5cc8cc72e14954b1c8ee
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Fri Mar 1 22:42:56 2024 +0000
+
+        Lots more tests and some code fixes
+
+    commit 47c481d146e40c9048a31a80c4db910c3bee0859
+    Author: Nick Radcliffe <njr@StochasticSolutions.com>
+    Date:   Sat Mar 2 08:22:55 2024 +0000
+
+        Add missing test files
+
+Change ...pd.constraints.py to use tdda.serial
+
+... rather than csvmetadata and fix a few problems pyflakes found.
+
+--------------------- end of serial metdata branch -----------------------
+
 """
```

### Comparing `tdda-2.0.9/tdda/__init__.py` & `tdda-2.1.2/tdda/__init__.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/base.py` & `tdda-2.1.2/tdda/constraints/base.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/baseconstraints.py` & `tdda-2.1.2/tdda/constraints/baseconstraints.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/console.py` & `tdda-2.1.2/tdda/constraints/console.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/db/constraints.py` & `tdda-2.1.2/tdda/constraints/db/constraints.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/db/detect.py` & `tdda-2.1.2/tdda/constraints/db/detect.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/db/discover.py` & `tdda-2.1.2/tdda/constraints/db/discover.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/db/drivers.py` & `tdda-2.1.2/tdda/constraints/db/drivers.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/db/extension.py` & `tdda-2.1.2/tdda/constraints/db/extension.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/db/testdbconstraints.py` & `tdda-2.1.2/tdda/constraints/db/testdbconstraints.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/db/verify.py` & `tdda-2.1.2/tdda/constraints/db/verify.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/examples/README.md` & `tdda-2.1.2/tdda/constraints/examples/README.md`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/examples/accounts25k.tdda` & `tdda-2.1.2/tdda/constraints/examples/accounts25k.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/examples/elements118.tdda` & `tdda-2.1.2/tdda/constraints/examples/elements118.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/examples/files_extension.py` & `tdda-2.1.2/tdda/constraints/examples/files_extension.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/examples/simple_discovery.py` & `tdda-2.1.2/tdda/constraints/examples/simple_discovery.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/examples/simple_verification.py` & `tdda-2.1.2/tdda/constraints/examples/simple_verification.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/examples/testdata/accounts.zip` & `tdda-2.1.2/tdda/constraints/examples/testdata/accounts.zip`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/examples/testdata/accounts1k.tdda` & `tdda-2.1.2/tdda/constraints/examples/testdata/accounts1k.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/examples/testdata/ddd.csv` & `tdda-2.1.2/tdda/constraints/examples/testdata/ddd.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/examples/testdata/ddd.tdda` & `tdda-2.1.2/tdda/constraints/examples/testdata/ddd.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/examples/testdata/elements118.csv` & `tdda-2.1.2/tdda/constraints/examples/testdata/elements118.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/examples/testdata/elements118.feather` & `tdda-2.1.2/tdda/constraints/examples/testdata/elements118.feather`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/examples/testdata/elements118.pmm` & `tdda-2.1.2/tdda/constraints/examples/testdata/elements118.pmm`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/examples/testdata/elements92.csv` & `tdda-2.1.2/tdda/constraints/examples/testdata/elements92.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/examples/testdata/elements92.tdda` & `tdda-2.1.2/tdda/constraints/examples/testdata/elements92.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/extension.py` & `tdda-2.1.2/tdda/constraints/extension.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/flags.py` & `tdda-2.1.2/tdda/constraints/flags.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/pd/constraints.py` & `tdda-2.1.2/tdda/constraints/pd/constraints.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,21 @@
     unicode_string, byte_string, long_type
 )
 
 from tdda.referencetest.checkpandas import (default_csv_loader,
                                             default_csv_writer)
 from tdda import rexpy
 
+from tdda.serial.reader import load_metadata
+from tdda.serial.utils import (
+    find_associated_metadata_file,
+    find_metadata_type_from_path
+)
+from tdda.serial.pandasio import to_pandas_read_csv_args
+
 # pd.tslib is deprecated in newer versions of Pandas
 if hasattr(pd, 'Timestamp'):
     pandas_Timestamp = pd.Timestamp
 else:
     pandas_Timestamp = pd.tslib.Timestamp
 
 isPy3 = sys.version_info[0] >= 3
@@ -328,14 +335,18 @@
                                rownumber_is_index=True,
                                boolean_ints=False,
                                interleave=False,
                                **kwargs):
         if self.out_df is None:
             return None
         orig_fields = list(self.df)
+        output_is_typed = (
+            detect_outpath
+            and file_format(detect_outpath) in ('parquet', 'feather')
+        )
         output_is_feather = (detect_outpath
                              and file_format(detect_outpath) == 'feather')
 
         out_df = self.out_df
         add_index = detect_index or detect_output_fields is None
         if detect_output_fields is None:
             detect_output_fields = []
@@ -369,35 +380,36 @@
         if interleave:
             out_df = self.interleave(out_df, orig_fields, nfailname)
 #             if detect_in_place:  # does not work in place
 #                 self.interleave(self.df, orig_fields, nfailname)
 
         if detect_outpath:
             index_is_trivial = is_pd_index_trivial(out_df)
-            if output_is_feather:
+            if output_is_typed:
                 df_to_save = out_df
             else:
                 df_to_save = convert_output_types(out_df, boolean_ints)
             if add_index:
                 # Add Index or RowNumber columns to output CSV file (or
                 # add appropriate columns to output feather file and reset
                 # its index, because feather doesn't support MultiIndexes
                 # and doesn't retain single indexes).
                 #
                 # TODO: If the feather file is going to be saved using
                 #       pmmif's featherpmm, and if featherpmm were able to
                 #       transparently retain indexes, then we wouldn't need
                 #       to do that in this case (when featherpmm is set, and
-                #       output_is_feather).
+                #       output_is_typed).
                 indexes = []
                 if output_is_feather or rownumber_is_index:
                     stem = 'Index' if rownumber_is_index else 'RowNumber'
                     if isinstance(df_to_save.index, pd.MultiIndex):
                         for i, level in enumerate(df_to_save.index.levels):
-                            name = (df.index.names[i] if df.index.names
+                            name = (df_to_save.index.names[i]
+                                    if df_to_save.index.names
                                     else '%s_%d' % (stem, (i+1)))
                             pair = (unique_column_name(df_to_save, name),
                                     df_to_save.index.get_level_values(i))
                             indexes.append(pair)
                     else:
                         indexes.append((unique_column_name(df_to_save, stem),
                                         df_to_save.index))
@@ -473,15 +485,17 @@
                                     is_real = True
                             else:
                                 is_numeric = False
                                 break
                     if is_numeric:
                         if is_real:
                             is_real = self.calc_non_integer_values_count(c) > 0
-                        self.df.loc[ser.notnull(), c] = ser.astype(str)
+                        self.df[c] = np.where(ser.notnull(),
+                                              ser.astype(str),
+                                              np.nan)
                         if not is_real:
                             self.df[c] = self.df[c].str.replace('.0', '',
                                                                 regex=False)
                 elif ctype == 'bool' and str(dtype).lower().startswith('int'):
                     self.df[c] = ser.astype(bool)
             except Exception as e:
                 print('%s: %s' % (e.__class__.__name__, str(e)))
@@ -864,15 +878,16 @@
                             ``bool`` constraint only if::
 
                                 c.dropnulls().astype(bool) == c.dropnulls()
 
         *outpath*:
                             This specifies that the verification process
                             should detect records that violate any constraints,
-                            and write them out to this CSV (or feather) file.
+                            and write them out to this CSV, parquet
+                            or feather file.
 
                             By default, only failing records are written out
                             to file, but this can be overridden with the
                             ``write_all`` parameter.
 
                             By default, the columns in the detection output
                             file will be a boolean ``ok`` field for each
@@ -1111,38 +1126,108 @@
     return constraints
 
 
 def file_format(path):
     if isinstance(path, StringIO):
         return 'csv'
     else:
-        parts = os.path.splitext(path)
-        return ('feather' if len(parts) > 1 and parts[1] == '.feather'
-                          else 'csv')
+        (stem, ext) = os.path.splitext(path)
+        return ext[1:] if ext else 'csv'
 
 
-def load_df(path):
-    if file_format(path) != 'feather':
+def load_df(path, mdpath=None, ignore_apparent_metadata=False,
+            infer_metadata=True):
+    """
+    Loads a pandas DataFrame from a path or stream.
+
+    Args:
+        path is usually a file path to be read, but can be a stream
+
+        mdpath is an optional path to an associated metadata file to use
+
+        ignore_apparent_metadata  Ordinarily, if a CSV file is provided
+                                  as path, and there is "next to it"
+                                  a file that looks likes a metadata file
+                                  (same stem name with an extension fitting
+                                  a recommended pattern for csvw, csvmetadata
+                                  or frictionless), that metadata will be read
+                                   and used.
+                                  Setting this to True prevents that.
+
+        infer_metadata  If a CSV file ('.csv', '.psv', '.tsv' or '.txt' file)
+                        is given and no metadata file is provided, this
+                        function will ordinarily try to infer the file
+                        format using the csvmetadata library.
+                        Setting this to False overrides that behaviour,
+                        forcing the default Pandas CSV reader to be used
+                        with few TDDA's default arguments for it.
+    """
+    if isinstance(path, StringIO):  # stream
         return default_csv_loader(path)
-    elif featherpmm and feather:
-        ds = featherpmm.read_dataframe(path)
-        return ds.df
-    elif feather:
-        return feather.read_dataframe(path)
-    else:
-        raise Exception('The Python feather module is not installed.\n'
-                        'Use:\n    pip install feather-format\n'
-                        'to add capability.\n')
+    exists = os.path.exists(os.path.expanduser(path))
+    stem, ext = os.path.splitext(path)
+    lcstem, ext = stem.lower(), ext.lower()
+
+    if ext == '.parquet':
+        return pd.read_parquet(path)
+    elif ext == '.feather':
+        if featherpmm and feather:
+            ds = featherpmm.read_dataframe(path)
+            return ds.df
+        elif feather:
+            return feather.read_dataframe(path)
+        else:
+            raise Exception('The Python feather module is not installed.\n'
+                            'Use:\n    pip install feather-format\n'
+                            'to add capability.\n')
+
+    if mdpath is None:
+        md_type, _ = find_metadata_type_from_path(path)
+        if md_type:
+            # path is a metadata file of a known type
+            # load the metadata from it and get the file path, if any
+            # from the metadata file
+            metadata = load_metadata(path)
+            if metadata and metadata.path:
+                print('** Using metadata %s.  '
+                      'Use --no-csv-metadata to override.' % path,
+                      file=sys.stderr)
+                kw = to_pandas_read_csv_args(metadata)
+                return default_csv_loader(metadata.path, **kw)
+
+        if not ignore_apparent_metadata:
+            # no explicit metadata path provided
+            mdpath = find_associated_metadata_file(path)
+            if mdpath:
+                metadata = load_metadata(path)
+                kw = to_pandas_read_csv_args(metadata)
+                return default_csv_loader(path, **kw)
+            elif infer_metadata:
+                # infer metadata
+                pass
+        # Told not to look for apparent metadata or infer metadata
+        return default_csv_loader(path)
+
+    else:  # explicit metadatapath provided
+        metadata = load_metadata(path)
+        kw = to_pandas_read_csv_args(metadata)
+        return default_csv_loader(path, **kw)
 
 
 def save_df(df, path, index=False):
     if path == '-' or path is None:
         print(default_csv_writer(df, None, index=index))
-    elif file_format(path) != 'feather':
+    else:
+        fmt = file_format(path)
+    if fmt == 'parquet':
+        df.to_parquet(path=path, index=False)
+    elif fmt in ('csv', 'psv', 'tsv', 'txt'):
         default_csv_writer(df, path, index=index)
+    elif fmt != 'feather':
+        raise Exception(f'Unknown output format: {fmt}')
     elif featherpmm and feather:
         featherpmm.write_dataframe(featherpmm.Dataset(df, name='verification'),
                                    path)
     elif feather:
         feather.write_dataframe(df, path)
     else:
         raise Exception('The Python feather module is not installed.\n'
```

### Comparing `tdda-2.0.9/tdda/constraints/pd/detect.py` & `tdda-2.1.2/tdda/constraints/pd/detect.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,22 +10,24 @@
 USAGE = '''
 
 Parameters:
 
   * input is one of:
 
       - a csv file
-      - a feather file containing a Pandas or R DataFrame
+      - a .parquet file
+      - a feather file containing a Pandas or R DataFrame (deprecated(
       - any of the other supported data sources
 
   * constraints.tdda, if provided, is a JSON .tdda file constaining
     constraints.
 
-  * name of output file (.csv or .feather) where detection results
-    are to be written. Can be - (or missing) to write to standard output.
+  * name of output file (.csv,  .parqet or .feather (deprecated))
+    where detection results are to be written.
+    Can be - (or missing) to write to standard output.
 
 '''
 
 import os
 import sys
 
 try:
@@ -50,35 +52,34 @@
 from tdda.constraints.pd.constraints import detect_df, load_df, file_format
 
 
 def detect_df_from_file(df_path, constraints_path, outpath,
                         verbose=True, **kwargs):
     if df_path == '-' or df_path is None:
         df_path = StringIO(sys.stdin.read())
-    if constraints_path is None:
-        if not isinstance(df_path, StringIO):
-            split = os.path.splitext(df_path)
-            if split[1] in ('.csv', '.feather'):
-                constraints_path = split[0] + '.tdda'
         if constraints_path is None:
             print('No constraints file specified.', file=sys.stderr)
             sys.exit(1)
+    elif constraints_path is None:
+        (stem, ext) = os.path.splitext(df_path)
+        constraints_path = stem + '.tdda'
 
-    df = load_df(df_path)
     from_feather = file_format(df_path) == 'feather'
+
+    df = load_df(df_path)
     v = detect_df(df, constraints_path, outpath=outpath,
                   rownumber_is_index=from_feather, **kwargs)
     if verbose and outpath is not None and outpath != '-':
         print(v)
     return v
 
 
 def pd_detect_parser():
     parser = detect_parser(USAGE)
-    parser.add_argument('input', help='CSV or feather file')
+    parser.add_argument('input', help='CSV, parquet or feather file')
     parser.add_argument('constraints', nargs='?',
                         help='constraints file to verify against')
     parser.add_argument('outpath', nargs='?',
                         help='file to write detection results to')
     return parser
```

### Comparing `tdda-2.0.9/tdda/constraints/pd/discover.py` & `tdda-2.1.2/tdda/constraints/pd/discover.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 USAGE = '''
 
 Parameters:
 
   * input is one of:
 
     - a csv file
-    - a .feather file containing a saved Pandas or R DataFrame
+    - a .parquet file
+    - a .feather file containing a saved Pandas or R DataFrame (deprecated)
     - any of the other supported data sources
 
   * constraints.tdda, if provided, specifies the name of a file to
     which the generated constraints will be written.  Can be - (or missing)
     to write to standard output.
 
 '''
@@ -63,15 +64,16 @@
     elif verbose or constraints_path == '-':
         print(output)
     return output
 
 
 def pd_discover_parser():
     parser = discover_parser(USAGE)
-    parser.add_argument('input', nargs=1, help='CSV or feather file')
+    parser.add_argument('input', nargs=1,
+                        help='CSV, parquet (or feather, deprecated) file')
     parser.add_argument('constraints', nargs='?',
                         help='name of constraints file to create')
     return parser
 
 
 def pd_discover_params(args):
     parser = pd_discover_parser()
```

### Comparing `tdda-2.0.9/tdda/constraints/pd/extension.py` & `tdda-2.1.2/tdda/constraints/pd/extension.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """
 Extensions to the ``tdda`` command line tool, to support Pandas dataframes
 and CSV files.
 """
 
+import os
 import sys
 
 from tdda.constraints.extension import ExtensionBase
 
 from tdda.constraints.pd.discover import PandasDiscoverer
 from tdda.constraints.pd.verify import PandasVerifier
 from tdda.constraints.pd.detect import PandasDetector
@@ -16,15 +17,19 @@
 
 class TDDAPandasExtension(ExtensionBase):
     def __init__(self, argv, verbose=False):
         ExtensionBase.__init__(self, argv, verbose=verbose)
 
     def applicable(self):
         for a in self.argv:
-            if a.endswith('.csv') or a.endswith('.feather') or a == '-':
+            if a == '-':
+                return True
+            (stem, ext) = os.path.splitext(a)
+            if (ext in ('.csv', '.psv', '.tsv', '.parquet', '.feather'
+                        '.json', '.yaml')):
                 return True
         return False
 
     def help(self, stream=sys.stdout):
         print('  - Flat files (filename.csv)', file=stream)
         print('  - Pandas DataFrames (filename.feather)', file=stream)
```

### Comparing `tdda-2.0.9/tdda/constraints/pd/testpdconstraints.py` & `tdda-2.1.2/tdda/constraints/pd/testpdconstraints.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 Test Suite
 """
 
 import datetime
 import json
 import math
 import os
+import re
 import time
 import shutil
 import subprocess
 import sys
 import tempfile
 import unittest
 
-from collections import OrderedDict
+from collections import OrderedDict, namedtuple
 from distutils.spawn import find_executable
 
 import pandas as pd
 import numpy as np
 
 try:
     import pmmif
@@ -55,17 +56,24 @@
 from tdda.constraints.pd import constraints as pdc
 from tdda.constraints.pd.constraints import (load_df, verify_df,
                                              discover_df, detect_df)
 from tdda.constraints.pd.discover import discover_df_from_file
 from tdda.constraints.pd.verify import verify_df_from_file#, detect_df_from_file
 from tdda.constraints.pd.detect import detect_df_from_file
 
+
 from tdda.examples import copy_accounts_data_unzipped
 
 from tdda.referencetest import ReferenceTestCase, tag
+from tdda.referencetest.pddates import (
+    infer_date_format,
+    DateRE,
+    Separators,
+    get_date_separators
+)
 
 isPython2 = sys.version_info[0] < 3
 
 THIS_DIR = os.path.dirname(os.path.abspath(__file__))
 TESTDATA_DIR = os.path.join(os.path.dirname(THIS_DIR), 'testdata')
 
 
@@ -1375,15 +1383,14 @@
         self.assertStringCorrect(ddf2.to_string(), 'detect_dups.df')
 
 
 class TestPandasMultipleConstraintGeneration(ReferenceTestCase):
     def testConstraintGenerationNoRex(self):
         self.constraintsGenerationTest(inc_rex=False)
 
-    @tag
     def testConstraintGenerationWithRex(self):
         self.constraintsGenerationTest(inc_rex=True)
 
     def constraintsGenerationTest(self, inc_rex=False):
         csv_path = os.path.join(TESTDATA_DIR, 'elements92.csv')
         df = pd.read_csv(csv_path)
         if inc_rex:
@@ -1652,14 +1659,156 @@
                      'a_b_min_ok',
                      'a_b_min_ok_68',
                      'a_min_ok68',
                      'a_transform_ok'):
             self.assertFalse(pdc.is_ver_field(name, 'a'))
 
 
+class TestUtilityFunctions(ReferenceTestCase):
+
+    @tag
+    def testDateInferrer(self):
+        df = pd.DataFrame({
+            'isod': ['2024-01-01', None, '2024-01-20', None],
+            'isodt': ['2024-01-01T12:34:56', None, '2024-01-20T21:22:23', None],
+            'eurod': ['01-01-2024', None, '20-01-2024', None],
+            'eurodt': ['01-01-2024:12:34:56', None, '20-01-2024:21:22:23',
+                       None],
+            'usd': ['01-01-2024', None, '01-20-2024', None],
+            'usdt': ['01-01-2024:12:34:56', None, '01-20-2024:21:22:23',
+                     None],
+            'nodate': ['foo', None, 'bar', None]
+        })
+        expected_fmt = {
+            'isod': '%Y-%m-%d',
+            'isodt': 'ISO8601',
+            'eurod': '%d-%m-%Y',
+            'eurodt': '%d-%m-%Y:%H:%M:%S',
+            'usd': '%m-%d-%Y',
+            'usdt': '%m-%d-%Y:%H:%M:%S',
+            'nodate': None
+        }
+
+        dtdt = datetime.datetime
+        date_col = [dtdt(2024, 1, 1), None, dtdt(2024, 1, 20), None]
+        dt_col = [dtdt(2024, 1, 1, 12, 34, 56), None,
+                  dtdt(2024, 1, 20, 21, 22, 23), None]
+
+        expected_df = pd.DataFrame({
+            'isod': date_col,
+            'isodt': dt_col,
+            'eurod': date_col,
+            'eurodt': dt_col,
+            'usd': date_col,
+            'usdt': dt_col,
+            'nodate': df['nodate'],
+        })
+
+        for k in df:
+            f = infer_date_format(df[k])
+            if f is None:
+                self.assertIs(f, expected_fmt[k])
+            else:
+                self.assertEqual((k, f), (k, expected_fmt[k]))
+                c = pd.to_datetime(df[k], format=f)
+                same = (c.dropna() == expected_df[k].dropna()).sum()
+                if same != 2:
+                    print(k)
+                    print(c.dropna())
+                    print(expected_df[k].dropna())
+                    print()
+                self.assertEqual(same, 2)
+                self.assertEqual(c.dtype, expected_df[k].dtype)
+
+    def testDateRE(self):
+        R = DateRE
+        dates = {
+            '2024-01-20': R.ISO_DATEISH,
+            '2024/01/20': R.ISO_DATEISH,
+
+            '2024-01-20T12:34:56': R.ISO_DATETIMEISH,
+            '2024-01-20 12:34:56.12345': R.ISO_DATETIMEISH,
+            '2024/01/20T12:34:56': R.ISO_DATETIMEISH,
+            '2024/01/20 12:34:56.12345': R.ISO_DATETIMEISH,
+
+
+            '20-01-2024': R.DATEISH4Y,
+            '20/01/2024': R.DATEISH4Y,
+
+            '01-20-2024': R.DATEISH4Y,
+            '01/20/2024': R.DATEISH4Y,
+
+            '20-01-2024': R.DATEISH4Y,
+            '20/01/2024': R.DATEISH4Y,
+
+            '01-20-2024': R.DATEISH4Y,
+            '01/20/2024': R.DATEISH4Y,
+
+            '20-01-2024T12:34:56': R.DATEISH4Y,
+            '20-01-2024T12:34:56.123456': R.DATEISH4Y,
+
+
+            '20-01-24': R.DATEISH2Y,
+            '20/01/24': R.DATEISH2Y,
+
+            '01-20-24': R.DATEISH2Y,
+            '01/20/24': R.DATEISH2Y,
+
+            '20-01-24': R.DATEISH2Y,
+            '20/01/24': R.DATEISH2Y,
+
+            '01-20-24': R.DATEISH2Y,
+            '01/20/24': R.DATEISH2Y,
+
+            '20-01-24T12:34:56': R.DATEISH2Y,
+            '20-01-24T12:34:56.123456': R.DATEISH2Y,
+
+        }
+
+        for k, r in dates.items():
+            m = re.match(r, k)
+            if not m:
+                print(f'Failing: {k} {r.pattern}')
+            self.assertIsNotNone(m)
+
+            m = re.match(R.DATEISH, k)
+            if not m:
+                print(f'Failing: {k} (not DATEISH)')
+            self.assertIsNotNone(m)
+
+        sep_dates = {
+            '20-01-2024': (
+                R.SEPS4Y,
+                Separators('-', None, None, False, False, '')
+            ),
+            '20-01-2024T12:34:56': (
+                R.SEPS4Y,
+                Separators('-', 'T', ':', True, False, 'T%H:%M:%S')
+            ),
+
+            '20-01-2024T12:34:56.123': (
+                R.SEPS4Y,
+                Separators('-', 'T', ':', True, True, 'T%H:%M:%S.%f')
+            ),
+            '20/01/2024 12.34.56.123': (
+                R.SEPS4Y,
+                Separators('/', ' ', '.', True, True, ' %H.%M.%S.%f')
+            ),
+        }
+        for k, (r, expected) in sep_dates.items():
+            actual = get_date_separators(r, k)
+            if actual != expected:
+                print('-->   actual', actual)
+                print('--> expected', expected)
+                print()
+            self.assertEqual(actual, expected)
+
+
+
+
 TestPandasMultipleConstraintVerifier.set_default_data_location(TESTDATA_DIR)
 TestPandasMultipleConstraintDetector.set_default_data_location(TESTDATA_DIR)
 TestPandasCommandLine.set_default_data_location(TESTDATA_DIR)
 TestPandasCommandAPI.set_default_data_location(TESTDATA_DIR)
 
 
 def rmdirs(parent, dirs):
```

### Comparing `tdda-2.0.9/tdda/constraints/pd/verify.py` & `tdda-2.1.2/tdda/constraints/pd/verify.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 USAGE = '''
 
 Parameters:
 
   * input is one of:
 
       - a csv file. Can be - to read from standard input.
-      - a feather file containing a Pandas or R DataFrame.
+      - a parquet file
+      - a feather file containing a Pandas or R DataFrame (deprecated).
       - any of the other supported data sources
 
   * constraints.tdda, if provided, is a JSON .tdda file constaining
     constraints.
 
 If no constraints file is provided, a file with the same path as the
 input file, with a .tdda extension will be tried.
@@ -49,33 +50,31 @@
 from tdda.constraints.flags import verify_parser, verify_flags
 from tdda.constraints.pd.constraints import verify_df, load_df
 
 
 def verify_df_from_file(df_path, constraints_path, verbose=True, **kwargs):
     if df_path == '-' or df_path is None:
         df_path = StringIO(sys.stdin.read())
-    if constraints_path is None:
-        if not isinstance(df_path, StringIO):
-            split = os.path.splitext(df_path)
-            if split[1] in ('.csv', '.feather'):
-                constraints_path = split[0] + '.tdda'
         if constraints_path is None:
             print('No constraints file specified.', file=sys.stderr)
             sys.exit(1)
+    if constraints_path is None:
+        stem, ext = os.path.splitext(df_path)
+        constraints_path = stem + '.tdda'
 
     df = load_df(df_path)
     v = verify_df(df, constraints_path, **kwargs)
     if verbose:
         print(v)
     return v
 
 
 def pd_verify_parser():
     parser = verify_parser(USAGE)
-    parser.add_argument('input', nargs=1, help='CSV or feather file')
+    parser.add_argument('input', nargs=1, help='CSV, parquet, or feather file')
     parser.add_argument('constraints', nargs='?',
                         help='constraints file to verify against')
     return parser
 
 
 def pd_verify_params(args):
     parser = pd_verify_parser()
```

### Comparing `tdda-2.0.9/tdda/constraints/tdda_json_file_format.md` & `tdda-2.1.2/tdda/constraints/tdda_json_file_format.md`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testbase.py` & `tdda-2.1.2/tdda/constraints/testbase.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testconstraints.py` & `tdda-2.1.2/tdda/constraints/testconstraints.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/ddd.csv` & `tdda-2.1.2/tdda/constraints/testdata/d.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/ddd.tdda` & `tdda-2.1.2/tdda/constraints/testdata/ddd.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/detect-els-cmdline-interleaved.csv` & `tdda-2.1.2/tdda/constraints/testdata/detect-els-cmdline-interleaved.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/detect-els-cmdline.csv` & `tdda-2.1.2/tdda/constraints/testdata/detect-els-cmdline.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/detect-els-cmdline2.csv` & `tdda-2.1.2/tdda/constraints/testdata/detect-els-cmdline2.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/elements118.csv` & `tdda-2.1.2/tdda/constraints/testdata/elements118.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/elements118.df` & `tdda-2.1.2/tdda/constraints/testdata/elements118.df`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/elements118.feather` & `tdda-2.1.2/tdda/constraints/testdata/elements118.feather`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/elements118.pmm` & `tdda-2.1.2/tdda/constraints/testdata/elements118.pmm`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/elements118.tdda` & `tdda-2.1.2/tdda/constraints/testdata/elements118.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/elements118_detect_from_csv.csv` & `tdda-2.1.2/tdda/constraints/testdata/elements118_detect_from_csv.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/elements118_detect_from_feather.csv` & `tdda-2.1.2/tdda/constraints/testdata/elements118_detect_from_feather.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/elements118_detect_from_feather.feather` & `tdda-2.1.2/tdda/constraints/testdata/elements118_detect_from_feather.feather`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/elements118oldrex-3.tdda` & `tdda-2.1.2/tdda/constraints/testdata/elements118oldrex-3.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/elements118oldrex.tdda` & `tdda-2.1.2/tdda/constraints/testdata/elements118oldrex.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/elements118rex-3.tdda` & `tdda-2.1.2/tdda/constraints/testdata/elements118rex-3.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/elements118rex.df` & `tdda-2.1.2/tdda/constraints/testdata/elements118rex.df`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/elements118rex.tdda` & `tdda-2.1.2/tdda/constraints/testdata/elements118rex.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/elements118rex_detect.df` & `tdda-2.1.2/tdda/constraints/testdata/elements118rex_detect.df`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/elements118rex_detect_perc.csv` & `tdda-2.1.2/tdda/constraints/testdata/elements118rex_detect_perc.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/elements92.csv` & `tdda-2.1.2/tdda/constraints/testdata/elements92.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/elements92.tdda` & `tdda-2.1.2/tdda/constraints/testdata/elements92.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/elements92_pandas.tdda` & `tdda-2.1.2/tdda/constraints/testdata/elements92_pandas.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/elements92oldrex.tdda` & `tdda-2.1.2/tdda/constraints/testdata/elements92oldrex.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/elements92rex.tdda` & `tdda-2.1.2/tdda/constraints/testdata/elements92rex.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/example.csv` & `tdda-2.1.2/tdda/constraints/testdata/example.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/example.db` & `tdda-2.1.2/tdda/constraints/testdata/example.db`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/example.sql` & `tdda-2.1.2/tdda/constraints/testdata/example.sql`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/ref-accounts1k.tdda` & `tdda-2.1.2/tdda/constraints/testdata/ref-accounts1k.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/ref-accounts25k.tdda` & `tdda-2.1.2/tdda/constraints/testdata/ref-accounts25k.tdda`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/constraints/testdata/ref-detect25k-failures.txt` & `tdda-2.1.2/tdda/constraints/testdata/ref-detect25k-failures.txt`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/examples.py` & `tdda-2.1.2/tdda/examples.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/gentest/examples/README.md` & `tdda-2.1.2/tdda/gentest/examples/README.md`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/gentest/examples/r-examples/0-set-variables.R` & `tdda-2.1.2/tdda/gentest/examples/r-examples/0-set-variables.R`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/gentest/examples/r-examples/2-compute-cumulative-percentiles.R` & `tdda-2.1.2/tdda/gentest/examples/r-examples/2-compute-cumulative-percentiles.R`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/gentest/examples/r-examples/3-parametric-regression.R` & `tdda-2.1.2/tdda/gentest/examples/r-examples/3-parametric-regression.R`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/gentest/examples/r-examples/4-non-parametric-regression.R` & `tdda-2.1.2/tdda/gentest/examples/r-examples/4-non-parametric-regression.R`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/gentest/examples/r-examples/README.md` & `tdda-2.1.2/tdda/gentest/examples/r-examples/README.md`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/gentest/examples/r-examples/env.data.or.txt` & `tdda-2.1.2/tdda/gentest/examples/r-examples/env.data.or.txt`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/gentest/examples/r-examples/env.data.txt` & `tdda-2.1.2/tdda/gentest/examples/r-examples/env.data.txt`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/gentest/examples/r-examples/site.species.or.txt` & `tdda-2.1.2/tdda/gentest/examples/r-examples/site.species.or.txt`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/gentest/examples/r-examples/site.species.txt` & `tdda-2.1.2/tdda/gentest/examples/r-examples/site.species.txt`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/__init__.py` & `tdda-2.1.2/tdda/referencetest/__init__.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/basecomparison.py` & `tdda-2.1.2/tdda/referencetest/basecomparison.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/captureoutput.py` & `tdda-2.1.2/tdda/referencetest/captureoutput.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/checkfiles.py` & `tdda-2.1.2/tdda/referencetest/checkfiles.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/checkpandas.py` & `tdda-2.1.2/tdda/referencetest/checkpandas.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,22 +13,52 @@
 import csv
 import os
 import sys
 
 from collections import OrderedDict
 
 from tdda.referencetest.basecomparison import BaseComparison, Diffs
+from tdda.referencetest.pddates import infer_date_format
 
 try:
     import pandas as pd
     import numpy as np
 except ImportError:
     pd = None
 
 
+def loosen_type(t):
+    name = ''.join(c for c in t if not c.isdigit()).lower()
+    p = name.find('[')
+    name = name[:p] if p > -1 else name
+    return 'bool' if name == 'boolean' else name
+
+
+def types_match(t1, t2, level=None):
+    assert level is None or level in ('strict', 'medium', 'permissive')
+    if level is None or level == 'strict' or t1.name == t2.name:
+        return t1.name == t2.name
+
+    t1loose = loosen_type(t1.name)
+    t2loose = loosen_type(t2.name)
+    object_types = ('string', 'boolean', 'datetime', 'bool')
+    if (t1loose == t2loose
+            or t1loose == 'object' and t2loose in object_types
+            or t2loose == 'object' and t1loose in object_types):
+        return True
+
+    numeric_types = ('bool', 'boolean', 'int', 'float')
+    if (level == 'permissive'
+            and t1loose in numeric_types
+            and t2loose in numeric_types):
+        return True
+    return False
+
+
+
 class PandasNotImplemented(object):
     """
     Null implementation of PandasComparison, used when pandas not available.
     """
     def __getattr__(self, name):
         return lambda *args, **kwargs: self.method(name, *args, **kwargs)
 
@@ -45,30 +75,31 @@
         if pd is None:
             return PandasNotImplemented()
         return super(PandasComparison, cls).__new__(cls)
 
     def check_dataframe(self, df, ref_df, actual_path=None, expected_path=None,
                         check_data=None, check_types=None, check_order=None,
                         check_extra_cols=None, sortby=None,
-                        condition=None, precision=None, msgs=None):
+                        condition=None, precision=None, msgs=None,
+                        type_matching=None):
         """
         Compare two pandas dataframes.
 
             *df*
                             Actual dataframe
             *ref_df*
                             Expected dataframe
             *actual_path*
                             Path for file where actual dataframe originated,
                             used for error messages.
             *expected_path*
                             Path for file where expected dataframe originated,
                             used for error messages.
             *check_types*
-                            Option to specify fields to use to compare typees.
+                            Option to specify fields to use to compare types.
             *check_order*
                             Option to specify fields to use to compare field
                             order.
             *check_data*
                             Option to specify fields to use to compare cell
                             values.
             *check_extra_cols*
@@ -85,27 +116,29 @@
                             a vector of booleans (to specify which rows should
                             be compared).
             *precision*
                             Number of decimal places to compare float values.
             *msgs*
                             Optional Diffs object.
 
+            *type_matching* 'strict', 'medium', 'permissive'.
+                            None is same as strict.
+
         Returns a tuple (failures, msgs), containing the number of failures,
         and a Diffs object containing error messages.
 
         the comparison 'Option' flags can be of any of the following:
 
             - ``None`` (to apply that kind of comparison to all fields)
             - ``False`` (to skip that kind of comparison completely)
             - a list of field names
             - a function taking a dataframe as its single parameter, and
               returning a list of field names to use.
         """
-
-        same = True
+        type_matching = type_matching or 'strict'
         if msgs is None:
             msgs = Diffs()
 
         if precision is None:
             precision = 6
 
         check_types = resolve_option_flag(check_types, ref_df)
@@ -114,25 +147,24 @@
         missing_cols = []
         extra_cols = []
         wrong_types = []
         wrong_ordering = False
         for c in check_types:
             if c not in list(df):
                 missing_cols.append(c)
-            elif df[c].dtype != ref_df[c].dtype:
+            elif not(types_match(df[c].dtype, ref_df[c].dtype, type_matching)):
                 wrong_types.append((c, df[c].dtype, ref_df[c].dtype))
         if check_extra_cols:
-        # todo: shouldn't check_extra_cols be a boolean?
-        #       ... and set(check_extra_cols) be set(list(df))
             extra_cols = set(check_extra_cols) - set(list(ref_df))
         if check_order != False and not missing_cols:
             check_order = resolve_option_flag(check_order, ref_df)
             c1 = [c for c in list(df) if c in check_order]
             c2 = [c for c in list(ref_df) if c in check_order]
             wrong_ordering = (list(df[c1]) != list(ref_df[c2]))
+
         same = not any((missing_cols, extra_cols, wrong_types, wrong_ordering))
 
         if not same:
             self.failure(msgs, 'Column check failed.',
                          actual_path, expected_path)
             if missing_cols:
                 self.info(msgs, 'Missing columns: %s' % missing_cols)
@@ -164,62 +196,90 @@
                 df.sort_values(sortby, inplace=True)
                 ref_df.sort_values(sortby, inplace=True)
 
         if condition:
             df = df[condition(df)].reindex()
             ref_df = ref_df[condition(ref_df)].reindex()
 
-        same = len(df) == len(ref_df)
-        if not same:
+        same_len = (len(df) == len(ref_df))
+        if not same_len:
             self.failure(msgs, 'Length check failed.',
                          actual_path, expected_path)
             self.info(msgs, 'Found %d records, expected %d'
                             % (len(df), len(ref_df)))
-        else:
+            same = False
+        elif same:
             check_data = resolve_option_flag(check_data, ref_df)
             if check_data:
                 check_data = [c for c in check_data if c not in missing_cols]
                 df = df[check_data]
                 ref_df = ref_df[check_data]
                 if precision is not None:
                     rounded = df.round(precision).reset_index(drop=True)
                     ref_rounded = (ref_df.round(precision)
                                          .reset_index(drop=True))
                 else:
                     rounded = df
                     ref_rounded = ref_df
-                same = rounded.equals(ref_rounded)
-                if not same:
-                    self.failure(msgs, 'Contents check failed.',
-                                 actual_path, expected_path)
+                same_content = rounded.equals(ref_rounded)
+                if not same_content:
+                    failures = []
                     for c in list(ref_rounded):
                         if not rounded[c].equals(ref_rounded[c]):
                             diffs = self.differences(c, rounded[c],
-                                                     ref_rounded[c], precision)
-                            self.info(msgs, 'Column values differ: %s' % c)
-                            self.info(msgs, diffs)
+                                                     ref_rounded[c],
+                                                     precision)
+                            if diffs:
+                                failures.append('Column values differ: %s' % c)
+                                failures.append('%s\nvs.\n%s\n'
+                                                % (rounded[c],
+                                                   ref_rounded[c]))
+                    if failures:
+                        self.failure(msgs, 'Contents check failed.',
+                                     actual_path, expected_path)
+                        for f in failures:
+                            self.info(msgs, f)
+                        same = False
 
         same = same and not any((missing_cols, extra_cols, wrong_types,
                                  wrong_ordering))
         return (0 if same else 1, msgs)
 
     def differences(self, name, values, ref_values, precision):
         """
+        Args:
+            name        is the name of the columns
+            values      is the left-hand series
+            ref_values    is the rish-hand series
+            precision
+
         Returns a short summary of where values differ, for two columns.
         """
         for i, val in enumerate(values):
             refval = ref_values[i]
-            if val != refval and not (pd.isnull(val) and pd.isnull(refval)):
-                stop = self.ndifferences(values, ref_values, i)
-                summary_vals = self.sample_format(values, i, stop, precision)
-                summary_ref_vals = self.sample_format(ref_values, i, stop,
-                                                      precision)
-                return 'From row %d: [%s] != [%s]' % (i+1,
-                                                      summary_vals,
-                                                      summary_ref_vals)
+            valnull = values.isnull()
+            refnull = ref_values.isnull()
+            bothnull = valnull & refnull
+            n_both_null = bothnull.sum()
+            assert bothnull.sum() < len(values)  # Shouldn't have got here
+            (L, R) = (values, ref_values) if n_both_null == 0 else (
+                values[np.logical_not(bothnull)],
+                ref_values[np.logical_not(bothnull)]
+            )
+            same = L.eq(R)
+            L = L[np.logical_not(same)][:10]
+            R = R[np.logical_not(same)][:10]
+            summary_vals = sample_format2(L, precision)
+            summary_ref_vals = sample_format2(R, precision)
+            n = len(L)
+            if n == 0:
+                return ''
+            s = ('First 10 differences' if n > 10 else
+                 ('Difference%s' % ('s' if n > 1 else '')))
+            return '%s: [%s] != [%s]' % (s, summary_vals, summary_ref_vals)
         if values.dtype != ref_values.dtype:
             return 'Different types'
         else:
             return 'But mysteriously appear to be identical!'
 
     def sample(self, values, start, stop):
         return [None if pd.isnull(values[i]) else values[i]
@@ -401,50 +461,52 @@
         - quoting               is :py:const:`csv.QUOTE_MINIMAL`
         - escapechar            is ``\\`` (backslash)
         - na_values             are the empty string, ``"NaN"``, and ``"NULL"``
         - keep_default_na       is ``False``
     """
     options = {
         'index_col': None,
-        'infer_datetime_format': True,
         'quotechar': '"',
         'quoting': csv.QUOTE_MINIMAL,
         'escapechar': '\\',
         'na_values': ['', 'NaN', 'NULL'],
         'keep_default_na': False,
     }
     options.update(kwargs)
+    if 'infer_datetime_format' in options:  # don't let pandas do it.
+        del options['infer_datetime_format']
+    infer_datetimes = kwargs.get('infer_datetime_format', True)
 
     try:
         df = pd.read_csv(csvfile, **options)
     except pd.errors.ParserError:
         # Pandas CSV reader gets confused by stutter-quoted text that
         # also includes escapechars. So try again, with no escapechar.
         del options['escapechar']
         df = pd.read_csv(csvfile, **options)
 
-    # the reader won't have inferred any datetime columns (even though we
-    # told it to), because we didn't explicitly tell it the column names
-    # in advance. so.... we'll do it by hand (looking at string columns, and
-    # seeing if we can convert them safely to datetimes).
-    if options.get('infer_datetime_format'):
+    if infer_datetimes:  # We do it ourselves, now, instead of lettings
+                         # pandas do it.
         colnames = df.columns.tolist()
         for c in colnames:
             if df[c].dtype == np.dtype('O'):
-                try:
-                    datecol = pd.to_datetime(df[c])
-                    if datecol.dtype == np.dtype('datetime64[ns]'):
-                        df[c] = datecol
-                except Exception as e:
-                    pass
+                fmt = infer_date_format(df[c])
+                if fmt:
+                    try:
+                        datecol = pd.to_datetime(df[c], format=fmt)
+                        if datecol.dtype == np.dtype('datetime64[ns]'):
+                            df[c] = datecol
+                    except Exception as e:
+                        pass
         ndf = pd.DataFrame()
         for c in colnames:
             ndf[c] = df[c]
-
-    return ndf
+        return ndf
+    else:
+        return df
 
 
 def default_csv_writer(df, csvfile, **kwargs):
     """
     Default function for writing a csv file.
 
     Wrapper around the standard pandas pd.to_csv() function, but with
@@ -491,22 +553,26 @@
 
 def resolve_option_flag(flag, df):
     """
     Method to resolve an option flag, which may be any of:
 
        ``None`` or ``True``:
                 use all columns in the dataframe
-       ``None``:
+       ``False``:
                 use no columns
        list of columns
                 use these columns
        function returning a list of columns
     """
     if flag is None or flag is True:
         return list(df)
     elif flag is False:
         return []
     elif hasattr(flag, '__call__'):
          return flag(df)
     else:
         return flag
 
+
+def sample_format2(values, precision=None):
+    return (', '.join('%d: %s' % (values.index[i], values.iloc[i])
+            for i in range(min(len(values), 10))))
```

### Comparing `tdda-2.0.9/tdda/referencetest/diffrex.py` & `tdda-2.1.2/tdda/referencetest/diffrex.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/README.md` & `tdda-2.1.2/tdda/referencetest/examples/README.md`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/dataframes.py` & `tdda-2.1.2/tdda/referencetest/examples/dataframes.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/exercises-pytest/exercise1/expected.html` & `tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise1/expected.html`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/exercises-pytest/exercise1/generators.py` & `tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise1/generators.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/exercises-pytest/exercise2/expected.html` & `tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise2/expected.html`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/exercises-pytest/exercise2/generators.py` & `tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise2/generators.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/exercises-pytest/exercise2/test_all.py` & `tdda-2.1.2/tdda/referencetest/examples/exercises-pytest/exercise2/test_all.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/exercises-unittest/exercise1/expected.html` & `tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise1/expected.html`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/exercises-unittest/exercise1/generators.py` & `tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise1/generators.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/exercises-unittest/exercise1/test_all.py` & `tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise1/test_all.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/exercises-unittest/exercise2/expected.html` & `tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise2/expected.html`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/exercises-unittest/exercise2/generators.py` & `tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise2/generators.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/exercises-unittest/exercise2/test_all.py` & `tdda-2.1.2/tdda/referencetest/examples/exercises-unittest/exercise2/test_all.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/generators.py` & `tdda-2.1.2/tdda/referencetest/examples/generators.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/pytest/conftest.py` & `tdda-2.1.2/tdda/referencetest/examples/pytest/conftest.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/pytest/test_using_referencepytest.py` & `tdda-2.1.2/tdda/referencetest/examples/pytest/test_using_referencepytest.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/reference/dataframe_result.csv` & `tdda-2.1.2/tdda/referencetest/examples/reference/dataframe_result.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/reference/dataframe_result2.csv` & `tdda-2.1.2/tdda/referencetest/examples/reference/dataframe_result2.csv`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/reference/file_result.html` & `tdda-2.1.2/tdda/referencetest/examples/reference/file_result.html`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/reference/string_result.html` & `tdda-2.1.2/tdda/referencetest/examples/reference/string_result.html`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples/unittest/test_using_referencetestcase.py` & `tdda-2.1.2/tdda/referencetest/examples/unittest/test_using_referencetestcase.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/examples.py` & `tdda-2.1.2/tdda/referencetest/examples.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/gentest.py` & `tdda-2.1.2/tdda/referencetest/gentest.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/gentest_boilerplate.py` & `tdda-2.1.2/tdda/referencetest/gentest_boilerplate.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/pytestconfig.py` & `tdda-2.1.2/tdda/referencetest/pytestconfig.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/referencepytest.py` & `tdda-2.1.2/tdda/referencetest/referencepytest.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/referencetest.py` & `tdda-2.1.2/tdda/referencetest/referencetest.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,15 @@
         """
         self.reference_data_locations[kind] = os.path.normpath(location)
 
     def assertDataFramesEqual(self, df, ref_df,
                               actual_path=None, expected_path=None,
                               check_data=None, check_types=None,
                               check_order=None, condition=None, sortby=None,
-                              precision=None):
+                              precision=None, type_matching=None):
         """Check that an in-memory Pandas `DataFrame` matches an in-memory
         reference one.
 
             *df*:
                 Actual `DataFrame`.
 
             *ref_df*:
@@ -308,26 +308,29 @@
                 should be compared).
 
             *precision*:
                 (Optional) number of decimal places to use for
                 floating-point comparisons.  Default is not to perform
                 rounding.
 
+            *type_matching*  'strict', 'medium', 'permissive'
+
         Raises :py:class:`NotImplementedError` if Pandas is not available.
 
         """
         r = self.pandas.check_dataframe(df, ref_df,
                                         actual_path=actual_path,
                                         expected_path=expected_path,
                                         check_data=check_data,
                                         check_types=check_types,
                                         check_order=check_order,
                                         condition=condition,
                                         sortby=sortby,
-                                        precision=precision)
+                                        precision=precision,
+                                        type_matching=type_matching)
         (failures, msgs) = r
         self._check_failures(failures, msgs)
 
     def assertDataFrameCorrect(self, df, ref_csv, actual_path=None,
                                kind='csv', csv_read_fn=None,
                                check_data=None, check_types=None,
                                check_order=None, condition=None, sortby=None,
```

### Comparing `tdda-2.0.9/tdda/referencetest/referencetestcase.py` & `tdda-2.1.2/tdda/referencetest/referencetestcase.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/tests/testbase.py` & `tdda-2.1.2/tdda/referencetest/tests/testbase.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/tests/testdata/colours.txt` & `tdda-2.1.2/tdda/referencetest/tests/testdata/colours.txt`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/tests/testfiles.py` & `tdda-2.1.2/tdda/referencetest/tests/testfiles.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/tests/testregeneration.py` & `tdda-2.1.2/tdda/referencetest/tests/testregeneration.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/tests/teststrings.py` & `tdda-2.1.2/tdda/referencetest/tests/teststrings.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/referencetest/utils.py` & `tdda-2.1.2/tdda/referencetest/utils.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/rexpy/examples/agents9.txt` & `tdda-2.1.2/tdda/rexpy/examples/agents9.txt`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/rexpy/rexpy.py` & `tdda-2.1.2/tdda/rexpy/rexpy.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/rexpy/seq.py` & `tdda-2.1.2/tdda/rexpy/seq.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/rexpy/testhypo.py` & `tdda-2.1.2/tdda/rexpy/testhypo.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/rexpy/testrexpy.py` & `tdda-2.1.2/tdda/rexpy/testrexpy.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/rexpy/testseq.py` & `tdda-2.1.2/tdda/rexpy/testseq.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/testconfig.py` & `tdda-2.1.2/tdda/testconfig.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda/testtdda.py` & `tdda-2.1.2/tdda/testtdda.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import sys
 
 from tdda.referencetest import ReferenceTestCase
 
 from tdda.constraints.testconstraints import *
 from tdda.rexpy.testrexpy import *
 from tdda.referencetest.tests.alltests import *
+from tdda.serial.testserialmetadata import *
 
 # Set the enviroment variable TDDA_CONFIG_TESTS to something (e.g. 1)
 # to report on environment from within which tests are run
 TDDA_CONFIG_TESTS = 'TDDA_CONFIG_TESTS' in os.environ
 
 
 if TDDA_CONFIG_TESTS:
```

### Comparing `tdda-2.0.9/tdda/writabletestcase.py` & `tdda-2.1.2/tdda/writabletestcase.py`

 * *Files identical despite different names*

### Comparing `tdda-2.0.9/tdda.egg-info/PKG-INFO` & `tdda-2.1.2/tdda.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: tdda
-Version: 2.0.9
-Summary: Test Driven Data Analysis
+Version: 2.1.2
 Home-page: http://www.stochasticsolutions.com
 Download-URL: https://github.com/tdda/tdda
-Author: Stochastic Solutions Limited
-Author-email: info@StochasticSolutions.com
+Author: Simon Brown
+Author-email: Nick Radcliffe <njr@stochasticsolutions.com>
 License: MIT
 Keywords: tdda constraint referencetest rexpy
+Requires-Python: >=3.8
 License-File: LICENSE.txt
+Requires-Dist: numpy>=1.20.3
+Requires-Dist: pandas>=1.5.2
 
 Test-Driven Data Analysis (Python TDDA library)
 ===============================================
 
 What is it?
 -----------
 
@@ -120,9 +122,12 @@
   * General Notes on Constraints and Assertions: http://www.tdda.info/constraints-and-assertions
   * Notes on using the Pandas constraints library:
     http://www.tdda.info/constraint-discovery-and-verification-for-pandas-dataframes
   * PyCon UK Talk on TDDA:
       - Video: https://www.youtube.com/watch?v=FIw_7aUuY50
       - Slides and Rough Transcript:   http://www.tdda.info/slides-and-rough-transcript-of-tdda-talk-from-pycon-uk-2016
 
+  * <a rel="me" href="https://mathstodon.xyz/@tdda">Mastodon</a>
+
+
 All examples, tests and code run under Python 2.7, Python 3.5 and Python 3.6.
```

### Comparing `tdda-2.0.9/tdda.egg-info/SOURCES.txt` & `tdda-2.1.2/tdda.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -72,37 +72,40 @@
 tdda/constraints/pd/__init__.py
 tdda/constraints/pd/constraints.py
 tdda/constraints/pd/detect.py
 tdda/constraints/pd/discover.py
 tdda/constraints/pd/extension.py
 tdda/constraints/pd/testpdconstraints.py
 tdda/constraints/pd/verify.py
+tdda/constraints/testdata/d.csv
 tdda/constraints/testdata/ddd.csv
 tdda/constraints/testdata/ddd.tdda
 tdda/constraints/testdata/detect-els-cmdline-interleaved.csv
 tdda/constraints/testdata/detect-els-cmdline.csv
 tdda/constraints/testdata/detect-els-cmdline2.csv
 tdda/constraints/testdata/detect_dups.df
 tdda/constraints/testdata/elements118.csv
 tdda/constraints/testdata/elements118.df
 tdda/constraints/testdata/elements118.feather
+tdda/constraints/testdata/elements118.parquet
 tdda/constraints/testdata/elements118.pmm
 tdda/constraints/testdata/elements118.tdda
 tdda/constraints/testdata/elements118_detect_from_csv.csv
 tdda/constraints/testdata/elements118_detect_from_feather.csv
 tdda/constraints/testdata/elements118_detect_from_feather.feather
 tdda/constraints/testdata/elements118oldrex-3.tdda
 tdda/constraints/testdata/elements118oldrex.tdda
 tdda/constraints/testdata/elements118rex-3.tdda
 tdda/constraints/testdata/elements118rex.df
 tdda/constraints/testdata/elements118rex.tdda
 tdda/constraints/testdata/elements118rex_detect.csv
 tdda/constraints/testdata/elements118rex_detect.df
 tdda/constraints/testdata/elements118rex_detect_perc.csv
 tdda/constraints/testdata/elements92.csv
+tdda/constraints/testdata/elements92.parquet
 tdda/constraints/testdata/elements92.tdda
 tdda/constraints/testdata/elements92_pandas.tdda
 tdda/constraints/testdata/elements92oldrex.tdda
 tdda/constraints/testdata/elements92rex.tdda
 tdda/constraints/testdata/example.csv
 tdda/constraints/testdata/example.db
 tdda/constraints/testdata/example.sql
@@ -130,14 +133,15 @@
 tdda/referencetest/captureoutput.py
 tdda/referencetest/checkfiles.py
 tdda/referencetest/checkpandas.py
 tdda/referencetest/diffrex.py
 tdda/referencetest/examples.py
 tdda/referencetest/gentest.py
 tdda/referencetest/gentest_boilerplate.py
+tdda/referencetest/pddates.py
 tdda/referencetest/pytestconfig.py
 tdda/referencetest/referencepytest.py
 tdda/referencetest/referencetest.py
 tdda/referencetest/referencetestcase.py
 tdda/referencetest/utils.py
 tdda/referencetest/examples/README.md
 tdda/referencetest/examples/dataframes.py
@@ -169,24 +173,36 @@
 tdda/referencetest/tests/testfiles.py
 tdda/referencetest/tests/testpandas.py
 tdda/referencetest/tests/testregeneration.py
 tdda/referencetest/tests/teststrings.py
 tdda/referencetest/tests/testdata/colours.txt
 tdda/referencetest/tests/testdata/double.txt
 tdda/referencetest/tests/testdata/empty.txt
+tdda/referencetest/tests/testdata/frames_fail1.txt
+tdda/referencetest/tests/testdata/frames_fail2.txt
+tdda/referencetest/tests/testdata/frames_fail3.txt
 tdda/referencetest/tests/testdata/left.txt
 tdda/referencetest/tests/testdata/ref.txt
 tdda/referencetest/tests/testdata/removals.txt
 tdda/referencetest/tests/testdata/single.txt
 tdda/referencetest/tests/testdata/single2.txt
 tdda/rexpy/__init__.py
 tdda/rexpy/examples.py
+tdda/rexpy/quality.py
 tdda/rexpy/relib.py
 tdda/rexpy/rexpy.py
 tdda/rexpy/seq.py
 tdda/rexpy/testhypo.py
 tdda/rexpy/testrexpy.py
 tdda/rexpy/testseq.py
 tdda/rexpy/examples/agents9.txt
 tdda/rexpy/examples/headed-ids.txt
 tdda/rexpy/examples/ids.py
-tdda/rexpy/examples/pandas_ids.py
+tdda/rexpy/examples/pandas_ids.py
+tdda/serial/__init__.py
+tdda/serial/base.py
+tdda/serial/cli.py
+tdda/serial/csvw.py
+tdda/serial/pandasio.py
+tdda/serial/reader.py
+tdda/serial/testserialmetadata.py
+tdda/serial/utils.py
```

