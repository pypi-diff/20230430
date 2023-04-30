# Comparing `tmp/vyxal-2.9.0.tar.gz` & `tmp/vyxal-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vyxal-2.9.0.tar", max compression
+gzip compressed data, was "vyxal-2.9.1.tar", max compression
```

## Comparing `vyxal-2.9.0.tar` & `vyxal-2.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1075 2022-03-13 11:46:13.723936 vyxal-2.9.0/LICENSE
--rw-r--r--   0        0        0     3201 2022-03-13 11:46:13.723936 vyxal-2.9.0/README.md
--rw-r--r--   0        0        0      696 2022-03-13 11:46:13.735936 vyxal-2.9.0/pyproject.toml
--rw-r--r--   0        0        0     7966 2022-03-13 11:46:13.735936 vyxal-2.9.0/vyxal/LazyList.py
--rw-r--r--   0        0        0        0 2022-03-13 11:46:13.735936 vyxal-2.9.0/vyxal/__init__.py
--rw-r--r--   0        0        0       34 2022-03-13 11:46:13.735936 vyxal-2.9.0/vyxal/__main__.py
--rw-r--r--   0        0        0     2061 2022-03-13 11:46:13.735936 vyxal-2.9.0/vyxal/context.py
--rw-r--r--   0        0        0   166247 2022-03-13 11:46:13.739935 vyxal-2.9.0/vyxal/dictionary.py
--rw-r--r--   0        0        0   160894 2022-03-13 11:46:13.739935 vyxal-2.9.0/vyxal/elements.py
--rw-r--r--   0        0        0     1613 2022-03-13 11:46:13.739935 vyxal-2.9.0/vyxal/encoding.py
--rw-r--r--   0        0        0    27626 2022-03-13 11:46:13.739935 vyxal-2.9.0/vyxal/helpers.py
--rw-r--r--   0        0        0     6465 2022-03-13 11:46:13.739935 vyxal-2.9.0/vyxal/lexer.py
--rw-r--r--   0        0        0     9650 2022-03-13 11:46:13.739935 vyxal-2.9.0/vyxal/main.py
--rw-r--r--   0        0        0    12458 2022-03-13 11:46:13.739935 vyxal-2.9.0/vyxal/parse.py
--rw-r--r--   0        0        0     4235 2022-03-13 11:46:13.739935 vyxal-2.9.0/vyxal/structure.py
--rw-r--r--   0        0        0    19291 2022-03-13 11:46:13.739935 vyxal-2.9.0/vyxal/transpile.py
--rw-r--r--   0        0        0     4043 2022-03-13 11:46:42.986045 vyxal-2.9.0/setup.py
--rw-r--r--   0        0        0     3796 2022-03-13 11:46:42.986478 vyxal-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2022-03-20 10:56:06.272637 vyxal-2.9.1/LICENSE
+-rw-r--r--   0        0        0     3201 2022-03-20 10:56:06.272637 vyxal-2.9.1/README.md
+-rw-r--r--   0        0        0      696 2022-03-20 10:56:06.284637 vyxal-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0     7966 2022-03-20 10:56:06.288637 vyxal-2.9.1/vyxal/LazyList.py
+-rw-r--r--   0        0        0        0 2022-03-20 10:56:06.288637 vyxal-2.9.1/vyxal/__init__.py
+-rw-r--r--   0        0        0       34 2022-03-20 10:56:06.288637 vyxal-2.9.1/vyxal/__main__.py
+-rw-r--r--   0        0        0     2061 2022-03-20 10:56:06.288637 vyxal-2.9.1/vyxal/context.py
+-rw-r--r--   0        0        0   166247 2022-03-20 10:56:06.288637 vyxal-2.9.1/vyxal/dictionary.py
+-rw-r--r--   0        0        0   162535 2022-03-20 10:56:06.288637 vyxal-2.9.1/vyxal/elements.py
+-rw-r--r--   0        0        0     1613 2022-03-20 10:56:06.288637 vyxal-2.9.1/vyxal/encoding.py
+-rw-r--r--   0        0        0    27565 2022-03-20 10:56:06.288637 vyxal-2.9.1/vyxal/helpers.py
+-rw-r--r--   0        0        0     6465 2022-03-20 10:56:06.292637 vyxal-2.9.1/vyxal/lexer.py
+-rw-r--r--   0        0        0     9650 2022-03-20 10:56:06.292637 vyxal-2.9.1/vyxal/main.py
+-rw-r--r--   0        0        0    12634 2022-03-20 10:56:06.292637 vyxal-2.9.1/vyxal/parse.py
+-rw-r--r--   0        0        0     4235 2022-03-20 10:56:06.292637 vyxal-2.9.1/vyxal/structure.py
+-rw-r--r--   0        0        0    19363 2022-03-20 10:56:06.292637 vyxal-2.9.1/vyxal/transpile.py
+-rw-r--r--   0        0        0     4043 2022-03-20 10:56:37.584638 vyxal-2.9.1/setup.py
+-rw-r--r--   0        0        0     3796 2022-03-20 10:56:37.585157 vyxal-2.9.1/PKG-INFO
```

### Comparing `vyxal-2.9.0/LICENSE` & `vyxal-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vyxal-2.9.0/README.md` & `vyxal-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `vyxal-2.9.0/pyproject.toml` & `vyxal-2.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vyxal"
-version = "2.9.0"
+version = "2.9.1"
 description = "A golfing language that has aspects of traditional programming languages."
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Vyxal/Vyxal/"
 homepage = "https://vyxal.pythonanywhere.com/"
```

