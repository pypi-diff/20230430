# Comparing `tmp/pyscemu-0.1.2.tar.gz` & `tmp/pyscemu-0.1.3.tar.gz`

## Comparing `pyscemu-0.1.2.tar` & `pyscemu-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 pyscemu-0.1.2/Cargo.toml
--rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.1.2/.github/workflows/CI.yml
--rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.1.2/.gitignore
--rw-r--r--   0     1000     1000     9727 2023-04-29 19:27:52.000000 pyscemu-0.1.2/README.md
--rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.1.2/examples/xloader_dexor.py
--rw-r--r--   0     1000     1000      409 2023-04-29 18:27:50.000000 pyscemu-0.1.2/examples/xloader_keygen.py
--rw-r--r--   0     1000     1000      369 2023-04-28 16:18:25.000000 pyscemu-0.1.2/pyproject.toml
--rw-r--r--   0     1000     1000    24020 2023-04-29 18:40:24.000000 pyscemu-0.1.2/src/lib.rs
--rw-r--r--   0     1000     1000    32749 2023-04-29 21:19:59.000000 pyscemu-0.1.2/Cargo.lock
--rw-r--r--   0        0        0    10053 1970-01-01 00:00:00.000000 pyscemu-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 pyscemu-0.1.3/Cargo.toml
+-rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.1.3/.github/workflows/CI.yml
+-rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.1.3/.gitignore
+-rw-r--r--   0     1000     1000     9899 2023-04-30 10:55:32.000000 pyscemu-0.1.3/README.md
+-rw-r--r--   0     1000     1000      723 2023-04-30 12:20:49.000000 pyscemu-0.1.3/examples/raccoon_strings.py
+-rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.1.3/examples/xloader_dexor.py
+-rw-r--r--   0     1000     1000      409 2023-04-29 18:27:50.000000 pyscemu-0.1.3/examples/xloader_keygen.py
+-rw-r--r--   0     1000     1000      369 2023-04-28 16:18:25.000000 pyscemu-0.1.3/pyproject.toml
+-rw-r--r--   0     1000     1000    24019 2023-04-30 12:21:37.000000 pyscemu-0.1.3/src/lib.rs
+-rw-r--r--   0     1000     1000    32749 2023-04-30 12:23:14.000000 pyscemu-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0    10225 1970-01-01 00:00:00.000000 pyscemu-0.1.3/PKG-INFO
```

### Comparing `pyscemu-0.1.2/.github/workflows/CI.yml` & `pyscemu-0.1.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.2/.gitignore` & `pyscemu-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.2/README.md` & `pyscemu-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 # PYSCEMU
 
 ## Install
+```bash
 pip install --upgrade pip
 pip3 install --upgrade pip
 curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
 pip install pyscemu
+```
 
+## Mac Install
+same procedure, if there is a problem with !tapi-tbd the solution is:
+```bash
+sudo xcode-select --switch /Library/Developer/CommandLineTools
+```
 
 ## Download maps
 download maps32 from releases or maps64 better from git:
 https://github.com/sha0coder/scemu
 
 releases:
```

### Comparing `pyscemu-0.1.2/examples/xloader_dexor.py` & `pyscemu-0.1.3/examples/xloader_dexor.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.2/src/lib.rs` & `pyscemu-0.1.3/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -486,16 +486,16 @@
                 return Err(PyValueError::new_err("reading on non allocated address"));
             }
         }
     }
 
 
     /// read a byte from a memory address.
-    fn read_byte(&self, addr:u64) -> PyResult<u16> {
-        match self.emu.maps.read_word(addr) {
+    fn read_byte(&self, addr:u64) -> PyResult<u8> {
+        match self.emu.maps.read_byte(addr) {
             Some(v) => return Ok(v),
             None => {
                 return Err(PyValueError::new_err("reading on non allocated address"));
             }
         }
     }
```

### Comparing `pyscemu-0.1.2/Cargo.lock` & `pyscemu-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -684,15 +684,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyscemu"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "libscemu",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
```

### Comparing `pyscemu-0.1.2/PKG-INFO` & `pyscemu-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Metadata-Version: 2.1
 Name: pyscemu
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # PYSCEMU
 
 ## Install
+```bash
 pip install --upgrade pip
 pip3 install --upgrade pip
 curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
 pip install pyscemu
+```
 
+## Mac Install
+same procedure, if there is a problem with !tapi-tbd the solution is:
+```bash
+sudo xcode-select --switch /Library/Developer/CommandLineTools
+```
 
 ## Download maps
 download maps32 from releases or maps64 better from git:
 https://github.com/sha0coder/scemu
 
 releases:
```

