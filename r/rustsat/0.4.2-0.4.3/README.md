# Comparing `tmp/rustsat-0.4.2.tar.gz` & `tmp/rustsat-0.4.3.tar.gz`

## Comparing `rustsat-0.4.2.tar` & `rustsat-0.4.3.tar`

### file list

```diff
@@ -1,165 +1,165 @@
--rw-r--r--   0     1001      127      972 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/Cargo.toml
--rw-r--r--   0     1001      127       26 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/.gitignore
--rw-r--r--   0     1001      127      549 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/CHANGELOG.md
--rw-r--r--   0     1001      127     1686 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/README.md
--rwxr-xr-x   0     1001      127     4238 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/build-all.sh
--rw-r--r--   0     1001      127     9247 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/build.rs
--rw-r--r--   0     1001      127  2717714 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/data/AProVE11-12.cnf
--rw-r--r--   0     1001      127   736676 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/data/AProVE11-12.cnf.bz2
--rw-r--r--   0     1001      127   644788 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/data/AProVE11-12.cnf.gz
--rw-r--r--   0     1001      127       44 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/data/bmo.wcnf
--rw-r--r--   0     1001      127       62 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/data/gbmo-1.wcnf
--rw-r--r--   0     1001      127       65 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/data/gbmo-2.wcnf
--rw-r--r--   0     1001      127       99 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/data/small-gbmo.wcnf
--rw-r--r--   0     1001      127       38 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/data/small.cnf
--rw-r--r--   0     1001      127      119 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/data/small.mcnf
--rw-r--r--   0     1001      127      194 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/data/small.opb
--rw-r--r--   0     1001      127       53 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/data/small.wcnf
--rw-r--r--   0     1001      127  1111443 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf
--rw-r--r--   0     1001      127   334484 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.bz2
--rw-r--r--   0     1001      127   305562 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.gz
--rw-r--r--   0     1001      127      131 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/data/tiny-opt.opb
--rw-r--r--   0     1001      127       97 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/data/tiny-sat.opb
--rw-r--r--   0     1001      127      109 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/data/tiny-unsat.opb
--rw-r--r--   0     1001      127     4878 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/patches/v150.patch
--rw-r--r--   0     1001      127     5194 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/patches/v154.patch
--rw-r--r--   0     1001      127     5240 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/patches/v156.patch
--rw-r--r--   0     1001      127     5240 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/patches/v160.patch
--rw-r--r--   0     1001      127     5240 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/patches/v170.patch
--rw-r--r--   0     1001      127     5239 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/patches/v171.patch
--rw-r--r--   0     1001      127     5239 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/patches/v180.patch
--rw-r--r--   0     1001      127     5240 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/patches/v190.patch
--rw-r--r--   0     1001      127     5224 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/patches/v192.patch
--rw-r--r--   0     1001      127    38527 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/src/lib.rs
--rwxr-xr-x   0     1001      127     2352 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/test-all.sh
--rw-r--r--   0     1001      127     3009 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/tests/incremental.rs
--rw-r--r--   0     1001      127     1158 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/tests/phasing.rs
--rw-r--r--   0     1001      127     1756 2024-01-11 14:25:12.000000 rustsat-0.4.2/cadical/tests/small.rs
--rw-r--r--   0     1001      127      725 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/Cargo.toml
--rw-r--r--   0     1001      127       20 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/.gitignore
--rw-r--r--   0     1001      127      516 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/CHANGELOG.md
--rw-r--r--   0     1001      127      978 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/README.md
--rw-r--r--   0     1001      127     3610 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/build.rs
--rw-r--r--   0     1001      127  2717714 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/data/AProVE11-12.cnf
--rw-r--r--   0     1001      127   736676 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/data/AProVE11-12.cnf.bz2
--rw-r--r--   0     1001      127   644788 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/data/AProVE11-12.cnf.gz
--rw-r--r--   0     1001      127       44 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/data/bmo.wcnf
--rw-r--r--   0     1001      127       62 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/data/gbmo-1.wcnf
--rw-r--r--   0     1001      127       65 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/data/gbmo-2.wcnf
--rw-r--r--   0     1001      127       99 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/data/small-gbmo.wcnf
--rw-r--r--   0     1001      127       38 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/data/small.cnf
--rw-r--r--   0     1001      127      119 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/data/small.mcnf
--rw-r--r--   0     1001      127      194 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/data/small.opb
--rw-r--r--   0     1001      127       53 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/data/small.wcnf
--rw-r--r--   0     1001      127  1111443 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf
--rw-r--r--   0     1001      127   334484 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.bz2
--rw-r--r--   0     1001      127   305562 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.gz
--rw-r--r--   0     1001      127      131 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/data/tiny-opt.opb
--rw-r--r--   0     1001      127       97 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/data/tiny-sat.opb
--rw-r--r--   0     1001      127      109 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/data/tiny-unsat.opb
--rw-r--r--   0     1001      127    13295 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/src/core.rs
--rw-r--r--   0     1001      127     1694 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/src/lib.rs
--rw-r--r--   0     1001      127    14217 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/src/simp.rs
--rw-r--r--   0     1001      127     3143 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/tests/incremental.rs
--rw-r--r--   0     1001      127     1235 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/tests/phasing.rs
--rw-r--r--   0     1001      127     1672 2024-01-11 14:25:12.000000 rustsat-0.4.2/minisat/tests/small.rs
--rw-r--r--   0     1001      127     1302 2024-01-11 14:25:12.000000 rustsat-0.4.2/tools/Cargo.toml
--rw-r--r--   0     1001      127       20 2024-01-11 14:25:12.000000 rustsat-0.4.2/tools/.gitignore
--rw-r--r--   0     1001      127      598 2024-01-11 14:25:12.000000 rustsat-0.4.2/tools/CHANGELOG.md
--rw-r--r--   0     1001      127      594 2024-01-11 14:25:12.000000 rustsat-0.4.2/tools/README.md
--rw-r--r--   0     1001      127     1424 2024-01-11 14:25:12.000000 rustsat-0.4.2/tools/src/bin/cnf2opb.rs
--rw-r--r--   0     1001      127     5938 2024-01-11 14:25:12.000000 rustsat-0.4.2/tools/src/bin/encodings.rs
--rw-r--r--   0     1001      127     1994 2024-01-11 14:25:12.000000 rustsat-0.4.2/tools/src/bin/enumerator.rs
--rw-r--r--   0     1001      127    18512 2024-01-11 14:25:12.000000 rustsat-0.4.2/tools/src/bin/gbmosplit.rs
--rw-r--r--   0     1001      127     1447 2024-01-11 14:25:12.000000 rustsat-0.4.2/tools/src/bin/mcnf2opb.rs
--rw-r--r--   0     1001      127     1387 2024-01-11 14:25:12.000000 rustsat-0.4.2/tools/src/bin/opb2cnf.rs
--rw-r--r--   0     1001      127     1611 2024-01-11 14:25:12.000000 rustsat-0.4.2/tools/src/bin/opb2mcnf.rs
--rw-r--r--   0     1001      127     1539 2024-01-11 14:25:12.000000 rustsat-0.4.2/tools/src/bin/opb2wcnf.rs
--rw-r--r--   0     1001      127     3013 2024-01-11 14:25:12.000000 rustsat-0.4.2/tools/src/bin/shuffledimacs.rs
--rw-r--r--   0     1001      127     1422 2024-01-11 14:25:12.000000 rustsat-0.4.2/tools/src/bin/wcnf2opb.rs
--rw-r--r--   0     1001      127    15930 2024-01-11 14:25:12.000000 rustsat-0.4.2/tools/src/encodings/clustering.rs
--rw-r--r--   0     1001      127     3819 2024-01-11 14:25:12.000000 rustsat-0.4.2/tools/src/encodings/knapsack.rs
--rw-r--r--   0     1001      127      463 2024-01-11 14:25:12.000000 rustsat-0.4.2/tools/src/lib.rs
--rw-r--r--   0     1001      127     6417 2024-01-11 14:25:12.000000 rustsat-0.4.2/tools/src/utils.rs
--rw-r--r--   0     1001      127     1903 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/Cargo.toml
--rw-r--r--   0     1001      127     1827 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/CHANGELOG.md
--rw-r--r--   0     1001      127     3934 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/README.md
--rw-r--r--   0     1001      127     2824 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/build.rs
--rw-r--r--   0     1001      127     2957 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/cbindgen.toml
--rw-r--r--   0     1001      127  2717714 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/data/AProVE11-12.cnf
--rw-r--r--   0     1001      127   736676 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/data/AProVE11-12.cnf.bz2
--rw-r--r--   0     1001      127   644788 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/data/AProVE11-12.cnf.gz
--rw-r--r--   0     1001      127       44 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/data/bmo.wcnf
--rw-r--r--   0     1001      127       62 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/data/gbmo-1.wcnf
--rw-r--r--   0     1001      127       65 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/data/gbmo-2.wcnf
--rw-r--r--   0     1001      127       99 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/data/small-gbmo.wcnf
--rw-r--r--   0     1001      127       38 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/data/small.cnf
--rw-r--r--   0     1001      127      119 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/data/small.mcnf
--rw-r--r--   0     1001      127      194 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/data/small.opb
--rw-r--r--   0     1001      127       53 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/data/small.wcnf
--rw-r--r--   0     1001      127  1111443 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf
--rw-r--r--   0     1001      127   334484 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.bz2
--rw-r--r--   0     1001      127   305562 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.gz
--rw-r--r--   0     1001      127      131 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/data/tiny-opt.opb
--rw-r--r--   0     1001      127       97 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/data/tiny-sat.opb
--rw-r--r--   0     1001      127      109 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/data/tiny-unsat.opb
--rw-r--r--   0     1001      127      283 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/examples/Makefile
--rw-r--r--   0     1001      127     1156 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/examples/capi-ipasir.cpp
--rw-r--r--   0     1001      127     1626 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/examples/capi.cpp
--rw-r--r--   0     1001      127     2288 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/examples/profiling.rs
--rw-r--r--   0     1001      127     1282 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/examples/pyapi-dpw.py
--rw-r--r--   0     1001      127      165 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/pyproject.toml
--rw-r--r--   0     1001      127      111 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/rustsat/__init__.py
--rw-r--r--   0     1001      127     1615 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/rustsat/__init__.pyi
--rw-r--r--   0     1001      127      152 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/rustsat/encodings/__init__.py
--rw-r--r--   0     1001      127     1201 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/rustsat/encodings/__init__.pyi
--rw-r--r--   0     1001      127        0 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/rustsat/py.typed
--rw-r--r--   0     1001      127     6635 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/rustsat.h
--rw-r--r--   0     1001      127     4820 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/bench.rs
--rw-r--r--   0     1001      127    17628 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/capi.rs
--rw-r--r--   0     1001      127     2151 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/encodings/am1/pairwise.rs
--rw-r--r--   0     1001      127     1295 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/encodings/am1.rs
--rw-r--r--   0     1001      127     2037 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/encodings/atomics.rs
--rw-r--r--   0     1001      127    43756 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/encodings/card/dbtotalizer.rs
--rw-r--r--   0     1001      127     9673 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/encodings/card/simulators.rs
--rw-r--r--   0     1001      127    38562 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/encodings/card/totalizer.rs
--rw-r--r--   0     1001      127    14019 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/encodings/card.rs
--rw-r--r--   0     1001      127    17143 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/encodings/nodedb.rs
--rw-r--r--   0     1001      127    24969 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/encodings/pb/dbgte.rs
--rw-r--r--   0     1001      127    22047 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/encodings/pb/dpw.rs
--rw-r--r--   0     1001      127    33575 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/encodings/pb/gte.rs
--rw-r--r--   0     1001      127    15787 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/encodings/pb/simulators.rs
--rw-r--r--   0     1001      127    16370 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/encodings/pb.rs
--rw-r--r--   0     1001      127     2664 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/encodings.rs
--rw-r--r--   0     1001      127    40757 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/instances/fio/dimacs.rs
--rw-r--r--   0     1001      127    34934 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/instances/fio/opb.rs
--rw-r--r--   0     1001      127     2774 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/instances/fio.rs
--rw-r--r--   0     1001      127    12027 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/instances/multiopt.rs
--rw-r--r--   0     1001      127    40171 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/instances/opt.rs
--rw-r--r--   0     1001      127    30353 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/instances/sat.rs
--rw-r--r--   0     1001      127    13256 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/instances.rs
--rw-r--r--   0     1001      127     4026 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/lib.rs
--rw-r--r--   0     1001      127     2510 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/pyapi.rs
--rw-r--r--   0     1001      127    17056 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/solvers/ipasir.rs
--rw-r--r--   0     1001      127    18434 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/solvers.rs
--rw-r--r--   0     1001      127    44321 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/types/constraints.rs
--rw-r--r--   0     1001      127    26661 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/types.rs
--rw-r--r--   0     1001      127     1299 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/src/utils.rs
--rw-r--r--   0     1001      127       33 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/stubtest-allowlist.txt
--rw-r--r--   0     1001      127      840 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/tests/am1_encodings.rs
--rw-r--r--   0     1001      127    16452 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/tests/card_encodings.rs
--rw-r--r--   0     1001      127     5225 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/tests/cnf.rs
--rw-r--r--   0     1001      127     1644 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/tests/compression.rs
--rw-r--r--   0     1001      127     5420 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/tests/constraints.rs
--rw-r--r--   0     1001      127     2774 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/tests/opb.rs
--rw-r--r--   0     1001      127    13296 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/tests/pb_encodings.rs
--rw-r--r--   0     1001      127     3934 2024-01-11 14:25:12.000000 rustsat-0.4.2/README.md
--rw-r--r--   0     1001      127    43257 2024-01-11 14:25:16.000000 rustsat-0.4.2/Cargo.lock
--rw-r--r--   0        0        0      101 1970-01-01 00:00:00.000000 rustsat-0.4.2/Cargo.toml
--rw-r--r--   0        0        0      202 1970-01-01 00:00:00.000000 rustsat-0.4.2/pyproject.toml
--rw-r--r--   0     1001      127     1615 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/__init__.pyi
--rw-r--r--   0     1001      127     1201 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/encodings/__init__.pyi
--rw-r--r--   0     1001      127      152 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/encodings/__init__.py
--rw-r--r--   0     1001      127      111 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/__init__.py
--rw-r--r--   0     1001      127        0 2024-01-11 14:25:12.000000 rustsat-0.4.2/rustsat/py.typed
--rw-r--r--   0        0        0     4544 1970-01-01 00:00:00.000000 rustsat-0.4.2/PKG-INFO
+-rw-r--r--   0     1001      127     1302 2024-02-23 08:21:57.000000 rustsat-0.4.3/tools/Cargo.toml
+-rw-r--r--   0     1001      127       20 2024-02-23 08:21:57.000000 rustsat-0.4.3/tools/.gitignore
+-rw-r--r--   0     1001      127      722 2024-02-23 08:21:57.000000 rustsat-0.4.3/tools/CHANGELOG.md
+-rw-r--r--   0     1001      127      594 2024-02-23 08:21:57.000000 rustsat-0.4.3/tools/README.md
+-rw-r--r--   0     1001      127     1424 2024-02-23 08:21:57.000000 rustsat-0.4.3/tools/src/bin/cnf2opb.rs
+-rw-r--r--   0     1001      127     5938 2024-02-23 08:21:57.000000 rustsat-0.4.3/tools/src/bin/encodings.rs
+-rw-r--r--   0     1001      127     1994 2024-02-23 08:21:57.000000 rustsat-0.4.3/tools/src/bin/enumerator.rs
+-rw-r--r--   0     1001      127    18509 2024-02-23 08:21:57.000000 rustsat-0.4.3/tools/src/bin/gbmosplit.rs
+-rw-r--r--   0     1001      127     1447 2024-02-23 08:21:57.000000 rustsat-0.4.3/tools/src/bin/mcnf2opb.rs
+-rw-r--r--   0     1001      127     1387 2024-02-23 08:21:57.000000 rustsat-0.4.3/tools/src/bin/opb2cnf.rs
+-rw-r--r--   0     1001      127     1611 2024-02-23 08:21:57.000000 rustsat-0.4.3/tools/src/bin/opb2mcnf.rs
+-rw-r--r--   0     1001      127     1539 2024-02-23 08:21:57.000000 rustsat-0.4.3/tools/src/bin/opb2wcnf.rs
+-rw-r--r--   0     1001      127     3013 2024-02-23 08:21:57.000000 rustsat-0.4.3/tools/src/bin/shuffledimacs.rs
+-rw-r--r--   0     1001      127     1422 2024-02-23 08:21:57.000000 rustsat-0.4.3/tools/src/bin/wcnf2opb.rs
+-rw-r--r--   0     1001      127    15930 2024-02-23 08:21:57.000000 rustsat-0.4.3/tools/src/encodings/clustering.rs
+-rw-r--r--   0     1001      127     3819 2024-02-23 08:21:57.000000 rustsat-0.4.3/tools/src/encodings/knapsack.rs
+-rw-r--r--   0     1001      127      463 2024-02-23 08:21:57.000000 rustsat-0.4.3/tools/src/lib.rs
+-rw-r--r--   0     1001      127     6417 2024-02-23 08:21:57.000000 rustsat-0.4.3/tools/src/utils.rs
+-rw-r--r--   0     1001      127      725 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/Cargo.toml
+-rw-r--r--   0     1001      127       20 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/.gitignore
+-rw-r--r--   0     1001      127      639 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/CHANGELOG.md
+-rw-r--r--   0     1001      127      978 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/README.md
+-rw-r--r--   0     1001      127     3656 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/build.rs
+-rw-r--r--   0     1001      127  2717714 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/data/AProVE11-12.cnf
+-rw-r--r--   0     1001      127   736676 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/data/AProVE11-12.cnf.bz2
+-rw-r--r--   0     1001      127   644788 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/data/AProVE11-12.cnf.gz
+-rw-r--r--   0     1001      127       44 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/data/bmo.wcnf
+-rw-r--r--   0     1001      127       62 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/data/gbmo-1.wcnf
+-rw-r--r--   0     1001      127       65 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/data/gbmo-2.wcnf
+-rw-r--r--   0     1001      127       99 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/data/small-gbmo.wcnf
+-rw-r--r--   0     1001      127       38 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/data/small.cnf
+-rw-r--r--   0     1001      127      119 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/data/small.mcnf
+-rw-r--r--   0     1001      127      194 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/data/small.opb
+-rw-r--r--   0     1001      127       53 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/data/small.wcnf
+-rw-r--r--   0     1001      127  1111443 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf
+-rw-r--r--   0     1001      127   334484 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.bz2
+-rw-r--r--   0     1001      127   305562 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.gz
+-rw-r--r--   0     1001      127      161 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/data/tiny-opt.opb
+-rw-r--r--   0     1001      127      127 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/data/tiny-sat.opb
+-rw-r--r--   0     1001      127      139 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/data/tiny-unsat.opb
+-rw-r--r--   0     1001      127    13295 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/src/core.rs
+-rw-r--r--   0     1001      127     1694 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/src/lib.rs
+-rw-r--r--   0     1001      127    14217 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/src/simp.rs
+-rw-r--r--   0     1001      127     3143 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/tests/incremental.rs
+-rw-r--r--   0     1001      127     1235 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/tests/phasing.rs
+-rw-r--r--   0     1001      127     1672 2024-02-23 08:21:57.000000 rustsat-0.4.3/minisat/tests/small.rs
+-rw-r--r--   0     1001      127      972 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/Cargo.toml
+-rw-r--r--   0     1001      127       26 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/.gitignore
+-rw-r--r--   0     1001      127      680 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/CHANGELOG.md
+-rw-r--r--   0     1001      127     1686 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/README.md
+-rwxr-xr-x   0     1001      127     4238 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/build-all.sh
+-rw-r--r--   0     1001      127     9247 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/build.rs
+-rw-r--r--   0     1001      127  2717714 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/data/AProVE11-12.cnf
+-rw-r--r--   0     1001      127   736676 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/data/AProVE11-12.cnf.bz2
+-rw-r--r--   0     1001      127   644788 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/data/AProVE11-12.cnf.gz
+-rw-r--r--   0     1001      127       44 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/data/bmo.wcnf
+-rw-r--r--   0     1001      127       62 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/data/gbmo-1.wcnf
+-rw-r--r--   0     1001      127       65 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/data/gbmo-2.wcnf
+-rw-r--r--   0     1001      127       99 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/data/small-gbmo.wcnf
+-rw-r--r--   0     1001      127       38 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/data/small.cnf
+-rw-r--r--   0     1001      127      119 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/data/small.mcnf
+-rw-r--r--   0     1001      127      194 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/data/small.opb
+-rw-r--r--   0     1001      127       53 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/data/small.wcnf
+-rw-r--r--   0     1001      127  1111443 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf
+-rw-r--r--   0     1001      127   334484 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.bz2
+-rw-r--r--   0     1001      127   305562 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.gz
+-rw-r--r--   0     1001      127      161 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/data/tiny-opt.opb
+-rw-r--r--   0     1001      127      127 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/data/tiny-sat.opb
+-rw-r--r--   0     1001      127      139 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/data/tiny-unsat.opb
+-rw-r--r--   0     1001      127     4878 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/patches/v150.patch
+-rw-r--r--   0     1001      127     5194 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/patches/v154.patch
+-rw-r--r--   0     1001      127     5240 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/patches/v156.patch
+-rw-r--r--   0     1001      127     5240 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/patches/v160.patch
+-rw-r--r--   0     1001      127     5240 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/patches/v170.patch
+-rw-r--r--   0     1001      127     5239 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/patches/v171.patch
+-rw-r--r--   0     1001      127     5239 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/patches/v180.patch
+-rw-r--r--   0     1001      127     5240 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/patches/v190.patch
+-rw-r--r--   0     1001      127     5224 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/patches/v192.patch
+-rw-r--r--   0     1001      127    38527 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/src/lib.rs
+-rwxr-xr-x   0     1001      127     2352 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/test-all.sh
+-rw-r--r--   0     1001      127     3009 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/tests/incremental.rs
+-rw-r--r--   0     1001      127     1158 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/tests/phasing.rs
+-rw-r--r--   0     1001      127     1756 2024-02-23 08:21:57.000000 rustsat-0.4.3/cadical/tests/small.rs
+-rw-r--r--   0     1001      127     1903 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/Cargo.toml
+-rw-r--r--   0     1001      127     2183 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/CHANGELOG.md
+-rw-r--r--   0     1001      127     3934 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/README.md
+-rw-r--r--   0     1001      127     2977 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/build.rs
+-rw-r--r--   0     1001      127     2957 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/cbindgen.toml
+-rw-r--r--   0     1001      127  2717714 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/data/AProVE11-12.cnf
+-rw-r--r--   0     1001      127   736676 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/data/AProVE11-12.cnf.bz2
+-rw-r--r--   0     1001      127   644788 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/data/AProVE11-12.cnf.gz
+-rw-r--r--   0     1001      127       44 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/data/bmo.wcnf
+-rw-r--r--   0     1001      127       62 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/data/gbmo-1.wcnf
+-rw-r--r--   0     1001      127       65 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/data/gbmo-2.wcnf
+-rw-r--r--   0     1001      127       99 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/data/small-gbmo.wcnf
+-rw-r--r--   0     1001      127       38 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/data/small.cnf
+-rw-r--r--   0     1001      127      119 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/data/small.mcnf
+-rw-r--r--   0     1001      127      194 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/data/small.opb
+-rw-r--r--   0     1001      127       53 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/data/small.wcnf
+-rw-r--r--   0     1001      127  1111443 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf
+-rw-r--r--   0     1001      127   334484 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.bz2
+-rw-r--r--   0     1001      127   305562 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.gz
+-rw-r--r--   0     1001      127      161 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/data/tiny-opt.opb
+-rw-r--r--   0     1001      127      127 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/data/tiny-sat.opb
+-rw-r--r--   0     1001      127      139 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/data/tiny-unsat.opb
+-rw-r--r--   0     1001      127      283 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/examples/Makefile
+-rw-r--r--   0     1001      127     1156 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/examples/capi-ipasir.cpp
+-rw-r--r--   0     1001      127     1626 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/examples/capi.cpp
+-rw-r--r--   0     1001      127     2288 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/examples/profiling.rs
+-rw-r--r--   0     1001      127     1282 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/examples/pyapi-dpw.py
+-rw-r--r--   0     1001      127      165 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/pyproject.toml
+-rw-r--r--   0     1001      127      111 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/rustsat/__init__.py
+-rw-r--r--   0     1001      127     1615 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/rustsat/__init__.pyi
+-rw-r--r--   0     1001      127      152 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/rustsat/encodings/__init__.py
+-rw-r--r--   0     1001      127     1201 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/rustsat/encodings/__init__.pyi
+-rw-r--r--   0     1001      127        0 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/rustsat/py.typed
+-rw-r--r--   0     1001      127     6635 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/rustsat.h
+-rw-r--r--   0     1001      127     4820 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/bench.rs
+-rw-r--r--   0     1001      127    17628 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/capi.rs
+-rw-r--r--   0     1001      127     2151 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/encodings/am1/pairwise.rs
+-rw-r--r--   0     1001      127     1295 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/encodings/am1.rs
+-rw-r--r--   0     1001      127     2037 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/encodings/atomics.rs
+-rw-r--r--   0     1001      127    43956 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/encodings/card/dbtotalizer.rs
+-rw-r--r--   0     1001      127     9673 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/encodings/card/simulators.rs
+-rw-r--r--   0     1001      127    38562 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/encodings/card/totalizer.rs
+-rw-r--r--   0     1001      127    14019 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/encodings/card.rs
+-rw-r--r--   0     1001      127    18810 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/encodings/nodedb.rs
+-rw-r--r--   0     1001      127    25232 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/encodings/pb/dbgte.rs
+-rw-r--r--   0     1001      127    22047 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/encodings/pb/dpw.rs
+-rw-r--r--   0     1001      127    33575 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/encodings/pb/gte.rs
+-rw-r--r--   0     1001      127    15787 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/encodings/pb/simulators.rs
+-rw-r--r--   0     1001      127    16370 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/encodings/pb.rs
+-rw-r--r--   0     1001      127     2664 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/encodings.rs
+-rw-r--r--   0     1001      127    40757 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/instances/fio/dimacs.rs
+-rw-r--r--   0     1001      127    35406 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/instances/fio/opb.rs
+-rw-r--r--   0     1001      127     2774 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/instances/fio.rs
+-rw-r--r--   0     1001      127    12027 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/instances/multiopt.rs
+-rw-r--r--   0     1001      127    40171 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/instances/opt.rs
+-rw-r--r--   0     1001      127    30353 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/instances/sat.rs
+-rw-r--r--   0     1001      127    13256 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/instances.rs
+-rw-r--r--   0     1001      127     4026 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/lib.rs
+-rw-r--r--   0     1001      127     2510 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/pyapi.rs
+-rw-r--r--   0     1001      127    17056 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/solvers/ipasir.rs
+-rw-r--r--   0     1001      127    18434 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/solvers.rs
+-rw-r--r--   0     1001      127    44321 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/types/constraints.rs
+-rw-r--r--   0     1001      127    26661 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/types.rs
+-rw-r--r--   0     1001      127     1299 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/src/utils.rs
+-rw-r--r--   0     1001      127       33 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/stubtest-allowlist.txt
+-rw-r--r--   0     1001      127      840 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/tests/am1_encodings.rs
+-rw-r--r--   0     1001      127    16452 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/tests/card_encodings.rs
+-rw-r--r--   0     1001      127     5225 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/tests/cnf.rs
+-rw-r--r--   0     1001      127     1644 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/tests/compression.rs
+-rw-r--r--   0     1001      127     5420 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/tests/constraints.rs
+-rw-r--r--   0     1001      127     2774 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/tests/opb.rs
+-rw-r--r--   0     1001      127    13296 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/tests/pb_encodings.rs
+-rw-r--r--   0     1001      127     3934 2024-02-23 08:21:57.000000 rustsat-0.4.3/README.md
+-rw-r--r--   0     1001      127    43206 2024-02-23 08:22:01.000000 rustsat-0.4.3/Cargo.lock
+-rw-r--r--   0        0        0      101 1970-01-01 00:00:00.000000 rustsat-0.4.3/Cargo.toml
+-rw-r--r--   0        0        0      202 1970-01-01 00:00:00.000000 rustsat-0.4.3/pyproject.toml
+-rw-r--r--   0     1001      127     1615 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/__init__.pyi
+-rw-r--r--   0     1001      127     1201 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/encodings/__init__.pyi
+-rw-r--r--   0     1001      127      152 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/encodings/__init__.py
+-rw-r--r--   0     1001      127      111 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/__init__.py
+-rw-r--r--   0     1001      127        0 2024-02-23 08:21:57.000000 rustsat-0.4.3/rustsat/py.typed
+-rw-r--r--   0        0        0     4544 1970-01-01 00:00:00.000000 rustsat-0.4.3/PKG-INFO
```