### Comparing `vyxal-2.9.0/vyxal/LazyList.py` & `vyxal-2.9.1/vyxal/LazyList.py`

 * *Files identical despite different names*

### Comparing `vyxal-2.9.0/vyxal/context.py` & `vyxal-2.9.1/vyxal/context.py`

 * *Files identical despite different names*

### Comparing `vyxal-2.9.0/vyxal/dictionary.py` & `vyxal-2.9.1/vyxal/dictionary.py`

 * *Files identical despite different names*

### Comparing `vyxal-2.9.0/vyxal/elements.py` & `vyxal-2.9.1/vyxal/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -792,32 +792,32 @@
     """Element ø↲
     (any, num, str) -> pad a on the left with c to length b
     (any, str, num) -> pad a on the left with b to length c
     (lst, any, any) -> vectorised
     """
     if isinstance(lhs, LazyList):
         return vectorise(custom_pad_left, lhs, rhs, other)
-    if isinstance(rhs, int):
-        return lhs.ljust(rhs, other)
-    if isinstance(other, int):
-        return lhs.ljust(other, rhs)
+    if vy_type(rhs) == NUMBER_TYPE:
+        return lhs.ljust(int(rhs), other)
+    if vy_type(other) == NUMBER_TYPE:
+        return lhs.ljust(int(other), rhs)
 
 
 def custom_pad_right(lhs, rhs, other, ctx):
     """Element ø↳
     (any, num, str) -> pad a on the right with c to length b
     (any, str, num) -> pad a on the right with b to length c
     (lst, any, any) -> vectorised
     """
     if isinstance(lhs, LazyList):
         return vectorise(custom_pad_left, lhs, rhs, other)
-    if isinstance(rhs, int):
-        return lhs.rjust(rhs, other)
-    if isinstance(other, int):
-        return lhs.rjust(other, rhs)
+    if vy_type(rhs) == NUMBER_TYPE:
+        return lhs.rjust(int(rhs), other)
+    if vy_type(other) == NUMBER_TYPE:
+        return lhs.rjust(int(other), rhs)
 
 
 def decrement(lhs, ctx):
     """Element ‹
     (num) -> a - 1
     (str) -> a + "-"
     """
