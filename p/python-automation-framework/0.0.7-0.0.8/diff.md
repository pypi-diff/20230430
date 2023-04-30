# Comparing `tmp/python-automation-framework-0.0.7.tar.gz` & `tmp/python-automation-framework-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-automation-framework-0.0.7.tar", last modified: Fri Apr 28 19:20:48 2023, max compression
+gzip compressed data, was "python-automation-framework-0.0.8.tar", last modified: Sun Apr 30 08:20:53 2023, max compression
```

## Comparing `python-automation-framework-0.0.7.tar` & `python-automation-framework-0.0.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 19:20:48.000652 python-automation-framework-0.0.7/
--rw-r--r--   0 mikereiche   (502) staff       (20)     3099 2023-04-28 19:20:48.000528 python-automation-framework-0.0.7/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)     2849 2023-04-28 07:57:13.000000 python-automation-framework-0.0.7/README.md
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 19:20:47.998983 python-automation-framework-0.0.7/paf/
--rw-r--r--   0 mikereiche   (502) staff       (20)     5741 2023-04-27 19:14:21.000000 python-automation-framework-0.0.7/paf/assertion.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2567 2023-04-27 06:43:23.000000 python-automation-framework-0.0.7/paf/common.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1547 2023-04-28 19:19:24.000000 python-automation-framework-0.0.7/paf/component.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      309 2023-04-25 06:43:36.000000 python-automation-framework-0.0.7/paf/config.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2430 2023-04-26 13:34:30.000000 python-automation-framework-0.0.7/paf/control.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      104 2023-04-14 17:12:01.000000 python-automation-framework-0.0.7/paf/dom.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1913 2023-04-20 08:51:37.000000 python-automation-framework-0.0.7/paf/javascript.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2544 2023-04-27 19:06:53.000000 python-automation-framework-0.0.7/paf/locator.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     4249 2023-04-27 19:41:20.000000 python-automation-framework-0.0.7/paf/manager.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2737 2023-04-27 09:49:20.000000 python-automation-framework-0.0.7/paf/page.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2476 2023-04-25 06:48:40.000000 python-automation-framework-0.0.7/paf/request.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      209 2023-04-19 09:45:36.000000 python-automation-framework-0.0.7/paf/types.py
--rw-r--r--   0 mikereiche   (502) staff       (20)    12783 2023-04-28 19:17:28.000000 python-automation-framework-0.0.7/paf/uielement.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     6580 2023-04-28 08:22:20.000000 python-automation-framework-0.0.7/paf/xpath.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 19:20:47.999580 python-automation-framework-0.0.7/python_automation_framework.egg-info/
--rw-r--r--   0 mikereiche   (502) staff       (20)     3099 2023-04-28 19:20:47.000000 python-automation-framework-0.0.7/python_automation_framework.egg-info/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)      631 2023-04-28 19:20:47.000000 python-automation-framework-0.0.7/python_automation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-04-28 19:20:47.000000 python-automation-framework-0.0.7/python_automation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       46 2023-04-28 19:20:47.000000 python-automation-framework-0.0.7/python_automation_framework.egg-info/requires.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        4 2023-04-28 19:20:47.000000 python-automation-framework-0.0.7/python_automation_framework.egg-info/top_level.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-04-28 19:20:48.000685 python-automation-framework-0.0.7/setup.cfg
--rw-r--r--   0 mikereiche   (502) staff       (20)      587 2023-04-28 19:20:42.000000 python-automation-framework-0.0.7/setup.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 19:20:48.000376 python-automation-framework-0.0.7/test/
--rw-r--r--   0 mikereiche   (502) staff       (20)     1811 2023-04-28 18:50:16.000000 python-automation-framework-0.0.7/test/test_component.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      569 2023-04-19 16:18:15.000000 python-automation-framework-0.0.7/test/test_javascript.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1869 2023-04-28 08:20:26.000000 python-automation-framework-0.0.7/test/test_locator.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1440 2023-04-27 19:24:35.000000 python-automation-framework-0.0.7/test/test_page.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1673 2023-04-27 19:37:23.000000 python-automation-framework-0.0.7/test/test_request.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     7013 2023-04-28 19:14:06.000000 python-automation-framework-0.0.7/test/test_uielement.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      844 2023-04-27 19:22:39.000000 python-automation-framework-0.0.7/test/test_webdriver.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-30 08:20:53.232520 python-automation-framework-0.0.8/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3872 2023-04-30 08:20:53.232356 python-automation-framework-0.0.8/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3622 2023-04-29 17:41:40.000000 python-automation-framework-0.0.8/README.md
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-30 08:20:53.229737 python-automation-framework-0.0.8/paf/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     6192 2023-04-29 17:46:30.000000 python-automation-framework-0.0.8/paf/assertion.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2567 2023-04-27 06:43:23.000000 python-automation-framework-0.0.8/paf/common.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2156 2023-04-29 16:20:38.000000 python-automation-framework-0.0.8/paf/component.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      309 2023-04-25 06:43:36.000000 python-automation-framework-0.0.8/paf/config.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2430 2023-04-26 13:34:30.000000 python-automation-framework-0.0.8/paf/control.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      104 2023-04-14 17:12:01.000000 python-automation-framework-0.0.8/paf/dom.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1913 2023-04-20 08:51:37.000000 python-automation-framework-0.0.8/paf/javascript.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2544 2023-04-27 19:06:53.000000 python-automation-framework-0.0.8/paf/locator.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     4249 2023-04-29 16:24:25.000000 python-automation-framework-0.0.8/paf/manager.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2966 2023-04-29 17:56:24.000000 python-automation-framework-0.0.8/paf/page.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2476 2023-04-25 06:48:40.000000 python-automation-framework-0.0.8/paf/request.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      265 2023-04-29 08:35:21.000000 python-automation-framework-0.0.8/paf/types.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)    13473 2023-04-29 17:11:48.000000 python-automation-framework-0.0.8/paf/uielement.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     6598 2023-04-29 16:11:44.000000 python-automation-framework-0.0.8/paf/xpath.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-30 08:20:53.230637 python-automation-framework-0.0.8/python_automation_framework.egg-info/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3872 2023-04-30 08:20:53.000000 python-automation-framework-0.0.8/python_automation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)      631 2023-04-30 08:20:53.000000 python-automation-framework-0.0.8/python_automation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-04-30 08:20:53.000000 python-automation-framework-0.0.8/python_automation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       46 2023-04-30 08:20:53.000000 python-automation-framework-0.0.8/python_automation_framework.egg-info/requires.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        4 2023-04-30 08:20:53.000000 python-automation-framework-0.0.8/python_automation_framework.egg-info/top_level.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-04-30 08:20:53.232576 python-automation-framework-0.0.8/setup.cfg
+-rw-r--r--   0 mikereiche   (502) staff       (20)      587 2023-04-30 08:20:20.000000 python-automation-framework-0.0.8/setup.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-30 08:20:53.232082 python-automation-framework-0.0.8/test/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1910 2023-04-29 16:10:05.000000 python-automation-framework-0.0.8/test/test_component.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      569 2023-04-19 16:18:15.000000 python-automation-framework-0.0.8/test/test_javascript.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1869 2023-04-28 08:20:26.000000 python-automation-framework-0.0.8/test/test_locator.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      855 2023-04-29 12:28:05.000000 python-automation-framework-0.0.8/test/test_page.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1673 2023-04-27 19:37:23.000000 python-automation-framework-0.0.8/test/test_request.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     7312 2023-04-29 17:55:55.000000 python-automation-framework-0.0.8/test/test_uielement.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      844 2023-04-27 19:22:39.000000 python-automation-framework-0.0.8/test/test_webdriver.py
```

### Comparing `python-automation-framework-0.0.7/PKG-INFO` & `python-automation-framework-0.0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: python-automation-framework
-Version: 0.0.7
-Summary: Automation framework for the WebDriver API
-Home-page: https://github.com/mreiche/python-automation-framework
-Author: Mike Reiche
-Description-Content-Type: text/markdown
-
 # PAF - Python Automation Framework
 
 Python implementation of [Testerra](https://github.com/telekom/testerra) API.
 
 It is basically a wrapper for Selenium *WebDriver* and *WebElement* which bring some more comfort features.
 This is not a test framework, but it implements some assertion features anyway.
 
@@ -81,14 +73,45 @@
 
 I added two examples.
 
 1. [test_google.py](examples/test_google.py): is a regular Google search, implemented with [Page Objects](doc/pages.md) and [Components](doc/components.md). 
 2. [test_todo_mvc.py](examples/test_todo_mvc.py): are re-implemented test cases from the [Robot Framework TodoMVC](https://docs.robotframework.org/docs/examples/todo) example. It's IMHO developer friendly, better readable and less code. 
 
 
+## Comparison
+
+Comparison of the syntax with other frameworks.
+
+**Pylenium**
+```python
+py.get("a[href='/about']").should().have_text("About")
+```
+```python
+find("a[href='/about']").expect.text.be("About")
+```
+**SeleniumBase**
+```python
+self.assert_text_not_visible("Thanks for your purchase.", "#app .success")
+```
+```python
+find("#app .success").expect.text.not_be("Thanks for your purchase.")
+```
+**Selene**
+```python
+browser.all('#rso>div').should(have.size_greater_than(5)) \
+    .first.should(have.text('Selenium automates browsers'))
+```
+```python
+div = find("#rso>div")
+div.expect.count.greater_than(5).be(True)
+div.first.expect.text.be("Selenium automates browsers")
+```
+
+References: https://www.nextgenerationautomation.com/post/python-test-automation-frameworks
+
 ## Developer area
 ### Run the tests
 ```shell
 PYTHONPATH="." pytest --numprocesses=4 --cov=paf test
 ```
 
 ### Utils
```

### Comparing `python-automation-framework-0.0.7/README.md` & `python-automation-framework-0.0.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: python-automation-framework
+Version: 0.0.8
+Summary: Automation framework for the WebDriver API
+Home-page: https://github.com/mreiche/python-automation-framework
+Author: Mike Reiche
+Description-Content-Type: text/markdown
+
 # PAF - Python Automation Framework
 
 Python implementation of [Testerra](https://github.com/telekom/testerra) API.
 
 It is basically a wrapper for Selenium *WebDriver* and *WebElement* which bring some more comfort features.
 This is not a test framework, but it implements some assertion features anyway.
 
@@ -73,14 +81,45 @@
 
 I added two examples.
 
 1. [test_google.py](examples/test_google.py): is a regular Google search, implemented with [Page Objects](doc/pages.md) and [Components](doc/components.md). 
 2. [test_todo_mvc.py](examples/test_todo_mvc.py): are re-implemented test cases from the [Robot Framework TodoMVC](https://docs.robotframework.org/docs/examples/todo) example. It's IMHO developer friendly, better readable and less code. 
 
 
+## Comparison
+
+Comparison of the syntax with other frameworks.
+
+**Pylenium**
+```python
+py.get("a[href='/about']").should().have_text("About")
+```
+```python
+find("a[href='/about']").expect.text.be("About")
+```
+**SeleniumBase**
+```python
+self.assert_text_not_visible("Thanks for your purchase.", "#app .success")
+```
+```python
+find("#app .success").expect.text.not_be("Thanks for your purchase.")
+```
+**Selene**
+```python
+browser.all('#rso>div').should(have.size_greater_than(5)) \
+    .first.should(have.text('Selenium automates browsers'))
+```
+```python
+div = find("#rso>div")
+div.expect.count.greater_than(5).be(True)
+div.first.expect.text.be("Selenium automates browsers")
+```
+
+References: https://www.nextgenerationautomation.com/post/python-test-automation-frameworks
+
 ## Developer area
 ### Run the tests
 ```shell
 PYTHONPATH="." pytest --numprocesses=4 --cov=paf test
 ```
 
 ### Utils
```

### Comparing `python-automation-framework-0.0.7/paf/assertion.py` & `python-automation-framework-0.0.8/paf/assertion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import re
-from typing import Callable, Iterable
+from typing import Callable, Iterable, TypeVar, Generic
 
 import inject
 
+from paf.common import Rect
 from paf.control import Control, RetryException
-from paf.types import Supplier, Predicate, Number
+from paf.types import Supplier, Predicate, Number, Mapper
 
+ACTUAL_TYPE = TypeVar("ACTUAL_TYPE")
 
 class Format:
     @staticmethod
     def param(value: any):
         if value is None:
             return "[null]"
         else:
             return f"[{value}]"
     #
     # @staticmethod
     # def separate(*args):
     #     return " ".join(map(str, args))
 
 
-class AbstractPropertyAssertion:
+class AbstractPropertyAssertion(Generic[ACTUAL_TYPE]):
     def __init__(
         self,
         parent: None | object,
-        actual: Supplier[any],
+        actual: Supplier[ACTUAL_TYPE],
         subject: Supplier[str],
         raise_exception: bool = True,
         failed: Callable = None,
         passed: Callable = None,
         failed_finally: Callable = None
     ):
         self._raise = raise_exception
@@ -42,15 +44,15 @@
         self._subject = subject
         self._failed = failed
         self._passed = passed
         self._failed_finally = failed_finally
 
     def _test_sequence(
         self,
-        test: Predicate[any],
+        test: Predicate[ACTUAL_TYPE],
         additional_subject: Supplier = None,
     ) -> bool:
 
         control = inject.instance(Control)
         try:
             def perform_test():
                 assert test(self._actual())
@@ -79,24 +81,30 @@
         while inst._parent:
             path.append(inst._parent)
             inst = inst._parent
 
         return " ".join(map(lambda x: x._subject(), reversed(path)))
 
     @property
-    def actual(self):
+    def actual(self) -> ACTUAL_TYPE:
         return self._actual()
 
 
-class BinaryAssertion(AbstractPropertyAssertion):
+class BinaryAssertion(AbstractPropertyAssertion[ACTUAL_TYPE]):
     def be(self, expected: any) -> bool:
         return self._test_sequence(lambda actual: actual == expected, lambda: f" to be {Format.param(expected)}")
 
 
-class QuantityAssertion(BinaryAssertion):
+class QuantityAssertion(Generic[ACTUAL_TYPE], BinaryAssertion[ACTUAL_TYPE]):
+    def map(self, mapper: Mapper):
+        return self.__class__(
+            parent=self,
+            actual=lambda: mapper(self._actual()),
+            subject=lambda: "mapped",
+        )
 
     def not_be(self, expected: any) -> bool:
         return self._test_sequence(lambda actual: actual != expected, lambda: f" not to be {Format.param(expected)}")
 
     def between(self, lower: Number, higher: Number):
         return BinaryAssertion(
             parent=self,
@@ -129,15 +137,15 @@
         return BinaryAssertion(
             parent=self,
             actual=lambda: self._actual() <= expected,
             subject=lambda: f"lower equal than {Format.param(expected)}",
         )
 
 
-class StringAssertion(QuantityAssertion):
+class StringAssertion(QuantityAssertion[str]):
     def starts_with(self, expected: str):
         return BinaryAssertion(
             parent=self,
             actual=lambda: str(self._actual()).startswith(expected),
             subject=lambda: f"starts with {Format.param(expected)}",
         )
 
@@ -174,15 +182,18 @@
 
         return BinaryAssertion(
             parent=self,
             actual=lambda: regex.search(self._actual()) is not None,
             subject=lambda: f"has words {Format.param(pattern)}",
         )
 
-
     @property
     def length(self):
         return QuantityAssertion(
             parent=self,
             actual=lambda: len(self._actual()),
             subject=lambda: f"length {Format.param(len(self._actual()))}",
         )
+
+
+class RectAssertion(AbstractPropertyAssertion[Rect]):
+    pass
```

### Comparing `python-automation-framework-0.0.7/paf/common.py` & `python-automation-framework-0.0.8/paf/common.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.7/paf/component.py` & `python-automation-framework-0.0.8/paf/component.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,71 @@
-from typing import TypeVar
+from typing import Type
 
 from selenium.webdriver.support.color import Color
 
 from paf.common import HasParent, Locator, Point
-from paf.uielement import UiElement, PageObject, PageObjectList
+from paf.types import COMPONENT, PAGE
+from paf.uielement import UiElement, PageObject, PageObjectList, UiElementTests
 
-T = TypeVar("T")
 
-
-class Component(PageObject[T], PageObjectList[T], HasParent):
+class Component(PageObject[COMPONENT], PageObjectList[COMPONENT], HasParent, UiElementTests):
 
     def highlight(self, color: Color = Color.from_string("#0f0"), seconds: float = 2):
         self._ui_element.highlight(color, seconds)
         return self
 
     def __init__(self, ui_element: UiElement):
         self._ui_element = ui_element
         ui_element._parent = self
 
     def _find(self, by: Locator):
         ui_element = self._ui_element.find(by)
-        ui_element._parent = self
+        #ui_element._parent = self
         return ui_element
 
     @property
     def name(self):
-        return f"{self.__class__.__name__}({self._ui_element.name})"
+        return f"{self.__class__.__name__}"
+
+    @property
+    def name_path(self):
+        return self._ui_element.name_path
 
     def __str__(self):
         return self.name
 
-    def scroll_into_view(self, offset: Point = Point()):
-        self._ui_element.scroll_into_view(offset)
+    def scroll_into_view(self, x: int = 0, y: int = 0):
+        self._ui_element.scroll_into_view(x, y)
 
-    def scroll_to_top(self, offset: Point = Point()):
-        self._ui_element.scroll_to_top(offset)
+    def scroll_to_top(self,  x: int = 0, y: int = 0):
+        self._ui_element.scroll_to_top(x, y)
 
     def __iter__(self):
         for i in range(self._ui_element._count_elements()):
             yield self.__getitem__(i)
 
-    def __getitem__(self, index: int) -> T:
+    def __getitem__(self, index: int) -> COMPONENT:
         ui_element = UiElement(
             ui_element=self._ui_element._ui_element,
             webdriver=self._ui_element._webdriver,
             by=self._ui_element._by,
             index=index
         )
         component = self.__class__(ui_element)
         component._parent = self._parent
         return component
+
+    def _create_component(self, component_class: Type[COMPONENT], ui_element: "UiElement") -> COMPONENT:
+        component = component_class(ui_element)
+        component._parent = self
+        return component
+
+    def _create_page(self, page_class: Type[PAGE]) -> PAGE:
+        return page_class(self._ui_element.webdriver)
+
+    @property
+    def expect(self):
+        return self._ui_element.expect
+
+    @property
+    def wait_for(self):
+        return self._ui_element.wait_for
```

### Comparing `python-automation-framework-0.0.7/paf/control.py` & `python-automation-framework-0.0.8/paf/control.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.7/paf/javascript.py` & `python-automation-framework-0.0.8/paf/javascript.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.7/paf/locator.py` & `python-automation-framework-0.0.8/paf/locator.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.7/paf/manager.py` & `python-automation-framework-0.0.8/paf/manager.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.7/paf/page.py` & `python-automation-framework-0.0.8/paf/page.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,79 +1,82 @@
 from typing import Type, TypeVar
 
 import inject
+from selenium.webdriver import ActionChains
 from selenium.webdriver.remote.webdriver import WebDriver
 
 from paf.assertion import StringAssertion, Format
-from paf.common import HasName, Locator
+from paf.common import HasName, Locator, Point
 from paf.manager import WebDriverManager
-
-C = TypeVar("C")
-P = TypeVar("P")
+from paf.types import PAGE, COMPONENT
 
 
 class PageFactory:
-    def create_page(self, page_class: Type[P], webdriver: WebDriver = None) -> P:
+    def create_page(self, page_class: Type[PAGE], webdriver: WebDriver = None) -> PAGE:
         if not webdriver:
             webdriver = inject.instance(WebDriverManager).get_webdriver()
 
         return page_class(webdriver)
 
 
 class BasePage(HasName):
     def __init__(self, webdriver: WebDriver):
         self._webdriver = webdriver
 
     def open(self, url: str):
         self._webdriver.get(url)
         return self
 
-    @property
-    def webdriver(self):
-        return self._webdriver
-
     def __str__(self):
         return self.name
 
     def _find(self, by: Locator):
         from paf.uielement import UiElement
         return UiElement(by, webdriver=self._webdriver, parent=self)
 
     @property
     def name(self):
         return self.__class__.__name__
 
     @property
-    def expect(self):
-        return PageAssertion(self, self._webdriver)
-
-    @property
-    def wait_for(self):
-        return PageAssertion(self, self._webdriver, raise_exception=False)
+    def webdriver(self):
+        return self._webdriver
 
 
 class FinderPage(BasePage):
     def find(self, by: Locator):
         ui_element = self._find(by)
         ui_element._parent = None
         return ui_element
 
 
 class Page(BasePage):
     def __init__(self, webdriver: WebDriver):
         super().__init__(webdriver)
 
-    def _create_component(self, component_class: Type[C], ui_element: "UiElement") -> C:
+    def _create_component(self, component_class: Type[COMPONENT], ui_element: "UiElement") -> COMPONENT:
         component = component_class(ui_element)
         component._parent = self
         return component
 
-    def _create_page(self, page_class: Type[P]) -> P:
+    def _create_page(self, page_class: Type[PAGE]) -> PAGE:
         return page_class(self._webdriver)
 
+    @property
+    def expect(self):
+        return PageAssertion(self, self._webdriver)
+
+    @property
+    def wait_for(self):
+        return PageAssertion(self, self._webdriver, raise_exception=False)
+
+    def scroll_by(self, x: int = 0, y: int = 0):
+        actions = ActionChains(self._webdriver)
+        actions.scroll_by_amount(x, y).perform()
+
 
 class PageAssertion:
 
     def __init__(
         self,
         page: BasePage,
         webdriver: WebDriver,
```

### Comparing `python-automation-framework-0.0.7/paf/request.py` & `python-automation-framework-0.0.8/paf/request.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.7/paf/uielement.py` & `python-automation-framework-0.0.8/paf/uielement.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 from selenium.webdriver import ActionChains
 from selenium.webdriver.common.by import By as SeleniumBy
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support.color import Color
 
 import paf.javascript as script
-from paf.assertion import StringAssertion, Format, BinaryAssertion, QuantityAssertion
+from paf.assertion import StringAssertion, Format, BinaryAssertion, QuantityAssertion, RectAssertion
 from paf.common import HasParent, Locator, Point, Rect, Property, Formatter
 from paf.control import Control
+from paf.dom import Attribute
 from paf.locator import By
 from paf.types import Mapper, Consumer, R
 from paf.xpath import XPath
 
 
 class UiElementActions:
 
@@ -55,14 +56,18 @@
     def type(self, value: str):
         pass
 
     @abstractmethod
     def clear(self):
         pass
 
+    @abstractmethod
+    def submit(self):
+        pass
+
 
 T = TypeVar('T')
 
 
 class PageObjectList(Generic[T], Iterable):
     @abstractmethod
     def __getitem__(self, index: int) -> T:
@@ -80,43 +85,47 @@
     def last(self) -> T:
         return self.__getitem__(-1)
 
 
 class PageObject(Generic[T]):
 
     @abstractmethod
-    def scroll_into_view(self, offset: Point = Point()):
+    def scroll_into_view(self, x: int = 0, y: int = 0):
         pass
 
     @abstractmethod
-    def scroll_to_top(self, offset: Point = Point()):
+    def scroll_to_top(self, x: int = 0, y: int = 0):
         pass
 
     @abstractmethod
     def highlight(self, color: Color = Color.from_string("#0f0"), seconds: float = 2):
         pass
 
 
-class TestableUiElement(PageObject["TestableUiElement"]):
+class UiElementTests:
     @property
     @abstractmethod
     def expect(self) -> "UiElementAssertion":
         pass
 
     @property
     @abstractmethod
     def wait_for(self) -> "UiElementAssertion":
         pass
 
 
-class InteractiveUiElement(TestableUiElement, UiElementActions, PageObject["InteractiveUiElement"], ABC):
+class TestableUiElement(PageObject["TestableUiElement"], UiElementTests, ABC):
+    pass
+
+
+class InteractiveUiElement(PageObject["InteractiveUiElement"], UiElementTests, UiElementActions, ABC):
     pass
 
 
-class UiElement(InteractiveUiElement, HasParent, PageObjectList["UiElement"]):
+class UiElement(UiElementTests, UiElementActions, HasParent, PageObjectList["UiElement"]):
 
     def __init__(
         self,
         by: Locator,
         ui_element: "UiElement" = None,
         webdriver: WebDriver = None,
         parent: object = None,
@@ -276,26 +285,30 @@
     def wait_for(self):
         return UiElementAssertion(self, raise_exception=False)
 
     def clear(self):
         self._action_sequence(lambda web_element: web_element.clear())
         return self
 
+    def submit(self):
+        self._action_sequence(lambda web_element: web_element.submit())
+        return self
+
     def __str__(self):
         return self.name
 
     @property
     def name(self):
         return f"UiElement({self._by.__str__()})[{self._index}]"
 
-    def scroll_into_view(self, offset: Point = Point()):
-        self._action_sequence(lambda web_element: script.scroll_to_center(self._webdriver, web_element, offset))
+    def scroll_into_view(self, x: int = 0, y: int = 0):
+        self._action_sequence(lambda web_element: script.scroll_to_center(self._webdriver, web_element, Point(x, y)))
 
-    def scroll_to_top(self, offset: Point = Point()):
-        self._action_sequence(lambda web_element: script.scroll_to_top(self._webdriver, web_element, offset))
+    def scroll_to_top(self, x: int = 0, y: int = 0):
+        self._action_sequence(lambda web_element: script.scroll_to_top(self._webdriver, web_element, Point(x, y)))
 
     def _count_elements(self):
         count = 0
 
         def _count(web_elements: List[WebElement]):
             nonlocal count
             count = len(web_elements)
@@ -321,26 +334,25 @@
             parent=self._parent,
             index=index
         )
 
 
 A = TypeVar('A')
 
-
 class UiElementAssertion:
 
     def __init__(
         self,
         ui_element: UiElement,
         raise_exception: bool = True,
     ):
         self._ui_element = ui_element
         self._raise = raise_exception
 
-    def _create_property_assertion(
+    def _map_web_element_property(
         self,
         assertion_class: Type[A],
         mapper: Mapper[WebElement, any],
         property_name: str
     ) -> A:
         return assertion_class(
             parent=None,
@@ -350,55 +362,61 @@
         )
 
     @property
     def text(self):
         def _map(web_element: WebElement):
             return web_element.text
 
-        return self._create_property_assertion(StringAssertion, _map, "text")
+        return self._map_web_element_property(StringAssertion, _map, "text")
 
     @property
     def displayed(self):
         def _map(web_element: WebElement):
             return web_element.is_displayed()
 
-        return self._create_property_assertion(BinaryAssertion, _map, "displayed")
+        return self._map_web_element_property(BinaryAssertion, _map, "displayed")
 
     @property
     def enabled(self):
         def _map(web_element: WebElement):
             return web_element.is_enabled()
 
-        return self._create_property_assertion(BinaryAssertion, _map, "enabled")
+        return self._map_web_element_property(BinaryAssertion, _map, "enabled")
 
     @property
     def selected(self):
         def _map(web_element: WebElement):
             return web_element.is_selected()
 
-        return self._create_property_assertion(BinaryAssertion, _map, "selected")
+        return self._map_web_element_property(BinaryAssertion, _map, "selected")
 
     @property
     def tag_name(self):
         def _map(web_element: WebElement):
             return web_element.tag_name
 
-        return self._create_property_assertion(StringAssertion, _map, "tag name")
+        return self._map_web_element_property(StringAssertion, _map, "tag name")
+
+    def attribute(self, attribute: str|Attribute):
+        if isinstance(attribute, Attribute):
+            attribute = attribute.value
 
-    def attribute(self, attribute: str):
         def _map(web_element: WebElement):
             return web_element.get_attribute(attribute)
 
-        return self._create_property_assertion(StringAssertion, _map, f"attribute({attribute}")
+        return self._map_web_element_property(StringAssertion, _map, f"attribute({attribute})")
 
     def css(self, property_name: str):
         def _map(web_element: WebElement):
             return web_element.value_of_css_property(property_name)
 
-        return self._create_property_assertion(StringAssertion, _map, f"css({property_name}")
+        return self._map_web_element_property(StringAssertion, _map, f"css({property_name}")
+
+    def classes(self, *classes):
+        return self.attribute(Attribute.CLASS).has_words(*classes)
 
     @property
     def visible(self):
         return self._visible(False)
 
     @property
     def fully_visible(self):
@@ -413,21 +431,28 @@
             else:
                 return viewport.intersects(bounds)
 
         name = "visible"
         if fully:
             name = f"fully {name}"
 
-        return self._create_property_assertion(BinaryAssertion, _map, name)
+        return self._map_web_element_property(BinaryAssertion, _map, name)
 
     @property
     def value(self):
         return self.attribute("value")
 
     @property
     def count(self):
-        return QuantityAssertion(
+        return QuantityAssertion[int](
             parent=None,
             actual=lambda: self._ui_element._count_elements(),
             subject=lambda: f"{self._ui_element.name_path} count {Format.param(self._ui_element._count_elements())}",
             raise_exception=self._raise,
         )
+
+    @property
+    def bounds(self):
+        def _map(web_element: WebElement):
+            return Rect.from_web_element(web_element)
+
+        return self._map_web_element_property(RectAssertion, _map, "bounds")
```

### Comparing `python-automation-framework-0.0.7/paf/xpath.py` & `python-automation-framework-0.0.8/paf/xpath.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,21 +111,21 @@
     def attribute(self, attribute: str):
         if not XPath._is_function(attribute):
             attribute = f"@{attribute}"
 
         return XPath.Test(self, attribute)
 
     def id(self, value: str):
-        return self.attribute(Attribute.ID).be(value)
+        return self.attribute(Attribute.ID.value).be(value)
 
     def name(self, value: str):
-        return self.attribute(Attribute.NAME).be(value)
+        return self.attribute(Attribute.NAME.value).be(value)
 
     def classes(self, *classes: any):
-        return self.attribute(Attribute.CLASS).has_words(*classes)
+        return self.attribute(Attribute.CLASS.value).has_words(*classes)
 
     @property
     def text(self):
         return XPath.Test(self, ".//text()")
 
     @staticmethod
     def _translate_sub_selection(selector: str):
```

### Comparing `python-automation-framework-0.0.7/python_automation_framework.egg-info/PKG-INFO` & `python-automation-framework-0.0.8/python_automation_framework.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-automation-framework
-Version: 0.0.7
+Version: 0.0.8
 Summary: Automation framework for the WebDriver API
 Home-page: https://github.com/mreiche/python-automation-framework
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 
 # PAF - Python Automation Framework
 
@@ -81,14 +81,45 @@
 
 I added two examples.
 
 1. [test_google.py](examples/test_google.py): is a regular Google search, implemented with [Page Objects](doc/pages.md) and [Components](doc/components.md). 
 2. [test_todo_mvc.py](examples/test_todo_mvc.py): are re-implemented test cases from the [Robot Framework TodoMVC](https://docs.robotframework.org/docs/examples/todo) example. It's IMHO developer friendly, better readable and less code. 
 
 
+## Comparison
+
+Comparison of the syntax with other frameworks.
+
+**Pylenium**
+```python
+py.get("a[href='/about']").should().have_text("About")
+```
+```python
+find("a[href='/about']").expect.text.be("About")
+```
+**SeleniumBase**
+```python
+self.assert_text_not_visible("Thanks for your purchase.", "#app .success")
+```
+```python
+find("#app .success").expect.text.not_be("Thanks for your purchase.")
+```
+**Selene**
+```python
+browser.all('#rso>div').should(have.size_greater_than(5)) \
+    .first.should(have.text('Selenium automates browsers'))
+```
+```python
+div = find("#rso>div")
+div.expect.count.greater_than(5).be(True)
+div.first.expect.text.be("Selenium automates browsers")
+```
+
+References: https://www.nextgenerationautomation.com/post/python-test-automation-frameworks
+
 ## Developer area
 ### Run the tests
 ```shell
 PYTHONPATH="." pytest --numprocesses=4 --cov=paf test
 ```
 
 ### Utils
```

### Comparing `python-automation-framework-0.0.7/python_automation_framework.egg-info/SOURCES.txt` & `python-automation-framework-0.0.8/python_automation_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.7/setup.py` & `python-automation-framework-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="python-automation-framework",
     description="Automation framework for the WebDriver API",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.0.7",
+    version="0.0.8",
     url="https://github.com/mreiche/python-automation-framework",
     author="Mike Reiche",
     packages=["paf"],
     install_requires=["inject>=4.3.1", "selenium>=4.8.3", "is-empty>=1.0.1"],
 )
```

### Comparing `python-automation-framework-0.0.7/test/test_component.py` & `python-automation-framework-0.0.8/test/test_component.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from functools import cache
 
 import inject
 import pytest
 
-import paf.config
 from paf.component import Component
 from paf.locator import By
-from paf.page import Page, PageFactory
 from paf.manager import WebDriverManager
+from paf.page import Page, PageFactory
 from paf.xpath import XPath
 
 
 @pytest.fixture
 def components_page():
     yield inject.instance(PageFactory).create_page(ComponentsPage)
 
@@ -36,24 +35,25 @@
 class TableRow(Component["TableRow"]):
     @property
     def col(self):
         return self._find(XPath.at("(th|td)"))
 
 
 def test_component_name_path(components_page: ComponentsPage):
-    assert components_page.custom_component.type.name_path == "ComponentsPage > MyComponent(UiElement(By.tag name(body))[0]) > UiElement(By.id(input))[0]"
+    assert components_page.custom_component.type.name_path == "ComponentsPage > MyComponent > UiElement(By.tag name(body))[0] > UiElement(By.id(input))[0]"
 
 
 def test_component_list_name(components_page: ComponentsPage):
-    assert components_page.custom_component.last.name_path == "ComponentsPage > MyComponent(UiElement(By.tag name(body))[-1])"
+    assert components_page.custom_component.last.name_path == "ComponentsPage > MyComponent > UiElement(By.tag name(body))[-1]"
 
 
 def test_component_list(components_page: ComponentsPage):
     components_page.open("https://testpages.herokuapp.com/styled/tag/dynamic-table.html")
     rows = components_page.table_row
+    assert rows.name_path == "ComponentsPage > TableRow > UiElement(By.xpath(//table[@ID='dynamictable']//tr))[0]"
     rows.expect.count.be(3)
     rows.first.col.first.expect.text.be("name")
     rows.first.col.last.expect.text.be("age")
 
     rows.last.col.last.expect.text.be("42")
 
     for row in rows:
```

### Comparing `python-automation-framework-0.0.7/test/test_javascript.py` & `python-automation-framework-0.0.8/test/test_javascript.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.7/test/test_locator.py` & `python-automation-framework-0.0.8/test/test_locator.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.7/test/test_request.py` & `python-automation-framework-0.0.8/test/test_request.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.7/test/test_uielement.py` & `python-automation-framework-0.0.8/test/test_uielement.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import inject
 import pytest
+from selenium.webdriver.remote.webdriver import WebDriver, BaseWebDriver
 from selenium.webdriver.support.color import Color
 
 from paf.control import Control
 from paf.locator import By
 from paf.manager import WebDriverManager
 from paf.page import PageFactory, FinderPage
 from paf.xpath import XPath
@@ -25,35 +26,43 @@
 
 def test_finder_page(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
 
     p = finder.find(By.id("para1"))
     assert p.name_path == 'UiElement(By.id(para1))[0]'
     assert p.name == p.name_path
+    assert isinstance(finder.webdriver, BaseWebDriver)
 
 
 # def test_rect():
 #     finder = page_factory.create_page(FinderPage, create_webdriver())
 #     finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
 #
 #     p = finder.find(By.id("para1"))
 #     rect = p._get_bounds()
 #     assert isinstance(rect, Rect)
 #     assert rect.width == 962
 #     assert rect.height == 27
 
-def test_text_assertions(finder: FinderPage):
+def test_assertions(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
 
     p = finder.find("#para1")
 
+    # tag name
     p.expect.tag_name.be("p")
 
+    # classes
+    p.expect.classes("main").be(True)
+    p.expect.classes("sub").be(False)
+
     text = p.expect.text
     text.be("A paragraph of text")
+    text.map(str.upper).be("A PARAGRAPH OF TEXT")
+    text.not_be("Bla")
     text.contains("paragraph").be(True)
     text.has_words("paragraph", "text").be(True)
     text.starts_with("A").be(True)
     text.ends_with("text").be(True)
     text.matches("hello").be(False)
     assert text.actual == "A paragraph of text"
 
@@ -80,15 +89,15 @@
     finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
 
     p = finder.find(By.id("para1"))
     p.highlight(color=Color.from_string("#0f0"))
     p.expect.css("outline").be("rgb(0, 255, 0) solid 5px")
 
 
-def test_scroll_until_visible(finder: FinderPage):
+def test_scroll_to_visible(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/find-by-playground-test.html")
 
     p = finder.find(By.id("pre1").unique)
     p.expect.visible.be(False)
     p.scroll_into_view()
     p.expect.visible.be(True)
     p.expect.fully_visible.be(True)
```

### Comparing `python-automation-framework-0.0.7/test/test_webdriver.py` & `python-automation-framework-0.0.8/test/test_webdriver.py`

 * *Files identical despite different names*