### Comparing `rustsat-0.4.2/cadical/Cargo.toml` & `rustsat-0.4.3/cadical/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rustsat-cadical"
-version = "0.2.3"
+version = "0.2.4"
 edition = "2021"
 authors = ["Christoph Jabs <christoph.jabs@helsinki.fi>"]
 license = "MIT"
 description = "Interface to the SAT solver CaDiCaL for the RustSAT library."
 keywords = ["sat-solver", "rustsat"]
 repository = "https://github.com/chrjabs/rustsat"
 readme = "README.md"
@@ -36,14 +36,14 @@
 v1-9-1 = []
 v1-9-2 = []
 v1-9-3 = []
 v1-9-4 = []
 
 [dependencies]
 cpu-time = "1.0.0"
-rustsat = { version = "0.4.2", path = "../rustsat", default-features = false }
+rustsat = { version = "0.4.3", path = "../rustsat", default-features = false }
 
 [build-dependencies]
 cc = { version = "1.0.83", features = ["parallel"] }
 git2 = "0.18.1"
 glob = "0.3.1"
 chrono = "0.4.31"
```

### Comparing `rustsat-0.4.2/cadical/README.md` & `rustsat-0.4.3/cadical/README.md`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/build-all.sh` & `rustsat-0.4.3/cadical/build-all.sh`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/build.rs` & `rustsat-0.4.3/cadical/build.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/data/AProVE11-12.cnf` & `rustsat-0.4.3/minisat/data/AProVE11-12.cnf`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/data/AProVE11-12.cnf.bz2` & `rustsat-0.4.3/minisat/data/AProVE11-12.cnf.bz2`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/data/AProVE11-12.cnf.gz` & `rustsat-0.4.3/minisat/data/AProVE11-12.cnf.gz`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf` & `rustsat-0.4.3/minisat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.bz2` & `rustsat-0.4.3/minisat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.bz2`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.gz` & `rustsat-0.4.3/minisat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.gz`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/patches/v150.patch` & `rustsat-0.4.3/cadical/patches/v150.patch`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/patches/v154.patch` & `rustsat-0.4.3/cadical/patches/v154.patch`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/patches/v156.patch` & `rustsat-0.4.3/cadical/patches/v156.patch`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/patches/v160.patch` & `rustsat-0.4.3/cadical/patches/v160.patch`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/patches/v170.patch` & `rustsat-0.4.3/cadical/patches/v170.patch`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/patches/v171.patch` & `rustsat-0.4.3/cadical/patches/v171.patch`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/patches/v180.patch` & `rustsat-0.4.3/cadical/patches/v180.patch`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/patches/v190.patch` & `rustsat-0.4.3/cadical/patches/v190.patch`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/patches/v192.patch` & `rustsat-0.4.3/cadical/patches/v192.patch`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/src/lib.rs` & `rustsat-0.4.3/cadical/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/test-all.sh` & `rustsat-0.4.3/cadical/test-all.sh`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/tests/incremental.rs` & `rustsat-0.4.3/cadical/tests/incremental.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/tests/phasing.rs` & `rustsat-0.4.3/cadical/tests/phasing.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/cadical/tests/small.rs` & `rustsat-0.4.3/cadical/tests/small.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/minisat/Cargo.toml` & `rustsat-0.4.3/minisat/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rustsat-minisat"
-version = "0.2.3"
+version = "0.2.4"
 edition = "2021"
 authors = ["Christoph Jabs <christoph.jabs@helsinki.fi>"]
 license = "MIT"
 description = "Interface to the SAT solver Minisat for the RustSAT library."
 keywords = ["sat-solver", "rustsat"]
 repository = "https://github.com/chrjabs/rustsat"
 readme = "README.md"
@@ -14,15 +14,15 @@
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [features]
 debug = []
 
 [dependencies]
 cpu-time = "1.0.0"
-rustsat = { version = "0.4.2", path = "../rustsat", default-features = false }
+rustsat = { version = "0.4.3", path = "../rustsat", default-features = false }
 
 [build-dependencies]
 cc = { version = "1.0.83", features = ["parallel"] }
 git2 = "0.18.1"
 glob = "0.3.1"
 chrono = "0.4.31"
 cmake = "0.1.50"
```

