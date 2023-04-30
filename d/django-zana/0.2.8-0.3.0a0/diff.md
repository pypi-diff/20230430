# Comparing `tmp/django_zana-0.2.8.tar.gz` & `tmp/django_zana-0.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_zana-0.2.8.tar", max compression
+gzip compressed data, was "django_zana-0.3.0a0.tar", max compression
```

## Comparing `django_zana-0.2.8.tar` & `django_zana-0.3.0a0.tar`

### file list

```diff
@@ -1,12 +1,9 @@
--rw-r--r--   0        0        0     1739 2023-02-20 01:21:14.645438 django_zana-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 01:21:14.645438 django_zana-0.2.8/zana/django/__init__.py
--rw-r--r--   0        0        0      187 2023-02-20 01:21:14.645438 django_zana-0.2.8/zana/django/apps.py
--rw-r--r--   0        0        0      165 2023-02-20 01:21:14.645438 django_zana-0.2.8/zana/django/models/__init__.py
--rw-r--r--   0        0        0      448 2023-02-20 01:21:14.645438 django_zana-0.2.8/zana/django/models/__init__.pyi
--rw-r--r--   0        0        0    17664 2023-02-20 01:21:14.645438 django_zana-0.2.8/zana/django/models/_xaliases.py
--rw-r--r--   0        0        0     1386 2023-02-20 01:21:14.645438 django_zana-0.2.8/zana/django/models/fields/__init__.py
--rw-r--r--   0        0        0    44946 2023-02-20 01:21:14.649438 django_zana-0.2.8/zana/django/models/fields/aliases.py
--rw-r--r--   0        0        0        0 2023-02-20 01:21:14.649438 django_zana-0.2.8/zana/django/utils/__init__.py
--rw-r--r--   0        0        0    10693 2023-02-20 01:21:14.649438 django_zana-0.2.8/zana/django/utils/operator.py
--rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 django_zana-0.2.8/setup.py
--rw-r--r--   0        0        0      611 1970-01-01 00:00:00.000000 django_zana-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1786 2023-04-30 02:54:51.599699 django_zana-0.3.0a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-30 02:54:51.603699 django_zana-0.3.0a0/zana/django/__init__.py
+-rw-r--r--   0        0        0      187 2023-04-30 02:54:51.603699 django_zana-0.3.0a0/zana/django/apps.py
+-rw-r--r--   0        0        0      165 2023-04-30 02:54:51.603699 django_zana-0.3.0a0/zana/django/models/__init__.py
+-rw-r--r--   0        0        0      159 2023-04-30 02:54:51.603699 django_zana-0.3.0a0/zana/django/models/__init__.pyi
+-rw-r--r--   0        0        0    18179 2023-04-30 02:54:51.603699 django_zana-0.3.0a0/zana/django/models/_xaliases.py
+-rw-r--r--   0        0        0     1386 2023-04-30 02:54:51.603699 django_zana-0.3.0a0/zana/django/models/fields/__init__.py
+-rw-r--r--   0        0        0    41199 2023-04-30 02:54:51.603699 django_zana-0.3.0a0/zana/django/models/fields/aliases.py
+-rw-r--r--   0        0        0      614 1970-01-01 00:00:00.000000 django_zana-0.3.0a0/PKG-INFO
```

### Comparing `django_zana-0.2.8/pyproject.toml` & `django_zana-0.3.0a0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Django-Zana"
-version = "0.2.8"
+version = "0.3.0a0"
 description = "A `django` extension for `zana`."
 packages = [
     { include="zana" },
 ]
 authors = ["David Kyalo <davidmkyalo@gmail.com>"]
 license = "MIT"
 classifiers = [
@@ -13,40 +13,43 @@
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
+
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 Django = ">=3.2.0"
 typing-extensions = ">=4.4.0"
-zana = ">=0.1.10,<0.2.0"
+zana = {version = "^0.2.0a4", allow-prereleases = true}
+
 
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 ipython = "^8.10.0"
-mysqlclient = "^2.1.1"
-psycopg2-binary = "^2.9.5"
+django-polymorphic = "^3.1.0"
+tox = "^4.4.8"
 
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.0"
 pytest-asyncio = "^0.20.3"
 pytest-cov = {version = "^4.0.0", extras = ["toml"]}
 pytest-django = "^4.5.2"
 django-polymorphic = "^3.1.0"
+tox = "^4.4.8"
 
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "*"
@@ -63,15 +66,15 @@
 addopts = "--showlocals --cov=zana --cov-report html --cov-config pyproject.toml"
 asyncio_mode="auto"
 xfail_strict= "True"
 log_level = "DEBUG"
 python_files = "tests.py test.py test_*.py"
 python_classes = "test_* Test_*"
 python_functions = "test_* test"
-DJANGO_SETTINGS_MODULE = "example.settings"
+DJANGO_SETTINGS_MODULE = "tests.app.settings"
 
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "^\\s*pass\\s*$",
     "^\\s*\\.\\.\\.\\s*$",
```

### Comparing `django_zana-0.2.8/zana/django/models/_xaliases.py` & `django_zana-0.3.0a0/zana/django/models/_xaliases.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from functools import reduce, wraps
 from operator import attrgetter
 from types import FunctionType
 from types import GenericAlias as GenericAliasType
 from types import MethodType
 
 from typing_extensions import Self
-from zana.common import NotSet, cached_attr
+from zana.util import NotSet, cached_attr
 
 from django.apps import apps
 from django.core import checks
 from django.core.exceptions import ImproperlyConfigured
 from django.db import models as m
 from django.db.models.expressions import Combinable
 from django.db.models.functions import Coalesce
@@ -173,18 +173,27 @@
         default=NotSet,
         cache: bool = None,
         defer: bool = None,
         boolean: bool = None,
         verbose_name: str = None,
         order_field: t.Any = None,
     ) -> None:
-        self.annotate, self.attr, self.expression, self.defer = annotate, attr, expression, defer
+        self.annotate, self.attr, self.expression, self.defer = (
+            annotate,
+            attr,
+            expression,
+            defer,
+        )
         self.fget, self.fset, self.fdel, self.doc = getter, setter, deleter, doc
         self.output_field, self.default, self.cache = output_field, default, cache
-        self.boolean, self.verbose_name, self.order_field = verbose_name, order_field, boolean
+        self.boolean, self.verbose_name, self.order_field = (
+            verbose_name,
+            order_field,
+            boolean,
+        )
         if default is NotSet:
             self.get_default = None
         elif isinstance(default, _T_Func):  # pragma: no cover
             self.get_default = default
         else:
             self.get_default = lambda: default
 
