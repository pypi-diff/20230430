# Comparing `tmp/PySide6_Customized_Window-1.0-py3-none-any.whl.zip` & `tmp/PySide6_Customized_Window-1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9244 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    40229 b- defN 23-Apr-29 12:35 PySide6_Customized_Window.py
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-29 13:54 PySide6_Customized_Window-1.0.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat      418 b- defN 23-Apr-29 13:54 PySide6_Customized_Window-1.0.dist-info/metadata.json
--rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-29 13:54 PySide6_Customized_Window-1.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 23-Apr-29 13:54 PySide6_Customized_Window-1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      271 b- defN 23-Apr-29 13:54 PySide6_Customized_Window-1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      672 b- defN 23-Apr-29 13:54 PySide6_Customized_Window-1.0.dist-info/RECORD
-7 files, 41698 bytes uncompressed, 8034 bytes compressed:  80.7%
+Zip file size: 9529 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    40992 b- defN 23-Apr-30 06:47 PySide6_Customized_Window.py
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-30 08:33 PySide6_Customized_Window-1.1.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat      619 b- defN 23-Apr-30 08:33 PySide6_Customized_Window-1.1.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-30 08:33 PySide6_Customized_Window-1.1.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Apr-30 08:33 PySide6_Customized_Window-1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      486 b- defN 23-Apr-30 08:33 PySide6_Customized_Window-1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      672 b- defN 23-Apr-30 08:33 PySide6_Customized_Window-1.1.dist-info/RECORD
+7 files, 42877 bytes uncompressed, 8319 bytes compressed:  80.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: PySide6_Customized_Window.py
 Comment: 
 
-Filename: PySide6_Customized_Window-1.0.dist-info/DESCRIPTION.rst
+Filename: PySide6_Customized_Window-1.1.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: PySide6_Customized_Window-1.0.dist-info/metadata.json
+Filename: PySide6_Customized_Window-1.1.dist-info/metadata.json
 Comment: 
 
-Filename: PySide6_Customized_Window-1.0.dist-info/top_level.txt
+Filename: PySide6_Customized_Window-1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: PySide6_Customized_Window-1.0.dist-info/WHEEL
+Filename: PySide6_Customized_Window-1.1.dist-info/WHEEL
 Comment: 
 
-Filename: PySide6_Customized_Window-1.0.dist-info/METADATA
+Filename: PySide6_Customized_Window-1.1.dist-info/METADATA
 Comment: 
 
-Filename: PySide6_Customized_Window-1.0.dist-info/RECORD
+Filename: PySide6_Customized_Window-1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## PySide6_Customized_Window.py

