# Comparing `tmp/TelegramChatbotProject-1.0.0.tar.gz` & `tmp/TelegramChatbotProject-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TelegramChatbotProject-1.0.0.tar", last modified: Sun Apr 30 15:59:02 2023, max compression
+gzip compressed data, was "TelegramChatbotProject-1.0.1.tar", last modified: Sun Apr 30 17:22:13 2023, max compression
```

## Comparing `TelegramChatbotProject-1.0.0.tar` & `TelegramChatbotProject-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 15:59:02.142190 TelegramChatbotProject-1.0.0/
--rw-rw-rw-   0        0        0      294 2023-04-30 15:59:02.141190 TelegramChatbotProject-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      462 2023-04-27 19:24:17.000000 TelegramChatbotProject-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 15:59:02.118189 TelegramChatbotProject-1.0.0/TelegramChatbotProject.egg-info/
--rw-rw-rw-   0        0        0      294 2023-04-30 15:59:02.000000 TelegramChatbotProject-1.0.0/TelegramChatbotProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2023-04-30 15:59:02.000000 TelegramChatbotProject-1.0.0/TelegramChatbotProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 15:59:02.000000 TelegramChatbotProject-1.0.0/TelegramChatbotProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-30 15:59:02.000000 TelegramChatbotProject-1.0.0/TelegramChatbotProject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 15:59:02.142190 TelegramChatbotProject-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      387 2023-04-30 15:59:00.000000 TelegramChatbotProject-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 15:59:02.140190 TelegramChatbotProject-1.0.0/telegramchatbotproject/
--rw-rw-rw-   0        0        0      214 2023-04-27 15:41:26.000000 TelegramChatbotProject-1.0.0/telegramchatbotproject/api_key.py
--rw-rw-rw-   0        0        0     2427 2023-04-27 16:32:48.000000 TelegramChatbotProject-1.0.0/telegramchatbotproject/appointment.py
--rw-rw-rw-   0        0        0     7294 2023-04-30 14:29:31.000000 TelegramChatbotProject-1.0.0/telegramchatbotproject/appointment_handler.py
--rw-rw-rw-   0        0        0    10645 2023-04-27 16:34:33.000000 TelegramChatbotProject-1.0.0/telegramchatbotproject/appointment_session.py
--rw-rw-rw-   0        0        0     2993 2023-04-28 14:40:24.000000 TelegramChatbotProject-1.0.0/telegramchatbotproject/base_valaszok.py
--rw-rw-rw-   0        0        0     1779 2023-04-28 15:01:01.000000 TelegramChatbotProject-1.0.0/telegramchatbotproject/kerdes.py
--rw-rw-rw-   0        0        0     3935 2023-04-28 14:42:28.000000 TelegramChatbotProject-1.0.0/telegramchatbotproject/main.py
--rw-rw-rw-   0        0        0      916 2023-04-27 16:32:48.000000 TelegramChatbotProject-1.0.0/telegramchatbotproject/panasz.py
--rw-rw-rw-   0        0        0      799 2023-04-27 16:32:48.000000 TelegramChatbotProject-1.0.0/telegramchatbotproject/panasz_session.py
--rw-rw-rw-   0        0        0     2698 2023-04-28 14:42:28.000000 TelegramChatbotProject-1.0.0/telegramchatbotproject/szam_jatek.py
+drwxrwxrwx   0        0        0        0 2023-04-30 17:22:13.077658 TelegramChatbotProject-1.0.1/
+-rw-rw-rw-   0        0        0      294 2023-04-30 17:22:13.076658 TelegramChatbotProject-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      734 2023-04-30 17:10:22.000000 TelegramChatbotProject-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 17:22:13.070209 TelegramChatbotProject-1.0.1/TelegramChatbotProject.egg-info/
+-rw-rw-rw-   0        0        0      294 2023-04-30 17:22:13.000000 TelegramChatbotProject-1.0.1/TelegramChatbotProject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-04-30 17:22:13.000000 TelegramChatbotProject-1.0.1/TelegramChatbotProject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 17:22:13.000000 TelegramChatbotProject-1.0.1/TelegramChatbotProject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-30 17:22:13.000000 TelegramChatbotProject-1.0.1/TelegramChatbotProject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 17:22:13.077658 TelegramChatbotProject-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      387 2023-04-30 17:17:47.000000 TelegramChatbotProject-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 17:22:13.076658 TelegramChatbotProject-1.0.1/telegramchatbotproject/
+-rw-rw-rw-   0        0        0      214 2023-04-27 15:41:26.000000 TelegramChatbotProject-1.0.1/telegramchatbotproject/api_key.py
+-rw-rw-rw-   0        0        0     2427 2023-04-27 16:32:48.000000 TelegramChatbotProject-1.0.1/telegramchatbotproject/appointment.py
+-rw-rw-rw-   0        0        0     7392 2023-04-30 17:04:13.000000 TelegramChatbotProject-1.0.1/telegramchatbotproject/appointment_handler.py
+-rw-rw-rw-   0        0        0    10645 2023-04-27 16:34:33.000000 TelegramChatbotProject-1.0.1/telegramchatbotproject/appointment_session.py
+-rw-rw-rw-   0        0        0     2993 2023-04-28 14:40:24.000000 TelegramChatbotProject-1.0.1/telegramchatbotproject/base_valaszok.py
+-rw-rw-rw-   0        0        0     1779 2023-04-28 15:01:01.000000 TelegramChatbotProject-1.0.1/telegramchatbotproject/kerdes.py
+-rw-rw-rw-   0        0        0     3957 2023-04-30 17:01:04.000000 TelegramChatbotProject-1.0.1/telegramchatbotproject/main.py
+-rw-rw-rw-   0        0        0      963 2023-04-30 17:04:13.000000 TelegramChatbotProject-1.0.1/telegramchatbotproject/panasz.py
+-rw-rw-rw-   0        0        0      799 2023-04-27 16:32:48.000000 TelegramChatbotProject-1.0.1/telegramchatbotproject/panasz_session.py
+-rw-rw-rw-   0        0        0     2698 2023-04-28 14:42:28.000000 TelegramChatbotProject-1.0.1/telegramchatbotproject/szam_jatek.py
```

### Comparing `TelegramChatbotProject-1.0.0/TelegramChatbotProject.egg-info/SOURCES.txt` & `TelegramChatbotProject-1.0.1/TelegramChatbotProject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TelegramChatbotProject-1.0.0/telegramchatbotproject/appointment.py` & `TelegramChatbotProject-1.0.1/telegramchatbotproject/appointment.py`

 * *Files identical despite different names*

### Comparing `TelegramChatbotProject-1.0.0/telegramchatbotproject/appointment_handler.py` & `TelegramChatbotProject-1.0.1/telegramchatbotproject/appointment_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 
 
 class AppointmentHandler:
     """
     Ebben az osztályban találhatóak az időpontok kezeléséért felelős függvények
     """
 