@@ -1137,15 +1137,17 @@
     ts = vy_type(lhs, rhs)
     return {
         (NUMBER_TYPE, NUMBER_TYPE): lambda: lhs**rhs,
         (NUMBER_TYPE, str): lambda: rhs
         + ((rhs[0] or " ") * (int(lhs) - len(rhs))),
         (str, NUMBER_TYPE): lambda: lhs
         + ((lhs[0] or " ") * (int(rhs) - len(lhs))),
-        (str, str): lambda: list(re.search(lhs, rhs).span()),
+        (str, str): lambda: []
+        if (mobj := re.search(rhs, lhs)) is None
+        else list(mobj.span()),
         (ts[0], types.FunctionType): lambda: list(vy_map(rhs, lhs, ctx)),
         (types.FunctionType, ts[1]): lambda: list(vy_map(lhs, rhs, ctx)),
     }.get(ts, lambda: vectorise(exponent, lhs, rhs, ctx=ctx))()
 
 
 def factorial(lhs, ctx):
     """Element ¡
@@ -1313,14 +1315,19 @@
     return "\n".join(result)
 
 
 def flip_brackets_vertical_palindromise(lhs, ctx):
     """Element øM
     (str) -> lhs vertically palindromised without duplicating the center, with brackets flipped.
     """
+    ts = vy_type(lhs)
+    if ts == NUMBER_TYPE:
+        return lhs
+    elif ts in (list, LazyList):
+        return vectorise(flip_brackets_vertical_palindromise, lhs, ctx=ctx)
     result = lhs.split("\n")
     for i in range(len(result)):
         result[i] += invert_brackets(result[i][:-1][::-1])
     return "\n".join(result)
 
 
 def foldl_columns(lhs, rhs, ctx):
@@ -1706,17 +1713,28 @@
                     break
 
                 prevs.append(curr)
 
         return gen()
 
     else:
-        lhs = iterable(lhs)
+        if primitive_type(rhs) is SCALAR_TYPE:
+            lhs, rhs = rhs, lhs
+        lhs = LazyList(iterable(lhs))
         rhs = iterable(rhs)
-        return vy_map(lambda item: lhs[item], rhs, ctx=ctx)
+
+        # Don't ask me why vectorise doesn't work here
+        # I tried.
+        def recursive_helper(value):
+            if primitive_type(value) is SCALAR_TYPE:
+                return lhs[value]
+            else:
+                return [recursive_helper(v) for v in value]
+
+        return recursive_helper(rhs)
 
 
 def infinite_cardinals(_, ctx=None):
     """Element Þc
     infinite sequence of cardinals
     """
     return LazyList(map(num2words.num2words, itertools.count(1)), isinf=True)
@@ -2172,15 +2190,15 @@
                        modifying_function=b, inital=c)
                        # Collect the results of apply a on c while b(c)
                        # is truthy
     """
     ts = vy_type(lhs, rhs, other)
     return {
         (NUMBER_TYPE, NUMBER_TYPE, NUMBER_TYPE): lambda: int(
-            lhs <= other <= rhs
+            simplify(lhs) <= simplify(other) <= simplify(rhs)
         ),
         (NUMBER_TYPE, NUMBER_TYPE, str): lambda: "\n".join([other * lhs] * rhs),
         (NUMBER_TYPE, str, NUMBER_TYPE): lambda: "\n".join([rhs * lhs] * other),
         (NUMBER_TYPE, str, str): lambda: vy_str(rhs, ctx=ctx).ljust(lhs, other),
         (str, NUMBER_TYPE, NUMBER_TYPE): lambda: "\n".join([lhs * other] * rhs),
         (str, NUMBER_TYPE, str): lambda: vy_str(lhs, ctx=ctx).ljust(rhs, other),
         (str, str, NUMBER_TYPE): lambda: vy_str(lhs, ctx=ctx).ljust(rhs, other),
@@ -2780,15 +2798,15 @@
     return {
         (ts[0], NUMBER_TYPE): lambda: index(
             iterable(lhs, ctx=ctx), [1, rhs], ctx
         ),
         (NUMBER_TYPE, ts[1]): lambda: index(
             iterable(rhs, ctx=ctx), [1, lhs], ctx
         ),
-        (str, str): lambda: vyxalify(re.match(lhs, rhs).groups()),
+        (str, str): lambda: vyxalify(re.match(rhs, lhs).groups()),
     }.get(ts, lambda: vectorise(one_slice, lhs, rhs, ctx=ctx))()
 
 
 def optimal_compress(lhs, ctx):
     """Element øD
     (str) -> return the most optimal dictionary compressed string
     """
@@ -2827,15 +2845,15 @@
         else lhs,
         (ts[0], types.FunctionType): lambda: scanl(
             multiply(rhs, 2, ctx), iterable(lhs, range, ctx=ctx), ctx=ctx
         ),
         (types.FunctionType, ts[1]): lambda: scanl(
             multiply(lhs, 2, ctx), iterable(rhs, range, ctx=ctx), ctx=ctx
         ),
-        (str, str): lambda: int(re.compile(lhs).search(rhs)),
+        (str, str): lambda: int(bool(re.compile(rhs).search(lhs))),
     }.get(ts, lambda: vectorise(orderless_range, lhs, rhs, ctx=ctx))()
 
 
 def overlapping_groups(lhs, rhs, ctx):
     """Element l
     (any, num) -> Overlapping groups/windows of a of length b
     (any, any) -> length(a) == length(b)
@@ -2949,16 +2967,16 @@
 
 
 def pluralise_count(lhs, rhs, ctx):
     """Element øP
     (str, num) -> count lhs lots of rhs
     (num, str) -> count rhs lots of lhs
     """
-    if isinstance(lhs, int):
-        return pluralise_count(rhs, lhs, ctx)
+    if vy_type(lhs) == NUMBER_TYPE:
+        return pluralise_count(rhs, int(lhs), ctx)
     return str(rhs) + " " + str(lhs) + "s" * (rhs != 1)
 
 
 def polynomial_expr_from_coeffs(lhs, ctx):
     """Element ∆Ċ
     (num) -> symbolic math representation of polynomial of degree n
              where each coefficient is 1
