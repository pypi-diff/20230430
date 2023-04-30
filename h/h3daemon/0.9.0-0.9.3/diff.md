# Comparing `tmp/h3daemon-0.9.0.tar.gz` & `tmp/h3daemon-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h3daemon-0.9.0.tar", max compression
+gzip compressed data, was "h3daemon-0.9.3.tar", max compression
```

## Comparing `h3daemon-0.9.0.tar` & `h3daemon-0.9.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-01-20 16:57:29.608387 h3daemon-0.9.0/LICENSE
--rw-r--r--   0        0        0     2635 2023-02-24 01:54:22.628085 h3daemon-0.9.0/README.md
--rw-r--r--   0        0        0       50 2023-02-24 01:54:22.628579 h3daemon-0.9.0/h3daemon/__init__.py
--rw-r--r--   0        0        0     3310 2023-02-24 15:38:31.383660 h3daemon-0.9.0/h3daemon/app.py
--rw-r--r--   0        0        0     3287 2023-02-24 17:08:04.095954 h3daemon-0.9.0/h3daemon/cli.py
--rw-r--r--   0        0        0     1758 2023-02-24 17:03:21.336171 h3daemon-0.9.0/h3daemon/process.py
--rw-r--r--   0        0        0      457 2023-02-24 17:08:13.370663 h3daemon-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3501 1970-01-01 00:00:00.000000 h3daemon-0.9.0/setup.py
--rw-r--r--   0        0        0     3235 1970-01-01 00:00:00.000000 h3daemon-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-01-20 16:57:29.608387 h3daemon-0.9.3/LICENSE
+-rw-r--r--   0        0        0     2635 2023-02-24 01:54:22.628085 h3daemon-0.9.3/README.md
+-rw-r--r--   0        0        0        0 2023-02-27 14:52:06.440475 h3daemon-0.9.3/h3daemon/__init__.py
+-rw-r--r--   0        0        0     3674 2023-02-27 16:34:12.433531 h3daemon-0.9.3/h3daemon/app.py
+-rw-r--r--   0        0        0     3791 2023-02-27 16:26:37.599290 h3daemon-0.9.3/h3daemon/cli.py
+-rw-r--r--   0        0        0     1758 2023-02-24 17:35:56.245301 h3daemon-0.9.3/h3daemon/process.py
+-rw-r--r--   0        0        0      481 2023-02-27 16:42:42.250661 h3daemon-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     3525 1970-01-01 00:00:00.000000 h3daemon-0.9.3/setup.py
+-rw-r--r--   0        0        0     3270 1970-01-01 00:00:00.000000 h3daemon-0.9.3/PKG-INFO
```

### Comparing `h3daemon-0.9.0/LICENSE` & `h3daemon-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `h3daemon-0.9.0/README.md` & `h3daemon-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `h3daemon-0.9.0/h3daemon/app.py` & `h3daemon-0.9.3/h3daemon/app.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,61 @@
-import signal
 import socket
 import sys
 import time
 from contextlib import closing
 from functools import partial
 from pathlib import Path
-from subprocess import DEVNULL, Popen, check_output
+from subprocess import Popen
 from typing import Callable, Optional
 
 import hmmer
+import psutil
 
-__all__ = ["H3Daemon"]
+__all__ = ["app_setup", "app_main", "app_terminate"]
 
 
 def check_socket(cport: int):
     with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as sock:
         return sock.connect_ex(("127.0.0.1", cport)) == 0
 
 
-def is_master_ready(proc: Popen, cport: int, wport: int):
-    out = check_output(["lsof", "-p", str(proc.pid)], stderr=DEVNULL).decode()
-    cport_listen = False
-    wport_listen = False
-    for x in out.split("\n"):
-        if "TCP" in x and f":{cport}" in x and "LISTEN" in x:
-            cport_listen = True
-        if "TCP" in x and f":{wport}" in x and "LISTEN" in x:
-            wport_listen = True
-    return cport_listen and wport_listen and check_socket(cport) and proc.poll() is None
+def is_listening(pid: int, port: int):
+    try:
+        for x in psutil.Process(pid).connections(kind="tcp"):
+            if x.status == "LISTEN" and x.laddr.port == port:
+                return True
+    except RuntimeError:
+        # Bug to be fixed: https://github.com/giampaolo/psutil/issues/2116
+        time.sleep(0.2)
+        return True
+    return False
 
 
-def is_worker_ready(proc: Popen):
-    out = check_output(["lsof", "-p", str(proc.pid)], stderr=DEVNULL).decode()
-    for x in out.split("\n"):
-        if "TCP" in x and "ESTABLISHED" in x:
-            return proc.poll() is None
+def has_connected(pid: int):
+    try:
+        for x in psutil.Process(pid).connections(kind="tcp"):
+            if x.status == "ESTABLISHED":
+                return True
+    except RuntimeError:
+        # Bug to be fixed: https://github.com/giampaolo/psutil/issues/2116
+        time.sleep(0.2)
+        return True
     return False
 
 
