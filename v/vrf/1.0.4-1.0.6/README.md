# Comparing `tmp/vrf-1.0.4.tar.gz` & `tmp/vrf-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vrf-1.0.4.tar", last modified: Tue Sep 12 14:42:26 2023, max compression
+gzip compressed data, was "vrf-1.0.6.tar", last modified: Tue Apr 30 20:17:11 2024, max compression
```

## Comparing `vrf-1.0.4.tar` & `vrf-1.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ancientevil   (501) staff       (20)        0 2023-09-12 14:42:26.349457 vrf-1.0.4/
--rw-r--r--   0 ancientevil   (501) staff       (20)       90 2023-09-12 04:52:07.000000 vrf-1.0.4/MANIFEST.in
--rw-r--r--   0 ancientevil   (501) staff       (20)      198 2023-09-12 14:42:26.348958 vrf-1.0.4/PKG-INFO
--rw-r--r--   0 ancientevil   (501) staff       (20)     8963 2023-09-12 04:10:14.000000 vrf-1.0.4/README.md
--rw-r--r--   0 ancientevil   (501) staff       (20)       57 2023-09-12 04:23:37.000000 vrf-1.0.4/requirements.txt
--rw-r--r--   0 ancientevil   (501) staff       (20)       38 2023-09-12 14:42:26.349634 vrf-1.0.4/setup.cfg
--rw-r--r--   0 ancientevil   (501) staff       (20)      722 2023-09-12 14:41:49.000000 vrf-1.0.4/setup.py
-drwxr-xr-x   0 ancientevil   (501) staff       (20)        0 2023-09-12 14:42:26.341151 vrf-1.0.4/tests/
--rw-r--r--   0 ancientevil   (501) staff       (20)        0 2023-09-11 15:39:44.000000 vrf-1.0.4/tests/__init__.py
--rw-r--r--   0 ancientevil   (501) staff       (20)    18790 2023-09-12 14:40:27.000000 vrf-1.0.4/tests/test_generate_beta_and_proof.py
--rw-r--r--   0 ancientevil   (501) staff       (20)     7318 2023-09-12 14:40:27.000000 vrf-1.0.4/tests/test_generate_seed_salt_hash.py
--rw-r--r--   0 ancientevil   (501) staff       (20)     2464 2023-09-11 23:40:20.000000 vrf-1.0.4/tests/test_integration.py
--rw-r--r--   0 ancientevil   (501) staff       (20)     5742 2023-09-12 14:40:27.000000 vrf-1.0.4/tests/test_new_game.py
--rw-r--r--   0 ancientevil   (501) staff       (20)    18789 2023-09-11 23:40:20.000000 vrf-1.0.4/tests/test_verify.py
-drwxr-xr-x   0 ancientevil   (501) staff       (20)        0 2023-09-12 14:42:26.345301 vrf-1.0.4/vrf.egg-info/
--rw-r--r--   0 ancientevil   (501) staff       (20)      198 2023-09-12 14:42:26.000000 vrf-1.0.4/vrf.egg-info/PKG-INFO
--rw-r--r--   0 ancientevil   (501) staff       (20)      408 2023-09-12 14:42:26.000000 vrf-1.0.4/vrf.egg-info/SOURCES.txt
--rw-r--r--   0 ancientevil   (501) staff       (20)        1 2023-09-12 14:42:26.000000 vrf-1.0.4/vrf.egg-info/dependency_links.txt
--rw-r--r--   0 ancientevil   (501) staff       (20)       57 2023-09-12 14:42:26.000000 vrf-1.0.4/vrf.egg-info/requires.txt
--rw-r--r--   0 ancientevil   (501) staff       (20)       13 2023-09-12 14:42:26.000000 vrf-1.0.4/vrf.egg-info/top_level.txt
-drwxr-xr-x   0 ancientevil   (501) staff       (20)        0 2023-09-12 14:42:26.348109 vrf-1.0.4/vrf_py/
--rw-r--r--   0 ancientevil   (501) staff       (20)    12150 2023-09-12 14:39:12.000000 vrf-1.0.4/vrf_py/VRF.py
--rw-r--r--   0 ancientevil   (501) staff       (20)      117 2023-09-12 14:38:35.000000 vrf-1.0.4/vrf_py/__init__.py
--rw-r--r--   0 ancientevil   (501) staff       (20)      808 2023-09-11 15:38:19.000000 vrf-1.0.4/vrf_py/error.py
--rw-r--r--   0 ancientevil   (501) staff       (20)      774 2023-09-11 15:38:19.000000 vrf-1.0.4/vrf_py/log.py
+drwxr-xr-x   0 ancientevil   (501) staff       (20)        0 2024-04-30 20:17:11.519765 vrf-1.0.6/
+-rw-r--r--   0 ancientevil   (501) staff       (20)       90 2023-09-12 04:52:07.000000 vrf-1.0.6/MANIFEST.in
+-rw-r--r--   0 ancientevil   (501) staff       (20)      198 2024-04-30 20:17:11.519287 vrf-1.0.6/PKG-INFO
+-rw-r--r--   0 ancientevil   (501) staff       (20)     9235 2024-04-30 19:39:45.000000 vrf-1.0.6/README.md
+-rw-r--r--   0 ancientevil   (501) staff       (20)       44 2023-09-12 15:00:59.000000 vrf-1.0.6/requirements.txt
+-rw-r--r--   0 ancientevil   (501) staff       (20)       38 2024-04-30 20:17:11.519934 vrf-1.0.6/setup.cfg
+-rw-r--r--   0 ancientevil   (501) staff       (20)      722 2024-04-30 19:40:18.000000 vrf-1.0.6/setup.py
+drwxr-xr-x   0 ancientevil   (501) staff       (20)        0 2024-04-30 20:17:11.513323 vrf-1.0.6/tests/
+-rw-r--r--   0 ancientevil   (501) staff       (20)        0 2023-09-11 15:39:44.000000 vrf-1.0.6/tests/__init__.py
+-rw-r--r--   0 ancientevil   (501) staff       (20)    18790 2023-09-12 14:40:27.000000 vrf-1.0.6/tests/test_generate_beta_and_proof.py
+-rw-r--r--   0 ancientevil   (501) staff       (20)     7294 2023-09-15 18:09:21.000000 vrf-1.0.6/tests/test_generate_seed_salt_hash.py
+-rw-r--r--   0 ancientevil   (501) staff       (20)     2469 2024-04-23 21:02:42.000000 vrf-1.0.6/tests/test_integration.py
+-rw-r--r--   0 ancientevil   (501) staff       (20)     5742 2023-09-12 14:40:27.000000 vrf-1.0.6/tests/test_new_game.py
+-rw-r--r--   0 ancientevil   (501) staff       (20)    27906 2024-04-23 21:01:04.000000 vrf-1.0.6/tests/test_verify.py
+drwxr-xr-x   0 ancientevil   (501) staff       (20)        0 2024-04-30 20:17:11.516718 vrf-1.0.6/vrf.egg-info/
+-rw-r--r--   0 ancientevil   (501) staff       (20)      198 2024-04-30 20:17:11.000000 vrf-1.0.6/vrf.egg-info/PKG-INFO
+-rw-r--r--   0 ancientevil   (501) staff       (20)      408 2024-04-30 20:17:11.000000 vrf-1.0.6/vrf.egg-info/SOURCES.txt
+-rw-r--r--   0 ancientevil   (501) staff       (20)        1 2024-04-30 20:17:11.000000 vrf-1.0.6/vrf.egg-info/dependency_links.txt
+-rw-r--r--   0 ancientevil   (501) staff       (20)       44 2024-04-30 20:17:11.000000 vrf-1.0.6/vrf.egg-info/requires.txt
+-rw-r--r--   0 ancientevil   (501) staff       (20)       13 2024-04-30 20:17:11.000000 vrf-1.0.6/vrf.egg-info/top_level.txt
+drwxr-xr-x   0 ancientevil   (501) staff       (20)        0 2024-04-30 20:17:11.518736 vrf-1.0.6/vrf_py/
+-rw-r--r--   0 ancientevil   (501) staff       (20)    11855 2024-04-23 21:06:33.000000 vrf-1.0.6/vrf_py/VRF.py
+-rw-r--r--   0 ancientevil   (501) staff       (20)      117 2023-09-12 14:38:35.000000 vrf-1.0.6/vrf_py/__init__.py
+-rw-r--r--   0 ancientevil   (501) staff       (20)      808 2023-09-11 15:38:19.000000 vrf-1.0.6/vrf_py/error.py
+-rw-r--r--   0 ancientevil   (501) staff       (20)      774 2023-09-11 15:38:19.000000 vrf-1.0.6/vrf_py/log.py
```

### Comparing `vrf-1.0.4/README.md` & `vrf-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 # Verifiable Random Function
 VRF.py provides an implementation of a Verifiable Random Function (VRF) to ensure the randomness and fairness of a game. The script contains functions to generate seeds, proofs, and random values, and to verify the outcome of a game.
 
 