@@ -255,15 +264,20 @@
             descriptor.__set_name__(cls, name)
 
         # print(f"{cls.__name__!r}, {self}", f"{cls.__query_aliases__.maps}", sep="\n -", end="\n\n")
 
         setattr(cls, name, descriptor)
 
     def _prepare(self, cls: t.Type[_T_Model], name: str):
-        annotate, attr, cache, expression = self.annotate, self.attr, self.cache, self.expression
+        annotate, attr, cache, expression = (
+            self.annotate,
+            self.attr,
+            self.cache,
+            self.expression,
+        )
         fget, fset, fdel, defer = self.fget, self.fset, self.fdel, self.defer
 
         if attr is None:
             lookup = attr
             if isinstance(expression, m.F):
                 lookup = expression.name
             elif isinstance(expression, str):
@@ -290,16 +304,27 @@
             else:
                 msg = (
                     "%s aliases cannot have an implicit `setter`. "
                     "Either provide custom `setter` or set `%s` to `False`."
                 ) % (("Annotated", "annotate") if annotate else ("Cached", "cache"))
             raise ImproperlyConfigured(f"alias {name!r} on {cls.__name__!r}. {msg}")
 
-        self.annotate, self.attr, self.cache, self.expression = annotate, attr, cache, expression
-        self.fget, self.fset, self.fdel, self.name, self.defer = fget, fset, fdel, name, defer
+        self.annotate, self.attr, self.cache, self.expression = (
+            annotate,
+            attr,
+            cache,
+            expression,
+        )
+        self.fget, self.fset, self.fdel, self.name, self.defer = (
+            fget,
+            fset,
+            fdel,
+            name,
+            defer,
+        )
 
     def get_descriptor_class(self, cls):
         return CachedAliasDescriptor if self.cache else DynamicAliasDescriptor
 
     def create_descriptor(self, cls):
         ret = self.get_descriptor_class(cls)(
             self.make_getter(),
@@ -316,15 +341,19 @@
                 fget = attrgetter(attr)
             else:
 
                 def fget(self: _T_Model):
                     nonlocal name
                     if self._state.adding:  # pragma: no cover
                         raise AttributeError(name)
-                    qs = self._meta.base_manager.filter(pk=self.pk).alias(name).annotate(name)
+                    qs = (
+                        self._meta.base_manager.filter(pk=self.pk)
+                        .alias(name)
+                        .annotate(name)
+                    )
                     return qs.values_list(name, flat=True).first()
 
         if fget and default is not None:
             fget_ = fget
 
             @wraps(fget_)
             def fget(self):
@@ -354,25 +383,29 @@
 
 
 class _Patcher:
     """Monkey patch Manager, Queryset and Model classes"""
 
     @staticmethod
     def model(cls: type[_T_Model]):
-        mro = (b.refresh_from_db for b in cls.__mro__ if "refresh_from_db" in b.__dict__)
+        mro = (
+            b.refresh_from_db for b in cls.__mro__ if "refresh_from_db" in b.__dict__
+        )
         if not all(getattr(b, "_loads_aliases_", None) for b in mro):
             orig_refresh_from_db = cls.refresh_from_db
 
             @wraps(orig_refresh_from_db)
             def refresh_from_db(self, using=None, fields=None):
                 nonlocal orig_refresh_from_db
                 if dct := get_query_aliases(self.__class__):
                     if fields_ := fields:
                         fields = list(fields)
-                        aliases = (n for n in fields if not (n in dct and not fields.remove(n)))
+                        aliases = (
+                            n for n in fields if not (n in dct and not fields.remove(n))
+                        )
                     else:
                         aliases = (n for n, a in dct.items() if a.cache)
 
                     for aka in aliases:
                         with suppress(AttributeError):
                             delattr(self, aka)
 
@@ -418,15 +451,17 @@
                     return {
                         n: m.F(n)
                         for n, a in get_query_aliases(self.model, {}).items()
                         if not a.defer and a.annotate
                     }
 
                 _initial_query_aliases_.__set_name__(cls, "_initial_query_aliases_")
-                _initial_query_annotations_.__set_name__(cls, "_initial_query_annotations_")
+                _initial_query_annotations_.__set_name__(
+                    cls, "_initial_query_annotations_"
+                )
 
                 cls._initial_query_aliases_ = _initial_query_aliases_
                 cls._initial_query_annotations_ = _initial_query_annotations_
 
     @staticmethod
     def queryset(cls: type[m.QuerySet[_T_Model]]):
         if not getattr(cls.annotate, "_loads_aliases_", None):
```

### Comparing `django_zana-0.2.8/zana/django/models/fields/__init__.py` & `django_zana-0.3.0a0/zana/django/models/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `django_zana-0.2.8/zana/django/models/fields/aliases.py` & `django_zana-0.3.0a0/zana/django/models/fields/aliases.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,84 +9,65 @@
 from logging import getLogger
 from operator import methodcaller, or_, setitem
 from threading import RLock
 from types import FunctionType, GenericAlias, MethodType, NoneType, new_class
 from weakref import WeakKeyDictionary
 
 from typing_extensions import Self
-from zana.common import cached_attr, pipeline
+from zana.canvas import maybe_compose
 from zana.types import NotSet
-from zana.types.collections import FrozenDict
+from zana.types.collections import DefaultDict, FrozenDict
+from zana.util import cached_attr
+from zana.util.operator import pipeline
 
 from django.conf import settings
 from django.core import checks
 from django.core.exceptions import ImproperlyConfigured
 from django.db import models as m
-from django.db.models.expressions import Combinable
 from django.db.models.functions import Coalesce
 from django.db.models.query_utils import FilteredRelation
 from django.dispatch import receiver
-from zana.django.models.fields import PseudoField
-from zana.django.utils import operator as op
+
+try:
+    from psycopg.types.json import Jsonb
+except ImportError:
+    Jsonb = None
+
+from . import PseudoField
 
 if t.TYPE_CHECKING:
     from django.db.backends.base.base import BaseDatabaseWrapper
 
 
 _T = t.TypeVar("_T")
 _KT = t.TypeVar("_KT")
 _FT = t.TypeVar("_FT")
 _VT = t.TypeVar("_VT")
 _T_Src = t.TypeVar("_T_Src")
 _T_Default = t.TypeVar("_T_Default")
 _T_Model = t.TypeVar("_T_Model", bound="ImplementsAliases", covariant=True)
 _T_Field = t.TypeVar("_T_Field", bound=m.Field, covariant=True)
 _T_Expr = t.Union[
-    Combinable,
+    m.expressions.Combinable,
     str,
-    t.Callable[[], Combinable | str],
+    t.Callable[[], m.expressions.Combinable | str],
 ]
 _T_Func = FunctionType | staticmethod | classmethod | MethodType | type
 
 logger = getLogger(__name__)
 debug = settings.DEBUG and logger.debug
 
 
 def get_alias_fields(model: type[_T_Model], default: _T_Default = None):
     fields = getattr(model, "_alias_fields_", None)
     if fields and isinstance(fields, ModelAliasFields):
         return fields
     return default
 
 
-class FallbackDict(dict[_KT, _VT | _FT], t.Generic[_KT, _FT, _VT]):
-    __slots__ = ("fallback",)
-    fallback: t.Final[_FT]
-
-    __dict_init = dict.__init__
-
-    def __init__(self, fallback: _FT = None, /, *args, **kwargs):
-        self.fallback = fallback
-        self.__dict_init(*args, **kwargs)
-
-    def __missing__(self, key: _KT):
-        return self.fallback
-
-    def __or__(self, x):
-        return self.__class__(self.fallback, {**self, **x})
-
-    def __ror__(self, x):
-        return self.__class__(self.fallback, {**x, **self})
-
-    def copy(self):
-        return self.__class__(self.fallback, self)
-
-    __copy__ = copy
-
-
 class ModelAliasFields(abc.Mapping[str, "AliasField"], t.Generic[_T_Model]):
     __slots__ = (
         "model",
         "_ready",
         "_populated",
         "_lock",
         "fields",
@@ -111,15 +92,20 @@
     cached: t.Final[abc.Mapping[str, "AliasField"]]
 
     _populated: t.Final[bool]
     _ready: t.Final[bool]
     _lock: t.Final[RLock]
 
     def __init__(self, model: type[_T_Model]) -> None:
-        self.model, self._lock, self._populated, self._ready = model, RLock(), False, False
+        self.model, self._lock, self._populated, self._ready = (
+            model,
+            RLock(),
+            False,
+            False,
+        )
 
     def prepare(self):
         with self._lock:
             if not self._ready:
                 self._prepare()
                 self.clear()
                 self._ready = True
@@ -127,15 +113,17 @@
     def _prepare(self):
         cls = self.model
         if cls._meta.proxy:
             concrete = cls._meta.concrete_model
             for b in cls.__mro__[1:][::-1]:
                 own = self.fields
                 if issubclass(b, ImplementsAliases):
-                    if b._meta.proxy or (b._meta.abstract and not issubclass(concrete, b)):
+                    if b._meta.proxy or (
+                        b._meta.abstract and not issubclass(concrete, b)
+                    ):
                         for n, af in b._alias_fields_.local.items():
                             if n not in own:
                                 cls._meta.add_field(copy.deepcopy(af), True)
                             elif own[n] != af:
                                 raise ImproperlyConfigured(
                                     f"cannot override AliasField `{af!s}` in `{cls._meta.label}`"
                                 )
@@ -154,15 +142,20 @@
                 name, maps = field.name, [fields]
                 maps.append(cache if field.cache else dynamic)
                 maps.append(defer if field.defer else eager)
                 field.model is self.model and maps.append(local)
                 field.select and maps.append(select)
                 [map.setdefault(name, field) for map in maps]
 
-        self.fields, self.eager, self.deferred, self.selected = fields, eager, defer, select
+        self.fields, self.eager, self.deferred, self.selected = (
+            fields,
+            eager,
+            defer,
+            select,
+        )
         self.local, self.cached, self.dynamic = local, cache, dynamic
 
     def clear(self):
         with self._lock:
             if self._populated:
                 for at in self._reset_attrs_:
                     if hasattr(self, at):
@@ -237,15 +230,15 @@
         return self.fields.items()
 
 
 class ImplementsAliasesManager(
     ABC, m.Manager[_T_Model] if t.TYPE_CHECKING else t.Generic[_T_Model]
 ):
     model: type[_T_Model]
-    _initial_alias_fields_: t.Final[abc.Mapping[str, Combinable]] = ...
+    _initial_alias_fields_: t.Final[abc.Mapping[str, m.expressions.Combinable]] = ...
     _initial_annotated_alias_fields_: t.Final[abc.Mapping[str, m.F]] = ...
 
 
 class ImplementsAliases(ABC, m.Model if t.TYPE_CHECKING else object):
     _alias_fields_: t.Final[ModelAliasFields[Self]] = None
 
     @classmethod
@@ -254,60 +247,14 @@
             cls._alias_fields_ = ModelAliasFields(cls)
 
         self.register(cls)
         cls._alias_fields_.clear()
         return cls
 
 
-class ExpressionBuilder(t.Generic[_T]):
-    __slots__ = ("__alias__", "__src__", "__expr__")
-
-    __alias__: t.Final["AliasField[_T]"]
-    __expr__: t.Final[tuple[_T_Expr, ...]]
-    __src__: t.Final[op.Accessor]
-
-    if t.TYPE_CHECKING:
-        __alias__ = __src__ = __expr__ = None
-
-    def __new__(
-        cls, alias: "AliasField[_T]", src: op.Accessor = None, expr: tuple[_T_Expr] = ()
-    ) -> Self:
-        self = object.__new__(cls)
-        self.__alias__, self.__src__, self.__expr__ = alias, src or op.Accessor(), tuple(expr or ())
-        return self
-
-    def __build__(self) -> "AliasField":
-        if src := self.__src__:
-            alias, expression = self.__alias__, self.__alias__.expression
-            if (e_list := not alias.has_expression() and self.__expr__) and None not in e_list:
-                expression = m.F("__".join(e_list))
-            return alias.alias_evolve(expression=expression, source=src)
-        raise TypeError(f"cannot build empty expression")
-
-    def __extend__(self, src=None, expr=None):
-        return self.__class__(self.__alias__, self.__src__ | (src or ()), self.__expr__ + (expr,))
-
-    def __getattr__(self, name: str):
-        if not isinstance(name, str) or name[:2] == "__" == name[-2:]:
-            raise AttributeError(name)
-        return self.__extend__(op.Attr(name), str(name))
-
-    def __getitem__(self, key):
-        if isinstance(key, slice):
-            return self.__extend__(op.Slice(key))
-        else:
-            return self.__extend__(op.Item(key), str(key) if isinstance(key, (str, int)) else None)
-
-    def __call__(self, *args, **kwargs):
-        return self.__extend__(op.Call(*args, **kwargs))
-
-    def contribute_to_class(self, cls: t.Type[_T_Model], name: str, *a, **kw):
-        return self.__build__().contribute_to_class(cls, name, *a, **kw)
-
-
 class BaseAliasDescriptor:
     field: "AliasField" = None
 
     def __init__(self, field: "AliasField") -> None:
         self.field = field
         super().__init__(field.get_getter(), field.get_setter(), field.get_deleter())
 
@@ -319,24 +266,30 @@
 class CachedAliasDescriptor(BaseAliasDescriptor, cached_attr[_T]):
     pass
 
 
 class ConcreteTypeRegistryType(type):
     _internal_type_map_: abc.Mapping[type[_T_Field], "type[_T_Field | AliasField]"]
     _name_type_map_: abc.Mapping[type[_T_Field], "type[_T_Field] | type[AliasField]"]
-    _json_compat_types_: abc.Mapping[type[_T_Field], "type[_T_Field] | type[m.JSONField]"]
+    _json_compat_types_: abc.Mapping[
+        type[_T_Field], "type[_T_Field] | type[m.JSONField]"
+    ]
     _base_: t.Final[type["AliasField"]]
     _basename_: t.Final[str]
     _lock_: RLock
     _concrete_init_defaults_: abc.Mapping[type[_T_Field], abc.Mapping[str, t.Any]]
 
     def __new__(self, name, bases, nspace: dict, /, **kw) -> None:
         cls = super().__new__(self, name, bases, nspace, **kw)
         cls._lock_ = RLock()
-        cls._internal_type_map_, cls._name_type_map_, cls._json_compat_types_ = {}, {}, {}
+        cls._internal_type_map_, cls._name_type_map_, cls._json_compat_types_ = (
+            {},
+            {},
+            {},
+        )
         return cls
 
     def __set_name__(self, owner: type["AliasField"], name: str):
         if not hasattr(self, "_base_"):
             self._base_ = owner
 
         if not hasattr(self, "_basename_"):
@@ -354,41 +307,42 @@
     def __getitem__(self, cls: type[_T_Field]):
         with self._lock_:
             try:
                 return self._internal_type_map_[cls]
             except KeyError:
                 return self(cls)
 
-    def __call__(self: type["ConcreteTypeRegistry"], cls: type[_T_Field], /, name: str = None):
+    def __call__(
+        self: type["ConcreteTypeRegistry"], cls: type[_T_Field], /, name: str = None
+    ):
         c2t: dict[type[cls], type[cls] | type["AliasField"]]
         n2t: dict[str, type[cls] | type["AliasField"]]
 
         assert isinstance(cls, type) and issubclass(cls, m.Field)
-        base, c2t, n2t = self._new_base_(cls), self._internal_type_map_, self._name_type_map_
-        assert issubclass(base, cls)
+        c2t, n2t = self._internal_type_map_, self._name_type_map_
 
         with self._lock_:
             assert (
-                c not in c2t for c in (cls, base)
+                c not in c2t for c in (cls, cls)
             ), f"type for concrete base {cls.__name__} already exists"
-            name = self._new_name_(name or base.__name__)
+            name = self._new_name_(name or cls.__name__)
             module, qualname = self.__module__, f"{self.__qualname__}.{name}"
 
-            n2t[name] = c2t[cls] = c2t[base] = new_class(
+            n2t[name] = c2t[cls] = c2t[cls] = new_class(
                 name,
-                (self._base_, base),
+                (self._base_, cls),
                 None,
                 methodcaller(
                     "update",
                     self._new_class_dict_(
-                        base,
+                        cls,
                         {
                             "__module__": module,
                             "__qualname__": qualname,
-                            "_internal_field_type_": base,
+                            "_internal_field_type_": cls,
                         },
                     ),
                 ),
             )
         return n2t[name]
 
     def json_compat_type(
@@ -407,14 +361,16 @@
                 return klass
 
             if issubclass(base, json_base):
                 return self._json_compat_types_.setdefault(key, base)
 
             dump_vendors = {"postgresql", "mysql"}
             non_dump_types = NoneType | _JSONString
+            if Jsonb:
+                non_dump_types |= Jsonb
 
             class Base(base):
                 pass
 
             class JSONCompatBase(json_base, Base):
                 _has_base_from_db_value_ = hasattr(base, "from_db_value")
                 __module__ = base.__module__
@@ -422,26 +378,30 @@
                 __qualname__ = base.__qualname__
 
                 def get_internal_type(self):
                     return super(Base, self).get_internal_type()
 
                 def get_prep_value(self, value, *, dump=None, prepared=True):
                     values = [value, None, None]
+                    vcls = type(value)
                     if not (dump and prepared):
                         value = super(Base, self).get_prep_value(value)
                         values[1] = value
                     if dump and value is not None:
                         value = super().get_prep_value(value)
                         if isinstance(value, str):
                             value = _JSONString(value)
                         values[2] = value
                     return value
 
                 def should_json_dump(self, value, conn: "BaseDatabaseWrapper"):
-                    return not isinstance(value, non_dump_types) and conn.vendor in dump_vendors
+                    return (
+                        not isinstance(value, non_dump_types)
+                        and conn.vendor in dump_vendors
+                    )
 
                 def get_db_prep_value(
                     self, value, connection: "BaseDatabaseWrapper", prepared=False
                 ):
                     values = [value, None, None]
                     value = super().get_db_prep_value(value, connection, prepared)
                     values[1] = value
@@ -451,48 +411,48 @@
                     return value
 
                 def from_db_value(self, value, expr, connection: "BaseDatabaseWrapper"):
                     nonlocal base, json_base
                     if value is not None:
                         if isinstance(value, (str, bytes, bytearray)):
                             if connection.vendor in dump_vendors:
-                                value = json_base.from_db_value(self, value, expr, connection)
+                                value = json_base.from_db_value(
+                                    self, value, expr, connection
+                                )
                         if self._has_base_from_db_value_:
                             value = base.from_db_value(self, value, expr, connection)
                     return value
 
+                def formfield(self, **kwargs):
+                    return super(Base, self).formfield(**kwargs)
+
             klass = self._json_compat_types_.setdefault(key, JSONCompatBase)
             return klass
 
     def _new_name_(self, base: str):
         n2t = self._name_type_map_.keys() | self.__dict__.keys()
         with self._lock_:
             base = f"{base.replace('Field', '')}{self._basename_}Field"
             for i in range(1000):
                 name = f"{base}_{i:03}" if i else base
                 if name not in n2t:
                     return name
             else:  # pragma: no cover
-                raise RuntimeError(f"unable to find a unique qualname for {name[:-3]!r}")
-
-    def _new_base_(self, cls: type[_T_Field]):
-        return cls
-
-    def _new_init_defaults_(self, cls: type[_T_Field]):
-        by_type = self._concrete_init_defaults_
-        return reduce(
-            or_,
-            [
-                *(by_type[b] for b in cls.__mro__[::-1] if b in by_type),
-                self._base_._INIT_DEFAULTS_,
-            ],
-        )
+                raise RuntimeError(
+                    f"unable to find a unique qualname for {name[:-3]!r}"
+                )
 
     def _new_class_dict_(self: type[Self], cls: type[_T_Field], nspace: dict):
-        return nspace | {"_INIT_DEFAULTS_": self._new_init_defaults_(cls)}
+        by_type, defaults = self._concrete_init_defaults_, self._base_._INIT_DEFAULTS_
+        return nspace | {
+            "_INIT_DEFAULTS_": reduce(
+                or_,
+                [*(by_type[b] for b in cls.__mro__[::-1] if b in by_type), defaults],
+            )
+        }
 
 
 class _JSONString(str):
     __slots__ = ()
 
     def __repr__(self) -> str:  # pragma: no cover
         return f"{self.__class__.__name__.strip('_')}({self!s})"
@@ -543,54 +503,52 @@
         "expression",
         "getter",
         "setter",
         "deleter",
     ]
 
     _KWARGS_TO_ATTRS_ = {
-        "expression": op.Attr("expression"),
-        "getter": op.Attr("fget"),
-        "setter": op.Attr("fset"),
-        "deleter": op.Attr("fdel"),
-        "select": op.Attr("select"),
-        "source": op.Attr("_source"),
-        "coalesce": op.Attr("_coalesce"),
-        "cache": op.Attr("cache"),
-        "defer": op.Attr("defer"),
-        "cast": op.Attr("cast"),
-        "wrap": op.Attr("_wrap"),
-        "json": op.Attr("json"),
-        "json_options": op.Attr("_json_options"),
+        "expression": "expression",
+        "getter": "fget",
+        "setter": "fset",
+        "deleter": "fdel",
+        "select": "select",
+        "coalesce": "_coalesce",
+        "cache": "cache",
+        "defer": "defer",
+        "cast": "cast",
+        "wrap": "_wrap",
+        "json": "json",
+        "json_options": "_json_options",
     }
-    _INIT_DEFAULTS_ = FallbackDict(
+    _INIT_DEFAULTS_ = DefaultDict(
+        (),
         NotSet,
         expression=None,
         getter=None,
         setter=None,
         deleter=None,
-        editable=False,
-        default=None,
         defer=False,
         cast=None,
+        default=None,
         json=None,
-        source=None,
         select=False,
         wrap=None,
         coalesce=False,
-        json_options=None,
+        json_options=lambda: dict(encoder=None, decoder=None),
     )
-    _NULLABLE_INIT_DEFAULTS_ = {"select", "coalesce", "defer"}
+    _NULLABLE_INIT_DEFAULTS_ = {"select", "coalesce", "defer", "json_options"}
 
     name: str
     expression: _T_Expr = None
     _init_args_: t.Final[set]
     json: bool
 
     verbose_name: str
-    _source: str | op.Accessor
+    # _source: str | Composable
     _coalesce: _T_Expr | bool | None
     _cached_descriptor_class_ = CachedAliasDescriptor
     _dynamic_descriptor_class_ = DynamicAliasDescriptor
 
     cast: bool
     fget: abc.Callable[[_T_Model], _T] = None
     fset: abc.Callable[[_T_Model, _T], t.NoReturn] = None
@@ -609,36 +567,39 @@
             params = (params,)
 
         if cls._internal_field_type_ is None:
             if isinstance(param := params[0], type) and issubclass(param, m.Field):
                 cls, params = cls.types[param], params[1:]
         return GenericAlias(cls, params)
 
-    def __new__(cls: type[Self], *a, internal: _T_Field = None, **kw) -> _T | Self | _T_Field:
+    def __new__(
+        cls: type[Self], *a, internal: _T_Field = None, **kw
+    ) -> _T | Self | _T_Field:
         if internal is not None and cls._internal_field_type_ is None:
-            cls = cls.types[internal if isinstance(internal, type) else internal.__class__]
+            cls = cls.types[
+                internal if isinstance(internal, type) else internal.__class__
+            ]
 
         self: _T | Self | _T_Field = object.__new__(cls)
         return self
 
     def __init_subclass__(cls, **kw) -> None:
         cls._internal_field_type_ = cls.__dict__.get("_internal_field_type_")
         cls._lock_ = cls.__dict__.get("_lock_", RLock())
         return super().__init_subclass__(**kw)
 
     @t.overload
     def __init__(
         self,
         expression: _T_Expr = None,
         getter: t.Union[abc.Callable[[_T_Model], _T], bool] = None,
-        setter: t.Union[abc.Callable[[_T_Model, _T], t.NoReturn], bool] = None,
+        setter: abc.Callable[[_T_Model, _T], t.NoReturn] = None,
         deleter: abc.Callable[[_T_Model], t.NoReturn] = None,
         *,
         select: bool = None,
-        source: str | op.Accessor = None,
         cache: bool = None,
         defer: bool = None,
         cast: bool = None,
         wrap: bool = None,
         coalesce: _T_Expr | bool | None,
         json: bool = False,
         json_options: abc.Mapping[str, t.Any] = None,
@@ -646,15 +607,15 @@
         **kwds,
     ) -> None:
         ...
 
     def __init__(self, *args, internal: _T_Field = None, **kwds) -> None:
         self._init_args_ = set()
         args = args and kwds.update({k: v for k, v in zip(self._POS_ARGS_, args)}) or ()
-        kwds, k2a = self._INIT_DEFAULTS_ | kwds, self._KWARGS_TO_ATTRS_
+        kwds, k2a = self._init_defaults_ | kwds, self._KWARGS_TO_ATTRS_
         local = {k: kwds.pop(k) for k in list(kwds) if k in k2a}
 
         if internal is not None:
             my_internal = self._internal_field_type_
             if internal.__class__ is my_internal:
                 *_, args, kwargs = internal.deconstruct()
                 kwds |= kwargs
@@ -667,76 +628,126 @@
     @property
     def _weak_cache_(self):
         if (cache := self._weak_cache_map_.get(self)) is None:
             cache = self._weak_cache_map_.setdefault(self, {})
         return cache
 
     @cached_attr
+    def _init_defaults_(self):
+        return self._INIT_DEFAULTS_ | {
+            k: v() if callable(v) else v for k, v in self._INIT_DEFAULTS_.items()
+        }
+
+    @cached_attr
     def f(self):
         return m.F(self.name)
 
     @cached_attr
     def coalesce(self):
         if (val := self._coalesce) is True:
             default, val = self.get_default(), None
             if default is not None:
                 val = m.Value(default, self.get_internal_field())
         return val or None
 
     @cached_attr
     def cache(self):
-        return not not self.select or not (self.fset or self.source)
-
-    @cached_attr
-    def cache(self):
-        return not not self.select or not (self.fset or self.source)
+        return not not self.select or not self.fset
 
     @property
     def json_field_options(self):
         return {"encoder": None, "decoder": None} | (self._json_options or {})
 
     @property
     def wrap(self) -> bool:
         cast, wrap = self.cast, self._wrap
         if wrap and cast:
-            raise TypeError(f"{self} arguments `wrap=True` and `cast=True` are mutually exclusive.")
+            raise TypeError(
+                f"{self} arguments `wrap=True` and `cast=True` are mutually exclusive."
+            )
         elif wrap is None:
             wrap = not (cast or self.is_json)
         return not not wrap
 
     @property
     @_weak_cached
     def is_json(self):
         if self.json is not None:
             return self.json
 
         for cls in self.get_concrete_field_path()[0][::-1]:
-            if isinstance(cls, m.JSONField) or (isinstance(cls, AliasField) and cls.is_json):
+            if isinstance(cls, m.JSONField) or (
+                isinstance(cls, AliasField) and cls.is_json
+            ):
                 return True
 
-    @property
+    def alias_evolve(self, arg=(), **kwds):
+        if isinstance(arg, abc.Mapping):
+            arg = arg.items()
+        k2a, ia = self._KWARGS_TO_ATTRS_, self._init_args_
+        for kv in (
+            ((kv for kv in arg if kv[0] not in kwds), kwds.items()) if kwds else (arg,)
+        ):
+            for k, v in kv:
+                setattr(self, k2a[k], maybe_compose(v)), ia.add(k)
+        return self
+
+    if t.TYPE_CHECKING:
+        alias_evolve: type[Self]
+
+    def annotation(self, expression: _T_Expr):
+        self.alias_evolve(expression=expression)
+        return expression
+
+    def getter(self, fget: t.Callable[[t.Any], _T]):
+        self.alias_evolve(getter=fget)
+        return fget
+
+    def setter(self, fset: t.Callable[[t.Any], _T]):
+        self.alias_evolve(setter=fset)
+        return fset
+
+    def deleter(self, fdel: t.Callable):
+        self.alias_evolve(deleter=fdel)
+        return fdel
+
+    def has_expression(self):
+        return self.expression is not None
+
     @_weak_cached
-    def source(self):
-        src = self._source
-        if isinstance(src, op.Accessor):
-            return src
-        elif isinstance(src, str):
-            return op.Accessor(op.Attr(src))
-        elif isinstance(src, abc.Iterable):
-            return op.Accessor(*src)
-        elif src is not None:
-            raise TypeError(f"`{self!s}.source` expected `str` or `Accessor` but got {type(src)}")
-        if isinstance(expr := self.expression, str):
-            return op.Accessor(op.Attr(expr.replace("__", ".")))
+    def get_expression(self) -> m.expressions.Combinable:
+        expr = self.expression
+        if isinstance(expr, _T_Func):
+            expr = expr()
+        if isinstance(expr, str):
+            expr = m.F(expr)
+
+        return expr
+
+    @_weak_cached
+    def get_annotation(self):
+        expr, internal = self.get_expression(), self.get_internal_field()
+        if expr is not None:
+            cast, coalesce, wrap = self.cast, self.coalesce, self.wrap
+            if wrap and internal:
+                expr = m.ExpressionWrapper(expr, internal)
+            if coalesce is not None:
+                expr = Coalesce(expr, coalesce)
+            if cast and internal:
+                expr = m.functions.Cast(expr, internal)
+        return expr
 
     @_weak_cached
     def get_internal_json_field(self) -> m.JSONField:
         if not self.is_json:
             return
-        internal, (path, part) = self._internal_field_type_, self.get_concrete_field_path()
+        internal, (path, part) = (
+            self._internal_field_type_,
+            self.get_concrete_field_path(),
+        )
         base = m.JSONField
         for field in path[::-1]:
             f_cls = field.__class__
             if issubclass(f_cls, base):
                 base = f_cls
                 break
 
@@ -777,24 +788,30 @@
         if cls is not None:
             return cls(*args, **kwds)
 
     def get_deconstructing_internal_field(self):
         if (cls := self._internal_field_type_) is not None:
             *_, args, kwds = cls.deconstruct(self)
             nulls = self._NULLABLE_INIT_DEFAULTS_
-            for k, v in self._INIT_DEFAULTS_.items():
+            for k, v in self._init_defaults_.items():
                 if k in kwds and (kwds[k] == v or (k in nulls and kwds[k] is None)):
                     kwds.pop(k)
             return cls(*args, **kwds)
 
     def get_concrete_field_path(self) -> tuple[tuple[_T_Field, ...], str | None]:
-        if not isinstance((expr := self.get_expression()), m.F):
+        expr = self.get_expression()
+        if not (hasattr(self, "model") and isinstance(expr, m.F)):
             return (), None
 
-        model, path, field, (seg, _, rem) = self.model, [], None, expr.name.partition("__")
+        model, path, field, (seg, _, rem) = (
+            self.model,
+            [],
+            None,
+            expr.name.partition("__"),
+        )
         while seg:
             try:
                 field = model._meta.get_field(seg)
             except Exception:
                 rem = f"{seg}__{rem}" if rem else seg
                 break
             else:
@@ -810,90 +827,76 @@
                 elif not field.is_relation:
                     break
                 model = field.related_model
                 seg, _, rem = rem.partition("__")
 
         return tuple(path), rem or None
 
-    def contribute_to_class(self, cls: type[_T_Model], name: str, private_only: bool = None):
+    def contribute_to_class(
+        self, cls: type[_T_Model], name: str, private_only: bool = None
+    ):
         if private_only is None:
             private_only = cls._meta.proxy
 
         super().contribute_to_class(cls, name, private_only=private_only)
 
         cls = ImplementsAliases.setup(cls)
 
         if descriptor := self.get_descriptor():
             if hasattr(descriptor, "__set_name__"):
                 descriptor.__set_name__(cls, self.attname)
             setattr(cls, self.attname, descriptor)
 
     def deconstruct(self):
-        k2a, ia, defaults = self._KWARGS_TO_ATTRS_, self._init_args_, self._INIT_DEFAULTS_
-        (name, path), cls = t.cast(tuple[str, str], super().deconstruct()[:2]), self.__class__
+        k2a, ia, defaults = (
+            self._KWARGS_TO_ATTRS_,
+            self._init_args_,
+            self._init_defaults_,
+        )
+        (name, path), cls = (
+            t.cast(tuple[str, str], super().deconstruct()[:2]),
+            self.__class__,
+        )
 
         nulls = self._NULLABLE_INIT_DEFAULTS_
         args, kwargs = [], {
-            k: v for k in ia if ((v := k2a[k](self)) is None and k in nulls) or v != defaults[k]
+            k: v
+            for k in ia
+            if ((v := getattr(self, k2a[k])) is None and k in nulls) or v != defaults[k]
         }
         if self._internal_field_type_:
             kwargs["internal"] = self.get_deconstructing_internal_field()
 
-        if "source" in kwargs:
-            kwargs["source"] = self.source.deconstruct()[1]
-
-        base, prefix = cls.types._base_, __name__[: __name__.index(".models.fields.") + 8]
+        base, prefix = (
+            cls.types._base_,
+            __name__[: __name__.index(".models.fields.") + 8],
+        )
         path = path.replace(f"{__name__}.", prefix, 1)
         path = re.sub(f"\.{base.__name__}\.types\..+", f".{base.__name__}", path)
         return name, path, args, kwargs
 
     def check(self, **kwargs):
         return super().check(**kwargs) + [
             *self._check_alias_expression(),
-            *self._check_alias_setter(),
+            *self._check_access_mutators(),
         ]
 
-    def _check_alias_setter(self):
-        source, select, cache, errors = self.source, self.select, self.cache, []
-        if self.fset is True and (not source or select or cache):
-            label = f"{self.__class__.__qualname__}"
-            if select:
-                errors += [
-                    checks.Error(
-                        f"Select {label} cannot have an implicit setter=True",
-                        hint=(
-                            "Set select=False, use a custom `setter` function, "
-                            "or remove setter=True argument on the field."
-                        ),
-                        obj=self,
-                        id="AliasField.E003",
-                    )
-                ]
-            elif cache:
-                errors += [
-                    checks.Error(
-                        f"Cached {label} cannot have an implicit `setter=True. ",
-                        hint=(
-                            "Set cache=False, use a custom `setter` function, "
-                            "or remove setter=True argument on the field."
-                        ),
-                        obj=self,
-                        id="AliasField.E004",
-                    )
-                ]
-            else:
+    def _check_access_mutators(self) -> list[checks.Error]:
+        errors, k2a = [], self._KWARGS_TO_ATTRS_
+
+        tp, gt = abc.Callable | None, abc.Callable | bool | None
+        for i, arg in enumerate(("getter", "setter", "deleter"), 2):
+            val, tt = getattr(self, k2a[arg]), gt if arg == "getter" else tp
+            if not isinstance(val, tt):
                 errors += [
                     checks.Error(
-                        f"{label}s with setter=True must have a `source`.",
-                        hint=(
-                            "Explicitly set `source`, use a custom `setter` function, "
-                            "or remove setter=True argument on the field."
-                        ),
+                        f"{arg} argument cannot be of type {val.__class__.__name__}.",
+                        hint=(f"Ensure {arg} argument is of type {tt}."),
                         obj=self,
-                        id="AliasField.E005",
+                        id=f"AliasField.E{i:03}",
                     )
                 ]
 
         return errors
 
     def _check_alias_expression(self):
         cast, internal, errors = self.cast, self.get_internal_field(), []
