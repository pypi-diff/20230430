# Comparing `tmp/GameMaker-0.1.2.tar.gz` & `tmp/GameMaker-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GameMaker-0.1.2.tar", last modified: Tue Mar 21 04:20:23 2023, max compression
+gzip compressed data, was "GameMaker-0.1.3.tar", last modified: Sun Apr 30 09:40:37 2023, max compression
```

## Comparing `GameMaker-0.1.2.tar` & `GameMaker-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 04:20:23.037578 GameMaker-0.1.2/
--rw-rw-rw-   0        0        0     1091 2023-01-15 07:00:47.000000 GameMaker-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      704 2023-03-21 04:20:23.035578 GameMaker-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-03-21 04:17:13.000000 GameMaker-0.1.2/README.md
--rw-rw-rw-   0        0        0      614 2023-03-21 04:19:06.000000 GameMaker-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-21 04:20:23.037675 GameMaker-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-21 04:20:22.921757 GameMaker-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-03-21 04:20:22.974679 GameMaker-0.1.2/src/GameMaker/
--rw-rw-rw-   0        0        0     8281 2023-03-21 04:15:21.000000 GameMaker-0.1.2/src/GameMaker/Assets.py
--rw-rw-rw-   0        0        0     3019 2023-03-21 04:15:21.000000 GameMaker-0.1.2/src/GameMaker/Globals.py
--rw-rw-rw-   0        0        0     1927 2023-03-21 04:15:21.000000 GameMaker-0.1.2/src/GameMaker/Helper.py
--rw-rw-rw-   0        0        0      860 2023-03-21 04:15:21.000000 GameMaker-0.1.2/src/GameMaker/Physics.py
--rw-rw-rw-   0        0        0     1670 2023-03-21 04:15:21.000000 GameMaker-0.1.2/src/GameMaker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-21 04:20:23.031578 GameMaker-0.1.2/src/GameMaker/examples/
--rw-rw-rw-   0        0        0      612 2023-03-21 04:15:21.000000 GameMaker-0.1.2/src/GameMaker/examples/Demo_Button.py
--rw-rw-rw-   0        0        0      792 2023-03-21 04:15:21.000000 GameMaker-0.1.2/src/GameMaker/examples/Demo_Collisions.py
--rw-rw-rw-   0        0        0      908 2023-03-21 04:15:21.000000 GameMaker-0.1.2/src/GameMaker/examples/Demo_Gravity.py
--rw-rw-rw-   0        0        0      241 2023-03-21 04:15:21.000000 GameMaker-0.1.2/src/GameMaker/examples/Demo_Image.py
--rw-rw-rw-   0        0        0      457 2023-03-21 04:15:21.000000 GameMaker-0.1.2/src/GameMaker/examples/Demo_ProgressBar.py
--rw-rw-rw-   0        0        0      574 2023-03-21 04:15:21.000000 GameMaker-0.1.2/src/GameMaker/examples/Demo_Text.py
--rw-rw-rw-   0        0        0      135 2023-03-21 04:15:21.000000 GameMaker-0.1.2/src/GameMaker/examples/Demo_Window.py
-drwxrwxrwx   0        0        0        0 2023-03-21 04:20:22.995411 GameMaker-0.1.2/src/GameMaker.egg-info/
--rw-rw-rw-   0        0        0      704 2023-03-21 04:20:22.000000 GameMaker-0.1.2/src/GameMaker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      577 2023-03-21 04:20:22.000000 GameMaker-0.1.2/src/GameMaker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 04:20:22.000000 GameMaker-0.1.2/src/GameMaker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-03-21 04:20:22.000000 GameMaker-0.1.2/src/GameMaker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 09:40:37.880006 GameMaker-0.1.3/
+-rw-rw-rw-   0        0        0     1091 2023-01-15 07:00:47.000000 GameMaker-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      704 2023-04-30 09:40:37.878045 GameMaker-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-03-21 04:17:13.000000 GameMaker-0.1.3/README.md
+-rw-rw-rw-   0        0        0      614 2023-04-30 09:34:48.000000 GameMaker-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 09:40:37.880006 GameMaker-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 09:40:37.836424 GameMaker-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 09:40:37.853425 GameMaker-0.1.3/src/GameMaker/
+-rw-rw-rw-   0        0        0    10203 2023-04-26 23:19:33.000000 GameMaker-0.1.3/src/GameMaker/Assets.py
+-rw-rw-rw-   0        0        0     3019 2023-03-21 23:05:56.000000 GameMaker-0.1.3/src/GameMaker/Globals.py
+-rw-rw-rw-   0        0        0     1927 2023-03-21 23:05:56.000000 GameMaker-0.1.3/src/GameMaker/Helper.py
+-rw-rw-rw-   0        0        0     1679 2023-04-24 02:18:39.000000 GameMaker-0.1.3/src/GameMaker/Physics.py
+-rw-rw-rw-   0        0        0     2046 2023-04-26 23:33:04.000000 GameMaker-0.1.3/src/GameMaker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 09:40:37.877002 GameMaker-0.1.3/src/GameMaker/examples/
+-rw-rw-rw-   0        0        0      612 2023-03-21 23:05:56.000000 GameMaker-0.1.3/src/GameMaker/examples/Demo_Button.py
+-rw-rw-rw-   0        0        0      792 2023-03-21 23:05:56.000000 GameMaker-0.1.3/src/GameMaker/examples/Demo_Collisions.py
+-rw-rw-rw-   0        0        0      908 2023-03-21 23:05:56.000000 GameMaker-0.1.3/src/GameMaker/examples/Demo_Gravity.py
+-rw-rw-rw-   0        0        0      241 2023-03-21 23:05:56.000000 GameMaker-0.1.3/src/GameMaker/examples/Demo_Image.py
+-rw-rw-rw-   0        0        0      356 2023-03-29 23:20:58.000000 GameMaker-0.1.3/src/GameMaker/examples/Demo_ImageList.py
+-rw-rw-rw-   0        0        0      457 2023-03-21 23:05:56.000000 GameMaker-0.1.3/src/GameMaker/examples/Demo_ProgressBar.py
+-rw-rw-rw-   0        0        0      574 2023-03-21 23:05:56.000000 GameMaker-0.1.3/src/GameMaker/examples/Demo_Text.py
+-rw-rw-rw-   0        0        0      135 2023-03-21 23:05:56.000000 GameMaker-0.1.3/src/GameMaker/examples/Demo_Window.py
+drwxrwxrwx   0        0        0        0 2023-04-30 09:40:37.861424 GameMaker-0.1.3/src/GameMaker.egg-info/
+-rw-rw-rw-   0        0        0      704 2023-04-30 09:40:37.000000 GameMaker-0.1.3/src/GameMaker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      618 2023-04-30 09:40:37.000000 GameMaker-0.1.3/src/GameMaker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 09:40:37.000000 GameMaker-0.1.3/src/GameMaker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-30 09:40:37.000000 GameMaker-0.1.3/src/GameMaker.egg-info/top_level.txt
```

### Comparing `GameMaker-0.1.2/LICENSE` & `GameMaker-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `GameMaker-0.1.2/PKG-INFO` & `GameMaker-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GameMaker
-Version: 0.1.2
+Version: 0.1.3
 Summary: pygame Wrapper for drawing/making games
 Author-email: Dennis Yahnov <den.yakhnov@gmail.com>
 Project-URL: Homepage, https://github.com/denyahnov/GameMaker
 Project-URL: Bug Tracker, https://github.com/denyahnov/GameMaker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `GameMaker-0.1.2/pyproject.toml` & `GameMaker-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "GameMaker"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Dennis Yahnov", email="den.yakhnov@gmail.com" },
 ]
 description = "pygame Wrapper for drawing/making games"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `GameMaker-0.1.2/src/GameMaker/Assets.py` & `GameMaker-0.1.3/src/GameMaker/Assets.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,14 +28,25 @@
 		temp_collisions = CheckCollision(obj1,obj2,x_tolerance=x_tolerance,y_tolerance=y_tolerance)
 		for i in temp_collisions:
 			if temp_collisions[i] != None:
 				all_collisions[i] = obj2
 
 	return all_collisions
 
+def ImageList(
+		image: str,
+		size: tuple[int,int],
+		x_copies: int,
+		y_copies: int,
+		x_offset: int = 0,
+		y_offset: int = 0
+	):
+
+	return [Image(image,[x * (x_offset + size[0]), y * (y_offset + size[1]),size[0],size[1]]) for x in range(x_copies) for y in range(y_copies)]
+
 class Text():
 	def __init__(
 			self,
 			text: str,
 			position: [int,int],
 			font_name: str = 'freesansbold.ttf',
 			color: tuple[int,int,int] = (0,0,0),
@@ -66,15 +77,22 @@
 
 		self.rect = self.rendered_text.get_rect()
 
 		self.w, self.h = self.rect.w, self.rect.h
 
 		self.rect.center = self.x + ((self.w // 2) * self.center[1]), self. y + ((self.h // 2) * self.center[0])
 
+	def update(self,text):
+		self.text = str(text)
+
+		self.rendered_text = self.font.render(self.text, self.antialias, self.color, self.background)
+		self.rect = self.rendered_text.get_rect()
+
 	def draw(self,window):
+		self.rect.center = self.x + ((self.w // 2) * self.center[1]), self. y + ((self.h // 2) * self.center[0])
 		window.blit(self.rendered_text,self.rect)
 
 class Rectangle():
 	def __init__(
 			self,
 			position: list[int,int,int,int],
 			background_color: tuple[int,int,int] = (50,50,50),
@@ -251,22 +269,77 @@
 			position: [int,int,int,int],
 		):
 		
 		self.path = path
 
 		self.collision_mask = self.x, self.y, self.w, self.h = position
 
-		self.image = pg.image.load(path)
+		self.image = pg.image.load(path).convert_alpha()
 
 		self.image = pg.transform.scale(self.image, (self.w, self.h))
 
 		self.rect = self.image.get_rect()
 
 		self.rect.x = self.x
 		self.rect.y = self.y
 		
 	def draw(self,window):
 		window.blit(self.image,self.rect)
 
+class RotatedImage():
+	def __init__(
+			self,
+			path: str,
+			position: [int,int,int,int],
+			rotation: float = 0.0,
+		):
+		
+		self.path = path
+
+		self.collision_mask = self.x, self.y, self.w, self.h = position
+
+		self.image = pg.image.load(path).convert_alpha()
+
+		self.image = pg.transform.scale(self.image, (self.w, self.h))
+
+		self.rect = self.image.get_rect()
+
+		self.rect.x = self.x
+		self.rect.y = self.y
+
+		self.rotation = rotation
+		
+	def draw(self,window):
+		rotated = pg.transform.rotate(self.image, self.rotation)
+
+		self.rect = rotated.get_rect()
+
+		self.rect.center = (self.x + self.w/2, self.y + self.h/2)
+
+		window.blit(rotated,self.rect)
+
+		self.collision_mask = self.rect
+
 class ScriptedObject():
 	def __init__(self,sprite: str, script: type(lambda x: None)):
-		pass
+		pass
+
+class AlphaRectangle():
+	def __init__(
+			self,
+			position: list[int,int,int,int],
+			color: tuple[int,int,int] = (200,200,200,255),
+			rotation: float = 0.0,
+		):
+
+		self.collision_mask = self.x, self.y, self.w, self.h = position
+		self.rotation = rotation
+		self.color = color
+
+	def draw(self,window):
+		surface = pg.Surface((self.w,self.h))
+		surface.set_alpha(self.color[3])
+		surface.fill(self.color[0:3])
+		new = pg.transform.rotate(surface, self.rotation)
+		rect = new.get_rect()
+		rect.center = (self.x + self.w/2, self.y + self.h/2)
+		window.blit(new,rect)
```

