# Comparing `tmp/rs_distances-0.5.0.tar.gz` & `tmp/rs_distances-0.6.0.tar.gz`

## Comparing `rs_distances-0.5.0.tar` & `rs_distances-0.6.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 rs_distances-0.5.0/Cargo.toml
--rw-r--r--   0        0        0     2807 2023-06-03 05:19:15.000000 rs_distances-0.5.0/.github/workflows/CI.yml
--rw-r--r--   0        0        0      764 2023-06-03 16:25:17.000000 rs_distances-0.5.0/.gitignore
--rw-r--r--   0        0        0     2313 2023-06-03 16:58:44.000000 rs_distances-0.5.0/README.md
--rw-r--r--   0        0        0      914 2023-06-03 18:38:08.000000 rs_distances-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       13 2023-06-04 16:25:45.000000 rs_distances-0.5.0/src/lib.rs
--rw-r--r--   0        0        0       13 2023-06-04 16:17:27.000000 rs_distances-0.5.0/src/spkd/mod.rs
--rw-r--r--   0        0        0     4872 2023-06-05 02:34:35.000000 rs_distances-0.5.0/src/spkd/spkd.rs
--rw-r--r--   0        0        0    65826 2023-06-05 03:28:05.000000 rs_distances-0.5.0/Cargo.lock
--rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 rs_distances-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 rs_distances-0.6.0/Cargo.toml
+-rw-r--r--   0        0        0     2807 2023-06-03 05:19:15.000000 rs_distances-0.6.0/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      764 2023-06-03 16:25:17.000000 rs_distances-0.6.0/.gitignore
+-rw-r--r--   0        0        0     2313 2023-06-03 16:58:44.000000 rs_distances-0.6.0/README.md
+-rw-r--r--   0        0        0      914 2023-06-03 18:38:08.000000 rs_distances-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-06-04 16:25:45.000000 rs_distances-0.6.0/src/lib.rs
+-rw-r--r--   0        0        0       13 2023-06-05 11:46:40.000000 rs_distances-0.6.0/src/spkd/mod.rs
+-rw-r--r--   0        0        0     5506 2023-06-05 22:38:31.000000 rs_distances-0.6.0/src/spkd/spkd.rs
+-rw-r--r--   0        0        0    66783 2023-06-05 23:11:08.000000 rs_distances-0.6.0/Cargo.lock
+-rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 rs_distances-0.6.0/PKG-INFO
```

### Comparing `rs_distances-0.5.0/.github/workflows/CI.yml` & `rs_distances-0.6.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rs_distances-0.5.0/.gitignore` & `rs_distances-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rs_distances-0.5.0/README.md` & `rs_distances-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `rs_distances-0.5.0/pyproject.toml` & `rs_distances-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rs_distances-0.5.0/src/spkd/spkd.rs` & `rs_distances-0.6.0/src/spkd/spkd.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-
-use ndarray::{Array, Array1, Array3, s, ArrayBase, OwnedRepr, Dim};
+use ndarray::Array2;
+use ndarray::{s, Array1, Array3, ArrayBase, ArrayView3, Dim, OwnedRepr};
+use numpy::{IntoPyArray, PyArray1, PyArray3};
 use pyo3::{prelude::*, types::PyList};
-use numpy::{PyArray3, IntoPyArray, PyArray1};
 
-pub fn iterate_spiketrains(scr: &mut Array3<f64>, sd: &Array3<f64>)  {
+pub fn iterate_spiketrains(scr: &mut Array3<f64>, sd: &ArrayView3<f64>) {
     let (num_qvals, num_spikes_xii, num_spikes_xjj) = scr.dim();
     for xii in 1..num_spikes_xii {
         for xjj in 1..num_spikes_xjj {
             for q in 0..num_qvals {
                 let a = scr[[q, xii - 1, xjj]] + 1.0;
                 let b = scr[[q, xii, xjj - 1]] + 1.0;
                 let c = scr[[q, xii - 1, xjj - 1]] + sd[[q, xii - 1, xjj - 1]];
@@ -15,119 +15,144 @@
                 scr[[q, xii, xjj]] = a.min(b.min(c));
             }
         }
     }
 }
 
 #[pyfunction]
-fn iterate_spiketrains_impl(py: Python, scr: &PyArray3<f64>, sd: &PyArray3<f64>)  -> PyResult<PyObject> {
-
+fn iterate_spiketrains_impl(
+    py: Python,
+    scr: &PyArray3<f64>,
+    sd: &PyArray3<f64>,
+) -> PyResult<PyObject> {
     let mut scr: Array3<f64> = scr.to_owned_array();
     let sd: Array3<f64> = sd.to_owned_array();
 
-    iterate_spiketrains(&mut scr, &sd);
+    iterate_spiketrains(&mut scr, &sd.view());
 
     // Convert the result to a PyArray
-    let res = scr.into_pyarray(py).to_owned();
+    let res: Py<numpy::PyArray<f64, Dim<[usize; 3]>>> = scr.into_pyarray(py).to_owned();
     Ok(res.into())
 }
 
-
-pub fn calculate_spkd(cspks: &Vec<Array1<f64>>, qvals: &ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>>, _res: Option<f64>)  -> ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>> {
-
+pub fn calculate_spkd(
+    cspks: &Vec<Array1<f64>>,
+    qvals: &ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>>,
+    _res: Option<f64>,
+) -> ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>> {
     let numt: usize = cspks.len(); // number of spike trains
-    let num_qvals = qvals.len(); // number of q values
+    let num_qvals: usize = qvals.len(); // number of q values
 
-    let mut d = Array3::<f64>::zeros((numt, numt, num_qvals));
+    let mut d: ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>> =
+        Array3::<f64>::zeros((numt, numt, num_qvals));
 
-    for xi in 0..numt - 1 { // if there are 40 spike trains, xi will be 0..39
-        for xj in xi + 1..numt { // if there are 40 spike trains, xj will be 1..39
-
-            let curcounts_xi = cspks[xi].len();
-            let curcounts_xj = cspks[xj].len();
+    for xi in 0..numt - 1 {
+        for xj in xi + 1..numt {
+            let curcounts_xi: usize = cspks[xi].len();
+            let curcounts_xj: usize = cspks[xj].len();
 
             if curcounts_xi != 0 && curcounts_xj != 0 {
-                let spk_train_a = &cspks[xi];
-                let spk_train_b = &cspks[xj];
+                let mut outer_diff = cspks[xi].clone().into_shape((curcounts_xi, 1)).unwrap()
+                    - cspks[xj].clone().into_shape((1, curcounts_xj)).unwrap();
+
+                outer_diff.mapv_inplace(|x| x.abs());
+
+                let sd = qvals.clone().into_shape((qvals.len(), 1, 1)).unwrap() * &outer_diff;
 
-                let spk_train_a_offset = spk_train_a.clone();
-                
+                let mut scr =
+                    Array3::<f64>::zeros((qvals.len(), curcounts_xi + 1, curcounts_xj + 1));
+                 let scr_len = scr.len();
 
-                let outer_diff = Array::from_shape_fn((spk_train_a_offset.len(), spk_train_b.len()), |(i, j)| {
-                    (spk_train_a_offset[i] - spk_train_b[j]).abs()
-                });
+                scr.slice_mut(s![.., 1.., 0])
+                    .assign(&Array2::from_elem((qvals.len(), curcounts_xi), 1.0));
+                scr.slice_mut(s![.., 0, 1..])
+                    .assign(&Array2::from_elem((qvals.len(), curcounts_xj), 1.0));
 
-                let sd = qvals.broadcast((num_qvals, spk_train_a_offset.len(), spk_train_b.len())).unwrap()
-                    .to_owned() * &outer_diff;
+                iterate_spiketrains(&mut scr, &sd.view());
 
-                let mut scr = Array::from_elem((num_qvals, curcounts_xi + 1, curcounts_xj + 1), 0.0);
-                scr.slice_mut(s![.., 1.., 0]).assign(&(1..=curcounts_xi).map(|x: usize| x as f64).collect::<Array1<_>>());
-                scr.slice_mut(s![.., 0, 1..]).assign(&Array::from_shape_fn((1, curcounts_xj), |(_, j)| (j + 1) as f64));
+                println!("scr's shape: {:?}", scr.dim());
+                // println!("d's slice shape: {:?}", d.slice(s![xi, xj, ..]).dim());
+               
+                d.slice_mut(s![xi, xj, ..]).assign(&scr.into_shape(scr_len).unwrap());
 
-                iterate_spiketrains(&mut scr, &sd);
-      
             } else {
-                d.slice_mut(s![xi, xj, ..]).fill(curcounts_xi.max(curcounts_xj) as f64);
+                println!("d's shape: {:?}", d.dim());
+                d.slice_mut(s![xi, xj, ..])
+                    .fill(curcounts_xi.max(curcounts_xj) as f64);
             }
         }
     }
-    d.mapv_into(|val| val.max(0.0))
-}
 
-// a function with a signature but without docs. Both blank lines after the `--` are mandatory.
+    // Transpose d
+    d = d.permuted_axes([1, 0, 2]);
+    d.mapv_inplace(|x| x.max(0.0));
+    d
+}
 
-/// sub(a, b, /)
-/// --
-///
-///
 #[pyfunction]
-fn calculate_spkd_impl(py: Python, cspks: &PyList, qvals: &PyArray1<f64>, res: Option<f64>) -> PyResult<PyObject> {
-    let cspks: Vec<Array1<f64>> = cspks.into_iter().map(|pyarray| {
-        let numpy_array: &PyArray1<f64> = pyarray.extract()?;
-        Ok(numpy_array.to_owned_array())
-    }).collect::<PyResult<_>>()?;
+fn calculate_spkd_impl(
+    py: Python,
+    cspks: &PyList,
+    qvals: &PyArray1<f64>,
+    res: Option<f64>,
+) -> PyResult<PyObject> {
+    let cspks: Vec<Array1<f64>> = cspks
+        .into_iter()
+        .map(|pyarray| {
+            let numpy_array: &PyArray1<f64> = pyarray.extract()?;
+            Ok(numpy_array.to_owned_array())
+        })
+        .collect::<PyResult<_>>()?;
 
     let qvals: Array1<f64> = qvals.to_owned_array();
-    let numqvals = qvals.len();
-    let q_reshaped = qvals.into_shape((numqvals, 1, 1)).unwrap();
+    let numqvals: usize = qvals.len();
+    let q_reshaped: ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>> =
+        qvals.into_shape((numqvals, 1, 1)).unwrap();
 
     // Assume calculate_spkd returns ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>>
-    let d = calculate_spkd(&cspks, &q_reshaped, res);
-    
+    let d: ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>> = calculate_spkd(&cspks, &q_reshaped, res);
+
     // Convert the ArrayBase to a PyArray
-    let py_array = d.into_pyarray(py);
+    let py_array: &numpy::PyArray<f64, Dim<[usize; 3]>> = d.into_pyarray(py);
 
     // Convert the PyArray to a PyObject
     Ok(py_array.to_object(py))
 }
 
 #[pymodule]
 fn rs_distances(_py: Python, m: &PyModule) -> PyResult<()> {
-    m.add_wrapped(wrap_pyfunction!(calculate_spkd_impl)).unwrap();
-    m.add_wrapped(wrap_pyfunction!(iterate_spiketrains_impl)).unwrap();
+    m.add_wrapped(wrap_pyfunction!(calculate_spkd_impl))
+        .unwrap();
+    m.add_wrapped(wrap_pyfunction!(iterate_spiketrains_impl))
+        .unwrap();
     Ok(())
 }
 
 #[cfg(test)]
 mod tests {
-    use ndarray::{ArrayBase, OwnedRepr, Dim};
-
     use super::*;
+    use env_logger::Builder;
+    use log::LevelFilter;
+    use ndarray::{ArrayBase, Dim, OwnedRepr};
+    use std::env;
 
     #[test]
     fn test_calculate_spkd() {
+        env::set_var("RUST_LOG", "debug");
+        Builder::new().filter_level(LevelFilter::Debug).init();
+
         // Mock data - list of 1D np.ndarrays, 3 spike trains
         let mut mock_data: Vec<ArrayBase<OwnedRepr<f64>, Dim<[usize; 1]>>> = vec![
-        ArrayBase::from(vec![0.1, 0.15, 0.2, 0.25, 0.3]),
-        ArrayBase::from(vec![0.35, 0.4, 0.45, 0.5, 0.55]),
-        ArrayBase::from(vec![0.6, 0.65, 0.7, 0.75, 0.8]),
-    ];
-        
+            ArrayBase::from(vec![0.1, 0.15, 0.2, 0.25, 0.3]),
+            ArrayBase::from(vec![0.35, 0.4, 0.45, 0.5, 0.55]),
+            ArrayBase::from(vec![0.6, 0.65, 0.7, 0.75, 0.8]),
+        ];
+
         // simulate a view of data given from a numpy spike train
         let qvals = Array1::from(vec![1.0, 2.0, 3.0]);
 
         let numqvals = qvals.len();
         let q_reshaped = qvals.into_shape((numqvals, 1, 1)).unwrap();
 
         calculate_spkd(&mut mock_data, &q_reshaped, Option::None);
     }
-}
+}
```

