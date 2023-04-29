# Comparing `tmp/ofscraper-1.83.tar.gz` & `tmp/ofscraper-1.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-1.83.tar", max compression
+gzip compressed data, was "ofscraper-1.86.tar", max compression
```

## Comparing `ofscraper-1.83.tar` & `ofscraper-1.86.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0     1067 2023-04-13 21:26:07.930007 ofscraper-1.83/LICENSE
--rw-r--r--   0        0        0     5800 2023-04-29 01:35:38.362445 ofscraper-1.83/README.md
--rw-r--r--   0        0        0     1235 2023-04-29 01:32:56.731751 ofscraper-1.83/pyproject.toml
--rw-r--r--   0        0        0      620 2023-04-06 15:33:38.742121 ofscraper-1.83/src/__init__.py
--rw-r--r--   0        0        0      733 2023-04-29 01:32:56.731751 ofscraper-1.83/src/__version__.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.83/src/api/__init__.py
--rw-r--r--   0        0        0     2169 2023-04-28 05:28:10.687970 ofscraper-1.83/src/api/highlights.py
--rw-r--r--   0        0        0      838 2023-04-28 05:28:10.687970 ofscraper-1.83/src/api/init.py
--rw-r--r--   0        0        0     1815 2023-04-06 15:33:38.742121 ofscraper-1.83/src/api/me.py
--rw-r--r--   0        0        0     3580 2023-04-28 05:28:10.687970 ofscraper-1.83/src/api/messages.py
--rw-r--r--   0        0        0     1788 2023-04-28 05:28:10.687970 ofscraper-1.83/src/api/paid.py
--rw-r--r--   0        0        0     7626 2023-04-28 11:23:57.457623 ofscraper-1.83/src/api/posts.py
--rw-r--r--   0        0        0     3247 2023-04-28 05:28:10.687970 ofscraper-1.83/src/api/profile.py
--rw-r--r--   0        0        0     2040 2023-04-06 15:33:38.742121 ofscraper-1.83/src/api/subscriptions.py
--rw-r--r--   0        0        0     5441 2023-04-28 05:28:10.687970 ofscraper-1.83/src/api/timeline.py
--rw-r--r--   0        0        0     4781 2023-04-28 11:23:57.457623 ofscraper-1.83/src/constants.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.83/src/db/__init__.py
--rw-r--r--   0        0        0    11266 2023-04-28 05:28:10.688970 ofscraper-1.83/src/db/operations.py
--rw-r--r--   0        0        0     3199 2023-04-06 17:48:03.239009 ofscraper-1.83/src/db/queries.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.83/src/interaction/__init__.py
--rw-r--r--   0        0        0     3169 2023-04-28 05:28:10.688970 ofscraper-1.83/src/interaction/like.py
--rw-r--r--   0        0        0     5080 2023-04-28 05:28:10.688970 ofscraper-1.83/src/prompts/prompt_functions.py
--rw-r--r--   0        0        0      359 2023-04-14 18:21:19.249081 ofscraper-1.83/src/prompts/prompt_strings.py
--rw-r--r--   0        0        0    17909 2023-04-28 11:23:57.457623 ofscraper-1.83/src/prompts/prompts.py
--rwxr-xr-x   0        0        0    19166 2023-04-28 14:14:09.709648 ofscraper-1.83/src/scraper.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.83/src/utils/__init__.py
--rw-r--r--   0        0        0     2726 2023-04-28 11:23:57.458623 ofscraper-1.83/src/utils/args.py
--rw-r--r--   0        0        0     8856 2023-04-28 05:28:10.689970 ofscraper-1.83/src/utils/auth.py
--rw-r--r--   0        0        0     8874 2023-04-28 11:59:24.168331 ofscraper-1.83/src/utils/config.py
--rw-r--r--   0        0        0      993 2023-04-07 16:49:03.190199 ofscraper-1.83/src/utils/dates.py
--rw-r--r--   0        0        0    10201 2023-04-29 01:21:35.196542 ofscraper-1.83/src/utils/download.py
--rw-r--r--   0        0        0      609 2023-04-06 15:33:38.743121 ofscraper-1.83/src/utils/encoding.py
--rw-r--r--   0        0        0     2938 2023-04-28 16:51:38.491314 ofscraper-1.83/src/utils/exit.py
--rw-r--r--   0        0        0     2795 2023-04-28 14:37:12.121950 ofscraper-1.83/src/utils/paths.py
--rw-r--r--   0        0        0     2998 2023-04-28 05:28:10.690970 ofscraper-1.83/src/utils/profiles.py
--rw-r--r--   0        0        0      779 2023-04-28 05:28:10.690970 ofscraper-1.83/src/utils/separate.py
--rw-r--r--   0        0        0     7009 1970-01-01 00:00:00.000000 ofscraper-1.83/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-13 21:26:07.930007 ofscraper-1.86/LICENSE
+-rw-r--r--   0        0        0     5800 2023-04-29 01:50:36.060807 ofscraper-1.86/README.md
+-rw-r--r--   0        0        0     1235 2023-04-29 22:25:20.860303 ofscraper-1.86/pyproject.toml
+-rw-r--r--   0        0        0      620 2023-04-06 15:33:38.742121 ofscraper-1.86/src/__init__.py
+-rw-r--r--   0        0        0      733 2023-04-29 22:25:20.860303 ofscraper-1.86/src/__version__.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.86/src/api/__init__.py
+-rw-r--r--   0        0        0     2195 2023-04-29 21:06:53.651540 ofscraper-1.86/src/api/highlights.py
+-rw-r--r--   0        0        0      838 2023-04-28 05:28:10.687970 ofscraper-1.86/src/api/init.py
+-rw-r--r--   0        0        0     1841 2023-04-29 21:06:53.652540 ofscraper-1.86/src/api/me.py
+-rw-r--r--   0        0        0     3598 2023-04-29 21:06:53.652540 ofscraper-1.86/src/api/messages.py
+-rw-r--r--   0        0        0     1788 2023-04-28 05:28:10.687970 ofscraper-1.86/src/api/paid.py
+-rw-r--r--   0        0        0     7626 2023-04-28 11:23:57.457623 ofscraper-1.86/src/api/posts.py
+-rw-r--r--   0        0        0     3273 2023-04-29 21:06:53.652540 ofscraper-1.86/src/api/profile.py
+-rw-r--r--   0        0        0     2058 2023-04-29 21:06:53.652540 ofscraper-1.86/src/api/subscriptions.py
+-rw-r--r--   0        0        0     5474 2023-04-29 21:06:53.652540 ofscraper-1.86/src/api/timeline.py
+-rw-r--r--   0        0        0     4793 2023-04-29 21:06:53.652540 ofscraper-1.86/src/constants.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.86/src/db/__init__.py
+-rw-r--r--   0        0        0    11266 2023-04-28 05:28:10.688970 ofscraper-1.86/src/db/operations.py
+-rw-r--r--   0        0        0     3199 2023-04-06 17:48:03.239009 ofscraper-1.86/src/db/queries.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.86/src/interaction/__init__.py
+-rw-r--r--   0        0        0     3169 2023-04-28 05:28:10.688970 ofscraper-1.86/src/interaction/like.py
+-rw-r--r--   0        0        0     5080 2023-04-28 05:28:10.688970 ofscraper-1.86/src/prompts/prompt_functions.py
+-rw-r--r--   0        0        0      359 2023-04-14 18:21:19.249081 ofscraper-1.86/src/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    17909 2023-04-28 11:23:57.457623 ofscraper-1.86/src/prompts/prompts.py
+-rwxr-xr-x   0        0        0    19182 2023-04-29 22:26:06.685815 ofscraper-1.86/src/scraper.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.86/src/utils/__init__.py
+-rw-r--r--   0        0        0     2864 2023-04-29 21:06:53.652540 ofscraper-1.86/src/utils/args.py
+-rw-r--r--   0        0        0     8856 2023-04-28 05:28:10.689970 ofscraper-1.86/src/utils/auth.py
+-rw-r--r--   0        0        0     8945 2023-04-29 21:06:53.652540 ofscraper-1.86/src/utils/config.py
+-rw-r--r--   0        0        0      993 2023-04-07 16:49:03.190199 ofscraper-1.86/src/utils/dates.py
+-rw-r--r--   0        0        0    11237 2023-04-29 21:54:25.606047 ofscraper-1.86/src/utils/download.py
+-rw-r--r--   0        0        0      609 2023-04-06 15:33:38.743121 ofscraper-1.86/src/utils/encoding.py
+-rw-r--r--   0        0        0     2938 2023-04-29 01:50:36.061807 ofscraper-1.86/src/utils/exit.py
+-rw-r--r--   0        0        0     1027 2023-04-29 22:23:00.769846 ofscraper-1.86/src/utils/logger.py
+-rw-r--r--   0        0        0     3004 2023-04-29 21:06:53.652540 ofscraper-1.86/src/utils/paths.py
+-rw-r--r--   0        0        0     2998 2023-04-28 05:28:10.690970 ofscraper-1.86/src/utils/profiles.py
+-rw-r--r--   0        0        0      779 2023-04-28 05:28:10.690970 ofscraper-1.86/src/utils/separate.py
+-rw-r--r--   0        0        0     7009 1970-01-01 00:00:00.000000 ofscraper-1.86/PKG-INFO
```

### Comparing `ofscraper-1.83/LICENSE` & `ofscraper-1.86/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-1.83/README.md` & `ofscraper-1.86/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-1.83/pyproject.toml` & `ofscraper-1.86/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "1.83"
+version = "1.86"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
```

### Comparing `ofscraper-1.83/src/__init__.py` & `ofscraper-1.86/src/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.83/src/__version__.py` & `ofscraper-1.86/src/__version__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,14 @@
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/       
 """
 
 __title__ = 'ofscraper'
-__version__ = '1.83'
+__version__ = '1.86'
 __author__ = 'datawhores'
 __author_email__ = 'datawhores@riseup.net'
 __description__ = 'A command-line program to quickly download,like or unlike posts, and more'
 __url__ = 'https://github.com/datawhores/ofscraper'
 __license__ = 'GNU General Public License v3 or later (GPLv3+)'
 __copyright__ = 'Copyright 2023'
```

### Comparing `ofscraper-1.83/src/api/highlights.py` & `ofscraper-1.86/src/api/highlights.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 import asyncio
 from itertools import chain
 
 import httpx
 from tenacity import retry,stop_after_attempt,wait_random
 
 
-from ..constants import highlightsWithStoriesEP, highlightsWithAStoryEP, storyEP
+from ..constants import NUM_TRIES,highlightsWithStoriesEP, highlightsWithAStoryEP, storyEP
 from ..utils import auth
 
 
-@retry(stop=stop_after_attempt(5),wait=wait_random(min=5, max=20),reraise=True)   
+@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
 def scrape_highlights(headers, user_id) -> list:
     with httpx.Client(http2=True, headers=headers) as c:
         url_stories = highlightsWithStoriesEP.format(user_id)
         url_story = highlightsWithAStoryEP.format(user_id)
 
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url_stories, headers))
@@ -49,15 +49,15 @@
 
 
 
 
 
 
 
-@retry(stop=stop_after_attempt(5),wait=wait_random(min=5, max=20),reraise=True)   
+@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
 async def scrape_story(headers, story_id: int) -> list:
     async with httpx.AsyncClient(http2=True, headers=headers) as c:
         url = storyEP.format(story_id)
 
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
```

### Comparing `ofscraper-1.83/src/api/init.py` & `ofscraper-1.86/src/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.83/src/api/me.py` & `ofscraper-1.86/src/api/me.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,18 @@
                  \/     \/           \/            \/         
 """
 
 import httpx
 from rich.console import Console
 console=Console()
 from tenacity import retry,stop_after_attempt,wait_random
