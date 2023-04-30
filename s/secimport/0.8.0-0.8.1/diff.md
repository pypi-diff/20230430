# Comparing `tmp/secimport-0.8.0.tar.gz` & `tmp/secimport-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secimport-0.8.0.tar", max compression
+gzip compressed data, was "secimport-0.8.1.tar", max compression
```

## Comparing `secimport-0.8.0.tar` & `secimport-0.8.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1069 2023-04-29 23:45:38.801932 secimport-0.8.0/LICENSE
--rw-r--r--   0        0        0     8403 2023-04-29 23:45:38.801932 secimport-0.8.0/README.md
--rw-r--r--   0        0        0     1715 2023-04-29 23:45:38.805932 secimport-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      437 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/__init__.py
--rw-r--r--   0        0        0      362 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/actions/kill_on_processing.bt
--rw-r--r--   0        0        0      373 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/actions/kill_process.bt
--rw-r--r--   0        0        0      125 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/actions/log_file_system.bt
--rw-r--r--   0        0        0      110 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/actions/log_network.bt
--rw-r--r--   0        0        0       72 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/actions/log_python_module_entry.bt
--rw-r--r--   0        0        0       71 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/actions/log_python_module_exit.bt
--rw-r--r--   0        0        0      183 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/actions/log_syscall.bt
--rw-r--r--   0        0        0     8757 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/bpftrace_backend.py
--rw-r--r--   0        0        0    22157 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/default.template.bt
--rw-r--r--   0        0        0     1651 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/default.yaml.template.bt
--rw-r--r--   0        0        0       67 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/filters/file_system.bt
--rw-r--r--   0        0        0      176 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/filters/is_current_module_under_supervision.bt
--rw-r--r--   0        0        0       40 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/filters/networking.bt
--rw-r--r--   0        0        0      553 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/filters/processes.bt
--rwxr-xr-x   0        0        0    22668 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/generate_profile.bt
--rw-r--r--   0        0        0     1203 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/new_template.bt
--rw-r--r--   0        0        0      502 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/bpftrace_backend/probes/module_syscalls_allowlist_template.bt
--rw-r--r--   0        0        0        0 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/common/__init__.py
--rw-r--r--   0        0        0      112 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/common/instrumentation_backend.py
--rw-r--r--   0        0        0    14433 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/common/utils.py
--rw-r--r--   0        0        0        0 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/__init__.py
--rw-r--r--   0        0        0      415 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/actions/kill_on_processing.d
--rw-r--r--   0        0        0      662 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/actions/kill_process.d
--rw-r--r--   0        0        0      134 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/actions/log_file_system.d
--rw-r--r--   0        0        0      124 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/actions/log_network.d
--rw-r--r--   0        0        0      187 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/actions/log_python_module_entry.d
--rw-r--r--   0        0        0      188 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/actions/log_python_module_exit.d
--rw-r--r--   0        0        0       64 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/actions/log_syscall.d
--rwxr-xr-x   0        0        0     1606 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/default.allowlist.template.d
--rwxr-xr-x   0        0        0     1081 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/default.blocklist.template.d
--rwxr-xr-x   0        0        0     1753 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/default.template.d
--rwxr-xr-x   0        0        0     2587 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/default.yaml.template.d
--rw-r--r--   0        0        0     8813 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/dtrace_backend.py
--rw-r--r--   0        0        0      172 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/filters/file_system.d
--rw-r--r--   0        0        0      177 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/filters/is_current_module_under_supervision.d
--rw-r--r--   0        0        0       31 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/filters/networking.d
--rw-r--r--   0        0        0      436 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/filters/processes.d
--rw-r--r--   0        0        0      969 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/generate_profile.d
--rw-r--r--   0        0        0       30 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/headers/destructive.d
--rw-r--r--   0        0        0     1238 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d
--rwxr-xr-x   0        0        0     4389 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/backends/dtrace_backend/py_sandbox.d
--rw-r--r--   0        0        0    13379 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/cli.py
--rwxr-xr-x   0        0        0    22294 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/profiles/trace.bt
--rw-r--r--   0        0        0     3048 2023-04-29 23:45:38.805932 secimport-0.8.0/secimport/sandbox_helper.py
--rw-r--r--   0        0        0     9130 1970-01-01 00:00:00.000000 secimport-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-30 00:41:45.696550 secimport-0.8.1/LICENSE
+-rw-r--r--   0        0        0     8403 2023-04-30 00:41:45.696550 secimport-0.8.1/README.md
+-rw-r--r--   0        0        0     1715 2023-04-30 00:41:45.696550 secimport-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      437 2023-04-30 00:41:45.696550 secimport-0.8.1/secimport/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 00:41:45.696550 secimport-0.8.1/secimport/backends/bpftrace_backend/__init__.py
+-rw-r--r--   0        0        0      362 2023-04-30 00:41:45.696550 secimport-0.8.1/secimport/backends/bpftrace_backend/actions/kill_on_processing.bt
+-rw-r--r--   0        0        0      373 2023-04-30 00:41:45.696550 secimport-0.8.1/secimport/backends/bpftrace_backend/actions/kill_process.bt
+-rw-r--r--   0        0        0      125 2023-04-30 00:41:45.696550 secimport-0.8.1/secimport/backends/bpftrace_backend/actions/log_file_system.bt
+-rw-r--r--   0        0        0      110 2023-04-30 00:41:45.696550 secimport-0.8.1/secimport/backends/bpftrace_backend/actions/log_network.bt
+-rw-r--r--   0        0        0       72 2023-04-30 00:41:45.696550 secimport-0.8.1/secimport/backends/bpftrace_backend/actions/log_python_module_entry.bt
+-rw-r--r--   0        0        0       71 2023-04-30 00:41:45.696550 secimport-0.8.1/secimport/backends/bpftrace_backend/actions/log_python_module_exit.bt
+-rw-r--r--   0        0        0      183 2023-04-30 00:41:45.696550 secimport-0.8.1/secimport/backends/bpftrace_backend/actions/log_syscall.bt
+-rw-r--r--   0        0        0     8757 2023-04-30 00:41:45.696550 secimport-0.8.1/secimport/backends/bpftrace_backend/bpftrace_backend.py
+-rw-r--r--   0        0        0    22157 2023-04-30 00:41:45.696550 secimport-0.8.1/secimport/backends/bpftrace_backend/default.template.bt
+-rw-r--r--   0        0        0     1651 2023-04-30 00:41:45.696550 secimport-0.8.1/secimport/backends/bpftrace_backend/default.yaml.template.bt
+-rw-r--r--   0        0        0       67 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/bpftrace_backend/filters/file_system.bt
+-rw-r--r--   0        0        0      176 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/bpftrace_backend/filters/is_current_module_under_supervision.bt
+-rw-r--r--   0        0        0       40 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/bpftrace_backend/filters/networking.bt
+-rw-r--r--   0        0        0      553 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/bpftrace_backend/filters/processes.bt
+-rwxr-xr-x   0        0        0    22668 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/bpftrace_backend/generate_profile.bt
+-rw-r--r--   0        0        0     1203 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/bpftrace_backend/new_template.bt
+-rw-r--r--   0        0        0      502 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/bpftrace_backend/probes/module_syscalls_allowlist_template.bt
+-rw-r--r--   0        0        0        0 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/common/__init__.py
+-rw-r--r--   0        0        0      112 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/common/instrumentation_backend.py
+-rw-r--r--   0        0        0    18726 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/common/utils.py
+-rw-r--r--   0        0        0        0 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/__init__.py
+-rw-r--r--   0        0        0      415 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/actions/kill_on_processing.d
+-rw-r--r--   0        0        0      662 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/actions/kill_process.d
+-rw-r--r--   0        0        0      134 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/actions/log_file_system.d
+-rw-r--r--   0        0        0      124 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/actions/log_network.d
+-rw-r--r--   0        0        0      187 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/actions/log_python_module_entry.d
+-rw-r--r--   0        0        0      188 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/actions/log_python_module_exit.d
+-rw-r--r--   0        0        0       64 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/actions/log_syscall.d
+-rwxr-xr-x   0        0        0     1606 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/default.allowlist.template.d
+-rwxr-xr-x   0        0        0     1081 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/default.blocklist.template.d
+-rwxr-xr-x   0        0        0     1753 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/default.template.d
+-rwxr-xr-x   0        0        0     2587 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/default.yaml.template.d
+-rw-r--r--   0        0        0     8813 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/dtrace_backend.py
+-rw-r--r--   0        0        0      172 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/filters/file_system.d
+-rw-r--r--   0        0        0      177 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/filters/is_current_module_under_supervision.d
+-rw-r--r--   0        0        0       31 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/filters/networking.d
+-rw-r--r--   0        0        0      436 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/filters/processes.d
+-rw-r--r--   0        0        0      969 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/generate_profile.d
+-rw-r--r--   0        0        0       30 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/headers/destructive.d
+-rw-r--r--   0        0        0     1238 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d
+-rwxr-xr-x   0        0        0     4389 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/backends/dtrace_backend/py_sandbox.d
+-rw-r--r--   0        0        0    13379 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/cli.py
+-rwxr-xr-x   0        0        0    22294 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/profiles/trace.bt
+-rw-r--r--   0        0        0     3048 2023-04-30 00:41:45.700551 secimport-0.8.1/secimport/sandbox_helper.py
+-rw-r--r--   0        0        0     9130 1970-01-01 00:00:00.000000 secimport-0.8.1/PKG-INFO
```

### Comparing `secimport-0.8.0/LICENSE` & `secimport-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `secimport-0.8.0/README.md` & `secimport-0.8.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     EXAMPLES:
         1. trace:
             $  secimport trace
             $  secimport trace -h
             $  secimport trace_pid 123
             $  secimport trace_pid -h
         2. build:
-            # secimport build
+            $ secimport build
             $ secimport build -h
         3. run:
             $  secimport run
             $  secimport run --entrypoint my_custom_main.py
             $  secimport run --entrypoint my_custom_main.py --stop_on_violation=true
             $  secimport run --entrypoint my_custom_main.py --kill_on_violation=true
             $  secimport run --sandbox_executable /path/to/my_sandbox.bt --pid 2884
```

