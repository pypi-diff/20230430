# Comparing `tmp/automation_editor-0.0.2.tar.gz` & `tmp/automation_editor-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_editor-0.0.2.tar", last modified: Sat Apr 29 10:30:02 2023, max compression
+gzip compressed data, was "automation_editor-0.0.3.tar", last modified: Sun Apr 30 08:01:56 2023, max compression
```

## Comparing `automation_editor-0.0.2.tar` & `automation_editor-0.0.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.025958 automation_editor-0.0.2/
--rw-rw-rw-   0        0        0     1085 2023-04-05 12:50:43.000000 automation_editor-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     5751 2023-04-29 10:30:02.024960 automation_editor-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5023 2023-04-29 10:29:31.000000 automation_editor-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.952155 automation_editor-0.0.2/automation_editor/
--rw-rw-rw-   0        0        0      130 2023-04-29 09:53:20.000000 automation_editor-0.0.2/automation_editor/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.969109 automation_editor-0.0.2/automation_editor/automation_editor_ui/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.973100 automation_editor-0.0.2/automation_editor/automation_editor_ui/editor_main/
--rw-rw-rw-   0        0        0        0 2023-04-24 10:50:57.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/editor_main/__init__.py
--rw-rw-rw-   0        0        0     1324 2023-04-29 09:53:20.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/editor_main/main_ui.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.976092 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.978087 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/api_testka_menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/api_testka_menu/__init__.py
--rw-rw-rw-   0        0        0     3998 2023-04-29 10:27:21.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.981078 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/auto_control_menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/auto_control_menu/__init__.py
--rw-rw-rw-   0        0        0     4129 2023-04-29 10:27:09.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.984071 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/load_density_menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/load_density_menu/__init__.py
--rw-rw-rw-   0        0        0     4161 2023-04-29 10:27:56.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.986064 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/web_runner_menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/web_runner_menu/__init__.py
--rw-rw-rw-   0        0        0     4040 2023-04-29 10:27:42.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.989056 automation_editor-0.0.2/automation_editor/automation_editor_ui/show_code_window/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/show_code_window/__init__.py
--rw-rw-rw-   0        0        0      791 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/show_code_window/code_window.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.993046 automation_editor-0.0.2/automation_editor/automation_editor_ui/syntax/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/syntax/__init__.py
--rw-rw-rw-   0        0        0      777 2023-04-29 09:53:20.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/syntax/syntax_extend.py
--rw-rw-rw-   0        0        0     3257 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/automation_editor_ui/syntax/syntax_keyword.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.995042 automation_editor-0.0.2/automation_editor/extend/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.997036 automation_editor-0.0.2/automation_editor/extend/mail_thunder_extend/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/extend/mail_thunder_extend/__init__.py
--rw-rw-rw-   0        0        0     1696 2023-04-29 09:53:20.000000 automation_editor-0.0.2/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.998033 automation_editor-0.0.2/automation_editor/utils/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.002022 automation_editor-0.0.2/automation_editor/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     1500 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      608 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.004016 automation_editor-0.0.2/automation_editor/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-04-27 10:28:14.000000 automation_editor-0.0.2/automation_editor/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.007008 automation_editor-0.0.2/automation_editor/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0      991 2023-04-29 09:53:20.000000 automation_editor-0.0.2/automation_editor/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.008006 automation_editor-0.0.2/automation_editor/utils/manager/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.011001 automation_editor-0.0.2/automation_editor/utils/manager/package_manager/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/manager/package_manager/__init__.py
--rw-rw-rw-   0        0        0     1737 2023-04-28 11:00:21.000000 automation_editor-0.0.2/automation_editor/utils/manager/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.013990 automation_editor-0.0.2/automation_editor/utils/test_executor/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.015985 automation_editor-0.0.2/automation_editor/utils/test_executor/api_testka/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/api_testka/__init__.py
--rw-rw-rw-   0        0        0     3935 2023-04-29 09:53:20.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/api_testka/api_testka_process.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.018976 automation_editor-0.0.2/automation_editor/utils/test_executor/auto_control/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/auto_control/__init__.py
--rw-rw-rw-   0        0        0     3939 2023-04-29 09:53:20.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/auto_control/auto_control_process.py
--rw-rw-rw-   0        0        0      498 2023-04-29 09:53:20.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/check_mail_thunder.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.020971 automation_editor-0.0.2/automation_editor/utils/test_executor/load_density/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/load_density/__init__.py
--rw-rw-rw-   0        0        0     3949 2023-04-29 09:53:20.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/load_density/load_density_process.py
--rw-rw-rw-   0        0        0     5837 2023-04-28 11:00:21.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/task_process_manager.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:02.023963 automation_editor-0.0.2/automation_editor/utils/test_executor/web_runner/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/web_runner/__init__.py
--rw-rw-rw-   0        0        0     3897 2023-04-29 09:53:20.000000 automation_editor-0.0.2/automation_editor/utils/test_executor/web_runner/web_runner_process.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:30:01.968112 automation_editor-0.0.2/automation_editor.egg-info/
--rw-rw-rw-   0        0        0     5751 2023-04-29 10:30:01.000000 automation_editor-0.0.2/automation_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2931 2023-04-29 10:30:01.000000 automation_editor-0.0.2/automation_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 10:30:01.000000 automation_editor-0.0.2/automation_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-04-29 10:30:01.000000 automation_editor-0.0.2/automation_editor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-29 10:30:01.000000 automation_editor-0.0.2/automation_editor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1143 2023-04-29 10:29:43.000000 automation_editor-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 10:30:02.025958 automation_editor-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.603769 automation_editor-0.0.3/
+-rw-rw-rw-   0        0        0     1085 2023-04-05 12:50:43.000000 automation_editor-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5793 2023-04-30 08:01:56.602741 automation_editor-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5065 2023-04-29 11:09:10.000000 automation_editor-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.537915 automation_editor-0.0.3/automation_editor/
+-rw-rw-rw-   0        0        0      130 2023-04-29 09:53:20.000000 automation_editor-0.0.3/automation_editor/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.554870 automation_editor-0.0.3/automation_editor/automation_editor_ui/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.557918 automation_editor-0.0.3/automation_editor/automation_editor_ui/editor_main/
+-rw-rw-rw-   0        0        0        0 2023-04-24 10:50:57.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/editor_main/__init__.py
+-rw-rw-rw-   0        0        0     1323 2023-04-30 07:37:34.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/editor_main/main_ui.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.558896 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/
+-rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.560854 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/api_testka_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/api_testka_menu/__init__.py
+-rw-rw-rw-   0        0        0     3998 2023-04-29 10:27:21.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.562849 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/auto_control_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/auto_control_menu/__init__.py
+-rw-rw-rw-   0        0        0     4129 2023-04-29 10:27:09.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.564880 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/load_density_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/load_density_menu/__init__.py
+-rw-rw-rw-   0        0        0     4161 2023-04-29 10:27:56.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.566873 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/web_runner_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/web_runner_menu/__init__.py
+-rw-rw-rw-   0        0        0     4040 2023-04-29 10:27:42.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.569831 automation_editor-0.0.3/automation_editor/automation_editor_ui/show_code_window/
+-rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/show_code_window/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/show_code_window/code_window.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.572822 automation_editor-0.0.3/automation_editor/automation_editor_ui/syntax/
+-rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/syntax/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-04-29 09:53:20.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/syntax/syntax_extend.py
+-rw-rw-rw-   0        0        0     3257 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/syntax/syntax_keyword.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.573819 automation_editor-0.0.3/automation_editor/extend/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.575850 automation_editor-0.0.3/automation_editor/extend/mail_thunder_extend/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/extend/mail_thunder_extend/__init__.py
+-rw-rw-rw-   0        0        0     1696 2023-04-29 09:53:20.000000 automation_editor-0.0.3/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.576810 automation_editor-0.0.3/automation_editor/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.580801 automation_editor-0.0.3/automation_editor/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     1500 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      608 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.583793 automation_editor-0.0.3/automation_editor/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.585787 automation_editor-0.0.3/automation_editor/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0      991 2023-04-29 09:53:20.000000 automation_editor-0.0.3/automation_editor/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.587782 automation_editor-0.0.3/automation_editor/utils/manager/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.590774 automation_editor-0.0.3/automation_editor/utils/manager/package_manager/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/manager/package_manager/__init__.py
+-rw-rw-rw-   0        0        0     1737 2023-04-28 11:00:21.000000 automation_editor-0.0.3/automation_editor/utils/manager/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.593765 automation_editor-0.0.3/automation_editor/utils/test_executor/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.595766 automation_editor-0.0.3/automation_editor/utils/test_executor/api_testka/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/api_testka/__init__.py
+-rw-rw-rw-   0        0        0     3935 2023-04-29 09:53:20.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/api_testka/api_testka_process.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.597792 automation_editor-0.0.3/automation_editor/utils/test_executor/auto_control/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/auto_control/__init__.py
+-rw-rw-rw-   0        0        0     3939 2023-04-29 09:53:20.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/auto_control/auto_control_process.py
+-rw-rw-rw-   0        0        0      498 2023-04-29 09:53:20.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/check_mail_thunder.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.599750 automation_editor-0.0.3/automation_editor/utils/test_executor/load_density/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/load_density/__init__.py
+-rw-rw-rw-   0        0        0     3949 2023-04-29 09:53:20.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/load_density/load_density_process.py
+-rw-rw-rw-   0        0        0     5837 2023-04-28 11:00:21.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/task_process_manager.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.601745 automation_editor-0.0.3/automation_editor/utils/test_executor/web_runner/
+-rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/web_runner/__init__.py
+-rw-rw-rw-   0        0        0     3897 2023-04-29 09:53:20.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/web_runner/web_runner_process.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.553912 automation_editor-0.0.3/automation_editor.egg-info/
+-rw-rw-rw-   0        0        0     5793 2023-04-30 08:01:56.000000 automation_editor-0.0.3/automation_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2931 2023-04-30 08:01:56.000000 automation_editor-0.0.3/automation_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 08:01:56.000000 automation_editor-0.0.3/automation_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-04-30 08:01:56.000000 automation_editor-0.0.3/automation_editor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-30 08:01:56.000000 automation_editor-0.0.3/automation_editor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1143 2023-04-30 07:49:28.000000 automation_editor-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 08:01:56.603769 automation_editor-0.0.3/setup.cfg
```

### Comparing `automation_editor-0.0.2/LICENSE` & `automation_editor-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.2/PKG-INFO` & `automation_editor-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation_editor
-Version: 0.0.2
+Version: 0.0.3
 Summary: Automation Editor for GUI, WEB, API, Load Automation
 Author-email: JE-Chen <zenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Integrated-Testing-Environment/AutomationEditor
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
@@ -45,70 +45,70 @@
 >>    * Auto-save (after first save or open).
 >>    * Tree file structure browsing.
 >>    * Save and open files.
 >>    * Python formatting check using yapf.
 >>    * Run python programs.
 >>    * Run shell commands.
 ---
