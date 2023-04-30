# Comparing `tmp/mwbot-1.0.8.tar.gz` & `tmp/mwbot-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwbot-1.0.8.tar", last modified: Wed Feb  1 02:34:57 2023, max compression
+gzip compressed data, was "mwbot-1.0.9.tar", last modified: Thu Feb  2 05:37:01 2023, max compression
```

## Comparing `mwbot-1.0.8.tar` & `mwbot-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1820 2023-01-29 09:01:55.740000 mwbot-1.0.8/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-01-31 03:08:06.156000 mwbot-1.0.8/mwbot/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1756 2023-01-31 03:14:15.772000 mwbot-1.0.8/mwbot/arktool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9976 2023-02-01 02:22:34.760000 mwbot-1.0.8/mwbot/bot.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1392 2023-01-31 03:08:06.520000 mwbot-1.0.8/mwbot/prototype.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1211 2023-01-31 03:08:06.628000 mwbot-1.0.8/mwbot/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      853 2023-01-31 13:03:16.068000 mwbot-1.0.8/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-01-19 06:39:52.288000 mwbot-1.0.8/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1756 2023-01-31 03:12:48.372000 mwbot-1.0.8/tests/arktool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7867 2023-01-30 06:27:09.284000 mwbot-1.0.8/tests/bot.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1392 2023-01-19 11:10:21.952000 mwbot-1.0.8/tests/prototype.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      511 2023-01-31 03:15:10.440000 mwbot-1.0.8/tests/testfile.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1211 2023-01-30 06:29:18.072000 mwbot-1.0.8/tests/utils.py
--rw-------   0 ubuntu    (1000) ubuntu    (1000)     2080 2023-02-01 02:34:57.996000 mwbot-1.0.8/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1978 2023-02-02 05:23:10.572000 mwbot-1.0.9/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-01-31 03:08:06.156000 mwbot-1.0.9/mwbot/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1756 2023-01-31 03:14:15.772000 mwbot-1.0.9/mwbot/arktool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9949 2023-02-02 05:21:14.828000 mwbot-1.0.9/mwbot/bot.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1392 2023-01-31 03:08:06.520000 mwbot-1.0.9/mwbot/prototype.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1211 2023-01-31 03:08:06.628000 mwbot-1.0.9/mwbot/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      853 2023-02-02 05:01:22.808000 mwbot-1.0.9/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-01-19 06:39:52.288000 mwbot-1.0.9/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1756 2023-01-31 03:12:48.372000 mwbot-1.0.9/tests/arktool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7867 2023-01-30 06:27:09.284000 mwbot-1.0.9/tests/bot.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1392 2023-01-19 11:10:21.952000 mwbot-1.0.9/tests/prototype.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      511 2023-01-31 03:15:10.440000 mwbot-1.0.9/tests/testfile.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1211 2023-01-30 06:29:18.072000 mwbot-1.0.9/tests/utils.py
+-rw-------   0 ubuntu    (1000) ubuntu    (1000)     2238 2023-02-02 05:37:01.932000 mwbot-1.0.9/PKG-INFO
```

### Comparing `mwbot-1.0.8/README.md` & `mwbot-1.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 ## mwbot(Python)
+mwbot是一个基于Python的异步 Mediawiki API库，同时封装了用于[PRTS wiki](https://prts.wiki)的[部分方法](https://github.com/GuGuMur/mwbot/blob/main/mwbot/arktool.py)
 
 ## 快速使用
 ### 前备工作
 #### 安装
     pip install -i https://pypi.org/simple/ mwbot
 #### 获取Bot应有的参数
 1. 前往对应wiki的 特殊:版本 页面获取wiki的index.php, api.php的路径
@@ -35,16 +36,14 @@
             # 将username和password替换为你刚才获得的机器人登录名和密码
             # 你只能选择一种登录方式，并填入对应登录方式的登录名和密码
     await bot.login()
     
     # 样例：打印页面 用户:User 的内容
     r = await bot.get_page_text(title="用户:User")
     print(r)
-    
-    await bot.close()
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 ## 深入
-* [范例](https://github.com/GuGuMur/mwbot/tree/main/examples)
+* [示例](https://github.com/GuGuMur/mwbot/tree/main/examples)
 * [文档](https://gugumur.github.io/mwbot)
```

### Comparing `mwbot-1.0.8/mwbot/arktool.py` & `mwbot-1.0.9/mwbot/arktool.py`

 * *Files identical despite different names*

### Comparing `mwbot-1.0.8/mwbot/bot.py` & `mwbot-1.0.9/mwbot/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.password = password
         timeout = httpx.Timeout(10.0, connect=60.0, read=60.0, write=60.0, pool=60.0)
         self.client = httpx.AsyncClient(verify=False,timeout=timeout)
         self.headers = {
             'User-Agent': 'Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/67.0.3396.62 Safari/537.36'}
 
     async def __aexit__(self):
-        await self.close()
+        await self.client.aclose()
 
     async def fetch_token(self, type:str)->str:
         '''fetch_token(type:str)
         根据不同的type类型返回对应的token'''
         PARAMS = {
             'action': "query",
             'meta': "tokens",
@@ -51,16 +51,14 @@
             'format': "json"
         }
         login = await self.client.post(url=self.api, data=login_PARAMS,headers=self.headers)
         login = login.json()
         if login['login']['result'] == "Success":
             logger.info(f'Welcome to {self.sitename}, {login["login"]["lgusername"]}!')
 
-    async def close(self):
-        await self.client.aclose()
 
     async def get_data(self, title:str):
         PARAMS = {
             "action": "query",
             "prop": "revisions",
             "titles": title,
             "rvslots": "*",
@@ -104,15 +102,15 @@
             key = str(key)
             value = str(value)
             PARAMS[key] = value
         PARAMS["token"] = await self.fetch_token(type="csrf")
         PARAMS["summary"] += " //Edit by Bot."
         act = await self.client.post(url=self.api, data=PARAMS, headers=self.headers)
         act = act.json()
-        if act['edit']['result'] == "Success":
+        if ('edit'['result'] in act) & (act['edit'][result]== "Success"):
             logger.info(f'Edit [[{PARAMS["title"]}]] successfully.')
         else:
             logger.debug(act)
 
     async def create_page(self,title:str,text:str,summary:str="")->bool:
         '''创建页面'''
         deal = await self.get_data(title=title)
```

### Comparing `mwbot-1.0.8/mwbot/prototype.py` & `mwbot-1.0.9/mwbot/prototype.py`

 * *Files identical despite different names*

### Comparing `mwbot-1.0.8/mwbot/utils.py` & `mwbot-1.0.9/mwbot/utils.py`

 * *Files identical despite different names*

### Comparing `mwbot-1.0.8/pyproject.toml` & `mwbot-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mwbot"
-version = "1.0.8"
+version = "1.0.9"
 description = "个性化封装的Python Mediawiki API库"
 authors = [
     { name = "咕咕mur", email = "2221533105@qq.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
     "ujson>=5.7.0",
```

### Comparing `mwbot-1.0.8/tests/arktool.py` & `mwbot-1.0.9/tests/arktool.py`

 * *Files identical despite different names*

### Comparing `mwbot-1.0.8/tests/bot.py` & `mwbot-1.0.9/tests/bot.py`

 * *Files identical despite different names*

### Comparing `mwbot-1.0.8/tests/prototype.py` & `mwbot-1.0.9/tests/prototype.py`

 * *Files identical despite different names*

### Comparing `mwbot-1.0.8/tests/utils.py` & `mwbot-1.0.9/tests/utils.py`

 * *Files identical despite different names*

### Comparing `mwbot-1.0.8/PKG-INFO` & `mwbot-1.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: mwbot
-Version: 1.0.8
+Version: 1.0.9
 Summary: 个性化封装的Python Mediawiki API库
 License: MIT
 Keywords: Mediawiki,API,bot,auto
 Author-email: 咕咕mur <2221533105@qq.com>
 Requires-Python: >=3.9,<4.0
 Description-Content-Type: text/markdown
 
 ## mwbot(Python)
+mwbot是一个基于Python的异步 Mediawiki API库，同时封装了用于[PRTS wiki](https://prts.wiki)的[部分方法](https://github.com/GuGuMur/mwbot/blob/main/mwbot/arktool.py)
 
 ## 快速使用
 ### 前备工作
 #### 安装
     pip install -i https://pypi.org/simple/ mwbot
 #### 获取Bot应有的参数
 1. 前往对应wiki的 特殊:版本 页面获取wiki的index.php, api.php的路径
@@ -45,17 +46,15 @@
             # 将username和password替换为你刚才获得的机器人登录名和密码
             # 你只能选择一种登录方式，并填入对应登录方式的登录名和密码
     await bot.login()
     
     # 样例：打印页面 用户:User 的内容
     r = await bot.get_page_text(title="用户:User")
     print(r)
-    
-    await bot.close()
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 ## 深入
-* [范例](https://github.com/GuGuMur/mwbot/tree/main/examples)
+* [示例](https://github.com/GuGuMur/mwbot/tree/main/examples)
 * [文档](https://gugumur.github.io/mwbot)
```

