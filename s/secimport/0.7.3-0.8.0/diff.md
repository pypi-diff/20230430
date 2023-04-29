# Comparing `tmp/secimport-0.7.3.tar.gz` & `tmp/secimport-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secimport-0.7.3.tar", max compression
+gzip compressed data, was "secimport-0.8.0.tar", max compression
```

## Comparing `secimport-0.7.3.tar` & `secimport-0.8.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1069 2023-04-09 23:14:32.882650 secimport-0.7.3/LICENSE
--rw-r--r--   0        0        0     4590 2023-04-09 23:14:32.882650 secimport-0.7.3/README.md
--rw-r--r--   0        0        0     1715 2023-04-09 23:14:32.882650 secimport-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      437 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/__init__.py
--rw-r--r--   0        0        0      362 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/actions/kill_on_processing.bt
--rw-r--r--   0        0        0      373 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/actions/kill_process.bt
--rw-r--r--   0        0        0      125 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/actions/log_file_system.bt
--rw-r--r--   0        0        0      110 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/actions/log_network.bt
--rw-r--r--   0        0        0       72 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/actions/log_python_module_entry.bt
--rw-r--r--   0        0        0       71 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/actions/log_python_module_exit.bt
--rw-r--r--   0        0        0      183 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/actions/log_syscall.bt
--rw-r--r--   0        0        0     8757 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/bpftrace_backend.py
--rw-r--r--   0        0        0    22157 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/default.template.bt
--rw-r--r--   0        0        0     1653 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/default.yaml.template.bt
--rw-r--r--   0        0        0       67 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/filters/file_system.bt
--rw-r--r--   0        0        0      176 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/filters/is_current_module_under_supervision.bt
--rw-r--r--   0        0        0       40 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/filters/networking.bt
--rw-r--r--   0        0        0      553 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/filters/processes.bt
--rwxr-xr-x   0        0        0    22668 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/generate_profile.bt
--rw-r--r--   0        0        0     1203 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/new_template.bt
--rw-r--r--   0        0        0      502 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/bpftrace_backend/probes/module_syscalls_allowlist_template.bt
--rw-r--r--   0        0        0        0 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/common/__init__.py
--rw-r--r--   0        0        0      112 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/common/instrumentation_backend.py
--rw-r--r--   0        0        0    14433 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/common/utils.py
--rw-r--r--   0        0        0        0 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/__init__.py
--rw-r--r--   0        0        0      415 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/actions/kill_on_processing.d
--rw-r--r--   0        0        0      662 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/actions/kill_process.d
--rw-r--r--   0        0        0      134 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/actions/log_file_system.d
--rw-r--r--   0        0        0      124 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/actions/log_network.d
--rw-r--r--   0        0        0      187 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/actions/log_python_module_entry.d
--rw-r--r--   0        0        0      188 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/actions/log_python_module_exit.d
--rw-r--r--   0        0        0       64 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/actions/log_syscall.d
--rwxr-xr-x   0        0        0     1606 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/default.allowlist.template.d
--rwxr-xr-x   0        0        0     1081 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/default.blocklist.template.d
--rwxr-xr-x   0        0        0     1753 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/default.template.d
--rwxr-xr-x   0        0        0     2587 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/default.yaml.template.d
--rw-r--r--   0        0        0     8813 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/dtrace_backend.py
--rw-r--r--   0        0        0      172 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/filters/file_system.d
--rw-r--r--   0        0        0      177 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/filters/is_current_module_under_supervision.d
--rw-r--r--   0        0        0       31 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/filters/networking.d
--rw-r--r--   0        0        0      436 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/filters/processes.d
--rw-r--r--   0        0        0      969 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/generate_profile.d
--rw-r--r--   0        0        0       30 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/headers/destructive.d
--rw-r--r--   0        0        0     1238 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d
--rwxr-xr-x   0        0        0     4389 2023-04-09 23:14:32.882650 secimport-0.7.3/secimport/backends/dtrace_backend/py_sandbox.d
--rw-r--r--   0        0        0    13365 2023-04-09 23:14:32.886650 secimport-0.7.3/secimport/cli.py
--rwxr-xr-x   0        0        0    22294 2023-04-09 23:14:32.886650 secimport-0.7.3/secimport/profiles/trace.bt
--rw-r--r--   0        0        0     3048 2023-04-09 23:14:32.886650 secimport-0.7.3/secimport/sandbox_helper.py
--rw-r--r--   0        0        0     5317 1970-01-01 00:00:00.000000 secimport-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-29 23:45:38.801932 secimport-0.8.0/LICENSE
+-rw-r--r--   0        0        0     8403 2023-04-29 23:45:38.801932 secimport-0.8.0/README.md
+-rw-r--r--   0        0        0     1715 2023-04-29 23:45:38.805932 secimport-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      437 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/__init__.py
+-rw-r--r--   0        0        0      362 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/actions/kill_on_processing.bt
+-rw-r--r--   0        0        0      373 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/actions/kill_process.bt
+-rw-r--r--   0        0        0      125 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/actions/log_file_system.bt
+-rw-r--r--   0        0        0      110 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/actions/log_network.bt
+-rw-r--r--   0        0        0       72 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/actions/log_python_module_entry.bt
+-rw-r--r--   0        0        0       71 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/actions/log_python_module_exit.bt
+-rw-r--r--   0        0        0      183 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/actions/log_syscall.bt
+-rw-r--r--   0        0        0     8757 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/bpftrace_backend.py
+-rw-r--r--   0        0        0    22157 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/default.template.bt
+-rw-r--r--   0        0        0     1651 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/default.yaml.template.bt
+-rw-r--r--   0        0        0       67 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/filters/file_system.bt
+-rw-r--r--   0        0        0      176 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/filters/is_current_module_under_supervision.bt
+-rw-r--r--   0        0        0       40 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/filters/networking.bt
+-rw-r--r--   0        0        0      553 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/filters/processes.bt
+-rwxr-xr-x   0        0        0    22668 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/generate_profile.bt
+-rw-r--r--   0        0        0     1203 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/new_template.bt
+-rw-r--r--   0        0        0      502 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/probes/module_syscalls_allowlist_template.bt
+-rw-r--r--   0        0        0        0 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/common/__init__.py
+-rw-r--r--   0        0        0      112 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/common/instrumentation_backend.py
+-rw-r--r--   0        0        0    14433 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/common/utils.py
+-rw-r--r--   0        0        0        0 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/__init__.py
+-rw-r--r--   0        0        0      415 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/actions/kill_on_processing.d
+-rw-r--r--   0        0        0      662 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/actions/kill_process.d
+-rw-r--r--   0        0        0      134 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/actions/log_file_system.d
+-rw-r--r--   0        0        0      124 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/actions/log_network.d
+-rw-r--r--   0        0        0      187 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/actions/log_python_module_entry.d
+-rw-r--r--   0        0        0      188 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/actions/log_python_module_exit.d
+-rw-r--r--   0        0        0       64 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/actions/log_syscall.d
+-rwxr-xr-x   0        0        0     1606 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/default.allowlist.template.d
+-rwxr-xr-x   0        0        0     1081 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/default.blocklist.template.d
+-rwxr-xr-x   0        0        0     1753 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/default.template.d
+-rwxr-xr-x   0        0        0     2587 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/default.yaml.template.d
+-rw-r--r--   0        0        0     8813 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/dtrace_backend.py
+-rw-r--r--   0        0        0      172 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/filters/file_system.d
+-rw-r--r--   0        0        0      177 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/filters/is_current_module_under_supervision.d
+-rw-r--r--   0        0        0       31 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/filters/networking.d
+-rw-r--r--   0        0        0      436 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/filters/processes.d
+-rw-r--r--   0        0        0      969 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/generate_profile.d
+-rw-r--r--   0        0        0       30 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/headers/destructive.d
+-rw-r--r--   0        0        0     1238 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d
+-rwxr-xr-x   0        0        0     4389 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/py_sandbox.d
+-rw-r--r--   0        0        0    13379 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/cli.py
+-rwxr-xr-x   0        0        0    22294 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/profiles/trace.bt
+-rw-r--r--   0        0        0     3048 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/sandbox_helper.py
+-rw-r--r--   0        0        0     9130 1970-01-01 00:00:00.000000 secimport-0.8.0/PKG-INFO
```

### Comparing `secimport-0.7.3/LICENSE` & `secimport-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `secimport-0.7.3/pyproject.toml` & `secimport-0.8.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secimport"
-version = "0.7.3"
+version = "0.8.0"
 description = "A sandbox/supervisor for python modules."
 authors = ["Avi Lumelsky"]
 license = "MIT"
 homepage = "https://github.com/avilum/secimport"
 readme = "README.md"
 packages = [
     { include = "secimport" },
```