@@ -3393,14 +3411,64 @@
                 result += ints[i]
                 lhs = lhs[len(n) :]
         return result
     elif vy_type(lhs) is list:
         return vectorise(roman_numeral, lhs, ctx=ctx)
 
 
+def rotate_left(lhs, rhs, ctx):
+    """Element Ǔ
+    (any, num) -> a rotated left by b
+    (any) -> a rotated left by 1
+    """
+
+    lhs = iterable(lhs, ctx=ctx)
+    ts = vy_type(lhs)
+
+    if (ts is LazyList and not bool(lhs)) or len(lhs) == 0:
+        return lhs
+
+    if ts is str:
+        return lhs[rhs:] + lhs[:rhs]
+
+    @lazylist
+    def gen():
+        rotating_list = lhs
+        for _ in range(rhs):
+            rotating_list = rotating_list[1:] + [rotating_list[0]]
+        yield from rotating_list
+
+    return gen()
+
+
+def rotate_right(lhs, rhs, ctx):
+    """Element ǔ
+    (any, num) -> a rotated right by b
+    (any) -> a rotated right by 1
+    """
+
+    lhs = iterable(lhs, ctx=ctx)
+    ts = vy_type(lhs)
+
+    if (ts is LazyList and not bool(lhs)) or len(lhs) == 0:
+        return lhs
+
+    if ts is str:
+        return lhs[-rhs:] + lhs[:-rhs]
+
+    @lazylist
+    def gen():
+        rotating_list = list(lhs)
+        for _ in range(abs(int(rhs))):
+            rotating_list = [rotating_list[-1]] + rotating_list[:-1]
+        yield from rotating_list
+
+    return gen()
+
+
 def round_to(lhs, rhs, ctx):
     """Element ∆W
     (num, num) -> round(a, no_dec_places=b)
     """
     ts = vy_type(lhs, rhs)
     return {
         (NUMBER_TYPE, NUMBER_TYPE): lambda: sympy.nsimplify(
@@ -4788,15 +4856,15 @@
     return {
         (ts[0], NUMBER_TYPE): lambda: index(
             iterable(lhs, ctx=ctx), [0, rhs], ctx=ctx
         ),
         (NUMBER_TYPE, ts[1]): lambda: index(
             iterable(rhs, ctx=ctx), [0, lhs], ctx=ctx
         ),
-        (str, str): lambda: re.findall(lhs, rhs),
+        (str, str): lambda: re.findall(rhs, lhs),
     }.get(ts, lambda: vectorise(zero_slice, lhs, rhs, ctx=ctx))()
 
 
 def zfiller(lhs, rhs, ctx):
     """Element ∆Z
     zfill to rhs
     """
@@ -4810,16 +4878,16 @@
         + lhs,
         (str, str): lambda: lhs.zfill(len(rhs)),
     }.get(ts, lambda: vectorise(zfiller, lhs, rhs, ctx=ctx))()
 
 
 elements: dict[str, tuple[str, int]] = {
     "¬": process_element("sympy.nsimplify(int(not lhs))", 1),
-    "∧": process_element("lhs and rhs", 2),
-    "∨": process_element("lhs or rhs", 2),
+    "∧": process_element("rhs and lhs", 2),
+    "∨": process_element("rhs or lhs", 2),
     "⟇": process_element(remove_at_index, 2),
     "÷": (
         "lhs = pop(stack, 1, ctx); stack += iterable(lhs, ctx=ctx)",
         1,
     ),
     "×": process_element("'*'", 0),
     "•": process_element(log_mold_multi, 2),
@@ -5092,30 +5160,26 @@
     "ǐ": process_element(prime_factors, 1),
     "Ǒ": process_element(multiplicity, 2),
     "ǒ": process_element(modulo_3, 1),
     "Ǔ": (
         "rhs = pop(stack, 1, ctx)\n"
         + "if vy_type(rhs) == NUMBER_TYPE: \n"
         + "    lhs = pop(stack, 1, ctx)\n"
-        + "    stack.append(merge(index(lhs, [rhs, None, None], ctx), "
-        + "index(lhs, [None, rhs, None], ctx), ctx))\n"
+        + "    stack.append(rotate_left(lhs, rhs, ctx))\n"
         + "else:\n"
-        + "    stack.append(merge(index(rhs, [1, None, None], ctx), "
-        + "index(rhs, 0, ctx), ctx))\n",
+        + "    stack.append(rotate_left(rhs, 1, ctx))\n",
         2,
     ),
     "ǔ": (
         "rhs = pop(stack, 1, ctx)\n"
         + "if vy_type(rhs) == NUMBER_TYPE: \n"
         + "    lhs = pop(stack, 1, ctx)\n"
-        + "    stack.append(merge(index(lhs, [-rhs, None, None], ctx), "
-        + "index(lhs, [None, -rhs, None], ctx), ctx))\n"
+        + "    stack.append(rotate_right(lhs, rhs, ctx))\n"
         + "else:\n"
-        + "    stack.append(merge(index(rhs, -1, ctx), "
-        + "index(rhs, [None, -1, None], ctx), ctx))\n",
+        + "    stack.append(rotate_right(rhs, 1, ctx))\n",
         2,
     ),
     "↵": process_element(newline_split, 1),
     "¼": process_element("ctx.global_array.pop()", 0),
     "⅛": ("lhs = pop(stack,1,ctx); ctx.global_array.append(lhs)", 1),
     "¾": process_element("list(deep_copy(ctx.global_array))", 0),
     "Π": process_element(product, 1),
@@ -5164,14 +5228,15 @@
         "top = pop(stack, 1, ctx)\n"
         "if vy_type(top, simple=True) is list:\n"
         "    stack.append(lowest_common_multiple(top, ctx=ctx))\n"
         "else:\n"
         "    stack.append(lowest_common_multiple(pop(stack, 1, ctx), top, ctx))\n",
         2,
     ),
+    "∆Ṙ": process_element("sympy.nsimplify(random.random())", 0),
     "∆Z": process_element(zfiller, 2),
     "∆ċ": process_element(nth_cardinal, 1),
     "∆o": process_element(nth_ordinal, 1),
     "∆M": process_element(mode, 1),
     "∆ṁ": process_element(median, 1),
     "∆ṫ": process_element(totient, 1),
     "∆Ċ": process_element(polynomial_expr_from_coeffs, 1),
@@ -5378,14 +5443,15 @@
     "k₂": process_element("2 ** 20", 0),
     "k₃": process_element("2 ** 30", 0),
     "k∪": process_element('"aeiouy"', 0),
     "k⊍": process_element('"AEIOUY"', 0),
     "k∩": process_element('"aeiouyAEIOUY"', 0),
     "k□": process_element("[[0,1],[1,0],[0,-1],[-1,0]]", 0),
     "kṘ": process_element('"IVXLCDM"', 0),
+    "k•": process_element('["qwertyuiop","asdfghjkl","zxcvbnm"]', 0),
 }
 modifiers: dict[str, str] = {
     "&": (
         "stack.append(ctx.register)\n"
         "ctx.register = safe_apply(function_A, "
         "pop(stack, function_A.arity, ctx), ctx=ctx)\n"
     ),
```

### Comparing `vyxal-2.9.0/vyxal/encoding.py` & `vyxal-2.9.1/vyxal/encoding.py`

 * *Files identical despite different names*

### Comparing `vyxal-2.9.0/vyxal/helpers.py` & `vyxal-2.9.1/vyxal/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,37 +211,37 @@
 
 
 def get_input(ctx: Context, explicit=False) -> Any:
     """Returns the next input depending on where ctx tells to get the
     input from."""
     if ctx.use_top_input:
         if ctx.array_inputs and not explicit:
-            return ctx.inputs[0][0]
+            return vyxalify(ctx.inputs[0][0])
         if ctx.inputs[0][0]:
             ret = ctx.inputs[0][0][ctx.inputs[0][1] % len(ctx.inputs[0][0])]
             ctx.inputs[0][1] += 1
-            return ret
+            return vyxalify(ret)
         else:
             try:
                 temp = vy_eval(input("> " * ctx.repl_mode), ctx)
                 if ctx.empty_input_is_zero and temp == "":
                     return 0
             except Exception:  # skipcq: PYL-W0703
                 temp = 0
             return temp
     else:
         if len(ctx.inputs) == 1:
             ctx.use_top_input = True
             temp = get_input(ctx)
             ctx.use_top_input = False
-            return temp
+            return vyxalify(temp)
         elif ctx.inputs[-1][0]:
             ret = ctx.inputs[-1][0][ctx.inputs[-1][1] % len(ctx.inputs[-1][0])]
             ctx.inputs[-1][1] += 1
-            return ret
+            return vyxalify(ret)
         else:
             return 0
 
 
 def has_ind(lst: VyList, ind: int) -> bool:
     """Whether or not the list is long enough for that index"""
     if isinstance(lst, LazyList):
@@ -456,15 +456,15 @@
     VyList
     The content, molded into the shape.
     """
     final = []
     original, content = itertools.tee(content)
     for item in shape:
         temp = []
-        if isinstance(item, (int, str)):
+        if isinstance(item, str) or is_sympy(item):
             item = [item]
         for _ in item:
             obj = next(content, None)
             if obj is None:
                 content = itertools.tee(original)[1]
                 obj = next(content)
             temp.append(obj)
@@ -915,25 +915,21 @@
     """Apply function to every element of vector"""
     for element in iterable(vector, range, ctx=ctx):
         yield safe_apply(function, element, ctx=ctx)
 
 
 def vyxalify(value: Any) -> Any:
     """Takes a value and returns it as one of the four types we use here."""
-    if isinstance(value, sympy.core.numbers.Integer):
-        return int(value)
+    if isinstance(value, bool):
+        return str(value)
     elif is_sympy(value):
         return sympy.nsimplify(value, rational=True)
-    elif isinstance(value, (float, complex)):
+    elif isinstance(value, (float, complex, int)):
         return sympy.nsimplify(value, rational=True)
-    elif isinstance(value, bool):
-        return str(value)
-    elif isinstance(
-        value, (int, sympy.Rational, str, LazyList, types.FunctionType)
-    ):
+    elif isinstance(value, (str, LazyList, types.FunctionType)):
         return value
     elif isinstance(value, list):
         return list(map(vyxalify, value))
     else:
         return LazyList(map(vyxalify, value))
```

### Comparing `vyxal-2.9.0/vyxal/lexer.py` & `vyxal-2.9.1/vyxal/lexer.py`

 * *Files identical despite different names*

### Comparing `vyxal-2.9.0/vyxal/main.py` & `vyxal-2.9.1/vyxal/main.py`

 * *Files identical despite different names*

### Comparing `vyxal-2.9.0/vyxal/parse.py` & `vyxal-2.9.1/vyxal/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 TRIADIC_MODIFIERS = list("≬")
 # The modifiers are stored as lists to allow for potential digraph
 # modifiers.
 
 BREAK_CHARACTER = "X"
 RECURSE_CHARACTER = "x"
 
+DEFAULT_ARITY = "default"
+
 
 def process_parameters(tokens: list[lexer.Token]) -> tuple[str, list[str]]:
     """Handles the tokens from the first branch of a function defintion structure
 
     Returns a tuple of the name and parameters."""
     token_values = [token.value for token in tokens]
     branch_data = "".join(token_values)
@@ -164,15 +166,15 @@
                     # No body, so it's a function call
                     assert not parameters
                     structures.append(structure.FunctionCall(name))
 
             elif structure_cls == structure.Lambda:
                 if len(branches) == 1:
                     # that is, there is only a body - no arity
-                    arity = "default"
+                    arity = DEFAULT_ARITY
                 else:
                     try:
                         arity = int(branches[0][0].value)
                     except ValueError as ve:
                         raise ValueError(
                             "Arity must be parseable as an integer"
                         ) from ve
@@ -215,29 +217,33 @@
             # -ant that you break the while loop after dealing with the
             # modifier.
             if not tokens:
                 break
             remaining = parse(tokens, structure.MonadicModifier)
             if head.value == "⁽":
                 # 1-element lambda
-                structures.append(structure.Lambda(1, [remaining[0]]))
+                structures.append(
+                    structure.Lambda(DEFAULT_ARITY, [remaining[0]])
+                )
             else:
                 structures.append(
                     structure.MonadicModifier(head.value, remaining[0])
                 )
             structures += remaining[1:]
             break
         elif head.value in DYADIC_MODIFIERS:
             if not tokens:
                 break
             remaining = parse(tokens, structure.DyadicModifier)
             if head.value == "‡":
                 # 2-element lambda
                 structures.append(
-                    structure.Lambda(1, [remaining[0], remaining[1]])
+                    structure.Lambda(
+                        DEFAULT_ARITY, [remaining[0], remaining[1]]
+                    )
                 )
             else:
                 structures.append(
                     structure.DyadicModifier(
                         head.value, remaining[0], remaining[1]
                     )
                 )
@@ -247,15 +253,16 @@
             if not tokens:
                 break
             remaining = parse(tokens, structure.TriadicModifier)
             if head.value == "≬":
                 # 3-element lambda
                 structures.append(
                     structure.Lambda(
-                        1, [remaining[0], remaining[1], remaining[2]]
+                        DEFAULT_ARITY,
+                        [remaining[0], remaining[1], remaining[2]],
                     )
                 )
             else:
                 structures.append(
                     structure.TriadicModifier(
                         head.value,
                         remaining[0],
```

### Comparing `vyxal-2.9.0/vyxal/structure.py` & `vyxal-2.9.1/vyxal/structure.py`

 * *Files identical despite different names*

### Comparing `vyxal-2.9.0/vyxal/transpile.py` & `vyxal-2.9.1/vyxal/transpile.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,21 +33,21 @@
             if branch[0].branches[0][0].name in NILADIC_TYPES:
                 return vyxal.structure.Lambda(0, branch)
             return vyxal.structure.Lambda(
                 elements.get(branch[0].branches[0][0].value, ("", 1))[1],
                 branch,
             )
         elif isinstance(branch[0], vyxal.structure.RecurseStatement):
-            return vyxal.structure.Lambda(1, branch)
+            return vyxal.structure.Lambda(vyxal.parse.DEFAULT_ARITY, branch)
         elif isinstance(branch[0], vyxal.structure.Lambda):
             return branch[0]
         else:
-            return vyxal.structure.Lambda(1, branch)
+            return vyxal.structure.Lambda(vyxal.parse.DEFAULT_ARITY, branch)
     else:
-        return vyxal.structure.Lambda(1, branch)
+        return vyxal.structure.Lambda(vyxal.parse.DEFAULT_ARITY, branch)
 
 
 def transpile(
     program: str,
     dict_compress: bool = True,
     variables_as_digraphs: bool = False,
 ) -> str:
```

### Comparing `vyxal-2.9.0/setup.py` & `vyxal-2.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['num2words>=0.5.10,<0.6.0', 'sympy>=1.9,<2.0']
 
 entry_points = \
 {'console_scripts': ['vyxal = vyxal.main:cli']}
 
 setup_kwargs = {
     'name': 'vyxal',
-    'version': '2.9.0',
+    'version': '2.9.1',
     'description': 'A golfing language that has aspects of traditional programming languages.',
     'long_description': "# Vyxal\n\n[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Vyxal/Vyxal.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Vyxal/Vyxal/context:python) ![Test status](https://github.com/Vyxal/Vyxal/actions/workflows/run-tests.yaml/badge.svg)\n\nVyxal is a golfing language with a unique design philosophy: make things as short as possible but retain elegance while doing so. In very simple terms, this means\nkeeping aspects of traditional programming languages that most developers are familiar with, while still providing commands that allow golfers to actually _win_\nchallenges.\n\nVyxal is _not_ a language which forces users to mash random characters togther until something works. Nor is it a language that needs to be verbose. Vyxal is terse when\nit needs to be, and readable/stylish when it wants to be.\n\nVyxal is also deliberately designed to be an easy language to learn. While it may be possible to teach golfers how to program in Vyxal, it is far more likely that they will just learn through experience. The language is designed to be easy to understand, and to allow for fast development.\n\nUltimately, Vyxal is a language for golfers, by golfers.\n\n## Installation\n\nYou can also use the [online interpreter](https://vyxal.pythonanywhere.com) with no need to install!\n\nIf you only want to run Vyxal, all you need to run is this:\n```\npip install vyxal\n```\n\nIf you are working on Vyxal, install [Poetry](https://python-poetry.org), and then you can clone this repo and run:\n```\npoetry install\n```\n\n## Usage\n\nTo run using the script:\n```\nvyxal <file> <flags (single string of flags)> <input(s)>\n```\n\nIf you're using Poetry:\n```\npoetry run vyxal <file> <flags (single string of flags)> <input(s)>\n```\n\n## Why Make Another Golfing Language When There's Like Hundreds of Them Already?\n\nMost golfing languages are created with the intent of terse code - a goal that is obviously essential to the very core of what a golfing language is. However, this is\nmostly done at the expense of losing constructs within traditional programming languages that make things simple to do. Vyxal's raison d'être is to provide structures\nof practical languages - such as functions, variables and comments - that are oftentimes lost within the modern golfing language market.\n\nAnother reason for Vyxal is to provide an easy to use golfing language that anyone can quickly pick up - by providing tools that both new and experienced users are\nfamiliar with, Vyxal aims to cater to a wide demographic of golfers.\n\nPut simply, Vyxal exists because golfers need a golfing language - and because golfing languages could be better.\n\n## Links\n\n- [Repository](https://github.com/Vyxal/Vyxal)\n- [Online Interpreter](http://vyxal.pythonanywhere.com)\n<!-- TODO: fix broken links\n- [Tutorial](https://github.com/Vyxal/Vyxal/blob/master/docs/Tutorial.md)\n- [Codepage](https://github.com/Vyxal/Vyxal/blob/master/docs/codepage.txt)\n-->\n- [Main Chat Room (SE Chat)](https://chat.stackexchange.com/rooms/106764/vyxal)\n- [Vycord (Discord)](https://discord.gg/hER4Avd6fz)\n- [Elements](https://github.com/Vyxal/Vyxal/blob/v2.6.0/documents/knowledge/elements.md)\n- [Vyxapedia](https://vyxapedia.hyper-neutrino.xyz/)\n",
     'author': None,
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://vyxal.pythonanywhere.com/',
```

### Comparing `vyxal-2.9.0/PKG-INFO` & `vyxal-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vyxal
-Version: 2.9.0
+Version: 2.9.1
 Summary: A golfing language that has aspects of traditional programming languages.
 Home-page: https://vyxal.pythonanywhere.com/
 License: MIT
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