### Comparing `rustsat-0.4.2/minisat/CHANGELOG.md` & `rustsat-0.4.3/tools/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.2.4] - 2024-02-22
+
+### Features
+
+- Make opb defaults more like pbo competition specs
+
 <!-- generated by git-cliff -->
 ## [0.2.3] - 2024-01-11
 
-### Documentation
+### Miscellaneous Tasks
 
-- Fix [docs.rs](https://docs.rs/rustsat-minisat) build
+- Updated the following local packages: rustsat, rustsat-minisat, rustsat-cadical
 
+<!-- generated by git-cliff -->
 ## [0.2.2] - 2024-01-11
 
-### Bug Fixes
+### Features
 
-- Build on non-linux
+- Select minisat/cadical via a cargo feature
+- Moved integration tests to main crate
 
 ### Documentation
 
 - Add shields to READMEs
 
-### Features
-
-- Debug feature
-
 <!-- generated by git-cliff -->
 ## [0.2.1] - 2023-12-18
 
 ### Miscellaneous Tasks
 
-- Updated the following local packages: rustsat
+- Updated the following local packages: rustsat, rustsat-cadical
 
 <!-- generated by git-cliff -->
```

### Comparing `rustsat-0.4.2/minisat/README.md` & `rustsat-0.4.3/minisat/README.md`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/minisat/build.rs` & `rustsat-0.4.3/minisat/build.rs`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     }
 
     // Build C++ library
     // Full commit hash needs to be provided
     build(
         "https://github.com/chrjabs/minisat.git",
         "master",
-        "f64a4f78eea61927dec9f151650504defba490c1",
+        "809d350ff282e695014e96a2afd3625196f58dff",
     );
 
     let out_dir = env::var("OUT_DIR").unwrap();
 
     // Built solver is in out_dir
     println!("cargo:rustc-link-search={}", out_dir);
     println!("cargo:rustc-link-search={}/lib", out_dir);