@@ -904,142 +907,79 @@
                     f"{label} with cast=True must have an internal type",
                     hint=(
                         f"Set internal=Field() argument, "
                         f"remove cast=True argument, or use {label}[FieldClass]() "
                         f"to create field with `FieldClass` as the internal type."
                     ),
                     obj=self,
-                    id="AliasField.E002",
+                    id="AliasField.E001",
                 )
             ]
         return errors
 
     def get_descriptor(self):
         if (cls := self.get_descriptor_class()) is not None:
             return cls(self)
 
     def get_descriptor_class(self):
-        return getattr(self, f"_{'cached' if self.cache else 'dynamic'}_descriptor_class_")
-
-    def alias_evolve(self, arg=(), **kwds):
-        if isinstance(arg, abc.Mapping):
-            arg = arg.items()
-        k2a, ia = self._KWARGS_TO_ATTRS_, self._init_args_
-        for kv in ((kv for kv in arg if kv[0] not in kwds), kwds.items()) if kwds else (arg,):
-            for k, v in kv:
-                k2a[k].set(self, v)
-                ia.add(k)
-        return self
-
-    if t.TYPE_CHECKING:
-        alias_evolve: type[Self]
-
-    def to(self, src: _T_Src) -> _T_Src:
-        return ExpressionBuilder[_T](self)
-
-    def annotation(self, expression: _T_Expr):
-        self.alias_evolve(expression=expression)
-        return expression
-
-    def getter(self, fget: t.Callable[[t.Any], _T]):
-        self.alias_evolve(getter=fget)
-        return fget
-
-    def setter(self, fset: t.Callable[[t.Any], _T]):
-        self.alias_evolve(setter=fset)
-        return fset
-
-    def deleter(self, fdel: t.Callable):
-        self.alias_evolve(deleter=fdel)
-        return fdel
-
-    def has_expression(self):
-        return self.expression is not None
-
-    @_weak_cached
-    def get_expression(self) -> m.expressions.Combinable:
-        expr = self.expression
-        if isinstance(expr, _T_Func):
-            expr = expr()
-        if isinstance(expr, str):
-            expr = m.F(expr)
-
-        return expr
-
-    @_weak_cached
-    def get_annotation(self):
-        expr, internal = self.get_expression(), self.get_internal_field()
-        if expr is not None:
-            cast, coalesce, wrap = self.cast, self.coalesce, self.wrap
-            if wrap and internal:
-                expr = m.ExpressionWrapper(expr, internal)
-            if coalesce is not None:
-                expr = Coalesce(expr, coalesce)
-            if cast and internal:
-                expr = m.functions.Cast(expr, internal)
-        return expr
+        return getattr(
+            self, f"_{'cached' if self.cache else 'dynamic'}_descriptor_class_"
+        )
 
     def get_getter(self):
         fget = self.fget
         if fget in (True, None):