-### GUI Testing components
+### GUI Automation components
 > Image & Coordinate based GUI Automation \
 > GUI automated based on image comparison and coordinates. \
 > Cross-platform and cross-programming language.\
 > Solve problems:
 >> * Provide automation execution for repetitive tasks.
->> * Multiple methods are available, including recording, image recognition, and coordinate-based testing.
+>> * Multiple methods are available, including recording, image recognition, and coordinate-based automation.
 >> * Tests can be executed remotely through TCP/IP.
 >> * Test reports can be generated with records for each action.
 >> * The same code can be used for three platforms, reducing the possibility of platform-dependent programs.
 >> * Provide hooks for keyboard and mouse events and state checks (including using code to simulate key presses).
 >> * Can use keywords for development to improve readability.
 ---
-### WEB Testing components
+### WEB Automation components
 > Multiton Selenium Instance Automation \
 > The WEB Automation component is a web automation solution based on Selenium. \
 > It wraps Selenium and therefore has all the functionality of Selenium. \
 > What problems does it solve? 
 >> * Automatically downloads and updates the required web driver, so users no longer need to install it manually.
 >> * Provides the ability to simultaneously run and monitor multiple Selenium instances.
->> * Provides a keyword-based testing approach that Selenium does not have.
+>> * Provides a keyword-based automation approach that Selenium does not have.
 >> * Can produce test reports that record actions taken during the test.
 >> * Can execute tests remotely through TCP/IP.
