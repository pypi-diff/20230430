# Comparing `tmp/IMDbTraktSyncer-1.0.3.tar.gz` & `tmp/IMDbTraktSyncer-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDbTraktSyncer-1.0.3.tar", last modified: Sat Apr 29 21:55:10 2023, max compression
+gzip compressed data, was "IMDbTraktSyncer-1.0.4.tar", last modified: Sat Apr 29 23:21:28 2023, max compression
```

## Comparing `IMDbTraktSyncer-1.0.3.tar` & `IMDbTraktSyncer-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 21:55:10.241639 IMDbTraktSyncer-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-04-29 21:55:10.221665 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/
--rw-rw-rw-   0        0        0     6673 2023-04-29 21:54:57.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/IMDbTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-26 17:50:08.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     2280 2023-04-29 02:08:16.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0      642 2023-04-28 23:59:44.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     3697 2023-04-29 02:12:00.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/imdbRatings.py
--rw-rw-rw-   0        0        0     1802 2023-04-29 02:08:38.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     1782 2023-04-29 02:19:56.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-04-29 21:55:10.239642 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     5850 2023-04-29 21:55:10.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-04-29 21:55:10.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 21:55:10.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-04-29 21:55:10.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-04-29 21:55:10.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-29 21:55:10.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDbTraktSyncer-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     5850 2023-04-29 21:55:10.241150 IMDbTraktSyncer-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5242 2023-04-29 21:54:18.000000 IMDbTraktSyncer-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-29 21:55:10.241639 IMDbTraktSyncer-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1280 2023-04-29 21:53:14.000000 IMDbTraktSyncer-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 23:21:28.728082 IMDbTraktSyncer-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-04-29 23:21:28.696633 IMDbTraktSyncer-1.0.4/IMDbTraktSyncer/
+-rw-rw-rw-   0        0        0     6834 2023-04-29 23:20:17.000000 IMDbTraktSyncer-1.0.4/IMDbTraktSyncer/IMDbTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.0.4/IMDbTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     2280 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.0.4/IMDbTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0      642 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.0.4/IMDbTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     3825 2023-04-29 23:02:25.000000 IMDbTraktSyncer-1.0.4/IMDbTraktSyncer/imdbRatings.py
+-rw-rw-rw-   0        0        0     1835 2023-04-29 22:57:30.000000 IMDbTraktSyncer-1.0.4/IMDbTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     1782 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.0.4/IMDbTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-04-29 23:21:28.724597 IMDbTraktSyncer-1.0.4/IMDbTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     5850 2023-04-29 23:21:28.000000 IMDbTraktSyncer-1.0.4/IMDbTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-04-29 23:21:28.000000 IMDbTraktSyncer-1.0.4/IMDbTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 23:21:28.000000 IMDbTraktSyncer-1.0.4/IMDbTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-04-29 23:21:28.000000 IMDbTraktSyncer-1.0.4/IMDbTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-04-29 23:21:28.000000 IMDbTraktSyncer-1.0.4/IMDbTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-29 23:21:28.000000 IMDbTraktSyncer-1.0.4/IMDbTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDbTraktSyncer-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5850 2023-04-29 23:21:28.727085 IMDbTraktSyncer-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5242 2023-04-29 21:54:18.000000 IMDbTraktSyncer-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-29 23:21:28.728581 IMDbTraktSyncer-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1280 2023-04-29 23:20:53.000000 IMDbTraktSyncer-1.0.4/setup.py
```

### Comparing `IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/IMDbTraktSyncer.py` & `IMDbTraktSyncer-1.0.4/IMDbTraktSyncer/IMDbTraktSyncer.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,24 +70,22 @@
     if "Sign In" in element.text:
         print("Not signed in")
     else:
         print("Signed in")
         
     print('Setting IMDB Ratings')
         
-    trakt_ratings = traktRatings.trakt_ratings
-    imdb_ratings = imdbRatings.imdb_ratings
-    trakt_ratings = [rating for rating in trakt_ratings if rating['ID'] is not None] #filter out items without imdb id
-    imdb_ratings = [rating for rating in imdb_ratings if rating['ID'] is not None] #filter out items without imdb id
+    trakt_ratings = [rating for rating in traktRatings.trakt_ratings if rating['ID'] is not None]
+    imdb_ratings = [rating for rating in imdbRatings.imdb_ratings if rating['ID'] is not None]
     imdb_ratings_to_set = [rating for rating in trakt_ratings if rating['ID'] not in [imdb_rating['ID'] for imdb_rating in imdb_ratings]]
     trakt_ratings_to_set = [rating for rating in imdb_ratings if rating['ID'] not in [trakt_rating['ID'] for trakt_rating in trakt_ratings]]
 
     # loop through each movie and TV show rating and submit rating on IMDb website
-    for item in imdb_ratings_to_set:
-        print(f'{item["Title"]} ({item["Year"]}): {item["Rating"]}/10 (IMDb ID: {item["ID"]})')
+    for i, item in enumerate(imdb_ratings_to_set, 1):
+        print(f'Rating {item["Type"]}: ({i} of {len(imdb_ratings_to_set)}) {item["Title"]} ({item["Year"]}): {item["Rating"]}/10 on IMDb')
         driver.get(f'https://www.imdb.com/title/{item["ID"]}/')
         time.sleep(2)
 
         # click on "Rate" button and select rating option, then submit rating
         buttons = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, 'button.ipc-btn span')))
         found_rate_button = False
         for button in buttons:
