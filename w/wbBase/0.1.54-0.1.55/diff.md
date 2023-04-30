# Comparing `tmp/wbBase-0.1.54.tar.gz` & `tmp/wbBase-0.1.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbBase-0.1.54.tar", last modified: Sat Apr 22 15:07:46 2023, max compression
+gzip compressed data, was "wbBase-0.1.55.tar", last modified: Sun Apr 30 08:43:35 2023, max compression
```

## Comparing `wbBase-0.1.54.tar` & `wbBase-0.1.55.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 15:07:46.038702 wbBase-0.1.54/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-22 15:07:44.000000 wbBase-0.1.54/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 15:07:46.026703 wbBase-0.1.54/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 15:07:46.032702 wbBase-0.1.54/Lib/wbBase/
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23965 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/application.py
--rw-rw-rw-   0 root         (0) root         (0)     2165 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/applicationInfo.py
--rw-rw-rw-   0 root         (0) root         (0)    20585 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/applicationWindow.py
--rw-rw-rw-   0 root         (0) root         (0)   309800 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/artprovider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 15:07:46.035702 wbBase-0.1.54/Lib/wbBase/control/
--rw-rw-rw-   0 root         (0) root         (0)     1118 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/control/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4414 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/control/externalToolConfig.py
--rw-rw-rw-   0 root         (0) root         (0)     5891 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/control/externalToolConfigUI.py
--rw-rw-rw-   0 root         (0) root         (0)     2666 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/control/filling.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/control/iePanel.py
--rw-rw-rw-   0 root         (0) root         (0)     8569 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/control/propgrid.py
--rw-rw-rw-   0 root         (0) root         (0)    47198 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/control/textEditControl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 15:07:46.036702 wbBase-0.1.54/Lib/wbBase/dialog/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/dialog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2342 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/dialog/multiSaveModifiedDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3293 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)    20381 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/dialog/preferences.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 15:07:46.038702 wbBase-0.1.54/Lib/wbBase/document/
--rw-rw-rw-   0 root         (0) root         (0)    23492 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/document/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    36999 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/document/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4743 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/document/notebook.py
--rw-rw-rw-   0 root         (0) root         (0)     8016 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/document/template.py
--rw-rw-rw-   0 root         (0) root         (0)     9208 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/document/view.py
--rw-rw-rw-   0 root         (0) root         (0)    21455 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/panelManager.py
--rw-rw-rw-   0 root         (0) root         (0)     2782 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/pluginManager.py
--rw-rw-rw-   0 root         (0) root         (0)     2942 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/pluginManager_old.py
--rw-rw-rw-   0 root         (0) root         (0)     8136 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/scripting.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 15:07:46.033702 wbBase-0.1.54/Lib/wbBase.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2708 2023-04-22 15:07:46.000000 wbBase-0.1.54/Lib/wbBase.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1027 2023-04-22 15:07:46.000000 wbBase-0.1.54/Lib/wbBase.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 15:07:46.000000 wbBase-0.1.54/Lib/wbBase.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-22 15:07:46.000000 wbBase-0.1.54/Lib/wbBase.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-22 15:07:46.000000 wbBase-0.1.54/Lib/wbBase.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2708 2023-04-22 15:07:46.038702 wbBase-0.1.54/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1347 2023-04-22 15:07:44.000000 wbBase-0.1.54/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2008 2023-04-22 15:07:46.039702 wbBase-0.1.54/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-22 15:07:44.000000 wbBase-0.1.54/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:43:35.465984 wbBase-0.1.55/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-30 08:43:33.000000 wbBase-0.1.55/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:43:35.452983 wbBase-0.1.55/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:43:35.458984 wbBase-0.1.55/Lib/wbBase/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23475 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/application.py
+-rw-rw-rw-   0 root         (0) root         (0)     2165 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/applicationInfo.py
+-rw-rw-rw-   0 root         (0) root         (0)    20585 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/applicationWindow.py
+-rw-rw-rw-   0 root         (0) root         (0)   309800 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/artprovider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:43:35.462984 wbBase-0.1.55/Lib/wbBase/control/
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/control/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4414 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/control/externalToolConfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     5891 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/control/externalToolConfigUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/control/filling.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/control/iePanel.py
+-rw-rw-rw-   0 root         (0) root         (0)     8569 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/control/propgrid.py
+-rw-rw-rw-   0 root         (0) root         (0)    47198 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/control/textEditControl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:43:35.463984 wbBase-0.1.55/Lib/wbBase/dialog/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/dialog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2342 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/dialog/multiSaveModifiedDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3293 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)    20381 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/dialog/preferences.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:43:35.465984 wbBase-0.1.55/Lib/wbBase/document/
+-rw-rw-rw-   0 root         (0) root         (0)    23492 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/document/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    36999 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/document/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4743 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/document/notebook.py
+-rw-rw-rw-   0 root         (0) root         (0)     8016 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/document/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     9208 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/document/view.py
+-rw-rw-rw-   0 root         (0) root         (0)    21455 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/panelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3366 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/pluginManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2942 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/pluginManager_old.py
+-rw-rw-rw-   0 root         (0) root         (0)     8814 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/scripting.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:43:35.460984 wbBase-0.1.55/Lib/wbBase.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-04-30 08:43:35.000000 wbBase-0.1.55/Lib/wbBase.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-04-30 08:43:35.000000 wbBase-0.1.55/Lib/wbBase.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 08:43:35.000000 wbBase-0.1.55/Lib/wbBase.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-04-30 08:43:35.000000 wbBase-0.1.55/Lib/wbBase.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-30 08:43:35.000000 wbBase-0.1.55/Lib/wbBase.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-04-30 08:43:35.465984 wbBase-0.1.55/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2023-04-30 08:43:33.000000 wbBase-0.1.55/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2008 2023-04-30 08:43:35.466984 wbBase-0.1.55/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-30 08:43:33.000000 wbBase-0.1.55/setup.py
```

### Comparing `wbBase-0.1.54/LICENSE` & `wbBase-0.1.55/LICENSE`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/application.py` & `wbBase-0.1.55/Lib/wbBase/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import mmap
 import os
 import pickle
 import sys
 import tempfile
 import time
 from argparse import ArgumentParser, Namespace
-from importlib import import_module, metadata, resources
+from importlib import metadata, resources
 from io import BytesIO
 from typing import TYPE_CHECKING, ClassVar, List, Optional, Union
 
 import wx
 from appdirs import AppDirs
 from wx.adv import (
     SPLASH_CENTER_ON_SCREEN,
@@ -22,14 +22,15 @@
 )
 
 from .applicationInfo import ApplicationInfo
 from .applicationWindow import ApplicationWindow
 from .artprovider import Artprovider
 from .document import DOC_SILENT
 from .pluginManager import PluginManager
+from .scripting import execfile, execsource
 
 try:
     from git import GitCommandError, InvalidGitRepositoryError
     from git.repo import Repo
 
     has_git = True
 except ImportError:
@@ -148,25 +149,25 @@
 
     _post_init_queue: List[FunctionType] = []
 
     def __init__(
         self,
         debug: int = 1,
         iconName: str = wx.ART_EXECUTABLE_FILE,
-        test:bool=False,
-        info:Optional[ApplicationInfo]= None
+        test: bool = False,
+        info: Optional[ApplicationInfo] = None,
     ):
         """
         Constructor
         """
         self._debug: int = debug
         self.iconName: str = iconName
         self._test = test
         self._splashScreen: Optional[AppSplashScreen] = None
-        self.info:ApplicationInfo = self._getAppInfo(info)
+        self.info: ApplicationInfo = self._getAppInfo(info)
         self.cmdLineArguments: Namespace = self._getCmdLineArguments()
         self._extChangeMode: int = self.EXT_CHANGE_TEST_ON_REQUEST
         self.extChangeTimerInterval: int = 60
         self.sharedDataDir: str = ""
         self.privateDataDir: str = ""
         self.globalObjects: List[str] = []
         self.dirs = AppDirs(self.info.AppName, self.info.VendorName)
@@ -175,15 +176,15 @@
     def __repr__(self) -> str:
         return '<Application: "%s" by %s>' % (self.AppName, self.VendorName)
 
     # =========================================================================
     # Private methods
     # =========================================================================
 
-    def _getAppInfo(self, info:Optional[ApplicationInfo]= None) -> ApplicationInfo:
+    def _getAppInfo(self, info: Optional[ApplicationInfo] = None) -> ApplicationInfo:
         if isinstance(info, ApplicationInfo):
             return info
         if not self.test:
             appInfoString = self.getResource("application.yml")
             if isinstance(appInfoString, str):
                 return ApplicationInfo.fromString(appInfoString)
         return ApplicationInfo()
@@ -235,22 +236,22 @@
         Handle command line arguments
         """
         arguments = self.cmdLineArguments
         config = self.config
         with wx.ConfigPathChanger(config, "/Application/Start/Script/"):
             # execute startup script
             if config.ReadBool("execute", False) and arguments.start_script_exec:
-                self.executeScript(config.Read("path", ""))
+                execfile(config.Read("path", ""))
             # open documents passed as command line arg
             for docPath in arguments.document:
                 if os.path.exists(docPath):
                     self.documentManager.CreateDocument(docPath, DOC_SILENT)
             # execute script passed as command line arg
             if arguments.scriptPath:
-                self.executeScript(arguments.scriptPath)
+                execfile(arguments.scriptPath)
 
     def _initExtChangesTest(self):
         """
         Setup external changes test
         """
         cfg = self.config
         with wx.ConfigPathChanger(cfg, "/Application/ExtChanges/"):
@@ -299,14 +300,26 @@
                     )
                     splashScreen.SetPosition(pos)
                     return splashScreen
         return AppSplashScreen(
             bmp, SPLASH_CENTER_ON_SCREEN | SPLASH_NO_TIMEOUT, 1000, None
         )
 
+    def _execFirstRunScript(self):
+        if self.test:
+            return
+        cfg = self.config
+        if cfg.ReadBool("/Application/firstRunDone", False):
+            return
+        scriptName = "firstRun.py"
+        firstRunCode = self.getResource(scriptName)
+        if firstRunCode:
+            execsource(firstRunCode, scriptName)
+        cfg.WriteBool("/Application/firstRunDone", True)
+
     # =========================================================================
     # Public methods
     # =========================================================================
 
     def OnPreInit(self) -> None:
         wx.App.OnPreInit(self)
         self.globalObjects = [
@@ -334,14 +347,15 @@
 
     def OnInit(self) -> bool:
         self.prepareSingleInstanceConfig()
         self._splashScreen = self._showSplashScreen()
         self._pluginManager: PluginManager = self.pluginManagerClass()
         self.prepareSharedDataFolder()
         self.preparePrivateDataFolder()
+        self._execFirstRunScript()
         self.SetTopWindow(self.topWindowClass(self.iconName))
         self.RunPostInitQueue()
         self._initExtChangesTest()
         return True
 
     def OnRun(self) -> int:
         """
@@ -381,15 +395,15 @@
         """
         if self._splashScreen:
             self._splashScreen.setMessage(text)
 
     @property
     def test(self) -> bool:
         """
-        Turns the application in test mode. This disables the splash screen 
+        Turns the application in test mode. This disables the splash screen
         and doesn't create directories, files or registry entries
 
         :return: Test mode enabled
         """
         return self._test
 
     @property
@@ -397,15 +411,15 @@
         """
         Mode how external changes of documents should be checked.
 
         May be one of:
             - EXT_CHANGE_TEST_ON_REQUEST
             - EXT_CHANGE_TEST_ON_ACTIVATE
             - EXT_CHANGE_TEST_ON_TIMER
-        
+
         :return: current mode
         """
         return self._extChangeMode
 
     @extChangeMode.setter
     def extChangeMode(self, value: int):
         assert value in (
@@ -445,15 +459,14 @@
         :return: The version string of the running application.
         """
         try:
             return metadata.version(self.__class__.__module__)
         except metadata.PackageNotFoundError:
             return "0.0.0"
 
-
     def getResource(self, name: str, type: str = "str") -> Optional[Union[str, bytes]]:
         if type not in ("str", "bytes"):
             raise ValueError(
                 f"Unknown resource type: '{type}', expected 'str' or 'bytes'"
             )
         module = self.__class__.__module__
         if module == "__main__":
@@ -523,23 +536,19 @@
                 sharedMemory = self._sharedMemory
                 while True:
                     sharedMemory.seek(0)
                     marker = sharedMemory.read_byte()
                     if marker == 0 or chr(marker) == "*":  # available buffer
                         sharedMemory.seek(0)
                         # set writing marker
-                        sharedMemory.write_byte(ord("-"))  
+                        sharedMemory.write_byte(ord("-"))
                         # write files we tried to open to shared memory
-                        sharedMemory.write(
-                            data
-                        )  
+                        sharedMemory.write(data)
                         sharedMemory.seek(0)
-                        sharedMemory.write_byte(
-                            ord("+")
-                        )  # set finished writing marker
+                        sharedMemory.write_byte(ord("+"))  # set finished writing marker
                         sharedMemory.flush()
                         break
                     else:
                         time.sleep(1)  # give enough time for buffer to be available
             sys.exit(0)
         else:
             self.listenAndLoadTimer.Start(250)
@@ -647,35 +656,14 @@
             except:
                 log.exception(
                     "Can't execute post init action '%s' from module '%s'",
                     action.__name__,
                     action.__module__,
                 )
 
-    def executeScript(self, scriptPath: str) -> None:
-        """
-        Execute a Python script located at scriptPath
-        in the name space of the running app.
-        """
-        if os.path.isfile(scriptPath):
-            del_name = False
-            # prepare environment
-            main = import_module("__main__")
-            global_vars = main.__dict__
-            if "__name__" not in global_vars:
-                global_vars["__name__"] = "__main__"
-                del_name = True
-            # execute the script
-            with open(scriptPath) as scriptFile:
-                code = compile(scriptFile.read(), scriptPath, "exec")
-                exec(code, global_vars)
-            # cleanup environment
-            if del_name and "__name__" in global_vars:
-                del global_vars["__name__"]
-
     # =========================================================================
     # Event Handler
     # =========================================================================
 
     def on_ACTIVATE_APP(self, event) -> None:
         if event.Active:
             self.documentManager.testForExternalChanges(testAll=True)
```