-![Coverage](https://img.shields.io/badge/VRF.py-Coverage:XX%-brightgreen.svg)
+![Coverage](https://img.shields.io/badge/VRF.py-Coverage:100%25-brightgreen.svg)
+
+## Demo
+
+
+https://github.com/0xlucyy/vrf/assets/109987865/5da41a5c-52d2-40d6-81f5-0eab4480fd3c
+
+
 
 
 # Table of Contents
 - [Verifiable Random Function](#verifiable-random-function)
 - [The Game](#the-game)
   - [generate_seed_salt_hash Function](#generate_seed_salt_hash-function)
   - [generate_beta_and_proof Function](#generate_beta_and_proof-function)
@@ -148,13 +155,20 @@
 
 
 ## Run
 - `git clone git@github.com:0xlucyfer/vrf.git`
 - `python3 -m venv venv`
 - `. venv/bin/activate`
 - `pip install -r requirements.txt`
-- Uncomment function `example_run` and `main` in VRF.py.
-- `python VRF.py`
+- Uncomment functions `example_run` and `main` in `vrf_py/VRF.py`.
+- `python vrf_py/VRF.py`
 
 
 ## Install
-- https://pypi.org/project/vrf/1.0.0/#description
+- https://pypi.org/project/vrf/1.0.4/
+- `pip install vrf==1.0.4`
+- `from vrf_py import new_game, verify`
+
+
+## Update Version
+- `python setup.py sdist bdist_wheel`
+- `twine upload --repository VRF_GAMING`
```

### Comparing `vrf-1.0.4/setup.py` & `vrf-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         encoding=kwargs.get('encoding', 'utf8')
     )
 
 install_dependencies = open_config_file('requirements.txt').read().splitlines()
 
 setup(
     name='vrf',
-    version='1.0.4',
+    version='1.0.6',
     author='lucyfer',
     description='VRF with ability to validate',
     packages=find_packages(),
     install_requires=install_dependencies,
     # entry_points={
     #     'console_scripts': [
     #         "test = vrf_py.VRF:func_name",
```

### Comparing `vrf-1.0.4/tests/test_generate_beta_and_proof.py` & `vrf-1.0.6/tests/test_generate_beta_and_proof.py`

 * *Files identical despite different names*

### Comparing `vrf-1.0.4/tests/test_generate_seed_salt_hash.py` & `vrf-1.0.6/tests/test_generate_seed_salt_hash.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Generated by CodiumAI
 import ecdsa
 import pytest
 from vrf_py.VRF import (
     generate_seed_salt_hash,
     generate_proof,
     generate_beta
 )
```

### Comparing `vrf-1.0.4/tests/test_integration.py` & `vrf-1.0.6/tests/test_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
   new_game,
   verify,
   ALGO,
   ITERATIONS
 )
 
 
-
 class TestIntegration(unittest.TestCase):
 
   def test_vrf_various_scenarios(self):
     """
     Test the VRF system end-to-end for various scenarios to ensure
     consistent and correct behavior across different inputs.
 
@@ -65,12 +64,12 @@
       # Step 2b: Generate a private key for signing.
       sk = ecdsa.SigningKey.generate(curve=ecdsa.SECP256k1)
 
       # Step 2c: Initialize a new game
       seed, seed_hash, salt, beta, proof, bullet_index, bullet_index_hash, public_key_pem = new_game(scenario['revolver_size'], sk, alpha)
 
       # Step 2d: Verify the outcome of the game using the provided values.
-      proof_validity, derived_bullet_index_hash = verify(public_key_pem, seed_hash, salt, proof, bullet_index_hash, alpha, scenario['revolver_size'])
+      proof_validity, derived_bullet_index_hash = verify(public_key_pem, seed_hash, salt, proof, bullet_index_hash, alpha, scenario['revolver_size'], beta)
 
       # Step 2e: Assert that the verification result is True.
       self.assertTrue(proof_validity, True)
       self.assertEqual(derived_bullet_index_hash, bullet_index_hash)
```

### Comparing `vrf-1.0.4/tests/test_new_game.py` & `vrf-1.0.6/tests/test_new_game.py`

 * *Files identical despite different names*

### Comparing `vrf-1.0.4/tests/test_verify.py` & `vrf-1.0.6/tests/test_verify.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,19 +22,29 @@
 -----END PUBLIC KEY-----'''
     seed_hash = "76bc35a3dae9c528e44cb9b7c8af1370d252335268ecd4b4d6b79c3b5600cc2d6fd6092cc59e333f12c91e603762e5a4d59feb5d985f9e1feffca0a5bc356ac1"
     salt = "d472f94b879c05d1498c08b7b5e774ace2de515a5f74b1731fde6820c668d28f"
     proof = bytes.fromhex('a60ffb4d2c36655d78e48c41d9887f8b8e29112a5a4f9e001d69a7aeaa72a00ba4acb71eb3d397e8017bd843591c6adc9f4397d92904ac9886e9a1067089efb2')
     bullet_index_hash = 'e9a9cc80a4e3883c16d3a28bf832cd80927d18e26777e058982126addfcd5dcf'
     alpha = b'1694274217300003000060000300006000030000'
     revolver_chambers = 41
-    proof_validity, derived_bullet_index_hash = verify(public_key, seed_hash, salt, proof, bullet_index_hash, alpha, revolver_chambers)
+    beta = '54f5063e16b06a6dd23727cec6d88d52a9e8f8a84b5f8c4cf1c94035b8316b3d'
+
+    proof_validity, derived_bullet_index_hash = verify(public_key,
+                                                       seed_hash,
+                                                       salt,
+                                                       proof,
+                                                       bullet_index_hash,
+                                                       alpha,
+                                                       revolver_chambers,
+                                                       beta)
 
     assert proof_validity == True
     assert derived_bullet_index_hash == bullet_index_hash
 
+
   # Tests that the function returns True when provided with a valid proof and a different set of valid inputs.
   def test_verify_valid_proof_with_different_inputs_same_pub_key(self):
     '''
     Tests the function with a different set of valid inputs but the same public key.
     '''
     public_key = b'''-----BEGIN PUBLIC KEY-----
 MFYwEAYHKoZIzj0CAQYFK4EEAAoDQgAED4BkWbqMmS/jxRQKC+xJVF2PeSwEx5g5
@@ -42,93 +52,140 @@
 -----END PUBLIC KEY-----'''
     seed_hash = "37dba05d813d44d52e6b6b9cf402e9b5948ef4e78f312647352016baa085bc5f1061b5c65a3e5d02f60b74df3e27e3eec0e9e09675b45751766fab1687b57593"
     salt = "bca580eeb2bc0605dc24d02d320f482e6293f86003aacfd2c23cf55c86b3b49e"
     proof = bytes.fromhex('bc738f603df0cf25a880c5c709e46346852ebc2f62a583474e0a52b7b4518bd75b51b3fcfe50c4a44768d0a8b15addde25780ef832695935d3624b0327504f0c')
     bullet_index_hash = '16a4abe5d7cfce33c117f09b836cab75e51824c954b61d159f9a391a1c4613b9'
     alpha = b'1694274772300003000060000300006000030000300003000030000'
     revolver_chambers = 22
-    proof_validity, derived_bullet_index_hash = verify(public_key, seed_hash, salt, proof, bullet_index_hash, alpha, revolver_chambers)
+    beta = '0aeb74b5b2c11a8f59b31034e198986d680128bb07c39801e1c77925af0f34bd'
+
+    proof_validity, derived_bullet_index_hash = verify(public_key,
+                                                       seed_hash,
+                                                       salt,
+                                                       proof,
+                                                       bullet_index_hash,
+                                                       alpha,
+                                                       revolver_chambers,
+                                                       beta)
 
     assert proof_validity == True
     assert derived_bullet_index_hash == bullet_index_hash
 
 
-  
   def test_verify_valid_proof_with_different_public_key(self):
     '''
     Tests the function with a different valid public key.
     '''
     public_key = b'''-----BEGIN PUBLIC KEY-----
 MFYwEAYHKoZIzj0CAQYFK4EEAAoDQgAE1DJ2RmUmTwg07t9w83Q5m4vNhqDqu2Xe
 c0S1sJX01clxnSv3PsPI7g9Lujsc5+87q6NJ05eljd8R6jMRJV7nlQ==
 -----END PUBLIC KEY-----'''
     seed_hash = "fdb3b943e81b4a7d312515ff871cf1638d12679a0b855bdaaa6f7c8263f574e60e6a87a0c079d27ccea50ba1ba0d632273bc01232c3ec685d63b07590733e039"
     salt = "96639d08641417aebe1b68912ab08c10da412bf57c126ded4adaeec0f5230d86"
     proof = bytes.fromhex('f58c633a2a947ed31c6143f5d73c6bec82e22081ba5536c52328fe8f93b320c2c5209de1f5dc0d6b0ad28b28fe712fcc88264e06ab14736f2bfc67106ed9b46d')
     bullet_index_hash = 'f06b63ab52e55bd1eb19824eca3882567a867a4166d6472e87dc4411f7aeeb3b'
     alpha = b'1694274952300003000060000300006000030000'
     revolver_chambers = 41
-    proof_validity, derived_bullet_index_hash = verify(public_key, seed_hash, salt, proof, bullet_index_hash, alpha, revolver_chambers)
+    beta = '91848bd9f29ce163cdac8999ec7278d7bc19c9fbe808e5184614588c298109a4'
+
+    proof_validity, derived_bullet_index_hash = verify(public_key,
+                                                       seed_hash,
+                                                       salt,
+                                                       proof,
+                                                       bullet_index_hash,
+                                                       alpha,
+                                                       revolver_chambers,
+                                                       beta)
 
     assert proof_validity == True
     assert derived_bullet_index_hash == bullet_index_hash
 
+
   def test_valid_verify_with_min_chambers(self):
     '''
     Tests the function with the minimum number of revolver chambers.
     '''
     public_key = b'''-----BEGIN PUBLIC KEY-----
 MFYwEAYHKoZIzj0CAQYFK4EEAAoDQgAE1DJ2RmUmTwg07t9w83Q5m4vNhqDqu2Xe
 c0S1sJX01clxnSv3PsPI7g9Lujsc5+87q6NJ05eljd8R6jMRJV7nlQ==
 -----END PUBLIC KEY-----'''
     seed_hash = "a39a775cb04afadbe7eaf95519ddb87d96c6883e341bfe46726692a46f3c96fba05ba619da7d22644feaae7103d2d0159243ec34a8e37e4a40c8dfb6e8d5708b"
     salt = "6ebc24ff40dc186c42d6b7fd71d1d844c1f5cafd2811633d044f5e188a1ba68e"
     proof = bytes.fromhex('8e1677fe5ea4c5a3e4980c92d5774820230c0d2743846888e52f42019001bea05f22739ab3f454c5f42181fc7eb7c9575ad57986c7963e275d00ea2d5e57320a')
     bullet_index_hash = 'afaf2081f389d32c34198693134350ab0373b92f224b5dee7b662e53f1cf558e'
     alpha = b'16942763713000030000'
     revolver_chambers = 2
-    proof_validity, derived_bullet_index_hash = verify(public_key, seed_hash, salt, proof, bullet_index_hash, alpha, revolver_chambers)
+    beta = '947f71a558be2612dafa457751bf2a9ae13031416df98c3e42f6c72220764492'
+
+    proof_validity, derived_bullet_index_hash = verify(public_key,
+                                                       seed_hash,
+                                                       salt,
+                                                       proof,
+                                                       bullet_index_hash,
+                                                       alpha,
+                                                       revolver_chambers,
+                                                       beta)
 
     assert proof_validity == True
     assert derived_bullet_index_hash == bullet_index_hash
 
+
   def test_valid_verify_with_small_chambers(self):
     '''
     Tests the function with a small number of revolver chambers.
     '''
     public_key = b'''-----BEGIN PUBLIC KEY-----
 MFYwEAYHKoZIzj0CAQYFK4EEAAoDQgAE1DJ2RmUmTwg07t9w83Q5m4vNhqDqu2Xe
 c0S1sJX01clxnSv3PsPI7g9Lujsc5+87q6NJ05eljd8R6jMRJV7nlQ==
 -----END PUBLIC KEY-----'''
     seed_hash = "fadfaa2797582565101054fd6859ab3666fd5ea981280726978b241bd47aba23c87c6a37234f9d3ebfff6c16707985ccf21b8f09b8e8608b964efc574dda014a"
     salt = "1232cd7e0920e12ffd22a96f2d2451ca9fb1fe58529fdb9265b6de516d7cd181"
     proof = bytes.fromhex('1ac6de4471e78bb1ef363b34d36d39b6b0989a834110f1e256a0ecc499446e18f1d3466ba037e7f4443ce3cae2eb9179af93da321b9563743c9ebc1ec86ee0d1')
     bullet_index_hash = '810e2393563512d3f794a69710ec5d750fd83920f68135d0916171fb77157657'
     alpha = b'1694276451300003000030000'
     revolver_chambers = 3
-    proof_validity, derived_bullet_index_hash = verify(public_key, seed_hash, salt, proof, bullet_index_hash, alpha, revolver_chambers)
+    beta = 'e311428f2a46a4f66f57b7e6cb3b7da829eb2eb4f2739105dd693f85d5ae4a13'
+
+    proof_validity, derived_bullet_index_hash = verify(public_key,
+                                                       seed_hash,
+                                                       salt,
+                                                       proof,
+                                                       bullet_index_hash,
+                                                       alpha,
+                                                       revolver_chambers,
+                                                       beta)
 
     assert proof_validity == True
     assert derived_bullet_index_hash == bullet_index_hash
 
+
   def test_valid_verify_with_same_chambers_and_bets(self):
     '''
     Tests the function with the same number of revolver chambers and bets.
     '''
     public_key = b'''-----BEGIN PUBLIC KEY-----
 MFYwEAYHKoZIzj0CAQYFK4EEAAoDQgAE1DJ2RmUmTwg07t9w83Q5m4vNhqDqu2Xe
 c0S1sJX01clxnSv3PsPI7g9Lujsc5+87q6NJ05eljd8R6jMRJV7nlQ==
 -----END PUBLIC KEY-----'''
     seed_hash = "6d52ffbb859f1d540e9529931ec053de9ffcb7b4c885e759a361d5f0a0c1f3f6677cda1de5b43ab0e56ca337759c86067735609b5bd5e59db5d37a42eb510b82"
     salt = "f371978c5b38a62e43043865b3f114d46af4422042821ecccab5e06fdad66587"
     proof = bytes.fromhex('1fb221216ed9e6c0e03281ded4f6edc51030834696788f24a3639946eed616de97b97d32dcd317acabbbfc759d83316ca6358a1d477b2480cf63d2fc8c6b1f24')
     bullet_index_hash = 'd2d7c65c5e89f56976deddc798f9da9f4f3bdff31a47114c5acc550af351256c'
     alpha = b'1694276581300003000030000'
     revolver_chambers = 3
-    proof_validity, derived_bullet_index_hash = verify(public_key, seed_hash, salt, proof, bullet_index_hash, alpha, revolver_chambers)
+    beta = 'd7340d5f541358eb77ff7eef968e5db1d68032edb9e39c8c2b6bda6b2f15911d'
+
+    proof_validity, derived_bullet_index_hash = verify(public_key,
+                                                       seed_hash,
+                                                       salt,
+                                                       proof,
+                                                       bullet_index_hash,
+                                                       alpha,
+                                                       revolver_chambers,
+                                                       beta)
 
     assert proof_validity == True
     assert derived_bullet_index_hash == bullet_index_hash
 
   def test_valid_verify_with_same_chambers_and_diff_bets(self):
     '''
     Tests the function with the same number of revolver chambers but different bets.
@@ -139,15 +196,24 @@
 -----END PUBLIC KEY-----'''
     seed_hash = "d51683bec03aaa13c3f9ec9eebc6eebec33e8642a483283e0fada0a8f73038435e5a8eb4f09a272f31c034f80114ba9bcdc342720dfaac2af5be0ff46526fef9"
     salt = "9c797ee4a9fb961c95ec1e2fe4ed9dd6209e3f3d1716fea33f1cd9715e310104"
     proof = bytes.fromhex('4a8fba40d6ef41a27d94e6c4ca13cd4dfa7bc9f9a4baadcc3c1854c8817c26269026f21295bf01916aeebaef859cd2c397cdb324a6af77d042e9a8680a960b7f')
     bullet_index_hash = '22b943c3736d5ebbb9e29ac735448f9e384d7fc0229ceec2e19fbbd01da52681'
     alpha = b'1694276755200020004000'
     revolver_chambers = 3
-    proof_validity, derived_bullet_index_hash = verify(public_key, seed_hash, salt, proof, bullet_index_hash, alpha, revolver_chambers)
+    beta = '0642433d6f7eaa69f3acab82269857f4a6f49a9c83b23452c3c31395df577240'
+
+    proof_validity, derived_bullet_index_hash = verify(public_key,
+                                                       seed_hash,
+                                                       salt,
+                                                       proof,
+                                                       bullet_index_hash,
+                                                       alpha,
+                                                       revolver_chambers,
+                                                       beta)
 
     assert proof_validity == True
     assert derived_bullet_index_hash == bullet_index_hash
 
   def test_invalid_revolver_size(self):
     '''
     Tests the function where the revolver chambers is incorrect.
@@ -158,38 +224,58 @@
 -----END PUBLIC KEY-----'''
     seed_hash = "fdb3b943e81b4a7d312515ff871cf1638d12679a0b855bdaaa6f7c8263f574e60e6a87a0c079d27ccea50ba1ba0d632273bc01232c3ec685d63b07590733e039"
     salt = "96639d08641417aebe1b68912ab08c10da412bf57c126ded4adaeec0f5230d86"
     proof = bytes.fromhex('f58c633a2a947ed31c6143f5d73c6bec82e22081ba5536c52328fe8f93b320c2c5209de1f5dc0d6b0ad28b28fe712fcc88264e06ab14736f2bfc67106ed9b46d')
     bullet_index_hash = None
     alpha = b'1694274952300003000060000300006000030000'
     revolver_chambers = 42 # Wrong, correct value is 41
-    proof_validity, derived_bullet_index_hash = verify(public_key, seed_hash, salt, proof, bullet_index_hash, alpha, revolver_chambers)
+    beta = '91848bd9f29ce163cdac8999ec7278d7bc19c9fbe808e5184614588c298109a4'
+
+    proof_validity, derived_bullet_index_hash = verify(public_key,
+                                                       seed_hash,
+                                                       salt,
+                                                       proof,
+                                                       bullet_index_hash,
+                                                       alpha,
+                                                       revolver_chambers,
+                                                       beta)
 
     assert proof_validity == False
     assert derived_bullet_index_hash == bullet_index_hash
 
+
   def test_invalid_alpha(self):
     '''
     Tests the function where the alpha is incorrect.
     '''
     public_key = b'''-----BEGIN PUBLIC KEY-----
 MFYwEAYHKoZIzj0CAQYFK4EEAAoDQgAE1DJ2RmUmTwg07t9w83Q5m4vNhqDqu2Xe
 c0S1sJX01clxnSv3PsPI7g9Lujsc5+87q6NJ05eljd8R6jMRJV7nlQ==
 -----END PUBLIC KEY-----'''
     seed_hash = "fdb3b943e81b4a7d312515ff871cf1638d12679a0b855bdaaa6f7c8263f574e60e6a87a0c079d27ccea50ba1ba0d632273bc01232c3ec685d63b07590733e039"
     salt = "96639d08641417aebe1b68912ab08c10da412bf57c126ded4adaeec0f5230d86"
     proof = bytes.fromhex('f58c633a2a947ed31c6143f5d73c6bec82e22081ba5536c52328fe8f93b320c2c5209de1f5dc0d6b0ad28b28fe712fcc88264e06ab14736f2bfc67106ed9b46d')
     bullet_index_hash = None
     alpha = b'16942749523000030000600003000060000' # Append '30000' for real value.
     revolver_chambers = 41
-    proof_validity, derived_bullet_index_hash = verify(public_key, seed_hash, salt, proof, bullet_index_hash, alpha, revolver_chambers)
+    beta = '947f71a558be2612dafa457751bf2a9ae13031416df98c3e42f6c72220764492'
+
+    proof_validity, derived_bullet_index_hash = verify(public_key,
+                                                       seed_hash,
+                                                       salt,
+                                                       proof,
+                                                       bullet_index_hash,
+                                                       alpha,
+                                                       revolver_chambers,
+                                                       beta)
 
     assert proof_validity == False
     assert derived_bullet_index_hash == bullet_index_hash
 
+
   def test_invalid_proof(self):
     '''
     Tests the function where the proof is incorrect.
     '''
     public_key = b'''-----BEGIN PUBLIC KEY-----
 MFYwEAYHKoZIzj0CAQYFK4EEAAoDQgAE1DJ2RmUmTwg07t9w83Q5m4vNhqDqu2Xe
 c0S1sJX01clxnSv3PsPI7g9Lujsc5+87q6NJ05eljd8R6jMRJV7nlQ==
@@ -197,19 +283,29 @@
     seed_hash = "fdb3b943e81b4a7d312515ff871cf1638d12679a0b855bdaaa6f7c8263f574e60e6a87a0c079d27ccea50ba1ba0d632273bc01232c3ec685d63b07590733e039"
     salt = "96639d08641417aebe1b68912ab08c10da412bf57c126ded4adaeec0f5230d86"
     # real_proof = bytes.fromhex('f58c633a2a947ed31c6143f5d73c6bec82e22081ba5536c52328fe8f93b320c2c5209de1f5dc0d6b0ad28b28fe712fcc88264e06ab14736f2bfc67106ed9b46d')
     proof = bytes.fromhex('f68c633a2a947ed31c6143f5d73c6bec82e22081ba5536c52328fe8f93b320c2c5209de1f5dc0d6b0ad28b28fe712fcc88264e06ab14736f2bfc67106ed9b46d')
     bullet_index_hash = None
     alpha = b'1694274952300003000060000300006000030000'
     revolver_chambers = 41
-    proof_validity, derived_bullet_index_hash = verify(public_key, seed_hash, salt, proof, bullet_index_hash, alpha, revolver_chambers)
+    beta = '947f71a558be2612dafa457751bf2a9ae13031416df98c3e42f6c72220764492'
+
+    proof_validity, derived_bullet_index_hash = verify(public_key,
+                                                       seed_hash,
+                                                       salt,
+                                                       proof,
+                                                       bullet_index_hash,
+                                                       alpha,
+                                                       revolver_chambers,
+                                                       beta)
 
     assert proof_validity == False
     assert derived_bullet_index_hash == bullet_index_hash
 
+
   def test_invalid_salt(self):
     '''
     Tests the function where the salt is incorrect.
     '''
     public_key = b'''-----BEGIN PUBLIC KEY-----
 MFYwEAYHKoZIzj0CAQYFK4EEAAoDQgAE1DJ2RmUmTwg07t9w83Q5m4vNhqDqu2Xe
 c0S1sJX01clxnSv3PsPI7g9Lujsc5+87q6NJ05eljd8R6jMRJV7nlQ==
@@ -217,19 +313,29 @@
     seed_hash = "fdb3b943e81b4a7d312515ff871cf1638d12679a0b855bdaaa6f7c8263f574e60e6a87a0c079d27ccea50ba1ba0d632273bc01232c3ec685d63b07590733e039"
     # real_salt = "96639d08641417aebe1b68912ab08c10da412bf57c126ded4adaeec0f5230d86"
     salt = "86639d08641417aebe1b68912ab08c10da412bf57c126ded4adaeec0f5230d86"
     proof = bytes.fromhex('f58c633a2a947ed31c6143f5d73c6bec82e22081ba5536c52328fe8f93b320c2c5209de1f5dc0d6b0ad28b28fe712fcc88264e06ab14736f2bfc67106ed9b46d')
     bullet_index_hash = None
     alpha = b'1694274952300003000060000300006000030000'
     revolver_chambers = 41
-    proof_validity, derived_bullet_index_hash = verify(public_key, seed_hash, salt, proof, bullet_index_hash, alpha, revolver_chambers)
+    beta = '947f71a558be2612dafa457751bf2a9ae13031416df98c3e42f6c72220764492'
+
+    proof_validity, derived_bullet_index_hash = verify(public_key,
+                                                       seed_hash,
+                                                       salt,
+                                                       proof,
+                                                       bullet_index_hash,
+                                                       alpha,
+                                                       revolver_chambers,
+                                                       beta)
 
     assert proof_validity == False
     assert derived_bullet_index_hash == bullet_index_hash
 
+
   def test_invalid_seed_hash(self):
     '''
     Tests the function where the seed hash is incorrect.
     '''
     public_key = b'''-----BEGIN PUBLIC KEY-----
 MFYwEAYHKoZIzj0CAQYFK4EEAAoDQgAE1DJ2RmUmTwg07t9w83Q5m4vNhqDqu2Xe
 c0S1sJX01clxnSv3PsPI7g9Lujsc5+87q6NJ05eljd8R6jMRJV7nlQ==
@@ -237,15 +343,24 @@
     # real_seed_hash = "fdb3b943e81b4a7d312515ff871cf1638d12679a0b855bdaaa6f7c8263f574e60e6a87a0c079d27ccea50ba1ba0d632273bc01232c3ec685d63b07590733e039"
     seed_hash = "fdb4b943e81b4a7d312515ff871cf1638d12679a0b855bdaaa6f7c8263f574e60e6a87a0c079d27ccea50ba1ba0d632273bc01232c3ec685d63b07590733e039"
     salt = "96639d08641417aebe1b68912ab08c10da412bf57c126ded4adaeec0f5230d86"
     proof = bytes.fromhex('f58c633a2a947ed31c6143f5d73c6bec82e22081ba5536c52328fe8f93b320c2c5209de1f5dc0d6b0ad28b28fe712fcc88264e06ab14736f2bfc67106ed9b46d')
     bullet_index_hash = None
     alpha = b'1694274952300003000060000300006000030000'
     revolver_chambers = 41
-    proof_validity, derived_bullet_index_hash = verify(public_key, seed_hash, salt, proof, bullet_index_hash, alpha, revolver_chambers)
+    beta = '3c120f9842793e5d8ac3e2a4b61b2118059aa0343004ed934bbc6b0ff9834fe1'
+
+    proof_validity, derived_bullet_index_hash = verify(public_key,
+                                                       seed_hash,
+                                                       salt,
+                                                       proof,
+                                                       bullet_index_hash,
+                                                       alpha,
+                                                       revolver_chambers,
+                                                       beta)
 
     assert proof_validity == False
     assert derived_bullet_index_hash == bullet_index_hash
 
   
   def test_invalid_pub_key(self):
     '''
@@ -261,15 +376,24 @@
 -----END PUBLIC KEY-----'''
     seed_hash = "fdb3b943e81b4a7d312515ff871cf1638d12679a0b855bdaaa6f7c8263f574e60e6a87a0c079d27ccea50ba1ba0d632273bc01232c3ec685d63b07590733e039"
     salt = "96639d08641417aebe1b68912ab08c10da412bf57c126ded4adaeec0f5230d86"
     proof = bytes.fromhex('f58c633a2a947ed31c6143f5d73c6bec82e22081ba5536c52328fe8f93b320c2c5209de1f5dc0d6b0ad28b28fe712fcc88264e06ab14736f2bfc67106ed9b46d')
     bullet_index_hash = None
     alpha = b'1694274952300003000060000300006000030000'
     revolver_chambers = 41
-    proof_validity, derived_bullet_index_hash = verify(public_key, seed_hash, salt, proof, bullet_index_hash, alpha, revolver_chambers)
+    beta = '947f71a558be2612dafa457751bf2a9ae13031416df98c3e42f6c72220764492'
+
+    proof_validity, derived_bullet_index_hash = verify(public_key,
+                                                       seed_hash,
+                                                       salt,
+                                                       proof,
+                                                       bullet_index_hash,
+                                                       alpha,
+                                                       revolver_chambers,
+                                                       beta)
 
     assert proof_validity == False
     assert derived_bullet_index_hash == bullet_index_hash
 
 
   @patch('ecdsa.keys.VerifyingKey.verify', side_effect=InterruptedError)
   def test_vk_verify_exception(self, mocked_sig):
@@ -280,35 +404,52 @@
     # real_seed_hash = "fdb3b943e81b4a7d312515ff871cf1638d12679a0b855bdaaa6f7c8263f574e60e6a87a0c079d27ccea50ba1ba0d632273bc01232c3ec685d63b07590733e039"
     seed_hash = "fdb4b943e81b4a7d312515ff871cf1638d12679a0b855bdaaa6f7c8263f574e60e6a87a0c079d27ccea50ba1ba0d632273bc01232c3ec685d63b07590733e039"
     salt = "96639d08641417aebe1b68912ab08c10da412bf57c126ded4adaeec0f5230d86"
     proof = bytes.fromhex('f58c633a2a947ed31c6143f5d73c6bec82e22081ba5536c52328fe8f93b320c2c5209de1f5dc0d6b0ad28b28fe712fcc88264e06ab14736f2bfc67106ed9b46d')
     bullet_index_hash = None
     alpha = b'1694274952300003000060000300006000030000'
     revolver_chambers = 41
+    beta = '575bf0b4da9be711155c744cd2eafda2bb91c642d355e66a3f20a3ca6b3bd54d'
 
-    proof_validity, derived_bullet_index_hash = verify(public_key, seed_hash, salt, proof, bullet_index_hash, alpha, revolver_chambers)
+    proof_validity, derived_bullet_index_hash = verify(public_key,
+                                                       seed_hash,
+                                                       salt,
+                                                       proof,
+                                                       bullet_index_hash,
+                                                       alpha,
+                                                       revolver_chambers,
+                                                       beta)
     
     assert proof_validity == False
     assert derived_bullet_index_hash == bullet_index_hash
 
+
   @patch('ecdsa.keys.VerifyingKey.verify', side_effect=ValueError)
   def test_vk_verify_exception_value_error(self, mocked_sig):
     public_key = b'''-----BEGIN PUBLIC KEY-----
 MFYwEAYHKoZIzj0CAQYFK4EEAAoDQgAE1DJ2RmUmTwg07t9w83Q5m4vNhqDqu2Xe
 c0S1sJX01clxnSv3PsPI7g9Lujsc5+87q6NJ05eljd8R6jMRJV7nlQ==
 -----END PUBLIC KEY-----'''
     # real_seed_hash = "fdb3b943e81b4a7d312515ff871cf1638d12679a0b855bdaaa6f7c8263f574e60e6a87a0c079d27ccea50ba1ba0d632273bc01232c3ec685d63b07590733e039"
     seed_hash = "fdb4b943e81b4a7d312515ff871cf1638d12679a0b855bdaaa6f7c8263f574e60e6a87a0c079d27ccea50ba1ba0d632273bc01232c3ec685d63b07590733e039"
     salt = "96639d08641417aebe1b68912ab08c10da412bf57c126ded4adaeec0f5230d86"
     proof = bytes.fromhex('f58c633a2a947ed31c6143f5d73c6bec82e22081ba5536c52328fe8f93b320c2c5209de1f5dc0d6b0ad28b28fe712fcc88264e06ab14736f2bfc67106ed9b46d')
     bullet_index_hash = None
     alpha = b'1694274952300003000060000300006000030000'
     revolver_chambers = 41
+    beta = '947f71a558be2612dafa457751bf2a9ae13031416df98c3e42f6c72220764492'
 
-    proof_validity, derived_bullet_index_hash = verify(public_key, seed_hash, salt, proof, bullet_index_hash, alpha, revolver_chambers)
+    proof_validity, derived_bullet_index_hash = verify(public_key,
+                                                       seed_hash,
+                                                       salt,
+                                                       proof,
+                                                       bullet_index_hash,
+                                                       alpha,
+                                                       revolver_chambers,
+                                                       beta)
     
     assert proof_validity == False
     assert derived_bullet_index_hash == bullet_index_hash
 
   
   @patch('ecdsa.keys.VerifyingKey.verify', return_valud=True)
   def test_happy_path_not_successful(self, mocked_sig):
@@ -319,12 +460,50 @@
     # real_seed_hash = "fdb3b943e81b4a7d312515ff871cf1638d12679a0b855bdaaa6f7c8263f574e60e6a87a0c079d27ccea50ba1ba0d632273bc01232c3ec685d63b07590733e039"
     seed_hash = "fdb4b943e81b4a7d312515ff871cf1638d12679a0b855bdaaa6f7c8263f574e60e6a87a0c079d27ccea50ba1ba0d632273bc01232c3ec685d63b07590733e039"
     salt = "96639d08641417aebe1b68912ab08c10da412bf57c126ded4adaeec0f5230d86"
     proof = bytes.fromhex('f58c633a2a947ed31c6143f5d73c6bec82e22081ba5536c52328fe8f93b320c2c5209de1f5dc0d6b0ad28b28fe712fcc88264e06ab14736f2bfc67106ed9b46d')
     bullet_index_hash = 'FAKE'
     alpha = b'1694274952300003000060000300006000030000'
     revolver_chambers = 41
+    beta = '947f71a558be2612dafa457751bf2a9ae13031416df98c3e42f6c72220764492'
 
-    proof_validity, derived_bullet_index_hash = verify(public_key, seed_hash, salt, proof, bullet_index_hash, alpha, revolver_chambers)
+    proof_validity, derived_bullet_index_hash = verify(public_key,
+                                                       seed_hash,
+                                                       salt,
+                                                       proof,
+                                                       bullet_index_hash,
+                                                       alpha,
+                                                       revolver_chambers,
+                                                       beta)
     
     assert proof_validity == False
-    assert 'FAKE' == bullet_index_hash
+    assert derived_bullet_index_hash == None
+
+
+  def test_invalid_beta(self):
+    '''
+    Tests the function with the same number of revolver chambers but different bets.
+    '''
+    public_key = b'''-----BEGIN PUBLIC KEY-----
+MFYwEAYHKoZIzj0CAQYFK4EEAAoDQgAE1DJ2RmUmTwg07t9w83Q5m4vNhqDqu2Xe
+c0S1sJX01clxnSv3PsPI7g9Lujsc5+87q6NJ05eljd8R6jMRJV7nlQ==
+-----END PUBLIC KEY-----'''
+    seed_hash = "d51683bec03aaa13c3f9ec9eebc6eebec33e8642a483283e0fada0a8f73038435e5a8eb4f09a272f31c034f80114ba9bcdc342720dfaac2af5be0ff46526fef9"
+    salt = "9c797ee4a9fb961c95ec1e2fe4ed9dd6209e3f3d1716fea33f1cd9715e310104"
+    proof = bytes.fromhex('4a8fba40d6ef41a27d94e6c4ca13cd4dfa7bc9f9a4baadcc3c1854c8817c26269026f21295bf01916aeebaef859cd2c397cdb324a6af77d042e9a8680a960b7f')
+    bullet_index_hash = '22b943c3736d5ebbb9e29ac735448f9e384d7fc0229ceec2e19fbbd01da52681'
+    alpha = b'1694276755200020004000'
+    revolver_chambers = 3
+    # real_beta = '0642433d6f7eaa69f3acab82269857f4a6f49a9c83b23452c3c31395df577240'
+    beta = '1234567890'
+
+    proof_validity, derived_bullet_index_hash = verify(public_key,
+                                                       seed_hash,
+                                                       salt,
+                                                       proof,
+                                                       bullet_index_hash,
+                                                       alpha,
+                                                       revolver_chambers,
+                                                       beta)
+
+    assert proof_validity == False
+    assert derived_bullet_index_hash == None
```

### Comparing `vrf-1.0.4/vrf_py/VRF.py` & `vrf-1.0.6/vrf_py/VRF.py`

 * *Files 14% similar despite different names*

```diff
@@ -100,17 +100,18 @@
     if not isinstance(salt, str):
         raise ValueError("salt must be a string")
     if not isinstance(seed_hash, str):
         raise ValueError("seed_hash must be a string")
 
     try:
         beta = hashlib.pbkdf2_hmac(
-            ALGO, 
+            ALGO,
             ((seed_hash + salt).encode() + proof),
-            salt.encode(), ITERATIONS
+            salt.encode(),
+            ITERATIONS
         ).hex()
         return beta
     except Exception as e:
         raise VerificationError('Failed to generate beta.') from e
 
 
 def generate_beta_and_proof(
@@ -212,116 +213,106 @@
     public_key_pem = private_key.verifying_key.to_pem()
 
     return seed, seed_hash, salt, beta, proof, bullet_index, bullet_index_hash, public_key_pem
 
 
 def verify(public_key: bytes, seed_hash: str, salt: str,
            proof: bytes, bullet_index_hash: str, alpha: bytes,
-           revolver_chambers: int) -> Union[bool, Tuple[bool, str]]:
+           revolver_chambers: int, beta: str) -> bool:
     """
-    Verify the integrity and authenticity of a game's
-    cryptographic parameters.
+    Verify the integrity of the game using the information published at the end of
+    the game and the information published at the beginning of the game.
 
     This function checks the validity of a provided proof
     using a public key and ensures that the derived bullet
     index hash matches the provided hash. It ensures that the
     game's outcome has not been tampered with and is verifiable.
 
     Args:
-        public_key (bytes): The public key in PEM format for verification.
-        seed_hash (str): Hashed value of the seed.
-        salt (str): A random string.
-        proof (bytes): A digital signature generated during the game initialization.
-        bullet_index_hash (str): A commitment of initial state of the game.
-        alpha (bytes): The input message.
-        revolver_chambers (int): The size of the revolver.
+        public_key (bytes): The public key in PEM format.
+        seed_hash (str): The hash of the randomly generated seed.
+        salt (str): The randomly generated salt used for hashing.
+        proof (bytes): The generated proof for the random number.
+        bullet_index_hash (str): The hash of the bullet index.
+        alpha (bytes): The input message to the VRF.
+        revolver_chambers (int): The number of chambers in the revolver.
+        beta (str): The randomly generated number in hex format.
 
     Returns:
-        Union[bool, Tuple[bool, str]]:
-            - False if any verification step fails.
-            - (proof_validity (bool), derived_bullet_index_hash (str)): A tuple 
+       Union[Tuple[bool, None], Tuple[bool, str]]:
+            - (proof_validity (bool), derived_bullet_index_hash (str)): A tuple
                 containing the validity of the proof and the derived bullet
                 index hash if all verification steps pass.
     """
     try:
-        '''
-        1a. Creating a verifying key object (vk) from public_key.
-        1a. `from_pem` is used to read public_key which is in Privacy
-            Enhanced Mail format.
-        1b. Using verifying key (vk) to verify the provided digital
-            signature (proof).
-        1b. The verify method checks if the proof is a valid signature 
-            with the message alpha using a public key (vk).
-        1c. If verification process does not raise any exceptions
-            (meaning the signature is valid), then the variable
-            proof_validity is set to True. This means that the
-            provided proof is a valid signature for the message
-            alpha, using the given public key.
-        '''
+        # Verify the proof using the public key and alpha
         vk = ecdsa.VerifyingKey.from_pem(public_key)
         vk.verify(proof, alpha, hashfunc=hashlib.sha256)
-        proof_validity = True
+
+        # Verify the beta value by generating it from the proof, salt, and seed_hash
+        derived_beta = generate_beta(proof, salt, seed_hash)
+
+        if derived_beta != beta:
+            logger.error("Beta value verification failed.")
+            return False, None
+
+        # Get determinisitc beta, get bullet index, get hash of index.
+        bullet_index = int(beta, 16) % revolver_chambers
+        derived_bullet_index_hash = hashlib.pbkdf2_hmac(
+            ALGO,
+            (str(bullet_index) + salt + seed_hash).encode(),
+            salt.encode(),
+            ITERATIONS
+        ).hex()
+
+        if derived_bullet_index_hash != bullet_index_hash:
+            logger.error("Bullet index verification failed.")
+            return False, None
+
+        return True, derived_bullet_index_hash
     except (ecdsa.keys.BadSignatureError, ecdsa.errors.MalformedPointError, ValueError) as error:
-        logger.error(f'1. Verification of the proof failed: {error}')
+        logger.error(f"Verification failed: {error}")
         return False, None
     except Exception as error:
-        logger.error(f'2. Verification of the proof failed: {error}')
+        logger.error(f"Verification failed: {error}")
         return False, None
 
-    # Get determinisitc beta, get bullet index, get hash of index.
-    beta = generate_beta(proof, salt, seed_hash)
-    bullet_index = int(beta, 16) % revolver_chambers
-    derived_bullet_index_hash = hashlib.pbkdf2_hmac(
-        ALGO,
-        (str(bullet_index) + salt + seed_hash).encode(),
-        salt.encode(),
-        ITERATIONS
-    ).hex()
-
-    # Ensure derived hash is equal to new_game commit.
-    if derived_bullet_index_hash == bullet_index_hash:
-        return proof_validity, derived_bullet_index_hash
-    return False, None
 
+# def example_run():
+#     revolver_chambers = 20
+#     bets = [30000, 30000, 60000, 30000, 60000]
+
+#     sk = ecdsa.SigningKey.generate(curve=ecdsa.SECP256k1)
+#     logger.info(f'Generated a new secret key.\n')
+#     # while True:
+#     #     import pdb;pdb.set_trace()
+#     revolver_chambers += 1
+#     bets.append(30000)
+#     logger.info(f'Revolver Size): {revolver_chambers}\n')
+#     logger.info(f'Bets): {bets}\n')
+
+#     timestamp = str(int(time.time()))
+#     alpha_raw = (timestamp + ''.join(map(str, bets)))
+#     alpha = alpha_raw.encode()
+#     logger.info(f'Alpha_Raw (Timestampe + Bets): {alpha_raw}')
+#     logger.info(f'Alpha (Input Message): {alpha}\n')
 
-
-def example_run():
-    revolver_chambers = 20
-    bets = [30000, 30000, 60000, 30000, 60000]
-
-    sk = ecdsa.SigningKey.generate(curve=ecdsa.SECP256k1)
-    logger.info(f'Generated a new secret key.\n')
-    # while True:
-    #     revolver_chambers += 1
-    #     bets.append(30000)
-    logger.info(f'Revolver Size): {revolver_chambers}\n')
-    logger.info(f'Bets): {bets}\n')
-
-    timestamp = str(int(time.time()))
-    alpha_raw = (timestamp + ''.join(map(str, bets)))
-    alpha = alpha_raw.encode()
-    logger.info(f'Alpha_Raw (Timestampe + Bets): {alpha_raw}')
-    logger.info(f'Alpha (Input Message): {alpha}\n')
-
-    # sk = ecdsa.SigningKey.generate(curve=ecdsa.SECP256k1)
-    # logger.info(f'Generated a new secret key.\n')
+#     # sk = ecdsa.SigningKey.generate(curve=ecdsa.SECP256k1)
+#     # logger.info(f'Generated a new secret key.\n')
     
-    seed, seed_hash, salt, beta, proof, bullet_index, bullet_index_hash, public_key_pem = new_game(revolver_chambers, sk, alpha)
-    logger.info(f"Seed: {seed}")
-    logger.info(f"Seed Hash: {seed_hash}")
-    logger.info(f"Salt: {salt}")
-    logger.info(f'Beta: {beta}')
-    logger.info(f'Proof: {proof.hex()}')
-    logger.info(f'bullet_index: {bullet_index}')
-    logger.info(f"bullet_index_hash: {bullet_index_hash}")
-    logger.info(f'Public Key: {public_key_pem.decode()}\n')
-
-    # import pdb;pdb.set_trace()
-
-    proof_validity, derived_bullet_index_hash = verify(public_key_pem, seed_hash, salt, proof, bullet_index_hash, alpha, revolver_chambers)
-    logger.info(f'Actual Bullet Index Hash: {derived_bullet_index_hash}')
-    logger.info(f'Expected Bullet Index Hash: {bullet_index_hash}')
-    logger.info(f'Verification Result: {proof_validity}')
+#     seed, seed_hash, salt, beta, proof, bullet_index, bullet_index_hash, public_key_pem = new_game(revolver_chambers, sk, alpha)
+#     logger.info(f"Seed: {seed}")
+#     logger.info(f"Seed Hash: {seed_hash}")
+#     logger.info(f"Salt: {salt}")
+#     logger.info(f'Beta: {beta}')
+#     logger.info(f'Proof: {proof.hex()}')
+#     logger.info(f'bullet_index: {bullet_index}')
+#     logger.info(f"bullet_index_hash: {bullet_index_hash}")
+#     logger.info(f'Public Key: {public_key_pem.decode()}\n')
+    
+#     proof_validity, derived_bullet_index_hash = verify(public_key_pem, seed_hash, salt, proof, bullet_index_hash, alpha, revolver_chambers, beta)
+#     logger.info(f'Actual Bullet Index Hash: {derived_bullet_index_hash}')
+#     logger.info(f'Expected Bullet Index Hash: {bullet_index_hash}')
+#     logger.info(f'Verification Result: {proof_validity}')
 
 # if __name__ == '__main__':
-#     example_run()
-
+#     example_run()
```

### Comparing `vrf-1.0.4/vrf_py/error.py` & `vrf-1.0.6/vrf_py/error.py`

 * *Files identical despite different names*

### Comparing `vrf-1.0.4/vrf_py/log.py` & `vrf-1.0.6/vrf_py/log.py`

 * *Files identical despite different names*