#### html2text {}

```diff
@@ -30,15 +30,15 @@
 secimport trace command. Once you have covered the logic you would like to
 sandbox, hit CTRL+C or CTRL+D, or wait for the program to finish. Then, build a
 sandbox from the trace using the secimport build command, and run the sandbox
 with the secimport run command. ```shell NAME SecImport - A toolkit for Tracing
 and Securing Python Runtime using USDT probes and eBPF/DTrace SYNOPSIS cli.py
 COMMAND DESCRIPTION QUICK START: >>> secimport interactive EXAMPLES: 1. trace:
 $ secimport trace $ secimport trace -h $ secimport trace_pid 123 $ secimport
-trace_pid -h 2. build: # secimport build $ secimport build -h 3. run: $
+trace_pid -h 2. build: $ secimport build $ secimport build -h 3. run: $
 secimport run $ secimport run --entrypoint my_custom_main.py $ secimport run --
 entrypoint my_custom_main.py --stop_on_violation=true $ secimport run --
 entrypoint my_custom_main.py --kill_on_violation=true $ secimport run --
 sandbox_executable /path/to/my_sandbox.bt --pid 2884 $ secimport run --
 sandbox_executable /path/to/my_sandbox.bt --sandbox_logfile my_log.log $
 secimport run -h COMMANDS COMMAND is one of the following: build interactive
 run Run a python process inside the sandbox. trace Traces trace_pid Traces a
