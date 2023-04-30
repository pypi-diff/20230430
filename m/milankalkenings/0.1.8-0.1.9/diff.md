# Comparing `tmp/milankalkenings-0.1.8.tar.gz` & `tmp/milankalkenings-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milankalkenings-0.1.8.tar", last modified: Tue Feb  7 21:57:04 2023, max compression
+gzip compressed data, was "milankalkenings-0.1.9.tar", last modified: Tue Feb  7 22:30:33 2023, max compression
```

## Comparing `milankalkenings-0.1.8.tar` & `milankalkenings-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-07 21:57:04.813578 milankalkenings-0.1.8/
--rw-rw-rw-   0        0        0     1086 2023-01-17 06:50:47.000000 milankalkenings-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      485 2023-02-07 21:57:04.814671 milankalkenings-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      110 2023-02-06 09:23:32.000000 milankalkenings-0.1.8/README.md
--rw-rw-rw-   0        0        0      102 2023-01-17 08:51:36.000000 milankalkenings-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0      555 2023-02-07 21:57:04.815674 milankalkenings-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-07 21:57:04.781498 milankalkenings-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-02-07 21:57:04.791612 milankalkenings-0.1.8/src/milankalkenings/
--rw-rw-rw-   0        0        0        0 2023-01-17 07:41:27.000000 milankalkenings-0.1.8/src/milankalkenings/__init__.py
--rw-rw-rw-   0        0        0    16162 2023-02-07 21:54:44.000000 milankalkenings-0.1.8/src/milankalkenings/deep_learning.py
-drwxrwxrwx   0        0        0        0 2023-02-07 21:57:04.813578 milankalkenings-0.1.8/src/milankalkenings.egg-info/
--rw-rw-rw-   0        0        0      485 2023-02-07 21:57:04.000000 milankalkenings-0.1.8/src/milankalkenings.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-02-07 21:57:04.000000 milankalkenings-0.1.8/src/milankalkenings.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-07 21:57:04.000000 milankalkenings-0.1.8/src/milankalkenings.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-02-07 21:57:04.000000 milankalkenings-0.1.8/src/milankalkenings.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-02-07 22:30:33.530463 milankalkenings-0.1.9/
+-rw-rw-rw-   0        0        0     1086 2023-01-17 06:50:47.000000 milankalkenings-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      485 2023-02-07 22:30:33.530463 milankalkenings-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      110 2023-02-06 09:23:32.000000 milankalkenings-0.1.9/README.md
+-rw-rw-rw-   0        0        0      102 2023-01-17 08:51:36.000000 milankalkenings-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      555 2023-02-07 22:30:33.537650 milankalkenings-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-02-07 22:30:33.504896 milankalkenings-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-02-07 22:30:33.513477 milankalkenings-0.1.9/src/milankalkenings/
+-rw-rw-rw-   0        0        0        0 2023-01-17 07:41:27.000000 milankalkenings-0.1.9/src/milankalkenings/__init__.py
+-rw-rw-rw-   0        0        0    16424 2023-02-07 22:29:48.000000 milankalkenings-0.1.9/src/milankalkenings/deep_learning.py
+drwxrwxrwx   0        0        0        0 2023-02-07 22:30:33.529462 milankalkenings-0.1.9/src/milankalkenings.egg-info/
+-rw-rw-rw-   0        0        0      485 2023-02-07 22:30:33.000000 milankalkenings-0.1.9/src/milankalkenings.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-02-07 22:30:33.000000 milankalkenings-0.1.9/src/milankalkenings.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-07 22:30:33.000000 milankalkenings-0.1.9/src/milankalkenings.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-02-07 22:30:33.000000 milankalkenings-0.1.9/src/milankalkenings.egg-info/top_level.txt
```

### Comparing `milankalkenings-0.1.8/LICENSE` & `milankalkenings-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `milankalkenings-0.1.8/src/milankalkenings/deep_learning.py` & `milankalkenings-0.1.9/src/milankalkenings/deep_learning.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,14 +356,17 @@
                 lr = lr * self.setup.lrrt_decay
         return best_lrs
 
     def train_overkill(self, max_epochs: int, freeze_pretrained: bool):
         losses_train = []
         losses_val = []
         best_lrs = []
+        module = torch.load(self.setup.checkpoint_running)
+        losses_train.append(self.loss_epoch_eval(module=module, loader_eval=self.setup.loader_train))
+        losses_val.append(self.loss_epoch_eval(module=module, loader_eval=self.setup.loader_val))
         for epoch in range(max_epochs):
             print("epoch", epoch + 1)
             best_lrs.append(self.train_overkill_one_epoch(freeze_pretrained=freeze_pretrained))
             module = torch.load(self.setup.checkpoint_running)
             losses_train.append(self.loss_epoch_eval(module=module, loader_eval=self.setup.loader_train))
             losses_val.append(self.loss_epoch_eval(module=module, loader_eval=self.setup.loader_val))
             print("train loss:", losses_train[-1])
```

