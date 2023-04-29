# Comparing `tmp/pysigma-0.9.6.tar.gz` & `tmp/pysigma-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma-0.9.6.tar", max compression
+gzip compressed data, was "pysigma-0.9.7.tar", max compression
```

## Comparing `pysigma-0.9.6.tar` & `pysigma-0.9.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    26526 2023-04-05 07:06:31.884199 pysigma-0.9.6/LICENSE
--rw-r--r--   0        0        0     9849 2023-04-05 07:06:31.884199 pysigma-0.9.6/README.md
--rw-r--r--   0        0        0      992 2023-04-05 07:06:31.888199 pysigma-0.9.6/pyproject.toml
--rw-r--r--   0        0        0      238 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/backends/test/__init__.py
--rw-r--r--   0        0        0     5421 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/backends/test/backend.py
--rw-r--r--   0        0        0     8202 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/collection.py
--rw-r--r--   0        0        0     9805 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/conditions.py
--rw-r--r--   0        0        0        0 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/conversion/__init__.py
--rw-r--r--   0        0        0    50318 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/conversion/base.py
--rw-r--r--   0        0        0     3401 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/conversion/deferred.py
--rw-r--r--   0        0        0     1307 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/conversion/state.py
--rw-r--r--   0        0        0    43469 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/data/mitre_attack.py
--rw-r--r--   0        0        0     3735 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/exceptions.py
--rw-r--r--   0        0        0    13738 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/modifiers.py
--rw-r--r--   0        0        0     8799 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/pipelines/common.py
--rw-r--r--   0        0        0      212 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/pipelines/test/__init__.py
--rw-r--r--   0        0        0      874 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/pipelines/test/pipeline.py
--rw-r--r--   0        0        0     8133 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/plugins.py
--rw-r--r--   0        0        0        0 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/processing/__init__.py
--rw-r--r--   0        0        0    10299 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/processing/conditions.py
--rw-r--r--   0        0        0    15823 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/processing/pipeline.py
--rw-r--r--   0        0        0     3680 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/processing/resolver.py
--rw-r--r--   0        0        0     2763 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/processing/tracking.py
--rw-r--r--   0        0        0    24020 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/processing/transformations.py
--rw-r--r--   0        0        0    30775 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/rule.py
--rw-r--r--   0        0        0    30150 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/types.py
--rw-r--r--   0        0        0     5956 2023-04-05 07:06:31.888199 pysigma-0.9.6/sigma/validation.py
--rw-r--r--   0        0        0    10301 2023-04-05 07:06:31.892199 pysigma-0.9.6/sigma/validators/base.py
--rw-r--r--   0        0        0      773 2023-04-05 07:06:31.892199 pysigma-0.9.6/sigma/validators/core/__init__.py
--rw-r--r--   0        0        0     4099 2023-04-05 07:06:31.892199 pysigma-0.9.6/sigma/validators/core/condition.py
--rw-r--r--   0        0        0     2976 2023-04-05 07:06:31.892199 pysigma-0.9.6/sigma/validators/core/logsources.py
--rw-r--r--   0        0        0     1545 2023-04-05 07:06:31.892199 pysigma-0.9.6/sigma/validators/core/metadata.py
--rw-r--r--   0        0        0     2832 2023-04-05 07:06:31.892199 pysigma-0.9.6/sigma/validators/core/modifiers.py
--rw-r--r--   0        0        0     3280 2023-04-05 07:06:31.892199 pysigma-0.9.6/sigma/validators/core/tags.py
--rw-r--r--   0        0        0     5627 2023-04-05 07:06:31.892199 pysigma-0.9.6/sigma/validators/core/values.py
--rw-r--r--   0        0        0    11003 1970-01-01 00:00:00.000000 pysigma-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-04-29 23:38:12.062451 pysigma-0.9.7/LICENSE
+-rw-r--r--   0        0        0     9849 2023-04-29 23:38:12.062451 pysigma-0.9.7/README.md
+-rw-r--r--   0        0        0      992 2023-04-29 23:38:12.062451 pysigma-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0      238 2023-04-29 23:38:12.062451 pysigma-0.9.7/sigma/backends/test/__init__.py
+-rw-r--r--   0        0        0     5504 2023-04-29 23:38:12.062451 pysigma-0.9.7/sigma/backends/test/backend.py
+-rw-r--r--   0        0        0     8202 2023-04-29 23:38:12.062451 pysigma-0.9.7/sigma/collection.py
+-rw-r--r--   0        0        0     9805 2023-04-29 23:38:12.062451 pysigma-0.9.7/sigma/conditions.py
+-rw-r--r--   0        0        0        0 2023-04-29 23:38:12.062451 pysigma-0.9.7/sigma/conversion/__init__.py
+-rw-r--r--   0        0        0    52093 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/conversion/base.py
+-rw-r--r--   0        0        0     3401 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/conversion/deferred.py
+-rw-r--r--   0        0        0     1307 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/conversion/state.py
+-rw-r--r--   0        0        0    43469 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/data/mitre_attack.py
+-rw-r--r--   0        0        0     3735 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/exceptions.py
+-rw-r--r--   0        0        0    14729 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/modifiers.py
+-rw-r--r--   0        0        0     8799 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/pipelines/common.py
+-rw-r--r--   0        0        0      212 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/pipelines/test/__init__.py
+-rw-r--r--   0        0        0      874 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/pipelines/test/pipeline.py
+-rw-r--r--   0        0        0     8133 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/plugins.py
+-rw-r--r--   0        0        0        0 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/processing/__init__.py
+-rw-r--r--   0        0        0    12233 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/processing/conditions.py
+-rw-r--r--   0        0        0    16539 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/processing/pipeline.py
+-rw-r--r--   0        0        0     3680 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/processing/resolver.py
+-rw-r--r--   0        0        0     2763 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/processing/tracking.py
+-rw-r--r--   0        0        0    25461 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/processing/transformations.py
+-rw-r--r--   0        0        0    30901 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/rule.py
+-rw-r--r--   0        0        0    30355 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/types.py
+-rw-r--r--   0        0        0     5956 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/validation.py
+-rw-r--r--   0        0        0    10301 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/validators/base.py
+-rw-r--r--   0        0        0      773 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/validators/core/__init__.py
+-rw-r--r--   0        0        0     4099 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/validators/core/condition.py
+-rw-r--r--   0        0        0     2976 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/validators/core/logsources.py
+-rw-r--r--   0        0        0     1545 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/validators/core/metadata.py
+-rw-r--r--   0        0        0     2832 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/validators/core/modifiers.py
+-rw-r--r--   0        0        0     3280 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/validators/core/tags.py
+-rw-r--r--   0        0        0     5627 2023-04-29 23:38:12.066451 pysigma-0.9.7/sigma/validators/core/values.py
+-rw-r--r--   0        0        0    11003 1970-01-01 00:00:00.000000 pysigma-0.9.7/PKG-INFO
```

### Comparing `pysigma-0.9.6/LICENSE` & `pysigma-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/README.md` & `pysigma-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/pyproject.toml` & `pysigma-0.9.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma"
-version = "0.9.6"
+version = "0.9.7"
 license = "LGPL-2.1-only"
 description = "Sigma rule processing and conversion tools"
 authors = ["Thomas Patzke <thomas@patzke.org>"]
 readme = "README.md"
 repository = "https://github.com/SigmaHQ/pySigma"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `pysigma-0.9.6/sigma/backends/test/backend.py` & `pysigma-0.9.7/sigma/backends/test/backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,16 @@
     compare_operators : ClassVar[Dict[SigmaCompareExpression.CompareOperators, str]] = {
         SigmaCompareExpression.CompareOperators.LT  : "<",
         SigmaCompareExpression.CompareOperators.LTE : "<=",
         SigmaCompareExpression.CompareOperators.GT  : ">",
         SigmaCompareExpression.CompareOperators.GTE : ">=",
     }
 
+    field_equals_field_expression : ClassVar[str] = "{field1}=fieldref({field2})"
+
     field_null_expression : ClassVar[str] = "{field} is null"
 
     convert_or_as_in : ClassVar[bool] = True
     convert_and_as_in : ClassVar[bool] = True
     in_expressions_allow_wildcards : ClassVar[bool] = True
     field_in_list_expression : ClassVar[str] = "{field} {op} ({list})"
     or_in_operator : ClassVar[Optional[str]] = "in"
```