-    def __init__(self):
+    def __init__(self, path):
         """Konstruktor
                     Args:
                         appointments[]: Az időpontokat tartalmazó tömb
                     """
         self.appointments = []
+        self.path=path
 
     def add_appointment(self, appointment):
         """Adott időpont foglalását rögzítő függvény
                                 Args:
                                     appointment (Appointment): Az adott időpont példánya,
                                     amelyet fel szeretnénk venni a listába.
                                 """
@@ -101,15 +102,15 @@
         for appointment in self.appointments:
             if appointment.name == name:
                 appointments.append(appointment)
         return appointments
 
     def load_appointments(self):
         """Fájlból betölti az eltárolt időpontokat egy tömbbe"""
-        filename = "Content/Appointments.json"
+        filename = self.path+"/TelegramChatbotProject/Content/Appointments.json"
         with open(filename, "r", encoding="utf-8") as file:
             data = json.load(file)
             for appointment_data in data["appointments"]:
                 appointment = Appointment(
                     appointment_data["date_time"],
                     appointment_data["is_free"],
                     appointment_data["name"]
@@ -130,15 +131,15 @@
                 free_appointments.append(appointment)
         return free_appointments
 
     def save_appointments(self):
         """"Fájlba mentjük a változtatásokat az időpontokon
                 Minden foglalás és törlés után mentünk, hogy ha bármilyen okból leáll a rendszer,
                 a felhasználók változtatásai ne veszhessenek el."""
-        filename = "Content/Appointments.json"
+        filename = self.path+"/TelegramChatbotProject/Content/Appointments.json"
         data = {"appointments": []}
         for appointment in self.appointments:
             appointment_data = {
                 "date_time": appointment.date_time.isoformat(),
                 "is_free": appointment.is_free,
                 "name": appointment.name
             }
```

### Comparing `TelegramChatbotProject-1.0.0/telegramchatbotproject/appointment_session.py` & `TelegramChatbotProject-1.0.1/telegramchatbotproject/appointment_session.py`

 * *Files identical despite different names*

### Comparing `TelegramChatbotProject-1.0.0/telegramchatbotproject/base_valaszok.py` & `TelegramChatbotProject-1.0.1/telegramchatbotproject/base_valaszok.py`

 * *Files identical despite different names*

### Comparing `TelegramChatbotProject-1.0.0/telegramchatbotproject/kerdes.py` & `TelegramChatbotProject-1.0.1/telegramchatbotproject/kerdes.py`

 * *Files identical despite different names*

### Comparing `TelegramChatbotProject-1.0.0/telegramchatbotproject/main.py` & `TelegramChatbotProject-1.0.1/telegramchatbotproject/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 from telegram.ext import Updater, CommandHandler, MessageHandler, Filters
 import api_key as keys
 import base_valaszok as R
 from appointment_handler import AppointmentHandler
 from appointment_session import AppointmentSession
 from panasz_session import PanaszSession
 from szam_jatek import JatekSession
+import os
 
 sessions = {}
 panasz = {}
 jatek = {}
-appointmentHandler = AppointmentHandler()
+appointmentHandler = AppointmentHandler(os.getcwd())
 appointmentHandler.load_appointments()
 appointmentHandler.remove_old_appointments()
 appointmentHandler.create_missing_appointments()
 
 
 def start_command(update, context):
     """
```

### Comparing `TelegramChatbotProject-1.0.0/telegramchatbotproject/panasz.py` & `TelegramChatbotProject-1.0.1/telegramchatbotproject/panasz.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Ebben a modulban a panaszkezeléshez szükséges
 Panasz osztályt valósítjuk meg.
 """
 from datetime import datetime
+import os
 
 
 class Panasz:
     """
     A panasz osztályban rögzítjük a felhasználó által
     felvett panaszt.
     """
@@ -21,14 +22,14 @@
         self.text = text
         self.ido = datetime.now()
 
     def save(self):
         """
         A panaszt file-ba mentő függvény
         """
-        filename = f"Reklamaciok/{self.username}-{self.ido.strftime('%Y-%m-%d_%H-%M-%S')}.txt"
+        filename = os.getcwd()+f"/TelegramChatbotProject/Reklamaciok/{self.username}-{self.ido.strftime('%Y-%m-%d_%H-%M-%S')}.txt"
         with open(filename, "w", encoding="utf-8") as file:
             file.write(f"{str(self.username)}\n{self.text}\n")
 
     def get_text(self):
         """Getter a szöveg tartalmához."""
         return self.text
```

### Comparing `TelegramChatbotProject-1.0.0/telegramchatbotproject/panasz_session.py` & `TelegramChatbotProject-1.0.1/telegramchatbotproject/panasz_session.py`

 * *Files identical despite different names*

### Comparing `TelegramChatbotProject-1.0.0/telegramchatbotproject/szam_jatek.py` & `TelegramChatbotProject-1.0.1/telegramchatbotproject/szam_jatek.py`

 * *Files identical despite different names*

