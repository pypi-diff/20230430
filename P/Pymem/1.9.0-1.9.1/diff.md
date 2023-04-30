# Comparing `tmp/Pymem-1.9.0.tar.gz` & `tmp/Pymem-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Pymem-1.9.0.tar", last modified: Tue Sep 27 06:25:26 2022, max compression
+gzip compressed data, was "dist\Pymem-1.9.1.tar", last modified: Mon Oct 17 15:07:14 2022, max compression
```

## Comparing `Pymem-1.9.0.tar` & `Pymem-1.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2022-09-27 06:25:26.000000 Pymem-1.9.0/
--rw-rw-rw-   0        0        0       22 2022-09-27 06:24:40.000000 Pymem-1.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3280 2022-09-27 06:25:26.000000 Pymem-1.9.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-09-27 06:25:26.000000 Pymem-1.9.0/pymem/
--rw-rw-rw-   0        0        0     1909 2022-09-27 06:24:40.000000 Pymem-1.9.0/pymem/exception.py
--rw-rw-rw-   0        0        0    34137 2022-09-27 06:24:40.000000 Pymem-1.9.0/pymem/memory.py
--rw-rw-rw-   0        0        0     5785 2022-09-27 06:24:40.000000 Pymem-1.9.0/pymem/pattern.py
--rw-rw-rw-   0        0        0    12674 2022-09-27 06:24:40.000000 Pymem-1.9.0/pymem/process.py
--rw-rw-rw-   0        0        0     3420 2022-09-27 06:24:40.000000 Pymem-1.9.0/pymem/ptypes.py
-drwxrwxrwx   0        0        0        0 2022-09-27 06:25:26.000000 Pymem-1.9.0/pymem/ressources/
--rw-rw-rw-   0        0        0     2490 2022-09-27 06:24:40.000000 Pymem-1.9.0/pymem/ressources/advapi32.py
--rw-rw-rw-   0        0        0     9775 2022-09-27 06:24:40.000000 Pymem-1.9.0/pymem/ressources/kernel32.py
--rw-rw-rw-   0        0        0      636 2022-09-27 06:24:40.000000 Pymem-1.9.0/pymem/ressources/ntdll.py
--rw-rw-rw-   0        0        0     1281 2022-09-27 06:24:40.000000 Pymem-1.9.0/pymem/ressources/psapi.py
--rw-rw-rw-   0        0        0    21912 2022-09-27 06:24:40.000000 Pymem-1.9.0/pymem/ressources/structure.py
--rw-rw-rw-   0        0        0      721 2022-09-27 06:24:40.000000 Pymem-1.9.0/pymem/ressources/__init__.py
--rw-rw-rw-   0        0        0     1787 2022-09-27 06:24:40.000000 Pymem-1.9.0/pymem/thread.py
--rw-rw-rw-   0        0        0    44156 2022-09-27 06:24:40.000000 Pymem-1.9.0/pymem/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-27 06:25:26.000000 Pymem-1.9.0/Pymem.egg-info/
--rw-rw-rw-   0        0        0        1 2022-09-27 06:25:26.000000 Pymem-1.9.0/Pymem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3280 2022-09-27 06:25:26.000000 Pymem-1.9.0/Pymem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      120 2022-09-27 06:25:26.000000 Pymem-1.9.0/Pymem.egg-info/requires.txt
--rw-rw-rw-   0        0        0      505 2022-09-27 06:25:26.000000 Pymem-1.9.0/Pymem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        6 2022-09-27 06:25:26.000000 Pymem-1.9.0/Pymem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1128 2022-09-27 06:24:40.000000 Pymem-1.9.0/README.md
--rw-rw-rw-   0        0        0       58 2022-09-27 06:24:40.000000 Pymem-1.9.0/requirements-doc.txt
--rw-rw-rw-   0        0        0       31 2022-09-27 06:24:40.000000 Pymem-1.9.0/requirements-test.txt
--rw-rw-rw-   0        0        0       42 2022-09-27 06:25:26.000000 Pymem-1.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1406 2022-09-27 06:24:40.000000 Pymem-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-17 15:07:14.000000 Pymem-1.9.1/
+-rw-rw-rw-   0        0        0       22 2022-10-17 15:06:13.000000 Pymem-1.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3280 2022-10-17 15:07:14.000000 Pymem-1.9.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-10-17 15:07:14.000000 Pymem-1.9.1/pymem/
+-rw-rw-rw-   0        0        0     1909 2022-10-17 15:06:13.000000 Pymem-1.9.1/pymem/exception.py
+-rw-rw-rw-   0        0        0    34161 2022-10-17 15:06:13.000000 Pymem-1.9.1/pymem/memory.py
+-rw-rw-rw-   0        0        0     5785 2022-10-17 15:06:13.000000 Pymem-1.9.1/pymem/pattern.py
+-rw-rw-rw-   0        0        0    12674 2022-10-17 15:06:13.000000 Pymem-1.9.1/pymem/process.py
+-rw-rw-rw-   0        0        0     3420 2022-10-17 15:06:13.000000 Pymem-1.9.1/pymem/ptypes.py
+drwxrwxrwx   0        0        0        0 2022-10-17 15:07:14.000000 Pymem-1.9.1/pymem/ressources/
+-rw-rw-rw-   0        0        0     2490 2022-10-17 15:06:13.000000 Pymem-1.9.1/pymem/ressources/advapi32.py
+-rw-rw-rw-   0        0        0    10005 2022-10-17 15:06:13.000000 Pymem-1.9.1/pymem/ressources/kernel32.py
+-rw-rw-rw-   0        0        0      636 2022-10-17 15:06:13.000000 Pymem-1.9.1/pymem/ressources/ntdll.py
+-rw-rw-rw-   0        0        0     1281 2022-10-17 15:06:13.000000 Pymem-1.9.1/pymem/ressources/psapi.py
+-rw-rw-rw-   0        0        0    21912 2022-10-17 15:06:13.000000 Pymem-1.9.1/pymem/ressources/structure.py
+-rw-rw-rw-   0        0        0      721 2022-10-17 15:06:13.000000 Pymem-1.9.1/pymem/ressources/__init__.py
+-rw-rw-rw-   0        0        0     1787 2022-10-17 15:06:13.000000 Pymem-1.9.1/pymem/thread.py
+-rw-rw-rw-   0        0        0    44156 2022-10-17 15:06:13.000000 Pymem-1.9.1/pymem/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-17 15:07:14.000000 Pymem-1.9.1/Pymem.egg-info/
+-rw-rw-rw-   0        0        0        1 2022-10-17 15:07:14.000000 Pymem-1.9.1/Pymem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3280 2022-10-17 15:07:14.000000 Pymem-1.9.1/Pymem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2022-10-17 15:07:14.000000 Pymem-1.9.1/Pymem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      505 2022-10-17 15:07:14.000000 Pymem-1.9.1/Pymem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        6 2022-10-17 15:07:14.000000 Pymem-1.9.1/Pymem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1128 2022-10-17 15:06:13.000000 Pymem-1.9.1/README.md
+-rw-rw-rw-   0        0        0       58 2022-10-17 15:06:13.000000 Pymem-1.9.1/requirements-doc.txt
+-rw-rw-rw-   0        0        0       31 2022-10-17 15:06:13.000000 Pymem-1.9.1/requirements-test.txt
+-rw-rw-rw-   0        0        0       42 2022-10-17 15:07:14.000000 Pymem-1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1406 2022-10-17 15:06:13.000000 Pymem-1.9.1/setup.py
```

### Comparing `Pymem-1.9.0/PKG-INFO` & `Pymem-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pymem
-Version: 1.9.0
+Version: 1.9.1
 Summary: pymem: python memory access made easy
 Home-page: http://pymem.readthedocs.org/en/latest/
 Author: Fabien Reboia
 Author-email: srounet@gmail.com
 Maintainer: Fabien Reboia
 Maintainer-email: srounet@gmail.com
 License: mit
