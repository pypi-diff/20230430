# Comparing `tmp/yroom-0.0.3.tar.gz` & `tmp/yroom-0.0.4.tar.gz`

## Comparing `yroom-0.0.3.tar` & `yroom-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      315 1970-01-01 00:00:00.000000 yroom-0.0.3/Cargo.toml
--rw-r--r--   0     1001      123     2772 2023-04-20 13:59:19.000000 yroom-0.0.3/.github/workflows/release.yml
--rw-r--r--   0     1001      123     1169 2023-04-20 13:59:19.000000 yroom-0.0.3/.github/workflows/test.yml
--rw-r--r--   0     1001      123       40 2023-04-20 13:59:19.000000 yroom-0.0.3/.gitignore
--rw-r--r--   0     1001      123     1083 2023-04-20 13:59:19.000000 yroom-0.0.3/LICENSE
--rw-r--r--   0     1001      123      141 2023-04-20 13:59:19.000000 yroom-0.0.3/README.md
--rw-r--r--   0     1001      123       10 2023-04-20 14:00:04.000000 yroom-0.0.3/dist/yroom-0.0.3.tar.gz
--rw-r--r--   0     1001      123      736 2023-04-20 13:59:19.000000 yroom-0.0.3/pyproject.toml
--rw-r--r--   0     1001      123      272 2023-04-20 13:59:19.000000 yroom-0.0.3/src/lib.rs
--rw-r--r--   0     1001      123    12399 2023-04-20 13:59:19.000000 yroom-0.0.3/src/roomsync.rs
--rw-r--r--   0     1001      123     2392 2023-04-20 13:59:19.000000 yroom-0.0.3/tests/test_yroom.py
--rw-r--r--   0     1001      123     3421 2023-04-20 13:59:19.000000 yroom-0.0.3/yroom.pyi
--rw-r--r--   0     1001      123    13697 2023-04-20 13:59:19.000000 yroom-0.0.3/Cargo.lock
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 yroom-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      315 1970-01-01 00:00:00.000000 yroom-0.0.4/Cargo.toml
+-rw-r--r--   0     1001      123     2772 2023-04-30 12:23:26.000000 yroom-0.0.4/.github/workflows/release.yml
+-rw-r--r--   0     1001      123     1174 2023-04-30 12:23:26.000000 yroom-0.0.4/.github/workflows/test.yml
+-rw-r--r--   0     1001      123       40 2023-04-30 12:23:26.000000 yroom-0.0.4/.gitignore
+-rw-r--r--   0     1001      123     1083 2023-04-30 12:23:26.000000 yroom-0.0.4/LICENSE
+-rw-r--r--   0     1001      123      141 2023-04-30 12:23:26.000000 yroom-0.0.4/README.md
+-rw-r--r--   0     1001      123       10 2023-04-30 12:24:29.000000 yroom-0.0.4/dist/yroom-0.0.4.tar.gz
+-rw-r--r--   0     1001      123      746 2023-04-30 12:23:26.000000 yroom-0.0.4/pyproject.toml
+-rw-r--r--   0     1001      123      272 2023-04-30 12:23:26.000000 yroom-0.0.4/src/lib.rs
+-rw-r--r--   0     1001      123    21486 2023-04-30 12:23:26.000000 yroom-0.0.4/src/roomsync.rs
+-rw-r--r--   0     1001      123     6485 2023-04-30 12:23:26.000000 yroom-0.0.4/tests/test_yroom.py
+-rw-r--r--   0     1001      123     3889 2023-04-30 12:23:26.000000 yroom-0.0.4/yroom.pyi
+-rw-r--r--   0     1001      123    13697 2023-04-30 12:23:26.000000 yroom-0.0.4/Cargo.lock
+-rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 yroom-0.0.4/PKG-INFO
```

### Comparing `yroom-0.0.3/.github/workflows/release.yml` & `yroom-0.0.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `yroom-0.0.3/.github/workflows/test.yml` & `yroom-0.0.4/.github/workflows/test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         uses: actions-rs/toolchain@v1
         with:
           toolchain: stable
           profile: minimal
           default: true
 
       - name: Install Dependencies
-        run: python3 -m pip install pytest maturin
+        run: python3 -m pip install pytest y_py maturin
 
       - name: Build and install package
         run: |
               maturin build
               python3 -m pip install ./target/wheels/*.whl
 
       - name: Run Tests
```

### Comparing `yroom-0.0.3/LICENSE` & `yroom-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yroom-0.0.3/pyproject.toml` & `yroom-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "yroom"
-version = "0.0.3"
+version = "0.0.4"
 requires-python = ">=3.7"
 description = "Yjs sync and awareness protocol handler for a non-editing client (e.g. server)"
 authors = [
     { name = "Stefan Wehrmeyer", email = "mail@stefanwehrmeyer.com" }
 ]
 classifiers = [
     "Programming Language :: Rust",
@@ -22,8 +22,9 @@
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 
 [project.optional-dependencies]
 test = [
     "pytest",
+    "ypy"
 ]
```

### Comparing `yroom-0.0.3/yroom.pyi` & `yroom-0.0.4/yroom.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,30 @@
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, TypedDict
 
 class YRoomMessage:
     """
     Container that holds two members: `payload` and `broadcast_payload`.
     `payload` is a message that should be sent to the connection that sent the message.
     `broadcast_payload` is a message that should be sent to all connections in the room.
     Either or both of the members can be of zero length and then must not be sent.
     """
 
     payload: bytes
     broadcast_payload: bytes
 
+class YRoomSettings(TypedDict):
+    wire_version: int  # The Yjs encoding/decoding version to use (1 or 2, default: 1)
+    name_prefixed: bool  # Whether to expect a prefix for wire messages (default: False)
+    server_start_sync: bool  # Whether to start sync on connect (default: True)
+
 class YRoomManager:
+    def __init__(self, settings: Optional[Dict[str, YRoomSettings]]) -> None:
+        """
+        Create a new YRoomManager with an optional settings dict.
+        """
     def connect(self, room: str, conn_id: int) -> YRoomMessage:
         """
         Connect to a room with a connection id, returning a YRoomMessage.
         """
     def connect_with_data(self, room: str, conn_id: int, data: bytes) -> YRoomMessage:
         """
         Connect to a room with a connection id and bytes of serialized Yjs document in
```

### Comparing `yroom-0.0.3/Cargo.lock` & `yroom-0.0.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -499,15 +499,15 @@
  "lib0",
  "thiserror",
  "yrs",
 ]
 
 [[package]]
 name = "yroom"
-version = "0.0.3"
+version = "0.0.4"
 dependencies = [
  "lib0",
  "log",
  "pyo3",
  "pyo3-log",
  "y-sync",
  "yrs",
```

### Comparing `yroom-0.0.3/PKG-INFO` & `yroom-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: yroom
-Version: 0.0.3
+Version: 0.0.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pytest; extra == 'test'
+Requires-Dist: ypy; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE
 Summary: Yjs sync and awareness protocol handler for a non-editing client (e.g. server)
 Author-email: Stefan Wehrmeyer <mail@stefanwehrmeyer.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