### Comparing `pysigma-0.9.6/sigma/collection.py` & `pysigma-0.9.7/sigma/collection.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/sigma/conditions.py` & `pysigma-0.9.7/sigma/conditions.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/sigma/conversion/base.py` & `pysigma-0.9.7/sigma/conversion/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from sigma.exceptions import SigmaError, SigmaValueError
 from sigma.conversion.deferred import DeferredQueryExpression
 from typing import Pattern, Union, ClassVar, Optional, Tuple, List, Dict, Any
 from sigma.processing.pipeline import ProcessingPipeline
 from sigma.collection import SigmaCollection
 from sigma.rule import SigmaRule
 from sigma.conditions import ConditionItem, ConditionOR, ConditionAND, ConditionNOT, ConditionFieldEqualsValueExpression, ConditionValueExpression, ConditionType
-from sigma.types import SigmaBool, SigmaExists, SigmaExpansion, SigmaRegularExpressionFlag, SigmaString, SigmaNumber, SigmaRegularExpression, SigmaCompareExpression, SigmaNull, SigmaQueryExpression, SigmaCIDRExpression, SpecialChars
+from sigma.types import SigmaBool, SigmaExists, SigmaExpansion, SigmaFieldReference, SigmaRegularExpressionFlag, SigmaString, SigmaNumber, SigmaRegularExpression, SigmaCompareExpression, SigmaNull, SigmaQueryExpression, SigmaCIDRExpression, SpecialChars
 from sigma.conversion.state import ConversionState
 
 class Backend(ABC):
     """
     Base class for Sigma conversion backends. A backend is made up from the following elements:
 
     * Some metadata about the properties of the backend.
@@ -228,14 +228,18 @@
         """Conversion of field matches CIDR expression value expressions"""
 
     @abstractmethod
     def convert_condition_field_compare_op_val(self, cond : ConditionFieldEqualsValueExpression, state : ConversionState) -> Any:
         """Conversion of field matches regular expression value expressions"""
 
     @abstractmethod
+    def convert_condition_field_eq_field(self, cond : SigmaFieldReference, state : ConversionState) -> Any:
+        """Conversion of field equals another field expressions."""
+
+    @abstractmethod
     def convert_condition_field_eq_val_null(self, cond : ConditionFieldEqualsValueExpression, state : ConversionState) -> Any:
         """Conversion of field is null expression value expressions"""
 
     @abstractmethod
     def convert_condition_field_exists(self, cond : ConditionFieldEqualsValueExpression, state : ConversionState) -> Any:
         """Conversion of field exists expressions"""
 
@@ -281,14 +285,16 @@
             return self.convert_condition_field_eq_val_bool(cond, state)
         elif isinstance(cond.value, SigmaRegularExpression):
             return self.convert_condition_field_eq_val_re(cond, state)
         elif isinstance(cond.value, SigmaCIDRExpression):
             return self.convert_condition_field_eq_val_cidr(cond, state)
         elif isinstance(cond.value, SigmaCompareExpression):
             return self.convert_condition_field_compare_op_val(cond, state)
+        elif isinstance(cond.value, SigmaFieldReference):
+            return self.convert_condition_field_eq_field(cond, state)
         elif isinstance(cond.value, SigmaNull):
             return self.convert_condition_field_eq_val_null(cond, state)
         elif isinstance(cond.value, SigmaQueryExpression):
             return self.convert_condition_field_eq_query_expr(cond, state)
         elif isinstance(cond.value, SigmaExists):
             return self.convert_condition_field_eq_val_exists(cond, state)
         elif isinstance(cond.value, SigmaExpansion):
@@ -464,14 +470,18 @@
     # CIDR values into string wildcard matches.
     cidr_expression : ClassVar[Optional[str]] = None    # CIDR expression query as format string with placeholders {field}, {value} (the whole CIDR value), {network} (network part only), {prefixlen} (length of network mask prefix) and {netmask} (CIDR network mask only)
 
     # Numeric comparison operators
     compare_op_expression : ClassVar[Optional[str]] = None      # Compare operation query as format string with placeholders {field}, {operator} and {value}
     compare_operators : ClassVar[Optional[Dict[SigmaCompareExpression.CompareOperators, str]]] = None       # Mapping between CompareOperators elements and strings used as replacement for {operator} in compare_op_expression
 
+    # Expression for comparing two event fields
+    field_equals_field_expression : ClassVar[Optional[str]] = None  # Field comparison expression with the placeholders {field1} and {field2} corresponding to left field and right value side of Sigma detection item
+    field_equals_field_escaping_quoting : Tuple[bool, bool] = (True, True)   # If regular field-escaping/quoting is applied to field1 and field2. A custom escaping/quoting can be implemented in the convert_condition_field_eq_field_escape_and_quote method.
+
     # Null/None expressions
     field_null_expression : ClassVar[Optional[str]] = None          # Expression for field has null value as format string with {field} placeholder for field name
 
     # Field existence condition expressions.
     field_exists_expression : ClassVar[Optional[str]] = None        # Expression for field existence as format string with {field} placeholder for field name
     field_not_exists_expression : ClassVar[Optional[str]] = None    # Expression for field non-existence as format string with {field} placeholder for field name. If not set, field_exists_expression is negated with boolean NOT.
 
@@ -787,14 +797,33 @@
         """Conversion of numeric comparison operations into queries."""
         return self.compare_op_expression.format(
             field=self.escape_and_quote_field(cond.field),
             operator=self.compare_operators[cond.value.op],
             value=cond.value.number,
         )
 
+    def convert_condition_field_eq_field_escape_and_quote(self, field1 : str, field2 : str) -> Tuple[str, str]:
+        """Escape and quote field names of a field-quals-field expression."""
+        return (
+            self.escape_and_quote_field(field1)
+            if self.field_equals_field_escaping_quoting[0] else
+            field1,
+            self.escape_and_quote_field(field2)
+            if self.field_equals_field_escaping_quoting[1] else
+            field2
+        )
+
+    def convert_condition_field_eq_field(self, cond : SigmaFieldReference, state : ConversionState) -> Union[str, DeferredQueryExpression]:
+        """Conversion of comparision of two fields."""
+        field1, field2 = self.convert_condition_field_eq_field_escape_and_quote(cond.field, cond.value.field)
+        return self.field_equals_field_expression.format(
+            field1=field1,
+            field2=field2,
+        )
+
     def convert_condition_field_eq_val_null(self, cond : ConditionFieldEqualsValueExpression, state : ConversionState) -> Union[str, DeferredQueryExpression]:
         """Conversion of field is null expression value expressions"""
         return self.field_null_expression.format(field=self.escape_and_quote_field(cond.field))
 
     def convert_condition_field_exists(self, cond : ConditionFieldEqualsValueExpression, state : ConversionState) -> Union[str, DeferredQueryExpression]:
         """Conversion of field exists expressions"""
         return self.field_exists_expression.format(field=self.escape_and_quote_field(cond.field))
```

### Comparing `pysigma-0.9.6/sigma/conversion/deferred.py` & `pysigma-0.9.7/sigma/conversion/deferred.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/sigma/conversion/state.py` & `pysigma-0.9.7/sigma/conversion/state.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/sigma/data/mitre_attack.py` & `pysigma-0.9.7/sigma/data/mitre_attack.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/sigma/exceptions.py` & `pysigma-0.9.7/sigma/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/sigma/modifiers.py` & `pysigma-0.9.7/sigma/modifiers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC, abstractmethod
 import re
 from typing import ClassVar, Optional, Union, List, Sequence, Dict, Type, get_origin, get_args, get_type_hints
 from collections.abc import Sequence as SequenceABC
 from base64 import b64encode
-from sigma.types import Placeholder, SigmaBool, SigmaExists, SigmaExpansion, SigmaRegularExpressionFlag, SigmaType, SigmaString, SigmaNumber, SpecialChars, SigmaRegularExpression, SigmaCompareExpression, SigmaCIDRExpression
+from sigma.types import Placeholder, SigmaBool, SigmaExists, SigmaExpansion, SigmaFieldReference, SigmaRegularExpressionFlag, SigmaType, SigmaString, SigmaNumber, SpecialChars, SigmaRegularExpression, SigmaCompareExpression, SigmaCIDRExpression
 from sigma.conditions import ConditionAND
 from sigma.exceptions import SigmaRuleLocation, SigmaTypeError, SigmaValueError
 import sigma
 
 ### Base Classes ###
 class SigmaModifier(ABC):
     """Base class for all Sigma modifiers"""
@@ -177,66 +177,83 @@
                 yield p
         return SigmaExpansion(
             val.replace_with_placeholder(re.compile("\\B[-/]\\b"), "_windash") \
                 .replace_placeholders(callback)
         )
 
 class SigmaRegularExpressionModifier(SigmaValueModifier):
+    """Treats string value as (case-sensitive) regular expression."""
     def modify(self, val : SigmaString) -> SigmaRegularExpression:
         if len(self.applied_modifiers) > 0:
             raise SigmaValueError("Regular expression modifier only applicable to unmodified values", source=self.source)
         return SigmaRegularExpression(val.original)
 
 class SigmaRegularExpressionFlagModifier(SigmaValueModifier):
     """Generic base class for setting a regular expression flag including checks"""
     flag : ClassVar[SigmaRegularExpressionFlag]
 
     def modify(self, val: SigmaRegularExpression) -> SigmaRegularExpression:
         val.add_flag(self.flag)
         return val
 
 class SigmaRegularExpressionIgnoreCaseFlagModifier(SigmaRegularExpressionFlagModifier):
+    """Match regular expression case-insensitive."""
     flag : ClassVar[SigmaRegularExpressionFlag] = SigmaRegularExpressionFlag.IGNORECASE
 
 class SigmaRegularExpressionMultilineFlagModifier(SigmaRegularExpressionFlagModifier):
+    """Match regular expression across multiple lines."""
     flag : ClassVar[SigmaRegularExpressionFlag] = SigmaRegularExpressionFlag.MULTILINE
 
 class SigmaRegularExpressionDotAllFlagModifier(SigmaRegularExpressionFlagModifier):
+    """Regular expression dot matches all characters."""
     flag : ClassVar[SigmaRegularExpressionFlag] = SigmaRegularExpressionFlag.DOTALL
 
 class SigmaCIDRModifier(SigmaValueModifier):
+    """Treat value as IP (v4 or v6) CIDR network."""
     def modify(self, val : SigmaString) -> SigmaCIDRExpression:
         if len(self.applied_modifiers) > 0:
             raise SigmaValueError("CIDR expression modifier only applicable to unmodified values", source=self.source)
         return SigmaCIDRExpression(str(val), source=self.source)
 
 class SigmaAllModifier(SigmaListModifier):
+    """Match all values of a list instead of any pf them."""
     def modify(self, val : Sequence[SigmaType]) -> List[SigmaType]:
         self.detection_item.value_linking = ConditionAND
         return val
 
 class SigmaCompareModifier(SigmaValueModifier):
     """Base class for numeric comparison operator modifiers."""
     op : ClassVar[SigmaCompareExpression.CompareOperators]
 
     def modify(self, val : SigmaNumber) -> SigmaCompareExpression:
         return SigmaCompareExpression(val, self.op, self.source)
 
 class SigmaLessThanModifier(SigmaCompareModifier):
+    """Numeric less than (<) matching."""
     op : ClassVar[SigmaCompareExpression.CompareOperators] = SigmaCompareExpression.CompareOperators.LT
 
 class SigmaLessThanEqualModifier(SigmaCompareModifier):
+    """Numeric less than or equal (<=) matching."""
     op : ClassVar[SigmaCompareExpression.CompareOperators] = SigmaCompareExpression.CompareOperators.LTE
 
 class SigmaGreaterThanModifier(SigmaCompareModifier):
+    """Numeric greater than (>) matching."""
     op : ClassVar[SigmaCompareExpression.CompareOperators] = SigmaCompareExpression.CompareOperators.GT
 
 class SigmaGreaterThanEqualModifier(SigmaCompareModifier):
+    """Numeric greater than or equal (>=) matching."""
     op : ClassVar[SigmaCompareExpression.CompareOperators] = SigmaCompareExpression.CompareOperators.GTE
 
+class SigmaFieldReferenceModifier(SigmaValueModifier):
+    """Modifiers a plain string into the field reference type."""
+    def modify(self, val : SigmaString) -> SigmaFieldReference:
+        if val.contains_special():
+            raise SigmaValueError("Field references must not contain wildcards", source=self.source)
+        return SigmaFieldReference(val.to_plain())
+
 class SigmaExistsModifier(SigmaValueModifier):
     """Modifies to check if the field name provided as value exists in the matched event."""
     def modify(self, val : SigmaBool) -> SigmaExists:
         if self.detection_item.field is None:
             raise SigmaValueError("Exists modifier must be applied to field", source=self.source)
         if len(self.applied_modifiers) > 0:
             raise SigmaValueError("Exists modifier only applicable to unmodified boolean values", source=self.source)
@@ -270,14 +287,15 @@
     "dotall"        : SigmaRegularExpressionDotAllFlagModifier,
     "cidr"          : SigmaCIDRModifier,
     "all"           : SigmaAllModifier,
     "lt"            : SigmaLessThanModifier,
     "lte"           : SigmaLessThanEqualModifier,
     "gt"            : SigmaGreaterThanModifier,
     "gte"           : SigmaGreaterThanEqualModifier,
+    "fieldref"      : SigmaFieldReferenceModifier,
     "expand"        : SigmaExpandModifier,
 }
 
 # Mapping from modifier class to identifier
 reverse_modifier_mapping : Dict[str, str] = {
     modifier_class.__name__: identifier
     for identifier, modifier_class in modifier_mapping.items()
```

### Comparing `pysigma-0.9.6/sigma/pipelines/common.py` & `pysigma-0.9.7/sigma/pipelines/common.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/sigma/pipelines/test/pipeline.py` & `pysigma-0.9.7/sigma/pipelines/test/pipeline.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/sigma/plugins.py` & `pysigma-0.9.7/sigma/plugins.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/sigma/processing/conditions.py` & `pysigma-0.9.7/sigma/processing/conditions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 
 import sigma
-from sigma.types import SigmaString, SigmaType, sigma_type
+from sigma.types import SigmaFieldReference, SigmaString, SigmaType, sigma_type
 from typing import Dict, List, Pattern, Literal, Optional, Union
 import re
 from sigma.rule import SigmaDetection, SigmaRule, SigmaDetectionItem, SigmaLogSource
 from sigma.exceptions import SigmaConfigurationError, SigmaRegularExpressionError
 
 ### Base Classes ###
 
@@ -24,21 +24,51 @@
     Base class for conditions on field names in detection items, Sigma rule field lists and other
     use cases that require matching on field names without detection item context.
     """
     @abstractmethod
     def match_field_name(self, pipeline: "sigma.processing.pipeline.ProcessingPipeline", field : str) -> bool:
         "The method match is called for each field name and must return a bool result."
 