->> * Offers a CLI mode for Web Testing.
+>> * Offers a CLI mode for Web automation.
 ---
-### API Testing components
+### API Automation components
 > Simple way to Automation Requests HTTP/S & Soap \
 > Wrapper for Requests package, designed for those with experience using Requests. \
 > Send HTTP/S and SOAP requests with a simple line of code or keyword. \
 > Detailed information on Requests and Responses. \
 > Solves problems such as:
->> * Detailed testing reports on Requests and Responses.
->> * Testing for SOAP protocol.
+>> * Detailed automation reports on Requests and Responses.
+>> * Automation for SOAP protocol.
 >> * Data comparison for each Request.
->> * API Testing in pure CLI mode.
+>> * API automation in pure CLI mode.
 ---
-### Load & Stress Testing components
+### Load & Stress Automation components
 > Locust Wrapper \
 > Wrapper for Locust, simplifying complex Locust configurations. \
 > Solves problems:
 >> * Checking Requests & Response for each load test
->> * Load testing for SOAP protocols
+>> * Load automation for SOAP protocols
 >> * Comparison of numerical values for each load test
 >> * Detailed load test reports for each test.
 ---
 
 ### Features
 
 > * GUI Automation (use AutoControl)
 > * API Automation (use APITestka)
 > * Web Automation (use WebRunner)
 > * Loading Automation (use LoadDensity)
 > * Multi test task runner (multiprocess, but without AutoControl)
