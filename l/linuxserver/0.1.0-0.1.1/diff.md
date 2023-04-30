# Comparing `tmp/linuxserver-0.1.0.tar.gz` & `tmp/linuxserver-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linuxserver-0.1.0.tar", last modified: Sun Aug 14 16:44:26 2022, max compression
+gzip compressed data, was "linuxserver-0.1.1.tar", last modified: Sun Apr 30 14:44:49 2023, max compression
```

## Comparing `linuxserver-0.1.0.tar` & `linuxserver-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 16:44:26.469889 linuxserver-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-08-14 16:44:19.000000 linuxserver-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2436 2022-08-14 16:44:26.469889 linuxserver-0.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 16:44:26.465889 linuxserver-0.1.0/linuxserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2436 2022-08-14 16:44:26.000000 linuxserver-0.1.0/linuxserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-08-14 16:44:26.000000 linuxserver-0.1.0/linuxserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-14 16:44:26.000000 linuxserver-0.1.0/linuxserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-08-14 16:44:26.000000 linuxserver-0.1.0/linuxserver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-14 16:44:26.000000 linuxserver-0.1.0/linuxserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-14 16:44:26.000000 linuxserver-0.1.0/linuxserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-14 16:44:26.469889 linuxserver-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-08-14 16:44:19.000000 linuxserver-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 16:44:26.465889 linuxserver-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 16:44:26.469889 linuxserver-0.1.0/src/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-14 16:44:19.000000 linuxserver-0.1.0/src/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2649 2022-08-14 16:44:19.000000 linuxserver-0.1.0/src/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2710 2022-08-14 16:44:19.000000 linuxserver-0.1.0/src/cli/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 16:44:26.469889 linuxserver-0.1.0/src/cli/docker/
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-08-14 16:44:19.000000 linuxserver-0.1.0/src/cli/docker/deluge-compose.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-08-14 16:44:19.000000 linuxserver-0.1.0/src/cli/docker/gluetun-compose.yml
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-08-14 16:44:19.000000 linuxserver-0.1.0/src/cli/docker/jackett-compose.yml
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-08-14 16:44:19.000000 linuxserver-0.1.0/src/cli/docker/plex-compose.yml
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-08-14 16:44:19.000000 linuxserver-0.1.0/src/cli/docker/radarr-compose.yml
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-08-14 16:44:19.000000 linuxserver-0.1.0/src/cli/docker/sonarr-compose.yml
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-14 16:44:19.000000 linuxserver-0.1.0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:44:49.122911 linuxserver-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-30 14:44:39.000000 linuxserver-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-30 14:44:49.122911 linuxserver-0.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:44:49.122911 linuxserver-0.1.1/linuxserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-30 14:44:48.000000 linuxserver-0.1.1/linuxserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-30 14:44:49.000000 linuxserver-0.1.1/linuxserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 14:44:48.000000 linuxserver-0.1.1/linuxserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-30 14:44:48.000000 linuxserver-0.1.1/linuxserver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-30 14:44:48.000000 linuxserver-0.1.1/linuxserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-30 14:44:48.000000 linuxserver-0.1.1/linuxserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 14:44:49.122911 linuxserver-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-30 14:44:39.000000 linuxserver-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:44:49.122911 linuxserver-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:44:49.122911 linuxserver-0.1.1/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 14:44:39.000000 linuxserver-0.1.1/src/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-30 14:44:39.000000 linuxserver-0.1.1/src/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-30 14:44:39.000000 linuxserver-0.1.1/src/cli/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:44:49.122911 linuxserver-0.1.1/src/cli/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-30 14:44:39.000000 linuxserver-0.1.1/src/cli/docker/deluge-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-30 14:44:39.000000 linuxserver-0.1.1/src/cli/docker/gluetun-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-30 14:44:39.000000 linuxserver-0.1.1/src/cli/docker/heimdall-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-30 14:44:39.000000 linuxserver-0.1.1/src/cli/docker/jackett-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-30 14:44:39.000000 linuxserver-0.1.1/src/cli/docker/plex-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-30 14:44:39.000000 linuxserver-0.1.1/src/cli/docker/radarr-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-30 14:44:39.000000 linuxserver-0.1.1/src/cli/docker/sonarr-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-30 14:44:39.000000 linuxserver-0.1.1/version.py
```

### Comparing `linuxserver-0.1.0/LICENSE` & `linuxserver-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `linuxserver-0.1.0/PKG-INFO` & `linuxserver-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxserver
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple CLI to deploy linuxserver services
 Home-page: https://github.com/foprel/linuxserver
 Author: Frank Oprel
 Author-email: fj.oprel@gmail.com
 License: Copyright (c) 2012-2022 Scott Chacon and others
 
 Permission is hereby granted, free of charge, to any person obtaining
@@ -24,22 +24,23 @@
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Description: # linuxserver
         
         ## About
-        linuxserver is a simple command-line interface that enables you to easily install a complete home media server onto your machine. It uses open-source images from linuxserver.io and deploys them to Docker. The following services are supported:
+        linuxserver is a simple command-line interface that enables you to easily install a complete home media server onto your machine. It uses open-source images from [linuxserver.io](https://www.linuxserver.io/) and deploys them to Docker. The following services are supported:
         
         - [Deluge](https://deluge-torrent.org/)
         - [Gluetun](https://github.com/qdm12/gluetun)
         - [Jackett](https://github.com/Jackett/Jackett)
         - [Plex](https://www.plex.tv/)
         - [Radarr](https://radarr.video/)
         - [Sonarr](https://sonarr.video/)
+        - [Heimdall](https://heimdall.site/)
         
         ## Requirements
         - Python
         - Docker
         
         ## Installation
         Please follow these steps to install Linux Server CLI:
@@ -53,12 +54,16 @@
         ```shell
         linuxserver -v
         ```
         
         ## Usage
         Please follow these steps to use Linux Server CLI
         
+        ```shell
+        linuxserver deploy gluetun deluge heimdall jackett sonarr radarr plex
+        ```
+        
         
         
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `linuxserver-0.1.0/linuxserver.egg-info/PKG-INFO` & `linuxserver-0.1.1/linuxserver.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxserver
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple CLI to deploy linuxserver services
 Home-page: https://github.com/foprel/linuxserver
 Author: Frank Oprel
 Author-email: fj.oprel@gmail.com
 License: Copyright (c) 2012-2022 Scott Chacon and others
 
 Permission is hereby granted, free of charge, to any person obtaining
