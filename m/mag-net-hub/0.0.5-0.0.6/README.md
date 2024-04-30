# Comparing `tmp/mag_net_hub-0.0.5.tar.gz` & `tmp/mag_net_hub-0.0.6.tar.gz`

## Comparing `mag_net_hub-0.0.5.tar` & `mag_net_hub-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,48 @@
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/requirements.txt
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/__init__.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/loss.py
--rw-r--r--   0        0        0    20707 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/paderborn.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/sydney.py
--rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_3C90_experiment_1b4d8_model_f3915868_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_3C92_experiment_ea1fe_model_72510647_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_3C94_experiment_56441_model_55693612_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_3C95_experiment_ad6ec_model_046383a5_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_3E6_experiment_a7817_model_a1035e58_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_3F4_experiment_c234d_model_2d43b97d_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44349 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_77_experiment_268ae_model_5b7c92ed_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44349 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_78_experiment_e5297_model_77fbd758_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44349 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_79_experiment_45989_model_7227af72_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_A_experiment_c9cfe_model_d893c778_p.pt
--rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_B_experiment_c9cfe_model_b6a920cc_p.pt
--rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_C_experiment_c9cfe_model_c1ced7b6_p.pt
--rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_D_experiment_c9cfe_model_11672810_p.pt
--rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_E_experiment_c9cfe_model_5ae50f9e_p.pt
--rw-r--r--   0        0        0    44502 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_ML95S_experiment_1c978_model_883a5d2f_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_N27_experiment_8b7f0_model_20954a2a_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_N30_experiment_5a78c_model_6bd86623_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_N49_experiment_27442_model_d6234a32_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_N87_experiment_985cb_model_d51b0f7e_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_T37_experiment_a084a_model_fb31325e_seed_0_fold_0.pt
--rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/tests/test_paderborn.py
--rw-r--r--   0        0        0  1524230 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/tests/test_files/unit_test_data_ploss_at_450kWpm3.csv
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/LICENSE
--rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/README.md
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 mag_net_hub-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/__init__.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/loss.py
+-rw-r--r--   0        0        0    20384 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/paderborn.py
+-rw-r--r--   0        0        0    14852 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/sydney.py
+-rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3C90_experiment_1b4d8_model_f3915868_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3C92_experiment_ea1fe_model_72510647_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3C94_experiment_56441_model_55693612_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3C95_experiment_ad6ec_model_046383a5_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3E6_experiment_a7817_model_a1035e58_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3F4_experiment_c234d_model_2d43b97d_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44349 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_77_experiment_268ae_model_5b7c92ed_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44349 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_78_experiment_e5297_model_77fbd758_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44349 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_79_experiment_45989_model_7227af72_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_A_experiment_c9cfe_model_d893c778_p.pt
+-rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_B_experiment_c9cfe_model_b6a920cc_p.pt
+-rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_C_experiment_c9cfe_model_c1ced7b6_p.pt
+-rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_D_experiment_c9cfe_model_11672810_p.pt
+-rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_E_experiment_c9cfe_model_5ae50f9e_p.pt
+-rw-r--r--   0        0        0    44502 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_ML95S_experiment_1c978_model_883a5d2f_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_N27_experiment_8b7f0_model_20954a2a_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_N30_experiment_5a78c_model_6bd86623_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_N49_experiment_27442_model_d6234a32_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_N87_experiment_985cb_model_d51b0f7e_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_T37_experiment_a084a_model_fb31325e_seed_0_fold_0.pt
+-rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/3C90.pt
+-rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/3C92.pt
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/3C94.pt
+-rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/3C95.pt
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/3E6.pt
+-rw-r--r--   0        0        0     6503 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/3F4.pt
+-rw-r--r--   0        0        0     6930 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/77.pt
+-rw-r--r--   0        0        0     6930 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/78.pt
+-rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/79.pt
+-rw-r--r--   0        0        0     6960 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/ML95S.pt
+-rw-r--r--   0        0        0     6503 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/N27.pt
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/N30.pt
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/N49.pt
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/N87.pt
+-rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/T37.pt
+-rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/tests/test_paderborn.py
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/tests/test_sydney.py
+-rw-r--r--   0        0        0  1524230 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/tests/test_files/unit_test_data_ploss_at_450kWpm3.csv
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/README.md
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/PKG-INFO
```

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/paderborn.py` & `mag_net_hub-0.0.6/src_py/magnethub/paderborn.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,21 +351,14 @@
                 case _:
                     raise ValueError(f"Expected b_seq to have either one or two dimensions, but is has {b_seq.ndim}.")
         case list() | tuple():
             b_seq = np.array(b_seq)
         case _:
             raise ValueError(f"Type of b_seq={type(b_seq)} nut supported. Please provide as np.ndarray or list")
 
-    # maybe resample b_seq to 1024 samples
-    if b_seq.shape[-1] != L:
-        actual_len = b_seq.shape[-1]
-        query_points = np.arange(L)
-        support_points = np.arange(actual_len) * L / actual_len
-        b_seq = np.row_stack([np.interp(query_points, support_points, b_seq[i]) for i in range(b_seq.shape[0])])
-
     waveforms = get_waveform_est(b_seq)
     waveforms_df = pd.DataFrame(
         np.zeros((len(waveforms), 4)),
         columns=["wav_other", "wav_square", "wav_triangular", "wav_sine"],
     )
     # one hot encode
     waveform_dummies = pd.get_dummies(waveforms, prefix="wav", dtype=float).rename(
```

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_3C90_experiment_1b4d8_model_f3915868_seed_0_fold_0.pt` & `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3C90_experiment_1b4d8_model_f3915868_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_3C92_experiment_ea1fe_model_72510647_seed_0_fold_0.pt` & `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3C92_experiment_ea1fe_model_72510647_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_3C94_experiment_56441_model_55693612_seed_0_fold_0.pt` & `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3C94_experiment_56441_model_55693612_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_3C95_experiment_ad6ec_model_046383a5_seed_0_fold_0.pt` & `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3C95_experiment_ad6ec_model_046383a5_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_3E6_experiment_a7817_model_a1035e58_seed_0_fold_0.pt` & `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3E6_experiment_a7817_model_a1035e58_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_3F4_experiment_c234d_model_2d43b97d_seed_0_fold_0.pt` & `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3F4_experiment_c234d_model_2d43b97d_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_77_experiment_268ae_model_5b7c92ed_seed_0_fold_0.pt` & `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_77_experiment_268ae_model_5b7c92ed_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_78_experiment_e5297_model_77fbd758_seed_0_fold_0.pt` & `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_78_experiment_e5297_model_77fbd758_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_79_experiment_45989_model_7227af72_seed_0_fold_0.pt` & `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_79_experiment_45989_model_7227af72_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_A_experiment_c9cfe_model_d893c778_p.pt` & `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_A_experiment_c9cfe_model_d893c778_p.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_B_experiment_c9cfe_model_b6a920cc_p.pt` & `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_B_experiment_c9cfe_model_b6a920cc_p.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_C_experiment_c9cfe_model_c1ced7b6_p.pt` & `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_C_experiment_c9cfe_model_c1ced7b6_p.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_D_experiment_c9cfe_model_11672810_p.pt` & `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_D_experiment_c9cfe_model_11672810_p.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_E_experiment_c9cfe_model_5ae50f9e_p.pt` & `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_E_experiment_c9cfe_model_5ae50f9e_p.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_ML95S_experiment_1c978_model_883a5d2f_seed_0_fold_0.pt` & `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_ML95S_experiment_1c978_model_883a5d2f_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_N27_experiment_8b7f0_model_20954a2a_seed_0_fold_0.pt` & `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_N27_experiment_8b7f0_model_20954a2a_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_N30_experiment_5a78c_model_6bd86623_seed_0_fold_0.pt` & `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_N30_experiment_5a78c_model_6bd86623_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_N49_experiment_27442_model_d6234a32_seed_0_fold_0.pt` & `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_N49_experiment_27442_model_d6234a32_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_N87_experiment_985cb_model_d51b0f7e_seed_0_fold_0.pt` & `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_N87_experiment_985cb_model_d51b0f7e_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/src_py/magnethub/models/paderborn/cnn_T37_experiment_a084a_model_fb31325e_seed_0_fold_0.pt` & `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_T37_experiment_a084a_model_fb31325e_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/tests/test_paderborn.py` & `mag_net_hub-0.0.6/tests/test_paderborn.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         p = np.array(p_preds_l)
         rel_err = np.abs(test_mat_df.ploss - p) / test_mat_df.ploss
         print(f"{m_lbl}: avg. rel err {np.mean(rel_err):.5%} 95th quantile {np.quantile(rel_err, 0.95):.5%}")
 
 
 def test_accuracy_slightly():
     test_ds = pd.read_csv(
-        Path.cwd() / "tests" / "test_files" / "unit_test_data_ploss_at_450kWpm3.csv", dtype={"material": str}
+        Path(__file__).parent / "test_files" / "unit_test_data_ploss_at_450kWpm3.csv", dtype={"material": str}
     )
     for m_lbl in MATERIALS:
         mdl = LossModel(material=m_lbl, team="paderborn")
         test_mat_df = test_ds.query("material == @m_lbl")
         p, h = mdl(
             test_mat_df.loc[:, [c for c in test_mat_df if c.startswith("B_t_")]].to_numpy(),
             test_mat_df.loc[:, "freq"].to_numpy(),
```

### Comparing `mag_net_hub-0.0.5/tests/test_files/unit_test_data_ploss_at_450kWpm3.csv` & `mag_net_hub-0.0.6/tests/test_files/unit_test_data_ploss_at_450kWpm3.csv`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/.gitignore` & `mag_net_hub-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/LICENSE` & `mag_net_hub-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.5/README.md` & `mag_net_hub-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -47,18 +47,14 @@
 or, alternatively, clone this repo and execute
 
 ```
 cd mag-net-hub
 pip install .
 ```
 
-### Matlab
-TBD
-
-
 ## Usage
 Models are provided as executable code with readily trained coefficients.
 Hence, no training is conducted in this project.
 
 ### Python
 ```py
 import numpy as np
@@ -79,17 +75,14 @@
 b_waves = np.random.randn(100, 1024)* 200e-3  # in T
 freqs = np.random.randint(100e3, 750e3, size=100)
 temps = np.random.randint(20, 80, size=100)
 p, h = mdl(b_waves, freqs, temps)
 
 ```
 
-### Matlab
-TBD
-
 
 ## Contributing
 Whether you want to contribute your submission to the MagNet Challenge, or you are a single contributor who wants to add an awesome model to this hub -- any contribution is welcome.
 
 Open a pull request to directly suggest small improvements to the infrastructure or to add your model (with performance statistics preferred). 
 For larger suggestions, please first open an issue or go to the discussion section to discuss your ideas. 
 
@@ -118,8 +111,13 @@
 ```
 
 Any number of models can be incorporated easily according to this code structure policy.
 If you have added model coefficients and execution logic via code, it only requires to be hooked in
 `loss.py` and you are ready to fire this pull request (PR).
 
 If it is possible, please also consider adding tests for your model logic under `tests/`, writing comprehensive docstrings in your code with some comments, and discuss the performance of your model in your PR. 
+
+Other open ToDos are:
+ - Matlab implementation
+ - improve documentation
+
 Thank you!
```

### Comparing `mag_net_hub-0.0.5/pyproject.toml` & `mag_net_hub-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mag-net-hub"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name = "Wilhelm Kirchgässner" },
 ]
 description = "MagNet Toolkit - Certified Models of the MagNet Challenge"
 readme = "README.md"
 requires-python = "~=3.10"
 classifiers = [
@@ -32,14 +32,15 @@
 [tool.hatch.build.targets.wheel]
 packages = ["src_py/magnethub"]
 
 [tool.hatch.build.targets.sdist]
 include = [
     "src_py/magnethub/*.py",
     "src_py/magnethub/models/paderborn/*.pt",
+    "src_py/magnethub/models/sydney/*.pt",
     "tests",
     "requirements.txt"
 ]
 
 
 
 [tool.ruff]
```

### Comparing `mag_net_hub-0.0.5/PKG-INFO` & `mag_net_hub-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.3
 Name: mag-net-hub
-Version: 0.0.5
+Version: 0.0.6
 Summary: MagNet Toolkit - Certified Models of the MagNet Challenge
 Project-URL: Homepage, https://github.com/upb-lea/mag-net-hub
 Project-URL: Issues, https://github.com/upb-lea/mag-net-hub/issues
 Author: Wilhelm Kirchgässner
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.10
 Requires-Dist: joblib>=1.3.2
 Requires-Dist: pandas>=2.0.3
+Requires-Dist: scipy
 Requires-Dist: torch>=2.0.1
 Requires-Dist: torchinfo>=1.8.0
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 
 <div align="center">
@@ -66,18 +67,14 @@
 or, alternatively, clone this repo and execute
 
 ```
 cd mag-net-hub
 pip install .
 ```
 
-### Matlab
-TBD
-
-
 ## Usage
 Models are provided as executable code with readily trained coefficients.
 Hence, no training is conducted in this project.
 
 ### Python
 ```py
 import numpy as np
@@ -98,17 +95,14 @@
 b_waves = np.random.randn(100, 1024)* 200e-3  # in T
 freqs = np.random.randint(100e3, 750e3, size=100)
 temps = np.random.randint(20, 80, size=100)
 p, h = mdl(b_waves, freqs, temps)
 
 ```
 
-### Matlab
-TBD
-
 
 ## Contributing
 Whether you want to contribute your submission to the MagNet Challenge, or you are a single contributor who wants to add an awesome model to this hub -- any contribution is welcome.
 
 Open a pull request to directly suggest small improvements to the infrastructure or to add your model (with performance statistics preferred). 
 For larger suggestions, please first open an issue or go to the discussion section to discuss your ideas. 
 
@@ -137,8 +131,13 @@
 ```
 
 Any number of models can be incorporated easily according to this code structure policy.
 If you have added model coefficients and execution logic via code, it only requires to be hooked in
 `loss.py` and you are ready to fire this pull request (PR).
 
 If it is possible, please also consider adding tests for your model logic under `tests/`, writing comprehensive docstrings in your code with some comments, and discuss the performance of your model in your PR. 
+
+Other open ToDos are:
+ - Matlab implementation
+ - improve documentation
+
 Thank you!
```