### Comparing `GameMaker-0.1.2/src/GameMaker/Globals.py` & `GameMaker-0.1.3/src/GameMaker/Globals.py`

 * *Files identical despite different names*

### Comparing `GameMaker-0.1.2/src/GameMaker/Helper.py` & `GameMaker-0.1.3/src/GameMaker/Helper.py`

 * *Files identical despite different names*

### Comparing `GameMaker-0.1.2/src/GameMaker/__init__.py` & `GameMaker-0.1.3/src/GameMaker/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,35 +8,47 @@
 	def __init__(
 			self,
 			screen_size: tuple[int,int],
 			title: str = "My Game",
 			fps: int = 60, 
 			background_color: tuple[int,int,int] = (255,255,255),
 			no_frame=False,
+			fullscreen=False,
 		):
 		pg.init()
 
 		self.RES = self.WIDTH, self.HEIGHT = screen_size
 		self.H_WIDTH, self.H_HEIGHT = self.WIDTH // 2, self.HEIGHT // 2
 
 		self.FPS = fps
 
-		self.screen = pg.display.set_mode(self.RES) if not no_frame else pg.display.set_mode(self.RES,pg.NOFRAME)
+		self.fullscreen = fullscreen
+
+		if self.fullscreen:
+			self.screen = pg.display.set_mode((self.WIDTH, self.HEIGHT),pg.FULLSCREEN)
+
+			self.RES = self.WIDTH, self.HEIGHT = self.screen.get_width(), self.screen.get_height()
+			self.H_WIDTH, self.H_HEIGHT = self.WIDTH // 2, self.HEIGHT // 2
+		else:
+			self.screen = pg.display.set_mode(self.RES) if not no_frame else pg.display.set_mode(self.RES,pg.NOFRAME)
+
 		self.clock = pg.time.Clock()
 
 		self.title = title
 		self.background_color = background_color
 
 		self.RUNNING = True
 
 		self.update_title(self.title)
 
 		self.drawlist = [[],[],[]]
 		self.keys_up = []
 