@@ -72,10 +72,10 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+Provides-Extra: test
 Provides-Extra: speed
 Provides-Extra: doc
-Provides-Extra: test
```

### Comparing `Pymem-1.9.0/pymem/exception.py` & `Pymem-1.9.1/pymem/exception.py`

 * *Files identical despite different names*

### Comparing `Pymem-1.9.0/pymem/memory.py` & `Pymem-1.9.1/pymem/memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     int
         The address of the allocated region of pages.
     """
     if not allocation_type:
         allocation_type = pymem.ressources.structure.MEMORY_STATE.MEM_COMMIT.value
     if not protection_type:
         protection_type = pymem.ressources.structure.MEMORY_PROTECTION.PAGE_EXECUTE_READWRITE.value
-    ctypes.windll.kernel32.SetLastError(0)
+    pymem.ressources.kernel32.SetLastError(0)
     address = pymem.ressources.kernel32.VirtualAllocEx(handle, None, size, allocation_type, protection_type)
     return address
 
 
 def free_memory(handle, address, free_type=None):
     """Releases, decommits, or releases and decommits a region of memory within the virtual address space of a specified
     process.
@@ -57,15 +57,15 @@
     Returns
     -------
     int
         A boolean indicating if the call was a success.
     """
     if not free_type:
         free_type = pymem.ressources.structure.MEMORY_STATE.MEM_RELEASE
-    ctypes.windll.kernel32.SetLastError(0)
+    pymem.ressources.kernel32.SetLastError(0)
     ret = pymem.ressources.kernel32.VirtualFreeEx(handle, address, 0, free_type)
     return ret
 
 
 def read_bytes(handle, address, byte):
     """Reads data from an area of memory in a specified process.
     The entire area to be read must be accessible or the operation fails.
