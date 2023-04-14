# Comparing `tmp/ferveo-0.1.6.tar.gz` & `tmp/ferveo-0.1.7.tar.gz`

## Comparing `ferveo-0.1.6.tar` & `ferveo-0.1.7.tar`

### file list

```diff
@@ -1,55 +1,58 @@
--rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/Cargo.toml
--rw-rw-r--   0     1000     1000     5872 2023-01-19 15:29:04.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/BENCHMARK.md
--rw-rw-r--   0     1000     1000      470 2023-04-05 16:16:20.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/README.md
--rw-rw-r--   0     1000     1000     9295 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/benches/arkworks.rs
--rw-rw-r--   0     1000     1000    19243 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/benches/tpke.rs
--rw-rw-r--   0     1000     1000     1674 2023-04-12 08:07:58.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/api.rs
--rw-rw-r--   0     1000     1000     7782 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/ciphertext.rs
--rw-rw-r--   0     1000     1000     5517 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/combine.rs
--rw-rw-r--   0     1000     1000     3471 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/context.rs
--rw-rw-r--   0     1000     1000    11755 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/decryption.rs
--rw-rw-r--   0     1000     1000     4254 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/hash_to_curve.rs
--rw-rw-r--   0     1000     1000     2179 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/key_share.rs
--rw-rw-r--   0     1000     1000    28991 2023-04-12 09:44:49.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/lib.rs
--rw-rw-r--   0     1000     1000     3487 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/refresh.rs
--rw-r--r--   0        0        0     1230 1970-01-01 00:00:00.000000 ferveo-0.1.6/local_dependencies/ferveo/Cargo.toml
--rw-rw-r--   0     1000     1000    51910 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/Cargo.lock
--rw-rw-r--   0     1000     1000      111 2023-04-05 16:16:20.000000 ferveo-0.1.6/local_dependencies/ferveo/README.md
--rw-rw-r--   0     1000     1000      214 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/benches/bench_main.rs
--rw-rw-r--   0     1000     1000     3863 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/benches/benchmarks/block_proposer.rs
--rw-rw-r--   0     1000     1000       71 2023-04-05 16:15:54.000000 ferveo-0.1.6/local_dependencies/ferveo/benches/benchmarks/mod.rs
--rw-rw-r--   0     1000     1000    11868 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/benches/benchmarks/pairing.rs
--rw-rw-r--   0     1000     1000     3516 2023-04-12 09:05:33.000000 ferveo-0.1.6/local_dependencies/ferveo/benches/benchmarks/pvdkg.rs
--rw-rw-r--   0     1000     1000     3207 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/benches/benchmarks/validity_checks.rs
--rw-rw-r--   0     1000     1000     4131 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/examples/bench_primitives_size.rs
--rw-rw-r--   0     1000     1000     2326 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/examples/pvdkg.rs
--rw-rw-r--   0     1000     1000     6932 2023-04-12 08:08:03.000000 ferveo-0.1.6/local_dependencies/ferveo/src/api.rs
--rw-rw-r--   0     1000     1000      410 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/src/dkg/common.rs
--rw-rw-r--   0     1000     1000    23980 2023-04-12 08:07:58.000000 ferveo-0.1.6/local_dependencies/ferveo/src/dkg/pv.rs
--rw-rw-r--   0     1000     1000      547 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/src/dkg.rs
--rw-rw-r--   0     1000     1000    16561 2023-04-12 08:07:58.000000 ferveo-0.1.6/local_dependencies/ferveo/src/lib.rs
--rw-rw-r--   0     1000     1000      560 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/src/primitives.rs
--rw-rw-r--   0     1000     1000    19002 2023-04-12 08:07:58.000000 ferveo-0.1.6/local_dependencies/ferveo/src/vss/pvss.rs
--rw-rw-r--   0     1000     1000      558 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/src/vss.rs
--rw-r--r--   0        0        0      356 1970-01-01 00:00:00.000000 ferveo-0.1.6/local_dependencies/ferveo-common/Cargo.toml
--rw-rw-r--   0     1000     1000     2469 2023-04-12 09:49:44.000000 ferveo-0.1.6/local_dependencies/ferveo-common/src/keypair.rs
--rw-rw-r--   0     1000     1000      831 2023-04-06 21:18:33.000000 ferveo-0.1.6/local_dependencies/ferveo-common/src/lib.rs
--rw-rw-r--   0     1000     1000     4008 2023-04-06 21:18:33.000000 ferveo-0.1.6/local_dependencies/ferveo-common/src/serialization.rs
--rw-rw-r--   0     1000     1000       74 2023-04-06 21:18:33.000000 ferveo-0.1.6/local_dependencies/ferveo-common/src/utils.rs
--rw-r--r--   0        0        0      231 1970-01-01 00:00:00.000000 ferveo-0.1.6/local_dependencies/subproductdomain/Cargo.toml
--rw-rw-r--   0     1000     1000    16742 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/subproductdomain/src/lib.rs
--rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 ferveo-0.1.6/Cargo.toml
--rw-rw-r--   0     1000     1000       54 2023-04-06 21:18:33.000000 ferveo-0.1.6/.gitignore
--rwxrwxr-x   0     1000     1000    34916 2023-04-06 21:18:33.000000 ferveo-0.1.6/LICENSE
--rw-rw-r--   0     1000     1000       77 2023-04-06 21:18:33.000000 ferveo-0.1.6/MANIFEST.in
--rw-rw-r--   0     1000     1000      161 2023-04-06 21:18:33.000000 ferveo-0.1.6/README.md
--rw-rw-r--   0     1000     1000       71 2023-04-06 21:18:33.000000 ferveo-0.1.6/build.rs
--rw-rw-r--   0     1000     1000     3369 2023-04-12 08:47:23.000000 ferveo-0.1.6/examples/server_api.py
--rw-rw-r--   0     1000     1000      303 2023-04-12 08:08:03.000000 ferveo-0.1.6/ferveo/__init__.py
--rw-rw-r--   0     1000     1000     2383 2023-04-12 09:05:42.000000 ferveo-0.1.6/ferveo/__init__.pyi
--rw-rw-r--   0     1000     1000        0 2023-04-06 21:18:33.000000 ferveo-0.1.6/ferveo/py.typed
--rw-rw-r--   0     1000     1000      316 2023-04-11 10:00:55.000000 ferveo-0.1.6/pyproject.toml
--rw-rw-r--   0     1000     1000     1444 2023-04-12 09:54:09.000000 ferveo-0.1.6/setup.py
--rw-rw-r--   0     1000     1000     9001 2023-04-12 08:37:18.000000 ferveo-0.1.6/src/lib.rs
--rw-rw-r--   0     1000     1000    56086 2023-04-12 09:54:10.000000 ferveo-0.1.6/Cargo.lock
--rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 ferveo-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 ferveo-0.1.7/local_dependencies/ferveo/Cargo.toml
+-rw-rw-r--   0     1000     1000    51910 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/ferveo/Cargo.lock
+-rw-rw-r--   0     1000     1000      111 2023-04-05 16:16:20.000000 ferveo-0.1.7/local_dependencies/ferveo/README.md
+-rw-rw-r--   0     1000     1000      214 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/ferveo/benches/bench_main.rs
+-rw-rw-r--   0     1000     1000     3863 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/ferveo/benches/benchmarks/block_proposer.rs
+-rw-rw-r--   0     1000     1000       71 2023-04-05 16:15:54.000000 ferveo-0.1.7/local_dependencies/ferveo/benches/benchmarks/mod.rs
+-rw-rw-r--   0     1000     1000    11868 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/ferveo/benches/benchmarks/pairing.rs
+-rw-rw-r--   0     1000     1000     3516 2023-04-12 12:02:25.000000 ferveo-0.1.7/local_dependencies/ferveo/benches/benchmarks/pvdkg.rs
+-rw-rw-r--   0     1000     1000     3207 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/ferveo/benches/benchmarks/validity_checks.rs
+-rw-rw-r--   0     1000     1000     4131 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/ferveo/examples/bench_primitives_size.rs
+-rw-rw-r--   0     1000     1000     2326 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/ferveo/examples/pvdkg.rs
+-rw-rw-r--   0     1000     1000    12719 2023-04-14 14:00:32.000000 ferveo-0.1.7/local_dependencies/ferveo/src/api.rs
+-rw-rw-r--   0     1000     1000      410 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/ferveo/src/dkg/common.rs
+-rw-rw-r--   0     1000     1000    23980 2023-04-14 08:59:50.000000 ferveo-0.1.7/local_dependencies/ferveo/src/dkg/pv.rs
+-rw-rw-r--   0     1000     1000      547 2023-04-13 21:16:41.000000 ferveo-0.1.7/local_dependencies/ferveo/src/dkg.rs
+-rw-rw-r--   0     1000     1000    16674 2023-04-14 16:12:38.000000 ferveo-0.1.7/local_dependencies/ferveo/src/lib.rs
+-rw-rw-r--   0     1000     1000      560 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/ferveo/src/primitives.rs
+-rw-rw-r--   0     1000     1000    18984 2023-04-14 11:01:01.000000 ferveo-0.1.7/local_dependencies/ferveo/src/vss/pvss.rs
+-rw-rw-r--   0     1000     1000      558 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/ferveo/src/vss.rs
+-rw-r--r--   0        0        0      356 1970-01-01 00:00:00.000000 ferveo-0.1.7/local_dependencies/ferveo-common/Cargo.toml
+-rw-rw-r--   0     1000     1000     2469 2023-04-14 08:59:50.000000 ferveo-0.1.7/local_dependencies/ferveo-common/src/keypair.rs
+-rw-rw-r--   0     1000     1000      831 2023-04-06 21:18:33.000000 ferveo-0.1.7/local_dependencies/ferveo-common/src/lib.rs
+-rw-rw-r--   0     1000     1000     4008 2023-04-06 21:18:33.000000 ferveo-0.1.7/local_dependencies/ferveo-common/src/serialization.rs
+-rw-rw-r--   0     1000     1000       74 2023-04-06 21:18:33.000000 ferveo-0.1.7/local_dependencies/ferveo-common/src/utils.rs
+-rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/Cargo.toml
+-rw-rw-r--   0     1000     1000     5872 2023-01-19 15:29:04.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/BENCHMARK.md
+-rw-rw-r--   0     1000     1000      470 2023-04-05 16:16:20.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/README.md
+-rw-rw-r--   0     1000     1000     9295 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/benches/arkworks.rs
+-rw-rw-r--   0     1000     1000    19197 2023-04-14 11:01:02.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/benches/tpke.rs
+-rw-rw-r--   0     1000     1000     1255 2023-04-14 13:31:54.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/api.rs
+-rw-rw-r--   0     1000     1000     7788 2023-04-14 09:08:00.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/ciphertext.rs
+-rw-rw-r--   0     1000     1000     5498 2023-04-14 11:01:02.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/combine.rs
+-rw-rw-r--   0     1000     1000     3453 2023-04-14 11:01:02.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/context.rs
+-rw-rw-r--   0     1000     1000    11743 2023-04-14 10:33:06.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/decryption.rs
+-rw-rw-r--   0     1000     1000     4254 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/hash_to_curve.rs
+-rw-rw-r--   0     1000     1000     2179 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/key_share.rs
+-rw-rw-r--   0     1000     1000    29218 2023-04-14 16:18:03.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/lib.rs
+-rw-rw-r--   0     1000     1000     3487 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/refresh.rs
+-rw-r--r--   0        0        0      231 1970-01-01 00:00:00.000000 ferveo-0.1.7/local_dependencies/subproductdomain/Cargo.toml
+-rw-rw-r--   0     1000     1000    16742 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/subproductdomain/src/lib.rs
+-rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 ferveo-0.1.7/Cargo.toml
+-rw-rw-r--   0     1000     1000       54 2023-04-06 21:18:33.000000 ferveo-0.1.7/.gitignore
+-rwxrwxr-x   0     1000     1000    34916 2023-04-06 21:18:33.000000 ferveo-0.1.7/LICENSE
+-rw-rw-r--   0     1000     1000       77 2023-04-06 21:18:33.000000 ferveo-0.1.7/MANIFEST.in
+-rw-rw-r--   0     1000     1000      161 2023-04-06 21:18:33.000000 ferveo-0.1.7/README.md
+-rw-rw-r--   0     1000     1000       71 2023-04-06 21:18:33.000000 ferveo-0.1.7/build.rs
+-rw-rw-r--   0     1000     1000     3481 2023-04-14 14:02:04.000000 ferveo-0.1.7/examples/server_api_precomputed.py
+-rw-rw-r--   0     1000     1000     3392 2023-04-14 14:02:04.000000 ferveo-0.1.7/examples/server_api_simple.py
+-rw-rw-r--   0     1000     1000      410 2023-04-14 14:43:54.000000 ferveo-0.1.7/ferveo/__init__.py
+-rw-rw-r--   0     1000     1000     3787 2023-04-14 13:53:26.000000 ferveo-0.1.7/ferveo/__init__.pyi
+-rw-rw-r--   0     1000     1000        0 2023-04-06 21:18:33.000000 ferveo-0.1.7/ferveo/py.typed
+-rw-rw-r--   0     1000     1000      316 2023-04-14 08:59:50.000000 ferveo-0.1.7/pyproject.toml
+-rw-rw-r--   0     1000     1000     1444 2023-04-14 16:19:01.000000 ferveo-0.1.7/setup.py
+-rw-rw-r--   0     1000     1000    11220 2023-04-14 13:37:22.000000 ferveo-0.1.7/src/lib.rs
+-rw-rw-r--   0     1000     1000     3554 2023-04-14 15:26:28.000000 ferveo-0.1.7/test/test_ferveo.py
+-rw-rw-r--   0     1000     1000     1514 2023-04-14 15:12:10.000000 ferveo-0.1.7/test/test_serialization.py
+-rw-rw-r--   0     1000     1000    56115 2023-04-14 16:19:10.000000 ferveo-0.1.7/Cargo.lock
+-rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 ferveo-0.1.7/PKG-INFO
```

