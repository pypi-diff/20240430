# Comparing `tmp/saltstack_age-0.2.1-py3-none-any.whl.zip` & `tmp/saltstack_age-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6133 bytes, number of entries: 11
+Zip file size: 9097 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 saltstack_age/__init__.py
 -rw-r--r--  2.0 unx     6101 b- defN 20-Feb-02 00:00 saltstack_age/cli.py
 -rw-r--r--  2.0 unx      752 b- defN 20-Feb-02 00:00 saltstack_age/identities.py
 -rw-r--r--  2.0 unx      109 b- defN 20-Feb-02 00:00 saltstack_age/passphrase.py
 -rw-r--r--  2.0 unx     1279 b- defN 20-Feb-02 00:00 saltstack_age/secure_value.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 saltstack_age/renderers/__init__.py
 -rw-r--r--  2.0 unx     2355 b- defN 20-Feb-02 00:00 saltstack_age/renderers/age.py
-?rw-r--r--  2.0 unx      345 b- defN 20-Feb-02 00:00 saltstack_age-0.2.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 saltstack_age-0.2.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx      102 b- defN 20-Feb-02 00:00 saltstack_age-0.2.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      909 b- defN 20-Feb-02 00:00 saltstack_age-0.2.1.dist-info/RECORD
-11 files, 12039 bytes uncompressed, 4579 bytes compressed:  62.0%
+?rw-r--r--  2.0 unx     7489 b- defN 20-Feb-02 00:00 saltstack_age-0.2.3.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 saltstack_age-0.2.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx      102 b- defN 20-Feb-02 00:00 saltstack_age-0.2.3.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      910 b- defN 20-Feb-02 00:00 saltstack_age-0.2.3.dist-info/RECORD
+11 files, 19184 bytes uncompressed, 7543 bytes compressed:  60.7%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: saltstack_age/renderers/__init__.py
 Comment: 
 
 Filename: saltstack_age/renderers/age.py
 Comment: 
 
-Filename: saltstack_age-0.2.1.dist-info/METADATA
+Filename: saltstack_age-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: saltstack_age-0.2.1.dist-info/WHEEL
+Filename: saltstack_age-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: saltstack_age-0.2.1.dist-info/entry_points.txt
+Filename: saltstack_age-0.2.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: saltstack_age-0.2.1.dist-info/RECORD
+Filename: saltstack_age-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `saltstack_age-0.2.1.dist-info/RECORD` & `saltstack_age-0.2.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 saltstack_age/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 saltstack_age/cli.py,sha256=m3KsLULzEmiZ0r5IedtghwZCC-KEQ-AAeBKECAPe_uA,6101
 saltstack_age/identities.py,sha256=5RicnFmDsKtYVqjRlI2wl9qFNtTkcm9jHKrPJ_9bXj4,752
 saltstack_age/passphrase.py,sha256=GdV9TmaAsIL5b043x6w0IUN0iN273tXjq2eW9SOU6XY,109
 saltstack_age/secure_value.py,sha256=kxPLJAg_gv7DRn-C6Le2x6sqiLKJrB89vK8VcoiOFyU,1279
 saltstack_age/renderers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 saltstack_age/renderers/age.py,sha256=S7J3DPq1Rtykg4T2Q-S6C46vRi1WEZVLG5rSXOmwF1Q,2355
-saltstack_age-0.2.1.dist-info/METADATA,sha256=IeldpI3UGNiE0qgh0X1NpdOkoe3hkg0RuycIVItV4q4,345
-saltstack_age-0.2.1.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
-saltstack_age-0.2.1.dist-info/entry_points.txt,sha256=AI6n3Tyjmxxz9FzJFJHJhhhv-hHZGhSrHFFjgbV2zH0,102
-saltstack_age-0.2.1.dist-info/RECORD,,
+saltstack_age-0.2.3.dist-info/METADATA,sha256=9Y9rm1NDEuiBcBG6XQuOjoyiAD4232C7on93lyCh4_I,7489
+saltstack_age-0.2.3.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+saltstack_age-0.2.3.dist-info/entry_points.txt,sha256=AI6n3Tyjmxxz9FzJFJHJhhhv-hHZGhSrHFFjgbV2zH0,102
+saltstack_age-0.2.3.dist-info/RECORD,,
```