```

### Comparing `secimport-0.8.0/pyproject.toml` & `secimport-0.8.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secimport"
-version = "0.8.0"
+version = "0.8.1"
 description = "A sandbox/supervisor for python modules."
 authors = ["Avi Lumelsky"]
 license = "MIT"
 homepage = "https://github.com/avilum/secimport"
 readme = "README.md"
 packages = [
     { include = "secimport" },
```

### Comparing `secimport-0.8.0/secimport/backends/bpftrace_backend/bpftrace_backend.py` & `secimport-0.8.1/secimport/backends/bpftrace_backend/bpftrace_backend.py`

 * *Files identical despite different names*

### Comparing `secimport-0.8.0/secimport/backends/bpftrace_backend/default.template.bt` & `secimport-0.8.1/secimport/backends/bpftrace_backend/default.template.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.8.0/secimport/backends/bpftrace_backend/default.yaml.template.bt` & `secimport-0.8.1/secimport/backends/bpftrace_backend/default.yaml.template.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.8.0/secimport/backends/bpftrace_backend/filters/processes.bt` & `secimport-0.8.1/secimport/backends/bpftrace_backend/filters/processes.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.8.0/secimport/backends/bpftrace_backend/generate_profile.bt` & `secimport-0.8.1/secimport/backends/bpftrace_backend/generate_profile.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.8.0/secimport/backends/bpftrace_backend/new_template.bt` & `secimport-0.8.1/secimport/backends/bpftrace_backend/new_template.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.8.0/secimport/backends/common/utils.py` & `secimport-0.8.1/secimport/backends/common/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -365,14 +365,251 @@
     332: "statx",
     333: "io_pgetevents",
     334: "rseq",
 }
 
 SYSCALLS_NAMES = {str(v): k for k, v in SYSCALLS_NUMBERS.items()}
 