-> * you can run multi testing on same time
-> * open log window to check testing result
-> * Send mail when testing failure (need to setting mail)
+> * you can run multi automation on same time
+> * open log window to check automation result
+> * Send mail when automation failure (need to setting mail)
 
 ---
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b7d32ed8600b4bd2a2f3e960f46f2ad0)](https://www.codacy.com/gh/JE-Chen/Integration-testing-environment/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=JE-Chen/Integration-testing-environment&amp;utm_campaign=Badge_Grade)
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/Integrated-Testing-Environment/Integration-testing-environment/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Integrated-Testing-Environment/Integration-testing-environment/tree/main)
```

### Comparing `automation_editor-0.0.2/README.md` & `automation_editor-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -26,70 +26,70 @@
 >>    * Auto-save (after first save or open).
 >>    * Tree file structure browsing.
 >>    * Save and open files.
 >>    * Python formatting check using yapf.
 >>    * Run python programs.
 >>    * Run shell commands.
 ---
-### GUI Testing components
+### GUI Automation components
 > Image & Coordinate based GUI Automation \
 > GUI automated based on image comparison and coordinates. \
 > Cross-platform and cross-programming language.\
 > Solve problems:
 >> * Provide automation execution for repetitive tasks.
->> * Multiple methods are available, including recording, image recognition, and coordinate-based testing.
+>> * Multiple methods are available, including recording, image recognition, and coordinate-based automation.
 >> * Tests can be executed remotely through TCP/IP.
 >> * Test reports can be generated with records for each action.
 >> * The same code can be used for three platforms, reducing the possibility of platform-dependent programs.
 >> * Provide hooks for keyboard and mouse events and state checks (including using code to simulate key presses).
 >> * Can use keywords for development to improve readability.
 ---
-### WEB Testing components
+### WEB Automation components
 > Multiton Selenium Instance Automation \
 > The WEB Automation component is a web automation solution based on Selenium. \
 > It wraps Selenium and therefore has all the functionality of Selenium. \
 > What problems does it solve? 
 >> * Automatically downloads and updates the required web driver, so users no longer need to install it manually.
 >> * Provides the ability to simultaneously run and monitor multiple Selenium instances.
->> * Provides a keyword-based testing approach that Selenium does not have.
+>> * Provides a keyword-based automation approach that Selenium does not have.
 >> * Can produce test reports that record actions taken during the test.
 >> * Can execute tests remotely through TCP/IP.
->> * Offers a CLI mode for Web Testing.
+>> * Offers a CLI mode for Web automation.
 ---
-### API Testing components
+### API Automation components
 > Simple way to Automation Requests HTTP/S & Soap \
 > Wrapper for Requests package, designed for those with experience using Requests. \
 > Send HTTP/S and SOAP requests with a simple line of code or keyword. \
 > Detailed information on Requests and Responses. \
 > Solves problems such as:
->> * Detailed testing reports on Requests and Responses.
->> * Testing for SOAP protocol.
+>> * Detailed automation reports on Requests and Responses.
+>> * Automation for SOAP protocol.
 >> * Data comparison for each Request.