@@ -24,22 +24,23 @@
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Description: # linuxserver
         
         ## About
-        linuxserver is a simple command-line interface that enables you to easily install a complete home media server onto your machine. It uses open-source images from linuxserver.io and deploys them to Docker. The following services are supported:
+        linuxserver is a simple command-line interface that enables you to easily install a complete home media server onto your machine. It uses open-source images from [linuxserver.io](https://www.linuxserver.io/) and deploys them to Docker. The following services are supported:
         
         - [Deluge](https://deluge-torrent.org/)
         - [Gluetun](https://github.com/qdm12/gluetun)
         - [Jackett](https://github.com/Jackett/Jackett)
         - [Plex](https://www.plex.tv/)
         - [Radarr](https://radarr.video/)
         - [Sonarr](https://sonarr.video/)
+        - [Heimdall](https://heimdall.site/)
         
         ## Requirements
         - Python
         - Docker
         
         ## Installation
         Please follow these steps to install Linux Server CLI:
@@ -53,12 +54,16 @@
         ```shell
         linuxserver -v
         ```
         
         ## Usage
         Please follow these steps to use Linux Server CLI
         
+        ```shell
+        linuxserver deploy gluetun deluge heimdall jackett sonarr radarr plex
+        ```
+        
         
         
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `linuxserver-0.1.0/setup.py` & `linuxserver-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `linuxserver-0.1.0/src/cli/cli.py` & `linuxserver-0.1.1/src/cli/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,19 +6,14 @@
 import subprocess
 
 
 SYSTEM = config.system
 SERVICES = config.services.keys()
 PATHS = config.paths
 ROOT = os.path.dirname(__file__)
-DOWNLOADS = PATHS[SYSTEM]['downloads']
-MOVIES = PATHS[SYSTEM]['movies']
-SERIES = PATHS[SYSTEM]['series']
-DOCKER = PATHS[SYSTEM]['docker']
-CONFIG = PATHS[SYSTEM]['docker']
 
 
 def main():
 
     parser = argparse.ArgumentParser()
     parser.add_argument(
         '-v',
@@ -26,19 +21,14 @@
         action='version',
         version=__version__
     )
     subparsers = parser.add_subparsers()
 
     deploy = subparsers.add_parser('deploy')
     deploy.add_argument('services', nargs='+', choices=SERVICES)
-    deploy.add_argument('--downloads-path', type=str, default=DOWNLOADS)
-    deploy.add_argument('--movies-path', type=str, default=MOVIES)
-    deploy.add_argument('--series-path', type=str, default=SERIES)
-    deploy.add_argument('--docker-path', type=str, default=DOCKER)
-    deploy.add_argument('--config-path', type=str, default=CONFIG)
 
     args = parser.parse_args()
 
     for service in args.services:
 
         # Get service paths
         service_paths = config.services[service]['paths']
@@ -81,19 +71,29 @@
     with open(src, 'r') as source, open(dst, 'w+') as destination:
         template = Template(source.read())
         render = template.render(config.services[service]['paths'])
         destination.write(render)
 
 
 def run_docker_yml(service, dst):
-    cmd = (
+
+    vars = (
         f'OPENVPN_USER={os.environ.get("OPENVPN_USER")} '
         f'WIREGUARD_PRIVATE_KEY={os.environ.get("WIREGUARD_PRIVATE_KEY")} '
         f'WIREGUARD_ADDRESSES={os.environ.get("WIREGUARD_ADDRESSES")} '
+    )
+
+    cmps = (
         f'docker compose -f {dst} up -d'
     )
-    print(cmd)
-    subprocess.call(cmd, shell=True)
+
+    if service == 'gluetun':
+        cmds = vars + cmps
+    else:
+        cmds = cmps
+        
+    print(cmds)
+    subprocess.call(cmds, shell=True)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `linuxserver-0.1.0/src/cli/config.py` & `linuxserver-0.1.1/src/cli/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,25 +9,25 @@
         'movies': os.path.expanduser('~/Videos/Movies'),
         'series': os.path.expanduser('~/Videos/Series'),
         'config': os.path.expanduser('~/.linuxserver'),
         'docker': os.path.expanduser('~/.linuxserver/docker'),
     },
     'Linux': {
         'downloads': os.path.expanduser('~/Downloads'),
-        'movies': os.path.expanduser('~/Movies/Movies'),
+        'movies': os.path.expanduser('~/Videos/Movies'),
         'series': os.path.expanduser('~/Videos/Series'),
         'config': os.path.expanduser('~/.linuxserver'),
         'docker': os.path.expanduser('~/.linuxserver/docker'),
     },
     'Darwin': {
         'downloads': os.path.expanduser('~/Downloads'),
         'movies': os.path.expanduser('~/Movies/Movies'),
         'series': os.path.expanduser('~/Movies/Series'),
-        'config': os.path.expanduser('~/linuxserver'),
-        'docker': os.path.expanduser('~/linuxserver/docker'),
+        'config': os.path.expanduser('~/.linuxserver'),
+        'docker': os.path.expanduser('~/.linuxserver/docker'),
     },
 }
 
 services = {
     'deluge': {
         'paths': {
             'downloads': paths[system]['downloads'],
@@ -70,8 +70,14 @@
         'paths': {
             'downloads': paths[system]['downloads'],
             'series': paths[system]['series'],
             'docker': os.path.join(paths[system]['docker'], 'sonarr'),
             'config': os.path.join(paths[system]['config'], 'sonarr'),
         },
     },
+    'heimdall': {
+        'paths': {
+            'docker': os.path.join(paths[system]['docker'], 'heimdall'),
+            'config': os.path.join(paths[system]['config'], 'heimdall'),
+        },
+    },
 }
```

### Comparing `linuxserver-0.1.0/src/cli/docker/gluetun-compose.yml` & `linuxserver-0.1.1/src/cli/docker/gluetun-compose.yml`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,32 @@
     container_name: gluetun
     # line above must be uncommented to allow external containers to connect. See https://github.com/qdm12/gluetun/wiki/Connect-a-container-to-gluetun#external-container-to-gluetun
     cap_add:
       - NET_ADMIN
     devices:
       - /dev/net/tun:/dev/net/tun
     ports:
-      - 8888:8888/tcp # HTTP proxy
-      - 8388:8388/tcp # Shadowsocks
-      - 8388:8388/udp # Shadowsocks
-      - 8112:8112 # Deluge
-      - 6881:6881 # Deluge
-      - 6881:6881/udp # Deluge
-      - 9117:9117 # Jackett
-      - 7878:7878 # Radarr
-      - 8989:8989
+      - 8888:8888/tcp   # HTTP proxy
+      - 8388:8388/tcp   # Shadowsocks
+      - 8388:8388/udp   # Shadowsocks
+      - 8112:8112       # Deluge
+      - 6881:6881       # Deluge
+      - 6881:6881/udp   # Deluge
+      - 9117:9117       # Jackett
+      - 7878:7878       # Radarr
+      - 8989:8989       # Sonarr
+      - 80:80           # Heimdall
+      - 443:443         # Heimdall
     volumes:
       - {{ config }}:/gluetun
     environment:
       # See https://github.com/qdm12/gluetun/wiki
       - VPN_SERVICE_PROVIDER=mullvad
       - VPN_TYPE=wireguard
       # OpenVPN:
       - OPENVPN_USER=${OPENVPN_USER}
       # Wireguard:
       - WIREGUARD_PRIVATE_KEY=${WIREGUARD_PRIVATE_KEY}
       - WIREGUARD_ADDRESSES=${WIREGUARD_ADDRESSES}
       # Timezone for accurate log times
-      - TZ=
+      - TZ=
+    restart: always
```