@@ -112,39 +110,44 @@
     # Set the headers
     headers = {
         "Content-Type": "application/json",
         "trakt-api-version": "2",
         "trakt-api-key": trakt_client_id,
         "Authorization": f"Bearer {trakt_access_token}"
     }
+    
+    # Count the total number of items to rate
+    num_items = len(trakt_ratings_to_set)
+    item_count = 0
             
     # Loop through your data table and rate each item on Trakt
     for item in trakt_ratings_to_set:
-        if "ID" in item:
+        item_count += 1
+        if item["Type"] == "show":
             # This is a TV show
             data = {
                 "shows": [{
                     "ids": {
                         "imdb": item["ID"]
                     },
                     "rating": item["Rating"]
                 }]
             }
-            print(f"Rating TV show {item['Title']} ({item['Year']}) with rating {item['Rating']}/10 on Trakt")
-        else:
+            print(f"Rating TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}) with rating {item['Rating']}/10 on Trakt")
+        elif item["Type"] == "movie":
             # This is a movie
             data = {
                 "movies": [{
                     "ids": {
                         "imdb": item["ID"]
                     },
                     "rating": item["Rating"]
                 }]
             }
-            print(f"Rating movie {item['Title']} ({item['Year']}) with rating {item['Rating']}/10 on Trakt")
+            print(f"Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}) with rating {item['Rating']}/10 on Trakt")
 
         # Make the API call to rate the item
         response = requests.post(rate_url, headers=headers, json=data)
         time.sleep(1)
         while response.status_code == 429:
             print("Rate limit exceeded. Waiting for 1 second...")
             time.sleep(1)
```

### Comparing `IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/authTrakt.py` & `IMDbTraktSyncer-1.0.4/IMDbTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/checkChromedriver.py` & `IMDbTraktSyncer-1.0.4/IMDbTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/imdbRatings.py` & `IMDbTraktSyncer-1.0.4/IMDbTraktSyncer/imdbRatings.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,15 +82,19 @@
         reader = csv.reader(file)
         header = next(reader)  # skip the header row
         for row in reader:
             title = row[3]
             year = row[8]
             rating = row[1]
             imdb_id = row[0]
-            imdb_ratings.append({'Title': title, 'Year': year, 'Rating': rating, 'ID': imdb_id})
+            if "tv" in row[5]:
+                type = "show"
+            else:
+                type = "movie"
+            imdb_ratings.append({'Title': title, 'Year': year, 'Rating': rating, 'ID': imdb_id, 'Type': type})
 except FileNotFoundError:
     print('Ratings file not found')
     
 # Delete csv files
 for file in os.listdir(directory):
     if file.endswith('.csv'):
         os.remove(os.path.join(directory, file))
```

### Comparing `IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/traktRatings.py` & `IMDbTraktSyncer-1.0.4/IMDbTraktSyncer/traktRatings.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 movie_ratings = []
 show_ratings = []
 
 for item in json_data:
     if item['type'] == 'movie':
         movie = item['movie']
         movie_id = movie['ids']['imdb']
-        movie_ratings.append({'Title': movie['title'], 'Year': movie['year'], 'Rating': item['rating'], 'ID': movie_id})
+        movie_ratings.append({'Title': movie['title'], 'Year': movie['year'], 'Rating': item['rating'], 'ID': movie_id, 'Type': 'movie'})
     elif item['type'] == 'show':
         show = item['show']
         show_id = show['ids']['imdb']
-        show_ratings.append({'Title': show['title'], 'Year': show['year'], 'Rating': item['rating'], 'ID': show_id})
+        show_ratings.append({'Title': show['title'], 'Year': show['year'], 'Rating': item['rating'], 'ID': show_id, 'Type': 'show'})
 
 trakt_ratings = movie_ratings + show_ratings
 
 #print('Movie ratings:')
 #for item in movie_ratings:
 #    print(f'{item["Title"]} ({item["Year"]}): {item["Rating"]}/10 (IMDb ID: {item["ID"]})')
 #
```

### Comparing `IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/verifyCredentials.py` & `IMDbTraktSyncer-1.0.4/IMDbTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.3/IMDbTraktSyncer.egg-info/PKG-INFO` & `IMDbTraktSyncer-1.0.4/IMDbTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDbTraktSyncer
-Version: 1.0.3
+Version: 1.0.4
 Summary: This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDbTraktSyncer-1.0.3/LICENSE` & `IMDbTraktSyncer-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.3/PKG-INFO` & `IMDbTraktSyncer-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDbTraktSyncer
-Version: 1.0.3
+Version: 1.0.4
 Summary: This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDbTraktSyncer-1.0.3/README.md` & `IMDbTraktSyncer-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.3/setup.py` & `IMDbTraktSyncer-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.3'
+VERSION = '1.0.4'
 DESCRIPTION = 'This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.'
 
 # Setting up
 setup(
     name="IMDbTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