```diff
@@ -207,16 +207,24 @@
         self.animation2 = QPropertyAnimation(self, b'windowOpacity')
         self.animation2.setDuration(250)
         self.animation2.setStartValue(1.0)
         self.animation2.setEndValue(0.0)
         self.nonclientareasizeinited = False
         self.isblurwindow = isinstance(self, BlurWindow)
         WNDPROC = ctypes.WINFUNCTYPE(ctypes.c_long, ctypes.c_int, ctypes.c_uint, ctypes.c_int, ctypes.c_int)
-        MessageHandlerAddress = ctypes.cast(WNDPROC(self.MessageHandler), ctypes.c_void_p).value
-        self.originalMessageHandler = ctypes.windll.user32.SetWindowLongW(self.hwnd, -4, MessageHandlerAddress)
+        BasicMessageHandlerAddress = ctypes.cast(WNDPROC(self.BasicMessageHandler), ctypes.c_void_p).value
+        try:
+            self.originalBasicMessageHandler = ctypes.windll.user32.GetWindowLongPtrW(self.hwnd, -4)
+        except:
+            self.originalBasicMessageHandler = ctypes.windll.user32.GetWindowLongW(self.hwnd, -4)
+        if ISPYSIDE1:
+            try:
+                ctypes.windll.user32.SetWindowLongPtrW(self.hwnd, -4, ctypes.c_int64(BasicMessageHandlerAddress))
+            except:
+                ctypes.windll.user32.SetWindowLongW(self.hwnd, -4, BasicMessageHandlerAddress)
         self.setAttribute(Qt.WA_TranslucentBackground, True)
         self.hwnd = gethwnd(self)
         if ISPYSIDE1:
             ctypes.windll.user32.SetWindowLongW(self.hwnd, -16, 0x40000 | 0x20000 | 0x10000)
         else:
             ctypes.windll.user32.SetWindowLongW(self.hwnd, -16, 0xc00000 | 0x40000 | 0x20000 | 0x10000)
         ctypes.windll.user32.SetWindowLongW(self.hwnd, -20, 0x200)
@@ -508,22 +516,23 @@
                 stylesheet3 = self.closeButtonPressedBackgroundStyleSheet
         elif button != 0:
             raise Exception
         self.minSizeButton.setStyleSheet(stylesheet1)
         self.maxSizeButton.setStyleSheet(stylesheet2)
         self.closeButton.setStyleSheet(stylesheet3)
     def MessageHandler(self, hwnd, message, wParam, lParam):
-        '''For PySide1/2/6, you should call super method after defining MessageHandler.
-Here's an example:
+        '''Example:
 class MyOwnWindow(self):
 |->|...
 |->|def MessageHandler(self, hwnd, message, wParam, lParam):
-|->||->|super(MyOwnWindow, self).MessageHandler(self, hwnd, message, wParam, lParam)
-|->||->|...
-'''
+|->||->|print(hwnd, message, wParam, lParam)
+|->||->|...'''
+        pass
+    def BasicMessageHandler(self, hwnd, message, wParam, lParam):
+        '''For PySide1/2/6, you should define MessageHandler instead of BasicMessageHandler.'''
         WM_ACTIVATE = 0x6
         WM_SHOWWINDOW = 0x18
         WM_SETTINGCHANGE = 0x1a
         WM_GETMINMAXINFO = 0x24
         WM_NCCALCSIZE = 0x83
         WM_NCHITTEST = 0x84
         WM_NCLBUTTONDOWN = 0xa1
@@ -568,15 +577,18 @@
             border_width = 0
             title_height = 0
             menubutton_width = 0
             windowmargin_left = 0
             windowmargin_right = 0
             windowmargin_top = 0
             windowmargin_bottom = 0
-        windowrect = self.GetWindowRect()
+        try:
+            windowrect = self.GetWindowRect()
+        except:
+            windowrect = RECT(0, 0, 0, 0)
         windowx = windowrect.left
         windowy = windowrect.top
         try:
             globalpos = POINT()
             ctypes.windll.user32.GetPhysicalCursorPos(ctypes.byref(globalpos))
             ctypes.windll.user32.PhysicalToLogicalPoint(self.hwnd, ctypes.byref(globalpos))
             x = globalpos.x - windowx
@@ -683,15 +695,15 @@
             self.setGeometry(x, y, width, height)
             self.border_width = int(5.0 * dpi / 96.0)
             self.title_height = int(30.0 * dpi / 96.0)
             self.menubutton_width = int(46.0 * dpi / 96.0)
             self.title_font_size = int(13.0 * dpi / 96.0)
             self.titleiconlayout_margin = int(7.0 * dpi / 96.0)
             self.paintTitleBarAndClientArea(self.isActiveWindow())
-            ctypes.windll.user32.CallWindowProcW(self.originalMessageHandler, hwnd, message, wParam, lParam)
+            ctypes.windll.user32.CallWindowProcW(self.originalBasicMessageHandler, hwnd, message, wParam, lParam)
             return 0
         if message == WM_SETTINGCHANGE:
             if self.themecolour == 0 and str(ctypes.cast(lParam, ctypes.c_wchar_p).value) == 'ImmersiveColorSet':
                 self.isdarktheme = isdarktheme()
                 self.paintTitleBarAndClientArea(self.isActiveWindow())
         if message == WM_DWMCOMPOSITIONCHANGED:
             self.isaeroenabled = isAeroEnabled()
@@ -704,15 +716,19 @@
         if message == WM_ACTIVATE:
             isactivewindow = 0 if wParam == 0 else 1
             if not isactivewindow:
                 self.setMenuButtonStyle(0)
             self.paintTitleBarAndClientArea(isactivewindow)
         if message == WM_SHOWWINDOW:
             self.paintTitleBarAndClientArea(self.isActiveWindow())
-        return ctypes.windll.user32.CallWindowProcW(self.originalMessageHandler, hwnd, message, wParam, lParam)
+        messagehandlerresult = self.MessageHandler(hwnd, message, wParam, lParam)
+        if messagehandlerresult != None:
+            return messagehandlerresult
+        if ISPYSIDE1:
+            return ctypes.windll.user32.CallWindowProcW(self.originalBasicMessageHandler, hwnd, message, wParam, lParam)
     def Handle_WM_NCCALCSIZE_Message(self, hwnd, message, wParam, lParam):
         try:
             nonclientareasizeinited = self.nonclientareasizeinited
         except:
             nonclientareasizeinited = False
         if not nonclientareasizeinited:
             if ISPYSIDE1:
@@ -775,32 +791,28 @@
             borderwidth_x = ctypes.windll.user32.GetSystemMetricsForDpi(SM_CXSIZEFRAME, dpi) + ctypes.windll.user32.GetSystemMetricsForDpi(SM_CXPADDEDBORDER, dpi)
             borderwidth_y = ctypes.windll.user32.GetSystemMetricsForDpi(SM_CYSIZEFRAME, dpi) + ctypes.windll.user32.GetSystemMetricsForDpi(SM_CXPADDEDBORDER, dpi)
         except:
             borderwidth_x = ctypes.windll.user32.GetSystemMetrics(SM_CXSIZEFRAME) + ctypes.windll.user32.GetSystemMetrics(SM_CXPADDEDBORDER)
             borderwidth_y = ctypes.windll.user32.GetSystemMetrics(SM_CYSIZEFRAME) + ctypes.windll.user32.GetSystemMetrics(SM_CXPADDEDBORDER)
         return [borderwidth_x, borderwidth_y]
     def nativeEvent(self, eventType, msg):
-        '''For PySide2/6, you should call super method after defining nativeEvent.
-Here's an example:
-class MyOwnWindow(self):
-|->|...
-|->|def nativeEvent(self, eventType, msg):
-|->||->|super(MyOwnWindow, self).nativeEvent(self, eventType, msg)
-|->||->|...
-'''
+        '''For PySide2/6, you should define MessageHandler instead of nativeEvent.'''
         WM_NCCALCSIZE = 0x83
         msg = MSG.from_address(msg.__int__())
         hwnd = msg.hWnd
         message = msg.message
         wParam = msg.wParam
         lParam = msg.lParam
         if message == WM_NCCALCSIZE:
             if not ISPYSIDE1:
                 return True, self.Handle_WM_NCCALCSIZE_Message(hwnd, message, wParam, lParam)
-        return super().nativeEvent(eventType, msg)
+        basicmessagehandlerresult = self.BasicMessageHandler(hwnd, message, wParam, lParam)
+        if basicmessagehandlerresult != None:
+            return True, basicmessagehandlerresult
+        return super(CustomizedWindow, self).nativeEvent(eventType, msg)
     def setBlurEffect(self):
         hwnd = self.hwnd
         try:
             bb = DWM_BLURBEHIND()
             bb.dwFlags = 1
             bb.fEnable = 1
             ctypes.windll.dwmapi.DwmSetWindowAttribute(hwnd, 2, ctypes.byref(ctypes.c_int(2)), ctypes.sizeof(ctypes.c_int(2)))
```

