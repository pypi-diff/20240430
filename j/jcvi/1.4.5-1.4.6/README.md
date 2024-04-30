# Comparing `tmp/jcvi-1.4.5.tar.gz` & `tmp/jcvi-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcvi-1.4.5.tar", last modified: Mon Apr 29 06:37:24 2024, max compression
+gzip compressed data, was "jcvi-1.4.6.tar", last modified: Tue Apr 30 16:08:55 2024, max compression
```

## Comparing `jcvi-1.4.5.tar` & `jcvi-1.4.6.tar`

### file list

```diff
@@ -1,208 +1,207 @@
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.136548 jcvi-1.4.5/
--rw-r--r--   0 bao        (501) staff       (20)     1292 2020-03-03 07:11:04.000000 jcvi-1.4.5/LICENSE
--rw-r--r--   0 bao        (501) staff       (20)       91 2022-11-27 15:24:30.000000 jcvi-1.4.5/MANIFEST.in
--rw-r--r--   0 bao        (501) staff       (20)     8915 2024-04-29 06:37:24.136638 jcvi-1.4.5/PKG-INFO
--rw-r--r--   0 bao        (501) staff       (20)     8250 2023-07-25 21:30:23.000000 jcvi-1.4.5/README.md
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.111129 jcvi-1.4.5/jcvi/
--rw-r--r--   0 bao        (501) staff       (20)      770 2022-11-26 21:23:29.000000 jcvi-1.4.5/jcvi/__init__.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.113130 jcvi-1.4.5/jcvi/algorithms/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/algorithms/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      263 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/algorithms/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)     6422 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/algorithms/ec.py
--rw-r--r--   0 bao        (501) staff       (20)     6412 2024-04-28 07:29:54.000000 jcvi-1.4.5/jcvi/algorithms/formula.py
--rw-r--r--   0 bao        (501) staff       (20)    14132 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/algorithms/graph.py
--rwxr-xr-x   0 bao        (501) staff       (20)     6275 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/algorithms/lis.py
--rwxr-xr-x   0 bao        (501) staff       (20)    24228 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/algorithms/lpsolve.py
--rw-r--r--   0 bao        (501) staff       (20)     6104 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/algorithms/matrix.py
--rw-r--r--   0 bao        (501) staff       (20)     1296 2021-06-19 19:45:56.000000 jcvi-1.4.5/jcvi/algorithms/maxsum.py
--rwxr-xr-x   0 bao        (501) staff       (20)     4999 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/algorithms/supermap.py
--rw-r--r--   0 bao        (501) staff       (20)    12559 2022-11-26 15:55:17.000000 jcvi-1.4.5/jcvi/algorithms/tsp.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.114664 jcvi-1.4.5/jcvi/annotation/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/annotation/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      261 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/annotation/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    21414 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/annotation/ahrd.py
--rw-r--r--   0 bao        (501) staff       (20)     7899 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/annotation/automaton.py
--rwxr-xr-x   0 bao        (501) staff       (20)     6417 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/annotation/depth.py
--rw-r--r--   0 bao        (501) staff       (20)     7042 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/annotation/evm.py
--rw-r--r--   0 bao        (501) staff       (20)    14687 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/annotation/maker.py
--rw-r--r--   0 bao        (501) staff       (20)    19485 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/annotation/pasa.py
--rw-r--r--   0 bao        (501) staff       (20)    12822 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/annotation/qc.py
--rw-r--r--   0 bao        (501) staff       (20)    42839 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/annotation/reformat.py
--rw-r--r--   0 bao        (501) staff       (20)    12645 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/annotation/stats.py
--rw-r--r--   0 bao        (501) staff       (20)     6793 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/annotation/train.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.117447 jcvi-1.4.5/jcvi/apps/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/apps/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      258 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/apps/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    20591 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/apps/align.py
--rw-r--r--   0 bao        (501) staff       (20)    68344 2024-04-28 07:29:54.000000 jcvi-1.4.5/jcvi/apps/base.py
--rw-r--r--   0 bao        (501) staff       (20)    12271 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/biomart.py
--rwxr-xr-x   0 bao        (501) staff       (20)     3554 2021-06-19 19:45:56.000000 jcvi-1.4.5/jcvi/apps/blastplus.py
--rw-r--r--   0 bao        (501) staff       (20)     5219 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/bowtie.py
--rw-r--r--   0 bao        (501) staff       (20)     7695 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/bwa.py
--rw-r--r--   0 bao        (501) staff       (20)     7279 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/cdhit.py
--rw-r--r--   0 bao        (501) staff       (20)     2623 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/emboss.py
--rw-r--r--   0 bao        (501) staff       (20)    21333 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/apps/fetch.py
--rw-r--r--   0 bao        (501) staff       (20)    19459 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/gbsubmit.py
--rw-r--r--   0 bao        (501) staff       (20)     6892 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/gmap.py
--rw-r--r--   0 bao        (501) staff       (20)    18477 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/apps/grid.py
--rwxr-xr-x   0 bao        (501) staff       (20)     7238 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/lastz.py
--rwxr-xr-x   0 bao        (501) staff       (20)     3004 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/mask.py
--rw-r--r--   0 bao        (501) staff       (20)    35471 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/phylo.py
--rw-r--r--   0 bao        (501) staff       (20)     1896 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/r.py
--rw-r--r--   0 bao        (501) staff       (20)     4901 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/restriction.py
--rw-r--r--   0 bao        (501) staff       (20)     3784 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/softlink.py
--rw-r--r--   0 bao        (501) staff       (20)    33065 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/uclust.py
--rw-r--r--   0 bao        (501) staff       (20)     5208 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/uniprot.py
--rw-r--r--   0 bao        (501) staff       (20)     3661 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/apps/vecscreen.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.120301 jcvi-1.4.5/jcvi/assembly/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/assembly/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      257 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/assembly/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    66136 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/allmaps.py
--rw-r--r--   0 bao        (501) staff       (20)    15451 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/allpaths.py
--rw-r--r--   0 bao        (501) staff       (20)    13265 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/automaton.py
--rw-r--r--   0 bao        (501) staff       (20)     5544 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/base.py
--rw-r--r--   0 bao        (501) staff       (20)    34986 2023-11-24 05:16:26.000000 jcvi-1.4.5/jcvi/assembly/ca.py
--rw-r--r--   0 bao        (501) staff       (20)     3457 2022-09-27 05:18:33.000000 jcvi-1.4.5/jcvi/assembly/chic.pyx
--rw-r--r--   0 bao        (501) staff       (20)     4581 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/coverage.py
--rw-r--r--   0 bao        (501) staff       (20)     8676 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/gaps.py
--rw-r--r--   0 bao        (501) staff       (20)    20002 2024-04-29 06:10:52.000000 jcvi-1.4.5/jcvi/assembly/geneticmap.py
--rw-r--r--   0 bao        (501) staff       (20)    34692 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/assembly/goldenpath.py
--rw-r--r--   0 bao        (501) staff       (20)    56167 2024-04-29 06:10:52.000000 jcvi-1.4.5/jcvi/assembly/hic.py
--rw-r--r--   0 bao        (501) staff       (20)    43034 2024-04-29 06:10:52.000000 jcvi-1.4.5/jcvi/assembly/kmer.py
--rw-r--r--   0 bao        (501) staff       (20)    12519 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/opticalmap.py
--rw-r--r--   0 bao        (501) staff       (20)    27279 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/patch.py
--rw-r--r--   0 bao        (501) staff       (20)    15741 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/postprocess.py
--rw-r--r--   0 bao        (501) staff       (20)    23472 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/assembly/preprocess.py
--rw-r--r--   0 bao        (501) staff       (20)     6287 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/sim.py
--rw-r--r--   0 bao        (501) staff       (20)     8830 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/soap.py
--rw-r--r--   0 bao        (501) staff       (20)    16183 2023-04-26 05:51:28.000000 jcvi-1.4.5/jcvi/assembly/syntenypath.py
--rw-r--r--   0 bao        (501) staff       (20)     5042 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/assembly/trinity.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.121981 jcvi-1.4.5/jcvi/compara/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/compara/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      251 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/compara/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)     4218 2023-09-28 09:59:53.000000 jcvi-1.4.5/jcvi/compara/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)     9796 2023-04-26 05:51:28.000000 jcvi-1.4.5/jcvi/compara/blastfilter.py
--rw-r--r--   0 bao        (501) staff       (20)    28698 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/compara/catalog.py
--rw-r--r--   0 bao        (501) staff       (20)    26355 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/compara/fractionation.py
--rw-r--r--   0 bao        (501) staff       (20)    33945 2024-04-29 06:10:52.000000 jcvi-1.4.5/jcvi/compara/ks.py
--rw-r--r--   0 bao        (501) staff       (20)     9216 2023-04-26 05:51:28.000000 jcvi-1.4.5/jcvi/compara/pad.py
--rw-r--r--   0 bao        (501) staff       (20)     8322 2024-04-29 06:10:52.000000 jcvi-1.4.5/jcvi/compara/pedigree.py
--rw-r--r--   0 bao        (501) staff       (20)     3051 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/compara/phylogeny.py
--rwxr-xr-x   0 bao        (501) staff       (20)     7948 2023-04-26 05:51:28.000000 jcvi-1.4.5/jcvi/compara/quota.py
--rw-r--r--   0 bao        (501) staff       (20)    10341 2023-04-26 05:51:28.000000 jcvi-1.4.5/jcvi/compara/reconstruct.py
--rwxr-xr-x   0 bao        (501) staff       (20)     9233 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/compara/synfind.py
--rwxr-xr-x   0 bao        (501) staff       (20)    57574 2023-04-26 05:51:28.000000 jcvi-1.4.5/jcvi/compara/synteny.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.125211 jcvi-1.4.5/jcvi/formats/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/formats/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      262 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/formats/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    63559 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/formats/agp.py
--rw-r--r--   0 bao        (501) staff       (20)    33830 2023-09-28 09:59:53.000000 jcvi-1.4.5/jcvi/formats/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)    75125 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/formats/bed.py
--rw-r--r--   0 bao        (501) staff       (20)    43184 2023-06-19 14:46:14.000000 jcvi-1.4.5/jcvi/formats/blast.py
--rw-r--r--   0 bao        (501) staff       (20)     7010 2022-09-27 05:18:33.000000 jcvi-1.4.5/jcvi/formats/cblast.pyx
--rw-r--r--   0 bao        (501) staff       (20)     3193 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/formats/cdt.py
--rw-r--r--   0 bao        (501) staff       (20)     8612 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/formats/chain.py
--rw-r--r--   0 bao        (501) staff       (20)     4644 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/formats/contig.py
--rw-r--r--   0 bao        (501) staff       (20)    15169 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/formats/coords.py
--rw-r--r--   0 bao        (501) staff       (20)     6529 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/formats/excel.py
--rw-r--r--   0 bao        (501) staff       (20)    75591 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/formats/fasta.py
--rw-r--r--   0 bao        (501) staff       (20)    29575 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/formats/fastq.py
--rw-r--r--   0 bao        (501) staff       (20)    15545 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/formats/genbank.py
--rw-r--r--   0 bao        (501) staff       (20)   120223 2024-04-05 14:11:25.000000 jcvi-1.4.5/jcvi/formats/gff.py
--rw-r--r--   0 bao        (501) staff       (20)     3979 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/formats/html.py
--rw-r--r--   0 bao        (501) staff       (20)     4612 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/formats/maf.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2842 2021-07-05 22:45:00.000000 jcvi-1.4.5/jcvi/formats/obo.py
--rw-r--r--   0 bao        (501) staff       (20)     2900 2021-01-11 06:59:36.000000 jcvi-1.4.5/jcvi/formats/paf.py
--rw-r--r--   0 bao        (501) staff       (20)     2783 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/formats/pdf.py
--rwxr-xr-x   0 bao        (501) staff       (20)    10355 2023-11-24 05:16:26.000000 jcvi-1.4.5/jcvi/formats/psl.py
--rw-r--r--   0 bao        (501) staff       (20)     2746 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/formats/pyblast.py
--rw-r--r--   0 bao        (501) staff       (20)    28231 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/formats/sam.py
--rw-r--r--   0 bao        (501) staff       (20)     8041 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/formats/sizes.py
--rw-r--r--   0 bao        (501) staff       (20)    25480 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/formats/vcf.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.127800 jcvi-1.4.5/jcvi/graphics/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/graphics/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      271 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/graphics/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    16271 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/graphics/align.py
--rw-r--r--   0 bao        (501) staff       (20)    15265 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/graphics/assembly.py
--rw-r--r--   0 bao        (501) staff       (20)    24647 2024-04-29 06:10:52.000000 jcvi-1.4.5/jcvi/graphics/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)    10002 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/graphics/blastplot.py
--rw-r--r--   0 bao        (501) staff       (20)    22341 2024-04-29 06:10:52.000000 jcvi-1.4.5/jcvi/graphics/chromosome.py
--rw-r--r--   0 bao        (501) staff       (20)     7145 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/graphics/coverage.py
--rwxr-xr-x   0 bao        (501) staff       (20)    14873 2023-04-26 05:51:28.000000 jcvi-1.4.5/jcvi/graphics/dotplot.py
--rw-r--r--   0 bao        (501) staff       (20)    21810 2023-02-06 05:16:46.000000 jcvi-1.4.5/jcvi/graphics/glyph.py
--rw-r--r--   0 bao        (501) staff       (20)    24862 2024-04-24 05:29:17.000000 jcvi-1.4.5/jcvi/graphics/grabseeds.py
--rw-r--r--   0 bao        (501) staff       (20)     5025 2021-03-26 15:38:36.000000 jcvi-1.4.5/jcvi/graphics/heatmap.py
--rw-r--r--   0 bao        (501) staff       (20)     9610 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/graphics/histogram.py
--rw-r--r--   0 bao        (501) staff       (20)    13375 2023-02-08 03:44:09.000000 jcvi-1.4.5/jcvi/graphics/karyotype.py
--rw-r--r--   0 bao        (501) staff       (20)    32418 2024-04-29 06:10:52.000000 jcvi-1.4.5/jcvi/graphics/landscape.py
--rw-r--r--   0 bao        (501) staff       (20)     3893 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/graphics/mummerplot.py
--rw-r--r--   0 bao        (501) staff       (20)    22507 2024-02-08 05:51:57.000000 jcvi-1.4.5/jcvi/graphics/synteny.py
--rw-r--r--   0 bao        (501) staff       (20)     5488 2021-06-19 19:45:56.000000 jcvi-1.4.5/jcvi/graphics/table.py
--rw-r--r--   0 bao        (501) staff       (20)    20377 2022-11-26 16:06:34.000000 jcvi-1.4.5/jcvi/graphics/tree.py
--rw-r--r--   0 bao        (501) staff       (20)     6194 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/graphics/wheel.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.129711 jcvi-1.4.5/jcvi/projects/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/projects/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/projects/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    22445 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/projects/age.py
--rw-r--r--   0 bao        (501) staff       (20)    15907 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/projects/allmaps.py
--rw-r--r--   0 bao        (501) staff       (20)     6750 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/projects/bites.py
--rw-r--r--   0 bao        (501) staff       (20)    14136 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/projects/ies.py
--rw-r--r--   0 bao        (501) staff       (20)     7050 2024-04-29 06:10:52.000000 jcvi-1.4.5/jcvi/projects/jcvi.py
--rw-r--r--   0 bao        (501) staff       (20)    22179 2024-04-29 06:10:52.000000 jcvi-1.4.5/jcvi/projects/misc.py
--rw-r--r--   0 bao        (501) staff       (20)    25024 2023-02-06 05:16:46.000000 jcvi-1.4.5/jcvi/projects/napus.py
--rw-r--r--   0 bao        (501) staff       (20)    12754 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/projects/pineapple.py
--rw-r--r--   0 bao        (501) staff       (20)    67853 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/projects/str.py
--rw-r--r--   0 bao        (501) staff       (20)    25766 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/projects/sugarcane.py
--rw-r--r--   0 bao        (501) staff       (20)    23950 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/projects/synfind.py
--rw-r--r--   0 bao        (501) staff       (20)    21554 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/projects/tgbs.py
--rw-r--r--   0 bao        (501) staff       (20)    11941 2023-04-26 05:51:28.000000 jcvi-1.4.5/jcvi/projects/vanilla.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.131265 jcvi-1.4.5/jcvi/utils/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/utils/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    24200 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/utils/aws.py
--rw-r--r--   0 bao        (501) staff       (20)    12513 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/utils/cbook.py
--rw-r--r--   0 bao        (501) staff       (20)      355 2021-01-11 02:34:49.000000 jcvi-1.4.5/jcvi/utils/console.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.135332 jcvi-1.4.5/jcvi/utils/data/
--rwxr-xr-x   0 bao        (501) staff       (20)    16912 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/Airswing.ttf
--rwxr-xr-x   0 bao        (501) staff       (20)   103940 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/Collegia.ttf
--rwxr-xr-x   0 bao        (501) staff       (20)    20468 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/HookedUp.ttf
--rw-r--r--   0 bao        (501) staff       (20)    25832 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/Humor-Sans.ttf
--rw-r--r--   0 bao        (501) staff       (20)    28065 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/TREDs.meta.csv
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      911 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/adapters.fasta
--rw-r--r--   0 bao        (501) staff       (20)     3321 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/blosum80.mat
--rw-r--r--   0 bao        (501) staff       (20)     7686 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/chrY.hg38.unique_ccn.gc
--rw-r--r--   0 bao        (501) staff       (20)      282 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/colorchecker.txt
--rw-r--r--   0 bao        (501) staff       (20)    45544 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/hg38.band.txt
--rw-r--r--   0 bao        (501) staff       (20)    11672 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/hg38.chrom.sizes
--rw-r--r--   0 bao        (501) staff       (20)     1000 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/utils/data/instance.json
--rw-r--r--   0 bao        (501) staff       (20)     9793 2024-04-29 06:36:47.000000 jcvi-1.4.5/jcvi/utils/db.py
--rw-r--r--   0 bao        (501) staff       (20)     4145 2021-01-09 20:22:53.000000 jcvi-1.4.5/jcvi/utils/ez_setup.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2884 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/utils/grouper.py
--rw-r--r--   0 bao        (501) staff       (20)    10437 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/utils/orderedcollections.py
--rw-r--r--   0 bao        (501) staff       (20)    14595 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/utils/range.py
--rw-r--r--   0 bao        (501) staff       (20)     3946 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/utils/table.py
--rw-r--r--   0 bao        (501) staff       (20)     4687 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/utils/taxonomy.py
--rw-r--r--   0 bao        (501) staff       (20)     1522 2021-07-13 05:06:52.000000 jcvi-1.4.5/jcvi/utils/validator.py
--rwxr-xr-x   0 bao        (501) staff       (20)     1377 2021-01-15 14:44:37.000000 jcvi-1.4.5/jcvi/utils/webcolors.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.136406 jcvi-1.4.5/jcvi/variation/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.5/jcvi/variation/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      259 2021-06-19 08:23:09.000000 jcvi-1.4.5/jcvi/variation/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    45321 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/variation/cnv.py
--rw-r--r--   0 bao        (501) staff       (20)     7036 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/variation/deconvolute.py
--rw-r--r--   0 bao        (501) staff       (20)     9385 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/variation/delly.py
--rw-r--r--   0 bao        (501) staff       (20)    11777 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/variation/impute.py
--rw-r--r--   0 bao        (501) staff       (20)     3478 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/variation/phase.py
--rw-r--r--   0 bao        (501) staff       (20)    10831 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/variation/snp.py
--rw-r--r--   0 bao        (501) staff       (20)    48818 2023-02-06 03:44:04.000000 jcvi-1.4.5/jcvi/variation/str.py
--rw-r--r--   0 bao        (501) staff       (20)      176 2024-04-29 06:37:23.000000 jcvi-1.4.5/jcvi/version.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-29 06:37:24.111885 jcvi-1.4.5/jcvi.egg-info/
--rw-r--r--   0 bao        (501) staff       (20)     8915 2024-04-29 06:37:24.000000 jcvi-1.4.5/jcvi.egg-info/PKG-INFO
--rw-r--r--   0 bao        (501) staff       (20)     4561 2024-04-29 06:37:24.000000 jcvi-1.4.5/jcvi.egg-info/SOURCES.txt
--rw-r--r--   0 bao        (501) staff       (20)        1 2024-04-29 06:37:24.000000 jcvi-1.4.5/jcvi.egg-info/dependency_links.txt
--rw-r--r--   0 bao        (501) staff       (20)        1 2022-11-26 21:54:22.000000 jcvi-1.4.5/jcvi.egg-info/not-zip-safe
--rw-r--r--   0 bao        (501) staff       (20)      221 2024-04-29 06:37:24.000000 jcvi-1.4.5/jcvi.egg-info/requires.txt
--rw-r--r--   0 bao        (501) staff       (20)        5 2024-04-29 06:37:24.000000 jcvi-1.4.5/jcvi.egg-info/top_level.txt
--rw-r--r--   0 bao        (501) staff       (20)      359 2022-11-26 21:23:29.000000 jcvi-1.4.5/pyproject.toml
--rw-r--r--   0 bao        (501) staff       (20)     1242 2024-04-29 06:37:24.137099 jcvi-1.4.5/setup.cfg
--rw-r--r--   0 bao        (501) staff       (20)      553 2022-11-26 21:23:29.000000 jcvi-1.4.5/setup.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.239858 jcvi-1.4.6/
+-rw-r--r--   0 bao        (501) staff       (20)     1292 2020-03-03 07:11:04.000000 jcvi-1.4.6/LICENSE
+-rw-r--r--   0 bao        (501) staff       (20)       91 2022-11-27 15:24:30.000000 jcvi-1.4.6/MANIFEST.in
+-rw-r--r--   0 bao        (501) staff       (20)     8915 2024-04-30 16:08:55.239964 jcvi-1.4.6/PKG-INFO
+-rw-r--r--   0 bao        (501) staff       (20)     8250 2024-04-30 16:06:02.000000 jcvi-1.4.6/README.md
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.205858 jcvi-1.4.6/jcvi/
+-rw-r--r--   0 bao        (501) staff       (20)      816 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/__init__.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.208632 jcvi-1.4.6/jcvi/algorithms/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/algorithms/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      263 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/algorithms/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)     6422 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/algorithms/ec.py
+-rw-r--r--   0 bao        (501) staff       (20)     6412 2024-04-28 07:29:54.000000 jcvi-1.4.6/jcvi/algorithms/formula.py
+-rw-r--r--   0 bao        (501) staff       (20)    14132 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/algorithms/graph.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     6275 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/algorithms/lis.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    24228 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/algorithms/lpsolve.py
+-rw-r--r--   0 bao        (501) staff       (20)     6104 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/algorithms/matrix.py
+-rw-r--r--   0 bao        (501) staff       (20)     1296 2021-06-19 19:45:56.000000 jcvi-1.4.6/jcvi/algorithms/maxsum.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     4999 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/algorithms/supermap.py
+-rw-r--r--   0 bao        (501) staff       (20)    12559 2022-11-26 15:55:17.000000 jcvi-1.4.6/jcvi/algorithms/tsp.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.211048 jcvi-1.4.6/jcvi/annotation/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/annotation/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      261 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/annotation/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    21414 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/annotation/ahrd.py
+-rw-r--r--   0 bao        (501) staff       (20)     7899 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/annotation/automaton.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     6417 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/annotation/depth.py
+-rw-r--r--   0 bao        (501) staff       (20)     7042 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/annotation/evm.py
+-rw-r--r--   0 bao        (501) staff       (20)    14687 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/annotation/maker.py
+-rw-r--r--   0 bao        (501) staff       (20)    19485 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/annotation/pasa.py
+-rw-r--r--   0 bao        (501) staff       (20)    12822 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/annotation/qc.py
+-rw-r--r--   0 bao        (501) staff       (20)    42839 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/annotation/reformat.py
+-rw-r--r--   0 bao        (501) staff       (20)    12645 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/annotation/stats.py
+-rw-r--r--   0 bao        (501) staff       (20)     6793 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/annotation/train.py
+-rw-r--r--   0 bao        (501) staff       (20)     5042 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/annotation/trinity.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.214876 jcvi-1.4.6/jcvi/apps/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/apps/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      258 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/apps/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    20591 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/apps/align.py
+-rw-r--r--   0 bao        (501) staff       (20)    66789 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/apps/base.py
+-rw-r--r--   0 bao        (501) staff       (20)    12271 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/biomart.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     3554 2021-06-19 19:45:56.000000 jcvi-1.4.6/jcvi/apps/blastplus.py
+-rw-r--r--   0 bao        (501) staff       (20)     5219 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/bowtie.py
+-rw-r--r--   0 bao        (501) staff       (20)     7695 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/bwa.py
+-rw-r--r--   0 bao        (501) staff       (20)     7279 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/cdhit.py
+-rw-r--r--   0 bao        (501) staff       (20)     2623 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/emboss.py
+-rw-r--r--   0 bao        (501) staff       (20)    21333 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/apps/fetch.py
+-rw-r--r--   0 bao        (501) staff       (20)    19459 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/gbsubmit.py
+-rw-r--r--   0 bao        (501) staff       (20)     6892 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/gmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    18477 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/apps/grid.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     7238 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/lastz.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     3004 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/mask.py
+-rw-r--r--   0 bao        (501) staff       (20)    35471 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/phylo.py
+-rw-r--r--   0 bao        (501) staff       (20)     1896 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/r.py
+-rw-r--r--   0 bao        (501) staff       (20)     4901 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/restriction.py
+-rw-r--r--   0 bao        (501) staff       (20)     3784 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/softlink.py
+-rw-r--r--   0 bao        (501) staff       (20)    33065 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/uclust.py
+-rw-r--r--   0 bao        (501) staff       (20)     5208 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/uniprot.py
+-rw-r--r--   0 bao        (501) staff       (20)     3661 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/vecscreen.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.220021 jcvi-1.4.6/jcvi/assembly/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/assembly/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      257 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/assembly/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    65602 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/assembly/allmaps.py
+-rw-r--r--   0 bao        (501) staff       (20)    15451 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/assembly/allpaths.py
+-rw-r--r--   0 bao        (501) staff       (20)    13265 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/assembly/automaton.py
+-rw-r--r--   0 bao        (501) staff       (20)     5544 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/assembly/base.py
+-rw-r--r--   0 bao        (501) staff       (20)     3457 2022-09-27 05:18:33.000000 jcvi-1.4.6/jcvi/assembly/chic.pyx
+-rw-r--r--   0 bao        (501) staff       (20)     4581 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/assembly/coverage.py
+-rw-r--r--   0 bao        (501) staff       (20)     8676 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/assembly/gaps.py
+-rw-r--r--   0 bao        (501) staff       (20)    20002 2024-04-29 06:10:52.000000 jcvi-1.4.6/jcvi/assembly/geneticmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    34692 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/assembly/goldenpath.py
+-rw-r--r--   0 bao        (501) staff       (20)    56167 2024-04-29 06:10:52.000000 jcvi-1.4.6/jcvi/assembly/hic.py
+-rw-r--r--   0 bao        (501) staff       (20)    43034 2024-04-29 06:10:52.000000 jcvi-1.4.6/jcvi/assembly/kmer.py
+-rw-r--r--   0 bao        (501) staff       (20)    12519 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/assembly/opticalmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    27279 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/assembly/patch.py
+-rw-r--r--   0 bao        (501) staff       (20)    15741 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/assembly/postprocess.py
+-rw-r--r--   0 bao        (501) staff       (20)    21473 2024-04-30 06:05:19.000000 jcvi-1.4.6/jcvi/assembly/preprocess.py
+-rw-r--r--   0 bao        (501) staff       (20)     6287 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/assembly/sim.py
+-rw-r--r--   0 bao        (501) staff       (20)     8830 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/assembly/soap.py
+-rw-r--r--   0 bao        (501) staff       (20)    16183 2023-04-26 05:51:28.000000 jcvi-1.4.6/jcvi/assembly/syntenypath.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.222250 jcvi-1.4.6/jcvi/compara/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/compara/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      251 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/compara/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)     4218 2023-09-28 09:59:53.000000 jcvi-1.4.6/jcvi/compara/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     9796 2023-04-26 05:51:28.000000 jcvi-1.4.6/jcvi/compara/blastfilter.py
+-rw-r--r--   0 bao        (501) staff       (20)    28506 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/compara/catalog.py
+-rw-r--r--   0 bao        (501) staff       (20)    26355 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/compara/fractionation.py
+-rw-r--r--   0 bao        (501) staff       (20)    33945 2024-04-29 06:10:52.000000 jcvi-1.4.6/jcvi/compara/ks.py
+-rw-r--r--   0 bao        (501) staff       (20)     9216 2023-04-26 05:51:28.000000 jcvi-1.4.6/jcvi/compara/pad.py
+-rw-r--r--   0 bao        (501) staff       (20)     8322 2024-04-29 06:10:52.000000 jcvi-1.4.6/jcvi/compara/pedigree.py
+-rw-r--r--   0 bao        (501) staff       (20)     3051 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/compara/phylogeny.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     7948 2023-04-26 05:51:28.000000 jcvi-1.4.6/jcvi/compara/quota.py
+-rw-r--r--   0 bao        (501) staff       (20)    10341 2023-04-26 05:51:28.000000 jcvi-1.4.6/jcvi/compara/reconstruct.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     9233 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/compara/synfind.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    57574 2023-04-26 05:51:28.000000 jcvi-1.4.6/jcvi/compara/synteny.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.227614 jcvi-1.4.6/jcvi/formats/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/formats/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      262 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/formats/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    63559 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/formats/agp.py
+-rw-r--r--   0 bao        (501) staff       (20)    33880 2024-04-30 06:05:19.000000 jcvi-1.4.6/jcvi/formats/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    71545 2024-04-30 06:05:19.000000 jcvi-1.4.6/jcvi/formats/bed.py
+-rw-r--r--   0 bao        (501) staff       (20)    43184 2023-06-19 14:46:14.000000 jcvi-1.4.6/jcvi/formats/blast.py
+-rw-r--r--   0 bao        (501) staff       (20)     7010 2022-09-27 05:18:33.000000 jcvi-1.4.6/jcvi/formats/cblast.pyx
+-rw-r--r--   0 bao        (501) staff       (20)     3193 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/formats/cdt.py
+-rw-r--r--   0 bao        (501) staff       (20)     8612 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/formats/chain.py
+-rw-r--r--   0 bao        (501) staff       (20)     4644 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/formats/contig.py
+-rw-r--r--   0 bao        (501) staff       (20)    15169 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/formats/coords.py
+-rw-r--r--   0 bao        (501) staff       (20)     6529 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/formats/excel.py
+-rw-r--r--   0 bao        (501) staff       (20)    75502 2024-04-30 06:05:19.000000 jcvi-1.4.6/jcvi/formats/fasta.py
+-rw-r--r--   0 bao        (501) staff       (20)    29575 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/formats/fastq.py
+-rw-r--r--   0 bao        (501) staff       (20)    15545 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/formats/genbank.py
+-rw-r--r--   0 bao        (501) staff       (20)   119858 2024-04-30 06:05:19.000000 jcvi-1.4.6/jcvi/formats/gff.py
+-rw-r--r--   0 bao        (501) staff       (20)     3979 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/formats/html.py
+-rw-r--r--   0 bao        (501) staff       (20)     4612 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/formats/maf.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2842 2021-07-05 22:45:00.000000 jcvi-1.4.6/jcvi/formats/obo.py
+-rw-r--r--   0 bao        (501) staff       (20)     2900 2021-01-11 06:59:36.000000 jcvi-1.4.6/jcvi/formats/paf.py
+-rw-r--r--   0 bao        (501) staff       (20)     2783 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/formats/pdf.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    10355 2023-11-24 05:16:26.000000 jcvi-1.4.6/jcvi/formats/psl.py
+-rw-r--r--   0 bao        (501) staff       (20)     2746 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/formats/pyblast.py
+-rw-r--r--   0 bao        (501) staff       (20)    28231 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/formats/sam.py
+-rw-r--r--   0 bao        (501) staff       (20)     8041 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/formats/sizes.py
+-rw-r--r--   0 bao        (501) staff       (20)    25480 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/formats/vcf.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.230852 jcvi-1.4.6/jcvi/graphics/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/graphics/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      271 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/graphics/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    16271 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/graphics/align.py
+-rw-r--r--   0 bao        (501) staff       (20)    15265 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/graphics/assembly.py
+-rw-r--r--   0 bao        (501) staff       (20)    24983 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/graphics/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    10002 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/graphics/blastplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    22322 2024-04-30 06:05:19.000000 jcvi-1.4.6/jcvi/graphics/chromosome.py
+-rw-r--r--   0 bao        (501) staff       (20)     7145 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/graphics/coverage.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    14873 2023-04-26 05:51:28.000000 jcvi-1.4.6/jcvi/graphics/dotplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    21810 2023-02-06 05:16:46.000000 jcvi-1.4.6/jcvi/graphics/glyph.py
+-rw-r--r--   0 bao        (501) staff       (20)    24862 2024-04-24 05:29:17.000000 jcvi-1.4.6/jcvi/graphics/grabseeds.py
+-rw-r--r--   0 bao        (501) staff       (20)     5025 2021-03-26 15:38:36.000000 jcvi-1.4.6/jcvi/graphics/heatmap.py
+-rw-r--r--   0 bao        (501) staff       (20)     9610 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/graphics/histogram.py
+-rw-r--r--   0 bao        (501) staff       (20)    13307 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/graphics/karyotype.py
+-rw-r--r--   0 bao        (501) staff       (20)    34080 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/graphics/landscape.py
+-rw-r--r--   0 bao        (501) staff       (20)     3893 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/graphics/mummerplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    22468 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/graphics/synteny.py
+-rw-r--r--   0 bao        (501) staff       (20)     5488 2021-06-19 19:45:56.000000 jcvi-1.4.6/jcvi/graphics/table.py
+-rw-r--r--   0 bao        (501) staff       (20)    20377 2022-11-26 16:06:34.000000 jcvi-1.4.6/jcvi/graphics/tree.py
+-rw-r--r--   0 bao        (501) staff       (20)     6194 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/graphics/wheel.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.233241 jcvi-1.4.6/jcvi/projects/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/projects/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/projects/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    22445 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/projects/age.py
+-rw-r--r--   0 bao        (501) staff       (20)    15907 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/projects/allmaps.py
+-rw-r--r--   0 bao        (501) staff       (20)     6750 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/projects/bites.py
+-rw-r--r--   0 bao        (501) staff       (20)    14136 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/projects/ies.py
+-rw-r--r--   0 bao        (501) staff       (20)     7085 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/projects/jcvi.py
+-rw-r--r--   0 bao        (501) staff       (20)    22179 2024-04-29 06:10:52.000000 jcvi-1.4.6/jcvi/projects/misc.py
+-rw-r--r--   0 bao        (501) staff       (20)    25024 2023-02-06 05:16:46.000000 jcvi-1.4.6/jcvi/projects/napus.py
+-rw-r--r--   0 bao        (501) staff       (20)    12754 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/projects/pineapple.py
+-rw-r--r--   0 bao        (501) staff       (20)    67853 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/projects/str.py
+-rw-r--r--   0 bao        (501) staff       (20)    25766 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/projects/sugarcane.py
+-rw-r--r--   0 bao        (501) staff       (20)    23950 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/projects/synfind.py
+-rw-r--r--   0 bao        (501) staff       (20)    21554 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/projects/tgbs.py
+-rw-r--r--   0 bao        (501) staff       (20)    11690 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/projects/vanilla.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.235000 jcvi-1.4.6/jcvi/utils/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/utils/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    24200 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/utils/aws.py
+-rw-r--r--   0 bao        (501) staff       (20)    12647 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/utils/cbook.py
+-rw-r--r--   0 bao        (501) staff       (20)      355 2021-01-11 02:34:49.000000 jcvi-1.4.6/jcvi/utils/console.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.238003 jcvi-1.4.6/jcvi/utils/data/
+-rwxr-xr-x   0 bao        (501) staff       (20)    16912 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/Airswing.ttf
+-rwxr-xr-x   0 bao        (501) staff       (20)   103940 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/Collegia.ttf
+-rwxr-xr-x   0 bao        (501) staff       (20)    20468 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/HookedUp.ttf
+-rw-r--r--   0 bao        (501) staff       (20)    25832 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/Humor-Sans.ttf
+-rw-r--r--   0 bao        (501) staff       (20)    28065 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/TREDs.meta.csv
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      911 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/adapters.fasta
+-rw-r--r--   0 bao        (501) staff       (20)     3321 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/blosum80.mat
+-rw-r--r--   0 bao        (501) staff       (20)     7686 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/chrY.hg38.unique_ccn.gc
+-rw-r--r--   0 bao        (501) staff       (20)      282 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/colorchecker.txt
+-rw-r--r--   0 bao        (501) staff       (20)    45544 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/hg38.band.txt
+-rw-r--r--   0 bao        (501) staff       (20)    11672 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/hg38.chrom.sizes
+-rw-r--r--   0 bao        (501) staff       (20)     1000 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/instance.json
+-rw-r--r--   0 bao        (501) staff       (20)     9793 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/utils/db.py
+-rw-r--r--   0 bao        (501) staff       (20)     4145 2021-01-09 20:22:53.000000 jcvi-1.4.6/jcvi/utils/ez_setup.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2884 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/utils/grouper.py
+-rw-r--r--   0 bao        (501) staff       (20)    10437 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/utils/orderedcollections.py
+-rw-r--r--   0 bao        (501) staff       (20)    14595 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/utils/range.py
+-rw-r--r--   0 bao        (501) staff       (20)     3946 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/utils/table.py
+-rw-r--r--   0 bao        (501) staff       (20)     4687 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/utils/taxonomy.py
+-rw-r--r--   0 bao        (501) staff       (20)     1522 2021-07-13 05:06:52.000000 jcvi-1.4.6/jcvi/utils/validator.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     1377 2021-01-15 14:44:37.000000 jcvi-1.4.6/jcvi/utils/webcolors.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.239393 jcvi-1.4.6/jcvi/variation/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/variation/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      259 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/variation/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    45321 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/variation/cnv.py
+-rw-r--r--   0 bao        (501) staff       (20)     7036 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/variation/deconvolute.py
+-rw-r--r--   0 bao        (501) staff       (20)     9385 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/variation/delly.py
+-rw-r--r--   0 bao        (501) staff       (20)    11777 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/variation/impute.py
+-rw-r--r--   0 bao        (501) staff       (20)     3478 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/variation/phase.py
+-rw-r--r--   0 bao        (501) staff       (20)    10831 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/variation/snp.py
+-rw-r--r--   0 bao        (501) staff       (20)    48818 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/variation/str.py
+-rw-r--r--   0 bao        (501) staff       (20)      176 2024-04-30 16:08:55.000000 jcvi-1.4.6/jcvi/version.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.206721 jcvi-1.4.6/jcvi.egg-info/
+-rw-r--r--   0 bao        (501) staff       (20)     8915 2024-04-30 16:08:55.000000 jcvi-1.4.6/jcvi.egg-info/PKG-INFO
+-rw-r--r--   0 bao        (501) staff       (20)     4543 2024-04-30 16:08:55.000000 jcvi-1.4.6/jcvi.egg-info/SOURCES.txt
+-rw-r--r--   0 bao        (501) staff       (20)        1 2024-04-30 16:08:55.000000 jcvi-1.4.6/jcvi.egg-info/dependency_links.txt
+-rw-r--r--   0 bao        (501) staff       (20)        1 2022-11-26 21:54:22.000000 jcvi-1.4.6/jcvi.egg-info/not-zip-safe
+-rw-r--r--   0 bao        (501) staff       (20)      221 2024-04-30 16:08:55.000000 jcvi-1.4.6/jcvi.egg-info/requires.txt
+-rw-r--r--   0 bao        (501) staff       (20)        5 2024-04-30 16:08:55.000000 jcvi-1.4.6/jcvi.egg-info/top_level.txt
+-rw-r--r--   0 bao        (501) staff       (20)      359 2022-11-26 21:23:29.000000 jcvi-1.4.6/pyproject.toml
+-rw-r--r--   0 bao        (501) staff       (20)     1242 2024-04-30 16:08:55.240326 jcvi-1.4.6/setup.cfg
+-rw-r--r--   0 bao        (501) staff       (20)      553 2022-11-26 21:23:29.000000 jcvi-1.4.6/setup.py
```

### Comparing `jcvi-1.4.5/LICENSE` & `jcvi-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/PKG-INFO` & `jcvi-1.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcvi
-Version: 1.4.5
+Version: 1.4.6
 Summary: Python utility libraries on genome assembly, annotation and comparative genomics
 Home-page: http://github.com/tanghaibao/jcvi
 Author: Haibao Tang, Vivek Krishnakumar, Jingping Li
 Author-email: tanghaibao@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -27,16 +27,16 @@
 Collection of Python libraries to parse bioinformatics files, or perform
 computation related to assembly, annotation, and comparative genomics.
 
 |         |                                                                  |
 | ------- | ---------------------------------------------------------------- |
 | Authors | Haibao Tang ([tanghaibao](http://github.com/tanghaibao))         |
 |         | Vivek Krishnakumar ([vivekkrish](https://github.com/vivekkrish)) |
-|         | Jingping Li ([Jingping](https://github.com/Jingping))            |
 |         | Xingtan Zhang ([tangerzhang](https://github.com/tangerzhang))    |
+|         | Won Cheol Yim ([wyim-pgl](https://github.com/wyim-pgl))          |
 | Email   | <tanghaibao@gmail.com>                                           |
 | License | [BSD](http://creativecommons.org/licenses/BSD/)                  |
 
 ## Citations
 
 - If you use the MCscan pipeline for synteny inference, please cite:
```

### Comparing `jcvi-1.4.5/README.md` & `jcvi-1.4.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 Collection of Python libraries to parse bioinformatics files, or perform
 computation related to assembly, annotation, and comparative genomics.
 
 |         |                                                                  |
 | ------- | ---------------------------------------------------------------- |
 | Authors | Haibao Tang ([tanghaibao](http://github.com/tanghaibao))         |
 |         | Vivek Krishnakumar ([vivekkrish](https://github.com/vivekkrish)) |
-|         | Jingping Li ([Jingping](https://github.com/Jingping))            |
 |         | Xingtan Zhang ([tangerzhang](https://github.com/tangerzhang))    |
+|         | Won Cheol Yim ([wyim-pgl](https://github.com/wyim-pgl))          |
 | Email   | <tanghaibao@gmail.com>                                           |
 | License | [BSD](http://creativecommons.org/licenses/BSD/)                  |
 
 ## Citations
 
 - If you use the MCscan pipeline for synteny inference, please cite:
```

### Comparing `jcvi-1.4.5/jcvi/__init__.py` & `jcvi-1.4.6/jcvi/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from datetime import datetime
 from pkg_resources import get_distribution, DistributionNotFound
 
 
-__author__ = ("Haibao Tang", "Vivek Krishnakumar", "Jingping Li")
-__copyright__ = "Copyright (c) 2010-{}, Haibao Tang".format(datetime.now().year)
+__author__ = (
+    "Haibao Tang",
+    "Vivek Krishnakumar",
+    "Xingtan Zhang",
+    "Won Cheol Yim",
+)
+__copyright__ = f"Copyright (c) 2010-{datetime.now().year}, Haibao Tang"
 __email__ = "tanghaibao@gmail.com"
 __license__ = "BSD"
 __status__ = "Development"
 
 
 try:
     VERSION = get_distribution(__name__).version
 except DistributionNotFound:  # pragma: no cover
     try:
         from .version import version as VERSION  # noqa
-    except ImportError:  # pragma: no cover
+    except ImportError as exc:  # pragma: no cover
         raise ImportError(
             "Failed to find (autogenerated) version.py. "
             "This might be because you are installing from GitHub's tarballs, "
             "use the PyPI ones."
-        )
+        ) from exc
 __version__ = VERSION
```

### Comparing `jcvi-1.4.5/jcvi/algorithms/ec.py` & `jcvi-1.4.6/jcvi/algorithms/ec.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/algorithms/formula.py` & `jcvi-1.4.6/jcvi/algorithms/formula.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/algorithms/graph.py` & `jcvi-1.4.6/jcvi/algorithms/graph.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/algorithms/lis.py` & `jcvi-1.4.6/jcvi/algorithms/lis.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/algorithms/lpsolve.py` & `jcvi-1.4.6/jcvi/algorithms/lpsolve.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/algorithms/matrix.py` & `jcvi-1.4.6/jcvi/algorithms/matrix.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/algorithms/maxsum.py` & `jcvi-1.4.6/jcvi/algorithms/maxsum.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/algorithms/supermap.py` & `jcvi-1.4.6/jcvi/algorithms/supermap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/algorithms/tsp.py` & `jcvi-1.4.6/jcvi/algorithms/tsp.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/annotation/ahrd.py` & `jcvi-1.4.6/jcvi/annotation/ahrd.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/annotation/automaton.py` & `jcvi-1.4.6/jcvi/annotation/automaton.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/annotation/depth.py` & `jcvi-1.4.6/jcvi/annotation/depth.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/annotation/evm.py` & `jcvi-1.4.6/jcvi/annotation/evm.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/annotation/maker.py` & `jcvi-1.4.6/jcvi/annotation/maker.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/annotation/pasa.py` & `jcvi-1.4.6/jcvi/annotation/pasa.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/annotation/qc.py` & `jcvi-1.4.6/jcvi/annotation/qc.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/annotation/reformat.py` & `jcvi-1.4.6/jcvi/annotation/reformat.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/annotation/stats.py` & `jcvi-1.4.6/jcvi/annotation/stats.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/annotation/train.py` & `jcvi-1.4.6/jcvi/annotation/train.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/apps/align.py` & `jcvi-1.4.6/jcvi/apps/align.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/apps/base.py` & `jcvi-1.4.6/jcvi/apps/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 """
 Basic support for running library as script
 """
 
 import errno
+import fnmatch
+import logging
 import os
-import time
 import os.path as op
 import shutil
 import signal
 import sys
-import logging
-import fnmatch
+import time
 
 from collections.abc import Iterable
-from http.client import HTTPSConnection
-from urllib.parse import urlencode
 from configparser import (
     ConfigParser,
     RawConfigParser,
     NoOptionError,
     NoSectionError,
     ParsingError,
 )
+
+from http.client import HTTPSConnection
+from optparse import OptionGroup, OptionParser as OptionP, SUPPRESS_HELP
 from socket import gethostname
-from subprocess import PIPE, call, check_output
-from optparse import OptionParser as OptionP, OptionGroup, SUPPRESS_HELP
+from subprocess import CalledProcessError, PIPE, call, check_output
+from time import ctime
 from typing import Any, Collection, List, Optional, Tuple, Union
-
+from urllib.parse import urlencode
 from natsort import natsorted
 from rich.console import Console
 from rich.logging import RichHandler
 
-from jcvi import __copyright__, __version__
+from .. import __copyright__, __version__ as version
 
-# http://newbebweb.blogspot.com/2012/02/python-head-ioerror-errno-32-broken.html
-nobreakbuffer = lambda: signal.signal(signal.SIGPIPE, signal.SIG_DFL)
-nobreakbuffer()
-os.environ["LC_ALL"] = "C"
-JCVIHELP = "JCVI utility libraries {} [{}]\n".format(__version__, __copyright__)
 
+os.environ["LC_ALL"] = "C"
+# http://newbebweb.blogspot.com/2012/02/python-head-ioerror-errno-32-broken.html
+signal.signal(signal.SIGPIPE, signal.SIG_DFL)
+JCVIHELP = f"JCVI utility libraries {version} [{__copyright__}]\n"
 TextCollection = Union[str, List[str], Tuple[str, ...]]
 
 
 def debug(level=logging.DEBUG):
     """
     Turn on the debugging
     """
@@ -54,15 +54,17 @@
     )
 
 
 debug()
 
 
 def get_logger(name: str, level: int = logging.DEBUG):
-    """Return a logger with a default ColoredFormatter."""
+    """
+    Return a logger with a default ColoredFormatter.
+    """
     logger = logging.getLogger(name)
     if logger.hasHandlers():
         logger.handlers.clear()
     logger.addHandler(RichHandler(console=Console(stderr=True)))
     logger.propagate = False
     logger.setLevel(level)
     return logger
@@ -624,15 +626,17 @@
                 logger.info("`lp` not found. latex use is disabled.")
 
         setup_theme(style=opts.style, font=opts.font, usetex=iopts.usetex)
 
         return opts, args, iopts
 
     def set_dotplot_opts(self, theme: int = 2) -> OptionGroup:
-        """Used in compara.catalog and graphics.dotplot"""
+        """
+        Used in compara.catalog and graphics.dotplot
+        """
         from jcvi.graphics.base import set1
 
         group = OptionGroup(self, "Dot plot parameters")
         group.add_option(
             "--skipempty",
             default=False,
             action="store_true",
@@ -998,50 +1002,23 @@
             "--uc",
             default=False,
             action="store_true",
             help="Toggle gene identifier upper case",
         )
 
     def set_home(self, prog, default=None):
-        tag = "--{0}_home".format(prog)
-        default = default or {
-            "amos": "~/code/amos-code",
-            "trinity": "~/export/trinityrnaseq-2.0.6",
-            "hpcgridrunner": "~/export/hpcgridrunner-1.0.2",
-            "cdhit": "~/export/cd-hit-v4.6.1-2012-08-27",
-            "maker": "~/export/maker",
-            "augustus": "~/export/maker/exe/augustus",
-            "pasa": "~/export/PASApipeline-2.0.2",
-            "gatk": "~/export",
-            "gmes": "~/export/gmes",
-            "gt": "~/export/genometools",
-            "sspace": "~/export/SSPACE-STANDARD-3.0_linux-x86_64",
-            "gapfiller": "~/export/GapFiller_v1-11_linux-x86_64",
-            "pbjelly": "~/export/PBSuite_15.2.20",
-            "picard": "~/export/picard-tools-1.138",
-            "khmer": "~/export/khmer",
-            "tassel": "/usr/local/projects/MTG4/packages/tassel",
-            "tgi": "~/export/seqclean-x86_64",
-            "eddyyeh": "/home/shared/scripts/eddyyeh",
-            "fiona": "~/export/fiona-0.2.0-Linux-x86_64",
-            "fermi": "~/export/fermi",
-            "lobstr": "/mnt/software/lobSTR",
-            "shapeit": "/mnt/software/shapeit",
-            "impute": "/mnt/software/impute",
-            "beagle": "java -jar /mnt/software/beagle.14Jan16.841.jar",
-            "minimac": "/mnt/software/Minimac3/bin",
-        }.get(prog, None)
+        tag = f"--{prog}_home"
         if default is None:  # Last attempt at guessing the path
             try:
                 default = op.dirname(which(prog))
             except:
                 default = None
         else:
             default = op.expanduser(default)
-        help = "Home directory for {0}".format(prog.upper())
+        help = f"Home directory for {prog.upper()}"
         self.add_option(tag, default=default, help=help)
 
     def set_aligner(self, aligner="bowtie"):
         valid_aligners = ("bowtie", "bwa")
         self.add_option(
             "--aligner", default=aligner, choices=valid_aligners, help="Use aligner"
         )
@@ -1049,25 +1026,25 @@
     def set_verbose(self, help="Print detailed reports"):
         self.add_option("--verbose", default=False, action="store_true", help=help)
 
 
 def ConfigSectionMap(Config, section):
     """
     Read a specific section from a ConfigParser() object and return
-    a dict() of all key-value pairs in that section
+    a dict of all key-value pairs in that section
     """
     cfg = {}
     options = Config.options(section)
     for option in options:
         try:
             cfg[option] = Config.get(section, option)
             if cfg[option] == -1:
-                logger.debug("skip: %s", option)
+                logger.debug("Skip: %s", option)
         except:
-            logger.debug("exception on %s!", option)
+            logger.error("Exception on %s", option)
             cfg[option] = None
     return cfg
 
 
 def get_abs_path(link_name):
     source = link_name
     if op.islink(source):
@@ -1081,15 +1058,21 @@
     if source == link_name:
         return source
     else:
         return get_abs_path(source)
 
 
 datadir = get_abs_path(op.join(op.dirname(__file__), "../utils/data"))
-datafile = lambda x: op.join(datadir, x)
+
+
+def datafile(x: str, datadir: str = datadir):
+    """
+    Return the full path to the data file in the data directory.
+    """
+    return op.join(datadir, x)
 
 
 def splitall(path):
     allparts = []
     while True:
         path, p1 = op.split(path)
         if not p1:
@@ -1462,17 +1445,16 @@
         downloader (str, optional): Use a given downloader. One of wget|curl|powershell|insecure.
         Defaults to None.
 
     Returns:
         str: Local file name.
     """
     from urllib.parse import urlsplit
-    from subprocess import CalledProcessError
 
-    scheme, netloc, path, query, fragment = urlsplit(url)
+    _, _, path, _, _ = urlsplit(url)
     basepath = op.basename(path)
     if basepath:
         url_gzipped = basepath.endswith(".gz")
         filename_gzipped = filename and filename.endswith(".gz")
         need_gunzip = url_gzipped and (not filename_gzipped)
         need_gzip = (not url_gzipped) and filename_gzipped
         if handle_gzip and (
@@ -1542,22 +1524,22 @@
         logger.warning("Gzip file estimated uncompressed size: %d", size)
 
     return size
 
 
 def main():
     actions = (
+        ("expand", "move files in subfolders into the current folder"),
         ("less", "enhance the unix `less` command"),
+        ("mdownload", "multiple download a list of files"),
+        ("mergecsv", "merge a set of tsv files"),
+        ("notify", "send an email/push notification"),
         ("timestamp", "record timestamps for all files in the current folder"),
-        ("expand", "move files in subfolders into the current folder"),
         ("touch", "recover timestamps for files in the current folder"),
-        ("mdownload", "multiple download a list of files"),
         ("waitpid", "wait for a PID to finish and then perform desired action"),
-        ("notify", "send an email/push notification"),
-        ("mergecsv", "merge a set of tsv files"),
     )
     p = ActionDispatcher(actions)
     p.dispatch(globals())
 
 
 def mdownload(args):
     """
@@ -1565,15 +1547,15 @@
 
     Multiple download a list of files. Use formats.html.links() to extract the
     links file.
     """
     from jcvi.apps.grid import Jobs
 
     p = OptionParser(mdownload.__doc__)
-    opts, args = p.parse_args(args)
+    _, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (linksfile,) = args
     links = [(x.strip(),) for x in open(linksfile)]
     j = Jobs(download, links)
@@ -1626,38 +1608,36 @@
 
     Record the timestamps for all files in the current folder.
     filename atime mtime
 
     This file can be used later to recover previous timestamps through touch().
     """
     p = OptionParser(timestamp.__doc__)
-    opts, args = p.parse_args(args)
+    _, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (path,) = args
-    for root, dirs, files in os.walk(path):
+    for root, _, files in os.walk(path):
         for f in files:
             filename = op.join(root, f)
             atime, mtime = get_times(filename)
             print(filename, atime, mtime)
 
 
 def touch(args):
     """
     %prog touch timestamp.info
 
     Recover timestamps for files in the current folder.
     CAUTION: you must execute this in the same directory as timestamp().
     """
-    from time import ctime
-
     p = OptionParser(touch.__doc__)
-    opts, args = p.parse_args(args)
+    _, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (info,) = args
     fp = open(info)
     for row in fp:
@@ -1703,15 +1683,15 @@
     $ %prog less myfile 100      # Go to certain byte number and streaming
     $ %prog less myfile 100,200  # Stream at several positions
     $ %prog less myfile all      # Generate a snapshot every 10% (10%, 20%, ..)
     """
     from jcvi.formats.base import must_open
 
     p = OptionParser(less.__doc__)
-    opts, args = p.parse_args(args)
+    _, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     filename, pos = args
     fsize = getfilesize(filename)
 
@@ -2015,15 +1995,14 @@
         )
 
 
 def pid_exists(pid):
     """Check whether pid exists in the current process table."""
     if pid < 0:
         return False
-    import errno
 
     try:
         os.kill(pid, 0)
     except OSError as e:
         return e.errno == errno.EPERM
     else:
         return True
@@ -2133,21 +2112,14 @@
     p.set_email()
     p.set_grid()
     opts, args = p.parse_args(args)
 
     if len(args) == 0:
         sys.exit(not p.print_help())
 
-    if not opts.message:
-        """
-        If notification message not specified by user, just get
-        the name of the running command and use it as the message
-        """
-        from subprocess import check_output
-
     sep = ":::"
     cmd = None
     if sep in args:
         sepidx = args.index(sep)
         cmd = " ".join(args[sepidx + 1 :]).strip()
         args = args[:sepidx]
 
@@ -2265,15 +2237,16 @@
         except Exception as e:
             details = e
 
         print("{}: {}".format(k, details), file=sys.stderr)
 
 
 def sample_N(a: Collection[Any], N: int, seed: Optional[int] = None) -> List[Any]:
-    """When size of N is > size of a, random.sample() will emit an error:
+    """
+    When size of N is > size of a, random.sample() will emit an error:
     ValueError: sample larger than population
 
     This method handles such restrictions by repeatedly sampling when that
     happens. Guaranteed to cover all items if N is > size of a.
 
     Examples:
     >>> sample_N([1, 2, 3], 2, seed=666)
```

### Comparing `jcvi-1.4.5/jcvi/apps/biomart.py` & `jcvi-1.4.6/jcvi/apps/biomart.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/apps/blastplus.py` & `jcvi-1.4.6/jcvi/apps/blastplus.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/apps/bowtie.py` & `jcvi-1.4.6/jcvi/apps/bowtie.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/apps/bwa.py` & `jcvi-1.4.6/jcvi/apps/bwa.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/apps/cdhit.py` & `jcvi-1.4.6/jcvi/apps/cdhit.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/apps/emboss.py` & `jcvi-1.4.6/jcvi/apps/emboss.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/apps/fetch.py` & `jcvi-1.4.6/jcvi/apps/fetch.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/apps/gbsubmit.py` & `jcvi-1.4.6/jcvi/apps/gbsubmit.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/apps/gmap.py` & `jcvi-1.4.6/jcvi/apps/gmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/apps/grid.py` & `jcvi-1.4.6/jcvi/apps/grid.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/apps/lastz.py` & `jcvi-1.4.6/jcvi/apps/lastz.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/apps/mask.py` & `jcvi-1.4.6/jcvi/apps/mask.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/apps/phylo.py` & `jcvi-1.4.6/jcvi/apps/phylo.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/apps/r.py` & `jcvi-1.4.6/jcvi/apps/r.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/apps/restriction.py` & `jcvi-1.4.6/jcvi/apps/restriction.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/apps/softlink.py` & `jcvi-1.4.6/jcvi/apps/softlink.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/apps/uclust.py` & `jcvi-1.4.6/jcvi/apps/uclust.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/apps/uniprot.py` & `jcvi-1.4.6/jcvi/apps/uniprot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/apps/vecscreen.py` & `jcvi-1.4.6/jcvi/apps/vecscreen.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/assembly/allmaps.py` & `jcvi-1.4.6/jcvi/assembly/allmaps.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,57 +3,57 @@
 
 """
 Scaffold Ordering with Weighted Maps.
 """
 import os.path as op
 import os
 import sys
-import logging
+
+from collections import Counter, defaultdict
+from functools import partial
+from itertools import combinations, product
+from typing import Optional
 
 import numpy as np
 import networkx as nx
 
 from cmmodule.utils import read_chain_file
 from cmmodule.mapbed import crossmap_bed_file
-from collections import Counter, defaultdict
-from functools import partial
-from itertools import combinations, product
 from more_itertools import pairwise
-from typing import Optional
 
-from jcvi import __version__ as version
-from jcvi.algorithms.formula import reject_outliers, spearmanr
-from jcvi.algorithms.lis import (
+from ..algorithms.ec import GA_setup, GA_run
+from ..algorithms.formula import reject_outliers, spearmanr
+from ..algorithms.lis import (
     longest_monotonic_subseq_length_loose as lms,
     longest_monotonic_subsequence_loose as lmseq,
 )
-from jcvi.algorithms.tsp import hamiltonian
-from jcvi.algorithms.matrix import determine_signs
-from jcvi.algorithms.ec import GA_setup, GA_run
-from jcvi.formats.agp import AGP, order_to_agp, build as agp_build, reindex
-from jcvi.formats.base import DictFile, FileMerger, must_open, read_block
-from jcvi.formats.bed import Bed, BedLine, natsorted, sort
-from jcvi.formats.chain import fromagp
-from jcvi.formats.sizes import Sizes
-from jcvi.graphics.landscape import draw_gauge
-from jcvi.utils.cbook import human_size, percentage
-from jcvi.utils.grouper import Grouper
-from jcvi.utils.table import tabulate
-from jcvi.apps.base import (
+from ..algorithms.matrix import determine_signs
+from ..apps.base import (
     ActionDispatcher,
     OptionGroup,
     OptionParser,
     SUPPRESS_HELP,
     cleanup,
     flatten,
     get_today,
+    logger,
     mkdir,
     need_update,
     sh,
+    version,
 )
+from ..formats.agp import AGP, order_to_agp, build as agp_build, reindex
+from ..formats.base import DictFile, FileMerger, must_open, read_block
+from ..formats.bed import Bed, BedLine, natsorted, sort
+from ..formats.chain import fromagp
+from ..formats.sizes import Sizes
+from ..graphics.landscape import draw_gauge
+from ..utils.cbook import human_size, percentage
+from ..utils.grouper import Grouper
+from ..utils.table import tabulate
 
 
 START, END = "START", "END"
 distance_choices = ("cM", "rank")
 linkage_choices = ("single", "double", "complete", "average", "median")
 np.seterr(invalid="ignore")
 
@@ -189,37 +189,35 @@
             if fitness:
                 fitness = "{0}".format(fitness).split(".")[0].replace("(", "")
                 label += "-" + fitness
             print_tour(fwtour, self.object, tag, label, tour, recode=True)
             return tour
 
         i = 0
-        best_tour, best_fitness = None, None
+        best_fitness = None
         while True:  # Multiple EC rounds due to orientation fixes
-            logging.debug("Start EC round {0}".format(i))
+            logger.debug("Start EC round %d", i)
             scaffolds_oo = dict(tour)
             scfs, tour, ww = self.prepare_ec(scaffolds, tour, weights)
             callbacki = partial(callback, i=i)
             toolbox = GA_setup(tour)
             toolbox.register("evaluate", colinear_evaluate_multi, scfs=scfs, weights=ww)
             tour, fitness = GA_run(
                 toolbox, ngen=ngen, npop=npop, cpus=cpus, seed=seed, callback=callbacki
             )
             tour = callbacki(tour, "FIN")
             if best_fitness and fitness <= best_fitness:
-                logging.debug(
-                    "No fitness improvement: {0}. Exit EC.".format(best_fitness)
-                )
+                logger.debug("No fitness improvement: %s. Exit EC.", best_fitness)
                 break
             tour = self.fix_orientation(tour)
-            best_tour, best_fitness = tour, fitness
+            best_fitness = fitness
             print_tour(
                 fwtour, self.object, tag, "GA{0}-FIXORI".format(i), tour, recode=True
             )
-            logging.debug("Current best fitness: {0}".format(best_fitness))
+            logger.debug("Current best fitness: %s", best_fitness)
             i += 1
 
         tour = self.fix_tour(tour)
         self.tour = recode_tour(tour)
         for fw in (sys.stderr, fwtour):
             print_tour(fw, self.object, tag, "FINAL", self.tour)
 
@@ -281,15 +279,15 @@
         for (a, b), v in distances.items():
             d = self.weighted_mean(v)
             G.add_edge(a, b, weight=d)
             if a == START or b == END:
                 continue
             G.add_edge(b, a, weight=d)
 
-        logging.debug("Graph size: |V|=%d, |E|=%d", len(G), G.size())
+        logger.debug("Graph size: |V|=%d, |E|=%d", len(G), G.size())
 
         L = dict(nx.all_pairs_dijkstra_path_length(G))
         for a, b in combinations(scaffolds, 2):
             if G.has_edge(a, b):
                 continue
             if a in L and b in L[a]:
                 l = L[a][b]
@@ -417,15 +415,15 @@
                 M = self.get_series(lg, s, o)
                 score_with = lms(L + M + U)[0]
                 score_without = lms(L + U)[0]
                 assert score_with >= score_without
                 if score_with > score_without:
                     keep.add(s)
         dropped = len(tour) - len(keep)
-        logging.debug("Dropped {0} minor scaffolds".format(dropped))
+        logger.debug("Dropped %d minor scaffolds", dropped)
         return [(s, o) for (s, o) in tour if s in keep]
 
     def fix_orientation(self, tour):
         """
         Test each scaffold if flipping will increass longest monotonic chain
         length.
         """
@@ -454,15 +452,15 @@
             old_d = orientations[s]
             new_d = np.sign(d)
             if new_d != old_d:
                 orientations[s] = new_d
                 fixed += 1
 
         tour = [(x, orientations[x]) for x in scaffolds]
-        logging.debug("Fixed orientations for {0} scaffolds.".format(fixed))
+        logger.debug("Fixed orientations for %d scaffolds.", fixed)
         return tour
 
 
 class CSVMapLine(object):
     def __init__(self, row, sep=",", mapname=None):
         # ScaffoldID,ScaffoldPosition,LinkageGroup,GeneticPosition
         args = [x.strip() for x in row.split(sep)]
@@ -485,15 +483,15 @@
     def __init__(self, b):
         self.seqid = b.seqid
         self.pos = b.start
         self.mlg, cm = b.accn.split(":")
         try:
             self.mapname, self.lg = b.accn.split("-", 1)
         except ValueError:
-            logging.error("Malformed marker name: {}".format(b.accn))
+            logger.error("Malformed marker name: %s", b.accn)
             sys.exit(1)
         self.cm = float(cm)
         self.accn = b.accn
         self.args = b.args
         self.rank = -1
 
     def parse_scaffold_info(self):
@@ -531,18 +529,18 @@
                 b.parse_scaffold_info()
 
     def report(self):
         self.nmarkers = len(self)
         self.seqids = sorted(set(x.seqid for x in self))
         self.mapnames = sorted(set(x.mapname for x in self))
         self.mlgs = sorted(set(x.mlg for x in self))
-        logging.debug(
-            "Map contains {0} markers in {1} linkage groups.".format(
-                self.nmarkers, len(self.mlgs)
-            )
+        logger.debug(
+            "Map contains %d markers in %d linkage groups.",
+            self.nmarkers,
+            len(self.mlgs),
         )
 
     def extract(self, seqid):
         r = [x for x in self if x.seqid == seqid]
         return sorted(r, key=lambda x: x.pos)
 
     def extract_mlg(self, mlg):
@@ -578,17 +576,15 @@
         if remove_outliers:
             original = clean = 0
             for pair, markers in s.items():
                 cm = self.remove_outliers(markers, function)
                 s[pair] = cm
                 original += len(markers)
                 clean += len(cm)
-            logging.debug(
-                "Retained {0} clean markers.".format(percentage(clean, original))
-            )
+            logger.debug("Retained %s clean markers.", percentage(clean, original))
         return s
 
     def remove_outliers(self, markers, function):
         data = [function(x) for x in markers]
         reject = reject_outliers(data)
         clean_markers = [m for m, r in zip(markers, reject) if not r]
         return clean_markers
@@ -644,34 +640,32 @@
         self.maps = [x.split()[0] for x in must_open(filename)]
         self.update_maps(mapnames)
         pivot_weight, o, pivot = self.get_pivot(mapnames)
         ref = self.maps[0]
         self.pivot = pivot
         self.ref = ref
 
-        logging.debug("Map weights: {0}".format(self.items()))
+        logger.debug("Map weights: %s", self.items())
 
     def update_maps(self, mapnames, default=1):
         keys = list(self.keys())
         for m in keys:
             if m not in mapnames:
                 del self[m]
         for m in mapnames:
             if m in self:
                 continue
             self[m] = default
-            logging.debug("Weight for `{0}` set to {1}.".format(m, default))
+            logger.debug("Weight for `%s` set to %d.", m, default)
 
     def get_pivot(self, mapnames):
         # Break ties by occurence in file
         common_mapnames = set(self.maps) & set(mapnames)
         if not common_mapnames:
-            logging.error(
-                "No common names found between %s and %s", self.maps, mapnames
-            )
+            logger.error("No common names found between %s and %s", self.maps, mapnames)
             sys.exit(1)
         return max(
             (w, -self.maps.index(m), m) for m, w in self.items() if m in common_mapnames
         )
 
 
 class Layout(object):
@@ -715,15 +709,15 @@
                 ystart -= mlen + gapsize
         self.coords = coords
 
 
 class GapEstimator(object):
     def __init__(self, mapc, agp, seqid, mlg, function=lambda x: x.cm):
         mm = mapc.extract_mlg(mlg)
-        logging.debug("Extracted {0} markers for {1}-{2}".format(len(mm), seqid, mlg))
+        logger.debug("Extracted %d markers for %s-%s", len(mm), seqid, mlg)
         self.mlgsize = max(function(x) for x in mm)
 
         self.agp = [x for x in agp if x.object == seqid]
         self.scaffolds = [x.component_id for x in self.agp if not x.is_gap]
         self.pp = [x.object_beg for x in self.agp if x.is_gap]
         self.chrsize = max(x.object_end for x in self.agp)
 
@@ -877,18 +871,18 @@
 
 def plotratio(args):
     """
     %prog plotratio JM-2 chr23 JMMale-23
 
     Illustrate physical vs map distance ratio, that were used in the gap estimation algorithm.
     """
-    from jcvi.graphics.base import plt, savefig, normalize_axes, panel_labels, set2
+    from ..graphics.base import plt, savefig, normalize_axes, panel_labels, set2
 
     p = OptionParser(estimategaps.__doc__)
-    opts, args, iopts = p.set_image_options(args, figsize="6x6", dpi=300)
+    _, args, iopts = p.set_image_options(args, figsize="6x6", dpi=300)
 
     if len(args) != 3:
         sys.exit(not p.print_help())
 
     pf, seqid, mlg = args
     bedfile = pf + ".lifted.bed"
     agpfile = pf + ".agp"
@@ -1050,17 +1044,15 @@
             start, end = mi.pos, mj.pos
             if start > end:
                 start, end = end, start
             if opts.splitsingle:
                 start = end = (start + end) / 2
             print("\t".join(str(x) for x in (mi.seqid, start - 1, end)))
             nbreaks += 1
-    logging.debug(
-        "A total of {} breakpoints inferred (--chunk={})".format(nbreaks, nchunk)
-    )
+    logger.debug("A total of %d breakpoints inferred (--chunk=%d)", nbreaks, nchunk)
 
 
 def movie(args):
     """
     %prog movie input.bed scaffolds.fasta chr1
 
     Visualize history of scaffold OO. The history is contained within the
@@ -1108,15 +1100,15 @@
             score = cur_score
 
         image_name = ".".join((seqid, "{0:04d}".format(i), label, "pdf"))
         if need_update(tourfile, image_name):
             fwagp = must_open(agpfile, "w")
             order_to_agp(seqid, tour, sizes, fwagp, gapsize=gapsize, evidence="map")
             fwagp.close()
-            logging.debug("%s written to `%s`.", header, agpfile)
+            logger.debug("%s written to `%s`.", header, agpfile)
             build([inputbed, scaffoldsfasta, "--cleanup"])
             pdf_name = plot([inputbed, seqid, "--title={0}".format(label)])
             sh("mv {0} {1}".format(pdf_name, image_name))
         if label in ("INIT", "FLIP", "TSP", "FINAL"):
             for j in range(5):  # Delay for 5 frames
                 image_delay = image_name.rsplit(".", 1)[0] + ".d{0}.pdf".format(j)
                 sh("cp {0} {1}/{2}".format(image_name, ffmpeg, image_delay))
@@ -1258,23 +1250,23 @@
     mapnames = set()
     for row in fp:
         mapname = filename_to_mapname(fp.filename())
         mapnames.add(mapname)
         try:
             m = CSVMapLine(row, mapname=mapname)
             if m.cm < 0:
-                logging.error("Ignore marker with negative genetic distance")
+                logger.error("Ignore marker with negative genetic distance")
                 print(row.strip(), file=sys.stderr)
             else:
                 b.append(BedLine(m.bedline))
         except (IndexError, ValueError):  # header or mal-formed line
             continue
 
     b.print_to_file(filename=outfile, sorted=True)
-    logging.debug("A total of %d markers written to `%s`.", len(b), outfile)
+    logger.debug("A total of %d markers written to `%s`.", len(b), outfile)
 
     assert len(maps) == len(mapnames), "You have a collision in map names"
     write_weightsfile(mapnames, weightsfile=opts.weightsfile)
 
 
 def mergebed(args):
     """
@@ -1305,32 +1297,30 @@
             m.accn = "{0}-{1}".format(mapname, m.accn)
             m.extra = ["{0}:{1}".format(m.seqid, m.start)]
             b.append(m)
         except (IndexError, ValueError):  # header or mal-formed line
             continue
 
     b.print_to_file(filename=outfile, sorted=True)
-    logging.debug("A total of %d markers written to `%s`.", len(b), outfile)
+    logger.debug("A total of %d markers written to `%s`.", len(b), outfile)
 
     assert len(maps) == len(mapnames), "You have a collision in map names"
     write_weightsfile(mapnames, weightsfile=opts.weightsfile)
 
 
 def write_weightsfile(mapnames, weightsfile="weights.txt"):
     if op.exists(weightsfile):
-        logging.debug(
-            "Weights file `{0}` found. Will not overwrite.".format(weightsfile)
-        )
+        logger.debug("Weights file `%s` found. Will not overwrite.", weightsfile)
         return
 
     fw = open(weightsfile, "w")
     for mapname in sorted(mapnames):
         weight = 1
         print(mapname, weight, file=fw)
-    logging.debug("Weights file written to `%s`.", weightsfile)
+    logger.debug("Weights file written to `%s`.", weightsfile)
 
 
 def best_no_ambiguous(d, label):
     best, best_value = max(d.items(), key=lambda x: x[1])
     if list(d.values()).count(best_value) > 1:  # tie
         print("AMBIGUOUS", label, d, file=sys.stderr)
         return None, None
@@ -1459,18 +1449,16 @@
     gapsize = opts.gapsize
     mincount = opts.mincount
     ngen = opts.ngen
     npop = opts.npop
     cpus = opts.cpus
     seed = opts.seed
     if sys.version_info[:2] < (2, 7):
-        logging.debug(
-            "Python version: {0}. CPUs set to 1.".format(
-                sys.version.splitlines()[0].strip()
-            )
+        logger.debug(
+            "Python version: %s. CPUs set to 1.", sys.version.splitlines()[0].strip()
         )
         cpus = 1
 
     function = get_function(opts.distance)
     cc = Map(
         bedfile,
         function=function,
@@ -1480,15 +1468,15 @@
     mapnames = cc.mapnames
     allseqids = cc.seqids
     weights = Weights(weightsfile, mapnames)
     pivot = weights.pivot
     ref = weights.ref
     linkage = opts.linkage
     oseqid = opts.seqid
-    logging.debug("Linkage function: {0}-linkage".format(linkage))
+    logger.debug("Linkage function: %s-linkage", linkage)
     linkage = {
         "single": min,
         "double": double_linkage,
         "complete": max,
         "average": np.mean,
         "median": np.median,
     }[linkage]
@@ -1496,20 +1484,20 @@
     # Partition the linkage groups into consensus clusters
     C = Grouper()
     # Initialize the partitions
     for mlg in cc.mlgs:
         C.join(mlg)
 
     if partitionsfile:
-        logging.debug("Partition LGs based on `{}`".format(partitionsfile))
+        logger.debug("Partition LGs based on `%s`", partitionsfile)
         fp = open(partitionsfile)
         for row in fp:
             C.join(*row.strip().split(","))
     else:
-        logging.debug("Partition LGs based on {0}".format(ref))
+        logger.debug("Partition LGs based on %s", ref)
         for mapname in mapnames:
             if mapname == ref:
                 continue
             # Compute co-occurrence between LG pairs
             G = defaultdict(int)
             for s in allseqids:
                 s = Scaffold(s, cc)
@@ -1557,17 +1545,17 @@
     solutions = []
     for lgs, scaffolds in natsorted(partitions.items()):
         if oseqid and oseqid not in lgs:
             continue
         tag = "|".join(lgs)
         lgs_maps = set(x.split("-")[0] for x in lgs)
         if pivot not in lgs_maps:
-            logging.debug("Skipping {0} ...".format(tag))
+            logger.debug("Skipping %s ...", tag)
             continue
-        logging.debug("Working on {0} ...".format(tag))
+        logger.debug("Working on %s ...", tag)
         s = ScaffoldOO(
             lgs,
             scaffolds,
             cc,
             pivot,
             weights,
             sizes,
@@ -1589,15 +1577,15 @@
         conversion = {}
         for s in solutions:
             chrsizes[s.object] = (
                 sum(sizes[x] for (x, o) in s.tour) + (len(s.tour) - 1) * gapsize
             )
         for i, (c, size) in enumerate(sorted(chrsizes.items(), key=lambda x: -x[1])):
             newc = "chr{0}".format(i + 1)
-            logging.debug("{0}: {1} => {2}".format(c, size, newc))
+            logger.debug("%s: %d => %d", c, size, newc)
             conversion[c] = newc
         for s in solutions:
             s.object = conversion[s.object]
 
     # meta-data about the run parameters
     command = "# COMMAND: python -m jcvi.assembly.allmaps path {0}".format(
         " ".join(oargs)
@@ -1605,16 +1593,16 @@
     comment = "Generated by ALLMAPS {} ({})\n{}".format(version, get_today(), command)
     AGP.print_header(fwagp, comment=comment)
 
     for s in natsorted(solutions, key=lambda x: x.object):
         order_to_agp(s.object, s.tour, sizes, fwagp, gapsize=gapsize, evidence="map")
     fwagp.close()
 
-    logging.debug("AGP file written to `%s`.", agpfile)
-    logging.debug("Tour file written to `%s`.", tourfile)
+    logger.debug("AGP file written to `%s`.", agpfile)
+    logger.debug("Tour file written to `%s`.", tourfile)
 
     build([inputbed, fastafile])
 
     summaryfile = pf + ".summary.txt"
     summary([inputbed, fastafile, "--outfile={0}".format(summaryfile)])
 
     if not opts.noplot:
@@ -1634,15 +1622,15 @@
     scaffolds_seen = set(x.component_id for x in agp)
     sizes = Sizes(scaffolds).mapping
     fwagp = must_open(unplaced_agp, "w")
     for s in natsorted(sizes.keys()):
         if s in scaffolds_seen:
             continue
         order_to_agp(s, [(s, "?")], sizes, fwagp)
-    logging.debug("Write unplaced AGP to `%s`", unplaced_agp)
+    logger.debug("Write unplaced AGP to `%s`", unplaced_agp)
 
 
 def summary(args):
     """
     %prog summary input.bed scaffolds.fasta
 
     Print out summary statistics per map, followed by consensus summary of
@@ -1760,15 +1748,15 @@
 
     chainfile = pf + ".chain"
     if need_update((combined_agp, scaffolds, combined_fasta), chainfile):
         fromagp([combined_agp, scaffolds, combined_fasta])
 
     liftedbed = mapbed.rsplit(".", 1)[0] + ".lifted.bed"
     if need_update((mapbed, chainfile), liftedbed):
-        logging.debug(
+        logger.debug(
             "Lifting markers from positions in `%s` to new positions in `%s`",
             mapbed,
             liftedbed,
         )
         liftover(chainfile, mapbed, liftedbed, unmapfile="unmapped", cstyle="l")
 
     if opts.cleanup:
@@ -1809,23 +1797,23 @@
 
     Plot the matchings between the reconstructed pseudomolecules and the maps.
     Two types of visualizations are available in one canvas:
 
     1. Parallel axes, and matching markers are shown in connecting lines;
     2. Scatter plot.
     """
-    from jcvi.graphics.base import (
+    from ..graphics.base import (
         plt,
         savefig,
         normalize_axes,
         set2,
         panel_labels,
         shorten,
     )
-    from jcvi.graphics.chromosome import Chromosome, GeneticMap, HorizontalChromosome
+    from ..graphics.chromosome import Chromosome, GeneticMap, HorizontalChromosome
 
     p = OptionParser(plot.__doc__)
     p.add_option("--title", help="Title of the plot")
     add_allmaps_plot_options(p)
     opts, args, iopts = p.set_image_options(args, figsize="10x6")
 
     if len(args) != 2:
@@ -1844,16 +1832,16 @@
     mapnames = cc.mapnames
     weights = Weights(weightsfile, mapnames)
     assert seqid in allseqids, "{0} not in {1}".format(seqid, allseqids)
 
     s = Scaffold(seqid, cc)
     mlgs = [k for k, v in s.mlg_counts.items() if v >= links]
     while not mlgs:
-        links /= 2
-        logging.error("No markers to plot, --links reset to {0}".format(links))
+        links //= 2
+        logger.error("No markers to plot, --links reset to %d", links)
         mlgs = [k for k, v in s.mlg_counts.items() if v >= links]
 
     mlgsizes = {}
     for mlg in mlgs:
         mm = cc.extract_mlg(mlg)
         mlgsize = max(function(x) for x in mm)
         mlgsizes[mlg] = mlgsize
@@ -1994,15 +1982,15 @@
             ha = "right" if i % 2 else "left"
         root.text(0.5, ypos, tlg, color=color, rotation=90, ha=ha, va="center")
 
     if opts.panels:
         labels = ((0.04, 0.96, "A"), (0.48, 0.96, "B"))
         panel_labels(root, labels)
 
-    normalize_axes((ax1, ax2, root))
+    normalize_axes(ax1, ax2, root)
     image_name = seqid + "." + iopts.format
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
     plt.close(fig)
     return image_name
 
 
 def plotall(xargs):
```

### Comparing `jcvi-1.4.5/jcvi/assembly/allpaths.py` & `jcvi-1.4.6/jcvi/assembly/allpaths.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/assembly/automaton.py` & `jcvi-1.4.6/jcvi/assembly/automaton.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/assembly/base.py` & `jcvi-1.4.6/jcvi/assembly/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/assembly/ca.py` & `jcvi-1.4.6/jcvi/assembly/goldenpath.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1216 +1,1192 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
-Prepare input files for Celera Assembler, dispatch based on file suffix::
-
-*.fasta: convert-fasta-to-v2.pl
-*.sff: sffToCA
-*.fastq: fastqToCA
+Procedures to validate and update golden path of a genome assembly. This relies
+heavily on formats.agp, and further includes several algorithms, e.g. overlap
+detection.
 """
-import logging
+import os
 import os.path as op
 import sys
-from pickle import dump, load
+import shutil
+import logging
 
-import networkx as nx
-from collections import Counter
-from random import choice
-from Bio import SeqIO
-
-from jcvi.formats.base import must_open
-from jcvi.formats.fasta import Fasta, SeqRecord, filter, format, parse_fasta
-from jcvi.formats.blast import Blast
-from jcvi.utils.console import printf
-from jcvi.utils.range import range_minmax
-from jcvi.algorithms.graph import graph_stats, graph_local_neighborhood
+from copy import deepcopy
+from functools import lru_cache
+from itertools import groupby
+
+from jcvi.formats.agp import AGP, TPF, get_phase, reindex, tidy, build
+from jcvi.formats.base import BaseFile, must_open
+from jcvi.formats.fasta import Fasta, SeqIO
+from jcvi.formats.blast import BlastSlow, BlastLine
+from jcvi.formats.coords import Overlap_types
+from jcvi.apps.fetch import entrez
+from jcvi.apps.grid import WriteJobs
 from jcvi.apps.base import (
     OptionParser,
     ActionDispatcher,
+    cleanup,
+    popen,
+    mkdir,
     sh,
     need_update,
-    glob,
-    get_abs_path,
-    popen,
 )
 
 
-def main():
+GoodPct = 98
+GoodOverlap = 200
+GoodOverhang = 2000
 
-    actions = (
-        ("tracedb", "convert trace archive files to frg file"),
-        ("clr", "prepare vector clear range file based on BLAST to vectors"),
-        ("fasta", "convert fasta to frg file"),
-        ("sff", "convert 454 reads to frg file"),
-        ("fastq", "convert Illumina reads to frg file"),
-        ("shred", "shred contigs into pseudo-reads"),
-        ("astat", "generate the coverage-rho scatter plot"),
-        ("unitigs", "output uniquely extended unitigs based on best.edges"),
-        ("merger", "merge reads into unitigs offline"),
-        ("removecontains", "remove contained reads from gkpStore"),
-        ("graph", "visualize best.edges"),
-        ("prune", "prune overlap graph"),
-        ("overlap", "visualize overlaps for a given fragment"),
-    )
-    p = ActionDispatcher(actions)
-    p.dispatch(globals())
 
+class Cutoff(object):
+    def __init__(self, pctid=GoodPct, overlap=GoodOverlap, hang=GoodOverhang):
+        self.pctid = pctid
+        self.overlap = overlap
+        self.hang = hang
+
+    def __str__(self):
+        return "Configuration: PCTID={} OVERLAP={} HANG={}".format(
+            self.pctid, self.overlap, self.hang
+        )
 
-frgTemplate = """{{FRG
-act:A
-acc:{fragID}
-rnd:1
-sta:G
-lib:{libID}
-pla:0
-loc:0
-src:
-.
-seq:
-{seq}
-.
-qlt:
-{qvs}
-.
-hps:
-.
-clr:{clr_beg},{clr_end}
-}}"""
-
-headerTemplate = """{{VER
-ver:2
-}}
-{{LIB
-act:A
-acc:{libID}
-ori:U
-mea:0.000
-std:0.000
-src:
-.
-nft:17
-fea:
-forceBOGunitigger=1
-isNotRandom=0
-doNotTrustHomopolymerRuns=0
-doTrim_initialNone=1
-doTrim_initialMerBased=0
-doTrim_initialFlowBased=0
-doTrim_initialQualityBased=0
-doRemoveDuplicateReads=1
-doTrim_finalLargestCovered=1
-doTrim_finalEvidenceBased=0
-doTrim_finalBestEdge=0
-doRemoveSpurReads=1
-doRemoveChimericReads=1
-doCheckForSubReads=0
-doConsensusCorrection=0
-forceShortReadFormat=0
-constantInsertSize=0
-.
-}}"""
 
+class CLR(object):
+    def __init__(self, id, size, orientation="+"):
+        self.id = id
+        self.start = 1
+        self.end = size
+        if orientation == "?":
+            orientation = "+"
+        assert orientation in ("+", "-")
+        self.orientation = orientation
+
+    def __str__(self):
+        return "{}: {}-{}({})".format(self.id, self.start, self.end, self.orientation)
+
+    @property
+    def is_valid(self):
+        return self.start < self.end
+
+    @classmethod
+    def from_agpline(cls, a):
+        c = CLR(a.component_id, 0, a.orientation)
+        c.start = a.component_beg
+        c.end = a.component_end
+        return c
+
+
+class Overlap(object):
+    def __init__(self, blastline, asize, bsize, cutoff, qreverse=False):
+
+        b = blastline
+        aid = b.query
+        bid = b.subject
+
+        self.aid = aid.split("|")[3] if aid.count("|") >= 3 else aid
+        self.bid = bid.split("|")[3] if bid.count("|") >= 3 else bid
+        self.asize = asize
+        self.bsize = bsize
+
+        self.qstart = b.qstart
+        self.qstop = b.qstop
+        self.sstart = b.sstart
+        self.sstop = b.sstop
+
+        self.pctid = b.pctid
+        self.hitlen = b.hitlen
+        self.orientation = b.orientation
+
+        self.cutoff = cutoff
+        self.qreverse = qreverse
+        self.blastline = b
+
+    def __str__(self):
+        ov = Overlap_types[self.otype]
+        s = "{0} - {1}: {2} ".format(self.aid, self.bid, ov)
+        s += "Overlap: {0} Identity: {1}% Orientation: {2}".format(
+            self.hitlen, self.pctid, self.orientation
+        )
+        return s
 
-class OverlapLine(object):
+    @property
+    def swapped(self):
+        blastline = self.blastline.swapped
+        asize = self.asize
+        bsize = self.bsize
+        _, bo = self.get_ao_bo()
+        qreverse = bo == "-"
+        return Overlap(blastline, bsize, asize, self.cutoff, qreverse=qreverse)
+
+    @property
+    def certificateline(self):
+        terminal_tag = "Terminal" if self.isTerminal else "Non-terminal"
+        return "\t".join(
+            str(x)
+            for x in (
+                self.bid,
+                self.asize,
+                self.qstart,
+                self.qstop,
+                self.orientation,
+                terminal_tag,
+            )
+        )
 
-    # See doc: http://wgs-assembler.sourceforge.net/wiki/index.php/OverlapStore
-    def __init__(self, line):
-        args = line.split()
-        self.aid = int(args[0])
-        self.bid = int(args[1])
-        self.orientation = args[2]
-        self.ahang = int(args[3])
-        self.bhang = int(args[4])
-        self.erate = float(args[5])
-        self.erate_adj = float(args[6])
+    @property
+    def isTerminal(self):
+        return self.isGoodQuality and self.otype in (1, 2)
+
+    @property
+    def isGoodQuality(self):
+        cutoff = self.cutoff
+        return self.hitlen >= cutoff.overlap and self.pctid >= cutoff.pctid
+
+    def get_hangs(self):
+        r"""
+        Determine the type of overlap given query, ref alignment coordinates
+        Consider the following alignment between sequence a and b:
+
+        aLhang \              / aRhang
+                \------------/
+                /------------\
+        bLhang /              \ bRhang
+
+        Terminal overlap: a before b, b before a
+        Contain overlap: a in b, b in a
+        """
+        aLhang, aRhang = self.qstart - 1, self.asize - self.qstop
+        bLhang, bRhang = self.sstart - 1, self.bsize - self.sstop
+        if self.orientation == "-":
+            bLhang, bRhang = bRhang, bLhang
+        if self.qreverse:
+            aLhang, aRhang = aRhang, aLhang
+            bLhang, bRhang = bRhang, bLhang
+
+        return aLhang, aRhang, bLhang, bRhang
+
+    def update_clr(self, aclr, bclr):
+        """
+        Zip the two sequences together, using "left-greedy" rule
+
+        =============                   seqA
+                 ||||
+                 ====(===============)  seqB
+        """
+        print(aclr, bclr, file=sys.stderr)
+        otype = self.otype
+
+        if otype == 1:
+            if aclr.orientation == "+":
+                aclr.end = self.qstop
+            else:
+                aclr.start = self.qstart
+            if bclr.orientation == "+":
+                bclr.start = self.sstop + 1
+            else:
+                bclr.end = self.sstart - 1
 
+        elif otype == 3:
+            aclr.start = aclr.end
 
-def add_graph_options(p):
-    p.add_option("--maxerr", default=100, type="int", help="Maximum error rate")
-    p.add_option(
-        "--frgctg",
-        default="../9-terminator/asm.posmap.frgctg",
-        help="Annotate graph with contig membership",
-    )
+        elif otype == 4:
+            bclr.start = bclr.end
 
+        print(aclr, bclr, file=sys.stderr)
 
-def prune(args):
-    """
-    %prog prune best.edges
+    def get_ao_bo(self):
+        ao = "-" if self.qreverse else "+"
+        bo = ao if self.orientation == "+" else {"+": "-", "-": "+"}[ao]
+        return ao, bo
 
-    Prune overlap graph.
-    """
-    from collections import defaultdict
+    def anneal(self, aclr, bclr):
+        ao, bo = self.get_ao_bo()
 
-    p = OptionParser(prune.__doc__)
-    add_graph_options(p)
-    opts, args = p.parse_args(args)
+        # Requirement: end-to-end join in correct order and orientation
+        can_anneal = self.otype in (1, 3, 4) and (ao, bo) == (
+            aclr.orientation,
+            bclr.orientation,
+        )
+        if not can_anneal:
+            print(
+                "* Cannot anneal! (otype={0}|{1}{2}|{3}{4})".format(
+                    self.otype, ao, bo, aclr.orientation, bclr.orientation
+                ),
+                file=sys.stderr,
+            )
+            return False
 
-    if len(args) != 1:
-        sys.exit(not p.print_help())
+        self.update_clr(aclr, bclr)
+        return True
 
-    (bestedges,) = args
-    G = read_graph(bestedges, maxerr=opts.maxerr)
-    reads_to_ctgs = parse_ctgs(opts.frgctg)
-    edges = defaultdict(int)
-    r = defaultdict(int)
-    for a, b, d in G.edges_iter(data=True):
-        ua, ub = reads_to_ctgs.get(a), reads_to_ctgs.get(b)
-        nn = (ua, ub).count(None)
-        if nn == 0:
-            if ua == ub:
-                r["Same tigs"] += 1
-            else:
-                r["Diff tigs"] += 1
-                if ua > ub:
-                    ua, ub = ub, ua
-                edges[(ua, ub)] += 1
-        elif nn == 1:
-            r["One null"] += 1
+    def print_graphic(self):
+        """
+        >>>>>>>>>>>>>>>>>>>             seqA (alen)
+                  ||||||||
+                 <<<<<<<<<<<<<<<<<<<<<  seqB (blen)
+        """
+        aLhang, aRhang, bLhang, bRhang = self.get_hangs()
+
+        achar = ">"
+        bchar = "<" if self.orientation == "-" else ">"
+        if self.qreverse:
+            achar = "<"
+            bchar = {">": "<", "<": ">"}[bchar]
+
+        print(aLhang, aRhang, bLhang, bRhang, file=sys.stderr)
+        width = 50  # Canvas
+        hitlen = self.hitlen
+        lmax = max(aLhang, bLhang)
+        rmax = max(aRhang, bRhang)
+        bpwidth = lmax + hitlen + rmax
+        ratio = width * 1.0 / bpwidth
+
+        _ = lambda x: int(round(x * ratio, 0))
+        a1, a2 = _(aLhang), _(aRhang)
+        b1, b2 = _(bLhang), _(bRhang)
+        hit = max(_(hitlen), 1)
+
+        msg = " " * max(b1 - a1, 0)
+        msg += achar * (a1 + hit + a2)
+        msg += " " * (width - len(msg) + 2)
+        msg += "{0} ({1})".format(self.aid, self.asize)
+        print(msg, file=sys.stderr)
+
+        msg = " " * max(a1, b1)
+        msg += "|" * hit
+        print(msg, file=sys.stderr)
+
+        msg = " " * max(a1 - b1, 0)
+        msg += bchar * (b1 + hit + b2)
+        msg += " " * (width - len(msg) + 2)
+        msg += "{0} ({1})".format(self.bid, self.bsize)
+        print(msg, file=sys.stderr)
+        print(self, file=sys.stderr)
+
+    @property
+    def otype(self):
+        if not self.isGoodQuality:
+            return 0
+
+        aLhang, aRhang, bLhang, bRhang = self.get_hangs()
+
+        s1 = aRhang + bLhang
+        s2 = aLhang + bRhang
+        s3 = aLhang + aRhang
+        s4 = bLhang + bRhang
+        ms = min(s1, s2, s3, s4)
+        if ms > self.cutoff.hang:
+            type = 0
+        elif ms == s1:
+            type = 1  # a ~ b
+        elif ms == s2:
+            type = 2  # b ~ a
+        elif ms == s3:
+            type = 3  # a in b
+        elif ms == s4:
+            type = 4  # b in a
         else:
-            assert nn == 2
-            r["Two nulls"] += 1
-
-    U = nx.Graph()
-    difftigs = "diff_tigs.txt"
-    neighbors = defaultdict(list)
-    fw = open(difftigs, "w")
-    for (ua, ub), count in edges.items():
-        print("\t".join((ua, ub, str(count))), file=fw)
-        U.add_edge(ua, ub, weight=count)
-        neighbors[ua].append((ub, count))
-        neighbors[ub].append((ua, count))
-    fw.close()
-
-    print("[Unitig edge property]", file=sys.stderr)
-    for k, v in r.items():
-        print(": ".join((k, str(v))), file=sys.stderr)
-    print("Total: {0}".format(sum(r.values())), file=sys.stderr)
-
-    print("[Unitig degree distribution]", file=sys.stderr)
-    degrees = U.degree()
-    degree_counter = Counter(degrees.values())
-    for degree, count in sorted(degree_counter.items()):
-        print("{0}\t{1}".format(degree, count), file=sys.stderr)
-
-    # To find associative contigs, one look for a contig that is connected and
-    # only connected to another single contig - and do that recursively until no
-    # more contigs can be found
-    associative = {}
-    for ua, ubs in neighbors.items():
-        if len(ubs) == 1:  # Only one neighbor
-            ub, count = ubs[0]
-            if count >= 2:  # Bubble
-                associative[ua] = (ub, count)
-    print(
-        "A total of {0} associative contigs found".format(len(associative)),
-        file=sys.stderr,
-    )
-
-    # Keep only one for mutual associative
-    for ua, ub in associative.items():
-        if ub in associative and ua < ub:
-            print(ua, "mutually associative with", ub, file=sys.stderr)
-            del associative[ub]
-    print(
-        "A total of {0} associative contigs retained".format(len(associative)),
-        file=sys.stderr,
-    )
+            assert 0
 
-    assids = "associative.ids"
-    fw = open(assids, "w")
-    for ua, (ub, count) in sorted(associative.items(), key=lambda x: (x[1], x[0])):
-        print("\t".join((ua, ub, str(count))), file=fw)
-    fw.close()
-    logging.debug("Associative contigs written to `{0}`".format(assids))
+        return type
 
 
-def removecontains(args):
+class CertificateLine(object):
     """
-    %prog removecontains 4-unitigger/best.contains asm.gkpStore
-
-    Remove contained reads from gkpStore. This will improve assembly contiguity
-    without sacrificing accuracy, when using bogart unitigger.
+    North  chr1  2  0  AC229737.8  telomere     58443
+    South  chr1  2  1  AC229737.8  AC202463.29  58443  37835  58443  + Non-terminal
     """
-    p = OptionParser(removecontains.__doc__)
-    opts, args = p.parse_args(args)
-
-    if len(args) != 2:
-        sys.exit(not p.print_help())
-
-    contains, gkpStore = args
-
-    s = set()
-    fp = open(contains)
-    for row in fp:
-        if row[0] == "#":
-            continue
-        iid = int(row.split()[0])
-        s.add(iid)
 
-    cmd = "gatekeeper -dumpfragments -lastfragiid {}".format(gkpStore)
-    gkpmsg = popen(cmd).read()
-    last_iid = int(gkpmsg.strip().split()[-1])
-
-    ndeleted = 0
-    editfile = "delete.edit"
-    fw = open(editfile, "w")
-    for iid in range(1, last_iid + 1):
-        if iid in s:
-            print("frg iid {0} isdeleted 1".format(iid), file=fw)
-            ndeleted += 1
+    def __init__(self, line):
+        args = line.split()
+        self.tag = args[0]
+        self.chr = args[1]
+        self.aphase = int(args[2])
+        self.bphase = int(args[3])
+        self.aid = args[4]
+        self.bid = args[5]
+        self.asize = int(args[6])
+        self.is_no_overlap = False
 
-    fw.close()
-    assert len(s) == ndeleted
-    logging.debug("A total of {0} contained reads flagged as deleted.".format(ndeleted))
-    print("Now you can run:", file=sys.stderr)
-    print("$ gatekeeper --edit {0} {1}".format(editfile, gkpStore), file=sys.stderr)
+        if len(args) == 7:
+            self.is_gap = True
+            return
 
+        self.is_gap = False
 
-def overlap(args):
-    """
-    %prog overlap best.contains iid
+        if len(args) == 8:
+            assert args[7] == "None"
+            self.is_no_overlap = True
+            self.terminal = "Non-terminal"
+            return
 
-    Visualize overlaps for a given fragment. Must be run in 4-unitigger. All
-    overlaps for iid were retrieved, excluding the ones matching best.contains.
-    """
-    p = OptionParser(overlap.__doc__)
-    p.add_option("--maxerr", default=2, type="int", help="Maximum error rate")
-    p.add_option("--canvas", default=100, type="int", help="Canvas size")
-    opts, args = p.parse_args(args)
+        self.astart = int(args[7])
+        self.astop = int(args[8])
+        self.orientation = args[9]
+        self.terminal = args[10]
+
+    @property
+    def isTerminal(self):
+        return self.terminal == "Terminal"
+
+    def __str__(self):
+        ar = [
+            self.tag,
+            self.chr,
+            self.aphase,
+            self.bphase,
+            self.aid,
+            self.bid,
+            self.asize,
+        ]
+
+        if self.is_no_overlap:
+            ar += ["None"]
+        elif not self.is_gap:
+            ar += [self.astart, self.astop, self.orientation, self.terminal]
+
+        return "\t".join(str(x) for x in ar)
+
+
+class Certificate(BaseFile):
+
+    gapsize = 100000
+    gaps = dict(
+        telomere=gapsize, centromere=gapsize, contig=gapsize, clone=50000, fragment=5000
+    )
+
+    def __init__(self, filename):
+
+        super(Certificate, self).__init__(filename)
+
+        fp = open(filename)
+        self.lines = [CertificateLine(x) for x in fp.readlines()]
+
+    def write(self, filename):
+        fw = must_open(filename, "w")
+        for b in self.lines:
+            print(b, file=fw)
+
+    def get_agp_gap(self, gap_type="contig"):
+        gap_length = Certificate.gaps[gap_type]
+        linkage = "yes" if gap_type in ("fragment", "clone") else "no"
+
+        return ["N", gap_length, gap_type, linkage, ""]
+
+    def write_AGP(self, filename, orientationguide={}):
+        """
+        For each component, we have two overlaps: North and South.
+
+        =======
+           ||||             South
+           ====(=================)  Current BAC
+           North             ||||
+                             ===============
+
+        For the case that says "Non-terminal", the overlap will not be
+        considered. North-South would suggest a '+' orientation, South-North
+        would suggest a '-' orientation. In most cases, unless the overlap
+        involves phase1 BAC, the selected range will be shown as the brackets
+        above - exclude North overlap, and include South overlap (aka the
+        "left-greedy" rule).
+        """
+        fw = must_open(filename, "w")
+        for aid, bb in groupby(self.lines, key=lambda x: x.aid):
+            bb = list(bb)
+            north, south = bb
+            aid = north.aid
+            assert aid == south.aid
+
+            aphase = north.aphase
+            chr = north.chr
+            size = north.asize
+            ar = [chr, 0, 0, 0]
+
+            northline = southline = None
+            northrange = southrange = None
+
+            # Warn if adjacent components do not have valid overlaps
+            if south.is_no_overlap:
+                print(south, file=sys.stderr)
+
+            # Most gaps, except telomeres occur twice, so only do the "North"
+            if north.is_gap:
+                bar = ar + self.get_agp_gap(north.bid)
+                northline = "\t".join(str(x) for x in bar)
+            else:
+                if north.isTerminal:
+                    northrange = north.astart, north.astop
 
-    if len(args) != 2:
-        sys.exit(not p.print_help())
+            if south.is_gap:
+                if south.bid == "telomere":
+                    bar = ar + self.get_agp_gap(south.bid)
+                    southline = "\t".join(str(x) for x in bar)
+            else:
+                if south.isTerminal:
+                    southrange = south.astart, south.astop
+                else:
+                    bar = ar + self.get_agp_gap("fragment")
+                    southline = "\t".join(str(x) for x in bar)
 
-    bestcontains, iid = args
-    canvas = opts.canvas
+            # Determine the orientation and clear range for the current BAC
+            clr = [1, size]
+            orientation = sorientation = None
+            if northrange:
+                start, stop = northrange
+                Lhang = start - 1
+                Rhang = size - stop
+
+                orientation = "+" if Lhang < Rhang else "-"
+                if north.bphase == 1 and north.bphase < aphase:
+                    if Lhang < Rhang:  # North overlap at 5`
+                        clr[0] = start
+                    else:
+                        clr[1] = stop
+                # Override left-greedy (also see below)
+                else:
+                    if Lhang < Rhang:
+                        clr[0] = stop + 1
+                    else:
+                        clr[1] = start - 1
+
+            if southrange:
+                start, stop = southrange
+                Lhang = start - 1
+                Rhang = size - stop
+
+                sorientation = "+" if Lhang > Rhang else "-"
+                # Override left-greedy (also see above)
+                if aphase == 1 and aphase < south.bphase:
+                    if Lhang < Rhang:  # South overlap at 5`
+                        clr[0] = stop + 1
+                    else:
+                        clr[1] = start - 1
+                else:
+                    if Lhang < Rhang:
+                        clr[0] = start
+                    else:
+                        clr[1] = stop
+
+            if orientation:
+                if sorientation:
+                    try:
+                        assert (
+                            orientation == sorientation
+                        ), "Orientation conflicts:\n{0}\n{1}".format(north, south)
+                    except AssertionError as e:
+                        logging.debug(e)
+            else:
+                if sorientation:
+                    orientation = sorientation
+                else:  # Both overlaps fail to define orientation
+                    orientation = orientationguide.get(aid, "+")
+
+            component_type = "D" if aphase in (1, 2) else "F"
+            bar = ar + [component_type, aid, clr[0], clr[1], orientation]
+            cline = "\t".join(str(x) for x in bar)
+
+            if northline:
+                print(northline, file=fw)
+            print(cline, file=fw)
+            if southline:
+                print(southline, file=fw)
 
-    bestcontainscache = bestcontains + ".cache"
-    if need_update(bestcontains, bestcontainscache):
-        fp = open(bestcontains)
-        fw = open(bestcontainscache, "w")
-        exclude = set()
-        for row in fp:
-            if row[0] == "#":
-                continue
-            j = int(row.split()[0])
-            exclude.add(j)
-        dump(exclude, fw)
         fw.close()
 
-    exclude = load(open(bestcontainscache))
-    logging.debug("A total of {0} reads to exclude".format(len(exclude)))
-
-    cmd = "overlapStore -d ../asm.ovlStore -b {0} -e {0}".format(iid)
-    cmd += " -E {0}".format(opts.maxerr)
-    frags = []
-    for row in popen(cmd):
-        r = OverlapLine(row)
-        if r.bid in exclude:
-            continue
-        frags.append(r)
+        reindex([filename, "--inplace"])
 
-    # Also include to query fragment
-    frags.append(OverlapLine("{0} {0} N 0 0 0 0".format(iid)))
-    frags.sort(key=lambda x: x.ahang)
-
-    # Determine size of the query fragment
-    cmd = "gatekeeper -b {0} -e {0}".format(iid)
-    cmd += " -tabular -dumpfragments ../asm.gkpStore"
-    fp = popen(cmd)
-    size = int(next(fp).split()[-1])
 
-    # Determine size of canvas
-    xmin = min(x.ahang for x in frags)
-    xmax = max(x.bhang for x in frags)
-    xsize = -xmin + size + xmax
-    ratio = xsize / canvas
-
-    for f in frags:
-        fsize = -f.ahang + size + f.bhang
-        a = (f.ahang - xmin) / ratio
-        b = fsize / ratio
-        t = "-" * b
-        if f.orientation == "N":
-            t = t[:-1] + ">"
-        else:
-            t = "<" + t[1:]
-        if f.ahang == 0 and f.bhang == 0:
-            t = "[green]{}".format(t)
-        c = canvas - a - b
-        printf(
-            "{}{}{}{} ({})".format(
-                " " * a, t, " " * c, str(f.bid).rjust(10), f.erate_adj
-            ),
-        )
+def main():
 
+    actions = (
+        ("bes", "confirm the BES mapping"),
+        ("flip", "flip the FASTA sequences according to a set of references"),
+        ("overlap", "check terminal overlaps between two records"),
+        ("batchoverlap", "check terminal overlaps for many pairs"),
+        ("neighbor", "check neighbors of a component in agpfile"),
+        ("blast", "blast a component to componentpool"),
+        ("certificate", "make certificates for all overlaps in agpfile"),
+        ("agp", "make agpfile based on certificates"),
+        ("anneal", "merge adjacent contigs and make new agpfile"),
+        ("dedup", "remove redundant contigs with cdhit"),
+    )
+    p = ActionDispatcher(actions)
+    p.dispatch(globals())
 
-def parse_ctgs(frgtoctg):
-    cache = "frgtoctg.cache"
-    if need_update(frgtoctg, cache):
-        reads_to_ctgs = {}
-        frgtodeg = frgtoctg.replace(".frgctg", ".frgdeg")
-        iidtouid = frgtoctg.replace(".posmap.frgctg", ".iidtouid")
-        fp = open(iidtouid)
-        frgstore = {}
-        for row in fp:
-            tag, iid, uid = row.split()
-            if tag == "FRG":
-                frgstore[uid] = int(iid)
-
-        for pf, f in zip(("ctg", "deg"), (frgtoctg, frgtodeg)):
-            fp = open(f)
-            logging.debug("Parse posmap file `{0}`".format(f))
-            for row in fp:
-                frg, ctg = row.split()[:2]
-                frg = frgstore[frg]
-                reads_to_ctgs[frg] = pf + ctg
-            logging.debug("Loaded mapping: {0}".format(len(reads_to_ctgs)))
 
-        fw = open(cache, "w")
-        dump(reads_to_ctgs, fw)
-        fw.close()
-        logging.debug("Contig mapping written to `{0}`".format(cache))
+def dedup(args):
+    """
+    %prog dedup scaffolds.fasta
 
-    reads_to_ctgs = load(open(cache))
-    logging.debug("Contig mapping loaded from `{0}`".format(cache))
-    return reads_to_ctgs
+    Remove redundant contigs with CD-HIT. This is run prior to
+    assembly.sspace.embed().
+    """
+    from jcvi.formats.fasta import gaps
+    from jcvi.apps.cdhit import deduplicate, ids
 
+    p = OptionParser(dedup.__doc__)
+    p.set_align(pctid=GoodPct)
+    p.set_mingap(default=10)
+    opts, args = p.parse_args(args)
 
-def read_graph(bestedges, maxerr=100, directed=False):
-    logging.debug("Max error = {0}%".format(maxerr))
-    tag = "dir." if directed else ""
-    bestgraph = bestedges.split(".")[0] + ".err{0}.{1}graph".format(maxerr, tag)
-    if need_update(bestedges, bestgraph):
-        G = {} if directed else nx.Graph()
-        fp = open(bestedges)
-        best_store = {}
-        for row in fp:
-            if row[0] == "#":
-                continue
-            id1, lib_id, best5, o5, best3, o3, j1, j2 = row.split()
-            id1, best5, best3 = int(id1), int(best5), int(best3)
-            j1, j2 = float(j1), float(j2)
-            if j1 <= maxerr or j2 <= maxerr:
-                if not directed:
-                    G.add_node(id1)
-                id1p5, id1p3 = "{0}-5'".format(id1), "{0}-3'".format(id1)
-                best5o5 = "{0}-{1}".format(best5, o5)
-                best3o3 = "{0}-{1}".format(best3, o3)
-                best_store[id1p5] = best5o5
-                best_store[id1p3] = best3o3
-            if best5 and j1 <= maxerr:
-                if directed:
-                    G[id1p5] = best5o5
-                else:
-                    G.add_edge(best5, id1, weight=10)
-            if best3 and j2 <= maxerr:
-                if directed:
-                    G[id1p3] = best3o3
-                else:
-                    G.add_edge(id1, best3, weight=10)
+    if len(args) != 1:
+        sys.exit(not p.print_help())
 
-        # Annotate edge weight for mutual best link, note that edge weights are
-        # (11) set close to 10, to minimize impact to layout (Yifan Hu's
-        # multilevel)
-        nmutuals = 0
-        for k, v in best_store.items():
-            if best_store.get(v) == k and k < v:
-                k, v = int(k.split("-")[0]), int(v.split("-")[0])
-                G[k][v]["weight"] = 11
-                nmutuals += 1
-        logging.debug("Mutual best edges: {0}".format(nmutuals))
-
-        if directed:
-            fw = open(bestgraph, "w")
-            dump(G, fw)
-            fw.close()
-        else:
-            nx.write_gpickle(G, bestgraph)
-        logging.debug("Graph pickled to `{0}`".format(bestgraph))
+    (scaffolds,) = args
+    mingap = opts.mingap
+    splitfile, oagpfile, cagpfile = gaps(
+        [scaffolds, "--split", "--mingap={0}".format(mingap)]
+    )
+
+    dd = splitfile + ".cdhit"
+    clstrfile = dd + ".clstr"
+    idsfile = dd + ".ids"
+    if need_update(splitfile, clstrfile):
+        deduplicate([splitfile, "--pctid={0}".format(opts.pctid)])
+    if need_update(clstrfile, idsfile):
+        ids([clstrfile])
+
+    agp = AGP(cagpfile)
+    reps = set(x.split()[-1] for x in open(idsfile))
+    pf = scaffolds.rsplit(".", 1)[0]
+    dedupagp = pf + ".dedup.agp"
+    fw = open(dedupagp, "w")
+
+    ndropped = ndroppedbases = 0
+    for a in agp:
+        if not a.is_gap and a.component_id not in reps:
+            span = a.component_span
+            logging.debug("Drop component {0} ({1})".format(a.component_id, span))
+            ndropped += 1
+            ndroppedbases += span
+            continue
+        print(a, file=fw)
+    fw.close()
 
-        # Compute node degree histogram and save in (degree, counts) tab file
-        degrees = G.degree()
-        degree_counter = Counter(degrees.values())
-        degreesfile = "degrees.txt"
-        fw = open(degreesfile, "w")
-        for degree, count in sorted(degree_counter.items()):
-            print("{0}\t{1}".format(degree, count), file=fw)
-        fw.close()
-        logging.debug("Node degree distribution saved to `{0}`".format(degreesfile))
+    logging.debug(
+        "Dropped components: {0}, Dropped bases: {1}".format(ndropped, ndroppedbases)
+    )
+    logging.debug("Deduplicated file written to `{0}`.".format(dedupagp))
 
-        # Save high degree (top 1%) nodes in save in (node, degree) tab file
-        percentile = sorted(degrees.values(), reverse=True)[len(degrees) / 1000]
-        logging.debug("Top 0.1% has degree of at least {0}".format(percentile))
-        hubs = [(k, v) for k, v in degrees.items() if v >= percentile]
-        hubs.sort(key=lambda x: x[1], reverse=True)  # degress descending
-        hubsfile = "hubs.txt"
-        fw = open(hubsfile, "w")
-        for node, degree in hubs:
-            print("{0}\t{1}".format(node, degree), file=fw)
-        fw.close()
-        logging.debug("Hubs saved to `{0}`".format(hubsfile))
+    tidyagp = tidy([dedupagp, splitfile])
+    dedupfasta = pf + ".dedup.fasta"
+    build([tidyagp, dd, dedupfasta])
 
-    logging.debug("Read graph from `{0}`".format(bestgraph))
-    if directed:
-        G = load(open(bestgraph))
-    else:
-        G = nx.read_gpickle(bestgraph)
-        graph_stats(G)
-    return G
+    return dedupfasta
 
 
-def merger(args):
+def get_shred_id(id):
     """
-    %prog merger layout gkpStore contigs.fasta
-
-    Merge reads into one contig.
+    >>> get_shred_id("ca-bacs.5638.frag11.22000-23608")
+    ("ca-bacs.5638", 11)
     """
-    p = OptionParser(merger.__doc__)
-    opts, args = p.parse_args(args)
+    try:
+        parts = id.split(".")
+        aid = ".".join(parts[:2])
+        fid = int(parts[2].replace("frag", ""))
+    except:
+        aid, fid = None, None
+    return aid, fid
 
-    if len(args) != 3:
-        sys.exit(not p.print_help())
 
-    layout, gkpstore, contigs = args
-    fp = open(layout)
-    pf = "0"
-    iidfile = pf + ".iids"
-    for i, row in enumerate(fp):
-        logging.debug("Read unitig {0}".format(i))
-        fw = open(iidfile, "w")
-        layout = row.split("|")
-        print("\n".join(layout), file=fw)
-        fw.close()
-        cmd = "gatekeeper -iid {0}.iids -dumpfasta {0} {1}".format(pf, gkpstore)
-        sh(cmd)
+def is_adjacent_shreds(a, b):
+    aid, bid = a.component_id, b.component_id
+    ao, bo = a.orientation, b.orientation
+    if ao != bo:
+        return False
 
-        fastafile = "{0}.fasta".format(pf)
-        newfastafile = "{0}.new.fasta".format(pf)
-        format(
-            [
-                fastafile,
-                newfastafile,
-                "--sequential=replace",
-                "--sequentialoffset=1",
-                "--nodesc",
-            ]
-        )
-        fasta([newfastafile])
+    ai, af = get_shred_id(aid)
+    bi, bf = get_shred_id(bid)
+    if ai is None or bi is None:
+        return False
 
-        sh("rm -rf {0}".format(pf))
-        cmd = "runCA {0}.frg -p {0} -d {0} consensus=pbutgcns".format(pf)
-        cmd += " unitigger=bogart doFragmentCorrection=0 doUnitigSplitting=0"
-        sh(cmd)
-        outdir = "{0}/9-terminator".format(pf)
+    # Same sequence, with fragment id offset by one
+    return ai == bi and abs(af - bf) == 1
 
-        cmd = "cat {0}/{1}.ctg.fasta {0}/{1}.deg.fasta {0}/{1}.singleton.fasta".format(
-            outdir, pf
-        )
-        sh(cmd, outfile=contigs, append=True)
 
+def overlap_blastline_writer(oopts):
+    o = overlap(oopts)
+    if not o:
+        return ""
 
-def unitigs(args):
-    """
-    %prog unitigs best.edges
+    return str(o.blastline)
 
-    Reads Celera Assembler's "best.edges" and extract all unitigs.
-    """
-    p = OptionParser(unitigs.__doc__)
-    p.add_option("--maxerr", default=2, type="int", help="Maximum error rate")
-    opts, args = p.parse_args(args)
 
-    if len(args) != 1:
-        sys.exit(not p.print_help())
+def get_overlap_opts(aid, bid, qreverse, outdir, opts):
+    oopts = [
+        aid,
+        bid,
+        "--suffix",
+        "fa",
+        "--dir",
+        outdir,
+        "--pctid={0}".format(opts.pctid),
+        "--hitlen={0}".format(opts.hitlen),
+    ]
+    if qreverse:
+        oopts += ["--qreverse"]
+    return oopts
 
-    (bestedges,) = args
-    G = read_graph(bestedges, maxerr=opts.maxerr, directed=True)
-    H = nx.Graph()
-    intconv = lambda x: int(x.split("-")[0])
-    for k, v in G.iteritems():
-        if k == G.get(v, None):
-            H.add_edge(intconv(k), intconv(v))
-
-    nunitigs = nreads = 0
-    for h in nx.connected_component_subgraphs(H, copy=False):
-        st = [x for x in h if h.degree(x) == 1]
-        if len(st) != 2:
-            continue
-        src, target = st
-        path = list(nx.all_simple_paths(h, src, target))
-        assert len(path) == 1
-        (path,) = path
-        print("|".join(str(x) for x in path))
-        nunitigs += 1
-        nreads += len(path)
-    logging.debug(
-        "A total of {0} unitigs built from {1} reads.".format(nunitigs, nreads)
-    )
 
+def populate_blastfile(blastfile, agp, outdir, opts):
+    assert not op.exists(blastfile)
+    all_oopts = []
+    for a, b, qreverse in agp.iter_paired_components():
+        aid = a.component_id
+        bid = b.component_id
+        oopts = get_overlap_opts(aid, bid, qreverse, outdir, opts)
+        all_oopts.append(oopts)
 
-def graph(args):
-    """
-    %prog graph best.edges
+    pool = WriteJobs(overlap_blastline_writer, all_oopts, blastfile, cpus=opts.cpus)
+    pool.run()
 
-    Convert Celera Assembler's "best.edges" to a GEXF which can be used to
-    feed into Gephi to check the topology of the best overlapping graph. Mutual
-    best edges are represented as thicker edges.
 
-    Reference:
-    https://github.com/PacificBiosciences/Bioinformatics-Training/blob/master/scripts/CeleraToGephi.py
+def anneal(args):
     """
-    p = OptionParser(graph.__doc__)
-    p.add_option(
-        "--query",
-        default=-1,
-        type="int",
-        help="Search from node, -1 to select random node, 0 to disable",
-    )
-    p.add_option("--contig", help="Search from contigs, use comma to separate")
-    p.add_option(
-        "--largest", default=0, type="int", help="Only show largest components"
-    )
-    p.add_option("--maxsize", default=500, type="int", help="Max graph size")
-    p.add_option(
-        "--nomutualbest",
-        default=False,
-        action="store_true",
-        help="Do not plot mutual best edges as heavy",
-    )
-    add_graph_options(p)
-    opts, args = p.parse_args(args)
+    %prog anneal agpfile contigs.fasta
 
-    if len(args) != 1:
-        sys.exit(not p.print_help())
+    Merge adjacent overlapping contigs and make new AGP file.
 
-    (bestedges,) = args
-    query = opts.query
-    contig = opts.contig
-    largest = opts.largest
-    frgctg = opts.frgctg
-    edgeweight = not opts.nomutualbest
-    G = read_graph(bestedges, maxerr=opts.maxerr)
-
-    if largest:
-        H = list(nx.connected_component_subgraphs(G))
-        c = min(len(H), largest)
-        logging.debug("{0} components found, {1} retained".format(len(H), c))
-        G = nx.Graph()
-        for x in H[:c]:
-            G.add_edges_from(x.edges())
-
-    if query:
-        if query == -1:
-            query = choice(G.nodes())
-        reads_to_ctgs = parse_ctgs(frgctg)
-        if contig:
-            contigs = set(contig.split(","))
-            core = [k for k, v in reads_to_ctgs.items() if v in contigs]
-        else:
-            ctg = reads_to_ctgs.get(query)
-            core = [k for k, v in reads_to_ctgs.items() if v == ctg]
-            logging.debug(
-                "Reads ({0}) extended from the same contig {1}".format(len(core), ctg)
-            )
+    By default it will also anneal lines like these together (unless --nozipshreds):
+    scaffold4       1       1608    1       W       ca-bacs.5638.frag11.22000-23608 1       1608    -
+    scaffold4       1609    1771    2       N       163     scaffold        yes     paired-ends
+    scaffold4       1772    3771    3       W       ca-bacs.5638.frag10.20000-22000 1       2000    -
 
-        # Extract a local neighborhood
-        SG = nx.Graph()
-        H = graph_local_neighborhood(G, query=core, maxsize=opts.maxsize)
-        SG.add_edges_from(H.edges(data=edgeweight))
-        G = SG
-
-        seen = []
-        for n, attrib in G.nodes_iter(data=True):
-            contig = reads_to_ctgs.get(n, "na")
-            attrib["label"] = contig
-            seen.append(contig)
-        c = Counter(seen)
-        cc = ["{0}({1})".format(k, v) for k, v in c.most_common()]
-        print("Contigs: {0}".format(" ".join(cc)), file=sys.stderr)
-
-    gexf = "best"
-    if query >= 0:
-        gexf += ".{0}".format(query)
-    gexf += ".gexf"
-    nx.write_gexf(G, gexf)
-    logging.debug(
-        "Graph written to `{0}` (|V|={1}, |E|={2})".format(gexf, len(G), G.size())
-    )
-
-
-def astat(args):
+    These are most likely shreds, which we look for based on names.
     """
-    %prog astat coverage.log
-
-    Create coverage-rho scatter plot.
-    """
-    p = OptionParser(astat.__doc__)
-    p.add_option("--cutoff", default=1000, type="int", help="Length cutoff")
-    p.add_option("--genome", default="", help="Genome name")
+    p = OptionParser(anneal.__doc__)
+    p.set_align(pctid=GoodPct, hitlen=GoodOverlap)
     p.add_option(
-        "--arrDist",
-        default=False,
-        action="store_true",
-        help="Use arrDist instead",
+        "--hang", default=GoodOverhang, type="int", help="Maximum overhang length"
     )
+    p.set_outdir(outdir="outdir")
+    p.set_cpus()
     opts, args = p.parse_args(args)
 
-    if len(args) != 1:
+    if len(args) != 2:
         sys.exit(not p.print_help())
 
-    (covfile,) = args
-    cutoff = opts.cutoff
-    genome = opts.genome
-    plot_arrDist = opts.arrDist
-
-    suffix = ".{0}".format(cutoff)
-    small_covfile = covfile + suffix
-    update_covfile = need_update(covfile, small_covfile)
-    if update_covfile:
-        fw = open(small_covfile, "w")
-    else:
-        logging.debug("Found `{0}`, will use this one".format(small_covfile))
-        covfile = small_covfile
-
-    fp = open(covfile)
-    header = next(fp)
-    if update_covfile:
-        fw.write(header)
-
-    data = []
-    msg = "{0} tigs scanned ..."
-    for row in fp:
-        tigID, rho, covStat, arrDist = row.split()
-        tigID = int(tigID)
-        if tigID % 1000000 == 0:
-            sys.stderr.write(msg.format(tigID) + "\r")
-
-        rho, covStat, arrDist = [float(x) for x in (rho, covStat, arrDist)]
-        if rho < cutoff:
-            continue
+    agpfile, contigs = args
+    outdir = opts.outdir
+    if not op.exists(outdir):
+        mkdir(outdir)
+        cmd = "faSplit byname {0} {1}/".format(contigs, outdir)
+        sh(cmd)
 
-        if update_covfile:
-            fw.write(row)
-        data.append((tigID, rho, covStat, arrDist))
+    cutoff = Cutoff(opts.pctid, opts.hitlen, opts.hang)
+    logging.debug(str(cutoff))
 
-    print(msg.format(tigID), file=sys.stderr)
+    agp = AGP(agpfile)
+    blastfile = agpfile.replace(".agp", ".blast")
+    if not op.exists(blastfile):
+        populate_blastfile(blastfile, agp, outdir, opts)
+
+    assert op.exists(blastfile)
+    logging.debug("File `{0}` found. Start loading.".format(blastfile))
+    blast = BlastSlow(blastfile).to_dict()
+
+    annealedagp = "annealed.agp"
+    annealedfasta = "annealed.fasta"
+
+    newagp = deepcopy(agp)
+    clrstore = {}
+    for a, b, qreverse in agp.iter_paired_components():
+        aid = a.component_id
+        bid = b.component_id
+
+        pair = (aid, bid)
+        if pair in blast:
+            bl = blast[pair]
+        else:
+            oopts = get_overlap_opts(aid, bid, qreverse, outdir, opts)
+            o = overlap(oopts)
+            if not o:
+                continue
+            bl = o.blastline
 
-    from jcvi.graphics.base import plt, savefig
+        o = Overlap(bl, a.component_span, b.component_span, cutoff, qreverse=qreverse)
 
-    logging.debug("Plotting {0} data points.".format(len(data)))
-    tigID, rho, covStat, arrDist = zip(*data)
+        if aid not in clrstore:
+            clrstore[aid] = CLR.from_agpline(a)
+        if bid not in clrstore:
+            clrstore[bid] = CLR.from_agpline(b)
 
-    y = arrDist if plot_arrDist else covStat
-    ytag = "arrDist" if plot_arrDist else "covStat"
+        aclr, bclr = clrstore[aid], clrstore[bid]
 
-    fig = plt.figure(1, (7, 7))
-    ax = fig.add_axes([0.12, 0.1, 0.8, 0.8])
-    ax.plot(rho, y, ".", color="lightslategrey")
+        o.print_graphic()
+        if o.anneal(aclr, bclr):
+            newagp.delete_between(aid, bid, verbose=True)
 
-    xtag = "rho"
-    info = (genome, xtag, ytag)
-    title = "{0} {1} vs. {2}".format(*info)
-    ax.set_title(title)
-    ax.set_xlabel(xtag)
-    ax.set_ylabel(ytag)
+        if o.otype == 2:  # b ~ a
+            o = o.swapped
+            o.print_graphic()
+            if o.anneal(bclr, aclr):
+                newagp.switch_between(bid, aid, verbose=True)
+                newagp.delete_between(bid, aid, verbose=True)
 
-    if plot_arrDist:
-        ax.set_yscale("log")
+    logging.debug("A total of {0} components with modified CLR.".format(len(clrstore)))
 
-    imagename = "{0}.png".format(".".join(info))
-    savefig(imagename, dpi=150)
+    for cid, c in clrstore.items():
+        if c.is_valid:
+            continue
+        print("Remove {0}".format(c), file=sys.stderr)
+        newagp.convert_to_gap(cid, verbose=True)
 
+    # Update all ranges that has modified clr
+    for a in newagp:
+        if a.is_gap:
+            continue
+        aid = a.component_id
+        if aid in clrstore:
+            c = clrstore[aid]
+            a.component_beg = c.start
+            a.component_end = c.end
 
-def emitFragment(fw, fragID, libID, shredded_seq, clr=None, qvchar="l", fasta=False):
-    """
-    Print out the shredded sequence.
-    """
-    if fasta:
-        s = SeqRecord(shredded_seq, id=fragID, description="")
-        SeqIO.write([s], fw, "fasta")
-        return
+    newagp.print_to_file(annealedagp)
+    tidyagp = tidy([annealedagp, contigs])
 
-    seq = str(shredded_seq)
-    slen = len(seq)
-    qvs = qvchar * slen  # shredded reads have default low qv
-
-    if clr is None:
-        clr_beg, clr_end = 0, slen
-    else:
-        clr_beg, clr_end = clr
-
-    print(
-        frgTemplate.format(
-            fragID=fragID,
-            libID=libID,
-            seq=seq,
-            qvs=qvs,
-            clr_beg=clr_beg,
-            clr_end=clr_end,
-        ),
-        file=fw,
-    )
+    build([tidyagp, contigs, annealedfasta])
+    return annealedfasta
 
 
-def shred(args):
+def blast(args):
     """
-    %prog shred fastafile
+    %prog blast allfasta clonename
 
-    Similar to the method of `shredContig` in runCA script. The contigs are
-    shredded into pseudo-reads with certain length and depth.
+    Insert a component into agpfile by aligning to the best hit in pool and see
+    if they have good overlaps.
     """
-    p = OptionParser(shred.__doc__)
-    p.set_depth(depth=2)
-    p.add_option(
-        "--readlen",
-        default=1000,
-        type="int",
-        help="Desired length of the reads",
-    )
-    p.add_option(
-        "--minctglen",
-        default=0,
-        type="int",
-        help="Ignore contig sequence less than",
-    )
-    p.add_option(
-        "--shift",
-        default=50,
-        type="int",
-        help="Overlap between reads must be at least",
-    )
-    p.add_option(
-        "--fasta",
-        default=False,
-        action="store_true",
-        help="Output shredded reads as FASTA sequences",
-    )
+    from jcvi.apps.align import run_megablast
+
+    p = OptionParser(blast.__doc__)
+    p.add_option("-n", type="int", default=2, help="Take best N hits")
     opts, args = p.parse_args(args)
 
-    if len(args) != 1:
+    if len(args) != 2:
         sys.exit(not p.print_help())
 
-    (fastafile,) = args
-    libID = fastafile.split(".")[0]
-    depth = opts.depth
-    readlen = opts.readlen
-    shift = opts.shift
-
-    outfile = libID + ".depth{0}".format(depth)
-    if opts.fasta:
-        outfile += ".fasta"
-    else:
-        outfile += ".frg"
-    f = Fasta(fastafile, lazy=True)
+    allfasta, clonename = args
+    fastadir = "fasta"
+    infile = op.join(fastadir, clonename + ".fasta")
+    if not op.exists(infile):
+        entrez([clonename, "--skipcheck", "--outdir=" + fastadir])
+
+    outfile = "{0}.{1}.blast".format(clonename, allfasta.split(".")[0])
+    run_megablast(
+        infile=infile, outfile=outfile, db=allfasta, pctid=GoodPct, hitlen=GoodOverlap
+    )
+
+    blasts = [BlastLine(x) for x in open(outfile)]
+    besthits = []
+    for b in blasts:
+        if b.query.count("|") >= 3:
+            b.query = b.query.split("|")[3]
+
+        if b.subject.count("|") >= 3:
+            b.subject = b.subject.split("|")[3]
 
-    fw = must_open(outfile, "w", checkexists=True)
-    if not opts.fasta:
-        print(headerTemplate.format(libID=libID), file=fw)
-
-    """
-    Taken from runCA:
-
-                    |*********|
-                    |###################|
-    |--------------------------------------------------|
-     ---------------1---------------
-               ---------------2---------------
-                         ---------------3---------------
-    *** - center_increments
-    ### - center_range_width
-    """
-    for ctgID, (name, rec) in enumerate(f.iteritems_ordered()):
-        seq = rec.seq
-        seqlen = len(seq)
-        if seqlen < opts.minctglen:
+        b.query = b.query.rsplit(".", 1)[0]
+        b.subject = b.subject.rsplit(".", 1)[0]
+
+        if b.query == b.subject:
             continue
 
-        shredlen = min(seqlen - shift, readlen)
-        numreads = max(seqlen * depth / shredlen, 1)
-        center_range_width = seqlen - shredlen
-
-        ranges = []
-        if depth == 1:
-            if seqlen < readlen:
-                ranges.append((0, seqlen))
-            else:
-                for begin in range(0, seqlen, readlen - shift):
-                    end = min(seqlen, begin + readlen)
-                    ranges.append((begin, end))
-        else:
-            if numreads == 1:
-                ranges.append((0, shredlen))
-            else:
-                prev_begin = -1
-                center_increments = center_range_width * 1.0 / (numreads - 1)
-                for i in range(numreads):
-                    begin = center_increments * i
-                    end = begin + shredlen
-                    begin, end = int(begin), int(end)
-
-                    if begin == prev_begin:
-                        continue
-
-                    ranges.append((begin, end))
-                    prev_begin = begin
-
-        for shredID, (begin, end) in enumerate(ranges):
-            shredded_seq = seq[begin:end]
-            fragID = "{0}.{1}.frag{2}.{3}-{4}".format(libID, ctgID, shredID, begin, end)
-            emitFragment(fw, fragID, libID, shredded_seq, fasta=opts.fasta)
+        if b.subject not in besthits:
+            besthits.append(b.subject)
+        if len(besthits) == opts.n:
+            break
 
-    fw.close()
-    logging.debug("Shredded reads are written to `{0}`.".format(outfile))
-    return outfile
+    for b in besthits:
+        overlap([clonename, b, "--dir=" + fastadir])
 
 
-def tracedb(args):
+def bes(args):
     """
-    %prog tracedb <xml|lib|frg>
+    %prog bes bacfasta clonename
 
-    Run `tracedb-to-frg.pl` within current folder.
+    Use the clone name to download BES gss sequences from Genbank, map and then
+    visualize.
     """
-    p = OptionParser(tracedb.__doc__)
+    from jcvi.apps.align import run_blat
 
+    p = OptionParser(bes.__doc__)
+    p.set_cpus()
     opts, args = p.parse_args(args)
 
-    if len(args) != 1:
-        sys.exit(p.print_help())
-
-    (action,) = args
-    assert action in ("xml", "lib", "frg")
-
-    CMD = "tracedb-to-frg.pl"
-    xmls = glob("xml*")
+    if len(args) != 2:
+        sys.exit(not p.print_help())
 
-    if action == "xml":
-        for xml in xmls:
-            cmd = CMD + " -xml {0}".format(xml)
-            sh(cmd, outfile="/dev/null", errfile="/dev/null", background=True)
+    bacfasta, clonename = args
 
-    elif action == "lib":
-        cmd = CMD + " -lib {0}".format(" ".join(xmls))
-        sh(cmd)
+    entrez([clonename, "--database=nucgss", "--skipcheck"])
+    besfasta = clonename + ".fasta"
+    blatfile = clonename + ".bes.blat"
+    run_blat(
+        infile=besfasta,
+        outfile=blatfile,
+        db=bacfasta,
+        pctid=95,
+        hitlen=100,
+        cpus=opts.cpus,
+    )
+
+    aid, asize = next(Fasta(bacfasta).itersizes())
+
+    width = 50
+    msg = "=" * width
+    msg += "  " + aid
+    print(msg, file=sys.stderr)
+
+    ratio = width * 1.0 / asize
+    _ = lambda x: int(round(x * ratio, 0))
+    blasts = [BlastLine(x) for x in open(blatfile)]
+    for b in blasts:
+        if b.orientation == "+":
+            msg = " " * _(b.sstart) + "->"
+        else:
+            msg = " " * (_(b.sstop) - 2) + "<-"
+        msg += " " * (width - len(msg) + 2)
+        msg += b.query
+        if b.orientation == "+":
+            msg += " (hang={0})".format(b.sstart - 1)
+        else:
+            msg += " (hang={0})".format(asize - b.sstop)
 
-    elif action == "frg":
-        for xml in xmls:
-            cmd = CMD + " -frg {0}".format(xml)
-            sh(cmd, background=True)
+        print(msg, file=sys.stderr)
 
 
-def make_matepairs(fastafile):
+def flip(args):
     """
-    Assumes the mates are adjacent sequence records
+    %prog flip fastafile
+
+    Go through each FASTA record, check against Genbank file and determines
+    whether or not to flip the sequence. This is useful before updates of the
+    sequences to make sure the same orientation is used.
     """
-    assert op.exists(fastafile)
+    p = OptionParser(flip.__doc__)
+    opts, args = p.parse_args(args)
 
-    matefile = fastafile.rsplit(".", 1)[0] + ".mates"
-    if op.exists(matefile):
-        logging.debug("matepairs file `{0}` found".format(matefile))
-    else:
-        logging.debug("parsing matepairs from `{0}`".format(fastafile))
-        matefw = open(matefile, "w")
-        it = SeqIO.parse(fastafile, "fasta")
-        for fwd, rev in zip(it, it):
-            print("{0}\t{1}".format(fwd.id, rev.id), file=matefw)
+    if len(args) != 1:
+        sys.exit(not p.print_help())
 
-        matefw.close()
+    (fastafile,) = args
+    outfastafile = fastafile.rsplit(".", 1)[0] + ".flipped.fasta"
+    fo = open(outfastafile, "w")
+    f = Fasta(fastafile, lazy=True)
+    for name, rec in f.iteritems_ordered():
+        tmpfasta = "a.fasta"
+        fw = open(tmpfasta, "w")
+        SeqIO.write([rec], fw, "fasta")
+        fw.close()
+
+        o = overlap([tmpfasta, name])
+        if o.orientation == "-":
+            rec.seq = rec.seq.reverse_complement()
 
-    return matefile
+        SeqIO.write([rec], fo, "fasta")
+        cleanup(tmpfasta)
 
 
-get_mean_sv = lambda size: (size, size / 5)
+def batchoverlap(args):
+    """
+    %prog batchoverlap pairs.txt outdir
 
+    Check overlaps between pairs of sequences.
+    """
+    p = OptionParser(batchoverlap.__doc__)
+    p.set_cpus()
+    opts, args = p.parse_args(args)
 
-def split_fastafile(fastafile, maxreadlen=32000):
-    pf = fastafile.split(".")[0]
-    smallfastafile = pf + "-small.fasta"
-    bigfastafile = pf + "-big.fasta"
-    shredfastafile = pf + "-big.depth1.fasta"
+    if len(args) != 2:
+        sys.exit(not p.print_help())
 
-    if need_update(fastafile, (smallfastafile, shredfastafile)):
-        filter([fastafile, str(maxreadlen), "--less", "-o", smallfastafile])
-        filter([fastafile, str(maxreadlen), "-o", bigfastafile])
-        shred(
-            [
-                "--depth=1",
-                "--shift={0}".format(maxreadlen / 100),
-                "--readlen={0}".format(maxreadlen),
-                "--fasta",
-                bigfastafile,
-            ]
-        )
+    pairsfile, outdir = args
+    fp = open(pairsfile)
+    cmds = []
+    mkdir("overlaps")
+    for row in fp:
+        a, b = row.split()[:2]
+        oa = op.join(outdir, a + ".fa")
+        ob = op.join(outdir, b + ".fa")
+        cmd = "python -m jcvi.assembly.goldenpath overlap {0} {1}".format(oa, ob)
+        cmd += " -o overlaps/{0}_{1}.ov".format(a, b)
+        cmds.append(cmd)
 
-    return smallfastafile, shredfastafile
+    print("\n".join(cmds))
 
 
-def fasta(args):
+def overlap(args):
     """
-    %prog fasta fastafile
+    %prog overlap <a|a.fasta> <b|b.fasta>
 
-    Convert reads formatted as FASTA file, and convert to CA frg file. If .qual
-    file is found, then use it, otherwise just make a fake qual file. Mates are
-    assumed as adjacent sequence records (i.e. /1, /2, /1, /2 ...) unless a
-    matefile is given.
+    Check overlaps between two fasta records. The arguments can be genBank IDs
+    instead of FASTA files. In case of IDs, the sequences will be downloaded
+    first.
     """
-    from jcvi.formats.fasta import clean, make_qual
+    from jcvi.formats.blast import chain_HSPs
 
-    p = OptionParser(fasta.__doc__)
+    p = OptionParser(overlap.__doc__)
     p.add_option(
-        "--clean",
-        default=False,
-        action="store_true",
-        help="Clean up irregular chars in seq",
+        "--dir",
+        default=os.getcwd(),
+        help="Download sequences to dir",
     )
-    p.add_option("--matefile", help="Matepairs file")
     p.add_option(
-        "--maxreadlen", default=262143, type="int", help="Maximum read length allowed"
+        "--suffix",
+        default="fasta",
+        help="Suffix of the sequence file in dir",
     )
     p.add_option(
-        "--minreadlen", default=1000, type="int", help="Minimum read length allowed"
+        "--qreverse",
+        default=False,
+        action="store_true",
+        help="Reverse seq a",
     )
     p.add_option(
-        "--sequential",
+        "--nochain",
         default=False,
         action="store_true",
-        help="Overwrite read name (e.g. long Pacbio name)",
+        help="Do not chain adjacent HSPs",
     )
-    p.set_size()
+    p.set_align(pctid=GoodPct, hitlen=GoodOverlap, evalue=0.01)
+    p.set_outfile(outfile=None)
     opts, args = p.parse_args(args)
 
-    if len(args) != 1:
+    if len(args) != 2:
         sys.exit(not p.print_help())
 
-    (fastafile,) = args
-    maxreadlen = opts.maxreadlen
-    minreadlen = opts.minreadlen
-    if maxreadlen > 0:
-        split = False
-        f = Fasta(fastafile, lazy=True)
-        for id, size in f.itersizes_ordered():
-            if size > maxreadlen:
-                logging.debug(
-                    "Sequence {0} (size={1}) longer than max read len {2}".format(
-                        id, size, maxreadlen
-                    )
-                )
-                split = True
-                break
-
-        if split:
-            for f in split_fastafile(fastafile, maxreadlen=maxreadlen):
-                fasta([f, "--maxreadlen=0"])
-            return
+    afasta, bfasta = args
+    dir = opts.dir
+    chain = not opts.nochain
+    suffix = opts.suffix
+    evalue = opts.evalue
+    pctid = opts.pctid
+    hitlen = opts.hitlen
+    cutoff = Cutoff(pctid, hitlen)
+
+    # Check first whether it is file or accession name
+    if not op.exists(afasta):
+        af = op.join(dir, ".".join((afasta, suffix)))
+        if not op.exists(af):  # Check to avoid redownload
+            entrez([afasta, "--skipcheck", "--outdir=" + dir])
+        afasta = af
+
+    if not op.exists(bfasta):
+        bf = op.join(dir, ".".join((bfasta, suffix)))
+        if not op.exists(bf):
+            entrez([bfasta, "--skipcheck", "--outdir=" + dir])
+        bfasta = bf
+
+    assert op.exists(afasta) and op.exists(bfasta)
+
+    cmd = "blastn -dust no"
+    cmd += " -query {0} -subject {1}".format(afasta, bfasta)
+    cmd += " -evalue {0} -outfmt 6 -perc_identity {1}".format(evalue, pctid)
 
-    plate = op.basename(fastafile).split(".")[0]
+    fp = popen(cmd)
+    hsps = fp.readlines()
 
-    mated = opts.size != 0
-    mean, sv = get_mean_sv(opts.size)
+    hsps = [BlastLine(x) for x in hsps]
+    hsps = [x for x in hsps if x.hitlen >= hitlen]
+    if chain:
+        logging.debug("Chain HSPs in the Blast output.")
+        dist = 2 * hitlen  # Distance to chain the HSPs
+        hsps = chain_HSPs(hsps, xdist=dist, ydist=dist)
+
+    if len(hsps) == 0:
+        print("No match found.", file=sys.stderr)
+        return None
+
+    besthsp = hsps[0]
+
+    aid, asize = next(Fasta(afasta).itersizes())
+    bid, bsize = next(Fasta(bfasta).itersizes())
+    o = Overlap(besthsp, asize, bsize, cutoff, qreverse=opts.qreverse)
+    o.print_graphic()
+
+    if opts.outfile:
+        fw = must_open(opts.outfile, "w")
+        print(str(o), file=fw)
+        fw.close()
 
-    if mated:
-        libname = "Sanger{0}Kb-".format(opts.size / 1000) + plate
-    else:
-        libname = plate
-
-    frgfile = libname + ".frg"
-
-    if opts.clean:
-        cleanfasta = fastafile.rsplit(".", 1)[0] + ".clean.fasta"
-        if need_update(fastafile, cleanfasta):
-            clean([fastafile, "--canonical", "-o", cleanfasta])
-        fastafile = cleanfasta
-
-    if mated:
-        qualfile = make_qual(fastafile, score=21)
-        if opts.matefile:
-            matefile = opts.matefile
-            assert op.exists(matefile)
-        else:
-            matefile = make_matepairs(fastafile)
+    return o
 
-        cmd = "convert-fasta-to-v2.pl"
-        cmd += " -l {0} -s {1} -q {2} ".format(libname, fastafile, qualfile)
-        if mated:
-            cmd += "-mean {0} -stddev {1} -m {2} ".format(mean, sv, matefile)
 
-        sh(cmd, outfile=frgfile)
-        return
+@lru_cache(maxsize=None)
+def phase(accession):
+    gbdir = "gb"
+    gbfile = op.join(gbdir, accession + ".gb")
+    if not op.exists(gbfile):
+        entrez([accession, "--skipcheck", "--outdir=" + gbdir, "--format=gb"])
+    rec = next(SeqIO.parse(gbfile, "gb"))
+    ph, keywords = get_phase(rec)
+    return ph, len(rec)
+
+
+def check_certificate(certificatefile):
+    data = {}
+    if op.exists(certificatefile):
+        # This will make updates resume-able and backed-up
+        certificatefilebak = certificatefile + ".orig"
+        shutil.copy2(certificatefile, certificatefilebak)
 
-    fw = must_open(frgfile, "w")
-    print(headerTemplate.format(libID=libname), file=fw)
+        fp = open(certificatefile)
+        for row in fp:
+            atoms = row.split()
+            tag, aid, bid = atoms[0], atoms[4], atoms[5]
+            data[(tag, aid, bid)] = row.strip()
 
-    sequential = opts.sequential
-    i = j = 0
-    for fragID, seq in parse_fasta(fastafile):
-        if len(seq) < minreadlen:
-            j += 1
-            continue
-        i += 1
-        if sequential:
-            fragID = libname + str(100000000 + i)
-        emitFragment(fw, fragID, libname, seq)
-    fw.close()
+    return data
 
-    logging.debug(
-        "A total of {0} fragments written to `{1}` ({2} discarded).".format(
-            i, frgfile, j
-        )
-    )
 
-
-def sff(args):
+def certificate(args):
     """
-    %prog sff sffiles
+    %prog certificate tpffile certificatefile
+
+    Generate certificate file for all overlaps in tpffile. tpffile can be
+    generated by jcvi.formats.agp.tpf().
 
-    Convert reads formatted as 454 SFF file, and convert to CA frg file.
-    Turn --nodedup on if another deduplication mechanism is used (e.g.
-    CD-HIT-454). See assembly.sff.deduplicate().
+    North chr1 2 0 AC229737.8 telomere 58443
+    South chr1 2 1 AC229737.8 AC202463.29 58443 37835 58443 + Non-terminal
+
+    Each line describes a relationship between the current BAC and the
+    north/south BAC. First, "North/South" tag, then the chromosome, phases of
+    the two BACs, ids of the two BACs, the size and the overlap start-stop of
+    the CURRENT BAC, and orientation. Each BAC will have two lines in the
+    certificate file.
     """
-    p = OptionParser(sff.__doc__)
-    p.add_option(
-        "--prefix", dest="prefix", default=None, help="Output frg filename prefix"
-    )
-    p.add_option(
-        "--nodedup",
-        default=False,
-        action="store_true",
-        help="Do not remove duplicates",
-    )
-    p.set_size()
+    p = OptionParser(certificate.__doc__)
     opts, args = p.parse_args(args)
 
-    if len(args) < 1:
-        sys.exit(p.print_help())
+    if len(args) != 2:
+        sys.exit(not p.print_help())
 
-    sffiles = args
-    plates = [x.split(".")[0].split("_")[-1] for x in sffiles]
+    tpffile, certificatefile = args
+    fastadir = "fasta"
 
-    mated = opts.size != 0
-    mean, sv = get_mean_sv(opts.size)
+    tpf = TPF(tpffile)
 
-    if len(plates) > 1:
-        plate = plates[0][:-1] + "X"
-    else:
-        plate = "_".join(plates)
-
-    if mated:
-        libname = "Titan{0}Kb-".format(opts.size / 1000) + plate
-    else:
-        libname = "TitanFrags-" + plate
-
-    if opts.prefix:
-        libname = opts.prefix
-
-    cmd = "sffToCA"
-    cmd += " -libraryname {0} -output {0} ".format(libname)
-    cmd += " -clear 454 -trim chop "
-    if mated:
-        cmd += " -linker titanium -insertsize {0} {1} ".format(mean, sv)
-    if opts.nodedup:
-        cmd += " -nodedup "
+    data = check_certificate(certificatefile)
+    fw = must_open(certificatefile, "w")
+    for i, a in enumerate(tpf):
+        if a.is_gap:
+            continue
 
-    cmd += " ".join(sffiles)
+        aid = a.component_id
 
-    sh(cmd)
+        af = op.join(fastadir, aid + ".fasta")
+        if not op.exists(af):  # Check to avoid redownload
+            entrez([aid, "--skipcheck", "--outdir=" + fastadir])
+
+        north, south = tpf.getNorthSouthClone(i)
+        aphase, asize = phase(aid)
+
+        for tag, p in (("North", north), ("South", south)):
+            if not p:  # end of the chromosome
+                ov = "telomere\t{0}".format(asize)
+            elif p.isCloneGap:
+                bphase = "0"
+                ov = "{0}\t{1}".format(p.gap_type, asize)
+            else:
+                bid = p.component_id
+                bphase, bsize = phase(bid)
+                key = (tag, aid, bid)
+                if key in data:
+                    print(data[key], file=fw)
+                    continue
+
+                ar = [aid, bid, "--dir=" + fastadir]
+                o = overlap(ar)
+                ov = o.certificateline if o else "{0}\t{1}\tNone".format(bid, asize)
+
+            print(
+                "\t".join(str(x) for x in (tag, a.object, aphase, bphase, aid, ov)),
+                file=fw,
+            )
+            fw.flush()
 
 
-def fastq(args):
+def neighbor(args):
     """
-    %prog fastq fastqfile
+    %prog neighbor agpfile componentID
 
-    Convert reads formatted as FASTQ file, and convert to CA frg file.
+    Check overlaps of a particular component in agpfile.
     """
-    from jcvi.formats.fastq import guessoffset
-
-    p = OptionParser(fastq.__doc__)
-    p.add_option(
-        "--outtie",
-        dest="outtie",
-        default=False,
-        action="store_true",
-        help="Are these outie reads?",
-    )
-    p.set_phred()
-    p.set_size()
-
+    p = OptionParser(neighbor.__doc__)
     opts, args = p.parse_args(args)
 
-    if len(args) < 1:
-        sys.exit(p.print_help())
+    if len(args) != 2:
+        sys.exit(not p.print_help())
 
-    fastqfiles = [get_abs_path(x) for x in args]
-    size = opts.size
-    outtie = opts.outtie
-    if size > 1000 and (not outtie):
-        logging.debug("[warn] long insert size {0} but not outtie".format(size))
+    agpfile, componentID = args
+    fastadir = "fasta"
 
-    mated = size != 0
-    libname = op.basename(args[0]).split(".")[0]
-    libname = libname.replace("_1_sequence", "")
+    cmd = "grep"
+    cmd += " --color -C2 {0} {1}".format(componentID, agpfile)
+    sh(cmd)
 
-    frgfile = libname + ".frg"
-    mean, sv = get_mean_sv(opts.size)
+    agp = AGP(agpfile)
+    aorder = agp.order
+    if componentID not in aorder:
+        print(
+            "Record {0} not present in `{1}`.".format(componentID, agpfile),
+            file=sys.stderr,
+        )
+        return
 
-    cmd = "fastqToCA"
-    cmd += " -libraryname {0} ".format(libname)
-    fastqs = " ".join("-reads {0}".format(x) for x in fastqfiles)
-    if mated:
-        assert len(args) in (1, 2), "you need one or two fastq files for mated library"
-        fastqs = "-mates {0}".format(",".join(fastqfiles))
-        cmd += "-insertsize {0} {1} ".format(mean, sv)
-    cmd += fastqs
+    i, c = aorder[componentID]
+    north, south = agp.getNorthSouthClone(i)
 
-    offset = int(opts.phred) if opts.phred else guessoffset([fastqfiles[0]])
-    illumina = offset == 64
-    if illumina:
-        cmd += " -type illumina"
-    if outtie:
-        cmd += " -outtie"
+    if not north.isCloneGap:
+        ar = [north.component_id, componentID, "--dir=" + fastadir]
+        if north.orientation == "-":
+            ar += ["--qreverse"]
+        overlap(ar)
 
-    sh(cmd, outfile=frgfile)
+    if not south.isCloneGap:
+        ar = [componentID, south.component_id, "--dir=" + fastadir]
+        if c.orientation == "-":
+            ar += ["--qreverse"]
+        overlap(ar)
 
 
-def clr(args):
+def agp(args):
     """
-    %prog blastfile fastafiles
+    %prog agp tpffile certificatefile agpfile
 
-    Calculate the vector clear range file based BLAST to the vectors.
-    """
-    p = OptionParser(clr.__doc__)
-    opts, args = p.parse_args(args)
+    Build agpfile from overlap certificates.
 
-    if len(args) < 2:
-        sys.exit(not p.print_help())
+    Tiling Path File (tpf) is a file that lists the component and the gaps.
+    It is a three-column file similar to below, also see jcvi.formats.agp.tpf():
 
-    blastfile = args[0]
-    fastafiles = args[1:]
+    telomere    chr1 na
+    AC229737.8  chr1 +
+    AC202463.29 chr1 +
 
-    sizes = {}
-    for fa in fastafiles:
-        f = Fasta(fa)
-        sizes.update(f.itersizes())
-
-    b = Blast(blastfile)
-    for query, hits in b.iter_hits():
-
-        qsize = sizes[query]
-        vectors = list((x.qstart, x.qstop) for x in hits)
-        vmin, vmax = range_minmax(vectors)
+    Note: the orientation of the component is only used as a guide. If the
+    orientation is derivable from a terminal overlap, it will use it regardless
+    of what the tpf says.
 
-        left_size = vmin - 1
-        right_size = qsize - vmax
+    See jcvi.assembly.goldenpath.certificate() which generates a list of
+    certificates based on agpfile. At first, it seems counter-productive to
+    convert first agp to certificates then certificates back to agp.
 
-        if left_size > right_size:
-            clr_start, clr_end = 0, vmin
-        else:
-            clr_start, clr_end = vmax, qsize
+    The certificates provide a way to edit the overlap information, so that the
+    agpfile can be corrected (without changing agpfile directly).
+    """
+    from jcvi.formats.base import DictFile
 
-        print("\t".join(str(x) for x in (query, clr_start, clr_end)))
-        del sizes[query]
+    p = OptionParser(agp.__doc__)
+    opts, args = p.parse_args(args)
+
+    if len(args) != 3:
+        sys.exit(not p.print_help())
 
-    for q, size in sorted(sizes.items()):
-        print("\t".join(str(x) for x in (q, 0, size)))
+    tpffile, certificatefile, agpfile = args
+    orientationguide = DictFile(tpffile, valuepos=2)
+    cert = Certificate(certificatefile)
+    cert.write_AGP(agpfile, orientationguide=orientationguide)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.5/jcvi/assembly/chic.pyx` & `jcvi-1.4.6/jcvi/assembly/chic.pyx`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/assembly/coverage.py` & `jcvi-1.4.6/jcvi/assembly/coverage.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/assembly/gaps.py` & `jcvi-1.4.6/jcvi/assembly/gaps.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/assembly/geneticmap.py` & `jcvi-1.4.6/jcvi/assembly/geneticmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/assembly/goldenpath.py` & `jcvi-1.4.6/jcvi/graphics/landscape.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,1192 +1,1221 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
-Procedures to validate and update golden path of a genome assembly. This relies
-heavily on formats.agp, and further includes several algorithms, e.g. overlap
-detection.
+Create chromosome landscape plots that are similar to the ones used in soybean
+and sorghum paper.
 """
-import os
-import os.path as op
-import sys
-import shutil
-import logging
-
-from copy import deepcopy
-from functools import lru_cache
-from itertools import groupby
-
-from jcvi.formats.agp import AGP, TPF, get_phase, reindex, tidy, build
-from jcvi.formats.base import BaseFile, must_open
-from jcvi.formats.fasta import Fasta, SeqIO
-from jcvi.formats.blast import BlastSlow, BlastLine
-from jcvi.formats.coords import Overlap_types
-from jcvi.apps.fetch import entrez
-from jcvi.apps.grid import WriteJobs
-from jcvi.apps.base import (
-    OptionParser,
-    ActionDispatcher,
-    cleanup,
-    popen,
-    mkdir,
-    sh,
-    need_update,
-)
-
 
-GoodPct = 98
-GoodOverlap = 200
-GoodOverhang = 2000
 
+import os.path as op
+import sys
 
-class Cutoff(object):
-    def __init__(self, pctid=GoodPct, overlap=GoodOverlap, hang=GoodOverhang):
-        self.pctid = pctid
-        self.overlap = overlap
-        self.hang = hang
+from collections import Counter, OrderedDict, defaultdict
+from typing import List, Optional
 
-    def __str__(self):
-        return "Configuration: PCTID={} OVERLAP={} HANG={}".format(
-            self.pctid, self.overlap, self.hang
-        )
+import numpy as np
 
+from ..algorithms.matrix import moving_sum
+from ..apps.base import ActionDispatcher, OptionParser, logger
+from ..formats.base import BaseFile, DictFile, LineFile, must_open
+from ..formats.bed import Bed, bins, get_nbins
+from ..formats.sizes import Sizes
+from ..utils.cbook import autoscale, human_size
+
+from .base import (
+    CirclePolygon,
+    Colormap,
+    Extent,
+    Rectangle,
+    adjust_extent,
+    adjust_spines,
+    human_readable_base,
+    latex,
+    markup,
+    normalize_axes,
+    plt,
+    savefig,
+    set_human_axis,
+    ticker,
+)
+from .chromosome import HorizontalChromosome
 
-class CLR(object):
-    def __init__(self, id, size, orientation="+"):
-        self.id = id
-        self.start = 1
-        self.end = size
-        if orientation == "?":
-            orientation = "+"
-        assert orientation in ("+", "-")
-        self.orientation = orientation
+# Colors picked from Schmutz soybean genome paper using ColorPic
+palette = ["#ACABD5", "#DBF0F5", "#3EA77A", "#FBF5AB", "#C162A6"] + list("rgbymck")
+gray = "#CCCCCB"
+Registration = {
+    "Gypsy": "LTR-RT/Gypsy",
+    "Copia": "LTR-RT/Copia",
+    "hAT": "DNA-TE/hAT",
+    "Helitron": "DNA-TE/Helitron",
+    "Tourist": "DNA-TE/Tourist",
+    "Introns": "Genes (introns)",
+    "Exons": "Genes (exons)",
+}
+
+
+class BinLine:
+    def __init__(self, row):
+        args = row.split()
+        self.chr = args[0]
+        self.len = float(args[1])
+        self.binlen = int(args[2])
 
     def __str__(self):
-        return "{}: {}-{}({})".format(self.id, self.start, self.end, self.orientation)
+        return "\t".join(str(x) for x in (self.chr, self.len, self.binlen))
 
-    @property
-    def is_valid(self):
-        return self.start < self.end
-
-    @classmethod
-    def from_agpline(cls, a):
-        c = CLR(a.component_id, 0, a.orientation)
-        c.start = a.component_beg
-        c.end = a.component_end
-        return c
-
-
-class Overlap(object):
-    def __init__(self, blastline, asize, bsize, cutoff, qreverse=False):
-
-        b = blastline
-        aid = b.query
-        bid = b.subject
-
-        self.aid = aid.split("|")[3] if aid.count("|") >= 3 else aid
-        self.bid = bid.split("|")[3] if bid.count("|") >= 3 else bid
-        self.asize = asize
-        self.bsize = bsize
-
-        self.qstart = b.qstart
-        self.qstop = b.qstop
-        self.sstart = b.sstart
-        self.sstop = b.sstop
-
-        self.pctid = b.pctid
-        self.hitlen = b.hitlen
-        self.orientation = b.orientation
-
-        self.cutoff = cutoff
-        self.qreverse = qreverse
-        self.blastline = b
+    def subtract(self, o):
+        self.binlen -= o.len
 
-    def __str__(self):
-        ov = Overlap_types[self.otype]
-        s = "{0} - {1}: {2} ".format(self.aid, self.bid, ov)
-        s += "Overlap: {0} Identity: {1}% Orientation: {2}".format(
-            self.hitlen, self.pctid, self.orientation
-        )
-        return s
 
-    @property
-    def swapped(self):
-        blastline = self.blastline.swapped
-        asize = self.asize
-        bsize = self.bsize
-        _, bo = self.get_ao_bo()
-        qreverse = bo == "-"
-        return Overlap(blastline, bsize, asize, self.cutoff, qreverse=qreverse)
-
-    @property
-    def certificateline(self):
-        terminal_tag = "Terminal" if self.isTerminal else "Non-terminal"
-        return "\t".join(
-            str(x)
-            for x in (
-                self.bid,
-                self.asize,
-                self.qstart,
-                self.qstop,
-                self.orientation,
-                terminal_tag,
-            )
-        )
+class BinFile(LineFile):
+    def __init__(self, filename):
+        super(BinFile, self).__init__(filename)
+        self.mapping = defaultdict(list)
 
-    @property
-    def isTerminal(self):
-        return self.isGoodQuality and self.otype in (1, 2)
-
-    @property
-    def isGoodQuality(self):
-        cutoff = self.cutoff
-        return self.hitlen >= cutoff.overlap and self.pctid >= cutoff.pctid
-
-    def get_hangs(self):
-        r"""
-        Determine the type of overlap given query, ref alignment coordinates
-        Consider the following alignment between sequence a and b:
-
-        aLhang \              / aRhang
-                \------------/
-                /------------\
-        bLhang /              \ bRhang
-
-        Terminal overlap: a before b, b before a
-        Contain overlap: a in b, b in a
-        """
-        aLhang, aRhang = self.qstart - 1, self.asize - self.qstop
-        bLhang, bRhang = self.sstart - 1, self.bsize - self.sstop
-        if self.orientation == "-":
-            bLhang, bRhang = bRhang, bLhang
-        if self.qreverse:
-            aLhang, aRhang = aRhang, aLhang
-            bLhang, bRhang = bRhang, bLhang
-
-        return aLhang, aRhang, bLhang, bRhang
-
-    def update_clr(self, aclr, bclr):
-        """
-        Zip the two sequences together, using "left-greedy" rule
-
-        =============                   seqA
-                 ||||
-                 ====(===============)  seqB
-        """
-        print(aclr, bclr, file=sys.stderr)
-        otype = self.otype
-
-        if otype == 1:
-            if aclr.orientation == "+":
-                aclr.end = self.qstop
-            else:
-                aclr.start = self.qstart
-            if bclr.orientation == "+":
-                bclr.start = self.sstop + 1
-            else:
-                bclr.end = self.sstart - 1
-
-        elif otype == 3:
-            aclr.start = aclr.end
-
-        elif otype == 4:
-            bclr.start = bclr.end
-
-        print(aclr, bclr, file=sys.stderr)
-
-    def get_ao_bo(self):
-        ao = "-" if self.qreverse else "+"
-        bo = ao if self.orientation == "+" else {"+": "-", "-": "+"}[ao]
-        return ao, bo
-
-    def anneal(self, aclr, bclr):
-        ao, bo = self.get_ao_bo()
-
-        # Requirement: end-to-end join in correct order and orientation
-        can_anneal = self.otype in (1, 3, 4) and (ao, bo) == (
-            aclr.orientation,
-            bclr.orientation,
-        )
-        if not can_anneal:
-            print(
-                "* Cannot anneal! (otype={0}|{1}{2}|{3}{4})".format(
-                    self.otype, ao, bo, aclr.orientation, bclr.orientation
-                ),
-                file=sys.stderr,
-            )
-            return False
+        fp = open(filename, encoding="utf-8")
+        for row in fp:
+            b = BinLine(row)
+            self.append(b)
+            chr, len, binlen = b.chr, b.len, b.binlen
+            self.mapping[chr].append((len, binlen))
+        fp.close()
 
-        self.update_clr(aclr, bclr)
-        return True
 
-    def print_graphic(self):
-        """
-        >>>>>>>>>>>>>>>>>>>             seqA (alen)
-                  ||||||||
-                 <<<<<<<<<<<<<<<<<<<<<  seqB (blen)
-        """
-        aLhang, aRhang, bLhang, bRhang = self.get_hangs()
-
-        achar = ">"
-        bchar = "<" if self.orientation == "-" else ">"
-        if self.qreverse:
-            achar = "<"
-            bchar = {">": "<", "<": ">"}[bchar]
-
-        print(aLhang, aRhang, bLhang, bRhang, file=sys.stderr)
-        width = 50  # Canvas
-        hitlen = self.hitlen
-        lmax = max(aLhang, bLhang)
-        rmax = max(aRhang, bRhang)
-        bpwidth = lmax + hitlen + rmax
-        ratio = width * 1.0 / bpwidth
-
-        _ = lambda x: int(round(x * ratio, 0))
-        a1, a2 = _(aLhang), _(aRhang)
-        b1, b2 = _(bLhang), _(bRhang)
-        hit = max(_(hitlen), 1)
-
-        msg = " " * max(b1 - a1, 0)
-        msg += achar * (a1 + hit + a2)
-        msg += " " * (width - len(msg) + 2)
-        msg += "{0} ({1})".format(self.aid, self.asize)
-        print(msg, file=sys.stderr)
-
-        msg = " " * max(a1, b1)
-        msg += "|" * hit
-        print(msg, file=sys.stderr)
-
-        msg = " " * max(a1 - b1, 0)
-        msg += bchar * (b1 + hit + b2)
-        msg += " " * (width - len(msg) + 2)
-        msg += "{0} ({1})".format(self.bid, self.bsize)
-        print(msg, file=sys.stderr)
-        print(self, file=sys.stderr)
-
-    @property
-    def otype(self):
-        if not self.isGoodQuality:
-            return 0
-
-        aLhang, aRhang, bLhang, bRhang = self.get_hangs()
-
-        s1 = aRhang + bLhang
-        s2 = aLhang + bRhang
-        s3 = aLhang + aRhang
-        s4 = bLhang + bRhang
-        ms = min(s1, s2, s3, s4)
-        if ms > self.cutoff.hang:
-            type = 0
-        elif ms == s1:
-            type = 1  # a ~ b
-        elif ms == s2:
-            type = 2  # b ~ a
-        elif ms == s3:
-            type = 3  # a in b
-        elif ms == s4:
-            type = 4  # b in a
+class ChrInfoLine:
+    def __init__(self, row, delimiter=","):
+        args = [x.strip() for x in row.split(delimiter)]
+        self.name = args[0]
+        self.color = args[1]
+        if len(args) > 2:
+            self.new_name = args[2]
         else:
-            assert 0
-
-        return type
-
+            self.new_name = self.name
 
-class CertificateLine(object):
-    """
-    North  chr1  2  0  AC229737.8  telomere     58443
-    South  chr1  2  1  AC229737.8  AC202463.29  58443  37835  58443  + Non-terminal
-    """
 
-    def __init__(self, line):
-        args = line.split()
-        self.tag = args[0]
-        self.chr = args[1]
-        self.aphase = int(args[2])
-        self.bphase = int(args[3])
-        self.aid = args[4]
-        self.bid = args[5]
-        self.asize = int(args[6])
-        self.is_no_overlap = False
-
-        if len(args) == 7:
-            self.is_gap = True
-            return
-
-        self.is_gap = False
-
-        if len(args) == 8:
-            assert args[7] == "None"
-            self.is_no_overlap = True
-            self.terminal = "Non-terminal"
-            return
-
-        self.astart = int(args[7])
-        self.astop = int(args[8])
-        self.orientation = args[9]
-        self.terminal = args[10]
-
-    @property
-    def isTerminal(self):
-        return self.terminal == "Terminal"
-
-    def __str__(self):
-        ar = [
-            self.tag,
-            self.chr,
-            self.aphase,
-            self.bphase,
-            self.aid,
-            self.bid,
-            self.asize,
-        ]
-
-        if self.is_no_overlap:
-            ar += ["None"]
-        elif not self.is_gap:
-            ar += [self.astart, self.astop, self.orientation, self.terminal]
-
-        return "\t".join(str(x) for x in ar)
-
-
-class Certificate(BaseFile):
-
-    gapsize = 100000
-    gaps = dict(
-        telomere=gapsize, centromere=gapsize, contig=gapsize, clone=50000, fragment=5000
-    )
-
-    def __init__(self, filename):
-
-        super(Certificate, self).__init__(filename)
-
-        fp = open(filename)
-        self.lines = [CertificateLine(x) for x in fp.readlines()]
-
-    def write(self, filename):
-        fw = must_open(filename, "w")
-        for b in self.lines:
-            print(b, file=fw)
-
-    def get_agp_gap(self, gap_type="contig"):
-        gap_length = Certificate.gaps[gap_type]
-        linkage = "yes" if gap_type in ("fragment", "clone") else "no"
-
-        return ["N", gap_length, gap_type, linkage, ""]
-
-    def write_AGP(self, filename, orientationguide={}):
-        """
-        For each component, we have two overlaps: North and South.
-
-        =======
-           ||||             South
-           ====(=================)  Current BAC
-           North             ||||
-                             ===============
-
-        For the case that says "Non-terminal", the overlap will not be
-        considered. North-South would suggest a '+' orientation, South-North
-        would suggest a '-' orientation. In most cases, unless the overlap
-        involves phase1 BAC, the selected range will be shown as the brackets
-        above - exclude North overlap, and include South overlap (aka the
-        "left-greedy" rule).
-        """
-        fw = must_open(filename, "w")
-        for aid, bb in groupby(self.lines, key=lambda x: x.aid):
-            bb = list(bb)
-            north, south = bb
-            aid = north.aid
-            assert aid == south.aid
-
-            aphase = north.aphase
-            chr = north.chr
-            size = north.asize
-            ar = [chr, 0, 0, 0]
-
-            northline = southline = None
-            northrange = southrange = None
-
-            # Warn if adjacent components do not have valid overlaps
-            if south.is_no_overlap:
-                print(south, file=sys.stderr)
-
-            # Most gaps, except telomeres occur twice, so only do the "North"
-            if north.is_gap:
-                bar = ar + self.get_agp_gap(north.bid)
-                northline = "\t".join(str(x) for x in bar)
-            else:
-                if north.isTerminal:
-                    northrange = north.astart, north.astop
-
-            if south.is_gap:
-                if south.bid == "telomere":
-                    bar = ar + self.get_agp_gap(south.bid)
-                    southline = "\t".join(str(x) for x in bar)
-            else:
-                if south.isTerminal:
-                    southrange = south.astart, south.astop
-                else:
-                    bar = ar + self.get_agp_gap("fragment")
-                    southline = "\t".join(str(x) for x in bar)
-
-            # Determine the orientation and clear range for the current BAC
-            clr = [1, size]
-            orientation = sorientation = None
-            if northrange:
-                start, stop = northrange
-                Lhang = start - 1
-                Rhang = size - stop
-
-                orientation = "+" if Lhang < Rhang else "-"
-                if north.bphase == 1 and north.bphase < aphase:
-                    if Lhang < Rhang:  # North overlap at 5`
-                        clr[0] = start
-                    else:
-                        clr[1] = stop
-                # Override left-greedy (also see below)
-                else:
-                    if Lhang < Rhang:
-                        clr[0] = stop + 1
-                    else:
-                        clr[1] = start - 1
-
-            if southrange:
-                start, stop = southrange
-                Lhang = start - 1
-                Rhang = size - stop
-
-                sorientation = "+" if Lhang > Rhang else "-"
-                # Override left-greedy (also see above)
-                if aphase == 1 and aphase < south.bphase:
-                    if Lhang < Rhang:  # South overlap at 5`
-                        clr[0] = stop + 1
-                    else:
-                        clr[1] = start - 1
-                else:
-                    if Lhang < Rhang:
-                        clr[0] = start
-                    else:
-                        clr[1] = stop
-
-            if orientation:
-                if sorientation:
-                    try:
-                        assert (
-                            orientation == sorientation
-                        ), "Orientation conflicts:\n{0}\n{1}".format(north, south)
-                    except AssertionError as e:
-                        logging.debug(e)
-            else:
-                if sorientation:
-                    orientation = sorientation
-                else:  # Both overlaps fail to define orientation
-                    orientation = orientationguide.get(aid, "+")
-
-            component_type = "D" if aphase in (1, 2) else "F"
-            bar = ar + [component_type, aid, clr[0], clr[1], orientation]
-            cline = "\t".join(str(x) for x in bar)
-
-            if northline:
-                print(northline, file=fw)
-            print(cline, file=fw)
-            if southline:
-                print(southline, file=fw)
+class ChrInfoFile(BaseFile, OrderedDict):
+    def __init__(self, filename, delimiter=","):
+        super(ChrInfoFile, self).__init__(filename)
+        with open(filename, encoding="utf-8") as fp:
+            for row in fp:
+                if row[0] == "#":
+                    continue
+                line = ChrInfoLine(row, delimiter=delimiter)
+                self[line.name] = line
 
-        fw.close()
 
-        reindex([filename, "--inplace"])
+class TitleInfoLine:
+    def __init__(self, row, delimiter=","):
+        args = [x.strip() for x in row.split(delimiter)]
+        self.name = args[0]
+        self.title = args[1]
+        self.subtitle = None
+        if len(args) > 2:
+            self.subtitle = args[2]
+
+
+class TitleInfoFile(BaseFile, OrderedDict):
+    def __init__(self, filename, delimiter=","):
+        super(TitleInfoFile, self).__init__(filename)
+        with open(filename, encoding="utf-8") as fp:
+            for row in fp:
+                if row[0] == "#":
+                    continue
+                line = TitleInfoLine(row, delimiter=delimiter)
+                self[line.name] = line
 
 
 def main():
 
     actions = (
-        ("bes", "confirm the BES mapping"),
-        ("flip", "flip the FASTA sequences according to a set of references"),
-        ("overlap", "check terminal overlaps between two records"),
-        ("batchoverlap", "check terminal overlaps for many pairs"),
-        ("neighbor", "check neighbors of a component in agpfile"),
-        ("blast", "blast a component to componentpool"),
-        ("certificate", "make certificates for all overlaps in agpfile"),
-        ("agp", "make agpfile based on certificates"),
-        ("anneal", "merge adjacent contigs and make new agpfile"),
-        ("dedup", "remove redundant contigs with cdhit"),
+        ("composite", "combine line plots, feature bars and alt-bars"),
+        ("depth", "show per chromosome depth plot across genome"),
+        ("heatmap", "similar to stack but adding heatmap"),
+        ("mosdepth", "plot depth vs. coverage per chromosome"),
+        ("multilineplot", "combine multiple line plots in one vertical stack"),
+        ("stack", "create landscape plot with genic/te composition"),
     )
     p = ActionDispatcher(actions)
     p.dispatch(globals())
 
 
-def dedup(args):
-    """
-    %prog dedup scaffolds.fasta
-
-    Remove redundant contigs with CD-HIT. This is run prior to
-    assembly.sspace.embed().
-    """
-    from jcvi.formats.fasta import gaps
-    from jcvi.apps.cdhit import deduplicate, ids
-
-    p = OptionParser(dedup.__doc__)
-    p.set_align(pctid=GoodPct)
-    p.set_mingap(default=10)
-    opts, args = p.parse_args(args)
+def parse_distfile(filename):
+    """Parse mosdepth dist.txt file. The file has contents like:
 
-    if len(args) != 1:
-        sys.exit(not p.print_help())
+    #chr    start   end     depth   (header added here for clarity)
+    chr01A  0       50000   31.00
+    chr01A  50000   100000  36.00
+    chr01A  100000  150000  280.00
+    chr01A  150000  200000  190.00
 
-    (scaffolds,) = args
-    mingap = opts.mingap
-    splitfile, oagpfile, cagpfile = gaps(
-        [scaffolds, "--split", "--mingap={0}".format(mingap)]
-    )
-
-    dd = splitfile + ".cdhit"
-    clstrfile = dd + ".clstr"
-    idsfile = dd + ".ids"
-    if need_update(splitfile, clstrfile):
-        deduplicate([splitfile, "--pctid={0}".format(opts.pctid)])
-    if need_update(clstrfile, idsfile):
-        ids([clstrfile])
-
-    agp = AGP(cagpfile)
-    reps = set(x.split()[-1] for x in open(idsfile))
-    pf = scaffolds.rsplit(".", 1)[0]
-    dedupagp = pf + ".dedup.agp"
-    fw = open(dedupagp, "w")
-
-    ndropped = ndroppedbases = 0
-    for a in agp:
-        if not a.is_gap and a.component_id not in reps:
-            span = a.component_span
-            logging.debug("Drop component {0} ({1})".format(a.component_id, span))
-            ndropped += 1
-            ndroppedbases += span
-            continue
-        print(a, file=fw)
-    fw.close()
-
-    logging.debug(
-        "Dropped components: {0}, Dropped bases: {1}".format(ndropped, ndroppedbases)
-    )
-    logging.debug("Deduplicated file written to `{0}`.".format(dedupagp))
-
-    tidyagp = tidy([dedupagp, splitfile])
-    dedupfasta = pf + ".dedup.fasta"
-    build([tidyagp, dd, dedupfasta])
-
-    return dedupfasta
-
-
-def get_shred_id(id):
-    """
-    >>> get_shred_id("ca-bacs.5638.frag11.22000-23608")
-    ("ca-bacs.5638", 11)
+    Args:
+        filename (str): Path to the file.
     """
-    try:
-        parts = id.split(".")
-        aid = ".".join(parts[:2])
-        fid = int(parts[2].replace("frag", ""))
-    except:
-        aid, fid = None, None
-    return aid, fid
-
-
-def is_adjacent_shreds(a, b):
-    aid, bid = a.component_id, b.component_id
-    ao, bo = a.orientation, b.orientation
-    if ao != bo:
-        return False
-
-    ai, af = get_shred_id(aid)
-    bi, bf = get_shred_id(bid)
-    if ai is None or bi is None:
-        return False
-
-    # Same sequence, with fragment id offset by one
-    return ai == bi and abs(af - bf) == 1
-
-
-def overlap_blastline_writer(oopts):
-    o = overlap(oopts)
-    if not o:
-        return ""
-
-    return str(o.blastline)
-
+    dists = defaultdict(Counter)
+    with must_open(filename) as fp:
+        for row in fp:
+            chromosome, _, _, depth = row.split()
+            depth = int(float(depth))
+            dists[chromosome][depth] += 1
+    logger.debug("Loaded %d seqids", len(dists))
+    return dists
+
+
+def parse_groupsfile(filename):
+    """Parse groupsfile, which contains the tracks to be plotted
+    in the vertically stacked mosdepth plot.
+
+    chr01A,chr01B g,m
+    chr02A,chr02B g,m
+    chr03A,chr03B g,m
 
-def get_overlap_opts(aid, bid, qreverse, outdir, opts):
-    oopts = [
-        aid,
-        bid,
-        "--suffix",
-        "fa",
-        "--dir",
-        outdir,
-        "--pctid={0}".format(opts.pctid),
-        "--hitlen={0}".format(opts.hitlen),
-    ]
-    if qreverse:
-        oopts += ["--qreverse"]
-    return oopts
+    Args:
+        filename (str): Path to the groups file.
+    """
+    groups = []
+    with open(filename, encoding="utf-8") as fp:
+        for row in fp:
+            chrs, colors = row.split()
+            groups.append((chrs.split(","), colors.split(",")))
+    logger.debug("Loaded %d groups", len(groups))
+    return groups
 
 
-def populate_blastfile(blastfile, agp, outdir, opts):
-    assert not op.exists(blastfile)
-    all_oopts = []
-    for a, b, qreverse in agp.iter_paired_components():
-        aid = a.component_id
-        bid = b.component_id
-        oopts = get_overlap_opts(aid, bid, qreverse, outdir, opts)
-        all_oopts.append(oopts)
+def cumarray_to_array(ar):
+    """Convert cumulative array to normal array.
 
-    pool = WriteJobs(overlap_blastline_writer, all_oopts, blastfile, cpus=opts.cpus)
-    pool.run()
+    Args:
+        ar (List): List of numbers
+    """
+    ans = []
+    for i, x in enumerate(ar):
+        ans.append(x if i == 0 else (ar[i] - ar[i - 1]))
+    return ans
 
 
-def anneal(args):
+def mosdepth(args):
     """
-    %prog anneal agpfile contigs.fasta
+    %prog mosdepth mosdepth.global.dist.txt groups
 
-    Merge adjacent overlapping contigs and make new AGP file.
+    Plot depth vs. coverage per chromosome. Inspired by mosdepth plot. See also:
+    https://github.com/brentp/mosdepth
+    """
+    import seaborn as sns
 
-    By default it will also anneal lines like these together (unless --nozipshreds):
-    scaffold4       1       1608    1       W       ca-bacs.5638.frag11.22000-23608 1       1608    -
-    scaffold4       1609    1771    2       N       163     scaffold        yes     paired-ends
-    scaffold4       1772    3771    3       W       ca-bacs.5638.frag10.20000-22000 1       2000    -
+    sns.set_style("darkgrid")
 
-    These are most likely shreds, which we look for based on names.
-    """
-    p = OptionParser(anneal.__doc__)
-    p.set_align(pctid=GoodPct, hitlen=GoodOverlap)
+    p = OptionParser(mosdepth.__doc__)
+    p.add_option("--maxdepth", default=100, type="int", help="Maximum depth to plot")
     p.add_option(
-        "--hang", default=GoodOverhang, type="int", help="Maximum overhang length"
+        "--logscale", default=False, action="store_true", help="Use log-scale on depth"
     )
-    p.set_outdir(outdir="outdir")
-    p.set_cpus()
-    opts, args = p.parse_args(args)
+    opts, args, iopts = p.set_image_options(args, style="dark", figsize="6x8")
 
     if len(args) != 2:
-        sys.exit(not p.print_help())
+        sys.exit(p.print_help())
 
-    agpfile, contigs = args
-    outdir = opts.outdir
-    if not op.exists(outdir):
-        mkdir(outdir)
-        cmd = "faSplit byname {0} {1}/".format(contigs, outdir)
-        sh(cmd)
-
-    cutoff = Cutoff(opts.pctid, opts.hitlen, opts.hang)
-    logging.debug(str(cutoff))
-
-    agp = AGP(agpfile)
-    blastfile = agpfile.replace(".agp", ".blast")
-    if not op.exists(blastfile):
-        populate_blastfile(blastfile, agp, outdir, opts)
-
-    assert op.exists(blastfile)
-    logging.debug("File `{0}` found. Start loading.".format(blastfile))
-    blast = BlastSlow(blastfile).to_dict()
-
-    annealedagp = "annealed.agp"
-    annealedfasta = "annealed.fasta"
-
-    newagp = deepcopy(agp)
-    clrstore = {}
-    for a, b, qreverse in agp.iter_paired_components():
-        aid = a.component_id
-        bid = b.component_id
-
-        pair = (aid, bid)
-        if pair in blast:
-            bl = blast[pair]
-        else:
-            oopts = get_overlap_opts(aid, bid, qreverse, outdir, opts)
-            o = overlap(oopts)
-            if not o:
-                continue
-            bl = o.blastline
+    # Read in datasets
+    distfile, groupsfile = args
+    dists = parse_distfile(distfile)
+    groups = parse_groupsfile(groupsfile)
+    logscale = opts.logscale
+
+    # Construct a composite figure with N tracks indicated in the groups
+    fig = plt.figure(1, (iopts.w, iopts.h))
+    root = fig.add_axes((0, 0, 1, 1))
+
+    rows = len(groups)
+    ypad = 0.05
+    yinterval = (1 - 2 * ypad) / (rows + 1)
+    yy = 1 - ypad
+
+    for group_idx, (chrs, colors) in enumerate(groups):
+        yy -= yinterval
+        ax = fig.add_axes((0.15, yy, 0.7, yinterval * 0.85))
+        for c, color in zip(chrs, colors):
+            cdata = dists[c].items()
+            logger.debug("Importing %d records for %s", len(cdata), c)
+            cx, cy = zip(*sorted(cdata))
+            ax.plot(cx, cy, "-", color=color)
+        if logscale:
+            ax.set_xscale("log", basex=2)
+        ax.set_xlim(1 if logscale else 0, opts.maxdepth)
+        ax.get_yaxis().set_visible(False)
+        if group_idx != rows - 1:
+            ax.get_xaxis().set_visible(False)
+
+        # Add legend to the right of the canvas
+        label_pad = 0.02
+        label_yy = yy + yinterval
+        for c, color in zip(chrs, colors):
+            label_yy -= label_pad
+            root.text(0.92, label_yy, c, color=color, ha="center", va="center")
+
+    root.text(
+        0.1,
+        0.5,
+        "Proportion of bases at coverage",
+        rotation=90,
+        color="darkslategray",
+        ha="center",
+        va="center",
+    )
+    root.text(0.5, 0.05, "Coverage", color="darkslategray", ha="center", va="center")
+    normalize_axes(root)
+    adjust_spines(ax, ["bottom"], outward=True)
+
+    pf = "mosdepth"
+    image_name = pf + "." + iopts.format
+    savefig(image_name, dpi=iopts.dpi, iopts=iopts)
+
+
+def draw_depth(
+    root,
+    ax,
+    bed: Bed,
+    chrinfo: dict = {},
+    defaultcolor: str = "k",
+    sepcolor: str = "w",
+    maxdepth: int = 100,
+    logscale: bool = False,
+    title: Optional[str] = None,
+    subtitle: Optional[str] = None,
+):
+    """Draw depth plot on the given axes, using data from bed
+
+    Args:
+        root (matplotlib.Axes): Canvas axes
+        ax (matplotlib.Axes): Axes to plot data on
+        bed (Bed): Bed data from mosdepth
+        chrinfo (ChrInfoFile): seqid => color, new name
+        defaultcolor (str): matplotlib-compatible color for data points
+        sepcolor (str): matplotlib-compatible color for chromosome breaks
+        maxdepth (int): Upper limit of the y-axis (depth)
+        title (str): Title of the figure, to the right of the axis
+        subtitle (str): Subtitle of the figure, just below title
+    """
+    if chrinfo is None:
+        chrinfo = {}
+    sizes = bed.max_bp_in_chr
+    seqids = chrinfo.keys() if chrinfo else sizes.keys()
+    starts = {}
+    ends = {}
+    label_positions = []
+    start = 0
+    for seqid in seqids:
+        if seqid not in sizes:
+            continue
+        starts[seqid] = start
+        end = start + sizes[seqid]
+        ends[seqid] = end
+        label_positions.append((seqid, (start + end) / 2))
+        start = end
+    xsize = end
+
+    # Extract plotting data
+    data = []
+    data_by_seqid = defaultdict(list)
+    for b in bed:
+        seqid = b.seqid
+        if seqid not in starts:
+            continue
+        # chr01A  2000000 3000000 113.00
+        x = starts[seqid] + (b.start + b.end) / 2
+        y = float(b.accn)
+        c = chrinfo[seqid].color if seqid in chrinfo else "k"
+        data.append((x, y, c))
+        data_by_seqid[seqid].append(y)
+
+    x, y, c = zip(*data)
+    ax.scatter(
+        x,
+        y,
+        c=c,
+        edgecolors="none",
+        s=8,
+        lw=0,
+    )
+    logger.debug("Obtained %d data points with depth data", len(data))
 
-        o = Overlap(bl, a.component_span, b.component_span, cutoff, qreverse=qreverse)
+    # Per seqid median
+    medians = {}
+    for seqid, values in data_by_seqid.items():
+        c = chrinfo[seqid].color if seqid in chrinfo else defaultcolor
+        seqid_start = starts[seqid]
+        seqid_end = ends[seqid]
+        seqid_median = np.median(values)
+        medians[seqid] = seqid_median
+        ax.plot(
+            (seqid_start, seqid_end),
+            (seqid_median, seqid_median),
+            "-",
+            lw=4,
+            color=c,
+            alpha=0.5,
+        )
 
-        if aid not in clrstore:
-            clrstore[aid] = CLR.from_agpline(a)
-        if bid not in clrstore:
-            clrstore[bid] = CLR.from_agpline(b)
+    # Vertical lines for all the breaks
+    for pos in starts.values():
+        ax.plot((pos, pos), (0, maxdepth), "-", lw=1, color=sepcolor)
+
+    # Beautify the numeric axis
+    for tick in ax.get_xticklines() + ax.get_yticklines():
+        tick.set_visible(False)
+
+    median_depth_y = 0.88
+    chr_label_y = 0.08
+    for seqid, position in label_positions:
+        xpos = 0.1 + position * 0.8 / xsize
+        c = chrinfo[seqid].color if seqid in chrinfo else defaultcolor
+        newseqid = chrinfo[seqid].new_name if seqid in chrinfo else seqid
+        root.text(
+            xpos, chr_label_y, newseqid, color=c, ha="center", va="center", rotation=20
+        )
+        seqid_median = medians[seqid]
+        root.text(
+            xpos,
+            median_depth_y,
+            str(int(seqid_median)),
+            color=c,
+            ha="center",
+            va="center",
+        )
 
-        aclr, bclr = clrstore[aid], clrstore[bid]
+    # Add an arrow to the right of the plot, indicating these are median depths
+    root.text(
+        0.91,
+        0.88,
+        r"$\leftarrow$median",
+        color="lightslategray",
+        va="center",
+    )
 
-        o.print_graphic()
-        if o.anneal(aclr, bclr):
-            newagp.delete_between(aid, bid, verbose=True)
+    if title:
+        root.text(
+            0.95,
+            0.5,
+            markup(title),
+            color="darkslategray",
+            ha="center",
+            va="center",
+            size=15,
+        )
+    if subtitle:
+        root.text(
+            0.95,
+            0.375,
+            markup(subtitle),
+            color="darkslategray",
+            ha="center",
+            va="center",
+            size=15,
+        )
 
-        if o.otype == 2:  # b ~ a
-            o = o.swapped
-            o.print_graphic()
-            if o.anneal(bclr, aclr):
-                newagp.switch_between(bid, aid, verbose=True)
-                newagp.delete_between(bid, aid, verbose=True)
+    ax.set_xticks([])
+    ax.set_xlim(0, xsize)
+    if logscale:
+        ax.set_yscale("log", basey=2)
+    ax.set_ylim(1 if logscale else 0, maxdepth)
+    ax.set_ylabel("Depth")
+
+    set_human_axis(ax)
+    plt.setp(ax.get_xticklabels() + ax.get_yticklabels(), color="gray", size=10)
+    normalize_axes(root)
+
+
+def draw_multi_depth(
+    root,
+    panel_roots,
+    panel_axes,
+    bedfiles: List[str],
+    chrinfo_file: str,
+    titleinfo_file: str,
+    maxdepth: int,
+    logscale: bool,
+):
+    """
+    Draw multiple depth plots on the same canvas.
+    """
+    chrinfo = ChrInfoFile(chrinfo_file) if chrinfo_file else {}
+    titleinfo = TitleInfoFile(titleinfo_file) if titleinfo_file else {}
+    npanels = len(bedfiles)
+    yinterval = 1.0 / npanels
+    ypos = 1 - yinterval
+    for bedfile, panel_root, panel_ax in zip(bedfiles, panel_roots, panel_axes):
+        pf = op.basename(bedfile).split(".", 1)[0]
+        bed = Bed(bedfile)
+
+        if ypos > 0.001:
+            root.plot((0.02, 0.98), (ypos, ypos), "-", lw=2, color="lightslategray")
+
+        title = titleinfo.get(bedfile, pf.split("_", 1)[0])
+        subtitle = None
+        if isinstance(title, TitleInfoLine):
+            subtitle = title.subtitle
+            title = title.title
+
+        draw_depth(
+            panel_root,
+            panel_ax,
+            bed,
+            chrinfo=chrinfo,
+            maxdepth=maxdepth,
+            logscale=logscale,
+            title=title,
+            subtitle=subtitle,
+        )
+        ypos -= yinterval
 
-    logging.debug("A total of {0} components with modified CLR.".format(len(clrstore)))
+    normalize_axes(root)
 
-    for cid, c in clrstore.items():
-        if c.is_valid:
-            continue
-        print("Remove {0}".format(c), file=sys.stderr)
-        newagp.convert_to_gap(cid, verbose=True)
 
-    # Update all ranges that has modified clr
-    for a in newagp:
-        if a.is_gap:
-            continue
-        aid = a.component_id
-        if aid in clrstore:
-            c = clrstore[aid]
-            a.component_beg = c.start
-            a.component_end = c.end
+def depth(args):
+    """
+    %prog depth *.regions.bed.gz
 
-    newagp.print_to_file(annealedagp)
-    tidyagp = tidy([annealedagp, contigs])
+    Plot the mosdepth regions BED file. We recommend to generate this BED file
+    by (please adjust the --by parameter to your required resolution):
 
-    build([tidyagp, contigs, annealedfasta])
-    return annealedfasta
+    $ mosdepth --no-per-base --use-median --fast-mode --by 1000000 sample.wgs
+    sample.bam
 
+    Use --chrinfo to specify a colormap between seqid, desired color, and
+    optionally a new name. For example:
 
-def blast(args):
-    """
-    %prog blast allfasta clonename
+    chr01A, #c51b7d, 1A
+    chr01B, #4d9221, 1B
+    ...
 
-    Insert a component into agpfile by aligning to the best hit in pool and see
-    if they have good overlaps.
-    """
-    from jcvi.apps.align import run_megablast
+    Only seqids that are in the colormap will be plotted, in the order that's
+    given in the file. When --colormap is not set, every seqid will be drawn in
+    black.
 
-    p = OptionParser(blast.__doc__)
-    p.add_option("-n", type="int", default=2, help="Take best N hits")
-    opts, args = p.parse_args(args)
+    Can take multiple BED files as input and then plot all of them in a
+    composite figure.
+    """
+    p = OptionParser(depth.__doc__)
+    p.add_option(
+        "--chrinfo", help="Comma-separated mappings between seqid, color, new_name"
+    )
+    p.add_option(
+        "--titleinfo",
+        help="Comma-separated titles mappings between filename, title",
+    )
+    p.add_option("--maxdepth", default=100, type="int", help="Maximum depth to show")
+    p.add_option(
+        "--logscale", default=False, action="store_true", help="Use log-scale on depth"
+    )
+    opts, args, iopts = p.set_image_options(args, style="dark", figsize="14x4")
 
-    if len(args) != 2:
+    if len(args) < 1:
         sys.exit(not p.print_help())
 
-    allfasta, clonename = args
-    fastadir = "fasta"
-    infile = op.join(fastadir, clonename + ".fasta")
-    if not op.exists(infile):
-        entrez([clonename, "--skipcheck", "--outdir=" + fastadir])
-
-    outfile = "{0}.{1}.blast".format(clonename, allfasta.split(".")[0])
-    run_megablast(
-        infile=infile, outfile=outfile, db=allfasta, pctid=GoodPct, hitlen=GoodOverlap
-    )
-
-    blasts = [BlastLine(x) for x in open(outfile)]
-    besthits = []
-    for b in blasts:
-        if b.query.count("|") >= 3:
-            b.query = b.query.split("|")[3]
-
-        if b.subject.count("|") >= 3:
-            b.subject = b.subject.split("|")[3]
+    bedfiles = args
 
-        b.query = b.query.rsplit(".", 1)[0]
-        b.subject = b.subject.rsplit(".", 1)[0]
+    fig = plt.figure(1, (iopts.w, iopts.h))
+    root = fig.add_axes((0, 0, 1, 1))
 
-        if b.query == b.subject:
-            continue
-
-        if b.subject not in besthits:
-            besthits.append(b.subject)
-        if len(besthits) == opts.n:
-            break
+    npanels = len(bedfiles)
+    yinterval = 1.0 / npanels
+    ypos = 1 - yinterval
+    panel_roots, panel_axes = [], []
+    for _ in range(npanels):
+        panel_root = root if npanels == 1 else fig.add_axes((0, ypos, 1, yinterval))
+        panel_ax = fig.add_axes((0.1, ypos + 0.2 * yinterval, 0.8, 0.65 * yinterval))
+        panel_roots.append(panel_root)
+        panel_axes.append(panel_ax)
+        ypos -= yinterval
+
+    draw_multi_depth(
+        root,
+        panel_roots,
+        panel_axes,
+        bedfiles,
+        opts.chrinfo,
+        opts.titleinfo,
+        opts.maxdepth,
+        opts.logscale,
+    )
 
-    for b in besthits:
-        overlap([clonename, b, "--dir=" + fastadir])
+    if npanels > 1:
+        pf = op.commonprefix(bedfiles)
+    pf = pf or "depth"
+    image_name = pf + "." + iopts.format
+    savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
-def bes(args):
+def add_window_options(p):
     """
-    %prog bes bacfasta clonename
-
-    Use the clone name to download BES gss sequences from Genbank, map and then
-    visualize.
+    Add options for window plotting.
     """
-    from jcvi.apps.align import run_blat
-
-    p = OptionParser(bes.__doc__)
-    p.set_cpus()
-    opts, args = p.parse_args(args)
-
-    if len(args) != 2:
-        sys.exit(not p.print_help())
+    p.add_option("--window", default=500000, type="int", help="Size of window")
+    p.add_option("--shift", default=100000, type="int", help="Size of shift")
+    p.add_option("--subtract", help="Subtract bases from window")
+    p.add_option(
+        "--nomerge", default=False, action="store_true", help="Do not merge features"
+    )
 
-    bacfasta, clonename = args
 
-    entrez([clonename, "--database=nucgss", "--skipcheck"])
-    besfasta = clonename + ".fasta"
-    blatfile = clonename + ".bes.blat"
-    run_blat(
-        infile=besfasta,
-        outfile=blatfile,
-        db=bacfasta,
-        pctid=95,
-        hitlen=100,
-        cpus=opts.cpus,
-    )
-
-    aid, asize = next(Fasta(bacfasta).itersizes())
-
-    width = 50
-    msg = "=" * width
-    msg += "  " + aid
-    print(msg, file=sys.stderr)
-
-    ratio = width * 1.0 / asize
-    _ = lambda x: int(round(x * ratio, 0))
-    blasts = [BlastLine(x) for x in open(blatfile)]
-    for b in blasts:
-        if b.orientation == "+":
-            msg = " " * _(b.sstart) + "->"
-        else:
-            msg = " " * (_(b.sstop) - 2) + "<-"
-        msg += " " * (width - len(msg) + 2)
-        msg += b.query
-        if b.orientation == "+":
-            msg += " (hang={0})".format(b.sstart - 1)
-        else:
-            msg += " (hang={0})".format(asize - b.sstop)
+def check_window_options(opts):
+    """
+    Check the window options, and return the values.
+    """
+    window = opts.window
+    shift = opts.shift
+    subtract = opts.subtract
+    assert window % shift == 0, "--window must be divisible by --shift"
+    logger.debug(
+        "Line/stack-plot options: window=%d shift=%d subtract=%s",
+        window,
+        shift,
+        subtract,
+    )
+    merge = not opts.nomerge
 
-        print(msg, file=sys.stderr)
+    return window, shift, subtract, merge
 
 
-def flip(args):
+def get_beds(s: List[str], binned: bool = False) -> List[str]:
     """
-    %prog flip fastafile
-
-    Go through each FASTA record, check against Genbank file and determines
-    whether or not to flip the sequence. This is useful before updates of the
-    sequences to make sure the same orientation is used.
+    Get the bed files for each feature, and return them as a list.
     """
-    p = OptionParser(flip.__doc__)
-    opts, args = p.parse_args(args)
+    return [x + ".bed" for x in s] if not binned else [x for x in s]
 
-    if len(args) != 1:
-        sys.exit(not p.print_help())
 
-    (fastafile,) = args
-    outfastafile = fastafile.rsplit(".", 1)[0] + ".flipped.fasta"
-    fo = open(outfastafile, "w")
-    f = Fasta(fastafile, lazy=True)
-    for name, rec in f.iteritems_ordered():
-        tmpfasta = "a.fasta"
-        fw = open(tmpfasta, "w")
-        SeqIO.write([rec], fw, "fasta")
-        fw.close()
+def linearray(binfile, chr, window, shift):
+    mn = binfile.mapping[chr]
+    m, _ = zip(*mn)
 
-        o = overlap([tmpfasta, name])
-        if o.orientation == "-":
-            rec.seq = rec.seq.reverse_complement()
+    m = np.array(m, dtype="float")
+    w = window // shift
+    m = moving_sum(m, window=w)
+    return m
 
-        SeqIO.write([rec], fo, "fasta")
-        cleanup(tmpfasta)
 
+def lineplot(ax, binfiles, nbins, chr, window, shift, color="br"):
+    assert len(binfiles) <= 2, "A max of two line plots are supported"
 
-def batchoverlap(args):
-    """
-    %prog batchoverlap pairs.txt outdir
+    t = np.arange(nbins)
+    bf = binfiles[0]
+    m = linearray(bf, chr, window, shift)
+    ax.plot(t, m, "{0}-".format(color[0]), lw=2)
 
-    Check overlaps between pairs of sequences.
-    """
-    p = OptionParser(batchoverlap.__doc__)
-    p.set_cpus()
-    opts, args = p.parse_args(args)
+    formatter = ticker.FuncFormatter(
+        lambda x, pos: human_readable_base(int(x) * shift, pos)
+    )
+    ax.xaxis.set_major_formatter(formatter)
+    for tl in ax.get_xticklabels():
+        tl.set_color("darkslategray")
+
+    label = bf.filename.split(".")[0]
+    perw = "per {0}".format(human_size(window, precision=0))
+    ax.set_ylabel(label + " " + perw, color=color[0])
+
+    if len(binfiles) == 2:
+        ax2 = ax.twinx()
+        bf = binfiles[1]
+        m = linearray(bf, chr, window, shift)
+        ax2.plot(t, m, "{0}-".format(color[1]), lw=2)
+        # Differentiate tick labels through colors
+        for tl in ax.get_yticklabels():
+            tl.set_color(color[0])
+        for tl in ax2.get_yticklabels():
+            tl.set_color(color[1])
+
+        label = bf.filename.split(".")[0]
+        ax2.set_ylabel(label + " " + perw, color=color[1])
+
+    ax.set_xlim(0, nbins)
+
+
+def composite(args):
+    """
+    %prog composite fastafile chr1
+
+    Combine line plots, feature bars and alt-bars, different data types
+    specified in options. Inputs must be BED-formatted. Three types of viz are
+    currently supported:
+
+    --lines: traditional line plots, useful for plotting feature freq
+    --bars: show where the extent of features are
+    --altbars: similar to bars, yet in two alternating tracks, e.g. scaffolds
+    """
+    p = OptionParser(composite.__doc__)
+    p.add_option("--lines", help="Features to plot in lineplot")
+    p.add_option("--bars", help="Features to plot in bars")
+    p.add_option("--altbars", help="Features to plot in alt-bars")
+    p.add_option(
+        "--fatten",
+        default=False,
+        action="store_true",
+        help="Help visualize certain narrow features",
+    )
+    p.add_option(
+        "--mode",
+        default="span",
+        choices=("span", "count", "score"),
+        help="Accumulate feature based on",
+    )
+    add_window_options(p)
+    opts, args, iopts = p.set_image_options(args, figsize="8x5")
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
-    pairsfile, outdir = args
-    fp = open(pairsfile)
-    cmds = []
-    mkdir("overlaps")
-    for row in fp:
-        a, b = row.split()[:2]
-        oa = op.join(outdir, a + ".fa")
-        ob = op.join(outdir, b + ".fa")
-        cmd = "python -m jcvi.assembly.goldenpath overlap {0} {1}".format(oa, ob)
-        cmd += " -o overlaps/{0}_{1}.ov".format(a, b)
-        cmds.append(cmd)
+    fastafile, chr = args
+    window, shift, _, merge = check_window_options(opts)
+    linebeds, barbeds, altbarbeds = [], [], []
+    fatten = opts.fatten
+    if opts.lines:
+        lines = opts.lines.split(",")
+        linebeds = get_beds(lines)
+    if opts.bars:
+        bars = opts.bars.split(",")
+        barbeds = get_beds(bars)
+    if opts.altbars:
+        altbars = opts.altbars.split(",")
+        altbarbeds = get_beds(altbars)
+
+    linebins = get_binfiles(linebeds, fastafile, shift, mode=opts.mode, merge=merge)
+
+    margin = 0.12
+    clen = Sizes(fastafile).mapping[chr]
+    nbins, _ = get_nbins(clen, shift)
+
+    plt.rcParams["xtick.major.size"] = 0
+    plt.rcParams["ytick.major.size"] = 0
+
+    fig = plt.figure(1, (iopts.w, iopts.h))
+    root = fig.add_axes((0, 0, 1, 1))
+
+    root.text(0.5, 0.95, chr, ha="center", color="darkslategray")
+
+    xstart, xend = margin, 1 - margin
+    xlen = xend - xstart
+    ratio = xlen / clen
+    # Line plots
+    ax = fig.add_axes((xstart, 0.6, xlen, 0.3))
+    lineplot(ax, linebins, nbins, chr, window, shift)
+
+    # Bar plots
+    yy = 0.5
+    yinterval = 0.08
+    xs = lambda x: xstart + ratio * x
+    r = 0.01
+    fattend = 0.0025
+    for bb in barbeds:
+        root.text(xend + 0.01, yy, bb.split(".")[0], va="center")
+        HorizontalChromosome(root, xstart, xend, yy, height=0.02)
+        bb = Bed(bb)
+        for b in bb:
+            start, end = xs(b.start), xs(b.end)
+            span = end - start
+            if fatten and span < fattend:
+                span = fattend
+
+            root.add_patch(
+                Rectangle((start, yy - r), span, 2 * r, lw=0, fc="darkslategray")
+            )
+        yy -= yinterval
 
-    print("\n".join(cmds))
+    # Alternative bar plots
+    offset = r / 2
+    for bb in altbarbeds:
+        root.text(xend + 0.01, yy, bb.split(".")[0], va="center")
+        bb = Bed(bb)
+        for b in bb:
+            start, end = xs(b.start), xs(b.end)
+            span = end - start
+            if span < 0.0001:
+                continue
+            offset = -offset
+            root.add_patch(
+                Rectangle(
+                    (start, yy + offset), end - start, 0.003, lw=0, fc="darkslategray"
+                )
+            )
+        yy -= yinterval
 
+    root.set_xlim(0, 1)
+    root.set_ylim(0, 1)
+    root.set_axis_off()
+
+    image_name = chr + "." + iopts.format
+    savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
-def overlap(args):
-    """
-    %prog overlap <a|a.fasta> <b|b.fasta>
 
-    Check overlaps between two fasta records. The arguments can be genBank IDs
-    instead of FASTA files. In case of IDs, the sequences will be downloaded
-    first.
+def multilineplot(args):
     """
-    from jcvi.formats.blast import chain_HSPs
+    %prog multilineplot fastafile chr1
 
-    p = OptionParser(overlap.__doc__)
-    p.add_option(
-        "--dir",
-        default=os.getcwd(),
-        help="Download sequences to dir",
-    )
+    Combine multiple line plots in one vertical stack
+    Inputs must be BED-formatted.
+
+    --lines: traditional line plots, useful for plotting feature freq
+    """
+    p = OptionParser(multilineplot.__doc__)
+    p.add_option("--lines", help="Features to plot in lineplot")
+    p.add_option("--colors", help="List of colors matching number of input bed files")
     p.add_option(
-        "--suffix",
-        default="fasta",
-        help="Suffix of the sequence file in dir",
+        "--mode",
+        default="span",
+        choices=("span", "count", "score"),
+        help="Accumulate feature based on",
     )
     p.add_option(
-        "--qreverse",
+        "--binned",
         default=False,
         action="store_true",
-        help="Reverse seq a",
+        help="Specify whether the input is already binned; "
+        + "if True, input files are considered to be binfiles",
     )
-    p.add_option(
-        "--nochain",
-        default=False,
-        action="store_true",
-        help="Do not chain adjacent HSPs",
-    )
-    p.set_align(pctid=GoodPct, hitlen=GoodOverlap, evalue=0.01)
-    p.set_outfile(outfile=None)
-    opts, args = p.parse_args(args)
+    p.add_option("--ymax", type="int", help="Set Y-axis max")
+    add_window_options(p)
+    opts, args, iopts = p.set_image_options(args, figsize="8x5")
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
-    afasta, bfasta = args
-    dir = opts.dir
-    chain = not opts.nochain
-    suffix = opts.suffix
-    evalue = opts.evalue
-    pctid = opts.pctid
-    hitlen = opts.hitlen
-    cutoff = Cutoff(pctid, hitlen)
-
-    # Check first whether it is file or accession name
-    if not op.exists(afasta):
-        af = op.join(dir, ".".join((afasta, suffix)))
-        if not op.exists(af):  # Check to avoid redownload
-            entrez([afasta, "--skipcheck", "--outdir=" + dir])
-        afasta = af
-
-    if not op.exists(bfasta):
-        bf = op.join(dir, ".".join((bfasta, suffix)))
-        if not op.exists(bf):
-            entrez([bfasta, "--skipcheck", "--outdir=" + dir])
-        bfasta = bf
-
-    assert op.exists(afasta) and op.exists(bfasta)
-
-    cmd = "blastn -dust no"
-    cmd += " -query {0} -subject {1}".format(afasta, bfasta)
-    cmd += " -evalue {0} -outfmt 6 -perc_identity {1}".format(evalue, pctid)
-
-    fp = popen(cmd)
-    hsps = fp.readlines()
-
-    hsps = [BlastLine(x) for x in hsps]
-    hsps = [x for x in hsps if x.hitlen >= hitlen]
-    if chain:
-        logging.debug("Chain HSPs in the Blast output.")
-        dist = 2 * hitlen  # Distance to chain the HSPs
-        hsps = chain_HSPs(hsps, xdist=dist, ydist=dist)
-
-    if len(hsps) == 0:
-        print("No match found.", file=sys.stderr)
-        return None
-
-    besthsp = hsps[0]
-
-    aid, asize = next(Fasta(afasta).itersizes())
-    bid, bsize = next(Fasta(bfasta).itersizes())
-    o = Overlap(besthsp, asize, bsize, cutoff, qreverse=opts.qreverse)
-    o.print_graphic()
-
-    if opts.outfile:
-        fw = must_open(opts.outfile, "w")
-        print(str(o), file=fw)
-        fw.close()
-
-    return o
-
-
-@lru_cache(maxsize=None)
-def phase(accession):
-    gbdir = "gb"
-    gbfile = op.join(gbdir, accession + ".gb")
-    if not op.exists(gbfile):
-        entrez([accession, "--skipcheck", "--outdir=" + gbdir, "--format=gb"])
-    rec = next(SeqIO.parse(gbfile, "gb"))
-    ph, keywords = get_phase(rec)
-    return ph, len(rec)
-
-
-def check_certificate(certificatefile):
-    data = {}
-    if op.exists(certificatefile):
-        # This will make updates resume-able and backed-up
-        certificatefilebak = certificatefile + ".orig"
-        shutil.copy2(certificatefile, certificatefilebak)
-
-        fp = open(certificatefile)
-        for row in fp:
-            atoms = row.split()
-            tag, aid, bid = atoms[0], atoms[4], atoms[5]
-            data[(tag, aid, bid)] = row.strip()
+    fastafile, chr = args
+    window, shift, _, merge = check_window_options(opts)
+    linebeds = []
+    colors = opts.colors
+    if opts.lines:
+        lines = opts.lines.split(",")
+        assert len(colors) == len(lines), (
+            "Number of chosen colors must match" + " number of input bed files"
+        )
+        linebeds = get_beds(lines, binned=opts.binned)
 
-    return data
+    linebins = get_binfiles(
+        linebeds, fastafile, shift, mode=opts.mode, binned=opts.binned, merge=merge
+    )
 
+    clen = Sizes(fastafile).mapping[chr]
+    nbins, _ = get_nbins(clen, shift)
 
-def certificate(args):
-    """
-    %prog certificate tpffile certificatefile
+    plt.rcParams["xtick.major.size"] = 0
+    plt.rcParams["ytick.major.size"] = 0
+    plt.rcParams["figure.figsize"] = iopts.w, iopts.h
+
+    fig, axarr = plt.subplots(nrows=len(lines))
+    if len(linebeds) == 1:
+        axarr = (axarr,)
+    fig.suptitle(latex(chr), color="darkslategray")
+
+    for i, ax in enumerate(axarr):
+        lineplot(
+            ax,
+            [linebins[i]],
+            nbins,
+            chr,
+            window,
+            shift,
+            color="{0}{1}".format(colors[i], "r"),
+        )
 
-    Generate certificate file for all overlaps in tpffile. tpffile can be
-    generated by jcvi.formats.agp.tpf().
+    if opts.ymax:
+        ax.set_ylim(0, opts.ymax)
 
-    North chr1 2 0 AC229737.8 telomere 58443
-    South chr1 2 1 AC229737.8 AC202463.29 58443 37835 58443 + Non-terminal
+    plt.subplots_adjust(hspace=0.5)
 
-    Each line describes a relationship between the current BAC and the
-    north/south BAC. First, "North/South" tag, then the chromosome, phases of
-    the two BACs, ids of the two BACs, the size and the overlap start-stop of
-    the CURRENT BAC, and orientation. Each BAC will have two lines in the
-    certificate file.
-    """
-    p = OptionParser(certificate.__doc__)
-    opts, args = p.parse_args(args)
+    image_name = chr + "." + iopts.format
+    savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
-    if len(args) != 2:
-        sys.exit(not p.print_help())
 
-    tpffile, certificatefile = args
-    fastadir = "fasta"
+def draw_heatmaps(
+    fig,
+    root,
+    root_extent: Extent,
+    fastafile: str,
+    chr: str,
+    stacks: List[str],
+    heatmaps: List[str],
+    window: int,
+    shift: int,
+    cmap: Colormap,
+    subtract: Optional[int] = None,
+    merge: bool = False,
+    meres: Optional[str] = None,
+):
+    """
+    Draw heatmap for the given chromosome.
+    """
+    stackbeds = get_beds(stacks)
+    heatmapbeds = get_beds(heatmaps)
+    stackbins = get_binfiles(
+        stackbeds, fastafile, shift, subtract=subtract, merge=merge
+    )
+    heatmapbins = get_binfiles(
+        heatmapbeds, fastafile, shift, subtract=subtract, merge=merge
+    )
 
-    tpf = TPF(tpffile)
+    margin = 0.06
+    inner = 0.015
+    clen = Sizes(fastafile).mapping[chr]
+
+    # Gauge
+    ratio = draw_gauge(root, margin, clen, rightmargin=4 * margin)
+    yinterval = 0.3
+    xx = margin
+    yy = 1 - margin
+    yy -= yinterval
+    xlen = clen / ratio
+    cc = chr
+    if "_" in chr:
+        ca, cb = chr.split("_")
+        cc = ca[0].upper() + cb
+
+    root.add_patch(Rectangle((xx, yy), xlen, yinterval - inner, color=gray))
+    extent = (xx, yy, xlen, yinterval - inner)
+    adjusted = adjust_extent(extent, root_extent)
+    ax = fig.add_axes(adjusted)
+
+    nbins, _ = get_nbins(clen, shift)
+
+    owindow = clen / 100
+    if owindow > window:
+        window = owindow // shift * shift
+
+    stackplot(ax, stackbins, nbins, palette, chr, window, shift)
+    ax.text(
+        0.05,
+        0.9,
+        cc,
+        va="top",
+        zorder=100,
+        transform=ax.transAxes,
+        bbox=dict(boxstyle="round", fc="w", alpha=0.5),
+    )
 
-    data = check_certificate(certificatefile)
-    fw = must_open(certificatefile, "w")
-    for i, a in enumerate(tpf):
-        if a.is_gap:
-            continue
+    # Legends
+    xx += xlen + 0.01
+    yspace = (yinterval - inner) / (len(stackbins) + 1)
+    yy = 1 - margin - yinterval
+    for s, p in zip(stacks, palette):
+        s = s.replace("_", " ")
+        s = Registration.get(s, s)
+
+        yy += yspace
+        root.add_patch(Rectangle((xx, yy), inner, inner, color=p, lw=0))
+        root.text(xx + 1.5 * inner, yy, s, size=10)
+
+    yh = 0.05  # Heatmap height
+    # Heatmaps
+    xx = margin
+    yy = 1 - margin - yinterval - inner
+    for s, p in zip(heatmaps, heatmapbins):
+        s = s.replace("_", " ")
+        s = Registration.get(s, s)
+
+        yy -= yh
+        m = stackarray(p, chr, window, shift)
+
+        Y = np.array([m, m])
+        root.imshow(
+            Y,
+            extent=(xx, xx + xlen, yy, yy + yh - inner),
+            interpolation="nearest",
+            aspect="auto",
+            cmap=cmap,
+        )
+        root.text(xx + xlen + 0.01, yy, s, size=10)
 
-        aid = a.component_id
+    yy -= yh
 
-        af = op.join(fastadir, aid + ".fasta")
-        if not op.exists(af):  # Check to avoid redownload
-            entrez([aid, "--skipcheck", "--outdir=" + fastadir])
-
-        north, south = tpf.getNorthSouthClone(i)
-        aphase, asize = phase(aid)
-
-        for tag, p in (("North", north), ("South", south)):
-            if not p:  # end of the chromosome
-                ov = "telomere\t{0}".format(asize)
-            elif p.isCloneGap:
-                bphase = "0"
-                ov = "{0}\t{1}".format(p.gap_type, asize)
-            else:
-                bid = p.component_id
-                bphase, bsize = phase(bid)
-                key = (tag, aid, bid)
-                if key in data:
-                    print(data[key], file=fw)
-                    continue
+    if meres:
+        bed = Bed(meres)
+        for b in bed:
+            if b.seqid != chr:
+                continue
+            pos = (b.start + b.end) / 2
+            cpos = pos / ratio
+            xx = margin + cpos
+            accn = b.accn.capitalize()
+            root.add_patch(CirclePolygon((xx, yy), radius=0.01, fc="m", ec="m"))
+            root.text(xx + 0.014, yy, accn, va="center", color="m")
 
-                ar = [aid, bid, "--dir=" + fastadir]
-                o = overlap(ar)
-                ov = o.certificateline if o else "{0}\t{1}\tNone".format(bid, asize)
-
-            print(
-                "\t".join(str(x) for x in (tag, a.object, aphase, bphase, aid, ov)),
-                file=fw,
-            )
-            fw.flush()
+    normalize_axes(root)
 
 
-def neighbor(args):
+def heatmap(args):
     """
-    %prog neighbor agpfile componentID
+    %prog heatmap fastafile chr1
 
-    Check overlaps of a particular component in agpfile.
+    Combine stack plot with heatmap to show abundance of various tracks along
+    given chromosome. Need to give multiple beds to --stacks and --heatmaps
     """
-    p = OptionParser(neighbor.__doc__)
-    opts, args = p.parse_args(args)
+    p = OptionParser(heatmap.__doc__)
+    p.add_option(
+        "--stacks",
+        default="Exons,Introns,DNA_transposons,Retrotransposons",
+        help="Features to plot in stackplot",
+    )
+    p.add_option(
+        "--heatmaps",
+        default="Copia,Gypsy,hAT,Helitron,Introns,Exons",
+        help="Features to plot in heatmaps",
+    )
+    p.add_option("--meres", default=None, help="Extra centromere / telomere features")
+    add_window_options(p)
+    opts, args, iopts = p.set_image_options(args, figsize="8x5")
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
-    agpfile, componentID = args
-    fastadir = "fasta"
+    fastafile, chr = args
+    window, shift, subtract, merge = check_window_options(opts)
 
-    cmd = "grep"
-    cmd += " --color -C2 {0} {1}".format(componentID, agpfile)
-    sh(cmd)
-
-    agp = AGP(agpfile)
-    aorder = agp.order
-    if componentID not in aorder:
-        print(
-            "Record {0} not present in `{1}`.".format(componentID, agpfile),
-            file=sys.stderr,
-        )
-        return
+    stacks = opts.stacks.split(",")
+    heatmaps = opts.heatmaps.split(",")
 
-    i, c = aorder[componentID]
-    north, south = agp.getNorthSouthClone(i)
-
-    if not north.isCloneGap:
-        ar = [north.component_id, componentID, "--dir=" + fastadir]
-        if north.orientation == "-":
-            ar += ["--qreverse"]
-        overlap(ar)
+    fig = plt.figure(1, (iopts.w, iopts.h))
+    root_extent = (0, 0, 1, 1)
+    root = fig.add_axes(root_extent)
+
+    draw_heatmaps(
+        fig,
+        root,
+        root_extent,
+        fastafile,
+        chr,
+        stacks,
+        heatmaps,
+        window,
+        shift,
+        iopts.cmap,
+        subtract,
+        merge,
+        meres=opts.meres,
+    )
 
-    if not south.isCloneGap:
-        ar = [componentID, south.component_id, "--dir=" + fastadir]
-        if c.orientation == "-":
-            ar += ["--qreverse"]
-        overlap(ar)
+    image_name = chr + "." + iopts.format
+    savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
-def agp(args):
+def draw_gauge(ax, margin: float, maxl: int, rightmargin: Optional[float] = None):
     """
-    %prog agp tpffile certificatefile agpfile
-
-    Build agpfile from overlap certificates.
+    Draw a gauge on the top of the canvas, showing the scale of the chromosome.
+    """
+    rightmargin = rightmargin or margin
+    ax.plot([margin, 1 - rightmargin], [1 - margin, 1 - margin], "k-", lw=2)
+
+    best_stride = autoscale(maxl)
+    nintervals = maxl / best_stride
+
+    xx, yy = margin, 1 - margin
+    tip = 0.005
+    xinterval = (1 - margin - rightmargin) / nintervals
+    l = human_size(best_stride)
+    if l[-1] == "b":
+        suffix = target = l[-2:]
+
+    for i in range(0, maxl + 1, best_stride):
+        l = human_size(i, precision=0, target=target)
+        if l[-1] == "b":
+            l, suffix = l[:-2], l[-2:]
+        ax.plot([xx, xx], [yy, yy + tip], "k-", lw=2)
+        ax.text(xx, yy + 2 * tip, l, ha="center", size=13)
+        xx += xinterval
+
+    xx += 4 * tip - xinterval
+    ax.text(xx + tip, yy + 2 * tip, suffix)
+
+    return best_stride / xinterval
+
+
+def get_binfiles(
+    inputfiles: List[str],
+    fastafile: str,
+    shift: int,
+    mode: str = "span",
+    subtract: Optional[int] = None,
+    binned: bool = False,
+    merge: bool = True,
+):
+    """
+    Get binfiles from input files. If not binned, then bin them first.
+    """
+    if not binned:
+        binopts = [f"--binsize={shift}"]
+        binopts.append(f"--mode={mode}")
+        if subtract:
+            binopts.append(f"--subtract={subtract}")
+        if not merge:
+            binopts.append("--nomerge")
+        binfiles = [bins([x, fastafile] + binopts) for x in inputfiles if op.exists(x)]
+    else:
+        binfiles = inputfiles
+    binfiles = [BinFile(x) for x in binfiles]
+
+    return binfiles
+
+
+def stackarray(binfile: BinFile, chr: str, window: int, shift: int):
+    """
+    Get stack array from binfile for the given chr.
+    """
+    mn = binfile.mapping[chr]
+    m, n = zip(*mn)
+
+    m = np.array(m, dtype="float")
+    n = np.array(n, dtype="float")
+
+    w = window // shift
+    m = moving_sum(m, window=w)
+    n = moving_sum(n, window=w)
+    m /= n
+
+    return m
+
+
+def stackplot(
+    ax,
+    binfiles: List[BinFile],
+    nbins: int,
+    palette: List[str],
+    chr: str,
+    window: int,
+    shift: int,
+):
+    """
+    Plot stackplot on the given axes, using data from binfiles.
+    """
+    t = np.arange(nbins, dtype="float") + 0.5
+    m = np.zeros(nbins, dtype="float")
+    zorders = range(10)[::-1]
+    for binfile, p, z in zip(binfiles, palette, zorders):
+        s = stackarray(binfile, chr, window, shift)
+        m += s
+        ax.fill_between(t, m, color=p, lw=0, zorder=z)
+
+    ax.set_xlim(0, nbins)
+    ax.set_ylim(0, 1)
+    ax.set_axis_off()
+
+
+def draw_stacks(
+    fig,
+    root,
+    root_extent: Extent,
+    stacks: List[str],
+    fastafile: str,
+    window: int,
+    shift: int,
+    top: int,
+    merge: bool = True,
+    subtract: Optional[int] = None,
+    switch: Optional[DictFile] = None,
+):
+    """
+    Draw stack plot.
+    """
+    bedfiles = get_beds(stacks)
+    binfiles = get_binfiles(bedfiles, fastafile, shift, subtract=subtract, merge=merge)
+
+    sizes = Sizes(fastafile)
+    s = list(sizes.iter_sizes())[:top]
+    maxl = max(x[1] for x in s)
+    margin = 0.08
+    inner = 0.02  # y distance between tracks
+
+    # Gauge
+    ratio = draw_gauge(root, margin, maxl)
+
+    # Per chromosome
+    yinterval = (1 - 2 * margin) / (top + 1)
+    xx = margin
+    yy = 1 - margin
+    for chr, clen in s:
+        yy -= yinterval
+        xlen = clen / ratio
+        cc = chr
+        if "_" in chr:
+            ca, cb = chr.split("_")
+            cc = ca[0].upper() + cb
+
+        if switch and cc in switch:
+            cc = "\n".join((cc, f"({switch[cc]})"))
+
+        extent = (xx, yy, xlen, yinterval - inner)
+        adjusted = adjust_extent(extent, root_extent)
+        root.add_patch(Rectangle((xx, yy), xlen, yinterval - inner, color=gray))
+        ax = fig.add_axes(adjusted)
+
+        nbins, _ = get_nbins(clen, shift)
+
+        stackplot(ax, binfiles, nbins, palette, chr, window, shift)
+        root.text(
+            xx - 0.04, yy + 0.5 * (yinterval - inner), cc, ha="center", va="center"
+        )
 
-    Tiling Path File (tpf) is a file that lists the component and the gaps.
-    It is a three-column file similar to below, also see jcvi.formats.agp.tpf():
+    # Legends
+    yy -= yinterval
+    xx = margin
+    for b, p in zip(bedfiles, palette):
+        b = b.rsplit(".", 1)[0].replace("_", " ")
+        b = Registration.get(b, b)
 
-    telomere    chr1 na
-    AC229737.8  chr1 +
-    AC202463.29 chr1 +
+        root.add_patch(Rectangle((xx, yy), inner, inner, color=p, lw=0))
+        xx += 2 * inner
+        root.text(xx, yy, b, size=13)
+        xx += len(b) * 0.015 + inner
 
-    Note: the orientation of the component is only used as a guide. If the
-    orientation is derivable from a terminal overlap, it will use it regardless
-    of what the tpf says.
+    normalize_axes(root)
 
-    See jcvi.assembly.goldenpath.certificate() which generates a list of
-    certificates based on agpfile. At first, it seems counter-productive to
-    convert first agp to certificates then certificates back to agp.
 
-    The certificates provide a way to edit the overlap information, so that the
-    agpfile can be corrected (without changing agpfile directly).
+def stack(args):
     """
-    from jcvi.formats.base import DictFile
+    %prog stack fastafile
 
-    p = OptionParser(agp.__doc__)
-    opts, args = p.parse_args(args)
+    Create landscape plots that show the amounts of genic sequences, and repetitive
+    sequences along the chromosomes.
+    """
+    p = OptionParser(stack.__doc__)
+    p.add_option("--top", default=10, type="int", help="Draw the first N chromosomes")
+    p.add_option(
+        "--stacks",
+        default="Exons,Introns,DNA_transposons,Retrotransposons",
+        help="Features to plot in stackplot",
+    )
+    p.add_option("--switch", help="Change chr names based on two-column file")
+    add_window_options(p)
+    opts, args, iopts = p.set_image_options(args, figsize="8x8")
 
-    if len(args) != 3:
+    if len(args) != 1:
         sys.exit(not p.print_help())
 
-    tpffile, certificatefile, agpfile = args
-    orientationguide = DictFile(tpffile, valuepos=2)
-    cert = Certificate(certificatefile)
-    cert.write_AGP(agpfile, orientationguide=orientationguide)
+    (fastafile,) = args
+    top = opts.top
+    window, shift, subtract, merge = check_window_options(opts)
+    switch = opts.switch
+    if switch:
+        switch = DictFile(opts.switch)
+
+    stacks = opts.stacks.split(",")
+
+    fig = plt.figure(1, (iopts.w, iopts.h))
+    root_extent = (0, 0, 1, 1)
+    root = fig.add_axes(root_extent)
+
+    draw_stacks(
+        fig,
+        root,
+        root_extent,
+        stacks,
+        fastafile,
+        window,
+        shift,
+        top,
+        merge,
+        subtract,
+        switch,
+    )
+
+    pf = fastafile.rsplit(".", 1)[0]
+    image_name = pf + "." + iopts.format
+    savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jcvi-1.4.5/jcvi/assembly/hic.py` & `jcvi-1.4.6/jcvi/assembly/hic.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/assembly/kmer.py` & `jcvi-1.4.6/jcvi/assembly/kmer.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/assembly/opticalmap.py` & `jcvi-1.4.6/jcvi/assembly/opticalmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/assembly/patch.py` & `jcvi-1.4.6/jcvi/assembly/patch.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/assembly/postprocess.py` & `jcvi-1.4.6/jcvi/assembly/postprocess.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/assembly/preprocess.py` & `jcvi-1.4.6/jcvi/assembly/preprocess.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 
 """
 Wrapper to trim and correct sequence data.
 """
 import os
 import os.path as op
 import sys
-import logging
 
-from jcvi.formats.base import BaseFile, write_file, must_open
-from jcvi.formats.fastq import guessoffset
-from jcvi.utils.cbook import depends, human_size
-from jcvi.apps.base import (
+from ..apps.base import (
     OptionParser,
     ActionDispatcher,
     cleanup,
+    datadir,
     download,
-    sh,
+    logger,
     mkdir,
     need_update,
-    datadir,
+    sh,
 )
+from ..formats.base import BaseFile, must_open, write_file
+from ..formats.fastq import guessoffset
+from ..utils.cbook import depends, human_size
 
 
 class FastQCdata(BaseFile, dict):
     def __init__(self, filename, human=False):
         super(FastQCdata, self).__init__(filename)
         if not op.exists(filename):
-            logging.debug("File `{0}` not found.".format(filename))
+            logger.debug("File `%s` not found.", filename)
             # Sample_RF37-1/RF37-1_GATCAG_L008_R2_fastqc =>
             # RF37-1_GATCAG_L008_R2
             self["Filename"] = op.basename(op.split(filename)[0]).rsplit("_", 1)[0]
             self["Total Sequences"] = self["Sequence length"] = self["Total Bases"] = (
                 "na"
             )
             return
@@ -62,22 +62,21 @@
         self["Total Sequences"] = human_size(ts).rstrip("b") if human else ts
         self["Total Bases"] = human_size(tb).rstrip("b") if human else tb
 
 
 def main():
 
     actions = (
-        ("count", "count reads based on FASTQC results"),
-        ("trim", "trim reads using TRIMMOMATIC"),
-        ("correct", "correct reads using ALLPATHS-LG"),
-        ("hetsmooth", "reduce K-mer diversity using het-smooth"),
-        ("alignextend", "increase read length by extending based on alignments"),
         ("contamination", "check reads contamination against Ecoli"),
+        ("correct", "correct reads using ALLPATHS-LG"),
+        ("count", "count reads based on FASTQC results"),
         ("diginorm", "run K-mer based normalization"),
         ("expand", "expand sequences using short reads"),
+        ("hetsmooth", "reduce K-mer diversity using het-smooth"),
+        ("trim", "trim reads using TRIMMOMATIC"),
     )
     p = ActionDispatcher(actions)
     p.dispatch(globals())
 
 
 def diginorm(args):
     """
@@ -201,15 +200,15 @@
 
     # Attract reads
     samfile, logfile = align(
         [bes, reads, "--reorder", "--mapped", "--firstN={0}".format(opts.firstN)]
     )
 
     samfile, mapped, _ = get_samfile(reads, bes, bowtie=True, mapped=True)
-    logging.debug("Extract first {0} reads from `{1}`.".format(nreads, mapped))
+    logger.debug("Extract first %d reads from `%s`.", nreads, mapped)
 
     pf = mapped.split(".")[0]
     pf = pf.split("-")[0]
     bespf = bes.split(".")[0]
     reads = pf + ".expand.fastq"
     first([str(nreads), mapped, "-o", reads])
 
@@ -248,17 +247,15 @@
         recs.append((keys.index(subject), rid, rec))
 
     recs = [x[-1] for x in sorted(recs)]
     SeqIO.write(recs, fw, "fasta")
     fw.close()
 
     cleanup(samfile, logfile, mapped, reads, fastafile, qualfile, blastfile, pf)
-    logging.debug(
-        "Annotated seqs (n={0}) written to `{1}`.".format(len(recs), annotatedfasta)
-    )
+    logger.debug("Annotated seqs (n=%d) written to `%s`.", len(recs), annotatedfasta)
 
     return annotatedfasta
 
 
 def contamination(args):
     """
     %prog contamination Ecoli.fasta genome.fasta read.fastq
@@ -298,76 +295,14 @@
     print(
         "{0}: Ecoli contamination rate {1}-{2}".format(fq, lowerbound, upperbound),
         file=sys.stderr,
     )
     fw.close()
 
 
-def alignextend(args):
-    """
-    %prog alignextend ref.fasta read.1.fastq read.2.fastq
-
-    Wrapper around AMOS alignextend.
-    """
-    choices = "prepare,align,filter,rmdup,genreads".split(",")
-    p = OptionParser(alignextend.__doc__)
-    p.add_option(
-        "--nosuffix",
-        default=False,
-        action="store_true",
-        help="Do not add /1/2 suffix to the read",
-    )
-    p.add_option(
-        "--rc",
-        default=False,
-        action="store_true",
-        help="Reverse complement the reads before alignment",
-    )
-    p.add_option("--len", default=100, type="int", help="Extend to this length")
-    p.add_option(
-        "--stage", default="prepare", choices=choices, help="Start from certain stage"
-    )
-    p.add_option(
-        "--dup",
-        default=10,
-        type="int",
-        help="Filter duplicates with coordinates within this distance",
-    )
-    p.add_option(
-        "--maxdiff", default=1, type="int", help="Maximum number of differences"
-    )
-    p.set_home("amos")
-    p.set_cpus()
-    opts, args = p.parse_args(args)
-
-    if len(args) != 3:
-        sys.exit(not p.print_help())
-
-    ref, r1, r2 = args
-    pf = op.basename(r1).split(".")[0]
-    cmd = op.join(opts.amos_home, "src/Experimental/alignextend.pl")
-    if not opts.nosuffix:
-        cmd += " -suffix"
-    bwa_idx = "{0}.ref.fa.sa".format(pf)
-    if not need_update(ref, bwa_idx):
-        cmd += " -noindex"
-    cmd += " -threads {0}".format(opts.cpus)
-    offset = guessoffset([r1])
-    if offset == 64:
-        cmd += " -I"
-    if opts.rc:
-        cmd += " -rc"
-    cmd += " -allow -len {0} -dup {1}".format(opts.len, opts.dup)
-    cmd += " -min {0} -max {1}".format(2 * opts.len, 20 * opts.len)
-    cmd += " -maxdiff {0}".format(opts.maxdiff)
-    cmd += " -stage {0}".format(opts.stage)
-    cmd += " ".join(("", pf, ref, r1, r2))
-    sh(cmd)
-
-
 def count(args):
     """
     %prog count *.gz
 
     Count reads based on FASTQC results. FASTQC needs to be run on all the input
     data given before running this command.
     """
```

### Comparing `jcvi-1.4.5/jcvi/assembly/sim.py` & `jcvi-1.4.6/jcvi/assembly/sim.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/assembly/soap.py` & `jcvi-1.4.6/jcvi/assembly/soap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/assembly/syntenypath.py` & `jcvi-1.4.6/jcvi/assembly/syntenypath.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/assembly/trinity.py` & `jcvi-1.4.6/jcvi/annotation/trinity.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/compara/base.py` & `jcvi-1.4.6/jcvi/compara/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/compara/blastfilter.py` & `jcvi-1.4.6/jcvi/compara/blastfilter.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/compara/catalog.py` & `jcvi-1.4.6/jcvi/compara/catalog.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 import os.path as op
 import sys
-import logging
 import string
 
 from collections import defaultdict
 from itertools import product, combinations
 
-from jcvi.formats.blast import BlastLine
-from jcvi.formats.fasta import Fasta
-from jcvi.formats.bed import Bed
-from jcvi.formats.base import must_open, BaseFile
-from jcvi.utils.grouper import Grouper
-from jcvi.utils.cbook import gene_name
-from jcvi.apps.base import (
+from ..apps.base import (
+    ActionDispatcher,
     OptionParser,
     glob,
-    ActionDispatcher,
+    logger,
+    mkdir,
     need_update,
     sh,
-    mkdir,
 )
+from ..formats.base import must_open, BaseFile
+from ..formats.bed import Bed
+from ..formats.blast import BlastLine
+from ..formats.fasta import Fasta
+from ..utils.cbook import gene_name
+from ..utils.grouper import Grouper
+
 from .base import AnchorFile
 from .synteny import check_beds
 
 
 class OMGFile(BaseFile):
     def __init__(self, filename):
         super(OMGFile, self).__init__(filename)
@@ -142,33 +143,29 @@
     groups = Grouper()
 
     fp = open(groupsfile)
     for row in fp:
         members = row.strip().split(",")
         groups.join(*members)
 
-    logging.debug(
-        "Imported {0} families with {1} members.".format(
-            len(groups), groups.num_members
-        )
+    logger.debug(
+        "Imported %d families with %d members.", len(groups), groups.num_members
     )
 
     seen = set()
     omggroups = Grouper()
     fp = open(omgfile)
     for row in fp:
         genes, idxs = row.split()
         genes = genes.split(",")
         seen.update(genes)
         omggroups.join(*genes)
 
     nmembers = omggroups.num_members
-    logging.debug(
-        "Imported {0} OMG families with {1} members.".format(len(omggroups), nmembers)
-    )
+    logger.debug("Imported %d OMG families with %d members.", len(omggroups), nmembers)
     assert nmembers == len(seen)
 
     alltaxa = set(str(x) for x in range(ntaxa))
     recruited = []
     fp = open(omgfile)
     for row in fp:
         genes, idxs = row.split()
@@ -226,15 +223,15 @@
                     pgenes.append(g)
             genes = pgenes
 
         print("\t".join((",".join(genes), ",".join(idxs))))
         if not ghost:
             seen.update(best_addition)
 
-    logging.debug("Recruited {0} new genes.".format(len(recruited)))
+    logger.debug("Recruited %d new genes.", len(recruited))
 
 
 def pairwise_distance(a, b, threadorder):
     d = 0
     for x, y in zip(a, b)[:-1]:  # Last column not used
         x, y = x.strip("|"), y.strip("|")
         if "." in (x, y):
@@ -255,15 +252,15 @@
         if d < min_d:
             min_idx = i
             min_d = d
 
     i = min_idx
     t = threaded[i]
     threaded.insert(i, atoms)
-    logging.debug("Insert {0} before {1} (d={2})".format(atoms, t, min_d))
+    logger.debug("Insert %s before %s (d=%d)", atoms, t, min_d)
 
 
 def sort_layout(thread, listfile, column=0):
     """
     Sort the syntelog table according to chromomomal positions. First orient the
     contents against threadbed, then for contents not in threadbed, insert to
     the nearest neighbor.
@@ -284,28 +281,28 @@
         imported.add(accn)
         atoms = lt[accn]
         threaded.append(atoms)
 
     assert len(threaded) == len(imported)
 
     total = sum(1 for x in open(listfile))
-    logging.debug("Total: {0}, currently threaded: {1}".format(total, len(threaded)))
+    logger.debug("Total: %d, currently threaded: %d", total, len(threaded))
     fp = open(listfile)
     for row in fp:
         atoms = row.split()
         accn = atoms[0]
         if accn in imported:
             continue
         insert_into_threaded(atoms, threaded, threadorder)
 
     for atoms in threaded:
         print("\t".join(atoms), file=fw)
 
     fw.close()
-    logging.debug("File `{0}` sorted to `{1}`.".format(outfile, thread.filename))
+    logger.debug("File `%s` sorted to `%s`.", outfile, thread.filename)
 
 
 def layout(args):
     """
     %prog layout omgfile taxa
 
     Build column formatted gene lists after omgparse(). Use species list
@@ -351,15 +348,15 @@
     print(s, file=sys.stderr)
 
     fw.close()
     lastcolumn = ntaxa + 1
     cmd = "sort -k{0},{0} {1} -o {1}".format(lastcolumn, listfile)
     sh(cmd)
 
-    logging.debug("List file written to `{0}`.".format(listfile))
+    logger.debug("List file written to `%s`.", listfile)
     sort = opts.sort
     if sort:
         thread = Bed(sort)
         sort_layout(thread, listfile)
 
 
 def omgparse(args):
@@ -401,17 +398,15 @@
     anchorfiles = args
     groups = Grouper()
     for anchorfile in anchorfiles:
         ac = AnchorFile(anchorfile)
         for a, b, idx in ac.iter_pairs():
             groups.join(a, b)
 
-    logging.debug(
-        "Created {0} groups with {1} members.".format(len(groups), groups.num_members)
-    )
+    logger.debug("Created %d groups with %d members.", len(groups), groups.num_members)
 
     outfile = opts.outfile
     fw = must_open(outfile, "w")
     for g in groups:
         print(",".join(sorted(g)), file=fw)
     fw.close()
 
@@ -494,15 +489,15 @@
 
         print(
             "\t".join(str(x) for x in (s.accn, chr, s.start, s.end, s.strand, idx, pd)),
             file=fwinfo,
         )
     fwinfo.close()
 
-    logging.debug("Update info file `{0}`.".format(infofile))
+    logger.debug("Update info file `%s`.", infofile)
 
     return infofile
 
 
 def omgprepare(args):
     """
     %prog omgprepare ploidy anchorsfile blastfile
@@ -542,15 +537,15 @@
     geneinfo(sbed, genomeidx, ploidy)
 
     pf = blastfile.rsplit(".", 1)[0]
     cscorefile = pf + ".cscore"
     cscore([blastfile, "-o", cscorefile, "--cutoff=0", "--pct"])
     ac = AnchorFile(anchorfile)
     pairs = set((a, b) for a, b, i in ac.iter_pairs())
-    logging.debug("Imported {0} pairs from `{1}`.".format(len(pairs), anchorfile))
+    logger.debug("Imported %d pairs from `%s`.", len(pairs), anchorfile)
 
     weightsfile = pf + ".weights"
     fp = open(cscorefile)
     fw = open(weightsfile, "w")
     npairs = 0
     for row in fp:
         a, b, c, pct = row.split()
@@ -565,15 +560,15 @@
                 continue
             c /= 10  # This severely penalizes RBH against synteny
 
         print("\t".join((a, b, str(c))), file=fw)
         npairs += 1
     fw.close()
 
-    logging.debug("Write {0} pairs to `{1}`.".format(npairs, weightsfile))
+    logger.debug("Write %d pairs to `%s`.", npairs, weightsfile)
 
 
 def make_ortholog(blocksfile, rbhfile, orthofile):
     from jcvi.formats.base import DictFile
 
     # Generate mapping both ways
     adict = DictFile(rbhfile)
@@ -588,15 +583,15 @@
         if b == ".":
             if a in adict:
                 b = adict[a]
                 nrecruited += 1
                 b += "'"
         print("\t".join((a, b)), file=fw)
 
-    logging.debug("Recruited {0} pairs from RBH.".format(nrecruited))
+    logger.debug("Recruited %d pairs from RBH.", nrecruited)
     fp.close()
     fw.close()
 
 
 def ortholog(args):
     """
     %prog ortholog species_a species_b
@@ -749,16 +744,16 @@
                 dargs += ["--no_strip_names"]
             if opts.liftover_dist:
                 dargs += ["--liftover_dist={}".format(opts.liftover_dist)]
             try:
                 scan(dargs)
             except ValueError as e:
                 if ignore_zero_anchor:
-                    logging.debug(f"{e}")
-                    logging.debug("Ignoring this error and continuing...")
+                    logger.debug(str(e))
+                    logger.debug("Ignoring this error and continuing...")
                     return
                 else:
                     raise ValueError(e)
         if quota:
             quota_main([lifted_anchors, "--quota={0}".format(quota), "--screen"])
         if need_update(anchors, pdf, warn=True) and not opts.no_dotplot:
             from jcvi.graphics.dotplot import dotplot_main
```

### Comparing `jcvi-1.4.5/jcvi/compara/fractionation.py` & `jcvi-1.4.6/jcvi/compara/fractionation.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/compara/ks.py` & `jcvi-1.4.6/jcvi/compara/ks.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/compara/pad.py` & `jcvi-1.4.6/jcvi/compara/pad.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/compara/pedigree.py` & `jcvi-1.4.6/jcvi/compara/pedigree.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/compara/phylogeny.py` & `jcvi-1.4.6/jcvi/compara/phylogeny.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/compara/quota.py` & `jcvi-1.4.6/jcvi/compara/quota.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/compara/reconstruct.py` & `jcvi-1.4.6/jcvi/compara/reconstruct.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/compara/synfind.py` & `jcvi-1.4.6/jcvi/compara/synfind.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/compara/synteny.py` & `jcvi-1.4.6/jcvi/compara/synteny.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/formats/agp.py` & `jcvi-1.4.6/jcvi/formats/agp.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/formats/base.py` & `jcvi-1.4.6/jcvi/formats/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import os
 import os.path as op
 import math
 import sys
 
 from collections import OrderedDict
-from itertools import groupby, islice, cycle
+from itertools import cycle, groupby, islice
 
 from Bio import SeqIO
 from ..apps.base import (
     OptionParser,
     ActionDispatcher,
     cleanup,
     logger,
@@ -333,15 +333,21 @@
 
 def timestamp():
     from datetime import datetime as dt
 
     return "{0}{1:02d}{2:02d}".format(dt.now().year, dt.now().month, dt.now().day)
 
 
-def must_open(filename, mode="r", checkexists=False, skipcheck=False, oappend=False):
+def must_open(
+    filename: str,
+    mode: str = "r",
+    checkexists: bool = False,
+    skipcheck: bool = False,
+    oappend: bool = False,
+):
     """
     Accepts filename and returns filehandle.
 
     Checks on multiple files, stdin/stdout/stderr, .gz or .bz2 file.
     """
     if isinstance(filename, list):
         assert "r" in mode
@@ -381,15 +387,15 @@
         if "r" in mode:
             fp = gzip.open(filename, mode + "t")
         elif "w" in mode:
             fp = gzip.open(filename, mode)
 
     elif filename.endswith(".bz2"):
         if "r" in mode:
-            cmd = "bzcat {0}".format(filename)
+            cmd = f"bzcat {filename}"
             fp = popen(cmd, debug=False)
         elif "w" in mode:
             import bz2
 
             fp = bz2.BZ2File(filename, mode)
 
     else:
```

### Comparing `jcvi-1.4.5/jcvi/formats/bed.py` & `jcvi-1.4.6/jcvi/formats/bed.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 """
 Classes to handle the .bed files
 """
 
-import logging
 import math
-import numpy as np
 import os
 import os.path as op
 import shutil
 import sys
 
 from collections import defaultdict, OrderedDict
 from itertools import groupby
-from typing import Optional
+from typing import Optional, Tuple
+
+import numpy as np
 
 from more_itertools import pairwise
 from natsort import natsorted, natsort_key
 
-from jcvi.formats.base import DictFile, LineFile, must_open, is_number, get_number
-from jcvi.formats.sizes import Sizes
-from jcvi.utils.cbook import SummaryStats, thousands, percentage
-from jcvi.utils.grouper import Grouper
-from jcvi.utils.range import (
-    Range,
-    range_union,
-    range_chain,
-    range_distance,
-    range_intersect,
-)
-from jcvi.apps.base import (
+from ..apps.base import (
     OptionParser,
     ActionDispatcher,
     cleanup,
+    logger,
     need_update,
     popen,
     sh,
 )
+from ..utils.cbook import SummaryStats, thousands, percentage
+from ..utils.grouper import Grouper
+from ..utils.range import (
+    Range,
+    range_union,
+    range_chain,
+    range_distance,
+    range_intersect,
+)
+
+from .base import DictFile, LineFile, get_number, is_number, must_open
+from .sizes import Sizes
 
 
 class BedLine(object):
     # the Bed format supports more columns. we only need
     # the first 4, but keep the information in 'extra'.
     __slots__ = (
         "seqid",
@@ -129,15 +131,15 @@
                 source,
                 type,
                 str(self.start),
                 str(self.end),
                 score,
                 strand,
                 ".",
-                "ID=" + self.accn,
+                f"ID={self.accn}",
             )
         )
         return row
 
 
 class Bed(LineFile):
     def __init__(self, filename=None, key=None, sorted=True, juncs=False, include=None):
@@ -172,15 +174,15 @@
     def print_to_file(self, filename="stdout", sorted=False):
         if sorted:
             self.sort(key=self.key)
 
         fw = must_open(filename, "w")
         for b in self:
             if b.start < 1:
-                logging.error("Start < 1. Reset start for `{0}`.".format(b.accn))
+                logger.error("Start < 1. Reset start for `%s`.", b.accn)
                 b.start = 1
             print(b, file=fw)
         fw.close()
 
     def sum(self, seqid=None, unique=True):
         return bed_sum(self, seqid=seqid, unique=unique)
 
@@ -446,48 +448,46 @@
     unique_sum = range_union(ranges)
     raw_sum = sum(x.span for x in beds)
     return unique_sum if unique else raw_sum
 
 
 def main():
     actions = (
-        ("depth", "calculate average depth per feature using coverageBed"),
-        ("mergebydepth", "returns union of features beyond certain depth"),
-        ("sort", "sort bed file"),
-        ("merge", "merge bed files"),
-        ("index", "index bed file using tabix"),
-        ("bins", "bin bed lengths into each window"),
-        ("summary", "summarize the lengths of the intervals"),
-        ("evaluate", "make truth table and calculate sensitivity and specificity"),
-        ("pile", "find the ids that intersect"),
-        ("pairs", "estimate insert size between paired reads from bedfile"),
-        ("mates", "print paired reads from bedfile"),
-        ("sizes", "infer the sizes for each seqid"),
-        ("uniq", "remove overlapping features with higher scores"),
-        ("longest", "select longest feature within overlapping piles"),
         ("bedpe", "convert to bedpe format"),
+        ("bins", "bin bed lengths into each window"),
+        ("chain", "chain bed segments together"),
+        ("closest", "find closest BED feature"),
+        ("density", "calculates density of features per seqid"),
+        ("depth", "calculate average depth per feature using coverageBed"),
         ("distance", "calculate distance between bed features"),
-        ("sample", "sample bed file and remove high-coverage regions"),
-        ("refine", "refine bed file using a second bed file"),
-        ("flanking", "get n flanking features for a given position"),
-        ("some", "get a subset of bed features given a list"),
-        ("fix", "fix non-standard bed files"),
+        ("evaluate", "make truth table and calculate sensitivity and specificity"),
         ("filter", "filter bedfile to retain records between size range"),
         ("filterbedgraph", "filter bedgraph to extract unique regions"),
-        ("random", "extract a random subset of features"),
+        ("fix", "fix non-standard bed files"),
+        ("flanking", "get n flanking features for a given position"),
+        ("format", "reformat BED file"),
+        ("gaps", "define gaps in BED file using complementBed"),
+        ("index", "index bed file using tabix"),
         ("juncs", "trim junctions.bed overhang to get intron, merge multiple beds"),
+        ("longest", "select longest feature within overlapping piles"),
+        ("mates", "print paired reads from bedfile"),
+        ("merge", "merge bed files"),
+        ("mergebydepth", "returns union of features beyond certain depth"),
+        ("pairs", "estimate insert size between paired reads from bedfile"),
+        ("pile", "find the ids that intersect"),
+        ("random", "extract a random subset of features"),
+        ("refine", "refine bed file using a second bed file"),
+        ("sample", "sample bed file and remove high-coverage regions"),
         ("seqids", "print out all seqids on one line"),
-        ("alignextend", "alignextend based on BEDPE and FASTA ref"),
-        ("clr", "extract clear range based on BEDPE"),
-        ("chain", "chain bed segments together"),
-        ("density", "calculates density of features per seqid"),
+        ("sizes", "infer the sizes for each seqid"),
+        ("some", "get a subset of bed features given a list"),
+        ("sort", "sort bed file"),
+        ("summary", "summarize the lengths of the intervals"),
         ("tiling", "compute the minimum tiling path"),
-        ("format", "reformat BED file"),
-        ("closest", "find closest BED feature"),
-        ("gaps", "define gaps in BED file using complementBed"),
+        ("uniq", "remove overlapping features with higher scores"),
     )
     p = ActionDispatcher(actions)
     p.dispatch(globals())
 
 
 def gaps(args):
     """
@@ -538,15 +538,15 @@
         miss = "_".join(na_in - set([seqid]))
         if miss:
             gap_name += f"_na_in_{miss}"
         print("\t".join((seqid, start, end, gap_name)), file=fw)
         n_gaps += 1
     for seqid, gap_sizes in all_gaps.items():
         total_gap_size = sum(gap_sizes)
-        logging.debug(
+        logger.debug(
             "Total gaps in %s: %d, %s",
             seqid,
             len(gap_sizes),
             percentage(total_gap_size, ref_sizes[seqid]),
         )
 
 
@@ -618,15 +618,15 @@
     """
     %prog filterbedgraph a.bedgraph 1
 
     Filter the bedGraph, typically from the gem-mappability pipeline. Unique
     regions are 1, two copies .5, etc.
     """
     p = OptionParser(filterbedgraph.__doc__)
-    opts, args = p.parse_args(args)
+    _, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     bedgraphfile, cutoff = args
     c = float(cutoff)
     fp = open(bedgraphfile)
@@ -637,18 +637,19 @@
     for row in fp:
         b = BedLine(row)
         ntotal += 1
         if float(b.accn) >= c:
             print(b, file=fw)
             nfiltered += 1
     fw.close()
-    logging.debug(
-        "A total of {} intervals (score >= {}) written to `{}`".format(
-            percentage(nfiltered, ntotal), cutoff, filteredbed
-        )
+    logger.debug(
+        "A total of %s intervals (score >= %.2f) written to `%s`",
+        percentage(nfiltered, ntotal),
+        cutoff,
+        filteredbed,
     )
 
     mergeBed(filteredbed, sorted=True, delim=None)
 
 
 def tiling(args):
     """
@@ -722,18 +723,16 @@
                 print("\n".join(str(x) for x in gbed))
                 print("*" * 30)
                 print("\n".join(str(gbed[x]) for x in chain))
                 print()
 
     tilingbedfile = bedfile.rsplit(".", 1)[0] + ".tiling.bed"
     selected.print_to_file(filename=tilingbedfile, sorted=True)
-    logging.debug(
-        "A total of {} tiling features written to `{}`".format(
-            len(selected), tilingbedfile
-        )
+    logger.debug(
+        "A total of %d tiling features written to `%s`", len(selected), tilingbedfile
     )
 
 
 def chain(args):
     """
     %prog chain bedfile
 
@@ -777,15 +776,15 @@
 def density(args):
     """
     %prog density bedfile ref.fasta
 
     Calculates density of features per seqid.
     """
     p = OptionParser(density.__doc__)
-    opts, args = p.parse_args(args)
+    _, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     bedfile, fastafile = args
     bed = Bed(bedfile)
     sizes = Sizes(fastafile).mapping
@@ -794,80 +793,32 @@
     for seqid, bb in bed.sub_beds():
         nfeats = len(bb)
         size = sizes[seqid]
         ds = nfeats * 1e6 / size
         print("\t".join(str(x) for x in (seqid, nfeats, size, "{0:.1f}".format(ds))))
 
 
-def clr(args):
-    """
-    %prog clr [bamfile|bedpefile] ref.fasta
-
-    Use mates from BEDPE to extract ranges where the ref is covered by mates.
-    This is useful in detection of chimeric contigs.
-    """
-    p = OptionParser(clr.__doc__)
-    p.set_bedpe()
-    opts, args = p.parse_args(args)
-
-    if len(args) != 2:
-        sys.exit(not p.print_help())
-
-    bedpe, ref = args
-    if bedpe.endswith(".bam"):
-        bedpefile = bedpe.replace(".bam", ".bedpe")
-        if need_update(bedpe, bedpefile):
-            cmd = "bamToBed -bedpe -i {0}".format(bedpe)
-            sh(cmd, outfile=bedpefile)
-        bedpe = bedpefile
-
-    filtered = bedpe + ".filtered"
-    if need_update(bedpe, filtered):
-        filter_bedpe(
-            bedpe, filtered, ref, rc=opts.rc, minlen=opts.minlen, maxlen=opts.maxlen
-        )
-
-    rmdup = filtered + ".sorted.rmdup"
-    if need_update(filtered, rmdup):
-        rmdup_bedpe(filtered, rmdup, dupwiggle=opts.dup)
-
-    converted = rmdup + ".converted"
-    if need_update(rmdup, converted):
-        fp = open(rmdup)
-        fw = open(converted, "w")
-        for row in fp:
-            r = BedpeLine(row)
-            print(r.bedline, file=fw)
-        fw.close()
-
-    merged = converted + ".merge.bed"
-    if need_update(converted, merged):
-        mergeBed(converted)
-
-
 def sfa_to_fq(sfa, qvchar):
     fq = sfa.rsplit(".", 1)[0] + ".fq"
     fp = must_open(sfa)
     fw = must_open(fq, "w")
     total = 0
     for row in fp:
         total += 1
         name, seq = row.split()
         qual = len(seq) * qvchar
         print("\n".join(("@" + name, seq, "+", qual)), file=fw)
-    logging.debug("A total of {0} sequences written to `{1}`.".format(total, fq))
+    logger.debug("A total of %d sequences written to `%s`.", total, fq)
     return fq
 
 
 def filter_bedpe(bedpe, filtered, ref, rc=False, rlen=None, minlen=2000, maxlen=8000):
     tag = " after RC" if rc else ""
-    logging.debug(
-        "Filter criteria: innie{0}, {1} <= insertsize <= {2}".format(
-            tag, minlen, maxlen
-        )
+    logger.debug(
+        "Filter criteria: innie%s, %d <= insertsize <= %d", tag, minlen, maxlen
     )
     sizes = Sizes(ref).mapping
     fp = must_open(bedpe)
     fw = must_open(filtered, "w")
     retained = total = 0
     for row in fp:
         b = BedpeLine(row)
@@ -879,33 +830,31 @@
         b.score = b.outerdist
         if not minlen <= b.score <= maxlen:
             continue
         retained += 1
         if rlen:
             b.extend(rlen, sizes[b.seqid1])
         print(b, file=fw)
-    logging.debug(
-        "A total of {0} mates written to `{1}`.".format(
-            percentage(retained, total), filtered
-        )
+    logger.debug(
+        "A total of %d mates written to `%s`.", percentage(retained, total), filtered
     )
     fw.close()
 
 
 def rmdup_bedpe(filtered, rmdup, dupwiggle=10):
     sortedfiltered = filtered + ".sorted"
     if need_update(filtered, sortedfiltered):
         sh("sort -k1,1 -k2,2n -i {0} -o {1}".format(filtered, sortedfiltered))
 
-    logging.debug("Rmdup criteria: wiggle <= {0}".format(dupwiggle))
+    logger.debug("Rmdup criteria: wiggle <= %d", dupwiggle)
     fp = must_open(sortedfiltered)
     fw = must_open(rmdup, "w")
     data = [BedpeLine(x) for x in fp]
     retained = total = 0
-    for seqid, ss in groupby(data, key=lambda x: x.seqid1):
+    for _, ss in groupby(data, key=lambda x: x.seqid1):
         ss = list(ss)
         for i, a in enumerate(ss):
             if a.isdup:
                 continue
             for b in ss[i + 1 :]:
                 if b.start1 > a.start1 + dupwiggle:
                     break
@@ -918,87 +867,20 @@
                     b.isdup = True
         for a in ss:
             total += 1
             if a.isdup:
                 continue
             retained += 1
             print(a, file=fw)
-    logging.debug(
-        "A total of {0} mates written to `{1}`.".format(
-            percentage(retained, total), rmdup
-        )
+    logger.debug(
+        "A total of %s mates written to `%s`.", percentage(retained, total), rmdup
     )
     fw.close()
 
 
-def alignextend(args):
-    """
-    %prog alignextend bedpefile ref.fasta
-
-    Similar idea to alignextend, using mates from BEDPE and FASTA ref. See AMOS
-    script here:
-
-    https://github.com/nathanhaigh/amos/blob/master/src/Experimental/alignextend.pl
-    """
-    p = OptionParser(alignextend.__doc__)
-    p.add_option("--len", default=100, type="int", help="Extend to this length")
-    p.add_option(
-        "--qv", default=31, type="int", help="Dummy qv score for extended bases"
-    )
-    p.add_option(
-        "--bedonly",
-        default=False,
-        action="store_true",
-        help="Only generate bed files, no FASTA",
-    )
-    p.set_bedpe()
-    opts, args = p.parse_args(args)
-
-    if len(args) != 2:
-        sys.exit(not p.print_help())
-
-    bedpe, ref = args
-    qvchar = chr(opts.qv + 33)
-    pf = bedpe.split(".")[0]
-
-    filtered = bedpe + ".filtered"
-    if need_update(bedpe, filtered):
-        filter_bedpe(
-            bedpe,
-            filtered,
-            ref,
-            rc=opts.rc,
-            minlen=opts.minlen,
-            maxlen=opts.maxlen,
-            rlen=opts.rlen,
-        )
-
-    rmdup = filtered + ".filtered.sorted.rmdup"
-    if need_update(filtered, rmdup):
-        rmdup_bedpe(filtered, rmdup, dupwiggle=opts.dup)
-
-    if opts.bedonly:
-        return
-
-    bed1, bed2 = pf + ".1e.bed", pf + ".2e.bed"
-    if need_update(rmdup, (bed1, bed2)):
-        sh("cut -f1-3,7-9 {0}".format(rmdup), outfile=bed1)
-        sh("cut -f4-6,7-8,10 {0}".format(rmdup), outfile=bed2)
-
-    sfa1, sfa2 = pf + ".1e.sfa", pf + ".2e.sfa"
-    if need_update((bed1, bed2, ref), (sfa1, sfa2)):
-        for bed in (bed1, bed2):
-            fastaFromBed(bed, ref, name=True, tab=True, stranded=True)
-
-    fq1, fq2 = pf + ".1e.fq", pf + ".2e.fq"
-    if need_update((sfa1, sfa2), (fq1, fq2)):
-        for sfa in (sfa1, sfa2):
-            sfa_to_fq(sfa, qvchar)
-
-
 def seqids(args):
     """
     %prog seqids bedfile
 
     Print out all seqids on one line. Useful for graphics.karyotype.
     """
     p = OptionParser(seqids.__doc__)
@@ -1098,15 +980,15 @@
 
     beds = sample(b, NN)
     new_bed = Bed()
     new_bed.extend(beds)
 
     outfile = bedfile.rsplit(".", 1)[0] + ".{0}.bed".format(N)
     new_bed.print_to_file(outfile)
-    logging.debug("Write {0} features to `{1}`".format(NN, outfile))
+    logger.debug("Write %d features to `%s`", NN, outfile)
 
 
 def filter(args):
     """
     %prog filter bedfile
 
     Filter the bedfile to retain records between certain size range.
@@ -1150,16 +1032,16 @@
         if minaccn and int(b.accn) < minaccn:
             continue
         if minscore and int(b.score) < minscore:
             continue
         print(b, file=fw)
         keep.append(span)
 
-    logging.debug("Stats: {0} features kept.".format(percentage(len(keep), len(total))))
-    logging.debug("Stats: {0} bases kept.".format(percentage(sum(keep), sum(total))))
+    logger.debug("Stats: %s features kept.", percentage(len(keep), len(total)))
+    logger.debug("Stats: %s bases kept.", percentage(sum(keep), sum(total)))
 
 
 def make_bedgraph(bedfile, fastafile):
     sizesfile = Sizes(fastafile).filename
     pf = bedfile.rsplit(".", 1)[0]
     bedfile = sort([bedfile])
     bedgraph = pf + ".bedgraph"
@@ -1280,23 +1162,21 @@
             continue
         max_size, max_accn = max(accn_sizes)
         if max_size < minsize:
             continue
         ids.add(max_accn)
 
     newids = remove_isoforms(ids)
-    logging.debug("Remove isoforms: before={0} after={1}".format(len(ids), len(newids)))
+    logger.debug("Remove isoforms: before=%d after=%d", len(ids), len(newids))
 
     longestidsfile = pf + ".longest.ids"
     fw = open(longestidsfile, "w")
     print("\n".join(newids), file=fw)
     fw.close()
-    logging.debug(
-        "A total of {0} records written to `{1}`.".format(len(newids), longestidsfile)
-    )
+    logger.debug("A total of %d records written to `%s`.", len(newids), longestidsfile)
 
     longestbedfile = pf + ".longest.bed"
     some(
         [
             bedfile,
             longestidsfile,
             "--outfile={0}".format(longestbedfile),
@@ -1368,17 +1248,17 @@
         if b.span >= minspan:
             print(b, file=fw)
             nfiltered += 1
 
         ntotal += 1
 
     if nfixed:
-        logging.debug("Total fixed: {0}".format(percentage(nfixed, ntotal)))
+        logger.debug("Total fixed: %s".format(percentage(nfixed, ntotal)))
     if nfiltered:
-        logging.debug("Total filtered: {0}".format(percentage(nfiltered, ntotal)))
+        logger.debug("Total filtered: %s".format(percentage(nfiltered, ntotal)))
 
 
 def some(args):
     """
     %prog some bedfile idsfile > newbedfile
 
     Retrieve a subset of bed features given a list of ids.
@@ -1418,15 +1298,15 @@
             keep = not keep
 
         if keep:
             nkeep += 1
             print(b, file=fw)
 
     fw.close()
-    logging.debug("Stats: {0} features kept.".format(percentage(nkeep, ntotal)))
+    logger.debug("Stats: %s features kept.".format(percentage(nkeep, ntotal)))
 
 
 def uniq(args):
     """
     %prog uniq bedfile
 
     Remove overlapping features with higher scores.
@@ -1474,15 +1354,15 @@
 
     if notselected:
         leftoverfile = bedfile.split(".")[0] + ".leftover.bed"
         leftoverbed = Bed()
         leftoverbed.extend(notselected)
         leftoverbed.print_to_file(leftoverfile, sorted=True)
 
-    logging.debug("Imported: {0}, Exported: {1}".format(len(bed), len(newbed)))
+    logger.debug("Imported: %d, Exported: %d", len(bed), len(newbed))
 
     return uniqbedfile
 
 
 def subtractbins(binfile1, binfile2):
     from jcvi.graphics.landscape import BinFile
 
@@ -1501,22 +1381,31 @@
         print(a, file=fw)
 
     fw.close()
 
     return binfile1
 
 
+def get_nbins(clen: int, shift: int) -> Tuple[int, int]:
+    """
+    Get the number of bins for a given chromosome length and shift.
+    """
+    nbins, last_bin = divmod(clen, shift)
+    if last_bin:
+        nbins += 1
+    return nbins, last_bin
+
+
 def bins(args):
     """
     %prog bins bedfile fastafile
 
     Bin bed lengths into each consecutive window. Use --subtract to remove bases
     from window, e.g. --subtract gaps.bed ignores the gap sequences.
     """
-    from jcvi.formats.sizes import Sizes
 
     p = OptionParser(bins.__doc__)
     p.add_option("--binsize", default=100000, type="int", help="Size of the bins")
     p.add_option("--subtract", help="Subtract bases from window")
     p.add_option(
         "--mode",
         default="span",
@@ -1558,29 +1447,26 @@
     bedfile = sort([bedfile, "-i"])
 
     bed = Bed(bedfile)
     sbdict = dict(bed.sub_beds())
     for chr, chr_len in sorted(sizes.items()):
         chr_len = sizes[chr]
         subbeds = sbdict.get(chr, [])
-        nbins = chr_len / binsize
-        last_bin = chr_len % binsize
-        if last_bin:
-            nbins += 1
+        nbins, last_bin = get_nbins(chr_len, binsize)
 
         a = np.zeros(nbins)  # values
         b = np.zeros(nbins, dtype="int")  # bases
         c = np.zeros(nbins, dtype="int")  # count
         b[:-1] = binsize
         b[-1] = last_bin
 
         for bb in subbeds:
             start, end = bb.start, bb.end
-            startbin = start / binsize
-            endbin = end / binsize
+            startbin = start // binsize
+            endbin = end // binsize
 
             assert startbin <= endbin
             c[startbin : endbin + 1] += 1
 
             if mode == "score":
                 a[startbin : endbin + 1] += float(bb.score)
 
@@ -1634,15 +1520,15 @@
 
     ngroups = 0
     for group in groups:
         if len(group) > 1:
             ngroups += 1
             print("|".join(group))
 
-    logging.debug("A total of {0} piles (>= 2 members)".format(ngroups))
+    logger.debug("A total of %d piles (>= 2 members)", ngroups)
 
 
 def index(args):
     """
     %prog index bedfile
 
     Compress and index bedfile using `tabix`. Use --fasta to give a FASTA file
@@ -1714,15 +1600,15 @@
         bedfile = sort([bedfile, "-i"])
     cmd = "mergeBed -i {0}".format(bedfile)
     if d:
         cmd += " -d {0}".format(d)
     if nms:
         nargs = len(open(bedfile).readline().split())
         if nargs <= 3:
-            logging.debug("Only {0} columns detected... set nms=True".format(nargs))
+            logger.debug("Only %d columns detected... set nms=True", nargs)
         else:
             cmd += " -c 4 -o collapse"
     if s:
         cmd += " -s"
     if scores:
         valid_opts = (
             "sum",
@@ -1948,15 +1834,15 @@
         br = (b.seqid, b.start, b.end, "+")
         dist, oo = range_distance(ar, br, distmode=opts.distmode)
         total += 1
         if dist > 0:
             print(dist)
             valid += 1
 
-    logging.debug("Total valid (> 0) distances: {0}.".format(percentage(valid, total)))
+    logger.debug("Total valid (> 0) distances: %s.", percentage(valid, total))
 
 
 def sample(args):
     """
     %prog sample bedfile sizesfile
 
     Sample bed file and remove high-coverage regions.
@@ -2005,18 +1891,19 @@
         reverse = []
         bed.sort(key=lambda x: -x.end)
         for b in bed:
             if not reverse or abs(b.end - reverse[-1].end) >= raindrop:
                 reverse.append(b)
 
         for tag, L in zip(("forward", "reverse"), (forward, reverse)):
-            logging.debug(
-                "Selected {0} features in {1} direction, span: {2}".format(
-                    len(L), tag, sum(x.span for x in L)
-                )
+            logger.debug(
+                "Selected %d features in %s direction, span: %d",
+                len(L),
+                tag,
+                sum(x.span for x in L),
             )
 
         selected = Bed()
         selected.extend(set(forward + reverse))
         selected.print_to_file(opts.outfile, sorted=True)
         return
 
@@ -2028,15 +1915,15 @@
         nfeats = len(bed)
         nbases = bed.sum(unique=False)
         targetfeats = int(round(nfeats * targetsize / nbases))
         sub_bed = random.sample(bed, targetfeats)
         for b in sub_bed:
             print(b, file=fw)
 
-        logging.debug("File written to `%s`.", samplebed)
+        logger.debug("File written to `%s`.", samplebed)
         return
 
     c = Coverage(bedfile, sizesfile)
     coveragefile = c.filename
     samplecoveragefile = pf + ".sample.coverage"
     fw = open(samplecoveragefile, "w")
     fp = open(coveragefile)
@@ -2046,15 +1933,15 @@
         if cov <= opts.max:
             fw.write(row)
     fw.close()
 
     samplebedfile = pf + ".sample.bed"
     cmd = "intersectBed -a {0} -b {1} -wa -u".format(bedfile, samplecoveragefile)
     sh(cmd, outfile=samplebedfile)
-    logging.debug("Sampled bedfile written to `{0}`.".format(samplebedfile))
+    logger.debug("Sampled bedfile written to `%s`.", samplebedfile)
 
 
 def bedpe(args):
     """
     %prog bedpe bedfile
 
     Convert to bedpe format. Use --span to write another bed file that contain
@@ -2107,42 +1994,42 @@
     sizesfile = bedfile.rsplit(".", 1)[0] + ".sizes"
 
     fw = must_open(sizesfile, "w", checkexists=True, skipcheck=True)
     if fw:
         b = Bed(bedfile)
         for s, sbeds in b.sub_beds():
             print("{0}\t{1}".format(s, max(x.end for x in sbeds)), file=fw)
-        logging.debug("Sizes file written to `{0}`.".format(sizesfile))
+        logger.debug("Sizes file written to `%s`.", sizesfile)
 
     return sizesfile
 
 
 def analyze_dists(dists, cutoff=1000, alpha=0.1):
     """
     The dists can show bimodal distribution if they come from a mate-pair
     library. Assume bimodal distribution and then separate the two peaks. Based
     on the percentage in each peak, we can decide if it is indeed one peak or
     two peaks, and report the median respectively.
     """
     peak0 = [d for d in dists if d < cutoff]
     peak1 = [d for d in dists if d >= cutoff]
     c0, c1 = len(peak0), len(peak1)
-    logging.debug("Component counts: {0} {1}".format(c0, c1))
+    logger.debug("Component counts: %d %d", c0, c1)
     if c0 == 0 or c1 == 0 or float(c1) / len(dists) < alpha:
-        logging.debug(
-            "Single peak identified ({0} / {1} < {2})".format(c1, len(dists), alpha)
-        )
+        logger.debug("Single peak identified (%d / %d < %.1f)", c1, len(dists), alpha)
         return np.median(dists)
 
     peak0_median = np.median(peak0)
     peak1_median = np.median(peak1)
-    logging.debug(
-        "Dual peaks identified: {0}bp ({1}), {2}bp ({3}) (selected)".format(
-            int(peak0_median), c0, int(peak1_median), c1
-        )
+    logger.debug(
+        "Dual peaks identified: %dbp (%d), %dbp (%d) (selected)",
+        int(peak0_median),
+        c0,
+        int(peak1_median),
+        c1,
     )
 
     return peak1_median
 
 
 def report_pairs(
     data,
@@ -2211,18 +2098,15 @@
 
     # try to infer cutoff as twice the median until convergence
     if cutoff <= 0:
         dists = np.array([x[0] for x in all_dist], dtype="int")
         p0 = analyze_dists(dists, cutoff=mpcutoff)
         cutoff = int(2 * p0)  # initial estimate
         cutoff = int(math.ceil(cutoff / bins)) * bins
-        logging.debug(
-            "Insert size cutoff set to {0}, ".format(cutoff)
-            + "use '--cutoff' to override"
-        )
+        logger.debug("Insert size cutoff set to %d, use '--cutoff' to override", cutoff)
 
     for dist, orientation, aquery, bquery in all_dist:
         if dist > cutoff:
             continue
         if cutoff > 2 * mpcutoff and dist < mpcutoff:
             continue
 
@@ -2350,15 +2234,15 @@
     bs = BedSummary(bed)
     if opts.sizes:
         sizesfile = bedfile + ".sizes"
         fw = open(sizesfile, "w")
         for span, accn in bs.mspans:
             print(span, file=fw)
         fw.close()
-        logging.debug("Spans written to `{0}`.".format(sizesfile))
+        logger.debug("Spans written to `%s`.", sizesfile)
         return bs
 
     if not opts.all:
         bs.report()
         return bs
 
     for seqid, subbeds in bed.sub_beds():
@@ -2492,15 +2376,15 @@
         mindist = max(stats.mean - sv, 1)
         maxdist = stats.mean + sv
         print("\t".join(str(x) for x in ("library", pf, mindist, maxdist)), file=fw)
 
     num_fragments = num_pairs = 0
     matesbedfile = matesfile + ".bed"
     fwm = open(matesbedfile, "w")
-    for pe, lines in groupby(bed, key=key):
+    for _, lines in groupby(bed, key=key):
         lines = list(lines)
         if len(lines) != 2:
             num_fragments += len(lines)
             continue
 
         a, b = lines
 
@@ -2520,18 +2404,20 @@
         if lib:
             pair.append(lib)
         print("\t".join(pair), file=fw)
 
         print(a, file=fwm)
         print(b, file=fwm)
 
-    logging.debug(
-        "Discard {0} frags and write {1} pairs to `{2}` and `{3}`.".format(
-            num_fragments, num_pairs, matesfile, matesbedfile
-        )
+    logger.debug(
+        "Discard %d frags and write %d pairs to `%s` and `%s`.",
+        num_fragments,
+        num_pairs,
+        matesfile,
+        matesbedfile,
     )
 
     fw.close()
     fwm.close()
 
     return matesfile, matesbedfile
```

### Comparing `jcvi-1.4.5/jcvi/formats/blast.py` & `jcvi-1.4.6/jcvi/formats/blast.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/formats/cblast.pyx` & `jcvi-1.4.6/jcvi/formats/cblast.pyx`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/formats/cdt.py` & `jcvi-1.4.6/jcvi/formats/cdt.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/formats/chain.py` & `jcvi-1.4.6/jcvi/formats/chain.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/formats/contig.py` & `jcvi-1.4.6/jcvi/formats/contig.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/formats/coords.py` & `jcvi-1.4.6/jcvi/formats/coords.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/formats/excel.py` & `jcvi-1.4.6/jcvi/formats/excel.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/formats/fasta.py` & `jcvi-1.4.6/jcvi/formats/fasta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 """
 Wrapper for biopython Fasta, add option to parse sequence headers
 """
 
 import re
 import sys
-import os
 import os.path as op
 import shutil
 import logging
 import string
 import hashlib
 
+from random import choice
+
 from itertools import groupby, zip_longest
 from more_itertools import grouper, pairwise
 
 from Bio import SeqIO
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord
 from Bio.SeqUtils.CheckSum import seguid
 
-from jcvi.formats.base import BaseFile, DictFile, must_open
-from jcvi.formats.bed import Bed
-from jcvi.utils.cbook import percentage
-from jcvi.utils.console import printf
-from jcvi.utils.table import write_csv
-from jcvi.apps.base import OptionParser, ActionDispatcher, cleanup, need_update
+from ..apps.base import OptionParser, ActionDispatcher, cleanup, need_update
+from ..utils.cbook import percentage
+from ..utils.console import printf
+from ..utils.table import write_csv
+
+from .base import BaseFile, DictFile, must_open
+from .bed import Bed
 
 
 class Fasta(BaseFile, dict):
     def __init__(self, filename, index=False, key_function=None, lazy=False):
         super(Fasta, self).__init__(filename)
         self.key_function = key_function
 
@@ -162,27 +164,25 @@
 
         if asstring:
             return str(seq)
 
         return seq
 
 
-"""
-Class derived from https://gist.github.com/933737
-Original code written by David Winter (https://github.com/dwinter)
-
-Code writted to answer this challenge at Biostar:
-http://biostar.stackexchange.com/questions/5902/
+class ORFFinder(object):
+    """
+    Class derived from https://gist.github.com/933737
+    Original code written by David Winter (https://github.com/dwinter)
 
-(Code includes improvements from Brad Chapman)
-"""
+    Code writted to answer this challenge at Biostar:
+    http://biostar.stackexchange.com/questions/5902/
 
+    (Code includes improvements from Brad Chapman)
 
-class ORFFinder(object):
-    """Find the longest ORF in a given sequence
+    Find the longest ORF in a given sequence
     "seq" is a string, if "start" is not provided any codon can be the start of
     and ORF. If muliple ORFs have the longest length the first one encountered
     is printed
     """
 
     def __init__(self, seq, start=[], stop=["TAG", "TAA", "TGA"]):
         self.seq = str(seq).upper()
@@ -352,70 +352,65 @@
     cs = s.translate(_complement)
     return cs[::-1]
 
 
 def main():
 
     actions = (
+        ("clean", "remove irregular chars in FASTA seqs"),
+        ("diff", "check if two fasta records contain same information"),
         (
             "extract",
-            "given fasta file and seq id, retrieve the sequence " + "in fasta format",
+            "given fasta file and seq id, retrieve the sequence in fasta format",
         ),
-        ("longestorf", "find longest orf for CDS fasta"),
-        ("translate", "translate CDS to proteins"),
-        ("info", "run `sequence_info` on fasta files"),
-        ("summary", "report the real no of bases and N's in fasta files"),
-        ("uniq", "remove records that are the same"),
-        ("ids", "generate a list of headers"),
+        ("fastq", "combine fasta and qual to create fastq file"),
         (
             "format",
-            "trim accession id to the first space or switch id "
-            + "based on 2-column mapping file",
+            "trim accession id to the first space or switch id based on 2-column mapping file",
         ),
-        ("pool", "pool a bunch of fastafiles together and add prefix"),
-        ("random", "randomly take some records"),
-        ("simulate", "simulate random fasta file for testing"),
-        ("diff", "check if two fasta records contain same information"),
-        ("identical", "given 2 fasta files, find all exactly identical records"),
-        ("trim", "given a cross_match screened fasta, trim the sequence"),
-        ("trimsplit", "split sequences at lower-cased letters"),
-        ("sort", "sort the records by IDs, sizes, etc."),
         ("filter", "filter the records by size"),
+        ("fromtab", "convert 2-column sequence file to FASTA format"),
+        ("gaps", "print out a list of gap sizes within sequences"),
+        ("gc", "plot G+C content distribution"),
+        ("identical", "given 2 fasta files, find all exactly identical records"),
+        ("ids", "generate a list of headers"),
+        ("info", "run `sequence_info` on fasta files"),
+        ("ispcr", "reformat paired primers into isPcr query format"),
+        ("join", "concatenate a list of seqs and add gaps in between"),
+        ("longestorf", "find longest orf for CDS fasta"),
         ("pair", "sort paired reads to .pairs, rest to .fragments"),
         (
             "pairinplace",
-            "starting from fragment.fasta, find if "
-            + "adjacent records can form pairs",
+            "starting from fragment.fasta, find if adjacent records can form pairs",
         ),
-        ("fastq", "combine fasta and qual to create fastq file"),
-        ("tidy", "normalize gap sizes and remove small components in fasta"),
+        ("pool", "pool a bunch of fastafiles together and add prefix"),
+        ("qual", "generate dummy .qual file based on FASTA file"),
+        ("random", "randomly take some records"),
         ("sequin", "generate a gapped fasta file for sequin submission"),
-        ("gaps", "print out a list of gap sizes within sequences"),
-        ("join", "concatenate a list of seqs and add gaps in between"),
+        ("simulate", "simulate random fasta file for testing"),
         (
             "some",
-            "include or exclude a list of records (also performs on "
-            + ".qual file if available)",
+            "include or exclude a list of records (also performs on .qual file if available)",
         ),
-        ("qual", "generate dummy .qual file based on FASTA file"),
-        ("clean", "remove irregular chars in FASTA seqs"),
-        ("ispcr", "reformat paired primers into isPcr query format"),
-        ("fromtab", "convert 2-column sequence file to FASTA format"),
-        ("gc", "plot G+C content distribution"),
+        ("sort", "sort the records by IDs, sizes, etc."),
+        ("summary", "report the real no of bases and N's in fasta files"),
+        ("tidy", "normalize gap sizes and remove small components in fasta"),
+        ("translate", "translate CDS to proteins"),
+        ("trim", "given a cross_match screened fasta, trim the sequence"),
+        ("trimsplit", "split sequences at lower-cased letters"),
+        ("uniq", "remove records that are the same"),
     )
     p = ActionDispatcher(actions)
     p.dispatch(globals())
 
 
 def simulate_one(fw, name, size):
     """
     Simulate a random sequence with name and size
     """
-    from random import choice
-
     seq = Seq("".join(choice("ACGT") for _ in range(size)))
     s = SeqRecord(seq, id=name, description="Fake sequence")
     SeqIO.write([s], fw, "fasta")
 
 
 def simulate(args):
     """
```

### Comparing `jcvi-1.4.5/jcvi/formats/fastq.py` & `jcvi-1.4.6/jcvi/formats/fastq.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/formats/genbank.py` & `jcvi-1.4.6/jcvi/formats/genbank.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/formats/gff.py` & `jcvi-1.4.6/jcvi/formats/gff.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
-import sys
 import os
 import os.path as op
-import logging
 import re
+import sys
 
 from collections import defaultdict
 from urllib.parse import quote, unquote
 
-from jcvi.utils.cbook import AutoVivification
-from jcvi.formats.base import DictFile, LineFile, must_open, is_number
-from jcvi.formats.fasta import Fasta, SeqIO
-from jcvi.formats.bed import Bed, BedLine, natsorted
-from jcvi.annotation.reformat import atg_name
-from jcvi.utils.range import range_minmax
-from jcvi.utils.orderedcollections import DefaultOrderedDict, OrderedDict, parse_qs
-from jcvi.apps.base import (
+from ..apps.base import (
     OptionParser,
     OptionGroup,
     ActionDispatcher,
     cleanup,
     flatten,
+    logger,
     mkdir,
     need_update,
     parse_multi_values,
     sh,
 )
+from ..annotation.reformat import atg_name
+from ..utils.cbook import AutoVivification
+from ..utils.range import Range, range_minmax
+from ..utils.orderedcollections import DefaultOrderedDict, OrderedDict, parse_qs
+
+from .base import DictFile, LineFile, must_open, is_number
+from .bed import Bed, BedLine, natsorted
+from .fasta import Fasta, SeqIO
 
 
 Valid_strands = ("+", "-", "?", ".")
 Valid_phases = ("0", "1", "2", ".")
 FastaTag = "##FASTA"
 RegionTag = "##sequence-region"
 valid_gff_parent_child = {
@@ -352,27 +353,27 @@
             self.append_attrib = append_attrib
             self.score_attrib = score_attrib
             self.keep_attr_order = keep_attr_order
             self.compute_signature = compute_signature
             if filename in ("-", "stdin") or filename.endswith(".gz"):
                 if ".gtf" in filename:
                     self.gff3 = False
-                    logging.debug("File is not gff3 standard.")
+                    logger.debug("File is not gff3 standard.")
                 return
 
             self.set_gff_type()
 
     def set_gff_type(self):
         # Determine file type
         row = None
         for row in self:
             break
         gff3 = False if not row else "=" in row.attributes_text
         if not gff3:
-            logging.debug("File is not gff3 standard.")
+            logger.debug("File is not gff3 standard.")
 
         self.gff3 = gff3
         self.fp.seek(0)
 
     def __iter__(self):
         if self.make_gff_store:
             for row in self.gffstore:
@@ -479,16 +480,14 @@
     return d
 
 
 def to_range(obj, score=None, id=None, strand=None):
     """
     Given a gffutils object, convert it to a range object
     """
-    from jcvi.utils.range import Range
-
     if score or id:
         _score = score if score else obj.score
         _id = id if id else obj.id
         return Range(
             seqid=obj.seqid, start=obj.start, end=obj.end, score=_score, id=_id
         )
     elif strand:
@@ -498,47 +497,47 @@
 
 
 def main():
     actions = (
         ("addparent", "merge sister features and infer their parent"),
         ("bed", "parse gff and produce bed file for particular feature type"),
         ("bed12", "produce bed12 file for coding features"),
-        ("fromgtf", "convert gtf to gff3 format"),
-        ("gtf", "convert gff3 to gtf format"),
-        ("gb", "convert gff3 to genbank format"),
-        ("sort", "sort the gff file"),
+        ("chain", "fill in parent features by chaining children"),
+        ("children", "find all children that belongs to the same parent"),
+        ("cluster", "cluster transcripts based on shared splicing structure"),
+        ("extract", "extract contig or features from gff file"),
         ("filter", "filter the gff file based on Identity and Coverage"),
-        ("sizes", "calculate sizes of features in gff file"),
-        ("format", "format the gff file, change seqid, etc."),
         (
             "fixboundaries",
             "fix boundaries of parent features by range chaining child features",
         ),
-        ("chain", "fill in parent features by chaining children"),
-        ("rename", "change the IDs within the gff3"),
-        ("uniq", "remove the redundant gene models"),
-        ("liftover", "adjust gff coordinates based on tile number"),
-        ("note", "extract certain attribute field for each feature"),
-        ("load", "extract the feature (e.g. CDS) sequences and concatenate"),
-        ("extract", "extract contig or features from gff file"),
-        ("split", "split the gff into one contig per file"),
-        ("merge", "merge several gff files into one"),
-        ("parents", "find the parents given a list of IDs"),
-        ("children", "find all children that belongs to the same parent"),
+        (
+            "fixpartials",
+            "fix 5/3 prime partial transcripts, locate nearest in-frame start/stop",
+        ),
+        ("format", "format the gff file, change seqid, etc."),
         ("frombed", "convert from bed format to gff3"),
+        ("fromgtf", "convert gtf to gff3 format"),
         ("fromsoap", "convert from soap format to gff3"),
         ("gapsplit", "split alignment GFF3 at gaps based on CIGAR string"),
+        ("gb", "convert gff3 to genbank format"),
+        ("gtf", "convert gff3 to gtf format"),
+        ("liftover", "adjust gff coordinates based on tile number"),
+        ("load", "extract the feature (e.g. CDS) sequences and concatenate"),
+        ("merge", "merge several gff files into one"),
+        ("note", "extract certain attribute field for each feature"),
         ("orient", "orient the coding features based on translation"),
+        ("parents", "find the parents given a list of IDs"),
+        ("rename", "change the IDs within the gff3"),
+        ("sizes", "calculate sizes of features in gff file"),
+        ("sort", "sort the gff file"),
         ("splicecov", "tag gff introns with coverage info from junctions.bed"),
+        ("split", "split the gff into one contig per file"),
         ("summary", "print summary stats for features of different types"),
-        ("cluster", "cluster transcripts based on shared splicing structure"),
-        (
-            "fixpartials",
-            "fix 5/3 prime partial transcripts, locate nearest in-frame start/stop",
-        ),
+        ("uniq", "remove the redundant gene models"),
     )
 
     p = ActionDispatcher(actions)
     p.dispatch(globals())
 
 
 def addparent(args):
@@ -560,17 +559,15 @@
     gff = Gff(gff_file)
     data = defaultdict(list)
     for g in gff:
         if g.type != opts.childfeat:
             continue
         data[g.parent].append(g)
 
-    logging.debug(
-        "A total of {0} {1} features clustered".format(len(data), opts.childfeat)
-    )
+    logger.debug("A total of %d %s features clustered", len(data), opts.childfeat)
 
     parents = []
     for parent, dd in data.items():
         d = dd[0]
         start, end = min(x.start for x in dd), max(x.end for x in dd)
         gffline = "\t".join(
             str(x)
@@ -584,15 +581,15 @@
                 d.strand,
                 ".",
                 "ID={0};Name={0}".format(parent),
             )
         )
         parents.append(GffLine(gffline))
     parents.sort(key=lambda x: (x.seqid, x.start))
-    logging.debug("Merged feature sorted")
+    logger.debug("Merged feature sorted")
 
     fw = must_open(opts.outfile, "w")
     for parent in parents:
         print(parent, file=fw)
         parent_id = parent.id
         for d in data[parent_id]:
             if d.accn == parent_id:
@@ -623,17 +620,16 @@
     if type == "start":
         if codon != "ATG":
             return False
     elif type == "stop":
         if not any(_codon == codon for _codon in ("TGA", "TAG", "TAA")):
             return False
     else:
-        logging.error(
-            "`{0}` is not a valid codon type. ".format(type)
-            + "Should be one of (`start` or `stop`)"
+        logger.error(
+            "`%s` is not a valid codon type. Should be one of (`start` or `stop`)", type
         )
         sys.exit()
 
     return True
 
 
 def scan_for_valid_codon(codon_span, strand, seqid, genome, type="start"):
@@ -735,22 +731,23 @@
 
                 if not is_valid_codon(stop_codon_fasta, type="stop"):
                     three_prime = False
                     nstop = scan_for_valid_codon(
                         stop_codon, strand, seqid, genome, type="stop"
                     )
 
-                logging.debug(
-                    "feature={0} ({1})".format(trid, strand)
-                    + ", 5'={0}, 3'={1}".format(five_prime, three_prime)
-                    + ", {0} <== {1} ==> {2}".format(
-                        nstart if strand == "+" else nstop,
-                        cds_span,
-                        nstop if strand == "+" else nstart,
-                    )
+                logger.debug(
+                    "feature=%s (%s), 5'=%s, 3'=%s, %d <== %d ==> %d",
+                    trid,
+                    strand,
+                    five_prime,
+                    three_prime,
+                    nstart if strand == "+" else nstop,
+                    cds_span,
+                    nstop if strand == "+" else nstart,
                 )
 
             if not five_prime or not three_prime:
                 if nstart != (None, None) and (start_codon != nstart):
                     i = 0 if strand == "+" else 1
                     new_cds_span[i] = nstart[i]
                 if nstop != (None, None) and (stop_codon != nstop):
@@ -985,15 +982,15 @@
         sys.exit(not p.print_help())
 
     (gff_file,) = args
     ids = opts.ids
 
     if ids:
         ids = SetFile(ids)
-        logging.debug("Total ids loaded: {0}".format(len(ids)))
+        logger.debug("Total ids loaded: %d", len(ids))
 
         if opts.isoform:
             pids = set()
             gff = Gff(gff_file)
             for g in gff:
                 if g.type != "mRNA":
                     continue
@@ -1002,22 +999,22 @@
                 if "longest" not in g.attributes:
                     pids = set(x + ".1" for x in ids)
                     break
                 if g.attributes["longest"][0] == "0":
                     continue
                 pids.add(g.id)
             ids = pids
-            logging.debug("After checking longest: {0}".format(len(ids)))
+            logger.debug("After checking longest: %d", len(ids))
 
         # Collects aliases
         gff = Gff(gff_file)
         for g in gff:
             if g.name in ids:
                 ids.add(g.id)
-        logging.debug("Total ids including aliases: {0}".format(len(ids)))
+        logger.debug("Total ids including aliases: %d", len(ids))
 
     gff = Gff(gff_file)
     beds = defaultdict(list)
     for g in gff:
         if ids and not (g.id in ids or g.name in ids or g.parent in ids):
             continue
 
@@ -1100,15 +1097,15 @@
         orientation = orientations.get(id, "+")
         if orientation == "-":
             g.strand = {"+": "-", "-": "+"}[g.strand]
             flipped += 1
 
         print(g)
 
-    logging.debug("A total of {0} features flipped.".format(flipped))
+    logger.debug("A total of %d features flipped.", flipped)
 
 
 def rename(args):
     """
     %prog rename in.gff3 switch.ids > reindexed.gff3
 
     Change the IDs within the gff3.
@@ -1221,15 +1218,15 @@
                 bad.add(g.id)
         elif oid and ocov:
             identity = float(g.attributes[id_attr][0])
             coverage = float(g.attributes[cov_attr][0])
             if identity < oid or coverage < ocov:
                 bad.add(g.id)
 
-    logging.debug("{0} bad accns marked.".format(len(bad)))
+    logger.debug("%d bad accns marked.", len(bad))
 
     fw = must_open(opts.outfile, "w")
     for g in gffdb.features_of_type(ptype, order_by=("seqid", "start")):
         if ptype != otype:
             feats = list(gffdb.children(g, featuretype=otype, order_by="start"))
             ok_feats = [f for f in feats if f.id not in bad]
             if len(ok_feats) > 0:
@@ -1766,18 +1763,17 @@
     if remove_attrs:
         mod_remove_attrs = []
         for remove_attr in remove_attrs:
             if remove_attr in mod_attrs:
                 mod_remove_attrs.append(remove_attr)
 
         if mod_remove_attrs:
-            logging.error(
-                "Attributes `{0}` cannot be removed and modified".format(
-                    ",".join(mod_remove_attrs)
-                )
+            logger.error(
+                "Attributes `%s` cannot be removed and modified",
+                ",".join(mod_remove_attrs),
             )
             sys.exit()
 
     if gsac:  # setting gsac will force IDs to be unique
         unique = True
         notes = {}
 
@@ -1908,17 +1904,15 @@
             g.phase = phaseT.get(phase, phase)
 
         if mapfile:
             if isinstance(mapping, dict):
                 if origid in mapping:
                     g.seqid = mapping[origid]
                 else:
-                    logging.error(
-                        "{0} not found in `{1}`. ID unchanged.".format(origid, mapfile)
-                    )
+                    logger.error("%s not found in `%s`. ID unchanged.", origid, mapfile)
             else:
                 g.seqid = mapfile
 
         if source:
             if isinstance(source, dict) and g.source in source:
                 g.source = source[g.source]
             else:
@@ -2243,15 +2237,15 @@
     gff = Gff(gffile)
     allgenes = []
     for g in gff:
         if g.type != type:
             continue
         allgenes.append(g)
 
-    logging.debug("A total of {0} {1} features imported.".format(len(allgenes), type))
+    logger.debug("A total of %d %s features imported.", len(allgenes), type)
     allgenes.sort(key=lambda x: (x.seqid, x.start))
     return allgenes
 
 
 def uniq(args):
     """
     %prog uniq gffile > uniq.gff
@@ -2315,55 +2309,55 @@
 
     populate_children(opts.outfile, bestids, gffile, iter=opts.iter)
 
 
 def populate_children(outfile, ids, gffile, iter="2", types=None):
     ids = set(ids)
     fw = must_open(outfile, "w")
-    logging.debug("A total of {0} features selected.".format(len(ids)))
-    logging.debug("Populate children. Iteration 1..")
+    logger.debug("A total of %d features selected.", len(ids))
+    logger.debug("Populate children. Iteration 1..")
     gff = Gff(gffile)
     children = set()
     for g in gff:
         if types and g.type in types:
             ids.add(g.accn)
         if "Parent" not in g.attributes:
             continue
         for parent in g.attributes["Parent"]:
             if parent in ids:
                 children.add(g.accn)
 
     if iter == "2":
-        logging.debug("Populate grand children. Iteration 2..")
+        logger.debug("Populate grand children. Iteration 2..")
         gff = Gff(gffile)
         for g in gff:
             if "Parent" not in g.attributes:
                 continue
             for parent in g.attributes["Parent"]:
                 if parent in children:
                     children.add(g.accn)
 
-    logging.debug("Populate parents..")
+    logger.debug("Populate parents..")
     gff = Gff(gffile)
     parents = set()
     for g in gff:
         if g.accn not in ids:
             continue
         if "Parent" not in g.attributes:
             continue
         for parent in g.attributes["Parent"]:
             parents.add(parent)
 
     combined = ids | children | parents
-    logging.debug("Original: {0}".format(len(ids)))
-    logging.debug("Children: {0}".format(len(children)))
-    logging.debug("Parents: {0}".format(len(parents)))
-    logging.debug("Combined: {0}".format(len(combined)))
+    logger.debug("Original: %d", len(ids))
+    logger.debug("Children: %d", len(children))
+    logger.debug("Parents: %d", len(parents))
+    logger.debug("Combined: %d", len(combined))
 
-    logging.debug("Filter gff file..")
+    logger.debug("Filter gff file..")
     gff = Gff(gffile)
     seen = set()
     for g in gff:
         accn = g.accn
         if accn in seen:
             continue
         if accn in combined:
@@ -2405,15 +2399,15 @@
 
     (gffile,) = args
     sortedgff = opts.outfile
     if opts.inplace:
         if opts.method == "topo" or (
             opts.method == "unix" and gffile in ("-", "stdin")
         ):
-            logging.error(
+            logger.error(
                 "Cannot perform inplace sort when method is `topo`"
                 + " or method is `unix` and input is `stdin` stream"
             )
             sys.exit()
 
     if opts.method == "unix":
         cmd = "sort"
@@ -2423,15 +2417,15 @@
         if opts.inplace:
             cmd += " -o {0}".gffile
             sortedgff = None
         sh(cmd, outfile=sortedgff)
     elif opts.method == "topo":
         GT_HOME = opts.gt_home
         if not op.isdir(GT_HOME):
-            logging.error("GT_HOME={0} directory does not exist".format(GT_HOME))
+            logger.error("GT_HOME=%s directory does not exist", GT_HOME)
             sys.exit()
         cmd = "{0}".format(op.join(GT_HOME, "bin", "gt"))
         cmd += " gff3 -sort -tidy -retainids -addids no {0}".format(gffile)
         sh(cmd, outfile=sortedgff)
 
 
 def fromgtf(args):
@@ -2486,15 +2480,15 @@
         else:
             assert 0, "Don't know how to deal with {0}".format(g.type)
 
         g.update_attributes()
         print(g, file=fw)
         nfeats += 1
 
-    logging.debug("A total of {0} features written.".format(nfeats))
+    logger.debug("A total of %d features written.", nfeats)
 
 
 def frombed(args):
     """
     %prog frombed bed_file [--options] > gff_file
 
     Convert bed to gff file. In bed, the accn will convert to key='ID'
@@ -2652,15 +2646,15 @@
 
     outfile = opts.outfile
 
     deflines = set()
     fw = must_open(outfile, "w")
     fastarecs = {}
     for gffile in natsorted(gffiles, key=lambda x: op.basename(x)):
-        logging.debug(gffile)
+        logger.debug(gffile)
         fp = open(gffile)
         for row in fp:
             row = row.rstrip()
             if not row or row[0] == "#":
                 if row == FastaTag:
                     break
                 if row in deflines:
@@ -2967,15 +2961,15 @@
     generate a bed file
     """
     p = OptionParser(bed.__doc__)
     p.add_option(
         "--type",
         dest="type",
         default="gene",
-        help="Feature type to extract, use comma for multiple",
+        help="Feature type to extract, use comma for multiple, and `all` for all",
     )
     p.add_option("--key", default="ID", help="Key in the attributes to extract")
     p.add_option("--accn", help="Use fixed accn in the 4th column")
     p.add_option("--source", help="Source to extract from, use comma for multiple")
     p.add_option(
         "--span",
         default=False,
@@ -3038,26 +3032,28 @@
 
     opts, args = p.parse_args(args)
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (gffile,) = args
     key = opts.key or None
-    type = opts.type or set()
     accn = opts.accn
-    source = opts.source or set()
     span = opts.span
     primary_only = opts.primary_only
     parent_key = opts.parent_key
     human_chr = opts.human_chr
     ensembl_cds = opts.ensembl_cds
-    if opts.type:
+    if opts.type and opts.type != "all":
         type = set(x.strip() for x in opts.type.split(","))
+    else:
+        type = set()
     if opts.source:
         source = set(x.strip() for x in opts.source.split(","))
+    else:
+        source = set()
     if ensembl_cds:
         type = {"CDS"}
 
     gff = Gff(
         gffile,
         key=key,
         parent_key=parent_key,
@@ -3105,39 +3101,41 @@
                 continue
             seen.add(position)
 
         b.append(bl)
 
     sorted = not opts.nosort
     b.print_to_file(opts.outfile, sorted=sorted)
-    logging.debug(
-        "Extracted {} features (type={} id={} parent={})".format(
-            len(b), ",".join(type), key, parent_key
-        )
+    logger.debug(
+        "Extracted %d features (type=%s id=%s parent=%s)",
+        len(b),
+        ",".join(type),
+        key,
+        parent_key,
     )
     if primary_only:
-        logging.debug("Skipped non-primary: %d", skipped_non_primary)
+        logger.debug("Skipped non-primary: %d", skipped_non_primary)
     if ensembl_cds:
-        logging.debug("Skipped due to identical range: %d", skipped_identical_range)
+        logger.debug("Skipped due to identical range: %d", skipped_identical_range)
 
 
 def make_index(gff_file):
     """
     Make a sqlite database for fast retrieval of features.
     """
     import gffutils
 
     db_file = gff_file + ".db"
 
     if need_update(gff_file, db_file):
         cleanup(db_file)
-        logging.debug("Indexing `{0}`".format(gff_file))
+        logger.debug("Indexing `%s`", gff_file)
         gffutils.create_db(gff_file, db_file, merge_strategy="create_unique")
     else:
-        logging.debug("Load index `{0}`".format(gff_file))
+        logger.debug("Load index `%s`", gff_file)
 
     return gffutils.FeatureDB(db_file)
 
 
 def get_parents(gff_file, parents):
     gff = Gff(gff_file)
     for g in gff:
@@ -3329,15 +3327,15 @@
             fparent = (
                 feat.attributes["Parent"][0] if "Parent" in feat.attributes else None
             )
             if fparent:
                 try:
                     g_fparent = g[fparent]
                 except gffutils.exceptions.FeatureNotFoundError:
-                    logging.error("{} not found in index .. skipped".format(fparent))
+                    logger.error("%s not found in index .. skipped", fparent)
                     continue
                 if desc_attr in g_fparent.attributes:
                     desc = ",".join(g_fparent.attributes[desc_attr])
             if not desc and desc_attr in feat.attributes:
                 desc = ",".join(feat.attributes[desc_attr])
 
         if opts.full_header:
```

### Comparing `jcvi-1.4.5/jcvi/formats/html.py` & `jcvi-1.4.6/jcvi/formats/html.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/formats/maf.py` & `jcvi-1.4.6/jcvi/formats/maf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/formats/obo.py` & `jcvi-1.4.6/jcvi/formats/obo.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/formats/paf.py` & `jcvi-1.4.6/jcvi/formats/paf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/formats/pdf.py` & `jcvi-1.4.6/jcvi/formats/pdf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/formats/psl.py` & `jcvi-1.4.6/jcvi/formats/psl.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/formats/pyblast.py` & `jcvi-1.4.6/jcvi/formats/pyblast.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/formats/sam.py` & `jcvi-1.4.6/jcvi/formats/sam.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/formats/sizes.py` & `jcvi-1.4.6/jcvi/formats/sizes.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/formats/vcf.py` & `jcvi-1.4.6/jcvi/formats/vcf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/graphics/align.py` & `jcvi-1.4.6/jcvi/graphics/align.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/graphics/assembly.py` & `jcvi-1.4.6/jcvi/graphics/assembly.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/graphics/base.py` & `jcvi-1.4.6/jcvi/graphics/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,18 +34,19 @@
     Ellipse,
     PathPatch,
     FancyArrow,
     FancyArrowPatch,
     FancyBboxPatch,
 )
 
-from ..apps.base import datadir, glob, listify, logger, sample_N, which
+from ..apps.base import datadir, glob, logger, sample_N, which
 from ..formats.base import LineFile
 from ..utils.cbook import human_size
 
+Extent = Tuple[float, float, float, float]
 
 CHARS = {
     "&": r"\&",
     "%": r"\%",
     "$": r"\$",
     "#": r"\#",
     "_": r"\_",
@@ -153,14 +154,23 @@
         markerset = sample_N(mpl.lines.Line2D.filled_markers, len(self), seed=seed)
         self.assign_array("marker", markerset)
 
     def __str__(self):
         return "\n".join(str(x) for x in self)
 
 
+def adjust_extent(extent: Extent, root_extent: Extent) -> Extent:
+    """
+    Adjust the extent of the root axes.
+    """
+    rx, ry, rw, rh = root_extent
+    ex, ey, ew, eh = extent
+    return rx + ex * rw, ry + ey * rh, ew * rw, eh * rh
+
+
 def linear_blend(from_color, to_color, fraction=0.5):
     """Interpolate a new color between two colors.
 
     https://github.com/PimpTrizkit/PJs/wiki/12.-Shade,-Blend-and-Convert-a-Web-Color-(pSBC.js)
 
     Args:
         from_color (matplotlib color): starting color
@@ -190,15 +200,18 @@
     """
     assert -1 <= fraction <= 1, "Fraction must be between -1 and 1"
     if fraction < 0:
         return linear_blend("k", from_color, 1 + fraction)
     return linear_blend(from_color, "w", fraction)
 
 
-def load_image(filename):
+def load_image(filename: str) -> np.ndarray:
+    """
+    Load an image file and return as numpy array.
+    """
     img = plt.imread(filename)
     if len(img.shape) == 2:  # Gray-scale image, convert to RGB
         # http://www.socouldanyone.com/2013/03/converting-grayscale-to-rgb-with-numpy.html
         h, w = img.shape
         ret = np.empty((h, w, 3), dtype=np.uint8)
         ret[:, :, 2] = ret[:, :, 1] = ret[:, :, 0] = img
         img = ret
@@ -271,19 +284,18 @@
 
     return blues_r, reds, blue_red, green_purple, red_purple
 
 
 blues_r, reds, blue_red, green_purple, red_purple = prettyplot()
 
 
-def normalize_axes(axes):
+def normalize_axes(*axes):
     """
     Normalize the axes to have the same scale.
     """
-    axes = listify(axes)
     for ax in axes:
         ax.set_xlim(0, 1)
         ax.set_ylim(0, 1)
         ax.set_axis_off()
 
 
 def panel_labels(ax, labels, size: int = 16):
```

### Comparing `jcvi-1.4.5/jcvi/graphics/blastplot.py` & `jcvi-1.4.6/jcvi/graphics/blastplot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/graphics/chromosome.py` & `jcvi-1.4.6/jcvi/graphics/chromosome.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,27 +15,28 @@
 
 from natsort import natsorted
 
 from ..apps.base import OptionGroup, OptionParser, datafile, logger, sample_N
 from ..formats.base import DictFile, get_number
 from ..formats.bed import Bed
 from ..formats.sizes import Sizes
-from ..graphics.base import (
+
+from .base import (
     CirclePolygon,
     Polygon,
     Rectangle,
     latex,
     markup,
     normalize_axes,
     plt,
     savefig,
     set1_n,
     set3_n,
 )
-from ..graphics.glyph import BaseGlyph, plot_cap
+from .glyph import BaseGlyph, plot_cap
 
 
 class Chromosome(BaseGlyph):
     # Chromosome styles: rect - rectangle, roundrect - rounded rectangle, auto -
     # automatically pick the best style
     Styles = ("auto", "rect", "roundrect")
```

### Comparing `jcvi-1.4.5/jcvi/graphics/coverage.py` & `jcvi-1.4.6/jcvi/graphics/coverage.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/graphics/dotplot.py` & `jcvi-1.4.6/jcvi/graphics/dotplot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/graphics/glyph.py` & `jcvi-1.4.6/jcvi/graphics/glyph.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/graphics/grabseeds.py` & `jcvi-1.4.6/jcvi/graphics/grabseeds.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/graphics/heatmap.py` & `jcvi-1.4.6/jcvi/graphics/heatmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/graphics/histogram.py` & `jcvi-1.4.6/jcvi/graphics/histogram.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/graphics/karyotype.py` & `jcvi-1.4.6/jcvi/graphics/karyotype.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 .4, .3, .6, 60, k, Athaliana, top, athaliana.bed, center
 # edges
 e, 0, 1, athaliana.grape.4x1.simple
 """
 
 
 import sys
-import logging
 
 from typing import Optional
 
-from jcvi.apps.base import OptionParser
-from jcvi.compara.synteny import SimpleFile
-from jcvi.formats.bed import Bed
-from jcvi.graphics.chromosome import Chromosome, HorizontalChromosome
-from jcvi.graphics.glyph import TextCircle
-from jcvi.graphics.synteny import Shade, ymid_offset
-from jcvi.graphics.base import AbstractLayout, markup, mpl, plt, savefig, update_figname
+from ..apps.base import OptionParser, logger
+from ..compara.synteny import SimpleFile
+from ..formats.bed import Bed
+
+from .base import AbstractLayout, markup, mpl, plt, savefig, update_figname
+from .chromosome import Chromosome, HorizontalChromosome
+from .glyph import TextCircle
+from .synteny import Shade, ymid_offset
 
 
 class LayoutLine(object):
     def __init__(self, row, delimiter=",", generank=True):
         args = row.rstrip().split(delimiter)
         args = [x.strip() for x in args]
 
@@ -373,15 +373,15 @@
                     (x, max(z.end for z in list(bed.sub_bed(x)))) for x in seqids
                 )
                 assert sz is not None, "sizes not available and cannot be inferred"
             t.seqids = seqids
             # validate if all seqids are non-empty
             for k, v in sz.items():
                 if v == 0:
-                    logging.error("Size of `%s` is empty. Please check", k)
+                    logger.error("Size of `%s` is empty. Please check", k)
             t.sizes = sz
 
         tracks = []
         for lo in layout:
             if lo.empty:
                 continue
             tr = Track(root, lo, gap=gap, height=height, lw=lw, draw=False)
```

### Comparing `jcvi-1.4.5/jcvi/graphics/mummerplot.py` & `jcvi-1.4.6/jcvi/graphics/mummerplot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/graphics/synteny.py` & `jcvi-1.4.6/jcvi/graphics/synteny.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,39 +17,39 @@
 For "va" (vertical alignment), accepted values are: top|bottom|center|""(empty)
 """
 
 import sys
 from typing import Optional
 
 import numpy as np
-import matplotlib.transforms as transforms
+from matplotlib import transforms
 from matplotlib.path import Path
 
 from ..apps.base import OptionParser, logger
 from ..compara.synteny import BlockFile
 from ..formats.base import DictFile
 from ..formats.bed import Bed
-from ..graphics.base import (
+from ..utils.cbook import human_size
+from ..utils.validator import validate_in_choices, validate_in_range
+
+from .base import (
+    AbstractLayout,
+    PathPatch,
     markup,
     plt,
     savefig,
-    PathPatch,
-    AbstractLayout,
 )
-from ..graphics.glyph import (
+from .glyph import (
     BasePalette,
     Glyph,
     OrientationPalette,
     OrthoGroupPalette,
     RoundLabel,
 )
-from ..graphics.tree import draw_tree, read_trees
-
-from ..utils.cbook import human_size
-from ..utils.validator import validate_in_choices, validate_in_range
+from .tree import draw_tree, read_trees
 
 
 HorizontalAlignments = ("left", "right", "leftalign", "rightalign", "center", "")
 VerticalAlignments = ("top", "bottom", "center", "")
 CANVAS_SIZE = 0.65
```

### Comparing `jcvi-1.4.5/jcvi/graphics/table.py` & `jcvi-1.4.6/jcvi/graphics/table.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/graphics/tree.py` & `jcvi-1.4.6/jcvi/graphics/tree.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/graphics/wheel.py` & `jcvi-1.4.6/jcvi/graphics/wheel.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/projects/age.py` & `jcvi-1.4.6/jcvi/projects/age.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/projects/allmaps.py` & `jcvi-1.4.6/jcvi/projects/allmaps.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/projects/bites.py` & `jcvi-1.4.6/jcvi/projects/bites.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/projects/ies.py` & `jcvi-1.4.6/jcvi/projects/ies.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/projects/jcvi.py` & `jcvi-1.4.6/jcvi/projects/jcvi.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 import networkx as nx
 
 from ..apps.base import ActionDispatcher, OptionParser, logger
 from ..assembly.geneticmap import draw_geneticmap_heatmap
 from ..assembly.hic import draw_hic_heatmap
 from ..assembly.kmer import draw_ks_histogram
 from ..compara.pedigree import Pedigree, calculate_inbreeding
-from ..graphics.base import normalize_axes, panel_labels, plt, savefig
+from ..graphics.base import cm, load_image, normalize_axes, panel_labels, plt, savefig
 from ..graphics.chromosome import draw_chromosomes
-from ..graphics.landscape import draw_multi_depth
+from ..graphics.landscape import draw_multi_depth, draw_heatmaps, draw_stacks
 
 
 def diversity(args):
     """
     %prog diversity pedigree.ped VAR?_srtd.wgs.regions.bed.gz
 
     Plot diversity composite figure, including:
@@ -50,15 +50,15 @@
     G = ped.to_graph(inb, title="Pedigree of Variety1")
     A = nx.nx_agraph.to_agraph(G)
     dpi = 300
     A.draw(pngfile, prog="dot", args=f"-Gdpi={dpi}")
     logger.info("Pedigree graph written to `%s`", pngfile)
 
     # Show the image as is
-    ax1_root.imshow(plt.imread(pngfile))
+    ax1_root.imshow(load_image(pngfile))
     ax1_root.set_axis_off()
 
     # Panel B
     logger.info("Plotting depth distribution across genomes")
     npanels = len(bedfiles)
     yinterval = 1.0 / npanels
     ypos = 1 - yinterval
@@ -84,42 +84,44 @@
     )
 
     labels = (
         (0.02, 0.95, "A"),
         (0.25 + 0.25 * 0.1, 0.95, "B"),
     )
     panel_labels(root, labels)
-    normalize_axes([root, ax2_root])
+    normalize_axes(root, ax2_root)
 
     image_name = "diversity.pdf"
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
 def landscape(args):
     """
-    %prog landscape features.bed athaliana.sizes Fig5.png
+    %prog landscape features.bed athaliana.sizes TAIR10_chr_all.fas Chr2
 
     Plot landscape composite figure, including:
     A. Example genomic features painted on Arabidopsis genome
     B. Landscape of genomic features across the genome
     """
     p = OptionParser(landscape.__doc__)
-    _, args, iopts = p.set_image_options(args, figsize="10x7")
+    _, args, iopts = p.set_image_options(args, figsize="12x8")
 
-    if len(args) != 3:
+    if len(args) != 4:
         sys.exit(not p.print_help())
 
-    bedfile, sizesfile, pngfile = args
+    bedfile, sizesfile, fastafile, ch = args
 
     fig = plt.figure(1, (iopts.w, iopts.h))
     root = fig.add_axes((0, 0, 1, 1))
     aspect_ratio = iopts.w / iopts.h
     ax1_root = fig.add_axes((0, 1 / 4, 0.4, 0.5 * aspect_ratio))
-    ax2_root = fig.add_axes((0.4, 0.43, 0.54, 0.57))
-    ax3_root = fig.add_axes((0.43, -0.13, 0.54, 0.57))
+    ax2_root_extent = (0.4, 0.5, 0.6, 0.47)
+    ax2_root = fig.add_axes(ax2_root_extent)
+    ax3_root_extent = (0.41, 0, 0.6, 0.47)
+    ax3_root = fig.add_axes(ax3_root_extent)
 
     # Panel A
     logger.info("Plotting example genomic features painted on Arabidopsis genome")
     draw_chromosomes(
         ax1_root,
         bedfile,
         sizesfile,
@@ -130,37 +132,50 @@
         legend=True,
         empty=False,
         title="*Arabidopsis* genome features",
     )
 
     # Panel B
     logger.info("Plotting landscape of genomic features across the genome")
-    M = plt.imread(pngfile)
-    width, height = M.shape[1], M.shape[0]
-    # Split the image into left and right parts
-    mid = width // 2 - 10
-    left_cut = right_cut = 900
-    logger.info("Image size: %dx%d", width, height)
-    logger.info("Splitting image at %d", mid)
-
-    LM, RM = M[:left_cut, :mid], M[:right_cut, mid:]
-    logger.info("Left image size: %dx%d", LM.shape[1], LM.shape[0])
-    logger.info("Right image size: %dx%d", RM.shape[1], RM.shape[0])
+    stacks = ["Repeats", "Exons"]
+    heatmaps = ["Copia", "Gypsy", "Helitron", "hAT", "Exons"]
+    window = 250000
+    shift = 50000
+    draw_stacks(
+        fig,
+        ax2_root,
+        ax2_root_extent,
+        stacks,
+        fastafile,
+        window,
+        shift,
+        top=5,
+    )
+    draw_heatmaps(
+        fig,
+        ax3_root,
+        ax3_root_extent,
+        fastafile,
+        "Chr2",
+        stacks,
+        heatmaps,
+        window,
+        shift,
+        cmap=cm.viridis,
+    )
 
-    ax2_root.imshow(LM, extent=(0.4, 1, 0.5, 1), aspect="auto")
-    ax3_root.imshow(RM, extent=(0.4, 1, 0, 0.5), aspect="auto")
     ax2_root.set_axis_off()
     ax3_root.set_axis_off()
 
     labels = (
         (0.02, 0.95, "A"),
         (0.42, 0.95, "B"),
     )
     panel_labels(root, labels)
-    normalize_axes([root, ax1_root])
+    normalize_axes(root, ax1_root)
 
     image_name = "landscape.pdf"
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
 def genomebuild(args):
     """
@@ -224,15 +239,15 @@
 
     labels = (
         (1 / 3 * 0.1, 0.95, "A"),
         (1 / 3 * 1.1, 0.95, "B"),
         (1 / 3 * 2.1, 0.95, "C"),
     )
     panel_labels(root, labels)
-    normalize_axes([root, ax1_root, ax2_root, ax3_root])
+    normalize_axes(root, ax1_root, ax2_root, ax3_root)
 
     image_name = "genomebuild.pdf"
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
 def main():
```

### Comparing `jcvi-1.4.5/jcvi/projects/misc.py` & `jcvi-1.4.6/jcvi/projects/misc.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/projects/napus.py` & `jcvi-1.4.6/jcvi/projects/napus.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/projects/pineapple.py` & `jcvi-1.4.6/jcvi/projects/pineapple.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/projects/str.py` & `jcvi-1.4.6/jcvi/projects/str.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/projects/sugarcane.py` & `jcvi-1.4.6/jcvi/projects/sugarcane.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/projects/synfind.py` & `jcvi-1.4.6/jcvi/projects/synfind.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/projects/tgbs.py` & `jcvi-1.4.6/jcvi/projects/tgbs.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/projects/vanilla.py` & `jcvi-1.4.6/jcvi/projects/vanilla.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Plotting scripts for the vanilla genome paper.
 """
-import logging
 import sys
 
-from jcvi.apps.base import ActionDispatcher, OptionParser
-from jcvi.compara.synteny import check_beds
-from jcvi.formats.base import get_number
-from jcvi.formats.bed import Bed
-from jcvi.graphics.base import normalize_axes, panel_labels, plt, savefig
-from jcvi.graphics.glyph import TextCircle
-from jcvi.graphics.synteny import Synteny, draw_gene_legend
+from ..apps.base import ActionDispatcher, OptionParser, logger
 from ..compara.base import AnchorFile
+from ..compara.synteny import check_beds
+from ..formats.base import get_number
+from ..formats.bed import Bed
+from ..graphics.base import normalize_axes, panel_labels, plt, savefig
+from ..graphics.chromosome import draw_chromosomes
+from ..graphics.glyph import TextCircle
+from ..graphics.synteny import Synteny, draw_gene_legend
+from ..graphics.tree import parse_tree, LeafInfoFile, WGDInfoFile, draw_tree
 
 
 def main():
     actions = (
         # Chromosome painting since WGD
         ("ancestral", "paint 14 chromosomes following alpha WGD (requires data)"),
         # main figures in text
@@ -38,28 +39,28 @@
 
 def phylogeny(args):
     """
     %prog phylogeny treefile ks.layout
 
     Create a composite figure with (A) tree and (B) ks.
     """
-    from jcvi.graphics.tree import parse_tree, LeafInfoFile, WGDInfoFile, draw_tree
+    from ..compara.ks import Layout, KsPlot, KsFile
 
     p = OptionParser(phylogeny.__doc__)
-    opts, args, iopts = p.set_image_options(args, figsize="10x12")
+    _, args, iopts = p.set_image_options(args, figsize="10x12")
 
     (datafile, layoutfile) = args
 
-    logging.debug("Load tree file `{0}`".format(datafile))
+    logger.debug("Load tree file `%s`", datafile)
     t, hpd = parse_tree(datafile)
 
     fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])
-    ax1 = fig.add_axes([0, 0.4, 1, 0.6])
-    ax2 = fig.add_axes([0.12, 0.065, 0.8, 0.3])
+    root = fig.add_axes((0, 0, 1, 1))
+    ax1 = fig.add_axes((0, 0.4, 1, 0.6))
+    ax2 = fig.add_axes((0.12, 0.065, 0.8, 0.3))
 
     margin, rmargin = 0.1, 0.2  # Left and right margin
     leafinfo = LeafInfoFile("leafinfo.csv").cache
     wgdinfo = WGDInfoFile("wgdinfo.csv").cache
     outgroup = "ginkgo"
 
     # Panel A
@@ -73,17 +74,14 @@
         internal=False,
         outgroup=outgroup,
         reroot=False,
         leafinfo=leafinfo,
         wgdinfo=wgdinfo,
         geoscale=True,
     )
-
-    from jcvi.apps.ks import Layout, KsPlot, KsFile
-
     # Panel B
     ks_min = 0.0
     ks_max = 3.0
     bins = 60
     fill = False
     layout = Layout(layoutfile)
     print(layout, file=sys.stderr)
@@ -102,39 +100,37 @@
             fill=fill,
             fitted=False,
             kde=True,
         )
 
     kp.draw(filename=None)
 
-    normalize_axes([root, ax1])
+    normalize_axes(root, ax1)
     labels = ((0.05, 0.95, "A"), (0.05, 0.4, "B"))
     panel_labels(root, labels)
 
     image_name = "phylogeny.pdf"
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
 def tree(args):
     """
     %prog tree treefile
 
     Create a tree figure.
     """
-    from jcvi.graphics.tree import parse_tree, LeafInfoFile, WGDInfoFile, draw_tree
-
     p = OptionParser(tree.__doc__)
-    opts, args, iopts = p.set_image_options(args, figsize="10x8")
+    _, args, iopts = p.set_image_options(args, figsize="10x8")
 
     (datafile,) = args
-    logging.debug("Load tree file `{0}`".format(datafile))
+    logger.debug("Load tree file `%s`", datafile)
     t, hpd = parse_tree(datafile)
 
     fig = plt.figure(1, (iopts.w, iopts.h))
-    ax1 = fig.add_axes([0, 0, 1, 1])
+    ax1 = fig.add_axes((0, 0, 1, 1))
 
     margin, rmargin = 0.1, 0.2  # Left and right margin
     leafinfo = LeafInfoFile("leafinfo.csv").cache
     wgdinfo = WGDInfoFile("wgdinfo.csv").cache
     outgroup = "ginkgo"
 
     # Panel A
@@ -149,34 +145,34 @@
         outgroup=outgroup,
         reroot=False,
         leafinfo=leafinfo,
         wgdinfo=wgdinfo,
         geoscale=True,
     )
 
-    normalize_axes([ax1])
+    normalize_axes(ax1)
     image_name = "tree.pdf"
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
 def ks(args):
     """
     %prog ks ks.layout
 
     Create a ks figure.
     """
+    from ..compara.ks import Layout, KsPlot, KsFile
+
     p = OptionParser(ks.__doc__)
-    opts, args, iopts = p.set_image_options(args, figsize="10x4")
+    _, args, iopts = p.set_image_options(args, figsize="10x4")
 
     (layoutfile,) = args
 
-    from jcvi.apps.ks import Layout, KsPlot, KsFile
-
     fig = plt.figure(1, (iopts.w, iopts.h))
-    ax2 = fig.add_axes([0.12, 0.12, 0.8, 0.8])
+    ax2 = fig.add_axes((0.12, 0.12, 0.8, 0.8))
 
     # Panel B
     ks_min = 0.0
     ks_max = 3.0
     bins = 60
     fill = False
     layout = Layout(layoutfile)
@@ -207,18 +203,16 @@
 def synteny(args):
     """
     %prog synteny vplanifoliaA_blocks.bed vplanifoliaA.sizes \
         b1.blocks all.bed b1.layout
 
     Create a composite figure with (A) wgd and (B) microsynteny.
     """
-    from jcvi.graphics.chromosome import draw_chromosomes
-
     p = OptionParser(synteny.__doc__)
-    opts, args, iopts = p.set_image_options(args, figsize="12x12")
+    _, args, iopts = p.set_image_options(args, figsize="12x12")
 
     (bedfile, sizesfile, blocksfile, allbedfile, blockslayout) = args
 
     fig = plt.figure(1, (iopts.w, iopts.h))
     root = fig.add_axes([0, 0, 1, 1])
     ax1 = fig.add_axes([0, 0.5, 1, 0.5])
     ax2 = fig.add_axes([0.02, 0, 0.98, 0.5])
@@ -237,37 +231,35 @@
         legend=False,
         title=title,
     )
 
     # Panel B
     draw_ploidy(fig, ax2, blocksfile, allbedfile, blockslayout)
 
-    normalize_axes([root, ax1, ax2])
+    normalize_axes(root, ax1, ax2)
     labels = ((0.05, 0.95, "A"), (0.05, 0.5, "B"))
     panel_labels(root, labels)
 
     image_name = "synteny.pdf"
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
 def wgd(args):
     """
     %prog wgd vplanifoliaA_blocks.bed vplanifoliaA.sizes
 
     Create a wgd figure.
     """
-    from jcvi.graphics.chromosome import draw_chromosomes
-
     p = OptionParser(synteny.__doc__)
-    opts, args, iopts = p.set_image_options(args, figsize="8x5")
+    _, args, iopts = p.set_image_options(args, figsize="8x5")
 
     (bedfile, sizesfile) = args
 
     fig = plt.figure(1, (iopts.w, iopts.h))
-    ax1 = fig.add_axes([0, 0, 1, 1])
+    ax1 = fig.add_axes((0, 0, 1, 1))
 
     title = r"Genome duplication $\alpha^{O}$ event in $\textit{Vanilla}$"
     draw_chromosomes(
         ax1,
         bedfile,
         sizes=sizesfile,
         iopts=iopts,
@@ -275,15 +267,15 @@
         winsize=50000,
         imagemap=False,
         gauge=True,
         legend=False,
         title=title,
     )
 
-    normalize_axes([ax1])
+    normalize_axes(ax1)
 
     image_name = "wgd.pdf"
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
 def microsynteny(args):
     """
@@ -293,19 +285,19 @@
     """
     p = OptionParser(synteny.__doc__)
     opts, args, iopts = p.set_image_options(args, figsize="12x6")
 
     (blocksfile, allbedfile, blockslayout) = args
 
     fig = plt.figure(1, (iopts.w, iopts.h))
-    ax2 = fig.add_axes([0, 0, 1, 1])
+    ax2 = fig.add_axes((0, 0, 1, 1))
 
     draw_ploidy(fig, ax2, blocksfile, allbedfile, blockslayout)
 
-    normalize_axes([ax2])
+    normalize_axes(ax2)
 
     image_name = "microsynteny.pdf"
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
 def ancestral(args):
     """
@@ -358,16 +350,16 @@
         )
 
     # Iterate through the blocks, store any regions that has hits to one of the
     # target_pairs
     ac = AnchorFile(anchorsfile)
     blocks = ac.blocks
     outbed = Bed()
-    for i, block in enumerate(blocks):
-        a, b, scores = zip(*block)
+    for block in blocks:
+        a, b, _ = zip(*block)
         a = [qorder[x] for x in a]
         b = [sorder[x] for x in b]
         astart, aend = min(a)[1], max(a)[1]
         bstart, bend = min(b)[1], max(b)[1]
         # Now convert to BED lines with new accn
         achr, bchr = astart.seqid, bstart.seqid
         target = get_target(achr, bchr)
```

### Comparing `jcvi-1.4.5/jcvi/utils/aws.py` & `jcvi-1.4.6/jcvi/utils/aws.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/utils/cbook.py` & `jcvi-1.4.6/jcvi/utils/cbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,27 +256,30 @@
                 size /= float(multiple)
             else:
                 break
 
     return "{0:.{1}f}{2}".format(size, precision, suffix)
 
 
-def autoscale(bp, optimal=6):
+def autoscale(bp: int, optimal: int = 6):
     """
+    Autoscale the basepair length to a more human readable number.
+    The optimal is the number of ticks we want to see on the axis.
+
     >>> autoscale(150000000)
     20000000
     >>> autoscale(97352632)
     10000000
     """
     slen = str(bp)
     tlen = slen[0:2] if len(slen) > 1 else slen[0]
     precision = len(slen) - 2  # how many zeros we need to pad?
     bp_len_scaled = int(tlen)  # scale bp_len to range (0, 100)
     tick_diffs = [(x, abs(bp_len_scaled / x - optimal)) for x in [1, 2, 5, 10]]
-    best_stride, best_tick_diff = min(tick_diffs, key=lambda x: x[1])
+    best_stride, _ = min(tick_diffs, key=lambda x: x[1])
 
     while precision > 0:
         best_stride *= 10
         precision -= 1
 
     return best_stride
```

### Comparing `jcvi-1.4.5/jcvi/utils/data/Airswing.ttf` & `jcvi-1.4.6/jcvi/utils/data/Airswing.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/utils/data/Collegia.ttf` & `jcvi-1.4.6/jcvi/utils/data/Collegia.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/utils/data/HookedUp.ttf` & `jcvi-1.4.6/jcvi/utils/data/HookedUp.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/utils/data/Humor-Sans.ttf` & `jcvi-1.4.6/jcvi/utils/data/Humor-Sans.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/utils/data/TREDs.meta.csv` & `jcvi-1.4.6/jcvi/utils/data/TREDs.meta.csv`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/utils/data/adapters.fasta` & `jcvi-1.4.6/jcvi/utils/data/adapters.fasta`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/utils/data/blosum80.mat` & `jcvi-1.4.6/jcvi/utils/data/blosum80.mat`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/utils/data/chrY.hg38.unique_ccn.gc` & `jcvi-1.4.6/jcvi/utils/data/chrY.hg38.unique_ccn.gc`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/utils/data/hg38.band.txt` & `jcvi-1.4.6/jcvi/utils/data/hg38.band.txt`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/utils/data/hg38.chrom.sizes` & `jcvi-1.4.6/jcvi/utils/data/hg38.chrom.sizes`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/utils/data/instance.json` & `jcvi-1.4.6/jcvi/utils/data/instance.json`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/utils/db.py` & `jcvi-1.4.6/jcvi/utils/db.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/utils/ez_setup.py` & `jcvi-1.4.6/jcvi/utils/ez_setup.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/utils/grouper.py` & `jcvi-1.4.6/jcvi/utils/grouper.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/utils/orderedcollections.py` & `jcvi-1.4.6/jcvi/utils/orderedcollections.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/utils/range.py` & `jcvi-1.4.6/jcvi/utils/range.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/utils/table.py` & `jcvi-1.4.6/jcvi/utils/table.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/utils/taxonomy.py` & `jcvi-1.4.6/jcvi/utils/taxonomy.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/utils/validator.py` & `jcvi-1.4.6/jcvi/utils/validator.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/utils/webcolors.py` & `jcvi-1.4.6/jcvi/utils/webcolors.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/variation/cnv.py` & `jcvi-1.4.6/jcvi/variation/cnv.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/variation/deconvolute.py` & `jcvi-1.4.6/jcvi/variation/deconvolute.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/variation/delly.py` & `jcvi-1.4.6/jcvi/variation/delly.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/variation/impute.py` & `jcvi-1.4.6/jcvi/variation/impute.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/variation/phase.py` & `jcvi-1.4.6/jcvi/variation/phase.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/variation/snp.py` & `jcvi-1.4.6/jcvi/variation/snp.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi/variation/str.py` & `jcvi-1.4.6/jcvi/variation/str.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/jcvi.egg-info/PKG-INFO` & `jcvi-1.4.6/jcvi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcvi
-Version: 1.4.5
+Version: 1.4.6
 Summary: Python utility libraries on genome assembly, annotation and comparative genomics
 Home-page: http://github.com/tanghaibao/jcvi
 Author: Haibao Tang, Vivek Krishnakumar, Jingping Li
 Author-email: tanghaibao@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -27,16 +27,16 @@
 Collection of Python libraries to parse bioinformatics files, or perform
 computation related to assembly, annotation, and comparative genomics.
 
 |         |                                                                  |
 | ------- | ---------------------------------------------------------------- |
 | Authors | Haibao Tang ([tanghaibao](http://github.com/tanghaibao))         |
 |         | Vivek Krishnakumar ([vivekkrish](https://github.com/vivekkrish)) |
-|         | Jingping Li ([Jingping](https://github.com/Jingping))            |
 |         | Xingtan Zhang ([tangerzhang](https://github.com/tangerzhang))    |
+|         | Won Cheol Yim ([wyim-pgl](https://github.com/wyim-pgl))          |
 | Email   | <tanghaibao@gmail.com>                                           |
 | License | [BSD](http://creativecommons.org/licenses/BSD/)                  |
 
 ## Citations
 
 - If you use the MCscan pipeline for synteny inference, please cite:
```

### Comparing `jcvi-1.4.5/jcvi.egg-info/SOURCES.txt` & `jcvi-1.4.6/jcvi.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 jcvi/annotation/evm.py
 jcvi/annotation/maker.py
 jcvi/annotation/pasa.py
 jcvi/annotation/qc.py
 jcvi/annotation/reformat.py
 jcvi/annotation/stats.py
 jcvi/annotation/train.py
+jcvi/annotation/trinity.py
 jcvi/apps/__init__.py
 jcvi/apps/__main__.py
 jcvi/apps/align.py
 jcvi/apps/base.py
 jcvi/apps/biomart.py
 jcvi/apps/blastplus.py
 jcvi/apps/bowtie.py
@@ -60,30 +61,28 @@
 jcvi/apps/vecscreen.py
 jcvi/assembly/__init__.py
 jcvi/assembly/__main__.py
 jcvi/assembly/allmaps.py
 jcvi/assembly/allpaths.py
 jcvi/assembly/automaton.py
 jcvi/assembly/base.py
-jcvi/assembly/ca.py
 jcvi/assembly/chic.pyx
 jcvi/assembly/coverage.py
 jcvi/assembly/gaps.py
 jcvi/assembly/geneticmap.py
 jcvi/assembly/goldenpath.py
 jcvi/assembly/hic.py
 jcvi/assembly/kmer.py
 jcvi/assembly/opticalmap.py
 jcvi/assembly/patch.py
 jcvi/assembly/postprocess.py
 jcvi/assembly/preprocess.py
 jcvi/assembly/sim.py
 jcvi/assembly/soap.py
 jcvi/assembly/syntenypath.py
-jcvi/assembly/trinity.py
 jcvi/compara/__init__.py
 jcvi/compara/__main__.py
 jcvi/compara/base.py
 jcvi/compara/blastfilter.py
 jcvi/compara/catalog.py
 jcvi/compara/fractionation.py
 jcvi/compara/ks.py
```

### Comparing `jcvi-1.4.5/setup.cfg` & `jcvi-1.4.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.5/setup.py` & `jcvi-1.4.6/setup.py`

 * *Files identical despite different names*

