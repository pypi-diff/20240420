# Comparing `tmp/dogma_rust-0.2.4.tar.gz` & `tmp/dogma_rust-0.2.5.tar.gz`

## Comparing `dogma_rust-0.2.4.tar` & `dogma_rust-0.2.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 dogma_rust-0.2.4/Cargo.toml
--rw-r--r--   0    23269        0     3526 2024-04-10 03:45:24.000000 dogma_rust-0.2.4/.github/workflows/CI.yml
--rw-r--r--   0    23269        0      686 2024-04-10 03:45:24.000000 dogma_rust-0.2.4/.gitignore
--rw-r--r--   0    23269        0      377 2024-04-10 03:45:24.000000 dogma_rust-0.2.4/README.md
--rw-r--r--   0    23269        0     2305 2024-04-10 04:14:26.000000 dogma_rust-0.2.4/src/data.rs
--rw-r--r--   0    23269        0     5185 2024-04-10 08:10:45.000000 dogma_rust-0.2.4/src/fasta.rs
--rw-r--r--   0    23269        0     5893 2024-04-10 08:04:45.000000 dogma_rust-0.2.4/src/lib.rs
--rw-r--r--   0    23269        0     2708 2024-04-10 03:45:24.000000 dogma_rust-0.2.4/src/parallel.rs
--rw-r--r--   0    23269        0    19296 2024-04-10 04:02:22.000000 dogma_rust-0.2.4/Cargo.lock
--rw-r--r--   0    23269        0      538 2024-04-10 03:45:24.000000 dogma_rust-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 dogma_rust-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 dogma_rust-0.2.5/Cargo.toml
+-rw-r--r--   0    23269        0     3526 2024-04-10 03:45:24.000000 dogma_rust-0.2.5/.github/workflows/CI.yml
+-rw-r--r--   0    23269        0      686 2024-04-10 03:45:24.000000 dogma_rust-0.2.5/.gitignore
+-rw-r--r--   0    23269        0      377 2024-04-10 03:45:24.000000 dogma_rust-0.2.5/README.md
+-rw-r--r--   0    23269        0     2405 2024-04-19 17:16:04.000000 dogma_rust-0.2.5/src/data.rs
+-rw-r--r--   0    23269        0     5191 2024-04-19 17:27:38.000000 dogma_rust-0.2.5/src/fasta.rs
+-rw-r--r--   0    23269        0     5877 2024-04-19 18:38:50.000000 dogma_rust-0.2.5/src/lib.rs
+-rw-r--r--   0    23269        0     3125 2024-04-19 17:54:10.000000 dogma_rust-0.2.5/src/parallel.rs
+-rw-r--r--   0    23269        0    19296 2024-04-19 17:56:30.000000 dogma_rust-0.2.5/Cargo.lock
+-rw-r--r--   0    23269        0      538 2024-04-10 03:45:24.000000 dogma_rust-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 dogma_rust-0.2.5/PKG-INFO
```

### Comparing `dogma_rust-0.2.4/.github/workflows/CI.yml` & `dogma_rust-0.2.5/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `dogma_rust-0.2.4/.gitignore` & `dogma_rust-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dogma_rust-0.2.4/src/data.rs` & `dogma_rust-0.2.5/src/data.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use crate::parallel::parallel_concatenate_buffers;
-use std::borrow::{Borrow, Cow};
+use std::borrow::Cow;
 use numpy::{PyArrayDescrMethods, PyUntypedArray, PyUntypedArrayMethods};
 use rayon::prelude::*;
-use pyo3::prelude::*;
+use pyo3::{exceptions::PyValueError, prelude::*};
 
 pub struct AwkwardArray<'a, T>
 where T: Clone {
     pub content: Cow<'a, [T]>,
     pub cu_seqlens: Cow<'a, [isize]>,
 }
 
@@ -16,52 +16,52 @@
         AwkwardArray {
             content: content.into(),
             cu_seqlens: cu_seqlens.into(),
         }
     }
 
     pub fn parallel_concatenate(arrs: &[&AwkwardArray<'_, T>]) -> AwkwardArray<'static, T> {
-        let content_buffers = arrs.iter().copied().map(|arr| arr.content.borrow()).collect::<Vec<_>>();
+        let content_buffers: Vec<&[T]> = arrs.iter().copied().map(|arr| arr.content.as_ref()).collect();
         let (cat_content, _) = parallel_concatenate_buffers(&content_buffers);
 
-        let cu_seqlen_offsets = arrs.iter().copied().scan(0, |acc, arr| {
+        let cu_seqlen_offsets: Vec<isize> = arrs.iter().copied().scan(0, |acc, arr| {
             let start = *acc;
             *acc += arr.cu_seqlens.last().copied().unwrap_or(0);
             Some(start)
-        }).collect::<Vec<_>>();
+        }).collect();
 
         let shifted_cu_seqlens = arrs.par_iter().zip(cu_seqlen_offsets).map(|(arr, offset)| {
             if offset == 0 {
                 arr.cu_seqlens.to_vec()
             } else {
                 let mut shifted = (&arr.cu_seqlens[1..]).to_vec(); // Skip the first element
                 shifted.iter_mut().for_each(|cu_seqlen| *cu_seqlen += offset);
                 shifted
             }
         }).collect::<Vec<_>>();
 
-        let shifted_cu_seqlens_refs = shifted_cu_seqlens.iter().map(|cu_seqlens| {
+        let shifted_cu_seqlens_refs: Vec<&[isize]> = shifted_cu_seqlens.iter().map(|cu_seqlens| {
             cu_seqlens.as_slice()
-        }).collect::<Vec<_>>();
+        }).collect();
 
         let (out_cu_seqlens, _) = parallel_concatenate_buffers(&shifted_cu_seqlens_refs);
 
 
         AwkwardArray::new(cat_content, out_cu_seqlens)
     }
 }
 
 
 pub trait TreatAsByteSlice<'a, T> {
-    fn as_slice(&self) -> &'a [T];
+    unsafe fn as_slice(&self) -> PyResult<&'a [T]>;
 }
 
 impl<'a, T> TreatAsByteSlice<'a, T> for Bound<'a, PyUntypedArray> {
-    fn as_slice(&self) -> &'a [T] {
-        unsafe {
-            assert!(self.is_contiguous());
-            let arr = *self.as_array_ptr();
-            let dtype_width = self.dtype().itemsize();
-            std::slice::from_raw_parts(arr.data as *const T, self.len() * dtype_width as usize / std::mem::size_of::<T>())
+    unsafe fn as_slice(&self) -> PyResult<&'a [T]> {
+        if !self.is_contiguous(){
+            return Err(PyValueError::new_err("Array is not contiguous"));
         }
+        let arr = *self.as_array_ptr();
+        let dtype_width = self.dtype().itemsize();
+        Ok(std::slice::from_raw_parts(arr.data as *const T, self.len() * dtype_width as usize / std::mem::size_of::<T>()))
     }
 }
```