### Comparing `wbBase-0.1.54/Lib/wbBase/applicationInfo.py` & `wbBase-0.1.55/Lib/wbBase/applicationInfo.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/applicationWindow.py` & `wbBase-0.1.55/Lib/wbBase/applicationWindow.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/artprovider.py` & `wbBase-0.1.55/Lib/wbBase/artprovider.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/control/__init__.py` & `wbBase-0.1.55/Lib/wbBase/control/__init__.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/control/externalToolConfig.py` & `wbBase-0.1.55/Lib/wbBase/control/externalToolConfig.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/control/externalToolConfigUI.py` & `wbBase-0.1.55/Lib/wbBase/control/externalToolConfigUI.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/control/filling.py` & `wbBase-0.1.55/Lib/wbBase/control/filling.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/control/iePanel.py` & `wbBase-0.1.55/Lib/wbBase/control/iePanel.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/control/propgrid.py` & `wbBase-0.1.55/Lib/wbBase/control/propgrid.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/control/textEditControl.py` & `wbBase-0.1.55/Lib/wbBase/control/textEditControl.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/dialog/multiSaveModifiedDialog.py` & `wbBase-0.1.55/Lib/wbBase/dialog/multiSaveModifiedDialog.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py` & `wbBase-0.1.55/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/dialog/preferences.py` & `wbBase-0.1.55/Lib/wbBase/dialog/preferences.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/document/__init__.py` & `wbBase-0.1.55/Lib/wbBase/document/__init__.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/document/manager.py` & `wbBase-0.1.55/Lib/wbBase/document/manager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/document/notebook.py` & `wbBase-0.1.55/Lib/wbBase/document/notebook.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/document/template.py` & `wbBase-0.1.55/Lib/wbBase/document/template.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/document/view.py` & `wbBase-0.1.55/Lib/wbBase/document/view.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/panelManager.py` & `wbBase-0.1.55/Lib/wbBase/panelManager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/pluginManager.py` & `wbBase-0.1.55/Lib/wbBase/pluginManager.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,26 @@
                                 )
                                 self.app.globalObjects.append(globalObject)
                     self[name] = module
                 except ImportError:
                     log.exception(
                         "=============== Can't load plugin %s ===============", name
                     )
