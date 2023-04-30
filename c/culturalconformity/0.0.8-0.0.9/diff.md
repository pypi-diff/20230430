# Comparing `tmp/culturalconformity-0.0.8.tar.gz` & `tmp/culturalconformity-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "culturalconformity-0.0.8.tar", last modified: Wed Apr 26 23:19:56 2023, max compression
+gzip compressed data, was "culturalconformity-0.0.9.tar", last modified: Fri Apr 28 00:06:37 2023, max compression
```

## Comparing `culturalconformity-0.0.8.tar` & `culturalconformity-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 23:19:56.777276 culturalconformity-0.0.8/
--rw-r--r--   0 kaledadenton   (501) staff       (20)      247 2023-04-26 23:19:56.777105 culturalconformity-0.0.8/PKG-INFO
-drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 23:19:56.776088 culturalconformity-0.0.8/culturalconformity/
--rw-r--r--   0 kaledadenton   (501) staff       (20)       80 2023-04-26 22:39:28.000000 culturalconformity-0.0.8/culturalconformity/__init__.py
--rw-r--r--   0 kaledadenton   (501) staff       (20)     3922 2023-04-26 22:38:29.000000 culturalconformity-0.0.8/culturalconformity/frq_over_time.py
--rw-r--r--   0 kaledadenton   (501) staff       (20)     6728 2023-04-26 23:19:36.000000 culturalconformity-0.0.8/culturalconformity/interactive.py
-drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 23:19:56.776889 culturalconformity-0.0.8/culturalconformity.egg-info/
--rw-r--r--   0 kaledadenton   (501) staff       (20)      247 2023-04-26 23:19:56.000000 culturalconformity-0.0.8/culturalconformity.egg-info/PKG-INFO
--rw-r--r--   0 kaledadenton   (501) staff       (20)      277 2023-04-26 23:19:56.000000 culturalconformity-0.0.8/culturalconformity.egg-info/SOURCES.txt
--rw-r--r--   0 kaledadenton   (501) staff       (20)        1 2023-04-26 23:19:56.000000 culturalconformity-0.0.8/culturalconformity.egg-info/dependency_links.txt
--rw-r--r--   0 kaledadenton   (501) staff       (20)       19 2023-04-26 23:19:56.000000 culturalconformity-0.0.8/culturalconformity.egg-info/top_level.txt
--rw-r--r--   0 kaledadenton   (501) staff       (20)       38 2023-04-26 23:19:56.777339 culturalconformity-0.0.8/setup.cfg
--rw-r--r--   0 kaledadenton   (501) staff       (20)      976 2023-04-26 23:19:49.000000 culturalconformity-0.0.8/setup.py
+drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-28 00:06:37.098923 culturalconformity-0.0.9/
+-rw-r--r--   0 kaledadenton   (501) staff       (20)      247 2023-04-28 00:06:37.098741 culturalconformity-0.0.9/PKG-INFO
+drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-28 00:06:37.097659 culturalconformity-0.0.9/culturalconformity/
+-rw-r--r--   0 kaledadenton   (501) staff       (20)      116 2023-04-28 00:05:02.000000 culturalconformity-0.0.9/culturalconformity/__init__.py
+-rw-r--r--   0 kaledadenton   (501) staff       (20)     3924 2023-04-26 23:22:57.000000 culturalconformity-0.0.9/culturalconformity/frq_over_time.py
+-rw-r--r--   0 kaledadenton   (501) staff       (20)     6743 2023-04-27 03:04:49.000000 culturalconformity-0.0.9/culturalconformity/interactive.py
+-rw-r--r--   0 kaledadenton   (501) staff       (20)       73 2023-04-28 00:05:05.000000 culturalconformity-0.0.9/culturalconformity/stochastic.py
+drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-28 00:06:37.098533 culturalconformity-0.0.9/culturalconformity.egg-info/
+-rw-r--r--   0 kaledadenton   (501) staff       (20)      247 2023-04-28 00:06:37.000000 culturalconformity-0.0.9/culturalconformity.egg-info/PKG-INFO
+-rw-r--r--   0 kaledadenton   (501) staff       (20)      351 2023-04-28 00:06:37.000000 culturalconformity-0.0.9/culturalconformity.egg-info/SOURCES.txt
+-rw-r--r--   0 kaledadenton   (501) staff       (20)        1 2023-04-28 00:06:37.000000 culturalconformity-0.0.9/culturalconformity.egg-info/dependency_links.txt
+-rw-r--r--   0 kaledadenton   (501) staff       (20)        6 2023-04-28 00:06:37.000000 culturalconformity-0.0.9/culturalconformity.egg-info/requires.txt
+-rw-r--r--   0 kaledadenton   (501) staff       (20)       19 2023-04-28 00:06:37.000000 culturalconformity-0.0.9/culturalconformity.egg-info/top_level.txt
+-rw-r--r--   0 kaledadenton   (501) staff       (20)       38 2023-04-28 00:06:37.098984 culturalconformity-0.0.9/setup.cfg
+-rw-r--r--   0 kaledadenton   (501) staff       (20)      983 2023-04-28 00:06:34.000000 culturalconformity-0.0.9/setup.py
```

### Comparing `culturalconformity-0.0.8/culturalconformity/frq_over_time.py` & `culturalconformity-0.0.9/culturalconformity/frq_over_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,8 +108,9 @@
         all_p_over_time[j] = [p[j]]
 
     for i in range(generations):
         p = p_next_gen(p, n, **coeff_dict)
         for j in range(m):
             all_p_over_time[j].append(p[j])
 