### Comparing `dogma_rust-0.2.4/src/fasta.rs` & `dogma_rust-0.2.5/src/fasta.rs`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,14 @@
 #[cfg(test)]
 mod tests {
     use super::*;
 
     #[test]
     fn test_big_fasta() {
         let fasta_path = "/lfs/local/0/roed/projects/dogma-data/fasta_data/result_rep_seq.fasta";
-        let result = parse_fasta(fasta_path, &[1, 2, 3, 4, 5]);
+        let result = parse_fasta(fasta_path, &[1, 2, 3, 4, 5], true);
 
         println!("Parsed fasta with {} sequences and {} tokens", result.sequences.cu_seqlens.len() - 1, result.sequences.content.len());
         println!("Got the following taxon ids: {:?}", result.taxon_ids);
         std::hint::black_box(&result);
     }
 }
```

### Comparing `dogma_rust-0.2.4/src/lib.rs` & `dogma_rust-0.2.5/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,14 @@
     Ok((a + b).to_string())
 }
 
 impl<'a, T: Clone + Sync> From<Bound<'a, PyTuple>> for AwkwardArray<'a, T> {
     fn from(value: Bound<'a, PyTuple>) -> Self {
         let _content = value.get_item(0);
         todo!()
-        // AwkwardArray {
-
-        // }
     }
 }
 
 #[pyfunction]
 fn parse_fasta<'py>(py: Python<'py>, path: &str, mapping: PyReadonlyArray1<'py, u8>, is_rna: bool) -> PyResult<(Bound<'py, PyArray1<u8>>, Bound<'py, PyArray1<isize>>, Bound<'py, PyArray1<u64>>)> {
     let mapping = mapping.as_slice()?;
 
@@ -41,16 +38,16 @@
     let awkwards: Vec<AwkwardArray<_>> = arrays.iter().map(|obj| {
         let tuple = obj.downcast::<PyTuple>()?;
         let tup_content = tuple.get_item(0)?;
         let tup_cu_seqlens = tuple.get_item(1)?;
         let content = tup_content.downcast::<PyUntypedArray>()?;
         let cu_seqlens = tup_cu_seqlens.downcast::<PyUntypedArray>()?;
 
-        let content: &[u8] = content.as_slice();
-        let cu_seqlens: &[isize] = cu_seqlens.as_slice();
+        let content: &[u8] = unsafe { content.as_slice() }?;
+        let cu_seqlens: &[isize] = unsafe { cu_seqlens.as_slice() }?;
         Ok(AwkwardArray::<u8>::new(content, cu_seqlens))
     }).collect::<PyResult<_>>()?;
 
     let awkward_refs = awkwards.iter().collect::<Vec<_>>();
 
     let AwkwardArray {content, cu_seqlens} = AwkwardArray::parallel_concatenate(&awkward_refs);
```

### Comparing `dogma_rust-0.2.4/src/parallel.rs` & `dogma_rust-0.2.5/src/parallel.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,58 @@
 use rayon::prelude::*;
 
 struct SendPtr<T>(*mut T);
 
 // unsafe impl<T> Send for SendPtr<T> {}
 unsafe impl<T> Sync for SendPtr<T> {}
 
-pub fn parallel_concatenate_buffers<T: Sync>(bufs: &[&[T]]) -> (Vec<T>, Vec<usize>) {
-    let out_buf_size = bufs.iter().map(|&buf| buf.len()).sum();
+pub trait ParallelConcatenate<T>{
+    fn parallel_concatenate(self) -> (Vec<T>, Vec<usize>);
+}
+
+impl<T, C> ParallelConcatenate<T> for C
+where
+C: ParallelIterator,
+T: Sync,
+C::Item: AsRef<[T]> + Sync, {
+    fn parallel_concatenate(self) -> (Vec<T>, Vec<usize>) {
+        let bufs: Vec<C::Item> = self.collect();
+        parallel_concatenate_buffers(&bufs)
+    }
+}
+
+pub fn parallel_concatenate_buffers<T: Sync>(bufs: &[impl AsRef<[T]> + Sync]) -> (Vec<T>, Vec<usize>) {
+    let out_buf_size = bufs.iter().map(|buf| buf.as_ref().len()).sum();
 
     let mut out_buf = Vec::with_capacity(out_buf_size);
     unsafe {out_buf.set_len(out_buf_size);}
     let data = SendPtr(out_buf.as_mut_ptr());
 
-    let starting_indices = bufs.iter().scan(0, |acc, buf| {
+    let starting_indices: Vec<usize> = bufs.iter().scan(0, |acc, buf| {
         let start = *acc;
-        *acc += buf.len();
+        *acc += buf.as_ref().len();
         Some(start)
-    }).collect::<Vec<_>>();
+    }).collect();
 
-    starting_indices.par_iter().zip(bufs).for_each(|(&start, &buf)| {
-        let buf_len = buf.len();
-        let buf_ptr = buf.as_ptr();
+    starting_indices.par_iter().zip(bufs).for_each(|(&start, buf)| {
+        let buf_len = buf.as_ref().len();
+        let buf_ptr = buf.as_ref().as_ptr();
         unsafe {
             let send_dest = &data;
             let dest_base: *mut T = send_dest.0;
             let dest: *mut T = dest_base.add(start);
             let src = buf_ptr;
             std::ptr::copy_nonoverlapping(src, dest, buf_len);
         }
     });
     
     (out_buf, starting_indices)
 }
 
 
-
 #[cfg(test)]
 mod tests {
     use std::hint::black_box;
 
     use super::*;
     use rand::prelude::*;
```

### Comparing `dogma_rust-0.2.4/Cargo.lock` & `dogma_rust-0.2.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 name = "crossbeam-utils"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
 name = "dogma-rust"
-version = "0.2.4"
+version = "0.2.5"
 dependencies = [
  "anyhow",
  "chrono",
  "eyre",
  "num-bigint",
  "numpy",
  "pyo3",
```

### Comparing `dogma_rust-0.2.4/pyproject.toml` & `dogma_rust-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dogma_rust-0.2.4/PKG-INFO` & `dogma_rust-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dogma_rust
-Version: 0.2.4
+Version: 0.2.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: homepage, https://github.com/marcelroed/dogma-data
 Project-URL: repository, https://github.com/marcelroed/dogma-data
```