### Comparing `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/Cargo.toml` & `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/BENCHMARK.md` & `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/BENCHMARK.md`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/benches/arkworks.rs` & `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/benches/arkworks.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/benches/tpke.rs` & `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/benches/tpke.rs`

 * *Files 0% similar despite different names*

```diff
@@ -300,17 +300,15 @@
                             &setup.shared.aad,
                         )
                         .unwrap()
                 })
                 .collect();
 
             move || {
-                black_box(share_combine_simple_precomputed::<E>(
-                    &decryption_shares,
-                ));
+                black_box(share_combine_precomputed::<E>(&decryption_shares));
             }
         };
 
         group.bench_function(
             BenchmarkId::new("share_combine_fast", shares_num),
             |b| b.iter(|| fast()),
         );
```

### Comparing `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/api.rs` & `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/api.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,33 @@
 //! Contains the public API of the library.
 
-use ark_serialize::{CanonicalDeserialize, CanonicalSerialize};
 use ferveo_common::serialization;
 use serde::{Deserialize, Serialize};
 use serde_with::serde_as;
 
 pub type E = ark_bls12_381::Bls12_381;
 pub type G1Prepared = <E as ark_ec::pairing::Pairing>::G1Prepared;
+pub type G1Affine = <E as ark_ec::pairing::Pairing>::G1Affine;
+pub type Fr = ark_bls12_381::Fr;
 pub type PrivateKey = ark_bls12_381::G2Affine;