+                    if plugin.Installation == "required":
+                        if app._splashScreen:
+                            app._splashScreen.Destroy()
+                        wx.LogError(
+                            "Required plugin error\n\n"
+                            f"Can't load plugin '{name}'\n"
+                            "See terminal output for traceback."
+                            "Application will terminate."
+                        )
+                        sys.exit(1)
             elif plugin.Installation == "required":
+                if app._splashScreen:
+                    app._splashScreen.Destroy()
                 wx.LogError(
                     "Missing required plugin\n\n"
                     f"Can't load plugin '{name}'\n"
                     "Application will terminate."
                 )
                 sys.exit(1)
```

### Comparing `wbBase-0.1.54/Lib/wbBase/pluginManager_old.py` & `wbBase-0.1.55/Lib/wbBase/pluginManager_old.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase/scripting.py` & `wbBase-0.1.55/Lib/wbBase/scripting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,49 @@
 """
 This module implements the scriptability of Workbench application
 """
 from __future__ import annotations
 
 import os
+from importlib import import_module
 from typing import TYPE_CHECKING, Optional, List
 
 import wx
 
 from .document.manager import DOC_SILENT
 
 if TYPE_CHECKING:
     from .application import App
 
+def execsource(source, filename:str="<string>", global_vars=None, local_vars=None):
+    """
+    Execute python source code.
+    """
+    code = compile(source, filename, "exec")
+    if not global_vars:
+        main = import_module("__main__")
+        global_vars = main.__dict__
+    # prepare environment
+    del_name = False
+    if "__name__" not in global_vars:
+        global_vars["__name__"] = "__main__"
+        del_name = True
+    # execute the code
+    exec(code, global_vars, local_vars)
+    # cleanup environment
+    if del_name and "__name__" in global_vars:
+        del global_vars["__name__"]
+
 
 def execfile(filePath:str, global_vars=None, local_vars=None) -> None:
     """
     Execute a python script given by filePath
     """
