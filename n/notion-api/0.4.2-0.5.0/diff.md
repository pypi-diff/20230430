# Comparing `tmp/notion_api-0.4.2.tar.gz` & `tmp/notion_api-0.5.0.tar.gz`

## Comparing `notion_api-0.4.2.tar` & `notion_api-0.5.0.tar`

### file list

```diff
@@ -1,38 +1,43 @@
--rw-r--r--   0        0        0    11253 2020-02-02 00:00:00.000000 notion_api-0.4.2/README.md
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/py.typed
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/api/__init__.py
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/api/_about.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/api/_pkgv.py
--rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/api/blockmixin.py
--rw-r--r--   0        0        0    20946 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/api/blocktypefactory.py
--rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/api/client.py
--rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/api/notionblock.py
--rw-r--r--   0        0        0    26159 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/api/notiondatabase.py
--rw-r--r--   0        0        0    20211 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/api/notionpage.py
--rw-r--r--   0        0        0    15457 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/api/notionworkspace.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/exceptions/__init__.py
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/exceptions/errors.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/exceptions/validate.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/properties/__init__.py
--rw-r--r--   0        0        0    13595 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/properties/blocktypes.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/properties/build.py
--rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/properties/common.py
--rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/properties/files.py
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/properties/options.py
--rw-r--r--   0        0        0    14699 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/properties/propertyobjects.py
--rw-r--r--   0        0        0    15442 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/properties/propertyvalues.py
--rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/properties/richtext.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/propertyitems/__init__.py
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/propertyitems/base.py
--rw-r--r--   0        0        0     8508 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/propertyitems/call.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/query/__init__.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/query/compound.py
--rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/query/conditions.py
--rw-r--r--   0        0        0     7600 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/query/propfilter.py
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/query/sort.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 notion_api-0.4.2/notion/query/timestamp.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 notion_api-0.4.2/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 notion_api-0.4.2/LICENSE
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 notion_api-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    12717 2020-02-02 00:00:00.000000 notion_api-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    12785 2020-02-02 00:00:00.000000 notion_api-0.5.0/README.md
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/py.typed
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/__init__.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/_about.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/_pkgv.py
+-rw-r--r--   0        0        0     5950 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/blockmixin.py
+-rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/client.py
+-rw-r--r--   0        0        0    30361 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/notionblock.py
+-rw-r--r--   0        0        0    25951 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/notiondatabase.py
+-rw-r--r--   0        0        0    20093 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/notionpage.py
+-rw-r--r--   0        0        0    15457 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/notionworkspace.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/block_ext/__init__.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/block_ext/code.py
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/block_ext/equation.py
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/block_ext/richtext.py
+-rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/block_ext/table.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/block_ext/todo.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/exceptions/__init__.py
+-rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/exceptions/errors.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/exceptions/validate.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/properties/__init__.py
+-rw-r--r--   0        0        0    15294 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/properties/blocktypes.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/properties/build.py
+-rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/properties/common.py
+-rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/properties/files.py
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/properties/options.py
+-rw-r--r--   0        0        0    14699 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/properties/propertyobjects.py
+-rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/properties/propertyvalues.py
+-rw-r--r--   0        0        0     7878 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/properties/richtext.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/propertyitems/__init__.py
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/propertyitems/base.py
+-rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/propertyitems/call.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/query/__init__.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/query/compound.py
+-rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/query/conditions.py
+-rw-r--r--   0        0        0     7493 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/query/propfilter.py
+-rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/query/sort.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/query/timestamp.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 notion_api-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 notion_api-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 notion_api-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    14249 2020-02-02 00:00:00.000000 notion_api-0.5.0/PKG-INFO
```

### Comparing `notion_api-0.4.2/README.md` & `notion_api-0.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,18 @@
     &nbsp;
     <a href="https://pycqa.github.io/isort/"><img alt="code style: black" src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336"></a>
 
 </p>
 
 __Disclaimer: This is an _unofficial_ package and has no affiliation with Notion.so__  
 
-A wrapper for Notion's API, aiming to simplify the dynamic nature of interacting with Notion. This project is still a work in progress, and features will continue to change. Below are a few examples of the current functionality. 
+A wrapper for Notion's API, aiming to simplify the dynamic nature of interacting with Notion.  
+README contains examples of the main functionality, including: creating Pages/Databases/Blocks, adding/removing/editing properties, retrieving property values, and database queries.  
+Some more in-depth walkthroughs can be be found in `examples/`    
+This package is not complete - new features will continue to be added, and current features may change.
 
 <br>
 
 <div border="0" align="center">
     <table>
         <tr>
             <td align="center"><b>Links: Notion API Updates</b></td>
@@ -123,86 +126,120 @@
 
 The current version of the Notion api does not allow pages to be created to the parent `workspace`.  
 Create objects by passing an existing Page/Database instance as an arg to the `create` classmethods.
 
 ```py
 new_database = notion.Database.create(
     parent_instance=testpage,
-    database_title="Title",
+    database_title="Example Database",
     name_column="page", # This is the column containing page names. Defaults to "Name".
-    is_inline=True,
-    description="Example Database.",
+    is_inline=True, # can also toggle inline with setters.
+    description="Database description can go here.",
 )
 
 new_page = notion.Page.create(new_database, page_title="A new database row")
 ```
 
-Blocks can be created with `notion.api.blocktypefactory.BlockFactory` by appending to an exisiting Block or Page.  
-The new block is always returned as an instance of `notion.api.notionblock.Block`.
+Blocks are also created using the classmethods of `Block`. They all require a parent instance of either `Page` or `Block` to append the new block too.
+The newly created block is returned as an instance of `Block`, which can be used as the parent instance to a nested block. 
 ```py
 from notion import properties as prop
 
-# `new_synced_block` refers to the original synced block in the Notion UI.
-original_synced_block = notion.BlockFactory.new_synced_block(homepage)
+# `original_synced_block` refers to the original synced block in the Notion UI.
+original_synced_block = notion.Block.original_synced_block(homepage)
 
 # Adding content to the synced block
-notion.BlockFactory.paragraph(
-    original_synced_block, [prop.RichText("This is a synced block.")]
-)
+notion.Block.paragraph(original_synced_block, [prop.RichText("This is a synced block.")])
+
 # Referencing the synced block in a new page.
-notion.BlockFactory.reference_synced_block(new_page, original_synced_block.id)
+notion.Block.duplicate_synced_block(new_page, original_synced_block.id)
 ```
 
 <br>
 
-### Example Workflow: **_Appending blocks to a page as a reminder._**
+There are few extensions to the `Block` class that have specific functions unique to their block-type.  
+Below is an example using `CodeBlock`. The others are `TableBlock`, `EquationBlock`, `RichTextBlock`, and `ToDoBlock`. You can see usage for them in `examples/block_extensions.md`.
 
 ```py
-def in_block_reminder(page: notion.Page, message: str, user_name: str) -> None:
-    mentionblock = notion.BlockFactory.paragraph(
+code_block = notion.CodeBlock("84c5721d8a954667902a757f0033f9e0")
+
+class_diagram = r"""
+%%{init: { 'logLevel': 'debug', 'theme': 'default' , 'themeVariables': { 'darkMode':'true', 'git0': '#ff0000', 'git1': '#00ff00', 'git2': '#0000ff', 'git3': '#ff00ff', 'git4': '#00ffff', 'git5': '#ffff00', 'git6': '#ff00ff', 'git7': '#00ffff' } } }%%
+gitGraph
+       commit
+       branch develop
+       commit tag:"v1.0.0"
+       commit
+       checkout main
+       commit type: HIGHLIGHT
+       commit
+       merge develop
+       commit
+       branch featureA
+       commit
+"""
+
+code_block.language = prop.CodeBlockLang.mermaid
+code_block.code = class_diagram
+code_block.caption = "Example from https://mermaid.js.org/syntax/classDiagram.html#syntax"
+```
+
+<p align="center">
+    <img src="examples/images/code_commit_diagram.png">
+</p>
+
+<br>
+
+**_Example Function: Using `notion.Workspace()` to retrieve a user, and appending blocks in a page to mention user/date._**
+
+```py
+def inline_mention(page: notion.Page, message: str, user_name: str) -> None:
+    mentionblock = notion.Block.paragraph(
         page,
         [
             prop.Mention.user(
                 notion.Workspace().retrieve_user(user_name=user_name),
                 annotations=prop.Annotations(
                     code=True, bold=True, color=prop.BlockColor.purple
                 ),
             ),
             prop.RichText(" - "),
             prop.Mention.date(
-                datetime.now().astimezone(target_page.tz).isoformat(),
+                datetime.now().astimezone(page.tz).isoformat(),
                 annotations=prop.Annotations(
-                    code=True, bold=True, color=prop.BlockColor.purple_background
+                    code=True,
+                    bold=True,
+                    italic=True,
+                    underline=True,
+                    color=prop.BlockColor.gray,
                 ),
             ),
             prop.RichText(":"),
         ],
     )
     # First method returned the newly created block that we append to here:
-    notion.BlockFactory.paragraph(mentionblock, [prop.RichText(message)])
-    notion.BlockFactory.divider(page)
+    notion.Block.paragraph(mentionblock, [prop.RichText(message)])
+    notion.Block.divider(page)
 ```
 
 ```py
->>> my_page = notion.Page("0b9eccfa890e4c3390175ee10c664a35")
->>> in_block_reminder(page=my_page, message="message here", user_name="Your Name")
+>>> homepage = notion.Page("0b9eccfa890e4c3390175ee10c664a35")
+>>> inline_mention(page=homepage, message="example", user_name="AYVI")
 ```
 <p align="center">
     <img src="examples/images/example_function_reminder.png">
 </p>
 
 <br>
 
 ## Add, Set, & Delete: Page property values | Database property objects
 
-The first argument for all database column methods is the name of the property,  
-If it does not exist, then a new property object is created.  
-If it already exists, then the method will overwrite it.
-
-If the name passed already exists, but it's a different column type than the method used - then the API will overwrite this and change the property object to the new column type.  
+The first argument for all database property methods is the name of the property,  
+If a property of that name does not exist, then a new property will be created. 
+If a property of that name already exists, but it's a different type than the method used - then the API will overwrite this and change the property object to the new type.  
 The original parameters will be saved if you decide to switch back (i.e. if you change a formula column to a select column, upon changing it back to a formula column, the original formula expression will still be there).   
 
 ```py
 new_database.formula_column("page id", expression="id()")
 
 new_database.delete_property("url")
 
@@ -221,16 +258,19 @@
 new_page.set_multiselect("options", ["option-a", "option-b"])
 ```
 
 <br>
 
 ## Database Queries
 
-A single `notion.query.propfilter.PropertyFilter` is equivalent to filtering one property type in Notion.
-To build filters equivalent to Notion's 'advanced filters', use `notion.query.compound.CompoundFilter`.
+A single `notion.query.PropertyFilter` is equivalent to filtering one property type in Notion.
+To build filters equivalent to Notion's 'advanced filters', use `notion.query.CompoundFilter`.
+
+The database method `query()` will return the raw response from the API.  
+The method `query_pages()` will extract the page ID for each object in the array of results, and return a list of `notion.Page` objects.
 
 ```py
 from datetime import datetime
 from datetime import timedelta
 
 from notion import query
 
@@ -257,16 +297,14 @@
     filter=query_filter,
     sort=query_sort,
     page_size=5,
     filter_property_values=["name", "options"],
 )
 ```
 
-A database also has the `query_pages()` method. It takes the same parameters, but for each page object in the `results` array, it retrieves the id(s), and instead returns a list of `notion.Page`.
-
 <br>
 
 ## Exceptions & Validating Responses
 
 Errors in Notion requests return an object with the keys: 'object', 'status', 'code', and 'message'.
 Exceptions are raised by matching the error code and returning the message. For example:
```

### Comparing `notion_api-0.4.2/notion/__init__.py` & `notion_api-0.5.0/notion/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,30 +15,56 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+
 """ 
-### Properties:
->>> from notion import properties as prop
+#### Main Objects:
+>>> notion.Page | notion.Database | notion.Block | notion.Workspace
 
-### PropertyItems:
+#### PropertyItems:
 >>> from notion import propertyitems
 
-### Queries:
+#### Queries:
 >>> from notion import query
+
+#### Properties:
+>>> from notion import properties as prop
+
+#### Block Extensions:
+>>> notion.CodeBlock | notion.ToDoBlock | notion.EquationBlock | notion.ParagraphBlock
+
+---
+
+Uncomment `check_for_pkg_update` method to enable auto-update check.
+
 """
 from typing import Sequence
 
-from notion.api import Block, BlockFactory, Database, Page, Workspace
-from notion.api._pkgv import inspect_pkg_version
+from notion.api import Block, Database, Page, Workspace
+from notion.api._pkgv import check_for_pkg_update
+from notion.api.block_ext import (
+    CodeBlock,
+    EquationBlock,
+    RichTextBlock,
+    TableBlock,
+    ToDoBlock,
+)
+
+# check_for_pkg_update()
+
 
 __all__: Sequence[str] = (
     "Page",
     "Database",
     "Block",
     "Workspace",
-    "BlockFactory",
-    "inspect_pkg_version",
+    "CodeBlock",
+    "EquationBlock",
+    "ToDoBlock",
+    "RichTextBlock",
+    "TableBlock",
+    "check_for_pkg_update",
 )
```

### Comparing `notion_api-0.4.2/notion/api/__init__.py` & `notion_api-0.5.0/notion/api/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,20 +18,18 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from typing import Sequence
 
-from notion.api.blocktypefactory import BlockFactory
 from notion.api.notionblock import Block
 from notion.api.notiondatabase import Database
 from notion.api.notionpage import Page
 from notion.api.notionworkspace import Workspace
 
 __all__: Sequence[str] = (
     "Workspace",
     "Block",
     "Page",
     "Database",
-    "BlockFactory",
 )
```

### Comparing `notion_api-0.4.2/notion/api/_about.py` & `notion_api-0.5.0/notion/api/_about.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "__package_url__",
     "__package_json__",
 )
 
 __notion_version__: Final[str] = "2022-06-28"
 __content_type__: Final[str] = "application/json"
 __base_url__: Final[str] = "https://api.notion.com/v1/"
-__version__: Final[str] = "0.4.2"
+__version__: Final[str] = "0.5.0"
 __package_url__: Final[str] = "https://pypi.org/pypi/notion-api/"
 __package_json__: Final[str] = "https://pypi.org/pypi/notion-api/json"
 
 
 # Notion API Changlog
 # https://developers.notion.com/page/changelog
```

### Comparing `notion_api-0.4.2/notion/api/blockmixin.py` & `notion_api-0.5.0/notion/api/blockmixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,16 @@
 
     @cached_property
     def _block(self) -> MutableMapping[str, Any]:
         """
         Same result as retrieve() for notion.api.notionblock.Block.
         If used with notion.api.notionpage.Page or notion.api.notiondatabase.Database,
         retrieves the page or database object from the blocks endpoint.
+
+        https://developers.notion.com/reference/block#block-type-objects
         """
         return self._get(self._block_endpoint(self.id))
 
     @property
     def type(self) -> str:
         return cast(str, self._block["type"])
```

### Comparing `notion_api-0.4.2/notion/api/client.py` & `notion_api-0.5.0/notion/api/client.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.2/notion/api/notiondatabase.py` & `notion_api-0.5.0/notion/api/notiondatabase.py`

 * *Files 2% similar despite different names*

```diff
@@ -376,35 +376,32 @@
         return self._post(url, payload=payload)
 
     def query_pages(
         self,
         *,
         filter: Optional[Union[CompoundFilter, PropertyFilter, TimestampFilter]] = None,
         sort: Optional[SortFilter] = None,
-        filter_property_values: Optional[list[str]] = None,
         page_size: Optional[int] = 100,
         start_cursor: Optional[str] = None,
     ) -> list[Page]:
         """
         :return: list of notion.Page objects
 
         :param filter: (optional) notion.query.compound.CompoundFilter or notion.query.propfilter.PropertyFilter
         :param sort: (optional) notion.query.sort.SortFilter
         :param page_size: (optional) The number of items from the full list desired in the response.\
                            Default: 100 page_size Maximum: 100.
         :param start_cursor: (optional) When supplied, returns a page of results starting after the cursor provided.\
                               If not supplied, this endpoint will return the first page of results.
-        :param filter_property_values: (optional) Return only the selected properties.
 
         https://developers.notion.com/reference/post-database-query
         """
         query = self.query(
             filter=filter,
             sort=sort,
-            filter_property_values=filter_property_values,
             page_size=page_size,
             start_cursor=start_cursor,
         )
 
         from notion.api.notionpage import Page
 
         return [Page(_object["id"]) for _object in query.get("results", [])]
@@ -605,15 +602,15 @@
         """Creates a `Files` property.
 
         https://developers.notion.com/reference/property-object#files
         """
         self._update(Properties(FilesPropertyObject(property_name)))
 
     def email_column(self, property_name: str, /) -> None:
-        """Creates a `Email` property.
+        """Creates an `Email` property.
 
         https://developers.notion.com/reference/property-object#email
         """
         self._update(Properties(EmailPropertyObject(property_name)))
 
     def url_column(self, property_name: str, /) -> None:
         """Creates a `URL` property.
```

### Comparing `notion_api-0.4.2/notion/api/notionpage.py` & `notion_api-0.5.0/notion/api/notionpage.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         *,
         cover_url: Optional[str] = None,
         icon_url: Optional[str] = None,
     ) -> Page:
         """
         Creates a blank page.
         Use Page methods to add values to properties described in parent database schema.
-        Add content to page by appending block children with notion.api.blocktypefactory.BlockFactory.
+        Add content to page by appending block children with `notion.Block`.
 
         ---
         :param parent_instance: (required) Either a Page or Database instance.
         :param page_title: (required) Title of page.
         :param cover_url: (optional) Url of image to use as cover.
         :param icon_url: (optional) Url of image to use as icon.
 
@@ -320,19 +320,15 @@
         return self._get(
             self._block_endpoint(
                 self.id, children=True, page_size=page_size, start_cursor=start_cursor
             )
         )
 
     def _append(self, payload: MutableMapping[str, Any]) -> MutableMapping[str, Any]:
-        """
-        Used internally by notion.api.blocktypefactory.BlockFactory.
-
-        https://developers.notion.com/reference/patch-block-children
-        """
+        """https://developers.notion.com/reference/patch-block-children"""
         return self._patch(self._block_endpoint(self.id, children=True), payload=payload)
 
     def set_select(self, property_name: str, /, select_option: str) -> None:
         """
         :param select_option: (required) If the option already exists, then it is case sensitive.\
                                If the option does not exist, it will be created.
```

### Comparing `notion_api-0.4.2/notion/api/notionworkspace.py` & `notion_api-0.5.0/notion/api/notionworkspace.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.2/notion/exceptions/__init__.py` & `notion_api-0.5.0/notion/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.2/notion/exceptions/errors.py` & `notion_api-0.5.0/notion/exceptions/errors.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.2/notion/exceptions/validate.py` & `notion_api-0.5.0/notion/exceptions/validate.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.2/notion/properties/__init__.py` & `notion_api-0.5.0/notion/query/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,15 +16,36 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from notion.properties.blocktypes import *
-from notion.properties.build import *
-from notion.properties.common import *
-from notion.properties.files import *
-from notion.properties.options import *
-from notion.properties.propertyobjects import *
-from notion.properties.propertyvalues import *
-from notion.properties.richtext import *
+""" 
+https://developers.notion.com/reference/post-database-query 
+
+notion.query.PropertyFilter && notion.query.TimestampFilter for individual filters as used in Notion UI.
+
+notion.query.CompoundFilter to combine filters.
+    :method: _and(): combine all filters in an and grouping.
+    :method: _or(): combine all filters in an or grouping.
+
+    Create a separate CompoundFilter object to nest an and/or operator inside another and/or.
+
+notion.query.SortFilter takes a list of either *notion.query.PropertyValueSort | notion.query.EntryTimestampSort
+"""
+from typing import Sequence
+
+from notion.query.compound import *
+from notion.query.conditions import *
+from notion.query.propfilter import *
+from notion.query.sort import *
+from notion.query.timestamp import *
+
+__all__: Sequence[str] = (
+    "SortFilter",
+    "PropertyFilter",
+    "CompoundFilter",
+    "TimestampFilter",
+    "EntryTimestampSort",
+    "PropertyValueSort",
+)
```

### Comparing `notion_api-0.4.2/notion/properties/blocktypes.py` & `notion_api-0.5.0/notion/properties/blocktypes.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,23 +16,21 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from typing import Optional, Sequence, Union
+from typing import Any, Collection, MutableMapping, Optional, Sequence, Union
 
 from notion.properties.build import NotionObject
 from notion.properties.common import _NotionURL
 from notion.properties.files import ExternalFile
 from notion.properties.options import BlockColor, CodeBlockLang
-from notion.properties.richtext import Equation, Mention, RichText
-
-# See docs in `notion.api.blockwrite.BlockFactory` for more info on block types.
+from notion.properties.richtext import Mention, RichText
 
 __all__: Sequence[str] = (
     "BlockChildren",
     "OriginalSyncedBlockType",
     "DuplicateSyncedBlockType",
     "ParagraphBlocktype",
     "NewLineBreak",
@@ -49,23 +47,30 @@
     "TableOfContentsBlocktype",
     "DividerBlock",
     "BreadcrumbBlock",
     "Heading1BlockType",
     "Heading2BlockType",
     "Heading3BlockType",
     "LinkToPageBlockType",
+    "VideoBlockType",
+    "ImageBlockType",
+    "ColumnListBlockType",
+    "TableBlockType",
+    "TableRowBlockType",
 )
 
 
 class BlockChildren(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
-        block_type_objects_array: Optional[list[NotionObject]] = None,
+        block_type_objects_array: Optional[
+            Sequence[NotionObject | MutableMapping[str, Any]]
+        ] = None,
     ) -> None:
         """https://developers.notion.com/reference/block"""
         super().__init__()
         if not block_type_objects_array:
             block_type_objects_array = []
 
         self.set("children", block_type_objects_array)
