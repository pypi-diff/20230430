# Comparing `tmp/loopgpt-0.0.8.tar.gz` & `tmp/loopgpt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopgpt-0.0.8.tar", last modified: Wed Apr 19 19:51:56 2023, max compression
+gzip compressed data, was "loopgpt-0.0.9.tar", last modified: Sat Apr 22 04:21:17 2023, max compression
```

## Comparing `loopgpt-0.0.8.tar` & `loopgpt-0.0.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 19:51:56.123895 loopgpt-0.0.8/
--rw-rw-rw-   0        0        0     1090 2023-04-15 06:20:55.000000 loopgpt-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      114 2023-04-19 19:51:56.123895 loopgpt-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     9552 2023-04-19 15:21:15.000000 loopgpt-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 19:51:56.092636 loopgpt-0.0.8/loopgpt/
--rw-rw-rw-   0        0        0      974 2023-04-19 19:51:26.000000 loopgpt-0.0.8/loopgpt/__init__.py
--rw-rw-rw-   0        0        0    16210 2023-04-19 19:42:51.000000 loopgpt-0.0.8/loopgpt/agent.py
--rw-rw-rw-   0        0        0     3962 2023-04-18 22:30:05.000000 loopgpt-0.0.8/loopgpt/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-19 19:51:56.092636 loopgpt-0.0.8/loopgpt/embeddings/
--rw-rw-rw-   0        0        0      775 2023-04-16 16:37:13.000000 loopgpt-0.0.8/loopgpt/embeddings/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-16 16:37:13.000000 loopgpt-0.0.8/loopgpt/embeddings/openai_.py
--rw-rw-rw-   0        0        0      426 2023-04-16 16:37:13.000000 loopgpt-0.0.8/loopgpt/embeddings/provider.py
--rw-rw-rw-   0        0        0       87 2023-04-19 00:06:55.000000 loopgpt-0.0.8/loopgpt/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-19 19:51:56.108269 loopgpt-0.0.8/loopgpt/loops/
--rw-rw-rw-   0        0        0       36 2023-04-17 09:20:22.000000 loopgpt-0.0.8/loopgpt/loops/__init__.py
--rw-rw-rw-   0        0        0     1711 2023-04-19 15:18:34.000000 loopgpt-0.0.8/loopgpt/loops/cli.py
--rw-rw-rw-   0        0        0     7084 2023-04-19 18:55:48.000000 loopgpt-0.0.8/loopgpt/loops/repl.py
--rw-rw-rw-   0        0        0     3108 2023-04-17 03:25:06.000000 loopgpt-0.0.8/loopgpt/loops/ui.py
-drwxrwxrwx   0        0        0        0 2023-04-19 19:51:56.108269 loopgpt-0.0.8/loopgpt/memory/
--rw-rw-rw-   0        0        0      698 2023-04-16 16:37:13.000000 loopgpt-0.0.8/loopgpt/memory/__init__.py
--rw-rw-rw-   0        0        0      423 2023-04-16 16:37:13.000000 loopgpt-0.0.8/loopgpt/memory/base_memory.py
--rw-rw-rw-   0        0        0     1998 2023-04-16 16:37:13.000000 loopgpt-0.0.8/loopgpt/memory/local_memory.py
-drwxrwxrwx   0        0        0        0 2023-04-19 19:51:56.108269 loopgpt-0.0.8/loopgpt/models/
--rw-rw-rw-   0        0        0       38 2023-04-15 06:20:55.000000 loopgpt-0.0.8/loopgpt/models/__init__.py
--rw-rw-rw-   0        0        0     1950 2023-04-19 15:18:34.000000 loopgpt-0.0.8/loopgpt/models/openai_.py
--rw-rw-rw-   0        0        0     1984 2023-04-18 22:30:05.000000 loopgpt-0.0.8/loopgpt/summarizer.py
-drwxrwxrwx   0        0        0        0 2023-04-19 19:51:56.123895 loopgpt-0.0.8/loopgpt/tools/
--rw-rw-rw-   0        0        0     1450 2023-04-17 08:31:57.000000 loopgpt-0.0.8/loopgpt/tools/__init__.py
--rw-rw-rw-   0        0        0     2276 2023-04-18 22:30:05.000000 loopgpt-0.0.8/loopgpt/tools/agent_manager.py
--rw-rw-rw-   0        0        0     1112 2023-04-16 16:37:13.000000 loopgpt-0.0.8/loopgpt/tools/base_tool.py
--rw-rw-rw-   0        0        0     4158 2023-04-19 00:05:57.000000 loopgpt-0.0.8/loopgpt/tools/browser.py
--rw-rw-rw-   0        0        0     3731 2023-04-19 19:22:21.000000 loopgpt-0.0.8/loopgpt/tools/code.py
--rw-rw-rw-   0        0        0     2645 2023-04-19 19:22:11.000000 loopgpt-0.0.8/loopgpt/tools/filesystem.py
--rw-rw-rw-   0        0        0     2006 2023-04-19 19:22:43.000000 loopgpt-0.0.8/loopgpt/tools/google_search.py
--rw-rw-rw-   0        0        0      421 2023-04-16 16:37:13.000000 loopgpt-0.0.8/loopgpt/tools/memory_manager.py
--rw-rw-rw-   0        0        0      675 2023-04-17 03:25:06.000000 loopgpt-0.0.8/loopgpt/tools/shell.py
--rw-rw-rw-   0        0        0     3136 2023-04-19 19:28:31.000000 loopgpt-0.0.8/loopgpt/tools/simple_browser.py
-drwxrwxrwx   0        0        0        0 2023-04-19 19:51:56.123895 loopgpt-0.0.8/loopgpt/utils/
--rw-rw-rw-   0        0        0        0 2023-04-19 00:30:19.000000 loopgpt-0.0.8/loopgpt/utils/__init__.py
--rw-rw-rw-   0        0        0     4174 2023-04-19 00:30:54.000000 loopgpt-0.0.8/loopgpt/utils/spinner.py
-drwxrwxrwx   0        0        0        0 2023-04-19 19:51:56.092636 loopgpt-0.0.8/loopgpt.egg-info/
--rw-rw-rw-   0        0        0      114 2023-04-19 19:51:55.000000 loopgpt-0.0.8/loopgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      962 2023-04-19 19:51:55.000000 loopgpt-0.0.8/loopgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 19:51:55.000000 loopgpt-0.0.8/loopgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-19 19:51:55.000000 loopgpt-0.0.8/loopgpt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-04-19 19:51:55.000000 loopgpt-0.0.8/loopgpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 19:51:55.000000 loopgpt-0.0.8/loopgpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 19:51:56.123895 loopgpt-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      464 2023-04-19 19:51:31.000000 loopgpt-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 04:21:17.375331 loopgpt-0.0.9/
+-rw-rw-rw-   0        0        0     1090 2023-04-15 06:20:55.000000 loopgpt-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      114 2023-04-22 04:21:17.375331 loopgpt-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    10253 2023-04-21 10:41:18.000000 loopgpt-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 04:21:17.343342 loopgpt-0.0.9/loopgpt/
+-rw-rw-rw-   0        0        0      974 2023-04-22 04:20:47.000000 loopgpt-0.0.9/loopgpt/__init__.py
+-rw-rw-rw-   0        0        0    16210 2023-04-21 19:38:35.000000 loopgpt-0.0.9/loopgpt/agent.py
+-rw-rw-rw-   0        0        0     3962 2023-04-21 10:41:18.000000 loopgpt-0.0.9/loopgpt/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-22 04:21:17.359335 loopgpt-0.0.9/loopgpt/embeddings/
+-rw-rw-rw-   0        0        0      775 2023-04-21 11:42:59.000000 loopgpt-0.0.9/loopgpt/embeddings/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-16 16:37:13.000000 loopgpt-0.0.9/loopgpt/embeddings/openai_.py
+-rw-rw-rw-   0        0        0      426 2023-04-16 16:37:13.000000 loopgpt-0.0.9/loopgpt/embeddings/provider.py
+-rw-rw-rw-   0        0        0       87 2023-04-21 10:41:18.000000 loopgpt-0.0.9/loopgpt/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-22 04:21:17.359335 loopgpt-0.0.9/loopgpt/loops/
+-rw-rw-rw-   0        0        0       36 2023-04-21 10:41:18.000000 loopgpt-0.0.9/loopgpt/loops/__init__.py
+-rw-rw-rw-   0        0        0     1711 2023-04-21 10:41:18.000000 loopgpt-0.0.9/loopgpt/loops/cli.py
+-rw-rw-rw-   0        0        0     7371 2023-04-21 20:31:54.000000 loopgpt-0.0.9/loopgpt/loops/repl.py
+-rw-rw-rw-   0        0        0     3108 2023-04-17 03:25:06.000000 loopgpt-0.0.9/loopgpt/loops/ui.py
+drwxrwxrwx   0        0        0        0 2023-04-22 04:21:17.359335 loopgpt-0.0.9/loopgpt/memory/
+-rw-rw-rw-   0        0        0      698 2023-04-16 16:37:13.000000 loopgpt-0.0.9/loopgpt/memory/__init__.py
+-rw-rw-rw-   0        0        0      423 2023-04-16 16:37:13.000000 loopgpt-0.0.9/loopgpt/memory/base_memory.py
+-rw-rw-rw-   0        0        0     1998 2023-04-16 16:37:13.000000 loopgpt-0.0.9/loopgpt/memory/local_memory.py
+drwxrwxrwx   0        0        0        0 2023-04-22 04:21:17.367330 loopgpt-0.0.9/loopgpt/models/
+-rw-rw-rw-   0        0        0       38 2023-04-21 19:38:35.000000 loopgpt-0.0.9/loopgpt/models/__init__.py
+-rw-rw-rw-   0        0        0     1950 2023-04-21 19:38:35.000000 loopgpt-0.0.9/loopgpt/models/openai_.py
+-rw-rw-rw-   0        0        0     1984 2023-04-21 19:38:35.000000 loopgpt-0.0.9/loopgpt/summarizer.py
+drwxrwxrwx   0        0        0        0 2023-04-22 04:21:17.375331 loopgpt-0.0.9/loopgpt/tools/
+-rw-rw-rw-   0        0        0     1450 2023-04-21 10:41:18.000000 loopgpt-0.0.9/loopgpt/tools/__init__.py
+-rw-rw-rw-   0        0        0     2276 2023-04-21 10:41:18.000000 loopgpt-0.0.9/loopgpt/tools/agent_manager.py
+-rw-rw-rw-   0        0        0     1112 2023-04-16 16:37:13.000000 loopgpt-0.0.9/loopgpt/tools/base_tool.py
+-rw-rw-rw-   0        0        0     5445 2023-04-22 04:20:27.000000 loopgpt-0.0.9/loopgpt/tools/browser.py
+-rw-rw-rw-   0        0        0     3731 2023-04-21 19:38:35.000000 loopgpt-0.0.9/loopgpt/tools/code.py
+-rw-rw-rw-   0        0        0     2645 2023-04-21 10:41:18.000000 loopgpt-0.0.9/loopgpt/tools/filesystem.py
+-rw-rw-rw-   0        0        0     2006 2023-04-21 10:41:18.000000 loopgpt-0.0.9/loopgpt/tools/google_search.py
+-rw-rw-rw-   0        0        0      421 2023-04-16 16:37:13.000000 loopgpt-0.0.9/loopgpt/tools/memory_manager.py
+-rw-rw-rw-   0        0        0      675 2023-04-17 03:25:06.000000 loopgpt-0.0.9/loopgpt/tools/shell.py
+-rw-rw-rw-   0        0        0     3136 2023-04-21 11:42:59.000000 loopgpt-0.0.9/loopgpt/tools/simple_browser.py
+drwxrwxrwx   0        0        0        0 2023-04-22 04:21:17.375331 loopgpt-0.0.9/loopgpt/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-21 10:41:18.000000 loopgpt-0.0.9/loopgpt/utils/__init__.py
+-rw-rw-rw-   0        0        0     4174 2023-04-21 10:41:18.000000 loopgpt-0.0.9/loopgpt/utils/spinner.py
+drwxrwxrwx   0        0        0        0 2023-04-22 04:21:17.351330 loopgpt-0.0.9/loopgpt.egg-info/
+-rw-rw-rw-   0        0        0      114 2023-04-22 04:21:17.000000 loopgpt-0.0.9/loopgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      962 2023-04-22 04:21:17.000000 loopgpt-0.0.9/loopgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 04:21:17.000000 loopgpt-0.0.9/loopgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-22 04:21:17.000000 loopgpt-0.0.9/loopgpt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-04-22 04:21:17.000000 loopgpt-0.0.9/loopgpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-22 04:21:17.000000 loopgpt-0.0.9/loopgpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 04:21:17.375331 loopgpt-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      464 2023-04-22 04:20:53.000000 loopgpt-0.0.9/setup.py
```

### Comparing `loopgpt-0.0.8/LICENSE` & `loopgpt-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.8/README.md` & `loopgpt-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -286,23 +286,29 @@
         - [Windows](https://www.architectryan.com/2018/08/31/how-to-change-environment-variables-on-windows-10/)
         - [Linux](https://www.freecodecamp.org/news/how-to-set-an-environment-variable-in-linux/)
         - [Mac](https://phoenixnap.com/kb/set-environment-variable-mac)
 - Google Chrome
 
 ### Optional Requirements
 
-For official google search support:
-- [Google API Key](https://console.developers.google.com) (for Google Search)
-    - Set environment variable `GOOGLE_API_KEY` to the API key
-- [Google Custom Search Engine ID](https://cse.google.com/cse/create/new) (also for Google Search)
-    - Set environment variable `CUSTOM_SEARCH_ENGINE_ID` to the CSE ID
+For official google search support you will need to setup two environment variable keys `GOOGLE_API_KEY` and `CUSTOM_SEARCH_ENGINE_ID`, here is how to get them:
 
-In case these are absent, L♾️pGPT will fall back to using [DuckDuckGo Search](https://pypi.org/project/duckduckgo-search/)
+1. Create an application on the [Google Developers Console][google-console].
+2. Create your custom search engine using [Google Custom Search][google-custom-search].
+3. Once your custom search engine is created, select it and get into the details page of the search engine.
+    - On the "Basic" section, you will find the "Search engine ID" field, that value is what you will use for the `CUSTOM_SEARCH_ENGINE_ID` environment variable.
+    - Now go to the "Programmatic Access" section at the bottom of the page.
+        - Create a "Custom Search JSON API"
+        - Follow the dialog by selecting the application you created on step #1 and when you get your API key use it to populate the `GOOGLE_API_KEY` environment variable.
 
+ℹ️ In case these are absent, L♾️pGPT will fall back to using [DuckDuckGo Search](https://pypi.org/project/duckduckgo-search/).
 
 ## 💌 Contribute 
 
 We need A LOT of Help! Please open an issue or a PR if you'd like to contribute.
 
 ## 🌳 Community
 
 Need help? Join our [Discord](https://discord.gg/rqs26cqx7v).
+
+[google-console]: https://console.developers.google.com
+[google-custom-search]: https://programmablesearchengine.google.com/controlpanel/create
```

#### html2text {}

```diff
@@ -101,16 +101,25 @@
 loopgpt.Agent.from_config(agent_config) ``` ## ð Requirements - Python 3.8+
 - [An OpenAI API Key](https://platform.openai.com/account/api-keys) - Set
 environment variable `OPENAI_API_KEY` to the API key - How to set environment
 variables: - [Windows](https://www.architectryan.com/2018/08/31/how-to-change-
 environment-variables-on-windows-10/) - [Linux](https://www.freecodecamp.org/
 news/how-to-set-an-environment-variable-in-linux/) - [Mac](https://
 phoenixnap.com/kb/set-environment-variable-mac) - Google Chrome ### Optional
-Requirements For official google search support: - [Google API Key](https://
-console.developers.google.com) (for Google Search) - Set environment variable
-`GOOGLE_API_KEY` to the API key - [Google Custom Search Engine ID](https://
-cse.google.com/cse/create/new) (also for Google Search) - Set environment
-variable `CUSTOM_SEARCH_ENGINE_ID` to the CSE ID In case these are absent,
+Requirements For official google search support you will need to setup two
+environment variable keys `GOOGLE_API_KEY` and `CUSTOM_SEARCH_ENGINE_ID`, here
+is how to get them: 1. Create an application on the [Google Developers Console]
+[google-console]. 2. Create your custom search engine using [Google Custom
+Search][google-custom-search]. 3. Once your custom search engine is created,
+select it and get into the details page of the search engine. - On the "Basic"
+section, you will find the "Search engine ID" field, that value is what you
+will use for the `CUSTOM_SEARCH_ENGINE_ID` environment variable. - Now go to
+the "Programmatic Access" section at the bottom of the page. - Create a "Custom
+Search JSON API" - Follow the dialog by selecting the application you created
+on step #1 and when you get your API key use it to populate the
+`GOOGLE_API_KEY` environment variable. â¹ï¸ In case these are absent,
 Lâ¾ï¸pGPT will fall back to using [DuckDuckGo Search](https://pypi.org/
-project/duckduckgo-search/) ## ð Contribute We need A LOT of Help! Please
+project/duckduckgo-search/). ## ð Contribute We need A LOT of Help! Please
 open an issue or a PR if you'd like to contribute. ## ð³ Community Need help?
-Join our [Discord](https://discord.gg/rqs26cqx7v).
+Join our [Discord](https://discord.gg/rqs26cqx7v). [google-console]: https://
+console.developers.google.com [google-custom-search]: https://
+programmablesearchengine.google.com/controlpanel/create
```

### Comparing `loopgpt-0.0.8/loopgpt/__init__.py` & `loopgpt-0.0.9/loopgpt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 
 from loopgpt.agent import Agent
 from loopgpt.tools import *
 from loopgpt.memory import *
 from loopgpt.embeddings import *
```

### Comparing `loopgpt-0.0.8/loopgpt/agent.py` & `loopgpt-0.0.9/loopgpt/agent.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.8/loopgpt/constants.py` & `loopgpt-0.0.9/loopgpt/constants.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.8/loopgpt/embeddings/__init__.py` & `loopgpt-0.0.9/loopgpt/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.8/loopgpt/embeddings/openai_.py` & `loopgpt-0.0.9/loopgpt/embeddings/openai_.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.8/loopgpt/loops/cli.py` & `loopgpt-0.0.9/loopgpt/loops/cli.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.8/loopgpt/loops/repl.py` & `loopgpt-0.0.9/loopgpt/loops/repl.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 HEADER = r"""
 +------------------------------------------------------------+
 | ██╗░░░░░░█████╗░░█████╗░██████╗░░██████╗░██████╗░████████╗ |
 | ██║░░░░░██╔══██╗██╔══██╗██╔══██╗██╔════╝░██╔══██╗╚══██╔══╝ |
-| ██║░░░░░██║░░██║██║░░██║██████╔╝██║░░██╗░██████╔╝░░░██║░░░ |
+| ██║░░░░░██║░░░░██░░░░██║██████╔╝██║░░██╗░██████╔╝░░░██║░░░ |
 | ██║░░░░░██║░░██║██║░░██║██╔═══╝░██║░░╚██╗██╔═══╝░░░░██║░░░ |
 | ███████╗╚█████╔╝╚█████╔╝██║░░░░░╚██████╔╝██║░░░░░░░░██║░░░ |
 | ╚══════╝░╚════╝░░╚════╝░╚═╝░░░░░░╚═════╝░╚═╝░░░░░░░░╚═╝░░░ |
 +------------------------------------------------------------+
 """
 
 from loopgpt.constants import (
@@ -70,17 +70,20 @@
 
 
 def prompt(speaker, line):
     print_line(speaker, line, end="")
     return input()
 
 
-def write_divider(big=False):
+def write_divider(big=False, default_columns=80):
     char = "\u2501" if big else "\u2500"
-    columns = os.get_terminal_size().columns
+    try:
+        columns = os.get_terminal_size().columns
+    except OSError:
+        columns = default_columns
     print(char * columns)
 
 
 def check_agent_config(agent):
     if agent.name is None or agent.name == DEFAULT_AGENT_NAME:
         name = prompt("loopgpt", "Enter the name of your AI agent: ")
         if name.lower().strip() == "exit":
@@ -105,14 +108,15 @@
 def cli(agent, continuous=False):
     print(HEADER)
     res = check_agent_config(agent)
     if res == -1:
         return
     write_divider(big=True)
     resp = agent.chat()
+    n = 1
     while True:
         if isinstance(resp, str):
             print_line(agent.name, resp)
         else:
             if "thoughts" in resp:
                 msgs = {}
                 thoughts = resp["thoughts"]
@@ -142,21 +146,24 @@
                     if command["name"]:
                         print_line(
                             "command",
                             f"{command['name']}, Args: {command['args']}",
                             end="\n\n",
                         )
                     while True:
-                        if continuous:
+                        if continuous or n > 1:
                             yn = "y"
+                            n -= 1
                         else:
-                            yn = input(f"Execute? (Y/N): ")
-                            if yn.lower().strip() == "exit":
-                                return
+                            inp = input(f"Execute? (Y/N/Y:n to execute n steps continuously): ")
+                            yn, n = inp.split(":") if ":" in inp else (inp, 1)
+                            n = int(n)
                             yn = yn.lower().strip()
+                            if yn == "exit":
+                                return
                         if yn in ("y", "n"):
                             break
                     if yn == "y":
                         cmd = agent.staging_tool.get("name", agent.staging_tool)
                         if cmd == "task_complete":
                             return
                         print_line("system", f"Executing command: {cmd}")
```

### Comparing `loopgpt-0.0.8/loopgpt/loops/ui.py` & `loopgpt-0.0.9/loopgpt/loops/ui.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.8/loopgpt/memory/__init__.py` & `loopgpt-0.0.9/loopgpt/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.8/loopgpt/memory/local_memory.py` & `loopgpt-0.0.9/loopgpt/memory/local_memory.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.8/loopgpt/models/openai_.py` & `loopgpt-0.0.9/loopgpt/models/openai_.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.8/loopgpt/summarizer.py` & `loopgpt-0.0.9/loopgpt/summarizer.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.8/loopgpt/tools/__init__.py` & `loopgpt-0.0.9/loopgpt/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.8/loopgpt/tools/agent_manager.py` & `loopgpt-0.0.9/loopgpt/tools/agent_manager.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.8/loopgpt/tools/base_tool.py` & `loopgpt-0.0.9/loopgpt/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.8/loopgpt/tools/browser.py` & `loopgpt-0.0.9/loopgpt/tools/browser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """
 Adapted from Auto-GPT (https://github.com/Significant-Gravitas/Auto-GPT)
 """
 
-
-from selenium.webdriver.chrome.options import Options
 from webdriver_manager.chrome import ChromeDriverManager
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from bs4 import BeautifulSoup
 from selenium.common.exceptions import NoSuchWindowException
 from loopgpt.tools.base_tool import BaseTool
@@ -15,32 +13,57 @@
 from loopgpt.summarizer import Summarizer
 from loopgpt.logger import logger
 import logging
 import atexit
 
 
 class Browser(BaseTool):
-    def __init__(self):
+    def __init__(self, browser_type="chrome"):
         super(Browser, self).__init__()
+        if browser_type not in ("chrome", "firefox"):
+            browser_type = "chrome"
+        self._set_browser_options(browser_type)
+        self.driver = None
+        self.summarizer = Summarizer()
+        self.cache = {}
+        atexit.register(self.close)
+    
+    def _set_browser_options(self, browser_type):
+        self.browser_type = browser_type
+        if self.browser_type == "chrome":
+            from selenium.webdriver.chrome.options import Options
+        elif self.browser_type == "firefox":
+            from selenium.webdriver.firefox.options import Options
         options = Options()
         options.add_argument(
             "user-agent=Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.5615.49 Safari/537.36"
         )
+        options.add_experimental_option("excludeSwitches", ["enable-logging"])
         options.headless = True
         self.options = options
-        self.driver = None
-        self.summarizer = Summarizer()
-        self.cache = {}
-        atexit.register(self.close)
+    
+    def _init_chrome_driver(self):
+        try:
+            self.driver = webdriver.Chrome(
+                executable_path=ChromeDriverManager().install(), options=self.options
+            )
+        except:
+            logger.log(logging.INFO, "Failed to initialize Chrome driver. Trying Firefox...")
+            self._set_browser_options("firefox")
+            self._init_driver()
+    
+    def _init_firefox_driver(self):
+        self.driver = webdriver.Firefox(options=self.options)
 
     def _init_driver(self):
         self.close()
-        self.driver = webdriver.Chrome(
-            executable_path=ChromeDriverManager().install(), options=self.options
-        )
+        if self.browser_type == "chrome":
+            self._init_chrome_driver()
+        elif self.browser_type == "firefox":
+            self._init_firefox_driver()
 
     def _get(self, url):
         if url in self.cache:
             return self.cache[url]
         if self.driver is None:
             self._init_driver()
         num_retries = 3
@@ -109,7 +132,16 @@
 
             return {
                 "text": summary,
                 "links": links[:5],
             }
         except Exception as e:
             return f"An error occured while scraping the website: {e}. Make sure the URL is valid."
+    
+    def config(self):
+        config = super().config()
+        config["browser_type"] = self.browser_type
+        return config
+
+    @classmethod
+    def from_config(cls, config):
+        return cls(config["browser_type"])
```

### Comparing `loopgpt-0.0.8/loopgpt/tools/code.py` & `loopgpt-0.0.9/loopgpt/tools/code.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.8/loopgpt/tools/filesystem.py` & `loopgpt-0.0.9/loopgpt/tools/filesystem.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.8/loopgpt/tools/google_search.py` & `loopgpt-0.0.9/loopgpt/tools/google_search.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.8/loopgpt/tools/shell.py` & `loopgpt-0.0.9/loopgpt/tools/shell.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.8/loopgpt/tools/simple_browser.py` & `loopgpt-0.0.9/loopgpt/tools/simple_browser.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.8/loopgpt/utils/spinner.py` & `loopgpt-0.0.9/loopgpt/utils/spinner.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.8/loopgpt.egg-info/SOURCES.txt` & `loopgpt-0.0.9/loopgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