-from ..constants import meEP,subscribeCountEP
+from ..constants import meEP,subscribeCountEP,NUM_TRIES
 from ..utils import auth, encoding
 
-@retry(stop=stop_after_attempt(5),wait=wait_random(min=2, max=6),reraise=True,after=lambda retry_state:print(f"Attempting to login attempt:{retry_state.attempt_number}/5")) 
+@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=2, max=6),reraise=True,after=lambda retry_state:print(f"Attempting to login attempt:{retry_state.attempt_number}/5")) 
 def scrape_user(headers):
     with httpx.Client(http2=True, headers=headers) as c:
         url = meEP
 
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
 
@@ -33,15 +33,15 @@
     name = encoding.encode_utf_16(profile['name'])
     username = profile['username']
     return (name, username)
 
 
 def print_user(name, username):
     console.print(f'Welcome, {name} | {username}')
-@retry(stop=stop_after_attempt(5),wait=wait_random(min=5, max=20),reraise=True)   
+@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
 def parse_subscriber_count(headers):
     with httpx.Client(http2=True, headers=headers) as c:
         url = subscribeCountEP
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
         r = c.get(url, timeout=None)
         if not r.is_error:
```

### Comparing `ofscraper-1.83/src/api/messages.py` & `ofscraper-1.86/src/api/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 import asyncio
 import time
 import httpx
 from tenacity import retry,stop_after_attempt,wait_random
 from tqdm.asyncio import tqdm
 import arrow