### Comparing `secimport-0.7.3/secimport/backends/bpftrace_backend/bpftrace_backend.py` & `secimport-0.8.0/secimport/backends/bpftrace_backend/bpftrace_backend.py`

 * *Files identical despite different names*

### Comparing `secimport-0.7.3/secimport/backends/bpftrace_backend/default.template.bt` & `secimport-0.8.0/secimport/backends/bpftrace_backend/default.template.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.7.3/secimport/backends/bpftrace_backend/default.yaml.template.bt` & `secimport-0.8.0/secimport/backends/bpftrace_backend/default.yaml.template.bt`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         signal("SIGSTOP");
         printf("\t\tPROCESS %d STOPPED.\r\n", pid);
     }
     else if (str($1) == "KILL") {
         printf("\n^^^ KILLING PROCESS %d DUE TO SYSCALL VIOLATION ^^^\n", pid);
         signal("SIGKILL");
         printf("\t\tKILLED.\r\n");
-        exit(); // optional
+        exit(); // option
     }
 }
 
 
 // Invoked before importlib imports a module
 // import__find__load__start(str modulename)
 // usdt:###INTERPRETER_PATH###:import__find__load__start {
```

### Comparing `secimport-0.7.3/secimport/backends/bpftrace_backend/filters/processes.bt` & `secimport-0.8.0/secimport/backends/bpftrace_backend/filters/processes.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.7.3/secimport/backends/bpftrace_backend/generate_profile.bt` & `secimport-0.8.0/secimport/backends/bpftrace_backend/generate_profile.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.7.3/secimport/backends/bpftrace_backend/new_template.bt` & `secimport-0.8.0/secimport/backends/bpftrace_backend/new_template.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.7.3/secimport/backends/common/utils.py` & `secimport-0.8.0/secimport/backends/common/utils.py`

 * *Files identical despite different names*

### Comparing `secimport-0.7.3/secimport/backends/dtrace_backend/actions/kill_process.d` & `secimport-0.8.0/secimport/backends/dtrace_backend/actions/kill_process.d`

 * *Files identical despite different names*

### Comparing `secimport-0.7.3/secimport/backends/dtrace_backend/default.allowlist.template.d` & `secimport-0.8.0/secimport/backends/dtrace_backend/default.allowlist.template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.7.3/secimport/backends/dtrace_backend/default.blocklist.template.d` & `secimport-0.8.0/secimport/backends/dtrace_backend/default.blocklist.template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.7.3/secimport/backends/dtrace_backend/default.template.d` & `secimport-0.8.0/secimport/backends/dtrace_backend/default.template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.7.3/secimport/backends/dtrace_backend/default.yaml.template.d` & `secimport-0.8.0/secimport/backends/dtrace_backend/default.yaml.template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.7.3/secimport/backends/dtrace_backend/dtrace_backend.py` & `secimport-0.8.0/secimport/backends/dtrace_backend/dtrace_backend.py`

 * *Files identical despite different names*

### Comparing `secimport-0.7.3/secimport/backends/dtrace_backend/generate_profile.d` & `secimport-0.8.0/secimport/backends/dtrace_backend/generate_profile.d`

 * *Files identical despite different names*

### Comparing `secimport-0.7.3/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d` & `secimport-0.8.0/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.7.3/secimport/backends/dtrace_backend/py_sandbox.d` & `secimport-0.8.0/secimport/backends/dtrace_backend/py_sandbox.d`

 * *Files identical despite different names*

### Comparing `secimport-0.7.3/secimport/cli.py` & `secimport-0.8.0/secimport/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,28 +297,28 @@
 
     @staticmethod
     def interactive():
         colored_print(
             COLORS.OKBLUE,
             "\nLet's create our first tailor-made sandbox with secimport!\n- A python shell will be opened\n- The behavior will be recorded.\n",
         )
-        start = input("OK? (y): ")
+        start = input("OK? (y): ") or "y"
         if start.lower() == "y":
             try:
                 SecImportCLI.trace()
             except KeyboardInterrupt:
                 ...
 
             SecImportCLI.build()
 
             colored_print(
                 COLORS.OKBLUE,
                 '\nNow, let\'s run the sandbox.\n- Run the same commands as before, they should run without any problem;.\n- Do something new in the shell; e.g:\t>>> __import__("os").system("ps")',
             )
-            run = input("\n\tOK? (y): ")
+            run = input("\n\tOK? (y): ") or "y"
 
             if run.lower() == "y":
                 SecImportCLI.run()
         else:
             colored_print(
                 COLORS.OKBLUE,
                 run,
```

### Comparing `secimport-0.7.3/secimport/profiles/trace.bt` & `secimport-0.8.0/secimport/profiles/trace.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.7.3/secimport/sandbox_helper.py` & `secimport-0.8.0/secimport/sandbox_helper.py`

 * *Files identical despite different names*

