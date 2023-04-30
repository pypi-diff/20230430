# Comparing `tmp/psic-0.0.8.9.tar.gz` & `tmp/psic-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psic-0.0.8.9.tar", last modified: Mon Feb 27 14:17:40 2023, max compression
+gzip compressed data, was "psic-0.0.9.tar", last modified: Sun Apr 30 15:21:02 2023, max compression
```

## Comparing `psic-0.0.8.9.tar` & `psic-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-02-27 14:17:40.474476 psic-0.0.8.9/
--rw-rw-rw-   0        0        0    35803 2022-09-03 18:02:06.000000 psic-0.0.8.9/LICENSE
--rw-rw-rw-   0        0        0      891 2023-02-27 14:17:40.473980 psic-0.0.8.9/PKG-INFO
--rw-rw-rw-   0        0        0      395 2022-09-16 12:17:58.000000 psic-0.0.8.9/README.md
--rw-rw-rw-   0        0        0       42 2023-02-27 14:17:40.474476 psic-0.0.8.9/setup.cfg
--rw-rw-rw-   0        0        0      805 2023-02-27 14:17:03.000000 psic-0.0.8.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-27 14:17:40.454637 psic-0.0.8.9/src/
-drwxrwxrwx   0        0        0        0 2023-02-27 14:17:40.467533 psic-0.0.8.9/src/psic/
--rw-rw-rw-   0        0        0        0 2022-09-03 18:02:06.000000 psic-0.0.8.9/src/psic/__init__.py
--rw-rw-rw-   0        0        0     4334 2022-09-05 13:01:14.000000 psic-0.0.8.9/src/psic/calc_fraction.py
--rw-rw-rw-   0        0        0    18780 2022-12-21 13:17:10.000000 psic-0.0.8.9/src/psic/create_mesh.py
--rw-rw-rw-   0        0        0     4901 2023-02-27 14:05:54.000000 psic-0.0.8.9/src/psic/create_submodel.py
--rw-rw-rw-   0        0        0    15514 2023-02-27 14:06:18.000000 psic-0.0.8.9/src/psic/packing_spheres_in_cube.py
--rw-rw-rw-   0        0        0     1873 2023-02-27 14:15:53.000000 psic-0.0.8.9/src/psic/plot_model.py
-drwxrwxrwx   0        0        0        0 2023-02-27 14:17:40.472493 psic-0.0.8.9/src/psic.egg-info/
--rw-rw-rw-   0        0        0      891 2023-02-27 14:17:40.000000 psic-0.0.8.9/src/psic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-02-27 14:17:40.000000 psic-0.0.8.9/src/psic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-27 14:17:40.000000 psic-0.0.8.9/src/psic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-02-27 14:17:40.000000 psic-0.0.8.9/src/psic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 15:21:02.077247 psic-0.0.9/
+-rw-rw-rw-   0        0        0    35803 2022-09-03 18:02:06.000000 psic-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      889 2023-04-30 15:21:02.076427 psic-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2022-09-16 12:17:58.000000 psic-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-30 15:21:02.077247 psic-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      803 2023-04-30 15:19:07.000000 psic-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 15:21:02.050659 psic-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 15:21:02.066506 psic-0.0.9/src/psic/
+-rw-rw-rw-   0        0        0        0 2022-09-03 18:02:06.000000 psic-0.0.9/src/psic/__init__.py
+-rw-rw-rw-   0        0        0     4508 2023-04-30 15:19:07.000000 psic-0.0.9/src/psic/calc_fraction.py
+-rw-rw-rw-   0        0        0    19040 2023-04-30 15:19:07.000000 psic-0.0.9/src/psic/create_mesh.py
+-rw-rw-rw-   0        0        0     4927 2023-04-30 15:19:07.000000 psic-0.0.9/src/psic/create_submodel.py
+-rw-rw-rw-   0        0        0    15646 2023-04-30 15:19:07.000000 psic-0.0.9/src/psic/packing_spheres_in_cube.py
+-rw-rw-rw-   0        0        0     1868 2023-04-30 15:19:07.000000 psic-0.0.9/src/psic/plot_model.py
+drwxrwxrwx   0        0        0        0 2023-04-30 15:21:02.074442 psic-0.0.9/src/psic.egg-info/
+-rw-rw-rw-   0        0        0      889 2023-04-30 15:21:02.000000 psic-0.0.9/src/psic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-04-30 15:21:02.000000 psic-0.0.9/src/psic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 15:21:02.000000 psic-0.0.9/src/psic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-30 15:21:02.000000 psic-0.0.9/src/psic.egg-info/top_level.txt
```

### Comparing `psic-0.0.8.9/LICENSE` & `psic-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `psic-0.0.8.9/PKG-INFO` & `psic-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psic
-Version: 0.0.8.9
+Version: 0.0.9
 Summary: Packing spheres in cube
 Home-page: https://github.com/sunwhale/psic
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/psic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `psic-0.0.8.9/setup.py` & `psic-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="psic",
-    version="0.0.8.9",
+    version="0.0.9",
     author="Jingyu Sun",
     author_email="sun.jingyu@outlook.com",
     description="Packing spheres in cube",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sunwhale/psic",
     project_urls={
```

### Comparing `psic-0.0.8.9/src/psic/calc_fraction.py` & `psic-0.0.9/src/psic/calc_fraction.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 """
 计算球体在立方体中的体积分数
 """
-
 import numpy as np
 
 
 def is_in_rectangle(point, xmin, xmax, ymin, ymax):  # 判断点位置在矩形内外
     x = point[0]
     y = point[1]
     if xmin <= x <= xmax and ymin <= y <= ymax:
@@ -15,62 +14,62 @@
         return False
 
 
 def cross_num(center, r, xmin, xmax, ymin, ymax):  # 判断圆与直线相交数量
     x = center[0]
     y = center[1]
     num = 0
-    if x-r <= xmin <= x+r or x-r <= xmax <= x+r:
+    if x - r <= xmin <= x + r or x - r <= xmax <= x + r:
         num += 1
-    if y-r <= ymin <= y+r or y-r <= ymax <= y+r:
+    if y - r <= ymin <= y + r or y - r <= ymax <= y + r:
         num += 1
     return num
 
 
 def calc_axisX_cross_point(center, r, Y):
     x0 = center[0]
     y0 = center[1]
-    a = -2*x0
-    b = -2*y0
-    c = x0**2 + y0**2 - r**2
-    e = Y**2 + b*Y + c
-    if a**2 - 4*e < 0:
+    a = -2 * x0
+    b = -2 * y0
+    c = x0 ** 2 + y0 ** 2 - r ** 2
+    e = Y ** 2 + b * Y + c
+    if a ** 2 - 4 * e < 0:
         return []
-    delta = np.sqrt(a**2 - 4*e)
-    root1 = (-a + delta)/2.0
-    root2 = (-a - delta)/2.0
+    delta = np.sqrt(a ** 2 - 4 * e)
+    root1 = (-a + delta) / 2.0
+    root2 = (-a - delta) / 2.0
     return [[root1, Y], [root2, Y]]
 
 
 def calc_axisY_cross_point(center, r, X):
     x0 = center[0]
     y0 = center[1]
-    a = -2*x0
-    b = -2*y0
-    c = x0**2 + y0**2 - r**2
-    e = X**2 + a*X + c
-    if b**2 - 4*e < 0:
+    a = -2 * x0
+    b = -2 * y0
+    c = x0 ** 2 + y0 ** 2 - r ** 2
+    e = X ** 2 + a * X + c
+    if b ** 2 - 4 * e < 0:
         return []
-    delta = np.sqrt(b**2 - 4*e)
-    root1 = (-b + delta)/2.0
-    root2 = (-b - delta)/2.0
+    delta = np.sqrt(b ** 2 - 4 * e)
+    root1 = (-b + delta) / 2.0
+    root2 = (-b - delta) / 2.0
     return [[X, root1], [X, root2]]
 
 
 def calc_cross_points(center, r, xmin, xmax, ymin, ymax):
     p1 = calc_axisY_cross_point(center, r, xmin)
     p2 = calc_axisY_cross_point(center, r, xmax)
     p3 = calc_axisX_cross_point(center, r, ymin)
     p4 = calc_axisX_cross_point(center, r, ymax)
-    return p1+p2+p3+p4
+    return p1 + p2 + p3 + p4
 
 
 def calc_minor_area(chrod_length, r):
-    half_angle = np.arcsin(0.5*chrod_length/r)
-    minor_area = r**2*half_angle - 0.5*chrod_length*r*np.cos(half_angle)
+    half_angle = np.arcsin(0.5 * chrod_length / r)
+    minor_area = r ** 2 * half_angle - 0.5 * chrod_length * r * np.cos(half_angle)
     return minor_area
 
 
 def calc_area_fraction(centers, radiuses, size):
     xmin, xmax, ymin, ymax = size[0][0], size[0][1], size[1][0], size[1][1]
     circles_area = 0
     for i, center in enumerate(centers):
@@ -80,43 +79,47 @@
         if num_int > 0:
             points = calc_cross_points(center, r, xmin, xmax, ymin, ymax)
             cross_points = []
             for point in points:
                 if is_in_rectangle(point, xmin, xmax, ymin, ymax):
                     cross_points.append(point)
             if len(cross_points) > 0:
-                chrod_length = np.sqrt((cross_points[0][0]-cross_points[1][0])**2+(cross_points[0][1]-cross_points[1][1])**2)
+                chrod_length = np.sqrt(
+                    (cross_points[0][0] - cross_points[1][0]) ** 2 + (cross_points[0][1] - cross_points[1][1]) ** 2)
         area = 0
         if is_in_rectangle(center, xmin, xmax, ymin, ymax) and num_int == 0:
-            area = np.pi*r**2
+            area = np.pi * r ** 2
         elif is_in_rectangle(center, xmin, xmax, ymin, ymax) and num_int == 1 and len(cross_points) > 0:
-            area = np.pi*r**2 - calc_minor_area(chrod_length, r)
+            area = np.pi * r ** 2 - calc_minor_area(chrod_length, r)
         elif is_in_rectangle(center, xmin, xmax, ymin, ymax) == False and num_int == 1 and len(cross_points) > 0:
             area = calc_minor_area(chrod_length, r)
         elif num_int == 2 and len(cross_points) > 0:
-            area = calc_minor_area(chrod_length, r) + np.absolute(0.5*(cross_points[0][0]-cross_points[1][0])*(cross_points[0][1]-cross_points[1][1]))
+            area = calc_minor_area(chrod_length, r) + np.absolute(
+                0.5 * (cross_points[0][0] - cross_points[1][0]) * (cross_points[0][1] - cross_points[1][1]))
         circles_area += area
-                
-    fraction = circles_area/(xmax-xmin)/(ymax-ymin)
+
+    fraction = circles_area / (xmax - xmin) / (ymax - ymin)
     return fraction
 
 
 def calc_volume_fraction(centers, radiuses, size):
     volume = 1.0
     for s in size:
         volume *= (s[1] - s[0])
-    return np.sum(4.0/3.0*np.pi*radiuses**3)/volume
-    
-    
+    return np.sum(4.0 / 3.0 * np.pi * radiuses ** 3) / volume
+
+
 if __name__ == "__main__":
-    centers = [[0.67903757, 0.37195601], [0.36737042, -0.01959854], [-0.01426161, 0.2907907, ], [0.46292355, 1.01283521], [0.29917023, 1.02242966], [1.0233473, -0.02120813],
-               [0.80638937, 0.70588318], [-0.03138388, 0.90409142], [1.01879076, 0.83622931], [0.37065488, 0.66405636], [0.84560447, 1.01858671], [0.64792281, 0.80065118], [0.2646079, 0.50382419]]
+    centers = [[0.67903757, 0.37195601], [0.36737042, -0.01959854], [-0.01426161, 0.2907907, ],
+               [0.46292355, 1.01283521], [0.29917023, 1.02242966], [1.0233473, -0.02120813],
+               [0.80638937, 0.70588318], [-0.03138388, 0.90409142], [1.01879076, 0.83622931], [0.37065488, 0.66405636],
+               [0.84560447, 1.01858671], [0.64792281, 0.80065118], [0.2646079, 0.50382419]]
 
     radiuses = [[0.21479203], [0.26824568], [0.1926382], [0.0552244], [0.10880974], [0.18590287],
                 [0.0876847], [0.10656674], [0.07639095], [0.07590341], [0.09191926], [0.07027798], [0.08319493]]
 
     size = [[0, 1], [0, 1]]
-    
+
     centers = np.array(centers)
     radiuses = np.array(radiuses)
 
     print('圆形面积占比', calc_area_fraction(centers, radiuses, size))
```

### Comparing `psic-0.0.8.9/src/psic/create_mesh.py` & `psic-0.0.9/src/psic/create_mesh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 生成四边形/六面体网格
 """
+import json
+import os
 
 import numpy as np
-import os
-import json
 
 
 def node_number(i, j, k, l, m, n):
     '''
     生成i，j，k对应的节点号
 
     Parameters
@@ -29,15 +29,15 @@
 
     Returns
     -------
     int
         节点编号
 
     '''
-    return k*l*m + j*l + i
+    return k * l * m + j * l + i
 
 
 def element_node_C3D8(i, j, k, l, m, n):
     '''
     生成i，j，k对应的三维单元的节点号
 
     Parameters
@@ -72,21 +72,21 @@
     n7 : int
         单元的7节点对应的总节点编号
     n8 : int
         单元的8节点对应的总节点编号
 
     '''
     n1 = node_number(i, j, k, l, m, n)
-    n2 = node_number(i+1, j, k, l, m, n)
-    n3 = node_number(i+1, j+1, k, l, m, n)
-    n4 = node_number(i, j+1, k, l, m, n)
-    n5 = node_number(i, j, k+1, l, m, n)
-    n6 = node_number(i+1, j, k+1, l, m, n)
-    n7 = node_number(i+1, j+1, k+1, l, m, n)
-    n8 = node_number(i, j+1, k+1, l, m, n)
+    n2 = node_number(i + 1, j, k, l, m, n)
+    n3 = node_number(i + 1, j + 1, k, l, m, n)
+    n4 = node_number(i, j + 1, k, l, m, n)
+    n5 = node_number(i, j, k + 1, l, m, n)
+    n6 = node_number(i + 1, j, k + 1, l, m, n)
+    n7 = node_number(i + 1, j + 1, k + 1, l, m, n)
+    n8 = node_number(i, j + 1, k + 1, l, m, n)
     return n1, n2, n3, n4, n5, n6, n7, n8
 
 
 def element_node_CPE4(i, j, l, m):
     '''
     生成i，j对应的二维单元的节点号
 
@@ -112,17 +112,17 @@
     n4 : array
         单元的4节点对应的总节点编号
 
     '''
     k = 0
     n = 0
     n1 = node_number(i, j, k, l, m, n)
-    n2 = node_number(i+1, j, k, l, m, n)
-    n3 = node_number(i+1, j+1, k, l, m, n)
-    n4 = node_number(i, j+1, k, l, m, n)
+    n2 = node_number(i + 1, j, k, l, m, n)
+    n3 = node_number(i + 1, j + 1, k, l, m, n)
+    n4 = node_number(i, j + 1, k, l, m, n)
     return n1, n2, n3, n4
 
 
 def element_centroid(node_shape, dimension):
     '''
     生成单元中心点的坐标数组
 
@@ -136,27 +136,27 @@
     Returns
     -------
     array
         单元中心点在不同方向上的坐标数组
 
     '''
     if len(node_shape) == 2:
-        x = np.linspace(dimension[0]/(node_shape[0]-1)/2, dimension[0] -
-                        dimension[0]/(node_shape[0]-1)/2, node_shape[0]-1)
-        y = np.linspace(dimension[1]/(node_shape[1]-1)/2, dimension[1] -
-                        dimension[1]/(node_shape[1]-1)/2, node_shape[1]-1)
+        x = np.linspace(dimension[0] / (node_shape[0] - 1) / 2, dimension[0] -
+                        dimension[0] / (node_shape[0] - 1) / 2, node_shape[0] - 1)
+        y = np.linspace(dimension[1] / (node_shape[1] - 1) / 2, dimension[1] -
+                        dimension[1] / (node_shape[1] - 1) / 2, node_shape[1] - 1)
         x, y = np.meshgrid(x, y)
         return x, y
     if len(node_shape) == 3:
-        x = np.linspace(dimension[0]/(node_shape[0]-1)/2, dimension[0] -
-                        dimension[0]/(node_shape[0]-1)/2, node_shape[0]-1)
-        y = np.linspace(dimension[1]/(node_shape[1]-1)/2, dimension[1] -
-                        dimension[1]/(node_shape[1]-1)/2, node_shape[1]-1)
-        z = np.linspace(dimension[2]/(node_shape[2]-1)/2, dimension[2] -
-                        dimension[2]/(node_shape[2]-1)/2, node_shape[2]-1)
+        x = np.linspace(dimension[0] / (node_shape[0] - 1) / 2, dimension[0] -
+                        dimension[0] / (node_shape[0] - 1) / 2, node_shape[0] - 1)
+        y = np.linspace(dimension[1] / (node_shape[1] - 1) / 2, dimension[1] -
+                        dimension[1] / (node_shape[1] - 1) / 2, node_shape[1] - 1)
+        z = np.linspace(dimension[2] / (node_shape[2] - 1) / 2, dimension[2] -
+                        dimension[2] / (node_shape[2] - 1) / 2, node_shape[2] - 1)
         x, y, z = np.meshgrid(x, y, z)
         return x, y, z
     return 0
 
 
 def create_node_coordinate(node_shape, dimension):
     '''
@@ -220,18 +220,18 @@
 
     Returns
     -------
     array
         与单元位置对应的索引编号数组
 
     '''
-    element_shape = [n-1 for n in node_shape]
+    element_shape = [n - 1 for n in node_shape]
     element_size = 1
     for n in node_shape:
-        element_size *= (n-1)
+        element_size *= (n - 1)
     return np.arange(element_size).reshape(element_shape)
 
 
 def create_lmn(node_shape):
     '''
     生成l, m, n
 
@@ -269,15 +269,15 @@
 
     Returns
     -------
     tuple
         每个坐标方向上的单元编号
 
     '''
-    element_shape = [n-1 for n in node_shape]
+    element_shape = [n - 1 for n in node_shape]
     ijk = [np.arange(n) for n in element_shape]
     if len(node_shape) == 2:
         i, j = np.meshgrid(ijk[0], ijk[1])
         return i, j
     elif len(node_shape) == 3:
         j, k, i = np.meshgrid(ijk[0], ijk[1], ijk[2])
         return i, j, k
@@ -289,29 +289,29 @@
     outfile = open(filename, 'w')
 
     outfile.write('*Part, name=PART-1\n')
     outfile.write('*Node\n')
 
     if dim == 2:
         for num, x, y in np.nditer(nodes):
-            outfile.write('%s, %s, %s, %s\n' % (num+1, x, y, 0))
+            outfile.write('%s, %s, %s, %s\n' % (num + 1, x, y, 0))
 
         outfile.write('*Element, type=%s\n' % element_type)
         for num, n1, n2, n3, n4 in np.nditer(elements):
             outfile.write('%s, %s, %s, %s, %s\n' %
-                          (num+1, n1+1, n2+1, n3+1, n4+1))
+                          (num + 1, n1 + 1, n2 + 1, n3 + 1, n4 + 1))
 
     elif dim >= 3:
         for num, x, y, z in np.nditer(nodes):
-            outfile.write('%s, %s, %s, %s,%s\n' % (num+1, x, y, z, 0))
+            outfile.write('%s, %s, %s, %s,%s\n' % (num + 1, x, y, z, 0))
 
         outfile.write('*Element, type=%s\n' % element_type)
         for num, n1, n2, n3, n4, n5, n6, n7, n8 in np.nditer(elements):
             outfile.write('%s, %s, %s, %s, %s, %s, %s, %s, %s\n' % (
-                num+1, n1+1, n2+1, n3+1, n4+1, n5+1, n6+1, n7+1, n8+1))
+                num + 1, n1 + 1, n2 + 1, n3 + 1, n4 + 1, n5 + 1, n6 + 1, n7 + 1, n8 + 1))
 
     for key in element_sets_dict.keys():
         outfile.write('*Elset, elset=ELSET_%s\n' % key)
         count = 0
         for i in element_sets_dict[key]:
             count += 1
             if count == len(element_sets_dict[key]):
@@ -328,15 +328,15 @@
         count += 1
         if count == len(nodes[0]):
             end = '\n'
         elif count % 8 == 0:
             end = '\n'
         else:
             end = ','
-        outfile.write(str(node+1) + end)
+        outfile.write(str(node + 1) + end)
 
     if dim == 2:
         x0 = min(nodes[1])
         x1 = max(nodes[1])
         y0 = min(nodes[2])
         y1 = max(nodes[2])
         node_sets_dict = {
@@ -371,35 +371,35 @@
             'X0Y1Z0': nodes[0][(nodes[1] == x0) & (nodes[2] == y1) & (nodes[3] == z0)],
             'X0Y1Z1': nodes[0][(nodes[1] == x0) & (nodes[2] == y1) & (nodes[3] == z1)],
             'X1Y0Z0': nodes[0][(nodes[1] == x1) & (nodes[2] == y0) & (nodes[3] == z0)],
             'X1Y0Z1': nodes[0][(nodes[1] == x1) & (nodes[2] == y0) & (nodes[3] == z1)],
             'X1Y1Z0': nodes[0][(nodes[1] == x1) & (nodes[2] == y1) & (nodes[3] == z0)],
             'X1Y1Z1': nodes[0][(nodes[1] == x1) & (nodes[2] == y1) & (nodes[3] == z1)]
         }
-        
+
     for key in node_sets_dict.keys():
         outfile.write('*Nset, nset=%s\n' % key)
         count = 0
         for node in np.nditer(node_sets_dict[key]):
             count += 1
             if count == len(node_sets_dict[key]):
                 end = '\n'
             elif count % 8 == 0:
                 end = '\n'
             else:
                 end = ','
-            outfile.write(str(node+1) + end)
+            outfile.write(str(node + 1) + end)
 
     outfile.close()
 
 
 def mesh(gap, dimension, node_shape, element_type, model_path, output_path, status, is_interface=True):
     model_file = os.path.join(model_path, 'model.npy')
     circles = np.load(model_file)
-    dim = circles.shape[-1]-1
+    dim = circles.shape[-1] - 1
     if dim == 2:
         node_index = create_node_index(node_shape)
         element_index = create_element_index(node_shape)
 
         x, y = create_node_coordinate(node_shape, dimension)
         ecx, ecy = element_centroid(node_shape, dimension)
 
@@ -418,40 +418,40 @@
         n1 = n1.flatten()
         n2 = n2.flatten()
         n3 = n3.flatten()
         n4 = n4.flatten()
         elements = [element_index, n1, n2, n3, n4]
 
         element_sets = np.zeros(len(element_index))
-            
+
         n1x = x[n1]
         n1y = y[n1]
         n2x = x[n2]
         n2y = y[n2]
         n3x = x[n3]
         n3y = y[n3]
         n4x = x[n4]
         n4y = y[n4]
-        
+
         if not is_interface:
             for i, circle in enumerate(circles):
                 cx = circle[0]
                 cy = circle[1]
                 r = circle[2] - gap
-                index = (ecx - cx)**2 + (ecy - cy)**2 < r**2
+                index = (ecx - cx) ** 2 + (ecy - cy) ** 2 < r ** 2
                 element_sets[index] = int(i) + 1
         else:
             for i, circle in enumerate(circles):
                 cx = circle[0]
                 cy = circle[1]
                 r = circle[2] - gap
-                index1 = (n1x-cx)**2 + (n1y-cy)**2 < r**2
-                index2 = (n2x-cx)**2 + (n2y-cy)**2 < r**2
-                index3 = (n3x-cx)**2 + (n3y-cy)**2 < r**2
-                index4 = (n4x-cx)**2 + (n4y-cy)**2 < r**2
+                index1 = (n1x - cx) ** 2 + (n1y - cy) ** 2 < r ** 2
+                index2 = (n2x - cx) ** 2 + (n2y - cy) ** 2 < r ** 2
+                index3 = (n3x - cx) ** 2 + (n3y - cy) ** 2 < r ** 2
+                index4 = (n4x - cx) ** 2 + (n4y - cy) ** 2 < r ** 2
                 index_inner = index1 & index2 & index3 & index4
                 element_sets[index_inner] = int(i) + 1
                 index_inter = (index1 | index2 | index3 | index4) ^ index_inner
                 element_sets[index_inter] = -1
 
     elif dim >= 3:
         node_index = create_node_index(node_shape)
@@ -504,70 +504,69 @@
         n6z = z[n6]
         n7x = x[n7]
         n7y = y[n7]
         n7z = z[n7]
         n8x = x[n8]
         n8y = y[n8]
         n8z = z[n8]
-        
+
         if not is_interface:
             for i, circle in enumerate(circles):
                 cx = circle[0]
                 cy = circle[1]
                 cz = circle[2]
                 r = circle[-1] - gap
-                index = (ecx - cx)**2 + (ecy - cy)**2 + (ecz-cz)**2 < r**2
+                index = (ecx - cx) ** 2 + (ecy - cy) ** 2 + (ecz - cz) ** 2 < r ** 2
                 element_sets[index] = int(i) + 1
         else:
             for i, circle in enumerate(circles):
                 cx = circle[0]
                 cy = circle[1]
                 cz = circle[2]
                 r = circle[-1] - gap
-                index1 = (n1x-cx)**2 + (n1y-cy)**2 + (n1z-cz)**2 < r**2
-                index2 = (n2x-cx)**2 + (n2y-cy)**2 + (n2z-cz)**2 < r**2
-                index3 = (n3x-cx)**2 + (n3y-cy)**2 + (n3z-cz)**2 < r**2
-                index4 = (n4x-cx)**2 + (n4y-cy)**2 + (n4z-cz)**2 < r**2
-                index5 = (n5x-cx)**2 + (n5y-cy)**2 + (n5z-cz)**2 < r**2
-                index6 = (n6x-cx)**2 + (n6y-cy)**2 + (n6z-cz)**2 < r**2
-                index7 = (n7x-cx)**2 + (n7y-cy)**2 + (n7z-cz)**2 < r**2
-                index8 = (n8x-cx)**2 + (n8y-cy)**2 + (n8z-cz)**2 < r**2
+                index1 = (n1x - cx) ** 2 + (n1y - cy) ** 2 + (n1z - cz) ** 2 < r ** 2
+                index2 = (n2x - cx) ** 2 + (n2y - cy) ** 2 + (n2z - cz) ** 2 < r ** 2
+                index3 = (n3x - cx) ** 2 + (n3y - cy) ** 2 + (n3z - cz) ** 2 < r ** 2
+                index4 = (n4x - cx) ** 2 + (n4y - cy) ** 2 + (n4z - cz) ** 2 < r ** 2
+                index5 = (n5x - cx) ** 2 + (n5y - cy) ** 2 + (n5z - cz) ** 2 < r ** 2
+                index6 = (n6x - cx) ** 2 + (n6y - cy) ** 2 + (n6z - cz) ** 2 < r ** 2
+                index7 = (n7x - cx) ** 2 + (n7y - cy) ** 2 + (n7z - cz) ** 2 < r ** 2
+                index8 = (n8x - cx) ** 2 + (n8y - cy) ** 2 + (n8z - cz) ** 2 < r ** 2
                 index_inner = index1 & index2 & index3 & index4 & index5 & index6 & index7 & index8
                 element_sets[index_inner] = int(i) + 1
                 index_inter = (index1 | index2 | index3 | index4 | index5 | index6 | index7 | index8) ^ index_inner
                 element_sets[index_inter] = -1
-                
+
     element_sets_names = np.unique(element_sets)
 
     element_sets_dict = {}
     for name in element_sets_names:
         element_sets_dict[int(name)] = []
         element_sets_dict['MATRIX'] = []
         element_sets_dict['PARTICLES'] = []
         element_sets_dict['INTERFACES'] = []
         element_sets_dict['ALL'] = []
     for i, _ in enumerate(element_sets):
-        element_sets_dict[int(element_sets[i])].append(element_index[i]+1)
+        element_sets_dict[int(element_sets[i])].append(element_index[i] + 1)
         if int(element_sets[i]) == 0:
-            element_sets_dict['MATRIX'].append(element_index[i]+1)
+            element_sets_dict['MATRIX'].append(element_index[i] + 1)
         elif int(element_sets[i]) == -1:
-            element_sets_dict['INTERFACES'].append(element_index[i]+1)
+            element_sets_dict['INTERFACES'].append(element_index[i] + 1)
         else:
-            element_sets_dict['PARTICLES'].append(element_index[i]+1)
-        element_sets_dict['ALL'].append(element_index[i]+1)
-        
+            element_sets_dict['PARTICLES'].append(element_index[i] + 1)
+        element_sets_dict['ALL'].append(element_index[i] + 1)
+
     write_input_file(dim, nodes, elements, element_type, element_sets_dict, output_path)
 
     status['message']['element_sets_names'] = element_sets_names.tolist()
     status['message']['nodes_number'] = len(node_index)
     status['message']['elements_number'] = len(element_index)
 
 
 def create_mesh(gap, size, dimension, node_shape, element_type, model_path, output_path, status):
-
     args = gap, size, dimension, node_shape, element_type, model_path, output_path, status
 
     status['message'] = {}
 
     mesh(gap, dimension, node_shape, element_type, model_path, output_path, status)
 
     filename = os.path.join(output_path, 'model.msg')
@@ -575,15 +574,15 @@
     status['message']['dimension'] = dimension
     status['message']['size'] = size
     status['message']['gap'] = gap
     status['message']['element_type'] = element_type
     status['message']['gap'] = gap
     with open(filename, 'w', encoding='utf-8') as f:
         json.dump(status['message'], f, ensure_ascii=False)
-        
+
     filename = os.path.join(output_path, 'args.json')
     with open(filename, 'w', encoding='utf-8') as f:
         json.dump(args[:-1], f, ensure_ascii=False)
 
     return 0
```

### Comparing `psic-0.0.8.9/src/psic/create_submodel.py` & `psic-0.0.9/src/psic/create_submodel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 """
 生成规则网格
 """
-
 import json
 import os
 
 import numpy as np
 
 from psic.calc_fraction import calc_area_fraction, calc_volume_fraction
 from psic.plot_model import plot_circle, plot_distribution, plot_sphere
@@ -39,15 +38,15 @@
     lower = (centers + radiuses) > np.array(subsize).T[0]
     upper = (centers - radiuses) < np.array(subsize).T[1]
 
     # 在子区域内部的布尔型矩阵
     is_in_cube_matrix = np.concatenate((lower, upper), axis=1)
 
     # 在子区域内部的布尔型列表
-    is_in_cube = np.sum(is_in_cube_matrix, axis=1) >= 2*len(subsize)
+    is_in_cube = np.sum(is_in_cube_matrix, axis=1) >= 2 * len(subsize)
 
     sub_centers = centers[is_in_cube]
     sub_radiuses = radiuses[is_in_cube]
 
     return sub_centers, sub_radiuses
 
 
@@ -88,61 +87,61 @@
 
     """
 
     status['status'] = 'Running'
     args = model_file, model_id, size, ndiv, gap, out_path, status
 
     circles = np.load(model_file)
-    dim = circles.shape[-1]-1
+    dim = circles.shape[-1] - 1
     centers = circles[:, 0:dim]
-    radiuses = circles[:, dim:dim+1]
+    radiuses = circles[:, dim:dim + 1]
     size = np.array(size)
-    subsize = size/ndiv
-    a = [np.arange(s[0], s[1], s[1]/ndiv) for s in size]
+    subsize = size / ndiv
+    a = [np.arange(s[0], s[1], s[1] / ndiv) for s in size]
     b = np.meshgrid(*a)
     c = np.array([bb.flatten() for bb in b])
 
     for i in range(c.shape[1]):
 
-        status['progress'] = int(i/c.shape[1]*100)
+        status['progress'] = int(i / c.shape[1] * 100)
 
-        submodel_id = i+1
+        submodel_id = i + 1
         shift_centers = centers - c[:, i]
         sub_centers, sub_radiuses = get_submodel(shift_centers, radiuses, subsize)
         data = np.concatenate((sub_centers, sub_radiuses), axis=1)
 
         submodel_path = os.path.join(out_path, str(submodel_id))
 
         if not os.path.isdir(submodel_path):
             os.makedirs(submodel_path)
 
         filename = os.path.join(submodel_path, 'model.npy')
         np.save(filename, data)
 
         filename = os.path.join(submodel_path, 'model.png')
         if len(size) == 2:
-            plot_circle(sub_centers, sub_radiuses-gap, subsize, filename, 150)
+            plot_circle(sub_centers, sub_radiuses - gap, subsize, filename, 150)
         if len(size) >= 3:
-            plot_sphere(sub_centers, sub_radiuses-gap, subsize, filename, (500, 500))
+            plot_sphere(sub_centers, sub_radiuses - gap, subsize, filename, (500, 500))
 
         filename = os.path.join(submodel_path, 'density.png')
-        plot_distribution(sub_radiuses-gap, filename, 150)
+        plot_distribution(sub_radiuses - gap, filename, 150)
 
         filename = os.path.join(submodel_path, 'model.msg')
         message = {}
         if len(size) == 2:
-            fraction = calc_area_fraction(sub_centers, sub_radiuses-gap, subsize)
+            fraction = calc_area_fraction(sub_centers, sub_radiuses - gap, subsize)
         if len(size) >= 3:
-            fraction = calc_volume_fraction(sub_centers, sub_radiuses-gap, subsize)
+            fraction = calc_volume_fraction(sub_centers, sub_radiuses - gap, subsize)
         message['model_id'] = model_id
         message['submodel_id'] = submodel_id
         message['fraction'] = fraction
         message['num_ball'] = len(sub_radiuses)
         message['subsize'] = subsize.tolist()
-        message['location'] = (subsize+c[:, i].reshape(-1, 1)).tolist()
+        message['location'] = (subsize + c[:, i].reshape(-1, 1)).tolist()
         message['size'] = size.tolist()
         message['gap'] = gap
         message['ndiv'] = ndiv
         with open(filename, 'w', encoding='utf-8') as f:
             json.dump(message, f, ensure_ascii=False)
 
         filename = os.path.join(submodel_path, 'args.json')
```

### Comparing `psic-0.0.8.9/src/psic/packing_spheres_in_cube.py` & `psic-0.0.9/src/psic/packing_spheres_in_cube.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 2D：矩形区域填充圆形
 3D：六面体区域填充球体
 >4D: 超立方体区域填充超球
 """
-
 import json
 import os
 
 import numpy as np
 from scipy.spatial.distance import cdist
 
 from psic.calc_fraction import calc_area_fraction, calc_volume_fraction
@@ -40,34 +39,34 @@
         两圆/球体碰撞时间位于区间[0, dt]内
 
     Returns
     -------
     tc : float
         两圆/球体发生碰撞的时间
     """
-    a = np.sum((velocity_2-velocity_1)**2)
-    b = 2*np.sum((velocity_2-velocity_1)*(center_2-center_1))
-    c = np.sum((center_2-center_1)**2)-(r_1[0]+r_2[0])**2
-    delta = np.sqrt(b**2-4*a*c)
-    t1 = (-b-delta)/(2*a)
-    t2 = (-b+delta)/(2*a)
+    a = np.sum((velocity_2 - velocity_1) ** 2)
+    b = 2 * np.sum((velocity_2 - velocity_1) * (center_2 - center_1))
+    c = np.sum((center_2 - center_1) ** 2) - (r_1[0] + r_2[0]) ** 2
+    delta = np.sqrt(b ** 2 - 4 * a * c)
+    t1 = (-b - delta) / (2 * a)
+    t2 = (-b + delta) / (2 * a)
     tc = min(t1, t2, dt)
 
     return tc
 
 
 def update_crash_velocity(center_1, center_2):
     """
     更新两圆/球碰撞后各自的速度矢量
     两球碰撞后的速度为沿着两球心连线方向互相远离对方的单位矢量
     """
-    v1 = center_2-center_1
-    v2 = center_1-center_2
-    v1 = v1/np.linalg.norm(v1)
-    v2 = v2/np.linalg.norm(v2)
+    v1 = center_2 - center_1
+    v2 = center_1 - center_2
+    v1 = v1 / np.linalg.norm(v1)
+    v2 = v2 / np.linalg.norm(v2)
     return v1, v2
 
 
 def dist_square(X=np.empty(0), Y=np.empty(0)):
     """
     求点集合X到Y中任意两点之间的距离平方
 
@@ -81,17 +80,17 @@
     Returns
     -------
     dist_square : array
         返回n*m的矩阵，i行j列代表X[i]和Y[j]之间的距离的平方
 
     """
     if Y.size == 0:
-        dist_square = cdist(X, X)**2
+        dist_square = cdist(X, X) ** 2
     else:
-        dist_square = cdist(X, Y)**2
+        dist_square = cdist(X, Y) ** 2
     return dist_square
 
 
 def r_square(X=np.empty(0), Y=np.empty(0)):
     """
     求两个半径集合和的平方
 
@@ -105,17 +104,17 @@
     Returns
     -------
     r_square : array
         返回n*m的矩阵，i行j列代表半径X[i]和Y[j]和的平方
 
     """
     if Y.size == 0:
-        r_square = (X+X.T)**2
+        r_square = (X + X.T) ** 2
     else:
-        r_square = (X+Y.T)**2
+        r_square = (X + Y.T) ** 2
     return r_square
 
 
 def is_crash_index(C0=np.empty(0), R0=np.empty(0), C1=np.empty(0), R1=np.empty(0)):
     """
     判断圆/球集合C0和C1是否存在重叠的元素，得到发生重叠的圆/球在C1中的索引
 
@@ -192,15 +191,15 @@
     Returns
     -------
     建立的圆心坐标数组，ncircle*维度
 
     """
     centers = np.random.rand(ncircle, len(size))
     for i, _ in enumerate(size):
-        centers[:, i] = centers[:, i]*(size[i][1]-size[i][0])+size[i][0]
+        centers[:, i] = centers[:, i] * (size[i][1] - size[i][0]) + size[i][0]
     return centers.astype('float32')
 
 
 def create_velocities(ncircle, size):
     """
     建立ncircle个随机分布的速度矢量数组
 
@@ -210,15 +209,15 @@
         建立的速度矢量数量
 
     Returns
     -------
     建立的速度矢量数组，ncircle*维度
 
     """
-    velocities = np.random.rand(ncircle, len(size))*2-1.0
+    velocities = np.random.rand(ncircle, len(size)) * 2 - 1.0
     return velocities.astype('float32')
 
 
 def create_radiuses(ncircle, radius_sets):
     """
     建立ncircle个符合radiuse_sets分布的半径数组
 
@@ -317,15 +316,15 @@
         velocities_new = np.delete(velocities_new, is_crash, 0)
         radiuses_new = np.delete(radiuses_new, is_crash, 0)
 
         centers_1 = np.concatenate((centers_0, centers_new), axis=0)
         velocities_1 = np.concatenate((velocities_0, velocities_new), axis=0)
         radiuses_1 = np.concatenate((radiuses_0, radiuses_new), axis=0)
 
-        n = len(radiuses_1)-1
+        n = len(radiuses_1) - 1
 
         centers_2 = centers_1
         velocities_2 = velocities_1
         radiuses_2 = radiuses_1
 
         dt = dt0
 
@@ -360,38 +359,39 @@
                     velocities_2[is_crash[1]] = v1
                     break
                 else:
                     dt *= 0.5
 
         if count >= max_iter:
             print('The number of iterations is out of range.')
-        
+
         try:
-            if i % int(num_add/10) == 0:
+            if i % int(num_add / 10) == 0:
                 if len(size) == 2:
-                    fraction = calc_area_fraction(centers_1, radiuses_1-gap, size)
+                    fraction = calc_area_fraction(centers_1, radiuses_1 - gap, size)
                     print(i, n, fraction)
                     status['log'] += '%s, %s, %s\n' % (i, n, fraction)
 
                 if len(size) == 3:
-                    fraction = calc_volume_fraction(centers_1, radiuses_1-gap, size)
+                    fraction = calc_volume_fraction(centers_1, radiuses_1 - gap, size)
                     status['log'] += '%s, %s, %s\n' % (i, n, fraction)
 
         except ZeroDivisionError:
             print(ZeroDivisionError)
 
-        if len(radius_sets_0) <= n+ncircle+1:
+        if len(radius_sets_0) <= n + ncircle + 1:
             break
-        
-        status['progress'] = int(i/num_add*100)
+
+        status['progress'] = int(i / num_add * 100)
 
     return centers_1, radiuses_1
 
 
-def create_model(ncircle, size, gap, num_add, max_iter, dt0, dt_interval, rayleigh_para, num_ball, rad_min, rad_max, model_path, status):
+def create_model(ncircle, size, gap, num_add, max_iter, dt0, dt_interval, rayleigh_para, num_ball, rad_min, rad_max,
+                 model_path, status):
     """
     根据参数列表生成填充模型
     
     create_model(ncircle, size, gap, num_add, max_iter, dt0, dt_interval, rayleigh_para, num_ball, rad_min, rad_max, model_path, status)
     
     Parameters
     ----------
@@ -434,75 +434,76 @@
     生成分布图片：density.png
     
     Returns
     -------
     0
 
     """
-    
+
     args = ncircle, size, gap, num_add, max_iter, dt0, dt_interval, rayleigh_para, num_ball, rad_min, rad_max, model_path, status
 
     # 生成需要填充的半径集合
     radius_sets = rayleigh_set(rayleigh_para, num_ball)
     radius_sets = radius_sets.astype('float32')
     radius_sets = abs(np.sort(-radius_sets))
     radius_sets = radius_sets[radius_sets > rad_min]
     radius_sets = radius_sets[radius_sets < rad_max]
 
     # 转换为半径，毫米
-    radius_sets *= 0.001/2.0
+    radius_sets *= 0.001 / 2.0
 
     status['status'] = 'Running'
 
-    centers, radiuses = packing_spheres_in_cube(ncircle, radius_sets, size, gap, num_add, max_iter, dt0, dt_interval, status)
+    centers, radiuses = packing_spheres_in_cube(ncircle, radius_sets, size, gap, num_add, max_iter, dt0, dt_interval,
+                                                status)
 
     data = np.concatenate((centers, radiuses), axis=1)
 
     filename = os.path.join(model_path, 'model.npy')
     status['log'] += 'Save %s\n' % filename
     np.save(filename, data)
-    
+
     filename = os.path.join(model_path, 'model.png')
     if len(size) == 2:
-        plot_circle(centers, radiuses-gap, size, filename, 150)
+        plot_circle(centers, radiuses - gap, size, filename, 150)
     if len(size) >= 3:
-        plot_sphere(centers, radiuses-gap, size, filename, (500, 500))
+        plot_sphere(centers, radiuses - gap, size, filename, (500, 500))
     status['log'] += 'Save %s\n' % filename
-    
+
     filename = os.path.join(model_path, 'density.png')
-    plot_distribution(radiuses-gap, filename, 150)
+    plot_distribution(radiuses - gap, filename, 150)
     status['log'] += 'Save %s\n' % filename
 
     status['progress'] = 100
     status['status'] = 'Done'
-    
+
     filename = os.path.join(model_path, 'model.msg')
     message = {}
     if len(size) == 2:
-        fraction = calc_area_fraction(centers, radiuses-gap, size)
+        fraction = calc_area_fraction(centers, radiuses - gap, size)
     if len(size) >= 3:
-        fraction = calc_volume_fraction(centers, radiuses-gap, size)
+        fraction = calc_volume_fraction(centers, radiuses - gap, size)
     message['fraction'] = fraction
     message['num_ball'] = len(radiuses)
     message['size'] = size
     message['gap'] = gap
     with open(filename, 'w', encoding='utf-8') as f:
         json.dump(message, f, ensure_ascii=False)
     status['log'] += 'Save %s\n' % filename
-    
+
     filename = os.path.join(model_path, 'args.json')
     status['log'] += 'Save %s\n' % filename
     with open(filename, 'w', encoding='utf-8') as f:
         json.dump(args[:-1], f, ensure_ascii=False)
 
     filename = os.path.join(model_path, 'model.log')
     status['log'] += 'Save %s\n' % filename
     with open(filename, 'w', encoding='utf-8') as f:
         f.write(status['log'])
-        
+
     return 0
 
 
 if __name__ == "__main__":
     ncircle = 2
     size = [[0, 0.1], [0, 0.1]]
     # size = [[0, 1], [0, 1], [0, 1]]
@@ -514,11 +515,13 @@
     rayleigh_para = 20
     num_ball = 1200
     rad_min = 10
     rad_max = 100
     model_path = ''
     thread_id = 1
     status = {'status': 'Submit', 'log': '', 'progress': 0}
-    args = (ncircle, size, gap, num_add, max_iter, dt0, dt_interval, rayleigh_para, num_ball, rad_min, rad_max, model_path, status)
+    args = (
+    ncircle, size, gap, num_add, max_iter, dt0, dt_interval, rayleigh_para, num_ball, rad_min, rad_max, model_path,
+    status)
     print(status)
     create_model(*args)
     print(status)
```

### Comparing `psic-0.0.8.9/src/psic/plot_model.py` & `psic-0.0.9/src/psic/plot_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-
 import matplotlib
 
 matplotlib.use('Agg')
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.patches import Circle
-# from mayavi import mlab
+from mayavi import mlab
 
 
 def plot_circle(centers, radiuses, size, filename, dpi=150):
-    fig, ax = plt.subplots(1, 1, figsize=(6,6))
+    fig, ax = plt.subplots(1, 1, figsize=(6, 6))
     for i, _ in enumerate(centers):
         C = Circle(centers[i], radius=radiuses[i], facecolor=(1, 1, 1, 1), edgecolor=(0, 0, 0, 1), linewidth=None)
         ax.add_patch(C)
     ax.axis('equal')
     ax.set_box_aspect(1)
     ax.set_xlim(size[0])
     ax.set_ylim(size[1])
@@ -25,34 +24,33 @@
     ax.set_ylabel('y, mm')
     fig.savefig(filename, dpi=dpi, transparent=False)
     plt.close(fig)
 
 
 def plot_sphere(centers, radiuses, size, filename, dpi=(500, 500)):
     x, y, z, r = centers[:, 0], centers[:, 1], centers[:, 2], radiuses[:, 0]
-    # mlab.options.offscreen = True
-    # fig = mlab.figure(size=(500,500), bgcolor=(1,1,1))
-    # mlab.points3d(x, y, z, r*2, scale_factor=1, resolution=30, mode="sphere")
-    # mlab.outline(fig)
-    # mlab.view(distance=4)
-    # mlab.savefig(filename, figure=fig, size=dpi)
-    # mlab.close(all=True)
+    mlab.options.offscreen = True
+    fig = mlab.figure(size=(500, 500), bgcolor=(1, 1, 1))
+    mlab.points3d(x, y, z, r * 2, scale_factor=1, resolution=30, mode="sphere")
+    mlab.outline(fig)
+    mlab.view(distance=4)
+    mlab.savefig(filename, figure=fig, size=dpi)
+    mlab.close(all=True)
 
 
 def plot_distribution(radiuses, filename, dpi=150):
-    fig, ax = plt.subplots(1, 1, figsize=(6,6))
-    plt.hist(radiuses*1000, bins=10, density=True)
+    fig, ax = plt.subplots(1, 1, figsize=(6, 6))
+    plt.hist(radiuses * 1000, bins=10, density=True)
     ax.set_xlabel('Radius, $\\mu$m')
     ax.set_ylabel('Density')
     fig.savefig(filename, dpi=dpi, transparent=False)
     plt.close(fig)
 
 
 if __name__ == "__main__":
     circles = np.load('model.npy')
-    dim = circles.shape[-1]-1
+    dim = circles.shape[-1] - 1
     centers = circles[:, 0:dim]
-    radiuses = circles[:, dim:dim+1]
-    plot_circle(centers, radiuses, [[0,1], [0,1]], 'model.png', 300)
+    radiuses = circles[:, dim:dim + 1]
+    plot_circle(centers, radiuses, [[0, 1], [0, 1]], 'model.png', 300)
     # plot_sphere(centers, radiuses, [[0, 1], [0, 1], [0, 1]], 'model.png', (400,400))
     # plot_distribution(radiuses, 'density.png', 300)
-
```

### Comparing `psic-0.0.8.9/src/psic.egg-info/PKG-INFO` & `psic-0.0.9/src/psic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psic
-Version: 0.0.8.9
+Version: 0.0.9
 Summary: Packing spheres in cube
 Home-page: https://github.com/sunwhale/psic
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/psic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