-from ..constants import messagesEP, messagesNextEP
+from ..constants import messagesEP, messagesNextEP,NUM_TRIES
 from ..utils import auth
 from ..db.operations import read_messages_response
 
 
 async def get_messages(headers,  model_id,username):
     global sem
     sem = asyncio.Semaphore(8)
@@ -59,15 +59,15 @@
     for message in responseArray:
         if message["id"] in dupeSet:
             continue
         dupeSet.add(message["id"])
         unduped.append(message)
     return unduped
 
-@retry(stop=stop_after_attempt(5),wait=wait_random(min=5, max=20),reraise=True)   
+@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
 async def scrape_messages(headers, user_id, message_id=None,recursive=False) -> list:
     ep = messagesNextEP if message_id else messagesEP
     url = ep.format(user_id, message_id)
     async with sem:
         async with httpx.AsyncClient(http2=True, headers=headers) as c:
             auth.add_cookies(c)
             c.headers.update(auth.create_sign(url, headers))
```

### Comparing `ofscraper-1.83/src/api/paid.py` & `ofscraper-1.86/src/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.83/src/api/posts.py` & `ofscraper-1.86/src/api/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.83/src/api/profile.py` & `ofscraper-1.86/src/api/profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 from datetime import datetime
 from itertools import zip_longest
 
 import httpx
 from rich.console import Console
 console=Console()
 from tenacity import retry,stop_after_attempt,wait_random
