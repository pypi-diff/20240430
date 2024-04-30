# Comparing `tmp/together-1.1.2.tar.gz` & `tmp/together-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "together-1.1.2.tar", max compression
+gzip compressed data, was "together-1.1.3.tar", max compression
```

## Comparing `together-1.1.2.tar` & `together-1.1.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    11357 2024-04-18 16:07:41.193542 together-1.1.2/LICENSE
--rw-r--r--   0        0        0     9667 2024-04-18 16:07:41.193542 together-1.1.2/README.md
--rw-r--r--   0        0        0     2439 2024-04-18 16:07:41.193542 together-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1401 2024-04-18 16:07:41.193542 together-1.1.2/src/together/__init__.py
--rw-r--r--   0        0        0       57 2024-04-18 16:07:41.193542 together-1.1.2/src/together/abstract/__init__.py
--rw-r--r--   0        0        0    25103 2024-04-18 16:07:41.193542 together-1.1.2/src/together/abstract/api_requestor.py
--rw-r--r--   0        0        0        0 2024-04-18 16:07:41.193542 together-1.1.2/src/together/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 16:07:41.193542 together-1.1.2/src/together/cli/api/__init__.py
--rw-r--r--   0        0        0     7838 2024-04-18 16:07:41.193542 together-1.1.2/src/together/cli/api/chat.py
--rw-r--r--   0        0        0     3691 2024-04-18 16:07:41.193542 together-1.1.2/src/together/cli/api/completions.py
--rw-r--r--   0        0        0     3186 2024-04-18 16:07:41.193542 together-1.1.2/src/together/cli/api/files.py
--rw-r--r--   0        0        0     4954 2024-04-18 16:07:41.193542 together-1.1.2/src/together/cli/api/finetune.py
--rw-r--r--   0        0        0     2363 2024-04-18 16:07:41.193542 together-1.1.2/src/together/cli/api/images.py
--rw-r--r--   0        0        0     1126 2024-04-18 16:07:41.193542 together-1.1.2/src/together/cli/api/models.py
--rw-r--r--   0        0        0     1977 2024-04-18 16:07:41.193542 together-1.1.2/src/together/cli/cli.py
--rw-r--r--   0        0        0     4774 2024-04-18 16:07:41.193542 together-1.1.2/src/together/client.py
--rw-r--r--   0        0        0      908 2024-04-18 16:07:41.193542 together-1.1.2/src/together/constants.py
--rw-r--r--   0        0        0     5329 2024-04-18 16:07:41.193542 together-1.1.2/src/together/error.py
--rw-r--r--   0        0        0    11438 2024-04-18 16:07:41.193542 together-1.1.2/src/together/filemanager.py
--rw-r--r--   0        0        0        0 2024-04-18 16:07:41.193542 together-1.1.2/src/together/legacy/__init__.py
--rw-r--r--   0        0        0      727 2024-04-18 16:07:41.193542 together-1.1.2/src/together/legacy/base.py
--rw-r--r--   0        0        0     2343 2024-04-18 16:07:41.193542 together-1.1.2/src/together/legacy/complete.py
--rw-r--r--   0        0        0      591 2024-04-18 16:07:41.193542 together-1.1.2/src/together/legacy/embeddings.py
--rw-r--r--   0        0        0     3863 2024-04-18 16:07:41.193542 together-1.1.2/src/together/legacy/files.py
--rw-r--r--   0        0        0     4917 2024-04-18 16:07:41.193542 together-1.1.2/src/together/legacy/finetune.py
--rw-r--r--   0        0        0      582 2024-04-18 16:07:41.193542 together-1.1.2/src/together/legacy/images.py
--rw-r--r--   0        0        0     1053 2024-04-18 16:07:41.193542 together-1.1.2/src/together/legacy/models.py
--rw-r--r--   0        0        0      701 2024-04-18 16:07:41.193542 together-1.1.2/src/together/resources/__init__.py
--rw-r--r--   0        0        0      617 2024-04-18 16:07:41.193542 together-1.1.2/src/together/resources/chat/__init__.py
--rw-r--r--   0        0        0    11140 2024-04-18 16:07:41.193542 together-1.1.2/src/together/resources/chat/completions.py
--rw-r--r--   0        0        0     8403 2024-04-18 16:07:41.193542 together-1.1.2/src/together/resources/completions.py
--rw-r--r--   0        0        0     2546 2024-04-18 16:07:41.193542 together-1.1.2/src/together/resources/embeddings.py
--rw-r--r--   0        0        0     4593 2024-04-18 16:07:41.193542 together-1.1.2/src/together/resources/files.py
--rw-r--r--   0        0        0    12416 2024-04-18 16:07:41.193542 together-1.1.2/src/together/resources/finetune.py
--rw-r--r--   0        0        0     4775 2024-04-18 16:07:41.197542 together-1.1.2/src/together/resources/images.py
--rw-r--r--   0        0        0     1786 2024-04-18 16:07:41.197542 together-1.1.2/src/together/resources/models.py
--rw-r--r--   0        0        0     1319 2024-04-18 16:07:41.197542 together-1.1.2/src/together/together_response.py
--rw-r--r--   0        0        0     1432 2024-04-18 16:07:41.197542 together-1.1.2/src/together/types/__init__.py
--rw-r--r--   0        0        0      642 2024-04-18 16:07:41.197542 together-1.1.2/src/together/types/abstract.py
--rw-r--r--   0        0        0     3630 2024-04-18 16:07:41.197542 together-1.1.2/src/together/types/chat_completions.py
--rw-r--r--   0        0        0     1491 2024-04-18 16:07:41.197542 together-1.1.2/src/together/types/common.py
--rw-r--r--   0        0        0     2173 2024-04-18 16:07:41.197542 together-1.1.2/src/together/types/completions.py
--rw-r--r--   0        0        0      751 2024-04-18 16:07:41.197542 together-1.1.2/src/together/types/embeddings.py
--rw-r--r--   0        0        0      370 2024-04-18 16:07:41.197542 together-1.1.2/src/together/types/error.py
--rw-r--r--   0        0        0     1954 2024-04-18 16:07:41.197542 together-1.1.2/src/together/types/files.py
--rw-r--r--   0        0        0     5775 2024-04-18 16:07:41.197542 together-1.1.2/src/together/types/finetune.py
--rw-r--r--   0        0        0      915 2024-04-18 16:07:41.197542 together-1.1.2/src/together/types/images.py
--rw-r--r--   0        0        0     1013 2024-04-18 16:07:41.197542 together-1.1.2/src/together/types/models.py
--rw-r--r--   0        0        0      662 2024-04-18 16:07:41.197542 together-1.1.2/src/together/utils/__init__.py
--rw-r--r--   0        0        0     1665 2024-04-18 16:07:41.197542 together-1.1.2/src/together/utils/_log.py
--rw-r--r--   0        0        0     2407 2024-04-18 16:07:41.197542 together-1.1.2/src/together/utils/api_helpers.py
--rw-r--r--   0        0        0     7165 2024-04-18 16:07:41.197542 together-1.1.2/src/together/utils/files.py
--rw-r--r--   0        0        0     1788 2024-04-18 16:07:41.197542 together-1.1.2/src/together/utils/tools.py
--rw-r--r--   0        0        0      126 2024-04-18 16:07:41.197542 together-1.1.2/src/together/version.py
--rw-r--r--   0        0        0    11114 1970-01-01 00:00:00.000000 together-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-30 18:14:31.730405 together-1.1.3/LICENSE
+-rw-r--r--   0        0        0    10365 2024-04-30 18:14:31.730405 together-1.1.3/README.md
+-rw-r--r--   0        0        0     2590 2024-04-30 18:14:31.730405 together-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1401 2024-04-30 18:14:31.734405 together-1.1.3/src/together/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-30 18:14:31.734405 together-1.1.3/src/together/abstract/__init__.py
+-rw-r--r--   0        0        0    25103 2024-04-30 18:14:31.734405 together-1.1.3/src/together/abstract/api_requestor.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:14:31.734405 together-1.1.3/src/together/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:14:31.734405 together-1.1.3/src/together/cli/api/__init__.py
+-rw-r--r--   0        0        0     7838 2024-04-30 18:14:31.734405 together-1.1.3/src/together/cli/api/chat.py
+-rw-r--r--   0        0        0     3691 2024-04-30 18:14:31.734405 together-1.1.3/src/together/cli/api/completions.py
+-rw-r--r--   0        0        0     3186 2024-04-30 18:14:31.734405 together-1.1.3/src/together/cli/api/files.py
+-rw-r--r--   0        0        0     4954 2024-04-30 18:14:31.734405 together-1.1.3/src/together/cli/api/finetune.py
+-rw-r--r--   0        0        0     2363 2024-04-30 18:14:31.734405 together-1.1.3/src/together/cli/api/images.py
+-rw-r--r--   0        0        0     1126 2024-04-30 18:14:31.734405 together-1.1.3/src/together/cli/api/models.py
+-rw-r--r--   0        0        0     1977 2024-04-30 18:14:31.734405 together-1.1.3/src/together/cli/cli.py
+-rw-r--r--   0        0        0     4774 2024-04-30 18:14:31.734405 together-1.1.3/src/together/client.py
+-rw-r--r--   0        0        0      908 2024-04-30 18:14:31.734405 together-1.1.3/src/together/constants.py
+-rw-r--r--   0        0        0     5329 2024-04-30 18:14:31.734405 together-1.1.3/src/together/error.py
+-rw-r--r--   0        0        0    11438 2024-04-30 18:14:31.734405 together-1.1.3/src/together/filemanager.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:14:31.734405 together-1.1.3/src/together/legacy/__init__.py
+-rw-r--r--   0        0        0      727 2024-04-30 18:14:31.734405 together-1.1.3/src/together/legacy/base.py
+-rw-r--r--   0        0        0     2343 2024-04-30 18:14:31.734405 together-1.1.3/src/together/legacy/complete.py
+-rw-r--r--   0        0        0      591 2024-04-30 18:14:31.734405 together-1.1.3/src/together/legacy/embeddings.py
+-rw-r--r--   0        0        0     3863 2024-04-30 18:14:31.734405 together-1.1.3/src/together/legacy/files.py
+-rw-r--r--   0        0        0     4917 2024-04-30 18:14:31.734405 together-1.1.3/src/together/legacy/finetune.py
+-rw-r--r--   0        0        0      582 2024-04-30 18:14:31.734405 together-1.1.3/src/together/legacy/images.py
+-rw-r--r--   0        0        0     1053 2024-04-30 18:14:31.734405 together-1.1.3/src/together/legacy/models.py
+-rw-r--r--   0        0        0      701 2024-04-30 18:14:31.734405 together-1.1.3/src/together/resources/__init__.py
+-rw-r--r--   0        0        0      617 2024-04-30 18:14:31.734405 together-1.1.3/src/together/resources/chat/__init__.py
+-rw-r--r--   0        0        0    11140 2024-04-30 18:14:31.734405 together-1.1.3/src/together/resources/chat/completions.py
+-rw-r--r--   0        0        0     8403 2024-04-30 18:14:31.734405 together-1.1.3/src/together/resources/completions.py
+-rw-r--r--   0        0        0     2546 2024-04-30 18:14:31.734405 together-1.1.3/src/together/resources/embeddings.py
+-rw-r--r--   0        0        0     4593 2024-04-30 18:14:31.734405 together-1.1.3/src/together/resources/files.py
+-rw-r--r--   0        0        0    12416 2024-04-30 18:14:31.734405 together-1.1.3/src/together/resources/finetune.py
+-rw-r--r--   0        0        0     4775 2024-04-30 18:14:31.734405 together-1.1.3/src/together/resources/images.py
+-rw-r--r--   0        0        0     1786 2024-04-30 18:14:31.734405 together-1.1.3/src/together/resources/models.py
+-rw-r--r--   0        0        0     1319 2024-04-30 18:14:31.734405 together-1.1.3/src/together/together_response.py
+-rw-r--r--   0        0        0     1432 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/__init__.py
+-rw-r--r--   0        0        0      642 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/abstract.py
+-rw-r--r--   0        0        0     3648 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/chat_completions.py
+-rw-r--r--   0        0        0     1491 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/common.py
+-rw-r--r--   0        0        0     2173 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/completions.py
+-rw-r--r--   0        0        0      751 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/embeddings.py
+-rw-r--r--   0        0        0      370 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/error.py
+-rw-r--r--   0        0        0     1954 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/files.py
+-rw-r--r--   0        0        0     5775 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/finetune.py
+-rw-r--r--   0        0        0      915 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/images.py
+-rw-r--r--   0        0        0     1013 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/models.py
+-rw-r--r--   0        0        0      662 2024-04-30 18:14:31.734405 together-1.1.3/src/together/utils/__init__.py
+-rw-r--r--   0        0        0     1665 2024-04-30 18:14:31.738405 together-1.1.3/src/together/utils/_log.py
+-rw-r--r--   0        0        0     2407 2024-04-30 18:14:31.738405 together-1.1.3/src/together/utils/api_helpers.py
+-rw-r--r--   0        0        0     7165 2024-04-30 18:14:31.738405 together-1.1.3/src/together/utils/files.py
+-rw-r--r--   0        0        0     1788 2024-04-30 18:14:31.738405 together-1.1.3/src/together/utils/tools.py
+-rw-r--r--   0        0        0      126 2024-04-30 18:14:31.738405 together-1.1.3/src/together/version.py
+-rw-r--r--   0        0        0    11812 1970-01-01 00:00:00.000000 together-1.1.3/PKG-INFO
```

### Comparing `together-1.1.2/LICENSE` & `together-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `together-1.1.2/README.md` & `together-1.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,605 +1,648 @@
-00000000: 5468 6520 5b54 6f67 6574 6865 7220 5079  The [Together Py
-00000010: 7468 6f6e 204c 6962 7261 7279 5d28 6874  thon Library](ht
-00000020: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00000030: 726f 6a65 6374 2f74 6f67 6574 6865 722f  roject/together/
-00000040: 2920 6973 2074 6865 206f 6666 6963 6961  ) is the officia
-00000050: 6c20 5079 7468 6f6e 2063 6c69 656e 7420  l Python client 
-00000060: 666f 7220 546f 6765 7468 6572 2773 2041  for Together's A
-00000070: 5049 2070 6c61 7466 6f72 6d2c 2070 726f  PI platform, pro
-00000080: 7669 6469 6e67 2061 2063 6f6e 7665 6e69  viding a conveni
-00000090: 656e 7420 7761 7920 666f 7220 696e 7465  ent way for inte
-000000a0: 7261 6374 696e 6720 7769 7468 2074 6865  racting with the
-000000b0: 2052 4553 5420 4150 4973 2061 6e64 2065   REST APIs and e
-000000c0: 6e61 626c 6573 2065 6173 7920 696e 7465  nables easy inte
-000000d0: 6772 6174 696f 6e73 2077 6974 6820 5079  grations with Py
-000000e0: 7468 6f6e 2033 2e38 2b20 6170 706c 6963  thon 3.8+ applic
-000000f0: 6174 696f 6e73 2077 6974 6820 6561 7379  ations with easy
-00000100: 2074 6f20 7573 6520 7379 6e63 6872 6f6e   to use synchron
-00000110: 6f75 7320 616e 6420 6173 796e 6368 726f  ous and asynchro
-00000120: 6e6f 7573 2063 6c69 656e 7473 2e0a 0a23  nous clients...#
-00000130: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a3e   Installation..>
-00000140: 20f0 9f9a a70a 3e20 5468 6520 6c69 6272   .....> The libr
-00000150: 6172 7920 7761 7320 7265 7772 6974 7465  ary was rewritte
-00000160: 6e20 696e 2076 312e 302e 3020 7265 6c65  n in v1.0.0 rele
-00000170: 6173 6564 2069 6e20 4170 7269 6c20 6f66  ased in April of
-00000180: 2032 3032 342e 2054 6865 7265 2077 6572   2024. There wer
-00000190: 6520 7369 676e 6966 6963 616e 7420 6368  e significant ch
-000001a0: 616e 6765 7320 6d61 6465 2e0a 0a54 6f20  anges made...To 
-000001b0: 696e 7374 616c 6c20 546f 6765 7468 6572  install Together
-000001c0: 2050 7974 686f 6e20 4c69 6272 6172 7920   Python Library 
-000001d0: 6672 6f6d 2050 7950 692c 2073 696d 706c  from PyPi, simpl
-000001e0: 7920 7275 6e3a 0a0a 6060 6073 6865 6c6c  y run:..```shell
-000001f0: 2053 6865 6c6c 0a70 6970 2069 6e73 7461   Shell.pip insta
-00000200: 6c6c 202d 2d75 7067 7261 6465 2074 6f67  ll --upgrade tog
-00000210: 6574 6865 720a 6060 600a 0a23 2320 5365  ether.```..## Se
-00000220: 7474 696e 6720 7570 2041 5049 204b 6579  tting up API Key
-00000230: 0a0a 3e20 f09f 9aa7 2059 6f75 2077 696c  ..> .... You wil
-00000240: 6c20 6e65 6564 2074 6f20 6372 6561 7465  l need to create
-00000250: 2061 6e20 6163 636f 756e 7420 7769 7468   an account with
-00000260: 205b 546f 6765 7468 6572 2e61 695d 2868   [Together.ai](h
-00000270: 7474 7073 3a2f 2f61 7069 2e74 6f67 6574  ttps://api.toget
-00000280: 6865 722e 7879 7a2f 2920 746f 206f 6274  her.xyz/) to obt
-00000290: 6169 6e20 6120 546f 6765 7468 6572 2041  ain a Together A
-000002a0: 5049 204b 6579 2e0a 0a4f 6e63 6520 6c6f  PI Key...Once lo
-000002b0: 6767 6564 2069 6e20 746f 2074 6865 2054  gged in to the T
-000002c0: 6f67 6574 6865 7220 506c 6179 6772 6f75  ogether Playgrou
-000002d0: 6e64 2c20 796f 7520 6361 6e20 6669 6e64  nd, you can find
-000002e0: 2061 7661 696c 6162 6c65 2041 5049 206b   available API k
-000002f0: 6579 7320 696e 205b 7468 6973 2073 6574  eys in [this set
-00000300: 7469 6e67 7320 7061 6765 5d28 6874 7470  tings page](http
-00000310: 733a 2f2f 6170 692e 746f 6765 7468 6572  s://api.together
-00000320: 2e78 797a 2f73 6574 7469 6e67 732f 6170  .xyz/settings/ap
-00000330: 692d 6b65 7973 292e 0a0a 2323 2320 5365  i-keys)...### Se
-00000340: 7474 696e 6720 656e 7669 726f 6e6d 656e  tting environmen
-00000350: 7420 7661 7269 6162 6c65 0a0a 6060 6073  t variable..```s
-00000360: 6865 6c6c 0a65 7870 6f72 7420 544f 4745  hell.export TOGE
-00000370: 5448 4552 5f41 5049 5f4b 4559 3d78 7878  THER_API_KEY=xxx
-00000380: 7878 0a60 6060 0a0a 2323 2320 5573 696e  xx.```..### Usin
-00000390: 6720 7468 6520 636c 6965 6e74 0a0a 6060  g the client..``
-000003a0: 6070 7974 686f 6e0a 6672 6f6d 2074 6f67  `python.from tog
-000003b0: 6574 6865 7220 696d 706f 7274 2054 6f67  ether import Tog
-000003c0: 6574 6865 720a 0a63 6c69 656e 7420 3d20  ether..client = 
-000003d0: 546f 6765 7468 6572 2861 7069 5f6b 6579  Together(api_key
-000003e0: 3d22 7878 7878 7822 290a 6060 600a 0a54  ="xxxxx").```..T
-000003f0: 6869 7320 6c69 6272 6172 7920 636f 6e74  his library cont
-00000400: 6169 6e73 2062 6f74 6820 6120 7079 7468  ains both a pyth
-00000410: 6f6e 206c 6962 7261 7279 2061 6e64 2061  on library and a
-00000420: 2043 4c49 2e20 5765 276c 6c20 6465 6d6f   CLI. We'll demo
-00000430: 6e73 7472 6174 6520 686f 7720 746f 2075  nstrate how to u
-00000440: 7365 2062 6f74 6820 6265 6c6f 772e 0a0a  se both below...
-00000450: 2320 5573 6167 6520 e280 9320 5079 7468  # Usage ... Pyth
-00000460: 6f6e 2043 6c69 656e 740a 0a23 2320 4368  on Client..## Ch
-00000470: 6174 2043 6f6d 706c 6574 696f 6e73 0a0a  at Completions..
-00000480: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
-00000490: 206f 730a 6672 6f6d 2074 6f67 6574 6865   os.from togethe
-000004a0: 7220 696d 706f 7274 2054 6f67 6574 6865  r import Togethe
-000004b0: 720a 0a63 6c69 656e 7420 3d20 546f 6765  r..client = Toge
-000004c0: 7468 6572 2861 7069 5f6b 6579 3d6f 732e  ther(api_key=os.
-000004d0: 656e 7669 726f 6e2e 6765 7428 2254 4f47  environ.get("TOG
-000004e0: 4554 4845 525f 4150 495f 4b45 5922 2929  ETHER_API_KEY"))
-000004f0: 0a0a 7265 7370 6f6e 7365 203d 2063 6c69  ..response = cli
-00000500: 656e 742e 6368 6174 2e63 6f6d 706c 6574  ent.chat.complet
-00000510: 696f 6e73 2e63 7265 6174 6528 0a20 2020  ions.create(.   
-00000520: 206d 6f64 656c 3d22 6d69 7374 7261 6c61   model="mistrala
-00000530: 692f 4d69 7874 7261 6c2d 3878 3742 2d49  i/Mixtral-8x7B-I
-00000540: 6e73 7472 7563 742d 7630 2e31 222c 0a20  nstruct-v0.1",. 
-00000550: 2020 206d 6573 7361 6765 733d 5b7b 2272     messages=[{"r
-00000560: 6f6c 6522 3a20 2275 7365 7222 2c20 2263  ole": "user", "c
-00000570: 6f6e 7465 6e74 223a 2022 7465 6c6c 206d  ontent": "tell m
-00000580: 6520 6162 6f75 7420 6e65 7720 796f 726b  e about new york
-00000590: 227d 5d2c 0a29 0a70 7269 6e74 2872 6573  "}],.).print(res
-000005a0: 706f 6e73 652e 6368 6f69 6365 735b 305d  ponse.choices[0]
-000005b0: 2e6d 6573 7361 6765 2e63 6f6e 7465 6e74  .message.content
-000005c0: 290a 6060 600a 0a23 2323 2053 7472 6561  ).```..### Strea
-000005d0: 6d69 6e67 0a0a 6060 6070 7974 686f 6e0a  ming..```python.
-000005e0: 696d 706f 7274 206f 730a 6672 6f6d 2074  import os.from t
-000005f0: 6f67 6574 6865 7220 696d 706f 7274 2054  ogether import T
-00000600: 6f67 6574 6865 720a 0a63 6c69 656e 7420  ogether..client 
-00000610: 3d20 546f 6765 7468 6572 2861 7069 5f6b  = Together(api_k
-00000620: 6579 3d6f 732e 656e 7669 726f 6e2e 6765  ey=os.environ.ge
-00000630: 7428 2254 4f47 4554 4845 525f 4150 495f  t("TOGETHER_API_
-00000640: 4b45 5922 2929 0a73 7472 6561 6d20 3d20  KEY")).stream = 
-00000650: 636c 6965 6e74 2e63 6861 742e 636f 6d70  client.chat.comp
-00000660: 6c65 7469 6f6e 732e 6372 6561 7465 280a  letions.create(.
-00000670: 2020 2020 6d6f 6465 6c3d 226d 6973 7472      model="mistr
-00000680: 616c 6169 2f4d 6978 7472 616c 2d38 7837  alai/Mixtral-8x7
-00000690: 422d 496e 7374 7275 6374 2d76 302e 3122  B-Instruct-v0.1"
-000006a0: 2c0a 2020 2020 6d65 7373 6167 6573 3d5b  ,.    messages=[
-000006b0: 7b22 726f 6c65 223a 2022 7573 6572 222c  {"role": "user",
-000006c0: 2022 636f 6e74 656e 7422 3a20 2274 656c   "content": "tel
-000006d0: 6c20 6d65 2061 626f 7574 206e 6577 2079  l me about new y
-000006e0: 6f72 6b22 7d5d 2c0a 2020 2020 7374 7265  ork"}],.    stre
-000006f0: 616d 3d54 7275 652c 0a29 0a0a 666f 7220  am=True,.)..for 
-00000700: 6368 756e 6b20 696e 2073 7472 6561 6d3a  chunk in stream:
-00000710: 0a20 2020 2070 7269 6e74 2863 6875 6e6b  .    print(chunk
-00000720: 2e63 686f 6963 6573 5b30 5d2e 6465 6c74  .choices[0].delt
-00000730: 612e 636f 6e74 656e 7420 6f72 2022 222c  a.content or "",
-00000740: 2065 6e64 3d22 222c 2066 6c75 7368 3d54   end="", flush=T
-00000750: 7275 6529 0a60 6060 0a0a 2323 2320 4173  rue).```..### As
-00000760: 796e 6320 7573 6167 650a 0a60 6060 7079  ync usage..```py
-00000770: 7468 6f6e 0a69 6d70 6f72 7420 6f73 2c20  thon.import os, 
-00000780: 6173 796e 6369 6f0a 6672 6f6d 2074 6f67  asyncio.from tog
-00000790: 6574 6865 7220 696d 706f 7274 2041 7379  ether import Asy
-000007a0: 6e63 546f 6765 7468 6572 0a0a 6173 796e  ncTogether..asyn
-000007b0: 635f 636c 6965 6e74 203d 2041 7379 6e63  c_client = Async
-000007c0: 546f 6765 7468 6572 2861 7069 5f6b 6579  Together(api_key
-000007d0: 3d6f 732e 656e 7669 726f 6e2e 6765 7428  =os.environ.get(
-000007e0: 2254 4f47 4554 4845 525f 4150 495f 4b45  "TOGETHER_API_KE
-000007f0: 5922 2929 0a6d 6573 7361 6765 7320 3d20  Y")).messages = 
-00000800: 5b0a 2020 2020 2257 6861 7420 6172 6520  [.    "What are 
-00000810: 7468 6520 746f 7020 7468 696e 6773 2074  the top things t
-00000820: 6f20 646f 2069 6e20 5361 6e20 4672 616e  o do in San Fran
-00000830: 6369 7363 6f3f 222c 0a20 2020 2022 5768  cisco?",.    "Wh
-00000840: 6174 2063 6f75 6e74 7279 2069 7320 5061  at country is Pa
-00000850: 7269 7320 696e 3f22 2c0a 5d0a 0a61 7379  ris in?",.]..asy
-00000860: 6e63 2064 6566 2061 7379 6e63 5f63 6861  nc def async_cha
-00000870: 745f 636f 6d70 6c65 7469 6f6e 286d 6573  t_completion(mes
-00000880: 7361 6765 7329 3a0a 2020 2020 6173 796e  sages):.    asyn
-00000890: 635f 636c 6965 6e74 203d 2041 7379 6e63  c_client = Async
-000008a0: 546f 6765 7468 6572 2861 7069 5f6b 6579  Together(api_key
-000008b0: 3d6f 732e 656e 7669 726f 6e2e 6765 7428  =os.environ.get(
-000008c0: 2254 4f47 4554 4845 525f 4150 495f 4b45  "TOGETHER_API_KE
-000008d0: 5922 2929 0a20 2020 2074 6173 6b73 203d  Y")).    tasks =
-000008e0: 205b 0a20 2020 2020 2020 2061 7379 6e63   [.        async
-000008f0: 5f63 6c69 656e 742e 6368 6174 2e63 6f6d  _client.chat.com
-00000900: 706c 6574 696f 6e73 2e63 7265 6174 6528  pletions.create(
-00000910: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
-00000920: 656c 3d22 6d69 7374 7261 6c61 692f 4d69  el="mistralai/Mi
-00000930: 7874 7261 6c2d 3878 3742 2d49 6e73 7472  xtral-8x7B-Instr
-00000940: 7563 742d 7630 2e31 222c 0a20 2020 2020  uct-v0.1",.     
-00000950: 2020 2020 2020 206d 6573 7361 6765 733d         messages=
-00000960: 5b7b 2272 6f6c 6522 3a20 2275 7365 7222  [{"role": "user"
-00000970: 2c20 2263 6f6e 7465 6e74 223a 206d 6573  , "content": mes
-00000980: 7361 6765 7d5d 2c0a 2020 2020 2020 2020  sage}],.        
-00000990: 290a 2020 2020 2020 2020 666f 7220 6d65  ).        for me
-000009a0: 7373 6167 6520 696e 206d 6573 7361 6765  ssage in message
-000009b0: 730a 2020 2020 5d0a 2020 2020 7265 7370  s.    ].    resp
-000009c0: 6f6e 7365 7320 3d20 6177 6169 7420 6173  onses = await as
-000009d0: 796e 6369 6f2e 6761 7468 6572 282a 7461  yncio.gather(*ta
-000009e0: 736b 7329 0a0a 2020 2020 666f 7220 7265  sks)..    for re
-000009f0: 7370 6f6e 7365 2069 6e20 7265 7370 6f6e  sponse in respon
-00000a00: 7365 733a 0a20 2020 2020 2020 2070 7269  ses:.        pri
-00000a10: 6e74 2872 6573 706f 6e73 652e 6368 6f69  nt(response.choi
-00000a20: 6365 735b 305d 2e6d 6573 7361 6765 2e63  ces[0].message.c
-00000a30: 6f6e 7465 6e74 290a 0a61 7379 6e63 696f  ontent)..asyncio
-00000a40: 2e72 756e 2861 7379 6e63 5f63 6861 745f  .run(async_chat_
-00000a50: 636f 6d70 6c65 7469 6f6e 286d 6573 7361  completion(messa
-00000a60: 6765 7329 290a 6060 600a 0a23 2320 436f  ges)).```..## Co
-00000a70: 6d70 6c65 7469 6f6e 730a 0a43 6f6d 706c  mpletions..Compl
-00000a80: 6574 696f 6e73 2061 7265 2066 6f72 2063  etions are for c
-00000a90: 6f64 6520 616e 6420 6c61 6e67 7561 6765  ode and language
-00000aa0: 206d 6f64 656c 7320 7368 6f77 6e20 5b68   models shown [h
-00000ab0: 6572 655d 2868 7474 7073 3a2f 2f64 6f63  ere](https://doc
-00000ac0: 732e 746f 6765 7468 6572 2e61 692f 646f  s.together.ai/do
-00000ad0: 6373 2f69 6e66 6572 656e 6365 2d6d 6f64  cs/inference-mod
-00000ae0: 656c 7329 2e20 4265 6c6f 772c 2061 2063  els). Below, a c
-00000af0: 6f64 6520 6d6f 6465 6c20 6578 616d 706c  ode model exampl
-00000b00: 6520 6973 2073 686f 776e 2e0a 0a60 6060  e is shown...```
-00000b10: 7079 7468 6f6e 0a69 6d70 6f72 7420 6f73  python.import os
-00000b20: 0a66 726f 6d20 746f 6765 7468 6572 2069  .from together i
-00000b30: 6d70 6f72 7420 546f 6765 7468 6572 0a0a  mport Together..
-00000b40: 636c 6965 6e74 203d 2054 6f67 6574 6865  client = Togethe
-00000b50: 7228 6170 695f 6b65 793d 6f73 2e65 6e76  r(api_key=os.env
-00000b60: 6972 6f6e 2e67 6574 2822 544f 4745 5448  iron.get("TOGETH
-00000b70: 4552 5f41 5049 5f4b 4559 2229 290a 0a72  ER_API_KEY"))..r
-00000b80: 6573 706f 6e73 6520 3d20 636c 6965 6e74  esponse = client
-00000b90: 2e63 6f6d 706c 6574 696f 6e73 2e63 7265  .completions.cre
-00000ba0: 6174 6528 0a20 2020 206d 6f64 656c 3d22  ate(.    model="
-00000bb0: 636f 6465 6c6c 616d 612f 436f 6465 4c6c  codellama/CodeLl
-00000bc0: 616d 612d 3334 622d 5079 7468 6f6e 2d68  ama-34b-Python-h
-00000bd0: 6622 2c0a 2020 2020 7072 6f6d 7074 3d22  f",.    prompt="
-00000be0: 5772 6974 6520 6120 4e65 7874 2e6a 7320  Write a Next.js 
-00000bf0: 636f 6d70 6f6e 656e 7420 7769 7468 2054  component with T
-00000c00: 6169 6c77 696e 6443 5353 2066 6f72 2061  ailwindCSS for a
-00000c10: 2068 6561 6465 7220 636f 6d70 6f6e 656e   header componen
-00000c20: 742e 222c 0a29 0a70 7269 6e74 2872 6573  t.",.).print(res
-00000c30: 706f 6e73 652e 6368 6f69 6365 735b 305d  ponse.choices[0]
-00000c40: 2e74 6578 7429 0a60 6060 0a0a 2323 2320  .text).```..### 
-00000c50: 5374 7265 616d 696e 670a 0a60 6060 7079  Streaming..```py
-00000c60: 7468 6f6e 0a69 6d70 6f72 7420 6f73 0a66  thon.import os.f
-00000c70: 726f 6d20 746f 6765 7468 6572 2069 6d70  rom together imp
-00000c80: 6f72 7420 546f 6765 7468 6572 0a0a 636c  ort Together..cl
-00000c90: 6965 6e74 203d 2054 6f67 6574 6865 7228  ient = Together(
-00000ca0: 6170 695f 6b65 793d 6f73 2e65 6e76 6972  api_key=os.envir
-00000cb0: 6f6e 2e67 6574 2822 544f 4745 5448 4552  on.get("TOGETHER
-00000cc0: 5f41 5049 5f4b 4559 2229 290a 7374 7265  _API_KEY")).stre
-00000cd0: 616d 203d 2063 6c69 656e 742e 636f 6d70  am = client.comp
-00000ce0: 6c65 7469 6f6e 732e 6372 6561 7465 280a  letions.create(.
-00000cf0: 2020 2020 6d6f 6465 6c3d 2263 6f64 656c      model="codel
-00000d00: 6c61 6d61 2f43 6f64 654c 6c61 6d61 2d33  lama/CodeLlama-3
-00000d10: 3462 2d50 7974 686f 6e2d 6866 222c 0a20  4b-Python-hf",. 
-00000d20: 2020 2070 726f 6d70 743d 2257 7269 7465     prompt="Write
-00000d30: 2061 204e 6578 742e 6a73 2063 6f6d 706f   a Next.js compo
-00000d40: 6e65 6e74 2077 6974 6820 5461 696c 7769  nent with Tailwi
-00000d50: 6e64 4353 5320 666f 7220 6120 6865 6164  ndCSS for a head
-00000d60: 6572 2063 6f6d 706f 6e65 6e74 2e22 2c0a  er component.",.
-00000d70: 2020 2020 7374 7265 616d 3d54 7275 652c      stream=True,
-00000d80: 0a29 0a0a 666f 7220 6368 756e 6b20 696e  .)..for chunk in
-00000d90: 2073 7472 6561 6d3a 0a20 2020 2070 7269   stream:.    pri
-00000da0: 6e74 2863 6875 6e6b 2e63 686f 6963 6573  nt(chunk.choices
-00000db0: 5b30 5d2e 6465 6c74 612e 636f 6e74 656e  [0].delta.conten
-00000dc0: 7420 6f72 2022 222c 2065 6e64 3d22 222c  t or "", end="",
-00000dd0: 2066 6c75 7368 3d54 7275 6529 0a60 6060   flush=True).```
-00000de0: 0a0a 2323 2320 4173 796e 6320 7573 6167  ..### Async usag
-00000df0: 650a 0a60 6060 7079 7468 6f6e 0a69 6d70  e..```python.imp
-00000e00: 6f72 7420 6f73 2c20 6173 796e 6369 6f0a  ort os, asyncio.
-00000e10: 6672 6f6d 2074 6f67 6574 6865 7220 696d  from together im
-00000e20: 706f 7274 2041 7379 6e63 546f 6765 7468  port AsyncTogeth
-00000e30: 6572 0a0a 6173 796e 635f 636c 6965 6e74  er..async_client
-00000e40: 203d 2041 7379 6e63 546f 6765 7468 6572   = AsyncTogether
-00000e50: 2861 7069 5f6b 6579 3d6f 732e 656e 7669  (api_key=os.envi
-00000e60: 726f 6e2e 6765 7428 2254 4f47 4554 4845  ron.get("TOGETHE
-00000e70: 525f 4150 495f 4b45 5922 2929 0a70 726f  R_API_KEY")).pro
-00000e80: 6d70 7473 203d 205b 0a20 2020 2022 5772  mpts = [.    "Wr
-00000e90: 6974 6520 6120 4e65 7874 2e6a 7320 636f  ite a Next.js co
-00000ea0: 6d70 6f6e 656e 7420 7769 7468 2054 6169  mponent with Tai
-00000eb0: 6c77 696e 6443 5353 2066 6f72 2061 2068  lwindCSS for a h
-00000ec0: 6561 6465 7220 636f 6d70 6f6e 656e 742e  eader component.
-00000ed0: 222c 0a20 2020 2022 5772 6974 6520 6120  ",.    "Write a 
-00000ee0: 7079 7468 6f6e 2066 756e 6374 696f 6e20  python function 
-00000ef0: 666f 7220 7468 6520 6669 626f 6e61 6363  for the fibonacc
-00000f00: 6920 7365 7175 656e 6365 222c 0a5d 0a0a  i sequence",.]..
-00000f10: 6173 796e 6320 6465 6620 6173 796e 635f  async def async_
-00000f20: 6368 6174 5f63 6f6d 706c 6574 696f 6e28  chat_completion(
-00000f30: 7072 6f6d 7074 7329 3a0a 2020 2020 6173  prompts):.    as
-00000f40: 796e 635f 636c 6965 6e74 203d 2041 7379  ync_client = Asy
-00000f50: 6e63 546f 6765 7468 6572 2861 7069 5f6b  ncTogether(api_k
-00000f60: 6579 3d6f 732e 656e 7669 726f 6e2e 6765  ey=os.environ.ge
-00000f70: 7428 2254 4f47 4554 4845 525f 4150 495f  t("TOGETHER_API_
-00000f80: 4b45 5922 2929 0a20 2020 2074 6173 6b73  KEY")).    tasks
-00000f90: 203d 205b 0a20 2020 2020 2020 2061 7379   = [.        asy
-00000fa0: 6e63 5f63 6c69 656e 742e 636f 6d70 6c65  nc_client.comple
-00000fb0: 7469 6f6e 732e 6372 6561 7465 280a 2020  tions.create(.  
-00000fc0: 2020 2020 2020 2020 2020 6d6f 6465 6c3d            model=
-00000fd0: 2263 6f64 656c 6c61 6d61 2f43 6f64 654c  "codellama/CodeL
-00000fe0: 6c61 6d61 2d33 3462 2d50 7974 686f 6e2d  lama-34b-Python-
-00000ff0: 6866 222c 0a20 2020 2020 2020 2020 2020  hf",.           
-00001000: 2070 726f 6d70 743d 7072 6f6d 7074 2c0a   prompt=prompt,.
-00001010: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00001020: 2020 666f 7220 7072 6f6d 7074 2069 6e20    for prompt in 
-00001030: 7072 6f6d 7074 730a 2020 2020 5d0a 2020  prompts.    ].  
-00001040: 2020 7265 7370 6f6e 7365 7320 3d20 6177    responses = aw
-00001050: 6169 7420 6173 796e 6369 6f2e 6761 7468  ait asyncio.gath
-00001060: 6572 282a 7461 736b 7329 0a0a 2020 2020  er(*tasks)..    
-00001070: 666f 7220 7265 7370 6f6e 7365 2069 6e20  for response in 
-00001080: 7265 7370 6f6e 7365 733a 0a20 2020 2020  responses:.     
-00001090: 2020 2070 7269 6e74 2872 6573 706f 6e73     print(respons
-000010a0: 652e 6368 6f69 6365 735b 305d 2e74 6578  e.choices[0].tex
-000010b0: 7429 0a0a 6173 796e 6369 6f2e 7275 6e28  t)..asyncio.run(
-000010c0: 6173 796e 635f 6368 6174 5f63 6f6d 706c  async_chat_compl
-000010d0: 6574 696f 6e28 7072 6f6d 7074 7329 290a  etion(prompts)).
-000010e0: 6060 600a 0a23 2320 496d 6167 6520 6765  ```..## Image ge
-000010f0: 6e65 7261 7469 6f6e 0a0a 6060 6070 7974  neration..```pyt
-00001100: 686f 6e0a 696d 706f 7274 206f 730a 6672  hon.import os.fr
-00001110: 6f6d 2074 6f67 6574 6865 7220 696d 706f  om together impo
-00001120: 7274 2054 6f67 6574 6865 720a 0a63 6c69  rt Together..cli
-00001130: 656e 7420 3d20 546f 6765 7468 6572 2861  ent = Together(a
-00001140: 7069 5f6b 6579 3d6f 732e 656e 7669 726f  pi_key=os.enviro
-00001150: 6e2e 6765 7428 2254 4f47 4554 4845 525f  n.get("TOGETHER_
-00001160: 4150 495f 4b45 5922 2929 0a0a 7265 7370  API_KEY"))..resp
-00001170: 6f6e 7365 203d 2063 6c69 656e 742e 696d  onse = client.im
-00001180: 6167 6573 2e67 656e 6572 6174 6528 0a20  ages.generate(. 
-00001190: 2020 2070 726f 6d70 743d 2273 7061 6365     prompt="space
-000011a0: 2072 6f62 6f74 7322 2c0a 2020 2020 6d6f   robots",.    mo
-000011b0: 6465 6c3d 2273 7461 6269 6c69 7479 6169  del="stabilityai
-000011c0: 2f73 7461 626c 652d 6469 6666 7573 696f  /stable-diffusio
-000011d0: 6e2d 786c 2d62 6173 652d 312e 3022 2c0a  n-xl-base-1.0",.
-000011e0: 2020 2020 7374 6570 733d 3130 2c0a 2020      steps=10,.  
-000011f0: 2020 6e3d 342c 0a29 0a70 7269 6e74 2872    n=4,.).print(r
-00001200: 6573 706f 6e73 652e 6461 7461 5b30 5d2e  esponse.data[0].
-00001210: 6236 345f 6a73 6f6e 290a 6060 600a 0a23  b64_json).```..#
-00001220: 2320 456d 6265 6464 696e 6773 0a0a 6060  # Embeddings..``
-00001230: 6070 7974 686f 6e0a 6672 6f6d 2074 7970  `python.from typ
-00001240: 696e 6720 696d 706f 7274 204c 6973 740a  ing import List.
-00001250: 6672 6f6d 2074 6f67 6574 6865 7220 696d  from together im
-00001260: 706f 7274 2054 6f67 6574 6865 720a 0a63  port Together..c
-00001270: 6c69 656e 7420 3d20 546f 6765 7468 6572  lient = Together
-00001280: 2861 7069 5f6b 6579 3d6f 732e 656e 7669  (api_key=os.envi
-00001290: 726f 6e2e 6765 7428 2254 4f47 4554 4845  ron.get("TOGETHE
-000012a0: 525f 4150 495f 4b45 5922 2929 0a0a 6465  R_API_KEY"))..de
-000012b0: 6620 6765 745f 656d 6265 6464 696e 6773  f get_embeddings
-000012c0: 2874 6578 7473 3a20 4c69 7374 5b73 7472  (texts: List[str
-000012d0: 5d2c 206d 6f64 656c 3a20 7374 7229 202d  ], model: str) -
-000012e0: 3e20 4c69 7374 5b4c 6973 745b 666c 6f61  > List[List[floa
-000012f0: 745d 5d3a 0a20 2020 2074 6578 7473 203d  t]]:.    texts =
-00001300: 205b 7465 7874 2e72 6570 6c61 6365 2822   [text.replace("
-00001310: 5c6e 222c 2022 2022 2920 666f 7220 7465  \n", " ") for te
-00001320: 7874 2069 6e20 7465 7874 735d 0a20 2020  xt in texts].   
-00001330: 206f 7574 7075 7473 203d 2063 6c69 656e   outputs = clien
-00001340: 742e 656d 6265 6464 696e 6773 2e63 7265  t.embeddings.cre
-00001350: 6174 6528 6d6f 6465 6c3d 6d6f 6465 6c2c  ate(model=model,
-00001360: 2069 6e70 7574 203d 2074 6578 7473 290a   input = texts).
-00001370: 2020 2020 7265 7475 726e 205b 6f75 7470      return [outp
-00001380: 7574 732e 6461 7461 5b69 5d2e 656d 6265  uts.data[i].embe
-00001390: 6464 696e 6720 666f 7220 6920 696e 2072  dding for i in r
-000013a0: 616e 6765 286c 656e 2874 6578 7473 2929  ange(len(texts))
-000013b0: 5d0a 0a69 6e70 7574 5f74 6578 7473 203d  ]..input_texts =
-000013c0: 205b 274f 7572 2073 6f6c 6172 2073 7973   ['Our solar sys
-000013d0: 7465 6d20 6f72 6269 7473 2074 6865 204d  tem orbits the M
-000013e0: 696c 6b79 2057 6179 2067 616c 6178 7920  ilky Way galaxy 
-000013f0: 6174 2061 626f 7574 2035 3135 2c30 3030  at about 515,000
-00001400: 206d 7068 275d 0a65 6d62 6564 6469 6e67   mph'].embedding
-00001410: 7320 3d20 6765 745f 656d 6265 6464 696e  s = get_embeddin
-00001420: 6773 2869 6e70 7574 5f74 6578 7473 2c20  gs(input_texts, 
-00001430: 6d6f 6465 6c3d 2774 6f67 6574 6865 7263  model='togetherc
-00001440: 6f6d 7075 7465 722f 6d32 2d62 6572 742d  omputer/m2-bert-
-00001450: 3830 4d2d 386b 2d72 6574 7269 6576 616c  80M-8k-retrieval
-00001460: 2729 0a0a 7072 696e 7428 656d 6265 6464  ')..print(embedd
-00001470: 696e 6773 290a 6060 600a 0a23 2320 4669  ings).```..## Fi
-00001480: 6c65 730a 0a54 6865 2066 696c 6573 2041  les..The files A
-00001490: 5049 2069 7320 7573 6564 2066 6f72 2066  PI is used for f
-000014a0: 696e 652d 7475 6e69 6e67 2061 6e64 2061  ine-tuning and a
-000014b0: 6c6c 6f77 7320 6465 7665 6c6f 7065 7273  llows developers
-000014c0: 2074 6f20 7570 6c6f 6164 2064 6174 6120   to upload data 
-000014d0: 746f 2066 696e 652d 7475 6e65 206f 6e2e  to fine-tune on.
-000014e0: 2049 7420 616c 736f 2068 6173 2073 6576   It also has sev
-000014f0: 6572 616c 206d 6574 686f 6473 2074 6f20  eral methods to 
-00001500: 6c69 7374 2061 6c6c 2066 696c 6573 2c20  list all files, 
-00001510: 7265 7472 6976 6520 6669 6c65 732c 2061  retrive files, a
-00001520: 6e64 2064 656c 6574 6520 6669 6c65 732e  nd delete files.
-00001530: 2050 6c65 6173 6520 7265 6665 7220 746f   Please refer to
-00001540: 206f 7572 2066 696e 652d 7475 6e69 6e67   our fine-tuning
-00001550: 2064 6f63 7320 5b68 6572 655d 2868 7474   docs [here](htt
-00001560: 7073 3a2f 2f64 6f63 732e 746f 6765 7468  ps://docs.togeth
-00001570: 6572 2e61 692f 646f 6373 2f66 696e 652d  er.ai/docs/fine-
-00001580: 7475 6e69 6e67 2d70 7974 686f 6e29 2e0a  tuning-python)..
-00001590: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
-000015a0: 7420 6f73 0a66 726f 6d20 746f 6765 7468  t os.from togeth
-000015b0: 6572 2069 6d70 6f72 7420 546f 6765 7468  er import Togeth
-000015c0: 6572 0a0a 636c 6965 6e74 203d 2054 6f67  er..client = Tog
-000015d0: 6574 6865 7228 6170 695f 6b65 793d 6f73  ether(api_key=os
-000015e0: 2e65 6e76 6972 6f6e 2e67 6574 2822 544f  .environ.get("TO
-000015f0: 4745 5448 4552 5f41 5049 5f4b 4559 2229  GETHER_API_KEY")
-00001600: 290a 0a63 6c69 656e 742e 6669 6c65 732e  )..client.files.
-00001610: 7570 6c6f 6164 2866 696c 653d 2273 6f6d  upload(file="som
-00001620: 6564 6174 612e 6a73 6f6e 6c22 2920 2320  edata.jsonl") # 
-00001630: 7570 6c6f 6164 7320 6120 6669 6c65 0a63  uploads a file.c
-00001640: 6c69 656e 742e 6669 6c65 732e 6c69 7374  lient.files.list
-00001650: 2829 2023 206c 6973 7473 2061 6c6c 2075  () # lists all u
-00001660: 706c 6f61 6465 6420 6669 6c65 730a 636c  ploaded files.cl
-00001670: 6965 6e74 2e66 696c 6573 2e72 6574 7269  ient.files.retri
-00001680: 6576 6528 6964 3d22 6669 6c65 2d64 3064  eve(id="file-d0d
-00001690: 3331 3863 622d 6237 6439 2d34 3933 612d  318cb-b7d9-493a-
-000016a0: 6264 3730 2d31 6366 6530 3839 6433 3831  bd70-1cfe089d381
-000016b0: 3522 2920 2320 7265 7472 6965 7665 7320  5") # retrieves 
-000016c0: 6120 7370 6563 6966 6963 2066 696c 650a  a specific file.
-000016d0: 636c 6965 6e74 2e66 696c 6573 2e72 6574  client.files.ret
-000016e0: 7269 6576 655f 636f 6e74 656e 7428 6964  rieve_content(id
-000016f0: 3d22 6669 6c65 2d64 3064 3331 3863 622d  ="file-d0d318cb-
-00001700: 6237 6439 2d34 3933 612d 6264 3730 2d31  b7d9-493a-bd70-1
-00001710: 6366 6530 3839 6433 3831 3522 2920 2320  cfe089d3815") # 
-00001720: 7265 7472 6965 7665 7320 636f 6e74 656e  retrieves conten
-00001730: 7420 6f66 2061 2073 7065 6369 6669 6320  t of a specific 
-00001740: 6669 6c65 0a63 6c69 656e 742e 6669 6c65  file.client.file
-00001750: 732e 6465 6c65 7465 2869 643d 2266 696c  s.delete(id="fil
-00001760: 652d 6430 6433 3138 6362 2d62 3764 392d  e-d0d318cb-b7d9-
-00001770: 3439 3361 2d62 6437 302d 3163 6665 3038  493a-bd70-1cfe08
-00001780: 3964 3338 3135 2229 2023 2064 656c 6574  9d3815") # delet
-00001790: 6573 2061 2066 696c 650a 6060 600a 0a23  es a file.```..#
-000017a0: 2320 4669 6e65 2d74 756e 6573 0a0a 5468  # Fine-tunes..Th
-000017b0: 6520 6669 6e65 7475 6e65 2041 5049 2069  e finetune API i
-000017c0: 7320 7573 6564 2066 6f72 2066 696e 652d  s used for fine-
-000017d0: 7475 6e69 6e67 2061 6e64 2061 6c6c 6f77  tuning and allow
-000017e0: 7320 6465 7665 6c6f 7065 7273 2074 6f20  s developers to 
-000017f0: 6372 6561 7465 2066 696e 6574 756e 696e  create finetunin
-00001800: 6720 6a6f 6273 2e20 4974 2061 6c73 6f20  g jobs. It also 
-00001810: 6861 7320 7365 7665 7261 6c20 6d65 7468  has several meth
-00001820: 6f64 7320 746f 206c 6973 7420 616c 6c20  ods to list all 
-00001830: 6a6f 6273 2c20 7265 7472 6976 6520 7374  jobs, retrive st
-00001840: 6174 7573 6573 2061 6e64 2067 6574 2063  atuses and get c
-00001850: 6865 636b 706f 696e 7473 2e20 506c 6561  heckpoints. Plea
-00001860: 7365 2072 6566 6572 2074 6f20 6f75 7220  se refer to our 
-00001870: 6669 6e65 2d74 756e 696e 6720 646f 6373  fine-tuning docs
-00001880: 205b 6865 7265 5d28 6874 7470 733a 2f2f   [here](https://
-00001890: 646f 6373 2e74 6f67 6574 6865 722e 6169  docs.together.ai
-000018a0: 2f64 6f63 732f 6669 6e65 2d74 756e 696e  /docs/fine-tunin
-000018b0: 672d 7079 7468 6f6e 292e 0a0a 6060 6070  g-python)...```p
-000018c0: 7974 686f 6e0a 696d 706f 7274 206f 730a  ython.import os.
-000018d0: 6672 6f6d 2074 6f67 6574 6865 7220 696d  from together im
-000018e0: 706f 7274 2054 6f67 6574 6865 720a 0a63  port Together..c
-000018f0: 6c69 656e 7420 3d20 546f 6765 7468 6572  lient = Together
-00001900: 2861 7069 5f6b 6579 3d6f 732e 656e 7669  (api_key=os.envi
-00001910: 726f 6e2e 6765 7428 2254 4f47 4554 4845  ron.get("TOGETHE
-00001920: 525f 4150 495f 4b45 5922 2929 0a0a 636c  R_API_KEY"))..cl
-00001930: 6965 6e74 2e66 696e 655f 7475 6e69 6e67  ient.fine_tuning
-00001940: 2e63 7265 6174 6528 0a20 2074 7261 696e  .create(.  train
-00001950: 696e 675f 6669 6c65 203d 2027 6669 6c65  ing_file = 'file
-00001960: 2d64 3064 3331 3863 622d 6237 6439 2d34  -d0d318cb-b7d9-4
-00001970: 3933 612d 6264 3730 2d31 6366 6530 3839  93a-bd70-1cfe089
-00001980: 6433 3831 3527 2c0a 2020 6d6f 6465 6c20  d3815',.  model 
-00001990: 3d20 276d 6973 7472 616c 6169 2f4d 6978  = 'mistralai/Mix
-000019a0: 7472 616c 2d38 7837 422d 496e 7374 7275  tral-8x7B-Instru
-000019b0: 6374 2d76 302e 3127 2c0a 2020 6e5f 6570  ct-v0.1',.  n_ep
-000019c0: 6f63 6873 203d 2033 2c0a 2020 6e5f 6368  ochs = 3,.  n_ch
-000019d0: 6563 6b70 6f69 6e74 7320 3d20 312c 0a20  eckpoints = 1,. 
-000019e0: 2062 6174 6368 5f73 697a 6520 3d20 342c   batch_size = 4,
-000019f0: 0a20 206c 6561 726e 696e 675f 7261 7465  .  learning_rate
-00001a00: 203d 2031 652d 352c 0a20 2073 7566 6669   = 1e-5,.  suffi
-00001a10: 7820 3d20 276d 792d 6465 6d6f 2d66 696e  x = 'my-demo-fin
-00001a20: 6574 756e 6527 2c0a 2020 7761 6e64 625f  etune',.  wandb_
-00001a30: 6170 695f 6b65 7920 3d20 2731 6132 6233  api_key = '1a2b3
-00001a40: 6334 6435 652e 2e2e 2e2e 2e2e 272c 0a29  c4d5e.......',.)
-00001a50: 0a63 6c69 656e 742e 6669 6e65 5f74 756e  .client.fine_tun
-00001a60: 696e 672e 6c69 7374 2829 2023 206c 6973  ing.list() # lis
-00001a70: 7473 2061 6c6c 2066 696e 652d 7475 6e65  ts all fine-tune
-00001a80: 6420 6a6f 6273 0a63 6c69 656e 742e 6669  d jobs.client.fi
-00001a90: 6e65 5f74 756e 696e 672e 7265 7472 6965  ne_tuning.retrie
-00001aa0: 7665 2869 643d 2266 742d 6336 3661 3563  ve(id="ft-c66a5c
-00001ab0: 3138 2d31 6436 642d 3433 6339 2d39 3462  18-1d6d-43c9-94b
-00001ac0: 642d 3332 6437 3536 3432 3562 3462 2229  d-32d756425b4b")
-00001ad0: 2023 2072 6574 7269 6576 6573 2069 6e66   # retrieves inf
-00001ae0: 6f72 6d61 7469 6f6e 206f 6e20 6669 6e65  ormation on fine
-00001af0: 7475 6e65 2065 7665 6e74 0a63 6c69 656e  tune event.clien
-00001b00: 742e 6669 6e65 5f74 756e 696e 672e 6361  t.fine_tuning.ca
-00001b10: 6e63 656c 2869 643d 2266 742d 6336 3661  ncel(id="ft-c66a
-00001b20: 3563 3138 2d31 6436 642d 3433 6339 2d39  5c18-1d6d-43c9-9
-00001b30: 3462 642d 3332 6437 3536 3432 3562 3462  4bd-32d756425b4b
-00001b40: 2229 2023 2043 616e 6365 6c73 2061 2066  ") # Cancels a f
-00001b50: 696e 652d 7475 6e69 6e67 206a 6f62 0a63  ine-tuning job.c
-00001b60: 6c69 656e 742e 6669 6e65 5f74 756e 696e  lient.fine_tunin
-00001b70: 672e 6c69 7374 5f65 7665 6e74 7328 6964  g.list_events(id
-00001b80: 3d22 6674 2d63 3636 6135 6331 382d 3164  ="ft-c66a5c18-1d
-00001b90: 3664 2d34 3363 392d 3934 6264 2d33 3264  6d-43c9-94bd-32d
-00001ba0: 3735 3634 3235 6234 6222 2920 2320 204c  756425b4b") #  L
-00001bb0: 6973 7473 2065 7665 6e74 7320 6f66 2061  ists events of a
-00001bc0: 2066 696e 652d 7475 6e65 206a 6f62 0a63   fine-tune job.c
-00001bd0: 6c69 656e 742e 6669 6e65 5f74 756e 696e  lient.fine_tunin
-00001be0: 672e 646f 776e 6c6f 6164 2869 643d 2266  g.download(id="f
-00001bf0: 742d 6336 3661 3563 3138 2d31 6436 642d  t-c66a5c18-1d6d-
-00001c00: 3433 6339 2d39 3462 642d 3332 6437 3536  43c9-94bd-32d756
-00001c10: 3432 3562 3462 2229 2023 2064 6f77 6e6c  425b4b") # downl
-00001c20: 6f61 6473 2063 6f6d 7072 6573 7365 6420  oads compressed 
-00001c30: 6669 6e65 2d74 756e 6564 206d 6f64 656c  fine-tuned model
-00001c40: 206f 7220 6368 6563 6b70 6f69 6e74 2074   or checkpoint t
-00001c50: 6f20 6c6f 6361 6c20 6469 736b 0a60 6060  o local disk.```
-00001c60: 0a0a 2323 204d 6f64 656c 730a 0a54 6869  ..## Models..Thi
-00001c70: 7320 6c69 7374 7320 616c 6c20 7468 6520  s lists all the 
-00001c80: 6d6f 6465 6c73 2074 6861 7420 546f 6765  models that Toge
-00001c90: 7468 6572 2073 7570 706f 7274 732e 0a0a  ther supports...
-00001ca0: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
-00001cb0: 206f 730a 6672 6f6d 2074 6f67 6574 6865   os.from togethe
-00001cc0: 7220 696d 706f 7274 2054 6f67 6574 6865  r import Togethe
-00001cd0: 720a 0a63 6c69 656e 7420 3d20 546f 6765  r..client = Toge
-00001ce0: 7468 6572 2861 7069 5f6b 6579 3d6f 732e  ther(api_key=os.
-00001cf0: 656e 7669 726f 6e2e 6765 7428 2254 4f47  environ.get("TOG
-00001d00: 4554 4845 525f 4150 495f 4b45 5922 2929  ETHER_API_KEY"))
-00001d10: 0a0a 6d6f 6465 6c73 203d 2063 6c69 656e  ..models = clien
-00001d20: 742e 6d6f 6465 6c73 2e6c 6973 7428 290a  t.models.list().
-00001d30: 0a66 6f72 206d 6f64 656c 2069 6e20 6d6f  .for model in mo
-00001d40: 6465 6c73 3a0a 2020 2020 7072 696e 7428  dels:.    print(
-00001d50: 6d6f 6465 6c29 0a60 6060 0a0a 2320 5573  model).```..# Us
-00001d60: 6167 6520 e280 9320 434c 490a 0a23 2320  age ... CLI..## 
-00001d70: 4368 6174 2043 6f6d 706c 6574 696f 6e73  Chat Completions
-00001d80: 0a0a 6060 6062 6173 680a 746f 6765 7468  ..```bash.togeth
-00001d90: 6572 2063 6861 742e 636f 6d70 6c65 7469  er chat.completi
-00001da0: 6f6e 7320 5c0a 2020 2d2d 6d65 7373 6167  ons \.  --messag
-00001db0: 6520 2273 7973 7465 6d22 2022 596f 7520  e "system" "You 
-00001dc0: 6172 6520 6120 6865 6c70 6675 6c20 6173  are a helpful as
-00001dd0: 7369 7374 616e 7420 6e61 6d65 6420 546f  sistant named To
-00001de0: 6765 7468 6572 2220 5c0a 2020 2d2d 6d65  gether" \.  --me
-00001df0: 7373 6167 6520 2275 7365 7222 2022 5768  ssage "user" "Wh
-00001e00: 6174 2069 7320 796f 7572 206e 616d 653f  at is your name?
-00001e10: 2220 5c0a 2020 2d2d 6d6f 6465 6c20 6d69  " \.  --model mi
-00001e20: 7374 7261 6c61 692f 4d69 7874 7261 6c2d  stralai/Mixtral-
-00001e30: 3878 3742 2d49 6e73 7472 7563 742d 7630  8x7B-Instruct-v0
-00001e40: 2e31 0a60 6060 0a0a 5468 6520 4368 6174  .1.```..The Chat
-00001e50: 2043 6f6d 706c 6574 696f 6e73 2043 4c49   Completions CLI
-00001e60: 2065 6e61 626c 6573 2073 7472 6561 6d69   enables streami
-00001e70: 6e67 2074 6f6b 656e 7320 746f 2073 7464  ng tokens to std
-00001e80: 6f75 7420 6279 2064 6566 6175 6c74 2e20  out by default. 
-00001e90: 546f 2064 6973 6162 6c65 2073 7472 6561  To disable strea
-00001ea0: 6d69 6e67 2c20 7573 6520 602d 2d6e 6f2d  ming, use `--no-
-00001eb0: 7374 7265 616d 602e 0a0a 2323 2043 6f6d  stream`...## Com
-00001ec0: 706c 6574 696f 6e73 0a0a 6060 6062 6173  pletions..```bas
-00001ed0: 680a 746f 6765 7468 6572 2063 6f6d 706c  h.together compl
-00001ee0: 6574 696f 6e73 205c 0a20 2022 4c61 7267  etions \.  "Larg
-00001ef0: 6520 6c61 6e67 7561 6765 206d 6f64 656c  e language model
-00001f00: 7320 6172 6520 2220 5c0a 2020 2d2d 6d6f  s are " \.  --mo
-00001f10: 6465 6c20 6d69 7374 7261 6c61 692f 4d69  del mistralai/Mi
-00001f20: 7874 7261 6c2d 3878 3742 2d76 302e 3120  xtral-8x7B-v0.1 
-00001f30: 5c0a 2020 2d2d 6d61 782d 746f 6b65 6e73  \.  --max-tokens
-00001f40: 2035 3132 205c 0a20 202d 2d73 746f 7020   512 \.  --stop 
-00001f50: 222e 220a 6060 600a 0a54 6865 2043 6f6d  ".".```..The Com
-00001f60: 706c 6574 696f 6e73 2043 4c49 2065 6e61  pletions CLI ena
-00001f70: 626c 6573 2073 7472 6561 6d69 6e67 2074  bles streaming t
-00001f80: 6f6b 656e 7320 746f 2073 7464 6f75 7420  okens to stdout 
-00001f90: 6279 2064 6566 6175 6c74 2e20 546f 2064  by default. To d
-00001fa0: 6973 6162 6c65 2073 7472 6561 6d69 6e67  isable streaming
-00001fb0: 2c20 7573 6520 602d 2d6e 6f2d 7374 7265  , use `--no-stre
-00001fc0: 616d 602e 0a0a 2323 2049 6d61 6765 2047  am`...## Image G
-00001fd0: 656e 6572 6174 696f 6e73 0a0a 6060 6062  enerations..```b
-00001fe0: 6173 680a 746f 6765 7468 6572 2069 6d61  ash.together ima
-00001ff0: 6765 7320 6765 6e65 7261 7465 205c 0a20  ges generate \. 
-00002000: 2022 7370 6163 6520 726f 626f 7473 2220   "space robots" 
-00002010: 5c0a 2020 2d2d 6d6f 6465 6c20 7374 6162  \.  --model stab
-00002020: 696c 6974 7961 692f 7374 6162 6c65 2d64  ilityai/stable-d
-00002030: 6966 6675 7369 6f6e 2d78 6c2d 6261 7365  iffusion-xl-base
-00002040: 2d31 2e30 205c 0a20 202d 2d6e 2034 0a60  -1.0 \.  --n 4.`
-00002050: 6060 0a0a 5468 6520 696d 6167 6520 6973  ``..The image is
-00002060: 206f 7065 6e65 6420 696e 2074 6865 2064   opened in the d
-00002070: 6566 6175 6c74 2069 6d61 6765 2076 6965  efault image vie
-00002080: 7765 7220 6279 2064 6566 6175 6c74 2e20  wer by default. 
-00002090: 546f 2064 6973 6162 6c65 2074 6869 732c  To disable this,
-000020a0: 2075 7365 2060 2d2d 6e6f 2d73 686f 7760   use `--no-show`
-000020b0: 2e0a 0a23 2320 4669 6c65 730a 0a60 6060  ...## Files..```
-000020c0: 6261 7368 0a23 2048 656c 700a 746f 6765  bash.# Help.toge
-000020d0: 7468 6572 2066 696c 6573 202d 2d68 656c  ther files --hel
-000020e0: 700a 0a23 2043 6865 636b 2066 696c 650a  p..# Check file.
-000020f0: 746f 6765 7468 6572 2066 696c 6573 2063  together files c
-00002100: 6865 636b 2065 7861 6d70 6c65 2e6a 736f  heck example.jso
-00002110: 6e6c 0a0a 2320 5570 6c6f 6164 2066 696c  nl..# Upload fil
-00002120: 650a 746f 6765 7468 6572 2066 696c 6573  e.together files
-00002130: 2075 706c 6f61 6420 6578 616d 706c 652e   upload example.
-00002140: 6a73 6f6e 6c0a 0a23 204c 6973 7420 6669  jsonl..# List fi
-00002150: 6c65 730a 746f 6765 7468 6572 2066 696c  les.together fil
-00002160: 6573 206c 6973 740a 0a23 2052 6574 7269  es list..# Retri
-00002170: 6576 6520 6669 6c65 206d 6574 6164 6174  eve file metadat
-00002180: 610a 746f 6765 7468 6572 2066 696c 6573  a.together files
-00002190: 2072 6574 7269 6576 6520 6669 6c65 2d36   retrieve file-6
-000021a0: 6635 3066 3964 312d 3562 3935 2d34 3136  f50f9d1-5b95-416
-000021b0: 632d 3930 3430 2d30 3739 3962 3262 3462  c-9040-0799b2b4b
-000021c0: 3839 340a 0a23 2052 6574 7269 6576 6520  894..# Retrieve 
-000021d0: 6669 6c65 2063 6f6e 7465 6e74 0a74 6f67  file content.tog
-000021e0: 6574 6865 7220 6669 6c65 7320 7265 7472  ether files retr
-000021f0: 6965 7665 2d63 6f6e 7465 6e74 2066 696c  ieve-content fil
-00002200: 652d 3666 3530 6639 6431 2d35 6239 352d  e-6f50f9d1-5b95-
-00002210: 3431 3663 2d39 3034 302d 3037 3939 6232  416c-9040-0799b2
-00002220: 6234 6238 3934 0a0a 2320 4465 6c65 7465  b4b894..# Delete
-00002230: 2072 656d 6f74 6520 6669 6c65 0a74 6f67   remote file.tog
-00002240: 6574 6865 7220 6669 6c65 7320 6465 6c65  ether files dele
-00002250: 7465 2066 696c 652d 3666 3530 6639 6431  te file-6f50f9d1
-00002260: 2d35 6239 352d 3431 3663 2d39 3034 302d  -5b95-416c-9040-
-00002270: 3037 3939 6232 6234 6238 3934 0a60 6060  0799b2b4b894.```
-00002280: 0a0a 2323 2046 696e 652d 7475 6e69 6e67  ..## Fine-tuning
-00002290: 0a0a 6060 6062 6173 680a 2320 4865 6c70  ..```bash.# Help
-000022a0: 0a74 6f67 6574 6865 7220 6669 6e65 2d74  .together fine-t
-000022b0: 756e 696e 6720 2d2d 6865 6c70 0a0a 2320  uning --help..# 
-000022c0: 4372 6561 7465 2066 696e 652d 7475 6e65  Create fine-tune
-000022d0: 206a 6f62 0a74 6f67 6574 6865 7220 6669   job.together fi
-000022e0: 6e65 2d74 756e 696e 6720 6372 6561 7465  ne-tuning create
-000022f0: 205c 0a20 202d 2d6d 6f64 656c 2074 6f67   \.  --model tog
-00002300: 6574 6865 7263 6f6d 7075 7465 722f 6c6c  ethercomputer/ll
-00002310: 616d 612d 322d 3762 2d63 6861 7420 5c0a  ama-2-7b-chat \.
-00002320: 2020 2d2d 7472 6169 6e69 6e67 2d66 696c    --training-fil
-00002330: 6520 6669 6c65 2d37 3131 6438 3732 342d  e file-711d8724-
-00002340: 6233 6533 2d34 6165 322d 6235 3136 2d39  b3e3-4ae2-b516-9
-00002350: 3438 3431 3935 3831 3137 640a 0a23 204c  4841958117d..# L
-00002360: 6973 7420 6669 6e65 2d74 756e 6520 6a6f  ist fine-tune jo
-00002370: 6273 0a74 6f67 6574 6865 7220 6669 6e65  bs.together fine
-00002380: 2d74 756e 696e 6720 6c69 7374 0a0a 2320  -tuning list..# 
-00002390: 5265 7472 6965 7665 2066 696e 652d 7475  Retrieve fine-tu
-000023a0: 6e65 206a 6f62 2064 6574 6169 6c73 0a74  ne job details.t
-000023b0: 6f67 6574 6865 7220 6669 6e65 2d74 756e  ogether fine-tun
-000023c0: 696e 6720 7265 7472 6965 7665 2066 742d  ing retrieve ft-
-000023d0: 6336 3661 3563 3138 2d31 6436 642d 3433  c66a5c18-1d6d-43
-000023e0: 6339 2d39 3462 642d 3332 6437 3536 3432  c9-94bd-32d75642
-000023f0: 3562 3462 0a0a 2320 4c69 7374 2066 696e  5b4b..# List fin
-00002400: 652d 7475 6e65 206a 6f62 2065 7665 6e74  e-tune job event
-00002410: 730a 746f 6765 7468 6572 2066 696e 652d  s.together fine-
-00002420: 7475 6e69 6e67 206c 6973 742d 6576 656e  tuning list-even
-00002430: 7473 2066 742d 6336 3661 3563 3138 2d31  ts ft-c66a5c18-1
-00002440: 6436 642d 3433 6339 2d39 3462 642d 3332  d6d-43c9-94bd-32
-00002450: 6437 3536 3432 3562 3462 0a0a 2320 4361  d756425b4b..# Ca
-00002460: 6e63 656c 2072 756e 6e69 6e67 206a 6f62  ncel running job
-00002470: 0a74 6f67 6574 6865 7220 6669 6e65 2d74  .together fine-t
-00002480: 756e 696e 6720 6361 6e63 656c 2066 742d  uning cancel ft-
-00002490: 6336 3661 3563 3138 2d31 6436 642d 3433  c66a5c18-1d6d-43
-000024a0: 6339 2d39 3462 642d 3332 6437 3536 3432  c9-94bd-32d75642
-000024b0: 3562 3462 0a0a 2320 446f 776e 6c6f 6164  5b4b..# Download
-000024c0: 2066 696e 652d 7475 6e65 6420 6d6f 6465   fine-tuned mode
-000024d0: 6c20 7765 6967 6874 730a 746f 6765 7468  l weights.togeth
-000024e0: 6572 2066 696e 652d 7475 6e69 6e67 2064  er fine-tuning d
-000024f0: 6f77 6e6c 6f61 6420 6674 2d63 3636 6135  ownload ft-c66a5
-00002500: 6331 382d 3164 3664 2d34 3363 392d 3934  c18-1d6d-43c9-94
-00002510: 6264 2d33 3264 3735 3634 3235 6234 620a  bd-32d756425b4b.
-00002520: 6060 600a 0a23 2320 4d6f 6465 6c73 0a0a  ```..## Models..
-00002530: 6060 6062 6173 680a 2320 4865 6c70 0a74  ```bash.# Help.t
-00002540: 6f67 6574 6865 7220 6d6f 6465 6c73 202d  ogether models -
-00002550: 2d68 656c 700a 0a23 204c 6973 7420 6d6f  -help..# List mo
-00002560: 6465 6c73 0a74 6f67 6574 6865 7220 6d6f  dels.together mo
-00002570: 6465 6c73 206c 6973 740a 6060 600a 0a23  dels list.```..#
-00002580: 2320 436f 6e74 7269 6275 7469 6e67 0a0a  # Contributing..
-00002590: 5265 6665 7220 746f 2074 6865 205b 436f  Refer to the [Co
-000025a0: 6e74 7269 6275 7469 6e67 2047 7569 6465  ntributing Guide
-000025b0: 5d28 434f 4e54 5249 4255 5449 4e47 2e6d  ](CONTRIBUTING.m
-000025c0: 6429 0a                                  d).
+00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000010: 6572 223e 0a20 203c 6120 6872 6566 3d22  er">.  <a href="
+00000020: 6874 7470 733a 2f2f 7777 772e 746f 6765  https://www.toge
+00000030: 7468 6572 2e61 692f 223e 0a20 2020 203c  ther.ai/">.    <
+00000040: 696d 6720 616c 743d 2274 6f67 6574 6865  img alt="togethe
+00000050: 722e 6169 2220 6865 6967 6874 3d22 3130  r.ai" height="10
+00000060: 3070 7822 2073 7263 3d22 6874 7470 733a  0px" src="https:
+00000070: 2f2f 6173 7365 7473 2d67 6c6f 6261 6c2e  //assets-global.
+00000080: 7765 6273 6974 652d 6669 6c65 732e 636f  website-files.co
+00000090: 6d2f 3634 6636 6632 6330 6533 6634 6335  m/64f6f2c0e3f4c5
+000000a0: 6139 3163 3165 3832 3361 2f36 3534 3639  a91c1e823a/65469
+000000b0: 3364 3536 3934 3934 3931 3263 6663 3063  3d569494912cfc0c
+000000c0: 3064 345f 6661 7669 636f 6e2e 7376 6722  0d4_favicon.svg"
+000000d0: 3e0a 2020 3c2f 613e 0a3c 2f64 6976 3e0a  >.  </a>.</div>.
+000000e0: 0a23 2054 6f67 6574 6865 7220 5079 7468  .# Together Pyth
+000000f0: 6f6e 2041 5049 206c 6962 7261 7279 0a0a  on API library..
+00000100: 5b21 5b50 7950 4920 7665 7273 696f 6e5d  [![PyPI version]
+00000110: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000120: 656c 6473 2e69 6f2f 7079 7069 2f76 2f74  elds.io/pypi/v/t
+00000130: 6f67 6574 6865 722e 7376 6729 5d28 6874  ogether.svg)](ht
+00000140: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00000150: 726f 6a65 6374 2f74 6f67 6574 6865 722f  roject/together/
+00000160: 290a 5b21 5b44 6973 636f 7264 5d28 6874  ).[![Discord](ht
+00000170: 7470 733a 2f2f 6463 6261 6467 652e 7665  tps://dcbadge.ve
+00000180: 7263 656c 2e61 7070 2f61 7069 2f73 6572  rcel.app/api/ser
+00000190: 7665 722f 3952 6b36 7353 6557 4547 3f73  ver/9Rk6sSeWEG?s
+000001a0: 7479 6c65 3d66 6c61 7426 636f 6d70 6163  tyle=flat&compac
+000001b0: 743d 7472 7565 295d 2868 7474 7073 3a2f  t=true)](https:/
+000001c0: 2f64 6973 636f 7264 2e63 6f6d 2f69 6e76  /discord.com/inv
+000001d0: 6974 652f 3952 6b36 7353 6557 4547 290a  ite/9Rk6sSeWEG).
+000001e0: 5b21 5b54 7769 7474 6572 5d28 6874 7470  [![Twitter](http
+000001f0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000200: 696f 2f74 7769 7474 6572 2f75 726c 2f68  io/twitter/url/h
+00000210: 7474 7073 2f74 7769 7474 6572 2e63 6f6d  ttps/twitter.com
+00000220: 2f74 6f67 6574 6865 7263 6f6d 7075 7465  /togethercompute
+00000230: 2e73 7667 3f73 7479 6c65 3d73 6f63 6961  .svg?style=socia
+00000240: 6c26 6c61 6265 6c3d 466f 6c6c 6f77 2532  l&label=Follow%2
+00000250: 3025 3430 746f 6765 7468 6572 636f 6d70  0%40togethercomp
+00000260: 7574 6529 5d28 6874 7470 733a 2f2f 7477  ute)](https://tw
+00000270: 6974 7465 722e 636f 6d2f 746f 6765 7468  itter.com/togeth
+00000280: 6572 636f 6d70 7574 6529 0a0a 5468 6520  ercompute)..The 
+00000290: 5b54 6f67 6574 6865 7220 5079 7468 6f6e  [Together Python
+000002a0: 2041 5049 204c 6962 7261 7279 5d28 6874   API Library](ht
+000002b0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+000002c0: 726f 6a65 6374 2f74 6f67 6574 6865 722f  roject/together/
+000002d0: 2920 6973 2074 6865 206f 6666 6963 6961  ) is the officia
+000002e0: 6c20 5079 7468 6f6e 2063 6c69 656e 7420  l Python client 
+000002f0: 666f 7220 546f 6765 7468 6572 2773 2041  for Together's A
+00000300: 5049 2070 6c61 7466 6f72 6d2c 2070 726f  PI platform, pro
+00000310: 7669 6469 6e67 2061 2063 6f6e 7665 6e69  viding a conveni
+00000320: 656e 7420 7761 7920 666f 7220 696e 7465  ent way for inte
+00000330: 7261 6374 696e 6720 7769 7468 2074 6865  racting with the
+00000340: 2052 4553 5420 4150 4973 2061 6e64 2065   REST APIs and e
+00000350: 6e61 626c 6573 2065 6173 7920 696e 7465  nables easy inte
+00000360: 6772 6174 696f 6e73 2077 6974 6820 5079  grations with Py
+00000370: 7468 6f6e 2033 2e38 2b20 6170 706c 6963  thon 3.8+ applic
+00000380: 6174 696f 6e73 2077 6974 6820 6561 7379  ations with easy
+00000390: 2074 6f20 7573 6520 7379 6e63 6872 6f6e   to use synchron
+000003a0: 6f75 7320 616e 6420 6173 796e 6368 726f  ous and asynchro
+000003b0: 6e6f 7573 2063 6c69 656e 7473 2e0a 0a0a  nous clients....
+000003c0: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
+000003d0: 0a0a 3e20 f09f 9aa7 0a3e 2054 6865 204c  ..> .....> The L
+000003e0: 6962 7261 7279 2077 6173 2072 6577 7269  ibrary was rewri
+000003f0: 7474 656e 2069 6e20 7631 2e30 2e30 2072  tten in v1.0.0 r
+00000400: 656c 6561 7365 6420 696e 2041 7072 696c  eleased in April
+00000410: 206f 6620 3230 3234 2e20 5468 6572 6520   of 2024. There 
+00000420: 7765 7265 2073 6967 6e69 6669 6361 6e74  were significant
+00000430: 2063 6861 6e67 6573 206d 6164 652e 0a0a   changes made...
+00000440: 546f 2069 6e73 7461 6c6c 2054 6f67 6574  To install Toget
+00000450: 6865 7220 5079 7468 6f6e 204c 6962 7261  her Python Libra
+00000460: 7279 2066 726f 6d20 5079 5049 2c20 7369  ry from PyPI, si
+00000470: 6d70 6c79 2072 756e 3a0a 0a60 6060 7368  mply run:..```sh
+00000480: 656c 6c20 5368 656c 6c0a 7069 7020 696e  ell Shell.pip in
+00000490: 7374 616c 6c20 2d2d 7570 6772 6164 6520  stall --upgrade 
+000004a0: 746f 6765 7468 6572 0a60 6060 0a0a 2323  together.```..##
+000004b0: 2320 5365 7474 696e 6720 7570 2041 5049  # Setting up API
+000004c0: 204b 6579 0a0a 3e20 f09f 9aa7 2059 6f75   Key..> .... You
+000004d0: 2077 696c 6c20 6e65 6564 2074 6f20 6372   will need to cr
+000004e0: 6561 7465 2061 6e20 6163 636f 756e 7420  eate an account 
+000004f0: 7769 7468 205b 546f 6765 7468 6572 2e61  with [Together.a
+00000500: 695d 2868 7474 7073 3a2f 2f61 7069 2e74  i](https://api.t
+00000510: 6f67 6574 6865 722e 7879 7a2f 2920 746f  ogether.xyz/) to
+00000520: 206f 6274 6169 6e20 6120 546f 6765 7468   obtain a Togeth
+00000530: 6572 2041 5049 204b 6579 2e0a 0a4f 6e63  er API Key...Onc
+00000540: 6520 6c6f 6767 6564 2069 6e20 746f 2074  e logged in to t
+00000550: 6865 2054 6f67 6574 6865 7220 506c 6179  he Together Play
+00000560: 6772 6f75 6e64 2c20 796f 7520 6361 6e20  ground, you can 
+00000570: 6669 6e64 2061 7661 696c 6162 6c65 2041  find available A
+00000580: 5049 206b 6579 7320 696e 205b 7468 6973  PI keys in [this
+00000590: 2073 6574 7469 6e67 7320 7061 6765 5d28   settings page](
+000005a0: 6874 7470 733a 2f2f 6170 692e 746f 6765  https://api.toge
+000005b0: 7468 6572 2e78 797a 2f73 6574 7469 6e67  ther.xyz/setting
+000005c0: 732f 6170 692d 6b65 7973 292e 0a0a 2323  s/api-keys)...##
+000005d0: 2323 2053 6574 7469 6e67 2065 6e76 6972  ## Setting envir
+000005e0: 6f6e 6d65 6e74 2076 6172 6961 626c 650a  onment variable.
+000005f0: 0a60 6060 7368 656c 6c0a 6578 706f 7274  .```shell.export
+00000600: 2054 4f47 4554 4845 525f 4150 495f 4b45   TOGETHER_API_KE
+00000610: 593d 7878 7878 780a 6060 600a 0a23 2323  Y=xxxxx.```..###
+00000620: 2320 5573 696e 6720 7468 6520 636c 6965  # Using the clie
+00000630: 6e74 0a0a 6060 6070 7974 686f 6e0a 6672  nt..```python.fr
+00000640: 6f6d 2074 6f67 6574 6865 7220 696d 706f  om together impo
+00000650: 7274 2054 6f67 6574 6865 720a 0a63 6c69  rt Together..cli
+00000660: 656e 7420 3d20 546f 6765 7468 6572 2861  ent = Together(a
+00000670: 7069 5f6b 6579 3d22 7878 7878 7822 290a  pi_key="xxxxx").
+00000680: 6060 600a 0a54 6869 7320 7265 706f 2063  ```..This repo c
+00000690: 6f6e 7461 696e 7320 626f 7468 2061 2050  ontains both a P
+000006a0: 7974 686f 6e20 4c69 6272 6172 7920 616e  ython Library an
+000006b0: 6420 6120 434c 492e 2057 6527 6c6c 2064  d a CLI. We'll d
+000006c0: 656d 6f6e 7374 7261 7465 2068 6f77 2074  emonstrate how t
+000006d0: 6f20 7573 6520 626f 7468 2062 656c 6f77  o use both below
+000006e0: 2e0a 0a23 2320 5573 6167 6520 e280 9320  ...## Usage ... 
+000006f0: 5079 7468 6f6e 2043 6c69 656e 740a 0a23  Python Client..#
+00000700: 2323 2043 6861 7420 436f 6d70 6c65 7469  ## Chat Completi
+00000710: 6f6e 730a 0a60 6060 7079 7468 6f6e 0a69  ons..```python.i
+00000720: 6d70 6f72 7420 6f73 0a66 726f 6d20 746f  mport os.from to
+00000730: 6765 7468 6572 2069 6d70 6f72 7420 546f  gether import To
+00000740: 6765 7468 6572 0a0a 636c 6965 6e74 203d  gether..client =
+00000750: 2054 6f67 6574 6865 7228 6170 695f 6b65   Together(api_ke
+00000760: 793d 6f73 2e65 6e76 6972 6f6e 2e67 6574  y=os.environ.get
+00000770: 2822 544f 4745 5448 4552 5f41 5049 5f4b  ("TOGETHER_API_K
+00000780: 4559 2229 290a 0a72 6573 706f 6e73 6520  EY"))..response 
+00000790: 3d20 636c 6965 6e74 2e63 6861 742e 636f  = client.chat.co
+000007a0: 6d70 6c65 7469 6f6e 732e 6372 6561 7465  mpletions.create
+000007b0: 280a 2020 2020 6d6f 6465 6c3d 226d 6973  (.    model="mis
+000007c0: 7472 616c 6169 2f4d 6978 7472 616c 2d38  tralai/Mixtral-8
+000007d0: 7837 422d 496e 7374 7275 6374 2d76 302e  x7B-Instruct-v0.
+000007e0: 3122 2c0a 2020 2020 6d65 7373 6167 6573  1",.    messages
+000007f0: 3d5b 7b22 726f 6c65 223a 2022 7573 6572  =[{"role": "user
+00000800: 222c 2022 636f 6e74 656e 7422 3a20 2274  ", "content": "t
+00000810: 656c 6c20 6d65 2061 626f 7574 206e 6577  ell me about new
+00000820: 2079 6f72 6b22 7d5d 2c0a 290a 7072 696e   york"}],.).prin
+00000830: 7428 7265 7370 6f6e 7365 2e63 686f 6963  t(response.choic
+00000840: 6573 5b30 5d2e 6d65 7373 6167 652e 636f  es[0].message.co
+00000850: 6e74 656e 7429 0a60 6060 0a0a 2323 2323  ntent).```..####
+00000860: 2053 7472 6561 6d69 6e67 0a0a 6060 6070   Streaming..```p
+00000870: 7974 686f 6e0a 696d 706f 7274 206f 730a  ython.import os.
+00000880: 6672 6f6d 2074 6f67 6574 6865 7220 696d  from together im
+00000890: 706f 7274 2054 6f67 6574 6865 720a 0a63  port Together..c
+000008a0: 6c69 656e 7420 3d20 546f 6765 7468 6572  lient = Together
+000008b0: 2861 7069 5f6b 6579 3d6f 732e 656e 7669  (api_key=os.envi
+000008c0: 726f 6e2e 6765 7428 2254 4f47 4554 4845  ron.get("TOGETHE
+000008d0: 525f 4150 495f 4b45 5922 2929 0a73 7472  R_API_KEY")).str
+000008e0: 6561 6d20 3d20 636c 6965 6e74 2e63 6861  eam = client.cha
+000008f0: 742e 636f 6d70 6c65 7469 6f6e 732e 6372  t.completions.cr
+00000900: 6561 7465 280a 2020 2020 6d6f 6465 6c3d  eate(.    model=
+00000910: 226d 6973 7472 616c 6169 2f4d 6978 7472  "mistralai/Mixtr
+00000920: 616c 2d38 7837 422d 496e 7374 7275 6374  al-8x7B-Instruct
+00000930: 2d76 302e 3122 2c0a 2020 2020 6d65 7373  -v0.1",.    mess
+00000940: 6167 6573 3d5b 7b22 726f 6c65 223a 2022  ages=[{"role": "
+00000950: 7573 6572 222c 2022 636f 6e74 656e 7422  user", "content"
+00000960: 3a20 2274 656c 6c20 6d65 2061 626f 7574  : "tell me about
+00000970: 206e 6577 2079 6f72 6b22 7d5d 2c0a 2020   new york"}],.  
+00000980: 2020 7374 7265 616d 3d54 7275 652c 0a29    stream=True,.)
+00000990: 0a0a 666f 7220 6368 756e 6b20 696e 2073  ..for chunk in s
+000009a0: 7472 6561 6d3a 0a20 2020 2070 7269 6e74  tream:.    print
+000009b0: 2863 6875 6e6b 2e63 686f 6963 6573 5b30  (chunk.choices[0
+000009c0: 5d2e 6465 6c74 612e 636f 6e74 656e 7420  ].delta.content 
+000009d0: 6f72 2022 222c 2065 6e64 3d22 222c 2066  or "", end="", f
+000009e0: 6c75 7368 3d54 7275 6529 0a60 6060 0a0a  lush=True).```..
+000009f0: 2323 2323 2041 7379 6e63 2075 7361 6765  #### Async usage
+00000a00: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
+00000a10: 7274 206f 732c 2061 7379 6e63 696f 0a66  rt os, asyncio.f
+00000a20: 726f 6d20 746f 6765 7468 6572 2069 6d70  rom together imp
+00000a30: 6f72 7420 4173 796e 6354 6f67 6574 6865  ort AsyncTogethe
+00000a40: 720a 0a61 7379 6e63 5f63 6c69 656e 7420  r..async_client 
+00000a50: 3d20 4173 796e 6354 6f67 6574 6865 7228  = AsyncTogether(
+00000a60: 6170 695f 6b65 793d 6f73 2e65 6e76 6972  api_key=os.envir
+00000a70: 6f6e 2e67 6574 2822 544f 4745 5448 4552  on.get("TOGETHER
+00000a80: 5f41 5049 5f4b 4559 2229 290a 6d65 7373  _API_KEY")).mess
+00000a90: 6167 6573 203d 205b 0a20 2020 2022 5768  ages = [.    "Wh
+00000aa0: 6174 2061 7265 2074 6865 2074 6f70 2074  at are the top t
+00000ab0: 6869 6e67 7320 746f 2064 6f20 696e 2053  hings to do in S
+00000ac0: 616e 2046 7261 6e63 6973 636f 3f22 2c0a  an Francisco?",.
+00000ad0: 2020 2020 2257 6861 7420 636f 756e 7472      "What countr
+00000ae0: 7920 6973 2050 6172 6973 2069 6e3f 222c  y is Paris in?",
+00000af0: 0a5d 0a0a 6173 796e 6320 6465 6620 6173  .]..async def as
+00000b00: 796e 635f 6368 6174 5f63 6f6d 706c 6574  ync_chat_complet
+00000b10: 696f 6e28 6d65 7373 6167 6573 293a 0a20  ion(messages):. 
+00000b20: 2020 2061 7379 6e63 5f63 6c69 656e 7420     async_client 
+00000b30: 3d20 4173 796e 6354 6f67 6574 6865 7228  = AsyncTogether(
+00000b40: 6170 695f 6b65 793d 6f73 2e65 6e76 6972  api_key=os.envir
+00000b50: 6f6e 2e67 6574 2822 544f 4745 5448 4552  on.get("TOGETHER
+00000b60: 5f41 5049 5f4b 4559 2229 290a 2020 2020  _API_KEY")).    
+00000b70: 7461 736b 7320 3d20 5b0a 2020 2020 2020  tasks = [.      
+00000b80: 2020 6173 796e 635f 636c 6965 6e74 2e63    async_client.c
+00000b90: 6861 742e 636f 6d70 6c65 7469 6f6e 732e  hat.completions.
+00000ba0: 6372 6561 7465 280a 2020 2020 2020 2020  create(.        
+00000bb0: 2020 2020 6d6f 6465 6c3d 226d 6973 7472      model="mistr
+00000bc0: 616c 6169 2f4d 6978 7472 616c 2d38 7837  alai/Mixtral-8x7
+00000bd0: 422d 496e 7374 7275 6374 2d76 302e 3122  B-Instruct-v0.1"
+00000be0: 2c0a 2020 2020 2020 2020 2020 2020 6d65  ,.            me
+00000bf0: 7373 6167 6573 3d5b 7b22 726f 6c65 223a  ssages=[{"role":
+00000c00: 2022 7573 6572 222c 2022 636f 6e74 656e   "user", "conten
+00000c10: 7422 3a20 6d65 7373 6167 657d 5d2c 0a20  t": message}],. 
+00000c20: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00000c30: 2066 6f72 206d 6573 7361 6765 2069 6e20   for message in 
+00000c40: 6d65 7373 6167 6573 0a20 2020 205d 0a20  messages.    ]. 
+00000c50: 2020 2072 6573 706f 6e73 6573 203d 2061     responses = a
+00000c60: 7761 6974 2061 7379 6e63 696f 2e67 6174  wait asyncio.gat
+00000c70: 6865 7228 2a74 6173 6b73 290a 0a20 2020  her(*tasks)..   
+00000c80: 2066 6f72 2072 6573 706f 6e73 6520 696e   for response in
+00000c90: 2072 6573 706f 6e73 6573 3a0a 2020 2020   responses:.    
+00000ca0: 2020 2020 7072 696e 7428 7265 7370 6f6e      print(respon
+00000cb0: 7365 2e63 686f 6963 6573 5b30 5d2e 6d65  se.choices[0].me
+00000cc0: 7373 6167 652e 636f 6e74 656e 7429 0a0a  ssage.content)..
+00000cd0: 6173 796e 6369 6f2e 7275 6e28 6173 796e  asyncio.run(asyn
+00000ce0: 635f 6368 6174 5f63 6f6d 706c 6574 696f  c_chat_completio
+00000cf0: 6e28 6d65 7373 6167 6573 2929 0a60 6060  n(messages)).```
+00000d00: 0a0a 2323 2320 436f 6d70 6c65 7469 6f6e  ..### Completion
+00000d10: 730a 0a43 6f6d 706c 6574 696f 6e73 2061  s..Completions a
+00000d20: 7265 2066 6f72 2063 6f64 6520 616e 6420  re for code and 
+00000d30: 6c61 6e67 7561 6765 206d 6f64 656c 7320  language models 
+00000d40: 7368 6f77 6e20 5b68 6572 655d 2868 7474  shown [here](htt
+00000d50: 7073 3a2f 2f64 6f63 732e 746f 6765 7468  ps://docs.togeth
+00000d60: 6572 2e61 692f 646f 6373 2f69 6e66 6572  er.ai/docs/infer
+00000d70: 656e 6365 2d6d 6f64 656c 7329 2e20 4265  ence-models). Be
+00000d80: 6c6f 772c 2061 2063 6f64 6520 6d6f 6465  low, a code mode
+00000d90: 6c20 6578 616d 706c 6520 6973 2073 686f  l example is sho
+00000da0: 776e 2e0a 0a60 6060 7079 7468 6f6e 0a69  wn...```python.i
+00000db0: 6d70 6f72 7420 6f73 0a66 726f 6d20 746f  mport os.from to
+00000dc0: 6765 7468 6572 2069 6d70 6f72 7420 546f  gether import To
+00000dd0: 6765 7468 6572 0a0a 636c 6965 6e74 203d  gether..client =
+00000de0: 2054 6f67 6574 6865 7228 6170 695f 6b65   Together(api_ke
+00000df0: 793d 6f73 2e65 6e76 6972 6f6e 2e67 6574  y=os.environ.get
+00000e00: 2822 544f 4745 5448 4552 5f41 5049 5f4b  ("TOGETHER_API_K
+00000e10: 4559 2229 290a 0a72 6573 706f 6e73 6520  EY"))..response 
+00000e20: 3d20 636c 6965 6e74 2e63 6f6d 706c 6574  = client.complet
+00000e30: 696f 6e73 2e63 7265 6174 6528 0a20 2020  ions.create(.   
+00000e40: 206d 6f64 656c 3d22 636f 6465 6c6c 616d   model="codellam
+00000e50: 612f 436f 6465 4c6c 616d 612d 3334 622d  a/CodeLlama-34b-
+00000e60: 5079 7468 6f6e 2d68 6622 2c0a 2020 2020  Python-hf",.    
+00000e70: 7072 6f6d 7074 3d22 5772 6974 6520 6120  prompt="Write a 
+00000e80: 4e65 7874 2e6a 7320 636f 6d70 6f6e 656e  Next.js componen
+00000e90: 7420 7769 7468 2054 6169 6c77 696e 6443  t with TailwindC
+00000ea0: 5353 2066 6f72 2061 2068 6561 6465 7220  SS for a header 
+00000eb0: 636f 6d70 6f6e 656e 742e 222c 0a20 2020  component.",.   
+00000ec0: 206d 6178 5f74 6f6b 656e 733d 3230 302c   max_tokens=200,
+00000ed0: 0a29 0a70 7269 6e74 2872 6573 706f 6e73  .).print(respons
+00000ee0: 652e 6368 6f69 6365 735b 305d 2e74 6578  e.choices[0].tex
+00000ef0: 7429 0a60 6060 0a0a 2323 2323 2053 7472  t).```..#### Str
+00000f00: 6561 6d69 6e67 0a0a 6060 6070 7974 686f  eaming..```pytho
+00000f10: 6e0a 696d 706f 7274 206f 730a 6672 6f6d  n.import os.from
+00000f20: 2074 6f67 6574 6865 7220 696d 706f 7274   together import
+00000f30: 2054 6f67 6574 6865 720a 0a63 6c69 656e   Together..clien
+00000f40: 7420 3d20 546f 6765 7468 6572 2861 7069  t = Together(api
+00000f50: 5f6b 6579 3d6f 732e 656e 7669 726f 6e2e  _key=os.environ.
+00000f60: 6765 7428 2254 4f47 4554 4845 525f 4150  get("TOGETHER_AP
+00000f70: 495f 4b45 5922 2929 0a73 7472 6561 6d20  I_KEY")).stream 
+00000f80: 3d20 636c 6965 6e74 2e63 6f6d 706c 6574  = client.complet
+00000f90: 696f 6e73 2e63 7265 6174 6528 0a20 2020  ions.create(.   
+00000fa0: 206d 6f64 656c 3d22 636f 6465 6c6c 616d   model="codellam
+00000fb0: 612f 436f 6465 4c6c 616d 612d 3334 622d  a/CodeLlama-34b-
+00000fc0: 5079 7468 6f6e 2d68 6622 2c0a 2020 2020  Python-hf",.    
+00000fd0: 7072 6f6d 7074 3d22 5772 6974 6520 6120  prompt="Write a 
+00000fe0: 4e65 7874 2e6a 7320 636f 6d70 6f6e 656e  Next.js componen
+00000ff0: 7420 7769 7468 2054 6169 6c77 696e 6443  t with TailwindC
+00001000: 5353 2066 6f72 2061 2068 6561 6465 7220  SS for a header 
+00001010: 636f 6d70 6f6e 656e 742e 222c 0a20 2020  component.",.   
+00001020: 2073 7472 6561 6d3d 5472 7565 2c0a 290a   stream=True,.).
+00001030: 0a66 6f72 2063 6875 6e6b 2069 6e20 7374  .for chunk in st
+00001040: 7265 616d 3a0a 2020 2020 7072 696e 7428  ream:.    print(
+00001050: 6368 756e 6b2e 6368 6f69 6365 735b 305d  chunk.choices[0]
+00001060: 2e64 656c 7461 2e63 6f6e 7465 6e74 206f  .delta.content o
+00001070: 7220 2222 2c20 656e 643d 2222 2c20 666c  r "", end="", fl
+00001080: 7573 683d 5472 7565 290a 6060 600a 0a23  ush=True).```..#
+00001090: 2323 2320 4173 796e 6320 7573 6167 650a  ### Async usage.
+000010a0: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
+000010b0: 7420 6f73 2c20 6173 796e 6369 6f0a 6672  t os, asyncio.fr
+000010c0: 6f6d 2074 6f67 6574 6865 7220 696d 706f  om together impo
+000010d0: 7274 2041 7379 6e63 546f 6765 7468 6572  rt AsyncTogether
+000010e0: 0a0a 6173 796e 635f 636c 6965 6e74 203d  ..async_client =
+000010f0: 2041 7379 6e63 546f 6765 7468 6572 2861   AsyncTogether(a
+00001100: 7069 5f6b 6579 3d6f 732e 656e 7669 726f  pi_key=os.enviro
+00001110: 6e2e 6765 7428 2254 4f47 4554 4845 525f  n.get("TOGETHER_
+00001120: 4150 495f 4b45 5922 2929 0a70 726f 6d70  API_KEY")).promp
+00001130: 7473 203d 205b 0a20 2020 2022 5772 6974  ts = [.    "Writ
+00001140: 6520 6120 4e65 7874 2e6a 7320 636f 6d70  e a Next.js comp
+00001150: 6f6e 656e 7420 7769 7468 2054 6169 6c77  onent with Tailw
+00001160: 696e 6443 5353 2066 6f72 2061 2068 6561  indCSS for a hea
+00001170: 6465 7220 636f 6d70 6f6e 656e 742e 222c  der component.",
+00001180: 0a20 2020 2022 5772 6974 6520 6120 7079  .    "Write a py
+00001190: 7468 6f6e 2066 756e 6374 696f 6e20 666f  thon function fo
+000011a0: 7220 7468 6520 6669 626f 6e61 6363 6920  r the fibonacci 
+000011b0: 7365 7175 656e 6365 222c 0a5d 0a0a 6173  sequence",.]..as
+000011c0: 796e 6320 6465 6620 6173 796e 635f 6368  ync def async_ch
+000011d0: 6174 5f63 6f6d 706c 6574 696f 6e28 7072  at_completion(pr
+000011e0: 6f6d 7074 7329 3a0a 2020 2020 6173 796e  ompts):.    asyn
+000011f0: 635f 636c 6965 6e74 203d 2041 7379 6e63  c_client = Async
+00001200: 546f 6765 7468 6572 2861 7069 5f6b 6579  Together(api_key
+00001210: 3d6f 732e 656e 7669 726f 6e2e 6765 7428  =os.environ.get(
+00001220: 2254 4f47 4554 4845 525f 4150 495f 4b45  "TOGETHER_API_KE
+00001230: 5922 2929 0a20 2020 2074 6173 6b73 203d  Y")).    tasks =
+00001240: 205b 0a20 2020 2020 2020 2061 7379 6e63   [.        async
+00001250: 5f63 6c69 656e 742e 636f 6d70 6c65 7469  _client.completi
+00001260: 6f6e 732e 6372 6561 7465 280a 2020 2020  ons.create(.    
+00001270: 2020 2020 2020 2020 6d6f 6465 6c3d 2263          model="c
+00001280: 6f64 656c 6c61 6d61 2f43 6f64 654c 6c61  odellama/CodeLla
+00001290: 6d61 2d33 3462 2d50 7974 686f 6e2d 6866  ma-34b-Python-hf
+000012a0: 222c 0a20 2020 2020 2020 2020 2020 2070  ",.            p
+000012b0: 726f 6d70 743d 7072 6f6d 7074 2c0a 2020  rompt=prompt,.  
+000012c0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000012d0: 666f 7220 7072 6f6d 7074 2069 6e20 7072  for prompt in pr
+000012e0: 6f6d 7074 730a 2020 2020 5d0a 2020 2020  ompts.    ].    
+000012f0: 7265 7370 6f6e 7365 7320 3d20 6177 6169  responses = awai
+00001300: 7420 6173 796e 6369 6f2e 6761 7468 6572  t asyncio.gather
+00001310: 282a 7461 736b 7329 0a0a 2020 2020 666f  (*tasks)..    fo
+00001320: 7220 7265 7370 6f6e 7365 2069 6e20 7265  r response in re
+00001330: 7370 6f6e 7365 733a 0a20 2020 2020 2020  sponses:.       
+00001340: 2070 7269 6e74 2872 6573 706f 6e73 652e   print(response.
+00001350: 6368 6f69 6365 735b 305d 2e74 6578 7429  choices[0].text)
+00001360: 0a0a 6173 796e 6369 6f2e 7275 6e28 6173  ..asyncio.run(as
+00001370: 796e 635f 6368 6174 5f63 6f6d 706c 6574  ync_chat_complet
+00001380: 696f 6e28 7072 6f6d 7074 7329 290a 6060  ion(prompts)).``
+00001390: 600a 0a23 2323 2049 6d61 6765 2067 656e  `..### Image gen
+000013a0: 6572 6174 696f 6e0a 0a60 6060 7079 7468  eration..```pyth
+000013b0: 6f6e 0a69 6d70 6f72 7420 6f73 0a66 726f  on.import os.fro
+000013c0: 6d20 746f 6765 7468 6572 2069 6d70 6f72  m together impor
+000013d0: 7420 546f 6765 7468 6572 0a0a 636c 6965  t Together..clie
+000013e0: 6e74 203d 2054 6f67 6574 6865 7228 6170  nt = Together(ap
+000013f0: 695f 6b65 793d 6f73 2e65 6e76 6972 6f6e  i_key=os.environ
+00001400: 2e67 6574 2822 544f 4745 5448 4552 5f41  .get("TOGETHER_A
+00001410: 5049 5f4b 4559 2229 290a 0a72 6573 706f  PI_KEY"))..respo
+00001420: 6e73 6520 3d20 636c 6965 6e74 2e69 6d61  nse = client.ima
+00001430: 6765 732e 6765 6e65 7261 7465 280a 2020  ges.generate(.  
+00001440: 2020 7072 6f6d 7074 3d22 7370 6163 6520    prompt="space 
+00001450: 726f 626f 7473 222c 0a20 2020 206d 6f64  robots",.    mod
+00001460: 656c 3d22 7374 6162 696c 6974 7961 692f  el="stabilityai/
+00001470: 7374 6162 6c65 2d64 6966 6675 7369 6f6e  stable-diffusion
+00001480: 2d78 6c2d 6261 7365 2d31 2e30 222c 0a20  -xl-base-1.0",. 
+00001490: 2020 2073 7465 7073 3d31 302c 0a20 2020     steps=10,.   
+000014a0: 206e 3d34 2c0a 290a 7072 696e 7428 7265   n=4,.).print(re
+000014b0: 7370 6f6e 7365 2e64 6174 615b 305d 2e62  sponse.data[0].b
+000014c0: 3634 5f6a 736f 6e29 0a60 6060 0a0a 2323  64_json).```..##
+000014d0: 2320 456d 6265 6464 696e 6773 0a0a 6060  # Embeddings..``
+000014e0: 6070 7974 686f 6e0a 6672 6f6d 2074 7970  `python.from typ
+000014f0: 696e 6720 696d 706f 7274 204c 6973 740a  ing import List.
+00001500: 6672 6f6d 2074 6f67 6574 6865 7220 696d  from together im
+00001510: 706f 7274 2054 6f67 6574 6865 720a 0a63  port Together..c
+00001520: 6c69 656e 7420 3d20 546f 6765 7468 6572  lient = Together
+00001530: 2861 7069 5f6b 6579 3d6f 732e 656e 7669  (api_key=os.envi
+00001540: 726f 6e2e 6765 7428 2254 4f47 4554 4845  ron.get("TOGETHE
+00001550: 525f 4150 495f 4b45 5922 2929 0a0a 6465  R_API_KEY"))..de
+00001560: 6620 6765 745f 656d 6265 6464 696e 6773  f get_embeddings
+00001570: 2874 6578 7473 3a20 4c69 7374 5b73 7472  (texts: List[str
+00001580: 5d2c 206d 6f64 656c 3a20 7374 7229 202d  ], model: str) -
+00001590: 3e20 4c69 7374 5b4c 6973 745b 666c 6f61  > List[List[floa
+000015a0: 745d 5d3a 0a20 2020 2074 6578 7473 203d  t]]:.    texts =
+000015b0: 205b 7465 7874 2e72 6570 6c61 6365 2822   [text.replace("
+000015c0: 5c6e 222c 2022 2022 2920 666f 7220 7465  \n", " ") for te
+000015d0: 7874 2069 6e20 7465 7874 735d 0a20 2020  xt in texts].   
+000015e0: 206f 7574 7075 7473 203d 2063 6c69 656e   outputs = clien
+000015f0: 742e 656d 6265 6464 696e 6773 2e63 7265  t.embeddings.cre
+00001600: 6174 6528 6d6f 6465 6c3d 6d6f 6465 6c2c  ate(model=model,
+00001610: 2069 6e70 7574 203d 2074 6578 7473 290a   input = texts).
+00001620: 2020 2020 7265 7475 726e 205b 6f75 7470      return [outp
+00001630: 7574 732e 6461 7461 5b69 5d2e 656d 6265  uts.data[i].embe
+00001640: 6464 696e 6720 666f 7220 6920 696e 2072  dding for i in r
+00001650: 616e 6765 286c 656e 2874 6578 7473 2929  ange(len(texts))
+00001660: 5d0a 0a69 6e70 7574 5f74 6578 7473 203d  ]..input_texts =
+00001670: 205b 274f 7572 2073 6f6c 6172 2073 7973   ['Our solar sys
+00001680: 7465 6d20 6f72 6269 7473 2074 6865 204d  tem orbits the M
+00001690: 696c 6b79 2057 6179 2067 616c 6178 7920  ilky Way galaxy 
+000016a0: 6174 2061 626f 7574 2035 3135 2c30 3030  at about 515,000
+000016b0: 206d 7068 275d 0a65 6d62 6564 6469 6e67   mph'].embedding
+000016c0: 7320 3d20 6765 745f 656d 6265 6464 696e  s = get_embeddin
+000016d0: 6773 2869 6e70 7574 5f74 6578 7473 2c20  gs(input_texts, 
+000016e0: 6d6f 6465 6c3d 2774 6f67 6574 6865 7263  model='togetherc
+000016f0: 6f6d 7075 7465 722f 6d32 2d62 6572 742d  omputer/m2-bert-
+00001700: 3830 4d2d 386b 2d72 6574 7269 6576 616c  80M-8k-retrieval
+00001710: 2729 0a0a 7072 696e 7428 656d 6265 6464  ')..print(embedd
+00001720: 696e 6773 290a 6060 600a 0a23 2323 2046  ings).```..### F
+00001730: 696c 6573 0a0a 5468 6520 6669 6c65 7320  iles..The files 
+00001740: 4150 4920 6973 2075 7365 6420 666f 7220  API is used for 
+00001750: 6669 6e65 2d74 756e 696e 6720 616e 6420  fine-tuning and 
+00001760: 616c 6c6f 7773 2064 6576 656c 6f70 6572  allows developer
+00001770: 7320 746f 2075 706c 6f61 6420 6461 7461  s to upload data
+00001780: 2074 6f20 6669 6e65 2d74 756e 6520 6f6e   to fine-tune on
+00001790: 2e20 4974 2061 6c73 6f20 6861 7320 7365  . It also has se
+000017a0: 7665 7261 6c20 6d65 7468 6f64 7320 746f  veral methods to
+000017b0: 206c 6973 7420 616c 6c20 6669 6c65 732c   list all files,
+000017c0: 2072 6574 7269 7665 2066 696c 6573 2c20   retrive files, 
+000017d0: 616e 6420 6465 6c65 7465 2066 696c 6573  and delete files
+000017e0: 2e20 506c 6561 7365 2072 6566 6572 2074  . Please refer t
+000017f0: 6f20 6f75 7220 6669 6e65 2d74 756e 696e  o our fine-tunin
+00001800: 6720 646f 6373 205b 6865 7265 5d28 6874  g docs [here](ht
+00001810: 7470 733a 2f2f 646f 6373 2e74 6f67 6574  tps://docs.toget
+00001820: 6865 722e 6169 2f64 6f63 732f 6669 6e65  her.ai/docs/fine
+00001830: 2d74 756e 696e 672d 7079 7468 6f6e 292e  -tuning-python).
+00001840: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
+00001850: 7274 206f 730a 6672 6f6d 2074 6f67 6574  rt os.from toget
+00001860: 6865 7220 696d 706f 7274 2054 6f67 6574  her import Toget
+00001870: 6865 720a 0a63 6c69 656e 7420 3d20 546f  her..client = To
+00001880: 6765 7468 6572 2861 7069 5f6b 6579 3d6f  gether(api_key=o
+00001890: 732e 656e 7669 726f 6e2e 6765 7428 2254  s.environ.get("T
+000018a0: 4f47 4554 4845 525f 4150 495f 4b45 5922  OGETHER_API_KEY"
+000018b0: 2929 0a0a 636c 6965 6e74 2e66 696c 6573  ))..client.files
+000018c0: 2e75 706c 6f61 6428 6669 6c65 3d22 736f  .upload(file="so
+000018d0: 6d65 6461 7461 2e6a 736f 6e6c 2229 2023  medata.jsonl") #
+000018e0: 2075 706c 6f61 6473 2061 2066 696c 650a   uploads a file.
+000018f0: 636c 6965 6e74 2e66 696c 6573 2e6c 6973  client.files.lis
+00001900: 7428 2920 2320 6c69 7374 7320 616c 6c20  t() # lists all 
+00001910: 7570 6c6f 6164 6564 2066 696c 6573 0a63  uploaded files.c
+00001920: 6c69 656e 742e 6669 6c65 732e 7265 7472  lient.files.retr
+00001930: 6965 7665 2869 643d 2266 696c 652d 6430  ieve(id="file-d0
+00001940: 6433 3138 6362 2d62 3764 392d 3439 3361  d318cb-b7d9-493a
+00001950: 2d62 6437 302d 3163 6665 3038 3964 3338  -bd70-1cfe089d38
+00001960: 3135 2229 2023 2072 6574 7269 6576 6573  15") # retrieves
+00001970: 2061 2073 7065 6369 6669 6320 6669 6c65   a specific file
+00001980: 0a63 6c69 656e 742e 6669 6c65 732e 7265  .client.files.re
+00001990: 7472 6965 7665 5f63 6f6e 7465 6e74 2869  trieve_content(i
+000019a0: 643d 2266 696c 652d 6430 6433 3138 6362  d="file-d0d318cb
+000019b0: 2d62 3764 392d 3439 3361 2d62 6437 302d  -b7d9-493a-bd70-
+000019c0: 3163 6665 3038 3964 3338 3135 2229 2023  1cfe089d3815") #
+000019d0: 2072 6574 7269 6576 6573 2063 6f6e 7465   retrieves conte
+000019e0: 6e74 206f 6620 6120 7370 6563 6966 6963  nt of a specific
+000019f0: 2066 696c 650a 636c 6965 6e74 2e66 696c   file.client.fil
+00001a00: 6573 2e64 656c 6574 6528 6964 3d22 6669  es.delete(id="fi
+00001a10: 6c65 2d64 3064 3331 3863 622d 6237 6439  le-d0d318cb-b7d9
+00001a20: 2d34 3933 612d 6264 3730 2d31 6366 6530  -493a-bd70-1cfe0
+00001a30: 3839 6433 3831 3522 2920 2320 6465 6c65  89d3815") # dele
+00001a40: 7465 7320 6120 6669 6c65 0a60 6060 0a0a  tes a file.```..
+00001a50: 2323 2320 4669 6e65 2d74 756e 6573 0a0a  ### Fine-tunes..
+00001a60: 5468 6520 6669 6e65 7475 6e65 2041 5049  The finetune API
+00001a70: 2069 7320 7573 6564 2066 6f72 2066 696e   is used for fin
+00001a80: 652d 7475 6e69 6e67 2061 6e64 2061 6c6c  e-tuning and all
+00001a90: 6f77 7320 6465 7665 6c6f 7065 7273 2074  ows developers t
+00001aa0: 6f20 6372 6561 7465 2066 696e 6574 756e  o create finetun
+00001ab0: 696e 6720 6a6f 6273 2e20 4974 2061 6c73  ing jobs. It als
+00001ac0: 6f20 6861 7320 7365 7665 7261 6c20 6d65  o has several me
+00001ad0: 7468 6f64 7320 746f 206c 6973 7420 616c  thods to list al
+00001ae0: 6c20 6a6f 6273 2c20 7265 7472 6976 6520  l jobs, retrive 
+00001af0: 7374 6174 7573 6573 2061 6e64 2067 6574  statuses and get
+00001b00: 2063 6865 636b 706f 696e 7473 2e20 506c   checkpoints. Pl
+00001b10: 6561 7365 2072 6566 6572 2074 6f20 6f75  ease refer to ou
+00001b20: 7220 6669 6e65 2d74 756e 696e 6720 646f  r fine-tuning do
+00001b30: 6373 205b 6865 7265 5d28 6874 7470 733a  cs [here](https:
+00001b40: 2f2f 646f 6373 2e74 6f67 6574 6865 722e  //docs.together.
+00001b50: 6169 2f64 6f63 732f 6669 6e65 2d74 756e  ai/docs/fine-tun
+00001b60: 696e 672d 7079 7468 6f6e 292e 0a0a 6060  ing-python)...``
+00001b70: 6070 7974 686f 6e0a 696d 706f 7274 206f  `python.import o
+00001b80: 730a 6672 6f6d 2074 6f67 6574 6865 7220  s.from together 
+00001b90: 696d 706f 7274 2054 6f67 6574 6865 720a  import Together.
+00001ba0: 0a63 6c69 656e 7420 3d20 546f 6765 7468  .client = Togeth
+00001bb0: 6572 2861 7069 5f6b 6579 3d6f 732e 656e  er(api_key=os.en
+00001bc0: 7669 726f 6e2e 6765 7428 2254 4f47 4554  viron.get("TOGET
+00001bd0: 4845 525f 4150 495f 4b45 5922 2929 0a0a  HER_API_KEY"))..
+00001be0: 636c 6965 6e74 2e66 696e 655f 7475 6e69  client.fine_tuni
+00001bf0: 6e67 2e63 7265 6174 6528 0a20 2074 7261  ng.create(.  tra
+00001c00: 696e 696e 675f 6669 6c65 203d 2027 6669  ining_file = 'fi
+00001c10: 6c65 2d64 3064 3331 3863 622d 6237 6439  le-d0d318cb-b7d9
+00001c20: 2d34 3933 612d 6264 3730 2d31 6366 6530  -493a-bd70-1cfe0
+00001c30: 3839 6433 3831 3527 2c0a 2020 6d6f 6465  89d3815',.  mode
+00001c40: 6c20 3d20 276d 6973 7472 616c 6169 2f4d  l = 'mistralai/M
+00001c50: 6978 7472 616c 2d38 7837 422d 496e 7374  ixtral-8x7B-Inst
+00001c60: 7275 6374 2d76 302e 3127 2c0a 2020 6e5f  ruct-v0.1',.  n_
+00001c70: 6570 6f63 6873 203d 2033 2c0a 2020 6e5f  epochs = 3,.  n_
+00001c80: 6368 6563 6b70 6f69 6e74 7320 3d20 312c  checkpoints = 1,
+00001c90: 0a20 2062 6174 6368 5f73 697a 6520 3d20  .  batch_size = 
+00001ca0: 342c 0a20 206c 6561 726e 696e 675f 7261  4,.  learning_ra
+00001cb0: 7465 203d 2031 652d 352c 0a20 2073 7566  te = 1e-5,.  suf
+00001cc0: 6669 7820 3d20 276d 792d 6465 6d6f 2d66  fix = 'my-demo-f
+00001cd0: 696e 6574 756e 6527 2c0a 2020 7761 6e64  inetune',.  wand
+00001ce0: 625f 6170 695f 6b65 7920 3d20 2731 6132  b_api_key = '1a2
+00001cf0: 6233 6334 6435 652e 2e2e 2e2e 2e2e 272c  b3c4d5e.......',
+00001d00: 0a29 0a63 6c69 656e 742e 6669 6e65 5f74  .).client.fine_t
+00001d10: 756e 696e 672e 6c69 7374 2829 2023 206c  uning.list() # l
+00001d20: 6973 7473 2061 6c6c 2066 696e 652d 7475  ists all fine-tu
+00001d30: 6e65 6420 6a6f 6273 0a63 6c69 656e 742e  ned jobs.client.
+00001d40: 6669 6e65 5f74 756e 696e 672e 7265 7472  fine_tuning.retr
+00001d50: 6965 7665 2869 643d 2266 742d 6336 3661  ieve(id="ft-c66a
+00001d60: 3563 3138 2d31 6436 642d 3433 6339 2d39  5c18-1d6d-43c9-9
+00001d70: 3462 642d 3332 6437 3536 3432 3562 3462  4bd-32d756425b4b
+00001d80: 2229 2023 2072 6574 7269 6576 6573 2069  ") # retrieves i
+00001d90: 6e66 6f72 6d61 7469 6f6e 206f 6e20 6669  nformation on fi
+00001da0: 6e65 7475 6e65 2065 7665 6e74 0a63 6c69  netune event.cli
+00001db0: 656e 742e 6669 6e65 5f74 756e 696e 672e  ent.fine_tuning.
+00001dc0: 6361 6e63 656c 2869 643d 2266 742d 6336  cancel(id="ft-c6
+00001dd0: 3661 3563 3138 2d31 6436 642d 3433 6339  6a5c18-1d6d-43c9
+00001de0: 2d39 3462 642d 3332 6437 3536 3432 3562  -94bd-32d756425b
+00001df0: 3462 2229 2023 2043 616e 6365 6c73 2061  4b") # Cancels a
+00001e00: 2066 696e 652d 7475 6e69 6e67 206a 6f62   fine-tuning job
+00001e10: 0a63 6c69 656e 742e 6669 6e65 5f74 756e  .client.fine_tun
+00001e20: 696e 672e 6c69 7374 5f65 7665 6e74 7328  ing.list_events(
+00001e30: 6964 3d22 6674 2d63 3636 6135 6331 382d  id="ft-c66a5c18-
+00001e40: 3164 3664 2d34 3363 392d 3934 6264 2d33  1d6d-43c9-94bd-3
+00001e50: 3264 3735 3634 3235 6234 6222 2920 2320  2d756425b4b") # 
+00001e60: 204c 6973 7473 2065 7665 6e74 7320 6f66   Lists events of
+00001e70: 2061 2066 696e 652d 7475 6e65 206a 6f62   a fine-tune job
+00001e80: 0a63 6c69 656e 742e 6669 6e65 5f74 756e  .client.fine_tun
+00001e90: 696e 672e 646f 776e 6c6f 6164 2869 643d  ing.download(id=
+00001ea0: 2266 742d 6336 3661 3563 3138 2d31 6436  "ft-c66a5c18-1d6
+00001eb0: 642d 3433 6339 2d39 3462 642d 3332 6437  d-43c9-94bd-32d7
+00001ec0: 3536 3432 3562 3462 2229 2023 2064 6f77  56425b4b") # dow
+00001ed0: 6e6c 6f61 6473 2063 6f6d 7072 6573 7365  nloads compresse
+00001ee0: 6420 6669 6e65 2d74 756e 6564 206d 6f64  d fine-tuned mod
+00001ef0: 656c 206f 7220 6368 6563 6b70 6f69 6e74  el or checkpoint
+00001f00: 2074 6f20 6c6f 6361 6c20 6469 736b 0a60   to local disk.`
+00001f10: 6060 0a0a 2323 2320 4d6f 6465 6c73 0a0a  ``..### Models..
+00001f20: 5468 6973 206c 6973 7473 2061 6c6c 2074  This lists all t
+00001f30: 6865 206d 6f64 656c 7320 7468 6174 2054  he models that T
+00001f40: 6f67 6574 6865 7220 7375 7070 6f72 7473  ogether supports
+00001f50: 2e0a 0a60 6060 7079 7468 6f6e 0a69 6d70  ...```python.imp
+00001f60: 6f72 7420 6f73 0a66 726f 6d20 746f 6765  ort os.from toge
+00001f70: 7468 6572 2069 6d70 6f72 7420 546f 6765  ther import Toge
+00001f80: 7468 6572 0a0a 636c 6965 6e74 203d 2054  ther..client = T
+00001f90: 6f67 6574 6865 7228 6170 695f 6b65 793d  ogether(api_key=
+00001fa0: 6f73 2e65 6e76 6972 6f6e 2e67 6574 2822  os.environ.get("
+00001fb0: 544f 4745 5448 4552 5f41 5049 5f4b 4559  TOGETHER_API_KEY
+00001fc0: 2229 290a 0a6d 6f64 656c 7320 3d20 636c  "))..models = cl
+00001fd0: 6965 6e74 2e6d 6f64 656c 732e 6c69 7374  ient.models.list
+00001fe0: 2829 0a0a 666f 7220 6d6f 6465 6c20 696e  ()..for model in
+00001ff0: 206d 6f64 656c 733a 0a20 2020 2070 7269   models:.    pri
+00002000: 6e74 286d 6f64 656c 290a 6060 600a 0a23  nt(model).```..#
+00002010: 2320 5573 6167 6520 e280 9320 434c 490a  # Usage ... CLI.
+00002020: 0a23 2323 2043 6861 7420 436f 6d70 6c65  .### Chat Comple
+00002030: 7469 6f6e 730a 0a60 6060 6261 7368 0a74  tions..```bash.t
+00002040: 6f67 6574 6865 7220 6368 6174 2e63 6f6d  ogether chat.com
+00002050: 706c 6574 696f 6e73 205c 0a20 202d 2d6d  pletions \.  --m
+00002060: 6573 7361 6765 2022 7379 7374 656d 2220  essage "system" 
+00002070: 2259 6f75 2061 7265 2061 2068 656c 7066  "You are a helpf
+00002080: 756c 2061 7373 6973 7461 6e74 206e 616d  ul assistant nam
+00002090: 6564 2054 6f67 6574 6865 7222 205c 0a20  ed Together" \. 
+000020a0: 202d 2d6d 6573 7361 6765 2022 7573 6572   --message "user
+000020b0: 2220 2257 6861 7420 6973 2079 6f75 7220  " "What is your 
+000020c0: 6e61 6d65 3f22 205c 0a20 202d 2d6d 6f64  name?" \.  --mod
+000020d0: 656c 206d 6973 7472 616c 6169 2f4d 6978  el mistralai/Mix
+000020e0: 7472 616c 2d38 7837 422d 496e 7374 7275  tral-8x7B-Instru
+000020f0: 6374 2d76 302e 310a 6060 600a 0a54 6865  ct-v0.1.```..The
+00002100: 2043 6861 7420 436f 6d70 6c65 7469 6f6e   Chat Completion
+00002110: 7320 434c 4920 656e 6162 6c65 7320 7374  s CLI enables st
+00002120: 7265 616d 696e 6720 746f 6b65 6e73 2074  reaming tokens t
+00002130: 6f20 7374 646f 7574 2062 7920 6465 6661  o stdout by defa
+00002140: 756c 742e 2054 6f20 6469 7361 626c 6520  ult. To disable 
+00002150: 7374 7265 616d 696e 672c 2075 7365 2060  streaming, use `
+00002160: 2d2d 6e6f 2d73 7472 6561 6d60 2e0a 0a23  --no-stream`...#
+00002170: 2323 2043 6f6d 706c 6574 696f 6e73 0a0a  ## Completions..
+00002180: 6060 6062 6173 680a 746f 6765 7468 6572  ```bash.together
+00002190: 2063 6f6d 706c 6574 696f 6e73 205c 0a20   completions \. 
+000021a0: 2022 4c61 7267 6520 6c61 6e67 7561 6765   "Large language
+000021b0: 206d 6f64 656c 7320 6172 6520 2220 5c0a   models are " \.
+000021c0: 2020 2d2d 6d6f 6465 6c20 6d69 7374 7261    --model mistra
+000021d0: 6c61 692f 4d69 7874 7261 6c2d 3878 3742  lai/Mixtral-8x7B
+000021e0: 2d76 302e 3120 5c0a 2020 2d2d 6d61 782d  -v0.1 \.  --max-
+000021f0: 746f 6b65 6e73 2035 3132 205c 0a20 202d  tokens 512 \.  -
+00002200: 2d73 746f 7020 222e 220a 6060 600a 0a54  -stop ".".```..T
+00002210: 6865 2043 6f6d 706c 6574 696f 6e73 2043  he Completions C
+00002220: 4c49 2065 6e61 626c 6573 2073 7472 6561  LI enables strea
+00002230: 6d69 6e67 2074 6f6b 656e 7320 746f 2073  ming tokens to s
+00002240: 7464 6f75 7420 6279 2064 6566 6175 6c74  tdout by default
+00002250: 2e20 546f 2064 6973 6162 6c65 2073 7472  . To disable str
+00002260: 6561 6d69 6e67 2c20 7573 6520 602d 2d6e  eaming, use `--n
+00002270: 6f2d 7374 7265 616d 602e 0a0a 2323 2320  o-stream`...### 
+00002280: 496d 6167 6520 4765 6e65 7261 7469 6f6e  Image Generation
+00002290: 730a 0a60 6060 6261 7368 0a74 6f67 6574  s..```bash.toget
+000022a0: 6865 7220 696d 6167 6573 2067 656e 6572  her images gener
+000022b0: 6174 6520 5c0a 2020 2273 7061 6365 2072  ate \.  "space r
+000022c0: 6f62 6f74 7322 205c 0a20 202d 2d6d 6f64  obots" \.  --mod
+000022d0: 656c 2073 7461 6269 6c69 7479 6169 2f73  el stabilityai/s
+000022e0: 7461 626c 652d 6469 6666 7573 696f 6e2d  table-diffusion-
+000022f0: 786c 2d62 6173 652d 312e 3020 5c0a 2020  xl-base-1.0 \.  
+00002300: 2d2d 6e20 340a 6060 600a 0a54 6865 2069  --n 4.```..The i
+00002310: 6d61 6765 2069 7320 6f70 656e 6564 2069  mage is opened i
+00002320: 6e20 7468 6520 6465 6661 756c 7420 696d  n the default im
+00002330: 6167 6520 7669 6577 6572 2062 7920 6465  age viewer by de
+00002340: 6661 756c 742e 2054 6f20 6469 7361 626c  fault. To disabl
+00002350: 6520 7468 6973 2c20 7573 6520 602d 2d6e  e this, use `--n
+00002360: 6f2d 7368 6f77 602e 0a0a 2323 2320 4669  o-show`...### Fi
+00002370: 6c65 730a 0a60 6060 6261 7368 0a23 2048  les..```bash.# H
+00002380: 656c 700a 746f 6765 7468 6572 2066 696c  elp.together fil
+00002390: 6573 202d 2d68 656c 700a 0a23 2043 6865  es --help..# Che
+000023a0: 636b 2066 696c 650a 746f 6765 7468 6572  ck file.together
+000023b0: 2066 696c 6573 2063 6865 636b 2065 7861   files check exa
+000023c0: 6d70 6c65 2e6a 736f 6e6c 0a0a 2320 5570  mple.jsonl..# Up
+000023d0: 6c6f 6164 2066 696c 650a 746f 6765 7468  load file.togeth
+000023e0: 6572 2066 696c 6573 2075 706c 6f61 6420  er files upload 
+000023f0: 6578 616d 706c 652e 6a73 6f6e 6c0a 0a23  example.jsonl..#
+00002400: 204c 6973 7420 6669 6c65 730a 746f 6765   List files.toge
+00002410: 7468 6572 2066 696c 6573 206c 6973 740a  ther files list.
+00002420: 0a23 2052 6574 7269 6576 6520 6669 6c65  .# Retrieve file
+00002430: 206d 6574 6164 6174 610a 746f 6765 7468   metadata.togeth
+00002440: 6572 2066 696c 6573 2072 6574 7269 6576  er files retriev
+00002450: 6520 6669 6c65 2d36 6635 3066 3964 312d  e file-6f50f9d1-
+00002460: 3562 3935 2d34 3136 632d 3930 3430 2d30  5b95-416c-9040-0
+00002470: 3739 3962 3262 3462 3839 340a 0a23 2052  799b2b4b894..# R
+00002480: 6574 7269 6576 6520 6669 6c65 2063 6f6e  etrieve file con
+00002490: 7465 6e74 0a74 6f67 6574 6865 7220 6669  tent.together fi
+000024a0: 6c65 7320 7265 7472 6965 7665 2d63 6f6e  les retrieve-con
+000024b0: 7465 6e74 2066 696c 652d 3666 3530 6639  tent file-6f50f9
+000024c0: 6431 2d35 6239 352d 3431 3663 2d39 3034  d1-5b95-416c-904
+000024d0: 302d 3037 3939 6232 6234 6238 3934 0a0a  0-0799b2b4b894..
+000024e0: 2320 4465 6c65 7465 2072 656d 6f74 6520  # Delete remote 
+000024f0: 6669 6c65 0a74 6f67 6574 6865 7220 6669  file.together fi
+00002500: 6c65 7320 6465 6c65 7465 2066 696c 652d  les delete file-
+00002510: 3666 3530 6639 6431 2d35 6239 352d 3431  6f50f9d1-5b95-41
+00002520: 3663 2d39 3034 302d 3037 3939 6232 6234  6c-9040-0799b2b4
+00002530: 6238 3934 0a60 6060 0a0a 2323 2320 4669  b894.```..### Fi
+00002540: 6e65 2d74 756e 696e 670a 0a60 6060 6261  ne-tuning..```ba
+00002550: 7368 0a23 2048 656c 700a 746f 6765 7468  sh.# Help.togeth
+00002560: 6572 2066 696e 652d 7475 6e69 6e67 202d  er fine-tuning -
+00002570: 2d68 656c 700a 0a23 2043 7265 6174 6520  -help..# Create 
+00002580: 6669 6e65 2d74 756e 6520 6a6f 620a 746f  fine-tune job.to
+00002590: 6765 7468 6572 2066 696e 652d 7475 6e69  gether fine-tuni
+000025a0: 6e67 2063 7265 6174 6520 5c0a 2020 2d2d  ng create \.  --
+000025b0: 6d6f 6465 6c20 746f 6765 7468 6572 636f  model togetherco
+000025c0: 6d70 7574 6572 2f6c 6c61 6d61 2d32 2d37  mputer/llama-2-7
+000025d0: 622d 6368 6174 205c 0a20 202d 2d74 7261  b-chat \.  --tra
+000025e0: 696e 696e 672d 6669 6c65 2066 696c 652d  ining-file file-
+000025f0: 3731 3164 3837 3234 2d62 3365 332d 3461  711d8724-b3e3-4a
+00002600: 6532 2d62 3531 362d 3934 3834 3139 3538  e2-b516-94841958
+00002610: 3131 3764 0a0a 2320 4c69 7374 2066 696e  117d..# List fin
+00002620: 652d 7475 6e65 206a 6f62 730a 746f 6765  e-tune jobs.toge
+00002630: 7468 6572 2066 696e 652d 7475 6e69 6e67  ther fine-tuning
+00002640: 206c 6973 740a 0a23 2052 6574 7269 6576   list..# Retriev
+00002650: 6520 6669 6e65 2d74 756e 6520 6a6f 6220  e fine-tune job 
+00002660: 6465 7461 696c 730a 746f 6765 7468 6572  details.together
+00002670: 2066 696e 652d 7475 6e69 6e67 2072 6574   fine-tuning ret
+00002680: 7269 6576 6520 6674 2d63 3636 6135 6331  rieve ft-c66a5c1
+00002690: 382d 3164 3664 2d34 3363 392d 3934 6264  8-1d6d-43c9-94bd
+000026a0: 2d33 3264 3735 3634 3235 6234 620a 0a23  -32d756425b4b..#
+000026b0: 204c 6973 7420 6669 6e65 2d74 756e 6520   List fine-tune 
+000026c0: 6a6f 6220 6576 656e 7473 0a74 6f67 6574  job events.toget
+000026d0: 6865 7220 6669 6e65 2d74 756e 696e 6720  her fine-tuning 
+000026e0: 6c69 7374 2d65 7665 6e74 7320 6674 2d63  list-events ft-c
+000026f0: 3636 6135 6331 382d 3164 3664 2d34 3363  66a5c18-1d6d-43c
+00002700: 392d 3934 6264 2d33 3264 3735 3634 3235  9-94bd-32d756425
+00002710: 6234 620a 0a23 2043 616e 6365 6c20 7275  b4b..# Cancel ru
+00002720: 6e6e 696e 6720 6a6f 620a 746f 6765 7468  nning job.togeth
+00002730: 6572 2066 696e 652d 7475 6e69 6e67 2063  er fine-tuning c
+00002740: 616e 6365 6c20 6674 2d63 3636 6135 6331  ancel ft-c66a5c1
+00002750: 382d 3164 3664 2d34 3363 392d 3934 6264  8-1d6d-43c9-94bd
+00002760: 2d33 3264 3735 3634 3235 6234 620a 0a23  -32d756425b4b..#
+00002770: 2044 6f77 6e6c 6f61 6420 6669 6e65 2d74   Download fine-t
+00002780: 756e 6564 206d 6f64 656c 2077 6569 6768  uned model weigh
+00002790: 7473 0a74 6f67 6574 6865 7220 6669 6e65  ts.together fine
+000027a0: 2d74 756e 696e 6720 646f 776e 6c6f 6164  -tuning download
+000027b0: 2066 742d 6336 3661 3563 3138 2d31 6436   ft-c66a5c18-1d6
+000027c0: 642d 3433 6339 2d39 3462 642d 3332 6437  d-43c9-94bd-32d7
+000027d0: 3536 3432 3562 3462 0a60 6060 0a0a 2323  56425b4b.```..##
+000027e0: 2320 4d6f 6465 6c73 0a0a 6060 6062 6173  # Models..```bas
+000027f0: 680a 2320 4865 6c70 0a74 6f67 6574 6865  h.# Help.togethe
+00002800: 7220 6d6f 6465 6c73 202d 2d68 656c 700a  r models --help.
+00002810: 0a23 204c 6973 7420 6d6f 6465 6c73 0a74  .# List models.t
+00002820: 6f67 6574 6865 7220 6d6f 6465 6c73 206c  ogether models l
+00002830: 6973 740a 6060 600a 0a23 2320 436f 6e74  ist.```..## Cont
+00002840: 7269 6275 7469 6e67 0a0a 5265 6665 7220  ributing..Refer 
+00002850: 746f 2074 6865 205b 436f 6e74 7269 6275  to the [Contribu
+00002860: 7469 6e67 2047 7569 6465 5d28 434f 4e54  ting Guide](CONT
+00002870: 5249 4255 5449 4e47 2e6d 6429 0a         RIBUTING.md).
```

### Comparing `together-1.1.2/pyproject.toml` & `together-1.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "oldest-supported-numpy>=0.14; python_version<'3.9'",
     "numpy>=1.25; python_version>='3.9'",
 ]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "together"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
     "Together AI <support@together.ai>"
 ]
 description = "Python client for Together's Cloud Platform!"
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
@@ -32,29 +32,29 @@
 typer = ">=0.9,<0.13"
 requests = "^2.31.0"
 tqdm = "^4.66.2"
 tabulate = "^0.9.0"
 pydantic = "^2.6.3"
 aiohttp = "^3.9.3"
 filelock = "^3.13.1"
-eval-type-backport = "^0.1.3"
+eval-type-backport = ">=0.1.3,<0.3.0"
 click = "^8.1.7"
 pillow = "^10.3.0"
 pyarrow = ">=10.0.1"
 numpy = [
     { version = ">=1.23.5", python = "<3.12" },
     { version = ">=1.26.0", python = ">=3.12" },
 ]
 
 [tool.poetry.group.quality]
 optional = true
 
 [tool.poetry.group.quality.dependencies]
 black = ">=23.1,<25.0"
-ruff = "^0.3.2"
+ruff = ">=0.3.2,<0.5.0"
 types-tqdm = "^4.65.0.0"
 types-tabulate = "^0.9.0.3"
 pre-commit = "3.5.0"
 types-requests = "^2.31.0.20240218"
 pyarrow-stubs = "^10.0.1.7"
 mypy = "^1.9.0"
 
@@ -62,14 +62,21 @@
 optional = true
 
 [tool.poetry.group.tests.dependencies]
 pytest = ">=7.4.2,<9.0.0"
 pytest-watch = "^4.2.0"
 tox = "^4.14.1"
 
+[tool.poetry.group.examples]
+optional = true
+
+[tool.poetry.group.examples.dependencies]
+datasets = "^2.18.0"
+transformers = "^4.39.3"
+
 
 [tool.poetry.urls]
 "Homepage" = "https://github.com/togethercomputer/together-python"
 "Bug Tracker" = "https://github.com/togethercomputer/together-python/issues"
 
 [tool.poetry.scripts]
 together = "together.cli.cli:main"
```

### Comparing `together-1.1.2/src/together/__init__.py` & `together-1.1.3/src/together/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/abstract/api_requestor.py` & `together-1.1.3/src/together/abstract/api_requestor.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/cli/api/chat.py` & `together-1.1.3/src/together/cli/api/chat.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/cli/api/completions.py` & `together-1.1.3/src/together/cli/api/completions.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/cli/api/files.py` & `together-1.1.3/src/together/cli/api/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/cli/api/finetune.py` & `together-1.1.3/src/together/cli/api/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/cli/api/images.py` & `together-1.1.3/src/together/cli/api/images.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/cli/api/models.py` & `together-1.1.3/src/together/cli/api/models.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/cli/cli.py` & `together-1.1.3/src/together/cli/cli.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/client.py` & `together-1.1.3/src/together/client.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/constants.py` & `together-1.1.3/src/together/constants.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/error.py` & `together-1.1.3/src/together/error.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/filemanager.py` & `together-1.1.3/src/together/filemanager.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/legacy/base.py` & `together-1.1.3/src/together/legacy/base.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/legacy/complete.py` & `together-1.1.3/src/together/legacy/complete.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/legacy/embeddings.py` & `together-1.1.3/src/together/legacy/embeddings.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/legacy/files.py` & `together-1.1.3/src/together/legacy/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/legacy/finetune.py` & `together-1.1.3/src/together/legacy/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/legacy/images.py` & `together-1.1.3/src/together/legacy/images.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/legacy/models.py` & `together-1.1.3/src/together/legacy/models.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/resources/__init__.py` & `together-1.1.3/src/together/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/resources/chat/__init__.py` & `together-1.1.3/src/together/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/resources/chat/completions.py` & `together-1.1.3/src/together/resources/chat/completions.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/resources/completions.py` & `together-1.1.3/src/together/resources/completions.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/resources/embeddings.py` & `together-1.1.3/src/together/resources/embeddings.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/resources/files.py` & `together-1.1.3/src/together/resources/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/resources/finetune.py` & `together-1.1.3/src/together/resources/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/resources/images.py` & `together-1.1.3/src/together/resources/images.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/resources/models.py` & `together-1.1.3/src/together/resources/models.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/together_response.py` & `together-1.1.3/src/together/together_response.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/types/__init__.py` & `together-1.1.3/src/together/types/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/types/abstract.py` & `together-1.1.3/src/together/types/abstract.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/types/chat_completions.py` & `together-1.1.3/src/together/types/chat_completions.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 )
 
 
 class MessageRole(str, Enum):
     ASSISTANT = "assistant"
     SYSTEM = "system"
     USER = "user"
+    TOOL = "tool"
 
 
 class ResponseFormatType(str, Enum):
     JSON_OBJECT = "json_object"
 
 
 class FunctionCall(BaseModel):
```

### Comparing `together-1.1.2/src/together/types/common.py` & `together-1.1.3/src/together/types/common.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/types/completions.py` & `together-1.1.3/src/together/types/completions.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/types/embeddings.py` & `together-1.1.3/src/together/types/embeddings.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/types/files.py` & `together-1.1.3/src/together/types/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/types/finetune.py` & `together-1.1.3/src/together/types/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/types/images.py` & `together-1.1.3/src/together/types/images.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/types/models.py` & `together-1.1.3/src/together/types/models.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/utils/__init__.py` & `together-1.1.3/src/together/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/utils/_log.py` & `together-1.1.3/src/together/utils/_log.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/utils/api_helpers.py` & `together-1.1.3/src/together/utils/api_helpers.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/utils/files.py` & `together-1.1.3/src/together/utils/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/src/together/utils/tools.py` & `together-1.1.3/src/together/utils/tools.py`

 * *Files identical despite different names*

### Comparing `together-1.1.2/PKG-INFO` & `together-1.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 746f 6765  : 2.1.Name: toge
 00000020: 7468 6572 0a56 6572 7369 6f6e 3a20 312e  ther.Version: 1.
-00000030: 312e 320a 5375 6d6d 6172 793a 2050 7974  1.2.Summary: Pyt
+00000030: 312e 330a 5375 6d6d 6172 793a 2050 7974  1.3.Summary: Pyt
 00000040: 686f 6e20 636c 6965 6e74 2066 6f72 2054  hon client for T
 00000050: 6f67 6574 6865 7227 7320 436c 6f75 6420  ogether's Cloud 
 00000060: 506c 6174 666f 726d 210a 486f 6d65 2d70  Platform!.Home-p
 00000070: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
 00000080: 6875 622e 636f 6d2f 746f 6765 7468 6572  hub.com/together
 00000090: 636f 6d70 7574 6572 2f74 6f67 6574 6865  computer/togethe
 000000a0: 722d 7079 7468 6f6e 0a4c 6963 656e 7365  r-python.License
@@ -44,15 +44,15 @@
 000002b0: 6573 2d44 6973 743a 2061 696f 6874 7470  es-Dist: aiohttp
 000002c0: 2028 3e3d 332e 392e 332c 3c34 2e30 2e30   (>=3.9.3,<4.0.0
 000002d0: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
 000002e0: 2063 6c69 636b 2028 3e3d 382e 312e 372c   click (>=8.1.7,
 000002f0: 3c39 2e30 2e30 290a 5265 7175 6972 6573  <9.0.0).Requires
 00000300: 2d44 6973 743a 2065 7661 6c2d 7479 7065  -Dist: eval-type
 00000310: 2d62 6163 6b70 6f72 7420 283e 3d30 2e31  -backport (>=0.1
-00000320: 2e33 2c3c 302e 322e 3029 0a52 6571 7569  .3,<0.2.0).Requi
+00000320: 2e33 2c3c 302e 332e 3029 0a52 6571 7569  .3,<0.3.0).Requi
 00000330: 7265 732d 4469 7374 3a20 6669 6c65 6c6f  res-Dist: filelo
 00000340: 636b 2028 3e3d 332e 3133 2e31 2c3c 342e  ck (>=3.13.1,<4.
 00000350: 302e 3029 0a52 6571 7569 7265 732d 4469  0.0).Requires-Di
 00000360: 7374 3a20 6e75 6d70 7920 283e 3d31 2e32  st: numpy (>=1.2
 00000370: 332e 3529 203b 2070 7974 686f 6e5f 7665  3.5) ; python_ve
 00000380: 7273 696f 6e20 3c20 2233 2e31 3222 0a52  rsion < "3.12".R
 00000390: 6571 7569 7265 732d 4469 7374 3a20 6e75  equires-Dist: nu
@@ -84,612 +84,656 @@
 00000530: 5072 6f6a 6563 742d 5552 4c3a 2052 6570  Project-URL: Rep
 00000540: 6f73 6974 6f72 792c 2068 7474 7073 3a2f  ository, https:/
 00000550: 2f67 6974 6875 622e 636f 6d2f 746f 6765  /github.com/toge
 00000560: 7468 6572 636f 6d70 7574 6572 2f74 6f67  thercomputer/tog
 00000570: 6574 6865 722d 7079 7468 6f6e 0a44 6573  ether-python.Des
 00000580: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
 00000590: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-000005a0: 646f 776e 0a0a 5468 6520 5b54 6f67 6574  down..The [Toget
-000005b0: 6865 7220 5079 7468 6f6e 204c 6962 7261  her Python Libra
-000005c0: 7279 5d28 6874 7470 733a 2f2f 7079 7069  ry](https://pypi
-000005d0: 2e6f 7267 2f70 726f 6a65 6374 2f74 6f67  .org/project/tog
-000005e0: 6574 6865 722f 2920 6973 2074 6865 206f  ether/) is the o
-000005f0: 6666 6963 6961 6c20 5079 7468 6f6e 2063  fficial Python c
-00000600: 6c69 656e 7420 666f 7220 546f 6765 7468  lient for Togeth
-00000610: 6572 2773 2041 5049 2070 6c61 7466 6f72  er's API platfor
-00000620: 6d2c 2070 726f 7669 6469 6e67 2061 2063  m, providing a c
-00000630: 6f6e 7665 6e69 656e 7420 7761 7920 666f  onvenient way fo
-00000640: 7220 696e 7465 7261 6374 696e 6720 7769  r interacting wi
-00000650: 7468 2074 6865 2052 4553 5420 4150 4973  th the REST APIs
-00000660: 2061 6e64 2065 6e61 626c 6573 2065 6173   and enables eas
-00000670: 7920 696e 7465 6772 6174 696f 6e73 2077  y integrations w
-00000680: 6974 6820 5079 7468 6f6e 2033 2e38 2b20  ith Python 3.8+ 
-00000690: 6170 706c 6963 6174 696f 6e73 2077 6974  applications wit
-000006a0: 6820 6561 7379 2074 6f20 7573 6520 7379  h easy to use sy
-000006b0: 6e63 6872 6f6e 6f75 7320 616e 6420 6173  nchronous and as
-000006c0: 796e 6368 726f 6e6f 7573 2063 6c69 656e  ynchronous clien
-000006d0: 7473 2e0a 0a23 2049 6e73 7461 6c6c 6174  ts...# Installat
-000006e0: 696f 6e0a 0a3e 20f0 9f9a a70a 3e20 5468  ion..> .....> Th
-000006f0: 6520 6c69 6272 6172 7920 7761 7320 7265  e library was re
-00000700: 7772 6974 7465 6e20 696e 2076 312e 302e  written in v1.0.
-00000710: 3020 7265 6c65 6173 6564 2069 6e20 4170  0 released in Ap
-00000720: 7269 6c20 6f66 2032 3032 342e 2054 6865  ril of 2024. The
-00000730: 7265 2077 6572 6520 7369 676e 6966 6963  re were signific
-00000740: 616e 7420 6368 616e 6765 7320 6d61 6465  ant changes made
-00000750: 2e0a 0a54 6f20 696e 7374 616c 6c20 546f  ...To install To
-00000760: 6765 7468 6572 2050 7974 686f 6e20 4c69  gether Python Li
-00000770: 6272 6172 7920 6672 6f6d 2050 7950 692c  brary from PyPi,
-00000780: 2073 696d 706c 7920 7275 6e3a 0a0a 6060   simply run:..``
-00000790: 6073 6865 6c6c 2053 6865 6c6c 0a70 6970  `shell Shell.pip
-000007a0: 2069 6e73 7461 6c6c 202d 2d75 7067 7261   install --upgra
-000007b0: 6465 2074 6f67 6574 6865 720a 6060 600a  de together.```.
-000007c0: 0a23 2320 5365 7474 696e 6720 7570 2041  .## Setting up A
-000007d0: 5049 204b 6579 0a0a 3e20 f09f 9aa7 2059  PI Key..> .... Y
-000007e0: 6f75 2077 696c 6c20 6e65 6564 2074 6f20  ou will need to 
-000007f0: 6372 6561 7465 2061 6e20 6163 636f 756e  create an accoun
-00000800: 7420 7769 7468 205b 546f 6765 7468 6572  t with [Together
-00000810: 2e61 695d 2868 7474 7073 3a2f 2f61 7069  .ai](https://api
-00000820: 2e74 6f67 6574 6865 722e 7879 7a2f 2920  .together.xyz/) 
-00000830: 746f 206f 6274 6169 6e20 6120 546f 6765  to obtain a Toge
-00000840: 7468 6572 2041 5049 204b 6579 2e0a 0a4f  ther API Key...O
-00000850: 6e63 6520 6c6f 6767 6564 2069 6e20 746f  nce logged in to
-00000860: 2074 6865 2054 6f67 6574 6865 7220 506c   the Together Pl
-00000870: 6179 6772 6f75 6e64 2c20 796f 7520 6361  ayground, you ca
-00000880: 6e20 6669 6e64 2061 7661 696c 6162 6c65  n find available
-00000890: 2041 5049 206b 6579 7320 696e 205b 7468   API keys in [th
-000008a0: 6973 2073 6574 7469 6e67 7320 7061 6765  is settings page
-000008b0: 5d28 6874 7470 733a 2f2f 6170 692e 746f  ](https://api.to
-000008c0: 6765 7468 6572 2e78 797a 2f73 6574 7469  gether.xyz/setti
-000008d0: 6e67 732f 6170 692d 6b65 7973 292e 0a0a  ngs/api-keys)...
-000008e0: 2323 2320 5365 7474 696e 6720 656e 7669  ### Setting envi
-000008f0: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
-00000900: 0a0a 6060 6073 6865 6c6c 0a65 7870 6f72  ..```shell.expor
-00000910: 7420 544f 4745 5448 4552 5f41 5049 5f4b  t TOGETHER_API_K
-00000920: 4559 3d78 7878 7878 0a60 6060 0a0a 2323  EY=xxxxx.```..##
-00000930: 2320 5573 696e 6720 7468 6520 636c 6965  # Using the clie
-00000940: 6e74 0a0a 6060 6070 7974 686f 6e0a 6672  nt..```python.fr
-00000950: 6f6d 2074 6f67 6574 6865 7220 696d 706f  om together impo
-00000960: 7274 2054 6f67 6574 6865 720a 0a63 6c69  rt Together..cli
-00000970: 656e 7420 3d20 546f 6765 7468 6572 2861  ent = Together(a
-00000980: 7069 5f6b 6579 3d22 7878 7878 7822 290a  pi_key="xxxxx").
-00000990: 6060 600a 0a54 6869 7320 6c69 6272 6172  ```..This librar
-000009a0: 7920 636f 6e74 6169 6e73 2062 6f74 6820  y contains both 
-000009b0: 6120 7079 7468 6f6e 206c 6962 7261 7279  a python library
-000009c0: 2061 6e64 2061 2043 4c49 2e20 5765 276c   and a CLI. We'l
-000009d0: 6c20 6465 6d6f 6e73 7472 6174 6520 686f  l demonstrate ho
-000009e0: 7720 746f 2075 7365 2062 6f74 6820 6265  w to use both be
-000009f0: 6c6f 772e 0a0a 2320 5573 6167 6520 e280  low...# Usage ..
-00000a00: 9320 5079 7468 6f6e 2043 6c69 656e 740a  . Python Client.
-00000a10: 0a23 2320 4368 6174 2043 6f6d 706c 6574  .## Chat Complet
-00000a20: 696f 6e73 0a0a 6060 6070 7974 686f 6e0a  ions..```python.
-00000a30: 696d 706f 7274 206f 730a 6672 6f6d 2074  import os.from t
-00000a40: 6f67 6574 6865 7220 696d 706f 7274 2054  ogether import T
-00000a50: 6f67 6574 6865 720a 0a63 6c69 656e 7420  ogether..client 
-00000a60: 3d20 546f 6765 7468 6572 2861 7069 5f6b  = Together(api_k
-00000a70: 6579 3d6f 732e 656e 7669 726f 6e2e 6765  ey=os.environ.ge
-00000a80: 7428 2254 4f47 4554 4845 525f 4150 495f  t("TOGETHER_API_
-00000a90: 4b45 5922 2929 0a0a 7265 7370 6f6e 7365  KEY"))..response
-00000aa0: 203d 2063 6c69 656e 742e 6368 6174 2e63   = client.chat.c
-00000ab0: 6f6d 706c 6574 696f 6e73 2e63 7265 6174  ompletions.creat
-00000ac0: 6528 0a20 2020 206d 6f64 656c 3d22 6d69  e(.    model="mi
-00000ad0: 7374 7261 6c61 692f 4d69 7874 7261 6c2d  stralai/Mixtral-
-00000ae0: 3878 3742 2d49 6e73 7472 7563 742d 7630  8x7B-Instruct-v0
-00000af0: 2e31 222c 0a20 2020 206d 6573 7361 6765  .1",.    message
-00000b00: 733d 5b7b 2272 6f6c 6522 3a20 2275 7365  s=[{"role": "use
-00000b10: 7222 2c20 2263 6f6e 7465 6e74 223a 2022  r", "content": "
-00000b20: 7465 6c6c 206d 6520 6162 6f75 7420 6e65  tell me about ne
-00000b30: 7720 796f 726b 227d 5d2c 0a29 0a70 7269  w york"}],.).pri
-00000b40: 6e74 2872 6573 706f 6e73 652e 6368 6f69  nt(response.choi
-00000b50: 6365 735b 305d 2e6d 6573 7361 6765 2e63  ces[0].message.c
-00000b60: 6f6e 7465 6e74 290a 6060 600a 0a23 2323  ontent).```..###
-00000b70: 2053 7472 6561 6d69 6e67 0a0a 6060 6070   Streaming..```p
-00000b80: 7974 686f 6e0a 696d 706f 7274 206f 730a  ython.import os.
-00000b90: 6672 6f6d 2074 6f67 6574 6865 7220 696d  from together im
-00000ba0: 706f 7274 2054 6f67 6574 6865 720a 0a63  port Together..c
-00000bb0: 6c69 656e 7420 3d20 546f 6765 7468 6572  lient = Together
-00000bc0: 2861 7069 5f6b 6579 3d6f 732e 656e 7669  (api_key=os.envi
-00000bd0: 726f 6e2e 6765 7428 2254 4f47 4554 4845  ron.get("TOGETHE
-00000be0: 525f 4150 495f 4b45 5922 2929 0a73 7472  R_API_KEY")).str
-00000bf0: 6561 6d20 3d20 636c 6965 6e74 2e63 6861  eam = client.cha
-00000c00: 742e 636f 6d70 6c65 7469 6f6e 732e 6372  t.completions.cr
-00000c10: 6561 7465 280a 2020 2020 6d6f 6465 6c3d  eate(.    model=
-00000c20: 226d 6973 7472 616c 6169 2f4d 6978 7472  "mistralai/Mixtr
-00000c30: 616c 2d38 7837 422d 496e 7374 7275 6374  al-8x7B-Instruct
-00000c40: 2d76 302e 3122 2c0a 2020 2020 6d65 7373  -v0.1",.    mess
-00000c50: 6167 6573 3d5b 7b22 726f 6c65 223a 2022  ages=[{"role": "
-00000c60: 7573 6572 222c 2022 636f 6e74 656e 7422  user", "content"
-00000c70: 3a20 2274 656c 6c20 6d65 2061 626f 7574  : "tell me about
-00000c80: 206e 6577 2079 6f72 6b22 7d5d 2c0a 2020   new york"}],.  
-00000c90: 2020 7374 7265 616d 3d54 7275 652c 0a29    stream=True,.)
-00000ca0: 0a0a 666f 7220 6368 756e 6b20 696e 2073  ..for chunk in s
-00000cb0: 7472 6561 6d3a 0a20 2020 2070 7269 6e74  tream:.    print
-00000cc0: 2863 6875 6e6b 2e63 686f 6963 6573 5b30  (chunk.choices[0
-00000cd0: 5d2e 6465 6c74 612e 636f 6e74 656e 7420  ].delta.content 
-00000ce0: 6f72 2022 222c 2065 6e64 3d22 222c 2066  or "", end="", f
-00000cf0: 6c75 7368 3d54 7275 6529 0a60 6060 0a0a  lush=True).```..
-00000d00: 2323 2320 4173 796e 6320 7573 6167 650a  ### Async usage.
-00000d10: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
-00000d20: 7420 6f73 2c20 6173 796e 6369 6f0a 6672  t os, asyncio.fr
-00000d30: 6f6d 2074 6f67 6574 6865 7220 696d 706f  om together impo
-00000d40: 7274 2041 7379 6e63 546f 6765 7468 6572  rt AsyncTogether
-00000d50: 0a0a 6173 796e 635f 636c 6965 6e74 203d  ..async_client =
-00000d60: 2041 7379 6e63 546f 6765 7468 6572 2861   AsyncTogether(a
-00000d70: 7069 5f6b 6579 3d6f 732e 656e 7669 726f  pi_key=os.enviro
-00000d80: 6e2e 6765 7428 2254 4f47 4554 4845 525f  n.get("TOGETHER_
-00000d90: 4150 495f 4b45 5922 2929 0a6d 6573 7361  API_KEY")).messa
-00000da0: 6765 7320 3d20 5b0a 2020 2020 2257 6861  ges = [.    "Wha
-00000db0: 7420 6172 6520 7468 6520 746f 7020 7468  t are the top th
-00000dc0: 696e 6773 2074 6f20 646f 2069 6e20 5361  ings to do in Sa
-00000dd0: 6e20 4672 616e 6369 7363 6f3f 222c 0a20  n Francisco?",. 
-00000de0: 2020 2022 5768 6174 2063 6f75 6e74 7279     "What country
-00000df0: 2069 7320 5061 7269 7320 696e 3f22 2c0a   is Paris in?",.
-00000e00: 5d0a 0a61 7379 6e63 2064 6566 2061 7379  ]..async def asy
-00000e10: 6e63 5f63 6861 745f 636f 6d70 6c65 7469  nc_chat_completi
-00000e20: 6f6e 286d 6573 7361 6765 7329 3a0a 2020  on(messages):.  
-00000e30: 2020 6173 796e 635f 636c 6965 6e74 203d    async_client =
-00000e40: 2041 7379 6e63 546f 6765 7468 6572 2861   AsyncTogether(a
-00000e50: 7069 5f6b 6579 3d6f 732e 656e 7669 726f  pi_key=os.enviro
-00000e60: 6e2e 6765 7428 2254 4f47 4554 4845 525f  n.get("TOGETHER_
-00000e70: 4150 495f 4b45 5922 2929 0a20 2020 2074  API_KEY")).    t
-00000e80: 6173 6b73 203d 205b 0a20 2020 2020 2020  asks = [.       
-00000e90: 2061 7379 6e63 5f63 6c69 656e 742e 6368   async_client.ch
-00000ea0: 6174 2e63 6f6d 706c 6574 696f 6e73 2e63  at.completions.c
-00000eb0: 7265 6174 6528 0a20 2020 2020 2020 2020  reate(.         
-00000ec0: 2020 206d 6f64 656c 3d22 6d69 7374 7261     model="mistra
-00000ed0: 6c61 692f 4d69 7874 7261 6c2d 3878 3742  lai/Mixtral-8x7B
-00000ee0: 2d49 6e73 7472 7563 742d 7630 2e31 222c  -Instruct-v0.1",
-00000ef0: 0a20 2020 2020 2020 2020 2020 206d 6573  .            mes
-00000f00: 7361 6765 733d 5b7b 2272 6f6c 6522 3a20  sages=[{"role": 
-00000f10: 2275 7365 7222 2c20 2263 6f6e 7465 6e74  "user", "content
-00000f20: 223a 206d 6573 7361 6765 7d5d 2c0a 2020  ": message}],.  
-00000f30: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00000f40: 666f 7220 6d65 7373 6167 6520 696e 206d  for message in m
-00000f50: 6573 7361 6765 730a 2020 2020 5d0a 2020  essages.    ].  
-00000f60: 2020 7265 7370 6f6e 7365 7320 3d20 6177    responses = aw
-00000f70: 6169 7420 6173 796e 6369 6f2e 6761 7468  ait asyncio.gath
-00000f80: 6572 282a 7461 736b 7329 0a0a 2020 2020  er(*tasks)..    
-00000f90: 666f 7220 7265 7370 6f6e 7365 2069 6e20  for response in 
-00000fa0: 7265 7370 6f6e 7365 733a 0a20 2020 2020  responses:.     
-00000fb0: 2020 2070 7269 6e74 2872 6573 706f 6e73     print(respons
-00000fc0: 652e 6368 6f69 6365 735b 305d 2e6d 6573  e.choices[0].mes
-00000fd0: 7361 6765 2e63 6f6e 7465 6e74 290a 0a61  sage.content)..a
-00000fe0: 7379 6e63 696f 2e72 756e 2861 7379 6e63  syncio.run(async
-00000ff0: 5f63 6861 745f 636f 6d70 6c65 7469 6f6e  _chat_completion
-00001000: 286d 6573 7361 6765 7329 290a 6060 600a  (messages)).```.
-00001010: 0a23 2320 436f 6d70 6c65 7469 6f6e 730a  .## Completions.
-00001020: 0a43 6f6d 706c 6574 696f 6e73 2061 7265  .Completions are
-00001030: 2066 6f72 2063 6f64 6520 616e 6420 6c61   for code and la
-00001040: 6e67 7561 6765 206d 6f64 656c 7320 7368  nguage models sh
-00001050: 6f77 6e20 5b68 6572 655d 2868 7474 7073  own [here](https
-00001060: 3a2f 2f64 6f63 732e 746f 6765 7468 6572  ://docs.together
-00001070: 2e61 692f 646f 6373 2f69 6e66 6572 656e  .ai/docs/inferen
-00001080: 6365 2d6d 6f64 656c 7329 2e20 4265 6c6f  ce-models). Belo
-00001090: 772c 2061 2063 6f64 6520 6d6f 6465 6c20  w, a code model 
-000010a0: 6578 616d 706c 6520 6973 2073 686f 776e  example is shown
-000010b0: 2e0a 0a60 6060 7079 7468 6f6e 0a69 6d70  ...```python.imp
-000010c0: 6f72 7420 6f73 0a66 726f 6d20 746f 6765  ort os.from toge
-000010d0: 7468 6572 2069 6d70 6f72 7420 546f 6765  ther import Toge
-000010e0: 7468 6572 0a0a 636c 6965 6e74 203d 2054  ther..client = T
-000010f0: 6f67 6574 6865 7228 6170 695f 6b65 793d  ogether(api_key=
-00001100: 6f73 2e65 6e76 6972 6f6e 2e67 6574 2822  os.environ.get("
-00001110: 544f 4745 5448 4552 5f41 5049 5f4b 4559  TOGETHER_API_KEY
-00001120: 2229 290a 0a72 6573 706f 6e73 6520 3d20  "))..response = 
-00001130: 636c 6965 6e74 2e63 6f6d 706c 6574 696f  client.completio
-00001140: 6e73 2e63 7265 6174 6528 0a20 2020 206d  ns.create(.    m
-00001150: 6f64 656c 3d22 636f 6465 6c6c 616d 612f  odel="codellama/
-00001160: 436f 6465 4c6c 616d 612d 3334 622d 5079  CodeLlama-34b-Py
-00001170: 7468 6f6e 2d68 6622 2c0a 2020 2020 7072  thon-hf",.    pr
-00001180: 6f6d 7074 3d22 5772 6974 6520 6120 4e65  ompt="Write a Ne
-00001190: 7874 2e6a 7320 636f 6d70 6f6e 656e 7420  xt.js component 
-000011a0: 7769 7468 2054 6169 6c77 696e 6443 5353  with TailwindCSS
-000011b0: 2066 6f72 2061 2068 6561 6465 7220 636f   for a header co
-000011c0: 6d70 6f6e 656e 742e 222c 0a29 0a70 7269  mponent.",.).pri
-000011d0: 6e74 2872 6573 706f 6e73 652e 6368 6f69  nt(response.choi
-000011e0: 6365 735b 305d 2e74 6578 7429 0a60 6060  ces[0].text).```
-000011f0: 0a0a 2323 2320 5374 7265 616d 696e 670a  ..### Streaming.
-00001200: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
-00001210: 7420 6f73 0a66 726f 6d20 746f 6765 7468  t os.from togeth
-00001220: 6572 2069 6d70 6f72 7420 546f 6765 7468  er import Togeth
-00001230: 6572 0a0a 636c 6965 6e74 203d 2054 6f67  er..client = Tog
-00001240: 6574 6865 7228 6170 695f 6b65 793d 6f73  ether(api_key=os
-00001250: 2e65 6e76 6972 6f6e 2e67 6574 2822 544f  .environ.get("TO
-00001260: 4745 5448 4552 5f41 5049 5f4b 4559 2229  GETHER_API_KEY")
-00001270: 290a 7374 7265 616d 203d 2063 6c69 656e  ).stream = clien
-00001280: 742e 636f 6d70 6c65 7469 6f6e 732e 6372  t.completions.cr
-00001290: 6561 7465 280a 2020 2020 6d6f 6465 6c3d  eate(.    model=
-000012a0: 2263 6f64 656c 6c61 6d61 2f43 6f64 654c  "codellama/CodeL
-000012b0: 6c61 6d61 2d33 3462 2d50 7974 686f 6e2d  lama-34b-Python-
-000012c0: 6866 222c 0a20 2020 2070 726f 6d70 743d  hf",.    prompt=
-000012d0: 2257 7269 7465 2061 204e 6578 742e 6a73  "Write a Next.js
-000012e0: 2063 6f6d 706f 6e65 6e74 2077 6974 6820   component with 
-000012f0: 5461 696c 7769 6e64 4353 5320 666f 7220  TailwindCSS for 
-00001300: 6120 6865 6164 6572 2063 6f6d 706f 6e65  a header compone
-00001310: 6e74 2e22 2c0a 2020 2020 7374 7265 616d  nt.",.    stream
-00001320: 3d54 7275 652c 0a29 0a0a 666f 7220 6368  =True,.)..for ch
-00001330: 756e 6b20 696e 2073 7472 6561 6d3a 0a20  unk in stream:. 
-00001340: 2020 2070 7269 6e74 2863 6875 6e6b 2e63     print(chunk.c
-00001350: 686f 6963 6573 5b30 5d2e 6465 6c74 612e  hoices[0].delta.
-00001360: 636f 6e74 656e 7420 6f72 2022 222c 2065  content or "", e
-00001370: 6e64 3d22 222c 2066 6c75 7368 3d54 7275  nd="", flush=Tru
-00001380: 6529 0a60 6060 0a0a 2323 2320 4173 796e  e).```..### Asyn
-00001390: 6320 7573 6167 650a 0a60 6060 7079 7468  c usage..```pyth
-000013a0: 6f6e 0a69 6d70 6f72 7420 6f73 2c20 6173  on.import os, as
-000013b0: 796e 6369 6f0a 6672 6f6d 2074 6f67 6574  yncio.from toget
-000013c0: 6865 7220 696d 706f 7274 2041 7379 6e63  her import Async
-000013d0: 546f 6765 7468 6572 0a0a 6173 796e 635f  Together..async_
-000013e0: 636c 6965 6e74 203d 2041 7379 6e63 546f  client = AsyncTo
-000013f0: 6765 7468 6572 2861 7069 5f6b 6579 3d6f  gether(api_key=o
-00001400: 732e 656e 7669 726f 6e2e 6765 7428 2254  s.environ.get("T
-00001410: 4f47 4554 4845 525f 4150 495f 4b45 5922  OGETHER_API_KEY"
-00001420: 2929 0a70 726f 6d70 7473 203d 205b 0a20  )).prompts = [. 
-00001430: 2020 2022 5772 6974 6520 6120 4e65 7874     "Write a Next
-00001440: 2e6a 7320 636f 6d70 6f6e 656e 7420 7769  .js component wi
-00001450: 7468 2054 6169 6c77 696e 6443 5353 2066  th TailwindCSS f
-00001460: 6f72 2061 2068 6561 6465 7220 636f 6d70  or a header comp
-00001470: 6f6e 656e 742e 222c 0a20 2020 2022 5772  onent.",.    "Wr
-00001480: 6974 6520 6120 7079 7468 6f6e 2066 756e  ite a python fun
-00001490: 6374 696f 6e20 666f 7220 7468 6520 6669  ction for the fi
-000014a0: 626f 6e61 6363 6920 7365 7175 656e 6365  bonacci sequence
-000014b0: 222c 0a5d 0a0a 6173 796e 6320 6465 6620  ",.]..async def 
-000014c0: 6173 796e 635f 6368 6174 5f63 6f6d 706c  async_chat_compl
-000014d0: 6574 696f 6e28 7072 6f6d 7074 7329 3a0a  etion(prompts):.
-000014e0: 2020 2020 6173 796e 635f 636c 6965 6e74      async_client
-000014f0: 203d 2041 7379 6e63 546f 6765 7468 6572   = AsyncTogether
-00001500: 2861 7069 5f6b 6579 3d6f 732e 656e 7669  (api_key=os.envi
-00001510: 726f 6e2e 6765 7428 2254 4f47 4554 4845  ron.get("TOGETHE
-00001520: 525f 4150 495f 4b45 5922 2929 0a20 2020  R_API_KEY")).   
-00001530: 2074 6173 6b73 203d 205b 0a20 2020 2020   tasks = [.     
-00001540: 2020 2061 7379 6e63 5f63 6c69 656e 742e     async_client.
-00001550: 636f 6d70 6c65 7469 6f6e 732e 6372 6561  completions.crea
-00001560: 7465 280a 2020 2020 2020 2020 2020 2020  te(.            
-00001570: 6d6f 6465 6c3d 2263 6f64 656c 6c61 6d61  model="codellama
-00001580: 2f43 6f64 654c 6c61 6d61 2d33 3462 2d50  /CodeLlama-34b-P
-00001590: 7974 686f 6e2d 6866 222c 0a20 2020 2020  ython-hf",.     
-000015a0: 2020 2020 2020 2070 726f 6d70 743d 7072         prompt=pr
-000015b0: 6f6d 7074 2c0a 2020 2020 2020 2020 290a  ompt,.        ).
-000015c0: 2020 2020 2020 2020 666f 7220 7072 6f6d          for prom
-000015d0: 7074 2069 6e20 7072 6f6d 7074 730a 2020  pt in prompts.  
-000015e0: 2020 5d0a 2020 2020 7265 7370 6f6e 7365    ].    response
-000015f0: 7320 3d20 6177 6169 7420 6173 796e 6369  s = await asynci
-00001600: 6f2e 6761 7468 6572 282a 7461 736b 7329  o.gather(*tasks)
-00001610: 0a0a 2020 2020 666f 7220 7265 7370 6f6e  ..    for respon
-00001620: 7365 2069 6e20 7265 7370 6f6e 7365 733a  se in responses:
-00001630: 0a20 2020 2020 2020 2070 7269 6e74 2872  .        print(r
-00001640: 6573 706f 6e73 652e 6368 6f69 6365 735b  esponse.choices[
-00001650: 305d 2e74 6578 7429 0a0a 6173 796e 6369  0].text)..asynci
-00001660: 6f2e 7275 6e28 6173 796e 635f 6368 6174  o.run(async_chat
-00001670: 5f63 6f6d 706c 6574 696f 6e28 7072 6f6d  _completion(prom
-00001680: 7074 7329 290a 6060 600a 0a23 2320 496d  pts)).```..## Im
-00001690: 6167 6520 6765 6e65 7261 7469 6f6e 0a0a  age generation..
-000016a0: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
-000016b0: 206f 730a 6672 6f6d 2074 6f67 6574 6865   os.from togethe
-000016c0: 7220 696d 706f 7274 2054 6f67 6574 6865  r import Togethe
-000016d0: 720a 0a63 6c69 656e 7420 3d20 546f 6765  r..client = Toge
-000016e0: 7468 6572 2861 7069 5f6b 6579 3d6f 732e  ther(api_key=os.
-000016f0: 656e 7669 726f 6e2e 6765 7428 2254 4f47  environ.get("TOG
-00001700: 4554 4845 525f 4150 495f 4b45 5922 2929  ETHER_API_KEY"))
-00001710: 0a0a 7265 7370 6f6e 7365 203d 2063 6c69  ..response = cli
-00001720: 656e 742e 696d 6167 6573 2e67 656e 6572  ent.images.gener
-00001730: 6174 6528 0a20 2020 2070 726f 6d70 743d  ate(.    prompt=
-00001740: 2273 7061 6365 2072 6f62 6f74 7322 2c0a  "space robots",.
-00001750: 2020 2020 6d6f 6465 6c3d 2273 7461 6269      model="stabi
-00001760: 6c69 7479 6169 2f73 7461 626c 652d 6469  lityai/stable-di
-00001770: 6666 7573 696f 6e2d 786c 2d62 6173 652d  ffusion-xl-base-
-00001780: 312e 3022 2c0a 2020 2020 7374 6570 733d  1.0",.    steps=
-00001790: 3130 2c0a 2020 2020 6e3d 342c 0a29 0a70  10,.    n=4,.).p
-000017a0: 7269 6e74 2872 6573 706f 6e73 652e 6461  rint(response.da
-000017b0: 7461 5b30 5d2e 6236 345f 6a73 6f6e 290a  ta[0].b64_json).
-000017c0: 6060 600a 0a23 2320 456d 6265 6464 696e  ```..## Embeddin
-000017d0: 6773 0a0a 6060 6070 7974 686f 6e0a 6672  gs..```python.fr
-000017e0: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
-000017f0: 204c 6973 740a 6672 6f6d 2074 6f67 6574   List.from toget
-00001800: 6865 7220 696d 706f 7274 2054 6f67 6574  her import Toget
-00001810: 6865 720a 0a63 6c69 656e 7420 3d20 546f  her..client = To
-00001820: 6765 7468 6572 2861 7069 5f6b 6579 3d6f  gether(api_key=o
-00001830: 732e 656e 7669 726f 6e2e 6765 7428 2254  s.environ.get("T
-00001840: 4f47 4554 4845 525f 4150 495f 4b45 5922  OGETHER_API_KEY"
-00001850: 2929 0a0a 6465 6620 6765 745f 656d 6265  ))..def get_embe
-00001860: 6464 696e 6773 2874 6578 7473 3a20 4c69  ddings(texts: Li
-00001870: 7374 5b73 7472 5d2c 206d 6f64 656c 3a20  st[str], model: 
-00001880: 7374 7229 202d 3e20 4c69 7374 5b4c 6973  str) -> List[Lis
-00001890: 745b 666c 6f61 745d 5d3a 0a20 2020 2074  t[float]]:.    t
-000018a0: 6578 7473 203d 205b 7465 7874 2e72 6570  exts = [text.rep
-000018b0: 6c61 6365 2822 5c6e 222c 2022 2022 2920  lace("\n", " ") 
-000018c0: 666f 7220 7465 7874 2069 6e20 7465 7874  for text in text
-000018d0: 735d 0a20 2020 206f 7574 7075 7473 203d  s].    outputs =
-000018e0: 2063 6c69 656e 742e 656d 6265 6464 696e   client.embeddin
-000018f0: 6773 2e63 7265 6174 6528 6d6f 6465 6c3d  gs.create(model=
-00001900: 6d6f 6465 6c2c 2069 6e70 7574 203d 2074  model, input = t
-00001910: 6578 7473 290a 2020 2020 7265 7475 726e  exts).    return
-00001920: 205b 6f75 7470 7574 732e 6461 7461 5b69   [outputs.data[i
-00001930: 5d2e 656d 6265 6464 696e 6720 666f 7220  ].embedding for 
-00001940: 6920 696e 2072 616e 6765 286c 656e 2874  i in range(len(t
-00001950: 6578 7473 2929 5d0a 0a69 6e70 7574 5f74  exts))]..input_t
-00001960: 6578 7473 203d 205b 274f 7572 2073 6f6c  exts = ['Our sol
-00001970: 6172 2073 7973 7465 6d20 6f72 6269 7473  ar system orbits
-00001980: 2074 6865 204d 696c 6b79 2057 6179 2067   the Milky Way g
-00001990: 616c 6178 7920 6174 2061 626f 7574 2035  alaxy at about 5
-000019a0: 3135 2c30 3030 206d 7068 275d 0a65 6d62  15,000 mph'].emb
-000019b0: 6564 6469 6e67 7320 3d20 6765 745f 656d  eddings = get_em
-000019c0: 6265 6464 696e 6773 2869 6e70 7574 5f74  beddings(input_t
-000019d0: 6578 7473 2c20 6d6f 6465 6c3d 2774 6f67  exts, model='tog
-000019e0: 6574 6865 7263 6f6d 7075 7465 722f 6d32  ethercomputer/m2
-000019f0: 2d62 6572 742d 3830 4d2d 386b 2d72 6574  -bert-80M-8k-ret
-00001a00: 7269 6576 616c 2729 0a0a 7072 696e 7428  rieval')..print(
-00001a10: 656d 6265 6464 696e 6773 290a 6060 600a  embeddings).```.
-00001a20: 0a23 2320 4669 6c65 730a 0a54 6865 2066  .## Files..The f
-00001a30: 696c 6573 2041 5049 2069 7320 7573 6564  iles API is used
-00001a40: 2066 6f72 2066 696e 652d 7475 6e69 6e67   for fine-tuning
-00001a50: 2061 6e64 2061 6c6c 6f77 7320 6465 7665   and allows deve
-00001a60: 6c6f 7065 7273 2074 6f20 7570 6c6f 6164  lopers to upload
-00001a70: 2064 6174 6120 746f 2066 696e 652d 7475   data to fine-tu
-00001a80: 6e65 206f 6e2e 2049 7420 616c 736f 2068  ne on. It also h
-00001a90: 6173 2073 6576 6572 616c 206d 6574 686f  as several metho
-00001aa0: 6473 2074 6f20 6c69 7374 2061 6c6c 2066  ds to list all f
-00001ab0: 696c 6573 2c20 7265 7472 6976 6520 6669  iles, retrive fi
-00001ac0: 6c65 732c 2061 6e64 2064 656c 6574 6520  les, and delete 
-00001ad0: 6669 6c65 732e 2050 6c65 6173 6520 7265  files. Please re
-00001ae0: 6665 7220 746f 206f 7572 2066 696e 652d  fer to our fine-
-00001af0: 7475 6e69 6e67 2064 6f63 7320 5b68 6572  tuning docs [her
-00001b00: 655d 2868 7474 7073 3a2f 2f64 6f63 732e  e](https://docs.
-00001b10: 746f 6765 7468 6572 2e61 692f 646f 6373  together.ai/docs
-00001b20: 2f66 696e 652d 7475 6e69 6e67 2d70 7974  /fine-tuning-pyt
-00001b30: 686f 6e29 2e0a 0a60 6060 7079 7468 6f6e  hon)...```python
-00001b40: 0a69 6d70 6f72 7420 6f73 0a66 726f 6d20  .import os.from 
-00001b50: 746f 6765 7468 6572 2069 6d70 6f72 7420  together import 
-00001b60: 546f 6765 7468 6572 0a0a 636c 6965 6e74  Together..client
-00001b70: 203d 2054 6f67 6574 6865 7228 6170 695f   = Together(api_
-00001b80: 6b65 793d 6f73 2e65 6e76 6972 6f6e 2e67  key=os.environ.g
-00001b90: 6574 2822 544f 4745 5448 4552 5f41 5049  et("TOGETHER_API
-00001ba0: 5f4b 4559 2229 290a 0a63 6c69 656e 742e  _KEY"))..client.
-00001bb0: 6669 6c65 732e 7570 6c6f 6164 2866 696c  files.upload(fil
-00001bc0: 653d 2273 6f6d 6564 6174 612e 6a73 6f6e  e="somedata.json
-00001bd0: 6c22 2920 2320 7570 6c6f 6164 7320 6120  l") # uploads a 
-00001be0: 6669 6c65 0a63 6c69 656e 742e 6669 6c65  file.client.file
-00001bf0: 732e 6c69 7374 2829 2023 206c 6973 7473  s.list() # lists
-00001c00: 2061 6c6c 2075 706c 6f61 6465 6420 6669   all uploaded fi
-00001c10: 6c65 730a 636c 6965 6e74 2e66 696c 6573  les.client.files
-00001c20: 2e72 6574 7269 6576 6528 6964 3d22 6669  .retrieve(id="fi
-00001c30: 6c65 2d64 3064 3331 3863 622d 6237 6439  le-d0d318cb-b7d9
-00001c40: 2d34 3933 612d 6264 3730 2d31 6366 6530  -493a-bd70-1cfe0
-00001c50: 3839 6433 3831 3522 2920 2320 7265 7472  89d3815") # retr
-00001c60: 6965 7665 7320 6120 7370 6563 6966 6963  ieves a specific
-00001c70: 2066 696c 650a 636c 6965 6e74 2e66 696c   file.client.fil
-00001c80: 6573 2e72 6574 7269 6576 655f 636f 6e74  es.retrieve_cont
-00001c90: 656e 7428 6964 3d22 6669 6c65 2d64 3064  ent(id="file-d0d
-00001ca0: 3331 3863 622d 6237 6439 2d34 3933 612d  318cb-b7d9-493a-
-00001cb0: 6264 3730 2d31 6366 6530 3839 6433 3831  bd70-1cfe089d381
-00001cc0: 3522 2920 2320 7265 7472 6965 7665 7320  5") # retrieves 
-00001cd0: 636f 6e74 656e 7420 6f66 2061 2073 7065  content of a spe
-00001ce0: 6369 6669 6320 6669 6c65 0a63 6c69 656e  cific file.clien
-00001cf0: 742e 6669 6c65 732e 6465 6c65 7465 2869  t.files.delete(i
-00001d00: 643d 2266 696c 652d 6430 6433 3138 6362  d="file-d0d318cb
-00001d10: 2d62 3764 392d 3439 3361 2d62 6437 302d  -b7d9-493a-bd70-
-00001d20: 3163 6665 3038 3964 3338 3135 2229 2023  1cfe089d3815") #
-00001d30: 2064 656c 6574 6573 2061 2066 696c 650a   deletes a file.
-00001d40: 6060 600a 0a23 2320 4669 6e65 2d74 756e  ```..## Fine-tun
-00001d50: 6573 0a0a 5468 6520 6669 6e65 7475 6e65  es..The finetune
-00001d60: 2041 5049 2069 7320 7573 6564 2066 6f72   API is used for
-00001d70: 2066 696e 652d 7475 6e69 6e67 2061 6e64   fine-tuning and
-00001d80: 2061 6c6c 6f77 7320 6465 7665 6c6f 7065   allows develope
-00001d90: 7273 2074 6f20 6372 6561 7465 2066 696e  rs to create fin
-00001da0: 6574 756e 696e 6720 6a6f 6273 2e20 4974  etuning jobs. It
-00001db0: 2061 6c73 6f20 6861 7320 7365 7665 7261   also has severa
-00001dc0: 6c20 6d65 7468 6f64 7320 746f 206c 6973  l methods to lis
-00001dd0: 7420 616c 6c20 6a6f 6273 2c20 7265 7472  t all jobs, retr
-00001de0: 6976 6520 7374 6174 7573 6573 2061 6e64  ive statuses and
-00001df0: 2067 6574 2063 6865 636b 706f 696e 7473   get checkpoints
-00001e00: 2e20 506c 6561 7365 2072 6566 6572 2074  . Please refer t
-00001e10: 6f20 6f75 7220 6669 6e65 2d74 756e 696e  o our fine-tunin
-00001e20: 6720 646f 6373 205b 6865 7265 5d28 6874  g docs [here](ht
-00001e30: 7470 733a 2f2f 646f 6373 2e74 6f67 6574  tps://docs.toget
-00001e40: 6865 722e 6169 2f64 6f63 732f 6669 6e65  her.ai/docs/fine
-00001e50: 2d74 756e 696e 672d 7079 7468 6f6e 292e  -tuning-python).
-00001e60: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
-00001e70: 7274 206f 730a 6672 6f6d 2074 6f67 6574  rt os.from toget
-00001e80: 6865 7220 696d 706f 7274 2054 6f67 6574  her import Toget
-00001e90: 6865 720a 0a63 6c69 656e 7420 3d20 546f  her..client = To
-00001ea0: 6765 7468 6572 2861 7069 5f6b 6579 3d6f  gether(api_key=o
-00001eb0: 732e 656e 7669 726f 6e2e 6765 7428 2254  s.environ.get("T
-00001ec0: 4f47 4554 4845 525f 4150 495f 4b45 5922  OGETHER_API_KEY"
-00001ed0: 2929 0a0a 636c 6965 6e74 2e66 696e 655f  ))..client.fine_
-00001ee0: 7475 6e69 6e67 2e63 7265 6174 6528 0a20  tuning.create(. 
-00001ef0: 2074 7261 696e 696e 675f 6669 6c65 203d   training_file =
-00001f00: 2027 6669 6c65 2d64 3064 3331 3863 622d   'file-d0d318cb-
-00001f10: 6237 6439 2d34 3933 612d 6264 3730 2d31  b7d9-493a-bd70-1
-00001f20: 6366 6530 3839 6433 3831 3527 2c0a 2020  cfe089d3815',.  
-00001f30: 6d6f 6465 6c20 3d20 276d 6973 7472 616c  model = 'mistral
-00001f40: 6169 2f4d 6978 7472 616c 2d38 7837 422d  ai/Mixtral-8x7B-
-00001f50: 496e 7374 7275 6374 2d76 302e 3127 2c0a  Instruct-v0.1',.
-00001f60: 2020 6e5f 6570 6f63 6873 203d 2033 2c0a    n_epochs = 3,.
-00001f70: 2020 6e5f 6368 6563 6b70 6f69 6e74 7320    n_checkpoints 
-00001f80: 3d20 312c 0a20 2062 6174 6368 5f73 697a  = 1,.  batch_siz
-00001f90: 6520 3d20 342c 0a20 206c 6561 726e 696e  e = 4,.  learnin
-00001fa0: 675f 7261 7465 203d 2031 652d 352c 0a20  g_rate = 1e-5,. 
-00001fb0: 2073 7566 6669 7820 3d20 276d 792d 6465   suffix = 'my-de
-00001fc0: 6d6f 2d66 696e 6574 756e 6527 2c0a 2020  mo-finetune',.  
-00001fd0: 7761 6e64 625f 6170 695f 6b65 7920 3d20  wandb_api_key = 
-00001fe0: 2731 6132 6233 6334 6435 652e 2e2e 2e2e  '1a2b3c4d5e.....
-00001ff0: 2e2e 272c 0a29 0a63 6c69 656e 742e 6669  ..',.).client.fi
-00002000: 6e65 5f74 756e 696e 672e 6c69 7374 2829  ne_tuning.list()
-00002010: 2023 206c 6973 7473 2061 6c6c 2066 696e   # lists all fin
-00002020: 652d 7475 6e65 6420 6a6f 6273 0a63 6c69  e-tuned jobs.cli
-00002030: 656e 742e 6669 6e65 5f74 756e 696e 672e  ent.fine_tuning.
-00002040: 7265 7472 6965 7665 2869 643d 2266 742d  retrieve(id="ft-
-00002050: 6336 3661 3563 3138 2d31 6436 642d 3433  c66a5c18-1d6d-43
-00002060: 6339 2d39 3462 642d 3332 6437 3536 3432  c9-94bd-32d75642
-00002070: 3562 3462 2229 2023 2072 6574 7269 6576  5b4b") # retriev
-00002080: 6573 2069 6e66 6f72 6d61 7469 6f6e 206f  es information o
-00002090: 6e20 6669 6e65 7475 6e65 2065 7665 6e74  n finetune event
-000020a0: 0a63 6c69 656e 742e 6669 6e65 5f74 756e  .client.fine_tun
-000020b0: 696e 672e 6361 6e63 656c 2869 643d 2266  ing.cancel(id="f
-000020c0: 742d 6336 3661 3563 3138 2d31 6436 642d  t-c66a5c18-1d6d-
-000020d0: 3433 6339 2d39 3462 642d 3332 6437 3536  43c9-94bd-32d756
-000020e0: 3432 3562 3462 2229 2023 2043 616e 6365  425b4b") # Cance
-000020f0: 6c73 2061 2066 696e 652d 7475 6e69 6e67  ls a fine-tuning
-00002100: 206a 6f62 0a63 6c69 656e 742e 6669 6e65   job.client.fine
-00002110: 5f74 756e 696e 672e 6c69 7374 5f65 7665  _tuning.list_eve
-00002120: 6e74 7328 6964 3d22 6674 2d63 3636 6135  nts(id="ft-c66a5
-00002130: 6331 382d 3164 3664 2d34 3363 392d 3934  c18-1d6d-43c9-94
-00002140: 6264 2d33 3264 3735 3634 3235 6234 6222  bd-32d756425b4b"
-00002150: 2920 2320 204c 6973 7473 2065 7665 6e74  ) #  Lists event
-00002160: 7320 6f66 2061 2066 696e 652d 7475 6e65  s of a fine-tune
-00002170: 206a 6f62 0a63 6c69 656e 742e 6669 6e65   job.client.fine
-00002180: 5f74 756e 696e 672e 646f 776e 6c6f 6164  _tuning.download
-00002190: 2869 643d 2266 742d 6336 3661 3563 3138  (id="ft-c66a5c18
-000021a0: 2d31 6436 642d 3433 6339 2d39 3462 642d  -1d6d-43c9-94bd-
-000021b0: 3332 6437 3536 3432 3562 3462 2229 2023  32d756425b4b") #
-000021c0: 2064 6f77 6e6c 6f61 6473 2063 6f6d 7072   downloads compr
-000021d0: 6573 7365 6420 6669 6e65 2d74 756e 6564  essed fine-tuned
-000021e0: 206d 6f64 656c 206f 7220 6368 6563 6b70   model or checkp
-000021f0: 6f69 6e74 2074 6f20 6c6f 6361 6c20 6469  oint to local di
-00002200: 736b 0a60 6060 0a0a 2323 204d 6f64 656c  sk.```..## Model
-00002210: 730a 0a54 6869 7320 6c69 7374 7320 616c  s..This lists al
-00002220: 6c20 7468 6520 6d6f 6465 6c73 2074 6861  l the models tha
-00002230: 7420 546f 6765 7468 6572 2073 7570 706f  t Together suppo
-00002240: 7274 732e 0a0a 6060 6070 7974 686f 6e0a  rts...```python.
-00002250: 696d 706f 7274 206f 730a 6672 6f6d 2074  import os.from t
-00002260: 6f67 6574 6865 7220 696d 706f 7274 2054  ogether import T
-00002270: 6f67 6574 6865 720a 0a63 6c69 656e 7420  ogether..client 
-00002280: 3d20 546f 6765 7468 6572 2861 7069 5f6b  = Together(api_k
-00002290: 6579 3d6f 732e 656e 7669 726f 6e2e 6765  ey=os.environ.ge
-000022a0: 7428 2254 4f47 4554 4845 525f 4150 495f  t("TOGETHER_API_
-000022b0: 4b45 5922 2929 0a0a 6d6f 6465 6c73 203d  KEY"))..models =
-000022c0: 2063 6c69 656e 742e 6d6f 6465 6c73 2e6c   client.models.l
-000022d0: 6973 7428 290a 0a66 6f72 206d 6f64 656c  ist()..for model
-000022e0: 2069 6e20 6d6f 6465 6c73 3a0a 2020 2020   in models:.    
-000022f0: 7072 696e 7428 6d6f 6465 6c29 0a60 6060  print(model).```
-00002300: 0a0a 2320 5573 6167 6520 e280 9320 434c  ..# Usage ... CL
-00002310: 490a 0a23 2320 4368 6174 2043 6f6d 706c  I..## Chat Compl
-00002320: 6574 696f 6e73 0a0a 6060 6062 6173 680a  etions..```bash.
-00002330: 746f 6765 7468 6572 2063 6861 742e 636f  together chat.co
-00002340: 6d70 6c65 7469 6f6e 7320 5c0a 2020 2d2d  mpletions \.  --
-00002350: 6d65 7373 6167 6520 2273 7973 7465 6d22  message "system"
-00002360: 2022 596f 7520 6172 6520 6120 6865 6c70   "You are a help
-00002370: 6675 6c20 6173 7369 7374 616e 7420 6e61  ful assistant na
-00002380: 6d65 6420 546f 6765 7468 6572 2220 5c0a  med Together" \.
-00002390: 2020 2d2d 6d65 7373 6167 6520 2275 7365    --message "use
-000023a0: 7222 2022 5768 6174 2069 7320 796f 7572  r" "What is your
-000023b0: 206e 616d 653f 2220 5c0a 2020 2d2d 6d6f   name?" \.  --mo
-000023c0: 6465 6c20 6d69 7374 7261 6c61 692f 4d69  del mistralai/Mi
-000023d0: 7874 7261 6c2d 3878 3742 2d49 6e73 7472  xtral-8x7B-Instr
-000023e0: 7563 742d 7630 2e31 0a60 6060 0a0a 5468  uct-v0.1.```..Th
-000023f0: 6520 4368 6174 2043 6f6d 706c 6574 696f  e Chat Completio
-00002400: 6e73 2043 4c49 2065 6e61 626c 6573 2073  ns CLI enables s
-00002410: 7472 6561 6d69 6e67 2074 6f6b 656e 7320  treaming tokens 
-00002420: 746f 2073 7464 6f75 7420 6279 2064 6566  to stdout by def
-00002430: 6175 6c74 2e20 546f 2064 6973 6162 6c65  ault. To disable
-00002440: 2073 7472 6561 6d69 6e67 2c20 7573 6520   streaming, use 
-00002450: 602d 2d6e 6f2d 7374 7265 616d 602e 0a0a  `--no-stream`...
-00002460: 2323 2043 6f6d 706c 6574 696f 6e73 0a0a  ## Completions..
-00002470: 6060 6062 6173 680a 746f 6765 7468 6572  ```bash.together
-00002480: 2063 6f6d 706c 6574 696f 6e73 205c 0a20   completions \. 
-00002490: 2022 4c61 7267 6520 6c61 6e67 7561 6765   "Large language
-000024a0: 206d 6f64 656c 7320 6172 6520 2220 5c0a   models are " \.
-000024b0: 2020 2d2d 6d6f 6465 6c20 6d69 7374 7261    --model mistra
-000024c0: 6c61 692f 4d69 7874 7261 6c2d 3878 3742  lai/Mixtral-8x7B
-000024d0: 2d76 302e 3120 5c0a 2020 2d2d 6d61 782d  -v0.1 \.  --max-
-000024e0: 746f 6b65 6e73 2035 3132 205c 0a20 202d  tokens 512 \.  -
-000024f0: 2d73 746f 7020 222e 220a 6060 600a 0a54  -stop ".".```..T
-00002500: 6865 2043 6f6d 706c 6574 696f 6e73 2043  he Completions C
-00002510: 4c49 2065 6e61 626c 6573 2073 7472 6561  LI enables strea
-00002520: 6d69 6e67 2074 6f6b 656e 7320 746f 2073  ming tokens to s
-00002530: 7464 6f75 7420 6279 2064 6566 6175 6c74  tdout by default
-00002540: 2e20 546f 2064 6973 6162 6c65 2073 7472  . To disable str
-00002550: 6561 6d69 6e67 2c20 7573 6520 602d 2d6e  eaming, use `--n
-00002560: 6f2d 7374 7265 616d 602e 0a0a 2323 2049  o-stream`...## I
-00002570: 6d61 6765 2047 656e 6572 6174 696f 6e73  mage Generations
-00002580: 0a0a 6060 6062 6173 680a 746f 6765 7468  ..```bash.togeth
-00002590: 6572 2069 6d61 6765 7320 6765 6e65 7261  er images genera
-000025a0: 7465 205c 0a20 2022 7370 6163 6520 726f  te \.  "space ro
-000025b0: 626f 7473 2220 5c0a 2020 2d2d 6d6f 6465  bots" \.  --mode
-000025c0: 6c20 7374 6162 696c 6974 7961 692f 7374  l stabilityai/st
-000025d0: 6162 6c65 2d64 6966 6675 7369 6f6e 2d78  able-diffusion-x
-000025e0: 6c2d 6261 7365 2d31 2e30 205c 0a20 202d  l-base-1.0 \.  -
-000025f0: 2d6e 2034 0a60 6060 0a0a 5468 6520 696d  -n 4.```..The im
-00002600: 6167 6520 6973 206f 7065 6e65 6420 696e  age is opened in
-00002610: 2074 6865 2064 6566 6175 6c74 2069 6d61   the default ima
-00002620: 6765 2076 6965 7765 7220 6279 2064 6566  ge viewer by def
-00002630: 6175 6c74 2e20 546f 2064 6973 6162 6c65  ault. To disable
-00002640: 2074 6869 732c 2075 7365 2060 2d2d 6e6f   this, use `--no
-00002650: 2d73 686f 7760 2e0a 0a23 2320 4669 6c65  -show`...## File
-00002660: 730a 0a60 6060 6261 7368 0a23 2048 656c  s..```bash.# Hel
-00002670: 700a 746f 6765 7468 6572 2066 696c 6573  p.together files
-00002680: 202d 2d68 656c 700a 0a23 2043 6865 636b   --help..# Check
-00002690: 2066 696c 650a 746f 6765 7468 6572 2066   file.together f
-000026a0: 696c 6573 2063 6865 636b 2065 7861 6d70  iles check examp
-000026b0: 6c65 2e6a 736f 6e6c 0a0a 2320 5570 6c6f  le.jsonl..# Uplo
-000026c0: 6164 2066 696c 650a 746f 6765 7468 6572  ad file.together
-000026d0: 2066 696c 6573 2075 706c 6f61 6420 6578   files upload ex
-000026e0: 616d 706c 652e 6a73 6f6e 6c0a 0a23 204c  ample.jsonl..# L
-000026f0: 6973 7420 6669 6c65 730a 746f 6765 7468  ist files.togeth
-00002700: 6572 2066 696c 6573 206c 6973 740a 0a23  er files list..#
-00002710: 2052 6574 7269 6576 6520 6669 6c65 206d   Retrieve file m
-00002720: 6574 6164 6174 610a 746f 6765 7468 6572  etadata.together
-00002730: 2066 696c 6573 2072 6574 7269 6576 6520   files retrieve 
-00002740: 6669 6c65 2d36 6635 3066 3964 312d 3562  file-6f50f9d1-5b
-00002750: 3935 2d34 3136 632d 3930 3430 2d30 3739  95-416c-9040-079
-00002760: 3962 3262 3462 3839 340a 0a23 2052 6574  9b2b4b894..# Ret
-00002770: 7269 6576 6520 6669 6c65 2063 6f6e 7465  rieve file conte
-00002780: 6e74 0a74 6f67 6574 6865 7220 6669 6c65  nt.together file
-00002790: 7320 7265 7472 6965 7665 2d63 6f6e 7465  s retrieve-conte
-000027a0: 6e74 2066 696c 652d 3666 3530 6639 6431  nt file-6f50f9d1
-000027b0: 2d35 6239 352d 3431 3663 2d39 3034 302d  -5b95-416c-9040-
-000027c0: 3037 3939 6232 6234 6238 3934 0a0a 2320  0799b2b4b894..# 
-000027d0: 4465 6c65 7465 2072 656d 6f74 6520 6669  Delete remote fi
-000027e0: 6c65 0a74 6f67 6574 6865 7220 6669 6c65  le.together file
-000027f0: 7320 6465 6c65 7465 2066 696c 652d 3666  s delete file-6f
-00002800: 3530 6639 6431 2d35 6239 352d 3431 3663  50f9d1-5b95-416c
-00002810: 2d39 3034 302d 3037 3939 6232 6234 6238  -9040-0799b2b4b8
-00002820: 3934 0a60 6060 0a0a 2323 2046 696e 652d  94.```..## Fine-
-00002830: 7475 6e69 6e67 0a0a 6060 6062 6173 680a  tuning..```bash.
-00002840: 2320 4865 6c70 0a74 6f67 6574 6865 7220  # Help.together 
-00002850: 6669 6e65 2d74 756e 696e 6720 2d2d 6865  fine-tuning --he
-00002860: 6c70 0a0a 2320 4372 6561 7465 2066 696e  lp..# Create fin
-00002870: 652d 7475 6e65 206a 6f62 0a74 6f67 6574  e-tune job.toget
-00002880: 6865 7220 6669 6e65 2d74 756e 696e 6720  her fine-tuning 
-00002890: 6372 6561 7465 205c 0a20 202d 2d6d 6f64  create \.  --mod
-000028a0: 656c 2074 6f67 6574 6865 7263 6f6d 7075  el togethercompu
-000028b0: 7465 722f 6c6c 616d 612d 322d 3762 2d63  ter/llama-2-7b-c
-000028c0: 6861 7420 5c0a 2020 2d2d 7472 6169 6e69  hat \.  --traini
-000028d0: 6e67 2d66 696c 6520 6669 6c65 2d37 3131  ng-file file-711
-000028e0: 6438 3732 342d 6233 6533 2d34 6165 322d  d8724-b3e3-4ae2-
-000028f0: 6235 3136 2d39 3438 3431 3935 3831 3137  b516-94841958117
-00002900: 640a 0a23 204c 6973 7420 6669 6e65 2d74  d..# List fine-t
-00002910: 756e 6520 6a6f 6273 0a74 6f67 6574 6865  une jobs.togethe
-00002920: 7220 6669 6e65 2d74 756e 696e 6720 6c69  r fine-tuning li
-00002930: 7374 0a0a 2320 5265 7472 6965 7665 2066  st..# Retrieve f
-00002940: 696e 652d 7475 6e65 206a 6f62 2064 6574  ine-tune job det
-00002950: 6169 6c73 0a74 6f67 6574 6865 7220 6669  ails.together fi
-00002960: 6e65 2d74 756e 696e 6720 7265 7472 6965  ne-tuning retrie
-00002970: 7665 2066 742d 6336 3661 3563 3138 2d31  ve ft-c66a5c18-1
-00002980: 6436 642d 3433 6339 2d39 3462 642d 3332  d6d-43c9-94bd-32
-00002990: 6437 3536 3432 3562 3462 0a0a 2320 4c69  d756425b4b..# Li
-000029a0: 7374 2066 696e 652d 7475 6e65 206a 6f62  st fine-tune job
-000029b0: 2065 7665 6e74 730a 746f 6765 7468 6572   events.together
-000029c0: 2066 696e 652d 7475 6e69 6e67 206c 6973   fine-tuning lis
-000029d0: 742d 6576 656e 7473 2066 742d 6336 3661  t-events ft-c66a
-000029e0: 3563 3138 2d31 6436 642d 3433 6339 2d39  5c18-1d6d-43c9-9
-000029f0: 3462 642d 3332 6437 3536 3432 3562 3462  4bd-32d756425b4b
-00002a00: 0a0a 2320 4361 6e63 656c 2072 756e 6e69  ..# Cancel runni
-00002a10: 6e67 206a 6f62 0a74 6f67 6574 6865 7220  ng job.together 
-00002a20: 6669 6e65 2d74 756e 696e 6720 6361 6e63  fine-tuning canc
-00002a30: 656c 2066 742d 6336 3661 3563 3138 2d31  el ft-c66a5c18-1
-00002a40: 6436 642d 3433 6339 2d39 3462 642d 3332  d6d-43c9-94bd-32
-00002a50: 6437 3536 3432 3562 3462 0a0a 2320 446f  d756425b4b..# Do
-00002a60: 776e 6c6f 6164 2066 696e 652d 7475 6e65  wnload fine-tune
-00002a70: 6420 6d6f 6465 6c20 7765 6967 6874 730a  d model weights.
-00002a80: 746f 6765 7468 6572 2066 696e 652d 7475  together fine-tu
-00002a90: 6e69 6e67 2064 6f77 6e6c 6f61 6420 6674  ning download ft
-00002aa0: 2d63 3636 6135 6331 382d 3164 3664 2d34  -c66a5c18-1d6d-4
-00002ab0: 3363 392d 3934 6264 2d33 3264 3735 3634  3c9-94bd-32d7564
-00002ac0: 3235 6234 620a 6060 600a 0a23 2320 4d6f  25b4b.```..## Mo
-00002ad0: 6465 6c73 0a0a 6060 6062 6173 680a 2320  dels..```bash.# 
-00002ae0: 4865 6c70 0a74 6f67 6574 6865 7220 6d6f  Help.together mo
-00002af0: 6465 6c73 202d 2d68 656c 700a 0a23 204c  dels --help..# L
-00002b00: 6973 7420 6d6f 6465 6c73 0a74 6f67 6574  ist models.toget
-00002b10: 6865 7220 6d6f 6465 6c73 206c 6973 740a  her models list.
-00002b20: 6060 600a 0a23 2320 436f 6e74 7269 6275  ```..## Contribu
-00002b30: 7469 6e67 0a0a 5265 6665 7220 746f 2074  ting..Refer to t
-00002b40: 6865 205b 436f 6e74 7269 6275 7469 6e67  he [Contributing
-00002b50: 2047 7569 6465 5d28 434f 4e54 5249 4255   Guide](CONTRIBU
-00002b60: 5449 4e47 2e6d 6429 0a0a                 TING.md)..
+000005a0: 646f 776e 0a0a 3c64 6976 2061 6c69 676e  down..<div align
+000005b0: 3d22 6365 6e74 6572 223e 0a20 203c 6120  ="center">.  <a 
+000005c0: 6872 6566 3d22 6874 7470 733a 2f2f 7777  href="https://ww
+000005d0: 772e 746f 6765 7468 6572 2e61 692f 223e  w.together.ai/">
+000005e0: 0a20 2020 203c 696d 6720 616c 743d 2274  .    <img alt="t
+000005f0: 6f67 6574 6865 722e 6169 2220 6865 6967  ogether.ai" heig
+00000600: 6874 3d22 3130 3070 7822 2073 7263 3d22  ht="100px" src="
+00000610: 6874 7470 733a 2f2f 6173 7365 7473 2d67  https://assets-g
+00000620: 6c6f 6261 6c2e 7765 6273 6974 652d 6669  lobal.website-fi
+00000630: 6c65 732e 636f 6d2f 3634 6636 6632 6330  les.com/64f6f2c0
+00000640: 6533 6634 6335 6139 3163 3165 3832 3361  e3f4c5a91c1e823a
+00000650: 2f36 3534 3639 3364 3536 3934 3934 3931  /654693d56949491
+00000660: 3263 6663 3063 3064 345f 6661 7669 636f  2cfc0c0d4_favico
+00000670: 6e2e 7376 6722 3e0a 2020 3c2f 613e 0a3c  n.svg">.  </a>.<
+00000680: 2f64 6976 3e0a 0a23 2054 6f67 6574 6865  /div>..# Togethe
+00000690: 7220 5079 7468 6f6e 2041 5049 206c 6962  r Python API lib
+000006a0: 7261 7279 0a0a 5b21 5b50 7950 4920 7665  rary..[![PyPI ve
+000006b0: 7273 696f 6e5d 2868 7474 7073 3a2f 2f69  rsion](https://i
+000006c0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+000006d0: 7069 2f76 2f74 6f67 6574 6865 722e 7376  pi/v/together.sv
+000006e0: 6729 5d28 6874 7470 733a 2f2f 7079 7069  g)](https://pypi
+000006f0: 2e6f 7267 2f70 726f 6a65 6374 2f74 6f67  .org/project/tog
+00000700: 6574 6865 722f 290a 5b21 5b44 6973 636f  ether/).[![Disco
+00000710: 7264 5d28 6874 7470 733a 2f2f 6463 6261  rd](https://dcba
+00000720: 6467 652e 7665 7263 656c 2e61 7070 2f61  dge.vercel.app/a
+00000730: 7069 2f73 6572 7665 722f 3952 6b36 7353  pi/server/9Rk6sS
+00000740: 6557 4547 3f73 7479 6c65 3d66 6c61 7426  eWEG?style=flat&
+00000750: 636f 6d70 6163 743d 7472 7565 295d 2868  compact=true)](h
+00000760: 7474 7073 3a2f 2f64 6973 636f 7264 2e63  ttps://discord.c
+00000770: 6f6d 2f69 6e76 6974 652f 3952 6b36 7353  om/invite/9Rk6sS
+00000780: 6557 4547 290a 5b21 5b54 7769 7474 6572  eWEG).[![Twitter
+00000790: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+000007a0: 6965 6c64 732e 696f 2f74 7769 7474 6572  ields.io/twitter
+000007b0: 2f75 726c 2f68 7474 7073 2f74 7769 7474  /url/https/twitt
+000007c0: 6572 2e63 6f6d 2f74 6f67 6574 6865 7263  er.com/togetherc
+000007d0: 6f6d 7075 7465 2e73 7667 3f73 7479 6c65  ompute.svg?style
+000007e0: 3d73 6f63 6961 6c26 6c61 6265 6c3d 466f  =social&label=Fo
+000007f0: 6c6c 6f77 2532 3025 3430 746f 6765 7468  llow%20%40togeth
+00000800: 6572 636f 6d70 7574 6529 5d28 6874 7470  ercompute)](http
+00000810: 733a 2f2f 7477 6974 7465 722e 636f 6d2f  s://twitter.com/
+00000820: 746f 6765 7468 6572 636f 6d70 7574 6529  togethercompute)
+00000830: 0a0a 5468 6520 5b54 6f67 6574 6865 7220  ..The [Together 
+00000840: 5079 7468 6f6e 2041 5049 204c 6962 7261  Python API Libra
+00000850: 7279 5d28 6874 7470 733a 2f2f 7079 7069  ry](https://pypi
+00000860: 2e6f 7267 2f70 726f 6a65 6374 2f74 6f67  .org/project/tog
+00000870: 6574 6865 722f 2920 6973 2074 6865 206f  ether/) is the o
+00000880: 6666 6963 6961 6c20 5079 7468 6f6e 2063  fficial Python c
+00000890: 6c69 656e 7420 666f 7220 546f 6765 7468  lient for Togeth
+000008a0: 6572 2773 2041 5049 2070 6c61 7466 6f72  er's API platfor
+000008b0: 6d2c 2070 726f 7669 6469 6e67 2061 2063  m, providing a c
+000008c0: 6f6e 7665 6e69 656e 7420 7761 7920 666f  onvenient way fo
+000008d0: 7220 696e 7465 7261 6374 696e 6720 7769  r interacting wi
+000008e0: 7468 2074 6865 2052 4553 5420 4150 4973  th the REST APIs
+000008f0: 2061 6e64 2065 6e61 626c 6573 2065 6173   and enables eas
+00000900: 7920 696e 7465 6772 6174 696f 6e73 2077  y integrations w
+00000910: 6974 6820 5079 7468 6f6e 2033 2e38 2b20  ith Python 3.8+ 
+00000920: 6170 706c 6963 6174 696f 6e73 2077 6974  applications wit
+00000930: 6820 6561 7379 2074 6f20 7573 6520 7379  h easy to use sy
+00000940: 6e63 6872 6f6e 6f75 7320 616e 6420 6173  nchronous and as
+00000950: 796e 6368 726f 6e6f 7573 2063 6c69 656e  ynchronous clien
+00000960: 7473 2e0a 0a0a 0a23 2320 496e 7374 616c  ts.....## Instal
+00000970: 6c61 7469 6f6e 0a0a 3e20 f09f 9aa7 0a3e  lation..> .....>
+00000980: 2054 6865 204c 6962 7261 7279 2077 6173   The Library was
+00000990: 2072 6577 7269 7474 656e 2069 6e20 7631   rewritten in v1
+000009a0: 2e30 2e30 2072 656c 6561 7365 6420 696e  .0.0 released in
+000009b0: 2041 7072 696c 206f 6620 3230 3234 2e20   April of 2024. 
+000009c0: 5468 6572 6520 7765 7265 2073 6967 6e69  There were signi
+000009d0: 6669 6361 6e74 2063 6861 6e67 6573 206d  ficant changes m
+000009e0: 6164 652e 0a0a 546f 2069 6e73 7461 6c6c  ade...To install
+000009f0: 2054 6f67 6574 6865 7220 5079 7468 6f6e   Together Python
+00000a00: 204c 6962 7261 7279 2066 726f 6d20 5079   Library from Py
+00000a10: 5049 2c20 7369 6d70 6c79 2072 756e 3a0a  PI, simply run:.
+00000a20: 0a60 6060 7368 656c 6c20 5368 656c 6c0a  .```shell Shell.
+00000a30: 7069 7020 696e 7374 616c 6c20 2d2d 7570  pip install --up
+00000a40: 6772 6164 6520 746f 6765 7468 6572 0a60  grade together.`
+00000a50: 6060 0a0a 2323 2320 5365 7474 696e 6720  ``..### Setting 
+00000a60: 7570 2041 5049 204b 6579 0a0a 3e20 f09f  up API Key..> ..
+00000a70: 9aa7 2059 6f75 2077 696c 6c20 6e65 6564  .. You will need
+00000a80: 2074 6f20 6372 6561 7465 2061 6e20 6163   to create an ac
+00000a90: 636f 756e 7420 7769 7468 205b 546f 6765  count with [Toge
+00000aa0: 7468 6572 2e61 695d 2868 7474 7073 3a2f  ther.ai](https:/
+00000ab0: 2f61 7069 2e74 6f67 6574 6865 722e 7879  /api.together.xy
+00000ac0: 7a2f 2920 746f 206f 6274 6169 6e20 6120  z/) to obtain a 
+00000ad0: 546f 6765 7468 6572 2041 5049 204b 6579  Together API Key
+00000ae0: 2e0a 0a4f 6e63 6520 6c6f 6767 6564 2069  ...Once logged i
+00000af0: 6e20 746f 2074 6865 2054 6f67 6574 6865  n to the Togethe
+00000b00: 7220 506c 6179 6772 6f75 6e64 2c20 796f  r Playground, yo
+00000b10: 7520 6361 6e20 6669 6e64 2061 7661 696c  u can find avail
+00000b20: 6162 6c65 2041 5049 206b 6579 7320 696e  able API keys in
+00000b30: 205b 7468 6973 2073 6574 7469 6e67 7320   [this settings 
+00000b40: 7061 6765 5d28 6874 7470 733a 2f2f 6170  page](https://ap
+00000b50: 692e 746f 6765 7468 6572 2e78 797a 2f73  i.together.xyz/s
+00000b60: 6574 7469 6e67 732f 6170 692d 6b65 7973  ettings/api-keys
+00000b70: 292e 0a0a 2323 2323 2053 6574 7469 6e67  )...#### Setting
+00000b80: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
+00000b90: 6961 626c 650a 0a60 6060 7368 656c 6c0a  iable..```shell.
+00000ba0: 6578 706f 7274 2054 4f47 4554 4845 525f  export TOGETHER_
+00000bb0: 4150 495f 4b45 593d 7878 7878 780a 6060  API_KEY=xxxxx.``
+00000bc0: 600a 0a23 2323 2320 5573 696e 6720 7468  `..#### Using th
+00000bd0: 6520 636c 6965 6e74 0a0a 6060 6070 7974  e client..```pyt
+00000be0: 686f 6e0a 6672 6f6d 2074 6f67 6574 6865  hon.from togethe
+00000bf0: 7220 696d 706f 7274 2054 6f67 6574 6865  r import Togethe
+00000c00: 720a 0a63 6c69 656e 7420 3d20 546f 6765  r..client = Toge
+00000c10: 7468 6572 2861 7069 5f6b 6579 3d22 7878  ther(api_key="xx
+00000c20: 7878 7822 290a 6060 600a 0a54 6869 7320  xxx").```..This 
+00000c30: 7265 706f 2063 6f6e 7461 696e 7320 626f  repo contains bo
+00000c40: 7468 2061 2050 7974 686f 6e20 4c69 6272  th a Python Libr
+00000c50: 6172 7920 616e 6420 6120 434c 492e 2057  ary and a CLI. W
+00000c60: 6527 6c6c 2064 656d 6f6e 7374 7261 7465  e'll demonstrate
+00000c70: 2068 6f77 2074 6f20 7573 6520 626f 7468   how to use both
+00000c80: 2062 656c 6f77 2e0a 0a23 2320 5573 6167   below...## Usag
+00000c90: 6520 e280 9320 5079 7468 6f6e 2043 6c69  e ... Python Cli
+00000ca0: 656e 740a 0a23 2323 2043 6861 7420 436f  ent..### Chat Co
+00000cb0: 6d70 6c65 7469 6f6e 730a 0a60 6060 7079  mpletions..```py
+00000cc0: 7468 6f6e 0a69 6d70 6f72 7420 6f73 0a66  thon.import os.f
+00000cd0: 726f 6d20 746f 6765 7468 6572 2069 6d70  rom together imp
+00000ce0: 6f72 7420 546f 6765 7468 6572 0a0a 636c  ort Together..cl
+00000cf0: 6965 6e74 203d 2054 6f67 6574 6865 7228  ient = Together(
+00000d00: 6170 695f 6b65 793d 6f73 2e65 6e76 6972  api_key=os.envir
+00000d10: 6f6e 2e67 6574 2822 544f 4745 5448 4552  on.get("TOGETHER
+00000d20: 5f41 5049 5f4b 4559 2229 290a 0a72 6573  _API_KEY"))..res
+00000d30: 706f 6e73 6520 3d20 636c 6965 6e74 2e63  ponse = client.c
+00000d40: 6861 742e 636f 6d70 6c65 7469 6f6e 732e  hat.completions.
+00000d50: 6372 6561 7465 280a 2020 2020 6d6f 6465  create(.    mode
+00000d60: 6c3d 226d 6973 7472 616c 6169 2f4d 6978  l="mistralai/Mix
+00000d70: 7472 616c 2d38 7837 422d 496e 7374 7275  tral-8x7B-Instru
+00000d80: 6374 2d76 302e 3122 2c0a 2020 2020 6d65  ct-v0.1",.    me
+00000d90: 7373 6167 6573 3d5b 7b22 726f 6c65 223a  ssages=[{"role":
+00000da0: 2022 7573 6572 222c 2022 636f 6e74 656e   "user", "conten
+00000db0: 7422 3a20 2274 656c 6c20 6d65 2061 626f  t": "tell me abo
+00000dc0: 7574 206e 6577 2079 6f72 6b22 7d5d 2c0a  ut new york"}],.
+00000dd0: 290a 7072 696e 7428 7265 7370 6f6e 7365  ).print(response
+00000de0: 2e63 686f 6963 6573 5b30 5d2e 6d65 7373  .choices[0].mess
+00000df0: 6167 652e 636f 6e74 656e 7429 0a60 6060  age.content).```
+00000e00: 0a0a 2323 2323 2053 7472 6561 6d69 6e67  ..#### Streaming
+00000e10: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
+00000e20: 7274 206f 730a 6672 6f6d 2074 6f67 6574  rt os.from toget
+00000e30: 6865 7220 696d 706f 7274 2054 6f67 6574  her import Toget
+00000e40: 6865 720a 0a63 6c69 656e 7420 3d20 546f  her..client = To
+00000e50: 6765 7468 6572 2861 7069 5f6b 6579 3d6f  gether(api_key=o
+00000e60: 732e 656e 7669 726f 6e2e 6765 7428 2254  s.environ.get("T
+00000e70: 4f47 4554 4845 525f 4150 495f 4b45 5922  OGETHER_API_KEY"
+00000e80: 2929 0a73 7472 6561 6d20 3d20 636c 6965  )).stream = clie
+00000e90: 6e74 2e63 6861 742e 636f 6d70 6c65 7469  nt.chat.completi
+00000ea0: 6f6e 732e 6372 6561 7465 280a 2020 2020  ons.create(.    
+00000eb0: 6d6f 6465 6c3d 226d 6973 7472 616c 6169  model="mistralai
+00000ec0: 2f4d 6978 7472 616c 2d38 7837 422d 496e  /Mixtral-8x7B-In
+00000ed0: 7374 7275 6374 2d76 302e 3122 2c0a 2020  struct-v0.1",.  
+00000ee0: 2020 6d65 7373 6167 6573 3d5b 7b22 726f    messages=[{"ro
+00000ef0: 6c65 223a 2022 7573 6572 222c 2022 636f  le": "user", "co
+00000f00: 6e74 656e 7422 3a20 2274 656c 6c20 6d65  ntent": "tell me
+00000f10: 2061 626f 7574 206e 6577 2079 6f72 6b22   about new york"
+00000f20: 7d5d 2c0a 2020 2020 7374 7265 616d 3d54  }],.    stream=T
+00000f30: 7275 652c 0a29 0a0a 666f 7220 6368 756e  rue,.)..for chun
+00000f40: 6b20 696e 2073 7472 6561 6d3a 0a20 2020  k in stream:.   
+00000f50: 2070 7269 6e74 2863 6875 6e6b 2e63 686f   print(chunk.cho
+00000f60: 6963 6573 5b30 5d2e 6465 6c74 612e 636f  ices[0].delta.co
+00000f70: 6e74 656e 7420 6f72 2022 222c 2065 6e64  ntent or "", end
+00000f80: 3d22 222c 2066 6c75 7368 3d54 7275 6529  ="", flush=True)
+00000f90: 0a60 6060 0a0a 2323 2323 2041 7379 6e63  .```..#### Async
+00000fa0: 2075 7361 6765 0a0a 6060 6070 7974 686f   usage..```pytho
+00000fb0: 6e0a 696d 706f 7274 206f 732c 2061 7379  n.import os, asy
+00000fc0: 6e63 696f 0a66 726f 6d20 746f 6765 7468  ncio.from togeth
+00000fd0: 6572 2069 6d70 6f72 7420 4173 796e 6354  er import AsyncT
+00000fe0: 6f67 6574 6865 720a 0a61 7379 6e63 5f63  ogether..async_c
+00000ff0: 6c69 656e 7420 3d20 4173 796e 6354 6f67  lient = AsyncTog
+00001000: 6574 6865 7228 6170 695f 6b65 793d 6f73  ether(api_key=os
+00001010: 2e65 6e76 6972 6f6e 2e67 6574 2822 544f  .environ.get("TO
+00001020: 4745 5448 4552 5f41 5049 5f4b 4559 2229  GETHER_API_KEY")
+00001030: 290a 6d65 7373 6167 6573 203d 205b 0a20  ).messages = [. 
+00001040: 2020 2022 5768 6174 2061 7265 2074 6865     "What are the
+00001050: 2074 6f70 2074 6869 6e67 7320 746f 2064   top things to d
+00001060: 6f20 696e 2053 616e 2046 7261 6e63 6973  o in San Francis
+00001070: 636f 3f22 2c0a 2020 2020 2257 6861 7420  co?",.    "What 
+00001080: 636f 756e 7472 7920 6973 2050 6172 6973  country is Paris
+00001090: 2069 6e3f 222c 0a5d 0a0a 6173 796e 6320   in?",.]..async 
+000010a0: 6465 6620 6173 796e 635f 6368 6174 5f63  def async_chat_c
+000010b0: 6f6d 706c 6574 696f 6e28 6d65 7373 6167  ompletion(messag
+000010c0: 6573 293a 0a20 2020 2061 7379 6e63 5f63  es):.    async_c
+000010d0: 6c69 656e 7420 3d20 4173 796e 6354 6f67  lient = AsyncTog
+000010e0: 6574 6865 7228 6170 695f 6b65 793d 6f73  ether(api_key=os
+000010f0: 2e65 6e76 6972 6f6e 2e67 6574 2822 544f  .environ.get("TO
+00001100: 4745 5448 4552 5f41 5049 5f4b 4559 2229  GETHER_API_KEY")
+00001110: 290a 2020 2020 7461 736b 7320 3d20 5b0a  ).    tasks = [.
+00001120: 2020 2020 2020 2020 6173 796e 635f 636c          async_cl
+00001130: 6965 6e74 2e63 6861 742e 636f 6d70 6c65  ient.chat.comple
+00001140: 7469 6f6e 732e 6372 6561 7465 280a 2020  tions.create(.  
+00001150: 2020 2020 2020 2020 2020 6d6f 6465 6c3d            model=
+00001160: 226d 6973 7472 616c 6169 2f4d 6978 7472  "mistralai/Mixtr
+00001170: 616c 2d38 7837 422d 496e 7374 7275 6374  al-8x7B-Instruct
+00001180: 2d76 302e 3122 2c0a 2020 2020 2020 2020  -v0.1",.        
+00001190: 2020 2020 6d65 7373 6167 6573 3d5b 7b22      messages=[{"
+000011a0: 726f 6c65 223a 2022 7573 6572 222c 2022  role": "user", "
+000011b0: 636f 6e74 656e 7422 3a20 6d65 7373 6167  content": messag
+000011c0: 657d 5d2c 0a20 2020 2020 2020 2029 0a20  e}],.        ). 
+000011d0: 2020 2020 2020 2066 6f72 206d 6573 7361         for messa
+000011e0: 6765 2069 6e20 6d65 7373 6167 6573 0a20  ge in messages. 
+000011f0: 2020 205d 0a20 2020 2072 6573 706f 6e73     ].    respons
+00001200: 6573 203d 2061 7761 6974 2061 7379 6e63  es = await async
+00001210: 696f 2e67 6174 6865 7228 2a74 6173 6b73  io.gather(*tasks
+00001220: 290a 0a20 2020 2066 6f72 2072 6573 706f  )..    for respo
+00001230: 6e73 6520 696e 2072 6573 706f 6e73 6573  nse in responses
+00001240: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
+00001250: 7265 7370 6f6e 7365 2e63 686f 6963 6573  response.choices
+00001260: 5b30 5d2e 6d65 7373 6167 652e 636f 6e74  [0].message.cont
+00001270: 656e 7429 0a0a 6173 796e 6369 6f2e 7275  ent)..asyncio.ru
+00001280: 6e28 6173 796e 635f 6368 6174 5f63 6f6d  n(async_chat_com
+00001290: 706c 6574 696f 6e28 6d65 7373 6167 6573  pletion(messages
+000012a0: 2929 0a60 6060 0a0a 2323 2320 436f 6d70  )).```..### Comp
+000012b0: 6c65 7469 6f6e 730a 0a43 6f6d 706c 6574  letions..Complet
+000012c0: 696f 6e73 2061 7265 2066 6f72 2063 6f64  ions are for cod
+000012d0: 6520 616e 6420 6c61 6e67 7561 6765 206d  e and language m
+000012e0: 6f64 656c 7320 7368 6f77 6e20 5b68 6572  odels shown [her
+000012f0: 655d 2868 7474 7073 3a2f 2f64 6f63 732e  e](https://docs.
+00001300: 746f 6765 7468 6572 2e61 692f 646f 6373  together.ai/docs
+00001310: 2f69 6e66 6572 656e 6365 2d6d 6f64 656c  /inference-model
+00001320: 7329 2e20 4265 6c6f 772c 2061 2063 6f64  s). Below, a cod
+00001330: 6520 6d6f 6465 6c20 6578 616d 706c 6520  e model example 
+00001340: 6973 2073 686f 776e 2e0a 0a60 6060 7079  is shown...```py
+00001350: 7468 6f6e 0a69 6d70 6f72 7420 6f73 0a66  thon.import os.f
+00001360: 726f 6d20 746f 6765 7468 6572 2069 6d70  rom together imp
+00001370: 6f72 7420 546f 6765 7468 6572 0a0a 636c  ort Together..cl
+00001380: 6965 6e74 203d 2054 6f67 6574 6865 7228  ient = Together(
+00001390: 6170 695f 6b65 793d 6f73 2e65 6e76 6972  api_key=os.envir
+000013a0: 6f6e 2e67 6574 2822 544f 4745 5448 4552  on.get("TOGETHER
+000013b0: 5f41 5049 5f4b 4559 2229 290a 0a72 6573  _API_KEY"))..res
+000013c0: 706f 6e73 6520 3d20 636c 6965 6e74 2e63  ponse = client.c
+000013d0: 6f6d 706c 6574 696f 6e73 2e63 7265 6174  ompletions.creat
+000013e0: 6528 0a20 2020 206d 6f64 656c 3d22 636f  e(.    model="co
+000013f0: 6465 6c6c 616d 612f 436f 6465 4c6c 616d  dellama/CodeLlam
+00001400: 612d 3334 622d 5079 7468 6f6e 2d68 6622  a-34b-Python-hf"
+00001410: 2c0a 2020 2020 7072 6f6d 7074 3d22 5772  ,.    prompt="Wr
+00001420: 6974 6520 6120 4e65 7874 2e6a 7320 636f  ite a Next.js co
+00001430: 6d70 6f6e 656e 7420 7769 7468 2054 6169  mponent with Tai
+00001440: 6c77 696e 6443 5353 2066 6f72 2061 2068  lwindCSS for a h
+00001450: 6561 6465 7220 636f 6d70 6f6e 656e 742e  eader component.
+00001460: 222c 0a20 2020 206d 6178 5f74 6f6b 656e  ",.    max_token
+00001470: 733d 3230 302c 0a29 0a70 7269 6e74 2872  s=200,.).print(r
+00001480: 6573 706f 6e73 652e 6368 6f69 6365 735b  esponse.choices[
+00001490: 305d 2e74 6578 7429 0a60 6060 0a0a 2323  0].text).```..##
+000014a0: 2323 2053 7472 6561 6d69 6e67 0a0a 6060  ## Streaming..``
+000014b0: 6070 7974 686f 6e0a 696d 706f 7274 206f  `python.import o
+000014c0: 730a 6672 6f6d 2074 6f67 6574 6865 7220  s.from together 
+000014d0: 696d 706f 7274 2054 6f67 6574 6865 720a  import Together.
+000014e0: 0a63 6c69 656e 7420 3d20 546f 6765 7468  .client = Togeth
+000014f0: 6572 2861 7069 5f6b 6579 3d6f 732e 656e  er(api_key=os.en
+00001500: 7669 726f 6e2e 6765 7428 2254 4f47 4554  viron.get("TOGET
+00001510: 4845 525f 4150 495f 4b45 5922 2929 0a73  HER_API_KEY")).s
+00001520: 7472 6561 6d20 3d20 636c 6965 6e74 2e63  tream = client.c
+00001530: 6f6d 706c 6574 696f 6e73 2e63 7265 6174  ompletions.creat
+00001540: 6528 0a20 2020 206d 6f64 656c 3d22 636f  e(.    model="co
+00001550: 6465 6c6c 616d 612f 436f 6465 4c6c 616d  dellama/CodeLlam
+00001560: 612d 3334 622d 5079 7468 6f6e 2d68 6622  a-34b-Python-hf"
+00001570: 2c0a 2020 2020 7072 6f6d 7074 3d22 5772  ,.    prompt="Wr
+00001580: 6974 6520 6120 4e65 7874 2e6a 7320 636f  ite a Next.js co
+00001590: 6d70 6f6e 656e 7420 7769 7468 2054 6169  mponent with Tai
+000015a0: 6c77 696e 6443 5353 2066 6f72 2061 2068  lwindCSS for a h
+000015b0: 6561 6465 7220 636f 6d70 6f6e 656e 742e  eader component.
+000015c0: 222c 0a20 2020 2073 7472 6561 6d3d 5472  ",.    stream=Tr
+000015d0: 7565 2c0a 290a 0a66 6f72 2063 6875 6e6b  ue,.)..for chunk
+000015e0: 2069 6e20 7374 7265 616d 3a0a 2020 2020   in stream:.    
+000015f0: 7072 696e 7428 6368 756e 6b2e 6368 6f69  print(chunk.choi
+00001600: 6365 735b 305d 2e64 656c 7461 2e63 6f6e  ces[0].delta.con
+00001610: 7465 6e74 206f 7220 2222 2c20 656e 643d  tent or "", end=
+00001620: 2222 2c20 666c 7573 683d 5472 7565 290a  "", flush=True).
+00001630: 6060 600a 0a23 2323 2320 4173 796e 6320  ```..#### Async 
+00001640: 7573 6167 650a 0a60 6060 7079 7468 6f6e  usage..```python
+00001650: 0a69 6d70 6f72 7420 6f73 2c20 6173 796e  .import os, asyn
+00001660: 6369 6f0a 6672 6f6d 2074 6f67 6574 6865  cio.from togethe
+00001670: 7220 696d 706f 7274 2041 7379 6e63 546f  r import AsyncTo
+00001680: 6765 7468 6572 0a0a 6173 796e 635f 636c  gether..async_cl
+00001690: 6965 6e74 203d 2041 7379 6e63 546f 6765  ient = AsyncToge
+000016a0: 7468 6572 2861 7069 5f6b 6579 3d6f 732e  ther(api_key=os.
+000016b0: 656e 7669 726f 6e2e 6765 7428 2254 4f47  environ.get("TOG
+000016c0: 4554 4845 525f 4150 495f 4b45 5922 2929  ETHER_API_KEY"))
+000016d0: 0a70 726f 6d70 7473 203d 205b 0a20 2020  .prompts = [.   
+000016e0: 2022 5772 6974 6520 6120 4e65 7874 2e6a   "Write a Next.j
+000016f0: 7320 636f 6d70 6f6e 656e 7420 7769 7468  s component with
+00001700: 2054 6169 6c77 696e 6443 5353 2066 6f72   TailwindCSS for
+00001710: 2061 2068 6561 6465 7220 636f 6d70 6f6e   a header compon
+00001720: 656e 742e 222c 0a20 2020 2022 5772 6974  ent.",.    "Writ
+00001730: 6520 6120 7079 7468 6f6e 2066 756e 6374  e a python funct
+00001740: 696f 6e20 666f 7220 7468 6520 6669 626f  ion for the fibo
+00001750: 6e61 6363 6920 7365 7175 656e 6365 222c  nacci sequence",
+00001760: 0a5d 0a0a 6173 796e 6320 6465 6620 6173  .]..async def as
+00001770: 796e 635f 6368 6174 5f63 6f6d 706c 6574  ync_chat_complet
+00001780: 696f 6e28 7072 6f6d 7074 7329 3a0a 2020  ion(prompts):.  
+00001790: 2020 6173 796e 635f 636c 6965 6e74 203d    async_client =
+000017a0: 2041 7379 6e63 546f 6765 7468 6572 2861   AsyncTogether(a
+000017b0: 7069 5f6b 6579 3d6f 732e 656e 7669 726f  pi_key=os.enviro
+000017c0: 6e2e 6765 7428 2254 4f47 4554 4845 525f  n.get("TOGETHER_
+000017d0: 4150 495f 4b45 5922 2929 0a20 2020 2074  API_KEY")).    t
+000017e0: 6173 6b73 203d 205b 0a20 2020 2020 2020  asks = [.       
+000017f0: 2061 7379 6e63 5f63 6c69 656e 742e 636f   async_client.co
+00001800: 6d70 6c65 7469 6f6e 732e 6372 6561 7465  mpletions.create
+00001810: 280a 2020 2020 2020 2020 2020 2020 6d6f  (.            mo
+00001820: 6465 6c3d 2263 6f64 656c 6c61 6d61 2f43  del="codellama/C
+00001830: 6f64 654c 6c61 6d61 2d33 3462 2d50 7974  odeLlama-34b-Pyt
+00001840: 686f 6e2d 6866 222c 0a20 2020 2020 2020  hon-hf",.       
+00001850: 2020 2020 2070 726f 6d70 743d 7072 6f6d       prompt=prom
+00001860: 7074 2c0a 2020 2020 2020 2020 290a 2020  pt,.        ).  
+00001870: 2020 2020 2020 666f 7220 7072 6f6d 7074        for prompt
+00001880: 2069 6e20 7072 6f6d 7074 730a 2020 2020   in prompts.    
+00001890: 5d0a 2020 2020 7265 7370 6f6e 7365 7320  ].    responses 
+000018a0: 3d20 6177 6169 7420 6173 796e 6369 6f2e  = await asyncio.
+000018b0: 6761 7468 6572 282a 7461 736b 7329 0a0a  gather(*tasks)..
+000018c0: 2020 2020 666f 7220 7265 7370 6f6e 7365      for response
+000018d0: 2069 6e20 7265 7370 6f6e 7365 733a 0a20   in responses:. 
+000018e0: 2020 2020 2020 2070 7269 6e74 2872 6573         print(res
+000018f0: 706f 6e73 652e 6368 6f69 6365 735b 305d  ponse.choices[0]
+00001900: 2e74 6578 7429 0a0a 6173 796e 6369 6f2e  .text)..asyncio.
+00001910: 7275 6e28 6173 796e 635f 6368 6174 5f63  run(async_chat_c
+00001920: 6f6d 706c 6574 696f 6e28 7072 6f6d 7074  ompletion(prompt
+00001930: 7329 290a 6060 600a 0a23 2323 2049 6d61  s)).```..### Ima
+00001940: 6765 2067 656e 6572 6174 696f 6e0a 0a60  ge generation..`
+00001950: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
+00001960: 6f73 0a66 726f 6d20 746f 6765 7468 6572  os.from together
+00001970: 2069 6d70 6f72 7420 546f 6765 7468 6572   import Together
+00001980: 0a0a 636c 6965 6e74 203d 2054 6f67 6574  ..client = Toget
+00001990: 6865 7228 6170 695f 6b65 793d 6f73 2e65  her(api_key=os.e
+000019a0: 6e76 6972 6f6e 2e67 6574 2822 544f 4745  nviron.get("TOGE
+000019b0: 5448 4552 5f41 5049 5f4b 4559 2229 290a  THER_API_KEY")).
+000019c0: 0a72 6573 706f 6e73 6520 3d20 636c 6965  .response = clie
+000019d0: 6e74 2e69 6d61 6765 732e 6765 6e65 7261  nt.images.genera
+000019e0: 7465 280a 2020 2020 7072 6f6d 7074 3d22  te(.    prompt="
+000019f0: 7370 6163 6520 726f 626f 7473 222c 0a20  space robots",. 
+00001a00: 2020 206d 6f64 656c 3d22 7374 6162 696c     model="stabil
+00001a10: 6974 7961 692f 7374 6162 6c65 2d64 6966  ityai/stable-dif
+00001a20: 6675 7369 6f6e 2d78 6c2d 6261 7365 2d31  fusion-xl-base-1
+00001a30: 2e30 222c 0a20 2020 2073 7465 7073 3d31  .0",.    steps=1
+00001a40: 302c 0a20 2020 206e 3d34 2c0a 290a 7072  0,.    n=4,.).pr
+00001a50: 696e 7428 7265 7370 6f6e 7365 2e64 6174  int(response.dat
+00001a60: 615b 305d 2e62 3634 5f6a 736f 6e29 0a60  a[0].b64_json).`
+00001a70: 6060 0a0a 2323 2320 456d 6265 6464 696e  ``..### Embeddin
+00001a80: 6773 0a0a 6060 6070 7974 686f 6e0a 6672  gs..```python.fr
+00001a90: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
+00001aa0: 204c 6973 740a 6672 6f6d 2074 6f67 6574   List.from toget
+00001ab0: 6865 7220 696d 706f 7274 2054 6f67 6574  her import Toget
+00001ac0: 6865 720a 0a63 6c69 656e 7420 3d20 546f  her..client = To
+00001ad0: 6765 7468 6572 2861 7069 5f6b 6579 3d6f  gether(api_key=o
+00001ae0: 732e 656e 7669 726f 6e2e 6765 7428 2254  s.environ.get("T
+00001af0: 4f47 4554 4845 525f 4150 495f 4b45 5922  OGETHER_API_KEY"
+00001b00: 2929 0a0a 6465 6620 6765 745f 656d 6265  ))..def get_embe
+00001b10: 6464 696e 6773 2874 6578 7473 3a20 4c69  ddings(texts: Li
+00001b20: 7374 5b73 7472 5d2c 206d 6f64 656c 3a20  st[str], model: 
+00001b30: 7374 7229 202d 3e20 4c69 7374 5b4c 6973  str) -> List[Lis
+00001b40: 745b 666c 6f61 745d 5d3a 0a20 2020 2074  t[float]]:.    t
+00001b50: 6578 7473 203d 205b 7465 7874 2e72 6570  exts = [text.rep
+00001b60: 6c61 6365 2822 5c6e 222c 2022 2022 2920  lace("\n", " ") 
+00001b70: 666f 7220 7465 7874 2069 6e20 7465 7874  for text in text
+00001b80: 735d 0a20 2020 206f 7574 7075 7473 203d  s].    outputs =
+00001b90: 2063 6c69 656e 742e 656d 6265 6464 696e   client.embeddin
+00001ba0: 6773 2e63 7265 6174 6528 6d6f 6465 6c3d  gs.create(model=
+00001bb0: 6d6f 6465 6c2c 2069 6e70 7574 203d 2074  model, input = t
+00001bc0: 6578 7473 290a 2020 2020 7265 7475 726e  exts).    return
+00001bd0: 205b 6f75 7470 7574 732e 6461 7461 5b69   [outputs.data[i
+00001be0: 5d2e 656d 6265 6464 696e 6720 666f 7220  ].embedding for 
+00001bf0: 6920 696e 2072 616e 6765 286c 656e 2874  i in range(len(t
+00001c00: 6578 7473 2929 5d0a 0a69 6e70 7574 5f74  exts))]..input_t
+00001c10: 6578 7473 203d 205b 274f 7572 2073 6f6c  exts = ['Our sol
+00001c20: 6172 2073 7973 7465 6d20 6f72 6269 7473  ar system orbits
+00001c30: 2074 6865 204d 696c 6b79 2057 6179 2067   the Milky Way g
+00001c40: 616c 6178 7920 6174 2061 626f 7574 2035  alaxy at about 5
+00001c50: 3135 2c30 3030 206d 7068 275d 0a65 6d62  15,000 mph'].emb
+00001c60: 6564 6469 6e67 7320 3d20 6765 745f 656d  eddings = get_em
+00001c70: 6265 6464 696e 6773 2869 6e70 7574 5f74  beddings(input_t
+00001c80: 6578 7473 2c20 6d6f 6465 6c3d 2774 6f67  exts, model='tog
+00001c90: 6574 6865 7263 6f6d 7075 7465 722f 6d32  ethercomputer/m2
+00001ca0: 2d62 6572 742d 3830 4d2d 386b 2d72 6574  -bert-80M-8k-ret
+00001cb0: 7269 6576 616c 2729 0a0a 7072 696e 7428  rieval')..print(
+00001cc0: 656d 6265 6464 696e 6773 290a 6060 600a  embeddings).```.
+00001cd0: 0a23 2323 2046 696c 6573 0a0a 5468 6520  .### Files..The 
+00001ce0: 6669 6c65 7320 4150 4920 6973 2075 7365  files API is use
+00001cf0: 6420 666f 7220 6669 6e65 2d74 756e 696e  d for fine-tunin
+00001d00: 6720 616e 6420 616c 6c6f 7773 2064 6576  g and allows dev
+00001d10: 656c 6f70 6572 7320 746f 2075 706c 6f61  elopers to uploa
+00001d20: 6420 6461 7461 2074 6f20 6669 6e65 2d74  d data to fine-t
+00001d30: 756e 6520 6f6e 2e20 4974 2061 6c73 6f20  une on. It also 
+00001d40: 6861 7320 7365 7665 7261 6c20 6d65 7468  has several meth
+00001d50: 6f64 7320 746f 206c 6973 7420 616c 6c20  ods to list all 
+00001d60: 6669 6c65 732c 2072 6574 7269 7665 2066  files, retrive f
+00001d70: 696c 6573 2c20 616e 6420 6465 6c65 7465  iles, and delete
+00001d80: 2066 696c 6573 2e20 506c 6561 7365 2072   files. Please r
+00001d90: 6566 6572 2074 6f20 6f75 7220 6669 6e65  efer to our fine
+00001da0: 2d74 756e 696e 6720 646f 6373 205b 6865  -tuning docs [he
+00001db0: 7265 5d28 6874 7470 733a 2f2f 646f 6373  re](https://docs
+00001dc0: 2e74 6f67 6574 6865 722e 6169 2f64 6f63  .together.ai/doc
+00001dd0: 732f 6669 6e65 2d74 756e 696e 672d 7079  s/fine-tuning-py
+00001de0: 7468 6f6e 292e 0a0a 6060 6070 7974 686f  thon)...```pytho
+00001df0: 6e0a 696d 706f 7274 206f 730a 6672 6f6d  n.import os.from
+00001e00: 2074 6f67 6574 6865 7220 696d 706f 7274   together import
+00001e10: 2054 6f67 6574 6865 720a 0a63 6c69 656e   Together..clien
+00001e20: 7420 3d20 546f 6765 7468 6572 2861 7069  t = Together(api
+00001e30: 5f6b 6579 3d6f 732e 656e 7669 726f 6e2e  _key=os.environ.
+00001e40: 6765 7428 2254 4f47 4554 4845 525f 4150  get("TOGETHER_AP
+00001e50: 495f 4b45 5922 2929 0a0a 636c 6965 6e74  I_KEY"))..client
+00001e60: 2e66 696c 6573 2e75 706c 6f61 6428 6669  .files.upload(fi
+00001e70: 6c65 3d22 736f 6d65 6461 7461 2e6a 736f  le="somedata.jso
+00001e80: 6e6c 2229 2023 2075 706c 6f61 6473 2061  nl") # uploads a
+00001e90: 2066 696c 650a 636c 6965 6e74 2e66 696c   file.client.fil
+00001ea0: 6573 2e6c 6973 7428 2920 2320 6c69 7374  es.list() # list
+00001eb0: 7320 616c 6c20 7570 6c6f 6164 6564 2066  s all uploaded f
+00001ec0: 696c 6573 0a63 6c69 656e 742e 6669 6c65  iles.client.file
+00001ed0: 732e 7265 7472 6965 7665 2869 643d 2266  s.retrieve(id="f
+00001ee0: 696c 652d 6430 6433 3138 6362 2d62 3764  ile-d0d318cb-b7d
+00001ef0: 392d 3439 3361 2d62 6437 302d 3163 6665  9-493a-bd70-1cfe
+00001f00: 3038 3964 3338 3135 2229 2023 2072 6574  089d3815") # ret
+00001f10: 7269 6576 6573 2061 2073 7065 6369 6669  rieves a specifi
+00001f20: 6320 6669 6c65 0a63 6c69 656e 742e 6669  c file.client.fi
+00001f30: 6c65 732e 7265 7472 6965 7665 5f63 6f6e  les.retrieve_con
+00001f40: 7465 6e74 2869 643d 2266 696c 652d 6430  tent(id="file-d0
+00001f50: 6433 3138 6362 2d62 3764 392d 3439 3361  d318cb-b7d9-493a
+00001f60: 2d62 6437 302d 3163 6665 3038 3964 3338  -bd70-1cfe089d38
+00001f70: 3135 2229 2023 2072 6574 7269 6576 6573  15") # retrieves
+00001f80: 2063 6f6e 7465 6e74 206f 6620 6120 7370   content of a sp
+00001f90: 6563 6966 6963 2066 696c 650a 636c 6965  ecific file.clie
+00001fa0: 6e74 2e66 696c 6573 2e64 656c 6574 6528  nt.files.delete(
+00001fb0: 6964 3d22 6669 6c65 2d64 3064 3331 3863  id="file-d0d318c
+00001fc0: 622d 6237 6439 2d34 3933 612d 6264 3730  b-b7d9-493a-bd70
+00001fd0: 2d31 6366 6530 3839 6433 3831 3522 2920  -1cfe089d3815") 
+00001fe0: 2320 6465 6c65 7465 7320 6120 6669 6c65  # deletes a file
+00001ff0: 0a60 6060 0a0a 2323 2320 4669 6e65 2d74  .```..### Fine-t
+00002000: 756e 6573 0a0a 5468 6520 6669 6e65 7475  unes..The finetu
+00002010: 6e65 2041 5049 2069 7320 7573 6564 2066  ne API is used f
+00002020: 6f72 2066 696e 652d 7475 6e69 6e67 2061  or fine-tuning a
+00002030: 6e64 2061 6c6c 6f77 7320 6465 7665 6c6f  nd allows develo
+00002040: 7065 7273 2074 6f20 6372 6561 7465 2066  pers to create f
+00002050: 696e 6574 756e 696e 6720 6a6f 6273 2e20  inetuning jobs. 
+00002060: 4974 2061 6c73 6f20 6861 7320 7365 7665  It also has seve
+00002070: 7261 6c20 6d65 7468 6f64 7320 746f 206c  ral methods to l
+00002080: 6973 7420 616c 6c20 6a6f 6273 2c20 7265  ist all jobs, re
+00002090: 7472 6976 6520 7374 6174 7573 6573 2061  trive statuses a
+000020a0: 6e64 2067 6574 2063 6865 636b 706f 696e  nd get checkpoin
+000020b0: 7473 2e20 506c 6561 7365 2072 6566 6572  ts. Please refer
+000020c0: 2074 6f20 6f75 7220 6669 6e65 2d74 756e   to our fine-tun
+000020d0: 696e 6720 646f 6373 205b 6865 7265 5d28  ing docs [here](
+000020e0: 6874 7470 733a 2f2f 646f 6373 2e74 6f67  https://docs.tog
+000020f0: 6574 6865 722e 6169 2f64 6f63 732f 6669  ether.ai/docs/fi
+00002100: 6e65 2d74 756e 696e 672d 7079 7468 6f6e  ne-tuning-python
+00002110: 292e 0a0a 6060 6070 7974 686f 6e0a 696d  )...```python.im
+00002120: 706f 7274 206f 730a 6672 6f6d 2074 6f67  port os.from tog
+00002130: 6574 6865 7220 696d 706f 7274 2054 6f67  ether import Tog
+00002140: 6574 6865 720a 0a63 6c69 656e 7420 3d20  ether..client = 
+00002150: 546f 6765 7468 6572 2861 7069 5f6b 6579  Together(api_key
+00002160: 3d6f 732e 656e 7669 726f 6e2e 6765 7428  =os.environ.get(
+00002170: 2254 4f47 4554 4845 525f 4150 495f 4b45  "TOGETHER_API_KE
+00002180: 5922 2929 0a0a 636c 6965 6e74 2e66 696e  Y"))..client.fin
+00002190: 655f 7475 6e69 6e67 2e63 7265 6174 6528  e_tuning.create(
+000021a0: 0a20 2074 7261 696e 696e 675f 6669 6c65  .  training_file
+000021b0: 203d 2027 6669 6c65 2d64 3064 3331 3863   = 'file-d0d318c
+000021c0: 622d 6237 6439 2d34 3933 612d 6264 3730  b-b7d9-493a-bd70
+000021d0: 2d31 6366 6530 3839 6433 3831 3527 2c0a  -1cfe089d3815',.
+000021e0: 2020 6d6f 6465 6c20 3d20 276d 6973 7472    model = 'mistr
+000021f0: 616c 6169 2f4d 6978 7472 616c 2d38 7837  alai/Mixtral-8x7
+00002200: 422d 496e 7374 7275 6374 2d76 302e 3127  B-Instruct-v0.1'
+00002210: 2c0a 2020 6e5f 6570 6f63 6873 203d 2033  ,.  n_epochs = 3
+00002220: 2c0a 2020 6e5f 6368 6563 6b70 6f69 6e74  ,.  n_checkpoint
+00002230: 7320 3d20 312c 0a20 2062 6174 6368 5f73  s = 1,.  batch_s
+00002240: 697a 6520 3d20 342c 0a20 206c 6561 726e  ize = 4,.  learn
+00002250: 696e 675f 7261 7465 203d 2031 652d 352c  ing_rate = 1e-5,
+00002260: 0a20 2073 7566 6669 7820 3d20 276d 792d  .  suffix = 'my-
+00002270: 6465 6d6f 2d66 696e 6574 756e 6527 2c0a  demo-finetune',.
+00002280: 2020 7761 6e64 625f 6170 695f 6b65 7920    wandb_api_key 
+00002290: 3d20 2731 6132 6233 6334 6435 652e 2e2e  = '1a2b3c4d5e...
+000022a0: 2e2e 2e2e 272c 0a29 0a63 6c69 656e 742e  ....',.).client.
+000022b0: 6669 6e65 5f74 756e 696e 672e 6c69 7374  fine_tuning.list
+000022c0: 2829 2023 206c 6973 7473 2061 6c6c 2066  () # lists all f
+000022d0: 696e 652d 7475 6e65 6420 6a6f 6273 0a63  ine-tuned jobs.c
+000022e0: 6c69 656e 742e 6669 6e65 5f74 756e 696e  lient.fine_tunin
+000022f0: 672e 7265 7472 6965 7665 2869 643d 2266  g.retrieve(id="f
+00002300: 742d 6336 3661 3563 3138 2d31 6436 642d  t-c66a5c18-1d6d-
+00002310: 3433 6339 2d39 3462 642d 3332 6437 3536  43c9-94bd-32d756
+00002320: 3432 3562 3462 2229 2023 2072 6574 7269  425b4b") # retri
+00002330: 6576 6573 2069 6e66 6f72 6d61 7469 6f6e  eves information
+00002340: 206f 6e20 6669 6e65 7475 6e65 2065 7665   on finetune eve
+00002350: 6e74 0a63 6c69 656e 742e 6669 6e65 5f74  nt.client.fine_t
+00002360: 756e 696e 672e 6361 6e63 656c 2869 643d  uning.cancel(id=
+00002370: 2266 742d 6336 3661 3563 3138 2d31 6436  "ft-c66a5c18-1d6
+00002380: 642d 3433 6339 2d39 3462 642d 3332 6437  d-43c9-94bd-32d7
+00002390: 3536 3432 3562 3462 2229 2023 2043 616e  56425b4b") # Can
+000023a0: 6365 6c73 2061 2066 696e 652d 7475 6e69  cels a fine-tuni
+000023b0: 6e67 206a 6f62 0a63 6c69 656e 742e 6669  ng job.client.fi
+000023c0: 6e65 5f74 756e 696e 672e 6c69 7374 5f65  ne_tuning.list_e
+000023d0: 7665 6e74 7328 6964 3d22 6674 2d63 3636  vents(id="ft-c66
+000023e0: 6135 6331 382d 3164 3664 2d34 3363 392d  a5c18-1d6d-43c9-
+000023f0: 3934 6264 2d33 3264 3735 3634 3235 6234  94bd-32d756425b4
+00002400: 6222 2920 2320 204c 6973 7473 2065 7665  b") #  Lists eve
+00002410: 6e74 7320 6f66 2061 2066 696e 652d 7475  nts of a fine-tu
+00002420: 6e65 206a 6f62 0a63 6c69 656e 742e 6669  ne job.client.fi
+00002430: 6e65 5f74 756e 696e 672e 646f 776e 6c6f  ne_tuning.downlo
+00002440: 6164 2869 643d 2266 742d 6336 3661 3563  ad(id="ft-c66a5c
+00002450: 3138 2d31 6436 642d 3433 6339 2d39 3462  18-1d6d-43c9-94b
+00002460: 642d 3332 6437 3536 3432 3562 3462 2229  d-32d756425b4b")
+00002470: 2023 2064 6f77 6e6c 6f61 6473 2063 6f6d   # downloads com
+00002480: 7072 6573 7365 6420 6669 6e65 2d74 756e  pressed fine-tun
+00002490: 6564 206d 6f64 656c 206f 7220 6368 6563  ed model or chec
+000024a0: 6b70 6f69 6e74 2074 6f20 6c6f 6361 6c20  kpoint to local 
+000024b0: 6469 736b 0a60 6060 0a0a 2323 2320 4d6f  disk.```..### Mo
+000024c0: 6465 6c73 0a0a 5468 6973 206c 6973 7473  dels..This lists
+000024d0: 2061 6c6c 2074 6865 206d 6f64 656c 7320   all the models 
+000024e0: 7468 6174 2054 6f67 6574 6865 7220 7375  that Together su
+000024f0: 7070 6f72 7473 2e0a 0a60 6060 7079 7468  pports...```pyth
+00002500: 6f6e 0a69 6d70 6f72 7420 6f73 0a66 726f  on.import os.fro
+00002510: 6d20 746f 6765 7468 6572 2069 6d70 6f72  m together impor
+00002520: 7420 546f 6765 7468 6572 0a0a 636c 6965  t Together..clie
+00002530: 6e74 203d 2054 6f67 6574 6865 7228 6170  nt = Together(ap
+00002540: 695f 6b65 793d 6f73 2e65 6e76 6972 6f6e  i_key=os.environ
+00002550: 2e67 6574 2822 544f 4745 5448 4552 5f41  .get("TOGETHER_A
+00002560: 5049 5f4b 4559 2229 290a 0a6d 6f64 656c  PI_KEY"))..model
+00002570: 7320 3d20 636c 6965 6e74 2e6d 6f64 656c  s = client.model
+00002580: 732e 6c69 7374 2829 0a0a 666f 7220 6d6f  s.list()..for mo
+00002590: 6465 6c20 696e 206d 6f64 656c 733a 0a20  del in models:. 
+000025a0: 2020 2070 7269 6e74 286d 6f64 656c 290a     print(model).
+000025b0: 6060 600a 0a23 2320 5573 6167 6520 e280  ```..## Usage ..
+000025c0: 9320 434c 490a 0a23 2323 2043 6861 7420  . CLI..### Chat 
+000025d0: 436f 6d70 6c65 7469 6f6e 730a 0a60 6060  Completions..```
+000025e0: 6261 7368 0a74 6f67 6574 6865 7220 6368  bash.together ch
+000025f0: 6174 2e63 6f6d 706c 6574 696f 6e73 205c  at.completions \
+00002600: 0a20 202d 2d6d 6573 7361 6765 2022 7379  .  --message "sy
+00002610: 7374 656d 2220 2259 6f75 2061 7265 2061  stem" "You are a
+00002620: 2068 656c 7066 756c 2061 7373 6973 7461   helpful assista
+00002630: 6e74 206e 616d 6564 2054 6f67 6574 6865  nt named Togethe
+00002640: 7222 205c 0a20 202d 2d6d 6573 7361 6765  r" \.  --message
+00002650: 2022 7573 6572 2220 2257 6861 7420 6973   "user" "What is
+00002660: 2079 6f75 7220 6e61 6d65 3f22 205c 0a20   your name?" \. 
+00002670: 202d 2d6d 6f64 656c 206d 6973 7472 616c   --model mistral
+00002680: 6169 2f4d 6978 7472 616c 2d38 7837 422d  ai/Mixtral-8x7B-
+00002690: 496e 7374 7275 6374 2d76 302e 310a 6060  Instruct-v0.1.``
+000026a0: 600a 0a54 6865 2043 6861 7420 436f 6d70  `..The Chat Comp
+000026b0: 6c65 7469 6f6e 7320 434c 4920 656e 6162  letions CLI enab
+000026c0: 6c65 7320 7374 7265 616d 696e 6720 746f  les streaming to
+000026d0: 6b65 6e73 2074 6f20 7374 646f 7574 2062  kens to stdout b
+000026e0: 7920 6465 6661 756c 742e 2054 6f20 6469  y default. To di
+000026f0: 7361 626c 6520 7374 7265 616d 696e 672c  sable streaming,
+00002700: 2075 7365 2060 2d2d 6e6f 2d73 7472 6561   use `--no-strea
+00002710: 6d60 2e0a 0a23 2323 2043 6f6d 706c 6574  m`...### Complet
+00002720: 696f 6e73 0a0a 6060 6062 6173 680a 746f  ions..```bash.to
+00002730: 6765 7468 6572 2063 6f6d 706c 6574 696f  gether completio
+00002740: 6e73 205c 0a20 2022 4c61 7267 6520 6c61  ns \.  "Large la
+00002750: 6e67 7561 6765 206d 6f64 656c 7320 6172  nguage models ar
+00002760: 6520 2220 5c0a 2020 2d2d 6d6f 6465 6c20  e " \.  --model 
+00002770: 6d69 7374 7261 6c61 692f 4d69 7874 7261  mistralai/Mixtra
+00002780: 6c2d 3878 3742 2d76 302e 3120 5c0a 2020  l-8x7B-v0.1 \.  
+00002790: 2d2d 6d61 782d 746f 6b65 6e73 2035 3132  --max-tokens 512
+000027a0: 205c 0a20 202d 2d73 746f 7020 222e 220a   \.  --stop ".".
+000027b0: 6060 600a 0a54 6865 2043 6f6d 706c 6574  ```..The Complet
+000027c0: 696f 6e73 2043 4c49 2065 6e61 626c 6573  ions CLI enables
+000027d0: 2073 7472 6561 6d69 6e67 2074 6f6b 656e   streaming token
+000027e0: 7320 746f 2073 7464 6f75 7420 6279 2064  s to stdout by d
+000027f0: 6566 6175 6c74 2e20 546f 2064 6973 6162  efault. To disab
+00002800: 6c65 2073 7472 6561 6d69 6e67 2c20 7573  le streaming, us
+00002810: 6520 602d 2d6e 6f2d 7374 7265 616d 602e  e `--no-stream`.
+00002820: 0a0a 2323 2320 496d 6167 6520 4765 6e65  ..### Image Gene
+00002830: 7261 7469 6f6e 730a 0a60 6060 6261 7368  rations..```bash
+00002840: 0a74 6f67 6574 6865 7220 696d 6167 6573  .together images
+00002850: 2067 656e 6572 6174 6520 5c0a 2020 2273   generate \.  "s
+00002860: 7061 6365 2072 6f62 6f74 7322 205c 0a20  pace robots" \. 
+00002870: 202d 2d6d 6f64 656c 2073 7461 6269 6c69   --model stabili
+00002880: 7479 6169 2f73 7461 626c 652d 6469 6666  tyai/stable-diff
+00002890: 7573 696f 6e2d 786c 2d62 6173 652d 312e  usion-xl-base-1.
+000028a0: 3020 5c0a 2020 2d2d 6e20 340a 6060 600a  0 \.  --n 4.```.
+000028b0: 0a54 6865 2069 6d61 6765 2069 7320 6f70  .The image is op
+000028c0: 656e 6564 2069 6e20 7468 6520 6465 6661  ened in the defa
+000028d0: 756c 7420 696d 6167 6520 7669 6577 6572  ult image viewer
+000028e0: 2062 7920 6465 6661 756c 742e 2054 6f20   by default. To 
+000028f0: 6469 7361 626c 6520 7468 6973 2c20 7573  disable this, us
+00002900: 6520 602d 2d6e 6f2d 7368 6f77 602e 0a0a  e `--no-show`...
+00002910: 2323 2320 4669 6c65 730a 0a60 6060 6261  ### Files..```ba
+00002920: 7368 0a23 2048 656c 700a 746f 6765 7468  sh.# Help.togeth
+00002930: 6572 2066 696c 6573 202d 2d68 656c 700a  er files --help.
+00002940: 0a23 2043 6865 636b 2066 696c 650a 746f  .# Check file.to
+00002950: 6765 7468 6572 2066 696c 6573 2063 6865  gether files che
+00002960: 636b 2065 7861 6d70 6c65 2e6a 736f 6e6c  ck example.jsonl
+00002970: 0a0a 2320 5570 6c6f 6164 2066 696c 650a  ..# Upload file.
+00002980: 746f 6765 7468 6572 2066 696c 6573 2075  together files u
+00002990: 706c 6f61 6420 6578 616d 706c 652e 6a73  pload example.js
+000029a0: 6f6e 6c0a 0a23 204c 6973 7420 6669 6c65  onl..# List file
+000029b0: 730a 746f 6765 7468 6572 2066 696c 6573  s.together files
+000029c0: 206c 6973 740a 0a23 2052 6574 7269 6576   list..# Retriev
+000029d0: 6520 6669 6c65 206d 6574 6164 6174 610a  e file metadata.
+000029e0: 746f 6765 7468 6572 2066 696c 6573 2072  together files r
+000029f0: 6574 7269 6576 6520 6669 6c65 2d36 6635  etrieve file-6f5
+00002a00: 3066 3964 312d 3562 3935 2d34 3136 632d  0f9d1-5b95-416c-
+00002a10: 3930 3430 2d30 3739 3962 3262 3462 3839  9040-0799b2b4b89
+00002a20: 340a 0a23 2052 6574 7269 6576 6520 6669  4..# Retrieve fi
+00002a30: 6c65 2063 6f6e 7465 6e74 0a74 6f67 6574  le content.toget
+00002a40: 6865 7220 6669 6c65 7320 7265 7472 6965  her files retrie
+00002a50: 7665 2d63 6f6e 7465 6e74 2066 696c 652d  ve-content file-
+00002a60: 3666 3530 6639 6431 2d35 6239 352d 3431  6f50f9d1-5b95-41
+00002a70: 3663 2d39 3034 302d 3037 3939 6232 6234  6c-9040-0799b2b4
+00002a80: 6238 3934 0a0a 2320 4465 6c65 7465 2072  b894..# Delete r
+00002a90: 656d 6f74 6520 6669 6c65 0a74 6f67 6574  emote file.toget
+00002aa0: 6865 7220 6669 6c65 7320 6465 6c65 7465  her files delete
+00002ab0: 2066 696c 652d 3666 3530 6639 6431 2d35   file-6f50f9d1-5
+00002ac0: 6239 352d 3431 3663 2d39 3034 302d 3037  b95-416c-9040-07
+00002ad0: 3939 6232 6234 6238 3934 0a60 6060 0a0a  99b2b4b894.```..
+00002ae0: 2323 2320 4669 6e65 2d74 756e 696e 670a  ### Fine-tuning.
+00002af0: 0a60 6060 6261 7368 0a23 2048 656c 700a  .```bash.# Help.
+00002b00: 746f 6765 7468 6572 2066 696e 652d 7475  together fine-tu
+00002b10: 6e69 6e67 202d 2d68 656c 700a 0a23 2043  ning --help..# C
+00002b20: 7265 6174 6520 6669 6e65 2d74 756e 6520  reate fine-tune 
+00002b30: 6a6f 620a 746f 6765 7468 6572 2066 696e  job.together fin
+00002b40: 652d 7475 6e69 6e67 2063 7265 6174 6520  e-tuning create 
+00002b50: 5c0a 2020 2d2d 6d6f 6465 6c20 746f 6765  \.  --model toge
+00002b60: 7468 6572 636f 6d70 7574 6572 2f6c 6c61  thercomputer/lla
+00002b70: 6d61 2d32 2d37 622d 6368 6174 205c 0a20  ma-2-7b-chat \. 
+00002b80: 202d 2d74 7261 696e 696e 672d 6669 6c65   --training-file
+00002b90: 2066 696c 652d 3731 3164 3837 3234 2d62   file-711d8724-b
+00002ba0: 3365 332d 3461 6532 2d62 3531 362d 3934  3e3-4ae2-b516-94
+00002bb0: 3834 3139 3538 3131 3764 0a0a 2320 4c69  841958117d..# Li
+00002bc0: 7374 2066 696e 652d 7475 6e65 206a 6f62  st fine-tune job
+00002bd0: 730a 746f 6765 7468 6572 2066 696e 652d  s.together fine-
+00002be0: 7475 6e69 6e67 206c 6973 740a 0a23 2052  tuning list..# R
+00002bf0: 6574 7269 6576 6520 6669 6e65 2d74 756e  etrieve fine-tun
+00002c00: 6520 6a6f 6220 6465 7461 696c 730a 746f  e job details.to
+00002c10: 6765 7468 6572 2066 696e 652d 7475 6e69  gether fine-tuni
+00002c20: 6e67 2072 6574 7269 6576 6520 6674 2d63  ng retrieve ft-c
+00002c30: 3636 6135 6331 382d 3164 3664 2d34 3363  66a5c18-1d6d-43c
+00002c40: 392d 3934 6264 2d33 3264 3735 3634 3235  9-94bd-32d756425
+00002c50: 6234 620a 0a23 204c 6973 7420 6669 6e65  b4b..# List fine
+00002c60: 2d74 756e 6520 6a6f 6220 6576 656e 7473  -tune job events
+00002c70: 0a74 6f67 6574 6865 7220 6669 6e65 2d74  .together fine-t
+00002c80: 756e 696e 6720 6c69 7374 2d65 7665 6e74  uning list-event
+00002c90: 7320 6674 2d63 3636 6135 6331 382d 3164  s ft-c66a5c18-1d
+00002ca0: 3664 2d34 3363 392d 3934 6264 2d33 3264  6d-43c9-94bd-32d
+00002cb0: 3735 3634 3235 6234 620a 0a23 2043 616e  756425b4b..# Can
+00002cc0: 6365 6c20 7275 6e6e 696e 6720 6a6f 620a  cel running job.
+00002cd0: 746f 6765 7468 6572 2066 696e 652d 7475  together fine-tu
+00002ce0: 6e69 6e67 2063 616e 6365 6c20 6674 2d63  ning cancel ft-c
+00002cf0: 3636 6135 6331 382d 3164 3664 2d34 3363  66a5c18-1d6d-43c
+00002d00: 392d 3934 6264 2d33 3264 3735 3634 3235  9-94bd-32d756425
+00002d10: 6234 620a 0a23 2044 6f77 6e6c 6f61 6420  b4b..# Download 
+00002d20: 6669 6e65 2d74 756e 6564 206d 6f64 656c  fine-tuned model
+00002d30: 2077 6569 6768 7473 0a74 6f67 6574 6865   weights.togethe
+00002d40: 7220 6669 6e65 2d74 756e 696e 6720 646f  r fine-tuning do
+00002d50: 776e 6c6f 6164 2066 742d 6336 3661 3563  wnload ft-c66a5c
+00002d60: 3138 2d31 6436 642d 3433 6339 2d39 3462  18-1d6d-43c9-94b
+00002d70: 642d 3332 6437 3536 3432 3562 3462 0a60  d-32d756425b4b.`
+00002d80: 6060 0a0a 2323 2320 4d6f 6465 6c73 0a0a  ``..### Models..
+00002d90: 6060 6062 6173 680a 2320 4865 6c70 0a74  ```bash.# Help.t
+00002da0: 6f67 6574 6865 7220 6d6f 6465 6c73 202d  ogether models -
+00002db0: 2d68 656c 700a 0a23 204c 6973 7420 6d6f  -help..# List mo
+00002dc0: 6465 6c73 0a74 6f67 6574 6865 7220 6d6f  dels.together mo
+00002dd0: 6465 6c73 206c 6973 740a 6060 600a 0a23  dels list.```..#
+00002de0: 2320 436f 6e74 7269 6275 7469 6e67 0a0a  # Contributing..
+00002df0: 5265 6665 7220 746f 2074 6865 205b 436f  Refer to the [Co
+00002e00: 6e74 7269 6275 7469 6e67 2047 7569 6465  ntributing Guide
+00002e10: 5d28 434f 4e54 5249 4255 5449 4e47 2e6d  ](CONTRIBUTING.m
+00002e20: 6429 0a0a                                d)..
```