-            if (source := self.source) is not None:
-                fget = source.get
-            else:
-                select, defer, name = self.select, self.defer, self.name
+            select, defer, name = self.select, self.defer, self.name
 
-                def fget(self: _T_Model):
-                    nonlocal name, defer, select
-                    if self._state.adding:
-                        raise AttributeError(name)
-                    qs = self._meta.base_manager.filter(pk=self.pk)
-                    if defer:
-                        qs = qs.alias(name)
-                    if not select:
-                        qs = qs.annotate(name)
-                    return qs.values_list(name, flat=True).get()
+            def fget(self: _T_Model):
+                nonlocal name, defer, select
+                if self._state.adding:
+                    raise AttributeError(name)
+                qs = self._meta.base_manager.filter(pk=self.pk)
+                if defer:
+                    qs = qs.alias(name)
+                if not select:
+                    qs = qs.annotate(name)
+                return qs.values_list(name, flat=True).get()
 
         if fget and self.has_default():
             fget_, field = fget, self
 
             @wraps(fget_)
             def fget(self):
                 nonlocal field, fget_
                 try:
                     val = fget_(self)
-                except AttributeError:
+                except (AttributeError, LookupError):
                     val = None
                 return field.get_default() if val is None else val
 
         return fget or None
 
     def get_setter(self):