-from ..constants import profileEP
+from ..constants import profileEP,NUM_TRIES
 from ..utils import auth, dates, encoding
 from xxhash import xxh32
 
-@retry(stop=stop_after_attempt(5),wait=wait_random(min=5, max=20),reraise=True)   
+@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
 def scrape_profile(headers, username) -> dict:
     with httpx.Client(http2=True, headers=headers) as c:
         url = profileEP.format(username)
 
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
 
@@ -65,15 +65,15 @@
 def print_profile_info(info):
     header_fmt = 'Name: {} | Username: {} | ID: {} | Joined: {}\n'
     info_fmt = '- {} posts\n -- {} photos\n -- {} videos\n -- {} audios\n- {} archived posts'
     final_fmt = header_fmt + info_fmt
     console.print(final_fmt.format(*info))
 
 
-@retry(stop=stop_after_attempt(5),wait=wait_random(min=5, max=20),reraise=True)   
+@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
 def get_id(headers, username):
     with httpx.Client(http2=True, headers=headers) as c:
         url = profileEP.format(username)
 
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
```

### Comparing `ofscraper-1.83/src/api/subscriptions.py` & `ofscraper-1.86/src/api/subscriptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 import asyncio
 from itertools import chain
 
 import httpx
 from rich.console import Console
 console=Console()
 from tenacity import retry,stop_after_attempt,wait_random
-from ..constants import subscriptionsEP
+from ..constants import subscriptionsEP,NUM_TRIES
 from ..utils import auth, dates
 
 
 async def get_subscriptions(headers, subscribe_count):
     offsets = range(0, subscribe_count, 10)
     tasks = [scrape_subscriptions(headers, offset) for offset in offsets]
     subscriptions = await asyncio.gather(*tasks)
     return list(chain.from_iterable(subscriptions))
 
 
-@retry(stop=stop_after_attempt(5),wait=wait_random(min=5, max=20),reraise=True)   
+@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
 async def scrape_subscriptions(headers, offset=500) -> list:
     async with httpx.AsyncClient(http2=True, headers=headers) as c:
         url = subscriptionsEP.format(offset)
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
 
         r = await c.get(subscriptionsEP.format(offset), timeout=None)
```

### Comparing `ofscraper-1.83/src/api/timeline.py` & `ofscraper-1.86/src/api/timeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 import asyncio
 import httpx
 from tenacity import retry,stop_after_attempt,wait_random
 from tqdm.asyncio import tqdm
 from ..constants import (
     timelineEP, timelineNextEP,
     timelinePinnedEP,
-    archivedEP, archivedNextEP,timelinePinnedNextEP 
+    archivedEP, archivedNextEP,timelinePinnedNextEP,NUM_TRIES
 )
 from ..utils import auth
 from ..db.operations import read_timeline_response
-@retry(stop=stop_after_attempt(5),wait=wait_random(min=5, max=20),reraise=True)   
+@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
 def scrape_pinned_posts(headers, model_id,timestamp=0) -> list:
     with httpx.Client(http2=True, headers=headers) as c:
         ep = timelinePinnedNextEP if timestamp else timelinePinnedEP
         url = ep.format(model_id, timestamp)
         # url = timelinePinnedEP.format(model_id)
 
         auth.add_cookies(c)