-    def match_detection_item(self, pipeline: "sigma.processing.pipeline.ProcessingPipeline", detection_item : SigmaDetectionItem):
+    def match_detection_item(self, pipeline: "sigma.processing.pipeline.ProcessingPipeline", detection_item : SigmaDetectionItem) -> bool:
         """
-        Match field name condition on detection item by default by match on the field name
-        contained in the detection item.
+        Field names can be contained in the detection item field as well as in field references in
+        detection item values. The detection item matching returns True for both cases, but in
+        subsequent processing it has to be verified which part of the detection item has matched and
+        should be subject of processing actions (e.g. field name mapping). This can be done with the
+        methods
+
+        * `match_detection_item_field` for the field of a detection item
+        * `match_detection_item_value` for the whole value list of a detection item and
+        * `match_value` for single detection items values.
         """
+        return self.match_detection_item_field(pipeline, detection_item) or self.match_detection_item_value(pipeline, detection_item)
+
+    def match_detection_item_field(self, pipeline: "sigma.processing.pipeline.ProcessingPipeline", detection_item : SigmaDetectionItem) -> bool:
+        """Returns True if the field of the detection item matches the implemented field name condition."""
         return self.match_field_name(pipeline, detection_item.field)
 
+    def match_detection_item_value(self, pipeline: "sigma.processing.pipeline.ProcessingPipeline", detection_item : SigmaDetectionItem) -> bool:
+        """Returns True if any value of a detection item contains a field reference to a field name
+        matching the implemented field name condition. Processing actions must only be applied to
+        matching individual values determined by `match_value`."""
+        return any((
+            self.match_value(pipeline, value)
+            for value in detection_item.value
+        ))
+
+    def match_value(self, pipeline: "sigma.processing.pipeline.ProcessingPipeline", value : SigmaType) -> bool:
+        """
+        Checks if a detection item value matches the field name condition implemented in
+        `match_field_name` if it is a field reference. For all other types the method returns False.
+        """
+        if isinstance(value, SigmaFieldReference):
+            return self.match_field_name(pipeline, value.field)
+        else:
+            return False
+
 @dataclass
 class DetectionItemProcessingCondition(ABC):
     """
     Base for Sigma detection item processing condition classes used in processing pipelines.
     """
     @abstractmethod
     def match(self, pipeline : "sigma.processing.pipeline.ProcessingPipeline", detection_item : SigmaDetectionItem) -> bool:
```

### Comparing `pysigma-0.9.6/sigma/processing/pipeline.py` & `pysigma-0.9.7/sigma/processing/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from sigma.processing.tracking import FieldMappingTracking
 from sigma.rule import SigmaDetectionItem, SigmaRule
 from sigma.processing.transformations import transformations, Transformation
 from sigma.processing.conditions import rule_conditions, RuleProcessingCondition, detection_item_conditions, DetectionItemProcessingCondition, field_name_conditions, FieldNameProcessingCondition
 from sigma.exceptions import SigmaConfigurationError, SigmaTypeError
 import yaml
 
+from sigma.types import SigmaFieldReference, SigmaType
+
 @dataclass
 class ProcessingItem:
     """
     A processing item consists of an optional condition and a transformation that is applied in the case that
     the condition evaluates to true against the given Sigma rule or if the condition is not present.
 
     Processing items are instantiated by the processing pipeline for a whole collection that is about to be
@@ -176,14 +178,30 @@
             for condition in self.field_name_conditions
         ])
         if self.field_name_condition_negation:
             field_name_cond_result = not field_name_cond_result
 
         return field_name_cond_result
 
+    def match_field_in_value(self, pipeline : "ProcessingPipeline", value : SigmaType) -> bool:
+        """
+        Evaluate field name conditions in field reference values and return result.
+        """
+        if isinstance(value, SigmaFieldReference):
+            field_name_cond_result = self.field_name_condition_linking([
+                condition.match_value(pipeline, value)
+                for condition in self.field_name_conditions
+            ])
+            if self.field_name_condition_negation:
+                field_name_cond_result = not field_name_cond_result
+
+            return field_name_cond_result
+        else:
+            return False
+
 @dataclass
 class ProcessingPipeline:
     """
     A processing pipeline is configured with the transformation steps that are applied on Sigma rules and
     are configured by:
 
     * a backend to apply a set of base preprocessing of Sigma rules (e.g. renaming of fields).