+def is_master_ready(proc: Popen, cport: int):
+    return is_listening(proc.pid, cport) and check_socket(cport) and proc.poll() is None
+
+
+def is_worker_ready(proc: Popen):
+    return has_connected(proc.pid) and proc.poll() is None
+
+
 def wait_until_ready(check_ready: Callable[[], bool]):
-    for _ in range(5):
+    for _ in range(50):
         if check_ready():
             return True
         time.sleep(0.1)
     return False
 
 
 def spawn_master(cport: int, wport: int, hmm_file: str):
@@ -69,43 +81,52 @@
 def find_free_port():
     port = _find_free_port()
     while not (49152 <= port and port <= 65535):
         port = _find_free_port()
     return port
 
 
-class H3Daemon:
-    def __init__(self, port: int, hmm_file: str):
-        self._port = port
-        self._hmmfile = hmm_file
-        self._worker: Optional[Popen] = None
-        self._master: Optional[Popen] = None
-
-    def _interrupt_terminate(self, *_):
-        if self._worker:
-            self._worker.terminate()
-        if self._master:
-            self._master.terminate()
-
-    def run(self):
-        cport = find_free_port() if self._port == 0 else self._port
-        wport = find_free_port()
-
-        master = spawn_master(cport, wport, self._hmmfile)
-        if not wait_until_ready(partial(is_master_ready, master, cport, wport)):
-            master.terminate()
-            sys.exit(master.wait())
-
-        worker = spawn_worker(wport)
-        if not wait_until_ready(partial(is_worker_ready, worker)):
-            worker.terminate()
-            master.terminate()
-            sys.exit(worker.wait())
-
-        self._master = master
-        self._worker = worker
-
-        signal.signal(signal.SIGINT, self._interrupt_terminate)
-        signal.signal(signal.SIGTERM, self._interrupt_terminate)
-
-        self._master.wait()
-        self._worker.wait()
+client_port: int = -1
+worker_port: int = -1
+worker: Optional[Popen] = None
+master: Optional[Popen] = None
+
+
+def app_setup(port: int):
+    global client_port, worker_port
+    client_port = find_free_port() if port == 0 else port
+    worker_port = find_free_port()
+
+
+def app_main(hmmfile: str):
+    global client_port, worker_port
+    global worker, master
+
+    master = spawn_master(client_port, worker_port, hmmfile)
+    if not wait_until_ready(partial(is_master_ready, master, client_port)):
+        master.kill()
+        sys.exit(master.wait())
+
+    worker = spawn_worker(worker_port)
+    if not wait_until_ready(partial(is_worker_ready, worker)):
+        worker.kill()
+        master.kill()
+        sys.exit(worker.wait())
+
+    open("/Users/horta/code/h3daemon/ponto1.txt", "w").close()
+    procs = [psutil.Process(master.pid), psutil.Process(worker.pid)]
+    open("/Users/horta/code/h3daemon/ponto2.txt", "w").close()
+    while len(psutil.wait_procs(procs, timeout=1)[0]) == 0:
+        open("/Users/horta/code/h3daemon/ponto3.txt", "w").close()
+        pass
+    open("/Users/horta/code/h3daemon/ponto4.txt", "w").close()
+
+    for x in psutil.wait_procs(procs, timeout=3)[1]:
+        x.kill()
+
+
+def app_terminate(*_):
+    global worker, master
+    if worker:
+        worker.terminate()
+    if master:
+        master.terminate()
```

### Comparing `h3daemon-0.9.0/h3daemon/cli.py` & `h3daemon-0.9.3/h3daemon/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import sys
 from pathlib import Path
 from typing import Optional
 
 import psutil
 import typer
 from daemon import DaemonContext
-from daemon.pidfile import PIDLockFile
+from pidlockfile import PIDLockFile
 from typer import echo
 