@@ -33,15 +33,15 @@
         if not r.is_error:
             return r.json()['list']
         r.raise_for_status()
 
 def get_pinned_post(headers,model_id,username):
     return scrape_pinned_posts(headers,model_id)
    
-@retry(stop=stop_after_attempt(1),wait=wait_random(min=5, max=20),reraise=True)   
+@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
 async def scrape_timeline_posts(headers, model_id, timestamp=None,recursive=False) -> list:
     global sem
     sem = asyncio.Semaphore(8)
     if timestamp:
         timestamp=str(timestamp)
         ep = timelineNextEP
         url = ep.format(model_id, timestamp)
@@ -115,15 +115,15 @@
         unduped.append(post)
     return unduped                                
 
 def get_archive_post(headers,model_id):
     return scrape_archived_posts(headers,model_id)
    
 
-@retry(stop=stop_after_attempt(5),wait=wait_random(min=5, max=20),reraise=True)   
+@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
 def scrape_archived_posts(headers, model_id, timestamp=0) -> list:
     ep = archivedNextEP if timestamp else archivedEP
     url = ep.format(model_id, timestamp)
 
     with httpx.Client(http2=True, headers=headers) as c:
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
```

### Comparing `ofscraper-1.83/src/constants.py` & `ofscraper-1.86/src/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,8 +96,9 @@
             "timeline":"posts",
             "archived":"archived",
             "paid":"paid",
             "stories":"stories",
             "highlights":"highlights",
             "profile":"profile",
             "pinned":"posts"
-        }
+        }
+NUM_TRIES=5
```

### Comparing `ofscraper-1.83/src/db/operations.py` & `ofscraper-1.86/src/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.83/src/db/queries.py` & `ofscraper-1.86/src/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.83/src/interaction/like.py` & `ofscraper-1.86/src/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.83/src/prompts/prompt_functions.py` & `ofscraper-1.86/src/prompts/prompt_functions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.83/src/prompts/prompts.py` & `ofscraper-1.86/src/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.83/src/scraper.py` & `ofscraper-1.86/src/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     urls, info = profile.parse_profile(user_profile)
     profile.print_profile_info(info)
     output=[]
     for ele in enumerate(urls):
         count=ele[0]
         data=ele[1]
         output.append(posts_.Media({"url":data["url"],"type":data["mediatype"]},count,posts_.Post(data,info[2],username,responsetype="profile")))
-    return output
+    reexcludedBittern8turn output
 
 
 
 
 def process_areas(headers, ele, model_id) -> list:
     args.posts = list(map(lambda x:x.capitalize(),(args.posts or prompts.areas_prompt())
 ))
```

### Comparing `ofscraper-1.83/src/utils/args.py` & `ofscraper-1.86/src/utils/args.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,21 +21,24 @@
     )
     general.add_argument(
         '-d', '--daemon', help='run script in the background\nSet value to minimum minutes between script runs\nOverdue runs will run as soon as previous run finishes', type=int,default=None
     )
     general.add_argument(
         '-s', '--silent', help = 'mute output', action = 'store_true',default=False
     )
+    general.add_argument(
+        '-l', '--log', help = 'set log level', type=str.upper,default=None,choices=["OFF","INFO","DEBUG"]
+    )
     post=parser.add_argument_group("Post",description="What type of post to scrape")                                      
 
     post.add_argument("-e","--dupe",action="store_true",default=False,help="Bypass the dupe check and redownload all files")
     post.add_argument(
         '-o', '--posts', help = 'Download content from a models wall',default=None,required=False,type = str.lower,choices=["highlights","all","archived","messages","timeline","pinned","stories","purchased",],action='append'
     )
-    post.add_argument("-l","--letter-count",action="store_true",default=False,help="intrepret config 'textlength' as max length by letter")
+    post.add_argument("-c","--letter-count",action="store_true",default=False,help="intrepret config 'textlength' as max length by letter")
     post.add_argument("-a","--action",default=None,help="perform like or unlike action on each post",choices=["like","unlike"])
      #Filters for accounts
     filters=parser.add_argument_group("filters",description="Filters out usernames based on selected parameters")
     
     filters.add_argument(
         '-t', '--account-type', help = 'Filter Free or paid accounts',default=None,required=False,type = str.lower,choices=["paid","free"]
     )