@@ -97,15 +102,15 @@
 
 
 class ParagraphBlocktype(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
-        rich_text: Sequence[Union[RichText, Mention, Equation]],
+        rich_text: Sequence[RichText | Mention],
         /,
         *,
         block_color: Optional[Union[BlockColor, str]] = None,
     ) -> None:
         """https://developers.notion.com/reference/block#paragraph"""
         super().__init__()
         if not block_color:
@@ -120,15 +125,15 @@
 
 
 class CalloutBlocktype(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
-        rich_text: Sequence[Union[RichText, Mention, Equation]],
+        rich_text: Sequence[RichText | Mention],
         /,
         *,
         icon: Optional[str] = None,
         block_color: Optional[Union[BlockColor, str]] = None,
     ) -> None:
         """https://developers.notion.com/reference/block#callout"""
         super().__init__()
@@ -143,15 +148,15 @@
 
 
 class QuoteBlocktype(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
-        rich_text: Sequence[Union[RichText, Mention, Equation]],
+        rich_text: Sequence[RichText | Mention],
         /,
         *,
         block_color: Optional[Union[BlockColor, str]] = None,
     ) -> None:
         """https://developers.notion.com/reference/block#quote"""
         super().__init__()
         if not block_color:
@@ -163,15 +168,15 @@
 
 
 class BulletedListItemBlocktype(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
-        rich_text: Sequence[Union[RichText, Mention, Equation]],
+        rich_text: Sequence[RichText | Mention],
         /,
         *,
         block_color: Optional[Union[BlockColor, str]] = None,
     ) -> None:
         """https://developers.notion.com/reference/block#bulleted-list-item"""
         super().__init__()
         if not block_color:
@@ -183,15 +188,15 @@
 
 
 class NumberedListItemBlocktype(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
-        rich_text: Sequence[Union[RichText, Mention, Equation]],
+        rich_text: Sequence[RichText | Mention],
         /,
         *,
         block_color: Optional[Union[BlockColor, str]] = None,
     ) -> None:
         """https://developers.notion.com/reference/block#numbered-list-item"""
         super().__init__()
         if not block_color:
@@ -203,15 +208,15 @@
 
 
 class ToDoBlocktype(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
-        rich_text: Sequence[Union[RichText, Mention, Equation]],
+        rich_text: Sequence[RichText | Mention],
         /,
         *,
         checked: Optional[bool] = False,
         block_color: Optional[Union[BlockColor, str]] = None,
     ) -> None:
         """https://developers.notion.com/reference/block#to-do"""
         super().__init__()
@@ -225,15 +230,15 @@
 
 
 class ToggleBlocktype(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
-        rich_text: Sequence[Union[RichText, Mention, Equation]],
+        rich_text: Sequence[RichText | Mention],
         /,
         *,
         block_color: Optional[Union[BlockColor, str]] = None,
     ) -> None:
         """https://developers.notion.com/reference/block#toggle-blocks"""
         super().__init__()
         if not block_color:
@@ -245,25 +250,28 @@
 
 
 class CodeBlocktype(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
-        rich_text: Sequence[Union[RichText, Mention, Equation]],
+        rich_text: Optional[Sequence[RichText | Mention]] = None,
         /,
         *,
         language: Optional[Union[CodeBlockLang, str]] = None,
-        caption: Optional[Sequence[Union[RichText, Mention, Equation]]] = None,
+        caption: Optional[Sequence[RichText | Mention | str]] = None,
     ) -> None:
         """https://developers.notion.com/reference/block#code"""
         super().__init__()
         if not language:
             language = CodeBlockLang.plain_text.value
 
+        if not rich_text:
+            rich_text = [RichText("")]
+
         self.set("type", "code")
         self.nest("code", "rich_text", rich_text)
         self.nest("code", "language", language)
         self.nest("code", "caption", caption) if caption else None
 
 
 class EmbedBlocktype(NotionObject):
@@ -280,15 +288,15 @@
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
         bookmark_url: str,
         /,
         *,
-        caption: Optional[Sequence[Union[RichText, Mention, Equation]]] = None,
+        caption: Optional[Sequence[RichText | Mention]] = None,
     ) -> None:
         """https://developers.notion.com/reference/block#bookmark"""
         super().__init__()
         self.set("type", "bookmark")
         self.set("bookmark", _NotionURL(bookmark_url))
         self.nest("bookmark", "caption", caption) if caption else None
 
@@ -317,15 +325,15 @@
 
 
 class Heading1BlockType(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
-        rich_text: Sequence[Union[RichText, Mention, Equation]],
+        rich_text: Sequence[RichText | Mention],
         /,
         *,
         block_color: Optional[Union[BlockColor, str]] = None,
         is_toggleable: Optional[bool] = False,
     ) -> None:
         """https://developers.notion.com/reference/block#headings"""
         super().__init__()
@@ -339,15 +347,15 @@
 
 
 class Heading2BlockType(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
-        rich_text: Sequence[Union[RichText, Mention, Equation]],
+        rich_text: Sequence[RichText | Mention],
         /,
         *,
         block_color: Optional[Union[BlockColor, str]] = None,
         is_toggleable: Optional[bool] = False,
     ) -> None:
         """https://developers.notion.com/reference/block#headings"""
         super().__init__()
@@ -361,15 +369,15 @@
 
 
 class Heading3BlockType(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
-        rich_text: Sequence[Union[RichText, Mention, Equation]],
+        rich_text: Sequence[RichText | Mention],
         /,
         *,
         block_color: Optional[Union[BlockColor, str]] = None,
         is_toggleable: Optional[bool] = False,
     ) -> None:
         """https://developers.notion.com/reference/block#headings"""
         super().__init__()
@@ -407,7 +415,59 @@
     __slots__: Sequence[str] = ()
 
     def __init__(self) -> None:
         """https://developers.notion.com/reference/block#divider"""
         super().__init__()
         self.set("type", "divider")
         self.set("divider", {})
+
+
+class VideoBlockType(NotionObject):
+    __slots__: Sequence[str] = ()
+
+    def __init__(self, url: str) -> None:
+        """https://developers.notion.com/reference/block#video"""
+        super().__init__()
+        self.set("type", "video")
+        self.set("video", ExternalFile(url))
+
+
+class ImageBlockType(NotionObject):
+    __slots__: Sequence[str] = ()
+
+    def __init__(self, url: str) -> None:
+        """https://developers.notion.com/reference/block#image"""
+        super().__init__()
+        self.set("type", "image")
+        self.set("image", ExternalFile(url))
+
+
+class TableBlockType(NotionObject):
+    __slots__: Sequence[str] = ()
+
+    def __init__(
+        self,
+        table_width: int | None = None,
+        has_column_header: bool | None = None,
+        has_row_header: bool | None = None,
+        children: Sequence[NotionObject | MutableMapping[str, Any]] | None = None,
+    ) -> None:
+        """https://developers.notion.com/reference/block#table"""
+        super().__init__()
+        self.set("type", "table")
+        self.nest("table", "table_width", table_width)
+        self.nest("table", "has_column_header", has_column_header)
+        self.nest("table", "has_row_header", has_row_header)
+        self.nest("table", "children", children)
+
+
+class TableRowBlockType(NotionObject):
+    __slots__: Sequence[str] = ()
+
+    def __init__(
+        self,
+        cells: Sequence[list[dict[str, Collection[str]]]] | None = None,
+    ) -> None:
+        """https://developers.notion.com/reference/block#table-rows"""
+        super().__init__()
+        self.set("type", "table_row")
+        self.nest("table_row", "cells", cells)
```

### Comparing `notion_api-0.4.2/notion/properties/build.py` & `notion_api-0.5.0/notion/properties/build.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.2/notion/properties/common.py` & `notion_api-0.5.0/notion/properties/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,14 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-""" 
-A page with a workspace parent is a top-level page within a Notion workspace. 
-https://developers.notion.com/reference/parent-object#workspace-parent
-
-Cannot create pages/databases at the top-level via the API.
-"""
 from __future__ import annotations
 
 from typing import Any, Optional, Sequence
 
 from notion.properties.build import NotionObject
 
 __all__: Sequence[str] = (
@@ -50,14 +44,18 @@
         Parent information is represented by a consistent parent object throughout the API.
 
         Parenting rules:
          - Pages can be parented by other pages, databases, blocks, or by the whole workspace.
          - Blocks can be parented by pages, databases, or blocks.
          - Databases can be parented by pages, blocks, or by the whole workspace.
 
+        A page with a workspace parent is a top-level page within a Notion workspace.
+        https://developers.notion.com/reference/parent-object#workspace-parent
+        Cannot create pages/databases at the top-level via the API.
+
         https://developers.notion.com/reference/parent-object
         """
         super().__init__()
         self.nest("parent", "type", type)
         self.nest("parent", type, id)
 
     @classmethod
@@ -114,15 +112,15 @@
         page property context, and the bot has the correct capabilities to access those properties.
 
         If your integration doesn't yet have access to the mentioned user,
         then the plain_text that would include a user's name reads as "@Anonymous".
         To update the integration to get access to the user,
         update the integration capabilities on the integration settings page.
 
-        All parameters are display-only and cannot be updated in Notion.
+        All parameters are display-only and cannot be updated.
 
         https://developers.notion.com/reference/user
         """
         super().__init__()
         self.set("object", "user")
         self.set("id", id)
         self.set("name", name) if name else None
```

### Comparing `notion_api-0.4.2/notion/properties/files.py` & `notion_api-0.5.0/notion/properties/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
         url: str,
         /,
         *,
-        caption: Optional[Sequence[Union[RichText, Mention, Equation]]] = None,
+        caption: Optional[Sequence[RichText | Mention]] = None,
     ) -> None:
         """
         The Notion API supports adding, retrieving, and updating links to external files.
         For "external" file objects, the name is the same as the file's host URL.
 
         https://developers.notion.com/reference/file-object#external-files
         """
@@ -122,15 +122,15 @@
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
         name: str,
         url: str,
         *,
-        caption: Optional[Sequence[Union[RichText, Mention, Equation]]] = None,
+        caption: Optional[Sequence[RichText | Mention]] = None,
     ) -> None:
         """
         Internal files are any files hosted on Notion
         They begin with: https://s3.us-west-2.amazonaws.com/secure.notion-static.com/{block_id}/...
         You can retrieve links to Notion-hosted files via the Retrieve block children endpoint.
 
         https://developers.notion.com/reference/file-object#notion-hosted-files
```

### Comparing `notion_api-0.4.2/notion/properties/options.py` & `notion_api-0.5.0/notion/properties/options.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.2/notion/properties/propertyobjects.py` & `notion_api-0.5.0/notion/properties/propertyobjects.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.2/notion/properties/propertyvalues.py` & `notion_api-0.5.0/notion/properties/propertyvalues.py`

 * *Files 7% similar despite different names*

```diff
@@ -111,50 +111,23 @@
 class RichTextPropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
     def __init__(
         self,
         property_name: str,
         /,
-        rich_text: Sequence[Union[RichText, Mention, Equation]],
+        rich_text: Sequence[RichText | Mention],
     ) -> None:
-        r"""
+        """
         The purpose of the rich text property value is to provide the key `rich_text`,
         whereas the object `notion.properties.RichText` has the key `text`.
 
-        ---
         :param rich_text: (required) An array of rich text objects.
-        Using `shift+enter` for multi-line text blocks results in a separate `text` key with a newline escape.
-        ```json
-        },  // ... first text line above
-        {
-            "type": "text",
-            "text": {
-                "content": "\nthis is the second line of a block"
-            }
-        }
-        ```
-        ---
-        If you hyperlink only part of a string in Notion,
-        the string will be split and return as separate keys in the rich text object.
-        Hyperlinking text to an internal Notion link will populate link/href
-        with the UUID's following notion.so/{workspace name}/...
-        ```json
-        {
-            "type": "text",
-            "text": {
-                "content": "hyperlink in text to notion link\n",
-                "link": {
-                    "url": "/3a2ec1e9308b4fd5a5749a5ee5aeeff9?v=f19121cb8e6f4329aba62edef93c39dc&p=bc5d3abdf3a942e0b6a7d8a5c94b5dc9&pm=s"
-                }          // database id // database view id // database page id
-        },
-        ```
 
         The RichText Object: https://developers.notion.com/reference/rich-text
-
         The RichText Property Value: https://developers.notion.com/reference/page-property-values#rich-text
         """
         super().__init__(property_name=property_name)
         self.set("type", "rich_text")
         self.set("rich_text", rich_text)
```

### Comparing `notion_api-0.4.2/notion/properties/richtext.py` & `notion_api-0.5.0/notion/properties/richtext.py`

 * *Files 5% similar despite different names*

```diff
@@ -208,25 +208,21 @@
 class Annotations(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
         bold: Optional[bool] = None,
         italic: Optional[bool] = None,
-        strike: Optional[bool] = None,
+        strikethrough: Optional[bool] = None,
         underline: Optional[bool] = None,
         code: Optional[bool] = None,
         color: Union[Optional[BlockColor], str] = None,
     ) -> None:
         """https://developers.notion.com/reference/rich-text#the-annotation-object"""
         super().__init__()
 
         self.set("bold", bold) if bold else None
         self.set("italic", italic) if italic else None
-        self.set("strike", strike) if strike else None
+        self.set("strikethrough", strikethrough) if strikethrough else None
         self.set("underline", underline) if underline else None
         self.set("code", code) if code else None
-
         self.set("color", color) if color else None
-
-        if not any([[bold, italic, strike, underline, code, color]]):
-            pass
```

### Comparing `notion_api-0.4.2/notion/propertyitems/__init__.py` & `notion_api-0.5.0/notion/propertyitems/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.2/notion/propertyitems/base.py` & `notion_api-0.5.0/notion/propertyitems/base.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.2/notion/propertyitems/call.py` & `notion_api-0.5.0/notion/propertyitems/call.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,16 +221,16 @@
     """:returns: The result of the rollup. The rollup property must return a number."""
     _assert_property_type(property, "rollup")
     if (func := _function_type(property)) in NOT_IMPLEMENTED_FUNCTIONS:
         raise NOT_IMPLEMENTED_ERR(func)
 
     if property.map["property_item"]["rollup"]["type"] == "number":
         return cast(float, property.map["property_item"]["rollup"]["number"])
-    else:
-        raise TypeError("rollup type is not number.")
+
+    raise TypeError("rollup type is not number.")
 
 
 def date_rollup(property: T_PropertyItem) -> datetime | tuple[datetime, datetime]:
     """ 
     :returns: The result of the rollup. The rollup property must return a date.\
               If the rollup is a date range, a tuple of (start, end) is returned.\
               Otherwise, a single datetime is returned.
```

### Comparing `notion_api-0.4.2/notion/query/__init__.py` & `notion_api-0.5.0/notion/query/compound.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,36 +16,52 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-""" 
-https://developers.notion.com/reference/post-database-query 
+from __future__ import annotations
 
-notion.query.PropertyFilter && notion.query.TimestampFilter for individual filters as used in Notion UI.
+from typing import Sequence, Union
 
-notion.query.CompoundFilter to combine filters.
-    :method: _and(): combine all filters in an and grouping.
-    :method: _or(): combine all filters in an or grouping.
-
-    Create a separate CompoundFilter object to nest an and/or operator inside another and/or.
-
-notion.query.SortFilter takes a list of either *notion.query.PropertyValueSort | notion.query.EntryTimestampSort
-"""
-from typing import Sequence
-
-from notion.query.compound import *
-from notion.query.conditions import *
-from notion.query.propfilter import *
-from notion.query.sort import *
-from notion.query.timestamp import *
-
-__all__: Sequence[str] = (
-    "SortFilter",
-    "PropertyFilter",
-    "CompoundFilter",
-    "TimestampFilter",
-    "EntryTimestampSort",
-    "PropertyValueSort",
-)
+from notion.properties.build import NotionObject
+from notion.query.propfilter import PropertyFilter
+from notion.query.timestamp import TimestampFilter
+
+__all__: Sequence[str] = ["CompoundFilter"]
+
+
+class CompoundFilter(NotionObject):
+    __slots__: Sequence[str] = ()
+
+    def __init__(self) -> None:
+        """NOTE: only up to two nesting levels deep.
+
+        :method: _and() combine all filters in an `and` grouping.
+        :method: _or() combine all filters in an `or` grouping.
+
+        Create a separate CompoundFilter object to nest an `and` operator inside another `and` or `or`.
+
+        https://developers.notion.com/reference/post-database-query-filter#compound-filter-object
+        """
+        super().__init__()
+
+    def _and(
+        self, *filters: Union[PropertyFilter, CompoundFilter, TimestampFilter]
+    ) -> CompoundFilter:
+        """
+        Example compound filter conditions
+        https://developers.notion.com/reference/post-database-query-filter#example-compound-filter-conditions
+        """
+        self.nest("filter", "and", [f["filter"] if "filter" in f else f for f in filters])
+        return self
+
+    def _or(
+        self, *filters: Union[PropertyFilter, CompoundFilter, TimestampFilter]
+    ) -> CompoundFilter:
+        """
+        Example compound filter conditions
+        https://developers.notion.com/reference/post-database-query-filter#example-compound-filter-conditions
+        """
+        self.nest("filter", "or", [f["filter"] if "filter" in f else f for f in filters])
+        return self
```

### Comparing `notion_api-0.4.2/notion/query/compound.py` & `notion_api-0.5.0/notion/api/block_ext/equation.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,52 +16,32 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from __future__ import annotations
+from typing import Optional, Sequence, cast
 
-from typing import Sequence, Union
+from notion.api.blockmixin import _TokenBlockMixin
 
-from notion.properties.build import NotionObject
-from notion.query.propfilter import PropertyFilter
-from notion.query.timestamp import TimestampFilter
-
-__all__: Sequence[str] = ["CompoundFilter"]
-
-
-class CompoundFilter(NotionObject):
-    __slots__: Sequence[str] = ()
-
-    def __init__(self) -> None:
-        """NOTE: only up to two nesting levels deep.
-
-        :method: _and() combine all filters in an `and` grouping.
-        :method: _or() combine all filters in an `or` grouping.
-
-        Create a separate CompoundFilter object to nest an `and` operator inside another `and` or `or`.
-
-        https://developers.notion.com/reference/post-database-query-filter#compound-filter-object
-        """
-        super().__init__()
-
-    def _and(
-        self, *filters: Union[PropertyFilter, CompoundFilter, TimestampFilter]
-    ) -> CompoundFilter:
-        """
-        Example compound filter conditions
-        https://developers.notion.com/reference/post-database-query-filter#example-compound-filter-conditions
-        """
-        self.nest("filter", "and", [f["filter"] if "filter" in f else f for f in filters])
-        return self
-
-    def _or(
-        self, *filters: Union[PropertyFilter, CompoundFilter, TimestampFilter]
-    ) -> CompoundFilter:
-        """
-        Example compound filter conditions
-        https://developers.notion.com/reference/post-database-query-filter#example-compound-filter-conditions
-        """
-        self.nest("filter", "or", [f["filter"] if "filter" in f else f for f in filters])
-        return self
+__all__: Sequence[str] = ["EquationBlock"]
+
+
+class EquationBlock(_TokenBlockMixin):
+    def __init__(self, id: str, /, *, token: Optional[str] = None) -> None:
+        super().__init__(id, token=token)
+
+        if self.type != "equation":
+            raise TypeError(
+                f"Block type must be 'equation', not '{self.type}' for EquationBlock."
+            )
+
+    @property
+    def expression(self) -> str:
+        return cast(str, self._block["equation"]["expression"])
+
+    @expression.setter
+    def expression(self, value: str) -> None:
+        equation = self._block["equation"]
+        equation["expression"] = value
+        self._patch(self._block_endpoint(self.id), payload={self.type: equation})
```

### Comparing `notion_api-0.4.2/notion/query/conditions.py` & `notion_api-0.5.0/notion/query/conditions.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.2/notion/query/propfilter.py` & `notion_api-0.5.0/notion/query/propfilter.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,16 +156,14 @@
         property_name: str,
         property_type: DateTypes,
         filter_condition: DateConditions,
         filter_value: Union[str, bool, dict[str, Any], datetime],
         /,
     ) -> PropertyFilter:
         """