-        source, func = self.source, self.fset
-        if func is True and source:
-            func = source.set
-        return func or None
+        return self.fset
 
     def get_deleter(self):
-        source, func = self.source, self.fdel
-        if func is True and source:
-            func = source.delete
-        return func or None
+        return self.fdel
 
 
 @receiver(m.signals.class_prepared, weak=False)
 def __on_class_prepared(sender: type[_T_Model], **kwds):
     if issubclass(sender, ImplementsAliases):
         ImplementsAliases.setup(sender)._alias_fields_.prepare()
 
 
 class _Patcher:
     """Monkey patch Manager, Queryset and Model classes"""
 
     @staticmethod
     def model(cls: type[_T_Model]):
-        mro = (b.refresh_from_db for b in cls.__mro__ if "refresh_from_db" in b.__dict__)
+        mro = (
+            b.refresh_from_db for b in cls.__mro__ if "refresh_from_db" in b.__dict__
+        )
         if not all(getattr(b, "_zana_checks_alias_fields_", None) for b in mro):
             orig_refresh_from_db = cls.refresh_from_db
 
             @wraps(orig_refresh_from_db)
             def refresh_from_db(self: _T_Model, using=None, fields=None):
                 nonlocal orig_refresh_from_db
                 cls = self.__class__
@@ -1088,15 +1028,17 @@
                 def _initial_alias_fields_(self: m.Manager[_T_Model]):
                     if aliases := get_alias_fields(self.model):
                         return {n: a.get_annotation() for n, a in aliases.eager.items()}
 
                 @cached_attr
                 def _initial_annotated_alias_fields_(self: m.Manager[_T_Model]):
                     if aliases := get_alias_fields(self.model):