```

### Comparing `ofscraper-1.83/src/utils/auth.py` & `ofscraper-1.86/src/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.83/src/utils/config.py` & `ofscraper-1.86/src/utils/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 
 def get_current_config_schema(config: dict) -> dict:
     config = config['config']
 
     new_config = {
         'config': {
-            mainProfile: config.get(mainProfile) or mainProfile,
+            mainProfile: get_main_profile(config),
             'save_location':get_save_location(config) ,
             'file_size_limit': get_filesize(config),
             'dir_format': get_dirformat(config),
             'file_format':get_fileformat(config),
             'textlength':get_textlength(config),
             'date': get_date(config),
             "metadata": get_metadata(config),
@@ -163,105 +163,105 @@
                         configText=f.read()
                         config = json.loads(configText)
                     break
                 except:
                     continue
 
 
-def get_save_location(config):
+def get_save_location(config=None):
     if not config:
         return SAVE_LOCATION_DEFAULT   
     return config.get('save_location') or SAVE_LOCATION_DEFAULT
 
-def get_main_profile(config):
+def get_main_profile(config=None):
     if not config:
         return PROFILE_DEFAULT   
     return config.get('main_profile',PROFILE_DEFAULT)
 
-def get_filesize(config):
+def get_filesize(config=None):
     if not config:
         return FILE_SIZE_DEFAULT      
     try:
         return int(config.get('file_size_limit', FILE_SIZE_DEFAULT))
     except:
         return 0
 
-def get_dirformat(config):
+def get_dirformat(config=None):
     if not config:
         return DIR_FORMAT_DEFAULT     
     return config.get('dir_format', DIR_FORMAT_DEFAULT)
 
-def get_fileformat(config):
+def get_fileformat(config=None):
     if not config:
         return FILE_FORMAT_DEFAULT     
     return config.get('file_format', FILE_FORMAT_DEFAULT)
 
-def get_textlength(config):
+def get_textlength(config=None):
     if not config:
         return TEXTLENGTH_DEFAULT    
     try:
         return int(config.get('textlength', TEXTLENGTH_DEFAULT))
     except:
         return 0
 
-def get_date(config):
+def get_date(config=None):
     if not config:
         return DATE_DEFAULT     
     return config.get('date', DATE_DEFAULT)
 
-def get_metadata(config):
+def get_metadata(config=None):
     if not config:
         return METADATA_DEFAULT      
     return config.get('metadata', METADATA_DEFAULT)
 
 
-def get_filter(config):
+def get_filter(config=None):
     if not config:
         return FILTER_DEFAULT
     filter=config.get('filter', FILTER_DEFAULT)
     if isinstance(filter,str):
         return list(map(lambda x:x.capitalize().strip(),filter.split(",")))
     elif isinstance(filter,list):
         return list(map(lambda x:x.capitalize(),filter))
     else:
         FILTER_DEFAULT
-def get_timeline_responsetype(config):
+def get_timeline_responsetype(config=None):
     if not config:
         return RESPONSE_TYPE_DEFAULT["timeline"]
     return config.get('responsetype',{}).get("timeline") or config.get('responsetype',{}).get("post") or RESPONSE_TYPE_DEFAULT["timeline"]
 
-def get_archived_responsetype(config):
+def get_archived_responsetype(config=None):
     if not config:
         return RESPONSE_TYPE_DEFAULT["archived"]
     return config.get('responsetype',{}).get("archived") or RESPONSE_TYPE_DEFAULT["archived"]
 
-def get_stories_responsetype(config):
+def get_stories_responsetype(config=None):
     if not config:
         return RESPONSE_TYPE_DEFAULT["stories"]    
     return config.get('responsetype',{}).get("stories") or RESPONSE_TYPE_DEFAULT["stories"]
 
-def get_highlights_responsetype(config):
+def get_highlights_responsetype(config=None):
     if not config:
         return RESPONSE_TYPE_DEFAULT["highlights"]       
     return config.get('responsetype',{}).get("highlights") or RESPONSE_TYPE_DEFAULT["highlights"]
 
-def get_paid_responsetype(config):
+def get_paid_responsetype(config=None):
     if not config:
         return RESPONSE_TYPE_DEFAULT["paid"]       
     return config.get('responsetype',{}).get("paid") or RESPONSE_TYPE_DEFAULT["paid"]
 
-def get_messages_responsetype(config):
+def get_messages_responsetype(config=None):
     if not config:
         return RESPONSE_TYPE_DEFAULT["message"]      
     return config.get('responsetype',{}).get("message") or RESPONSE_TYPE_DEFAULT["message"]
 
 
-def get_profile_responsetype(config):
+def get_profile_responsetype(config=None):
     if not config:
         return RESPONSE_TYPE_DEFAULT["profile"]       
     return config.get('responsetype',{}).get("profile") or RESPONSE_TYPE_DEFAULT["profile"]
 
 
-def get_pinned_responsetype(config):
+def get_pinned_responsetype(config=None):
     if not config:
         return RESPONSE_TYPE_DEFAULT["pinned"]       
     return config.get('responsetype',{}).get("pinned") or RESPONSE_TYPE_DEFAULT["pinned"]
```

### Comparing `ofscraper-1.83/src/utils/dates.py` & `ofscraper-1.86/src/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.83/src/utils/download.py` & `ofscraper-1.86/src/utils/download.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 import platform
 import sys
 import shutil
 import traceback
 import re
 import httpx
 import os
+import contextvars
+
 from rich.console import Console
 console=Console()
 from tqdm.asyncio import tqdm
 import arrow
 try:
     from win32_setctime import setctime  # pylint: disable=import-error
 except ModuleNotFoundError:
@@ -30,20 +32,23 @@
 
 from .auth import add_cookies
 from .config import read_config
 from .separate import separate_by_id
 from ..db import operations
 from .paths import set_directory,getmediadir
 from ..utils import auth
-from ..constants import configPath,FILE_FORMAT_DEFAULT,DATE_DEFAULT,TEXTLENGTH_DEFAULT,FILE_SIZE_DEFAULT
+from ..constants import NUM_TRIES,FILE_FORMAT_DEFAULT,DATE_DEFAULT,TEXTLENGTH_DEFAULT,FILE_SIZE_DEFAULT
 from ..utils.profiles import get_current_profile
 from .dates import convert_local_time
-
+import logging
+attempt = contextvars.ContextVar("attempt")
 
 config = read_config()['config']
+import src.utils.logger as logger
+log=logger.log
 
 
 async def process_dicts(username, model_id, medialist,forced=False):
     if medialist:
         if not forced:
             media_ids = set(operations.get_media_ids(model_id,username))
             medialist = separate_by_id(medialist, media_ids)
@@ -71,15 +76,14 @@
                                                             )))
             for coro in asyncio.as_completed(aws):
                     try:
                         media_type, num_bytes_downloaded = await coro
                     except Exception as e:
                         media_type = "skipped"
                         num_bytes_downloaded = 0