-    with open(filePath) as f:
-        code = compile(f.read(), filePath, "exec")
-        exec(code, global_vars, local_vars)
+    with open(filePath, "r", encoding="utf-8") as sourcefile:
+        execsource(sourcefile.read(), filePath, global_vars, local_vars)
 
 
 def makeMacroTree(folder, tree):
     if os.path.isdir(folder):
         for name in os.listdir(folder):
             if not name.startswith("_") and not name.startswith("."):
                 fullPath = os.path.join(folder, name)
@@ -136,39 +155,42 @@
                 subMenu.addMacroTree(item, subMenu)
                 menuItem = menu.AppendSubMenu(subMenu, name)
                 menuItem.SetBitmap(bmpDir)
             elif os.path.isfile(item):
                 self.Append(MacroMenuItem(self, item, self.handler))
         return menu
 
+    def rebuild(self) -> None:
+        self._macroTree = None
+        self._clearMenu()
+        self._updateMenue()
+
+
     # =========================================================================
     # Event Handler
     # =========================================================================
 
     def on_macroRepeat(self, event):
-        self.app.executeScript(self._lastMacroPath)
+        execfile(self._lastMacroPath)
 
     def on_MenuSelection(self, event):
         menuItem:MacroMenuItem = self.FindItemById(event.Id)
         if menuItem.path and os.path.isfile(menuItem.path):
             if wx.GetKeyState(wx.WXK_CONTROL):
                 self.app.documentManager.CreateDocument(menuItem.path, DOC_SILENT)
             else:
-                self.app.executeScript(menuItem.path)
+                execfile(menuItem.path)
                 self._lastMacroPath = menuItem.path
                 self.menuItem_repeat.SetItemLabel(
                     f"Repeat: {os.path.splitext(os.path.basename(menuItem.path))[0]}"
                 )
                 self.menuItem_repeat.Enable(True)
 
     def on_menuUpdate(self, event):
-        self._macroTree = None
-        self._clearMenu()
-        self._updateMenue()
-
+        self.rebuild()
 
 class MacroButtonMixin:
     def __init__(self, macroButton, folderName, view=None):
         self._folderName = folderName
         self.view = view
         self._macroFolderPath = []
         self._macroMenu = None
```

### Comparing `wbBase-0.1.54/Lib/wbBase/tools.py` & `wbBase-0.1.55/Lib/wbBase/tools.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/Lib/wbBase.egg-info/PKG-INFO` & `wbBase-0.1.55/Lib/wbBase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbBase
-Version: 0.1.54
+Version: 0.1.55
 Summary: Base package for WorkBench applications.
 Home-page: https://gitlab.com/workbench2/wbbase
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/wbbase
 Project-URL: Documentation, https://workbench2.gitlab.io/wbbase
 Project-URL: Tracker, https://gitlab.com/workbench2/wbbase/-/issues
```

### Comparing `wbBase-0.1.54/Lib/wbBase.egg-info/SOURCES.txt` & `wbBase-0.1.55/Lib/wbBase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/PKG-INFO` & `wbBase-0.1.55/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbBase
-Version: 0.1.54
+Version: 0.1.55
 Summary: Base package for WorkBench applications.
 Home-page: https://gitlab.com/workbench2/wbbase
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/wbbase
 Project-URL: Documentation, https://workbench2.gitlab.io/wbbase
 Project-URL: Tracker, https://gitlab.com/workbench2/wbbase/-/issues
```

### Comparing `wbBase-0.1.54/README.md` & `wbBase-0.1.55/README.md`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.54/setup.cfg` & `wbBase-0.1.55/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.54
+current_version = 0.1.55
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -64,15 +64,15 @@
 where = Lib
 
 [bumpversion:file:Lib/wbBase/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
 [tox:tox]
-min_version = 4.4
+min_version = 4.5
 env_list = 
 	py38
 	py39
 	py10
 
 [testenv]
 deps =
```