@@ -29,14 +29,15 @@
     if update_repo(minisat_dir, repo, branch, commit)
         || !Path::new(&out_dir)
             .join("lib")
             .join("libminisat.a")
             .exists()
     {
         let mut conf = cmake::Config::new(minisat_dir);
+        conf.define("BUILD_BINARIES", "OFF");
         if cfg!(not(feature = "debug")) {
             conf.profile("Release");
         }
         conf.build();
     };
 
     println!("cargo:rustc-link-lib=static=minisat");
```

### Comparing `rustsat-0.4.2/minisat/data/AProVE11-12.cnf` & `rustsat-0.4.3/cadical/data/AProVE11-12.cnf`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/minisat/data/AProVE11-12.cnf.bz2` & `rustsat-0.4.3/cadical/data/AProVE11-12.cnf.bz2`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/minisat/data/AProVE11-12.cnf.gz` & `rustsat-0.4.3/cadical/data/AProVE11-12.cnf.gz`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/minisat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf` & `rustsat-0.4.3/cadical/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/minisat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.bz2` & `rustsat-0.4.3/cadical/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.bz2`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/minisat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.gz` & `rustsat-0.4.3/cadical/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.gz`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/minisat/src/core.rs` & `rustsat-0.4.3/minisat/src/core.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/minisat/src/lib.rs` & `rustsat-0.4.3/minisat/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/minisat/src/simp.rs` & `rustsat-0.4.3/minisat/src/simp.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/minisat/tests/incremental.rs` & `rustsat-0.4.3/minisat/tests/incremental.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/minisat/tests/phasing.rs` & `rustsat-0.4.3/minisat/tests/phasing.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/minisat/tests/small.rs` & `rustsat-0.4.3/minisat/tests/small.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/tools/Cargo.toml` & `rustsat-0.4.3/tools/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [package]
 name = "rustsat-tools"
-version = "0.2.3"
+version = "0.2.4"
 edition = "2021"
 authors = ["Christoph Jabs <christoph.jabs@helsinki.fi>"]
 license = "MIT"
 description = "Tools and examples built on the RustSAT library"
 keywords = ["rustsat", "sat", "satisfiability"]
 repository = "https://github.com/chrjabs/rustsat"
 readme = "README.md"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
-rustsat = { version = "0.4.2", path = "../rustsat", features = ["compression", "multiopt", "rand", "internals"] }
-rustsat-cadical = { version = "0.2.3", path = "../cadical", optional = true }
-rustsat-minisat = { version = "0.2.3", path = "../minisat", optional = true }
+rustsat = { version = "0.4.3", path = "../rustsat", features = ["compression", "multiopt", "rand", "internals"] }
+rustsat-cadical = { version = "0.2.4", path = "../cadical", optional = true }
+rustsat-minisat = { version = "0.2.4", path = "../minisat", optional = true }
 clap = { version = "4.2.4", features = ["derive", "cargo"] }
 concolor-clap = { version = "0.1.0" }
 termcolor = { version = "1.2.0" }
 atty = { version = "0.2.14" }
 nom = "7.1.3"
 rand = "0.8.5"
 rand_chacha = "0.3.1"
```

### Comparing `rustsat-0.4.2/tools/CHANGELOG.md` & `rustsat-0.4.3/cadical/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
-## [0.2.3] - 2024-01-11
+## [0.2.4] - 2024-02-22
 
 ### Miscellaneous Tasks
 
-- Updated the following local packages: rustsat, rustsat-minisat, rustsat-cadical
+- Updated the following local packages: rustsat
 
 <!-- generated by git-cliff -->