-                        return {n: a.f for n, a in aliases.selected.items() if not a.defer}
+                        return {
+                            n: a.f for n, a in aliases.selected.items() if not a.defer
+                        }
 
                 _initial_alias_fields_.__set_name__(cls, "_initial_alias_fields_")
                 _initial_annotated_alias_fields_.__set_name__(
                     cls, "_initial_annotated_alias_fields_"
                 )
 
                 cls._initial_alias_fields_ = _initial_alias_fields_
@@ -1119,15 +1061,16 @@
                                 n := a
                                 if isinstance(a, str)
                                 else a.name
                                 if isinstance(a, m.F)
                                 else None
                             )
                             and n in aliases
-                            and kwds.setdefault(n, (an := m.F(n) if a is n else a)) is an
+                            and kwds.setdefault(n, (an := m.F(n) if a is n else a))
+                            is an
                         )
                     ]
                 return orig_annotate(self, *args, **kwds)
 
             annotate._zana_checks_alias_fields_ = True
             cls.annotate = annotate
 
@@ -1178,15 +1121,16 @@
 
                 for arg in args:
                     # The default_alias property may raise a TypeError.
                     try:
                         if arg.default_alias in kwargs:
                             raise ValueError(
                                 "The named annotation '%s' conflicts with the "
-                                "default name for another annotation." % arg.default_alias
+                                "default name for another annotation."
+                                % arg.default_alias
                             )
                     except TypeError:
                         raise TypeError("Complex annotations require an alias")
                     annotations[arg.default_alias] = arg
                 annotations.update(kwargs)
 
                 clone: cls[_T_Model] = self._chain()