-    return all_p_over_time
+    return all_p_over_time
+
```

### Comparing `culturalconformity-0.0.8/culturalconformity/interactive.py` & `culturalconformity-0.0.9/culturalconformity/interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,33 +46,32 @@
 
 def choose_d(d_min, d_max, denom_high, denom_low, x_vec, n):
     pr = 9  # Precision for rounding
     # Redo this because need it again
     x_subset = [j for j in x_vec if j != 0]
     x_avg = n / len(x_subset)
 
-    msg = "For x = " + str(x_vec) + ", choose d(x) \nbetween " + str(d_min) + " and " + str(d_max) + ". \n(For help, enter '?')"
-
+    msg = "For the state x = " + str(x_vec) + ", choose a d(x) \nvalue that lies between " + str(d_min) + " and " + str(d_max) + ". \n(For help, enter '?')"
     d = input(msg)
     if d == '?':
         # Find g_i(x)*d(x) for each element
         g_values = []
         for l in range(len(x_vec)):
             x_l = x_vec[l]
             if (round(x_l, pr) == 0) or (round(x_l, pr) == n) or (round(x_l, pr) == round(x_avg, pr)):
                 g_values.append(0)
             elif x_l > x_avg:
                 g_values.append(x_l / denom_high)
             elif x_l < x_avg:
                 g_values.append(- (1 / x_l) * (1 / denom_low))
 
         g_msg = ("For a given xi in x = " + str(x_vec) + ", the value of d(x) that you choose \n"
-                 + "will be divided by the number of role models, " + str(n) + ", and multiplied \n"
-                 + "by gi where g = " + str(g_values) + ". Remember that this d(x) must be \n"
-                 + "between " + str(d_min) + " and " + str(d_max) + ". Please enter your choice: ")
+                 + "will be divided by the number of role models, " + str(n) + ", and multiplied by gi\n"
+                 + "where g = " + str(g_values) + ". Remember that this d(x) must be between\n"
+                 + str(d_min) + " and " + str(d_max) + ". Please enter your choice: ")
         d = input(g_msg)
 
     d = float(d)
     while d > d_max or d < d_min:
         d = input("This d(x) is invalid or out of bounds; try again.")
         d = choose_d(d_min, d_max, denom_high, denom_low, x_vec, n)
 
@@ -142,20 +141,20 @@
     p_vec.append(last_pi)
 
     return p_vec
 
 def interactive():
     intro = input("Press ? for a detailed description of this function or any key to continue.")
     if intro == '?':
-        print("This function will allow you to specify conformity coefficients, initial variant frequencies, \n"
-              + "and more, but only one option at a time. Make sure to store your results in a variable, e.g., \n"
-              + "do not write interactive() all by itself but rather, say, x = interactive() so that \n"
-              + "your results will go into the variable called x. They will be in the appropriate format \n"
-              + "for input into future functions. See github.com/kaleda/culturalconformity for how to use \n"
-              + "the output of the interactive() function in the other functions. Let's get started!")
+        print("This function will allow you to specify conformity coefficients, initial variant frequencies,\n"
+              + "and more, but only one option at a time. Make sure to store your results in a variable, e.g.,\n"
+              + "do not write interactive() all by itself but rather, say, x = interactive() so that your\n"
+              + "results will go into the variable called x. They will be in the appropriate format for input\n"
+              + "into future functions. See github.com/kaleda/culturalconformity for how to use the output\n"
+              + "of the interactive() function in the other functions. Let's get started!")
 
     msg = "Enter 1 to make your dictionary of conformity coefficients. \nEnter 2 to make your list of initial frequencies. \nEnter 9 to quit. "
     answer = float(input("What would you like to do? \n" + msg))
     while not answer.is_integer() or answer < 1 or answer > 9:
         answer = float(input("Sorry, that was not a valid number. \n" + msg))
 
     if answer == 1 or answer == 2:
```

### Comparing `culturalconformity-0.0.8/setup.py` & `culturalconformity-0.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Simulations of conformity, anti-conformity, and unbiased frequency-dependent transmission'
 # LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 # Setting up
 setup(
     name="culturalconformity",
     version=VERSION,
     author="Kaleda Denton",
     # author_email="kdenton@ucla.edu",
     description=DESCRIPTION,
     # long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=[],  # add any additional packages that
+    install_requires=['numpy'],  # add any additional packages that
     # needs to be installed along with your package. Eg: 'caer'
 
     # keywords=['python', 'first package'],
     # classifiers=[
     #    "Development Status :: 3 - Alpha",
     #    "Intended Audience :: Education",
     #    "Programming Language :: Python :: 2",
```