+<!-- generated by git-cliff -->
+## [0.2.3] - 2024-01-11
+
+### Documentation
+
+- Fix [docs.rs](https://docs.rs/rustsat-cadical) build
+
 ## [0.2.2] - 2024-01-11
 
-### Features
+### Bug Fixes
 
-- Select minisat/cadical via a cargo feature
-- Moved integration tests to main crate
+- Specify c++ std version in cadical build
 
 ### Documentation
 
+- Mention broken windows build
 - Add shields to READMEs
 
+### Features
+
+- Cadical versions 1.9.[3-4]
+
 <!-- generated by git-cliff -->
 ## [0.2.1] - 2023-12-18
 
-### Miscellaneous Tasks
+### Features
 
-- Updated the following local packages: rustsat, rustsat-cadical
+- Cadical v1.9.0 - v1.9.2
 
 <!-- generated by git-cliff -->
```

### Comparing `rustsat-0.4.2/tools/README.md` & `rustsat-0.4.3/tools/README.md`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/tools/src/bin/cnf2opb.rs` & `rustsat-0.4.3/tools/src/bin/cnf2opb.rs`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #[command(author, version, about, long_about = None)]
 struct Args {
     /// The DIMACS CNF input file. Reads from `stdin` if not given.
     in_path: Option<PathBuf>,
     /// The OPB output path. Writes to `stdout` if not given.
     out_path: Option<PathBuf>,
     /// The index in the OPB file to treat as the lowest variable
-    #[arg(long, default_value_t = 0)]
+    #[arg(long, default_value_t = 1)]
     first_var_idx: u32,
     /// Avoid negated literals in the OPB file by transforming constraints
     #[arg(long)]
     avoid_negated_lits: bool,
 }
 
 fn main() {
```

### Comparing `rustsat-0.4.2/tools/src/bin/encodings.rs` & `rustsat-0.4.3/tools/src/bin/encodings.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/tools/src/bin/enumerator.rs` & `rustsat-0.4.3/tools/src/bin/enumerator.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/tools/src/bin/gbmosplit.rs` & `rustsat-0.4.3/tools/src/bin/gbmosplit.rs`

 * *Files 1% similar despite different names*

```diff
@@ -342,15 +342,15 @@
         a %= b;
         std::mem::swap(&mut a, &mut b);
     }
     a
 }
 
 fn get_sums_pot_splits_gcds(
-    sorted_clauses: &Vec<(Clause, usize)>,
+    sorted_clauses: &[(Clause, usize)],
 ) -> (Vec<usize>, Vec<usize>, Vec<usize>) {
     let mut sums = vec![];
     let mut pot_split_ends = vec![];
     let mut sum = 0;
     // find sums and potential splits
     for idx in 0..sorted_clauses.len() {
         sum += sorted_clauses[idx].1;
```

### Comparing `rustsat-0.4.2/tools/src/bin/mcnf2opb.rs` & `rustsat-0.4.3/tools/src/bin/mcnf2opb.rs`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #[command(author, version, about, long_about = None)]
 struct Args {
     /// The DIMACS MCNF input file. Reads from `stdin` if not given.
     in_path: Option<PathBuf>,
     /// The OPB output path. Writes to `stdout` if not given.
     out_path: Option<PathBuf>,
     /// The index in the OPB file to treat as the lowest variable
-    #[arg(long, default_value_t = 0)]
+    #[arg(long, default_value_t = 1)]
     first_var_idx: u32,
     /// Avoid negated literals in the OPB file by transforming constraints
     #[arg(long)]
     avoid_negated_lits: bool,
 }
 
 fn main() {
```

### Comparing `rustsat-0.4.2/tools/src/bin/opb2cnf.rs` & `rustsat-0.4.3/tools/src/bin/opb2cnf.rs`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #[command(author, version, about, long_about = None)]
 struct Args {
     /// The OPB input file. Reads from `stdin` if not given.
     in_path: Option<PathBuf>,
     /// The DIMACS CNF output path. Writes to `stdout` if not given.
     out_path: Option<PathBuf>,
     /// The index in the OPB file to treat as the lowest variable
-    #[arg(long, default_value_t = 0)]
+    #[arg(long, default_value_t = 1)]
     first_var_idx: usize,
 }
 
 fn main() {
     let args = Args::parse();
     let opb_opts = OpbOptions {
         first_var_idx: 0,
```

### Comparing `rustsat-0.4.2/tools/src/bin/opb2mcnf.rs` & `rustsat-0.4.3/tools/src/bin/opb2mcnf.rs`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #[command(author, version, about, long_about = None)]
 struct Args {
     /// The OPB input file. Reads from `stdin` if not given.
     in_path: Option<PathBuf>,
     /// The DIMACS MCNF output path. Writes to `stdout` if not given.
     out_path: Option<PathBuf>,
     /// The index in the OPB file to treat as the lowest variable
-    #[arg(long, default_value_t = 0)]
+    #[arg(long, default_value_t = 1)]
     first_var_idx: usize,
 }
 
 fn main() {
     let args = Args::parse();
     let opb_opts = OpbOptions {
         first_var_idx: 0,
```

### Comparing `rustsat-0.4.2/tools/src/bin/opb2wcnf.rs` & `rustsat-0.4.3/tools/src/bin/opb2wcnf.rs`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #[command(author, version, about, long_about = None)]
 struct Args {
     /// The OPB input file. Reads from `stdin` if not given.
     in_path: Option<PathBuf>,
     /// The DIMACS WCNF output path. Writes to `stdout` if not given.
     out_path: Option<PathBuf>,
     /// The index in the OPB file to treat as the lowest variable
-    #[arg(long, default_value_t = 0)]
+    #[arg(long, default_value_t = 1)]
     first_var_idx: usize,
 }
 
 fn main() {
     let args = Args::parse();
     let opb_opts = OpbOptions {
         first_var_idx: 0,
```

### Comparing `rustsat-0.4.2/tools/src/bin/shuffledimacs.rs` & `rustsat-0.4.3/tools/src/bin/shuffledimacs.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/tools/src/bin/wcnf2opb.rs` & `rustsat-0.4.3/tools/src/bin/wcnf2opb.rs`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #[command(author, version, about, long_about = None)]
 struct Args {
     /// The DIMACS WCNF input file. Reads from `stdin` if not given.
     in_path: Option<PathBuf>,
     /// The OPB output path. Writes to `stdout` if not given.
     out_path: Option<PathBuf>,
     /// The index in the OPB file to treat as the lowest variable
-    #[arg(long, default_value_t = 0)]
+    #[arg(long, default_value_t = 1)]
     first_var_idx: u32,
     /// Avoid negated literals in the OPB file by transforming constraints
     #[arg(long)]
     avoid_negated_lits: bool,
 }
 
 fn main() {
```

### Comparing `rustsat-0.4.2/tools/src/encodings/clustering.rs` & `rustsat-0.4.3/tools/src/encodings/clustering.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/tools/src/encodings/knapsack.rs` & `rustsat-0.4.3/tools/src/encodings/knapsack.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/tools/src/utils.rs` & `rustsat-0.4.3/tools/src/utils.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/Cargo.toml` & `rustsat-0.4.3/rustsat/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rustsat"
-version = "0.4.2"
+version = "0.4.3"
 edition = "2021"
 authors = ["Christoph Jabs <christoph.jabs@helsinki.fi>"]
 license = "MIT"
 description = "This library aims to provide implementations of elements commonly used in the development on software in the area of satisfiability solving. The focus of the library is to provide as much ease of use without giving up on performance."
 keywords = ["sat", "satisfiability", "encodings"]
 repository = "https://github.com/chrjabs/rustsat"
 readme = "README.md"
```

### Comparing `rustsat-0.4.2/rustsat/CHANGELOG.md` & `rustsat-0.4.3/rustsat/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,29 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.4.3] - 2024-02-22
+
+### Features
+
+- Internal `from_raw` methods for db totalizers
+- Thorough merge strategy for `NodeById`
+- Make opb defaults more like pbo competition specs
+- Output opbs with `#variable` line
+
+### Bug Fixes
+
+- Remove `weight_sum` field from `DbGte`
+
+### Documentation
+
+- Disable cbindgen on docs.rs
+
+<!-- generated by git-cliff -->
 <!-- generated by git-cliff -->
 ## [0.4.2] - 2024-01-11
 
 ### Documentation
 
 - Mark required features in documentation on [docs.rs](https://docs.rs/rustsat)
```

### Comparing `rustsat-0.4.2/rustsat/README.md` & `rustsat-0.4.3/rustsat/README.md`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/build.rs` & `rustsat-0.4.3/rustsat/build.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 extern crate cbindgen;
 
 use std::env;
 
 fn main() {
+    if std::env::var("DOCS_RS").is_ok() {
+        // exit the build script early on docs.rs because cbindgen needs network access
+        return;
+    }
+
     #[cfg(feature = "ipasir")]
     {
         // Link to custom IPASIR solver
         // Uncomment and modify this for linking to your static library
         // The name of the library should be _without_ the prefix 'lib' and the suffix '.a'
         //println!("cargo:rustc-link-lib=static=<path-to-your-static-lib>");
         //println!("cargo:rustc-link-search=<name-of-your-static-lib>");
```

### Comparing `rustsat-0.4.2/rustsat/cbindgen.toml` & `rustsat-0.4.3/rustsat/cbindgen.toml`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/data/AProVE11-12.cnf` & `rustsat-0.4.3/rustsat/data/AProVE11-12.cnf`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/data/AProVE11-12.cnf.bz2` & `rustsat-0.4.3/rustsat/data/AProVE11-12.cnf.bz2`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/data/AProVE11-12.cnf.gz` & `rustsat-0.4.3/rustsat/data/AProVE11-12.cnf.gz`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf` & `rustsat-0.4.3/rustsat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.bz2` & `rustsat-0.4.3/rustsat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.bz2`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.gz` & `rustsat-0.4.3/rustsat/data/smtlib-qfbv-aigs-ext_con_032_008_0256-tseitin.cnf.gz`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/examples/capi-ipasir.cpp` & `rustsat-0.4.3/rustsat/examples/capi-ipasir.cpp`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/examples/capi.cpp` & `rustsat-0.4.3/rustsat/examples/capi.cpp`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/examples/profiling.rs` & `rustsat-0.4.3/rustsat/examples/profiling.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/examples/pyapi-dpw.py` & `rustsat-0.4.3/rustsat/examples/pyapi-dpw.py`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/rustsat/__init__.pyi` & `rustsat-0.4.3/rustsat/rustsat/__init__.pyi`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/rustsat/encodings/__init__.pyi` & `rustsat-0.4.3/rustsat/rustsat/encodings/__init__.pyi`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/rustsat.h` & `rustsat-0.4.3/rustsat/rustsat.h`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/bench.rs` & `rustsat-0.4.3/rustsat/src/bench.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/capi.rs` & `rustsat-0.4.3/rustsat/src/capi.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/encodings/am1/pairwise.rs` & `rustsat-0.4.3/rustsat/src/encodings/am1/pairwise.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/encodings/am1.rs` & `rustsat-0.4.3/rustsat/src/encodings/am1.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/encodings/atomics.rs` & `rustsat-0.4.3/rustsat/src/encodings/atomics.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/encodings/card/dbtotalizer.rs` & `rustsat-0.4.3/rustsat/src/encodings/card/dbtotalizer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,23 @@
     /// The number of clauses in the totalizer
     n_clauses: usize,
     /// The node database of the totalizer
     db: TotDb,
 }
 
 impl DbTotalizer {
+    #[cfg(feature = "internals")]
+    pub fn from_raw(root: NodeId, db: TotDb) -> Self {
+        Self {
+            root: Some(root),
+            db,
+            ..Default::default()
+        }
+    }
+
     fn extend_tree(&mut self) {
         if self.lit_buffer.is_empty() {
             return;
         }
         let new_tree = self.db.lit_tree(&self.lit_buffer);
         self.root = Some(match self.root {
             Some(old_root) => {
```

### Comparing `rustsat-0.4.2/rustsat/src/encodings/card/simulators.rs` & `rustsat-0.4.3/rustsat/src/encodings/card/simulators.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/encodings/card/totalizer.rs` & `rustsat-0.4.3/rustsat/src/encodings/card/totalizer.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/encodings/card.rs` & `rustsat-0.4.3/rustsat/src/encodings/card.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/encodings/nodedb.rs` & `rustsat-0.4.3/rustsat/src/encodings/nodedb.rs`

 * *Files 5% similar despite different names*

```diff
@@ -225,15 +225,15 @@
             multiplier: weight.try_into().unwrap(),
             ..self
         }
     }
 
     #[inline]
     pub fn offset(&self) -> usize {
-        self.offset.into()
+        self.offset
     }
 
     #[inline]
     pub fn divisor(&self) -> usize {
         let div: u8 = self.divisor.into();
         div.into()
     }
@@ -447,14 +447,58 @@
         }
 
         let lcon = self.merge(&cons[..split]);
         let rcon = self.merge(&cons[split..]);
 
         NodeCon::full(self.insert(Self::Node::internal(lcon, rcon, self)))
     }
+
+    /// Merges the given connections according to the following strategy: sort
+    /// the connections by multiplier, then merge connections with equal
+    /// multiplier, then merge resulting connections with
+    /// [`NodeById::merge_balanced`].
+    #[cfg(feature = "internals")]
+    fn merge_thorough(&mut self, cons: &mut [NodeCon]) -> NodeCon
+    where
+        Self: Sized,
+    {
+        debug_assert!(!cons.is_empty());
+        cons.sort_unstable_by_key(|con| con.multiplier());
+
+        // Detect sequences of connections of equal weight and merge them
+        let mut seg_begin = 0;
+        let mut seg_end = 0;
+        let mut merged_cons = vec![];
+        loop {
+            seg_end += 1;
+            if seg_end < cons.len() && cons[seg_end].multiplier() == cons[seg_begin].multiplier() {
+                continue;
+            }
+            if seg_end > seg_begin + 1 {
+                // merge lits of equal weight
+                let mut seg: Vec<_> = cons[seg_begin..seg_end]
+                    .iter()
+                    .map(|&con| con.reweight(1))
+                    .collect();
+                seg.sort_unstable_by_key(|&con| self.con_len(con));
+                let con = self.merge_balanced(&seg);
+                debug_assert_eq!(con.multiplier(), 1);
+                merged_cons.push(con.reweight(cons[seg_begin].multiplier()));
+            } else {
+                merged_cons.push(cons[seg_begin])
+            }
+            seg_begin = seg_end;
+            if seg_end >= cons.len() {
+                break;
+            }
+        }
+
+        merged_cons.sort_unstable_by_key(|&con| self.con_len(con));
+        self.merge_balanced(&merged_cons)
+    }
 }
 
 #[cfg(test)]
 mod tests {
     use super::{NodeCon, NodeId};
 
     #[test]
```

### Comparing `rustsat-0.4.2/rustsat/src/encodings/pb/dbgte.rs` & `rustsat-0.4.3/rustsat/src/encodings/pb/dbgte.rs`

 * *Files 2% similar despite different names*

```diff
@@ -39,25 +39,33 @@
     /// Input literals and weights not yet in the tree
     lit_buffer: RsHashMap<Lit, usize>,
     /// The root of the tree, if constructed
     root: Option<NodeCon>,
     /// Maximum weight of a leaf, needed for computing how much more than
     /// `max_rhs` to encode
     max_leaf_weight: usize,
-    /// Sum of all input weight
-    weight_sum: usize,
     /// The number of variables in the totalizer
     n_vars: u32,
     /// The number of clauses in the totalizer
     n_clauses: usize,
     /// The node database of the totalizer
     db: TotDb,
 }
 
 impl DbGte {
+    #[cfg(feature = "internals")]
+    pub fn from_raw(root: NodeCon, db: TotDb, max_leaf_weight: usize) -> Self {
+        Self {
+            root: Some(root),
+            max_leaf_weight,
+            db,
+            ..Default::default()
+        }
+    }
+
     fn extend_tree(&mut self, max_weight: usize) {
         if !self.lit_buffer.is_empty() {
             let mut new_lits: Vec<(Lit, usize)> = self
                 .lit_buffer
                 .iter()
                 .filter_map(|(&l, &w)| {
                     if w <= max_weight {
@@ -106,15 +114,20 @@
     pub fn depth(&self) -> usize {
         self.root.map_or(0, |con| self.db[con.id].depth())
     }
 }
 
 impl Encode for DbGte {
     fn weight_sum(&self) -> usize {
-        self.weight_sum
+        self.lit_buffer.iter().fold(0, |sum, (_, w)| sum + w)
+            + if let Some(root) = self.root {
+                root.map(self.db[root.id].max_val())
+            } else {
+                0
+            }
     }
 
     fn next_higher(&self, val: usize) -> usize {
         if let Some(con) = self.root {
             self.db[con.id]
                 .vals(con.rev_map_round_up(val + 1)..)
                 .next()
@@ -155,15 +168,15 @@
         R: RangeBounds<usize>,
     {
         self.db.reset_encoded();
         self.encode_ub_change(range, collector, var_manager);
     }
 
     fn enforce_ub(&self, ub: usize) -> Result<Vec<Lit>, Error> {
-        if ub >= self.weight_sum {
+        if ub >= self.weight_sum() {
             return Ok(vec![]);
         }
 
         let mut assumps = vec![];
         self.lit_buffer.iter().try_for_each(|(&l, &w)| {
             if w <= ub {
                 Err(Error::NotEncoded)
@@ -248,18 +261,16 @@
     fn n_vars(&self) -> u32 {
         self.n_vars
     }
 }
 
 impl From<RsHashMap<Lit, usize>> for DbGte {
     fn from(lits: RsHashMap<Lit, usize>) -> Self {
-        let weight_sum = lits.iter().fold(0, |sum, (_, w)| sum + *w);
         Self {
             lit_buffer: lits,
-            weight_sum,
             ..Default::default()
         }
     }
 }
 
 impl FromIterator<(Lit, usize)> for DbGte {
     fn from_iter<T: IntoIterator<Item = (Lit, usize)>>(iter: T) -> Self {
@@ -267,15 +278,14 @@
         Self::from(lits)
     }
 }
 
 impl Extend<(Lit, usize)> for DbGte {
     fn extend<T: IntoIterator<Item = (Lit, usize)>>(&mut self, iter: T) {
         iter.into_iter().for_each(|(l, w)| {
-            self.weight_sum += w;
             // Insert into buffer to be added to tree
             match self.lit_buffer.get_mut(&l) {
                 Some(old_w) => *old_w += w,
                 None => {
                     self.lit_buffer.insert(l, w);
                 }
             };
```

### Comparing `rustsat-0.4.2/rustsat/src/encodings/pb/dpw.rs` & `rustsat-0.4.3/rustsat/src/encodings/pb/dpw.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/encodings/pb/gte.rs` & `rustsat-0.4.3/rustsat/src/encodings/pb/gte.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/encodings/pb/simulators.rs` & `rustsat-0.4.3/rustsat/src/encodings/pb/simulators.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/encodings/pb.rs` & `rustsat-0.4.3/rustsat/src/encodings/pb.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/encodings.rs` & `rustsat-0.4.3/rustsat/src/encodings.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/instances/fio/dimacs.rs` & `rustsat-0.4.3/rustsat/src/instances/fio/dimacs.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/instances/fio/opb.rs` & `rustsat-0.4.3/rustsat/src/instances/fio/opb.rs`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     pub no_negated_lits: bool,
 }
 
 impl Default for Options {
     /// Default options following the OPB specification
     fn default() -> Self {
         Self {
-            first_var_idx: 0,
+            first_var_idx: 1,
             no_negated_lits: true,
         }
     }
 }
 
 /// Possible relational operators
 #[derive(Debug, PartialEq, Eq)]
@@ -363,14 +363,20 @@
     inst: SatInstance<VM>,
     opts: Options,
 ) -> Result<(), io::Error>
 where
     W: Write,
     VM: ManageVars,
 {
+    writeln!(
+        writer,
+        "* #variable = {} #constraint= {}",
+        inst.var_manager.n_used(),
+        inst.n_clauses() + inst.cards.len() + inst.pbs.len()
+    )?;
     writeln!(writer, "* OPB file written by RustSAT")?;
     if let Some(max_var) = inst.var_manager.max_var() {
         writeln!(writer, "* maximum variable: {}", max_var)?;
     }
     writeln!(writer, "* {} clauses", inst.n_clauses())?;
     writeln!(writer, "* {} cardinality constraints", inst.cards.len())?;
     writeln!(writer, "* {} pseudo-boolean constraints", inst.pbs.len())?;
@@ -399,14 +405,20 @@
 {
     let (constrs, obj) = inst.decompose();
     let cnf = constrs.cnf;
     let cards = constrs.cards;
     let pbs = constrs.pbs;
     let mut vm = constrs.var_manager;
     let (hardened, softs) = obj.as_soft_lits(&mut vm);
+    writeln!(
+        writer,
+        "* #variable = {} #constraint= {}",
+        vm.n_used(),
+        cnf.len() + cards.len() + pbs.len()
+    )?;
     writeln!(writer, "* OPB file written by RustSAT")?;
     if let Some(max_var) = vm.max_var() {
         writeln!(writer, "* maximum variable: {}", max_var)?;
     }
     writeln!(writer, "* {} original hard clauses", cnf.len())?;
     writeln!(writer, "* {} cardinality constraints", cards.len())?;
     writeln!(writer, "* {} pseudo-boolean constraints", pbs.len())?;
@@ -445,14 +457,20 @@
     let cards = constrs.cards;
     let pbs = constrs.pbs;
     let mut vm = constrs.var_manager;
     let (hardened, objs) = objs
         .into_iter()
         .map(|o| o.as_soft_lits(&mut vm))
         .unzip::<_, _, Vec<_>, Vec<_>>();
+    writeln!(
+        writer,
+        "* #variable = {} #constraint= {}",
+        vm.n_used(),
+        cnf.len() + cards.len() + pbs.len()
+    )?;
     writeln!(writer, "* OPB file written by RustSAT")?;
     if let Some(max_var) = vm.max_var() {
         writeln!(writer, "* maximum variable: {}", max_var)?;
     }
     writeln!(writer, "* {} original hard clauses", cnf.len())?;
     writeln!(writer, "* {} cardinality constraints", cards.len())?;
     writeln!(writer, "* {} pseudo-boolean constraints", pbs.len())?;
@@ -702,53 +720,53 @@
         );
     }
 
     #[test]
     fn parse_variable() {
         assert_eq!(
             variable("x5 test", Options::default()),
-            Ok((" test", var![5]))
+            Ok((" test", var![4]))
         );
         assert_eq!(
             variable(
                 "x5 test",
                 Options {
-                    first_var_idx: 1,
+                    first_var_idx: 0,
                     no_negated_lits: true
                 }
             ),
-            Ok((" test", var![4]))
+            Ok((" test", var![5]))
         );
         assert_eq!(
             variable("x2 test", Options::default()),
-            Ok((" test", var![2]))
+            Ok((" test", var![1]))
         );
         assert_eq!(
             variable(" test\n", Options::default()),
             Err(nom::Err::Error(NomError::new(" test\n", ErrorKind::Tag)))
         );
     }
 
     #[test]
     fn parse_literal() {
         assert_eq!(
             literal("x5 test", Options::default()),
-            Ok((" test", lit![5]))
+            Ok((" test", lit![4]))
         );
         assert_eq!(
             literal("x2 test", Options::default()),
-            Ok((" test", lit![2]))
+            Ok((" test", lit![1]))
         );
         assert_eq!(
             literal("~x5 test", Options::default()),
-            Ok((" test", !lit![5]))
+            Ok((" test", !lit![4]))
         );
         assert_eq!(
             literal("~x2 test", Options::default()),
-            Ok((" test", !lit![2]))
+            Ok((" test", !lit![1]))
         );
     }
 
     #[test]
     fn parse_operator() {
         assert_eq!(operator("<= test"), Ok((" test", OpbOperator::LE)));
         assert_eq!(operator(">= test"), Ok((" test", OpbOperator::GE)));
@@ -764,35 +782,35 @@
         assert_eq!(weight("-5 test"), Ok((" test", -5)));
     }
 
     #[test]
     fn parse_weighted_literal() {
         assert_eq!(
             weighted_literal("5 x1 test", Options::default()),
-            Ok(("test", (lit![1], 5)))
+            Ok(("test", (lit![0], 5)))
         );
         assert_eq!(
             weighted_literal("-5  x1 test", Options::default()),
-            Ok(("test", (lit![1], -5)))
+            Ok(("test", (lit![0], -5)))
         );
         assert_eq!(
             weighted_literal("5 ~x1  test", Options::default()),
-            Ok(("test", (!lit![1], 5)))
+            Ok(("test", (!lit![0], 5)))
         );
         assert_eq!(
             weighted_literal("-5 ~x1 test", Options::default()),
-            Ok(("test", (!lit![1], -5)))
+            Ok(("test", (!lit![0], -5)))
         );
     }
 
     #[test]
     fn parse_weighted_lit_sum() {
         assert_eq!(
             weighted_lit_sum("5  x1    -3 ~x2  test", Options::default()),
-            Ok(("test", vec![(lit![1], 5), (!lit![2], -3)]))
+            Ok(("test", vec![(lit![0], 5), (!lit![1], -3)]))
         );
     }
 
     #[test]
     fn parse_opb_ending() {
         assert_eq!(opb_ending("   ; test"), Ok(("test", "   ; ")));
         assert_eq!(opb_ending("   \n test"), Ok(("test", "   \n ")));
@@ -803,15 +821,15 @@
     #[test]
     fn parse_constraint() {
         match constraint("3 x1 -2 ~x2 <= 4;", Options::default()) {
             Ok((rest, constr)) => match constr {
                 PBConstraint::UB(constr) => {
                     assert_eq!(rest, "");
                     let (lits, b) = constr.decompose();
-                    let should_be_lits = vec![(lit![1], 3), (lit![2], 2)];
+                    let should_be_lits = vec![(lit![0], 3), (lit![1], 2)];
                     assert_eq!(lits, should_be_lits);
                     assert_eq!(b, 6);
                 }
                 PBConstraint::LB(_) => panic!(),
                 PBConstraint::EQ(_) => panic!(),
             },
             Err(_) => panic!(),
@@ -821,16 +839,16 @@
     #[cfg(feature = "optimization")]
     #[test]
     fn parse_objective() {
         match objective("min: 3 x1 -2 ~x2;", Options::default()) {
             Ok((rest, obj)) => {
                 assert_eq!(rest, "");
                 let mut should_be_obj = Objective::new();
-                should_be_obj.increase_soft_lit_int(3, lit![1]);
-                should_be_obj.increase_soft_lit_int(-2, !lit![2]);
+                should_be_obj.increase_soft_lit_int(3, lit![0]);
+                should_be_obj.increase_soft_lit_int(-2, !lit![1]);
                 assert_eq!(obj, should_be_obj);
             }
             Err(_) => panic!(),
         }
         match objective("min: x0;", Options::default()) {
             Ok(_) => panic!(),
             Err(err) => assert_eq!(err, nom::Err::Error(NomError::new("x0;", ErrorKind::Eof))),
@@ -857,40 +875,40 @@
     #[cfg(feature = "optimization")]
     #[test]
     fn single_opb_data() {
         assert_eq!(
             opb_data("* test\n", Options::default()),
             Ok(("", OpbData::Cmt(String::from("* test\n"))))
         );
-        let lits = vec![(lit![1], 3), (!lit![2], -2)];
+        let lits = vec![(lit![0], 3), (!lit![1], -2)];
         let should_be_constr = PBConstraint::new_ub(lits, 4);
         assert_eq!(
             opb_data("3 x1 -2 ~x2 <= 4;\n", Options::default()),
             Ok(("", OpbData::Constr(should_be_constr)))
         );
         #[cfg(feature = "optimization")]
         {
             let mut obj = Objective::new();
             obj.increase_soft_lit_int(-3, lit![0]);
             obj.increase_soft_lit_int(4, lit![1]);
             assert_eq!(
-                opb_data("min: -3 x0 4 x1;", Options::default()),
+                opb_data("min: -3 x1 4 x2;", Options::default()),
                 Ok(("", OpbData::Obj(obj)))
             );
             assert_eq!(
-                opb_data("min: x0;", Options::default()),
-                Err(nom::Err::Error(NomError::new("x0;", ErrorKind::Eof)))
+                opb_data("min: x1;", Options::default()),
+                Err(nom::Err::Error(NomError::new("x1;", ErrorKind::Eof)))
             );
         }
     }
 
     #[cfg(feature = "optimization")]
     #[test]
     fn multi_opb_data() {
-        let data = "* test\n5 x0 -3 x1 >= 4;\nmin: 1 x0;";
+        let data = "* test\n5 x1 -3 x2 >= 4;\nmin: 1 x1;";
         let reader = Cursor::new(data);
         let reader = BufReader::new(reader);
         match parse_opb_data(reader, Options::default()) {
             Ok(data) => {
                 assert_eq!(data.len(), 3);
                 assert_eq!(data[0], OpbData::Cmt(String::from("* test\n")));
                 if let OpbData::Constr(_) = data[1] {
@@ -902,20 +920,20 @@
                     ()
                 } else {
                     panic!()
                 }
             }
             Err(_) => panic!(),
         }
-        let data = "* test\n5 x0 -3 x1 >= 4;\nmin: x0;";
+        let data = "* test\n5 x1 -3 x2 >= 4;\nmin: x1;";
         let reader = Cursor::new(data);
         let reader = BufReader::new(reader);
         assert_eq!(
             parse_opb_data(reader, Options::default()),
-            Err(Error::InvalidLine(String::from("min: x0;")))
+            Err(Error::InvalidLine(String::from("min: x1;")))
         );
     }
 
     #[test]
     fn write_parse_clause() {
         let cl = clause![!lit![0], lit![1], !lit![2]];
```

### Comparing `rustsat-0.4.2/rustsat/src/instances/fio.rs` & `rustsat-0.4.3/rustsat/src/instances/fio.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/instances/multiopt.rs` & `rustsat-0.4.3/rustsat/src/instances/multiopt.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/instances/opt.rs` & `rustsat-0.4.3/rustsat/src/instances/opt.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/instances/sat.rs` & `rustsat-0.4.3/rustsat/src/instances/sat.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/instances.rs` & `rustsat-0.4.3/rustsat/src/instances.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/lib.rs` & `rustsat-0.4.3/rustsat/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/pyapi.rs` & `rustsat-0.4.3/rustsat/src/pyapi.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/solvers/ipasir.rs` & `rustsat-0.4.3/rustsat/src/solvers/ipasir.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/solvers.rs` & `rustsat-0.4.3/rustsat/src/solvers.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/types/constraints.rs` & `rustsat-0.4.3/rustsat/src/types/constraints.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/types.rs` & `rustsat-0.4.3/rustsat/src/types.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/src/utils.rs` & `rustsat-0.4.3/rustsat/src/utils.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/tests/am1_encodings.rs` & `rustsat-0.4.3/rustsat/tests/am1_encodings.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/tests/card_encodings.rs` & `rustsat-0.4.3/rustsat/tests/card_encodings.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/tests/cnf.rs` & `rustsat-0.4.3/rustsat/tests/cnf.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/tests/compression.rs` & `rustsat-0.4.3/rustsat/tests/compression.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/tests/constraints.rs` & `rustsat-0.4.3/rustsat/tests/constraints.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/tests/opb.rs` & `rustsat-0.4.3/rustsat/tests/opb.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/tests/pb_encodings.rs` & `rustsat-0.4.3/rustsat/tests/pb_encodings.rs`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/README.md` & `rustsat-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/Cargo.lock` & `rustsat-0.4.3/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -30,31 +30,31 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.6.5"
+version = "0.6.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d664a92ecae85fd0a7392615844904654d1d5f5514837f471ddef4a057aba1b6"
+checksum = "96b09b5178381e0874812a9b157f7fe84982617e48f71f4e3235482775e5b540"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "1.0.4"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7079075b41f533b8c61d2a4d073c4676e1f8b249ff94a393b0595db304e0dd87"
+checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
 
 [[package]]
 name = "anstyle-parse"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c75ac65da39e5fe5ab759307499ddad880d724eed2f6ce5b5e8a26f4f387928c"
 dependencies = [
@@ -115,34 +115,34 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.1"
+version = "2.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "327762f6e5a765692301e5bb513e0d9fef63be86bbc14528052b1cd3e6f03e07"
+checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
 
 [[package]]
 name = "bstr"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba3569f383e8f1598449f1a423e72e99569137b47740b1da11ef19af3d5c3223"
 dependencies = [
  "lazy_static",
  "memchr",
  "regex-automata 0.1.10",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.14.0"
+version = "3.15.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f30e7476521f6f8af1a1c4c0b8cc94f0bee37d91763d0ca2665f299b6cd8aec"
+checksum = "8ea184aa71bb362a1157c896979544cc23974e08fd265f29ea96b59f0b4a555b"
 
 [[package]]
 name = "bzip2"
 version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bdb116a6ef3f6c3698828873ad02c3014b3c85cadb88496095628e3ef1e347f8"
 dependencies = [
@@ -178,105 +178,104 @@
  "syn 1.0.109",
  "tempfile",
  "toml",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.83"
+version = "1.0.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
+checksum = "7f9fa1897e4325be0d68d48df6aa1a71ac2ed4d27723887e7754192705350730"
 dependencies = [
- "jobserver",
  "libc",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.31"
+version = "0.4.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f2c685bad3eb3d45a01354cedb7d5faa66194d1d58ba6e267a8de788f79db38"
+checksum = "5bc015644b92d5890fab7489e49d21f879d5c990186827d42ec511919404f38b"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "wasm-bindgen",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.3",
 ]
 
 [[package]]
 name = "clap"
 version = "3.2.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ea181bf566f71cb9a5d17a59e1871af638180a18fb0035c92ae62b705207123"
 dependencies = [
  "atty",
  "bitflags 1.3.2",
  "clap_lex 0.2.4",
  "indexmap",
- "strsim",
+ "strsim 0.10.0",
  "termcolor",
  "textwrap",
 ]
 
 [[package]]
 name = "clap"
-version = "4.4.14"
+version = "4.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "33e92c5c1a78c62968ec57dbc2440366a2d6e5a23faf829970ff1585dc6b18e2"
+checksum = "c918d541ef2913577a0f9566e9ce27cb35b6df072075769e0b26cb5a554520da"
 dependencies = [
  "clap_builder",
  "clap_derive",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.4.14"
+version = "4.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f4323769dc8a61e2c39ad7dc26f6f2800524691a44d74fe3d1071a5c24db6370"
+checksum = "9f3e7391dad68afb0c2ede1bf619f579a3dc9c2ec67f089baa397123a2f3d1eb"
 dependencies = [
  "anstream",
  "anstyle",
- "clap_lex 0.6.0",
- "strsim",
+ "clap_lex 0.7.0",
+ "strsim 0.11.0",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.4.7"
+version = "4.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf9804afaaf59a91e75b022a30fb7229a7901f60c755489cc61c9b423b836442"
+checksum = "307bc0538d5f0f83b8248db3087aa92fe504e4691294d0c96c0eabc33f47ba47"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.50",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
 dependencies = [
  "os_str_bytes",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.6.0"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "702fc72eb24e5a1e48ce58027a675bc24edd52096d5397d4aea7c6dd9eca0bd1"
+checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
 
 [[package]]
 name = "cmake"
 version = "0.1.50"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a31c789563b815f77f4250caee12365734369f942439b7defd71e18a48197130"
 dependencies = [
@@ -302,15 +301,15 @@
 
 [[package]]
 name = "concolor-clap"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435ff0007a3bb04099fe1beedc6b76e7dd5340c90b168008ac0d7e87441de1bf"
 dependencies = [
- "clap 4.4.14",
+ "clap 4.5.1",
  "concolor",
 ]
 
 [[package]]
 name = "concolor-query"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -333,17 +332,17 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "crc32fast"
-version = "1.3.2"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
+checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "difflib"
 version = "0.4.0"
@@ -354,17 +353,17 @@
 name = "doc-comment"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fea41bba32d969b513997752735605054bc0dfa92b4c56bf1189f2e174be7a10"
 
 [[package]]
 name = "either"
-version = "1.9.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
+checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
 [[package]]
 name = "errno"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
 dependencies = [
@@ -416,19 +415,19 @@
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "git2"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbf97ba92db08df386e10c8ede66a2a0369bd277090afd8710e19e38de9ec0cd"
+checksum = "1b3ba52851e73b46a4c3df1d89343741112003f0f6f13beb0dfac9e457c3fdcd"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.4.2",
  "libc",
  "libgit2-sys",
  "log",
  "openssl-probe",
  "openssl-sys",
  "url",
 ]
@@ -458,23 +457,23 @@
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.3"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d77f7ec81a6d05a3abb01ab6eb7590f6083d08449fe5a1c8b1e620283546ccb7"
+checksum = "bd5256b483761cd23699d0da46cc6fd2ee3be420bbe6d020ae4a091e70b7e9fd"
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.59"
+version = "0.1.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b6a67363e2aa4443928ce15e57ebae94fd8949958fd1223c4cfc0cd473ad7539"
+checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
  "windows-core",
@@ -541,20 +540,20 @@
  "proc-macro2",
  "quote",
  "rustc_version",
 ]
 
 [[package]]
 name = "is-terminal"
-version = "0.4.10"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0bad00257d07be169d870ab665980b06cdb366d792ad690bf2e76876dc503455"
+checksum = "f23ff5ef2b80d608d61efee834934d862cd92461afc0560dedf493e4c033738b"
 dependencies = [
- "hermit-abi 0.3.3",
- "rustix",
+ "hermit-abi 0.3.6",
+ "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -566,48 +565,39 @@
 [[package]]
 name = "itoa"
 version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
 
 [[package]]
-name = "jobserver"
-version = "0.1.27"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c37f63953c4c63420ed5fd3d6d398c719489b9f872b9fa683262f8edd363c7d"
-dependencies = [
- "libc",
-]
-
-[[package]]
 name = "js-sys"
-version = "0.3.66"
+version = "0.3.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cee9c64da59eae3b50095c18d3e74f8b73c0b86d2792824ff01bbce68ba229ca"
+checksum = "406cda4b368d531c842222cf9d2600a9a4acce8d29423695379c6868a143a9ee"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.152"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13e3bf6590cbc649f4d1a3eefc9d5d6eb746f5200ffb04e5e142700b8faa56e7"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libgit2-sys"
-version = "0.16.1+1.7.1"
+version = "0.16.2+1.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f2a2bb3680b094add03bb3732ec520ece34da31a8cd2d633d1389d0f0fb60d0c"
+checksum = "ee4126d8b4ee5c9d9ea891dd875cfdc1e9d0950437179104b183d7d8a74d24e8"
 dependencies = [
  "cc",
  "libc",
  "libssh2-sys",
  "libz-sys",
  "openssl-sys",
  "pkg-config",
@@ -625,39 +615,39 @@
  "openssl-sys",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
 name = "libz-ng-sys"
-version = "1.1.14"
+version = "1.1.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "81157dde2fd4ad2b45ea3a4bb47b8193b52a6346b678840d91d80d3c2cd166c5"
+checksum = "c6409efc61b12687963e602df8ecf70e8ddacf95bc6576bcf16e3ac6328083c5"
 dependencies = [
  "cmake",
  "libc",
 ]
 
 [[package]]
 name = "libz-sys"
-version = "1.1.14"
+version = "1.1.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "295c17e837573c8c821dbaeb3cceb3d745ad082f7572191409e69cbc1b3fd050"
+checksum = "037731f5d3aaa87a5675e895b63ddff1a87624bc29f77004ea829809654e48f6"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.4.12"
+version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4cd1a83af159aa67994778be9070f0ae1bd732942279cabb14f86f986a21456"
+checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
 name = "lock_api"
 version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
@@ -701,17 +691,17 @@
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "nom"
 version = "7.1.3"
@@ -726,17 +716,17 @@
 name = "normalize-line-endings"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "61807f77802ff30975e01f4f071c8ba10c022052f98b3294119f3e615d13e5be"
 
 [[package]]
 name = "num-traits"
-version = "0.2.17"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39e3200413f237f41ab11ad6d161bc7239c84dcb631773ccd7de3dfe4b5c267c"
+checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.19.0"
@@ -747,17 +737,17 @@
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.98"
+version = "0.9.101"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1665caf8ab2dc9aef43d1c0023bd904633a6a05cb30b0ad59bec2ae986e57a7"
+checksum = "dda2b0f344e78efc2facf7d195d098df0dd72151b26ab98da807afc26c198dff"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
@@ -794,28 +784,28 @@
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pest"
-version = "2.7.6"
+version = "2.7.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f200d8d83c44a45b21764d1916299752ca035d15ecd46faca3e9a2a2bf6ad06"
+checksum = "219c0dcc30b6a27553f9cc242972b67f75b60eb0db71f0b5462f38b058c41546"
 dependencies = [
  "memchr",
  "thiserror",
  "ucd-trie",
 ]
 
 [[package]]
 name = "pkg-config"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69d3587f8a9e599cc7ec2c00e331f71c4e69a5f9a4b8a6efd5b07466b9736f9a"
+checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
@@ -847,17 +837,17 @@
 dependencies = [
  "predicates-core",
  "termtree",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.76"
+version = "1.0.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95fc56cda0b5c3325f5fbbd7ff9fda9e02bb00bb3dac51252d2f1bfa1cb8cc8c"
+checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.20.2"
@@ -878,15 +868,15 @@
 [[package]]
 name = "pyo3-build-config"
 version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07426f0d8fe5a601f26293f300afd1a7b1ed5e78b2a705870c5f30893c5163be"
 dependencies = [
  "once_cell",
- "target-lexicon 0.12.13",
+ "target-lexicon 0.12.14",
 ]
 
 [[package]]
 name = "pyo3-ffi"
 version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dbb7dec17e17766b46bca4f1a4215a85006b4c2ecde122076c562dd058da6cf1"
@@ -900,27 +890,27 @@
 version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05f738b4e40d50b5711957f142878cfa0f28e054aa0ebdfc3fd137a843f74ed3"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.50",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fc910d4851847827daf9d6cdd4a823fbdaab5b8818325c5e97a86da79e8881f"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.50",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
@@ -965,35 +955,35 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.2"
+version = "1.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "380b951a9c5e80ddfd6136919eef32310721aa4aacd4889a8d39124b026ab343"
+checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-automata 0.4.3",
+ "regex-automata 0.4.5",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 
 [[package]]
 name = "regex-automata"
-version = "0.4.3"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f804c7828047e88b2d32e2d7fe5a105da8ee3264f01902f796c8e067dc2483f"
+checksum = "5bb987efffd3c6d0d8f5f89510bb458559eab11e4f869acb20bf845e016259cd"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
@@ -1015,28 +1005,28 @@
 checksum = "f0dfe2087c51c460008730de8b57e6a320782fbfb312e1f4d520e6c6fae155ee"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.28"
+version = "0.38.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72e572a5e8ca657d7366229cdde4bd14c4eb5499a9573d4d366fe1b599daa316"
+checksum = "6ea3e1a662af26cd7a3ba09c0297a31af215563ecf42817c98df621387f4e949"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.4.2",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustsat"
-version = "0.4.2"
+version = "0.4.3"
 dependencies = [
  "bzip2",
  "cbindgen",
  "cpu-time",
  "flate2",
  "inline-c",
  "nom",
@@ -1049,83 +1039,83 @@
  "thiserror",
  "visibility",
  "xz2",
 ]
 
 [[package]]
 name = "rustsat-cadical"
-version = "0.2.3"
+version = "0.2.4"
 dependencies = [
  "cc",
  "chrono",
  "cpu-time",
  "git2",
  "glob",
  "rustsat",
 ]
 
 [[package]]
 name = "rustsat-glucose"
-version = "0.2.3"
+version = "0.2.4"
 dependencies = [
  "cc",
  "chrono",
  "cmake",
  "cpu-time",
  "git2",
  "glob",
  "rustsat",
 ]
 
 [[package]]
 name = "rustsat-kissat"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = [
  "cc",
  "chrono",
  "cpu-time",
  "git2",
  "glob",
  "rustsat",
 ]
 
 [[package]]
 name = "rustsat-minisat"
-version = "0.2.3"
+version = "0.2.4"
 dependencies = [
  "cc",
  "chrono",
  "cmake",
  "cpu-time",
  "git2",
  "glob",
  "rustsat",
 ]
 
 [[package]]
 name = "rustsat-tools"
-version = "0.2.3"
+version = "0.2.4"
 dependencies = [
  "atty",
- "clap 4.4.14",
+ "clap 4.5.1",
  "concolor-clap",
  "nom",
  "rand",
  "rand_chacha",
  "rustsat",
  "rustsat-cadical",
  "rustsat-minisat",
  "termcolor",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.16"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f98d2aa92eebf49b69786be48e4477826b256916e84a57ff2a4f21923b48eb4c"
+checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
@@ -1145,98 +1135,103 @@
 checksum = "00b0bef5b7f9e0df16536d3961cfb6e84331c065b4066afb39768d0e319411f7"
 dependencies = [
  "pest",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.195"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "63261df402c67811e9ac6def069e4786148c4563f4b50fd4bf30aa370d626b02"
+checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.195"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46fe8f8603d81ba86327b23a2e9cdf49e1255fb94a4c5f297f6ee0547178ea2c"
+checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.50",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.111"
+version = "1.0.114"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "176e46fa42316f18edd598015a5166857fc835ec732f5215eac6b7bdbf0a84f4"
+checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.11.2"
+version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dccd0940a2dcdf68d092b8cbab7dc0ad8fa938bf95787e1b916b0e3d0e8e970"
+checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
 
 [[package]]
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
+name = "strsim"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ee073c9e4cd00e28217186dbe12796d692868f432bf2e97ee73bed0c56dfa01"
+
+[[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.48"
+version = "2.0.50"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f3531638e407dfc0814761abb7c00a5b54992b849452a0646b7f65c9f770f3f"
+checksum = "74f1bdc9872430ce9b75da68329d1c1746faf50ffac5f19e02b71e37ff881ffb"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "422045212ea98508ae3d28025bc5aaa2bd4a9cdaecd442a08da2ee620ee9ea95"
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.13"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69758bda2e78f098e4ccb393021a0963bb3442eac05f135c30f61b7370bbafae"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tempfile"
-version = "3.9.0"
+version = "3.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01ce4141aa927a6d1bd34a041795abd0db1cccba5d5f24b009f694bdf3a1f3fa"
+checksum = "a365e8cd18e44762ef95d87f284f4b5cd04107fec2ff3052bd6a3e6069669e67"
 dependencies = [
  "cfg-if",
  "fastrand",
- "redox_syscall",
  "rustix",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "termcolor"
 version = "1.4.1"
@@ -1250,36 +1245,36 @@
 name = "termtree"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3369f5ac52d5eb6ab48c6b4ffdc8efbcad6b89c765749064ba298f2c68a16a76"
 
 [[package]]
 name = "textwrap"
-version = "0.16.0"
+version = "0.16.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
+checksum = "23d434d3f8967a09480fb04132ebe0a3e088c173e6d0ee7897abbdf4eab0f8b9"
 
 [[package]]
 name = "thiserror"
-version = "1.0.56"
+version = "1.0.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d54378c645627613241d077a3a79db965db602882668f9136ac42af9ecb730ad"
+checksum = "1e45bcbe8ed29775f228095caf2cd67af7a4ccf756ebff23a306bf3e8b47b24b"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.56"
+version = "1.0.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa0faa943b50f3db30a20aa7e265dbc66076993efed8463e8de414e5d06d3471"
+checksum = "a953cb265bef375dae3de6663da4d3804eee9682ea80d8e2542529b73c531c81"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.50",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
@@ -1306,29 +1301,29 @@
 name = "ucd-trie"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed646292ffc8188ef8ea4d1e0e0150fb15a5c2e12ad9b8fc191ae7a8a7f3c4b9"
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.14"
+version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f2528f27a9eb2b21e69c95319b30bd0efd85d09c379741b0f78ea1d86be2416"
+checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-normalization"
-version = "0.1.22"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unindent"
 version = "0.2.3"
@@ -1362,15 +1357,15 @@
 name = "visibility"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b3fd98999db9227cf28e59d83e1f120f42bc233d4b152e8fab9bc87d5bb1e0f8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.50",
 ]
 
 [[package]]
 name = "wait-timeout"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f200f5b12eb75f8c1ed65abd4b2db8a6e1b138a20de009dacee265a2498f3f6"
@@ -1382,65 +1377,65 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.89"
+version = "0.2.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0ed0d4f68a3015cc185aff4db9506a015f4b96f95303897bfa23f846db54064e"
+checksum = "c1e124130aee3fb58c5bdd6b639a0509486b0338acaaae0c84a5124b0f588b7f"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.89"
+version = "0.2.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b56f625e64f3a1084ded111c4d5f477df9f8c92df113852fa5a374dbda78826"
+checksum = "c9e7e1900c352b609c8488ad12639a311045f40a35491fb69ba8c12f758af70b"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.50",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.89"
+version = "0.2.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0162dbf37223cd2afce98f3d0785506dcb8d266223983e4b5b525859e6e182b2"
+checksum = "b30af9e2d358182b5c7449424f017eba305ed32a7010509ede96cdc4696c46ed"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.89"
+version = "0.2.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0eb82fcb7930ae6219a7ecfd55b217f5f0893484b7a13022ebb2b2bf20b5283"
+checksum = "642f325be6301eb8107a83d12a8ac6c1e1c54345a7ef1a9261962dfefda09e66"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.50",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.89"
+version = "0.2.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ab9b36309365056cd639da3134bf87fa8f3d86008abf99e612384a6eecd459f"
+checksum = "4f186bd2dcf04330886ce82d6f33dd75a7bfcf69ecf5763b89fcde53b6ac9838"
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
@@ -1471,15 +1466,15 @@
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.0",
+ "windows-targets 0.52.3",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
@@ -1489,15 +1484,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.0",
+ "windows-targets 0.52.3",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
@@ -1524,25 +1519,25 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.0"
+version = "0.52.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a18201040b24831fbb9e4eb208f8892e1f50a37feb53cc7ff887feb8f50e7cd"
+checksum = "d380ba1dc7187569a8a9e91ed34b8ccfc33123bbacb8c0aed2d1ad7f3ef2dc5f"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.0",
- "windows_aarch64_msvc 0.52.0",
- "windows_i686_gnu 0.52.0",
- "windows_i686_msvc 0.52.0",
- "windows_x86_64_gnu 0.52.0",
- "windows_x86_64_gnullvm 0.52.0",
- "windows_x86_64_msvc 0.52.0",
+ "windows_aarch64_gnullvm 0.52.3",
+ "windows_aarch64_msvc 0.52.3",
+ "windows_i686_gnu 0.52.3",
+ "windows_i686_msvc 0.52.3",
+ "windows_x86_64_gnu 0.52.3",
+ "windows_x86_64_gnullvm 0.52.3",
+ "windows_x86_64_msvc 0.52.3",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
@@ -1551,17 +1546,17 @@
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.0"
+version = "0.52.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb7764e35d4db8a7921e09562a0304bf2f93e0a51bfccee0bd0bb0b666b015ea"
+checksum = "68e5dcfb9413f53afd9c8f86e56a7b4d86d9a2fa26090ea2dc9e40fba56c6ec6"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
@@ -1569,17 +1564,17 @@
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.0"
+version = "0.52.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbaa0368d4f1d2aaefc55b6fcfee13f41544ddf36801e793edbbfd7d7df075ef"
+checksum = "8dab469ebbc45798319e69eebf92308e541ce46760b49b18c6b3fe5e8965b30f"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
@@ -1587,17 +1582,17 @@
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.0"
+version = "0.52.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a28637cb1fa3560a16915793afb20081aba2c92ee8af57b4d5f28e4b3e7df313"
+checksum = "2a4e9b6a7cac734a8b4138a4e1044eac3404d8326b6c0f939276560687a033fb"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
@@ -1605,17 +1600,17 @@
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.0"
+version = "0.52.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffe5e8e31046ce6230cc7215707b816e339ff4d4d67c65dffa206fd0f7aa7b9a"
+checksum = "28b0ec9c422ca95ff34a78755cfa6ad4a51371da2a5ace67500cf7ca5f232c58"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
@@ -1623,17 +1618,17 @@
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.0"
+version = "0.52.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d6fa32db2bc4a2f5abeacf2b69f7992cd09dca97498da74a151a3132c26befd"
+checksum = "704131571ba93e89d7cd43482277d6632589b18ecf4468f591fbae0a8b101614"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
@@ -1641,17 +1636,17 @@
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.0"
+version = "0.52.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a657e1e9d3f514745a572a6846d3c7aa7dbe1658c056ed9c3344c4109a6949e"
+checksum = "42079295511643151e98d61c38c0acc444e52dd42ab456f7ccfd5152e8ecf21c"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
@@ -1659,17 +1654,17 @@
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.0"
+version = "0.52.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
+checksum = "0770833d60a970638e989b3fa9fd2bb1aaadcf88963d1659fd7d9990196ed2d6"
 
 [[package]]
 name = "xz2"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "388c44dc09d76f1536602ead6d325eb532f5c122f17782bd57fb47baeeb767e2"
 dependencies = [
```

### Comparing `rustsat-0.4.2/rustsat/__init__.pyi` & `rustsat-0.4.3/rustsat/__init__.pyi`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/rustsat/encodings/__init__.pyi` & `rustsat-0.4.3/rustsat/encodings/__init__.pyi`

 * *Files identical despite different names*

### Comparing `rustsat-0.4.2/PKG-INFO` & `rustsat-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustsat
-Version: 0.4.2
+Version: 0.4.3
 Summary: This library aims to provide implementations of elements commonly used in the development on software in the area of satisfiability solving. The focus of the library is to provide as much ease of use without giving up on performance.
 Keywords: sat,satisfiability,encodings
 Author: Christoph Jabs <christoph.jabs@helsinki.fi>
 Author-email: Christoph Jabs <christoph.jabs@helsinki.fi>
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