@@ -1202,25 +1146,21 @@
                     )
                     if aliases:
                         names -= aliases.keys()
 
                 for alias, annotation in annotations.items():
                     if alias in names:
                         raise ValueError(
-                            "The annotation '%s' conflicts with a field on " "the model." % alias
+                            "The annotation '%s' conflicts with a field on "
+                            "the model." % alias
                         )
                     if isinstance(annotation, FilteredRelation):
                         clone.query.add_filtered_relation(annotation, alias)
                     else:
-                        clone.query.add_annotation(
-                            annotation,
-                            alias,
-                            is_summary=False,
-                            select=select,
-                        )
+                        clone.query.add_annotation(annotation, alias, select=select)
                 for alias, annotation in clone.query.annotations.items():
                     if alias in annotations and annotation.contains_aggregate:
                         if clone._fields is None:
                             clone.query.group_by = True
                         else:
                             clone.query.set_group_by()
                         break
```

### Comparing `django_zana-0.2.8/PKG-INFO` & `django_zana-0.3.0a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-zana
-Version: 0.2.8
+Version: 0.3.0a0
 Summary: A `django` extension for `zana`.
 License: MIT
 Author: David Kyalo
 Author-email: davidmkyalo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Django (>=3.2.0)
 Requires-Dist: typing-extensions (>=4.4.0)
-Requires-Dist: zana (>=0.1.10,<0.2.0)
+Requires-Dist: zana (>=0.2.0a4,<0.3.0)
```