-                        console.print(e)
 
                     total_bytes_downloaded += num_bytes_downloaded
                     data = convert_num_bytes(total_bytes_downloaded)
                     if media_type == 'images':
                         photo_count += 1
                         main_bar.set_description(
                             desc.format(
@@ -105,21 +109,23 @@
 
                     main_bar.update()
 
 
 def retry_required(value):
     return value == ('skipped', 1)
 
-@retry(retry=retry_if_result(retry_required),stop=stop_after_attempt(5),wait=wait_random(min=20, max=40),reraise=True) 
+@retry(retry=retry_if_result(retry_required),stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=20, max=40),reraise=True) 
 async def download(ele,path,model_id,username,file_size_limit,id_=None):
     url=ele.url
     media_type=ele.mediatype
     id_=ele.id
     bar=None
     temp=None
+    attempt.set(attempt.get(0) + 1)
+    log.debug(f"Attempting to download media {ele.filename} with {url or 'no url'}")
     if not url:
         return 'skipped', 1
     try:
         async with sem:
             async with httpx.AsyncClient(http2=True, headers = auth.make_headers(auth.read_auth()), follow_redirects=True, timeout=None) as c: 
                 auth.add_cookies(c)        
                 async with c.stream('GET',url) as r:
@@ -127,39 +133,47 @@
                         rheaders=r.headers
                         total = int(rheaders['Content-Length'])
                         if file_size_limit and total > int(file_size_limit): 
                                 return 'skipped', 1       
                         content_type = rheaders.get("content-type").split('/')[-1]
                         filename=createfilename(ele,username,model_id,content_type)
                         path_to_file = trunicate(pathlib.Path(path,f"{filename}"))
+                        
+                        
                         temp=trunicate(f"{path_to_file}.part")
                         pathlib.Path(temp).unlink(missing_ok=True)
                         with open(temp, 'wb') as f:
                             pathstr=str(path_to_file)
-                            bar=tqdm(desc=(pathstr[:50] + '....') if len(pathstr) > 50 else pathstr ,total=total, unit_scale=True, unit_divisor=1024, unit='B', leave=False)
+                            bar=tqdm(desc=f"{attempt.get()}/{NUM_TRIES} {(pathstr[:50] + '....') if len(pathstr) > 50 else pathstr}" ,total=total, unit_scale=True, unit_divisor=1024, unit='B', leave=False)
                             num_bytes_downloaded = r.num_bytes_downloaded
                             async for chunk in r.aiter_bytes(chunk_size=1024):
                                 f.write(chunk)
                                 bar.update(r.num_bytes_downloaded - num_bytes_downloaded)
                                 num_bytes_downloaded = r.num_bytes_downloaded 
-                                                    
-                            if pathlib.Path(temp).exists() and num_bytes_downloaded==total:
-                                shutil.move(temp,path_to_file)
-                                if ele.postdate:
-                                    set_time(path_to_file, convert_local_time(ele.postdate))
-                                if id_:
-                                    operations.write_media_table(ele,path_to_file,model_id,username)
-                                return media_type,total
-                            else:
-                                return 'skipped', 1
+                        
+                        if not pathlib.Path(temp).exists():
+                            log.debug(f"[attempt {attempt.get()}/{NUM_TRIES}] {temp} was not created") 
+                            return "skipped",1
+                        elif abs(total-pathlib.Path(temp).absolute().stat().st_size)>500:
+                            log.debug(f"[attempt {attempt.get()}/{NUM_TRIES}] {filename} size mixmatch target: {total} vs actual: {pathlib.Path(temp).absolute().stat().st_size}")   
+                            return "skipped",1 
+                        else:
+                            log.debug(f"[attempt {attempt.get()}/{NUM_TRIES}] {filename} size match target: {total} vs actual: {pathlib.Path(temp).absolute().stat().st_size}")   
+                            log.debug(f"[attempt {attempt.get()}/{NUM_TRIES}] renaming {pathlib.Path(temp).absolute()} -> {path_to_file}")   
+                            shutil.move(temp,path_to_file)
+                            if ele.postdate:
+                                set_time(path_to_file, convert_local_time(ele.postdate))
+                            if id_:
+                                operations.write_media_table(ele,path_to_file,model_id,username)
+                            return media_type,total
                     else:
                         r.raise_for_status()
     except Exception as e:
-        # if not r or r.status_code==200:
-        #     # print(traceback.format_exc())
+        log.debug(f"[attempt {attempt.get()}/{NUM_TRIES}] exception {e}")   
+        log.debug(f"[attempt {attempt.get()}/{NUM_TRIES}] exception {traceback.format_exc()}")   
         return 'skipped', 1
     finally:
         if bar:
             bar.close()
         if temp:
             pathlib.Path(temp).unlink(missing_ok=True)
```

### Comparing `ofscraper-1.83/src/utils/encoding.py` & `ofscraper-1.86/src/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.83/src/utils/exit.py` & `ofscraper-1.86/src/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.83/src/utils/paths.py` & `ofscraper-1.86/src/utils/paths.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 import re
 from rich.console import Console
 console=Console()
 import arrow
 
 from ..constants import configPath,DIR_FORMAT_DEFAULT,DATE_DEFAULT,SAVE_LOCATION_DEFAULT
 from ..utils import profiles
-from .config import read_config
+import src.utils.config as config_
 
 
 homeDir=pathlib.Path.home()
-config = read_config()['config']
+config = config_.read_config()['config']
 @contextmanager
 def set_directory(path: Path):
     """Sets the cwd within the context
 
         Args:``
             path (``Path): The path to the cwd
 
@@ -66,8 +66,14 @@
     profile = profiles.get_current_profile()
     return homeDir / configPath / profile / ".data"/f"{username}_{model_id}"/"pinned.json"
 
 def cleanup():
     console.print("Cleaning up .part files\n\n")
     root= pathlib.Path((config.get('save_location') or SAVE_LOCATION_DEFAULT))
     for file in list(filter(lambda x:re.search("\.part$",str(x))!=None,root.glob("**/*"))):
-        file.unlink(missing_ok=True)
+        file.unlink(missing_ok=True)
+
+
+def getlogpath():
+    path=pathlib.Path.home() / configPath / "logging"/f'ofscraper_{config_.get_main_profile()}_{arrow.get().format("YYYY-MM-DD")}.log'
+    createDir(path.parent)
+    return path
```

### Comparing `ofscraper-1.83/src/utils/profiles.py` & `ofscraper-1.86/src/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.83/src/utils/separate.py` & `ofscraper-1.86/src/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.83/PKG-INFO` & `ofscraper-1.86/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 1.83
+Version: 1.86
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