-pub type UnblindingKey = ark_bls12_381::Fr;
-pub type SharedSecret = <E as ark_ec::pairing::Pairing>::TargetField;
 pub type Result<T> = crate::Result<T>;
 pub type PrivateDecryptionContextSimple =
     crate::PrivateDecryptionContextSimple<E>;
-pub type DecryptionShareSimplePrecomputed =
-    crate::DecryptionShareSimplePrecomputed<E>;
+pub type DecryptionSharePrecomputed = crate::DecryptionSharePrecomputed<E>;
 pub type DecryptionShareSimple = crate::DecryptionShareSimple<E>;
 pub type Ciphertext = crate::Ciphertext<E>;
+pub type TargetField = <E as ark_ec::pairing::Pairing>::TargetField;
 
 pub use crate::{
     decrypt_symmetric, decrypt_with_shared_secret, encrypt,
-    share_combine_simple_precomputed,
+    prepare_combine_simple, share_combine_precomputed, share_combine_simple,
 };
 
 #[serde_as]
-#[derive(Clone, Debug, PartialEq, Serialize, Deserialize)]
-pub struct DomainPoint(
-    #[serde_as(as = "serialization::SerdeAs")] pub ark_bls12_381::Fr,
-);
+#[derive(Copy, Clone, Debug, PartialEq, Serialize, Deserialize)]
+pub struct DomainPoint(#[serde_as(as = "serialization::SerdeAs")] pub Fr);
 
 #[serde_as]
 #[derive(Copy, Clone, Debug, PartialEq, Serialize, Deserialize)]
-pub struct DkgPublicKey(
-    #[serde_as(as = "serialization::SerdeAs")] pub ark_bls12_381::G1Affine,
+pub struct SharedSecret(
+    #[serde_as(as = "serialization::SerdeAs")] pub TargetField,
 );
-
-impl DkgPublicKey {
-    pub fn to_bytes(&self) -> Result<Vec<u8>> {
-        let mut writer = Vec::new();
-        self.0.serialize_uncompressed(&mut writer)?;
-        Ok(writer)
-    }
-
-    pub fn from_bytes(bytes: &[u8]) -> Result<DkgPublicKey> {
-        let mut reader = bytes;
-        let pk =
-            ark_bls12_381::G1Affine::deserialize_uncompressed(&mut reader)?;
-        Ok(Self(pk))
-    }
-}
```

### Comparing `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/ciphertext.rs` & `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/ciphertext.rs`

 * *Files 4% similar despite different names*

```diff
@@ -13,22 +13,25 @@
 use sha2::{digest::Digest, Sha256};
 
 use crate::{htp_bls12381_g2, Error, Result};
 
 #[serde_as]
 #[derive(Clone, Debug, PartialEq, Serialize, Deserialize)]
 pub struct Ciphertext<E: Pairing> {
+    // U
     #[serde_as(as = "serialization::SerdeAs")]
     pub commitment: E::G1Affine,
-    // U
+
+    // W
     #[serde_as(as = "serialization::SerdeAs")]
     pub auth_tag: E::G2Affine,
-    // W
+
+    // V
     #[serde(with = "serde_bytes")]
-    pub ciphertext: Vec<u8>, // V
+    pub ciphertext: Vec<u8>,
 }
 
 impl<E: Pairing> Ciphertext<E> {
     pub fn check(&self, g_inv: &E::G1Prepared) -> Result<bool> {
         let hash_g2 = E::G2Prepared::from(self.construct_tag_hash()?);
 
         Ok(E::multi_pairing(
```

### Comparing `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/combine.rs` & `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/combine.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 use ark_ec::{pairing::Pairing, CurveGroup};
 use ark_ff::{Field, One, PrimeField, Zero};
 use itertools::izip;
 use subproductdomain::SubproductDomain;
 
 use crate::{
     verify_decryption_shares_fast, Ciphertext, DecryptionShareFast,
-    DecryptionShareSimple, DecryptionShareSimplePrecomputed, Error,
+    DecryptionSharePrecomputed, DecryptionShareSimple, Error,
     PublicDecryptionContextFast, Result,
 };
 
 pub fn prepare_combine_fast<E: Pairing>(
     public_decryption_contexts: &[PublicDecryptionContextFast<E>],
     shares: &[DecryptionShareFast<E>],
 ) -> Vec<E::G2Prepared> {
@@ -123,16 +123,16 @@
         E::TargetField::one(),
         |acc, (c_i, alpha_i)| {
             acc * c_i.decryption_share.pow(alpha_i.into_bigint())
         },
     )
 }
 
-pub fn share_combine_simple_precomputed<E: Pairing>(
-    shares: &[DecryptionShareSimplePrecomputed<E>],
+pub fn share_combine_precomputed<E: Pairing>(
+    shares: &[DecryptionSharePrecomputed<E>],
 ) -> E::TargetField {
     // s = ∏ C_{λ_i}, where λ_i is the Lagrange coefficient for i
     shares
         .iter()
         .fold(E::TargetField::one(), |acc, c_i| acc * c_i.decryption_share)
 }
```

### Comparing `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/context.rs` & `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/context.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use std::ops::Mul;
 
 use ark_ec::{pairing::Pairing, CurveGroup};
 
 use crate::{
     check_ciphertext_validity, prepare_combine_simple, BlindedKeyShare,
-    Ciphertext, DecryptionShareFast, DecryptionShareSimple,
-    DecryptionShareSimplePrecomputed, PrivateKeyShare, PublicKeyShare, Result,
+    Ciphertext, DecryptionShareFast, DecryptionSharePrecomputed,
+    DecryptionShareSimple, PrivateKeyShare, PublicKeyShare, Result,
 };
 
 #[derive(Clone, Debug)]
 pub struct PublicDecryptionContextFast<E: Pairing> {
     pub domain: E::ScalarField,
     pub public_key_share: PublicKeyShare<E>,
     pub blinded_key_share: BlindedKeyShare<E>,
@@ -95,23 +95,23 @@
         )
     }
 
     pub fn create_share_precomputed(
         &self,
         ciphertext: &Ciphertext<E>,
         aad: &[u8],
-    ) -> Result<DecryptionShareSimplePrecomputed<E>> {
+    ) -> Result<DecryptionSharePrecomputed<E>> {
         let domain = self
             .public_decryption_contexts
             .iter()
             .map(|c| c.domain)
             .collect::<Vec<_>>();
         let lagrange_coeffs = prepare_combine_simple::<E>(&domain);
 
-        DecryptionShareSimplePrecomputed::new(
+        DecryptionSharePrecomputed::new(
             self.index,
             &self.validator_private_key,
             &self.private_key_share,
             ciphertext,
             aad,
             &lagrange_coeffs[self.index],
             &self.setup_params.g_inv,
```

### Comparing `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/decryption.rs` & `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/decryption.rs`

 * *Files 0% similar despite different names*

```diff
@@ -150,22 +150,22 @@
 
 #[serde_as]
 #[derive(Clone, Debug, PartialEq, Serialize, Deserialize)]
 #[serde(bound(
     serialize = "ValidatorShareChecksum<E>: Serialize",
     deserialize = "ValidatorShareChecksum<E>: DeserializeOwned"
 ))]
-pub struct DecryptionShareSimplePrecomputed<E: Pairing> {
+pub struct DecryptionSharePrecomputed<E: Pairing> {
     pub decrypter_index: usize,
     #[serde_as(as = "serialization::SerdeAs")]
     pub decryption_share: E::TargetField,
     pub validator_checksum: ValidatorShareChecksum<E>,
 }
 
-impl<E: Pairing> DecryptionShareSimplePrecomputed<E> {
+impl<E: Pairing> DecryptionSharePrecomputed<E> {
     pub fn new(
         validator_index: usize,
         validator_decryption_key: &E::ScalarField,
         private_key_share: &PrivateKeyShare<E>,
         ciphertext: &Ciphertext<E>,
         aad: &[u8],
         lagrange_coeff: &E::ScalarField,
```

### Comparing `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/hash_to_curve.rs` & `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/hash_to_curve.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/key_share.rs` & `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/key_share.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/lib.rs` & `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -266,14 +266,26 @@
         }
         for private in private_contexts.iter_mut() {
             private.public_decryption_contexts = public_contexts.clone();
         }
 
         (pubkey.into(), privkey.into(), private_contexts)
     }
+
+    pub fn setup_precomputed<E: Pairing>(
+        shares_num: usize,
+        rng: &mut impl rand::Rng,
+    ) -> (
+        E::G1Affine,
+        E::G2Affine,
+        Vec<PrivateDecryptionContextSimple<E>>,
+    ) {
+        // In precomputed variant, the security threshold is equal to the number of shares
+        setup_simple::<E>(shares_num, shares_num, rng)
+    }
 }
 
 #[cfg(test)]
 mod tests {
     use std::{collections::HashMap, ops::Mul};
 
     use ark_bls12_381::Fr;
@@ -419,30 +431,30 @@
     ) -> E::TargetField {
         let domain = pub_contexts.iter().map(|c| c.domain).collect::<Vec<_>>();
         let lagrange_coeffs = prepare_combine_simple::<E>(&domain);
         share_combine_simple::<E>(decryption_shares, &lagrange_coeffs)
     }
 
     #[test]
-    fn fast_decryption_share_validation() {
+    fn tdec_fast_variant_share_validation() {
         let rng = &mut test_rng();
         let shares_num = 16;
         let threshold = shares_num * 2 / 3;
         let msg: &[u8] = "abc".as_bytes();
         let aad: &[u8] = "my-aad".as_bytes();
 
         let (pubkey, _, contexts) = setup_fast::<E>(threshold, shares_num, rng);
         let ciphertext = encrypt::<E>(msg, aad, &pubkey, rng).unwrap();
 
         let bad_aad = "bad aad".as_bytes();
         assert!(contexts[0].create_share(&ciphertext, bad_aad).is_err());
     }
 
     #[test]
-    fn simple_decryption_share_validation() {
+    fn tdec_simple_variant_share_validation() {
         let rng = &mut test_rng();
         let shares_num = 16;
         let threshold = shares_num * 2 / 3;
         let msg: &[u8] = "abc".as_bytes();
         let aad: &[u8] = "my-aad".as_bytes();
 
         let (pubkey, _, contexts) =
@@ -450,15 +462,15 @@
         let ciphertext = encrypt::<E>(msg, aad, &pubkey, rng).unwrap();
 
         let bad_aad = "bad aad".as_bytes();
         assert!(contexts[0].create_share(&ciphertext, bad_aad).is_err());
     }
 
     #[test]
-    fn fast_threshold_encryption() {
+    fn tdec_fast_variant_e2e() {
         let mut rng = &mut test_rng();
         let shares_num = 16;
         let threshold = shares_num * 2 / 3;
         let msg: &[u8] = "abc".as_bytes();
         let aad: &[u8] = "my-aad".as_bytes();
 
         let (pubkey, _, contexts) =
@@ -498,15 +510,15 @@
             &ciphertext,
             &shared_secret,
             g_inv,
         );
     }
 
     #[test]
-    fn simple_threshold_decryption() {
+    fn tdec_simple_variant_e2e() {
         let mut rng = &mut test_rng();
         let shares_num = 16;
         let threshold = shares_num * 2 / 3;
         let msg: &[u8] = "abc".as_bytes();
         let aad: &[u8] = "my-aad".as_bytes();
 
         let (pubkey, _, contexts) =
@@ -531,61 +543,59 @@
             &ciphertext,
             &shared_secret,
             g_inv,
         );
     }
 
     #[test]
-    fn simple_threshold_decryption_precomputed() {
+    fn tdec_precomputed_variant_e2e() {
         let mut rng = &mut test_rng();
         let shares_num = 16;
-        let threshold = shares_num * 2 / 3;
         let msg: &[u8] = "abc".as_bytes();
         let aad: &[u8] = "my-aad".as_bytes();
 
         let (pubkey, _, contexts) =
-            setup_simple::<E>(threshold, shares_num, &mut rng);
+            setup_precomputed::<E>(shares_num, &mut rng);
         let g_inv = &contexts[0].setup_params.g_inv;
         let ciphertext = encrypt::<E>(msg, aad, &pubkey, rng).unwrap();
 
         let decryption_shares: Vec<_> = contexts
             .iter()
             .map(|context| {
                 context.create_share_precomputed(&ciphertext, aad).unwrap()
             })
             .collect();
 
-        let shared_secret =
-            share_combine_simple_precomputed::<E>(&decryption_shares);
+        let shared_secret = share_combine_precomputed::<E>(&decryption_shares);
 
         test_ciphertext_validation_fails(
             msg,
             aad,
             &ciphertext,
             &shared_secret,
             g_inv,
         );
 
         // Note that in this variant, if we use less than `share_num` shares, we will get a
         // decryption error.
 
         let not_enough_shares = &decryption_shares[0..shares_num - 1];
         let bad_shared_secret =
-            share_combine_simple_precomputed::<E>(not_enough_shares);
+            share_combine_precomputed::<E>(not_enough_shares);
         assert!(decrypt_with_shared_secret(
             &ciphertext,
             aad,
             &bad_shared_secret,
             g_inv,
         )
         .is_err());
     }
 
     #[test]
-    fn simple_threshold_decryption_share_verification() {
+    fn tdec_simple_variant_share_verification() {
         let mut rng = &mut test_rng();
         let shares_num = 16;
         let threshold = shares_num * 2 / 3;
         let msg: &[u8] = "abc".as_bytes();
         let aad: &[u8] = "my-aad".as_bytes();
 
         let (pubkey, _, contexts) =
@@ -641,15 +651,15 @@
             &ciphertext,
         ));
     }
 
     /// Ñ parties (where t <= Ñ <= N) jointly execute a "share recovery" algorithm, and the output is 1 new share.
     /// The new share is intended to restore a previously existing share, e.g., due to loss or corruption.
     #[test]
-    fn simple_threshold_decryption_with_share_recovery_at_selected_point() {
+    fn tdec_simple_variant_share_recovery_at_selected_point() {
         let rng = &mut test_rng();
         let shares_num = 16;
         let threshold = shares_num * 2 / 3;
 
         let (_, _, mut contexts) =
             setup_simple::<E>(threshold, shares_num, rng);
 
@@ -692,15 +702,15 @@
 
         assert_eq!(new_private_key_share, original_private_key_share);
     }
 
     /// Ñ parties (where t <= Ñ <= N) jointly execute a "share recovery" algorithm, and the output is 1 new share.
     /// The new share is independent from the previously existing shares. We can use this to on-board a new participant into an existing cohort.
     #[test]
-    fn simple_threshold_decryption_with_share_recovery_at_random_point() {
+    fn tdec_simple_variant_share_recovery_at_random_point() {
         let rng = &mut test_rng();
         let shares_num = 16;
         let threshold = shares_num * 2 / 3;
         let msg: &[u8] = "abc".as_bytes();
         let aad: &[u8] = "my-aad".as_bytes();
 
         let (pubkey, _, contexts) =
@@ -773,15 +783,15 @@
         assert_eq!(old_shared_secret, new_shared_secret);
     }
 
     /// Ñ parties (where t <= Ñ <= N) jointly execute a "share refresh" algorithm.
     /// The output is M new shares (with M <= Ñ), with each of the M new shares substituting the
     /// original share (i.e., the original share is deleted).
     #[test]
-    fn simple_threshold_decryption_with_share_refreshing() {
+    fn tdec_simple_variant_share_refreshing() {
         let rng = &mut test_rng();
         let shares_num = 16;
         let threshold = shares_num * 2 / 3;
         let msg: &[u8] = "abc".as_bytes();
         let aad: &[u8] = "my-aad".as_bytes();
 
         let (pubkey, _, contexts) =
```

### Comparing `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/refresh.rs` & `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/refresh.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/local_dependencies/ferveo/Cargo.toml` & `ferveo-0.1.7/local_dependencies/ferveo/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ferveo-common = { path = "../ferveo-common" }
 subproductdomain = { path = "../subproductdomain" }
 ark-std = "0.4"
 ark-bls12-381 = "0.4"
 ark-ec = "0.4"
 ark-ff = "0.4"
 ark-poly = "0.4"
+ark-serialize = "0.4"
 rand = "0.8"
 rand_old = { package = "rand", version = "0.7" } # used by benchmarks/pairing.rs
 serde = { version = "1.0", features = ["derive"] }
 bincode = "1.3"
 itertools = "0.10.1"
 measure_time = "0.8"
 rand_core = "0.6.4"
```

### Comparing `ferveo-0.1.6/local_dependencies/ferveo/Cargo.lock` & `ferveo-0.1.7/local_dependencies/ferveo/Cargo.lock`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/local_dependencies/ferveo/benches/benchmarks/block_proposer.rs` & `ferveo-0.1.7/local_dependencies/ferveo/benches/benchmarks/block_proposer.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/local_dependencies/ferveo/benches/benchmarks/pairing.rs` & `ferveo-0.1.7/local_dependencies/ferveo/benches/benchmarks/pairing.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/local_dependencies/ferveo/benches/benchmarks/pvdkg.rs` & `ferveo-0.1.7/local_dependencies/ferveo/benches/benchmarks/pvdkg.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/local_dependencies/ferveo/benches/benchmarks/validity_checks.rs` & `ferveo-0.1.7/local_dependencies/ferveo/benches/benchmarks/validity_checks.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/local_dependencies/ferveo/examples/bench_primitives_size.rs` & `ferveo-0.1.7/local_dependencies/ferveo/examples/bench_primitives_size.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/local_dependencies/ferveo/examples/pvdkg.rs` & `ferveo-0.1.7/local_dependencies/ferveo/examples/pvdkg.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/local_dependencies/ferveo/src/dkg/pv.rs` & `ferveo-0.1.7/local_dependencies/ferveo/src/dkg/pv.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/local_dependencies/ferveo/src/dkg.rs` & `ferveo-0.1.7/local_dependencies/ferveo/src/dkg.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/local_dependencies/ferveo/src/lib.rs` & `ferveo-0.1.7/local_dependencies/ferveo/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,18 @@
     /// Not enough validators to perform the DKG for a given number of shares
     #[error("Not enough validators (expected {0}, got {1})")]
     InsufficientValidators(u32, u32),
 
     /// Transcript aggregate doesn't match the received PVSS instances
     #[error("Transcript aggregate doesn't match the received PVSS instances")]
     InvalidTranscriptAggregate,
+
+    /// Serialization error
+    #[error("Serialization error")]
+    SerializationError(#[from] ark_serialize::SerializationError),
 }
 
 pub type Result<T> = std::result::Result<T, Error>;
 
 #[cfg(test)]
 mod test_dkg_full {
     use std::collections::HashMap;
@@ -79,15 +83,15 @@
     use ark_ec::{pairing::Pairing, AffineRepr, CurveGroup};
     use ark_ff::{UniformRand, Zero};
     use ark_poly::EvaluationDomain;
     use ark_std::test_rng;
     use ferveo_common::Keypair;
     use group_threshold_cryptography as tpke;
     use group_threshold_cryptography::{
-        Ciphertext, DecryptionShareSimple, DecryptionShareSimplePrecomputed,
+        Ciphertext, DecryptionSharePrecomputed, DecryptionShareSimple,
     };
     use itertools::{izip, Itertools};
 
     use super::*;
     use crate::dkg::pv::test_common::*;
 
     type TargetField = <E as Pairing>::TargetField;
@@ -192,15 +196,15 @@
         let pvss_aggregated = aggregate(&dkg);
         let domain_points = dkg
             .domain
             .elements()
             .take(validator_keypairs.len())
             .collect::<Vec<_>>();
 
-        let decryption_shares: Vec<DecryptionShareSimplePrecomputed<E>> =
+        let decryption_shares: Vec<DecryptionSharePrecomputed<E>> =
             validator_keypairs
                 .iter()
                 .enumerate()
                 .map(|(validator_index, validator_keypair)| {
                     pvss_aggregated
                         .make_decryption_share_simple_precomputed(
                             &ciphertext,
@@ -211,15 +215,15 @@
                             &dkg.pvss_params.g_inv(),
                         )
                         .unwrap()
                 })
                 .collect();
 
         let shared_secret =
-            tpke::share_combine_simple_precomputed::<E>(&decryption_shares);
+            tpke::share_combine_precomputed::<E>(&decryption_shares);
 
         // Combination works, let's decrypt
         let plaintext = tpke::decrypt_with_shared_secret(
             &ciphertext,
             aad,
             &shared_secret,
             &dkg.pvss_params.g_inv(),
```

### Comparing `ferveo-0.1.6/local_dependencies/ferveo/src/primitives.rs` & `ferveo-0.1.7/local_dependencies/ferveo/src/primitives.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/local_dependencies/ferveo/src/vss/pvss.rs` & `ferveo-0.1.7/local_dependencies/ferveo/src/vss/pvss.rs`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 use measure_time::print_time;
 use rand::RngCore;
 use serde::{Deserialize, Serialize};
 use serde_with::serde_as;
 use subproductdomain::fast_multiexp;
 use tpke::{
     prepare_combine_simple, refresh_private_key_share,
-    update_share_for_recovery, Ciphertext, DecryptionShareSimple,
-    DecryptionShareSimplePrecomputed, PrivateKeyShare,
+    update_share_for_recovery, Ciphertext, DecryptionSharePrecomputed,
+    DecryptionShareSimple, PrivateKeyShare,
 };
 
 use crate::{
     batch_to_projective_g1, batch_to_projective_g2, Error,
     PubliclyVerifiableDkg, Result,
 };
 
@@ -257,23 +257,23 @@
         &self,
         ciphertext: &Ciphertext<E>,
         aad: &[u8],
         validator_decryption_key: &E::ScalarField,
         validator_index: usize,
         domain_points: &[E::ScalarField],
         g_inv: &E::G1Prepared,
-    ) -> Result<DecryptionShareSimplePrecomputed<E>> {
+    ) -> Result<DecryptionSharePrecomputed<E>> {
         let private_key_share = self.decrypt_private_key_share(
             validator_decryption_key,
             validator_index,
         );
 
         let lagrange_coeffs = prepare_combine_simple::<E>(domain_points);
 
-        DecryptionShareSimplePrecomputed::new(
+        DecryptionSharePrecomputed::new(
             validator_index,
             validator_decryption_key,
             &private_key_share,
             ciphertext,
             aad,
             &lagrange_coeffs[validator_index],
             g_inv,
```

### Comparing `ferveo-0.1.6/local_dependencies/ferveo/src/vss.rs` & `ferveo-0.1.7/local_dependencies/ferveo/src/vss.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/local_dependencies/ferveo-common/src/keypair.rs` & `ferveo-0.1.7/local_dependencies/ferveo-common/src/keypair.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/local_dependencies/ferveo-common/src/lib.rs` & `ferveo-0.1.7/local_dependencies/ferveo-common/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/local_dependencies/ferveo-common/src/serialization.rs` & `ferveo-0.1.7/local_dependencies/ferveo-common/src/serialization.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/local_dependencies/subproductdomain/src/lib.rs` & `ferveo-0.1.7/local_dependencies/subproductdomain/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/Cargo.toml` & `ferveo-0.1.7/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "ferveo-python"
 authors = ["Piotr Roslaniec <p.roslaniec@gmail.com>"]
-version = "0.1.6"
+version = "0.1.7"
 edition = "2018"
 
 [lib]
 crate-type = ["cdylib"]
 name = "ferveo_py"
 
 [dependencies]
```

### Comparing `ferveo-0.1.6/LICENSE` & `ferveo-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.6/examples/server_api.py` & `ferveo-0.1.7/examples/server_api_precomputed.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 import os
 
 from ferveo_py import (
     encrypt,
-    combine_decryption_shares,
+    combine_decryption_shares_precomputed,
     decrypt_with_shared_secret,
     Keypair,
+    PublicKey,
     ExternalValidator,
     Transcript,
     Dkg,
-    AggregatedTranscript,
     Ciphertext,
+    UnblindingKey,
+    DecryptionSharePrecomputed,
+    AggregatedTranscript,
     DkgPublicKey,
+    DkgPublicParameters,
+    SharedSecret,
 )
 
 tau = 1
-security_threshold = 3
 shares_num = 4
+# In precomputed variant, security threshold must be equal to shares_num
+security_threshold = shares_num
 validator_keypairs = [Keypair.random() for _ in range(0, shares_num)]
 validators = [
     ExternalValidator(f"validator-{i}", keypair.public_key)
     for i, keypair in enumerate(validator_keypairs)
 ]
 
 # Each validator holds their own DKG instance and generates a transcript every
@@ -41,14 +47,16 @@
 dkg = Dkg(
     tau=tau,
     shares_num=shares_num,
     security_threshold=security_threshold,
     validators=validators,
     me=me,
 )
+# Let's say that we've only received `security_threshold` transcripts
+messages = messages[:security_threshold]
 pvss_aggregated = dkg.aggregate_transcripts(messages)
 assert pvss_aggregated.validate(dkg)
 
 # Server can persist transcripts and the aggregated transcript
 transcripts_ser = [bytes(transcript) for _, transcript in messages]
 _transcripts_deser = [Transcript.from_bytes(t) for t in transcripts_ser]
 agg_transcript_ser = bytes(pvss_aggregated)
@@ -75,37 +83,24 @@
     agg_transcript_deser = AggregatedTranscript.from_bytes(agg_transcript_ser)
     agg_transcript_deser.validate(dkg)
 
     # The ciphertext is obtained from the client
     ciphertext_deser = Ciphertext.from_bytes(ciphertext_ser)
 
     # Create a decryption share for the ciphertext
-    decryption_share = agg_transcript_deser.create_decryption_share(
+    decryption_share = agg_transcript_deser.create_decryption_share_precomputed(
         dkg, ciphertext, aad, validator_keypair
     )
     decryption_shares.append(decryption_share)
 
 # Now, the decryption share can be used to decrypt the ciphertext
 # This part is in the client API
 
-shared_secret = combine_decryption_shares(decryption_shares)
+# The client should have access to the public parameters of the DKG
+dkg_public_params_ser = bytes(dkg.public_params)
+dkg_public_params_deser = DkgPublicParameters.from_bytes(dkg_public_params_ser)
 
-plaintext = decrypt_with_shared_secret(ciphertext, aad, shared_secret, dkg.public_params)
-assert bytes(plaintext) == msg
+shared_secret = combine_decryption_shares_precomputed(decryption_shares)
 
-# Other serializable objects
+plaintext = decrypt_with_shared_secret(ciphertext, aad, shared_secret, dkg_public_params_deser)
+assert bytes(plaintext) == msg
 
-# Keypair
-keypair = Keypair.random()
-keypair_ser = bytes(keypair)
-keypair_deser = Keypair.from_bytes(keypair_ser)
-
-# DKG public key
-dkg_pk = dkg.final_key
-dkg_pk_ser = bytes(dkg_pk)
-dkg_pk_deser = DkgPublicKey.from_bytes(dkg_pk_ser)
-
-# Other utilities
-
-bytes_len = Keypair.secure_randomness_size()
-secure_randomness = os.urandom(bytes_len)
-keypair = Keypair.from_secure_randomness(secure_randomness)
```

### Comparing `ferveo-0.1.6/setup.py` & `ferveo-0.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ferveo",
     description="Ferveo DKG scheme",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.1.6",
+    version="0.1.7",
     author="Piotr Roslaniec",
     author_email="p.roslaniec@gmail.com",
     url="https://github.com/nucypher/ferveo/tree/master/ferveo-python",
     rust_extensions=[RustExtension(
         "ferveo._ferveo", binding=Binding.PyO3, debug=False)],
     packages=["ferveo"],
     package_data={
```

### Comparing `ferveo-0.1.6/src/lib.rs` & `ferveo-0.1.7/src/lib.rs`

 * *Files 24% similar despite different names*

```diff
@@ -22,42 +22,65 @@
     PyValueError::new_err(format!("{}", err))
 }
 
 #[pyfunction]
 pub fn encrypt(
     message: &[u8],
     aad: &[u8],
-    public_key: &DkgPublicKey,
+    dkg_public_key: &DkgPublicKey,
 ) -> PyResult<Ciphertext> {
     let rng = &mut thread_rng();
-    let ciphertext = ferveo::api::encrypt(message, aad, &public_key.0 .0, rng)
-        .map_err(map_py_error)?;
+    let ciphertext =
+        ferveo::api::encrypt(message, aad, &dkg_public_key.0 .0, rng)
+            .map_err(map_py_error)?;
     Ok(Ciphertext(ciphertext))
 }
 
 #[pyfunction]
-pub fn combine_decryption_shares(shares: Vec<DecryptionShare>) -> SharedSecret {
+pub fn combine_decryption_shares_simple(
+    shares: Vec<DecryptionShareSimple>,
+    dkg_public_params: &DkgPublicParameters,
+) -> SharedSecret {
     let shares = shares
         .iter()
         .map(|share| share.0.clone())
         .collect::<Vec<_>>();
-    SharedSecret(ferveo::api::share_combine_simple_precomputed(&shares))
+    let domain_points = &dkg_public_params.0.domain_points;
+    let lagrange_coefficients =
+        ferveo::api::prepare_combine_simple::<E>(&domain_points[..]);
+    let shared_secret = ferveo::api::share_combine_simple(
+        &shares[..],
+        &lagrange_coefficients[..],
+    );
+    SharedSecret(ferveo::api::SharedSecret(shared_secret))
+}
+
+#[pyfunction]
+pub fn combine_decryption_shares_precomputed(
+    shares: Vec<DecryptionSharePrecomputed>,
+) -> SharedSecret {
+    let shares = shares
+        .iter()
+        .map(|share| share.0.clone())
+        .collect::<Vec<_>>();
+    let shared_secret = ferveo::api::share_combine_precomputed(&shares[..]);
+    SharedSecret(ferveo::api::SharedSecret(shared_secret))
 }
 
 #[pyfunction]
 pub fn decrypt_with_shared_secret(
     ciphertext: &Ciphertext,
     aad: &[u8],
     shared_secret: &SharedSecret,
     dkg_params: &DkgPublicParameters,
 ) -> PyResult<Vec<u8>> {
     ferveo::api::decrypt_with_shared_secret(
         &ciphertext.0,
         aad,
-        &shared_secret.0,
+        &shared_secret.0 .0,
         &dkg_params.0.g1_inv,
     )
     .map_err(map_py_error)
 }
 
 #[pyclass(module = "ferveo")]
 #[derive(derive_more::AsRef)]
@@ -75,14 +98,26 @@
     }
 }
 
 #[pyclass(module = "ferveo")]
 #[derive(derive_more::AsRef)]
 pub struct SharedSecret(ferveo::api::SharedSecret);
 
+#[pymethods]
+impl SharedSecret {
+    #[staticmethod]
+    pub fn from_bytes(bytes: &[u8]) -> PyResult<Self> {
+        from_py_bytes(bytes).map(Self)
+    }
+
+    fn __bytes__(&self) -> PyResult<PyObject> {
+        to_py_bytes(self.0)
+    }
+}
+
 #[pyclass(module = "ferveo")]
 #[derive(derive_more::From, derive_more::AsRef)]
 pub struct Keypair(ferveo::api::Keypair<E>);
 
 #[pymethods]
 impl Keypair {
     #[staticmethod]
@@ -265,57 +300,92 @@
     }
 }
 
 #[pyclass(module = "ferveo")]
 #[derive(derive_more::From, derive_more::AsRef)]
 pub struct UnblindingKey(ferveo::api::UnblindingKey);
 
+#[pymethods]
+impl UnblindingKey {
+    #[staticmethod]
+    pub fn from_bytes(bytes: &[u8]) -> PyResult<Self> {
+        from_py_bytes(bytes).map(Self)
+    }
+
+    fn __bytes__(&self) -> PyResult<PyObject> {
+        to_py_bytes(self.0)
+    }
+}
+
 #[pyclass(module = "ferveo")]
 #[derive(Clone, derive_more::AsRef, derive_more::From)]
-pub struct DecryptionShare(ferveo::api::DecryptionShare);
+pub struct DecryptionShareSimple(ferveo::api::DecryptionShareSimple);
 
 #[pymethods]
-impl DecryptionShare {
+impl DecryptionShareSimple {
     #[staticmethod]
     pub fn from_bytes(bytes: &[u8]) -> PyResult<Self> {
         from_py_bytes(bytes).map(Self)
     }
 
     fn __bytes__(&self) -> PyResult<PyObject> {
         to_py_bytes(&self.0)
     }
 }
 
 #[pyclass(module = "ferveo")]
+#[derive(Clone, derive_more::AsRef, derive_more::From)]
+pub struct DecryptionSharePrecomputed(ferveo::api::DecryptionSharePrecomputed);
+
+#[pyclass(module = "ferveo")]
 #[derive(derive_more::From, derive_more::AsRef)]
 pub struct AggregatedTranscript(ferveo::api::AggregatedTranscript);
 
 #[pymethods]
 impl AggregatedTranscript {
     pub fn validate(&self, dkg: &Dkg) -> bool {
         self.0.validate(&dkg.0)
     }
 
-    pub fn create_decryption_share(
+    pub fn create_decryption_share_precomputed(
+        &self,
+        dkg: &Dkg,
+        ciphertext: &Ciphertext,
+        aad: &[u8],
+        validator_keypair: &Keypair,
+    ) -> PyResult<DecryptionSharePrecomputed> {
+        let decryption_share = self
+            .0
+            .create_decryption_share_precomputed(
+                &dkg.0,
+                &ciphertext.0,
+                aad,
+                &validator_keypair.0,
+            )
+            .map_err(map_py_error)?;
+        Ok(DecryptionSharePrecomputed(decryption_share))
+    }
+
+    pub fn create_decryption_share_simple(
         &self,
         dkg: &Dkg,
         ciphertext: &Ciphertext,
         aad: &[u8],
         validator_keypair: &Keypair,
-    ) -> PyResult<DecryptionShare> {
+    ) -> PyResult<DecryptionShareSimple> {
         let decryption_share = self
             .0
-            .create_decryption_share(
+            .create_decryption_share_simple(
                 &dkg.0,
                 &ciphertext.0,
                 aad,
                 &validator_keypair.0,
             )
             .map_err(map_py_error)?;
-        Ok(DecryptionShare(decryption_share))
+        Ok(DecryptionShareSimple(decryption_share))
     }
 
     #[staticmethod]
     pub fn from_bytes(bytes: &[u8]) -> PyResult<Self> {
         from_py_bytes(bytes).map(Self)
     }
 
@@ -324,21 +394,28 @@
     }
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
 fn ferveo_py(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(encrypt, m)?)?;
-    m.add_function(wrap_pyfunction!(combine_decryption_shares, m)?)?;
+    m.add_function(wrap_pyfunction!(combine_decryption_shares_simple, m)?)?;
+    m.add_function(wrap_pyfunction!(
+        combine_decryption_shares_precomputed,
+        m
+    )?)?;
     m.add_function(wrap_pyfunction!(decrypt_with_shared_secret, m)?)?;
     m.add_class::<Keypair>()?;
     m.add_class::<PublicKey>()?;
     m.add_class::<ExternalValidator>()?;
     m.add_class::<Transcript>()?;
     m.add_class::<Dkg>()?;
     m.add_class::<Ciphertext>()?;
     m.add_class::<UnblindingKey>()?;
-    m.add_class::<DecryptionShare>()?;
+    m.add_class::<DecryptionShareSimple>()?;
+    m.add_class::<DecryptionSharePrecomputed>()?;
     m.add_class::<AggregatedTranscript>()?;
     m.add_class::<DkgPublicKey>()?;
+    m.add_class::<DkgPublicParameters>()?;
+    m.add_class::<SharedSecret>()?;
     Ok(())
 }
```

### Comparing `ferveo-0.1.6/Cargo.lock` & `ferveo-0.1.7/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -742,14 +742,15 @@
 name = "ferveo"
 version = "0.1.1"
 dependencies = [
  "ark-bls12-381",
  "ark-ec",
  "ark-ff",
  "ark-poly",
+ "ark-serialize",
  "ark-std",
  "bincode",
  "criterion 0.3.6",
  "digest",
  "ferveo-common",
  "group-threshold-cryptography",
  "itertools",
@@ -777,15 +778,15 @@
  "rand_core 0.6.4",
  "serde",
  "serde_with",
 ]
 
 [[package]]
 name = "ferveo-python"
-version = "0.1.6"
+version = "0.1.7"
 dependencies = [
  "derive_more",
  "ferveo",
  "ferveo-common",
  "pyo3",
  "pyo3-build-config 0.17.3",
  "rand 0.8.5",
@@ -1949,14 +1950,15 @@
 
 [[package]]
 name = "tpke-wasm"
 version = "0.1.0-alpha.1"
 dependencies = [
  "ark-serialize",
  "console_error_panic_hook",
+ "ferveo",
  "ferveo-common",
  "getrandom 0.2.8",
  "group-threshold-cryptography",
  "js-sys",
  "rand 0.8.5",
  "rand_core 0.6.4",
  "serde",
```

### Comparing `ferveo-0.1.6/PKG-INFO` & `ferveo-0.1.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ferveo
-Version: 0.1.6
+Version: 0.1.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Author: Piotr Roslaniec <p.roslaniec@gmail.com>
 Author-email: Piotr Roslaniec <p.roslaniec@gmail.com>
 Requires-Python: >=3.7
```