+INSECURE_SYSCALLS = [
+    "vfork",
+    "clone",
+    "access",
+    "chdir",
+    "creat",
+    "dup",
+    "dup2",
+    "execve",
+    "faccessat",
+    "fcntl",
+    "fdatasync",
+    "fork",
+    "fstat",
+    "fsync",
+    "getegid",
+    "geteuid",
+    "getgid",
+    "getgroups",
+    "getpid",
+    "getppid",
+    "getrlimit",
+    "getsockname",
+    "getsid",
+    "getuid",
+    "ioctl",
+    "link",
+    "lseek",
+    "lstat",
+    "mkdir",
+    "mknod",
+    "open",
+    "openat",
+    "pipe",
+    "poll",
+    "read",
+    "readlink",
+    "readv",
+    "recvfrom",
+    "recvmsg",
+    "rename",
+    "rmdir",
+    "select",
+    "sendmsg",
+    "sendto",
+    "setgid",
+    "setgroups",
+    "setpgid",
+    "setpriority",
+    "setregid",
+    "setreuid",
+    "setrlimit",
+    "setsid",
+    "setsockopt",
+    "stat",
+    "symlink",
+    "truncate",
+    "umask",
+    "utime",
+    "utimes",
+    "write",
+    "writev",
+]
+
+# NETWORKING_SYSCALLS = [
+#     "socket",
+#     "connect",
+#     "bind",
+#     "listen",
+#     "accept",
+#     "send",
+#     "recv",
+#     "sendto",
+#     "recvfrom",
+#     "shutdown",
+#     "setsockopt",
+#     "getsockopt",
+#     "getpeername",
+#     "getsockname",
+#     "gethostbyname",
+#     "gethostbyaddr",
+#     "getservbyname",
+#     "getservbyport",
+#     "getifaddrs",
+#     "ioctl",
+#     "rt_names_to_index",
+#     "rt_index_to_name",
+#     "rt_newlink",
+#     "rt_dellink",
+#     "rt_changelink",
+#     "rt_getlink",
+#     "rt_getroute",
+#     "rt_newroute",
+#     "rt_delroute",
+#     "rt_changeroute",
+#     "rt_priority",
+#     "rt_classid",
+#     "rt_mark",
+#     "rt_table",
+#     "rt_protocol",
+#     "rt_scope",
+#     "rt_flags",
+#     "rt_ifindex",
+#     "rt_metric",
+#     "rt_gateway",
+#     "rt_src",
+#     "rt_dst",
+#     "rt_genmask",
+#     "rt_flags",
+#     "rt_refcnt",
+#     "rt_fib",
+#     "rt_nexthop",
+#     "rt_ifa",
+#     "rt_ifa_index",
+#     "rt_ifa_flags",
+#     "rt_ifa_scope",
+#     "rt_ifa_mntr",
+#     "rt_ifa_brd",
+#     "rt_ifa_dst",
+#     "rt_ifa_netmask",
+#     "rt_ifa_net",
+#     "rt_ifa_flags",
+#     "rt_ifa_ifindex",
+#     "rt_ifa_hwaddr",
+#     "rt_ifa_rtnl",
+#     "rt_ifa_type",
+#     "rt_ifa_metric",
+#     "rt_ifa_refcnt",
+#     "rt_ifa_mtu",
+#     "rt_ifa_lladdr",
+#     "rt_ifa_addr",
+#     "rt_ifa_brd",
+#     "rt_ifa_netmask",
+#     "rt_ifa_net",
+#     "rt_ifa_flags",
+#     "rt_ifa_ifindex",
+#     "rt_ifa_hwaddr",
+#     "rt_ifa_rtnl",
+#     "rt_ifa_type",
+#     "rt_ifa_metric",
+#     "rt_ifa_refcnt",
+#     "rt_ifa_mtu",
+#     "rt_ifa_lladdr",
+# ]
+# FILESYSTEM_SYSCALLS = [
+#     "access",
+#     "chdir",
+#     "chmod",
+#     "chown",
+#     "cksum",
+#     "creat",
+#     "ctermid",
+#     "dup",
+#     "dup2",
+#     "execve",
+#     "faccessat",
+#     "fchmod",
+#     "fchown",
+#     "fcntl",
+#     "fdatasync",
+#     "fdopendir",
+#     "fdopen",
+#     "fexecve",
+#     "fflush",
+#     "fgetpos",
+#     "fgets",
+#     "fgetwc",
+#     "fileno",
+#     "flock",
+#     "fmemopen",
+#     "fopen",
+#     "fopencookie",
+#     "fork",
+#     "fputwc",
+#     "fstat",
+#     "fsync",
+#     "ftruncate",
+#     "getegid",
+#     "geteuid",
+#     "getgid",
+#     "getgroups",
+#     "getpid",
+#     "getppid",
+#     "getrlimit",
+#     "getsockname",
+#     "getsid",
+#     "getuid",
+#     "ioctl",
+#     "link",
+#     "lseek",
+#     "lstat",
+#     "mkdir",
+#     "mknod",
+#     "open",
+#     "openat",
+#     "pipe",
+#     "poll",
+#     # "posix_fallocate",
+#     # "posix_fadvise",
+#     # "posix_fadvise64",
+#     "read",
+#     "readlink",
+#     # "readdir",
+#     "readv",
+#     "recv",
+#     "recvfrom",
+#     "recvmsg",
+#     "rename",
+#     "rewind",
+#     "rmdir",
+#     "seekdir",
+#     "select",
+#     "send",
+#     "sendmsg",
+#     "sendto",
+#     "setegid",
+#     "seteuid",
+#     "setgid",
+#     "setgroups",
+#     "setpgid",
+#     "setpriority",
+#     "setregid",
+#     "setreuid",
+#     "setrlimit",
+#     "setsid",
+#     "setsockopt",
+#     "stat",
+#     "symlink",
+#     "truncate",
+#     "umask",
+#     "umount",
+#     "utime",
+#     "utimes",
+#     "write",
+#     "writev",
+# ]
+
 
 def render_syscalls_filter(
     syscalls_list: List[str],
     allow: bool,
     instrumentation_backend: InstrumentationBackend,
     module_name=None,
 ):