@@ -94,25 +94,25 @@
     bytes
         The raw value read as bytes
     """
     if not isinstance(address, int):
         raise TypeError('Address must be int: {}'.format(address))
     buff = ctypes.create_string_buffer(byte)
     bytes_read = ctypes.c_size_t()
-    ctypes.windll.kernel32.SetLastError(0)
+    pymem.ressources.kernel32.SetLastError(0)
     pymem.ressources.kernel32.ReadProcessMemory(
         handle,
         ctypes.c_void_p(address),
         ctypes.byref(buff),
         byte,
         ctypes.byref(bytes_read)
     )
     error_code = ctypes.windll.kernel32.GetLastError()
     if error_code:
-        ctypes.windll.kernel32.SetLastError(0)
+        pymem.ressources.kernel32.SetLastError(0)
         raise pymem.exception.WinAPIError(error_code)
     raw = buff.raw
     return raw
 
 
 def read_bool(handle, address):
     """Reads 1 byte from an area of memory in a specified process.
@@ -614,22 +614,22 @@
         if WriteProcessMemory failed
 
     Returns
     -------
     bool
         A boolean indicating a successful write.
     """
-    ctypes.windll.kernel32.SetLastError(0)
+    pymem.ressources.kernel32.SetLastError(0)
     if not isinstance(address, int):
         raise TypeError('Address must be int: {}'.format(address))
     dst = ctypes.cast(address, ctypes.c_char_p)
     res = ctypes.windll.kernel32.WriteProcessMemory(handle, dst, data, length, 0x0)
     error_code = ctypes.windll.kernel32.GetLastError()
     if error_code:
-        ctypes.windll.kernel32.SetLastError(0)
+        pymem.ressources.kernel32.SetLastError(0)
         raise pymem.exception.WinAPIError(error_code)
     return res
 
 
 def write_bool(handle, address, value):
     """Writes 1 byte to an area of memory in a specified process.
     The entire area to be written to must be accessible or the operation fails.