-from h3daemon import H3Daemon
+from h3daemon.app import app_setup, app_terminate, app_main
 from h3daemon.process import wait_for_port
 
 __all__ = ["app"]
 
 
 app = typer.Typer(
     add_completion=False,
@@ -47,82 +47,99 @@
     stdin: Optional[Path] = O_STDIN,
     stdout: Optional[Path] = O_STDOUT,
     stderr: Optional[Path] = O_STDERR,
 ):
     """
     Start daemon.
     """
+    hmmfile = hmmfile.absolute()
+
     if not hmmfile.name.endswith(".hmm"):
         raise ValueError(f"`{hmmfile}` does not end with `.hmm`.")
 
     if not hmmfile.exists():
         raise ValueError(f"`{hmmfile}` does not exist.")
 
     extensions = ["h3f", "h3i", "h3m", "h3p"]
     for x in extensions:
         filename = Path(f"{hmmfile}.{x}")
         if not filename.exists():
             raise ValueError(f"`{filename.name}` must exist as well.")
 
     workdir = str(hmmfile.parent)
-    pidfile = PIDLockFile(hmmfile.name + ".pid")
+    pidfile = PIDLockFile(f"{hmmfile}.pid", timeout=5)
     ctx = DaemonContext(working_directory=workdir, pidfile=pidfile)
     ctx.stdin = open(stdin, "r") if stdin else stdin
     ctx.stdout = open(stdout, "w+") if stdout else stdout
     ctx.stderr = open(stderr, "w+") if stderr else stderr
+    ctx.signal_map = {signal.SIGTERM: app_terminate, signal.SIGINT: app_terminate}
+    app_setup(port)
     with ctx:
-        daemon = H3Daemon(port, hmmfile.name)
-        daemon.run()
+        app_main(str(hmmfile))
 
 
 @app.command()
 def stop(hmmfile: Optional[Path] = typer.Argument(None), all: bool = O_ALL):
     """
     Stop daemon.
     """
     if all:
         stop_all()
         return
 
     assert hmmfile
+    hmmfile = hmmfile.absolute()
+
     if not hmmfile.name.endswith(".hmm"):
         raise ValueError(f"`{hmmfile}` does not end with `.hmm`.")
 
     if not hmmfile.exists():
         raise ValueError(f"`{hmmfile}` does not exist.")
 
-    os.kill(read_pidfile(str(hmmfile) + ".pid"), signal.SIGTERM)
+    pidfile = PIDLockFile(f"{hmmfile}.pid", timeout=5)
+    pid = pidfile.is_locked()
+    if pid:
+        os.kill(pid, signal.SIGTERM)
+    else:
+        echo(f"{hmmfile}: NOT running")
 
 
 @app.command()
-def port(hmmfile: Optional[Path] = typer.Argument(None)):
+def port(hmmfile: Path):
     """
     Get port or fail.
     """
-    pid = int(read_pidfile(str(hmmfile) + ".pid"))
-    port = wait_for_port(pid)
-    if port == -1:
-        raise typer.Exit(1)
-    echo(f"{port}")
+    hmmfile = hmmfile.absolute()
+
+    if not hmmfile.name.endswith(".hmm"):
+        raise ValueError(f"`{hmmfile}` does not end with `.hmm`.")
+
+    if not hmmfile.exists():
+        raise ValueError(f"`{hmmfile}` does not exist.")
+
+    pidfile = PIDLockFile(f"{hmmfile}.pid", timeout=5)
+    pid = pidfile.is_locked()
+    if pid:
+        port = wait_for_port(pid)
+        if port == -1:
+            raise typer.Exit(1)
+        echo(f"{port}")
 
 
 def stop_all():
     pid = os.getpid()
     exe = sys.argv[0]
     uid = os.getuid()
 
     found = True
     while found:
         found = False
         for proc in psutil.process_iter(["pid", "cmdline", "uids"]):
             if proc.uids().real != uid or proc.pid == pid:
                 continue
+            if proc.status() == "zombie":
+                continue
             cmdline = proc.cmdline()
             if len(cmdline) > 1 and cmdline[1] == exe:
                 proc.terminate()
                 found = True
                 break
-
-
-def read_pidfile(pidfile):
-    with open(pidfile, "r") as file:
-        return int(file.readline().strip())
```

### Comparing `h3daemon-0.9.0/h3daemon/process.py` & `h3daemon-0.9.3/h3daemon/process.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,13 +47,13 @@
     master_ports.remove(worker_rport[0])
     assert len(master_ports) == 1
     return int(list(master_ports)[0])
 
 
 def wait_for_port(pid: int) -> int:
     proc = psutil.Process(pid)