@@ -446,14 +683,22 @@
         template_path
     ).exists(), f"The template does not exist at {template_path}"
     import yaml
 
     safe_yaml = yaml.safe_load(open(template_path, "r").read())
     parsed_probes = []
     syscalls_filter = ""
+    # Adding the general syscalls filter
+    syscalls_filter += render_syscalls_filter(
+        syscalls_list=INSECURE_SYSCALLS,
+        allow=False,
+        instrumentation_backend=InstrumentationBackend.EBPF,
+        module_name="general_requirements",
+    )
+
     for module_name, module_config in safe_yaml.get("modules", {}).items():
         # Finding the module without loading
         module = importlib.machinery.PathFinder().find_spec(module_name)
         if module is None:
             pass
             # raise ModuleNotFoundError(msg)
```

### Comparing `secimport-0.8.0/secimport/backends/dtrace_backend/actions/kill_process.d` & `secimport-0.8.1/secimport/backends/dtrace_backend/actions/kill_process.d`

 * *Files identical despite different names*

### Comparing `secimport-0.8.0/secimport/backends/dtrace_backend/default.allowlist.template.d` & `secimport-0.8.1/secimport/backends/dtrace_backend/default.allowlist.template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.8.0/secimport/backends/dtrace_backend/default.blocklist.template.d` & `secimport-0.8.1/secimport/backends/dtrace_backend/default.blocklist.template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.8.0/secimport/backends/dtrace_backend/default.template.d` & `secimport-0.8.1/secimport/backends/dtrace_backend/default.template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.8.0/secimport/backends/dtrace_backend/default.yaml.template.d` & `secimport-0.8.1/secimport/backends/dtrace_backend/default.yaml.template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.8.0/secimport/backends/dtrace_backend/dtrace_backend.py` & `secimport-0.8.1/secimport/backends/dtrace_backend/dtrace_backend.py`

 * *Files identical despite different names*

### Comparing `secimport-0.8.0/secimport/backends/dtrace_backend/generate_profile.d` & `secimport-0.8.1/secimport/backends/dtrace_backend/generate_profile.d`

 * *Files identical despite different names*

### Comparing `secimport-0.8.0/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d` & `secimport-0.8.1/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.8.0/secimport/backends/dtrace_backend/py_sandbox.d` & `secimport-0.8.1/secimport/backends/dtrace_backend/py_sandbox.d`

 * *Files identical despite different names*

### Comparing `secimport-0.8.0/secimport/cli.py` & `secimport-0.8.1/secimport/cli.py`

 * *Files identical despite different names*

### Comparing `secimport-0.8.0/secimport/profiles/trace.bt` & `secimport-0.8.1/secimport/profiles/trace.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.8.0/secimport/sandbox_helper.py` & `secimport-0.8.1/secimport/sandbox_helper.py`

 * *Files identical despite different names*

### Comparing `secimport-0.8.0/PKG-INFO` & `secimport-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secimport
-Version: 0.8.0
+Version: 0.8.1
 Summary: A sandbox/supervisor for python modules.
 Home-page: https://github.com/avilum/secimport
 License: MIT
 Author: Avi Lumelsky
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -79,15 +79,15 @@
     EXAMPLES:
         1. trace:
             $  secimport trace
             $  secimport trace -h
             $  secimport trace_pid 123
             $  secimport trace_pid -h
         2. build:
-            # secimport build
+            $ secimport build
             $ secimport build -h
         3. run:
             $  secimport run
             $  secimport run --entrypoint my_custom_main.py
             $  secimport run --entrypoint my_custom_main.py --stop_on_violation=true
             $  secimport run --entrypoint my_custom_main.py --kill_on_violation=true
             $  secimport run --sandbox_executable /path/to/my_sandbox.bt --pid 2884
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: secimport Version: 0.8.0 Summary: A sandbox/
+Metadata-Version: 2.1 Name: secimport Version: 0.8.1 Summary: A sandbox/
 supervisor for python modules. Home-page: https://github.com/avilum/secimport
 License: MIT Author: Avi Lumelsky Requires-Python: >=3.6,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -40,15 +40,15 @@
 secimport trace command. Once you have covered the logic you would like to
 sandbox, hit CTRL+C or CTRL+D, or wait for the program to finish. Then, build a
 sandbox from the trace using the secimport build command, and run the sandbox
 with the secimport run command. ```shell NAME SecImport - A toolkit for Tracing
 and Securing Python Runtime using USDT probes and eBPF/DTrace SYNOPSIS cli.py
 COMMAND DESCRIPTION QUICK START: >>> secimport interactive EXAMPLES: 1. trace:
 $ secimport trace $ secimport trace -h $ secimport trace_pid 123 $ secimport
-trace_pid -h 2. build: # secimport build $ secimport build -h 3. run: $
+trace_pid -h 2. build: $ secimport build $ secimport build -h 3. run: $
 secimport run $ secimport run --entrypoint my_custom_main.py $ secimport run --
 entrypoint my_custom_main.py --stop_on_violation=true $ secimport run --
 entrypoint my_custom_main.py --kill_on_violation=true $ secimport run --
 sandbox_executable /path/to/my_sandbox.bt --pid 2884 $ secimport run --
 sandbox_executable /path/to/my_sandbox.bt --sandbox_logfile my_log.log $
 secimport run -h COMMANDS COMMAND is one of the following: build interactive
 run Run a python process inside the sandbox. trace Traces trace_pid Traces a
```