@@ -1125,14 +1125,14 @@
 
     Returns
     -------
     MEMORY_BASIC_INFORMATION
         A memory basic information object
     """
     mbi = pymem.ressources.structure.MEMORY_BASIC_INFORMATION()
-    ctypes.windll.kernel32.SetLastError(0)
+    pymem.ressources.kernel32.SetLastError(0)
     pymem.ressources.kernel32.VirtualQueryEx(handle, address, ctypes.byref(mbi), ctypes.sizeof(mbi))
     error_code = ctypes.windll.kernel32.GetLastError()
     if error_code:
-        ctypes.windll.kernel32.SetLastError(0)
+        pymem.ressources.kernel32.SetLastError(0)
         raise pymem.exception.WinAPIError(error_code)
     return mbi
```

### Comparing `Pymem-1.9.0/pymem/pattern.py` & `Pymem-1.9.1/pymem/pattern.py`

 * *Files identical despite different names*

### Comparing `Pymem-1.9.0/pymem/process.py` & `Pymem-1.9.1/pymem/process.py`

 * *Files identical despite different names*

### Comparing `Pymem-1.9.0/pymem/ptypes.py` & `Pymem-1.9.1/pymem/ptypes.py`

 * *Files identical despite different names*

### Comparing `Pymem-1.9.0/pymem/ressources/advapi32.py` & `Pymem-1.9.1/pymem/ressources/advapi32.py`

 * *Files identical despite different names*

### Comparing `Pymem-1.9.0/pymem/ressources/kernel32.py` & `Pymem-1.9.1/pymem/ressources/kernel32.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 try:
     dll = ctypes.WinDLL('kernel32.dll')
 except AttributeError:
     class MockObject:
         def __getattr__(self, item):
             return self
 
+
     dll = MockObject()
 
 #: Opens an existing local process object.
 #:
 #: https://msdn.microsoft.com/en-us/library/windows/desktop/ms684320%28v=vs.85%29.aspx
 OpenProcess = dll.OpenProcess
 OpenProcess.restype = ctypes.c_void_p
@@ -35,14 +36,20 @@
 #: Retrieves the calling thread's last-error code value. The last-error code is maintained on a per-thread basis.
 #: Multiple threads do not overwrite each other's last-error code.
 #:
 #: https://msdn.microsoft.com/en-us/library/windows/desktop/ms679360%28v=vs.85%29.aspx
 GetLastError = dll.GetLastError
 GetLastError.restype = ctypes.c_ulong
 
+#: Sets the last-error code for the calling thread.
+#:
+#: https://docs.microsoft.com/en-us/windows/win32/api/errhandlingapi/nf-errhandlingapi-setlasterror
+SetLastError = dll.SetLastError
+SetLastError.argtypes = [ctypes.c_ulong]
+
 #: Retrieves a pseudo handle for the current process.
 #:
 #: https://msdn.microsoft.com/en-us/library/windows/desktop/ms683179%28v=vs.85%29.aspx
 GetCurrentProcess = dll.GetCurrentProcess
 GetCurrentProcess.argtypes = []
 GetCurrentProcess.restype = ctypes.c_ulong
```

### Comparing `Pymem-1.9.0/pymem/ressources/ntdll.py` & `Pymem-1.9.1/pymem/ressources/ntdll.py`

 * *Files identical despite different names*

### Comparing `Pymem-1.9.0/pymem/ressources/psapi.py` & `Pymem-1.9.1/pymem/ressources/psapi.py`

 * *Files identical despite different names*

### Comparing `Pymem-1.9.0/pymem/ressources/structure.py` & `Pymem-1.9.1/pymem/ressources/structure.py`

 * *Files identical despite different names*

### Comparing `Pymem-1.9.0/pymem/ressources/__init__.py` & `Pymem-1.9.1/pymem/ressources/__init__.py`

 * *Files identical despite different names*

### Comparing `Pymem-1.9.0/pymem/thread.py` & `Pymem-1.9.1/pymem/thread.py`

 * *Files identical despite different names*

### Comparing `Pymem-1.9.0/pymem/__init__.py` & `Pymem-1.9.1/pymem/__init__.py`

 * *Files identical despite different names*

### Comparing `Pymem-1.9.0/Pymem.egg-info/PKG-INFO` & `Pymem-1.9.1/Pymem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pymem
-Version: 1.9.0
+Version: 1.9.1
 Summary: pymem: python memory access made easy
 Home-page: http://pymem.readthedocs.org/en/latest/
 Author: Fabien Reboia
 Author-email: srounet@gmail.com
 Maintainer: Fabien Reboia
 Maintainer-email: srounet@gmail.com
 License: mit
@@ -72,10 +72,10 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+Provides-Extra: test
 Provides-Extra: speed
 Provides-Extra: doc
-Provides-Extra: test
```

### Comparing `Pymem-1.9.0/README.md` & `Pymem-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `Pymem-1.9.0/setup.py` & `Pymem-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 with open(ROOT + '/PYPI-README.md', encoding="utf-8") as fp:
     long_description = fp.read()
 
 
 setuptools.setup(
     name='Pymem',
-    version='1.9.0',
+    version='1.9.1',
     long_description=long_description,
     long_description_content_type="text/markdown",
     description='pymem: python memory access made easy',
     author='Fabien Reboia',
     author_email='srounet@gmail.com',
     maintainer='Fabien Reboia',
     maintainer_email='srounet@gmail.com',
```