```

### Comparing `pysigma-0.9.6/sigma/processing/resolver.py` & `pysigma-0.9.7/sigma/processing/resolver.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/sigma/processing/tracking.py` & `pysigma-0.9.7/sigma/processing/tracking.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/sigma/processing/transformations.py` & `pysigma-0.9.7/sigma/processing/transformations.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import dataclasses
 import random
 import string
 import re
 import sigma
 from sigma.rule import SigmaLogSource, SigmaRule, SigmaDetection, SigmaDetectionItem
 from sigma.exceptions import SigmaRegularExpressionError, SigmaTransformationError, SigmaValueError, SigmaConfigurationError
-from sigma.types import Placeholder, SigmaString, SigmaType, SpecialChars, SigmaQueryExpression
+from sigma.types import Placeholder, SigmaString, SigmaType, SpecialChars, SigmaQueryExpression, SigmaFieldReference
 
 ### Base Classes ###
 @dataclass
 class Transformation(ABC):
     """
     Base class for processing steps used in pipelines. Override `apply` with transformation that is
     applied to the whole rule.
@@ -101,22 +101,42 @@
             if self.processing_item is not None:
                 pipeline.track_field_processing_items(field, result, self.processing_item.identifier)
             return result
         else:
             return [ field ]
 
     def apply(self, pipeline: "sigma.processing.pipeline.ProcessingPipeline", rule: SigmaRule) -> None:
+        """Apply field name transformations to Sigma rule field names listed in 'fields' attribute."""
         _apply_field_name = partial(self._apply_field_name, pipeline)
         rule.fields = [
             item
             for mapping in map(_apply_field_name, rule.fields)
             for item in mapping
         ]
         return super().apply(pipeline, rule)
 
+    def apply_detection_item(self, detection_item: SigmaDetectionItem) -> Optional[Union[SigmaDetection, SigmaDetectionItem]]:
+        """Apply field name transformations to field references in detection item values."""
+        new_values = []
+        match = False
+        for value in detection_item.value:
+            if self.processing_item is not None and self.processing_item.match_field_in_value(self.pipeline, value):
+                new_values.extend((
+                    SigmaFieldReference(mapped_field)
+                    for mapped_field in self._apply_field_name(self.pipeline, value.field)
+                ))
+                match = True
+            else:
+                new_values.append(value)
+
+        if match:       # replace value only if something matched
+            detection_item.value = new_values
+
+        return super().apply_detection_item(detection_item)
+
 @dataclass
 class ValueTransformation(DetectionItemTransformation):
     """
     Iterates over all values in all detection items of a Sigma rule and call apply_value method
     for each of them. The apply_value method can return a single value or a list of values which
     are inserted into the value list or None if the original value should be passed through. An
     empty list should be returned by apply_value to drop the value from the transformed results.