-    for _ in range(10):
+    for _ in range(50):
         try:
             return _get_port(proc)
         except AssertionError:
             time.sleep(0.1)
     return -1
```

### Comparing `h3daemon-0.9.0/setup.py` & `h3daemon-0.9.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 packages = \
 ['h3daemon']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['hmmer>=0.2.1', 'psutil>=5.9.4', 'python-daemon>=2.3.2', 'typer[all]>=0.7.0']
+['hmmer>=0.2.1',
+ 'pidlockfile>=0.3',
+ 'psutil>=5.9.4',
+ 'python-daemon>=2.3.2',
+ 'typer[all]>=0.7.0']
 
 entry_points = \
 {'console_scripts': ['h3daemon = h3daemon.cli:app']}
 
 setup_kwargs = {
     'name': 'h3daemon',
-    'version': '0.9.0',
+    'version': '0.9.3',
     'description': 'HMMER server',
     'long_description': '# Welcome to h3daemon 👋\n\n> Command-line for running HMMER server on arm64 and amd64 machines.\n\n### 🏠 [Homepage](https://github.com/EBI-Metagenomics/h3daemon)\n\n## ⚡️ Requirements\n\n- Python >= 3.9\n- Pip\n- [Homebrew](https://brew.sh) on MacOS (recommended)\n- [Pipx](https://pypa.github.io/pipx/) for Python package management (recommended)\n\n### MacOS\n\nInstall Python and Pipx:\n\n```sh\nbrew update && brew install python pipx\n```\n\nEnsure that your `PATH` environment variable is all set:\n\n```sh\npipx ensurepath\n```\n\n💡 You might need to close your terminal and reopen it for the changes to take effect.\n\n### Ubuntu (and Debian-based distros)\n\nInstall Python and Pipx:\n\n```sh\nsudo apt update && \\\n    sudo apt install python3 python3-pip python3-venv --yes && \\\n    python3 -m pip install --user pipx\n```\n\nEnsure that your `PATH` environment variable is all set:\n\n```sh\npython3 -m pipx ensurepath\n```\n\n💡 You might need to close your terminal and reopen it for the changes to take effect.\n\n## 📦 Install\n\n```sh\npipx install h3daemon\n```\n\n## Usage\n\n```\n Usage: h3daemon [OPTIONS] COMMAND [ARGS]...\n\n╭─ Options ─────────────────────────────────────────────────────╮\n│ --version                                                     │\n│ --help             Show this message and exit.                │\n╰───────────────────────────────────────────────────────────────╯\n╭─ Commands ────────────────────────────────────────────────────╮\n│ start                 Start daemon.                           │\n│ stop                  Stop daemon.                            │\n╰───────────────────────────────────────────────────────────────╯\n```\n\n### Example\n\nDownload `minifam.hmm` database:\n\n```sh\npipx run blx get \\\n  fe305d9c09e123f987f49b9056e34c374e085d8831f815cc73d8ea4cdec84960 \\\n  minifam.hmm\n```\n\nPress it:\n\n```sh\npipx run --spec hmmer hmmpress minifam.hmm\n```\n\nStart the daemon to listen on a random (available) port:\n\n```sh\nh3daemon start minifam.hmm\n```\n\nAnd stop it:\n\n```sh\nh3daemon stop minifam.hmm\n```\n\n## 👤 Author\n\n- [Danilo Horta](https://github.com/horta)\n\n## Show your support\n\nGive a ⭐️ if this project helped you!\n',
     'author': 'Danilo Horta',
     'author_email': 'danilo.horta@pm.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `h3daemon-0.9.0/PKG-INFO` & `h3daemon-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: h3daemon
-Version: 0.9.0
+Version: 0.9.3
 Summary: HMMER server
 License: MIT
 Author: Danilo Horta
 Author-email: danilo.horta@pm.me
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: hmmer (>=0.2.1)
+Requires-Dist: pidlockfile (>=0.3)
 Requires-Dist: psutil (>=5.9.4)
 Requires-Dist: python-daemon (>=2.3.2)
 Requires-Dist: typer[all] (>=0.7.0)
 Description-Content-Type: text/markdown
 
 # Welcome to h3daemon 👋
```