-        When selecting any DateCondition containing `past`, `this`, or `next`, set filter value to `{}`
-
         :param filter_value: - When selecting any DateCondition containing `past`, `this`, or `next`, set filter value to `{}`\
                              - If value is datetime, it will be converted to ISO 8601 format.
 
         https://developers.notion.com/reference/post-database-query-filter#date
         """
         if isinstance(filter_value, datetime):
             filter_value = filter_value.isoformat()
```

### Comparing `notion_api-0.4.2/notion/query/sort.py` & `notion_api-0.5.0/notion/query/sort.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.2/notion/query/timestamp.py` & `notion_api-0.5.0/notion/query/timestamp.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.2/.gitignore` & `notion_api-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.2/LICENSE` & `notion_api-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `notion_api-0.4.2/pyproject.toml` & `notion_api-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -96,11 +96,7 @@
 show_error_codes = true
 incremental = true
 disallow_untyped_defs = true
 show_column_numbers = true
 show_error_context = true
 allow_redefinition = true
 disable_error_code = "no-redef"
-
-[[tool.mypy.overrides]]
-module = ["notion.api.blocktypefactory"]
-disable_error_code = ["empty-body", "type-arg"]
```

### Comparing `notion_api-0.4.2/PKG-INFO` & `notion_api-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6e6f 7469  : 2.1.Name: noti
 00000020: 6f6e 2d61 7069 0a56 6572 7369 6f6e 3a20  on-api.Version: 
-00000030: 302e 342e 320a 5375 6d6d 6172 793a 2041  0.4.2.Summary: A
+00000030: 302e 352e 300a 5375 6d6d 6172 793a 2041  0.5.0.Summary: A
 00000040: 6e20 756e 6f66 6669 6369 616c 2077 7261  n unofficial wra
 00000050: 7070 6572 2066 6f72 204e 6f74 696f 6e27  pper for Notion'
 00000060: 7320 4150 492c 2061 696d 696e 6720 746f  s API, aiming to
 00000070: 2073 696d 706c 6966 7920 7468 6520 6479   simplify the dy
 00000080: 6e61 6d69 6320 6e61 7475 7265 206f 6620  namic nature of 
 00000090: 696e 7465 7261 6374 696e 6720 7769 7468  interacting with
 000000a0: 204e 6f74 696f 6e2e 0a50 726f 6a65 6374   Notion..Project
@@ -177,619 +177,715 @@
 00000b00: 6974 6820 4e6f 7469 6f6e 2e73 6f5f 5f20  ith Notion.so__ 
 00000b10: 200a 0a41 2077 7261 7070 6572 2066 6f72   ..A wrapper for
 00000b20: 204e 6f74 696f 6e27 7320 4150 492c 2061   Notion's API, a
 00000b30: 696d 696e 6720 746f 2073 696d 706c 6966  iming to simplif
 00000b40: 7920 7468 6520 6479 6e61 6d69 6320 6e61  y the dynamic na
 00000b50: 7475 7265 206f 6620 696e 7465 7261 6374  ture of interact
 00000b60: 696e 6720 7769 7468 204e 6f74 696f 6e2e  ing with Notion.
-00000b70: 2054 6869 7320 7072 6f6a 6563 7420 6973   This project is
-00000b80: 2073 7469 6c6c 2061 2077 6f72 6b20 696e   still a work in
-00000b90: 2070 726f 6772 6573 732c 2061 6e64 2066   progress, and f
-00000ba0: 6561 7475 7265 7320 7769 6c6c 2063 6f6e  eatures will con
-00000bb0: 7469 6e75 6520 746f 2063 6861 6e67 652e  tinue to change.
-00000bc0: 2042 656c 6f77 2061 7265 2061 2066 6577   Below are a few
-00000bd0: 2065 7861 6d70 6c65 7320 6f66 2074 6865   examples of the
-00000be0: 2063 7572 7265 6e74 2066 756e 6374 696f   current functio
-00000bf0: 6e61 6c69 7479 2e20 0a0a 3c62 723e 0a0a  nality. ..<br>..
-00000c00: 3c64 6976 2062 6f72 6465 723d 2230 2220  <div border="0" 
-00000c10: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-00000c20: 2020 2020 3c74 6162 6c65 3e0a 2020 2020      <table>.    
-00000c30: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
-00000c40: 2020 2020 203c 7464 2061 6c69 676e 3d22       <td align="
-00000c50: 6365 6e74 6572 223e 3c62 3e4c 696e 6b73  center"><b>Links
-00000c60: 3a20 4e6f 7469 6f6e 2041 5049 2055 7064  : Notion API Upd
-00000c70: 6174 6573 3c2f 623e 3c2f 7464 3e0a 2020  ates</b></td>.  
-00000c80: 2020 2020 2020 3c2f 7472 3e0a 2020 2020        </tr>.    
-00000c90: 2020 2020 2020 2020 3c74 643e 203c 6120          <td> <a 
-00000ca0: 6872 6566 3d22 6874 7470 733a 2f2f 6465  href="https://de
-00000cb0: 7665 6c6f 7065 7273 2e6e 6f74 696f 6e2e  velopers.notion.
-00000cc0: 636f 6d2f 7265 6665 7265 6e63 652f 696e  com/reference/in
-00000cd0: 7472 6f22 3e41 5049 2052 6566 6572 656e  tro">API Referen
-00000ce0: 6365 3c2f 613e 3c2f 7464 3e3c 7472 3e0a  ce</a></td><tr>.
-00000cf0: 2020 2020 2020 2020 3c2f 7464 3e0a 2020          </td>.  
-00000d00: 2020 2020 2020 2020 2020 3c74 643e 3c61            <td><a
-00000d10: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
-00000d20: 6576 656c 6f70 6572 732e 6e6f 7469 6f6e  evelopers.notion
-00000d30: 2e63 6f6d 2f70 6167 652f 6368 616e 6765  .com/page/change
-00000d40: 6c6f 6722 3e4e 6f74 696f 6e20 4150 4920  log">Notion API 
-00000d50: 4368 616e 6765 6c6f 6720 3c2f 696d 673e  Changelog </img>
-00000d60: 3c2f 613e 3c2f 7472 3e0a 2020 2020 2020  </a></tr>.      
-00000d70: 2020 2020 2020 3c74 643e 203c 6120 6872        <td> <a hr
-00000d80: 6566 3d22 6874 7470 733a 2f2f 7777 772e  ef="https://www.
-00000d90: 6e6f 7469 6f6e 2e73 6f2f 7265 6c65 6173  notion.so/releas
-00000da0: 6573 223e 4e6f 7469 6f6e 2e73 6f20 5265  es">Notion.so Re
-00000db0: 6c65 6173 6573 3c2f 613e 3c2f 7464 3e3c  leases</a></td><
-00000dc0: 2f74 723e 0a20 2020 2020 2020 2020 2020  /tr>.           
-00000dd0: 203c 7464 3e20 3c61 2068 7265 663d 2268   <td> <a href="h
-00000de0: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
-00000df0: 732e 6e6f 7469 6f6e 2e63 6f6d 2f70 6167  s.notion.com/pag
-00000e00: 652f 6e6f 7469 6f6e 2d70 6c61 7466 6f72  e/notion-platfor
-00000e10: 6d2d 726f 6164 6d61 7022 3e4e 6f74 696f  m-roadmap">Notio
-00000e20: 6e20 506c 6174 666f 726d 2052 6f61 646d  n Platform Roadm
-00000e30: 6170 3c2f 613e 3c2f 7464 3e0a 2020 2020  ap</a></td>.    
-00000e40: 2020 2020 3c2f 7472 3e0a 2020 2020 3c2f      </tr>.    </
-00000e50: 7461 626c 653e 0a3c 2f64 6976 3e0a 0a2d  table>.</div>..-
-00000e60: 2d2d 0a0a 2323 2049 6e73 7461 6c6c 0a60  --..## Install.`
-00000e70: 6060 0a70 6970 2069 6e73 7461 6c6c 202d  ``.pip install -
-00000e80: 5520 6e6f 7469 6f6e 2d61 7069 0a60 6060  U notion-api.```
-00000e90: 0a0a 2323 2055 7361 6765 0a60 6060 7079  ..## Usage.```py
-00000ea0: 0a69 6d70 6f72 7420 646f 7465 6e76 0a0a  .import dotenv..
-00000eb0: 696d 706f 7274 206e 6f74 696f 6e0a 0a23  import notion..#
-00000ec0: 2063 6c69 656e 7420 7769 6c6c 2063 6865   client will che
-00000ed0: 636b 2065 6e76 2076 6172 6961 626c 6573  ck env variables
-00000ee0: 2066 6f72 2027 4e4f 5449 4f4e 5f54 4f4b   for 'NOTION_TOK
-00000ef0: 454e 270a 646f 7465 6e76 2e6c 6f61 645f  EN'.dotenv.load_
-00000f00: 646f 7465 6e76 2829 2020 0a0a 686f 6d65  dotenv()  ..home
-00000f10: 7061 6765 203d 206e 6f74 696f 6e2e 5061  page = notion.Pa
-00000f20: 6765 2827 3737 3362 3038 6666 3338 6234  ge('773b08ff38b4
-00000f30: 3435 3231 6234 3462 3131 3538 3237 6538  4521b44b115827e8
-00000f40: 3530 6632 2729 0a70 6172 656e 745f 6462  50f2').parent_db
-00000f50: 203d 206e 6f74 696f 6e2e 4461 7461 6261   = notion.Databa
-00000f60: 7365 2868 6f6d 6570 6167 652e 7061 7265  se(homepage.pare
-00000f70: 6e74 5f69 6429 0a0a 2320 7769 6c6c 2061  nt_id)..# will a
-00000f80: 6c73 6f20 6c6f 6f6b 2066 6f72 2065 6e76  lso look for env
-00000f90: 2076 6172 2060 545a 6020 746f 2073 6574   var `TZ` to set
-00000fa0: 2074 6865 2074 696d 657a 6f6e 6520 666f   the timezone fo
-00000fb0: 7220 616c 6c20 6e6f 7469 6f6e 206f 626a  r all notion obj
-00000fc0: 6563 7473 2e20 4966 206e 6f74 2066 6f75  ects. If not fou
-00000fd0: 6e64 2c20 7769 6c6c 2064 6566 6175 6c74  nd, will default
-00000fe0: 2074 6f20 6c6f 6361 6c20 7469 6d65 7a6f   to local timezo
-00000ff0: 6e65 2e0a 6060 600a 0a60 5f5f 6765 7469  ne..```..`__geti
-00001000: 7465 6d5f 5f60 2073 6561 7263 6873 2066  tem__` searchs f
-00001010: 6f72 2070 6167 6520 7072 6f70 6572 7479  or page property
-00001020: 2076 616c 7565 7320 7768 656e 2069 6e64   values when ind
-00001030: 6578 696e 6720 6120 5061 6765 2c20 616e  exing a Page, an
-00001040: 6420 666f 7220 7072 6f70 6572 7479 206f  d for property o
-00001050: 626a 6563 7473 2077 6865 6e20 696e 6465  bjects when inde
-00001060: 7869 6e67 2061 2044 6174 6162 6173 652e  xing a Database.
-00001070: 0a0a 6060 6070 790a 686f 6d65 7061 6765  ..```py.homepage
-00001080: 5b27 6465 7065 6e64 656e 6369 6573 275d  ['dependencies']
-00001090: 0a23 207b 0a23 2020 2020 2022 6964 223a  .# {.#     "id":
-000010a0: 2022 5759 5971 222c 0a23 2020 2020 2022   "WYYq",.#     "
-000010b0: 7479 7065 223a 2022 7265 6c61 7469 6f6e  type": "relation
-000010c0: 222c 0a23 2020 2020 2022 7265 6c61 7469  ",.#     "relati
-000010d0: 6f6e 223a 205b 0a23 2020 2020 2020 2020  on": [.#        
-000010e0: 207b 0a23 2020 2020 2020 2020 2020 2020   {.#            
-000010f0: 2022 6964 223a 2022 3762 6362 6338 6536   "id": "7bcbc8e6
-00001100: 2d65 3233 372d 3433 3462 2d62 6430 642d  -e237-434b-bd0d-
-00001110: 3662 3536 6530 3434 3230 3062 220a 2320  6b56e044200b".# 
-00001120: 2020 2020 2020 2020 7d0a 2320 2020 2020          }.#     
-00001130: 5d2c 0a23 2020 2020 2022 6861 735f 6d6f  ],.#     "has_mo
-00001140: 7265 223a 2066 616c 7365 0a23 207d 0a0a  re": false.# }..
-00001150: 7061 7265 6e74 5f64 625b 2764 6570 656e  parent_db['depen
-00001160: 6465 6e63 6965 7327 5d0a 2320 7b0a 2320  dencies'].# {.# 
-00001170: 2020 2020 2269 6422 3a20 2257 5959 7122      "id": "WYYq"
-00001180: 2c0a 2320 2020 2020 226e 616d 6522 3a20  ,.#     "name": 
-00001190: 2264 6570 656e 6465 6e63 6965 7322 2c0a  "dependencies",.
-000011a0: 2320 2020 2020 2274 7970 6522 3a20 2272  #     "type": "r
-000011b0: 656c 6174 696f 6e22 2c0a 2320 2020 2020  elation",.#     
-000011c0: 2272 656c 6174 696f 6e22 3a20 7b0a 2320  "relation": {.# 
-000011d0: 2020 2020 2020 2020 2264 6174 6162 6173          "databas
-000011e0: 655f 6964 223a 2022 6635 3938 3461 3765  e_id": "f5984a7e
-000011f0: 2d32 3235 372d 3461 6230 2d39 6430 612d  -2257-4ab0-9d0a-
-00001200: 3233 6561 3132 3332 3430 3331 222c 0a23  23ea12324031",.#
-00001210: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00001220: 2022 6475 616c 5f70 726f 7065 7274 7922   "dual_property"
-00001230: 2c0a 2320 2020 2020 2020 2020 2264 7561  ,.#         "dua
-00001240: 6c5f 7072 6f70 6572 7479 223a 207b 0a23  l_property": {.#
-00001250: 2020 2020 2020 2020 2020 2020 2022 7379               "sy
-00001260: 6e63 6564 5f70 726f 7065 7274 795f 6e61  nced_property_na
-00001270: 6d65 223a 2022 626c 6f63 6b65 6422 2c0a  me": "blocked",.
-00001280: 2320 2020 2020 2020 2020 2020 2020 2273  #             "s
-00001290: 796e 6365 645f 7072 6f70 6572 7479 5f69  ynced_property_i
-000012a0: 6422 3a20 2277 7825 3744 5122 0a23 2020  d": "wx%7DQ".#  
-000012b0: 2020 2020 2020 207d 0a23 2020 2020 207d         }.#     }
-000012c0: 0a23 207d 0a60 6060 0a0a 2a2a 5f53 6565  .# }.```..**_See
-000012d0: 2075 7361 6765 206f 6620 7265 7472 6965   usage of retrie
-000012e0: 7669 6e67 2076 616c 7565 7320 6672 6f6d  ving values from
-000012f0: 2061 2070 6167 6520 696e 2065 7861 6d70   a page in examp
-00001300: 6c65 732f 7265 7472 6965 7669 6e67 2d70  les/retrieving-p
-00001310: 726f 7065 7274 792d 6974 656d 732e 6d64  roperty-items.md
-00001320: 5f2a 2a20 200a 0a42 656c 6f77 2069 7320  _**  ..Below is 
-00001330: 6120 6272 6965 6620 6578 616d 706c 6520  a brief example 
-00001340: 6966 2077 6520 7765 7265 2077 616e 7469  if we were wanti
-00001350: 6e67 2074 6f20 6765 7420 7468 6520 7061  ng to get the pa
-00001360: 6765 2069 6420 6672 6f6d 2074 6865 2061  ge id from the a
-00001370: 626f 7665 2070 726f 7065 7274 7920 6064  bove property `d
-00001380: 6570 656e 6465 6e63 6965 7360 2069 6e20  ependencies` in 
-00001390: 6068 6f6d 6570 6167 6560 2e0a 0a60 6060  `homepage`...```
-000013a0: 7079 0a66 726f 6d20 6e6f 7469 6f6e 2069  py.from notion i
-000013b0: 6d70 6f72 7420 7072 6f70 6572 7479 6974  mport propertyit
-000013c0: 656d 730a 0a72 656c 6174 6564 5f69 643a  ems..related_id:
-000013d0: 206c 6973 745b 7374 725d 203d 2070 726f   list[str] = pro
-000013e0: 7065 7274 7969 7465 6d73 2e72 656c 6174  pertyitems.relat
-000013f0: 696f 6e28 686f 6d65 7061 6765 2e64 6570  ion(homepage.dep
-00001400: 656e 6465 6e63 6965 7329 0a60 6060 0a60  endencies).```.`
-00001410: 6060 7079 0a3e 3e3e 205b 2237 6263 6263  ``py.>>> ["7bcbc
-00001420: 3865 362d 6532 3337 2d34 3334 622d 6264  8e6-e237-434b-bd
-00001430: 3064 2d36 6235 3665 3034 3432 3030 6222  0d-6b56e044200b"
-00001440: 5d0a 6060 600a 0a42 6f74 6820 5061 6765  ].```..Both Page
-00001450: 2773 2061 6e64 2044 6174 6162 6173 6527  's and Database'
-00001460: 7320 6861 7665 2073 6574 7465 7273 2066  s have setters f
-00001470: 6f72 2074 6974 6c65 2f69 636f 6e2f 636f  or title/icon/co
-00001480: 7665 722e 0a0a 6060 6070 790a 686f 6d65  ver...```py.home
-00001490: 7061 6765 2e74 6974 6c65 203d 2022 6e65  page.title = "ne
-000014a0: 7720 7061 6765 220a 686f 6d65 7061 6765  w page".homepage
-000014b0: 2e63 6f76 6572 203d 2022 6874 7470 733a  .cover = "https:
-000014c0: 2f2f 7777 772e 6e6f 7469 6f6e 2e73 6f2f  //www.notion.so/
-000014d0: 696d 6167 6573 2f70 6167 652d 636f 7665  images/page-cove
-000014e0: 722f 7765 6262 312e 6a70 6722 0a68 6f6d  r/webb1.jpg".hom
-000014f0: 6570 6167 652e 6963 6f6e 203d 2022 6874  epage.icon = "ht
-00001500: 7470 733a 2f2f 7777 772e 6e6f 7469 6f6e  tps://www.notion
-00001510: 2e73 6f2f 6963 6f6e 732f 616c 6965 6e2d  .so/icons/alien-
-00001520: 7069 7865 6c5f 7075 7270 6c65 2e73 7667  pixel_purple.svg
-00001530: 220a 6060 600a 0a3c 7020 616c 6967 6e3d  ".```..<p align=
-00001540: 2263 656e 7465 7222 3e20 3c69 6d67 2073  "center"> <img s
-00001550: 7263 3d22 6578 616d 706c 6573 2f69 6d61  rc="examples/ima
-00001560: 6765 732f 6e65 775f 7061 6765 2e70 6e67  ges/new_page.png
-00001570: 223e 203c 2f70 3e0a 0a3c 6272 3e0a 0a23  "> </p>..<br>..#
-00001580: 2320 4372 6561 7469 6e67 2050 6167 6573  # Creating Pages
-00001590: 2f44 6174 6162 6173 6573 2f42 6c6f 636b  /Databases/Block
-000015a0: 730a 0a54 6865 2063 7572 7265 6e74 2076  s..The current v
-000015b0: 6572 7369 6f6e 206f 6620 7468 6520 4e6f  ersion of the No
-000015c0: 7469 6f6e 2061 7069 2064 6f65 7320 6e6f  tion api does no
-000015d0: 7420 616c 6c6f 7720 7061 6765 7320 746f  t allow pages to
-000015e0: 2062 6520 6372 6561 7465 6420 746f 2074   be created to t
-000015f0: 6865 2070 6172 656e 7420 6077 6f72 6b73  he parent `works
-00001600: 7061 6365 602e 2020 0a43 7265 6174 6520  pace`.  .Create 
-00001610: 6f62 6a65 6374 7320 6279 2070 6173 7369  objects by passi
-00001620: 6e67 2061 6e20 6578 6973 7469 6e67 2050  ng an existing P
-00001630: 6167 652f 4461 7461 6261 7365 2069 6e73  age/Database ins
-00001640: 7461 6e63 6520 6173 2061 6e20 6172 6720  tance as an arg 
-00001650: 746f 2074 6865 2060 6372 6561 7465 6020  to the `create` 
-00001660: 636c 6173 736d 6574 686f 6473 2e0a 0a60  classmethods...`
-00001670: 6060 7079 0a6e 6577 5f64 6174 6162 6173  ``py.new_databas
-00001680: 6520 3d20 6e6f 7469 6f6e 2e44 6174 6162  e = notion.Datab
-00001690: 6173 652e 6372 6561 7465 280a 2020 2020  ase.create(.    
-000016a0: 7061 7265 6e74 5f69 6e73 7461 6e63 653d  parent_instance=
-000016b0: 7465 7374 7061 6765 2c0a 2020 2020 6461  testpage,.    da
-000016c0: 7461 6261 7365 5f74 6974 6c65 3d22 5469  tabase_title="Ti
-000016d0: 746c 6522 2c0a 2020 2020 6e61 6d65 5f63  tle",.    name_c
-000016e0: 6f6c 756d 6e3d 2270 6167 6522 2c20 2320  olumn="page", # 
-000016f0: 5468 6973 2069 7320 7468 6520 636f 6c75  This is the colu
-00001700: 6d6e 2063 6f6e 7461 696e 696e 6720 7061  mn containing pa
-00001710: 6765 206e 616d 6573 2e20 4465 6661 756c  ge names. Defaul
-00001720: 7473 2074 6f20 224e 616d 6522 2e0a 2020  ts to "Name"..  
-00001730: 2020 6973 5f69 6e6c 696e 653d 5472 7565    is_inline=True
-00001740: 2c0a 2020 2020 6465 7363 7269 7074 696f  ,.    descriptio
-00001750: 6e3d 2245 7861 6d70 6c65 2044 6174 6162  n="Example Datab
-00001760: 6173 652e 222c 0a29 0a0a 6e65 775f 7061  ase.",.)..new_pa
-00001770: 6765 203d 206e 6f74 696f 6e2e 5061 6765  ge = notion.Page
-00001780: 2e63 7265 6174 6528 6e65 775f 6461 7461  .create(new_data
-00001790: 6261 7365 2c20 7061 6765 5f74 6974 6c65  base, page_title
-000017a0: 3d22 4120 6e65 7720 6461 7461 6261 7365  ="A new database
-000017b0: 2072 6f77 2229 0a60 6060 0a0a 426c 6f63   row").```..Bloc
-000017c0: 6b73 2063 616e 2062 6520 6372 6561 7465  ks can be create
-000017d0: 6420 7769 7468 2060 6e6f 7469 6f6e 2e61  d with `notion.a
-000017e0: 7069 2e62 6c6f 636b 7479 7065 6661 6374  pi.blocktypefact
-000017f0: 6f72 792e 426c 6f63 6b46 6163 746f 7279  ory.BlockFactory
-00001800: 6020 6279 2061 7070 656e 6469 6e67 2074  ` by appending t
-00001810: 6f20 616e 2065 7869 7369 7469 6e67 2042  o an exisiting B
-00001820: 6c6f 636b 206f 7220 5061 6765 2e20 200a  lock or Page.  .
-00001830: 5468 6520 6e65 7720 626c 6f63 6b20 6973  The new block is
-00001840: 2061 6c77 6179 7320 7265 7475 726e 6564   always returned
-00001850: 2061 7320 616e 2069 6e73 7461 6e63 6520   as an instance 
-00001860: 6f66 2060 6e6f 7469 6f6e 2e61 7069 2e6e  of `notion.api.n
-00001870: 6f74 696f 6e62 6c6f 636b 2e42 6c6f 636b  otionblock.Block
-00001880: 602e 0a60 6060 7079 0a66 726f 6d20 6e6f  `..```py.from no
-00001890: 7469 6f6e 2069 6d70 6f72 7420 7072 6f70  tion import prop
-000018a0: 6572 7469 6573 2061 7320 7072 6f70 0a0a  erties as prop..
-000018b0: 2320 606e 6577 5f73 796e 6365 645f 626c  # `new_synced_bl
-000018c0: 6f63 6b60 2072 6566 6572 7320 746f 2074  ock` refers to t
-000018d0: 6865 206f 7269 6769 6e61 6c20 7379 6e63  he original sync
-000018e0: 6564 2062 6c6f 636b 2069 6e20 7468 6520  ed block in the 
-000018f0: 4e6f 7469 6f6e 2055 492e 0a6f 7269 6769  Notion UI..origi
-00001900: 6e61 6c5f 7379 6e63 6564 5f62 6c6f 636b  nal_synced_block
-00001910: 203d 206e 6f74 696f 6e2e 426c 6f63 6b46   = notion.BlockF
-00001920: 6163 746f 7279 2e6e 6577 5f73 796e 6365  actory.new_synce
-00001930: 645f 626c 6f63 6b28 686f 6d65 7061 6765  d_block(homepage
-00001940: 290a 0a23 2041 6464 696e 6720 636f 6e74  )..# Adding cont
-00001950: 656e 7420 746f 2074 6865 2073 796e 6365  ent to the synce
-00001960: 6420 626c 6f63 6b0a 6e6f 7469 6f6e 2e42  d block.notion.B
-00001970: 6c6f 636b 4661 6374 6f72 792e 7061 7261  lockFactory.para
-00001980: 6772 6170 6828 0a20 2020 206f 7269 6769  graph(.    origi
-00001990: 6e61 6c5f 7379 6e63 6564 5f62 6c6f 636b  nal_synced_block
-000019a0: 2c20 5b70 726f 702e 5269 6368 5465 7874  , [prop.RichText
-000019b0: 2822 5468 6973 2069 7320 6120 7379 6e63  ("This is a sync
-000019c0: 6564 2062 6c6f 636b 2e22 295d 0a29 0a23  ed block.")].).#
-000019d0: 2052 6566 6572 656e 6369 6e67 2074 6865   Referencing the
-000019e0: 2073 796e 6365 6420 626c 6f63 6b20 696e   synced block in
-000019f0: 2061 206e 6577 2070 6167 652e 0a6e 6f74   a new page..not
-00001a00: 696f 6e2e 426c 6f63 6b46 6163 746f 7279  ion.BlockFactory
-00001a10: 2e72 6566 6572 656e 6365 5f73 796e 6365  .reference_synce
-00001a20: 645f 626c 6f63 6b28 6e65 775f 7061 6765  d_block(new_page
-00001a30: 2c20 6f72 6967 696e 616c 5f73 796e 6365  , original_synce
-00001a40: 645f 626c 6f63 6b2e 6964 290a 6060 600a  d_block.id).```.
-00001a50: 0a3c 6272 3e0a 0a23 2323 2045 7861 6d70  .<br>..### Examp
-00001a60: 6c65 2057 6f72 6b66 6c6f 773a 202a 2a5f  le Workflow: **_
-00001a70: 4170 7065 6e64 696e 6720 626c 6f63 6b73  Appending blocks
-00001a80: 2074 6f20 6120 7061 6765 2061 7320 6120   to a page as a 
-00001a90: 7265 6d69 6e64 6572 2e5f 2a2a 0a0a 6060  reminder._**..``
-00001aa0: 6070 790a 6465 6620 696e 5f62 6c6f 636b  `py.def in_block
-00001ab0: 5f72 656d 696e 6465 7228 7061 6765 3a20  _reminder(page: 
-00001ac0: 6e6f 7469 6f6e 2e50 6167 652c 206d 6573  notion.Page, mes
-00001ad0: 7361 6765 3a20 7374 722c 2075 7365 725f  sage: str, user_
-00001ae0: 6e61 6d65 3a20 7374 7229 202d 3e20 4e6f  name: str) -> No
-00001af0: 6e65 3a0a 2020 2020 6d65 6e74 696f 6e62  ne:.    mentionb
-00001b00: 6c6f 636b 203d 206e 6f74 696f 6e2e 426c  lock = notion.Bl
-00001b10: 6f63 6b46 6163 746f 7279 2e70 6172 6167  ockFactory.parag
-00001b20: 7261 7068 280a 2020 2020 2020 2020 7061  raph(.        pa
-00001b30: 6765 2c0a 2020 2020 2020 2020 5b0a 2020  ge,.        [.  
-00001b40: 2020 2020 2020 2020 2020 7072 6f70 2e4d            prop.M
-00001b50: 656e 7469 6f6e 2e75 7365 7228 0a20 2020  ention.user(.   
-00001b60: 2020 2020 2020 2020 2020 2020 206e 6f74               not
-00001b70: 696f 6e2e 576f 726b 7370 6163 6528 292e  ion.Workspace().
-00001b80: 7265 7472 6965 7665 5f75 7365 7228 7573  retrieve_user(us
-00001b90: 6572 5f6e 616d 653d 7573 6572 5f6e 616d  er_name=user_nam
-00001ba0: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-00001bb0: 2020 2020 616e 6e6f 7461 7469 6f6e 733d      annotations=
-00001bc0: 7072 6f70 2e41 6e6e 6f74 6174 696f 6e73  prop.Annotations
-00001bd0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00001be0: 2020 2020 2020 636f 6465 3d54 7275 652c        code=True,
-00001bf0: 2062 6f6c 643d 5472 7565 2c20 636f 6c6f   bold=True, colo
-00001c00: 723d 7072 6f70 2e42 6c6f 636b 436f 6c6f  r=prop.BlockColo
-00001c10: 722e 7075 7270 6c65 0a20 2020 2020 2020  r.purple.       
-00001c20: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-00001c30: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-00001c40: 2020 2020 2020 2070 726f 702e 5269 6368         prop.Rich
-00001c50: 5465 7874 2822 202d 2022 292c 0a20 2020  Text(" - "),.   
-00001c60: 2020 2020 2020 2020 2070 726f 702e 4d65           prop.Me
-00001c70: 6e74 696f 6e2e 6461 7465 280a 2020 2020  ntion.date(.    
-00001c80: 2020 2020 2020 2020 2020 2020 6461 7465              date
-00001c90: 7469 6d65 2e6e 6f77 2829 2e61 7374 696d  time.now().astim
-00001ca0: 657a 6f6e 6528 7461 7267 6574 5f70 6167  ezone(target_pag
-00001cb0: 652e 747a 292e 6973 6f66 6f72 6d61 7428  e.tz).isoformat(
-00001cc0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00001cd0: 2020 2061 6e6e 6f74 6174 696f 6e73 3d70     annotations=p
-00001ce0: 726f 702e 416e 6e6f 7461 7469 6f6e 7328  rop.Annotations(
-00001cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001d00: 2020 2020 2063 6f64 653d 5472 7565 2c20       code=True, 
-00001d10: 626f 6c64 3d54 7275 652c 2063 6f6c 6f72  bold=True, color
-00001d20: 3d70 726f 702e 426c 6f63 6b43 6f6c 6f72  =prop.BlockColor
-00001d30: 2e70 7572 706c 655f 6261 636b 6772 6f75  .purple_backgrou
-00001d40: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
-00001d50: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-00001d60: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-00001d70: 2070 726f 702e 5269 6368 5465 7874 2822   prop.RichText("
-00001d80: 3a22 292c 0a20 2020 2020 2020 205d 2c0a  :"),.        ],.
-00001d90: 2020 2020 290a 2020 2020 2320 4669 7273      ).    # Firs
-00001da0: 7420 6d65 7468 6f64 2072 6574 7572 6e65  t method returne
-00001db0: 6420 7468 6520 6e65 776c 7920 6372 6561  d the newly crea
-00001dc0: 7465 6420 626c 6f63 6b20 7468 6174 2077  ted block that w
-00001dd0: 6520 6170 7065 6e64 2074 6f20 6865 7265  e append to here
-00001de0: 3a0a 2020 2020 6e6f 7469 6f6e 2e42 6c6f  :.    notion.Blo
-00001df0: 636b 4661 6374 6f72 792e 7061 7261 6772  ckFactory.paragr
-00001e00: 6170 6828 6d65 6e74 696f 6e62 6c6f 636b  aph(mentionblock
-00001e10: 2c20 5b70 726f 702e 5269 6368 5465 7874  , [prop.RichText
-00001e20: 286d 6573 7361 6765 295d 290a 2020 2020  (message)]).    
-00001e30: 6e6f 7469 6f6e 2e42 6c6f 636b 4661 6374  notion.BlockFact
-00001e40: 6f72 792e 6469 7669 6465 7228 7061 6765  ory.divider(page
-00001e50: 290a 6060 600a 0a60 6060 7079 0a3e 3e3e  ).```..```py.>>>
-00001e60: 206d 795f 7061 6765 203d 206e 6f74 696f   my_page = notio
-00001e70: 6e2e 5061 6765 2822 3062 3965 6363 6661  n.Page("0b9eccfa
-00001e80: 3839 3065 3463 3333 3930 3137 3565 6531  890e4c3390175ee1
-00001e90: 3063 3636 3461 3335 2229 0a3e 3e3e 2069  0c664a35").>>> i
-00001ea0: 6e5f 626c 6f63 6b5f 7265 6d69 6e64 6572  n_block_reminder
-00001eb0: 2870 6167 653d 6d79 5f70 6167 652c 206d  (page=my_page, m
-00001ec0: 6573 7361 6765 3d22 6d65 7373 6167 6520  essage="message 
-00001ed0: 6865 7265 222c 2075 7365 725f 6e61 6d65  here", user_name
-00001ee0: 3d22 596f 7572 204e 616d 6522 290a 6060  ="Your Name").``
-00001ef0: 600a 3c70 2061 6c69 676e 3d22 6365 6e74  `.<p align="cent
-00001f00: 6572 223e 0a20 2020 203c 696d 6720 7372  er">.    <img sr
-00001f10: 633d 2265 7861 6d70 6c65 732f 696d 6167  c="examples/imag
-00001f20: 6573 2f65 7861 6d70 6c65 5f66 756e 6374  es/example_funct
-00001f30: 696f 6e5f 7265 6d69 6e64 6572 2e70 6e67  ion_reminder.png
-00001f40: 223e 0a3c 2f70 3e0a 0a3c 6272 3e0a 0a23  ">.</p>..<br>..#
-00001f50: 2320 4164 642c 2053 6574 2c20 2620 4465  # Add, Set, & De
-00001f60: 6c65 7465 3a20 5061 6765 2070 726f 7065  lete: Page prope
-00001f70: 7274 7920 7661 6c75 6573 207c 2044 6174  rty values | Dat
-00001f80: 6162 6173 6520 7072 6f70 6572 7479 206f  abase property o
-00001f90: 626a 6563 7473 0a0a 5468 6520 6669 7273  bjects..The firs
-00001fa0: 7420 6172 6775 6d65 6e74 2066 6f72 2061  t argument for a
-00001fb0: 6c6c 2064 6174 6162 6173 6520 636f 6c75  ll database colu
-00001fc0: 6d6e 206d 6574 686f 6473 2069 7320 7468  mn methods is th
-00001fd0: 6520 6e61 6d65 206f 6620 7468 6520 7072  e name of the pr
-00001fe0: 6f70 6572 7479 2c20 200a 4966 2069 7420  operty,  .If it 
-00001ff0: 646f 6573 206e 6f74 2065 7869 7374 2c20  does not exist, 
-00002000: 7468 656e 2061 206e 6577 2070 726f 7065  then a new prope
-00002010: 7274 7920 6f62 6a65 6374 2069 7320 6372  rty object is cr
-00002020: 6561 7465 642e 2020 0a49 6620 6974 2061  eated.  .If it a
-00002030: 6c72 6561 6479 2065 7869 7374 732c 2074  lready exists, t
-00002040: 6865 6e20 7468 6520 6d65 7468 6f64 2077  hen the method w
-00002050: 696c 6c20 6f76 6572 7772 6974 6520 6974  ill overwrite it
-00002060: 2e0a 0a49 6620 7468 6520 6e61 6d65 2070  ...If the name p
-00002070: 6173 7365 6420 616c 7265 6164 7920 6578  assed already ex
-00002080: 6973 7473 2c20 6275 7420 6974 2773 2061  ists, but it's a
-00002090: 2064 6966 6665 7265 6e74 2063 6f6c 756d   different colum
-000020a0: 6e20 7479 7065 2074 6861 6e20 7468 6520  n type than the 
-000020b0: 6d65 7468 6f64 2075 7365 6420 2d20 7468  method used - th
-000020c0: 656e 2074 6865 2041 5049 2077 696c 6c20  en the API will 
-000020d0: 6f76 6572 7772 6974 6520 7468 6973 2061  overwrite this a
-000020e0: 6e64 2063 6861 6e67 6520 7468 6520 7072  nd change the pr
-000020f0: 6f70 6572 7479 206f 626a 6563 7420 746f  operty object to
-00002100: 2074 6865 206e 6577 2063 6f6c 756d 6e20   the new column 
-00002110: 7479 7065 2e20 200a 5468 6520 6f72 6967  type.  .The orig
-00002120: 696e 616c 2070 6172 616d 6574 6572 7320  inal parameters 
-00002130: 7769 6c6c 2062 6520 7361 7665 6420 6966  will be saved if
-00002140: 2079 6f75 2064 6563 6964 6520 746f 2073   you decide to s
-00002150: 7769 7463 6820 6261 636b 2028 692e 652e  witch back (i.e.
-00002160: 2069 6620 796f 7520 6368 616e 6765 2061   if you change a
-00002170: 2066 6f72 6d75 6c61 2063 6f6c 756d 6e20   formula column 
-00002180: 746f 2061 2073 656c 6563 7420 636f 6c75  to a select colu
-00002190: 6d6e 2c20 7570 6f6e 2063 6861 6e67 696e  mn, upon changin
-000021a0: 6720 6974 2062 6163 6b20 746f 2061 2066  g it back to a f
-000021b0: 6f72 6d75 6c61 2063 6f6c 756d 6e2c 2074  ormula column, t
-000021c0: 6865 206f 7269 6769 6e61 6c20 666f 726d  he original form
-000021d0: 756c 6120 6578 7072 6573 7369 6f6e 2077  ula expression w
-000021e0: 696c 6c20 7374 696c 6c20 6265 2074 6865  ill still be the
-000021f0: 7265 292e 2020 200a 0a60 6060 7079 0a6e  re).   ..```py.n
-00002200: 6577 5f64 6174 6162 6173 652e 666f 726d  ew_database.form
-00002210: 756c 615f 636f 6c75 6d6e 2822 7061 6765  ula_column("page
-00002220: 2069 6422 2c20 6578 7072 6573 7369 6f6e   id", expression
-00002230: 3d22 6964 2829 2229 0a0a 6e65 775f 6461  ="id()")..new_da
-00002240: 7461 6261 7365 2e64 656c 6574 655f 7072  tabase.delete_pr
-00002250: 6f70 6572 7479 2822 7572 6c22 290a 0a6e  operty("url")..n
-00002260: 6577 5f64 6174 6162 6173 652e 6d75 6c74  ew_database.mult
-00002270: 6973 656c 6563 745f 636f 6c75 6d6e 280a  iselect_column(.
-00002280: 2020 2020 226e 6577 206f 7074 696f 6e73      "new options
-00002290: 2063 6f6c 756d 6e22 2c0a 2020 2020 6f70   column",.    op
-000022a0: 7469 6f6e 733d 5b0a 2020 2020 2020 2020  tions=[.        
-000022b0: 7072 6f70 2e4f 7074 696f 6e28 226f 7074  prop.Option("opt
-000022c0: 696f 6e2d 6122 2c20 7072 6f70 2e50 726f  ion-a", prop.Pro
-000022d0: 7065 7274 7943 6f6c 6f72 2e72 6564 292c  pertyColor.red),
-000022e0: 0a20 2020 2020 2020 2070 726f 702e 4f70  .        prop.Op
-000022f0: 7469 6f6e 2822 6f70 7469 6f6e 2d62 222c  tion("option-b",
-00002300: 2070 726f 702e 5072 6f70 6572 7479 436f   prop.PropertyCo
-00002310: 6c6f 722e 6772 6565 6e29 2c0a 2020 2020  lor.green),.    
-00002320: 2020 2020 7072 6f70 2e4f 7074 696f 6e28      prop.Option(
-00002330: 226f 7074 696f 6e2d 6322 2c20 7072 6f70  "option-c", prop
-00002340: 2e50 726f 7065 7274 7943 6f6c 6f72 2e62  .PropertyColor.b
-00002350: 6c75 6529 2c0a 2020 2020 5d2c 0a29 0a0a  lue),.    ],.)..
-00002360: 2320 6966 2061 6e20 6f70 7469 6f6e 2064  # if an option d
-00002370: 6f65 7320 6e6f 7420 616c 7265 6164 7920  oes not already 
-00002380: 6578 6973 742c 2061 206e 6577 206f 6e65  exist, a new one
-00002390: 2077 696c 6c20 6265 2063 7265 6174 6564   will be created
-000023a0: 2077 6974 6820 6120 7261 6e64 6f6d 2063   with a random c
-000023b0: 6f6c 6f72 2e0a 2320 7468 6973 2069 7320  olor..# this is 
-000023c0: 6e6f 7420 7472 7565 2066 6f72 2060 7374  not true for `st
-000023d0: 6174 7573 6020 636f 6c75 6d6e 2074 7970  atus` column typ
-000023e0: 6573 2c20 7768 6963 6820 6361 6e20 6f6e  es, which can on
-000023f0: 6c79 2062 6520 6564 6974 6564 2076 6961  ly be edited via
-00002400: 2055 492e 0a0a 6e65 775f 7061 6765 2e73   UI...new_page.s
-00002410: 6574 5f6d 756c 7469 7365 6c65 6374 2822  et_multiselect("
-00002420: 6f70 7469 6f6e 7322 2c20 5b22 6f70 7469  options", ["opti
-00002430: 6f6e 2d61 222c 2022 6f70 7469 6f6e 2d62  on-a", "option-b
-00002440: 225d 290a 6060 600a 0a3c 6272 3e0a 0a23  "]).```..<br>..#
-00002450: 2320 4461 7461 6261 7365 2051 7565 7269  # Database Queri
-00002460: 6573 0a0a 4120 7369 6e67 6c65 2060 6e6f  es..A single `no
-00002470: 7469 6f6e 2e71 7565 7279 2e70 726f 7066  tion.query.propf
-00002480: 696c 7465 722e 5072 6f70 6572 7479 4669  ilter.PropertyFi
-00002490: 6c74 6572 6020 6973 2065 7175 6976 616c  lter` is equival
-000024a0: 656e 7420 746f 2066 696c 7465 7269 6e67  ent to filtering
-000024b0: 206f 6e65 2070 726f 7065 7274 7920 7479   one property ty
-000024c0: 7065 2069 6e20 4e6f 7469 6f6e 2e0a 546f  pe in Notion..To
-000024d0: 2062 7569 6c64 2066 696c 7465 7273 2065   build filters e
-000024e0: 7175 6976 616c 656e 7420 746f 204e 6f74  quivalent to Not
-000024f0: 696f 6e27 7320 2761 6476 616e 6365 6420  ion's 'advanced 
-00002500: 6669 6c74 6572 7327 2c20 7573 6520 606e  filters', use `n
-00002510: 6f74 696f 6e2e 7175 6572 792e 636f 6d70  otion.query.comp
-00002520: 6f75 6e64 2e43 6f6d 706f 756e 6446 696c  ound.CompoundFil
-00002530: 7465 7260 2e0a 0a60 6060 7079 0a66 726f  ter`...```py.fro
-00002540: 6d20 6461 7465 7469 6d65 2069 6d70 6f72  m datetime impor
-00002550: 7420 6461 7465 7469 6d65 0a66 726f 6d20  t datetime.from 
-00002560: 6461 7465 7469 6d65 2069 6d70 6f72 7420  datetime import 
-00002570: 7469 6d65 6465 6c74 610a 0a66 726f 6d20  timedelta..from 
-00002580: 6e6f 7469 6f6e 2069 6d70 6f72 7420 7175  notion import qu
-00002590: 6572 790a 0a54 4f44 4159 203d 2064 6174  ery..TODAY = dat
-000025a0: 6574 696d 652e 636f 6d62 696e 6528 6461  etime.combine(da
-000025b0: 7465 7469 6d65 2e74 6f64 6179 2829 2c20  tetime.today(), 
-000025c0: 6461 7465 7469 6d65 2e6d 696e 2e74 696d  datetime.min.tim
-000025d0: 6528 2929 0a54 4f4d 4f52 524f 5720 3d20  e()).TOMORROW = 
-000025e0: 544f 4441 5920 2b20 7469 6d65 6465 6c74  TODAY + timedelt
-000025f0: 6128 3129 0a0a 7175 6572 795f 6669 6c74  a(1)..query_filt
-00002600: 6572 203d 2071 7565 7279 2e43 6f6d 706f  er = query.Compo
-00002610: 756e 6446 696c 7465 7228 292e 5f61 6e64  undFilter()._and
-00002620: 280a 2020 2020 7175 6572 792e 5072 6f70  (.    query.Prop
-00002630: 6572 7479 4669 6c74 6572 2e64 6174 6528  ertyFilter.date(
-00002640: 2264 6174 6522 2c20 2263 7265 6174 6564  "date", "created
-00002650: 5f74 696d 6522 2c20 226f 6e5f 6f72 5f61  _time", "on_or_a
-00002660: 6674 6572 222c 2054 4f44 4159 2e69 736f  fter", TODAY.iso
-00002670: 666f 726d 6174 2829 292c 0a20 2020 2071  format()),.    q
-00002680: 7565 7279 2e50 726f 7065 7274 7946 696c  uery.PropertyFil
-00002690: 7465 722e 6461 7465 2822 6461 7465 222c  ter.date("date",
-000026a0: 2022 6372 6561 7465 645f 7469 6d65 222c   "created_time",
-000026b0: 2022 6265 666f 7265 222c 2054 4f4d 4f52   "before", TOMOR
-000026c0: 524f 572e 6973 6f66 6f72 6d61 7428 2929  ROW.isoformat())
-000026d0: 2c0a 2020 2020 7175 6572 792e 436f 6d70  ,.    query.Comp
-000026e0: 6f75 6e64 4669 6c74 6572 2829 2e5f 6f72  oundFilter()._or
-000026f0: 280a 2020 2020 2020 2020 7175 6572 792e  (.        query.
-00002700: 5072 6f70 6572 7479 4669 6c74 6572 2e74  PropertyFilter.t
-00002710: 6578 7428 226e 616d 6522 2c20 2274 6974  ext("name", "tit
-00002720: 6c65 222c 2022 636f 6e74 6169 6e73 222c  le", "contains",
-00002730: 2022 796f 7572 2070 6167 6520 7469 746c   "your page titl
-00002740: 6522 292c 0a20 2020 2020 2020 2071 7565  e"),.        que
-00002750: 7279 2e50 726f 7065 7274 7946 696c 7465  ry.PropertyFilte
-00002760: 722e 7465 7874 2822 6e61 6d65 222c 2022  r.text("name", "
-00002770: 7469 746c 6522 2c20 2263 6f6e 7461 696e  title", "contain
-00002780: 7322 2c20 2279 6f75 7220 6f74 6865 7220  s", "your other 
-00002790: 7061 6765 2074 6974 6c65 2229 2c0a 2020  page title"),.  
-000027a0: 2020 292c 0a29 0a0a 7175 6572 795f 736f    ),.)..query_so
-000027b0: 7274 203d 2071 7565 7279 2e53 6f72 7446  rt = query.SortF
-000027c0: 696c 7465 7228 0a20 2020 205b 0a20 2020  ilter(.    [.   
-000027d0: 2020 2020 2071 7565 7279 2e50 726f 7065       query.Prope
-000027e0: 7274 7956 616c 7565 536f 7274 2e61 7363  rtyValueSort.asc
-000027f0: 656e 6469 6e67 2822 796f 7572 2070 726f  ending("your pro
-00002800: 7065 7274 7920 6e61 6d65 2229 2c0a 2020  perty name"),.  
-00002810: 2020 2020 2020 7175 6572 792e 456e 7472        query.Entr
-00002820: 7954 696d 6573 7461 6d70 536f 7274 2e63  yTimestampSort.c
-00002830: 7265 6174 6564 5f74 696d 655f 6465 7363  reated_time_desc
-00002840: 656e 6469 6e67 2829 2c0a 2020 2020 5d0a  ending(),.    ].
-00002850: 290a 0a71 7565 7279 5f72 6573 756c 7420  )..query_result 
-00002860: 3d20 6e65 775f 6461 7461 6261 7365 2e71  = new_database.q
-00002870: 7565 7279 280a 2020 2020 6669 6c74 6572  uery(.    filter
-00002880: 3d71 7565 7279 5f66 696c 7465 722c 0a20  =query_filter,. 
-00002890: 2020 2073 6f72 743d 7175 6572 795f 736f     sort=query_so
-000028a0: 7274 2c0a 2020 2020 7061 6765 5f73 697a  rt,.    page_siz
-000028b0: 653d 352c 0a20 2020 2066 696c 7465 725f  e=5,.    filter_
-000028c0: 7072 6f70 6572 7479 5f76 616c 7565 733d  property_values=
-000028d0: 5b22 6e61 6d65 222c 2022 6f70 7469 6f6e  ["name", "option
-000028e0: 7322 5d2c 0a29 0a60 6060 0a0a 4120 6461  s"],.).```..A da
-000028f0: 7461 6261 7365 2061 6c73 6f20 6861 7320  tabase also has 
-00002900: 7468 6520 6071 7565 7279 5f70 6167 6573  the `query_pages
-00002910: 2829 6020 6d65 7468 6f64 2e20 4974 2074  ()` method. It t
-00002920: 616b 6573 2074 6865 2073 616d 6520 7061  akes the same pa
-00002930: 7261 6d65 7465 7273 2c20 6275 7420 666f  rameters, but fo
-00002940: 7220 6561 6368 2070 6167 6520 6f62 6a65  r each page obje
-00002950: 6374 2069 6e20 7468 6520 6072 6573 756c  ct in the `resul
-00002960: 7473 6020 6172 7261 792c 2069 7420 7265  ts` array, it re
-00002970: 7472 6965 7665 7320 7468 6520 6964 2873  trieves the id(s
-00002980: 292c 2061 6e64 2069 6e73 7465 6164 2072  ), and instead r
-00002990: 6574 7572 6e73 2061 206c 6973 7420 6f66  eturns a list of
-000029a0: 2060 6e6f 7469 6f6e 2e50 6167 6560 2e0a   `notion.Page`..
-000029b0: 0a3c 6272 3e0a 0a23 2320 4578 6365 7074  .<br>..## Except
-000029c0: 696f 6e73 2026 2056 616c 6964 6174 696e  ions & Validatin
-000029d0: 6720 5265 7370 6f6e 7365 730a 0a45 7272  g Responses..Err
-000029e0: 6f72 7320 696e 204e 6f74 696f 6e20 7265  ors in Notion re
-000029f0: 7175 6573 7473 2072 6574 7572 6e20 616e  quests return an
-00002a00: 206f 626a 6563 7420 7769 7468 2074 6865   object with the
-00002a10: 206b 6579 733a 2027 6f62 6a65 6374 272c   keys: 'object',
-00002a20: 2027 7374 6174 7573 272c 2027 636f 6465   'status', 'code
-00002a30: 272c 2061 6e64 2027 6d65 7373 6167 6527  ', and 'message'
-00002a40: 2e0a 4578 6365 7074 696f 6e73 2061 7265  ..Exceptions are
-00002a50: 2072 6169 7365 6420 6279 206d 6174 6368   raised by match
-00002a60: 696e 6720 7468 6520 6572 726f 7220 636f  ing the error co
-00002a70: 6465 2061 6e64 2072 6574 7572 6e69 6e67  de and returning
-00002a80: 2074 6865 206d 6573 7361 6765 2e20 466f   the message. Fo
-00002a90: 7220 6578 616d 706c 653a 0a0a 6060 6070  r example:..```p
-00002aa0: 790a 686f 6d65 7061 6765 2e5f 7061 7463  y.homepage._patc
-00002ab0: 685f 7072 6f70 6572 7469 6573 2870 6179  h_properties(pay
-00002ac0: 6c6f 6164 3d7b 2761 6e5f 696e 636f 7272  load={'an_incorr
-00002ad0: 6563 745f 6b65 7927 3a27 7661 6c75 6527  ect_key':'value'
-00002ae0: 7d29 0a23 2045 7861 6d70 6c65 2065 7272  }).# Example err
-00002af0: 6f72 206f 626a 6563 7420 666f 7220 6c69  or object for li
-00002b00: 6e65 2061 626f 7665 2e2e 0a23 207b 0a23  ne above...# {.#
-00002b10: 2020 2027 6f62 6a65 6374 273a 2027 6572     'object': 'er
-00002b20: 726f 7227 2c20 0a23 2020 2027 7374 6174  ror', .#   'stat
-00002b30: 7573 273a 2034 3030 2c20 0a23 2020 2027  us': 400, .#   '
-00002b40: 636f 6465 273a 2027 7661 6c69 6461 7469  code': 'validati
-00002b50: 6f6e 5f65 7272 6f72 272c 200a 2320 2020  on_error', .#   
-00002b60: 276d 6573 7361 6765 273a 2027 626f 6479  'message': 'body
-00002b70: 2066 6169 6c65 6420 7661 6c69 6461 7469   failed validati
-00002b80: 6f6e 3a20 626f 6479 2e61 6e5f 696e 636f  on: body.an_inco
-00002b90: 7272 6563 745f 6b65 7920 7368 6f75 6c64  rrect_key should
-00002ba0: 2062 6520 6e6f 7420 7072 6573 656e 742c   be not present,
-00002bb0: 2069 6e73 7465 6164 2077 6173 2060 2276   instead was `"v
-00002bc0: 616c 7565 2260 2e27 0a23 207d 0a60 6060  alue"`.'.# }.```
-00002bd0: 0a0a 6060 6073 680a 5472 6163 6562 6163  ..```sh.Tracebac
-00002be0: 6b20 286d 6f73 7420 7265 6365 6e74 2063  k (most recent c
-00002bf0: 616c 6c20 6c61 7374 293a 0a46 696c 6520  all last):.File 
-00002c00: 2263 3a5c 7061 7468 5c74 6f5c 6669 6c65  "c:\path\to\file
-00002c10: 5c5f 2e70 7922 2c20 6c69 6e65 2036 2c20  \_.py", line 6, 
-00002c20: 696e 203c 6d6f 6475 6c65 3e0a 2020 2020  in <module>.    
-00002c30: 686f 6d65 7061 6765 2e5f 7061 7463 685f  homepage._patch_
-00002c40: 7072 6f70 6572 7469 6573 2870 6179 6c6f  properties(paylo
-00002c50: 6164 3d7b 2761 6e5f 696e 636f 7272 6563  ad={'an_incorrec
-00002c60: 745f 6b65 7927 3a27 7661 6c75 6527 7d29  t_key':'value'})
-00002c70: 0a46 696c 6520 2263 3a5c 2e2e 2e5c 6e6f  .File "c:\...\no
-00002c80: 7469 6f6e 5c65 7863 6570 7469 6f6e 735c  tion\exceptions\
-00002c90: 7661 6c69 6461 7465 2e70 7922 2c20 6c69  validate.py", li
-00002ca0: 6e65 2034 382c 2069 6e20 7661 6c69 6461  ne 48, in valida
-00002cb0: 7465 5f72 6573 706f 6e73 650a 2020 2020  te_response.    
-00002cc0: 7261 6973 6520 4e6f 7469 6f6e 5661 6c69  raise NotionVali
-00002cd0: 6461 7469 6f6e 4572 726f 7228 6d65 7373  dationError(mess
-00002ce0: 6167 6529 0a6e 6f74 696f 6e2e 6578 6365  age).notion.exce
-00002cf0: 7074 696f 6e73 2e65 7272 6f72 732e 4e6f  ptions.errors.No
-00002d00: 7469 6f6e 5661 6c69 6461 7469 6f6e 4572  tionValidationEr
-00002d10: 726f 723a 2062 6f64 7920 6661 696c 6564  ror: body failed
-00002d20: 2076 616c 6964 6174 696f 6e3a 2062 6f64   validation: bod
-00002d30: 792e 616e 5f69 6e63 6f72 7265 6374 5f6b  y.an_incorrect_k
-00002d40: 6579 2073 686f 756c 6420 6265 206e 6f74  ey should be not
-00002d50: 2070 7265 7365 6e74 2c20 696e 7374 6561   present, instea
-00002d60: 6420 7761 7320 6022 7661 6c75 6522 602e  d was `"value"`.
-00002d70: 0a45 7272 6f72 2034 3030 3a20 5468 6520  .Error 400: The 
-00002d80: 7265 7175 6573 7420 626f 6479 2064 6f65  request body doe
-00002d90: 7320 6e6f 7420 6d61 7463 6820 7468 6520  s not match the 
-00002da0: 7363 6865 6d61 2066 6f72 2074 6865 2065  schema for the e
-00002db0: 7870 6563 7465 6420 7061 7261 6d65 7465  xpected paramete
-00002dc0: 7273 2e0a 6060 600a 0a50 6f73 7369 626c  rs..```..Possibl
-00002dd0: 6520 6572 726f 7273 2061 7265 3a0a 202d  e errors are:. -
-00002de0: 2060 4e6f 7469 6f6e 496e 7661 6c69 644a   `NotionInvalidJ
-00002df0: 736f 6e60 0a20 2d20 604e 6f74 696f 6e49  son`. - `NotionI
-00002e00: 6e76 616c 6964 5265 7175 6573 7455 726c  nvalidRequestUrl
-00002e10: 600a 202d 2060 4e6f 7469 6f6e 496e 7661  `. - `NotionInva
-00002e20: 6c69 6452 6571 7565 7374 600a 202d 2060  lidRequest`. - `
-00002e30: 4e6f 7469 6f6e 5661 6c69 6461 7469 6f6e  NotionValidation
-00002e40: 4572 726f 7260 0a20 2d20 604e 6f74 696f  Error`. - `Notio
-00002e50: 6e4d 6973 7369 6e67 5665 7273 696f 6e60  nMissingVersion`
-00002e60: 0a20 2d20 604e 6f74 696f 6e55 6e61 7574  . - `NotionUnaut
-00002e70: 686f 7269 7a65 6460 0a20 2d20 604e 6f74  horized`. - `Not
-00002e80: 696f 6e52 6573 7472 6963 7465 6452 6573  ionRestrictedRes
-00002e90: 6f75 7263 6560 0a20 2d20 604e 6f74 696f  ource`. - `Notio
-00002ea0: 6e4f 626a 6563 744e 6f74 466f 756e 6460  nObjectNotFound`
-00002eb0: 0a20 2d20 604e 6f74 696f 6e43 6f6e 666c  . - `NotionConfl
-00002ec0: 6963 7445 7272 6f72 600a 202d 2060 4e6f  ictError`. - `No
-00002ed0: 7469 6f6e 5261 7465 4c69 6d69 7465 6460  tionRateLimited`
-00002ee0: 0a20 2d20 604e 6f74 696f 6e49 6e74 6572  . - `NotionInter
-00002ef0: 6e61 6c53 6572 7665 7245 7272 6f72 600a  nalServerError`.
-00002f00: 202d 2060 4e6f 7469 6f6e 5365 7276 6963   - `NotionServic
-00002f10: 6555 6e61 7661 696c 6162 6c65 600a 202d  eUnavailable`. -
-00002f20: 2060 4e6f 7469 6f6e 4461 7461 6261 7365   `NotionDatabase
-00002f30: 436f 6e6e 6563 7469 6f6e 556e 6176 6169  ConnectionUnavai
-00002f40: 6c61 626c 6560 0a0a 4120 636f 6d6d 6f6e  lable`..A common
-00002f50: 2065 7272 6f72 2074 6f20 6c6f 6f6b 206f   error to look o
-00002f60: 7574 2066 6f72 2069 7320 604e 6f74 696f  ut for is `Notio
-00002f70: 6e4f 626a 6563 744e 6f74 466f 756e 6460  nObjectNotFound`
-00002f80: 2e20 5468 6973 2065 7272 6f72 2069 7320  . This error is 
-00002f90: 6f66 7465 6e20 7261 6973 6564 2062 6563  often raised bec
-00002fa0: 6175 7365 2079 6f75 7220 626f 7420 6861  ause your bot ha
-00002fb0: 7320 6e6f 7420 6265 656e 2061 6464 6564  s not been added
-00002fc0: 2061 7320 6120 636f 6e6e 6563 7469 6f6e   as a connection
-00002fd0: 2074 6f20 7468 6520 7061 6765 2e20 0a0a   to the page. ..
-00002fe0: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00002ff0: 223e 0a20 2020 203c 696d 6720 7372 633d  ">.    <img src=
-00003000: 2265 7861 6d70 6c65 732f 696d 6167 6573  "examples/images
-00003010: 2f64 6972 6563 746f 7279 5f61 6464 5f63  /directory_add_c
-00003020: 6f6e 6e65 6374 696f 6e73 2e70 6e67 223e  onnections.png">
-00003030: 2020 0a3c 2f70 3e0a 0a42 7920 6465 6661    .</p>..By defa
-00003040: 756c 742c 2061 2062 6f74 2077 696c 6c20  ult, a bot will 
-00003050: 6861 7665 2061 6363 6573 7320 746f 2074  have access to t
-00003060: 6865 2063 6869 6c64 7265 6e20 6f66 2061  he children of a
-00003070: 6e79 2050 6172 656e 7420 6f62 6a65 6374  ny Parent object
-00003080: 2069 7420 6861 7320 6163 6365 7373 2074   it has access t
-00003090: 6f6f 2e20 4265 2073 7572 6520 746f 2064  oo. Be sure to d
-000030a0: 6f75 626c 6520 6368 6563 6b20 7468 6973  ouble check this
-000030b0: 2063 6f6e 6e65 6374 696f 6e20 7768 656e   connection when
-000030c0: 206d 6f76 696e 6720 7061 6765 732e 2020   moving pages.  
-000030d0: 0a49 6620 796f 7527 7265 2077 6f72 6b69  .If you're worki
-000030e0: 6e67 206f 6e20 6120 7061 6765 2074 6861  ng on a page tha
-000030f0: 7420 796f 7572 2074 6f6b 656e 2068 6173  t your token has
-00003100: 2061 6363 6573 7320 746f 2076 6961 2069   access to via i
-00003110: 7473 2070 6172 656e 7420 7061 6765 2f64  ts parent page/d
-00003120: 6174 6162 6173 652c 2062 7574 2079 6f75  atabase, but you
-00003130: 206e 6576 6572 2065 7870 6c69 6369 746c   never explicitl
-00003140: 7920 6772 616e 7465 6420 6163 6365 7373  y granted access
-00003150: 2074 6f20 7468 6520 6368 696c 6420 7061   to the child pa
-00003160: 6765 202d 2020 616e 6420 796f 7520 6c61  ge -  and you la
-00003170: 7465 7220 6d6f 7665 2074 6861 7420 6368  ter move that ch
-00003180: 696c 6420 7061 6765 206f 7574 2c20 7468  ild page out, th
-00003190: 656e 2069 7420 7769 6c6c 206c 6f73 6520  en it will lose 
-000031a0: 6163 6365 7373 2e0a 0a2d 2d2d 0a         access...---.
+00000b70: 2020 0a52 4541 444d 4520 636f 6e74 6169    .README contai
+00000b80: 6e73 2065 7861 6d70 6c65 7320 6f66 2074  ns examples of t
+00000b90: 6865 206d 6169 6e20 6675 6e63 7469 6f6e  he main function
+00000ba0: 616c 6974 792c 2069 6e63 6c75 6469 6e67  ality, including
+00000bb0: 3a20 6372 6561 7469 6e67 2050 6167 6573  : creating Pages
+00000bc0: 2f44 6174 6162 6173 6573 2f42 6c6f 636b  /Databases/Block
+00000bd0: 732c 2061 6464 696e 672f 7265 6d6f 7669  s, adding/removi
+00000be0: 6e67 2f65 6469 7469 6e67 2070 726f 7065  ng/editing prope
+00000bf0: 7274 6965 732c 2072 6574 7269 6576 696e  rties, retrievin
+00000c00: 6720 7072 6f70 6572 7479 2076 616c 7565  g property value
+00000c10: 732c 2061 6e64 2064 6174 6162 6173 6520  s, and database 
+00000c20: 7175 6572 6965 732e 2020 0a53 6f6d 6520  queries.  .Some 
+00000c30: 6d6f 7265 2069 6e2d 6465 7074 6820 7761  more in-depth wa
+00000c40: 6c6b 7468 726f 7567 6873 2063 616e 2062  lkthroughs can b
+00000c50: 6520 6265 2066 6f75 6e64 2069 6e20 6065  e be found in `e
+00000c60: 7861 6d70 6c65 732f 6020 2020 200a 5468  xamples/`    .Th
+00000c70: 6973 2070 6163 6b61 6765 2069 7320 6e6f  is package is no
+00000c80: 7420 636f 6d70 6c65 7465 202d 206e 6577  t complete - new
+00000c90: 2066 6561 7475 7265 7320 7769 6c6c 2063   features will c
+00000ca0: 6f6e 7469 6e75 6520 746f 2062 6520 6164  ontinue to be ad
+00000cb0: 6465 642c 2061 6e64 2063 7572 7265 6e74  ded, and current
+00000cc0: 2066 6561 7475 7265 7320 6d61 7920 6368   features may ch
+00000cd0: 616e 6765 2e0a 0a3c 6272 3e0a 0a3c 6469  ange...<br>..<di
+00000ce0: 7620 626f 7264 6572 3d22 3022 2061 6c69  v border="0" ali
+00000cf0: 676e 3d22 6365 6e74 6572 223e 0a20 2020  gn="center">.   
+00000d00: 203c 7461 626c 653e 0a20 2020 2020 2020   <table>.       
+00000d10: 203c 7472 3e0a 2020 2020 2020 2020 2020   <tr>.          
+00000d20: 2020 3c74 6420 616c 6967 6e3d 2263 656e    <td align="cen
+00000d30: 7465 7222 3e3c 623e 4c69 6e6b 733a 204e  ter"><b>Links: N
+00000d40: 6f74 696f 6e20 4150 4920 5570 6461 7465  otion API Update
+00000d50: 733c 2f62 3e3c 2f74 643e 0a20 2020 2020  s</b></td>.     
+00000d60: 2020 203c 2f74 723e 0a20 2020 2020 2020     </tr>.       
+00000d70: 2020 2020 203c 7464 3e20 3c61 2068 7265       <td> <a hre
+00000d80: 663d 2268 7474 7073 3a2f 2f64 6576 656c  f="https://devel
+00000d90: 6f70 6572 732e 6e6f 7469 6f6e 2e63 6f6d  opers.notion.com
+00000da0: 2f72 6566 6572 656e 6365 2f69 6e74 726f  /reference/intro
+00000db0: 223e 4150 4920 5265 6665 7265 6e63 653c  ">API Reference<
+00000dc0: 2f61 3e3c 2f74 643e 3c74 723e 0a20 2020  /a></td><tr>.   
+00000dd0: 2020 2020 203c 2f74 643e 0a20 2020 2020       </td>.     
+00000de0: 2020 2020 2020 203c 7464 3e3c 6120 6872         <td><a hr
+00000df0: 6566 3d22 6874 7470 733a 2f2f 6465 7665  ef="https://deve
+00000e00: 6c6f 7065 7273 2e6e 6f74 696f 6e2e 636f  lopers.notion.co
+00000e10: 6d2f 7061 6765 2f63 6861 6e67 656c 6f67  m/page/changelog
+00000e20: 223e 4e6f 7469 6f6e 2041 5049 2043 6861  ">Notion API Cha
+00000e30: 6e67 656c 6f67 203c 2f69 6d67 3e3c 2f61  ngelog </img></a
+00000e40: 3e3c 2f74 723e 0a20 2020 2020 2020 2020  ></tr>.         
+00000e50: 2020 203c 7464 3e20 3c61 2068 7265 663d     <td> <a href=
+00000e60: 2268 7474 7073 3a2f 2f77 7777 2e6e 6f74  "https://www.not
+00000e70: 696f 6e2e 736f 2f72 656c 6561 7365 7322  ion.so/releases"
+00000e80: 3e4e 6f74 696f 6e2e 736f 2052 656c 6561  >Notion.so Relea
+00000e90: 7365 733c 2f61 3e3c 2f74 643e 3c2f 7472  ses</a></td></tr
+00000ea0: 3e0a 2020 2020 2020 2020 2020 2020 3c74  >.            <t
+00000eb0: 643e 203c 6120 6872 6566 3d22 6874 7470  d> <a href="http
+00000ec0: 733a 2f2f 6465 7665 6c6f 7065 7273 2e6e  s://developers.n
+00000ed0: 6f74 696f 6e2e 636f 6d2f 7061 6765 2f6e  otion.com/page/n
+00000ee0: 6f74 696f 6e2d 706c 6174 666f 726d 2d72  otion-platform-r
+00000ef0: 6f61 646d 6170 223e 4e6f 7469 6f6e 2050  oadmap">Notion P
+00000f00: 6c61 7466 6f72 6d20 526f 6164 6d61 703c  latform Roadmap<
+00000f10: 2f61 3e3c 2f74 643e 0a20 2020 2020 2020  /a></td>.       
+00000f20: 203c 2f74 723e 0a20 2020 203c 2f74 6162   </tr>.    </tab
+00000f30: 6c65 3e0a 3c2f 6469 763e 0a0a 2d2d 2d0a  le>.</div>..---.
+00000f40: 0a23 2320 496e 7374 616c 6c0a 6060 600a  .## Install.```.
+00000f50: 7069 7020 696e 7374 616c 6c20 2d55 206e  pip install -U n
+00000f60: 6f74 696f 6e2d 6170 690a 6060 600a 0a23  otion-api.```..#
+00000f70: 2320 5573 6167 650a 6060 6070 790a 696d  # Usage.```py.im
+00000f80: 706f 7274 2064 6f74 656e 760a 0a69 6d70  port dotenv..imp
+00000f90: 6f72 7420 6e6f 7469 6f6e 0a0a 2320 636c  ort notion..# cl
+00000fa0: 6965 6e74 2077 696c 6c20 6368 6563 6b20  ient will check 
+00000fb0: 656e 7620 7661 7269 6162 6c65 7320 666f  env variables fo
+00000fc0: 7220 274e 4f54 494f 4e5f 544f 4b45 4e27  r 'NOTION_TOKEN'
+00000fd0: 0a64 6f74 656e 762e 6c6f 6164 5f64 6f74  .dotenv.load_dot
+00000fe0: 656e 7628 2920 200a 0a68 6f6d 6570 6167  env()  ..homepag
+00000ff0: 6520 3d20 6e6f 7469 6f6e 2e50 6167 6528  e = notion.Page(
+00001000: 2737 3733 6230 3866 6633 3862 3434 3532  '773b08ff38b4452
+00001010: 3162 3434 6231 3135 3832 3765 3835 3066  1b44b115827e850f
+00001020: 3227 290a 7061 7265 6e74 5f64 6220 3d20  2').parent_db = 
+00001030: 6e6f 7469 6f6e 2e44 6174 6162 6173 6528  notion.Database(
+00001040: 686f 6d65 7061 6765 2e70 6172 656e 745f  homepage.parent_
+00001050: 6964 290a 0a23 2077 696c 6c20 616c 736f  id)..# will also
+00001060: 206c 6f6f 6b20 666f 7220 656e 7620 7661   look for env va
+00001070: 7220 6054 5a60 2074 6f20 7365 7420 7468  r `TZ` to set th
+00001080: 6520 7469 6d65 7a6f 6e65 2066 6f72 2061  e timezone for a
+00001090: 6c6c 206e 6f74 696f 6e20 6f62 6a65 6374  ll notion object
+000010a0: 732e 2049 6620 6e6f 7420 666f 756e 642c  s. If not found,
+000010b0: 2077 696c 6c20 6465 6661 756c 7420 746f   will default to
+000010c0: 206c 6f63 616c 2074 696d 657a 6f6e 652e   local timezone.
+000010d0: 0a60 6060 0a0a 605f 5f67 6574 6974 656d  .```..`__getitem
+000010e0: 5f5f 6020 7365 6172 6368 7320 666f 7220  __` searchs for 
+000010f0: 7061 6765 2070 726f 7065 7274 7920 7661  page property va
+00001100: 6c75 6573 2077 6865 6e20 696e 6465 7869  lues when indexi
+00001110: 6e67 2061 2050 6167 652c 2061 6e64 2066  ng a Page, and f
+00001120: 6f72 2070 726f 7065 7274 7920 6f62 6a65  or property obje
+00001130: 6374 7320 7768 656e 2069 6e64 6578 696e  cts when indexin
+00001140: 6720 6120 4461 7461 6261 7365 2e0a 0a60  g a Database...`
+00001150: 6060 7079 0a68 6f6d 6570 6167 655b 2764  ``py.homepage['d
+00001160: 6570 656e 6465 6e63 6965 7327 5d0a 2320  ependencies'].# 
+00001170: 7b0a 2320 2020 2020 2269 6422 3a20 2257  {.#     "id": "W
+00001180: 5959 7122 2c0a 2320 2020 2020 2274 7970  YYq",.#     "typ
+00001190: 6522 3a20 2272 656c 6174 696f 6e22 2c0a  e": "relation",.
+000011a0: 2320 2020 2020 2272 656c 6174 696f 6e22  #     "relation"
+000011b0: 3a20 5b0a 2320 2020 2020 2020 2020 7b0a  : [.#         {.
+000011c0: 2320 2020 2020 2020 2020 2020 2020 2269  #             "i
+000011d0: 6422 3a20 2237 6263 6263 3865 362d 6532  d": "7bcbc8e6-e2
+000011e0: 3337 2d34 3334 622d 6264 3064 2d36 6235  37-434b-bd0d-6b5
+000011f0: 3665 3034 3432 3030 6222 0a23 2020 2020  6e044200b".#    
+00001200: 2020 2020 207d 0a23 2020 2020 205d 2c0a       }.#     ],.
+00001210: 2320 2020 2020 2268 6173 5f6d 6f72 6522  #     "has_more"
+00001220: 3a20 6661 6c73 650a 2320 7d0a 0a70 6172  : false.# }..par
+00001230: 656e 745f 6462 5b27 6465 7065 6e64 656e  ent_db['dependen
+00001240: 6369 6573 275d 0a23 207b 0a23 2020 2020  cies'].# {.#    
+00001250: 2022 6964 223a 2022 5759 5971 222c 0a23   "id": "WYYq",.#
+00001260: 2020 2020 2022 6e61 6d65 223a 2022 6465       "name": "de
+00001270: 7065 6e64 656e 6369 6573 222c 0a23 2020  pendencies",.#  
+00001280: 2020 2022 7479 7065 223a 2022 7265 6c61     "type": "rela
+00001290: 7469 6f6e 222c 0a23 2020 2020 2022 7265  tion",.#     "re
+000012a0: 6c61 7469 6f6e 223a 207b 0a23 2020 2020  lation": {.#    
+000012b0: 2020 2020 2022 6461 7461 6261 7365 5f69       "database_i
+000012c0: 6422 3a20 2266 3539 3834 6137 652d 3232  d": "f5984a7e-22
+000012d0: 3537 2d34 6162 302d 3964 3061 2d32 3365  57-4ab0-9d0a-23e
+000012e0: 6131 3233 3234 3033 3122 2c0a 2320 2020  a12324031",.#   
+000012f0: 2020 2020 2020 2274 7970 6522 3a20 2264        "type": "d
+00001300: 7561 6c5f 7072 6f70 6572 7479 222c 0a23  ual_property",.#
+00001310: 2020 2020 2020 2020 2022 6475 616c 5f70           "dual_p
+00001320: 726f 7065 7274 7922 3a20 7b0a 2320 2020  roperty": {.#   
+00001330: 2020 2020 2020 2020 2020 2273 796e 6365            "synce
+00001340: 645f 7072 6f70 6572 7479 5f6e 616d 6522  d_property_name"
+00001350: 3a20 2262 6c6f 636b 6564 222c 0a23 2020  : "blocked",.#  
+00001360: 2020 2020 2020 2020 2020 2022 7379 6e63             "sync
+00001370: 6564 5f70 726f 7065 7274 795f 6964 223a  ed_property_id":
+00001380: 2022 7778 2537 4451 220a 2320 2020 2020   "wx%7DQ".#     
+00001390: 2020 2020 7d0a 2320 2020 2020 7d0a 2320      }.#     }.# 
+000013a0: 7d0a 6060 600a 0a2a 2a5f 5365 6520 7573  }.```..**_See us
+000013b0: 6167 6520 6f66 2072 6574 7269 6576 696e  age of retrievin
+000013c0: 6720 7661 6c75 6573 2066 726f 6d20 6120  g values from a 
+000013d0: 7061 6765 2069 6e20 6578 616d 706c 6573  page in examples
+000013e0: 2f72 6574 7269 6576 696e 672d 7072 6f70  /retrieving-prop
+000013f0: 6572 7479 2d69 7465 6d73 2e6d 645f 2a2a  erty-items.md_**
+00001400: 2020 0a0a 4265 6c6f 7720 6973 2061 2062    ..Below is a b
+00001410: 7269 6566 2065 7861 6d70 6c65 2069 6620  rief example if 
+00001420: 7765 2077 6572 6520 7761 6e74 696e 6720  we were wanting 
+00001430: 746f 2067 6574 2074 6865 2070 6167 6520  to get the page 
+00001440: 6964 2066 726f 6d20 7468 6520 6162 6f76  id from the abov
+00001450: 6520 7072 6f70 6572 7479 2060 6465 7065  e property `depe
+00001460: 6e64 656e 6369 6573 6020 696e 2060 686f  ndencies` in `ho
+00001470: 6d65 7061 6765 602e 0a0a 6060 6070 790a  mepage`...```py.
+00001480: 6672 6f6d 206e 6f74 696f 6e20 696d 706f  from notion impo
+00001490: 7274 2070 726f 7065 7274 7969 7465 6d73  rt propertyitems
+000014a0: 0a0a 7265 6c61 7465 645f 6964 3a20 6c69  ..related_id: li
+000014b0: 7374 5b73 7472 5d20 3d20 7072 6f70 6572  st[str] = proper
+000014c0: 7479 6974 656d 732e 7265 6c61 7469 6f6e  tyitems.relation
+000014d0: 2868 6f6d 6570 6167 652e 6465 7065 6e64  (homepage.depend
+000014e0: 656e 6369 6573 290a 6060 600a 6060 6070  encies).```.```p
+000014f0: 790a 3e3e 3e20 5b22 3762 6362 6338 6536  y.>>> ["7bcbc8e6
+00001500: 2d65 3233 372d 3433 3462 2d62 6430 642d  -e237-434b-bd0d-
+00001510: 3662 3536 6530 3434 3230 3062 225d 0a60  6b56e044200b"].`
+00001520: 6060 0a0a 426f 7468 2050 6167 6527 7320  ``..Both Page's 
+00001530: 616e 6420 4461 7461 6261 7365 2773 2068  and Database's h
+00001540: 6176 6520 7365 7474 6572 7320 666f 7220  ave setters for 
+00001550: 7469 746c 652f 6963 6f6e 2f63 6f76 6572  title/icon/cover
+00001560: 2e0a 0a60 6060 7079 0a68 6f6d 6570 6167  ...```py.homepag
+00001570: 652e 7469 746c 6520 3d20 226e 6577 2070  e.title = "new p
+00001580: 6167 6522 0a68 6f6d 6570 6167 652e 636f  age".homepage.co
+00001590: 7665 7220 3d20 2268 7474 7073 3a2f 2f77  ver = "https://w
+000015a0: 7777 2e6e 6f74 696f 6e2e 736f 2f69 6d61  ww.notion.so/ima
+000015b0: 6765 732f 7061 6765 2d63 6f76 6572 2f77  ges/page-cover/w
+000015c0: 6562 6231 2e6a 7067 220a 686f 6d65 7061  ebb1.jpg".homepa
+000015d0: 6765 2e69 636f 6e20 3d20 2268 7474 7073  ge.icon = "https
+000015e0: 3a2f 2f77 7777 2e6e 6f74 696f 6e2e 736f  ://www.notion.so
+000015f0: 2f69 636f 6e73 2f61 6c69 656e 2d70 6978  /icons/alien-pix
+00001600: 656c 5f70 7572 706c 652e 7376 6722 0a60  el_purple.svg".`
+00001610: 6060 0a0a 3c70 2061 6c69 676e 3d22 6365  ``..<p align="ce
+00001620: 6e74 6572 223e 203c 696d 6720 7372 633d  nter"> <img src=
+00001630: 2265 7861 6d70 6c65 732f 696d 6167 6573  "examples/images
+00001640: 2f6e 6577 5f70 6167 652e 706e 6722 3e20  /new_page.png"> 
+00001650: 3c2f 703e 0a0a 3c62 723e 0a0a 2323 2043  </p>..<br>..## C
+00001660: 7265 6174 696e 6720 5061 6765 732f 4461  reating Pages/Da
+00001670: 7461 6261 7365 732f 426c 6f63 6b73 0a0a  tabases/Blocks..
+00001680: 5468 6520 6375 7272 656e 7420 7665 7273  The current vers
+00001690: 696f 6e20 6f66 2074 6865 204e 6f74 696f  ion of the Notio
+000016a0: 6e20 6170 6920 646f 6573 206e 6f74 2061  n api does not a
+000016b0: 6c6c 6f77 2070 6167 6573 2074 6f20 6265  llow pages to be
+000016c0: 2063 7265 6174 6564 2074 6f20 7468 6520   created to the 
+000016d0: 7061 7265 6e74 2060 776f 726b 7370 6163  parent `workspac
+000016e0: 6560 2e20 200a 4372 6561 7465 206f 626a  e`.  .Create obj
+000016f0: 6563 7473 2062 7920 7061 7373 696e 6720  ects by passing 
+00001700: 616e 2065 7869 7374 696e 6720 5061 6765  an existing Page
+00001710: 2f44 6174 6162 6173 6520 696e 7374 616e  /Database instan
+00001720: 6365 2061 7320 616e 2061 7267 2074 6f20  ce as an arg to 
+00001730: 7468 6520 6063 7265 6174 6560 2063 6c61  the `create` cla
+00001740: 7373 6d65 7468 6f64 732e 0a0a 6060 6070  ssmethods...```p
+00001750: 790a 6e65 775f 6461 7461 6261 7365 203d  y.new_database =
+00001760: 206e 6f74 696f 6e2e 4461 7461 6261 7365   notion.Database
+00001770: 2e63 7265 6174 6528 0a20 2020 2070 6172  .create(.    par
+00001780: 656e 745f 696e 7374 616e 6365 3d74 6573  ent_instance=tes
+00001790: 7470 6167 652c 0a20 2020 2064 6174 6162  tpage,.    datab
+000017a0: 6173 655f 7469 746c 653d 2245 7861 6d70  ase_title="Examp
+000017b0: 6c65 2044 6174 6162 6173 6522 2c0a 2020  le Database",.  
+000017c0: 2020 6e61 6d65 5f63 6f6c 756d 6e3d 2270    name_column="p
+000017d0: 6167 6522 2c20 2320 5468 6973 2069 7320  age", # This is 
+000017e0: 7468 6520 636f 6c75 6d6e 2063 6f6e 7461  the column conta
+000017f0: 696e 696e 6720 7061 6765 206e 616d 6573  ining page names
+00001800: 2e20 4465 6661 756c 7473 2074 6f20 224e  . Defaults to "N
+00001810: 616d 6522 2e0a 2020 2020 6973 5f69 6e6c  ame"..    is_inl
+00001820: 696e 653d 5472 7565 2c20 2320 6361 6e20  ine=True, # can 
+00001830: 616c 736f 2074 6f67 676c 6520 696e 6c69  also toggle inli
+00001840: 6e65 2077 6974 6820 7365 7474 6572 732e  ne with setters.
+00001850: 0a20 2020 2064 6573 6372 6970 7469 6f6e  .    description
+00001860: 3d22 4461 7461 6261 7365 2064 6573 6372  ="Database descr
+00001870: 6970 7469 6f6e 2063 616e 2067 6f20 6865  iption can go he
+00001880: 7265 2e22 2c0a 290a 0a6e 6577 5f70 6167  re.",.)..new_pag
+00001890: 6520 3d20 6e6f 7469 6f6e 2e50 6167 652e  e = notion.Page.
+000018a0: 6372 6561 7465 286e 6577 5f64 6174 6162  create(new_datab
+000018b0: 6173 652c 2070 6167 655f 7469 746c 653d  ase, page_title=
+000018c0: 2241 206e 6577 2064 6174 6162 6173 6520  "A new database 
+000018d0: 726f 7722 290a 6060 600a 0a42 6c6f 636b  row").```..Block
+000018e0: 7320 6172 6520 616c 736f 2063 7265 6174  s are also creat
+000018f0: 6564 2075 7369 6e67 2074 6865 2063 6c61  ed using the cla
+00001900: 7373 6d65 7468 6f64 7320 6f66 2060 426c  ssmethods of `Bl
+00001910: 6f63 6b60 2e20 5468 6579 2061 6c6c 2072  ock`. They all r
+00001920: 6571 7569 7265 2061 2070 6172 656e 7420  equire a parent 
+00001930: 696e 7374 616e 6365 206f 6620 6569 7468  instance of eith
+00001940: 6572 2060 5061 6765 6020 6f72 2060 426c  er `Page` or `Bl
+00001950: 6f63 6b60 2074 6f20 6170 7065 6e64 2074  ock` to append t
+00001960: 6865 206e 6577 2062 6c6f 636b 2074 6f6f  he new block too
+00001970: 2e0a 5468 6520 6e65 776c 7920 6372 6561  ..The newly crea
+00001980: 7465 6420 626c 6f63 6b20 6973 2072 6574  ted block is ret
+00001990: 7572 6e65 6420 6173 2061 6e20 696e 7374  urned as an inst
+000019a0: 616e 6365 206f 6620 6042 6c6f 636b 602c  ance of `Block`,
+000019b0: 2077 6869 6368 2063 616e 2062 6520 7573   which can be us
+000019c0: 6564 2061 7320 7468 6520 7061 7265 6e74  ed as the parent
+000019d0: 2069 6e73 7461 6e63 6520 746f 2061 206e   instance to a n
+000019e0: 6573 7465 6420 626c 6f63 6b2e 200a 6060  ested block. .``
+000019f0: 6070 790a 6672 6f6d 206e 6f74 696f 6e20  `py.from notion 
+00001a00: 696d 706f 7274 2070 726f 7065 7274 6965  import propertie
+00001a10: 7320 6173 2070 726f 700a 0a23 2060 6f72  s as prop..# `or
+00001a20: 6967 696e 616c 5f73 796e 6365 645f 626c  iginal_synced_bl
+00001a30: 6f63 6b60 2072 6566 6572 7320 746f 2074  ock` refers to t
+00001a40: 6865 206f 7269 6769 6e61 6c20 7379 6e63  he original sync
+00001a50: 6564 2062 6c6f 636b 2069 6e20 7468 6520  ed block in the 
+00001a60: 4e6f 7469 6f6e 2055 492e 0a6f 7269 6769  Notion UI..origi
+00001a70: 6e61 6c5f 7379 6e63 6564 5f62 6c6f 636b  nal_synced_block
+00001a80: 203d 206e 6f74 696f 6e2e 426c 6f63 6b2e   = notion.Block.
+00001a90: 6f72 6967 696e 616c 5f73 796e 6365 645f  original_synced_
+00001aa0: 626c 6f63 6b28 686f 6d65 7061 6765 290a  block(homepage).
+00001ab0: 0a23 2041 6464 696e 6720 636f 6e74 656e  .# Adding conten
+00001ac0: 7420 746f 2074 6865 2073 796e 6365 6420  t to the synced 
+00001ad0: 626c 6f63 6b0a 6e6f 7469 6f6e 2e42 6c6f  block.notion.Blo
+00001ae0: 636b 2e70 6172 6167 7261 7068 286f 7269  ck.paragraph(ori
+00001af0: 6769 6e61 6c5f 7379 6e63 6564 5f62 6c6f  ginal_synced_blo
+00001b00: 636b 2c20 5b70 726f 702e 5269 6368 5465  ck, [prop.RichTe
+00001b10: 7874 2822 5468 6973 2069 7320 6120 7379  xt("This is a sy
+00001b20: 6e63 6564 2062 6c6f 636b 2e22 295d 290a  nced block.")]).
+00001b30: 0a23 2052 6566 6572 656e 6369 6e67 2074  .# Referencing t
+00001b40: 6865 2073 796e 6365 6420 626c 6f63 6b20  he synced block 
+00001b50: 696e 2061 206e 6577 2070 6167 652e 0a6e  in a new page..n
+00001b60: 6f74 696f 6e2e 426c 6f63 6b2e 6475 706c  otion.Block.dupl
+00001b70: 6963 6174 655f 7379 6e63 6564 5f62 6c6f  icate_synced_blo
+00001b80: 636b 286e 6577 5f70 6167 652c 206f 7269  ck(new_page, ori
+00001b90: 6769 6e61 6c5f 7379 6e63 6564 5f62 6c6f  ginal_synced_blo
+00001ba0: 636b 2e69 6429 0a60 6060 0a0a 3c62 723e  ck.id).```..<br>
+00001bb0: 0a0a 5468 6572 6520 6172 6520 6665 7720  ..There are few 
+00001bc0: 6578 7465 6e73 696f 6e73 2074 6f20 7468  extensions to th
+00001bd0: 6520 6042 6c6f 636b 6020 636c 6173 7320  e `Block` class 
+00001be0: 7468 6174 2068 6176 6520 7370 6563 6966  that have specif
+00001bf0: 6963 2066 756e 6374 696f 6e73 2075 6e69  ic functions uni
+00001c00: 7175 6520 746f 2074 6865 6972 2062 6c6f  que to their blo
+00001c10: 636b 2d74 7970 652e 2020 0a42 656c 6f77  ck-type.  .Below
+00001c20: 2069 7320 616e 2065 7861 6d70 6c65 2075   is an example u
+00001c30: 7369 6e67 2060 436f 6465 426c 6f63 6b60  sing `CodeBlock`
+00001c40: 2e20 5468 6520 6f74 6865 7273 2061 7265  . The others are
+00001c50: 2060 5461 626c 6542 6c6f 636b 602c 2060   `TableBlock`, `
+00001c60: 4571 7561 7469 6f6e 426c 6f63 6b60 2c20  EquationBlock`, 
+00001c70: 6052 6963 6854 6578 7442 6c6f 636b 602c  `RichTextBlock`,
+00001c80: 2061 6e64 2060 546f 446f 426c 6f63 6b60   and `ToDoBlock`
+00001c90: 2e20 596f 7520 6361 6e20 7365 6520 7573  . You can see us
+00001ca0: 6167 6520 666f 7220 7468 656d 2069 6e20  age for them in 
+00001cb0: 6065 7861 6d70 6c65 732f 626c 6f63 6b5f  `examples/block_
+00001cc0: 6578 7465 6e73 696f 6e73 2e6d 6460 2e0a  extensions.md`..
+00001cd0: 0a60 6060 7079 0a63 6f64 655f 626c 6f63  .```py.code_bloc
+00001ce0: 6b20 3d20 6e6f 7469 6f6e 2e43 6f64 6542  k = notion.CodeB
+00001cf0: 6c6f 636b 2822 3834 6335 3732 3164 3861  lock("84c5721d8a
+00001d00: 3935 3436 3637 3930 3261 3735 3766 3030  954667902a757f00
+00001d10: 3333 6639 6530 2229 0a0a 636c 6173 735f  33f9e0")..class_
+00001d20: 6469 6167 7261 6d20 3d20 7222 2222 0a25  diagram = r""".%
+00001d30: 257b 696e 6974 3a20 7b20 276c 6f67 4c65  %{init: { 'logLe
+00001d40: 7665 6c27 3a20 2764 6562 7567 272c 2027  vel': 'debug', '
+00001d50: 7468 656d 6527 3a20 2764 6566 6175 6c74  theme': 'default
+00001d60: 2720 2c20 2774 6865 6d65 5661 7269 6162  ' , 'themeVariab
+00001d70: 6c65 7327 3a20 7b20 2764 6172 6b4d 6f64  les': { 'darkMod
+00001d80: 6527 3a27 7472 7565 272c 2027 6769 7430  e':'true', 'git0
+00001d90: 273a 2027 2366 6630 3030 3027 2c20 2767  ': '#ff0000', 'g
+00001da0: 6974 3127 3a20 2723 3030 6666 3030 272c  it1': '#00ff00',
+00001db0: 2027 6769 7432 273a 2027 2330 3030 3066   'git2': '#0000f
+00001dc0: 6627 2c20 2767 6974 3327 3a20 2723 6666  f', 'git3': '#ff
+00001dd0: 3030 6666 272c 2027 6769 7434 273a 2027  00ff', 'git4': '
+00001de0: 2330 3066 6666 6627 2c20 2767 6974 3527  #00ffff', 'git5'
+00001df0: 3a20 2723 6666 6666 3030 272c 2027 6769  : '#ffff00', 'gi
+00001e00: 7436 273a 2027 2366 6630 3066 6627 2c20  t6': '#ff00ff', 
+00001e10: 2767 6974 3727 3a20 2723 3030 6666 6666  'git7': '#00ffff
+00001e20: 2720 7d20 7d20 7d25 250a 6769 7447 7261  ' } } }%%.gitGra
+00001e30: 7068 0a20 2020 2020 2020 636f 6d6d 6974  ph.       commit
+00001e40: 0a20 2020 2020 2020 6272 616e 6368 2064  .       branch d
+00001e50: 6576 656c 6f70 0a20 2020 2020 2020 636f  evelop.       co
+00001e60: 6d6d 6974 2074 6167 3a22 7631 2e30 2e30  mmit tag:"v1.0.0
+00001e70: 220a 2020 2020 2020 2063 6f6d 6d69 740a  ".       commit.
+00001e80: 2020 2020 2020 2063 6865 636b 6f75 7420         checkout 
+00001e90: 6d61 696e 0a20 2020 2020 2020 636f 6d6d  main.       comm
+00001ea0: 6974 2074 7970 653a 2048 4947 484c 4947  it type: HIGHLIG
+00001eb0: 4854 0a20 2020 2020 2020 636f 6d6d 6974  HT.       commit
+00001ec0: 0a20 2020 2020 2020 6d65 7267 6520 6465  .       merge de
+00001ed0: 7665 6c6f 700a 2020 2020 2020 2063 6f6d  velop.       com
+00001ee0: 6d69 740a 2020 2020 2020 2062 7261 6e63  mit.       branc
+00001ef0: 6820 6665 6174 7572 6541 0a20 2020 2020  h featureA.     
+00001f00: 2020 636f 6d6d 6974 0a22 2222 0a0a 636f    commit."""..co
+00001f10: 6465 5f62 6c6f 636b 2e6c 616e 6775 6167  de_block.languag
+00001f20: 6520 3d20 7072 6f70 2e43 6f64 6542 6c6f  e = prop.CodeBlo
+00001f30: 636b 4c61 6e67 2e6d 6572 6d61 6964 0a63  ckLang.mermaid.c
+00001f40: 6f64 655f 626c 6f63 6b2e 636f 6465 203d  ode_block.code =
+00001f50: 2063 6c61 7373 5f64 6961 6772 616d 0a63   class_diagram.c
+00001f60: 6f64 655f 626c 6f63 6b2e 6361 7074 696f  ode_block.captio
+00001f70: 6e20 3d20 2245 7861 6d70 6c65 2066 726f  n = "Example fro
+00001f80: 6d20 6874 7470 733a 2f2f 6d65 726d 6169  m https://mermai
+00001f90: 642e 6a73 2e6f 7267 2f73 796e 7461 782f  d.js.org/syntax/
+00001fa0: 636c 6173 7344 6961 6772 616d 2e68 746d  classDiagram.htm
+00001fb0: 6c23 7379 6e74 6178 220a 6060 600a 0a3c  l#syntax".```..<
+00001fc0: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+00001fd0: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
+00001fe0: 6578 616d 706c 6573 2f69 6d61 6765 732f  examples/images/
+00001ff0: 636f 6465 5f63 6f6d 6d69 745f 6469 6167  code_commit_diag
+00002000: 7261 6d2e 706e 6722 3e0a 3c2f 703e 0a0a  ram.png">.</p>..
+00002010: 3c62 723e 0a0a 2a2a 5f45 7861 6d70 6c65  <br>..**_Example
+00002020: 2046 756e 6374 696f 6e3a 2055 7369 6e67   Function: Using
+00002030: 2060 6e6f 7469 6f6e 2e57 6f72 6b73 7061   `notion.Workspa
+00002040: 6365 2829 6020 746f 2072 6574 7269 6576  ce()` to retriev
+00002050: 6520 6120 7573 6572 2c20 616e 6420 6170  e a user, and ap
+00002060: 7065 6e64 696e 6720 626c 6f63 6b73 2069  pending blocks i
+00002070: 6e20 6120 7061 6765 2074 6f20 6d65 6e74  n a page to ment
+00002080: 696f 6e20 7573 6572 2f64 6174 652e 5f2a  ion user/date._*
+00002090: 2a0a 0a60 6060 7079 0a64 6566 2069 6e6c  *..```py.def inl
+000020a0: 696e 655f 6d65 6e74 696f 6e28 7061 6765  ine_mention(page
+000020b0: 3a20 6e6f 7469 6f6e 2e50 6167 652c 206d  : notion.Page, m
+000020c0: 6573 7361 6765 3a20 7374 722c 2075 7365  essage: str, use
+000020d0: 725f 6e61 6d65 3a20 7374 7229 202d 3e20  r_name: str) -> 
+000020e0: 4e6f 6e65 3a0a 2020 2020 6d65 6e74 696f  None:.    mentio
+000020f0: 6e62 6c6f 636b 203d 206e 6f74 696f 6e2e  nblock = notion.
+00002100: 426c 6f63 6b2e 7061 7261 6772 6170 6828  Block.paragraph(
+00002110: 0a20 2020 2020 2020 2070 6167 652c 0a20  .        page,. 
+00002120: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+00002130: 2020 2020 2070 726f 702e 4d65 6e74 696f       prop.Mentio
+00002140: 6e2e 7573 6572 280a 2020 2020 2020 2020  n.user(.        
+00002150: 2020 2020 2020 2020 6e6f 7469 6f6e 2e57          notion.W
+00002160: 6f72 6b73 7061 6365 2829 2e72 6574 7269  orkspace().retri
+00002170: 6576 655f 7573 6572 2875 7365 725f 6e61  eve_user(user_na
+00002180: 6d65 3d75 7365 725f 6e61 6d65 292c 0a20  me=user_name),. 
+00002190: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000021a0: 6e6e 6f74 6174 696f 6e73 3d70 726f 702e  nnotations=prop.
+000021b0: 416e 6e6f 7461 7469 6f6e 7328 0a20 2020  Annotations(.   
+000021c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021d0: 2063 6f64 653d 5472 7565 2c20 626f 6c64   code=True, bold
+000021e0: 3d54 7275 652c 2063 6f6c 6f72 3d70 726f  =True, color=pro
+000021f0: 702e 426c 6f63 6b43 6f6c 6f72 2e70 7572  p.BlockColor.pur
+00002200: 706c 650a 2020 2020 2020 2020 2020 2020  ple.            
+00002210: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00002220: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
+00002230: 2020 7072 6f70 2e52 6963 6854 6578 7428    prop.RichText(
+00002240: 2220 2d20 2229 2c0a 2020 2020 2020 2020  " - "),.        
+00002250: 2020 2020 7072 6f70 2e4d 656e 7469 6f6e      prop.Mention
+00002260: 2e64 6174 6528 0a20 2020 2020 2020 2020  .date(.         
+00002270: 2020 2020 2020 2064 6174 6574 696d 652e         datetime.
+00002280: 6e6f 7728 292e 6173 7469 6d65 7a6f 6e65  now().astimezone
+00002290: 2870 6167 652e 747a 292e 6973 6f66 6f72  (page.tz).isofor
+000022a0: 6d61 7428 292c 0a20 2020 2020 2020 2020  mat(),.         
+000022b0: 2020 2020 2020 2061 6e6e 6f74 6174 696f         annotatio
+000022c0: 6e73 3d70 726f 702e 416e 6e6f 7461 7469  ns=prop.Annotati
+000022d0: 6f6e 7328 0a20 2020 2020 2020 2020 2020  ons(.           
+000022e0: 2020 2020 2020 2020 2063 6f64 653d 5472           code=Tr
+000022f0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00002300: 2020 2020 2020 2020 626f 6c64 3d54 7275          bold=Tru
+00002310: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00002320: 2020 2020 2020 2069 7461 6c69 633d 5472         italic=Tr
+00002330: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00002340: 2020 2020 2020 2020 756e 6465 726c 696e          underlin
+00002350: 653d 5472 7565 2c0a 2020 2020 2020 2020  e=True,.        
+00002360: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
+00002370: 723d 7072 6f70 2e42 6c6f 636b 436f 6c6f  r=prop.BlockColo
+00002380: 722e 6772 6179 2c0a 2020 2020 2020 2020  r.gray,.        
+00002390: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+000023a0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+000023b0: 2020 2020 2020 7072 6f70 2e52 6963 6854        prop.RichT
+000023c0: 6578 7428 223a 2229 2c0a 2020 2020 2020  ext(":"),.      
+000023d0: 2020 5d2c 0a20 2020 2029 0a20 2020 2023    ],.    ).    #
+000023e0: 2046 6972 7374 206d 6574 686f 6420 7265   First method re
+000023f0: 7475 726e 6564 2074 6865 206e 6577 6c79  turned the newly
+00002400: 2063 7265 6174 6564 2062 6c6f 636b 2074   created block t
+00002410: 6861 7420 7765 2061 7070 656e 6420 746f  hat we append to
+00002420: 2068 6572 653a 0a20 2020 206e 6f74 696f   here:.    notio
+00002430: 6e2e 426c 6f63 6b2e 7061 7261 6772 6170  n.Block.paragrap
+00002440: 6828 6d65 6e74 696f 6e62 6c6f 636b 2c20  h(mentionblock, 
+00002450: 5b70 726f 702e 5269 6368 5465 7874 286d  [prop.RichText(m
+00002460: 6573 7361 6765 295d 290a 2020 2020 6e6f  essage)]).    no
+00002470: 7469 6f6e 2e42 6c6f 636b 2e64 6976 6964  tion.Block.divid
+00002480: 6572 2870 6167 6529 0a60 6060 0a0a 6060  er(page).```..``
+00002490: 6070 790a 3e3e 3e20 686f 6d65 7061 6765  `py.>>> homepage
+000024a0: 203d 206e 6f74 696f 6e2e 5061 6765 2822   = notion.Page("
+000024b0: 3062 3965 6363 6661 3839 3065 3463 3333  0b9eccfa890e4c33
+000024c0: 3930 3137 3565 6531 3063 3636 3461 3335  90175ee10c664a35
+000024d0: 2229 0a3e 3e3e 2069 6e6c 696e 655f 6d65  ").>>> inline_me
+000024e0: 6e74 696f 6e28 7061 6765 3d68 6f6d 6570  ntion(page=homep
+000024f0: 6167 652c 206d 6573 7361 6765 3d22 6578  age, message="ex
+00002500: 616d 706c 6522 2c20 7573 6572 5f6e 616d  ample", user_nam
+00002510: 653d 2241 5956 4922 290a 6060 600a 3c70  e="AYVI").```.<p
+00002520: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00002530: 0a20 2020 203c 696d 6720 7372 633d 2265  .    <img src="e
+00002540: 7861 6d70 6c65 732f 696d 6167 6573 2f65  xamples/images/e
+00002550: 7861 6d70 6c65 5f66 756e 6374 696f 6e5f  xample_function_
+00002560: 7265 6d69 6e64 6572 2e70 6e67 223e 0a3c  reminder.png">.<
+00002570: 2f70 3e0a 0a3c 6272 3e0a 0a23 2320 4164  /p>..<br>..## Ad
+00002580: 642c 2053 6574 2c20 2620 4465 6c65 7465  d, Set, & Delete
+00002590: 3a20 5061 6765 2070 726f 7065 7274 7920  : Page property 
+000025a0: 7661 6c75 6573 207c 2044 6174 6162 6173  values | Databas
+000025b0: 6520 7072 6f70 6572 7479 206f 626a 6563  e property objec
+000025c0: 7473 0a0a 5468 6520 6669 7273 7420 6172  ts..The first ar
+000025d0: 6775 6d65 6e74 2066 6f72 2061 6c6c 2064  gument for all d
+000025e0: 6174 6162 6173 6520 7072 6f70 6572 7479  atabase property
+000025f0: 206d 6574 686f 6473 2069 7320 7468 6520   methods is the 
+00002600: 6e61 6d65 206f 6620 7468 6520 7072 6f70  name of the prop
+00002610: 6572 7479 2c20 200a 4966 2061 2070 726f  erty,  .If a pro
+00002620: 7065 7274 7920 6f66 2074 6861 7420 6e61  perty of that na
+00002630: 6d65 2064 6f65 7320 6e6f 7420 6578 6973  me does not exis
+00002640: 742c 2074 6865 6e20 6120 6e65 7720 7072  t, then a new pr
+00002650: 6f70 6572 7479 2077 696c 6c20 6265 2063  operty will be c
+00002660: 7265 6174 6564 2e20 0a49 6620 6120 7072  reated. .If a pr
+00002670: 6f70 6572 7479 206f 6620 7468 6174 206e  operty of that n
+00002680: 616d 6520 616c 7265 6164 7920 6578 6973  ame already exis
+00002690: 7473 2c20 6275 7420 6974 2773 2061 2064  ts, but it's a d
+000026a0: 6966 6665 7265 6e74 2074 7970 6520 7468  ifferent type th
+000026b0: 616e 2074 6865 206d 6574 686f 6420 7573  an the method us
+000026c0: 6564 202d 2074 6865 6e20 7468 6520 4150  ed - then the AP
+000026d0: 4920 7769 6c6c 206f 7665 7277 7269 7465  I will overwrite
+000026e0: 2074 6869 7320 616e 6420 6368 616e 6765   this and change
+000026f0: 2074 6865 2070 726f 7065 7274 7920 6f62   the property ob
+00002700: 6a65 6374 2074 6f20 7468 6520 6e65 7720  ject to the new 
+00002710: 7479 7065 2e20 200a 5468 6520 6f72 6967  type.  .The orig
+00002720: 696e 616c 2070 6172 616d 6574 6572 7320  inal parameters 
+00002730: 7769 6c6c 2062 6520 7361 7665 6420 6966  will be saved if
+00002740: 2079 6f75 2064 6563 6964 6520 746f 2073   you decide to s
+00002750: 7769 7463 6820 6261 636b 2028 692e 652e  witch back (i.e.
+00002760: 2069 6620 796f 7520 6368 616e 6765 2061   if you change a
+00002770: 2066 6f72 6d75 6c61 2063 6f6c 756d 6e20   formula column 
+00002780: 746f 2061 2073 656c 6563 7420 636f 6c75  to a select colu
+00002790: 6d6e 2c20 7570 6f6e 2063 6861 6e67 696e  mn, upon changin
+000027a0: 6720 6974 2062 6163 6b20 746f 2061 2066  g it back to a f
+000027b0: 6f72 6d75 6c61 2063 6f6c 756d 6e2c 2074  ormula column, t
+000027c0: 6865 206f 7269 6769 6e61 6c20 666f 726d  he original form
+000027d0: 756c 6120 6578 7072 6573 7369 6f6e 2077  ula expression w
+000027e0: 696c 6c20 7374 696c 6c20 6265 2074 6865  ill still be the
+000027f0: 7265 292e 2020 200a 0a60 6060 7079 0a6e  re).   ..```py.n
+00002800: 6577 5f64 6174 6162 6173 652e 666f 726d  ew_database.form
+00002810: 756c 615f 636f 6c75 6d6e 2822 7061 6765  ula_column("page
+00002820: 2069 6422 2c20 6578 7072 6573 7369 6f6e   id", expression
+00002830: 3d22 6964 2829 2229 0a0a 6e65 775f 6461  ="id()")..new_da
+00002840: 7461 6261 7365 2e64 656c 6574 655f 7072  tabase.delete_pr
+00002850: 6f70 6572 7479 2822 7572 6c22 290a 0a6e  operty("url")..n
+00002860: 6577 5f64 6174 6162 6173 652e 6d75 6c74  ew_database.mult
+00002870: 6973 656c 6563 745f 636f 6c75 6d6e 280a  iselect_column(.
+00002880: 2020 2020 226e 6577 206f 7074 696f 6e73      "new options
+00002890: 2063 6f6c 756d 6e22 2c0a 2020 2020 6f70   column",.    op
+000028a0: 7469 6f6e 733d 5b0a 2020 2020 2020 2020  tions=[.        
+000028b0: 7072 6f70 2e4f 7074 696f 6e28 226f 7074  prop.Option("opt
+000028c0: 696f 6e2d 6122 2c20 7072 6f70 2e50 726f  ion-a", prop.Pro
+000028d0: 7065 7274 7943 6f6c 6f72 2e72 6564 292c  pertyColor.red),
+000028e0: 0a20 2020 2020 2020 2070 726f 702e 4f70  .        prop.Op
+000028f0: 7469 6f6e 2822 6f70 7469 6f6e 2d62 222c  tion("option-b",
+00002900: 2070 726f 702e 5072 6f70 6572 7479 436f   prop.PropertyCo
+00002910: 6c6f 722e 6772 6565 6e29 2c0a 2020 2020  lor.green),.    
+00002920: 2020 2020 7072 6f70 2e4f 7074 696f 6e28      prop.Option(
+00002930: 226f 7074 696f 6e2d 6322 2c20 7072 6f70  "option-c", prop
+00002940: 2e50 726f 7065 7274 7943 6f6c 6f72 2e62  .PropertyColor.b
+00002950: 6c75 6529 2c0a 2020 2020 5d2c 0a29 0a0a  lue),.    ],.)..
+00002960: 2320 6966 2061 6e20 6f70 7469 6f6e 2064  # if an option d
+00002970: 6f65 7320 6e6f 7420 616c 7265 6164 7920  oes not already 
+00002980: 6578 6973 742c 2061 206e 6577 206f 6e65  exist, a new one
+00002990: 2077 696c 6c20 6265 2063 7265 6174 6564   will be created
+000029a0: 2077 6974 6820 6120 7261 6e64 6f6d 2063   with a random c
+000029b0: 6f6c 6f72 2e0a 2320 7468 6973 2069 7320  olor..# this is 
+000029c0: 6e6f 7420 7472 7565 2066 6f72 2060 7374  not true for `st
+000029d0: 6174 7573 6020 636f 6c75 6d6e 2074 7970  atus` column typ
+000029e0: 6573 2c20 7768 6963 6820 6361 6e20 6f6e  es, which can on
+000029f0: 6c79 2062 6520 6564 6974 6564 2076 6961  ly be edited via
+00002a00: 2055 492e 0a0a 6e65 775f 7061 6765 2e73   UI...new_page.s
+00002a10: 6574 5f6d 756c 7469 7365 6c65 6374 2822  et_multiselect("
+00002a20: 6f70 7469 6f6e 7322 2c20 5b22 6f70 7469  options", ["opti
+00002a30: 6f6e 2d61 222c 2022 6f70 7469 6f6e 2d62  on-a", "option-b
+00002a40: 225d 290a 6060 600a 0a3c 6272 3e0a 0a23  "]).```..<br>..#
+00002a50: 2320 4461 7461 6261 7365 2051 7565 7269  # Database Queri
+00002a60: 6573 0a0a 4120 7369 6e67 6c65 2060 6e6f  es..A single `no
+00002a70: 7469 6f6e 2e71 7565 7279 2e50 726f 7065  tion.query.Prope
+00002a80: 7274 7946 696c 7465 7260 2069 7320 6571  rtyFilter` is eq
+00002a90: 7569 7661 6c65 6e74 2074 6f20 6669 6c74  uivalent to filt
+00002aa0: 6572 696e 6720 6f6e 6520 7072 6f70 6572  ering one proper
+00002ab0: 7479 2074 7970 6520 696e 204e 6f74 696f  ty type in Notio
+00002ac0: 6e2e 0a54 6f20 6275 696c 6420 6669 6c74  n..To build filt
+00002ad0: 6572 7320 6571 7569 7661 6c65 6e74 2074  ers equivalent t
+00002ae0: 6f20 4e6f 7469 6f6e 2773 2027 6164 7661  o Notion's 'adva
+00002af0: 6e63 6564 2066 696c 7465 7273 272c 2075  nced filters', u
+00002b00: 7365 2060 6e6f 7469 6f6e 2e71 7565 7279  se `notion.query
+00002b10: 2e43 6f6d 706f 756e 6446 696c 7465 7260  .CompoundFilter`
+00002b20: 2e0a 0a54 6865 2064 6174 6162 6173 6520  ...The database 
+00002b30: 6d65 7468 6f64 2060 7175 6572 7928 2960  method `query()`
+00002b40: 2077 696c 6c20 7265 7475 726e 2074 6865   will return the
+00002b50: 2072 6177 2072 6573 706f 6e73 6520 6672   raw response fr
+00002b60: 6f6d 2074 6865 2041 5049 2e20 200a 5468  om the API.  .Th
+00002b70: 6520 6d65 7468 6f64 2060 7175 6572 795f  e method `query_
+00002b80: 7061 6765 7328 2960 2077 696c 6c20 6578  pages()` will ex
+00002b90: 7472 6163 7420 7468 6520 7061 6765 2049  tract the page I
+00002ba0: 4420 666f 7220 6561 6368 206f 626a 6563  D for each objec
+00002bb0: 7420 696e 2074 6865 2061 7272 6179 206f  t in the array o
+00002bc0: 6620 7265 7375 6c74 732c 2061 6e64 2072  f results, and r
+00002bd0: 6574 7572 6e20 6120 6c69 7374 206f 6620  eturn a list of 
+00002be0: 606e 6f74 696f 6e2e 5061 6765 6020 6f62  `notion.Page` ob
+00002bf0: 6a65 6374 732e 0a0a 6060 6070 790a 6672  jects...```py.fr
+00002c00: 6f6d 2064 6174 6574 696d 6520 696d 706f  om datetime impo
+00002c10: 7274 2064 6174 6574 696d 650a 6672 6f6d  rt datetime.from
+00002c20: 2064 6174 6574 696d 6520 696d 706f 7274   datetime import
+00002c30: 2074 696d 6564 656c 7461 0a0a 6672 6f6d   timedelta..from
+00002c40: 206e 6f74 696f 6e20 696d 706f 7274 2071   notion import q
+00002c50: 7565 7279 0a0a 544f 4441 5920 3d20 6461  uery..TODAY = da
+00002c60: 7465 7469 6d65 2e63 6f6d 6269 6e65 2864  tetime.combine(d
+00002c70: 6174 6574 696d 652e 746f 6461 7928 292c  atetime.today(),
+00002c80: 2064 6174 6574 696d 652e 6d69 6e2e 7469   datetime.min.ti
+00002c90: 6d65 2829 290a 544f 4d4f 5252 4f57 203d  me()).TOMORROW =
+00002ca0: 2054 4f44 4159 202b 2074 696d 6564 656c   TODAY + timedel
+00002cb0: 7461 2831 290a 0a71 7565 7279 5f66 696c  ta(1)..query_fil
+00002cc0: 7465 7220 3d20 7175 6572 792e 436f 6d70  ter = query.Comp
+00002cd0: 6f75 6e64 4669 6c74 6572 2829 2e5f 616e  oundFilter()._an
+00002ce0: 6428 0a20 2020 2071 7565 7279 2e50 726f  d(.    query.Pro
+00002cf0: 7065 7274 7946 696c 7465 722e 6461 7465  pertyFilter.date
+00002d00: 2822 6461 7465 222c 2022 6372 6561 7465  ("date", "create
+00002d10: 645f 7469 6d65 222c 2022 6f6e 5f6f 725f  d_time", "on_or_
+00002d20: 6166 7465 7222 2c20 544f 4441 592e 6973  after", TODAY.is
+00002d30: 6f66 6f72 6d61 7428 2929 2c0a 2020 2020  oformat()),.    
+00002d40: 7175 6572 792e 5072 6f70 6572 7479 4669  query.PropertyFi
+00002d50: 6c74 6572 2e64 6174 6528 2264 6174 6522  lter.date("date"
+00002d60: 2c20 2263 7265 6174 6564 5f74 696d 6522  , "created_time"
+00002d70: 2c20 2262 6566 6f72 6522 2c20 544f 4d4f  , "before", TOMO
+00002d80: 5252 4f57 2e69 736f 666f 726d 6174 2829  RROW.isoformat()
+00002d90: 292c 0a20 2020 2071 7565 7279 2e43 6f6d  ),.    query.Com
+00002da0: 706f 756e 6446 696c 7465 7228 292e 5f6f  poundFilter()._o
+00002db0: 7228 0a20 2020 2020 2020 2071 7565 7279  r(.        query
+00002dc0: 2e50 726f 7065 7274 7946 696c 7465 722e  .PropertyFilter.
+00002dd0: 7465 7874 2822 6e61 6d65 222c 2022 7469  text("name", "ti
+00002de0: 746c 6522 2c20 2263 6f6e 7461 696e 7322  tle", "contains"
+00002df0: 2c20 2279 6f75 7220 7061 6765 2074 6974  , "your page tit
+00002e00: 6c65 2229 2c0a 2020 2020 2020 2020 7175  le"),.        qu
+00002e10: 6572 792e 5072 6f70 6572 7479 4669 6c74  ery.PropertyFilt
+00002e20: 6572 2e74 6578 7428 226e 616d 6522 2c20  er.text("name", 
+00002e30: 2274 6974 6c65 222c 2022 636f 6e74 6169  "title", "contai
+00002e40: 6e73 222c 2022 796f 7572 206f 7468 6572  ns", "your other
+00002e50: 2070 6167 6520 7469 746c 6522 292c 0a20   page title"),. 
+00002e60: 2020 2029 2c0a 290a 0a71 7565 7279 5f73     ),.)..query_s
+00002e70: 6f72 7420 3d20 7175 6572 792e 536f 7274  ort = query.Sort
+00002e80: 4669 6c74 6572 280a 2020 2020 5b0a 2020  Filter(.    [.  
+00002e90: 2020 2020 2020 7175 6572 792e 5072 6f70        query.Prop
+00002ea0: 6572 7479 5661 6c75 6553 6f72 742e 6173  ertyValueSort.as
+00002eb0: 6365 6e64 696e 6728 2279 6f75 7220 7072  cending("your pr
+00002ec0: 6f70 6572 7479 206e 616d 6522 292c 0a20  operty name"),. 
+00002ed0: 2020 2020 2020 2071 7565 7279 2e45 6e74         query.Ent
+00002ee0: 7279 5469 6d65 7374 616d 7053 6f72 742e  ryTimestampSort.
+00002ef0: 6372 6561 7465 645f 7469 6d65 5f64 6573  created_time_des
+00002f00: 6365 6e64 696e 6728 292c 0a20 2020 205d  cending(),.    ]
+00002f10: 0a29 0a0a 7175 6572 795f 7265 7375 6c74  .)..query_result
+00002f20: 203d 206e 6577 5f64 6174 6162 6173 652e   = new_database.
+00002f30: 7175 6572 7928 0a20 2020 2066 696c 7465  query(.    filte
+00002f40: 723d 7175 6572 795f 6669 6c74 6572 2c0a  r=query_filter,.
+00002f50: 2020 2020 736f 7274 3d71 7565 7279 5f73      sort=query_s
+00002f60: 6f72 742c 0a20 2020 2070 6167 655f 7369  ort,.    page_si
+00002f70: 7a65 3d35 2c0a 2020 2020 6669 6c74 6572  ze=5,.    filter
+00002f80: 5f70 726f 7065 7274 795f 7661 6c75 6573  _property_values
+00002f90: 3d5b 226e 616d 6522 2c20 226f 7074 696f  =["name", "optio
+00002fa0: 6e73 225d 2c0a 290a 6060 600a 0a3c 6272  ns"],.).```..<br
+00002fb0: 3e0a 0a23 2320 4578 6365 7074 696f 6e73  >..## Exceptions
+00002fc0: 2026 2056 616c 6964 6174 696e 6720 5265   & Validating Re
+00002fd0: 7370 6f6e 7365 730a 0a45 7272 6f72 7320  sponses..Errors 
+00002fe0: 696e 204e 6f74 696f 6e20 7265 7175 6573  in Notion reques
+00002ff0: 7473 2072 6574 7572 6e20 616e 206f 626a  ts return an obj
+00003000: 6563 7420 7769 7468 2074 6865 206b 6579  ect with the key
+00003010: 733a 2027 6f62 6a65 6374 272c 2027 7374  s: 'object', 'st
+00003020: 6174 7573 272c 2027 636f 6465 272c 2061  atus', 'code', a
+00003030: 6e64 2027 6d65 7373 6167 6527 2e0a 4578  nd 'message'..Ex
+00003040: 6365 7074 696f 6e73 2061 7265 2072 6169  ceptions are rai
+00003050: 7365 6420 6279 206d 6174 6368 696e 6720  sed by matching 
+00003060: 7468 6520 6572 726f 7220 636f 6465 2061  the error code a
+00003070: 6e64 2072 6574 7572 6e69 6e67 2074 6865  nd returning the
+00003080: 206d 6573 7361 6765 2e20 466f 7220 6578   message. For ex
+00003090: 616d 706c 653a 0a0a 6060 6070 790a 686f  ample:..```py.ho
+000030a0: 6d65 7061 6765 2e5f 7061 7463 685f 7072  mepage._patch_pr
+000030b0: 6f70 6572 7469 6573 2870 6179 6c6f 6164  operties(payload
+000030c0: 3d7b 2761 6e5f 696e 636f 7272 6563 745f  ={'an_incorrect_
+000030d0: 6b65 7927 3a27 7661 6c75 6527 7d29 0a23  key':'value'}).#
+000030e0: 2045 7861 6d70 6c65 2065 7272 6f72 206f   Example error o
+000030f0: 626a 6563 7420 666f 7220 6c69 6e65 2061  bject for line a
+00003100: 626f 7665 2e2e 0a23 207b 0a23 2020 2027  bove...# {.#   '
+00003110: 6f62 6a65 6374 273a 2027 6572 726f 7227  object': 'error'
+00003120: 2c20 0a23 2020 2027 7374 6174 7573 273a  , .#   'status':
+00003130: 2034 3030 2c20 0a23 2020 2027 636f 6465   400, .#   'code
+00003140: 273a 2027 7661 6c69 6461 7469 6f6e 5f65  ': 'validation_e
+00003150: 7272 6f72 272c 200a 2320 2020 276d 6573  rror', .#   'mes
+00003160: 7361 6765 273a 2027 626f 6479 2066 6169  sage': 'body fai
+00003170: 6c65 6420 7661 6c69 6461 7469 6f6e 3a20  led validation: 
+00003180: 626f 6479 2e61 6e5f 696e 636f 7272 6563  body.an_incorrec
+00003190: 745f 6b65 7920 7368 6f75 6c64 2062 6520  t_key should be 
+000031a0: 6e6f 7420 7072 6573 656e 742c 2069 6e73  not present, ins
+000031b0: 7465 6164 2077 6173 2060 2276 616c 7565  tead was `"value
+000031c0: 2260 2e27 0a23 207d 0a60 6060 0a0a 6060  "`.'.# }.```..``
+000031d0: 6073 680a 5472 6163 6562 6163 6b20 286d  `sh.Traceback (m
+000031e0: 6f73 7420 7265 6365 6e74 2063 616c 6c20  ost recent call 
+000031f0: 6c61 7374 293a 0a46 696c 6520 2263 3a5c  last):.File "c:\
+00003200: 7061 7468 5c74 6f5c 6669 6c65 5c5f 2e70  path\to\file\_.p
+00003210: 7922 2c20 6c69 6e65 2036 2c20 696e 203c  y", line 6, in <
+00003220: 6d6f 6475 6c65 3e0a 2020 2020 686f 6d65  module>.    home
+00003230: 7061 6765 2e5f 7061 7463 685f 7072 6f70  page._patch_prop
+00003240: 6572 7469 6573 2870 6179 6c6f 6164 3d7b  erties(payload={
+00003250: 2761 6e5f 696e 636f 7272 6563 745f 6b65  'an_incorrect_ke
+00003260: 7927 3a27 7661 6c75 6527 7d29 0a46 696c  y':'value'}).Fil
+00003270: 6520 2263 3a5c 2e2e 2e5c 6e6f 7469 6f6e  e "c:\...\notion
+00003280: 5c65 7863 6570 7469 6f6e 735c 7661 6c69  \exceptions\vali
+00003290: 6461 7465 2e70 7922 2c20 6c69 6e65 2034  date.py", line 4
+000032a0: 382c 2069 6e20 7661 6c69 6461 7465 5f72  8, in validate_r
+000032b0: 6573 706f 6e73 650a 2020 2020 7261 6973  esponse.    rais
+000032c0: 6520 4e6f 7469 6f6e 5661 6c69 6461 7469  e NotionValidati
+000032d0: 6f6e 4572 726f 7228 6d65 7373 6167 6529  onError(message)
+000032e0: 0a6e 6f74 696f 6e2e 6578 6365 7074 696f  .notion.exceptio
+000032f0: 6e73 2e65 7272 6f72 732e 4e6f 7469 6f6e  ns.errors.Notion
+00003300: 5661 6c69 6461 7469 6f6e 4572 726f 723a  ValidationError:
+00003310: 2062 6f64 7920 6661 696c 6564 2076 616c   body failed val
+00003320: 6964 6174 696f 6e3a 2062 6f64 792e 616e  idation: body.an
+00003330: 5f69 6e63 6f72 7265 6374 5f6b 6579 2073  _incorrect_key s
+00003340: 686f 756c 6420 6265 206e 6f74 2070 7265  hould be not pre
+00003350: 7365 6e74 2c20 696e 7374 6561 6420 7761  sent, instead wa
+00003360: 7320 6022 7661 6c75 6522 602e 0a45 7272  s `"value"`..Err
+00003370: 6f72 2034 3030 3a20 5468 6520 7265 7175  or 400: The requ
+00003380: 6573 7420 626f 6479 2064 6f65 7320 6e6f  est body does no
+00003390: 7420 6d61 7463 6820 7468 6520 7363 6865  t match the sche
+000033a0: 6d61 2066 6f72 2074 6865 2065 7870 6563  ma for the expec
+000033b0: 7465 6420 7061 7261 6d65 7465 7273 2e0a  ted parameters..
+000033c0: 6060 600a 0a50 6f73 7369 626c 6520 6572  ```..Possible er
+000033d0: 726f 7273 2061 7265 3a0a 202d 2060 4e6f  rors are:. - `No
+000033e0: 7469 6f6e 496e 7661 6c69 644a 736f 6e60  tionInvalidJson`
+000033f0: 0a20 2d20 604e 6f74 696f 6e49 6e76 616c  . - `NotionInval
+00003400: 6964 5265 7175 6573 7455 726c 600a 202d  idRequestUrl`. -
+00003410: 2060 4e6f 7469 6f6e 496e 7661 6c69 6452   `NotionInvalidR
+00003420: 6571 7565 7374 600a 202d 2060 4e6f 7469  equest`. - `Noti
+00003430: 6f6e 5661 6c69 6461 7469 6f6e 4572 726f  onValidationErro
+00003440: 7260 0a20 2d20 604e 6f74 696f 6e4d 6973  r`. - `NotionMis
+00003450: 7369 6e67 5665 7273 696f 6e60 0a20 2d20  singVersion`. - 
+00003460: 604e 6f74 696f 6e55 6e61 7574 686f 7269  `NotionUnauthori
+00003470: 7a65 6460 0a20 2d20 604e 6f74 696f 6e52  zed`. - `NotionR
+00003480: 6573 7472 6963 7465 6452 6573 6f75 7263  estrictedResourc
+00003490: 6560 0a20 2d20 604e 6f74 696f 6e4f 626a  e`. - `NotionObj
+000034a0: 6563 744e 6f74 466f 756e 6460 0a20 2d20  ectNotFound`. - 
+000034b0: 604e 6f74 696f 6e43 6f6e 666c 6963 7445  `NotionConflictE
+000034c0: 7272 6f72 600a 202d 2060 4e6f 7469 6f6e  rror`. - `Notion
+000034d0: 5261 7465 4c69 6d69 7465 6460 0a20 2d20  RateLimited`. - 
+000034e0: 604e 6f74 696f 6e49 6e74 6572 6e61 6c53  `NotionInternalS
+000034f0: 6572 7665 7245 7272 6f72 600a 202d 2060  erverError`. - `
+00003500: 4e6f 7469 6f6e 5365 7276 6963 6555 6e61  NotionServiceUna
+00003510: 7661 696c 6162 6c65 600a 202d 2060 4e6f  vailable`. - `No
+00003520: 7469 6f6e 4461 7461 6261 7365 436f 6e6e  tionDatabaseConn
+00003530: 6563 7469 6f6e 556e 6176 6169 6c61 626c  ectionUnavailabl
+00003540: 6560 0a0a 4120 636f 6d6d 6f6e 2065 7272  e`..A common err
+00003550: 6f72 2074 6f20 6c6f 6f6b 206f 7574 2066  or to look out f
+00003560: 6f72 2069 7320 604e 6f74 696f 6e4f 626a  or is `NotionObj
+00003570: 6563 744e 6f74 466f 756e 6460 2e20 5468  ectNotFound`. Th
+00003580: 6973 2065 7272 6f72 2069 7320 6f66 7465  is error is ofte
+00003590: 6e20 7261 6973 6564 2062 6563 6175 7365  n raised because
+000035a0: 2079 6f75 7220 626f 7420 6861 7320 6e6f   your bot has no
+000035b0: 7420 6265 656e 2061 6464 6564 2061 7320  t been added as 
+000035c0: 6120 636f 6e6e 6563 7469 6f6e 2074 6f20  a connection to 
+000035d0: 7468 6520 7061 6765 2e20 0a0a 3c70 2061  the page. ..<p a
+000035e0: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
+000035f0: 2020 203c 696d 6720 7372 633d 2265 7861     <img src="exa
+00003600: 6d70 6c65 732f 696d 6167 6573 2f64 6972  mples/images/dir
+00003610: 6563 746f 7279 5f61 6464 5f63 6f6e 6e65  ectory_add_conne
+00003620: 6374 696f 6e73 2e70 6e67 223e 2020 0a3c  ctions.png">  .<
+00003630: 2f70 3e0a 0a42 7920 6465 6661 756c 742c  /p>..By default,
+00003640: 2061 2062 6f74 2077 696c 6c20 6861 7665   a bot will have
+00003650: 2061 6363 6573 7320 746f 2074 6865 2063   access to the c
+00003660: 6869 6c64 7265 6e20 6f66 2061 6e79 2050  hildren of any P
+00003670: 6172 656e 7420 6f62 6a65 6374 2069 7420  arent object it 
+00003680: 6861 7320 6163 6365 7373 2074 6f6f 2e20  has access too. 
+00003690: 4265 2073 7572 6520 746f 2064 6f75 626c  Be sure to doubl
+000036a0: 6520 6368 6563 6b20 7468 6973 2063 6f6e  e check this con
+000036b0: 6e65 6374 696f 6e20 7768 656e 206d 6f76  nection when mov
+000036c0: 696e 6720 7061 6765 732e 2020 0a49 6620  ing pages.  .If 
+000036d0: 796f 7527 7265 2077 6f72 6b69 6e67 206f  you're working o
+000036e0: 6e20 6120 7061 6765 2074 6861 7420 796f  n a page that yo
+000036f0: 7572 2074 6f6b 656e 2068 6173 2061 6363  ur token has acc
+00003700: 6573 7320 746f 2076 6961 2069 7473 2070  ess to via its p
+00003710: 6172 656e 7420 7061 6765 2f64 6174 6162  arent page/datab
+00003720: 6173 652c 2062 7574 2079 6f75 206e 6576  ase, but you nev
+00003730: 6572 2065 7870 6c69 6369 746c 7920 6772  er explicitly gr
+00003740: 616e 7465 6420 6163 6365 7373 2074 6f20  anted access to 
+00003750: 7468 6520 6368 696c 6420 7061 6765 202d  the child page -
+00003760: 2020 616e 6420 796f 7520 6c61 7465 7220    and you later 
+00003770: 6d6f 7665 2074 6861 7420 6368 696c 6420  move that child 
+00003780: 7061 6765 206f 7574 2c20 7468 656e 2069  page out, then i
+00003790: 7420 7769 6c6c 206c 6f73 6520 6163 6365  t will lose acce
+000037a0: 7373 2e0a 0a2d 2d2d 0a                   ss...---.
```