+		self.screen.fill(self.background_color)
+
 	def draw(self,item: list,layer: int = FOREGROUND) -> None:
 		if type(item) == list:
 			for i in item:
 				self.drawlist[layer].append(i)
 		else:
 			self.drawlist[layer].append(item)
 
@@ -48,30 +60,29 @@
 		return pg.key.get_pressed()
 
 	def get_key(self,key: int) -> bool:
 		return self.keys()[key]
 
 	def update(self) -> None:
 		self.keys_up = []
-
-		self.clock.tick(self.FPS)
-
+		
 		for e in pg.event.get():
 			if e.type == pg.QUIT:
 				pg.quit()
 				self.RUNNING = False
 				return
 			elif e.type == pg.KEYUP:
 				self.keys_up.append(e.key)
 
-		self.screen.fill(self.background_color)
-
 		for layer in self.drawlist:
 			for item in layer:
 				item.draw(self.screen)
 
 		self.drawlist = [[],[],[]]
 
 		pg.display.update()
+		self.clock.tick(self.FPS)
+
+		self.screen.fill(self.background_color)
 
 	def close(self) -> None:
 		self.RUNNING = False
```

### Comparing `GameMaker-0.1.2/src/GameMaker/examples/Demo_Button.py` & `GameMaker-0.1.3/src/GameMaker/examples/Demo_Button.py`

 * *Files identical despite different names*

### Comparing `GameMaker-0.1.2/src/GameMaker/examples/Demo_Collisions.py` & `GameMaker-0.1.3/src/GameMaker/examples/Demo_Collisions.py`

 * *Files identical despite different names*

### Comparing `GameMaker-0.1.2/src/GameMaker/examples/Demo_Gravity.py` & `GameMaker-0.1.3/src/GameMaker/examples/Demo_Gravity.py`

 * *Files identical despite different names*

### Comparing `GameMaker-0.1.2/src/GameMaker/examples/Demo_Text.py` & `GameMaker-0.1.3/src/GameMaker/examples/Demo_Text.py`

 * *Files identical despite different names*

### Comparing `GameMaker-0.1.2/src/GameMaker.egg-info/PKG-INFO` & `GameMaker-0.1.3/src/GameMaker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GameMaker
-Version: 0.1.2
+Version: 0.1.3
 Summary: pygame Wrapper for drawing/making games
 Author-email: Dennis Yahnov <den.yakhnov@gmail.com>
 Project-URL: Homepage, https://github.com/denyahnov/GameMaker
 Project-URL: Bug Tracker, https://github.com/denyahnov/GameMaker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `GameMaker-0.1.2/src/GameMaker.egg-info/SOURCES.txt` & `GameMaker-0.1.3/src/GameMaker.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,10 +10,11 @@
 src/GameMaker.egg-info/SOURCES.txt
 src/GameMaker.egg-info/dependency_links.txt
 src/GameMaker.egg-info/top_level.txt
 src/GameMaker/examples/Demo_Button.py
 src/GameMaker/examples/Demo_Collisions.py
 src/GameMaker/examples/Demo_Gravity.py
 src/GameMaker/examples/Demo_Image.py
+src/GameMaker/examples/Demo_ImageList.py
 src/GameMaker/examples/Demo_ProgressBar.py
 src/GameMaker/examples/Demo_Text.py
 src/GameMaker/examples/Demo_Window.py
```

