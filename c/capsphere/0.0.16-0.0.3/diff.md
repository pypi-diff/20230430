# Comparing `tmp/capsphere-0.0.16.tar.gz` & `tmp/capsphere-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capsphere-0.0.16.tar", last modified: Sun Apr 30 21:41:44 2023, max compression
+gzip compressed data, was "capsphere-0.0.3.tar", last modified: Mon Mar 20 11:42:15 2023, max compression
```

## Comparing `capsphere-0.0.16.tar` & `capsphere-0.0.3.tar`

### file list

```diff
@@ -1,65 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:41:44.655679 capsphere-0.0.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-30 21:41:44.655679 capsphere-0.0.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-30 21:40:58.000000 capsphere-0.0.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:41:44.651679 capsphere-0.0.16/capsphere/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:41:44.651679 capsphere-0.0.16/capsphere/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/common/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/common/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:41:44.651679 capsphere-0.0.16/capsphere/common/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/common/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/common/test/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/common/test/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/common/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:41:44.651679 capsphere-0.0.16/capsphere/domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:41:44.655679 capsphere-0.0.16/capsphere/domain/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/domain/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/domain/input/bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/domain/input/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:41:44.655679 capsphere-0.0.16/capsphere/domain/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/domain/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/domain/output/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/domain/output/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:41:44.655679 capsphere-0.0.16/capsphere/domain/output/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/domain/output/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/domain/output/test/test_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/domain/output/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/domain/output/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/domain/output/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:41:44.655679 capsphere-0.0.16/capsphere/recognition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/recognition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:41:44.655679 capsphere-0.0.16/capsphere/recognition/plumber/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/recognition/plumber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/recognition/plumber/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/recognition/plumber/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:41:44.655679 capsphere-0.0.16/capsphere/recognition/plumber/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/recognition/plumber/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/recognition/plumber/test/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/recognition/plumber/test/test_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:41:44.655679 capsphere-0.0.16/capsphere/recognition/pytesseract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/recognition/pytesseract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:41:44.655679 capsphere-0.0.16/capsphere/recognition/textract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/recognition/textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/recognition/textract/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:41:44.655679 capsphere-0.0.16/capsphere/recognition/textract/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/recognition/textract/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/recognition/textract/test/test_extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:41:44.655679 capsphere-0.0.16/capsphere/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/resources/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:41:44.655679 capsphere-0.0.16/capsphere/resources/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/resources/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   169258 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/resources/test/ambank.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-30 21:40:58.000000 capsphere-0.0.16/capsphere/resources/test/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:41:44.651679 capsphere-0.0.16/capsphere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-30 21:41:44.000000 capsphere-0.0.16/capsphere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-30 21:41:44.000000 capsphere-0.0.16/capsphere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 21:41:44.000000 capsphere-0.0.16/capsphere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-30 21:41:44.000000 capsphere-0.0.16/capsphere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-30 21:41:44.000000 capsphere-0.0.16/capsphere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 21:41:44.655679 capsphere-0.0.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-30 21:40:58.000000 capsphere-0.0.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-20 11:42:15.203372 capsphere-0.0.3/
+-rw-rw-rw-   0        0        0      850 2023-03-20 11:42:15.203372 capsphere-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-03-19 09:25:46.000000 capsphere-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-03-20 11:42:15.165350 capsphere-0.0.3/capsphere/
+-rw-rw-rw-   0        0        0        0 2023-03-11 12:18:58.000000 capsphere-0.0.3/capsphere/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-20 11:42:15.184386 capsphere-0.0.3/capsphere/common/
+-rw-rw-rw-   0        0        0        0 2023-03-11 12:18:58.000000 capsphere-0.0.3/capsphere/common/__init__.py
+-rw-rw-rw-   0        0        0      168 2023-03-12 02:25:13.000000 capsphere-0.0.3/capsphere/common/date.py
+-rw-rw-rw-   0        0        0      137 2023-03-18 20:12:44.000000 capsphere-0.0.3/capsphere/common/s3.py
+drwxrwxrwx   0        0        0        0 2023-03-20 11:42:15.188348 capsphere-0.0.3/capsphere/common/test/
+-rw-rw-rw-   0        0        0        0 2023-03-11 12:18:58.000000 capsphere-0.0.3/capsphere/common/test/__init__.py
+-rw-rw-rw-   0        0        0      586 2023-03-11 12:18:58.000000 capsphere-0.0.3/capsphere/common/test/test_date.py
+-rw-rw-rw-   0        0        0      346 2023-03-19 22:38:30.000000 capsphere-0.0.3/capsphere/common/test/test_s3.py
+-rw-rw-rw-   0        0        0      743 2023-03-12 07:43:36.000000 capsphere-0.0.3/capsphere/common/test/test_utils.py
+-rw-rw-rw-   0        0        0      350 2023-03-12 07:42:39.000000 capsphere-0.0.3/capsphere/common/utils.py
+drwxrwxrwx   0        0        0        0 2023-03-20 11:42:15.189347 capsphere-0.0.3/capsphere/domain/
+-rw-rw-rw-   0        0        0        0 2023-03-11 12:18:58.000000 capsphere-0.0.3/capsphere/domain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-20 11:42:15.192346 capsphere-0.0.3/capsphere/domain/input/
+-rw-rw-rw-   0        0        0        0 2023-03-13 10:03:45.000000 capsphere-0.0.3/capsphere/domain/input/__init__.py
+-rw-rw-rw-   0        0        0      144 2023-03-14 10:14:30.000000 capsphere-0.0.3/capsphere/domain/input/bank.py
+-rw-rw-rw-   0        0        0     3877 2023-03-14 11:13:03.000000 capsphere-0.0.3/capsphere/domain/input/model.py
+drwxrwxrwx   0        0        0        0 2023-03-20 11:42:15.196344 capsphere-0.0.3/capsphere/domain/output/
+-rw-rw-rw-   0        0        0        0 2023-03-13 10:03:11.000000 capsphere-0.0.3/capsphere/domain/output/__init__.py
+-rw-rw-rw-   0        0        0     2602 2023-03-19 11:47:54.000000 capsphere-0.0.3/capsphere/domain/output/excel.py
+-rw-rw-rw-   0        0        0     1853 2023-03-19 22:23:06.000000 capsphere-0.0.3/capsphere/domain/output/model.py
+drwxrwxrwx   0        0        0        0 2023-03-20 11:42:15.199348 capsphere-0.0.3/capsphere/domain/output/test/
+-rw-rw-rw-   0        0        0        0 2023-03-13 10:04:26.000000 capsphere-0.0.3/capsphere/domain/output/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-20 11:42:15.202346 capsphere-0.0.3/capsphere/domain/output/test/resources/
+-rw-rw-rw-   0        0        0        0 2023-03-18 23:07:18.000000 capsphere-0.0.3/capsphere/domain/output/test/resources/__init__.py
+-rw-rw-rw-   0        0        0      895 2023-03-18 23:32:11.000000 capsphere-0.0.3/capsphere/domain/output/test/resources/data.py
+-rw-rw-rw-   0        0        0     3408 2023-03-19 22:23:06.000000 capsphere-0.0.3/capsphere/domain/output/test/test_excel.py
+-rw-rw-rw-   0        0        0     1181 2023-03-13 10:08:56.000000 capsphere-0.0.3/capsphere/domain/output/test/test_model.py
+drwxrwxrwx   0        0        0        0 2023-03-20 11:42:15.179344 capsphere-0.0.3/capsphere.egg-info/
+-rw-rw-rw-   0        0        0      850 2023-03-20 11:42:15.000000 capsphere-0.0.3/capsphere.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      899 2023-03-20 11:42:15.000000 capsphere-0.0.3/capsphere.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-20 11:42:15.000000 capsphere-0.0.3/capsphere.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-03-20 11:42:15.000000 capsphere-0.0.3/capsphere.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-03-20 11:42:15.000000 capsphere-0.0.3/capsphere.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-20 11:42:15.204346 capsphere-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      864 2023-03-20 11:41:59.000000 capsphere-0.0.3/setup.py
```

### Comparing `capsphere-0.0.16/capsphere/domain/input/model.py` & `capsphere-0.0.3/capsphere/domain/input/model.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-import abc
-from dataclasses import dataclass
-from dataclass_wizard import JSONWizard
-from abc import ABC, ABCMeta, abstractmethod
-
-HEADERS = {
-    'ambank': ['date', 'transaction', 'cheque no.', 'debit', 'credit', 'balance'],
-    'cimb': ['date', 'description', 'cheque / ref no', 'withdrawal', 'deposits', 'balance'],
-    'rhb': ['date', 'branch', 'description', 'sender''s beneficiary''s name', 'reference 1 / recipient''s reference',
-            'reference 2 / other payment details', 'refnum', 'amount (dr)', 'amount (cr)', 'balance'],
-    'maybank': ['entry_date', 'value_date', 'transaction description', 'transaction amount', 'statement balance']
-}
-
-
-@dataclass(unsafe_hash=True)
-class Transaction(JSONWizard):
-
-    """
-    Single transaction schema that all banks need to adhere to. The best way to think of this is as a generic row
-    from a bank statement
-    """
-
-    date: str
-    description: str
-    reference: str
-    debit: str
-    credit: str
-    balance: str
-
-
-class TransactionConverter(ABC):
-
-    @abstractmethod
-    def to_transaction(self) -> Transaction:
-        raise NotImplementedError
-
-
-def create_dataclass(fields, base_class=None):
-
-    """
-    Dynamically creates a dataclass with the given field names.
-    """
-
-    # Remove any invalid characters from the field names
-    field_names = [name.replace(" ", "_").replace("'", "").replace("\\", "")
-                   .replace("//", "").replace(",", "").replace(".", "") for name in fields]
-
-    # Define the dataclass with the given field names
-    @dataclass(unsafe_hash=True)
-    class _DataRow(base_class or object, JSONWizard):
-        __slots__ = ()
-        # Define the fields with default values of None
-        __annotations__ = {name: str for name in field_names}
-    if base_class:
-        _DataRow.__bases__ = (base_class,)
-    if issubclass(base_class, ABC):
-        ABCMeta.register(_DataRow)
-    return dataclass(_DataRow)
-
-
-def create_transaction_class(class_name: str, base_class: type, class_fields: list[str]):
-
-    """
-    Dynamically creates a class that inherits from a given base class and has the given fields as instance variables.
-
-    :param class_name: Name of the class to be created.
-    :param base_class: Abstract base class that the created class should inherit from.
-    :param class_fields: List of strings representing the instance variables that the created class should have.
-    :return: A dynamically created class that inherits from the given base class and has the given fields as instance variables.
-    """
-
-    non_strings = [item for item in class_fields if not isinstance(item, str)]
-
-    if non_strings:
-        raise ValueError(f"Found non-string elements in class_fields: {non_strings}")
-
-    field_names = [name.replace(" ", "_").replace("'", "").replace("\\", "")
-                   .replace("//", "").replace(",", "").replace(".", "") for name in class_fields]
-
-    class_dict = {}
-    for field in field_names:
-        class_dict[field] = None
-
-    def to_transaction(self):
-        return base_class(*[getattr(self, field_name) for field_name in field_names])
-
-    class_dict["to_transaction"] = to_transaction
-
-    return abc.ABCMeta(class_name, (base_class,), class_dict)
-
-
-class TransactionConverterMeta(ABCMeta):
-    def __new__(cls, name, bases, attrs):
-        if name in HEADERS:
-            fields = HEADERS[name]
-
-            @abstractmethod
-            def to_transaction(self) -> Transaction:
-                pass
-
-            for i, field in enumerate(fields):
-                attrs[field] = property(lambda self, i=i: getattr(self, f"_data[{i}]"))
-
-            attrs['__annotations__'] = {field: str for field in fields}
-            attrs['_fields'] = tuple(fields)
-
-        return super().__new__(cls, name, bases, attrs)
+import abc
+from dataclasses import dataclass
+from dataclass_wizard import JSONWizard
+from abc import ABC, ABCMeta, abstractmethod
+
+HEADERS = {
+    'ambank': ['date', 'transaction', 'cheque no.', 'debit', 'credit', 'balance'],
+    'cimb': ['date', 'description', 'cheque / ref no', 'withdrawal', 'deposits', 'balance'],
+    'rhb': ['date', 'branch', 'description', 'sender''s beneficiary''s name', 'reference 1 / recipient''s reference',
+            'reference 2 / other payment details', 'refnum', 'amount (dr)', 'amount (cr)', 'balance'],
+    'maybank': ['entry_date', 'value_date', 'transaction description', 'transaction amount', 'statement balance']
+}
+
+
+@dataclass(unsafe_hash=True)
+class Transaction(JSONWizard):
+
+    """
+    Single transaction schema that all banks need to adhere to. The best way to think of this is as a generic row
+    from a bank statement
+    """
+
+    date: str
+    description: str
+    reference: str
+    debit: str
+    credit: str
+    balance: str
+
+
+class TransactionConverter(ABC):
+
+    @abstractmethod
+    def to_transaction(self) -> Transaction:
+        raise NotImplementedError
+
+
+def create_dataclass(fields, base_class=None):
+
+    """
+    Dynamically creates a dataclass with the given field names.
+    """
+
+    # Remove any invalid characters from the field names
+    field_names = [name.replace(" ", "_").replace("'", "").replace("\\", "")
+                   .replace("//", "").replace(",", "").replace(".", "") for name in fields]
+
+    # Define the dataclass with the given field names
+    @dataclass(unsafe_hash=True)
+    class _DataRow(base_class or object, JSONWizard):
+        __slots__ = ()
+        # Define the fields with default values of None
+        __annotations__ = {name: str for name in field_names}
+    if base_class:
+        _DataRow.__bases__ = (base_class,)
+    if issubclass(base_class, ABC):
+        ABCMeta.register(_DataRow)
+    return dataclass(_DataRow)
+
+
+def create_transaction_class(class_name: str, base_class: type, class_fields: list[str]):
+
+    """
+    Dynamically creates a class that inherits from a given base class and has the given fields as instance variables.
+
+    :param class_name: Name of the class to be created.
+    :param base_class: Abstract base class that the created class should inherit from.
+    :param class_fields: List of strings representing the instance variables that the created class should have.
+    :return: A dynamically created class that inherits from the given base class and has the given fields as instance variables.
+    """
+
+    non_strings = [item for item in class_fields if not isinstance(item, str)]
+
+    if non_strings:
+        raise ValueError(f"Found non-string elements in class_fields: {non_strings}")
+
+    field_names = [name.replace(" ", "_").replace("'", "").replace("\\", "")
+                   .replace("//", "").replace(",", "").replace(".", "") for name in class_fields]
+
+    class_dict = {}
+    for field in field_names:
+        class_dict[field] = None
+
+    def to_transaction(self):
+        return base_class(*[getattr(self, field_name) for field_name in field_names])
+
+    class_dict["to_transaction"] = to_transaction
+
+    return abc.ABCMeta(class_name, (base_class,), class_dict)
+
+
+class TransactionConverterMeta(ABCMeta):
+    def __new__(cls, name, bases, attrs):
+        if name in HEADERS:
+            fields = HEADERS[name]
+
+            @abstractmethod
+            def to_transaction(self) -> Transaction:
+                pass
+
+            for i, field in enumerate(fields):
+                attrs[field] = property(lambda self, i=i: getattr(self, f"_data[{i}]"))
+
+            attrs['__annotations__'] = {field: str for field in fields}
+            attrs['_fields'] = tuple(fields)
+
+        return super().__new__(cls, name, bases, attrs)
```

### Comparing `capsphere-0.0.16/capsphere/domain/output/model.py` & `capsphere-0.0.3/capsphere/domain/output/model.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from dataclasses import dataclass
-from decimal import Decimal
-from dataclass_wizard import JSONWizard
-from typing import Type
-
-BANKS = ['Maybank', 'CIMB', 'Ambank', 'Hong Leong', 'Alliance', 'Public Bank', 'RHB']
-
-
-@dataclass(unsafe_hash=True)
-class Cf(JSONWizard):
-    customer_name: str
-    bank_name: str
-    month: str
-    start_balance: Decimal
-    end_balance: Decimal
-    total_debit: Decimal
-    total_credit: Decimal
-    average_debit: Decimal
-    average_credit: Decimal
-
-    def __post_init__(self):
-        if not isinstance(self.customer_name, str):
-            raise TypeError("Field 'customer_name' must be of type 'str'.")
-        if not isinstance(self.bank_name, str):
-            raise TypeError("Field 'bank_name' must be of type 'str'.")
-        if not isinstance(self.month, str):
-            raise TypeError("Field 'month' must be of type 'str'.")
-        if not isinstance(self.start_balance, Decimal):
-            raise TypeError("Field 'start_balance' must be of type 'Decimal'.")
-        if not isinstance(self.end_balance, Decimal):
-            raise TypeError("Field 'end_balance' must be of type 'Decimal'.")
-        if not isinstance(self.total_debit, Decimal):
-            raise TypeError("Field 'total_debit' must be of type 'Decimal'.")
-        if not isinstance(self.total_credit, Decimal):
-            raise TypeError("Field 'total_credit' must be of type 'Decimal'.")
-        if not isinstance(self.average_debit, Decimal):
-            raise TypeError("Field 'average_debit' must be of type 'Decimal'.")
-        if not isinstance(self.average_credit, Decimal):
-            raise TypeError("Field 'average_credit' must be of type 'Decimal'.")
-
-
-@dataclass(unsafe_hash=True)
-class MultiCf(JSONWizard):
-    cf_list: list[Type[Cf]]
-
-    def aggregate(self):
-        pass
-
+from dataclasses import dataclass
+from decimal import Decimal
+from dataclass_wizard import JSONWizard
+from typing import Type
+
+BANKS = ['Maybank', 'CIMB', 'Ambank', 'Hong Leong', 'Alliance', 'Public Bank', 'RHB']
+
+
+@dataclass(unsafe_hash=True)
+class Cf(JSONWizard):
+    customer_name: str
+    bank_name: str
+    month: str
+    start_balance: Decimal
+    end_balance: Decimal
+    total_debit: Decimal
+    total_credit: Decimal
+    average_debit: Decimal
+    average_credit: Decimal
+
+    def __post_init__(self):
+        if not isinstance(self.customer_name, str):
+            raise TypeError("Field 'customer_name' must be of type 'str'.")
+        if not isinstance(self.bank_name, str):
+            raise TypeError("Field 'bank_name' must be of type 'str'.")
+        if not isinstance(self.month, str):
+            raise TypeError("Field 'month' must be of type 'str'.")
+        if not isinstance(self.start_balance, Decimal):
+            raise TypeError("Field 'start_balance' must be of type 'Decimal'.")
+        if not isinstance(self.end_balance, Decimal):
+            raise TypeError("Field 'end_balance' must be of type 'Decimal'.")
+        if not isinstance(self.total_debit, Decimal):
+            raise TypeError("Field 'total_debit' must be of type 'Decimal'.")
+        if not isinstance(self.total_credit, Decimal):
+            raise TypeError("Field 'total_credit' must be of type 'Decimal'.")
+        if not isinstance(self.average_debit, Decimal):
+            raise TypeError("Field 'average_debit' must be of type 'Decimal'.")
+        if not isinstance(self.average_credit, Decimal):
+            raise TypeError("Field 'average_credit' must be of type 'Decimal'.")
+
+
+@dataclass(unsafe_hash=True)
+class MultiCf(JSONWizard):
+    cf_list: list[Type[Cf]]
+
+    def aggregate(self):
+        pass
+
```

### Comparing `capsphere-0.0.16/capsphere/domain/output/test/test_excel.py` & `capsphere-0.0.3/capsphere/domain/output/test/test_excel.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,70 @@
-import unittest
-import pandas as pd
-
-from capsphere.resources.test.data import CF, CF2, CF3
-from capsphere.domain.output.excel import _generate_average_rcf, create_worksheet
-
-
-class TestExcel(unittest.TestCase):
-    single_cashflow = [CF]
-    multi_cashflow = [CF, CF2]
-    multi_cashflow2 = [CF3]
-    headers = ['start_balance', 'end_balance', 'total_debit', 'total_credit',
-               'average_debit', 'average_credit']
-    labels = ['Apr 2023', 'Apr 2022', 'Total', 'Average']
-
-    def test_single_cashflow(self):
-        df = _generate_average_rcf(self.single_cashflow)
-        actual_totals = df.loc['Total']
-        actual_averages = df.loc['Average']
-        expected_totals = [133271.25, 99927.34, 228106.89, 194762.98, 3660.80, 7041.59]
-        expected_averages = [66635.63, 49963.67, 114053.45, 97381.49, 1830.40, 3520.80]
-        df_rows = 4
-        self.__assert_dataframes(df)
-        self.assertEqual(len(df.index), df_rows)
-        self.__assert_data_row(actual_totals, expected_totals)
-        self.__assert_data_row(actual_averages, expected_averages)
-
-    def test_multi_cashflow(self):
-        df = _generate_average_rcf(self.multi_cashflow)
-        actual_totals = df.loc['Total']
-        actual_averages = df.loc['Average']
-        expected_totals = [266542.5, 199854.68, 456213.78, 389525.96, 7321.6, 14083.18]
-        expected_averages = [133271.25, 99927.34, 228106.89, 194762.98, 3660.80, 7041.59]
-        df_rows = 4
-        self.__assert_dataframes(df)
-        self.assertEqual(len(df.index), df_rows)
-        self.__assert_data_row(actual_totals, expected_totals)
-        self.__assert_data_row(actual_averages, expected_averages)
-
-    def __assert_dataframes(self, df: pd.DataFrame) -> None:
-
-        if len(df.index) != len(self.labels):
-            raise ValueError(f'{len(df.index)} total labels supplied, expected {len(self.labels)}')
-
-        if len(df.columns) != len(self.headers):
-            raise ValueError(f'{len(df.columns)} total labels supplied, expected {len(self.headers)}')
-
-        self.assertEqual(len(df.columns), 6)
-
-        for header in self.headers:
-            self.assertTrue(header in df.columns)
-
-        for label in self.labels:
-            self.assertTrue(label in df.index)
-
-        # TODO assert using numpy instead once the series has been sorted in month order
-        # index_array = np.array(df.index)
-        # columns_array = np.array(df.columns)
-        #
-        # if self.assertFalse(index_array, self.labels):
-        #     mask = index_array != self.labels
-        #     raise ValueError(f"Different elements: {index_array[mask]} (in lst1) and {self.labels[mask]} (in lst2).")
-        #
-        # if self.assertFalse(columns_array, self.headers): mask = columns_array != self.headers raise ValueError(
-        # f"Different elements: {columns_array[mask]} (in lst1) and {self.headers[mask]} (in lst2).")
-
-    def __assert_data_row(self, data_row: pd.Series, expected_values: list[float]) -> None:
-        if len(data_row) != len(expected_values):
-            raise ValueError(f'data row has {len(data_row)} elements, expected {len(expected_values)}')
-        diff_list = [{"index": index, "actual": x, "expected": y} for index, (x, y)
-                     in enumerate(zip(data_row, expected_values)) if abs(x - y) >= 0.00001]
-        self.assertFalse(diff_list, f"Lists are not equal: {diff_list}")
-
-    # TODO write up a unit resources for excel file somehow, output looks good
-    # def test_worksheet_single_cashflow(self):
-    #     data = create_worksheet(self.single_cashflow)
-    #     with open("single.xlsx", "wb") as f:
-    #         f.write(data.getvalue())
-
-    # def test_worksheet_multi_cashflow(self):
-    #     data = create_worksheet(self.multi_cashflow2)
-    #     with open("multi.xlsx", "wb") as f:
-    #         f.write(data.read())
+import unittest
+from capsphere.domain.output.test.resources.data import CF, CF2
+from capsphere.domain.output.excel import generate_average_rcf
+import pandas as pd
+
+
+class TestExcel(unittest.TestCase):
+    single_cashflow = [CF]
+    multi_cashflow = [CF, CF2]
+    headers = ['start_balance', 'end_balance', 'total_debit', 'total_credit',
+               'average_debit', 'average_credit']
+    labels = ['Mar 2022', 'Apr 2022', 'Total', 'Average']
+
+    def test_single_cashflow(self):
+        df = generate_average_rcf(self.single_cashflow)
+        actual_totals = df.loc['Total']
+        actual_averages = df.loc['Average']
+        expected_totals = [133271.25, 99927.34, 228106.89, 194762.98, 3660.80, 7041.59]
+        expected_averages = [66635.63, 49963.67, 114053.45, 97381.49, 1830.40, 3520.80]
+        df_rows = 4
+        self.__assert_dataframes(df)
+        self.assertEqual(len(df.index), df_rows)
+        self.__assert_data_row(actual_totals, expected_totals)
+        self.__assert_data_row(actual_averages, expected_averages)
+
+    def test_multi_cashflow(self):
+        df = generate_average_rcf(self.multi_cashflow)
+        actual_totals = df.loc['Total']
+        actual_averages = df.loc['Average']
+        expected_totals = [266542.5, 199854.68, 456213.78, 389525.96, 7321.6, 14083.18]
+        expected_averages = [133271.25, 99927.34, 228106.89, 194762.98, 3660.80, 7041.59]
+        df_rows = 4
+        self.__assert_dataframes(df)
+        self.assertEqual(len(df.index), df_rows)
+        self.__assert_data_row(actual_totals, expected_totals)
+        self.__assert_data_row(actual_averages, expected_averages)
+
+    def __assert_dataframes(self, df: pd.DataFrame) -> None:
+
+        if len(df.index) != len(self.labels):
+            raise ValueError(f'{len(df.index)} total labels supplied, expected {len(self.labels)}')
+
+        if len(df.columns) != len(self.headers):
+            raise ValueError(f'{len(df.columns)} total labels supplied, expected {len(self.headers)}')
+
+        self.assertEqual(len(df.columns), 6)
+
+        for header in self.headers:
+            self.assertTrue(header in df.columns)
+
+        for label in self.labels:
+            self.assertTrue(label in df.index)
+
+        # TODO assert using numpy instead once the series has been sorted in month order
+        # index_array = np.array(df.index)
+        # columns_array = np.array(df.columns)
+        #
+        # if self.assertFalse(index_array, self.labels):
+        #     mask = index_array != self.labels
+        #     raise ValueError(f"Different elements: {index_array[mask]} (in lst1) and {self.labels[mask]} (in lst2).")
+        #
+        # if self.assertFalse(columns_array, self.headers): mask = columns_array != self.headers raise ValueError(
+        # f"Different elements: {columns_array[mask]} (in lst1) and {self.headers[mask]} (in lst2).")
+
+    def __assert_data_row(self, data_row: pd.Series, expected_values: list[float]) -> None:
+        if len(data_row) != len(expected_values):
+            raise ValueError(f'data row has {len(data_row)} elements, expected {len(expected_values)}')
+        diff_list = [{"index": index, "actual": x, "expected": y} for index, (x, y)
+                     in enumerate(zip(data_row, expected_values)) if abs(x - y) >= 0.00001]
+        self.assertFalse(diff_list, f"Lists are not equal: {diff_list}")
```