->> * API Testing in pure CLI mode.
+>> * API automation in pure CLI mode.
 ---
-### Load & Stress Testing components
+### Load & Stress Automation components
 > Locust Wrapper \
 > Wrapper for Locust, simplifying complex Locust configurations. \
 > Solves problems:
 >> * Checking Requests & Response for each load test
->> * Load testing for SOAP protocols
+>> * Load automation for SOAP protocols
 >> * Comparison of numerical values for each load test
 >> * Detailed load test reports for each test.
 ---
 
 ### Features
 
 > * GUI Automation (use AutoControl)
 > * API Automation (use APITestka)
 > * Web Automation (use WebRunner)
 > * Loading Automation (use LoadDensity)
 > * Multi test task runner (multiprocess, but without AutoControl)
-> * you can run multi testing on same time
-> * open log window to check testing result
-> * Send mail when testing failure (need to setting mail)
+> * you can run multi automation on same time
+> * open log window to check automation result
+> * Send mail when automation failure (need to setting mail)
 
 ---
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b7d32ed8600b4bd2a2f3e960f46f2ad0)](https://www.codacy.com/gh/JE-Chen/Integration-testing-environment/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=JE-Chen/Integration-testing-environment&amp;utm_campaign=Badge_Grade)
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/Integrated-Testing-Environment/Integration-testing-environment/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Integrated-Testing-Environment/Integration-testing-environment/tree/main)
```

### Comparing `automation_editor-0.0.2/automation_editor/automation_editor_ui/editor_main/main_ui.py` & `automation_editor-0.0.3/automation_editor/automation_editor_ui/editor_main/main_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 
 
 def start_editor():
     new_editor = QApplication(sys.argv)
     window = ITE()
     apply_stylesheet(new_editor, theme='dark_amber.xml')
     window.show()
-    sys.exit(new_editor.exec_())
+    sys.exit(new_editor.exec())
```

### Comparing `automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py` & `automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py` & `automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py` & `automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.2/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py` & `automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.2/automation_editor/automation_editor_ui/show_code_window/code_window.py` & `automation_editor-0.0.3/automation_editor/automation_editor_ui/show_code_window/code_window.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.2/automation_editor/automation_editor_ui/syntax/syntax_extend.py` & `automation_editor-0.0.3/automation_editor/automation_editor_ui/syntax/syntax_extend.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.2/automation_editor/automation_editor_ui/syntax/syntax_keyword.py` & `automation_editor-0.0.3/automation_editor/automation_editor_ui/syntax/syntax_keyword.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.2/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py` & `automation_editor-0.0.3/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.2/automation_editor/utils/exception/exception_tags.py` & `automation_editor-0.0.3/automation_editor/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.2/automation_editor/utils/exception/exceptions.py` & `automation_editor-0.0.3/automation_editor/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.2/automation_editor/utils/file_process/get_dir_file_list.py` & `automation_editor-0.0.3/automation_editor/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.2/automation_editor/utils/json_format/json_process.py` & `automation_editor-0.0.3/automation_editor/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.2/automation_editor/utils/manager/package_manager/package_manager_class.py` & `automation_editor-0.0.3/automation_editor/utils/manager/package_manager/package_manager_class.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.2/automation_editor/utils/test_executor/api_testka/api_testka_process.py` & `automation_editor-0.0.3/automation_editor/utils/test_executor/api_testka/api_testka_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.2/automation_editor/utils/test_executor/auto_control/auto_control_process.py` & `automation_editor-0.0.3/automation_editor/utils/test_executor/auto_control/auto_control_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.2/automation_editor/utils/test_executor/load_density/load_density_process.py` & `automation_editor-0.0.3/automation_editor/utils/test_executor/load_density/load_density_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.2/automation_editor/utils/test_executor/task_process_manager.py` & `automation_editor-0.0.3/automation_editor/utils/test_executor/task_process_manager.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.2/automation_editor/utils/test_executor/web_runner/web_runner_process.py` & `automation_editor-0.0.3/automation_editor/utils/test_executor/web_runner/web_runner_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.2/automation_editor.egg-info/PKG-INFO` & `automation_editor-0.0.3/automation_editor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-editor
-Version: 0.0.2
+Version: 0.0.3
 Summary: Automation Editor for GUI, WEB, API, Load Automation
 Author-email: JE-Chen <zenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Integrated-Testing-Environment/AutomationEditor
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
@@ -45,70 +45,70 @@
 >>    * Auto-save (after first save or open).
 >>    * Tree file structure browsing.
 >>    * Save and open files.
 >>    * Python formatting check using yapf.
 >>    * Run python programs.
 >>    * Run shell commands.
 ---