@@ -194,17 +214,18 @@
 
     def get_mapping(self, field: str) -> Union[None, str, List[str]]:
         if field in self.mapping:
             mapping = self.mapping[field]
             return mapping
 
     def apply_detection_item(self, detection_item : SigmaDetectionItem):
+        super().apply_detection_item(detection_item)
         field = detection_item.field
         mapping = self.get_mapping(field)
-        if mapping is not None:
+        if mapping is not None and self.processing_item.match_field_name(self.pipeline, field):
             self.pipeline.field_mappings.add_mapping(field, mapping)
             if isinstance(mapping, str):    # 1:1 mapping, map field name of detection item directly
                 detection_item.field = mapping
                 self.processing_item_applied(detection_item)
             else:
                 return SigmaDetection([
                     dataclasses.replace(detection_item, field=field, auto_modifiers=False)
@@ -217,15 +238,14 @@
             return [mapping]
         else:
             return mapping
 
 @dataclass
 class FieldPrefixMappingTransformation(FieldMappingTransformation):
     """Map a field name prefix to one or multiple different prefixes."""
-
     def get_mapping(self, field: str) -> Union[None, str, List[str]]:
         for src, dest in self.mapping.items():
             if field.startswith(src):      # found matching prefix
                 if isinstance(dest, str):
                     return dest + field[len(src):]
                 else:
                     return [
@@ -259,15 +279,16 @@
 class AddFieldnameSuffixTransformation(FieldMappingTransformationBase):
     """
     Add field name suffix.
     """
     suffix : str
 
     def apply_detection_item(self, detection_item : SigmaDetectionItem):
-        if type(orig_field := detection_item.field) is str:
+        super().apply_detection_item(detection_item)
+        if type(orig_field := detection_item.field) is str and (self.processing_item is None or self.processing_item.match_field_name(self.pipeline, orig_field)):
             detection_item.field += self.suffix
             self.pipeline.field_mappings.add_mapping(orig_field, detection_item.field)
         self.processing_item_applied(detection_item)
 
     def apply_field_name(self, field: str) -> List[str]:
         return [ field + self.suffix ]
 
@@ -275,15 +296,16 @@
 class AddFieldnamePrefixTransformation(FieldMappingTransformationBase):
     """
     Add field name prefix.
     """
     prefix : str
 
     def apply_detection_item(self, detection_item : SigmaDetectionItem):
-        if type(orig_field := detection_item.field) is str:
+        super().apply_detection_item(detection_item)
+        if type(orig_field := detection_item.field) is str and (self.processing_item is None or self.processing_item.match_field_name(self.pipeline, orig_field)):
             detection_item.field = self.prefix + detection_item.field
             self.pipeline.field_mappings.add_mapping(orig_field, detection_item.field)
         self.processing_item_applied(detection_item)
 
     def apply_field_name(self, field: str) -> List[str]:
         return [ self.prefix + field ]
```

### Comparing `pysigma-0.9.6/sigma/rule.py` & `pysigma-0.9.7/sigma/rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import InitVar, dataclass, field
 import dataclasses
 from typing import Any, Dict, Optional, Union, Sequence, List, Mapping, Type
 from uuid import UUID
 from enum import Enum, auto
-from datetime import date
+from datetime import date, datetime
 import yaml
 import sigma
 from sigma.types import SigmaType, SigmaNull, SigmaString, SigmaNumber, sigma_type
 from sigma.modifiers import SigmaModifier, modifier_mapping, reverse_modifier_mapping, SigmaValueModifier, SigmaListModifier
 from sigma.conditions import SigmaCondition, ConditionAND, ConditionOR, ConditionFieldEqualsValueExpression, ConditionValueExpression, ParentChainMixin
 from sigma.processing.tracking import ProcessingItemTrackingMixin
 import sigma.exceptions as sigma_exceptions
@@ -589,21 +589,22 @@
                 status = SigmaStatus[status.upper()]
             except KeyError:
                 errors.append(sigma_exceptions.SigmaStatusError(f"'{ status }' is no valid Sigma rule status", source=source))
 
         # parse rule date if existing
         rule_date = rule.get("date")
         if rule_date is not None:
-            try:
-                rule_date = date(*(int(i) for i in rule_date.split("/")))
-            except ValueError:
+            if not isinstance(rule_date, date) and not isinstance(rule_date, datetime):
                 try:
-                    rule_date = date(*(int(i) for i in rule_date.split("-")))
+                    rule_date = date(*(int(i) for i in rule_date.split("/")))
                 except ValueError:
-                    errors.append(sigma_exceptions.SigmaDateError(f"Rule date '{ rule_date }' is invalid, must be yyyy/mm/dd or yyyy-mm-dd", source=source))
+                    try:
+                        rule_date = date(*(int(i) for i in rule_date.split("-")))
+                    except ValueError:
+                        errors.append(sigma_exceptions.SigmaDateError(f"Rule date '{ rule_date }' is invalid, must be yyyy/mm/dd or yyyy-mm-dd", source=source))
 
         # parse log source
         logsource = None
         try:
             logsource = SigmaLogSource.from_dict(rule["logsource"], source)
         except KeyError:
             errors.append(sigma_exceptions.SigmaLogsourceError("Sigma rule must have a log source", source=source))
```

### Comparing `pysigma-0.9.6/sigma/types.py` & `pysigma-0.9.7/sigma/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -615,14 +615,15 @@
                     patterns.append(str(subnet)[:i] + "*")  # Generate pattern by cutting of at first difference
                 else:                                       # The /128 case - no differences
                     patterns.append(str(subnet))            # Return the single address
         return patterns
 
 @dataclass
 class SigmaCompareExpression(NoPlainConversionMixin, SigmaType):
+    """Type for numeric comparison."""
     class CompareOperators(Enum):
         LT  = auto()    # <
         LTE = auto()    # <=
         GT  = auto()    # >
         GTE = auto()    # >=
 
     number : SigmaNumber
@@ -630,14 +631,19 @@
     source : Optional[SigmaRuleLocation] = None
 
     def __post_init__(self):
         if not isinstance(self.number, SigmaNumber):
             raise SigmaTypeError("Compare operator expects number", source=self.source)
 
 @dataclass
+class SigmaFieldReference(NoPlainConversionMixin, SigmaType):
+    """Type for referencing to other fields for comparison between them."""
+    field : str
+
+@dataclass
 class SigmaQueryExpression(NoPlainConversionMixin, SigmaType):
     """
     Special purpose type for passing a query part (e.g. list lookups in placeholders) directly into the generated
     query. The query string may contain a {field} placeholder, which is replaced with the field name contained in
     the detection item containing the query expression. This is done by the finalize method.
 
     Because this is very specific to the target language, it has to be used in late stages of the conversion
```

### Comparing `pysigma-0.9.6/sigma/validation.py` & `pysigma-0.9.7/sigma/validation.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/sigma/validators/base.py` & `pysigma-0.9.7/sigma/validators/base.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/sigma/validators/core/__init__.py` & `pysigma-0.9.7/sigma/validators/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/sigma/validators/core/condition.py` & `pysigma-0.9.7/sigma/validators/core/condition.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/sigma/validators/core/logsources.py` & `pysigma-0.9.7/sigma/validators/core/logsources.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/sigma/validators/core/metadata.py` & `pysigma-0.9.7/sigma/validators/core/metadata.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/sigma/validators/core/modifiers.py` & `pysigma-0.9.7/sigma/validators/core/modifiers.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/sigma/validators/core/tags.py` & `pysigma-0.9.7/sigma/validators/core/tags.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/sigma/validators/core/values.py` & `pysigma-0.9.7/sigma/validators/core/values.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.6/PKG-INFO` & `pysigma-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysigma
-Version: 0.9.6
+Version: 0.9.7
 Summary: Sigma rule processing and conversion tools
 Home-page: https://github.com/SigmaHQ/pySigma
 License: LGPL-2.1-only
 Author: Thomas Patzke
 Author-email: thomas@patzke.org
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