### Comparing `rs_distances-0.5.0/Cargo.lock` & `rs_distances-0.6.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -89,14 +89,25 @@
 [[package]]
 name = "anyhow"
 version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
+name = "atty"
+version = "0.2.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
+dependencies = [
+ "hermit-abi 0.1.19",
+ "libc",
+ "winapi",
+]
+
+[[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "base64"
@@ -618,14 +629,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "env_logger"
+version = "0.9.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a12e6657c4c97ebab115a42dcee77225f7f482cdd841cf7088c657a42e9e00e7"
+dependencies = [
+ "atty",
+ "humantime",
+ "log",
+ "regex",
+ "termcolor",
+]
+
+[[package]]
 name = "errno"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
@@ -767,14 +791,23 @@
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
+version = "0.1.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
+dependencies = [
+ "libc",
+]
+
+[[package]]
+name = "hermit-abi"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
 
@@ -790,14 +823,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5444c27eef6923071f7ebcc33e3444508466a76f7a2b93da00ed6e19f30c1ddb"
 dependencies = [
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "humantime"
+version = "2.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
+
+[[package]]
 name = "idna"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e14ddfc70884202db2244c223200c204c2bda1bc6e0998d11b5e024d657209e6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
@@ -1632,17 +1671,19 @@
  "untrusted",
  "web-sys",
  "winapi",
 ]
 
 [[package]]
 name = "rs-distances"
-version = "0.5.0"
+version = "0.6.0"
 dependencies = [
+ "env_logger",
  "itertools",
+ "log",
  "maturin",
  "ndarray",
  "numpy",
  "pyo3",
 ]
 
 [[package]]
```

### Comparing `rs_distances-0.5.0/PKG-INFO` & `rs_distances-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rs-distances
-Version: 0.5.0
+Version: 0.6.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: A Python module implemented in Rust for efficient calculations
 Author-email: Flynn OConnell <flynnoconnell@gmail.com>
 License: MIT
 Requires-Python: >=3.7
```