-### GUI Testing components
+### GUI Automation components
 > Image & Coordinate based GUI Automation \
 > GUI automated based on image comparison and coordinates. \
 > Cross-platform and cross-programming language.\
 > Solve problems:
 >> * Provide automation execution for repetitive tasks.
->> * Multiple methods are available, including recording, image recognition, and coordinate-based testing.
+>> * Multiple methods are available, including recording, image recognition, and coordinate-based automation.
 >> * Tests can be executed remotely through TCP/IP.
 >> * Test reports can be generated with records for each action.
 >> * The same code can be used for three platforms, reducing the possibility of platform-dependent programs.
 >> * Provide hooks for keyboard and mouse events and state checks (including using code to simulate key presses).
 >> * Can use keywords for development to improve readability.
 ---
-### WEB Testing components
+### WEB Automation components
 > Multiton Selenium Instance Automation \
 > The WEB Automation component is a web automation solution based on Selenium. \
 > It wraps Selenium and therefore has all the functionality of Selenium. \
 > What problems does it solve? 
 >> * Automatically downloads and updates the required web driver, so users no longer need to install it manually.
 >> * Provides the ability to simultaneously run and monitor multiple Selenium instances.
->> * Provides a keyword-based testing approach that Selenium does not have.
+>> * Provides a keyword-based automation approach that Selenium does not have.
 >> * Can produce test reports that record actions taken during the test.
 >> * Can execute tests remotely through TCP/IP.
->> * Offers a CLI mode for Web Testing.
+>> * Offers a CLI mode for Web automation.
 ---
-### API Testing components
+### API Automation components
 > Simple way to Automation Requests HTTP/S & Soap \
 > Wrapper for Requests package, designed for those with experience using Requests. \
 > Send HTTP/S and SOAP requests with a simple line of code or keyword. \
 > Detailed information on Requests and Responses. \
 > Solves problems such as:
->> * Detailed testing reports on Requests and Responses.
->> * Testing for SOAP protocol.
+>> * Detailed automation reports on Requests and Responses.
+>> * Automation for SOAP protocol.
 >> * Data comparison for each Request.
->> * API Testing in pure CLI mode.
+>> * API automation in pure CLI mode.
 ---
-### Load & Stress Testing components
+### Load & Stress Automation components
 > Locust Wrapper \
 > Wrapper for Locust, simplifying complex Locust configurations. \
 > Solves problems:
 >> * Checking Requests & Response for each load test
->> * Load testing for SOAP protocols
+>> * Load automation for SOAP protocols
 >> * Comparison of numerical values for each load test
 >> * Detailed load test reports for each test.
 ---
 
 ### Features
 
 > * GUI Automation (use AutoControl)
 > * API Automation (use APITestka)
 > * Web Automation (use WebRunner)
 > * Loading Automation (use LoadDensity)
 > * Multi test task runner (multiprocess, but without AutoControl)
-> * you can run multi testing on same time
-> * open log window to check testing result
-> * Send mail when testing failure (need to setting mail)
+> * you can run multi automation on same time
+> * open log window to check automation result
+> * Send mail when automation failure (need to setting mail)
 
 ---
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b7d32ed8600b4bd2a2f3e960f46f2ad0)](https://www.codacy.com/gh/JE-Chen/Integration-testing-environment/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=JE-Chen/Integration-testing-environment&amp;utm_campaign=Badge_Grade)
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/Integrated-Testing-Environment/Integration-testing-environment/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Integrated-Testing-Environment/Integration-testing-environment/tree/main)
```

### Comparing `automation_editor-0.0.2/automation_editor.egg-info/SOURCES.txt` & `automation_editor-0.0.3/automation_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.2/pyproject.toml` & `automation_editor-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is stable version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "automation_editor"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "JE-Chen", email = "zenmailman@gmail.com" },
 ]
 description = "Automation Editor for GUI, WEB, API, Load Automation"
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.8"
 license = { text = "MIT" }
```

